# Comparing `tmp/pbx_code_owners-1.2.0a3-py3-none-any.whl.zip` & `tmp/pbx_code_owners-1.2.0a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3777 bytes, number of entries: 8
--rw-r--r--  2.0 unx       50 b- defN 24-May-24 13:06 code_owners/__init__.py
--rw-r--r--  2.0 unx      549 b- defN 24-May-24 13:06 code_owners/config.py
--rw-r--r--  2.0 unx     3072 b- defN 24-May-24 13:06 code_owners/parser.py
--rw-r--r--  2.0 unx     1070 b- defN 24-May-24 13:06 pbx_code_owners-1.2.0a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 13:06 pbx_code_owners-1.2.0a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-May-24 13:06 pbx_code_owners-1.2.0a3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-May-24 13:06 pbx_code_owners-1.2.0a3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      676 b- defN 24-May-24 13:06 pbx_code_owners-1.2.0a3.dist-info/RECORD
-8 files, 5574 bytes uncompressed, 2581 bytes compressed:  53.7%
+Zip file size: 3791 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       50 b- defN 24-May-24 13:21 code_owners/__init__.py
+-rw-r--r--  2.0 unx      618 b- defN 24-May-24 13:21 code_owners/config.py
+-rw-r--r--  2.0 unx     2931 b- defN 24-May-24 13:21 code_owners/parser.py
+-rw-r--r--  2.0 unx     1070 b- defN 24-May-24 13:22 pbx_code_owners-1.2.0a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 13:22 pbx_code_owners-1.2.0a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-May-24 13:22 pbx_code_owners-1.2.0a6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-24 13:22 pbx_code_owners-1.2.0a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      676 b- defN 24-May-24 13:22 pbx_code_owners-1.2.0a6.dist-info/RECORD
+8 files, 5502 bytes uncompressed, 2595 bytes compressed:  52.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: code_owners/config.py
 Comment: 
 
 Filename: code_owners/parser.py
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a3.dist-info/METADATA
+Filename: pbx_code_owners-1.2.0a6.dist-info/METADATA
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a3.dist-info/WHEEL
+Filename: pbx_code_owners-1.2.0a6.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a3.dist-info/entry_points.txt
+Filename: pbx_code_owners-1.2.0a6.dist-info/entry_points.txt
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a3.dist-info/top_level.txt
+Filename: pbx_code_owners-1.2.0a6.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a3.dist-info/RECORD
+Filename: pbx_code_owners-1.2.0a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## code_owners/config.py

```diff
@@ -6,14 +6,15 @@
 
 
 CI_SERVER_URL = os.environ["CI_SERVER_URL"]
 CI_PROJECT_ID = os.environ["CI_PROJECT_ID"]
 CI_MERGE_REQUEST_IID = os.environ["CI_MERGE_REQUEST_IID"]
 GITLAB_TOKEN = os.environ["CODE_OWNERS_GITLAB_TOKEN"]
 
+CI_COMMIT_BRANCH = os.environ["CI_MERGE_REQUEST_SOURCE_BRANCH_NAME"]
 
 THREADS_PER_PAGE = 100
 
 GITLAB_DISCUSSIONS_URL = (
     f"{CI_SERVER_URL}/api/v4/projects/{CI_PROJECT_ID}"
     f"/merge_requests/{CI_MERGE_REQUEST_IID}/discussions?per_page={THREADS_PER_PAGE}"
 )
```

## code_owners/parser.py

```diff
@@ -8,21 +8,15 @@
 
 def load_codeowners() -> dict:
     with open(config.CODEOWNERS_FILE) as file:
         return yaml.safe_load(file)
 
 
 def get_changed_paths() -> list[str]:
-    current_branch_name = (
-        subprocess.run(  # nosec
-            ["git", "branch", "--show-current"], stdout=subprocess.PIPE
-        )
-        .stdout.decode()
-        .strip()
-    )
+    current_branch_name = config.CI_COMMIT_BRANCH
     print(f"Current branch: {current_branch_name}")
     source_commit = (
         subprocess.run(  # nosec
             ["git", "merge-base", config.DEFAULT_BRANCH, current_branch_name],
             stdout=subprocess.PIPE,
         )
         .stdout.decode()
```

## Comparing `pbx_code_owners-1.2.0a3.dist-info/METADATA` & `pbx_code_owners-1.2.0a6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbx-code-owners
-Version: 1.2.0a3
+Version: 1.2.0a6
 Summary: Code Owners implementation
 Home-page: https://getprintbox.com/
 Author: 
 Author-email: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
```

## Comparing `pbx_code_owners-1.2.0a3.dist-info/RECORD` & `pbx_code_owners-1.2.0a6.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 code_owners/__init__.py,sha256=LJjCu9ALtw6cc5dtCNTr_k5poVo56o8pDWi9Pc6sb_E,50
-code_owners/config.py,sha256=IduMYTSXbIruRagSk35TFB_BuXkMvxuD-OaQjnpd2iU,549
-code_owners/parser.py,sha256=EjuHE52FcOgbGjgngcwbBe6r9_nG_OB-Mrtsc9Iaqy0,3072
-pbx_code_owners-1.2.0a3.dist-info/METADATA,sha256=Hjqj5Gte9qj58YgLeTiggyEPT_XYUwF33TVZ_VAPL0I,1070
-pbx_code_owners-1.2.0a3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pbx_code_owners-1.2.0a3.dist-info/entry_points.txt,sha256=f95eIPd8GX6RCorAFvYPHsC9PsAnWwjqTuAT5DA5y3Y,53
-pbx_code_owners-1.2.0a3.dist-info/top_level.txt,sha256=sL_gdls-fhXq9nUJZAzuPTtGYSYn-SF_D_t9hwGqArA,12
-pbx_code_owners-1.2.0a3.dist-info/RECORD,,
+code_owners/config.py,sha256=OvmnTO-zZqP-njl6qbJlTG9NdCZmfmpeeW2ccnmED6U,618
+code_owners/parser.py,sha256=OuoxuSNRPfSotpkiO9JsfOXQLrzoNO1fAXESxNadI5E,2931
+pbx_code_owners-1.2.0a6.dist-info/METADATA,sha256=SRQvQhG7mooqDmgDveVLz9cFWfs7be2U1L9JRNjO4OU,1070
+pbx_code_owners-1.2.0a6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pbx_code_owners-1.2.0a6.dist-info/entry_points.txt,sha256=f95eIPd8GX6RCorAFvYPHsC9PsAnWwjqTuAT5DA5y3Y,53
+pbx_code_owners-1.2.0a6.dist-info/top_level.txt,sha256=sL_gdls-fhXq9nUJZAzuPTtGYSYn-SF_D_t9hwGqArA,12
+pbx_code_owners-1.2.0a6.dist-info/RECORD,,
```

