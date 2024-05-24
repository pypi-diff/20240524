# Comparing `tmp/muttfuzz-0.6.4-py3-none-any.whl.zip` & `tmp/muttfuzz-0.6.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7860 bytes, number of entries: 8
+Zip file size: 7862 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     3509 b- defN 24-May-24 14:07 muttfuzz/fuzz.py
 -rw-r--r--  2.0 unx     8013 b- defN 24-May-24 14:07 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     3975 b- defN 24-May-24 14:40 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-24 14:40 muttfuzz-0.6.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 14:40 muttfuzz-0.6.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-24 14:40 muttfuzz-0.6.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-24 14:40 muttfuzz-0.6.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-24 14:40 muttfuzz-0.6.4.dist-info/RECORD
-8 files, 20870 bytes uncompressed, 6776 bytes compressed:  67.5%
+-rw-r--r--  2.0 unx     3976 b- defN 24-May-24 14:42 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-24 14:42 muttfuzz-0.6.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 14:42 muttfuzz-0.6.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-24 14:42 muttfuzz-0.6.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-24 14:42 muttfuzz-0.6.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-24 14:42 muttfuzz-0.6.5.dist-info/RECORD
+8 files, 20871 bytes uncompressed, 6778 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.6.4.dist-info/METADATA
+Filename: muttfuzz-0.6.5.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.6.4.dist-info/WHEEL
+Filename: muttfuzz-0.6.5.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.6.4.dist-info/entry_points.txt
+Filename: muttfuzz-0.6.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.6.4.dist-info/top_level.txt
+Filename: muttfuzz-0.6.5.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.6.4.dist-info/RECORD
+Filename: muttfuzz-0.6.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/mutate.py

```diff
@@ -61,15 +61,15 @@
 def pick_and_change(jumps):
     loc = random.choice(list(jumps.keys()))
     changed = different_jump(jumps[loc][1])
     print("MUTATING JUMP IN", jumps[loc][2], "WITH ORIGINAL OPCODE", jumps[loc][0])
     print("ORIGINAL CODE:", jumps[loc][3])
     if changed in SHORT_NAMES:
         print("CHANGING TO", SHORT_NAMES[changed])
-    else
+    else:
         print("CHANGING TO", NEAR_NAMES[changed])
     return (loc, changed)
 
 def get_code(filename):
     with open(filename, "rb") as f:
         return bytearray(f.read())
```

## Comparing `muttfuzz-0.6.4.dist-info/METADATA` & `muttfuzz-0.6.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.6.4
+Version: 0.6.5
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.6.4.dist-info/RECORD` & `muttfuzz-0.6.5.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 muttfuzz/fuzz.py,sha256=4-9vfmiK_DgtxYpTZmUT7VJg9rcUbL7mTvZ4Nv2C_9M,3509
 muttfuzz/fuzzutil.py,sha256=Iit46_WsVQVQ0dgjVZ27RcikSrxoVJzz1Ei3I9tJHAk,8013
-muttfuzz/mutate.py,sha256=ejiXZViYys6M1k_jipje6IJ-dMLW5JNS5FGOHeWqOwo,3975
-muttfuzz-0.6.4.dist-info/METADATA,sha256=49eErJsMLdv3Q9adFNUzIulV1vLJ73TrDG4VYqnQ-Hg,4589
-muttfuzz-0.6.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.6.4.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.6.4.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.6.4.dist-info/RECORD,,
+muttfuzz/mutate.py,sha256=4vrpd1i2plSixSKygMK9tY0w4GramESBa6xPeuOtQSU,3976
+muttfuzz-0.6.5.dist-info/METADATA,sha256=AbdBg7FRhnmCSf3MVGp5EwHnqBQiNV883T7LJr-Tico,4589
+muttfuzz-0.6.5.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.6.5.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.6.5.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.6.5.dist-info/RECORD,,
```

