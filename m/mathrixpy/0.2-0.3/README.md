# Comparing `tmp/mathrixpy-0.2.tar.gz` & `tmp/mathrixpy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathrixpy-0.2.tar", last modified: Fri May 24 04:13:57 2024, max compression
+gzip compressed data, was "mathrixpy-0.3.tar", last modified: Fri May 24 04:19:15 2024, max compression
```

## Comparing `mathrixpy-0.2.tar` & `mathrixpy-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 04:13:57.130608 mathrixpy-0.2/
--rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-0.2/LICENSE
--rw-rw-rw-   0        0        0      467 2024-05-24 04:13:57.129621 mathrixpy-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       13 2024-05-24 02:34:08.000000 mathrixpy-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 04:13:57.111559 mathrixpy-0.2/mathrixpy/
--rw-rw-rw-   0        0        0       40 2024-05-24 04:11:26.000000 mathrixpy-0.2/mathrixpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 04:13:57.127603 mathrixpy-0.2/mathrixpy.egg-info/
--rw-rw-rw-   0        0        0      467 2024-05-24 04:13:57.000000 mathrixpy-0.2/mathrixpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-24 04:13:57.000000 mathrixpy-0.2/mathrixpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 04:13:57.000000 mathrixpy-0.2/mathrixpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-24 04:13:57.000000 mathrixpy-0.2/mathrixpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-24 04:13:57.133613 mathrixpy-0.2/setup.cfg
--rw-rw-rw-   0        0        0      620 2024-05-24 04:12:06.000000 mathrixpy-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 04:19:15.615533 mathrixpy-0.3/
+-rw-rw-rw-   0        0        0     1087 2024-05-24 02:28:32.000000 mathrixpy-0.3/LICENSE
+-rw-rw-rw-   0        0        0      467 2024-05-24 04:19:15.614520 mathrixpy-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2024-05-24 02:34:08.000000 mathrixpy-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 04:19:15.597606 mathrixpy-0.3/mathrixpy/
+-rw-rw-rw-   0        0        0       25 2024-05-24 04:18:07.000000 mathrixpy-0.3/mathrixpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 04:19:15.612520 mathrixpy-0.3/mathrixpy.egg-info/
+-rw-rw-rw-   0        0        0      467 2024-05-24 04:19:15.000000 mathrixpy-0.3/mathrixpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-24 04:19:15.000000 mathrixpy-0.3/mathrixpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 04:19:15.000000 mathrixpy-0.3/mathrixpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 04:19:15.000000 mathrixpy-0.3/mathrixpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-24 04:19:15.616531 mathrixpy-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      620 2024-05-24 04:17:34.000000 mathrixpy-0.3/setup.py
```

### Comparing `mathrixpy-0.2/LICENSE` & `mathrixpy-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mathrixpy-0.2/setup.py` & `mathrixpy-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mathrixpy",
-    version="0.2",
+    version="0.3",
     author="AmJoJADeOrg",
     license='MIT',
     author_email="glroberto1810@gmail.com",
     description="Operaciones con matrices",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Ampere-G/mathrixPy",
```

