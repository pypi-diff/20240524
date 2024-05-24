# Comparing `tmp/wuthery_l10n-0.1.0.tar.gz` & `tmp/wuthery_l10n-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wuthery_l10n-0.1.0.tar", max compression
+gzip compressed data, was "wuthery_l10n-0.2.0.tar", max compression
```

## Comparing `wuthery_l10n-0.1.0.tar` & `wuthery_l10n-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35823 2024-05-23 07:27:52.520136 wuthery_l10n-0.1.0/LICENSE
--rw-r--r--   0        0        0     1798 2024-05-23 08:46:32.142571 wuthery_l10n-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      741 2024-05-23 08:53:58.536864 wuthery_l10n-0.1.0/README.md
--rw-r--r--   0        0        0      149 2024-05-23 08:49:39.629718 wuthery_l10n-0.1.0/wuthery/l10n/__init__.py
--rw-r--r--   0        0        0      318 2024-05-23 08:48:44.223851 wuthery_l10n-0.1.0/wuthery/l10n/enums.py
--rw-r--r--   0        0        0     3950 2024-05-23 08:29:54.196329 wuthery_l10n-0.1.0/wuthery/l10n/translator.py
--rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 wuthery_l10n-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-05-23 07:27:52.520136 wuthery_l10n-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1798 2024-05-23 11:49:10.397210 wuthery_l10n-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      741 2024-05-23 08:53:58.536864 wuthery_l10n-0.2.0/README.md
+-rw-r--r--   0        0        0      149 2024-05-23 08:49:39.629718 wuthery_l10n-0.2.0/wuthery/l10n/__init__.py
+-rw-r--r--   0        0        0      318 2024-05-23 08:48:44.223851 wuthery_l10n-0.2.0/wuthery/l10n/enums.py
+-rw-r--r--   0        0        0     3950 2024-05-23 08:29:54.196329 wuthery_l10n-0.2.0/wuthery/l10n/translator.py
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 wuthery_l10n-0.2.0/PKG-INFO
```

### Comparing `wuthery_l10n-0.1.0/LICENSE` & `wuthery_l10n-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wuthery_l10n-0.1.0/pyproject.toml` & `wuthery_l10n-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [tool.poetry]
 authors = ["seria <seria.ati@gmail.com>"]
 description = "Python package to interact with Wuthery's localization files."
 license = "GPL-3.0"
 name = "wuthery-l10n"
 packages = [{include = "wuthery"}]
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 aiofiles = "^23.2.1"
 aiohttp = "^3.9.5"
 python = "^3.11"
 pyyaml = "^6.0.1"
```

### Comparing `wuthery_l10n-0.1.0/README.md` & `wuthery_l10n-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wuthery_l10n-0.1.0/wuthery/l10n/translator.py` & `wuthery_l10n-0.2.0/wuthery/l10n/translator.py`

 * *Files identical despite different names*

### Comparing `wuthery_l10n-0.1.0/PKG-INFO` & `wuthery_l10n-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wuthery-l10n
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package to interact with Wuthery's localization files.
 License: GPL-3.0
 Author: seria
 Author-email: seria.ati@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

