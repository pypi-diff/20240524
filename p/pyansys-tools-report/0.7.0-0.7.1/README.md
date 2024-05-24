# Comparing `tmp/pyansys_tools_report-0.7.0.tar.gz` & `tmp/pyansys_tools_report-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyansys_tools_report-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyansys_tools_report-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyansys_tools_report-0.7.0.tar` & `pyansys_tools_report-0.7.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-10-04 10:16:11.378368 pyansys_tools_report-0.7.0/LICENSE
--rw-r--r--   0        0        0     6908 2023-10-04 10:16:11.378368 pyansys_tools_report-0.7.0/README.md
--rw-r--r--   0        0        0     1694 2023-10-04 10:16:11.378368 pyansys_tools_report-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      208 2023-10-04 10:16:11.378368 pyansys_tools_report-0.7.0/src/ansys/tools/report/__init__.py
--rw-r--r--   0        0        0      384 2023-10-04 10:16:11.378368 pyansys_tools_report-0.7.0/src/ansys/tools/report/_version.py
--rw-r--r--   0        0        0     6391 2023-10-04 10:16:11.378368 pyansys_tools_report-0.7.0/src/ansys/tools/report/report.py
--rw-r--r--   0        0        0     8098 1970-01-01 00:00:00.000000 pyansys_tools_report-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-24 07:19:41.053146 pyansys_tools_report-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6908 2024-05-24 07:19:41.053146 pyansys_tools_report-0.7.1/README.md
+-rw-r--r--   0        0        0     1694 2024-05-24 07:19:41.057146 pyansys_tools_report-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1362 2024-05-24 07:19:41.057146 pyansys_tools_report-0.7.1/src/ansys/tools/report/__init__.py
+-rw-r--r--   0        0        0     1538 2024-05-24 07:19:41.057146 pyansys_tools_report-0.7.1/src/ansys/tools/report/_version.py
+-rw-r--r--   0        0        0     7545 2024-05-24 07:19:41.057146 pyansys_tools_report-0.7.1/src/ansys/tools/report/report.py
+-rw-r--r--   0        0        0     8098 1970-01-01 00:00:00.000000 pyansys_tools_report-0.7.1/PKG-INFO
```

### Comparing `pyansys_tools_report-0.7.0/LICENSE` & `pyansys_tools_report-0.7.1/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 MIT License
 
-Copyright (c) 2022 ANSYS, Inc. All rights reserved.
+Copyright (c) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
```

### Comparing `pyansys_tools_report-0.7.0/README.md` & `pyansys_tools_report-0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 Each wheelhouse archive contains all the python wheels necessary to install
 PyAnsys Tools Report from scratch on Windows and Linux for Python >=3.9. You can install
 this on an isolated system with a fresh python or on a virtual environment.
 
 For example, on Linux with Python 3.9, unzip it and install it with the following:
 
 ```bash
-   unzip pyansys-tools-report-v0.7.0-wheelhouse-Linux-3.9.zip wheelhouse
+   unzip pyansys-tools-report-v0.7.1-wheelhouse-Linux-3.9.zip wheelhouse
    pip install pyansys-tools-report -f wheelhouse --no-index --upgrade --ignore-installed
 ```
 
 If you're on Windows with Python 3.9, unzip to a ``wheelhouse`` directory and
 install using the same command as before.
 
 Consider installing using a [virtual environment](https://docs.python.org/3/library/venv.html).
```

### Comparing `pyansys_tools_report-0.7.0/pyproject.toml` & `pyansys_tools_report-0.7.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "pyansys-tools-report"
-version = "0.7.0"
+version = "0.7.1"
 dynamic = ["description"]
 readme = "README.md"
 requires-python = ">=3.9,<4"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -29,23 +29,23 @@
     "setuptools>=65.5.1",
     "scooby>=0.5.12",
     "pyvista>=0.34.1",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "pytest==7.4.2",
-    "pytest-cov==4.1.0",
+    "pytest==8.2.1",
+    "pytest-cov==5.0.0",
 ]
 doc = [
-    "ansys_sphinx_theme==0.12.1",
-    "numpydoc==1.6.0",
+    "ansys_sphinx_theme==0.16.0",
+    "numpydoc==1.7.0",
     "Sphinx==7.2.1",
     "Sphinx-copybutton==0.5.2",
-    "myst-parser==2.0.0",
+    "myst-parser==3.0.1",
 ]
 
 [tool.flit.module]
 name = "ansys.tools.report"
 
 [project.urls]
 Source = "https://github.com/ansys/pyansys-tools-report"
```

### Comparing `pyansys_tools_report-0.7.0/src/ansys/tools/report/report.py` & `pyansys_tools_report-0.7.1/src/ansys/tools/report/report.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+# Copyright (C) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
+# SPDX-License-Identifier: MIT
+#
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """
 PyAnsys Tools Report.
 
 Module containing the standardized Report class for PyAnsys projects.
 """
 import os
 import sys
```

### Comparing `pyansys_tools_report-0.7.0/PKG-INFO` & `pyansys_tools_report-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyansys-tools-report
-Version: 0.7.0
+Version: 0.7.1
 Summary: PyAnsys Tools Report package.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
@@ -12,21 +12,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: setuptools>=65.5.1
 Requires-Dist: scooby>=0.5.12
 Requires-Dist: pyvista>=0.34.1
-Requires-Dist: ansys_sphinx_theme==0.12.1 ; extra == "doc"
-Requires-Dist: numpydoc==1.6.0 ; extra == "doc"
+Requires-Dist: ansys_sphinx_theme==0.16.0 ; extra == "doc"
+Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
 Requires-Dist: Sphinx==7.2.1 ; extra == "doc"
 Requires-Dist: Sphinx-copybutton==0.5.2 ; extra == "doc"
-Requires-Dist: myst-parser==2.0.0 ; extra == "doc"
-Requires-Dist: pytest==7.4.2 ; extra == "tests"
-Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
+Requires-Dist: myst-parser==3.0.1 ; extra == "doc"
+Requires-Dist: pytest==8.2.1 ; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
 Project-URL: Source, https://github.com/ansys/pyansys-tools-report
 Provides-Extra: doc
 Provides-Extra: tests
 
 # PyAnsys Tools Report
 
 [![PyAnsys](https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC)](https://docs.pyansys.com/)
@@ -131,15 +131,15 @@
 Each wheelhouse archive contains all the python wheels necessary to install
 PyAnsys Tools Report from scratch on Windows and Linux for Python >=3.9. You can install
 this on an isolated system with a fresh python or on a virtual environment.
 
 For example, on Linux with Python 3.9, unzip it and install it with the following:
 
 ```bash
-   unzip pyansys-tools-report-v0.7.0-wheelhouse-Linux-3.9.zip wheelhouse
+   unzip pyansys-tools-report-v0.7.1-wheelhouse-Linux-3.9.zip wheelhouse
    pip install pyansys-tools-report -f wheelhouse --no-index --upgrade --ignore-installed
 ```
 
 If you're on Windows with Python 3.9, unzip to a ``wheelhouse`` directory and
 install using the same command as before.
 
 Consider installing using a [virtual environment](https://docs.python.org/3/library/venv.html).
```

