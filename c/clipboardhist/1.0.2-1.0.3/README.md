# Comparing `tmp/clipboardhist-1.0.2.tar.gz` & `tmp/clipboardhist-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipboardhist-1.0.2.tar", last modified: Fri May 24 20:42:55 2024, max compression
+gzip compressed data, was "clipboardhist-1.0.3.tar", last modified: Fri May 24 20:52:05 2024, max compression
```

## Comparing `clipboardhist-1.0.2.tar` & `clipboardhist-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shiro      (501) staff       (20)        0 2024-05-24 20:42:55.502688 clipboardhist-1.0.2/
--rw-r--r--   0 shiro      (501) staff       (20)     1068 2024-05-24 17:25:54.000000 clipboardhist-1.0.2/LICENSE
--rw-r--r--   0 shiro      (501) staff       (20)      419 2024-05-24 20:42:55.502490 clipboardhist-1.0.2/PKG-INFO
--rw-r--r--   0 shiro      (501) staff       (20)      554 2024-05-24 19:22:55.000000 clipboardhist-1.0.2/README.md
-drwxr-xr-x   0 shiro      (501) staff       (20)        0 2024-05-24 20:42:55.501446 clipboardhist-1.0.2/clipboardhist/
--rw-r--r--   0 shiro      (501) staff       (20)      228 2024-05-24 20:35:38.000000 clipboardhist-1.0.2/clipboardhist/__init__.py
--rw-r--r--   0 shiro      (501) staff       (20)     2064 2024-05-24 18:57:22.000000 clipboardhist-1.0.2/clipboardhist/clipboardhist.py
-drwxr-xr-x   0 shiro      (501) staff       (20)        0 2024-05-24 20:42:55.502280 clipboardhist-1.0.2/clipboardhist.egg-info/
--rw-r--r--   0 shiro      (501) staff       (20)      419 2024-05-24 20:42:55.000000 clipboardhist-1.0.2/clipboardhist.egg-info/PKG-INFO
--rw-r--r--   0 shiro      (501) staff       (20)      267 2024-05-24 20:42:55.000000 clipboardhist-1.0.2/clipboardhist.egg-info/SOURCES.txt
--rw-r--r--   0 shiro      (501) staff       (20)        1 2024-05-24 20:42:55.000000 clipboardhist-1.0.2/clipboardhist.egg-info/dependency_links.txt
--rw-r--r--   0 shiro      (501) staff       (20)       10 2024-05-24 20:42:55.000000 clipboardhist-1.0.2/clipboardhist.egg-info/requires.txt
--rw-r--r--   0 shiro      (501) staff       (20)       14 2024-05-24 20:42:55.000000 clipboardhist-1.0.2/clipboardhist.egg-info/top_level.txt
--rw-r--r--   0 shiro      (501) staff       (20)       38 2024-05-24 20:42:55.502778 clipboardhist-1.0.2/setup.cfg
--rw-r--r--   0 shiro      (501) staff       (20)      557 2024-05-24 20:41:30.000000 clipboardhist-1.0.2/setup.py
+drwxr-xr-x   0 shiro      (501) staff       (20)        0 2024-05-24 20:52:05.714429 clipboardhist-1.0.3/
+-rw-r--r--   0 shiro      (501) staff       (20)     1068 2024-05-24 17:25:54.000000 clipboardhist-1.0.3/LICENSE
+-rw-r--r--   0 shiro      (501) staff       (20)      419 2024-05-24 20:52:05.714251 clipboardhist-1.0.3/PKG-INFO
+-rw-r--r--   0 shiro      (501) staff       (20)      554 2024-05-24 19:22:55.000000 clipboardhist-1.0.3/README.md
+drwxr-xr-x   0 shiro      (501) staff       (20)        0 2024-05-24 20:52:05.713094 clipboardhist-1.0.3/clipboardhist/
+-rw-r--r--   0 shiro      (501) staff       (20)      228 2024-05-24 20:35:38.000000 clipboardhist-1.0.3/clipboardhist/__init__.py
+-rw-r--r--   0 shiro      (501) staff       (20)     2064 2024-05-24 18:57:22.000000 clipboardhist-1.0.3/clipboardhist/clipboardhist.py
+drwxr-xr-x   0 shiro      (501) staff       (20)        0 2024-05-24 20:52:05.714022 clipboardhist-1.0.3/clipboardhist.egg-info/
+-rw-r--r--   0 shiro      (501) staff       (20)      419 2024-05-24 20:52:05.000000 clipboardhist-1.0.3/clipboardhist.egg-info/PKG-INFO
+-rw-r--r--   0 shiro      (501) staff       (20)      267 2024-05-24 20:52:05.000000 clipboardhist-1.0.3/clipboardhist.egg-info/SOURCES.txt
+-rw-r--r--   0 shiro      (501) staff       (20)        1 2024-05-24 20:52:05.000000 clipboardhist-1.0.3/clipboardhist.egg-info/dependency_links.txt
+-rw-r--r--   0 shiro      (501) staff       (20)       10 2024-05-24 20:52:05.000000 clipboardhist-1.0.3/clipboardhist.egg-info/requires.txt
+-rw-r--r--   0 shiro      (501) staff       (20)       14 2024-05-24 20:52:05.000000 clipboardhist-1.0.3/clipboardhist.egg-info/top_level.txt
+-rw-r--r--   0 shiro      (501) staff       (20)       38 2024-05-24 20:52:05.714488 clipboardhist-1.0.3/setup.cfg
+-rw-r--r--   0 shiro      (501) staff       (20)      557 2024-05-24 20:50:57.000000 clipboardhist-1.0.3/setup.py
```

### Comparing `clipboardhist-1.0.2/LICENSE` & `clipboardhist-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clipboardhist-1.0.2/README.md` & `clipboardhist-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `clipboardhist-1.0.2/clipboardhist/clipboardhist.py` & `clipboardhist-1.0.3/clipboardhist/clipboardhist.py`

 * *Files identical despite different names*

### Comparing `clipboardhist-1.0.2/setup.py` & `clipboardhist-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='clipboardhist',
-    version='1.0.2',
+    version='1.0.3',
     description='A simple clipboard history management tool',
     author='HIRO TAKAGI',
     author_email='s2222103@stu.musashino-u.ac.jp',
     url='https://github.com/h1l2o/clipboardhist.git',
     packages=find_packages(),
     install_requires=['pyperclip'],
     classifiers=[
```

