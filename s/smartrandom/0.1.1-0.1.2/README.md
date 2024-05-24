# Comparing `tmp/smartrandom-0.1.1.tar.gz` & `tmp/smartrandom-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartrandom-0.1.1.tar", last modified: Sat May 18 07:30:58 2024, max compression
+gzip compressed data, was "smartrandom-0.1.2.tar", last modified: Fri May 24 03:09:50 2024, max compression
```

## Comparing `smartrandom-0.1.1.tar` & `smartrandom-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-18 07:30:58.958706 smartrandom-0.1.1/
--rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-18 07:14:25.000000 smartrandom-0.1.1/LICENSE
--rw-r--r--   0 smart     (1000) smart     (1000)      123 2024-05-18 07:29:54.000000 smartrandom-0.1.1/MANIFEST.in
--rw-r--r--   0 smart     (1000) smart     (1000)     3706 2024-05-18 07:30:58.958706 smartrandom-0.1.1/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)     2679 2024-05-18 07:20:58.000000 smartrandom-0.1.1/README.md
--rw-r--r--   0 smart     (1000) smart     (1000)        0 2024-05-18 07:28:29.000000 smartrandom-0.1.1/requirements.txt
--rw-r--r--   0 smart     (1000) smart     (1000)     1215 2024-05-18 07:30:58.958706 smartrandom-0.1.1/setup.cfg
--rw-r--r--   0 smart     (1000) smart     (1000)      442 2024-05-18 07:14:25.000000 smartrandom-0.1.1/setup.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-18 07:30:58.955373 smartrandom-0.1.1/smartrandom/
--rw-r--r--   0 smart     (1000) smart     (1000)      621 2024-05-18 07:20:58.000000 smartrandom-0.1.1/smartrandom/__init__.py
--rw-r--r--   0 smart     (1000) smart     (1000)     2746 2024-05-18 07:17:00.000000 smartrandom-0.1.1/smartrandom/random_master.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-18 07:30:58.958706 smartrandom-0.1.1/smartrandom.egg-info/
--rw-r--r--   0 smart     (1000) smart     (1000)     3706 2024-05-18 07:30:58.000000 smartrandom-0.1.1/smartrandom.egg-info/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)      292 2024-05-18 07:30:58.000000 smartrandom-0.1.1/smartrandom.egg-info/SOURCES.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-18 07:30:58.000000 smartrandom-0.1.1/smartrandom.egg-info/dependency_links.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-18 07:30:58.000000 smartrandom-0.1.1/smartrandom.egg-info/not-zip-safe
--rw-r--r--   0 smart     (1000) smart     (1000)       12 2024-05-18 07:30:58.000000 smartrandom-0.1.1/smartrandom.egg-info/top_level.txt
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-24 03:09:50.441337 smartrandom-0.1.2/
+-rw-r--r--   0 smart     (1000) smart     (1000)     1499 2024-05-24 03:09:32.000000 smartrandom-0.1.2/LICENSE
+-rw-r--r--   0 smart     (1000) smart     (1000)      123 2024-05-18 07:29:54.000000 smartrandom-0.1.2/MANIFEST.in
+-rw-r--r--   0 smart     (1000) smart     (1000)     3711 2024-05-24 03:09:50.441337 smartrandom-0.1.2/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)     2683 2024-05-24 03:09:32.000000 smartrandom-0.1.2/README.md
+-rw-r--r--   0 smart     (1000) smart     (1000)        0 2024-05-18 07:28:29.000000 smartrandom-0.1.2/requirements.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)     1216 2024-05-24 03:09:50.441337 smartrandom-0.1.2/setup.cfg
+-rw-r--r--   0 smart     (1000) smart     (1000)      443 2024-05-24 03:09:32.000000 smartrandom-0.1.2/setup.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-24 03:09:50.438004 smartrandom-0.1.2/smartrandom/
+-rw-r--r--   0 smart     (1000) smart     (1000)      622 2024-05-24 03:09:32.000000 smartrandom-0.1.2/smartrandom/__init__.py
+-rw-r--r--   0 smart     (1000) smart     (1000)     2745 2024-05-24 03:00:55.000000 smartrandom-0.1.2/smartrandom/random_master.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-24 03:09:50.441337 smartrandom-0.1.2/smartrandom.egg-info/
+-rw-r--r--   0 smart     (1000) smart     (1000)     3711 2024-05-24 03:09:50.000000 smartrandom-0.1.2/smartrandom.egg-info/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)      292 2024-05-24 03:09:50.000000 smartrandom-0.1.2/smartrandom.egg-info/SOURCES.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-24 03:09:50.000000 smartrandom-0.1.2/smartrandom.egg-info/dependency_links.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-24 03:09:50.000000 smartrandom-0.1.2/smartrandom.egg-info/not-zip-safe
+-rw-r--r--   0 smart     (1000) smart     (1000)       12 2024-05-24 03:09:50.000000 smartrandom-0.1.2/smartrandom.egg-info/top_level.txt
```

### Comparing `smartrandom-0.1.1/LICENSE` & `smartrandom-0.1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, A.A Suvorov
+Copyright (c) 2024, A.A. Suvorov
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `smartrandom-0.1.1/PKG-INFO` & `smartrandom-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: smartrandom
-Version: 0.1.1
+Version: 0.1.2
 Summary: Random Data Generators.
 Home-page: https://github.com/smartlegionlab/smartrandom/
-Author: A.A Suvorov
+Author: A.A. Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartrandom/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartrandom/releases
 Keywords: password generator,code generator,random generator,random code generator,random string generator,random bytes generator,smartrandom,smartlegionlab
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -16,34 +16,34 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# smartrandom <sup>v0.1.1</sup>
+# smartrandom <sup>v0.1.2</sup>
 ---
 
 ## Random Data Generators:
 
-Allows you to generate random strings of a given length from letters, numbers, and symbols.
-Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
+>Allows you to generate random strings of a given length from letters, numbers, and symbols.
+>Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
 
 ---
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartrandom?label=pypi%20downloads)](https://pypi.org/project/smartrandom/)
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartrandom)
 [![PyPI](https://img.shields.io/pypi/v/smartrandom)](https://pypi.org/project/smartrandom)
 [![GitHub](https://img.shields.io/github/license/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/blob/master/LICENSE)
 [![PyPI - Format](https://img.shields.io/pypi/format/smartrandom)](https://pypi.org/project/smartrandom)
 
 ***
 
-Author and developer: ___A.A Suvorov.___
+Author and developer: ___A.A. Suvorov.___
 
 ***
 
 ## Help:
 
 `pip install smartrandom`
 
@@ -76,10 +76,10 @@
 
 ***
 
 ## Copyright:
     --------------------------------------------------------
     Licensed under the terms of the BSD 3-Clause License
     (see LICENSE for details).
-    Copyright © 2018-2024, A.A Suvorov
+    Copyright © 2018-2024, A.A. Suvorov
     All rights reserved.
     --------------------------------------------------------
```

### Comparing `smartrandom-0.1.1/README.md` & `smartrandom-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# smartrandom <sup>v0.1.1</sup>
+# smartrandom <sup>v0.1.2</sup>
 ---
 
 ## Random Data Generators:
 
-Allows you to generate random strings of a given length from letters, numbers, and symbols.
-Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
+>Allows you to generate random strings of a given length from letters, numbers, and symbols.
+>Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
 
 ---
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartrandom?label=pypi%20downloads)](https://pypi.org/project/smartrandom/)
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartrandom)
 [![PyPI](https://img.shields.io/pypi/v/smartrandom)](https://pypi.org/project/smartrandom)
 [![GitHub](https://img.shields.io/github/license/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/blob/master/LICENSE)
 [![PyPI - Format](https://img.shields.io/pypi/format/smartrandom)](https://pypi.org/project/smartrandom)
 
 ***
 
-Author and developer: ___A.A Suvorov.___
+Author and developer: ___A.A. Suvorov.___
 
 ***
 
 ## Help:
 
 `pip install smartrandom`
 
@@ -54,10 +54,10 @@
 
 ***
 
 ## Copyright:
     --------------------------------------------------------
     Licensed under the terms of the BSD 3-Clause License
     (see LICENSE for details).
-    Copyright © 2018-2024, A.A Suvorov
+    Copyright © 2018-2024, A.A. Suvorov
     All rights reserved.
     --------------------------------------------------------
```

### Comparing `smartrandom-0.1.1/setup.cfg` & `smartrandom-0.1.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = smartrandom
 version = attr: smartrandom.__version__
-author = A.A Suvorov
+author = A.A. Suvorov
 author_email = smartlegiondev@gmail.com
 description = Random Data Generators.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/smartlegionlab/smartrandom/
 project_urls = 
 	Documentation = https://github.com/smartlegionlab/smartrandom/blob/master/README.md
```

### Comparing `smartrandom-0.1.1/smartrandom/__init__.py` & `smartrandom-0.1.2/smartrandom/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # --------------------------------------------------------
 # Licensed under the terms of the BSD 3-Clause License
 # (see LICENSE for details).
-# Copyright © 2018-2024, A.A Suvorov
+# Copyright © 2018-2024, A.A. Suvorov
 # All rights reserved.
 # --------------------------------------------------------
 # https://github.com/smartlegionlab
 # --------------------------------------------------------
 """Smart Random - Random Data Generators.
 
 Allows you to generate random strings of a given length from letters, numbers, and symbols.
 Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
 """
-__version__ = '0.1.1'
+__version__ = '0.1.2'
```

### Comparing `smartrandom-0.1.1/smartrandom/random_master.py` & `smartrandom-0.1.2/smartrandom/random_master.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     @classmethod
     def create(cls, length=10):
         return ''.join((random.choice(cls.numbers) for _ in range(length)))
 
 
 class RandomSymbolsMaster:
-    symbols = '@$!%*#?&-'
+    symbols = '!@#$%&^_'
 
     @classmethod
     def create(cls, length=10):
         return ''.join((random.choice(cls.symbols) for _ in range(length)))
 
 
 class HashMaster:
```

### Comparing `smartrandom-0.1.1/smartrandom.egg-info/PKG-INFO` & `smartrandom-0.1.2/smartrandom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: smartrandom
-Version: 0.1.1
+Version: 0.1.2
 Summary: Random Data Generators.
 Home-page: https://github.com/smartlegionlab/smartrandom/
-Author: A.A Suvorov
+Author: A.A. Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartrandom/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartrandom/releases
 Keywords: password generator,code generator,random generator,random code generator,random string generator,random bytes generator,smartrandom,smartlegionlab
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -16,34 +16,34 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# smartrandom <sup>v0.1.1</sup>
+# smartrandom <sup>v0.1.2</sup>
 ---
 
 ## Random Data Generators:
 
-Allows you to generate random strings of a given length from letters, numbers, and symbols.
-Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
+>Allows you to generate random strings of a given length from letters, numbers, and symbols.
+>Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
 
 ---
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartrandom?label=pypi%20downloads)](https://pypi.org/project/smartrandom/)
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartrandom)
 [![PyPI](https://img.shields.io/pypi/v/smartrandom)](https://pypi.org/project/smartrandom)
 [![GitHub](https://img.shields.io/github/license/smartlegionlab/smartrandom)](https://github.com/smartlegionlab/smartrandom/blob/master/LICENSE)
 [![PyPI - Format](https://img.shields.io/pypi/format/smartrandom)](https://pypi.org/project/smartrandom)
 
 ***
 
-Author and developer: ___A.A Suvorov.___
+Author and developer: ___A.A. Suvorov.___
 
 ***
 
 ## Help:
 
 `pip install smartrandom`
 
@@ -76,10 +76,10 @@
 
 ***
 
 ## Copyright:
     --------------------------------------------------------
     Licensed under the terms of the BSD 3-Clause License
     (see LICENSE for details).
-    Copyright © 2018-2024, A.A Suvorov
+    Copyright © 2018-2024, A.A. Suvorov
     All rights reserved.
     --------------------------------------------------------
```

