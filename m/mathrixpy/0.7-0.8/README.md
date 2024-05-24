# Comparing `tmp/mathrixpy-0.7.tar.gz` & `tmp/mathrixpy-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathrixpy-0.7.tar", last modified: Fri May 24 04:39:35 2024, max compression
+gzip compressed data, was "mathrixpy-0.8.tar", last modified: Fri May 24 04:48:27 2024, max compression
```

## Comparing `mathrixpy-0.7.tar` & `mathrixpy-0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 04:39:35.645862 mathrixpy-0.7/
--rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-0.7/LICENSE
--rw-rw-rw-   0        0        0      467 2024-05-24 04:39:35.644869 mathrixpy-0.7/PKG-INFO
--rw-rw-rw-   0        0        0       13 2024-05-24 02:34:08.000000 mathrixpy-0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 04:39:35.629826 mathrixpy-0.7/mathrixpy/
--rw-rw-rw-   0        0        0       40 2024-05-24 04:35:23.000000 mathrixpy-0.7/mathrixpy/__init__.py
--rw-rw-rw-   0        0        0     6038 2024-05-24 04:18:45.000000 mathrixpy-0.7/mathrixpy/base.py
--rw-rw-rw-   0        0        0     5906 2024-05-23 18:35:49.000000 mathrixpy-0.7/mathrixpy/cambios.py
-drwxrwxrwx   0        0        0        0 2024-05-24 04:39:35.643855 mathrixpy-0.7/mathrixpy.egg-info/
--rw-rw-rw-   0        0        0      467 2024-05-24 04:39:35.000000 mathrixpy-0.7/mathrixpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-05-24 04:39:35.000000 mathrixpy-0.7/mathrixpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 04:39:35.000000 mathrixpy-0.7/mathrixpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-24 04:39:35.000000 mathrixpy-0.7/mathrixpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-24 04:39:35.647989 mathrixpy-0.7/setup.cfg
--rw-rw-rw-   0        0        0      620 2024-05-24 04:38:02.000000 mathrixpy-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 04:48:27.591402 mathrixpy-0.8/
+-rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-0.8/LICENSE
+-rw-rw-rw-   0        0        0      467 2024-05-24 04:48:27.590399 mathrixpy-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2024-05-24 02:34:08.000000 mathrixpy-0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 04:48:27.571872 mathrixpy-0.8/mathrixpy/
+-rw-rw-rw-   0        0        0       23 2024-05-24 04:47:17.000000 mathrixpy-0.8/mathrixpy/__init__.py
+-rw-rw-rw-   0        0        0     6038 2024-05-24 04:18:45.000000 mathrixpy-0.8/mathrixpy/base.py
+-rw-rw-rw-   0        0        0     5906 2024-05-23 18:35:49.000000 mathrixpy-0.8/mathrixpy/cambios.py
+drwxrwxrwx   0        0        0        0 2024-05-24 04:48:27.588400 mathrixpy-0.8/mathrixpy.egg-info/
+-rw-rw-rw-   0        0        0      467 2024-05-24 04:48:27.000000 mathrixpy-0.8/mathrixpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-24 04:48:27.000000 mathrixpy-0.8/mathrixpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 04:48:27.000000 mathrixpy-0.8/mathrixpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 04:48:27.000000 mathrixpy-0.8/mathrixpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-24 04:48:27.596465 mathrixpy-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      620 2024-05-24 04:47:51.000000 mathrixpy-0.8/setup.py
```

### Comparing `mathrixpy-0.7/LICENSE` & `mathrixpy-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mathrixpy-0.7/mathrixpy/base.py` & `mathrixpy-0.8/mathrixpy/base.py`

 * *Files identical despite different names*

### Comparing `mathrixpy-0.7/mathrixpy/cambios.py` & `mathrixpy-0.8/mathrixpy/cambios.py`

 * *Files identical despite different names*

### Comparing `mathrixpy-0.7/setup.py` & `mathrixpy-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mathrixpy",
-    version="0.7",
+    version="0.8",
     author="AmJoJADeOrg",
     license='MIT',
     author_email="glroberto1810@gmail.com",
     description="Operaciones con matrices",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Ampere-G/mathrixPy",
```

