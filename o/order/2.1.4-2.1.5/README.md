# Comparing `tmp/order-2.1.4.tar.gz` & `tmp/order-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "order-2.1.4.tar", last modified: Thu Jul 20 08:44:05 2023, max compression
+gzip compressed data, was "order-2.1.5.tar", last modified: Fri May 24 05:29:26 2024, max compression
```

## Comparing `order-2.1.4.tar` & `order-2.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:44:05.089727 order-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-20 08:43:54.000000 order-2.1.4/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-20 08:43:54.000000 order-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-20 08:43:54.000000 order-2.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-20 08:44:05.089727 order-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-20 08:43:54.000000 order-2.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:44:05.089727 order-2.1.4/order/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-20 08:43:54.000000 order-2.1.4/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-20 08:43:54.000000 order-2.1.4/order/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-20 08:43:54.000000 order-2.1.4/order/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-07-20 08:43:54.000000 order-2.1.4/order/category.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-20 08:43:54.000000 order-2.1.4/order/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-07-20 08:43:54.000000 order-2.1.4/order/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    43464 2023-07-20 08:43:54.000000 order-2.1.4/order/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-07-20 08:43:54.000000 order-2.1.4/order/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-07-20 08:43:54.000000 order-2.1.4/order/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    50840 2023-07-20 08:43:54.000000 order-2.1.4/order/unique.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-07-20 08:43:54.000000 order-2.1.4/order/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-07-20 08:43:54.000000 order-2.1.4/order/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:44:05.089727 order-2.1.4/order.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-20 08:44:05.000000 order-2.1.4/order.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-20 08:44:05.000000 order-2.1.4/order.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:44:05.000000 order-2.1.4/order.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:44:05.000000 order-2.1.4/order.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 08:44:05.000000 order-2.1.4/order.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 08:44:05.000000 order-2.1.4/order.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 08:43:54.000000 order-2.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:44:05.089727 order-2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-20 08:43:54.000000 order-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:29:26.598864 order-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-24 05:29:19.000000 order-2.1.5/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-24 05:29:19.000000 order-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-24 05:29:19.000000 order-2.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-24 05:29:26.598864 order-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-24 05:29:19.000000 order-2.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:29:26.594864 order-2.1.5/order/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-24 05:29:19.000000 order-2.1.5/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-24 05:29:19.000000 order-2.1.5/order/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-24 05:29:19.000000 order-2.1.5/order/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11736 2024-05-24 05:29:19.000000 order-2.1.5/order/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-05-24 05:29:19.000000 order-2.1.5/order/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-05-24 05:29:19.000000 order-2.1.5/order/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43464 2024-05-24 05:29:19.000000 order-2.1.5/order/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-24 05:29:19.000000 order-2.1.5/order/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-05-24 05:29:19.000000 order-2.1.5/order/shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50840 2024-05-24 05:29:19.000000 order-2.1.5/order/unique.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-05-24 05:29:19.000000 order-2.1.5/order/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20429 2024-05-24 05:29:19.000000 order-2.1.5/order/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:29:26.598864 order-2.1.5/order.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-24 05:29:26.000000 order-2.1.5/order.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-24 05:29:26.000000 order-2.1.5/order.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 05:29:26.000000 order-2.1.5/order.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 05:29:26.000000 order-2.1.5/order.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 05:29:26.000000 order-2.1.5/order.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 05:29:26.000000 order-2.1.5/order.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 05:29:19.000000 order-2.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 05:29:26.598864 order-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-24 05:29:19.000000 order-2.1.5/setup.py
```

### Comparing `order-2.1.4/LICENSE` & `order-2.1.5/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018-2021, Marcel Rieger
+Copyright (c) 2018-2024, Marcel Rieger
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `order-2.1.4/PKG-INFO` & `order-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: order
-Version: 2.1.4
+Version: 2.1.5
 Summary: Pythonic class collection that helps you structure external data from LHC / HEP experiments.
 Home-page: https://github.com/riga/order
 Author: Marcel Rieger
 Author-email: github.riga@icloud.com
 License: BSD-3-Clause
 Keywords: physics,analysis,experiment,order,structure,database,lhc,hep,alice,atlas,cms,lhcb
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: order Version: 2.1.4 Summary: Pythonic class
+Metadata-Version: 2.1 Name: order Version: 2.1.5 Summary: Pythonic class
 collection that helps you structure external data from LHC / HEP experiments.
 Home-page: https://github.com/riga/order Author: Marcel Rieger Author-email:
 github.riga@icloud.com License: BSD-3-Clause Keywords:
 physics,analysis,experiment,order,structure,database,lhc,hep,alice,atlas,cms,lhcb
 Platform: UNKNOWN Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 2 Classifier: Programming Language :: Python
 :: 2.7 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `order-2.1.4/README.md` & `order-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `order-2.1.4/order/__init__.py` & `order-2.1.5/order/__init__.py`

 * *Files identical despite different names*

### Comparing `order-2.1.4/order/analysis.py` & `order-2.1.5/order/analysis.py`

 * *Files identical despite different names*

### Comparing `order-2.1.4/order/category.py` & `order-2.1.5/order/category.py`

 * *Files identical despite different names*

### Comparing `order-2.1.4/order/config.py` & `order-2.1.5/order/config.py`

 * *Files identical despite different names*

### Comparing `order-2.1.4/order/dataset.py` & `order-2.1.5/order/dataset.py`

 * *Files identical despite different names*

### Comparing `order-2.1.4/order/mixins.py` & `order-2.1.5/order/mixins.py`

 * *Files identical despite different names*

### Comparing `order-2.1.4/order/process.py` & `order-2.1.5/order/process.py`

 * *Files identical despite different names*

### Comparing `order-2.1.4/order/shift.py` & `order-2.1.5/order/shift.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,19 +162,19 @@
         Flag denoting if the shift type is rate- and shape-changing.
     """
 
     cls_name_singular = "shift"
     cls_name_plural = "shifts"
 
     # nominal flag
-    NOMINAL = sn.Number.NOMINAL
+    NOMINAL = str(sn.Number.NOMINAL)
 
     # shift directions
-    UP = sn.Number.UP
-    DOWN = sn.Number.DOWN
+    UP = str(sn.Number.UP)
+    DOWN = str(sn.Number.DOWN)
 
     # shift types
     RATE = "rate"
     SHAPE = "shape"
     RATE_SHAPE = "rate_shape"
 
     # attributes for copying
```

### Comparing `order-2.1.4/order/unique.py` & `order-2.1.5/order/unique.py`

 * *Files identical despite different names*

### Comparing `order-2.1.4/order/util.py` & `order-2.1.5/order/util.py`

 * *Files identical despite different names*

### Comparing `order-2.1.4/order/variable.py` & `order-2.1.5/order/variable.py`

 * *Files identical despite different names*

### Comparing `order-2.1.4/order.egg-info/PKG-INFO` & `order-2.1.5/order.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: order
-Version: 2.1.4
+Version: 2.1.5
 Summary: Pythonic class collection that helps you structure external data from LHC / HEP experiments.
 Home-page: https://github.com/riga/order
 Author: Marcel Rieger
 Author-email: github.riga@icloud.com
 License: BSD-3-Clause
 Keywords: physics,analysis,experiment,order,structure,database,lhc,hep,alice,atlas,cms,lhcb
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: order Version: 2.1.4 Summary: Pythonic class
+Metadata-Version: 2.1 Name: order Version: 2.1.5 Summary: Pythonic class
 collection that helps you structure external data from LHC / HEP experiments.
 Home-page: https://github.com/riga/order Author: Marcel Rieger Author-email:
 github.riga@icloud.com License: BSD-3-Clause Keywords:
 physics,analysis,experiment,order,structure,database,lhc,hep,alice,atlas,cms,lhcb
 Platform: UNKNOWN Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 2 Classifier: Programming Language :: Python
 :: 2.7 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `order-2.1.4/setup.py` & `order-2.1.5/setup.py`

 * *Files identical despite different names*

