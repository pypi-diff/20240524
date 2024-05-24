# Comparing `tmp/inmanta-2024.2.tar.gz` & `tmp/inmanta-2024.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmanta-2024.2.tar", last modified: Tue Apr  2 09:05:41 2024, max compression
+gzip compressed data, was "inmanta-2024.2.1.tar", last modified: Fri May 24 10:00:01 2024, max compression
```

## Comparing `inmanta-2024.2.tar` & `inmanta-2024.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-02 09:05:41.263446 inmanta-2024.2/
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    11357 2024-04-02 09:03:35.000000 inmanta-2024.2/LICENSE
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       17 2024-04-02 09:03:35.000000 inmanta-2024.2/MANIFEST.in
--rw-r--r--   0 jenkins    (988) jenkins    (986)      888 2024-04-02 09:05:41.263446 inmanta-2024.2/PKG-INFO
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      245 2024-04-02 09:03:35.000000 inmanta-2024.2/README.md
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-02 09:05:41.262446 inmanta-2024.2/inmanta.egg-info/
--rw-r--r--   0 jenkins    (988) jenkins    (986)      888 2024-04-02 09:05:41.000000 inmanta-2024.2/inmanta.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      217 2024-04-02 09:05:41.000000 inmanta-2024.2/inmanta.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)        1 2024-04-02 09:05:41.000000 inmanta-2024.2/inmanta.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       39 2024-04-02 09:05:41.000000 inmanta-2024.2/inmanta.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)        1 2024-04-02 09:05:41.000000 inmanta-2024.2/inmanta.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1908 2024-04-02 09:03:35.000000 inmanta-2024.2/pyproject.toml
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       59 2024-04-02 09:05:41.263446 inmanta-2024.2/setup.cfg
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1142 2024-04-02 09:03:35.000000 inmanta-2024.2/setup.py
+drwxr-xr-x   0      987 root         (0)        0 2024-05-24 10:00:01.153517 inmanta-2024.2.1/
+-rw-rw-r--   0      987 root         (0)    11357 2024-05-24 09:57:51.000000 inmanta-2024.2.1/LICENSE
+-rw-rw-r--   0      987 root         (0)       17 2024-05-24 09:57:51.000000 inmanta-2024.2.1/MANIFEST.in
+-rw-r--r--   0      987 root         (0)      890 2024-05-24 10:00:01.153517 inmanta-2024.2.1/PKG-INFO
+-rw-rw-r--   0      987 root         (0)      245 2024-05-24 09:57:51.000000 inmanta-2024.2.1/README.md
+drwxr-xr-x   0      987 root         (0)        0 2024-05-24 10:00:01.153517 inmanta-2024.2.1/inmanta.egg-info/
+-rw-r--r--   0      987 root         (0)      890 2024-05-24 10:00:01.000000 inmanta-2024.2.1/inmanta.egg-info/PKG-INFO
+-rw-r--r--   0      987 root         (0)      217 2024-05-24 10:00:01.000000 inmanta-2024.2.1/inmanta.egg-info/SOURCES.txt
+-rw-r--r--   0      987 root         (0)        1 2024-05-24 10:00:01.000000 inmanta-2024.2.1/inmanta.egg-info/dependency_links.txt
+-rw-r--r--   0      987 root         (0)       39 2024-05-24 10:00:01.000000 inmanta-2024.2.1/inmanta.egg-info/requires.txt
+-rw-r--r--   0      987 root         (0)        1 2024-05-24 10:00:01.000000 inmanta-2024.2.1/inmanta.egg-info/top_level.txt
+-rw-rw-r--   0      987 root         (0)     1908 2024-05-24 09:57:51.000000 inmanta-2024.2.1/pyproject.toml
+-rw-rw-r--   0      987 root         (0)       59 2024-05-24 10:00:01.154517 inmanta-2024.2.1/setup.cfg
+-rw-rw-r--   0      987 root         (0)     1144 2024-05-24 09:57:51.000000 inmanta-2024.2.1/setup.py
```

### Comparing `inmanta-2024.2/LICENSE` & `inmanta-2024.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inmanta-2024.2/PKG-INFO` & `inmanta-2024.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta
-Version: 2024.2
+Version: 2024.2.1
 Summary: Inmanta deployment tool
 Home-page: https://github.com/inmanta/inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Project-URL: Documentation, https://docs.inmanta.com/community/latest/
@@ -14,9 +14,9 @@
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 License-File: LICENSE
-Requires-Dist: inmanta-core==12.0.0
+Requires-Dist: inmanta-core==12.1.0
 Requires-Dist: inmanta-ui==5.1.1
```

### Comparing `inmanta-2024.2/inmanta.egg-info/PKG-INFO` & `inmanta-2024.2.1/inmanta.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta
-Version: 2024.2
+Version: 2024.2.1
 Summary: Inmanta deployment tool
 Home-page: https://github.com/inmanta/inmanta
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Project-URL: Documentation, https://docs.inmanta.com/community/latest/
@@ -14,9 +14,9 @@
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 License-File: LICENSE
-Requires-Dist: inmanta-core==12.0.0
+Requires-Dist: inmanta-core==12.1.0
 Requires-Dist: inmanta-ui==5.1.1
```

### Comparing `inmanta-2024.2/pyproject.toml` & `inmanta-2024.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -58,8 +58,8 @@
 image_name = "orchestrator"
 image_tags = [ "latest", "{version}",]
 registry_username_env = "GITHUB_REGISTRY_USERNAME"
 registry_password_env = "GITHUB_REGISTRY_PASSWORD"
 
 [tool.irt.dependencies.npm.web-console]
 repo = "https://github.com/inmanta/web-console"
-version = "==1.16.0"
+version = "==1.16.1"
```

### Comparing `inmanta-2024.2/setup.py` & `inmanta-2024.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(
-    version="2024.2",
+    version="2024.2.1",
     python_requires=">=3.11",  # also update classifiers
     # Meta data
     name="inmanta",
     description="Inmanta deployment tool",
     author="Inmanta",
     author_email="code@inmanta.com",
     url="https://github.com/inmanta/inmanta",
@@ -22,13 +22,13 @@
     ],
     keywords="orchestrator orchestration configurationmanagement",
     project_urls={
         "Bug Tracker": "https://github.com/inmanta/inmanta-core/issues",
         "Documentation": "https://docs.inmanta.com/community/latest/",
     },
     install_requires=[
-        "inmanta-core==12.0.0",
+        "inmanta-core==12.1.0",
         "inmanta-ui==5.1.1",
     ],
     # explicitly declare packages so setuptools does not attempt auto discovery
     packages=[],
 )
```

