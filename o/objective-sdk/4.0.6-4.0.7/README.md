# Comparing `tmp/objective_sdk-4.0.6.tar.gz` & `tmp/objective_sdk-4.0.7.tar.gz`

## Comparing `objective_sdk-4.0.6.tar` & `objective_sdk-4.0.7.tar`

### file list

```diff
@@ -1,13 +1,11 @@
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 objective_sdk-4.0.6/index.html
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 objective_sdk-4.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 objective_sdk-4.0.6/src/objective/__init__.py
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 objective_sdk-4.0.6/src/objective/a.ipynb
--rw-r--r--   0        0        0    20445 2020-02-02 00:00:00.000000 objective_sdk-4.0.6/src/objective/objective.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 objective_sdk-4.0.6/tests/__init__.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 objective_sdk-4.0.6/tests/sdk_integration_test.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 objective_sdk-4.0.6/tests/test_objective.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 objective_sdk-4.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 objective_sdk-4.0.6/LICENSE
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 objective_sdk-4.0.6/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 objective_sdk-4.0.6/pyproject.toml
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 objective_sdk-4.0.6/PKG-INFO
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 objective_sdk-4.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 objective_sdk-4.0.7/src/objective/__init__.py
+-rw-r--r--   0        0        0    21136 2020-02-02 00:00:00.000000 objective_sdk-4.0.7/src/objective/objective.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 objective_sdk-4.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 objective_sdk-4.0.7/tests/sdk_integration_test.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 objective_sdk-4.0.7/tests/test_objective.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 objective_sdk-4.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 objective_sdk-4.0.7/LICENSE
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 objective_sdk-4.0.7/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 objective_sdk-4.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 objective_sdk-4.0.7/PKG-INFO
```

### Comparing `objective_sdk-4.0.6/.github/workflows/python-publish.yml` & `objective_sdk-4.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `objective_sdk-4.0.6/src/objective/objective.py` & `objective_sdk-4.0.7/src/objective/objective.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,29 @@
                 # response can be None for timeouts or connect errors.
                 if e.response is not None:
                     if (
                         e.response.status_code >= 400
                         and e.response.status_code <= 499
                         and e.response.status_code != 429
                     ):
-                        raise (e)
+                        if (
+                            e.response.status_code == 422
+                            and "errors" in e.response.json()
+                        ):
+                            errors_str = ", ".join(
+                                [
+                                    f'Error code {err.get("code")}: {err.get("message")}'
+                                    for err in e.response.json().get("errors", [])
+                                ]
+                            )
+                            raise Error(
+                                f"Failed to create index with the following errors: {errors_str}",
+                            )
+                        else:
+                            raise (e)
 
                 if attempt < MAX_RETRIES - 1:  # i.e. if it's not the last attempt
                     sleep_time = BACKOFF_FACTOR * (2**attempt)
                     time.sleep(sleep_time)
                     continue
                 else:
                     raise (e)
@@ -452,16 +466,16 @@
         # return self.client.request(
         #     "PUT", f"indexes/{self.id}", data=new_fields
         # )
 
     def delete(self):
         return self.client.request("DELETE", f"indexes/{self.id}")
 
-    def autofinetune(self, feedback: List[Dict[str, Any]]) -> "Index":
-        print("Creating a autofinetuned index...", file=sys.stderr)
+    def finetune(self, feedback: List[Dict[str, Any]]) -> "Index":
+        print("Creating a finetuned index...", file=sys.stderr)
         finetuned_create_index = self.client.request(
             "POST",
             "indexes",
             data={
                 "configuration": {
                     "index_type": {
                         **(
@@ -476,15 +490,15 @@
                 }
             },
         )
         if not finetuned_create_index:
             raise ValueError("Failed to create finetuned index!")
         else:
             print(
-                f"Autofinetuned index {finetuned_create_index['id']} successfully created.",
+                f"Finetuned index {finetuned_create_index['id']} successfully created.",
                 file=sys.stderr,
             )
             return Index(
                 client=self.client,
                 id=finetuned_create_index["id"],
                 index_type=self.index_type,
                 version=self.version,
```

### Comparing `objective_sdk-4.0.6/tests/sdk_integration_test.py` & `objective_sdk-4.0.7/tests/sdk_integration_test.py`

 * *Files identical despite different names*

### Comparing `objective_sdk-4.0.6/tests/test_objective.py` & `objective_sdk-4.0.7/tests/test_objective.py`

 * *Files identical despite different names*

### Comparing `objective_sdk-4.0.6/.gitignore` & `objective_sdk-4.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `objective_sdk-4.0.6/LICENSE` & `objective_sdk-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `objective_sdk-4.0.6/README.md` & `objective_sdk-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `objective_sdk-4.0.6/pyproject.toml` & `objective_sdk-4.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "objective-sdk"
-version = "4.0.6"
+version = "4.0.7"
 description = "Official Python SDK for Objective, Inc. APIs"
 authors = [
     { name = "Objective, Inc.", email = "support@objective.inc" }
 ]
 dependencies = [
     "requests>=2.26.0",
     "more-itertools>=8.10.0"
```

### Comparing `objective_sdk-4.0.6/PKG-INFO` & `objective_sdk-4.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: objective-sdk
-Version: 4.0.6
+Version: 4.0.7
 Summary: Official Python SDK for Objective, Inc. APIs
 Project-URL: Homepage, https://github.com/objective-inc/objective-py
 Project-URL: Repository, https://github.com/objective-inc/objective-py
 Author-email: "Objective, Inc." <support@objective.inc>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: more-itertools>=8.10.0
```

