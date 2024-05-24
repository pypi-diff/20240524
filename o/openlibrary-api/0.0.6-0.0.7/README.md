# Comparing `tmp/openlibrary_api-0.0.6.tar.gz` & `tmp/openlibrary_api-0.0.7.tar.gz`

## Comparing `openlibrary_api-0.0.6.tar` & `openlibrary_api-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/.gitattributes
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/requirements.txt
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/.vscode/settings.json
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/src/openlibrary_api/__init__.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/src/openlibrary_api/errors.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/src/openlibrary_api/models.py
--rw-r--r--   0        0        0     9757 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/src/openlibrary_api/ol_api.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/LICENSE
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 openlibrary_api-0.0.7/.gitattributes
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openlibrary_api-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 openlibrary_api-0.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 openlibrary_api-0.0.7/src/openlibrary_api/__init__.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 openlibrary_api-0.0.7/src/openlibrary_api/errors.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 openlibrary_api-0.0.7/src/openlibrary_api/models.py
+-rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 openlibrary_api-0.0.7/src/openlibrary_api/ol_api.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 openlibrary_api-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 openlibrary_api-0.0.7/LICENSE
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openlibrary_api-0.0.7/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 openlibrary_api-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openlibrary_api-0.0.7/PKG-INFO
```

### Comparing `openlibrary_api-0.0.6/src/openlibrary_api/errors.py` & `openlibrary_api-0.0.7/src/openlibrary_api/errors.py`

 * *Files identical despite different names*

### Comparing `openlibrary_api-0.0.6/src/openlibrary_api/models.py` & `openlibrary_api-0.0.7/src/openlibrary_api/models.py`

 * *Files identical despite different names*

### Comparing `openlibrary_api-0.0.6/src/openlibrary_api/ol_api.py` & `openlibrary_api-0.0.7/src/openlibrary_api/ol_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,19 @@
             APIErrorException: Error raised if error found in response dict keys
 
         Returns:
             dict containing response data
         """
         start = time.time()
         logger.debug(f"Sending request: {request}")
-        result = requests.get(request, timeout=4)
+        try:
+            result = requests.get(request, timeout=4)
+        except Exception as e:
+            logger.error(e)
+            raise e
         logger.debug(f"Received response:\nTime Taken: {time.time()-start}s\nCode: {result.status_code}\nContent: {result.json()}")
         if result.status_code != 200:
             raise StatusCodeException(result.status_code, request)
         data = result.json() #type: dict
         if "error" in data.keys():
             raise APIErrorException(data["error"], request)
         return data
```

### Comparing `openlibrary_api-0.0.6/.gitignore` & `openlibrary_api-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `openlibrary_api-0.0.6/LICENSE` & `openlibrary_api-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openlibrary_api-0.0.6/pyproject.toml` & `openlibrary_api-0.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openlibrary_api"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Angel Thomas", email="tnf.angel.19@gmail.com" },
 ]
 description = "A wrapper for the OpenLibrary API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `openlibrary_api-0.0.6/PKG-INFO` & `openlibrary_api-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openlibrary_api
-Version: 0.0.6
+Version: 0.0.7
 Summary: A wrapper for the OpenLibrary API
 Project-URL: Homepage, https://github.com/angelt19/openlibrary_api
 Project-URL: Issues, https://github.com/angelt19/openlibrary_api/issues
 Author-email: Angel Thomas <tnf.angel.19@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

