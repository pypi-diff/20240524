# Comparing `tmp/smartpasslib-0.4.1.tar.gz` & `tmp/smartpasslib-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartpasslib-0.4.1.tar", last modified: Sat May 18 07:47:44 2024, max compression
+gzip compressed data, was "smartpasslib-0.4.2.tar", last modified: Fri May 24 03:23:33 2024, max compression
```

## Comparing `smartpasslib-0.4.1.tar` & `smartpasslib-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-18 07:47:44.565972 smartpasslib-0.4.1/
--rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-18 07:36:22.000000 smartpasslib-0.4.1/LICENSE
--rw-r--r--   0 smart     (1000) smart     (1000)      139 2024-05-18 07:46:48.000000 smartpasslib-0.4.1/MANIFEST.in
--rw-r--r--   0 smart     (1000) smart     (1000)     3832 2024-05-18 07:47:44.565972 smartpasslib-0.4.1/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)     2599 2024-05-18 07:44:43.000000 smartpasslib-0.4.1/README.md
--rw-r--r--   0 smart     (1000) smart     (1000)       18 2024-05-18 07:38:01.000000 smartpasslib-0.4.1/requirements.txt
--rw-r--r--   0 smart     (1000) smart     (1000)     1271 2024-05-18 07:47:44.569306 smartpasslib-0.4.1/setup.cfg
--rw-r--r--   0 smart     (1000) smart     (1000)      387 2024-05-18 07:36:22.000000 smartpasslib-0.4.1/setup.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-18 07:47:44.562639 smartpasslib-0.4.1/smartpasslib/
--rw-r--r--   0 smart     (1000) smart     (1000)      371 2024-05-18 07:38:01.000000 smartpasslib-0.4.1/smartpasslib/__init__.py
--rw-r--r--   0 smart     (1000) smart     (1000)     2866 2024-05-18 07:44:43.000000 smartpasslib-0.4.1/smartpasslib/generators.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-18 07:47:44.565972 smartpasslib-0.4.1/smartpasslib.egg-info/
--rw-r--r--   0 smart     (1000) smart     (1000)     3832 2024-05-18 07:47:44.000000 smartpasslib-0.4.1/smartpasslib.egg-info/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)      339 2024-05-18 07:47:44.000000 smartpasslib-0.4.1/smartpasslib.egg-info/SOURCES.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-18 07:47:44.000000 smartpasslib-0.4.1/smartpasslib.egg-info/dependency_links.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-18 07:47:44.000000 smartpasslib-0.4.1/smartpasslib.egg-info/not-zip-safe
--rw-r--r--   0 smart     (1000) smart     (1000)       19 2024-05-18 07:47:44.000000 smartpasslib-0.4.1/smartpasslib.egg-info/requires.txt
--rw-r--r--   0 smart     (1000) smart     (1000)       13 2024-05-18 07:47:44.000000 smartpasslib-0.4.1/smartpasslib.egg-info/top_level.txt
--rw-r--r--   0 smart     (1000) smart     (1000)      103 2024-05-18 07:36:22.000000 smartpasslib-0.4.1/tox.ini
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-24 03:23:33.284108 smartpasslib-0.4.2/
+-rw-r--r--   0 smart     (1000) smart     (1000)     1499 2024-05-24 03:21:47.000000 smartpasslib-0.4.2/LICENSE
+-rw-r--r--   0 smart     (1000) smart     (1000)      139 2024-05-18 07:46:48.000000 smartpasslib-0.4.2/MANIFEST.in
+-rw-r--r--   0 smart     (1000) smart     (1000)     3835 2024-05-24 03:23:33.284108 smartpasslib-0.4.2/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)     2601 2024-05-24 03:21:47.000000 smartpasslib-0.4.2/README.md
+-rw-r--r--   0 smart     (1000) smart     (1000)       18 2024-05-24 03:21:47.000000 smartpasslib-0.4.2/requirements.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)     1272 2024-05-24 03:23:33.284108 smartpasslib-0.4.2/setup.cfg
+-rw-r--r--   0 smart     (1000) smart     (1000)      388 2024-05-24 03:21:47.000000 smartpasslib-0.4.2/setup.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-24 03:23:33.277441 smartpasslib-0.4.2/smartpasslib/
+-rw-r--r--   0 smart     (1000) smart     (1000)      372 2024-05-24 03:21:47.000000 smartpasslib-0.4.2/smartpasslib/__init__.py
+-rw-r--r--   0 smart     (1000) smart     (1000)     2884 2024-05-24 03:21:47.000000 smartpasslib-0.4.2/smartpasslib/generators.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-24 03:23:33.280774 smartpasslib-0.4.2/smartpasslib.egg-info/
+-rw-r--r--   0 smart     (1000) smart     (1000)     3835 2024-05-24 03:23:33.000000 smartpasslib-0.4.2/smartpasslib.egg-info/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)      339 2024-05-24 03:23:33.000000 smartpasslib-0.4.2/smartpasslib.egg-info/SOURCES.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-24 03:23:33.000000 smartpasslib-0.4.2/smartpasslib.egg-info/dependency_links.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-24 03:23:33.000000 smartpasslib-0.4.2/smartpasslib.egg-info/not-zip-safe
+-rw-r--r--   0 smart     (1000) smart     (1000)       19 2024-05-24 03:23:33.000000 smartpasslib-0.4.2/smartpasslib.egg-info/requires.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)       13 2024-05-24 03:23:33.000000 smartpasslib-0.4.2/smartpasslib.egg-info/top_level.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)      103 2024-05-18 07:36:22.000000 smartpasslib-0.4.2/tox.ini
```

### Comparing `smartpasslib-0.4.1/LICENSE` & `smartpasslib-0.4.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2024, A.A Suvorov
+Copyright (c) 2024, A.A. Suvorov
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `smartpasslib-0.4.1/PKG-INFO` & `smartpasslib-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: smartpasslib
-Version: 0.4.1
+Version: 0.4.2
 Summary: 'Cross-platform library for generating smart passwords.'
 Home-page: https://github.com/smartlegionlab
-Author: A.A Suvorov
+Author: A.A. Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartpasslib/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartpasslib/releases
 Keywords: smart password,smart pass gen,smart password generator,smartlegionlab
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -20,17 +20,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: smartrandom~=0.1.1
+Requires-Dist: smartrandom==0.1.1
 
-# Smart Passwords Library <sup>v0.4.1</sup>
+# Smart Passwords Library <sup>v0.4.2</sup>
 
 ***
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartpasslib)](https://github.com/smartlegionlab/smartpasslib/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartpasslib?label=pypi%20downloads)](https://pypi.org/project/smartpasslib/)
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartpasslib)
 [![PyPI](https://img.shields.io/pypi/v/smartpasslib)](https://pypi.org/project/smartpasslib)
@@ -40,15 +40,15 @@
 ***
 
 ## Short Description:
 ___smartpasslib___ - Cross-platform library for generating smart passwords.
 
 ***
 
-Author and developer: ___A.A Suvorov.___
+Author and developer: ___A.A. Suvorov.___
 
 ***
 
 ## Supported:
 
 - Linux: All.
 - Windows: 7/8/10.
@@ -98,9 +98,9 @@
     OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
     OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ***
 
     Licensed under the terms of the BSD 3-Clause License
     (see LICENSE for details).
-    Copyright © 2018-2024, A.A Suvorov
+    Copyright © 2018-2024, A.A. Suvorov
     All rights reserved.
```

### Comparing `smartpasslib-0.4.1/README.md` & `smartpasslib-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Smart Passwords Library <sup>v0.4.1</sup>
+# Smart Passwords Library <sup>v0.4.2</sup>
 
 ***
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartpasslib)](https://github.com/smartlegionlab/smartpasslib/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartpasslib?label=pypi%20downloads)](https://pypi.org/project/smartpasslib/)
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartpasslib)
 [![PyPI](https://img.shields.io/pypi/v/smartpasslib)](https://pypi.org/project/smartpasslib)
@@ -12,15 +12,15 @@
 ***
 
 ## Short Description:
 ___smartpasslib___ - Cross-platform library for generating smart passwords.
 
 ***
 
-Author and developer: ___A.A Suvorov.___
+Author and developer: ___A.A. Suvorov.___
 
 ***
 
 ## Supported:
 
 - Linux: All.
 - Windows: 7/8/10.
@@ -70,9 +70,9 @@
     OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
     OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ***
 
     Licensed under the terms of the BSD 3-Clause License
     (see LICENSE for details).
-    Copyright © 2018-2024, A.A Suvorov
+    Copyright © 2018-2024, A.A. Suvorov
     All rights reserved.
```

### Comparing `smartpasslib-0.4.1/setup.cfg` & `smartpasslib-0.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = smartpasslib
 version = attr: smartpasslib.__version__
-author = A.A Suvorov
+author = A.A. Suvorov
 author_email = smartlegiondev@gmail.com
 description = 'Cross-platform library for generating smart passwords.'
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/smartlegionlab
 project_urls = 
 	Documentation = https://github.com/smartlegionlab/smartpasslib/blob/master/README.md
@@ -32,13 +32,13 @@
 
 [options]
 python_requires = >=3.6
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
-	smartrandom~=0.1.1
+	smartrandom==0.1.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `smartpasslib-0.4.1/smartpasslib/generators.py` & `smartpasslib-0.4.2/smartpasslib/generators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------
 # Licensed under the terms of the BSD 3-Clause License
 # (see LICENSE for details).
-# Copyright © 2018-2024, A.A Suvorov
+# Copyright © 2018-2024, A.A. Suvorov
 # All rights reserved.
 # --------------------------------------------------------
 """Smart Random Generators"""
 import random
 
 from smartrandom.random_master import RandomStringMaster, HashMaster, UrandomGen
 
@@ -71,14 +71,15 @@
     key_gen = SmartKeyGen()
     smart_pass_gen = BaseSmartPassGen()
 
     @classmethod
     def get_password(cls, length=10):
         return cls.random_master.create_string(length)
 
+    @classmethod
     def get_default_password(cls, secret='', length=10):
         return cls.get_smart_password(secret=secret, length=length)
 
     @classmethod
     def get_smart_password(cls, login='', secret='', length=10):
         seed = cls.key_gen.get_private_key(login, secret)
         return cls.smart_pass_gen.generate(seed, length=length)
```

### Comparing `smartpasslib-0.4.1/smartpasslib.egg-info/PKG-INFO` & `smartpasslib-0.4.2/smartpasslib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: smartpasslib
-Version: 0.4.1
+Version: 0.4.2
 Summary: 'Cross-platform library for generating smart passwords.'
 Home-page: https://github.com/smartlegionlab
-Author: A.A Suvorov
+Author: A.A. Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartpasslib/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartpasslib/releases
 Keywords: smart password,smart pass gen,smart password generator,smartlegionlab
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -20,17 +20,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: smartrandom~=0.1.1
+Requires-Dist: smartrandom==0.1.1
 
-# Smart Passwords Library <sup>v0.4.1</sup>
+# Smart Passwords Library <sup>v0.4.2</sup>
 
 ***
 
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smartpasslib)](https://github.com/smartlegionlab/smartpasslib/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smartpasslib?label=pypi%20downloads)](https://pypi.org/project/smartpasslib/)
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smartpasslib)
 [![PyPI](https://img.shields.io/pypi/v/smartpasslib)](https://pypi.org/project/smartpasslib)
@@ -40,15 +40,15 @@
 ***
 
 ## Short Description:
 ___smartpasslib___ - Cross-platform library for generating smart passwords.
 
 ***
 
-Author and developer: ___A.A Suvorov.___
+Author and developer: ___A.A. Suvorov.___
 
 ***
 
 ## Supported:
 
 - Linux: All.
 - Windows: 7/8/10.
@@ -98,9 +98,9 @@
     OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
     OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ***
 
     Licensed under the terms of the BSD 3-Clause License
     (see LICENSE for details).
-    Copyright © 2018-2024, A.A Suvorov
+    Copyright © 2018-2024, A.A. Suvorov
     All rights reserved.
```

