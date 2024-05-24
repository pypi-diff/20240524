# Comparing `tmp/torchcat-0.0.3.tar.gz` & `tmp/torchcat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchcat-0.0.3.tar", last modified: Fri May 24 02:52:32 2024, max compression
+gzip compressed data, was "torchcat-0.0.4.tar", last modified: Fri May 24 03:13:38 2024, max compression
```

## Comparing `torchcat-0.0.3.tar` & `torchcat-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 02:52:32.213183 torchcat-0.0.3/
--rw-rw-rw-   0        0        0    17765 2024-05-21 13:29:45.000000 torchcat-0.0.3/License
--rw-rw-rw-   0        0        0      285 2024-05-24 02:52:32.213183 torchcat-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        6 2024-05-21 13:35:58.000000 torchcat-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 02:52:32.213183 torchcat-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      528 2024-05-24 02:51:40.000000 torchcat-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 02:52:32.206206 torchcat-0.0.3/torchcat/
--rw-rw-rw-   0        0        0     2242 2024-05-23 10:04:24.000000 torchcat-0.0.3/torchcat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 02:52:32.212186 torchcat-0.0.3/torchcat.egg-info/
--rw-rw-rw-   0        0        0      285 2024-05-24 02:52:32.000000 torchcat-0.0.3/torchcat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2024-05-24 02:52:32.000000 torchcat-0.0.3/torchcat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 02:52:32.000000 torchcat-0.0.3/torchcat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-24 02:52:32.000000 torchcat-0.0.3/torchcat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-24 02:52:32.000000 torchcat-0.0.3/torchcat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 03:13:38.824401 torchcat-0.0.4/
+-rw-rw-rw-   0        0        0    17765 2024-05-21 13:29:45.000000 torchcat-0.0.4/License
+-rw-rw-rw-   0        0        0     1766 2024-05-24 03:13:38.822992 torchcat-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1336 2024-05-24 03:08:16.000000 torchcat-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1404 2024-05-24 03:13:04.000000 torchcat-0.0.4/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-24 03:13:38.824401 torchcat-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      561 2024-05-24 03:13:33.000000 torchcat-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 03:13:38.814952 torchcat-0.0.4/torchcat/
+-rw-rw-rw-   0        0        0     2242 2024-05-23 10:04:24.000000 torchcat-0.0.4/torchcat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 03:13:38.822992 torchcat-0.0.4/torchcat.egg-info/
+-rw-rw-rw-   0        0        0     1766 2024-05-24 03:13:38.000000 torchcat-0.0.4/torchcat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-24 03:13:38.000000 torchcat-0.0.4/torchcat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 03:13:38.000000 torchcat-0.0.4/torchcat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-24 03:13:38.000000 torchcat-0.0.4/torchcat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-24 03:13:38.000000 torchcat-0.0.4/torchcat.egg-info/top_level.txt
```

### Comparing `torchcat-0.0.3/License` & `torchcat-0.0.4/License`

 * *Files identical despite different names*

### Comparing `torchcat-0.0.3/setup.py` & `torchcat-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
-with open("README.md", "r") as f:
-  long_description = f.read()
+with open('README.rst', 'r', encoding='utf-8') as f:
+    long_description = f.read()
 
 setup(
     name='torchcat',
-    version='0.0.3',
+    version='0.0.4',
     author='kaiyu',
     author_email='2971934557@qq.com',
     license='GPL',
-    url='https://www.baidu.com/',
+    url='https://pypi.org/project/torchcat/',
     description='用于简化 torch 模型训练的工具',
     long_description=long_description,
     packages=['torchcat'],
     install_requires=['numpy', 'torchsummary'],
 )
 
 '''
```

### Comparing `torchcat-0.0.3/torchcat/__init__.py` & `torchcat-0.0.4/torchcat/__init__.py`

 * *Files identical despite different names*

