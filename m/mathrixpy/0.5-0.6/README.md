# Comparing `tmp/mathrixpy-0.5.tar.gz` & `tmp/mathrixpy-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathrixpy-0.5.tar", last modified: Fri May 24 04:29:08 2024, max compression
+gzip compressed data, was "mathrixpy-0.6.tar", last modified: Fri May 24 04:31:56 2024, max compression
```

## Comparing `mathrixpy-0.5.tar` & `mathrixpy-0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 04:29:08.372407 mathrixpy-0.5/
--rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-0.5/LICENSE
--rw-rw-rw-   0        0        0      467 2024-05-24 04:29:08.372407 mathrixpy-0.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2024-05-24 02:34:08.000000 mathrixpy-0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 04:29:08.347612 mathrixpy-0.5/mathrixpy/
--rw-rw-rw-   0        0        0       54 2024-05-24 04:28:45.000000 mathrixpy-0.5/mathrixpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 04:29:08.369418 mathrixpy-0.5/mathrixpy/mathrixpybase/
--rw-rw-rw-   0        0        0       54 2024-05-24 04:28:45.000000 mathrixpy-0.5/mathrixpy/mathrixpybase/__init__.py
--rw-rw-rw-   0        0        0     6038 2024-05-24 04:18:45.000000 mathrixpy-0.5/mathrixpy/mathrixpybase/base.py
--rw-rw-rw-   0        0        0     5906 2024-05-23 18:35:49.000000 mathrixpy-0.5/mathrixpy/mathrixpybase/cambios.py
-drwxrwxrwx   0        0        0        0 2024-05-24 04:29:08.370413 mathrixpy-0.5/mathrixpy.egg-info/
--rw-rw-rw-   0        0        0      467 2024-05-24 04:29:08.000000 mathrixpy-0.5/mathrixpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-05-24 04:29:08.000000 mathrixpy-0.5/mathrixpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 04:29:08.000000 mathrixpy-0.5/mathrixpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-24 04:29:08.000000 mathrixpy-0.5/mathrixpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-24 04:29:08.374912 mathrixpy-0.5/setup.cfg
--rw-rw-rw-   0        0        0      620 2024-05-24 04:28:01.000000 mathrixpy-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 04:31:56.587624 mathrixpy-0.6/
+-rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-0.6/LICENSE
+-rw-rw-rw-   0        0        0      467 2024-05-24 04:31:56.587624 mathrixpy-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2024-05-24 02:34:08.000000 mathrixpy-0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 04:31:56.567375 mathrixpy-0.6/mathrixpy/
+-rw-rw-rw-   0        0        0       54 2024-05-24 04:28:45.000000 mathrixpy-0.6/mathrixpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 04:31:56.583498 mathrixpy-0.6/mathrixpy/mathrixpybase/
+-rw-rw-rw-   0        0        0       54 2024-05-24 04:28:45.000000 mathrixpy-0.6/mathrixpy/mathrixpybase/__init__.py
+-rw-rw-rw-   0        0        0     6038 2024-05-24 04:18:45.000000 mathrixpy-0.6/mathrixpy/mathrixpybase/base.py
+-rw-rw-rw-   0        0        0     5906 2024-05-23 18:35:49.000000 mathrixpy-0.6/mathrixpy/mathrixpybase/cambios.py
+drwxrwxrwx   0        0        0        0 2024-05-24 04:31:56.585601 mathrixpy-0.6/mathrixpy.egg-info/
+-rw-rw-rw-   0        0        0      467 2024-05-24 04:31:56.000000 mathrixpy-0.6/mathrixpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-05-24 04:31:56.000000 mathrixpy-0.6/mathrixpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 04:31:56.000000 mathrixpy-0.6/mathrixpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 04:31:56.000000 mathrixpy-0.6/mathrixpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-24 04:31:56.589610 mathrixpy-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      620 2024-05-24 04:31:42.000000 mathrixpy-0.6/setup.py
```

### Comparing `mathrixpy-0.5/LICENSE` & `mathrixpy-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mathrixpy-0.5/mathrixpy/mathrixpybase/base.py` & `mathrixpy-0.6/mathrixpy/mathrixpybase/base.py`

 * *Files identical despite different names*

### Comparing `mathrixpy-0.5/mathrixpy/mathrixpybase/cambios.py` & `mathrixpy-0.6/mathrixpy/mathrixpybase/cambios.py`

 * *Files identical despite different names*

### Comparing `mathrixpy-0.5/setup.py` & `mathrixpy-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mathrixpy",
-    version="0.5",
+    version="0.6",
     author="AmJoJADeOrg",
     license='MIT',
     author_email="glroberto1810@gmail.com",
     description="Operaciones con matrices",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Ampere-G/mathrixPy",
```

