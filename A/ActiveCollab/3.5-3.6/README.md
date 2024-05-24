# Comparing `tmp/activecollab-3.5.tar.gz` & `tmp/activecollab-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activecollab-3.5.tar", last modified: Wed Apr 24 05:16:27 2024, max compression
+gzip compressed data, was "activecollab-3.6.tar", last modified: Fri May 24 03:30:17 2024, max compression
```

## Comparing `activecollab-3.5.tar` & `activecollab-3.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:16:27.171677 activecollab-3.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:16:27.167677 activecollab-3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:16:27.171677 activecollab-3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-24 05:16:20.000000 activecollab-3.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 05:16:20.000000 activecollab-3.5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:16:27.171677 activecollab-3.5/ActiveCollab/
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-24 05:16:20.000000 activecollab-3.5/ActiveCollab/ActiveCollab.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 05:16:20.000000 activecollab-3.5/ActiveCollab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:16:27.171677 activecollab-3.5/ActiveCollab/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-24 05:16:20.000000 activecollab-3.5/ActiveCollab/__pycache__/ActiveCollab.cpython-38.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:16:27.171677 activecollab-3.5/ActiveCollab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-24 05:16:27.000000 activecollab-3.5/ActiveCollab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-24 05:16:27.000000 activecollab-3.5/ActiveCollab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 05:16:27.000000 activecollab-3.5/ActiveCollab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 05:16:27.000000 activecollab-3.5/ActiveCollab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 05:16:27.000000 activecollab-3.5/ActiveCollab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 05:16:20.000000 activecollab-3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-24 05:16:27.171677 activecollab-3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 05:16:20.000000 activecollab-3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-24 05:16:20.000000 activecollab-3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 05:16:27.171677 activecollab-3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-24 05:16:20.000000 activecollab-3.5/setup.py_bck
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:30:17.910588 activecollab-3.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:30:17.906588 activecollab-3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:30:17.906588 activecollab-3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-24 03:30:12.000000 activecollab-3.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-24 03:30:12.000000 activecollab-3.6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:30:17.910588 activecollab-3.6/ActiveCollab/
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-24 03:30:12.000000 activecollab-3.6/ActiveCollab/ActiveCollab.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 03:30:12.000000 activecollab-3.6/ActiveCollab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:30:17.910588 activecollab-3.6/ActiveCollab/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-24 03:30:12.000000 activecollab-3.6/ActiveCollab/__pycache__/ActiveCollab.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:30:17.910588 activecollab-3.6/ActiveCollab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-24 03:30:17.000000 activecollab-3.6/ActiveCollab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-24 03:30:17.000000 activecollab-3.6/ActiveCollab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 03:30:17.000000 activecollab-3.6/ActiveCollab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 03:30:17.000000 activecollab-3.6/ActiveCollab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 03:30:17.000000 activecollab-3.6/ActiveCollab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-24 03:30:12.000000 activecollab-3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-24 03:30:17.910588 activecollab-3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-24 03:30:12.000000 activecollab-3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-24 03:30:12.000000 activecollab-3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 03:30:17.910588 activecollab-3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-24 03:30:12.000000 activecollab-3.6/setup.py_bck
```

### Comparing `activecollab-3.5/.github/workflows/publish.yml` & `activecollab-3.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `activecollab-3.5/ActiveCollab/ActiveCollab.py` & `activecollab-3.6/ActiveCollab/ActiveCollab.py`

 * *Files identical despite different names*

### Comparing `activecollab-3.5/ActiveCollab/__pycache__/ActiveCollab.cpython-38.pyc` & `activecollab-3.6/ActiveCollab/__pycache__/ActiveCollab.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `activecollab-3.5/ActiveCollab.egg-info/PKG-INFO` & `activecollab-3.6/ActiveCollab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ActiveCollab
-Version: 3.5
+Version: 3.6
 Summary: A python library working with activeCollab
-Author-email: Ankushtpss <ankushkumartpss@gmail.com>
-Project-URL: Homepage, https://github.com/Ankushtpss/ActiveCollab
-Project-URL: Bug Tracker, https://github.com/Ankushtpss/ActiveCollab/issues
+Author-email: Ankush Kumar <ankush1611996@gmail.com>
+Project-URL: Homepage, https://github.com/AnkushRozra/ActiveCollab
+Project-URL: Bug Tracker, https://github.com/AnkushRozra/ActiveCollab/issues
 Keywords: Active Collab,ActiveCollab,Active Collab SDK,active collab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `activecollab-3.5/LICENSE` & `activecollab-3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `activecollab-3.5/PKG-INFO` & `activecollab-3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ActiveCollab
-Version: 3.5
+Version: 3.6
 Summary: A python library working with activeCollab
-Author-email: Ankushtpss <ankushkumartpss@gmail.com>
-Project-URL: Homepage, https://github.com/Ankushtpss/ActiveCollab
-Project-URL: Bug Tracker, https://github.com/Ankushtpss/ActiveCollab/issues
+Author-email: Ankush Kumar <ankush1611996@gmail.com>
+Project-URL: Homepage, https://github.com/AnkushRozra/ActiveCollab
+Project-URL: Bug Tracker, https://github.com/AnkushRozra/ActiveCollab/issues
 Keywords: Active Collab,ActiveCollab,Active Collab SDK,active collab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `activecollab-3.5/README.md` & `activecollab-3.6/README.md`

 * *Files identical despite different names*

### Comparing `activecollab-3.5/pyproject.toml` & `activecollab-3.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "ActiveCollab"
 authors = [
-  { name="Ankushtpss", email="ankushkumartpss@gmail.com" },
+  { name="Ankush Kumar", email="ankush1611996@gmail.com" },
 ]
 description = "A python library working with activeCollab"
 keywords = ["Active Collab", "ActiveCollab",  "Active Collab SDK", "active collab"]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -14,19 +14,19 @@
 ]
 
 dependencies = [
     "requests",
     "sys",
 ]
 
-version = "3.5"
+version = "3.6"
 
 [tool.setuptools_scm]
 
 [project.urls]
-"Homepage" = "https://github.com/Ankushtpss/ActiveCollab"
-"Bug Tracker" = "https://github.com/Ankushtpss/ActiveCollab/issues"
+"Homepage" = "https://github.com/AnkushRozra/ActiveCollab"
+"Bug Tracker" = "https://github.com/AnkushRozra/ActiveCollab/issues"
 
 
 [build-system]
 requires = ["setuptools","setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
```

### Comparing `activecollab-3.5/setup.py_bck` & `activecollab-3.6/setup.py_bck`

 * *Files identical despite different names*

