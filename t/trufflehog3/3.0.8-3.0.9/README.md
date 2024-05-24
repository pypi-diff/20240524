# Comparing `tmp/trufflehog3-3.0.8.tar.gz` & `tmp/trufflehog3-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trufflehog3-3.0.8.tar", last modified: Thu Oct 26 21:35:23 2023, max compression
+gzip compressed data, was "trufflehog3-3.0.9.tar", last modified: Sat Jan 27 20:47:14 2024, max compression
```

## Comparing `trufflehog3-3.0.8.tar` & `trufflehog3-3.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2023-10-26 21:35:23.253700 trufflehog3-3.0.8/
--rw-r--r--   0 ekzo       (501) staff       (20)    18046 2021-08-06 20:47:08.000000 trufflehog3-3.0.8/LICENSE
--rw-r--r--   0 ekzo       (501) staff       (20)       29 2021-08-06 20:47:15.000000 trufflehog3-3.0.8/MANIFEST.in
--rw-r--r--   0 ekzo       (501) staff       (20)     3918 2023-10-26 21:35:23.253746 trufflehog3-3.0.8/PKG-INFO
--rw-r--r--   0 ekzo       (501) staff       (20)     3615 2023-07-18 16:35:02.000000 trufflehog3-3.0.8/README.md
--rw-r--r--   0 ekzo       (501) staff       (20)      229 2023-10-26 21:35:23.253926 trufflehog3-3.0.8/setup.cfg
--rw-r--r--   0 ekzo       (501) staff       (20)      791 2021-08-09 06:55:14.000000 trufflehog3-3.0.8/setup.py
-drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2023-10-26 21:35:23.252398 trufflehog3-3.0.8/trufflehog3/
--rw-r--r--   0 ekzo       (501) staff       (20)     1559 2023-10-26 21:32:44.000000 trufflehog3-3.0.8/trufflehog3/__init__.py
--rw-r--r--   0 ekzo       (501) staff       (20)      210 2021-08-06 20:47:15.000000 trufflehog3-3.0.8/trufflehog3/__main__.py
--rwxr-xr-x   0 ekzo       (501) staff       (20)     8559 2021-12-08 21:56:24.000000 trufflehog3-3.0.8/trufflehog3/cli.py
--rw-r--r--   0 ekzo       (501) staff       (20)     8414 2021-08-12 11:54:21.000000 trufflehog3-3.0.8/trufflehog3/core.py
--rw-r--r--   0 ekzo       (501) staff       (20)     4151 2021-08-06 20:47:15.000000 trufflehog3-3.0.8/trufflehog3/helper.py
--rw-r--r--   0 ekzo       (501) staff       (20)    15165 2021-08-07 14:45:16.000000 trufflehog3-3.0.8/trufflehog3/models.py
--rw-r--r--   0 ekzo       (501) staff       (20)     3765 2021-08-06 20:47:15.000000 trufflehog3-3.0.8/trufflehog3/render.py
--rw-r--r--   0 ekzo       (501) staff       (20)     6187 2021-08-06 20:47:15.000000 trufflehog3-3.0.8/trufflehog3/search.py
--rw-r--r--   0 ekzo       (501) staff       (20)     7413 2021-11-04 17:17:22.000000 trufflehog3-3.0.8/trufflehog3/source.py
-drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2023-10-26 21:35:23.253570 trufflehog3-3.0.8/trufflehog3/static/
--rw-r--r--   0 ekzo       (501) staff       (20)    18591 2021-08-06 20:47:15.000000 trufflehog3-3.0.8/trufflehog3/static/report.html.j2
--rw-r--r--   0 ekzo       (501) staff       (20)      960 2021-08-06 20:47:15.000000 trufflehog3-3.0.8/trufflehog3/static/report.text.j2
--rw-r--r--   0 ekzo       (501) staff       (20)     4195 2021-08-09 06:55:14.000000 trufflehog3-3.0.8/trufflehog3/static/rules.yml
-drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2023-10-26 21:35:23.252974 trufflehog3-3.0.8/trufflehog3.egg-info/
--rw-r--r--   0 ekzo       (501) staff       (20)     3918 2023-10-26 21:35:23.000000 trufflehog3-3.0.8/trufflehog3.egg-info/PKG-INFO
--rw-r--r--   0 ekzo       (501) staff       (20)      554 2023-10-26 21:35:23.000000 trufflehog3-3.0.8/trufflehog3.egg-info/SOURCES.txt
--rw-r--r--   0 ekzo       (501) staff       (20)        1 2023-10-26 21:35:23.000000 trufflehog3-3.0.8/trufflehog3.egg-info/dependency_links.txt
--rw-r--r--   0 ekzo       (501) staff       (20)       52 2023-10-26 21:35:23.000000 trufflehog3-3.0.8/trufflehog3.egg-info/entry_points.txt
--rw-r--r--   0 ekzo       (501) staff       (20)       60 2023-10-26 21:35:23.000000 trufflehog3-3.0.8/trufflehog3.egg-info/requires.txt
--rw-r--r--   0 ekzo       (501) staff       (20)       12 2023-10-26 21:35:23.000000 trufflehog3-3.0.8/trufflehog3.egg-info/top_level.txt
+drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2024-01-27 20:47:14.896305 trufflehog3-3.0.9/
+-rw-r--r--   0 ekzo       (501) staff       (20)    18046 2021-08-06 20:47:08.000000 trufflehog3-3.0.9/LICENSE
+-rw-r--r--   0 ekzo       (501) staff       (20)       29 2021-08-06 20:47:15.000000 trufflehog3-3.0.9/MANIFEST.in
+-rw-r--r--   0 ekzo       (501) staff       (20)     3918 2024-01-27 20:47:14.896395 trufflehog3-3.0.9/PKG-INFO
+-rw-r--r--   0 ekzo       (501) staff       (20)     3615 2023-07-18 16:35:02.000000 trufflehog3-3.0.9/README.md
+-rw-r--r--   0 ekzo       (501) staff       (20)      229 2024-01-27 20:47:14.896621 trufflehog3-3.0.9/setup.cfg
+-rw-r--r--   0 ekzo       (501) staff       (20)      791 2021-08-09 06:55:14.000000 trufflehog3-3.0.9/setup.py
+drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2024-01-27 20:47:14.895117 trufflehog3-3.0.9/trufflehog3/
+-rw-r--r--   0 ekzo       (501) staff       (20)     1559 2024-01-27 20:43:34.000000 trufflehog3-3.0.9/trufflehog3/__init__.py
+-rw-r--r--   0 ekzo       (501) staff       (20)      210 2021-08-06 20:47:15.000000 trufflehog3-3.0.9/trufflehog3/__main__.py
+-rwxr-xr-x   0 ekzo       (501) staff       (20)     8559 2021-12-08 21:56:24.000000 trufflehog3-3.0.9/trufflehog3/cli.py
+-rw-r--r--   0 ekzo       (501) staff       (20)     8414 2021-08-12 11:54:21.000000 trufflehog3-3.0.9/trufflehog3/core.py
+-rw-r--r--   0 ekzo       (501) staff       (20)     4151 2021-08-06 20:47:15.000000 trufflehog3-3.0.9/trufflehog3/helper.py
+-rw-r--r--   0 ekzo       (501) staff       (20)    15165 2021-08-07 14:45:16.000000 trufflehog3-3.0.9/trufflehog3/models.py
+-rw-r--r--   0 ekzo       (501) staff       (20)     3765 2021-08-06 20:47:15.000000 trufflehog3-3.0.9/trufflehog3/render.py
+-rw-r--r--   0 ekzo       (501) staff       (20)     6187 2021-08-06 20:47:15.000000 trufflehog3-3.0.9/trufflehog3/search.py
+-rw-r--r--   0 ekzo       (501) staff       (20)     7413 2021-11-04 17:17:22.000000 trufflehog3-3.0.9/trufflehog3/source.py
+drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2024-01-27 20:47:14.896189 trufflehog3-3.0.9/trufflehog3/static/
+-rw-r--r--   0 ekzo       (501) staff       (20)    18591 2021-08-06 20:47:15.000000 trufflehog3-3.0.9/trufflehog3/static/report.html.j2
+-rw-r--r--   0 ekzo       (501) staff       (20)      960 2021-08-06 20:47:15.000000 trufflehog3-3.0.9/trufflehog3/static/report.text.j2
+-rw-r--r--   0 ekzo       (501) staff       (20)     4195 2021-08-09 06:55:14.000000 trufflehog3-3.0.9/trufflehog3/static/rules.yml
+drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2024-01-27 20:47:14.895770 trufflehog3-3.0.9/trufflehog3.egg-info/
+-rw-r--r--   0 ekzo       (501) staff       (20)     3918 2024-01-27 20:47:14.000000 trufflehog3-3.0.9/trufflehog3.egg-info/PKG-INFO
+-rw-r--r--   0 ekzo       (501) staff       (20)      554 2024-01-27 20:47:14.000000 trufflehog3-3.0.9/trufflehog3.egg-info/SOURCES.txt
+-rw-r--r--   0 ekzo       (501) staff       (20)        1 2024-01-27 20:47:14.000000 trufflehog3-3.0.9/trufflehog3.egg-info/dependency_links.txt
+-rw-r--r--   0 ekzo       (501) staff       (20)       52 2024-01-27 20:47:14.000000 trufflehog3-3.0.9/trufflehog3.egg-info/entry_points.txt
+-rw-r--r--   0 ekzo       (501) staff       (20)       60 2024-01-27 20:47:14.000000 trufflehog3-3.0.9/trufflehog3.egg-info/requires.txt
+-rw-r--r--   0 ekzo       (501) staff       (20)       12 2024-01-27 20:47:14.000000 trufflehog3-3.0.9/trufflehog3.egg-info/top_level.txt
```

### Comparing `trufflehog3-3.0.8/LICENSE` & `trufflehog3-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.8/PKG-INFO` & `trufflehog3-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trufflehog3
-Version: 3.0.8
+Version: 3.0.9
 Summary: Find secrets in your codebase
 Home-page: https://github.com/feeltheajf/trufflehog3
 Author: Ilya Radostev
 Author-email: feeltheajf@gmail.com
 License: GNU
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trufflehog3 Version: 3.0.8 Summary: Find secrets in
+Metadata-Version: 2.1 Name: trufflehog3 Version: 3.0.9 Summary: Find secrets in
 your codebase Home-page: https://github.com/feeltheajf/trufflehog3 Author: Ilya
 Radostev Author-email: feeltheajf@gmail.com License: GNU Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE [![Package
 Version](https://img.shields.io/pypi/v/trufflehog3.svg)](https://pypi.org/
 project/trufflehog3) ![Python Version](https://img.shields.io/badge/python-3.7-
 informational.svg) [![Downloads](https://pepy.tech/badge/trufflehog3)](https://
 pepy.tech/project/trufflehog3) [![Tests](https://github.com/feeltheajf/
```

### Comparing `trufflehog3-3.0.8/README.md` & `trufflehog3-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.8/setup.py` & `trufflehog3-3.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.8/trufflehog3/__init__.py` & `trufflehog3-3.0.9/trufflehog3/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 
 from pathlib import Path
 
 from trufflehog3 import helper
 
 __NAME__ = "trufflehog3"
-__VERSION__ = "3.0.8"
+__VERSION__ = "3.0.9"
 
 HERE = Path(__file__).parent
 STATIC_DIR = HERE / "static"
 HTML_TEMPLATE_FILE = "report.html.j2"
 TEXT_TEMPLATE_FILE = "report.text.j2"
 DEFAULT_RULES_FILE = STATIC_DIR / "rules.yml"
```

### Comparing `trufflehog3-3.0.8/trufflehog3/cli.py` & `trufflehog3-3.0.9/trufflehog3/cli.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.8/trufflehog3/core.py` & `trufflehog3-3.0.9/trufflehog3/core.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.8/trufflehog3/helper.py` & `trufflehog3-3.0.9/trufflehog3/helper.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.8/trufflehog3/models.py` & `trufflehog3-3.0.9/trufflehog3/models.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.8/trufflehog3/render.py` & `trufflehog3-3.0.9/trufflehog3/render.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.8/trufflehog3/search.py` & `trufflehog3-3.0.9/trufflehog3/search.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.8/trufflehog3/source.py` & `trufflehog3-3.0.9/trufflehog3/source.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.8/trufflehog3/static/report.html.j2` & `trufflehog3-3.0.9/trufflehog3/static/report.html.j2`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.8/trufflehog3/static/report.text.j2` & `trufflehog3-3.0.9/trufflehog3/static/report.text.j2`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.8/trufflehog3/static/rules.yml` & `trufflehog3-3.0.9/trufflehog3/static/rules.yml`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.8/trufflehog3.egg-info/PKG-INFO` & `trufflehog3-3.0.9/trufflehog3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trufflehog3
-Version: 3.0.8
+Version: 3.0.9
 Summary: Find secrets in your codebase
 Home-page: https://github.com/feeltheajf/trufflehog3
 Author: Ilya Radostev
 Author-email: feeltheajf@gmail.com
 License: GNU
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trufflehog3 Version: 3.0.8 Summary: Find secrets in
+Metadata-Version: 2.1 Name: trufflehog3 Version: 3.0.9 Summary: Find secrets in
 your codebase Home-page: https://github.com/feeltheajf/trufflehog3 Author: Ilya
 Radostev Author-email: feeltheajf@gmail.com License: GNU Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE [![Package
 Version](https://img.shields.io/pypi/v/trufflehog3.svg)](https://pypi.org/
 project/trufflehog3) ![Python Version](https://img.shields.io/badge/python-3.7-
 informational.svg) [![Downloads](https://pepy.tech/badge/trufflehog3)](https://
 pepy.tech/project/trufflehog3) [![Tests](https://github.com/feeltheajf/
```

### Comparing `trufflehog3-3.0.8/trufflehog3.egg-info/SOURCES.txt` & `trufflehog3-3.0.9/trufflehog3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

