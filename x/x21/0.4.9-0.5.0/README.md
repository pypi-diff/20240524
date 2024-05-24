# Comparing `tmp/x21-0.4.9-cp39-cp39-win_amd64.whl.zip` & `tmp/x21-0.5.0-pp310-pypy310_pp73-macosx_10_14_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,7 @@
-Zip file size: 76899 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat   160256 b- defN 23-Feb-24 21:43 _x21.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      267 b- defN 23-Feb-24 21:38 x21/__init__.py
--rw-rw-rw-  2.0 fat      637 b- defN 23-Feb-24 21:38 x21/_main.py
--rw-rw-rw-  2.0 fat      124 b- defN 23-Feb-24 21:43 x21-0.4.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Feb-24 21:43 x21-0.4.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Feb-24 21:43 x21-0.4.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      502 b- defN 23-Feb-24 21:43 x21-0.4.9.dist-info/RECORD
-7 files, 161895 bytes uncompressed, 76021 bytes compressed:  53.0%
+Zip file size: 45108 bytes, number of entries: 5
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 09:41 x21-0.5.0.dist-info/
+-rwxr-xr-x  2.0 unx   114984 b- defN 24-May-24 09:41 x21.pypy310-pp73-darwin.so
+-rw-rw-r--  2.0 unx      283 b- defN 24-May-24 09:41 x21-0.5.0.dist-info/RECORD
+-rw-rw-r--  2.0 unx      122 b- defN 24-May-24 09:41 x21-0.5.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      475 b- defN 24-May-24 09:41 x21-0.5.0.dist-info/METADATA
+5 files, 115864 bytes uncompressed, 44456 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -1,22 +1,16 @@
-Filename: _x21.cp39-win_amd64.pyd
+Filename: x21-0.5.0.dist-info/
 Comment: 
 
-Filename: x21/__init__.py
+Filename: x21.pypy310-pp73-darwin.so
 Comment: 
 
-Filename: x21/_main.py
+Filename: x21-0.5.0.dist-info/RECORD
 Comment: 
 
-Filename: x21-0.4.9.dist-info/METADATA
+Filename: x21-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: x21-0.4.9.dist-info/WHEEL
-Comment: 
-
-Filename: x21-0.4.9.dist-info/top_level.txt
-Comment: 
-
-Filename: x21-0.4.9.dist-info/RECORD
+Filename: x21-0.5.0.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

