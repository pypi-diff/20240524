# Comparing `tmp/muttfuzz-0.6.5-py3-none-any.whl.zip` & `tmp/muttfuzz-0.6.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7862 bytes, number of entries: 8
--rw-r--r--  2.0 unx     3509 b- defN 24-May-24 14:07 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx     8013 b- defN 24-May-24 14:07 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     3976 b- defN 24-May-24 14:42 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-24 14:42 muttfuzz-0.6.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 14:42 muttfuzz-0.6.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-24 14:42 muttfuzz-0.6.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-24 14:42 muttfuzz-0.6.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-24 14:42 muttfuzz-0.6.5.dist-info/RECORD
-8 files, 20871 bytes uncompressed, 6778 bytes compressed:  67.5%
+Zip file size: 8116 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     3761 b- defN 24-May-24 15:08 muttfuzz/fuzz.py
+-rw-r--r--  2.0 unx     8226 b- defN 24-May-24 15:08 muttfuzz/fuzzutil.py
+-rw-r--r--  2.0 unx     4296 b- defN 24-May-24 15:08 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-24 15:08 muttfuzz-0.6.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 15:08 muttfuzz-0.6.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-24 15:08 muttfuzz-0.6.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-24 15:08 muttfuzz-0.6.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-24 15:08 muttfuzz-0.6.6.dist-info/RECORD
+8 files, 21656 bytes uncompressed, 7032 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.6.5.dist-info/METADATA
+Filename: muttfuzz-0.6.6.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.6.5.dist-info/WHEEL
+Filename: muttfuzz-0.6.6.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.6.5.dist-info/entry_points.txt
+Filename: muttfuzz-0.6.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.6.5.dist-info/top_level.txt
+Filename: muttfuzz-0.6.6.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.6.5.dist-info/RECORD
+Filename: muttfuzz-0.6.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzz.py

```diff
@@ -13,14 +13,16 @@
                         help='executable to be fuzzer/mutated')
     parser.add_argument('--budget', type=int, default=3600,
                         help='total fuzzing budget in seconds (default 3600)')
     parser.add_argument('--time_per_mutant', type=int, default=300,
                         help='max time to fuzz each mutant in seconds (default 300)')
     parser.add_argument('--fraction_mutant', type=float, default=0.5,
                         help='portion of budget to devote to mutants (default 0.5)')
+    parser.add_argument('--avoid_mutating', type=str, default="",
+                        help='string with comma delimited list of sections not to mutate inside')
     parser.add_argument('--prune_mutant_cmd', type=str, default="",
                         help='command to check mutants for validity/interest')
     parser.add_argument('--prune_mutant_timeout', type=float, default=2.0,
                         help='timeout for mutant check')
     parser.add_argument('--initial_fuzz_cmd', type=str, default="",
                         help='command for initial fuzzing before mutants')
     parser.add_argument('--initial_budget', type=int, default=60,
@@ -56,14 +58,15 @@
     config = make_config(parsed_args)
     try:
         fuzzutil.fuzz_with_mutants(config.fuzzer_cmd,
                                    config.executable,
                                    config.budget,
                                    config.time_per_mutant,
                                    config.fraction_mutant,
+                                   config.avoid_mutating.replace(", ", ",").split(",").
                                    config.prune_mutant_cmd,
                                    config.prune_mutant_timeout,
                                    config.initial_fuzz_cmd,
                                    config.initial_budget,
                                    config.post_initial_cmd,
                                    config.post_mutant_cmd,
                                    config.status_cmd,
```

## muttfuzz/fuzzutil.py

```diff
@@ -54,24 +54,25 @@
     finally:
         if P.poll() is None:
             os.killpg(os.getpgid(P.pid), signal.SIGTERM)
     return P.returncode
 
 
 def fuzz_with_mutants(fuzzer_cmd, executable, budget, time_per_mutant, fraction_mutant,
+                      avoid_mutating=[],
                       prune_mutant_cmd="",
                       prune_mutant_timeout=1,
                       initial_fuzz_cmd="",
                       initial_budget=0,
                       post_initial_cmd="",
                       post_mutant_cmd="",
                       status_cmd="",
                       order=1):
     executable_code = mutate.get_code(executable)
-    executable_jumps = mutate.get_jumps(executable)
+    executable_jumps = mutate.get_jumps(executable, avoid_mutating)
     start_fuzz = time.time()
     mutant_no = 1
     try:
         if initial_fuzz_cmd != "":
             print("=" * 10,
                   datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'),
                   "=" * 10)
@@ -120,15 +121,16 @@
         if status_cmd != "":
             print("FINAL STATUS:")
             subprocess.call(status_cmd, shell=True)
     finally:
         # always restore the original binary!
         restore_executable(executable, executable_code)
 
-
+# Currently this is not used, and is not updated to match all changes to the API!
+# It should work, but it does not support everything the command line does
 def fuzz_with_mutants_via_function(fuzzer_fn, executable, budget,
                                    time_per_mutant, fraction_mutant,
                                    initial_fn=None, initial_budget=0,
                                    post_initial_fn=None,
                                    post_mutant_fn=None,
                                    status_fn=None, order=1):
     executable_code = mutate.get_code(executable)
```

## muttfuzz/mutate.py

```diff
@@ -7,30 +7,38 @@
 NEAR_JUMPS = list(map(bytes.fromhex, ["0F 84", "0F 85", "0F 8C", "0F 8D", "0F 8E", "0F 8F", "90 E9"]))
 NEAR_NAMES = dict(zip(NEAR_JUMPS, ["je", "jne", "jl", "jge", "jle", "jg", "jmp"]))
 
 # known markers for fuzzer/compiler injected instrumentation/etc.
 INST_SET = ["__afl", "__asan", "__ubsan", "__sanitizer", "__lsan", "__sancov", "AFL_"]
 INST_SET.extend(["DeepState", "deepstate"])
 
-def get_jumps(filename):
+def get_jumps(filename, avoid_mutating=[]):
     jumps = {}
 
     proc = subprocess.Popen(["objdump", "-d", "--file-offsets", filename],
                             stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     out, err = proc.communicate()
     output = str(out, encoding="utf-8")
 
+    avoid = False
+
     for line in output.split("\n"):
         try:
             if "File Offset" in line and line[-1] == ":":
+                avoid = False
                 section_name = line.split()[1]
+                for s in avoid_mutating:
+                    if s in section_name:
+                        avoid = True
                 section_base = int(line.split()[0], 16)
                 offset_hex = line.split("File Offset:")[1].split(")")[0]
                 section_offset = int(offset_hex, 16) - section_base
                 continue
+            if avoid:
+                continue
             found_inst = False
             for i in INST_SET:
                 if i in line:
                     found_inst = True
                     break
             if found_inst:
                 continue # Don't mutate these things
@@ -77,17 +85,17 @@
     new_code = bytearray(code)
     for i in range(order): # allows higher-order mutants, though can undo mutations
         (loc, new_data) = pick_and_change(jumps)
         for offset in range(0, len(new_data)):
             new_code[loc + offset] = new_data[offset]
     return new_code
 
-def mutant(filename, order=1):
-    return mutant_from(get_code(filename), get_jumps(filename), order=order)
+def mutant(filename, order=1, avoid_mutating=[]):
+    return mutant_from(get_code(filename), get_jumps(filename, avoid_mutating), order=order)
 
 def mutate_from(code, jumps, new_filename, order=1):
     with open(new_filename, 'wb') as f:
         f.write(mutant_from(code, jumps, order=order))
 
-def mutate(filename, new_filename, order=1):
+def mutate(filename, new_filename, order=1, avoid_mutating=[]):
     with open(new_filename, "wb") as f:
-        f.write(mutant(filename, order=order))
+        f.write(mutant(filename, order=order, avoid_mutating=avoid_mutating))
```

## Comparing `muttfuzz-0.6.5.dist-info/METADATA` & `muttfuzz-0.6.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.6.5
+Version: 0.6.6
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

