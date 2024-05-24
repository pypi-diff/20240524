# Comparing `tmp/pbx_code_owners-1.2.0a0-py3-none-any.whl.zip` & `tmp/pbx_code_owners-1.2.0a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3722 bytes, number of entries: 8
--rw-r--r--  2.0 unx       50 b- defN 24-May-24 11:31 code_owners/__init__.py
--rw-r--r--  2.0 unx      549 b- defN 24-May-24 11:31 code_owners/config.py
--rw-r--r--  2.0 unx     2849 b- defN 24-May-24 11:31 code_owners/parser.py
--rw-r--r--  2.0 unx     1070 b- defN 24-May-24 11:31 pbx_code_owners-1.2.0a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 11:31 pbx_code_owners-1.2.0a0.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-May-24 11:31 pbx_code_owners-1.2.0a0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-May-24 11:31 pbx_code_owners-1.2.0a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      676 b- defN 24-May-24 11:31 pbx_code_owners-1.2.0a0.dist-info/RECORD
-8 files, 5351 bytes uncompressed, 2526 bytes compressed:  52.8%
+Zip file size: 3749 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       50 b- defN 24-May-24 12:23 code_owners/__init__.py
+-rw-r--r--  2.0 unx      549 b- defN 24-May-24 12:23 code_owners/config.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-May-24 12:23 code_owners/parser.py
+-rw-r--r--  2.0 unx     1070 b- defN 24-May-24 12:23 pbx_code_owners-1.2.0a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 12:23 pbx_code_owners-1.2.0a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-May-24 12:23 pbx_code_owners-1.2.0a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-24 12:23 pbx_code_owners-1.2.0a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      676 b- defN 24-May-24 12:23 pbx_code_owners-1.2.0a1.dist-info/RECORD
+8 files, 5442 bytes uncompressed, 2553 bytes compressed:  53.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: code_owners/config.py
 Comment: 
 
 Filename: code_owners/parser.py
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a0.dist-info/METADATA
+Filename: pbx_code_owners-1.2.0a1.dist-info/METADATA
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a0.dist-info/WHEEL
+Filename: pbx_code_owners-1.2.0a1.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a0.dist-info/entry_points.txt
+Filename: pbx_code_owners-1.2.0a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a0.dist-info/top_level.txt
+Filename: pbx_code_owners-1.2.0a1.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a0.dist-info/RECORD
+Filename: pbx_code_owners-1.2.0a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## code_owners/parser.py

```diff
@@ -89,15 +89,18 @@
 def main() -> None:
     codeowners = load_codeowners()
     changed_paths = get_changed_paths()
     if not changed_paths:
         print("No changes, checking codeowners stopped")
         return
 
+    print(f"Changed paths: {changed_paths}")
+
     for section in codeowners["sections"]:
+        print(f"Matching section {section}")
         if match_any_path(changed_paths, section["paths"], section.get("exclude", [])):
             notify_owners(section["owners"], section["name"])
     return
 
 
 if __name__ == "__main__":
     main()
```

## Comparing `pbx_code_owners-1.2.0a0.dist-info/METADATA` & `pbx_code_owners-1.2.0a1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbx-code-owners
-Version: 1.2.0a0
+Version: 1.2.0a1
 Summary: Code Owners implementation
 Home-page: https://getprintbox.com/
 Author: 
 Author-email: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
```

## Comparing `pbx_code_owners-1.2.0a0.dist-info/RECORD` & `pbx_code_owners-1.2.0a1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 code_owners/__init__.py,sha256=LJjCu9ALtw6cc5dtCNTr_k5poVo56o8pDWi9Pc6sb_E,50
 code_owners/config.py,sha256=IduMYTSXbIruRagSk35TFB_BuXkMvxuD-OaQjnpd2iU,549
-code_owners/parser.py,sha256=FsFjHxM7wGItRSkpHGHymKLnU9W_oWKPoh_j0gq2RHA,2849
-pbx_code_owners-1.2.0a0.dist-info/METADATA,sha256=1qvoaDBj1CI8vgx4YsSkU3tmZhf3OBuCVQEc99-9V2k,1070
-pbx_code_owners-1.2.0a0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pbx_code_owners-1.2.0a0.dist-info/entry_points.txt,sha256=f95eIPd8GX6RCorAFvYPHsC9PsAnWwjqTuAT5DA5y3Y,53
-pbx_code_owners-1.2.0a0.dist-info/top_level.txt,sha256=sL_gdls-fhXq9nUJZAzuPTtGYSYn-SF_D_t9hwGqArA,12
-pbx_code_owners-1.2.0a0.dist-info/RECORD,,
+code_owners/parser.py,sha256=4T-lDJYfoPv-xjcIhVrMBH_eaWMq4wu99exWgZe7Gto,2940
+pbx_code_owners-1.2.0a1.dist-info/METADATA,sha256=Z6UdfCwZPLvCkVhLnw_xdozXwJjANb3b68aF_HxoPRU,1070
+pbx_code_owners-1.2.0a1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pbx_code_owners-1.2.0a1.dist-info/entry_points.txt,sha256=f95eIPd8GX6RCorAFvYPHsC9PsAnWwjqTuAT5DA5y3Y,53
+pbx_code_owners-1.2.0a1.dist-info/top_level.txt,sha256=sL_gdls-fhXq9nUJZAzuPTtGYSYn-SF_D_t9hwGqArA,12
+pbx_code_owners-1.2.0a1.dist-info/RECORD,,
```

