# Comparing `tmp/aiida_bader-0.0.6.tar.gz` & `tmp/aiida_bader-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_bader-0.0.6.tar", last modified: Fri May 10 07:02:13 2024, max compression
+gzip compressed data, was "aiida_bader-0.0.7.tar", last modified: Fri May 24 13:59:41 2024, max compression
```

## Comparing `aiida_bader-0.0.6.tar` & `aiida_bader-0.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-10 07:02:13.005303 aiida_bader-0.0.6/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1066 2024-03-25 15:26:07.000000 aiida_bader-0.0.6/LICENSE
--rw-r--r--   0 xing      (1000) xing      (1000)     2142 2024-05-10 07:02:13.005303 aiida_bader-0.0.6/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     1606 2024-03-25 15:26:07.000000 aiida_bader-0.0.6/README.md
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-10 07:02:13.005303 aiida_bader-0.0.6/aiida_bader/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.6/aiida_bader/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-10 07:02:13.005303 aiida_bader-0.0.6/aiida_bader/calculations/
--rw-rw-r--   0 xing      (1000) xing      (1000)     4842 2024-05-10 07:00:42.000000 aiida_bader-0.0.6/aiida_bader/calculations/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-10 07:02:13.005303 aiida_bader-0.0.6/aiida_bader/parsers/
--rw-rw-r--   0 xing      (1000) xing      (1000)     2005 2024-03-25 15:26:07.000000 aiida_bader-0.0.6/aiida_bader/parsers/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-10 07:02:13.005303 aiida_bader-0.0.6/aiida_bader/qeapp/
--rw-rw-r--   0 xing      (1000) xing      (1000)      708 2024-04-24 20:36:37.000000 aiida_bader-0.0.6/aiida_bader/qeapp/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3858 2024-04-10 19:56:14.000000 aiida_bader-0.0.6/aiida_bader/qeapp/result.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2857 2024-04-10 19:56:14.000000 aiida_bader-0.0.6/aiida_bader/qeapp/widget.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2758 2024-04-10 19:56:14.000000 aiida_bader-0.0.6/aiida_bader/qeapp/workchain.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-10 07:02:13.005303 aiida_bader-0.0.6/aiida_bader/workchains/
--rw-rw-r--   0 xing      (1000) xing      (1000)       93 2024-03-25 15:26:07.000000 aiida_bader-0.0.6/aiida_bader/workchains/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-10 07:02:13.005303 aiida_bader-0.0.6/aiida_bader/workchains/protocols/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.6/aiida_bader/workchains/protocols/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1196 2024-03-25 15:26:07.000000 aiida_bader-0.0.6/aiida_bader/workchains/protocols/bader.yaml
--rw-rw-r--   0 xing      (1000) xing      (1000)    10097 2024-05-10 07:00:42.000000 aiida_bader-0.0.6/aiida_bader/workchains/qe_bader.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-10 07:02:13.005303 aiida_bader-0.0.6/aiida_bader/workgraph/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.6/aiida_bader/workgraph/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      511 2024-05-10 07:00:42.000000 aiida_bader-0.0.6/aiida_bader/workgraph/cp2k_bader.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      900 2024-05-10 07:00:42.000000 aiida_bader-0.0.6/aiida_bader/workgraph/qe_bader.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-10 07:02:13.005303 aiida_bader-0.0.6/aiida_bader.egg-info/
--rw-r--r--   0 xing      (1000) xing      (1000)     2142 2024-05-10 07:02:13.000000 aiida_bader-0.0.6/aiida_bader.egg-info/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)      731 2024-05-10 07:02:13.000000 aiida_bader-0.0.6/aiida_bader.egg-info/SOURCES.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-05-10 07:02:13.000000 aiida_bader-0.0.6/aiida_bader.egg-info/dependency_links.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      256 2024-05-10 07:02:13.000000 aiida_bader-0.0.6/aiida_bader.egg-info/entry_points.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      106 2024-05-10 07:02:13.000000 aiida_bader-0.0.6/aiida_bader.egg-info/requires.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       12 2024-05-10 07:02:13.000000 aiida_bader-0.0.6/aiida_bader.egg-info/top_level.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-05-10 07:02:13.005303 aiida_bader-0.0.6/setup.cfg
--rw-rw-r--   0 xing      (1000) xing      (1000)     1562 2024-05-10 07:01:42.000000 aiida_bader-0.0.6/setup.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-10 07:02:13.005303 aiida_bader-0.0.6/tests/
--rw-rw-r--   0 xing      (1000) xing      (1000)      122 2024-03-25 15:26:07.000000 aiida_bader-0.0.6/tests/test_bader.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-24 13:59:41.345124 aiida_bader-0.0.7/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1066 2024-03-25 15:26:07.000000 aiida_bader-0.0.7/LICENSE
+-rw-r--r--   0 xing      (1000) xing      (1000)     2136 2024-05-24 13:59:41.345124 aiida_bader-0.0.7/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1606 2024-03-25 15:26:07.000000 aiida_bader-0.0.7/README.md
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-24 13:59:41.341124 aiida_bader-0.0.7/aiida_bader/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.7/aiida_bader/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-24 13:59:41.341124 aiida_bader-0.0.7/aiida_bader/calculations/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4842 2024-05-10 07:00:42.000000 aiida_bader-0.0.7/aiida_bader/calculations/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-24 13:59:41.341124 aiida_bader-0.0.7/aiida_bader/parsers/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2005 2024-03-25 15:26:07.000000 aiida_bader-0.0.7/aiida_bader/parsers/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-24 13:59:41.341124 aiida_bader-0.0.7/aiida_bader/qeapp/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      708 2024-04-24 20:36:37.000000 aiida_bader-0.0.7/aiida_bader/qeapp/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3858 2024-04-10 19:56:14.000000 aiida_bader-0.0.7/aiida_bader/qeapp/result.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2857 2024-04-10 19:56:14.000000 aiida_bader-0.0.7/aiida_bader/qeapp/widget.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2758 2024-04-10 19:56:14.000000 aiida_bader-0.0.7/aiida_bader/qeapp/workchain.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-24 13:59:41.341124 aiida_bader-0.0.7/aiida_bader/workchains/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       93 2024-03-25 15:26:07.000000 aiida_bader-0.0.7/aiida_bader/workchains/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-24 13:59:41.341124 aiida_bader-0.0.7/aiida_bader/workchains/protocols/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.7/aiida_bader/workchains/protocols/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1196 2024-03-25 15:26:07.000000 aiida_bader-0.0.7/aiida_bader/workchains/protocols/bader.yaml
+-rw-rw-r--   0 xing      (1000) xing      (1000)    10097 2024-05-10 07:00:42.000000 aiida_bader-0.0.7/aiida_bader/workchains/qe_bader.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-24 13:59:41.345124 aiida_bader-0.0.7/aiida_bader/workgraph/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.7/aiida_bader/workgraph/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      511 2024-05-10 07:00:42.000000 aiida_bader-0.0.7/aiida_bader/workgraph/cp2k_bader.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      900 2024-05-10 07:00:42.000000 aiida_bader-0.0.7/aiida_bader/workgraph/qe_bader.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-24 13:59:41.345124 aiida_bader-0.0.7/aiida_bader.egg-info/
+-rw-r--r--   0 xing      (1000) xing      (1000)     2136 2024-05-24 13:59:41.000000 aiida_bader-0.0.7/aiida_bader.egg-info/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)      731 2024-05-24 13:59:41.000000 aiida_bader-0.0.7/aiida_bader.egg-info/SOURCES.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-05-24 13:59:41.000000 aiida_bader-0.0.7/aiida_bader.egg-info/dependency_links.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      256 2024-05-24 13:59:41.000000 aiida_bader-0.0.7/aiida_bader.egg-info/entry_points.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      101 2024-05-24 13:59:41.000000 aiida_bader-0.0.7/aiida_bader.egg-info/requires.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       12 2024-05-24 13:59:41.000000 aiida_bader-0.0.7/aiida_bader.egg-info/top_level.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-05-24 13:59:41.345124 aiida_bader-0.0.7/setup.cfg
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1556 2024-05-24 13:59:14.000000 aiida_bader-0.0.7/setup.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-24 13:59:41.345124 aiida_bader-0.0.7/tests/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      122 2024-03-25 15:26:07.000000 aiida_bader-0.0.7/tests/test_bader.py
```

### Comparing `aiida_bader-0.0.6/LICENSE` & `aiida_bader-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.6/PKG-INFO` & `aiida_bader-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: aiida-bader
-Version: 0.0.6
+Version: 0.0.7
 Summary: AiiDA plugin for bader code.
-Home-page: https://github.com/superstart54/aiida-bader
+Home-page: https://github.com/superstar54/aiida-bader
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiida-core
 Requires-Dist: aiida-workgraph
-Requires-Dist: aiida-quantumespresso~=4.4
+Requires-Dist: aiida-quantumespresso
 Requires-Dist: aiida-cp2k
 Requires-Dist: weas-widget
 Requires-Dist: pytest
 Requires-Dist: pytest-cov
 Requires-Dist: pre-commit
 
 # AiiDA-Bader
```

### Comparing `aiida_bader-0.0.6/README.md` & `aiida_bader-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.6/aiida_bader/calculations/__init__.py` & `aiida_bader-0.0.7/aiida_bader/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.6/aiida_bader/parsers/__init__.py` & `aiida_bader-0.0.7/aiida_bader/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.6/aiida_bader/qeapp/__init__.py` & `aiida_bader-0.0.7/aiida_bader/qeapp/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.6/aiida_bader/qeapp/result.py` & `aiida_bader-0.0.7/aiida_bader/qeapp/result.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.6/aiida_bader/qeapp/widget.py` & `aiida_bader-0.0.7/aiida_bader/qeapp/widget.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.6/aiida_bader/qeapp/workchain.py` & `aiida_bader-0.0.7/aiida_bader/qeapp/workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.6/aiida_bader/workchains/protocols/bader.yaml` & `aiida_bader-0.0.7/aiida_bader/workchains/protocols/bader.yaml`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.6/aiida_bader/workchains/qe_bader.py` & `aiida_bader-0.0.7/aiida_bader/workchains/qe_bader.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.6/aiida_bader/workgraph/qe_bader.py` & `aiida_bader-0.0.7/aiida_bader/workgraph/qe_bader.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.6/aiida_bader.egg-info/PKG-INFO` & `aiida_bader-0.0.7/aiida_bader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: aiida-bader
-Version: 0.0.6
+Version: 0.0.7
 Summary: AiiDA plugin for bader code.
-Home-page: https://github.com/superstart54/aiida-bader
+Home-page: https://github.com/superstar54/aiida-bader
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiida-core
 Requires-Dist: aiida-workgraph
-Requires-Dist: aiida-quantumespresso~=4.4
+Requires-Dist: aiida-quantumespresso
 Requires-Dist: aiida-cp2k
 Requires-Dist: weas-widget
 Requires-Dist: pytest
 Requires-Dist: pytest-cov
 Requires-Dist: pre-commit
 
 # AiiDA-Bader
```

### Comparing `aiida_bader-0.0.6/aiida_bader.egg-info/SOURCES.txt` & `aiida_bader-0.0.7/aiida_bader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.6/setup.py` & `aiida_bader-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="aiida-bader",
-    version="0.0.6",
+    version="0.0.7",
     description="AiiDA plugin for bader code.",
     long_description=README,
     long_description_content_type="text/markdown",
-    url="https://github.com/superstart54/aiida-bader",
+    url="https://github.com/superstar54/aiida-bader",
     author="Xing Wang",
     author_email="xingwang1991@gmail.com",
     license="MIT License",
     classifiers=[],
     packages=find_packages(),
     install_requires=[
         "aiida-core",
         "aiida-workgraph",
-        "aiida-quantumespresso~=4.4",
+        "aiida-quantumespresso",
         "aiida-cp2k",
         "weas-widget",
         "pytest",
         "pytest-cov",
         "pre-commit",
     ],
     entry_points={
```

