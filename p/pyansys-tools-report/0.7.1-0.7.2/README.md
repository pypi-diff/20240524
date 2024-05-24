# Comparing `tmp/pyansys_tools_report-0.7.1.tar.gz` & `tmp/pyansys_tools_report-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyansys_tools_report-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyansys_tools_report-0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyansys_tools_report-0.7.1.tar` & `pyansys_tools_report-0.7.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-05-24 07:19:41.053146 pyansys_tools_report-0.7.1/LICENSE
--rw-r--r--   0        0        0     6908 2024-05-24 07:19:41.053146 pyansys_tools_report-0.7.1/README.md
--rw-r--r--   0        0        0     1694 2024-05-24 07:19:41.057146 pyansys_tools_report-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1362 2024-05-24 07:19:41.057146 pyansys_tools_report-0.7.1/src/ansys/tools/report/__init__.py
--rw-r--r--   0        0        0     1538 2024-05-24 07:19:41.057146 pyansys_tools_report-0.7.1/src/ansys/tools/report/_version.py
--rw-r--r--   0        0        0     7545 2024-05-24 07:19:41.057146 pyansys_tools_report-0.7.1/src/ansys/tools/report/report.py
--rw-r--r--   0        0        0     8098 1970-01-01 00:00:00.000000 pyansys_tools_report-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-24 07:38:53.323074 pyansys_tools_report-0.7.2/LICENSE
+-rw-r--r--   0        0        0     6908 2024-05-24 07:38:53.323074 pyansys_tools_report-0.7.2/README.md
+-rw-r--r--   0        0        0     1694 2024-05-24 07:38:53.327074 pyansys_tools_report-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1362 2024-05-24 07:38:53.327074 pyansys_tools_report-0.7.2/src/ansys/tools/report/__init__.py
+-rw-r--r--   0        0        0     1538 2024-05-24 07:38:53.327074 pyansys_tools_report-0.7.2/src/ansys/tools/report/_version.py
+-rw-r--r--   0        0        0     7545 2024-05-24 07:38:53.327074 pyansys_tools_report-0.7.2/src/ansys/tools/report/report.py
+-rw-r--r--   0        0        0     8098 1970-01-01 00:00:00.000000 pyansys_tools_report-0.7.2/PKG-INFO
```

### Comparing `pyansys_tools_report-0.7.1/LICENSE` & `pyansys_tools_report-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyansys_tools_report-0.7.1/README.md` & `pyansys_tools_report-0.7.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 Each wheelhouse archive contains all the python wheels necessary to install
 PyAnsys Tools Report from scratch on Windows and Linux for Python >=3.9. You can install
 this on an isolated system with a fresh python or on a virtual environment.
 
 For example, on Linux with Python 3.9, unzip it and install it with the following:
 
 ```bash
-   unzip pyansys-tools-report-v0.7.1-wheelhouse-Linux-3.9.zip wheelhouse
+   unzip pyansys-tools-report-v0.7.2-wheelhouse-Linux-3.9.zip wheelhouse
    pip install pyansys-tools-report -f wheelhouse --no-index --upgrade --ignore-installed
 ```
 
 If you're on Windows with Python 3.9, unzip to a ``wheelhouse`` directory and
 install using the same command as before.
 
 Consider installing using a [virtual environment](https://docs.python.org/3/library/venv.html).
```

### Comparing `pyansys_tools_report-0.7.1/pyproject.toml` & `pyansys_tools_report-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "pyansys-tools-report"
-version = "0.7.1"
+version = "0.7.2"
 dynamic = ["description"]
 readme = "README.md"
 requires-python = ">=3.9,<4"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
```

### Comparing `pyansys_tools_report-0.7.1/src/ansys/tools/report/__init__.py` & `pyansys_tools_report-0.7.2/src/ansys/tools/report/__init__.py`

 * *Files identical despite different names*

### Comparing `pyansys_tools_report-0.7.1/src/ansys/tools/report/_version.py` & `pyansys_tools_report-0.7.2/src/ansys/tools/report/_version.py`

 * *Files identical despite different names*

### Comparing `pyansys_tools_report-0.7.1/src/ansys/tools/report/report.py` & `pyansys_tools_report-0.7.2/src/ansys/tools/report/report.py`

 * *Files identical despite different names*

### Comparing `pyansys_tools_report-0.7.1/PKG-INFO` & `pyansys_tools_report-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyansys-tools-report
-Version: 0.7.1
+Version: 0.7.2
 Summary: PyAnsys Tools Report package.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
@@ -131,15 +131,15 @@
 Each wheelhouse archive contains all the python wheels necessary to install
 PyAnsys Tools Report from scratch on Windows and Linux for Python >=3.9. You can install
 this on an isolated system with a fresh python or on a virtual environment.
 
 For example, on Linux with Python 3.9, unzip it and install it with the following:
 
 ```bash
-   unzip pyansys-tools-report-v0.7.1-wheelhouse-Linux-3.9.zip wheelhouse
+   unzip pyansys-tools-report-v0.7.2-wheelhouse-Linux-3.9.zip wheelhouse
    pip install pyansys-tools-report -f wheelhouse --no-index --upgrade --ignore-installed
 ```
 
 If you're on Windows with Python 3.9, unzip to a ``wheelhouse`` directory and
 install using the same command as before.
 
 Consider installing using a [virtual environment](https://docs.python.org/3/library/venv.html).
```

