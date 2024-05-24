# Comparing `tmp/validate_pyproject_schema_store-2024.5.20.tar.gz` & `tmp/validate_pyproject_schema_store-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue May 21 04:55:19 2024, max compression
+gzip compressed data, last modified: Fri May 24 02:52:07 2024, max compression
```

## Comparing `validate_pyproject_schema_store-2024.5.20.tar` & `validate_pyproject_schema_store-2024.5.24.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2273 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.pre-commit-config.yaml
--rw-r--r--   0        0        0      305 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0     2412 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/release.yml
--rw-r--r--   0        0        0      668 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1093 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/workflows/bump.yml
--rw-r--r--   0        0        0      843 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/workflows/cd.yml
--rw-r--r--   0        0        0      885 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/workflows/ci.yml
--rw-r--r--   0        0        0      188 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/__init__.py
--rw-r--r--   0        0        0        0 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/py.typed
--rw-r--r--   0        0        0     1373 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/schema.py
--rw-r--r--   0        0        0     6871 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/black.schema.json
--rw-r--r--   0        0        0    20516 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json
--rw-r--r--   0        0        0    27093 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/hatch.schema.json
--rw-r--r--   0        0        0    44330 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/mypy.schema.json
--rw-r--r--   0        0        0    25354 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/pdm.schema.json
--rw-r--r--   0        0        0    20027 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/poetry.schema.json
--rw-r--r--   0        0        0    70835 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/pyright.schema.json
--rw-r--r--   0        0        0   128445 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/ruff.schema.json
--rw-r--r--   0        0        0    20535 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/scikit-build.schema.json
--rw-r--r--   0        0        0    13647 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/setuptools.schema.json
--rw-r--r--   0        0        0      691 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/tool.json
--rw-r--r--   0        0        0    24630 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/uv.schema.json
--rw-r--r--   0        0        0      890 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/tests/test_package.py
--rw-r--r--   0        0        0      850 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/tests/test_validate_pyproject.py
--rwxr-xr-x   0        0        0     2467 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/tools/sync.py
--rw-r--r--   0        0        0     2218 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.gitignore
--rw-r--r--   0        0        0    11358 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/LICENSE
--rw-r--r--   0        0        0     2080 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/README.md
--rw-r--r--   0        0        0     4986 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/pyproject.toml
--rw-r--r--   0        0        0     4156 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/PKG-INFO
+-rw-r--r--   0        0        0     2273 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      305 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     2412 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/release.yml
+-rw-r--r--   0        0        0      668 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1093 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/workflows/bump.yml
+-rw-r--r--   0        0        0      843 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      885 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      188 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/py.typed
+-rw-r--r--   0        0        0     1373 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/schema.py
+-rw-r--r--   0        0        0     6871 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/black.schema.json
+-rw-r--r--   0        0        0    20516 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json
+-rw-r--r--   0        0        0    27093 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/hatch.schema.json
+-rw-r--r--   0        0        0    44330 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/mypy.schema.json
+-rw-r--r--   0        0        0    25354 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/pdm.schema.json
+-rw-r--r--   0        0        0    20182 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/poetry.schema.json
+-rw-r--r--   0        0        0    70835 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/pyright.schema.json
+-rw-r--r--   0        0        0   128445 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/ruff.schema.json
+-rw-r--r--   0        0        0    20535 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/scikit-build.schema.json
+-rw-r--r--   0        0        0    13647 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/setuptools.schema.json
+-rw-r--r--   0        0        0      691 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/tool.json
+-rw-r--r--   0        0        0    24630 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/uv.schema.json
+-rw-r--r--   0        0        0      890 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/tests/test_package.py
+-rw-r--r--   0        0        0      850 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/tests/test_validate_pyproject.py
+-rwxr-xr-x   0        0        0     2467 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/tools/sync.py
+-rw-r--r--   0        0        0     2218 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/.gitignore
+-rw-r--r--   0        0        0    11358 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/LICENSE
+-rw-r--r--   0        0        0     2080 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/README.md
+-rw-r--r--   0        0        0     4986 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/pyproject.toml
+-rw-r--r--   0        0        0     4156 2024-05-24 02:52:07.000000 validate_pyproject_schema_store-2024.5.24/PKG-INFO
```

### Comparing `validate_pyproject_schema_store-2024.5.20/.pre-commit-config.yaml` & `validate_pyproject_schema_store-2024.5.24/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/.github/CONTRIBUTING.md` & `validate_pyproject_schema_store-2024.5.24/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/.github/matchers/pylint.json` & `validate_pyproject_schema_store-2024.5.24/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/.github/workflows/bump.yml` & `validate_pyproject_schema_store-2024.5.24/.github/workflows/bump.yml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/.github/workflows/cd.yml` & `validate_pyproject_schema_store-2024.5.24/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/.github/workflows/ci.yml` & `validate_pyproject_schema_store-2024.5.24/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/schema.py` & `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/schema.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/black.schema.json` & `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/black.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json` & `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/hatch.schema.json` & `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/hatch.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/mypy.schema.json` & `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/mypy.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/pdm.schema.json` & `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/pdm.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/poetry.schema.json` & `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/poetry.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999945746527777%*

 * *Differences: {"'properties'": "{'packages': {'items': {'properties': {'to': OrderedDict([('type', 'string'), "*

 * *                 "('description', 'Where the package should be installed in the final "*

 * *                 "distribution.')])}}}}"}*

```diff
@@ -606,14 +606,18 @@
                     },
                     "from": {
                         "description": "Where the source directory of the package resides.",
                         "type": "string"
                     },
                     "include": {
                         "$ref": "#/definitions/poetry-include-path"
+                    },
+                    "to": {
+                        "description": "Where the package should be installed in the final distribution.",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "include"
                 ],
                 "type": "object"
             },
```

### Comparing `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/pyright.schema.json` & `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/pyright.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/ruff.schema.json` & `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/ruff.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/scikit-build.schema.json` & `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/scikit-build.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/setuptools.schema.json` & `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/setuptools.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/tool.json` & `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/tool.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/uv.schema.json` & `validate_pyproject_schema_store-2024.5.24/src/validate_pyproject_schema_store/resources/uv.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/tests/test_package.py` & `validate_pyproject_schema_store-2024.5.24/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/tests/test_validate_pyproject.py` & `validate_pyproject_schema_store-2024.5.24/tests/test_validate_pyproject.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/tools/sync.py` & `validate_pyproject_schema_store-2024.5.24/tools/sync.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/.gitignore` & `validate_pyproject_schema_store-2024.5.24/.gitignore`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/LICENSE` & `validate_pyproject_schema_store-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/README.md` & `validate_pyproject_schema_store-2024.5.24/README.md`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.20/pyproject.toml` & `validate_pyproject_schema_store-2024.5.24/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "validate-pyproject-schema-store"
-version = "2024.05.20"
+version = "2024.05.24"
 authors = [
   { name = "Henry Schreiner", email = "henryfs@princeton.edu" },
 ]
 description = "A plugin set for validate-pyproject and schema-store."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `validate_pyproject_schema_store-2024.5.20/PKG-INFO` & `validate_pyproject_schema_store-2024.5.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: validate-pyproject-schema-store
-Version: 2024.5.20
+Version: 2024.5.24
 Summary: A plugin set for validate-pyproject and schema-store.
 Project-URL: Homepage, https://github.com/henryiii/validate-pyproject-schema-store
 Project-URL: Bug Tracker, https://github.com/henryiii/validate-pyproject-schema-store/issues
 Project-URL: Discussions, https://github.com/henryiii/validate-pyproject-schema-store/discussions
 Project-URL: Changelog, https://github.com/henryiii/validate-pyproject-schema-store/releases
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
```

