# Comparing `tmp/pbx_code_owners-1.2.0a6-py3-none-any.whl.zip` & `tmp/pbx_code_owners-1.2.0a7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3791 bytes, number of entries: 8
--rw-r--r--  2.0 unx       50 b- defN 24-May-24 13:21 code_owners/__init__.py
--rw-r--r--  2.0 unx      618 b- defN 24-May-24 13:21 code_owners/config.py
--rw-r--r--  2.0 unx     2931 b- defN 24-May-24 13:21 code_owners/parser.py
--rw-r--r--  2.0 unx     1070 b- defN 24-May-24 13:22 pbx_code_owners-1.2.0a6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 13:22 pbx_code_owners-1.2.0a6.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-May-24 13:22 pbx_code_owners-1.2.0a6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-May-24 13:22 pbx_code_owners-1.2.0a6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      676 b- defN 24-May-24 13:22 pbx_code_owners-1.2.0a6.dist-info/RECORD
-8 files, 5502 bytes uncompressed, 2595 bytes compressed:  52.8%
+Zip file size: 3797 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       50 b- defN 24-May-24 13:29 code_owners/__init__.py
+-rw-r--r--  2.0 unx      618 b- defN 24-May-24 13:29 code_owners/config.py
+-rw-r--r--  2.0 unx     2925 b- defN 24-May-24 13:29 code_owners/parser.py
+-rw-r--r--  2.0 unx     1070 b- defN 24-May-24 13:29 pbx_code_owners-1.2.0a7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 13:29 pbx_code_owners-1.2.0a7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-May-24 13:29 pbx_code_owners-1.2.0a7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-24 13:29 pbx_code_owners-1.2.0a7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      676 b- defN 24-May-24 13:29 pbx_code_owners-1.2.0a7.dist-info/RECORD
+8 files, 5496 bytes uncompressed, 2601 bytes compressed:  52.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: code_owners/config.py
 Comment: 
 
 Filename: code_owners/parser.py
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a6.dist-info/METADATA
+Filename: pbx_code_owners-1.2.0a7.dist-info/METADATA
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a6.dist-info/WHEEL
+Filename: pbx_code_owners-1.2.0a7.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a6.dist-info/entry_points.txt
+Filename: pbx_code_owners-1.2.0a7.dist-info/entry_points.txt
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a6.dist-info/top_level.txt
+Filename: pbx_code_owners-1.2.0a7.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a6.dist-info/RECORD
+Filename: pbx_code_owners-1.2.0a7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## code_owners/parser.py

```diff
@@ -19,15 +19,15 @@
             ["git", "merge-base", config.DEFAULT_BRANCH, current_branch_name],
             stdout=subprocess.PIPE,
         )
         .stdout.decode()
         .strip()
     )
     print(f"Source commit: {source_commit}")
-    subprocess.run(["git", "fetch", "origin", config.DEFAULT_BRANCH])  # nosec
+    subprocess.run(["git", "fetch", "origin", "master:master"])  # nosec
     git_diff = subprocess.run(  # nosec
         ["git", "diff", "--name-only", source_commit], stdout=subprocess.PIPE
     )
     return git_diff.stdout.decode().splitlines()
 
 
 def match_any_path(
```

## Comparing `pbx_code_owners-1.2.0a6.dist-info/METADATA` & `pbx_code_owners-1.2.0a7.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbx-code-owners
-Version: 1.2.0a6
+Version: 1.2.0a7
 Summary: Code Owners implementation
 Home-page: https://getprintbox.com/
 Author: 
 Author-email: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
```

## Comparing `pbx_code_owners-1.2.0a6.dist-info/RECORD` & `pbx_code_owners-1.2.0a7.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 code_owners/__init__.py,sha256=LJjCu9ALtw6cc5dtCNTr_k5poVo56o8pDWi9Pc6sb_E,50
 code_owners/config.py,sha256=OvmnTO-zZqP-njl6qbJlTG9NdCZmfmpeeW2ccnmED6U,618
-code_owners/parser.py,sha256=OuoxuSNRPfSotpkiO9JsfOXQLrzoNO1fAXESxNadI5E,2931
-pbx_code_owners-1.2.0a6.dist-info/METADATA,sha256=SRQvQhG7mooqDmgDveVLz9cFWfs7be2U1L9JRNjO4OU,1070
-pbx_code_owners-1.2.0a6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pbx_code_owners-1.2.0a6.dist-info/entry_points.txt,sha256=f95eIPd8GX6RCorAFvYPHsC9PsAnWwjqTuAT5DA5y3Y,53
-pbx_code_owners-1.2.0a6.dist-info/top_level.txt,sha256=sL_gdls-fhXq9nUJZAzuPTtGYSYn-SF_D_t9hwGqArA,12
-pbx_code_owners-1.2.0a6.dist-info/RECORD,,
+code_owners/parser.py,sha256=tnh124DG5eXkTwzgTFMDoZi3l48yeERzUNlk331yGL0,2925
+pbx_code_owners-1.2.0a7.dist-info/METADATA,sha256=EeLGh1k6fE5cvHuCkri4GXysaT1aVeffQ_AoQyK-ZY4,1070
+pbx_code_owners-1.2.0a7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pbx_code_owners-1.2.0a7.dist-info/entry_points.txt,sha256=f95eIPd8GX6RCorAFvYPHsC9PsAnWwjqTuAT5DA5y3Y,53
+pbx_code_owners-1.2.0a7.dist-info/top_level.txt,sha256=sL_gdls-fhXq9nUJZAzuPTtGYSYn-SF_D_t9hwGqArA,12
+pbx_code_owners-1.2.0a7.dist-info/RECORD,,
```

