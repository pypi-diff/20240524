# Comparing `tmp/pbx_code_owners-1.2.0a2-py3-none-any.whl.zip` & `tmp/pbx_code_owners-1.2.0a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3790 bytes, number of entries: 8
--rw-r--r--  2.0 unx       50 b- defN 24-May-24 12:58 code_owners/__init__.py
--rw-r--r--  2.0 unx      549 b- defN 24-May-24 12:58 code_owners/config.py
--rw-r--r--  2.0 unx     3081 b- defN 24-May-24 12:58 code_owners/parser.py
--rw-r--r--  2.0 unx     1070 b- defN 24-May-24 12:58 pbx_code_owners-1.2.0a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 12:58 pbx_code_owners-1.2.0a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-May-24 12:58 pbx_code_owners-1.2.0a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-May-24 12:58 pbx_code_owners-1.2.0a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      676 b- defN 24-May-24 12:58 pbx_code_owners-1.2.0a2.dist-info/RECORD
-8 files, 5583 bytes uncompressed, 2594 bytes compressed:  53.5%
+Zip file size: 3777 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       50 b- defN 24-May-24 13:06 code_owners/__init__.py
+-rw-r--r--  2.0 unx      549 b- defN 24-May-24 13:06 code_owners/config.py
+-rw-r--r--  2.0 unx     3072 b- defN 24-May-24 13:06 code_owners/parser.py
+-rw-r--r--  2.0 unx     1070 b- defN 24-May-24 13:06 pbx_code_owners-1.2.0a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 13:06 pbx_code_owners-1.2.0a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-May-24 13:06 pbx_code_owners-1.2.0a3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-24 13:06 pbx_code_owners-1.2.0a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      676 b- defN 24-May-24 13:06 pbx_code_owners-1.2.0a3.dist-info/RECORD
+8 files, 5574 bytes uncompressed, 2581 bytes compressed:  53.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: code_owners/config.py
 Comment: 
 
 Filename: code_owners/parser.py
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a2.dist-info/METADATA
+Filename: pbx_code_owners-1.2.0a3.dist-info/METADATA
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a2.dist-info/WHEEL
+Filename: pbx_code_owners-1.2.0a3.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a2.dist-info/entry_points.txt
+Filename: pbx_code_owners-1.2.0a3.dist-info/entry_points.txt
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a2.dist-info/top_level.txt
+Filename: pbx_code_owners-1.2.0a3.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a2.dist-info/RECORD
+Filename: pbx_code_owners-1.2.0a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## code_owners/parser.py

```diff
@@ -10,15 +10,15 @@
     with open(config.CODEOWNERS_FILE) as file:
         return yaml.safe_load(file)
 
 
 def get_changed_paths() -> list[str]:
     current_branch_name = (
         subprocess.run(  # nosec
-            ["git", "rev-parse", "--abbrev-ref", "HEAD"], stdout=subprocess.PIPE
+            ["git", "branch", "--show-current"], stdout=subprocess.PIPE
         )
         .stdout.decode()
         .strip()
     )
     print(f"Current branch: {current_branch_name}")
     source_commit = (
         subprocess.run(  # nosec
```

## Comparing `pbx_code_owners-1.2.0a2.dist-info/METADATA` & `pbx_code_owners-1.2.0a3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbx-code-owners
-Version: 1.2.0a2
+Version: 1.2.0a3
 Summary: Code Owners implementation
 Home-page: https://getprintbox.com/
 Author: 
 Author-email: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
```

## Comparing `pbx_code_owners-1.2.0a2.dist-info/RECORD` & `pbx_code_owners-1.2.0a3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 code_owners/__init__.py,sha256=LJjCu9ALtw6cc5dtCNTr_k5poVo56o8pDWi9Pc6sb_E,50
 code_owners/config.py,sha256=IduMYTSXbIruRagSk35TFB_BuXkMvxuD-OaQjnpd2iU,549
-code_owners/parser.py,sha256=Ns4WmKfXfkMPv33vECKeZcspsVITBRZ6ChkvWM3oS0Y,3081
-pbx_code_owners-1.2.0a2.dist-info/METADATA,sha256=EYkStyLStOFQS4x_SwGyjWCzZyfKK9yjb0OLVWzGiw0,1070
-pbx_code_owners-1.2.0a2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pbx_code_owners-1.2.0a2.dist-info/entry_points.txt,sha256=f95eIPd8GX6RCorAFvYPHsC9PsAnWwjqTuAT5DA5y3Y,53
-pbx_code_owners-1.2.0a2.dist-info/top_level.txt,sha256=sL_gdls-fhXq9nUJZAzuPTtGYSYn-SF_D_t9hwGqArA,12
-pbx_code_owners-1.2.0a2.dist-info/RECORD,,
+code_owners/parser.py,sha256=EjuHE52FcOgbGjgngcwbBe6r9_nG_OB-Mrtsc9Iaqy0,3072
+pbx_code_owners-1.2.0a3.dist-info/METADATA,sha256=Hjqj5Gte9qj58YgLeTiggyEPT_XYUwF33TVZ_VAPL0I,1070
+pbx_code_owners-1.2.0a3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pbx_code_owners-1.2.0a3.dist-info/entry_points.txt,sha256=f95eIPd8GX6RCorAFvYPHsC9PsAnWwjqTuAT5DA5y3Y,53
+pbx_code_owners-1.2.0a3.dist-info/top_level.txt,sha256=sL_gdls-fhXq9nUJZAzuPTtGYSYn-SF_D_t9hwGqArA,12
+pbx_code_owners-1.2.0a3.dist-info/RECORD,,
```

