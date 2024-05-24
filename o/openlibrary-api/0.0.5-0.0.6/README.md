# Comparing `tmp/openlibrary_api-0.0.5.tar.gz` & `tmp/openlibrary_api-0.0.6.tar.gz`

## Comparing `openlibrary_api-0.0.5.tar` & `openlibrary_api-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/.gitattributes
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/requirements.txt
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/.vscode/settings.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/src/openlibrary_api/__init__.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/src/openlibrary_api/errors.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/src/openlibrary_api/models.py
--rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/src/openlibrary_api/ol_api.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/LICENSE
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openlibrary_api-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/.gitattributes
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/.vscode/settings.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/src/openlibrary_api/__init__.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/src/openlibrary_api/errors.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/src/openlibrary_api/models.py
+-rw-r--r--   0        0        0     9757 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/src/openlibrary_api/ol_api.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/LICENSE
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openlibrary_api-0.0.6/PKG-INFO
```

### Comparing `openlibrary_api-0.0.5/src/openlibrary_api/errors.py` & `openlibrary_api-0.0.6/src/openlibrary_api/errors.py`

 * *Files identical despite different names*

### Comparing `openlibrary_api-0.0.5/src/openlibrary_api/models.py` & `openlibrary_api-0.0.6/src/openlibrary_api/models.py`

 * *Files identical despite different names*

### Comparing `openlibrary_api-0.0.5/src/openlibrary_api/ol_api.py` & `openlibrary_api-0.0.6/src/openlibrary_api/ol_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,14 +175,15 @@
             works, 
             result["physical_format"] if "physical_format" in result.keys() else "unknown",
             result["isbn_10"] if "isbn_10" in result.keys() else "unknown",
             result["isbn_13"] if "isbn_13" in result.keys() else "unknown",
             result["contributions"] if "contributions" in result.keys() else []
             )
         self.editions_cache.add(olid, edition)
+        return edition
 
     def get_edition_by_isbn(self, isbn: str) -> Edition | None:
         result = self.__make_isbn_request(isbn)
         if result is None:
             return None
         return self.__build_edition_from_result(result)
```

### Comparing `openlibrary_api-0.0.5/.gitignore` & `openlibrary_api-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `openlibrary_api-0.0.5/LICENSE` & `openlibrary_api-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openlibrary_api-0.0.5/pyproject.toml` & `openlibrary_api-0.0.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openlibrary_api"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Angel Thomas", email="tnf.angel.19@gmail.com" },
 ]
 description = "A wrapper for the OpenLibrary API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `openlibrary_api-0.0.5/PKG-INFO` & `openlibrary_api-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openlibrary_api
-Version: 0.0.5
+Version: 0.0.6
 Summary: A wrapper for the OpenLibrary API
 Project-URL: Homepage, https://github.com/angelt19/openlibrary_api
 Project-URL: Issues, https://github.com/angelt19/openlibrary_api/issues
 Author-email: Angel Thomas <tnf.angel.19@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

