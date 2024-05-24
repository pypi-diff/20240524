# Comparing `tmp/pbx_code_owners-1.2.0a8-py3-none-any.whl.zip` & `tmp/pbx_code_owners-1.2.0a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3798 bytes, number of entries: 8
--rw-r--r--  2.0 unx       50 b- defN 24-May-24 13:41 code_owners/__init__.py
--rw-r--r--  2.0 unx      618 b- defN 24-May-24 13:41 code_owners/config.py
--rw-r--r--  2.0 unx     2925 b- defN 24-May-24 13:41 code_owners/parser.py
--rw-r--r--  2.0 unx     1070 b- defN 24-May-24 13:42 pbx_code_owners-1.2.0a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 13:42 pbx_code_owners-1.2.0a8.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-May-24 13:42 pbx_code_owners-1.2.0a8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-May-24 13:42 pbx_code_owners-1.2.0a8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      676 b- defN 24-May-24 13:42 pbx_code_owners-1.2.0a8.dist-info/RECORD
-8 files, 5496 bytes uncompressed, 2602 bytes compressed:  52.7%
+Zip file size: 3803 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       50 b- defN 24-May-24 13:48 code_owners/__init__.py
+-rw-r--r--  2.0 unx      618 b- defN 24-May-24 13:48 code_owners/config.py
+-rw-r--r--  2.0 unx     2912 b- defN 24-May-24 13:48 code_owners/parser.py
+-rw-r--r--  2.0 unx     1070 b- defN 24-May-24 13:49 pbx_code_owners-1.2.0a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 13:49 pbx_code_owners-1.2.0a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-May-24 13:49 pbx_code_owners-1.2.0a9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-24 13:49 pbx_code_owners-1.2.0a9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      676 b- defN 24-May-24 13:49 pbx_code_owners-1.2.0a9.dist-info/RECORD
+8 files, 5483 bytes uncompressed, 2607 bytes compressed:  52.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: code_owners/config.py
 Comment: 
 
 Filename: code_owners/parser.py
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a8.dist-info/METADATA
+Filename: pbx_code_owners-1.2.0a9.dist-info/METADATA
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a8.dist-info/WHEEL
+Filename: pbx_code_owners-1.2.0a9.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a8.dist-info/entry_points.txt
+Filename: pbx_code_owners-1.2.0a9.dist-info/entry_points.txt
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a8.dist-info/top_level.txt
+Filename: pbx_code_owners-1.2.0a9.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a8.dist-info/RECORD
+Filename: pbx_code_owners-1.2.0a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## code_owners/parser.py

```diff
@@ -13,15 +13,15 @@
 
 def get_changed_paths() -> list[str]:
     current_branch_name = config.CI_COMMIT_BRANCH
     print(f"Current branch: {current_branch_name}")
     subprocess.run(["git", "fetch", "origin", "master:master"])  # nosec
     source_commit = (
         subprocess.run(  # nosec
-            ["git", "merge-base", config.DEFAULT_BRANCH, current_branch_name],
+            ["git", "merge-base", config.DEFAULT_BRANCH, "HEAD"],
             stdout=subprocess.PIPE,
         )
         .stdout.decode()
         .strip()
     )
     print(f"Source commit: {source_commit}")
     git_diff = subprocess.run(  # nosec
```

## Comparing `pbx_code_owners-1.2.0a8.dist-info/METADATA` & `pbx_code_owners-1.2.0a9.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbx-code-owners
-Version: 1.2.0a8
+Version: 1.2.0a9
 Summary: Code Owners implementation
 Home-page: https://getprintbox.com/
 Author: 
 Author-email: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
```

## Comparing `pbx_code_owners-1.2.0a8.dist-info/RECORD` & `pbx_code_owners-1.2.0a9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 code_owners/__init__.py,sha256=LJjCu9ALtw6cc5dtCNTr_k5poVo56o8pDWi9Pc6sb_E,50
 code_owners/config.py,sha256=OvmnTO-zZqP-njl6qbJlTG9NdCZmfmpeeW2ccnmED6U,618
-code_owners/parser.py,sha256=56BPdwBQ-t7i_MbOfDsC7F2MdZMEuWEND1ntlIavbR4,2925
-pbx_code_owners-1.2.0a8.dist-info/METADATA,sha256=TSz8ZBsAGgOOXm1GzunXtlXOCd7sxFTNEleCgQ-2EQQ,1070
-pbx_code_owners-1.2.0a8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pbx_code_owners-1.2.0a8.dist-info/entry_points.txt,sha256=f95eIPd8GX6RCorAFvYPHsC9PsAnWwjqTuAT5DA5y3Y,53
-pbx_code_owners-1.2.0a8.dist-info/top_level.txt,sha256=sL_gdls-fhXq9nUJZAzuPTtGYSYn-SF_D_t9hwGqArA,12
-pbx_code_owners-1.2.0a8.dist-info/RECORD,,
+code_owners/parser.py,sha256=PNULs_UqHIP9MjGr70OmxKy8DKvVICbi1sPR4MZT09U,2912
+pbx_code_owners-1.2.0a9.dist-info/METADATA,sha256=p1q_MuBw3Vvd-cWTe7Mc2FE0kjcufubzOJ1tD8Cy_1c,1070
+pbx_code_owners-1.2.0a9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pbx_code_owners-1.2.0a9.dist-info/entry_points.txt,sha256=f95eIPd8GX6RCorAFvYPHsC9PsAnWwjqTuAT5DA5y3Y,53
+pbx_code_owners-1.2.0a9.dist-info/top_level.txt,sha256=sL_gdls-fhXq9nUJZAzuPTtGYSYn-SF_D_t9hwGqArA,12
+pbx_code_owners-1.2.0a9.dist-info/RECORD,,
```

