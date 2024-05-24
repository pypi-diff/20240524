# Comparing `tmp/HiYaPyCo-0.5.6.tar.gz` & `tmp/HiYaPyCo-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HiYaPyCo-0.5.6.tar", last modified: Sat May 11 05:03:28 2024, max compression
+gzip compressed data, was "HiYaPyCo-0.6.0.tar", last modified: Fri May 24 10:42:32 2024, max compression
```

## Comparing `HiYaPyCo-0.5.6.tar` & `HiYaPyCo-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-05-11 05:03:28.522827 HiYaPyCo-0.5.6/
-drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-05-11 05:03:28.518827 HiYaPyCo-0.5.6/HiYaPyCo.egg-info/
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    11283 2024-05-11 05:03:28.000000 HiYaPyCo-0.5.6/HiYaPyCo.egg-info/PKG-INFO
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)      489 2024-05-11 05:03:28.000000 HiYaPyCo-0.5.6/HiYaPyCo.egg-info/SOURCES.txt
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)        1 2024-05-11 05:03:28.000000 HiYaPyCo-0.5.6/HiYaPyCo.egg-info/dependency_links.txt
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)       34 2024-05-11 05:03:28.000000 HiYaPyCo-0.5.6/HiYaPyCo.egg-info/requires.txt
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)        9 2024-05-11 05:03:28.000000 HiYaPyCo-0.5.6/HiYaPyCo.egg-info/top_level.txt
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    35141 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/LICENSE
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)       36 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/MANIFEST.in
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    11283 2024-05-11 05:03:28.522827 HiYaPyCo-0.5.6/PKG-INFO
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    10492 2024-05-11 04:56:25.000000 HiYaPyCo-0.5.6/README.rst
-drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-05-11 05:03:28.518827 HiYaPyCo-0.5.6/hiyapyco/
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    21991 2024-05-10 18:45:35.000000 HiYaPyCo-0.5.6/hiyapyco/__init__.py
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)     2604 2024-04-13 08:37:32.000000 HiYaPyCo-0.5.6/hiyapyco/odyldo.py
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)       16 2024-05-11 04:43:26.000000 HiYaPyCo-0.5.6/hiyapyco/version.py
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)      109 2024-05-11 05:03:28.522827 HiYaPyCo-0.5.6/setup.cfg
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1357 2024-05-11 04:53:17.000000 HiYaPyCo-0.5.6/setup.py
-drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-05-11 05:03:28.518827 HiYaPyCo-0.5.6/test/
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1739 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_castinterpolated.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     3021 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_interpolation.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1734 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_interpolationunicode.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     4905 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_invocation.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     5075 2023-11-29 07:36:03.000000 HiYaPyCo-0.5.6/test/test_merge.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     4313 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_missingfiles.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1753 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_multiple.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     2836 2022-05-04 08:47:46.000000 HiYaPyCo-0.5.6/test/test_odict.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1913 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_simple.py
+drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-05-24 10:42:32.372515 HiYaPyCo-0.6.0/
+drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-05-24 10:42:32.372515 HiYaPyCo-0.6.0/HiYaPyCo.egg-info/
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    11343 2024-05-24 10:42:32.000000 HiYaPyCo-0.6.0/HiYaPyCo.egg-info/PKG-INFO
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)      514 2024-05-24 10:42:32.000000 HiYaPyCo-0.6.0/HiYaPyCo.egg-info/SOURCES.txt
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)        1 2024-05-24 10:42:32.000000 HiYaPyCo-0.6.0/HiYaPyCo.egg-info/dependency_links.txt
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)       34 2024-05-24 10:42:32.000000 HiYaPyCo-0.6.0/HiYaPyCo.egg-info/requires.txt
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)        9 2024-05-24 10:42:32.000000 HiYaPyCo-0.6.0/HiYaPyCo.egg-info/top_level.txt
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    35141 2020-06-18 09:22:15.000000 HiYaPyCo-0.6.0/LICENSE
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)       36 2020-06-18 09:22:15.000000 HiYaPyCo-0.6.0/MANIFEST.in
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    11343 2024-05-24 10:42:32.372515 HiYaPyCo-0.6.0/PKG-INFO
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    10552 2024-05-24 10:35:48.000000 HiYaPyCo-0.6.0/README.rst
+drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-05-24 10:42:32.372515 HiYaPyCo-0.6.0/hiyapyco/
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    22946 2024-05-24 10:24:34.000000 HiYaPyCo-0.6.0/hiyapyco/__init__.py
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)     2604 2024-04-13 08:37:32.000000 HiYaPyCo-0.6.0/hiyapyco/odyldo.py
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)       16 2024-05-24 10:38:43.000000 HiYaPyCo-0.6.0/hiyapyco/version.py
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)      109 2024-05-24 10:42:32.372515 HiYaPyCo-0.6.0/setup.cfg
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1357 2024-05-24 10:36:45.000000 HiYaPyCo-0.6.0/setup.py
+drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-05-24 10:42:32.372515 HiYaPyCo-0.6.0/test/
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1915 2024-05-24 10:24:34.000000 HiYaPyCo-0.6.0/test/test_anchoralias.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1739 2020-06-18 09:22:15.000000 HiYaPyCo-0.6.0/test/test_castinterpolated.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     3021 2020-06-18 09:22:15.000000 HiYaPyCo-0.6.0/test/test_interpolation.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1734 2020-06-18 09:22:15.000000 HiYaPyCo-0.6.0/test/test_interpolationunicode.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     4905 2020-06-18 09:22:15.000000 HiYaPyCo-0.6.0/test/test_invocation.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     5075 2023-11-29 07:36:03.000000 HiYaPyCo-0.6.0/test/test_merge.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     4313 2020-06-18 09:22:15.000000 HiYaPyCo-0.6.0/test/test_missingfiles.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1753 2020-06-18 09:22:15.000000 HiYaPyCo-0.6.0/test/test_multiple.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     2836 2022-05-04 08:47:46.000000 HiYaPyCo-0.6.0/test/test_odict.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1913 2020-06-18 09:22:15.000000 HiYaPyCo-0.6.0/test/test_simple.py
```

### Comparing `HiYaPyCo-0.5.6/HiYaPyCo.egg-info/PKG-INFO` & `HiYaPyCo-0.6.0/HiYaPyCo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiYaPyCo
-Version: 0.5.6
+Version: 0.6.0
 Summary: Hierarchical Yaml Python Config
 Home-page: https://github.com/zerwes/hiyapyco
 Author: Klaus Zerwes zero-sys.net
 Author-email: zerwes@users.noreply.github.com
 License: GPLv3
 Keywords: configuration parser yaml
 Platform: any
@@ -15,26 +15,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-.. |isrf| image:: https://upload.wikimedia.org/wikipedia/commons/thumb/d/d4/Flag_of_Israel.svg/64px-Flag_of_Israel.svg.png
-   :alt: Stand with the people of Israel
-
-|isrf| Stand with the people of Israel
-
-.. image:: https://badgen.net/badge/stand%20with/UKRAINE/?color=0057B8&labelColor=FFD700
-
-.. image:: https://github.com/zerwes/hiyapyco/actions/workflows/pylint.yml/badge.svg?branch=master
+.. |pylint| image:: https://github.com/zerwes/hiyapyco/actions/workflows/pylint.yml/badge.svg?branch=main
     :target: https://github.com/zerwes/hiyapyco/actions/workflows/pylint.yml
-
-.. image:: https://github.com/zerwes/hiyapyco/actions/workflows/test.yml/badge.svg
+.. |test| image:: https://github.com/zerwes/hiyapyco/actions/workflows/test.yml/badge.svg
      :target: https://github.com/zerwes/hiyapyco/actions/workflows/test.yml
+.. |gpl| image:: https://img.shields.io/badge/License-GPL%20v3-blue.svg
+     :target: http://www.gnu.org/licenses/gpl-3.0
+
+|pylint| |test| |gpl|
 
 hiyapyco
 ========
 
 HiYaPyCo - A Hierarchical Yaml Python Config
 
 Description
@@ -171,14 +167,16 @@
    match* cast for interpolated strings (default: ``False``)
 
 -  ``usedefaultyamlloader``: boolean : force the usage of the default
    *PyYAML* loader/dumper instead of *HiYaPyCo*\ s implementation of a
    OrderedDict loader/dumper (see: Ordered Dict Yaml Loader / Dumper
    aka. ODYLDo) (default: ``False``)
 
+- ``dereferenceyamlanchors``: boolean : dereference yaml anchors and use a copy (default: ``True``)
+
 - ``encoding``: string : encoding used to read yaml files (default: ``utf-8``)
 
 -  ``failonmissingfiles``: boolean : fail if a supplied YAML file can
    not be found (default: ``True``)
 
 -  ``loglevel``: int : loglevel for the hiyapyco logger; should be one
    of the valid levels from ``logging``: 'WARN', 'ERROR', 'DEBUG', 'I
@@ -348,15 +346,21 @@
 Foundation.
 See
 `https://www.gnu.org/licenses/gpl.html <https://www.gnu.org/licenses/gpl.html>`_
 
 Changelog
 ---------
 
-0.5.5
+0.6.0
+~~~~~~
+
+FIXED: #69 (weird merge behavior with anchors)
+MERGED: #71 (dereference anchors)
+
+0.5.6
 ~~~~~~
 
 MERGED: #70 by itachi-cracker
 
 FIXED: #61 (removed deprecated distutils)
 
 0.5.5
```

### Comparing `HiYaPyCo-0.5.6/LICENSE` & `HiYaPyCo-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.6/PKG-INFO` & `HiYaPyCo-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiYaPyCo
-Version: 0.5.6
+Version: 0.6.0
 Summary: Hierarchical Yaml Python Config
 Home-page: https://github.com/zerwes/hiyapyco
 Author: Klaus Zerwes zero-sys.net
 Author-email: zerwes@users.noreply.github.com
 License: GPLv3
 Keywords: configuration parser yaml
 Platform: any
@@ -15,26 +15,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-.. |isrf| image:: https://upload.wikimedia.org/wikipedia/commons/thumb/d/d4/Flag_of_Israel.svg/64px-Flag_of_Israel.svg.png
-   :alt: Stand with the people of Israel
-
-|isrf| Stand with the people of Israel
-
-.. image:: https://badgen.net/badge/stand%20with/UKRAINE/?color=0057B8&labelColor=FFD700
-
-.. image:: https://github.com/zerwes/hiyapyco/actions/workflows/pylint.yml/badge.svg?branch=master
+.. |pylint| image:: https://github.com/zerwes/hiyapyco/actions/workflows/pylint.yml/badge.svg?branch=main
     :target: https://github.com/zerwes/hiyapyco/actions/workflows/pylint.yml
-
-.. image:: https://github.com/zerwes/hiyapyco/actions/workflows/test.yml/badge.svg
+.. |test| image:: https://github.com/zerwes/hiyapyco/actions/workflows/test.yml/badge.svg
      :target: https://github.com/zerwes/hiyapyco/actions/workflows/test.yml
+.. |gpl| image:: https://img.shields.io/badge/License-GPL%20v3-blue.svg
+     :target: http://www.gnu.org/licenses/gpl-3.0
+
+|pylint| |test| |gpl|
 
 hiyapyco
 ========
 
 HiYaPyCo - A Hierarchical Yaml Python Config
 
 Description
@@ -171,14 +167,16 @@
    match* cast for interpolated strings (default: ``False``)
 
 -  ``usedefaultyamlloader``: boolean : force the usage of the default
    *PyYAML* loader/dumper instead of *HiYaPyCo*\ s implementation of a
    OrderedDict loader/dumper (see: Ordered Dict Yaml Loader / Dumper
    aka. ODYLDo) (default: ``False``)
 
+- ``dereferenceyamlanchors``: boolean : dereference yaml anchors and use a copy (default: ``True``)
+
 - ``encoding``: string : encoding used to read yaml files (default: ``utf-8``)
 
 -  ``failonmissingfiles``: boolean : fail if a supplied YAML file can
    not be found (default: ``True``)
 
 -  ``loglevel``: int : loglevel for the hiyapyco logger; should be one
    of the valid levels from ``logging``: 'WARN', 'ERROR', 'DEBUG', 'I
@@ -348,15 +346,21 @@
 Foundation.
 See
 `https://www.gnu.org/licenses/gpl.html <https://www.gnu.org/licenses/gpl.html>`_
 
 Changelog
 ---------
 
-0.5.5
+0.6.0
+~~~~~~
+
+FIXED: #69 (weird merge behavior with anchors)
+MERGED: #71 (dereference anchors)
+
+0.5.6
 ~~~~~~
 
 MERGED: #70 by itachi-cracker
 
 FIXED: #61 (removed deprecated distutils)
 
 0.5.5
```

### Comparing `HiYaPyCo-0.5.6/README.rst` & `HiYaPyCo-0.6.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-.. |isrf| image:: https://upload.wikimedia.org/wikipedia/commons/thumb/d/d4/Flag_of_Israel.svg/64px-Flag_of_Israel.svg.png
-   :alt: Stand with the people of Israel
-
-|isrf| Stand with the people of Israel
-
-.. image:: https://badgen.net/badge/stand%20with/UKRAINE/?color=0057B8&labelColor=FFD700
-
-.. image:: https://github.com/zerwes/hiyapyco/actions/workflows/pylint.yml/badge.svg?branch=master
+.. |pylint| image:: https://github.com/zerwes/hiyapyco/actions/workflows/pylint.yml/badge.svg?branch=main
     :target: https://github.com/zerwes/hiyapyco/actions/workflows/pylint.yml
-
-.. image:: https://github.com/zerwes/hiyapyco/actions/workflows/test.yml/badge.svg
+.. |test| image:: https://github.com/zerwes/hiyapyco/actions/workflows/test.yml/badge.svg
      :target: https://github.com/zerwes/hiyapyco/actions/workflows/test.yml
+.. |gpl| image:: https://img.shields.io/badge/License-GPL%20v3-blue.svg
+     :target: http://www.gnu.org/licenses/gpl-3.0
+
+|pylint| |test| |gpl|
 
 hiyapyco
 ========
 
 HiYaPyCo - A Hierarchical Yaml Python Config
 
 Description
@@ -150,14 +146,16 @@
    match* cast for interpolated strings (default: ``False``)
 
 -  ``usedefaultyamlloader``: boolean : force the usage of the default
    *PyYAML* loader/dumper instead of *HiYaPyCo*\ s implementation of a
    OrderedDict loader/dumper (see: Ordered Dict Yaml Loader / Dumper
    aka. ODYLDo) (default: ``False``)
 
+- ``dereferenceyamlanchors``: boolean : dereference yaml anchors and use a copy (default: ``True``)
+
 - ``encoding``: string : encoding used to read yaml files (default: ``utf-8``)
 
 -  ``failonmissingfiles``: boolean : fail if a supplied YAML file can
    not be found (default: ``True``)
 
 -  ``loglevel``: int : loglevel for the hiyapyco logger; should be one
    of the valid levels from ``logging``: 'WARN', 'ERROR', 'DEBUG', 'I
@@ -327,15 +325,21 @@
 Foundation.
 See
 `https://www.gnu.org/licenses/gpl.html <https://www.gnu.org/licenses/gpl.html>`_
 
 Changelog
 ---------
 
-0.5.5
+0.6.0
+~~~~~~
+
+FIXED: #69 (weird merge behavior with anchors)
+MERGED: #71 (dereference anchors)
+
+0.5.6
 ~~~~~~
 
 MERGED: #70 by itachi-cracker
 
 FIXED: #61 (removed deprecated distutils)
 
 0.5.5
```

### Comparing `HiYaPyCo-0.5.6/hiyapyco/__init__.py` & `HiYaPyCo-0.6.0/hiyapyco/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from __future__ import unicode_literals
 
 import sys
 import os
 import logging
 import re
 import io
+import copy
 import yaml
 from yaml import parser
 from jinja2 import Environment, Undefined, DebugUndefined, StrictUndefined, TemplateError
 
 from . import odyldo
 
 __all__ = [
@@ -77,14 +78,15 @@
           * method: one of
             hiyapyco.METHOD_SIMPLE | hiyapyco.METHOD_MERGE | hiyapyco.METHOD_SUBSTITUTE
           * mergelists: boolean (default: True) try to merge lists
             (only makes sense if hiyapyco.METHOD_MERGE or hiyapyco.METHOD_SUBSTITUTE)
           * interpolate: boolean (default: False)
           * castinterpolated: boolean (default: False) try to cast values after interpolating
           * usedefaultyamlloader: boolean (default: False)
+          * dereferenceyamlanchors: boolean (default: True)
           * encoding: (default: 'utf-8') encoding used to read yaml files
           * loglevel: one of  the valid levels from the logging module
           * failonmissingfiles: boolean (default: True)
           * loglevelmissingfiles
 
         Returns a representation of the merged and (if requested) interpolated config.
         Will mostly be a OrderedDict (dict if usedefaultyamlloader), but can be of any other type,
@@ -141,14 +143,24 @@
                         'value of "usedefaultyamlloader" must be boolean (got: "%s" as %s)' %
                         (kwargs['usedefaultyamlloader'], type(kwargs['usedefaultyamlloader']),)
                         )
             global _USEDEFAULTYAMLLOADER
             _USEDEFAULTYAMLLOADER = kwargs['usedefaultyamlloader']
             del kwargs['usedefaultyamlloader']
 
+        self.dereferenceyamlanchors = True
+        if 'dereferenceyamlanchors' in kwargs:
+            if not isinstance(kwargs['dereferenceyamlanchors'], bool):
+                raise HiYaPyCoInvocationException(
+                        'value of "dereferenceyamlanchors" must be boolean (got: "%s" as %s)' %
+                        (kwargs['dereferenceyamlanchors'], type(kwargs['dereferenceyamlanchors']),)
+                        )
+            self.dereferenceyamlanchors = bool(kwargs['dereferenceyamlanchors'])
+            del kwargs['dereferenceyamlanchors']
+
         self.failonmissingfiles = True
         if 'failonmissingfiles' in kwargs:
             if not isinstance(kwargs['failonmissingfiles'], bool):
                 raise HiYaPyCoInvocationException(
                         'value of "failonmissingfiles" must be boolean (got: "%s" as %s)' %
                         (kwargs['failonmissingfiles'], type(kwargs['failonmissingfiles']),)
                         )
@@ -301,14 +313,17 @@
                             si = int(si)
                     except ValueError:
                         pass
             logger.debug('interpolated "%s" to "%s" (type: %s)' % (s, si, type(si),))
         return si
 
     def _simplemerge(self, a, b):
+        if self.dereferenceyamlanchors:
+            a = copy.deepcopy(a)
+            b = copy.deepcopy(b)
         logger.debug('simplemerge %s (%s) and %s (%s)' % (a, type(a), b, type(b),))
         # FIXME: make None usage configurable
         if b is None:
             logger.debug('pass as b is None')
             pass
         elif isinstance(b, primitiveTypes):
             logger.debug('simplemerge: primitiveTypes replace a "%s"  w/ b "%s"' % (a, b,))
@@ -336,14 +351,17 @@
             raise HiYaPyCoImplementationException(
                     'can not (simple)merge %s to %s (@ "%s" try to merge "%s")' %
                     (type(b), type(a), a, b,)
                     )
         return a
 
     def _substmerge(self, a, b):
+        if self.dereferenceyamlanchors:
+            a = copy.deepcopy(a)
+            b = copy.deepcopy(b)
         logger.debug('>' * 30)
         logger.debug('substmerge %s and %s' % (a, b,))
         # FIXME: make None usage configurable
         if b is None:
             logger.debug('pass as b is None')
             pass
 
@@ -384,14 +402,17 @@
                 )
         logger.debug('end substmerge part: return: "%s"' % a)
         logger.debug('<' * 30)
         return a
 
     def _deepmerge(self, a, b):
         logger.debug('>'*30)
+        if self.dereferenceyamlanchors:
+            a = copy.deepcopy(a)
+            b = copy.deepcopy(b)
         logger.debug('deepmerge %s and %s' % (a, b,))
         # FIXME: make None usage configurable
         if b is None:
             logger.debug('pass as b is None')
             pass
         if a is None or isinstance(b, primitiveTypes):
             logger.debug('deepmerge: replace a "%s"  w/ b "%s"' % (a, b,))
```

### Comparing `HiYaPyCo-0.5.6/hiyapyco/odyldo.py` & `HiYaPyCo-0.6.0/hiyapyco/odyldo.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.6/setup.py` & `HiYaPyCo-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 from setuptools import setup
 
 basepath = os.path.dirname(os.path.realpath(__file__))
 sys.path.insert(0, os.path.dirname(basepath))
 
-HIYAPYCOVERSION='0.5.6'
+HIYAPYCOVERSION='0.6.0'
 
 long_description = open('README.rst').read()
 
 installrequires = [
     'PyYAML<7',
     'Jinja2>3,<4',
     'MarkupSafe<3'
```

### Comparing `HiYaPyCo-0.5.6/test/test_castinterpolated.py` & `HiYaPyCo-0.6.0/test/test_castinterpolated.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.6/test/test_interpolation.py` & `HiYaPyCo-0.6.0/test/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.6/test/test_interpolationunicode.py` & `HiYaPyCo-0.6.0/test/test_interpolationunicode.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.6/test/test_invocation.py` & `HiYaPyCo-0.6.0/test/test_invocation.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.6/test/test_merge.py` & `HiYaPyCo-0.6.0/test/test_merge.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.6/test/test_missingfiles.py` & `HiYaPyCo-0.6.0/test/test_missingfiles.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.6/test/test_multiple.py` & `HiYaPyCo-0.6.0/test/test_multiple.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.6/test/test_odict.py` & `HiYaPyCo-0.6.0/test/test_odict.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.6/test/test_simple.py` & `HiYaPyCo-0.6.0/test/test_simple.py`

 * *Files identical despite different names*

