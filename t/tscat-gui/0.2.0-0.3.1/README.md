# Comparing `tmp/tscat_gui-0.2.0.tar.gz` & `tmp/tscat_gui-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tscat_gui-0.2.0.tar", last modified: Tue Nov 29 22:58:41 2022, max compression
+gzip compressed data, was "tscat_gui-0.3.1.tar", last modified: Fri May 24 15:16:50 2024, max compression
```

## Comparing `tscat_gui-0.2.0.tar` & `tscat_gui-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4891 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      426 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/tscat_gui/
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tscat_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tscat_gui/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tscat_gui/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tscat_gui/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20597 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tscat_gui/predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tscat_gui/state.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tscat_gui/tscat_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tscat_gui/undo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/tscat_gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tscat_gui/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tscat_gui/utils/editable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tscat_gui/utils/flow_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tscat_gui/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2022-11-29 22:58:33.000000 tscat_gui-0.2.0/tscat_gui/utils/keyword_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/tscat_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/tscat_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/tscat_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/tscat_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/tscat_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/tscat_gui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/tscat_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-11-29 22:58:41.000000 tscat_gui-0.2.0/tscat_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.252851 tscat_gui-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-24 15:16:50.252851 tscat_gui-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.248851 tscat_gui-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4891 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-24 15:16:50.256851 tscat_gui-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.248851 tscat_gui-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tests/test_mypy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.252851 tscat_gui-0.3.1/tscat_gui/
+-rw-r--r--   0 runner    (1001) docker     (127)    23012 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21591 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.252851 tscat_gui-0.3.1/tscat_gui/tscat_driver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/catalog_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_driver/tscat_root_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/tscat_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12569 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/undo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.252851 tscat_gui-0.3.1/tscat_gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/utils/editable_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/utils/flow_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-24 15:16:42.000000 tscat_gui-0.3.1/tscat_gui/utils/keyword_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:16:50.252851 tscat_gui-0.3.1/tscat_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 15:16:50.000000 tscat_gui-0.3.1/tscat_gui.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tscat_gui-0.2.0/CONTRIBUTING.rst` & `tscat_gui-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.2.0/LICENSE` & `tscat_gui-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.2.0/PKG-INFO` & `tscat_gui-0.3.1/tscat_gui.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,69 @@
-Metadata-Version: 1.2
-Name: tscat_gui
-Version: 0.2.0
+Metadata-Version: 2.1
+Name: tscat-gui
+Version: 0.3.1
 Summary: Time-series catalogue - graphical user interface library
 Home-page: https://github.com/SciQLop/tscat_gui
 Author: Patrick Boettcher
 Author-email: p@yai.se
 License: GNU General Public License v3
-Description: ===========================
-        Time series catalogue - GUI
-        ===========================
-        
-        
-        .. image:: https://img.shields.io/pypi/v/tscat_gui.svg
-                :target: https://pypi.python.org/pypi/tscat_gui
-        
-        .. image:: https://img.shields.io/travis/SciQLop/tscat_gui.svg
-                :target: https://travis-ci.com/SciQLop/tscat_gui
-        
-        .. image:: https://readthedocs.org/projects/tscat-gui/badge/?version=latest
-                :target: https://tscat-gui.readthedocs.io/en/latest/?version=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        Time-series catalogue - graphical user interface library
-        
-        
-        * Free software: GNU General Public License v3
-        * Documentation: https://tscat-gui.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2021-11-04)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: tscat_gui
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+===========================
+Time series catalogue - GUI
+===========================
+
+
+.. image:: https://img.shields.io/pypi/v/tscat_gui.svg
+        :target: https://pypi.python.org/pypi/tscat_gui
+
+.. image:: https://img.shields.io/travis/SciQLop/tscat_gui.svg
+        :target: https://travis-ci.com/SciQLop/tscat_gui
+
+.. image:: https://readthedocs.org/projects/tscat-gui/badge/?version=latest
+        :target: https://tscat-gui.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+
+
+
+Time-series catalogue - graphical user interface library
+
+
+* Free software: GNU General Public License v3
+* Documentation: https://tscat-gui.readthedocs.io.
+
+
+Features
+--------
+
+* TODO
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.1.0 (2021-11-04)
+------------------
+
+* First release on PyPI.
```

### Comparing `tscat_gui-0.2.0/README.rst` & `tscat_gui-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.2.0/docs/Makefile` & `tscat_gui-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.2.0/docs/conf.py` & `tscat_gui-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.2.0/docs/installation.rst` & `tscat_gui-0.3.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.2.0/docs/make.bat` & `tscat_gui-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.2.0/setup.py` & `tscat_gui-0.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,46 +8,46 @@
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = [
     'PySide6',
-    'tscat',
+    'tscat==0.3.*',
 ]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Patrick Boettcher",
     author_email='p@yai.se',
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     description="Time-series catalogue - graphical user interface library",
     entry_points={
         'console_scripts': [
-            'tscat_gui=tscat_gui.cli:main',
+            'tscat_gui=tscat_gui.app:main',
         ],
     },
     install_requires=requirements,
     license="GNU General Public License v3",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='tscat_gui',
     name='tscat_gui',
     packages=find_packages(include=['tscat_gui', 'tscat_gui.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/SciQLop/tscat_gui',
-    version='0.2.0',
-    zip_safe=False,
+    version='0.3.1',
+    zip_safe=False
 )
```

### Comparing `tscat_gui-0.2.0/tscat_gui/__init__.py` & `tscat_gui-0.3.1/tscat_gui/edit.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,387 +1,490 @@
-"""Top-level package for Time series catalogue - GUI."""
+import datetime as dt
+import functools
+from typing import Union, Dict, Optional, List, Type, cast, Any, Callable
+
+import tscat
+import tscat.filtering
+from PySide6 import QtCore, QtWidgets
 
-__author__ = """Patrick Boettcher"""
-__email__ = 'p@yai.se'
-__version__ = '0.2.0'
+from .metadata import catalogue_meta_data
+from .predicate import SimplePredicateEditDialog
+from .state import AppState
+from .tscat_driver.actions import Action, GetCatalogueAction, SetAttributeAction
+from .undo import NewAttribute, RenameAttribute, DeleteAttributeAction, SetAttributeValue, DeleteAttribute
+from .utils.editable_label import EditableLabel
+from .utils.helper import AttributeNameValidator, IntDelegate, FloatDelegate, \
+    DateTimeDelegate, StrDelegate, BoolDelegate
+from .utils.keyword_list import EditableKeywordListWidget
 
-from PySide6 import QtWidgets, QtGui
-from PySide6 import QtCore
 
-from typing import Union
-import datetime as dt
-from pathlib import Path
-import os
+class _UuidLabelDelegate(QtWidgets.QWidget):
+    editingFinished = QtCore.Signal()  # never emitted
 
-import tscat
+    def __init__(self, value: str, parent: Optional[QtWidgets.QWidget] = None):
+        super().__init__(parent)
 
-from .model import CatalogueModel, EventModel, UUIDRole
+        label = QtWidgets.QLabel(value, self)
+        label.setTextInteractionFlags(QtCore.Qt.TextSelectableByMouse)  # type: ignore
+        layout = QtWidgets.QHBoxLayout(self)
+        layout.addWidget(label)
+        layout.addStretch()
+        layout.setContentsMargins(0, 0, 0, 0)
+        self.setLayout(layout)
 
-from .edit import EntityEditView
-from .state import AppState
 
-from .undo import NewCatalogue, MoveEntityToTrash, RestoreEntityFromTrash, DeletePermanently, NewEvent, Import
+class _ReadOnlyString(str):
+    pass
 
-from .utils.helper import get_entity_from_uuid_safe
 
+class _PredicateDelegate(QtWidgets.QWidget):
+    editingFinished = QtCore.Signal()
 
-class _TrashAlwaysTopOrBottomSortFilterModel(QtCore.QSortFilterProxyModel):
-    def __init__(self, parent=None):
+    def __init__(self, value: Optional[tscat.filtering.Predicate], parent: Optional[QtWidgets.QWidget] = None):
         super().__init__(parent)
 
-    def lessThan(self, source_left: Union[QtCore.QModelIndex, QtCore.QPersistentModelIndex],
-                 source_right: Union[QtCore.QModelIndex, QtCore.QPersistentModelIndex]) -> bool:
-        left = self.sourceModel().data(source_left)
-        right = self.sourceModel().data(source_right)
-
-        if left == 'Trash':
-            return False
-        elif right == 'Trash':
-            return True
-        else:
-            return left.lower() < right.lower()
+        self.predicate = value
 
+        layout = QtWidgets.QHBoxLayout()
+        layout.setContentsMargins(0, 0, 0, 0)
 
-class TSCatGUI(QtWidgets.QWidget):
-    event_selected = QtCore.Signal(str)
-    catalogue_selected = QtCore.Signal(str)
-    event_changed = QtCore.Signal(str)
-    catalogue_changed = QtCore.Signal(str)
+        value_str = str(value)
+        if len(value_str) > 50:
+            value_str = value_str[:50] + '...'
+        self.label = QtWidgets.QLabel(value_str)
+        layout.addWidget(self.label)
+
+        button = QtWidgets.QPushButton("Edit")
+        button.clicked.connect(self.edit_predicate)  # type: ignore
+        layout.addWidget(button)
+
+        button = QtWidgets.QPushButton("Clear")
+        button.clicked.connect(self.clear_predicate)  # type: ignore
+        layout.addWidget(button)
+        layout.addStretch()
 
-    def __init__(self, parent=None):
+        self.setLayout(layout)
+
+    def edit_predicate(self):
+        dialog = SimplePredicateEditDialog(self.predicate, self)
+        result = dialog.exec_()
+        if result == QtWidgets.QDialog.Accepted:
+            self.predicate = dialog.predicate
+            self.editingFinished.emit()
+
+    def clear_predicate(self):
+        self.predicate = None
+        self.editingFinished.emit()
+
+    def value(self) -> Union[tscat.filtering.Predicate, None]:
+        return self.predicate
+
+
+class _MultipleDifferentValues(list):
+    def __init__(self, attribute: str, *args: List) -> None:
+        super().__init__(*args)
+        self.attribute = attribute
+
+
+class _RatingDelegate(QtWidgets.QWidget):
+    editingFinished = QtCore.Signal()
+
+    def __init__(self, value: Optional[int], parent: Optional[QtWidgets.QWidget] = None):
         super().__init__(parent)
 
-        self.state = AppState()
+        self.label = QtWidgets.QLabel(self)
+        self.slider = QtWidgets.QSlider(self)
+        self.slider.setOrientation(QtCore.Qt.Horizontal)  # type: ignore
+        self.slider.setRange(0, 10)
+        self.slider.setTickInterval(1)
+        self.slider.setTickPosition(QtWidgets.QSlider.TicksBelow)  # type: ignore
+        self.slider.valueChanged.connect(self._slider_value_changed)  # type: ignore
+        self.slider.sliderReleased.connect(lambda: self.editingFinished.emit())  # type: ignore
+
+        if value:
+            self.label.setText(str(value))
+            self.slider.setValue(value)
+        else:
+            self.label.setText(" ")
+            self.slider.setValue(0)
+
+        layout = QtWidgets.QHBoxLayout(self)
+        layout.addWidget(self.slider)
+        layout.addWidget(self.label)
+        layout.addStretch()
+        layout.setContentsMargins(0, 0, 0, 0)
+        self.setLayout(layout)
 
-        self.state.state_changed.connect(self._external_signal_emission)
+    def _slider_value_changed(self, value: int) -> None:
+        if value == 0:
+            self.label.setText(" ")
+        else:
+            self.label.setText(str(value))
 
-        self.events_model = EventModel(self.state, self)
-        self.events_sort_model = QtCore.QSortFilterProxyModel()
-        self.events_sort_model.setSourceModel(self.events_model)
-
-        self.events_view = QtWidgets.QTableView()
-        self.events_view.setMinimumSize(1000, 500)
-        self.events_view.setSortingEnabled(True)
-        self.events_view.sortByColumn(0, QtCore.Qt.SortOrder.AscendingOrder)
-
-        self.events_view.setModel(self.events_sort_model)
-        self.events_view.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectionBehavior.SelectRows)
-        self.events_view.setSelectionMode(QtWidgets.QAbstractItemView.SingleSelection)
-
-        self.programmatic_select = False
-
-        def current_event_changed(selected: QtCore.QModelIndex, deselected: QtCore.QModelIndex):
-            if self.programmatic_select:
-                return
-            if selected.isValid():
-                if not deselected.isValid() or deselected.row() != selected.row():
-                    uuid = self.events_sort_model.data(selected, UUIDRole)
-                    self.state.updated('active_select', tscat._Event, uuid)
-            else:
-                self.state.updated('active_select', tscat._Event, None)
+    def value(self) -> Any:
+        if self.slider.value() == 0:
+            return None
+        else:
+            return self.slider.value()
 
-        self.events_view.selectionModel().currentChanged.connect(current_event_changed,
-                                                                 type=QtCore.Qt.DirectConnection)
 
-        self.edit_view = EntityEditView(self.state, self)
+_delegate_widget_class_factory = {
+    'uuid': _UuidLabelDelegate,
+    'predicate': _PredicateDelegate,
+    'rating': _RatingDelegate,
 
-        self.splitter_right = QtWidgets.QSplitter(QtCore.Qt.Vertical, self)
-        self.splitter_right.addWidget(self.events_view)
-        self.splitter_right.addWidget(self.edit_view)
+    _ReadOnlyString: _UuidLabelDelegate,
+    int: IntDelegate,
+    str: StrDelegate,
+    float: FloatDelegate,
+    list: EditableKeywordListWidget,
+    bool: BoolDelegate,
+    dt.datetime: DateTimeDelegate,
+}
 
-        self.catalogue_model = CatalogueModel(self)
 
-        self.catalogues_view = QtWidgets.QTreeView()
-        self.catalogues_view.setMinimumSize(300, 900)
-        self.catalogues_view.setSelectionMode(QtWidgets.QAbstractItemView.ExtendedSelection)
+class _MultipleDifferentValuesDelegate(QtWidgets.QPushButton):
+    editingFinished = QtCore.Signal()
 
-        self.catalogue_sort_filter_model = _TrashAlwaysTopOrBottomSortFilterModel()
-        self.catalogue_sort_filter_model.setSourceModel(self.catalogue_model)
-        self.catalogue_sort_filter_model.setRecursiveFilteringEnabled(True)
-        self.catalogue_sort_filter_model.setFilterCaseSensitivity(QtCore.Qt.CaseSensitivity.CaseInsensitive)
+    def __init__(self,
+                 values: _MultipleDifferentValues,
+                 reset_value_selection: Callable[[List[Any]], Any] = lambda x: x[0],
+                 parent: Optional[QtWidgets.QWidget] = None):
+        super().__init__('<multiple-values-click-to-reset>', parent)
+        assert len(values) > 0
 
-        self.catalogues_view.setModel(self.catalogue_sort_filter_model)
-        self.catalogues_view.setSortingEnabled(True)
-        self.catalogues_view.sortByColumn(0, QtCore.Qt.SortOrder.AscendingOrder)
+        self.reset_value = reset_value_selection(values)
 
-        self.catalogues_view.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
+        self.clicked.connect(lambda x: self.editingFinished.emit())  # type: ignore
 
-        def current_catalogue_activated(index: QtCore.QModelIndex) -> None:
-            if self.programmatic_select:
-                return
+    def value(self) -> Any:
+        return self.reset_value
 
-            if index.isValid():
-                uuid = self.catalogue_sort_filter_model.data(index, UUIDRole)
-                self.state.updated('active_select', tscat._Catalogue, uuid)
-            else:
-                self.state.updated('active_select', tscat._Catalogue, None)
 
-        def current_catalogue_changed(selected: QtCore.QModelIndex, deselected: QtCore.QModelIndex):
-            current_catalogue_activated(selected)
+class _MultipleDifferentValuesDelegateMin(_MultipleDifferentValuesDelegate):
+    def __init__(self,
+                 values: _MultipleDifferentValues,
+                 parent: Optional[QtWidgets.QWidget] = None):
+        super().__init__(values, min, parent)
+
+
+class _MultipleDifferentValuesDelegateMax(_MultipleDifferentValuesDelegate):
+    def __init__(self,
+                 values: _MultipleDifferentValues,
+                 parent: Optional[QtWidgets.QWidget] = None):
+        super().__init__(values, max, parent)
+
+
+_type_name = {
+    'Boolean': bool,
+    'DateTime': dt.datetime,
+    'Float': float,
+    'Integer': int,
+    'String': str,
+    'Word List': list,
+}
+
+_type_name_initial_value = {
+    'DateTime': lambda: dt.datetime.now()
+}
+
 
+class AttributesGroupBox(QtWidgets.QGroupBox):
+    valuesChanged = QtCore.Signal()
 
-        self.catalogues_view.selectionModel().currentChanged.connect(current_catalogue_changed,
-                                                                     type=QtCore.Qt.DirectConnection)
-        self.catalogues_view.clicked.connect(current_catalogue_activated)
+    def create_label(self, text: str) -> QtWidgets.QLabel:  # type: ignore
+        return QtWidgets.QLabel(text.title())
 
-        self.catalogues_view.setSelectionMode(QtWidgets.QAbstractItemView.SelectionMode.SingleSelection)
+    def __init__(self, title: str,
+                 state: AppState,
+                 parent: Optional[QtWidgets.QWidget] = None) -> None:
+        super().__init__(title, parent)
 
-        def state_changed(action, type, uuid):
-            if action in ['changed', 'moved', 'inserted', 'deleted', 'active_select', 'passive_select']:
-                if type == tscat._Catalogue:
-                    if action not in ['active_select', 'passive_select']:
-                        self.catalogue_model.reset()
+        self.attribute_name_labels: Dict[str, QtWidgets.QLabel] = {}
+        self.state = state
+        self.values: Dict = {}
 
-                    index = self.catalogue_model.index_from_uuid(uuid)
-                    index = self.catalogue_sort_filter_model.mapFromSource(index)
-                    self.programmatic_select = True
-                    self.catalogues_view.setCurrentIndex(index)
-                    self.programmatic_select = False
+        self._layout = QtWidgets.QGridLayout()
+        self._layout.setContentsMargins(0, 0, 0, 0)
+        self.setLayout(self._layout)
+
+    def setup_values(self, values: Dict):
+        # clear layout, destroy all widgets
+        while True:
+            item = self._layout.takeAt(0)
+            if item:
+                item.widget().deleteLater()
+            else:
+                break
+
+        self.values = values
+        self.attribute_name_labels = {}
+        for row, attr in enumerate(values.keys()):
+            label = self.create_label(attr)
+            self._layout.addWidget(label, row, 0)
+
+            self.attribute_name_labels[attr] = label
+
+            value = values[attr]
+
+            cls: Type[Union[_MultipleDifferentValuesDelegate, _UuidLabelDelegate, _PredicateDelegate,
+            IntDelegate, StrDelegate, FloatDelegate,
+            EditableKeywordListWidget, BoolDelegate, DateTimeDelegate]]
+
+            if isinstance(value, _MultipleDifferentValues):
+                if attr == 'start':
+                    cls = _MultipleDifferentValuesDelegateMin
+                elif attr == 'stop':
+                    cls = _MultipleDifferentValuesDelegateMax
                 else:
-                    if action not in ['active_select', 'passive_select']:
-                        self.events_model.reset()
-                    index = self.events_model.index_from_uuid(uuid)
-                    index = self.events_sort_model.mapFromSource(index)
-                    self.programmatic_select = True
-                    self.events_view.setCurrentIndex(index)
-                    self.programmatic_select = False
-
-            if action == 'active_select':
-                self.move_to_trash_action.setEnabled(False)
-                self.restore_from_trash_action.setEnabled(False)
-                self.delete_action.setEnabled(False)
-                self.new_event_action.setEnabled(False)
-                self.export_action.setEnabled(False)
-
-                if uuid:
-                    entity = get_entity_from_uuid_safe(uuid)
-                    if entity.is_removed():
-                        self.restore_from_trash_action.setEnabled(True)
-                    else:
-                        self.move_to_trash_action.setEnabled(True)
-                    self.delete_action.setEnabled(True)
-                    self.new_event_action.setEnabled(True)
-                    self.export_action.setEnabled(True)
-
-        self.state.state_changed.connect(state_changed)
-
-        hlayout = QtWidgets.QHBoxLayout()
-        hlayout.setContentsMargins(0, 0, 0, 0)
-        hlayout.addWidget(QtWidgets.QLabel('Filter:'))
-        catalogue_filter = QtWidgets.QLineEdit()
-        catalogue_filter.textChanged.connect(lambda t: self.catalogue_sort_filter_model.setFilterRegularExpression(t))
+                    cls = _MultipleDifferentValuesDelegate
+            elif attr in _delegate_widget_class_factory:
+                cls = _delegate_widget_class_factory[attr]
+            else:
+                cls = _delegate_widget_class_factory.get(type(value), QtWidgets.QLabel)
 
-        hlayout.addWidget(catalogue_filter)
+            widget = cls(value, parent=self)
 
-        layout = QtWidgets.QVBoxLayout()
-        layout.setContentsMargins(0, 0, 0, 0)
-        layout.addLayout(hlayout)
-        layout.addWidget(self.catalogues_view)
+            # special case for UUIDs - read-only
+            if attr == 'uuid':
+                widget.setEnabled(False)
+            else:
+                # the editingFinished-signal is not seen by mypy coming from PySide6
+                widget.editingFinished.connect(  # type: ignore
+                    functools.partial(self._edit_finished_on_widget, widget, attr))  # type: ignore
+            self._layout.addWidget(widget, row, 1)
+
+    def _edit_finished_on_widget(self, w: QtWidgets.QWidget, a: str) -> None:
+
+        assert isinstance(w, (_MultipleDifferentValuesDelegate, _PredicateDelegate, _RatingDelegate,
+                              IntDelegate, StrDelegate, FloatDelegate,
+                              EditableKeywordListWidget, BoolDelegate, DateTimeDelegate))
+
+        self._editing_finished(a, w.value())
+
+    def _editing_finished(self, attr, value) -> None:
+        if value != self.values[attr]:
+            self.state.push_undo_command(SetAttributeValue, attr, value)
+            self.valuesChanged.emit()
+            self.values[attr] = value
+
+
+class FixedAttributesGroupBox(AttributesGroupBox):
+    def __init__(self,
+                 state: AppState,
+                 parent: Optional[QtWidgets.QWidget] = None):
+        super().__init__("Global", state, parent)
+
+    def setup(self, entities: List[Union[tscat._Catalogue, tscat._Event]]) -> None:
+        values: Dict[str, Any] = {}
+
+        for entity in entities:
+            for attr in entity.fixed_attributes().keys():
+                value = entity.__dict__[attr]
+                if attr in values:
+                    if isinstance(values[attr], _MultipleDifferentValues):
+                        values[attr].append(value)
+                    elif values[attr] != value:
+                        values[attr] = _MultipleDifferentValues(attr, [values[attr], value])
+                else:
+                    values[attr] = value
 
-        left_widget = QtWidgets.QWidget()
-        left_widget.setLayout(layout)
+        super().setup_values(values)
 
-        splitter = QtWidgets.QSplitter(QtCore.Qt.Horizontal, self)
-        splitter.addWidget(left_widget)
-        splitter.addWidget(self.splitter_right)
 
-        layout = QtWidgets.QVBoxLayout()
-        layout.setContentsMargins(0, 0, 0, 0)
+class CustomAttributesGroupBox(AttributesGroupBox):
+
+    def create_label(self, text: str) -> EditableLabel:  # type: ignore
+        attrs = self.all_attribute_names[:]
+        attrs.remove(text)
 
-        toolbar = QtWidgets.QToolBar()
+        name = EditableLabel(text, AttributeNameValidator(attrs))
+        name.editing_finished.connect(lambda x, _text=text: self._attribute_name_changed(_text, x))
+        name.text_changed.connect(lambda x, _text=text: self._attribute_name_is_changing(_text, x))
 
-        action = QtGui.QAction(self.style().standardIcon(QtWidgets.QStyle.SP_FileDialogNewFolder),
-                               "Create Catalogue", self)
+        return name
 
-        def new_catalogue():
-            self.state.push_undo_command(NewCatalogue)
+    def __init__(self,
+                 state: AppState,
+                 parent: Optional[QtWidgets.QWidget] = None) -> None:
+        super().__init__("Custom", state, parent)
 
-        action.triggered.connect(new_catalogue)
-        toolbar.addAction(action)
-
-        action = QtGui.QAction(self.style().standardIcon(QtWidgets.QStyle.SP_FileIcon),
-                               "Create Event", self)
-
-        def new_event():
-            self.state.push_undo_command(NewEvent)
-
-        action.triggered.connect(new_event)
-        action.setEnabled(False)
-        toolbar.addAction(action)
-
-        self.new_event_action = action
-
-        toolbar.addSeparator()
-        action = QtGui.QAction(self.style().standardIcon(QtWidgets.QStyle.SP_DialogSaveButton), "Save To Disk",
-                               self)
-
-        action.triggered.connect(self.save)
-        toolbar.addAction(action)
-        action.setEnabled(False)
-        self.state.undo_stack_clean_changed.connect(lambda state, a=action: a.setEnabled(not state))
-
-        toolbar.addSeparator()
-        undo_action, redo_action = self.state.create_undo_redo_action()
-
-        undo_action.setIcon(self.style().standardIcon(QtWidgets.QStyle.SP_ArrowBack))
-        undo_action.setShortcut(QtCore.Qt.CTRL | QtCore.Qt.Key_Z)
-        toolbar.addAction(undo_action)
-
-        redo_action.setIcon(self.style().standardIcon(QtWidgets.QStyle.SP_ArrowForward))
-        redo_action.setShortcut(QtCore.Qt.CTRL | QtCore.Qt.SHIFT | QtCore.Qt.Key_Z)
-        toolbar.addAction(redo_action)
-
-        toolbar.addSeparator()
-
-        action = QtGui.QAction(self.style().standardIcon(QtWidgets.QStyle.SP_TrashIcon), "Move to Trash", self)
-
-        def trash():
-            self.state.push_undo_command(MoveEntityToTrash)
-
-        action.triggered.connect(trash)
-        action.setEnabled(False)
-        toolbar.addAction(action)
-        self.move_to_trash_action = action
-
-        action = QtGui.QAction(self.style().standardIcon(QtWidgets.QStyle.SP_DialogResetButton),
-                               "Restore from Trash", self)
-
-        def restore():
-            self.state.push_undo_command(RestoreEntityFromTrash)
-
-        action.triggered.connect(restore)
-        action.setEnabled(False)
-        toolbar.addAction(action)
-        self.restore_from_trash_action = action
-
-        action = QtGui.QAction(self.style().standardIcon(QtWidgets.QStyle.SP_BrowserStop), "Delete permanently",
-                               self)
-
-        def delete():
-            self.state.push_undo_command(DeletePermanently)
-
-        action.triggered.connect(delete)
-        action.setEnabled(False)
-        toolbar.addAction(action)
-        self.delete_action = action
-
-        toolbar.addSeparator()
-
-        action = QtGui.QAction(self.style().standardIcon(QtWidgets.QStyle.SP_DialogRetryButton), "Refresh",
-                               self)
-
-        def refresh():
-            current_selection = self.state.select_state()
-            self.catalogue_model.reset()
-            self.events_model.reset()
-
-            if current_selection.type == tscat._Event:
-                self.state.updated('passive_select', tscat._Catalogue, current_selection.active_catalogue)
-            self.state.updated('active_select', current_selection.type, current_selection.active)
-
-        action.triggered.connect(refresh)
-        toolbar.addAction(action)
-
-        self.refresh_action = action
-
-        toolbar.addSeparator()
-
-        action = QtGui.QAction(self.style().standardIcon(QtWidgets.QStyle.SP_ArrowUp), "Import Catalogue",
-                               self)
-
-        def import_from_file():
-            filename, filetype = QtWidgets.QFileDialog.getOpenFileName(
-                self.activateWindow(),
-                "Select a catalogue file to be imported",
-                str(Path.home()),
-                "JSON Document (*.json)")
-            if filename == '':
-                return
-
-            try:
-                with open(filename) as f:
-                    data = f.read()
-                    import_dict = tscat.canonicalize_json_import(data)
-                    self.state.push_undo_command(Import, filename, import_dict)
-            except Exception as e:
-                QtWidgets.QMessageBox.critical(self.activateWindow(),
-                                               "Catalogue import",
-                                               f"The selected file could not be imported: '{e}'.")
-
-        action.triggered.connect(import_from_file)
-        toolbar.addAction(action)
-
-        action = QtGui.QAction(self.style().standardIcon(QtWidgets.QStyle.SP_ArrowDown), "Export Catalogue",
-                               self)
-
-        def export_to_file():
-            filename, filetype = QtWidgets.QFileDialog.getSaveFileName(
-                self.activateWindow(),
-                "Specify the filename for exporting the selected catalogue",
-                str(Path.home()),
-                "JSON Document (*.json)")
-            if filename == '':
-                return
-            split_filename = os.path.splitext(filename)
-            if split_filename[1] != '.json':
-                filename = split_filename[0] + '.json'
-
-            try:
-                with open(filename, 'w+') as f:
-                    catalogue = get_entity_from_uuid_safe(self.state.select_state().active_catalogue)
-                    json = tscat.export_json(catalogue)
-                    f.write(json)
-                QtWidgets.QMessageBox.information(self.activateWindow(),
-                                                  "Catalogue export",
-                                                  "The selected catalogue has been successfully exported")
-            except Exception as e:
-                QtWidgets.QMessageBox.critical(self.activateWindow(),
-                                               "Catalogue export",
-                                               f"The selected catalogue could not be exported to {filename} due to '{e}'.")
-
-        action.triggered.connect(export_to_file)
-        action.setEnabled(False)
-        toolbar.addAction(action)
+        self.all_attribute_names: List[str] = []
 
-        self.export_action = action
+    def setup(self, entities: List[Union[tscat._Catalogue, tscat._Event]]) -> None:
+        if len(entities) > 1:
+            self.hide()
+            return
+
+        self.show()
+
+        entity = entities[0]
+        self.all_attribute_names = list(entity.variable_attributes().keys()) + \
+                                   list(entity.fixed_attributes().keys())
+
+        attributes = sorted(entity.variable_attributes().keys())
+        values = {}
+        for attr in attributes:
+            values[attr] = entity.__dict__[attr]
+
+        super().setup_values(values)
+
+        layout = cast(QtWidgets.QGridLayout, self.layout())
+
+        # add a delete-button to each row
+        for row, attr in enumerate(attributes):
+            but = QtWidgets.QToolButton()
+            but.setText('✖')
+            but.clicked.connect(lambda a=attr, x=False: self._delete(a))  # type: ignore
+            layout.addWidget(but, row, 2)
+
+        # add the new-attribute-button
+        new_section_layout = QtWidgets.QHBoxLayout()
+        new_section_layout.setContentsMargins(0, 0, 0, 0)
+
+        self.type_combobox = QtWidgets.QComboBox()
+        self.type_combobox.addItems(list(_type_name.keys()))
+        new_section_layout.addWidget(self.type_combobox)
+
+        button = QtWidgets.QToolButton()
+        button.setText('➕')
+        button.clicked.connect(self._new)  # type: ignore
+        new_section_layout.addWidget(button)
+
+        new_section_layout.addStretch()
+
+        widget = QtWidgets.QWidget()
+        widget.setLayout(new_section_layout)
+
+        row = layout.rowCount()
+        layout.addWidget(QtWidgets.QLabel('New'), row, 0)
+        layout.addWidget(widget, row, 1)
+
+    def _delete(self, attr) -> None:
+        self.state.push_undo_command(DeleteAttribute, attr)
+
+    def _new(self) -> None:
+        name = 'attribute{}'
+
+        i = 1
+        while name.format(i) in self.values.keys():
+            i += 1
+
+        name = name.format(i)
+
+        type_name = self.type_combobox.itemText(self.type_combobox.currentIndex())
+        default = _type_name_initial_value.get(type_name, _type_name[type_name])()
+
+        self.state.push_undo_command(NewAttribute, name, default)
+
+    def _attribute_name_changed(self, previous: str, text: str) -> None:
+        self.state.push_undo_command(RenameAttribute, previous, text)
+
+    def _attribute_name_is_changing(self, previous: str, text: str) -> None:
+        # highlight the existing attribute which is using the same text as name
+        for label in self.attribute_name_labels.values():
+            label.setStyleSheet('background-color: none')
+
+        if text in self.attribute_name_labels and previous != text:
+            self.attribute_name_labels[text].setStyleSheet('color: red')
+
+
+class CatalogueMetaDataGroupBox(AttributesGroupBox):
+    def __init__(self,
+                 state: AppState,
+                 parent: Optional[QtWidgets.QWidget] = None):
+        super().__init__("Catalogue(s) information", state, parent)
+
+    def setup(self, entities: List[Union[tscat._Catalogue, tscat._Event]]) -> None:
+
+        catalogues = [entity for entity in entities if isinstance(entity, tscat._Catalogue)]
+        if len(catalogues) == 0:
+            self.hide()
+        else:
+            values = {}
+            self.show()
+
+            for k, value_func in catalogue_meta_data.items():
+                value = value_func(catalogues)
+                values[k] = _ReadOnlyString(value)
+
+            super().setup_values(values)
+
+
+class _EntityEditWidget(QtWidgets.QWidget):
+    def __init__(self, state: AppState, parent=None) -> None:
+        super().__init__(parent)
+
+        layout = QtWidgets.QVBoxLayout()
+        layout.setContentsMargins(5, 5, 5, 5)
+
+        self.meta_data = CatalogueMetaDataGroupBox(state)
+        layout.addWidget(self.meta_data)
+
+        self.fixed_attributes = FixedAttributesGroupBox(state)
+        layout.addWidget(self.fixed_attributes)
+
+        self.attributes: Optional[CustomAttributesGroupBox]
+        self.attributes = CustomAttributesGroupBox(state)
+        layout.addWidget(self.attributes)
+
+        layout.addStretch()
 
-        layout.addWidget(toolbar)
-        layout.addWidget(splitter)
         self.setLayout(layout)
 
-    def _external_signal_emission(self, action: str, type: Union[tscat._Catalogue, tscat._Event], uuid: str):
-        if action == "active_select":
-            if type == tscat._Catalogue:
-                self.catalogue_selected.emit(uuid)
-            else:
-                self.event_selected.emit(uuid)
+    def setup(self, uuids: List[str]) -> None:
 
-        elif action == 'changed':
-            if type == tscat._Catalogue:
-                self.catalogue_changed.emit(uuid)
-            else:
-                self.event_changed.emit(uuid)
+        from .tscat_driver.model import tscat_model
+        entities = tscat_model.entities_from_uuids(uuids)
+
+        if self.meta_data:
+            self.meta_data.setup(entities)
+        if self.attributes:
+            self.attributes.setup(entities)
+        self.fixed_attributes.setup(entities)
+
+
+class EntityEditView(QtWidgets.QScrollArea):
+
+    def __init__(self, state: AppState, parent=None) -> None:
+        super().__init__(parent)
+
+        self.edit: Optional[_EntityEditWidget] = None
+        self.state = state
+        self.current_uuids: List[str] = []
+
+        self.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOn)  # type: ignore
+        self.setWidgetResizable(True)
+
+        self.state.state_changed.connect(self.state_changed)
+
+        from .tscat_driver.model import tscat_model
+        tscat_model.action_done.connect(self._model_action_done)
+
+    def state_changed(self, action: str,
+                      _: Union[Type[tscat._Catalogue], Type[tscat._Event]],
+                      uuids: List[str]) -> None:
+        if action == 'active_select':
+            if self.current_uuids != uuids:
+                if self.edit:
+                    self.edit.deleteLater()
+                    self.edit = None
+
+                self.current_uuids = uuids
+
+                if len(uuids) > 0:
+                    self.edit = _EntityEditWidget(self.state)
+                    self.setWidget(self.edit)
+                    self.edit.setup(self.current_uuids)
+        elif action == 'passive_select':
+            pass
+        else:
+            print('unsupported (old) state-changed', action)
 
-    def update_event_range(self, uuid: str, start: dt.datetime, stop: dt.datetime) -> None:
-        event = get_entity_from_uuid_safe(uuid)
-        event.start = start
-        event.stop = stop
-        self.state.updated('changed', tscat._Event, uuid)
-
-    def create_event(self, start: dt.datetime, stop: dt.datetime, author: str, catalogue_uuid: str) -> tscat._Event:
-        catalogue = get_entity_from_uuid_safe(catalogue_uuid)
-        with tscat.Session() as s:
-            event = s.create_event(start, stop, author)
-            tscat.add_events_to_catalogue(catalogue, event)
-
-        self.state.updated('inserted', tscat._Event, event.uuid)
-
-        return event
-
-    def move_to_trash(self, uuid: str) -> None:
-        entity = get_entity_from_uuid_safe(uuid)
-        entity.remove()
-        self.state.updated('moved', type(entity), uuid)
-
-    def save(self) -> None:
-        tscat.save()
-        self.state.set_undo_stack_clean()
+    def _model_action_done(self, action: Action) -> None:
+        if self.edit:
+            if isinstance(action, GetCatalogueAction):
+                if action.uuid in self.current_uuids:
+                    self.edit.setup(self.current_uuids)
+            elif isinstance(action, (SetAttributeAction, DeleteAttributeAction)):
+                if any(entity.uuid in self.current_uuids for entity in action.entities):
+                    self.edit.setup(self.current_uuids)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tscat_gui-0.2.0/tscat_gui/predicate.py` & `tscat_gui-0.3.1/tscat_gui/predicate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from PySide6 import QtCore, QtWidgets, QtGui
-
-from .utils.helper import AttributeNameValidator, IntDelegate, FloatDelegate, DateTimeDelegate, BoolDelegate, \
-    StrDelegate
-from .utils.editable_label import EditableLabel
+import datetime as dt
+import typing
+from typing import Dict, Optional, Type, Union, cast
 
-from typing import Union, Type, Optional, Dict, cast
+from PySide6 import QtCore, QtGui, QtWidgets
 
-from tscat.filtering import Comparison, Field, Attribute, Any, All, Not, In, InCatalogue, Has, Predicate, Match
 import tscat.filtering
-import datetime as dt
+from tscat.filtering import All, Any, Attribute, Comparison, Field, Has, In, InCatalogue, Match, Not, Predicate
+from .utils.editable_label import EditableLabel
+from .utils.helper import AttributeNameValidator, BoolDelegate, DateTimeDelegate, FloatDelegate, IntDelegate, \
+    StrDelegate
 
 
 class _PredicateWidget(QtWidgets.QWidget):
     changed = QtCore.Signal()
 
     def __init__(self, parent: Optional[QtWidgets.QWidget]):
         super().__init__(parent)
@@ -26,15 +26,15 @@
         pass
 
 
 class _Root(_PredicateWidget):
     def __init__(self, predicate: Predicate):
         super().__init__(None)
 
-        self._first = predicate_to_widget_factory(predicate, None)
+        self._first = predicate_to_widget_factory(predicate, self)
         if self._first:
             c = QtWidgets.QHBoxLayout()
             c.setContentsMargins(0, 0, 0, 0)
             c.addWidget(self._first)
             self.setLayout(c)
 
             self._first.changed.connect(lambda: self.changed.emit())
@@ -175,14 +175,15 @@
             widget.editingFinished.connect(lambda: self.changed.emit())  # type: ignore
             self._value_widgets[_type] = widget
         else:
             widget = self._value_widgets[_type]
 
         self._current_value_widget = widget
         self._layout.addWidget(widget)
+        widget.show()
         self.changed.emit()
 
     def predicate(self) -> Optional[Union[Comparison, Match, Not]]:
         if self._current_value_widget is None:
             return None
 
         field: Union[Field, Attribute]
@@ -294,30 +295,48 @@
 
 class _InCatalogue(_PredicateWidget):
     OP_IN = 0
     OP_NOT_IN = 1
 
     OP_LABELS = ['is in catalogue', 'is not in catalogue']
 
-    def __init__(self, predicate: Union[InCatalogue, None], negate: bool, parent: _PredicateWidget):
+    def __init__(self, predicate: Optional[InCatalogue], negate: bool, parent: _PredicateWidget):
         super().__init__(parent)
 
         c = QtWidgets.QHBoxLayout()
         c.setContentsMargins(0, 0, 0, 0)
 
         self._op_label = QtWidgets.QLabel()
         self.set_operator(_InCatalogue.OP_NOT_IN if negate else _InCatalogue.OP_IN)
         c.addWidget(self._op_label)
 
         self.catalogues = QtWidgets.QComboBox()
-        for cat in tscat.get_catalogues():
-            self.catalogues.addItem(cat.name, cat)
 
-        for cat in tscat.get_catalogues(removed_items=True):
-            self.catalogues.addItem(cat.name + " (in trash)", cat)
+        from .tscat_driver.model import tscat_model
+        from .tscat_driver.nodes import CatalogNode
+
+        for cat in tscat_model.tscat_root().catalogue_nodes(in_trash=False):
+            if isinstance(cat, CatalogNode):
+                self.catalogues.addItem(cat.name, cat.node)
+
+        for cat in tscat_model.tscat_root().catalogue_nodes(in_trash=True):
+            if isinstance(cat, CatalogNode):
+                self.catalogues.addItem(cat.name + " (in trash)", cat.node)
+
+        if predicate is not None:
+            for index in range(self.catalogues.count()):
+                catalogue = cast(tscat._Catalogue, self.catalogues.itemData(index))
+                if catalogue and predicate.catalogue and predicate.catalogue.uuid == catalogue.uuid:
+                    break
+            else:
+                index = -1
+
+            if index != -1:
+                self.catalogues.setCurrentIndex(index)
+
         self.catalogues.currentIndexChanged.connect(lambda: self.changed.emit())  # type: ignore
 
         c.addWidget(self.catalogues)
 
         self.setLayout(c)
 
     def predicate(self) -> Union[InCatalogue, Not]:
@@ -349,15 +368,16 @@
     ['Attribute Present', _AttributeIsPresent, _AttributeIsPresent.OP_HAS],
     ['Attribute Not Present', _AttributeIsPresent, _AttributeIsPresent.OP_HAS_NOT],
 ]
 
 
 class _Condition(_PredicateWidget):
     def __init__(self, predicate: Union[Comparison, Match, In, Has, InCatalogue, None],
-                 parent: Optional[_PredicateWidget]):
+                 negate: bool,
+                 parent: _PredicateWidget):
         super().__init__(parent)
 
         self._hlayout = QtWidgets.QHBoxLayout()
         self._hlayout.setContentsMargins(0, 0, 0, 0)
 
         self._cb = QtWidgets.QComboBox()
         for op in operators:
@@ -427,21 +447,24 @@
         return self.condition.predicate()
 
     def delete_child(self, child):
         raise AssertionError('Should never be called.')
 
 
 class _LogicalCombination(_PredicateWidget):
-    def __init__(self, predicate: Union[All, Any, None], parent: Optional[_PredicateWidget]):
+    def __init__(self,
+                 predicate: Union[All, Any, None],
+                 negate: bool,
+                 parent: _PredicateWidget):
         super().__init__(parent)
 
         if predicate is None:
             predicate = Any()
 
-        self._children: list[_PredicateWidget] = []
+        self._children: typing.List[_PredicateWidget] = []
 
         self._layout = QtWidgets.QVBoxLayout()
         self._layout.setContentsMargins(20, 0, 0, 0)
 
         button_group = QtWidgets.QButtonGroup(self)
 
         sub_layout = QtWidgets.QHBoxLayout()
@@ -474,16 +497,22 @@
 
         add = _AddPredicateWidget(self)
         add.new.connect(lambda x: self.new(x.selected_type()))
         self._layout.addWidget(add)
 
         self.setLayout(self._layout)
 
-    def new(self, cls: Type[_PredicateWidget]):
-        t = cls(predicate=None, parent=self)
+    def new(self, cls: Union[
+            Type['_LogicalCombination'],
+            Type[_Condition],
+            Type[_Comparison],
+            Type[_AttributeIsPresent],
+            Type[_StringInStringList],
+            Type[_InCatalogue]]):
+        t = cls(predicate=None, negate=False, parent=self)
         self._layout.insertWidget(self._layout.count() - 1, t)
         self.add_child_predicate(t)
         self.changed.emit()
 
     def add_child_predicate(self, widget: _PredicateWidget):
         self._children += [widget]
 
@@ -503,21 +532,21 @@
     def delete_child(self, widget):
         widget.deleteLater()
         self._layout.removeWidget(widget)
         self._children.remove(widget)
         self.changed.emit()
 
 
-def predicate_to_widget_factory(predicate: Predicate, parent: Optional[_PredicateWidget]) -> \
+def predicate_to_widget_factory(predicate: Predicate, parent: _PredicateWidget) -> \
     Union[_LogicalCombination, _Condition]:
     if isinstance(predicate, Any) or isinstance(predicate, All):
-        return _LogicalCombination(predicate, parent)
+        return _LogicalCombination(predicate, False, parent)
     elif isinstance(predicate, Comparison) or isinstance(predicate, Match) or \
         isinstance(predicate, In) or isinstance(predicate, Has) or isinstance(predicate, InCatalogue):
-        return _Condition(predicate, parent)
+        return _Condition(predicate, False, parent)
 
     raise ValueError('Unknown predicate type for factory')
 
 
 class _AddPredicateWidget(QtWidgets.QWidget):
     new = QtCore.Signal(QtWidgets.QWidget)
 
@@ -548,19 +577,19 @@
 
 class _DeletePredicateWidget(QtWidgets.QToolButton):
     def __init__(self, widget: _PredicateWidget):
         super().__init__(widget)
 
         self.setText('✖')
 
-        self.clicked.connect(lambda: cast(widget.parent(), QtWidgets.QWidget).delete_child(widget))  # type: ignore
+        self.clicked.connect(lambda: widget.parent().delete_child(widget))  # type: ignore
 
 
 class SimplePredicateEditDialog(QtWidgets.QDialog):
-    def __init__(self, predicate: Optional[tscat.Predicate], parent=None):
+    def __init__(self, predicate: Optional[Predicate], parent=None):
         super().__init__(parent)
 
         layout = QtWidgets.QVBoxLayout()
 
         self.predicate = predicate
 
         if predicate is None:
```

### Comparing `tscat_gui-0.2.0/tscat_gui/state.py` & `tscat_gui-0.3.1/tscat_gui/state.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,60 @@
-from PySide6 import QtWidgets, QtGui
+from PySide6 import QtGui
 from PySide6 import QtCore
 
-import tscat
-
-from typing import Union, Type
+import copy
 import dataclasses
+from typing import Union, Type, Optional, List
+
+import tscat
 
 from .logger import log
 
 
 @dataclasses.dataclass
 class SelectState:
-    active: str
+    selected: List[str]
     type: Union[Type[tscat._Catalogue], Type[tscat._Event]]
-    active_catalogue: str
+    selected_catalogues: List[str]
 
 
 class AppState(QtCore.QObject):
-    state_changed = QtCore.Signal(str, type, str)
+    state_changed = QtCore.Signal(str, type, list)
 
     undo_stack_clean_changed = QtCore.Signal(bool)
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
-        self.active: str = None
-        self.active_type = tscat._Catalogue
-        self.active_catalogue: str = None
+        self._select_state = SelectState([], tscat._Catalogue, [])
 
         self._undo_stack = QtGui.QUndoStack()
-        self._undo_stack.cleanChanged.connect(lambda x: self.undo_stack_clean_changed.emit(x))
+        self._undo_stack.cleanChanged.connect(lambda x: self.undo_stack_clean_changed.emit(x))  # type: ignore
 
     def push_undo_command(self, cls, *args) -> None:
         self._undo_stack.push(cls(self, *args))
 
     def set_undo_stack_clean(self):
         self._undo_stack.setClean()
 
     def create_undo_redo_action(self):
         return self._undo_stack.createUndoAction(self), self._undo_stack.createRedoAction(self)
 
     def select_state(self) -> SelectState:
-        return SelectState(self.active, self.active_type, self.active_catalogue)
+        return copy.deepcopy(self._select_state)
+
+    def undo_stack(self) -> QtGui.QUndoStack:
+        return self._undo_stack
 
-    def updated(self, action: str, type: Union[Type[tscat._Catalogue], Type[tscat._Event]], uuid: str) -> None:
+    def updated(self, action: str, ty: Union[Type[tscat._Catalogue], Type[tscat._Event]],
+                uuids: List[str]) -> None:
         if action == 'active_select':
-            if uuid != self.active:
-                self.active = uuid
-                self.active_type = type
+            if uuids != self._select_state.selected:
+                self._select_state.selected = uuids[:]
+                self._select_state.type = ty
 
-                if self.active_type == tscat._Catalogue:
-                    self.active_catalogue = uuid
+                if self._select_state.type == tscat._Catalogue:
+                    self._select_state.selected_catalogues = uuids[:]
             else:
-                log.debug(f'already active "{uuid}"')
+                log.debug(f'already active "{uuids}"')
 
-        log.debug(f'app-state-updated action:{action}, type:{type}, uuid:{uuid}')
-        self.state_changed.emit(action, type, uuid)
+        log.debug(f'app-state-updated action:{action}, type:{ty}, uuids:{uuids}')
+        self.state_changed.emit(action, ty, uuids)
```

### Comparing `tscat_gui-0.2.0/tscat_gui/utils/editable_label.py` & `tscat_gui-0.3.1/tscat_gui/utils/editable_label.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             super().__init__(text, parent)
 
         def mousePressEvent(self, event: QtGui.QMouseEvent) -> None:
             if event.button() == QtCore.Qt.MouseButton.LeftButton:
                 self.clicked.emit()
             super().mousePressEvent(event)
 
-        def enterEvent(self, event: QtCore.QEvent) -> None:  # type: ignore
+        def enterEvent(self, event: QtGui.QEnterEvent) -> None:
             self.setCursor(QtCore.Qt.IBeamCursor)  # type: ignore
             super().enterEvent(event)
 
         def leaveEvent(self, event: QtCore.QEvent) -> None:
             self.setCursor(QtCore.Qt.ArrowCursor)  # type: ignore
             super().leaveEvent(event)
 
@@ -62,15 +62,15 @@
 
         def keyPressEvent(self, event: QtGui.QKeyEvent) -> None:
             if event.key() == QtCore.Qt.Key_Escape:  # type: ignore
                 self.canceled.emit()
 
             super().keyPressEvent(event)
 
-    def __init__(self, text: str, validator: QtGui.QValidator = None, parent=None):
+    def __init__(self, text: str, validator: typing.Optional[QtGui.QValidator] = None, parent=None):
         super().__init__(parent)
 
         self.setSizePolicy(QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Maximum)  # type: ignore
 
         self.text = text
         self.validator = validator
         self.label: typing.Optional[EditableLabel.Label] = None
```

### Comparing `tscat_gui-0.2.0/tscat_gui/utils/flow_layout.py` & `tscat_gui-0.3.1/tscat_gui/utils/flow_layout.py`

 * *Files identical despite different names*

### Comparing `tscat_gui-0.2.0/tscat_gui/utils/helper.py` & `tscat_gui-0.3.1/tscat_gui/utils/keyword_list.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,142 @@
-from PySide6 import QtGui, QtWidgets, QtCore
+from .flow_layout import FlowLayout
+from .editable_label import EditableLabel
+
+from PySide6 import QtWidgets, QtCore, QtGui
 
 import re
-from typing import Union, cast
-import datetime as dt
+import typing
 
-import tscat
+# UTF-8 letters in the beginning, then also numbers and underscore
+_tag_validation_regex = re.compile(r'^[a-z][^,]*$')
 
 
-# this function should go to tscat - this is a kludge to work-around missing functions or wrong concepts
-# get an entity from a UUID (catalogue or event)
-# get an entity from a UUID independently whether it is removed (in trash) or not
-def get_entity_from_uuid_safe(uuid: str) -> Union[tscat._Catalogue, tscat._Event]:
-    catalogues = tscat.get_catalogues(tscat.filtering.UUID(uuid))
-    if len(catalogues) == 1:
-        return catalogues[0]
-    elif len(catalogues) == 0:
-        catalogues = tscat.get_catalogues(tscat.filtering.UUID(uuid), removed_items=True)
-        if len(catalogues) == 1:
-            return catalogues[0]
-        elif len(catalogues) == 0:
-            events = tscat.get_events(tscat.filtering.UUID(uuid))
-            if len(events) == 1:
-                return events[0]
-            elif len(events) == 0:
-                events = tscat.get_events(tscat.filtering.UUID(uuid), removed_items=True)
-                if len(events) == 1:
-                    return events[0]
+class _Keyword(EditableLabel):
+    closed = QtCore.Signal(QtWidgets.QWidget)
 
-    raise ValueError(f"No entity (catalogue or event) found for this UUID {uuid}")
+    class DeleteLabel(QtWidgets.QLabel):
+        clicked = QtCore.Signal()
 
+        def __init__(self, parent=None):
+            super().__init__('✕', parent)
+            self.setMargin(1)
+            self.setObjectName('DeleteLabel')
+            self.setStyleSheet(
+                f"""#DeleteLabel {{
+                    border-radius: 5px;
+                    background: {self.palette().dark().color().name()};
+                    min-width: 10px;
+                    min-height: 10px;
+                }}""")
 
-_valid_attribute_name_re = re.compile(r'^[A-Za-z][A-Za-z_0-9]*$')
+        def enterEvent(self, event: QtCore.QEvent) -> None:
+            self.setText('✖')
+            super().enterEvent(event)  # type: ignore
 
+        def leaveEvent(self, event: QtCore.QEvent) -> None:
+            self.setText('✕')
+            super().leaveEvent(event)
 
-class AttributeNameValidator(QtGui.QValidator):
-    def __init__(self, invalid_words: list[str] = [], parent=None):
-        super().__init__(parent)
-        self.invalid_words = invalid_words
+        def mousePressEvent(self, event: QtGui.QMouseEvent) -> None:
+            if event.button() == QtCore.Qt.MouseButton.LeftButton:
+                self.clicked.emit()
 
-    def validate(self, word: str, pos: int) -> QtGui.QValidator.State:
-        if len(word) == 0:
-            return QtGui.QValidator.Intermediate  # type: ignore
+            super().mousePressEvent(event)
 
-        if word in self.invalid_words:
-            return QtGui.QValidator.Intermediate  # type: ignore
+    class Validator(QtGui.QValidator):
+        def __init__(self, parent=None):
+            super().__init__(parent)
 
-        if not _valid_attribute_name_re.match(word):
-            return QtGui.QValidator.Intermediate  # type: ignore
+        def validate(self, word: str, pos: int) -> QtGui.QValidator.State:
+            if len(word) == 0:
+                return QtGui.QValidator.Intermediate  # type: ignore
 
-        return QtGui.QValidator.Acceptable  # type: ignore
+            if not _tag_validation_regex.match(word):
+                return QtGui.QValidator.Intermediate  # type: ignore
 
+            return QtGui.QValidator.Acceptable  # type: ignore
 
-class IntDelegate(QtWidgets.QSpinBox):
-    def __init__(self, value: Union[int, None] = None, parent: QtWidgets.QWidget = None):
-        super().__init__(parent)
-        self.setRange(-2 ** 31, 2 ** 31 - 1)
-        if value is None:
-            value = 0
-        self.setValue(0 if value is None else value)
+    def __init__(self, text: str, parent: 'EditableKeywordListWidget'):
+        super().__init__(text, _Keyword.Validator(), parent)
 
-    def set_value(self, value: int):
-        self.setValue(value)
+        self.list_widget = parent
 
+        self.delete_label = _Keyword.DeleteLabel()
+        self.delete_label.clicked.connect(lambda: self.closed.emit(self))
 
-class FloatDelegate(QtWidgets.QLineEdit):
-    def __init__(self, value: Union[float, None] = None, parent: QtWidgets.QWidget = None):
-        super().__init__(parent)
+        self._layout.addWidget(self.delete_label)
+        self._layout.setContentsMargins(5, 5, 5, 5)
 
-        validator = QtGui.QDoubleValidator(self)
-        validator.setNotation(QtGui.QDoubleValidator.Notation.ScientificNotation)
-        self.setValidator(validator)
+        self.setObjectName('OneKeyword')
+        self.setStyleSheet(f"""#OneKeyword {{
+                border-radius: 15px;
+                background: {self.palette().mid().color().name()};
+            }}""")
 
-        if value is None:
-            value = 0
-        self.setText(str(value))
+    def edit(self):
+        super().edit()
 
-    def value(self) -> float:
-        return float(self.text())
+        completer = QtWidgets.QCompleter(self.list_widget.completion_strings, parent=self)
+        completer.setCaseSensitivity(QtCore.Qt.CaseInsensitive)
 
-    def set_value(self, value: float):
-        self.setText(str(value))
+        self.lineedit.setCompleter(completer)
 
 
-class BoolDelegate(QtWidgets.QCheckBox):
+class EditableKeywordListWidget(QtWidgets.QWidget):
     editingFinished = QtCore.Signal()
 
-    def __init__(self, value: Union[bool, None] = None, parent: QtWidgets.QWidget = None):
+    def __init__(self, strings: typing.List[str], completion_strings: typing.List[str] = [], parent=None):
         super().__init__(parent)
-        self.setChecked(False if value is None else value)
-        self.stateChanged.connect(lambda: self.editingFinished.emit())  # type: ignore
-
-    def value(self) -> bool:
-        return self.isChecked()
-
-    def set_value(self, value: bool):
-        self.setChecked(value)
-
-
-class StrDelegate(QtWidgets.QLineEdit):
-    def __init__(self, value: Union[str, None] = None, parent: QtWidgets.QWidget = None):
-        super().__init__("" if value is None else value, parent)
-
-    def value(self) -> str:
-        return self.text()
-
-    def set_value(self, value: str):
-        self.setText(value)
 
+        self._layout = FlowLayout()
 
-class DateTimeDelegate(QtWidgets.QDateTimeEdit):
-    def __init__(self, value: Union[dt.datetime, None] = None, parent: QtWidgets.QWidget = None):
-        super().__init__(dt.datetime.now() if value is None else value, parent)  # type: ignore
+        self.new_tag = QtWidgets.QToolButton()
+        self.new_tag.setText('➕')
+        self.new_tag.clicked.connect(lambda _: self._add_tag('', edit=True))  # type: ignore
+        self._layout.addWidget(self.new_tag)
+
+        self.tags: typing.List[_Keyword] = []
+        for text in strings:
+            self._add_tag(text)
+
+        self.completion_strings = set(completion_strings + strings)
+
+        self.setLayout(self._layout)
+
+    def _add_tag(self, text: str, edit=False):
+        tag = _Keyword(text, self)
+        self.tags += [tag]
+        tag.editing_finished.connect(lambda x, _tag=tag: self._tag_text_updated(tag, x))
+        tag.closed.connect(self._delete_tag)
+
+        # insert before the new_tag-button
+        self._layout.removeWidget(self.new_tag)
+        self._layout.addWidget(tag)
+        self._layout.addWidget(self.new_tag)
+
+        if edit:
+            self._request_edit(tag)
+
+    def _update_tag_texts(self):
+        self.editingFinished.emit()
+
+    def _tag_text_updated(self, tag: _Keyword, text: str):
+        if len(text) == 0:
+            self._delete_tag(tag)
+        else:
+            self.completion_strings.add(text)
+        self._update_tag_texts()
+
+    def _request_edit(self, tag: _Keyword):
+        for t in self.tags:
+            t.finish_editing()
+        tag.edit()
+
+    def _delete_tag(self, tag: _Keyword):
+        self.tags.remove(tag)
+        self._layout.removeWidget(tag)
+        tag.deleteLater()
 
-    def value(self) -> dt.datetime:
-        return cast(dt.datetime, self.dateTime().toPython())
+        self._update_tag_texts()
 
-    def set_value(self, value: dt.datetime):
-        self.setDateTime(value)  # type: ignore
+    def value(self) -> typing.List[str]:
+        return [tag.text for tag in self.tags if tag.text]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tscat_gui-0.2.0/tscat_gui.egg-info/PKG-INFO` & `tscat_gui-0.3.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,69 @@
-Metadata-Version: 1.2
-Name: tscat-gui
-Version: 0.2.0
+Metadata-Version: 2.1
+Name: tscat_gui
+Version: 0.3.1
 Summary: Time-series catalogue - graphical user interface library
 Home-page: https://github.com/SciQLop/tscat_gui
 Author: Patrick Boettcher
 Author-email: p@yai.se
 License: GNU General Public License v3
-Description: ===========================
-        Time series catalogue - GUI
-        ===========================
-        
-        
-        .. image:: https://img.shields.io/pypi/v/tscat_gui.svg
-                :target: https://pypi.python.org/pypi/tscat_gui
-        
-        .. image:: https://img.shields.io/travis/SciQLop/tscat_gui.svg
-                :target: https://travis-ci.com/SciQLop/tscat_gui
-        
-        .. image:: https://readthedocs.org/projects/tscat-gui/badge/?version=latest
-                :target: https://tscat-gui.readthedocs.io/en/latest/?version=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        Time-series catalogue - graphical user interface library
-        
-        
-        * Free software: GNU General Public License v3
-        * Documentation: https://tscat-gui.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2021-11-04)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: tscat_gui
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+===========================
+Time series catalogue - GUI
+===========================
+
+
+.. image:: https://img.shields.io/pypi/v/tscat_gui.svg
+        :target: https://pypi.python.org/pypi/tscat_gui
+
+.. image:: https://img.shields.io/travis/SciQLop/tscat_gui.svg
+        :target: https://travis-ci.com/SciQLop/tscat_gui
+
+.. image:: https://readthedocs.org/projects/tscat-gui/badge/?version=latest
+        :target: https://tscat-gui.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+
+
+
+Time-series catalogue - graphical user interface library
+
+
+* Free software: GNU General Public License v3
+* Documentation: https://tscat-gui.readthedocs.io.
+
+
+Features
+--------
+
+* TODO
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.1.0 (2021-11-04)
+------------------
+
+* First release on PyPI.
```

