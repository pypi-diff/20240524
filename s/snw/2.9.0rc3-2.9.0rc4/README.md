# Comparing `tmp/snw-2.9.0rc3.tar.gz` & `tmp/snw-2.9.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/snw-2.9.0rc3.tar", last modified: Thu Jul 22 10:01:47 2021, max compression
+gzip compressed data, was "dist/snw-2.9.0rc4.tar", last modified: Fri Jul 23 10:40:00 2021, max compression
```

## Comparing `snw-2.9.0rc3.tar` & `snw-2.9.0rc4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-22 10:01:47.000000 snw-2.9.0rc3/
--rw-rw-r--   0 chuan     (1000) chuan     (1000)    10187 2021-07-22 10:00:04.000000 snw-2.9.0rc3/README.md
-drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-22 10:01:47.000000 snw-2.9.0rc3/nmt-wizard/
-drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-22 10:01:47.000000 snw-2.9.0rc3/nmt-wizard/client/
--rw-rw-r--   0 chuan     (1000) chuan     (1000)    30605 2021-07-22 10:00:32.000000 snw-2.9.0rc3/nmt-wizard/client/launcher.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)        0 2021-07-22 10:00:32.000000 snw-2.9.0rc3/nmt-wizard/client/__init__.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)       38 2021-07-22 10:01:47.000000 snw-2.9.0rc3/setup.cfg
--rw-rw-r--   0 chuan     (1000) chuan     (1000)      227 2021-07-22 10:01:47.000000 snw-2.9.0rc3/PKG-INFO
-drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-22 10:01:47.000000 snw-2.9.0rc3/client/
--rwxrwxr-x   0 chuan     (1000) chuan     (1000)     7965 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/snw
-drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-22 10:01:47.000000 snw-2.9.0rc3/client/lib/
--rw-rw-r--   0 chuan     (1000) chuan     (1000)    28559 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/opts.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)     2248 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/credentials.py
-drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-22 10:01:47.000000 snw-2.9.0rc3/client/lib/commands/
--rw-rw-r--   0 chuan     (1000) chuan     (1000)     3836 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/group.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)     2798 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/share.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)     3246 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/tag.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)    26441 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/task.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)     7561 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/user.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)     6071 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/service.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)     2778 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/docker.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)     1500 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/vocab.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)     4187 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/role.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)     4514 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/resource.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)      660 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/permission.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)    22114 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/model.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)        0 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/__init__.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)     3688 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/commands/entity.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)    13664 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/snwtrans.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)        0 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/__init__.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)    22623 2021-07-22 10:00:04.000000 snw-2.9.0rc3/client/lib/utils.py
-drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-22 10:01:47.000000 snw-2.9.0rc3/corpus-acquisition/
-drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-22 10:01:47.000000 snw-2.9.0rc3/corpus-acquisition/pyscripts/
--rw-rw-r--   0 chuan     (1000) chuan     (1000)     3369 2021-07-22 10:00:32.000000 snw-2.9.0rc3/corpus-acquisition/pyscripts/segmenting.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)        0 2021-07-22 10:00:32.000000 snw-2.9.0rc3/corpus-acquisition/pyscripts/__init__.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)     2228 2021-07-22 10:00:32.000000 snw-2.9.0rc3/corpus-acquisition/pyscripts/nameent-divergence-fren.py
--rw-rw-r--   0 chuan     (1000) chuan     (1000)      810 2021-07-22 10:00:32.000000 snw-2.9.0rc3/corpus-acquisition/pyscripts/segmenter.py
-drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-22 10:01:47.000000 snw-2.9.0rc3/snw.egg-info/
--rw-rw-r--   0 chuan     (1000) chuan     (1000)      106 2021-07-22 10:01:47.000000 snw-2.9.0rc3/snw.egg-info/requires.txt
--rw-rw-r--   0 chuan     (1000) chuan     (1000)        1 2021-07-22 10:01:47.000000 snw-2.9.0rc3/snw.egg-info/dependency_links.txt
--rw-rw-r--   0 chuan     (1000) chuan     (1000)      932 2021-07-22 10:01:47.000000 snw-2.9.0rc3/snw.egg-info/SOURCES.txt
--rw-rw-r--   0 chuan     (1000) chuan     (1000)      227 2021-07-22 10:01:47.000000 snw-2.9.0rc3/snw.egg-info/PKG-INFO
--rw-rw-r--   0 chuan     (1000) chuan     (1000)       15 2021-07-22 10:01:47.000000 snw-2.9.0rc3/snw.egg-info/top_level.txt
--rw-rw-r--   0 chuan     (1000) chuan     (1000)      658 2021-07-22 10:01:38.000000 snw-2.9.0rc3/setup.py
+drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-23 10:40:00.000000 snw-2.9.0rc4/
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)    10187 2021-07-23 10:38:03.000000 snw-2.9.0rc4/README.md
+drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-23 10:40:00.000000 snw-2.9.0rc4/nmt-wizard/
+drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-23 10:40:00.000000 snw-2.9.0rc4/nmt-wizard/client/
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)    30605 2021-07-23 10:39:19.000000 snw-2.9.0rc4/nmt-wizard/client/launcher.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)        0 2021-07-23 10:39:19.000000 snw-2.9.0rc4/nmt-wizard/client/__init__.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)       38 2021-07-23 10:40:00.000000 snw-2.9.0rc4/setup.cfg
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)      227 2021-07-23 10:40:00.000000 snw-2.9.0rc4/PKG-INFO
+drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-23 10:40:00.000000 snw-2.9.0rc4/client/
+-rwxrwxr-x   0 chuan     (1000) chuan     (1000)     7965 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/snw
+drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-23 10:40:00.000000 snw-2.9.0rc4/client/lib/
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)    28559 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/opts.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     2248 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/credentials.py
+drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-23 10:40:00.000000 snw-2.9.0rc4/client/lib/commands/
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     3836 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/group.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     2798 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/share.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     3246 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/tag.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)    26441 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/task.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     7561 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/user.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     6071 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/service.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     2778 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/docker.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     1500 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/vocab.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     4187 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/role.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     4514 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/resource.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)      660 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/permission.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)    22114 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/model.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)        0 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/__init__.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     3688 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/commands/entity.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)    13664 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/snwtrans.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)        0 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/__init__.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)    22623 2021-07-23 10:38:03.000000 snw-2.9.0rc4/client/lib/utils.py
+drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-23 10:40:00.000000 snw-2.9.0rc4/corpus-acquisition/
+drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-23 10:40:00.000000 snw-2.9.0rc4/corpus-acquisition/pyscripts/
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     3369 2021-07-23 10:39:19.000000 snw-2.9.0rc4/corpus-acquisition/pyscripts/segmenting.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)        0 2021-07-23 10:39:19.000000 snw-2.9.0rc4/corpus-acquisition/pyscripts/__init__.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     2228 2021-07-23 10:39:19.000000 snw-2.9.0rc4/corpus-acquisition/pyscripts/nameent-divergence-fren.py
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)      810 2021-07-23 10:39:19.000000 snw-2.9.0rc4/corpus-acquisition/pyscripts/segmenter.py
+drwxrwxr-x   0 chuan     (1000) chuan     (1000)        0 2021-07-23 10:40:00.000000 snw-2.9.0rc4/snw.egg-info/
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)      106 2021-07-23 10:40:00.000000 snw-2.9.0rc4/snw.egg-info/requires.txt
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)        1 2021-07-23 10:40:00.000000 snw-2.9.0rc4/snw.egg-info/dependency_links.txt
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)      932 2021-07-23 10:40:00.000000 snw-2.9.0rc4/snw.egg-info/SOURCES.txt
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)      227 2021-07-23 10:40:00.000000 snw-2.9.0rc4/snw.egg-info/PKG-INFO
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)       15 2021-07-23 10:40:00.000000 snw-2.9.0rc4/snw.egg-info/top_level.txt
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)      658 2021-07-23 10:39:49.000000 snw-2.9.0rc4/setup.py
```

### Comparing `snw-2.9.0rc3/README.md` & `snw-2.9.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/nmt-wizard/client/launcher.py` & `snw-2.9.0rc4/nmt-wizard/client/launcher.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/snw` & `snw-2.9.0rc4/client/snw`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/opts.py` & `snw-2.9.0rc4/client/lib/opts.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/credentials.py` & `snw-2.9.0rc4/client/lib/credentials.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/commands/group.py` & `snw-2.9.0rc4/client/lib/commands/group.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/commands/share.py` & `snw-2.9.0rc4/client/lib/commands/share.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/commands/tag.py` & `snw-2.9.0rc4/client/lib/commands/tag.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/commands/task.py` & `snw-2.9.0rc4/client/lib/commands/task.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/commands/user.py` & `snw-2.9.0rc4/client/lib/commands/user.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/commands/service.py` & `snw-2.9.0rc4/client/lib/commands/service.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/commands/docker.py` & `snw-2.9.0rc4/client/lib/commands/docker.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/commands/vocab.py` & `snw-2.9.0rc4/client/lib/commands/vocab.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/commands/role.py` & `snw-2.9.0rc4/client/lib/commands/role.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/commands/resource.py` & `snw-2.9.0rc4/client/lib/commands/resource.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/commands/permission.py` & `snw-2.9.0rc4/client/lib/commands/permission.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/commands/model.py` & `snw-2.9.0rc4/client/lib/commands/model.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/commands/entity.py` & `snw-2.9.0rc4/client/lib/commands/entity.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/snwtrans.py` & `snw-2.9.0rc4/client/lib/snwtrans.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/client/lib/utils.py` & `snw-2.9.0rc4/client/lib/utils.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/corpus-acquisition/pyscripts/segmenting.py` & `snw-2.9.0rc4/corpus-acquisition/pyscripts/segmenting.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/corpus-acquisition/pyscripts/nameent-divergence-fren.py` & `snw-2.9.0rc4/corpus-acquisition/pyscripts/nameent-divergence-fren.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/corpus-acquisition/pyscripts/segmenter.py` & `snw-2.9.0rc4/corpus-acquisition/pyscripts/segmenter.py`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/snw.egg-info/SOURCES.txt` & `snw-2.9.0rc4/snw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snw-2.9.0rc3/setup.py` & `snw-2.9.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='snw',
-    version='2.9.0rc3',
+    version='2.9.0rc4',
     description='snw client tool',
     author='Jean Senellart',
     author_email='jean.senellart@systrangroup.com',
     url='http://www.systransoft.com',
     scripts=['client/snw'],
     package_dir={'client': 'nmt-wizard/client', 'lib': 'client/lib', 'srx': 'corpus-acquisition/pyscripts'},
     packages=['client', 'lib', 'lib.commands', 'srx'],
```

