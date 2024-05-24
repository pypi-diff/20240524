# Comparing `tmp/yapecs-0.0.7.tar.gz` & `tmp/yapecs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yapecs-0.0.7.tar", last modified: Wed Jun 28 18:51:37 2023, max compression
+gzip compressed data, was "yapecs-0.0.8.tar", last modified: Fri May 24 21:01:14 2024, max compression
```

## Comparing `yapecs-0.0.7.tar` & `yapecs-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-06-28 18:51:37.500568 yapecs-0.0.7/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1069 2023-06-28 18:51:10.000000 yapecs-0.0.7/LICENSE
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      757 2023-06-28 18:51:37.496568 yapecs-0.0.7/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      417 2023-06-28 18:51:10.000000 yapecs-0.0.7/README.md
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       38 2023-06-28 18:51:37.500568 yapecs-0.0.7/setup.cfg
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      565 2023-06-28 18:51:10.000000 yapecs-0.0.7/setup.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-06-28 18:51:37.496568 yapecs-0.0.7/test/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      874 2023-06-28 18:51:10.000000 yapecs-0.0.7/test/test_core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-06-28 18:51:37.496568 yapecs-0.0.7/yapecs/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3944 2023-06-28 18:51:10.000000 yapecs-0.0.7/yapecs/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2561 2023-06-28 18:51:10.000000 yapecs-0.0.7/yapecs/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-06-28 18:51:37.496568 yapecs-0.0.7/yapecs.egg-info/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      757 2023-06-28 18:51:37.000000 yapecs-0.0.7/yapecs.egg-info/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      198 2023-06-28 18:51:37.000000 yapecs-0.0.7/yapecs.egg-info/SOURCES.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        1 2023-06-28 18:51:37.000000 yapecs-0.0.7/yapecs.egg-info/dependency_links.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        7 2023-06-28 18:51:37.000000 yapecs-0.0.7/yapecs.egg-info/top_level.txt
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-24 21:01:14.057545 yapecs-0.0.8/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1069 2024-05-17 15:05:52.000000 yapecs-0.0.8/LICENSE
+-rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)    10199 2024-05-24 21:01:14.057545 yapecs-0.0.8/PKG-INFO
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     9835 2024-05-24 21:00:41.000000 yapecs-0.0.8/README.md
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       38 2024-05-24 21:01:14.057545 yapecs-0.0.8/setup.cfg
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      600 2024-05-24 21:00:41.000000 yapecs-0.0.8/setup.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-24 21:01:14.057545 yapecs-0.0.8/test/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2317 2024-05-24 21:00:41.000000 yapecs-0.0.8/test/test_core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-24 21:01:14.057545 yapecs-0.0.8/yapecs/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2024-05-24 21:00:41.000000 yapecs-0.0.8/yapecs/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10116 2024-05-24 21:00:41.000000 yapecs-0.0.8/yapecs/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2024-05-24 21:01:14.057545 yapecs-0.0.8/yapecs.egg-info/
+-rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)    10199 2024-05-24 21:01:14.000000 yapecs-0.0.8/yapecs.egg-info/PKG-INFO
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      227 2024-05-24 21:01:14.000000 yapecs-0.0.8/yapecs.egg-info/SOURCES.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        1 2024-05-24 21:01:14.000000 yapecs-0.0.8/yapecs.egg-info/dependency_links.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        9 2024-05-24 21:01:14.000000 yapecs-0.0.8/yapecs.egg-info/requires.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        7 2024-05-24 21:01:14.000000 yapecs-0.0.8/yapecs.egg-info/top_level.txt
```

### Comparing `yapecs-0.0.7/LICENSE` & `yapecs-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yapecs-0.0.7/setup.py` & `yapecs-0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 with open('README.md', encoding='utf8') as file:
     long_description = file.read()
 
 
 setup(
     name='yapecs',
     description='Yet Another Python Experiment Configuration System (YAPECS)',
-    version='0.0.7',
+    version='0.0.8',
     author='Max Morrison',
     author_email='maxrmorrison@gmail.com',
     url='https://github.com/maxrmorrison/yapecs',
+    install_requires=['filelock'],
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['configuration', 'config', 'experiment', 'manager'])
```

