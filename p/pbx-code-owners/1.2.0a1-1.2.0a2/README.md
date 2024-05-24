# Comparing `tmp/pbx_code_owners-1.2.0a1-py3-none-any.whl.zip` & `tmp/pbx_code_owners-1.2.0a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3749 bytes, number of entries: 8
--rw-r--r--  2.0 unx       50 b- defN 24-May-24 12:23 code_owners/__init__.py
--rw-r--r--  2.0 unx      549 b- defN 24-May-24 12:23 code_owners/config.py
--rw-r--r--  2.0 unx     2940 b- defN 24-May-24 12:23 code_owners/parser.py
--rw-r--r--  2.0 unx     1070 b- defN 24-May-24 12:23 pbx_code_owners-1.2.0a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 12:23 pbx_code_owners-1.2.0a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-May-24 12:23 pbx_code_owners-1.2.0a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-May-24 12:23 pbx_code_owners-1.2.0a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      676 b- defN 24-May-24 12:23 pbx_code_owners-1.2.0a1.dist-info/RECORD
-8 files, 5442 bytes uncompressed, 2553 bytes compressed:  53.1%
+Zip file size: 3790 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       50 b- defN 24-May-24 12:58 code_owners/__init__.py
+-rw-r--r--  2.0 unx      549 b- defN 24-May-24 12:58 code_owners/config.py
+-rw-r--r--  2.0 unx     3081 b- defN 24-May-24 12:58 code_owners/parser.py
+-rw-r--r--  2.0 unx     1070 b- defN 24-May-24 12:58 pbx_code_owners-1.2.0a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 12:58 pbx_code_owners-1.2.0a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-May-24 12:58 pbx_code_owners-1.2.0a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-24 12:58 pbx_code_owners-1.2.0a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      676 b- defN 24-May-24 12:58 pbx_code_owners-1.2.0a2.dist-info/RECORD
+8 files, 5583 bytes uncompressed, 2594 bytes compressed:  53.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: code_owners/config.py
 Comment: 
 
 Filename: code_owners/parser.py
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a1.dist-info/METADATA
+Filename: pbx_code_owners-1.2.0a2.dist-info/METADATA
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a1.dist-info/WHEEL
+Filename: pbx_code_owners-1.2.0a2.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a1.dist-info/entry_points.txt
+Filename: pbx_code_owners-1.2.0a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a1.dist-info/top_level.txt
+Filename: pbx_code_owners-1.2.0a2.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_code_owners-1.2.0a1.dist-info/RECORD
+Filename: pbx_code_owners-1.2.0a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## code_owners/parser.py

```diff
@@ -15,22 +15,24 @@
     current_branch_name = (
         subprocess.run(  # nosec
             ["git", "rev-parse", "--abbrev-ref", "HEAD"], stdout=subprocess.PIPE
         )
         .stdout.decode()
         .strip()
     )
+    print(f"Current branch: {current_branch_name}")
     source_commit = (
         subprocess.run(  # nosec
             ["git", "merge-base", config.DEFAULT_BRANCH, current_branch_name],
             stdout=subprocess.PIPE,
         )
         .stdout.decode()
         .strip()
     )
+    print(f"Source commit: {source_commit}")
     subprocess.run(["git", "fetch", "origin", config.DEFAULT_BRANCH])  # nosec
     git_diff = subprocess.run(  # nosec
         ["git", "diff", "--name-only", source_commit], stdout=subprocess.PIPE
     )
     return git_diff.stdout.decode().splitlines()
 
 
@@ -84,23 +86,23 @@
     headers = {"PRIVATE-TOKEN": config.GITLAB_TOKEN}
     resp = requests.post(url, headers=headers, json={"body": content}, timeout=(3, 30))
     resp.raise_for_status()
 
 
 def main() -> None:
     codeowners = load_codeowners()
+    print(f"Loaded config: {codeowners}")
     changed_paths = get_changed_paths()
+    print(f"Changed paths: {changed_paths}")
     if not changed_paths:
         print("No changes, checking codeowners stopped")
         return
 
-    print(f"Changed paths: {changed_paths}")
-
     for section in codeowners["sections"]:
-        print(f"Matching section {section}")
         if match_any_path(changed_paths, section["paths"], section.get("exclude", [])):
+            print(f"Matched section {section}")
             notify_owners(section["owners"], section["name"])
     return
 
 
 if __name__ == "__main__":
     main()
```

## Comparing `pbx_code_owners-1.2.0a1.dist-info/METADATA` & `pbx_code_owners-1.2.0a2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbx-code-owners
-Version: 1.2.0a1
+Version: 1.2.0a2
 Summary: Code Owners implementation
 Home-page: https://getprintbox.com/
 Author: 
 Author-email: 
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
```

