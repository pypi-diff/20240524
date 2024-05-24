# Comparing `tmp/muttfuzz-0.6.2-py3-none-any.whl.zip` & `tmp/muttfuzz-0.6.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7532 bytes, number of entries: 8
--rw-r--r--  2.0 unx     3106 b- defN 24-Mar-01 15:40 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx     7445 b- defN 24-Mar-01 15:40 muttfuzz/fuzzutil.py
+Zip file size: 7754 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     3509 b- defN 24-May-24 14:07 muttfuzz/fuzz.py
+-rw-r--r--  2.0 unx     8013 b- defN 24-May-24 14:07 muttfuzz/fuzzutil.py
 -rw-r--r--  2.0 unx     3527 b- defN 24-Mar-01 16:10 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-Mar-01 16:10 muttfuzz-0.6.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-01 16:10 muttfuzz-0.6.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-Mar-01 16:10 muttfuzz-0.6.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-Mar-01 16:10 muttfuzz-0.6.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-Mar-01 16:10 muttfuzz-0.6.2.dist-info/RECORD
-8 files, 19451 bytes uncompressed, 6448 bytes compressed:  66.9%
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-24 14:08 muttfuzz-0.6.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 14:08 muttfuzz-0.6.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-24 14:08 muttfuzz-0.6.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-24 14:08 muttfuzz-0.6.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-24 14:08 muttfuzz-0.6.3.dist-info/RECORD
+8 files, 20422 bytes uncompressed, 6670 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.6.2.dist-info/METADATA
+Filename: muttfuzz-0.6.3.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.6.2.dist-info/WHEEL
+Filename: muttfuzz-0.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.6.2.dist-info/entry_points.txt
+Filename: muttfuzz-0.6.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.6.2.dist-info/top_level.txt
+Filename: muttfuzz-0.6.3.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.6.2.dist-info/RECORD
+Filename: muttfuzz-0.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzz.py

```diff
@@ -13,14 +13,18 @@
                         help='executable to be fuzzer/mutated')
     parser.add_argument('--budget', type=int, default=3600,
                         help='total fuzzing budget in seconds (default 3600)')
     parser.add_argument('--time_per_mutant', type=int, default=300,
                         help='max time to fuzz each mutant in seconds (default 300)')
     parser.add_argument('--fraction_mutant', type=float, default=0.5,
                         help='portion of budget to devote to mutants (default 0.5)')
+    parser.add_argument('--prune_mutant_cmd', type=str, default="",
+                        help='command to check mutants for validity/interest')
+    parser.add_argument('--prune_mutant_timeout', type=float, default=2.0,
+                        help='timeout for mutant check')
     parser.add_argument('--initial_fuzz_cmd', type=str, default="",
                         help='command for initial fuzzing before mutants')
     parser.add_argument('--initial_budget', type=int, default=60,
                         help='how long to run initial fuzzing, in seconds (default 60)')
     parser.add_argument('--post_initial_cmd', type=str, default="",
                         help='command to run after initial fuzzing')
     parser.add_argument('--post_mutant_cmd', type=str, default="",
@@ -52,14 +56,16 @@
     config = make_config(parsed_args)
     try:
         fuzzutil.fuzz_with_mutants(config.fuzzer_cmd,
                                    config.executable,
                                    config.budget,
                                    config.time_per_mutant,
                                    config.fraction_mutant,
+                                   config.prune_mutant_cmd,
+                                   config.prune_mutant_timeout,
                                    config.initial_fuzz_cmd,
                                    config.initial_budget,
                                    config.post_initial_cmd,
                                    config.post_mutant_cmd,
                                    config.status_cmd,
                                    config.order)
     except IndexError:
```

## muttfuzz/fuzzutil.py

```diff
@@ -39,33 +39,37 @@
     dnull = open(os.devnull, 'w')
     start_P = time.time()
     try:
         with open("cmd_errors.txt", 'w') as cmd_errors:
             P = subprocess.Popen(cmd, shell=True, preexec_fn=os.setsid,
                                  stdout=dnull, stderr=cmd_errors)
             while (P.poll() is None) and ((time.time() - start_P) < timeout):
-                time.sleep(0.5)
+                time.sleep(min(0.5, timeout / 10.0)) # Allow for small timeouts
             if P.poll() is None:
                 os.killpg(os.getpgid(P.pid), signal.SIGTERM)
         with open("cmd_errors.txt", 'r') as cmd_errors:
             cmd_errors_out = cmd_errors.read()
         if len(cmd_errors_out) > 0:
             print("ERRORS:")
             print(cmd_errors_out)
     finally:
         if P.poll() is None:
             os.killpg(os.getpgid(P.pid), signal.SIGTERM)
+    return P.returncode
 
 
-def fuzz_with_mutants(fuzzer_cmd, executable, budget,
-                      time_per_mutant, fraction_mutant,
-                      initial_fuzz_cmd="", initial_budget=0,
+def fuzz_with_mutants(fuzzer_cmd, executable, budget, time_per_mutant, fraction_mutant,
+                      prune_mutant_cmd="",
+                      prune_mutant_timeout=1,
+                      initial_fuzz_cmd="",
+                      initial_budget=0,
                       post_initial_cmd="",
                       post_mutant_cmd="",
-                      status_cmd="", order=1):
+                      status_cmd="",
+                      order=1):
     executable_code = mutate.get_code(executable)
     executable_jumps = mutate.get_jumps(executable)
     start_fuzz = time.time()
     mutant_no = 1
     try:
         if initial_fuzz_cmd != "":
             print("=" * 10,
@@ -86,23 +90,31 @@
             print(round(time.time() - start_fuzz, 2),
                   "ELAPSED: GENERATING MUTANT #" + str(mutant_no))
             mutant_no += 1
             # make a new mutant of the executable; rename avoids hitting a busy executable
             mutate.mutate_from(executable_code, executable_jumps, "/tmp/new_executable", order=order)
             os.rename("/tmp/new_executable", executable)
             subprocess.check_call(['chmod', '+x', executable])
-            print("FUZZING MUTANT...")
-            start_run = time.time()
-            silent_run_with_timeout(fuzzer_cmd, time_per_mutant)
-            print("FINISHED FUZZING IN", round(time.time() - start_run, 2), "SECONDS")
-            if post_mutant_cmd != "":
-                subprocess.call(post_mutant_cmd, shell=True)
-            if status_cmd != "":
-                print("STATUS:")
-                subprocess.call(status_cmd, shell=True)
+            mutant_ok = True
+            if prune_mutant_cmd != "":
+                print("CHECKING MUTANT...")
+                r = silent_run_with_timeout(prune_mutant_cmd, prune_mutant_timeout)
+                if r != 0:
+                    print("CHECK FAILED WITH RETURN CODE", r)
+                    mutant_ok = False
+            if mutant_ok:
+                print("FUZZING MUTANT...")
+                start_run = time.time()
+                silent_run_with_timeout(fuzzer_cmd, time_per_mutant)
+                print("FINISHED FUZZING IN", round(time.time() - start_run, 2), "SECONDS")
+                if post_mutant_cmd != "":
+                    subprocess.call(post_mutant_cmd, shell=True)
+                if status_cmd != "":
+                    print("STATUS:")
+                    subprocess.call(status_cmd, shell=True)
 
         print(datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'))
         print(round(time.time() - start_fuzz, 2), "ELAPSED: STARTING FINAL FUZZ")
         restore_executable(executable, executable_code)
         silent_run_with_timeout(fuzzer_cmd, budget - (time.time() - start_fuzz))
         print("COMPLETED ALL FUZZING AFTER", round(time.time() - start_fuzz, 2), "SECONDS")
         if status_cmd != "":
```

## Comparing `muttfuzz-0.6.2.dist-info/METADATA` & `muttfuzz-0.6.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.6.2
+Version: 0.6.3
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.6.2.dist-info/RECORD` & `muttfuzz-0.6.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-muttfuzz/fuzz.py,sha256=xs1PmEkIYTagE2gLVvCV2yVl5sis0LnEmj853hqKpk8,3106
-muttfuzz/fuzzutil.py,sha256=DuPtSdLALzpoLR3ynwkiqDwbI_Q-ASQmPD_Gq8mSAT0,7445
+muttfuzz/fuzz.py,sha256=4-9vfmiK_DgtxYpTZmUT7VJg9rcUbL7mTvZ4Nv2C_9M,3509
+muttfuzz/fuzzutil.py,sha256=Iit46_WsVQVQ0dgjVZ27RcikSrxoVJzz1Ei3I9tJHAk,8013
 muttfuzz/mutate.py,sha256=ah7yxBxOX0nEv5Rlqh3vO1zPr6UV2g65h6r-lymre3I,3527
-muttfuzz-0.6.2.dist-info/METADATA,sha256=iWZnUK0XHs08V4-mObBQYuPhpygvnRJYXCekuuVislE,4589
-muttfuzz-0.6.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.6.2.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.6.2.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.6.2.dist-info/RECORD,,
+muttfuzz-0.6.3.dist-info/METADATA,sha256=3LaWjcqXjBkt_JjP6Gp50mA9Kc8K91ZUt7WqXQiCdyY,4589
+muttfuzz-0.6.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.6.3.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.6.3.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.6.3.dist-info/RECORD,,
```

