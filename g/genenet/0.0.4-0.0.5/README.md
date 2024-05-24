# Comparing `tmp/genenet-0.0.4.tar.gz` & `tmp/genenet-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genenet-0.0.4.tar", last modified: Tue May 14 13:30:36 2024, max compression
+gzip compressed data, was "genenet-0.0.5.tar", last modified: Fri May 24 01:12:41 2024, max compression
```

## Comparing `genenet-0.0.4.tar` & `genenet-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 13:30:36.184022 genenet-0.0.4/
--rw-rw-rw-   0        0        0     8250 2024-05-14 13:30:36.182015 genenet-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     7622 2024-05-08 12:32:33.000000 genenet-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 13:30:36.179769 genenet-0.0.4/genenet.egg-info/
--rw-rw-rw-   0        0        0     8250 2024-05-14 13:30:35.000000 genenet-0.0.4/genenet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      142 2024-05-14 13:30:36.000000 genenet-0.0.4/genenet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 13:30:36.000000 genenet-0.0.4/genenet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 13:30:36.000000 genenet-0.0.4/genenet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 13:30:36.185470 genenet-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      689 2024-05-14 13:29:58.000000 genenet-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 01:12:41.676492 genenet-0.0.5/
+-rw-rw-rw-   0        0        0     8250 2024-05-24 01:12:41.673492 genenet-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7622 2024-05-08 12:32:33.000000 genenet-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 01:12:41.671491 genenet-0.0.5/genenet.egg-info/
+-rw-rw-rw-   0        0        0     8250 2024-05-24 01:12:41.000000 genenet-0.0.5/genenet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2024-05-24 01:12:41.000000 genenet-0.0.5/genenet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 01:12:41.000000 genenet-0.0.5/genenet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 01:12:41.000000 genenet-0.0.5/genenet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 01:12:41.676492 genenet-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      689 2024-05-24 01:08:19.000000 genenet-0.0.5/setup.py
```

### Comparing `genenet-0.0.4/PKG-INFO` & `genenet-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genenet
-Version: 0.0.4
+Version: 0.0.5
 Summary: Constructing gene association networks using chromosomal conformational capture technology based on three-dimensional space (3D-GeneNet)
 Home-page: https://github.com/gaoyuanccc/3D-GeneNet
 Author: gaoyuan
 Author-email: 18434753515@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `genenet-0.0.4/README.md` & `genenet-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `genenet-0.0.4/genenet.egg-info/PKG-INFO` & `genenet-0.0.5/genenet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genenet
-Version: 0.0.4
+Version: 0.0.5
 Summary: Constructing gene association networks using chromosomal conformational capture technology based on three-dimensional space (3D-GeneNet)
 Home-page: https://github.com/gaoyuanccc/3D-GeneNet
 Author: gaoyuan
 Author-email: 18434753515@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `genenet-0.0.4/setup.py` & `genenet-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="genenet",
-    version="0.0.4",
+    version="0.0.5",
     author="gaoyuan",
     author_email="18434753515@163.com",
     description="Constructing gene association networks using chromosomal conformational capture technology based on three-dimensional space (3D-GeneNet)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyuanccc/3D-GeneNet",
     packages=setuptools.find_packages(),
```

