# Comparing `tmp/nlpx-0.9.0.tar.gz` & `tmp/nlpx-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-0.9.0.tar", last modified: Fri May 24 03:26:25 2024, max compression
+gzip compressed data, was "nlpx-1.0.0.tar", last modified: Fri May 24 03:33:32 2024, max compression
```

## Comparing `nlpx-0.9.0.tar` & `nlpx-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:26:25.440696 nlpx-0.9.0/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 03:26:25.439942 nlpx-0.9.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-0.9.0/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:26:25.426806 nlpx-0.9.0/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-0.9.0/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:26:25.438819 nlpx-0.9.0/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-23 12:28:24.000000 nlpx-0.9.0/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2639 2024-05-24 03:18:24.000000 nlpx-0.9.0/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)     3681 2024-05-24 03:25:51.000000 nlpx-0.9.0/nlpx/models/_trainer.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-0.9.0/nlpx/text_token.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:26:25.433972 nlpx-0.9.0/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 03:26:25.000000 nlpx-0.9.0/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      267 2024-05-24 03:26:25.000000 nlpx-0.9.0/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 03:26:25.000000 nlpx-0.9.0/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 03:26:25.000000 nlpx-0.9.0/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 03:26:25.000000 nlpx-0.9.0/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 03:26:25.440952 nlpx-0.9.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 03:26:18.000000 nlpx-0.9.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:33:32.793537 nlpx-1.0.0/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 03:33:32.792742 nlpx-1.0.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.0.0/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:33:32.783513 nlpx-1.0.0/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.0.0/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:33:32.791689 nlpx-1.0.0/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       76 2024-05-24 03:33:06.000000 nlpx-1.0.0/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2639 2024-05-24 03:18:24.000000 nlpx-1.0.0/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)     3681 2024-05-24 03:25:51.000000 nlpx-1.0.0/nlpx/models/_trainer.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.0.0/nlpx/text_token.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:33:32.788964 nlpx-1.0.0/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 03:33:32.000000 nlpx-1.0.0/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      267 2024-05-24 03:33:32.000000 nlpx-1.0.0/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 03:33:32.000000 nlpx-1.0.0/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 03:26:25.000000 nlpx-1.0.0/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 03:33:32.000000 nlpx-1.0.0/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 03:33:32.793789 nlpx-1.0.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 03:33:23.000000 nlpx-1.0.0/setup.py
```

### Comparing `nlpx-0.9.0/PKG-INFO` & `nlpx-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.9.0
+Version: 1.0.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-0.9.0/nlpx/models/_text_cnn.py` & `nlpx-1.0.0/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-0.9.0/nlpx/models/_trainer.py` & `nlpx-1.0.0/nlpx/models/_trainer.py`

 * *Files identical despite different names*

### Comparing `nlpx-0.9.0/nlpx/text_token.py` & `nlpx-1.0.0/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-0.9.0/nlpx.egg-info/PKG-INFO` & `nlpx-1.0.0/nlpx.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.9.0
+Version: 1.0.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-0.9.0/setup.py` & `nlpx-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.0',
+    version='1.0.0',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

