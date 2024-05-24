# Comparing `tmp/polymatch-0.4.2.tar.gz` & `tmp/polymatch-0.5.0.tar.gz`

## Comparing `polymatch-0.4.2.tar` & `polymatch-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 polymatch-0.4.2/.editorconfig
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 polymatch-0.4.2/.gitattributes
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 polymatch-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 polymatch-0.4.2/CHANGELOG.md
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 polymatch-0.4.2/codecov.yml
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 polymatch-0.4.2/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 polymatch-0.4.2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 polymatch-0.4.2/.vscode/extensions.json
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 polymatch-0.4.2/.vscode/settings.json
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 polymatch-0.4.2/polymatch/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 polymatch-0.4.2/polymatch/_version.py
--rw-r--r--   0        0        0    11300 2020-02-02 00:00:00.000000 polymatch-0.4.2/polymatch/base.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 polymatch-0.4.2/polymatch/error.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polymatch-0.4.2/polymatch/py.typed
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 polymatch-0.4.2/polymatch/registry.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 polymatch-0.4.2/polymatch/matchers/__init__.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 polymatch-0.4.2/polymatch/matchers/glob.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 polymatch-0.4.2/polymatch/matchers/regex.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 polymatch-0.4.2/polymatch/matchers/standard.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 polymatch-0.4.2/scripts/__init__.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 polymatch-0.4.2/scripts/fix_pre_commit.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 polymatch-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 polymatch-0.4.2/tests/base_test.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 polymatch-0.4.2/tests/test_glob.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 polymatch-0.4.2/tests/test_pickling.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 polymatch-0.4.2/tests/test_regex.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 polymatch-0.4.2/tests/test_registry.py
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 polymatch-0.4.2/tests/test_standard.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 polymatch-0.4.2/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 polymatch-0.4.2/LICENSE.txt
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 polymatch-0.4.2/README.md
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 polymatch-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 polymatch-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 polymatch-0.5.0/.editorconfig
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 polymatch-0.5.0/.gitattributes
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 polymatch-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 polymatch-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 polymatch-0.5.0/codecov.yml
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 polymatch-0.5.0/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 polymatch-0.5.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 polymatch-0.5.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 polymatch-0.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 polymatch-0.5.0/polymatch/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 polymatch-0.5.0/polymatch/_version.py
+-rw-r--r--   0        0        0    11300 2020-02-02 00:00:00.000000 polymatch-0.5.0/polymatch/base.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 polymatch-0.5.0/polymatch/error.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polymatch-0.5.0/polymatch/py.typed
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 polymatch-0.5.0/polymatch/registry.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 polymatch-0.5.0/polymatch/matchers/__init__.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 polymatch-0.5.0/polymatch/matchers/glob.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 polymatch-0.5.0/polymatch/matchers/regex.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 polymatch-0.5.0/polymatch/matchers/standard.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 polymatch-0.5.0/scripts/__init__.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 polymatch-0.5.0/scripts/fix_pre_commit.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 polymatch-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 polymatch-0.5.0/tests/base_test.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 polymatch-0.5.0/tests/test_glob.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 polymatch-0.5.0/tests/test_pickling.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 polymatch-0.5.0/tests/test_regex.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 polymatch-0.5.0/tests/test_registry.py
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 polymatch-0.5.0/tests/test_standard.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 polymatch-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 polymatch-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 polymatch-0.5.0/README.md
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 polymatch-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 polymatch-0.5.0/PKG-INFO
```

### Comparing `polymatch-0.4.2/.pre-commit-config.yaml` & `polymatch-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/.devcontainer/devcontainer.json` & `polymatch-0.5.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/.vscode/settings.json` & `polymatch-0.5.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/polymatch/__init__.py` & `polymatch-0.5.0/polymatch/__init__.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/polymatch/base.py` & `polymatch-0.5.0/polymatch/base.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/polymatch/error.py` & `polymatch-0.5.0/polymatch/error.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/polymatch/registry.py` & `polymatch-0.5.0/polymatch/registry.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/polymatch/matchers/glob.py` & `polymatch-0.5.0/polymatch/matchers/glob.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/polymatch/matchers/regex.py` & `polymatch-0.5.0/polymatch/matchers/regex.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/polymatch/matchers/standard.py` & `polymatch-0.5.0/polymatch/matchers/standard.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/scripts/fix_pre_commit.py` & `polymatch-0.5.0/scripts/fix_pre_commit.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/tests/base_test.py` & `polymatch-0.5.0/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/tests/test_glob.py` & `polymatch-0.5.0/tests/test_glob.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/tests/test_pickling.py` & `polymatch-0.5.0/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/tests/test_regex.py` & `polymatch-0.5.0/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/tests/test_registry.py` & `polymatch-0.5.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/tests/test_standard.py` & `polymatch-0.5.0/tests/test_standard.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/.gitignore` & `polymatch-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/LICENSE.txt` & `polymatch-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/README.md` & `polymatch-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/pyproject.toml` & `polymatch-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polymatch-0.4.2/PKG-INFO` & `polymatch-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polymatch
-Version: 0.4.2
+Version: 0.5.0
 Summary: A polymorphic pattern matching library for Python
 Project-URL: Homepage, https://github.com/TotallyNotRobots/polymatch
 Author-email: linuxdaemon <linuxdaemon.irc@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: library,pattern-matching,regex,utility
 Classifier: Development Status :: 3 - Alpha
```

