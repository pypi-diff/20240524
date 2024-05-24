# Comparing `tmp/pyqvd-1.1.3.tar.gz` & `tmp/pyqvd-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqvd-1.1.3.tar", last modified: Thu May 16 15:06:05 2024, max compression
+gzip compressed data, was "pyqvd-2.0.0a1.tar", last modified: Fri May 24 16:35:35 2024, max compression
```

## Comparing `pyqvd-1.1.3.tar` & `pyqvd-2.0.0a1.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:06:05.127341 pyqvd-1.1.3/
--rw-rw-rw-   0        0        0     1096 2024-03-27 12:50:40.000000 pyqvd-1.1.3/LICENSE.md
--rw-rw-rw-   0        0        0    12492 2024-05-16 15:06:05.126342 pyqvd-1.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 15:06:05.125334 pyqvd-1.1.3/PyQvd.egg-info/
--rw-rw-rw-   0        0        0    12492 2024-05-16 15:06:05.000000 pyqvd-1.1.3/PyQvd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-05-16 15:06:05.000000 pyqvd-1.1.3/PyQvd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:06:05.000000 pyqvd-1.1.3/PyQvd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-16 15:06:05.000000 pyqvd-1.1.3/PyQvd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-16 15:06:05.000000 pyqvd-1.1.3/PyQvd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10282 2024-04-07 10:48:20.000000 pyqvd-1.1.3/README.md
--rw-rw-rw-   0        0        0     1288 2024-05-16 15:04:02.000000 pyqvd-1.1.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-16 15:06:05.123551 pyqvd-1.1.3/pyqvd/
--rw-rw-rw-   0        0        0       88 2024-04-02 10:45:55.000000 pyqvd-1.1.3/pyqvd/__init__.py
--rw-rw-rw-   0        0        0    38233 2024-05-16 15:03:41.000000 pyqvd-1.1.3/pyqvd/qvd.py
--rw-rw-rw-   0        0        0       42 2024-05-16 15:06:05.128312 pyqvd-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 16:35:35.194218 pyqvd-2.0.0a1/
+-rw-rw-rw-   0        0        0     1096 2024-03-27 12:50:40.000000 pyqvd-2.0.0a1/LICENSE.md
+-rw-rw-rw-   0        0        0     4927 2024-05-24 16:35:35.193199 pyqvd-2.0.0a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-24 16:35:35.191697 pyqvd-2.0.0a1/PyQvd.egg-info/
+-rw-rw-rw-   0        0        0     4927 2024-05-24 16:35:35.000000 pyqvd-2.0.0a1/PyQvd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-05-24 16:35:35.000000 pyqvd-2.0.0a1/PyQvd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 16:35:35.000000 pyqvd-2.0.0a1/PyQvd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-24 16:35:35.000000 pyqvd-2.0.0a1/PyQvd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-24 16:35:35.000000 pyqvd-2.0.0a1/PyQvd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2707 2024-05-24 16:33:25.000000 pyqvd-2.0.0a1/README.md
+-rw-rw-rw-   0        0        0     1298 2024-05-24 16:33:25.000000 pyqvd-2.0.0a1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-24 16:35:35.160724 pyqvd-2.0.0a1/pyqvd/
+-rw-rw-rw-   0        0        0      231 2024-05-24 16:12:10.000000 pyqvd-2.0.0a1/pyqvd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:35:35.190666 pyqvd-2.0.0a1/pyqvd/io/
+-rw-rw-rw-   0        0        0      342 2024-05-24 16:12:10.000000 pyqvd-2.0.0a1/pyqvd/io/__init__.py
+-rw-rw-rw-   0        0        0    11216 2024-05-24 16:12:10.000000 pyqvd-2.0.0a1/pyqvd/io/reader.py
+-rw-rw-rw-   0        0        0    17359 2024-05-24 16:12:10.000000 pyqvd-2.0.0a1/pyqvd/io/writer.py
+-rw-rw-rw-   0        0        0    55617 2024-05-24 16:12:10.000000 pyqvd-2.0.0a1/pyqvd/qvd.py
+-rw-rw-rw-   0        0        0       42 2024-05-24 16:35:35.194218 pyqvd-2.0.0a1/setup.cfg
```

### Comparing `pyqvd-1.1.3/LICENSE.md` & `pyqvd-2.0.0a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyqvd-1.1.3/pyproject.toml` & `pyqvd-2.0.0a1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyQvd"
-version = "1.1.3"
+version = "2.0.0-alpha.1"
 description = "Utility library for reading/writing Qlik View Data (QVD) files in Python."
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE.md"}
 authors = [
     {name = "Constantin Müller", email = "info@mueller-constantin.de"},
 ]
 keywords = ["qlik", "qvd", "qlik sense", "qlik view", "pandas"]
 requires-python = ">=3.8"
 dependencies = [
     "tabulate"
 ]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.8"
 ]
 
 [project.urls]
 Homepage = "https://github.com/MuellerConstantin/PyQvd"
 Repository = "https://github.com/MuellerConstantin/PyQvd.git"
 Issues = "https://github.com/MuellerConstantin/PyQvd/issues"
+Documentation = "https://pyqvd.readthedocs.io"
 
 [project.optional-dependencies]
 pandas = ["pandas"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

