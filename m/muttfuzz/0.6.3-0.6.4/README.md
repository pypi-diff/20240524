# Comparing `tmp/muttfuzz-0.6.3-py3-none-any.whl.zip` & `tmp/muttfuzz-0.6.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7754 bytes, number of entries: 8
+Zip file size: 7860 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     3509 b- defN 24-May-24 14:07 muttfuzz/fuzz.py
 -rw-r--r--  2.0 unx     8013 b- defN 24-May-24 14:07 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     3527 b- defN 24-Mar-01 16:10 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-24 14:08 muttfuzz-0.6.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 14:08 muttfuzz-0.6.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-24 14:08 muttfuzz-0.6.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-24 14:08 muttfuzz-0.6.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-24 14:08 muttfuzz-0.6.3.dist-info/RECORD
-8 files, 20422 bytes uncompressed, 6670 bytes compressed:  67.3%
+-rw-r--r--  2.0 unx     3975 b- defN 24-May-24 14:40 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-24 14:40 muttfuzz-0.6.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 14:40 muttfuzz-0.6.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-24 14:40 muttfuzz-0.6.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-24 14:40 muttfuzz-0.6.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-24 14:40 muttfuzz-0.6.4.dist-info/RECORD
+8 files, 20870 bytes uncompressed, 6776 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.6.3.dist-info/METADATA
+Filename: muttfuzz-0.6.4.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.6.3.dist-info/WHEEL
+Filename: muttfuzz-0.6.4.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.6.3.dist-info/entry_points.txt
+Filename: muttfuzz-0.6.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.6.3.dist-info/top_level.txt
+Filename: muttfuzz-0.6.4.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.6.3.dist-info/RECORD
+Filename: muttfuzz-0.6.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/mutate.py

```diff
@@ -1,14 +1,15 @@
 import random
 import subprocess
 
 JUMP_OPCODES = ["je", "jne", "jl", "jle", "jg", "jge"]
 SHORT_JUMPS = list(map(bytes.fromhex, ["74", "75", "7C", "7D", "7E", "7F", "EB"]))
-# no unconditional for near jumps, since changes opcode length, not worth it
+SHORT_NAMES = dict(zip(SHORT_JUMPS, ["je", "jne", "jl", "jge", "jle", "jg", "jmp"]))
 NEAR_JUMPS = list(map(bytes.fromhex, ["0F 84", "0F 85", "0F 8C", "0F 8D", "0F 8E", "0F 8F", "90 E9"]))
+NEAR_NAMES = dict(zip(NEAR_JUMPS, ["je", "jne", "jl", "jge", "jle", "jg", "jmp"]))
 
 # known markers for fuzzer/compiler injected instrumentation/etc.
 INST_SET = ["__afl", "__asan", "__ubsan", "__sanitizer", "__lsan", "__sancov", "AFL_"]
 INST_SET.extend(["DeepState", "deepstate"])
 
 def get_jumps(filename):
     jumps = {}
@@ -17,14 +18,15 @@
                             stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     out, err = proc.communicate()
     output = str(out, encoding="utf-8")
 
     for line in output.split("\n"):
         try:
             if "File Offset" in line and line[-1] == ":":
+                section_name = line.split()[1]
                 section_base = int(line.split()[0], 16)
                 offset_hex = line.split("File Offset:")[1].split(")")[0]
                 section_offset = int(offset_hex, 16) - section_base
                 continue
             found_inst = False
             for i in INST_SET:
                 if i in line:
@@ -34,15 +36,15 @@
                 continue # Don't mutate these things
             fields = line.split("\t")
             if len(fields) > 1:
                 opcode = fields[2].split()[0]
                 if opcode in JUMP_OPCODES:
                     loc_bytes = fields[0].split(":")[0]
                     loc = int(loc_bytes, 16) + section_offset
-                    jumps[loc] = (opcode, bytes.fromhex(fields[1]))
+                    jumps[loc] = (opcode, bytes.fromhex(fields[1]), section_name, line)
         except: # If we can't parse some line in the objdump, just skip it
             pass
 
     return jumps
 
 def different_jump(hexdata):
     if hexdata[0] == 15: # NEAR JUMP BYTE CHECK
@@ -54,15 +56,22 @@
         # Have a high chance of just changing short JE and JNE to a forced JMP, "removing" a branch
         if ((hexdata[0] == SHORT_JUMPS[0][0])  or (hexdata[0] == SHORT_JUMPS[1][0])) and (random.random() <= 0.75):
             return SHORT_JUMPS[-1]
         return random.choice(list(filter(lambda j: j[0] != hexdata[0], SHORT_JUMPS)))
 
 def pick_and_change(jumps):
     loc = random.choice(list(jumps.keys()))
-    return (loc, different_jump(jumps[loc][1]))
+    changed = different_jump(jumps[loc][1])
+    print("MUTATING JUMP IN", jumps[loc][2], "WITH ORIGINAL OPCODE", jumps[loc][0])
+    print("ORIGINAL CODE:", jumps[loc][3])
+    if changed in SHORT_NAMES:
+        print("CHANGING TO", SHORT_NAMES[changed])
+    else
+        print("CHANGING TO", NEAR_NAMES[changed])
+    return (loc, changed)
 
 def get_code(filename):
     with open(filename, "rb") as f:
         return bytearray(f.read())
 
 def mutant_from(code, jumps, order=1):
     new_code = bytearray(code)
```

## Comparing `muttfuzz-0.6.3.dist-info/METADATA` & `muttfuzz-0.6.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.6.3
+Version: 0.6.4
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.6.3.dist-info/RECORD` & `muttfuzz-0.6.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 muttfuzz/fuzz.py,sha256=4-9vfmiK_DgtxYpTZmUT7VJg9rcUbL7mTvZ4Nv2C_9M,3509
 muttfuzz/fuzzutil.py,sha256=Iit46_WsVQVQ0dgjVZ27RcikSrxoVJzz1Ei3I9tJHAk,8013
-muttfuzz/mutate.py,sha256=ah7yxBxOX0nEv5Rlqh3vO1zPr6UV2g65h6r-lymre3I,3527
-muttfuzz-0.6.3.dist-info/METADATA,sha256=3LaWjcqXjBkt_JjP6Gp50mA9Kc8K91ZUt7WqXQiCdyY,4589
-muttfuzz-0.6.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.6.3.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.6.3.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.6.3.dist-info/RECORD,,
+muttfuzz/mutate.py,sha256=ejiXZViYys6M1k_jipje6IJ-dMLW5JNS5FGOHeWqOwo,3975
+muttfuzz-0.6.4.dist-info/METADATA,sha256=49eErJsMLdv3Q9adFNUzIulV1vLJ73TrDG4VYqnQ-Hg,4589
+muttfuzz-0.6.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.6.4.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.6.4.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.6.4.dist-info/RECORD,,
```

