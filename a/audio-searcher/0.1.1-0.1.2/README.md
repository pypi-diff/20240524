# Comparing `tmp/audio_searcher-0.1.1.tar.gz` & `tmp/audio_searcher-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_searcher-0.1.1.tar", last modified: Thu May 23 06:53:44 2024, max compression
+gzip compressed data, was "audio_searcher-0.1.2.tar", last modified: Fri May 24 08:46:11 2024, max compression
```

## Comparing `audio_searcher-0.1.1.tar` & `audio_searcher-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hamazakikotomi   (501) staff       (20)        0 2024-05-23 06:53:44.127869 audio_searcher-0.1.1/
--rw-r--r--   0 hamazakikotomi   (501) staff       (20)      283 2024-05-23 06:37:01.000000 audio_searcher-0.1.1/LICENSE
--rw-r--r--   0 hamazakikotomi   (501) staff       (20)     1137 2024-05-23 06:53:44.127694 audio_searcher-0.1.1/PKG-INFO
--rw-r--r--   0 hamazakikotomi   (501) staff       (20)      642 2024-05-23 06:46:05.000000 audio_searcher-0.1.1/README.md
-drwxr-xr-x   0 hamazakikotomi   (501) staff       (20)        0 2024-05-23 06:53:44.126183 audio_searcher-0.1.1/audio_searcher/
--rw-r--r--   0 hamazakikotomi   (501) staff       (20)        0 2024-05-23 06:11:02.000000 audio_searcher-0.1.1/audio_searcher/__init__.py
--rw-r--r--   0 hamazakikotomi   (501) staff       (20)     2070 2024-05-23 06:43:02.000000 audio_searcher-0.1.1/audio_searcher/audio_search.py
-drwxr-xr-x   0 hamazakikotomi   (501) staff       (20)        0 2024-05-23 06:53:44.127458 audio_searcher-0.1.1/audio_searcher.egg-info/
--rw-r--r--   0 hamazakikotomi   (501) staff       (20)     1137 2024-05-23 06:53:43.000000 audio_searcher-0.1.1/audio_searcher.egg-info/PKG-INFO
--rw-r--r--   0 hamazakikotomi   (501) staff       (20)      314 2024-05-23 06:53:44.000000 audio_searcher-0.1.1/audio_searcher.egg-info/SOURCES.txt
--rw-r--r--   0 hamazakikotomi   (501) staff       (20)        1 2024-05-23 06:53:43.000000 audio_searcher-0.1.1/audio_searcher.egg-info/dependency_links.txt
--rw-r--r--   0 hamazakikotomi   (501) staff       (20)       70 2024-05-23 06:53:43.000000 audio_searcher-0.1.1/audio_searcher.egg-info/entry_points.txt
--rw-r--r--   0 hamazakikotomi   (501) staff       (20)       24 2024-05-23 06:53:43.000000 audio_searcher-0.1.1/audio_searcher.egg-info/requires.txt
--rw-r--r--   0 hamazakikotomi   (501) staff       (20)       15 2024-05-23 06:53:44.000000 audio_searcher-0.1.1/audio_searcher.egg-info/top_level.txt
--rw-r--r--   0 hamazakikotomi   (501) staff       (20)       38 2024-05-23 06:53:44.127930 audio_searcher-0.1.1/setup.cfg
--rw-r--r--   0 hamazakikotomi   (501) staff       (20)      835 2024-05-23 06:53:35.000000 audio_searcher-0.1.1/setup.py
+drwxr-xr-x   0 hamazakikotomi   (501) staff       (20)        0 2024-05-24 08:46:11.998259 audio_searcher-0.1.2/
+-rw-r--r--   0 hamazakikotomi   (501) staff       (20)      283 2024-05-23 06:37:01.000000 audio_searcher-0.1.2/LICENSE
+-rw-r--r--   0 hamazakikotomi   (501) staff       (20)     1919 2024-05-24 08:46:11.998084 audio_searcher-0.1.2/PKG-INFO
+-rw-r--r--   0 hamazakikotomi   (501) staff       (20)     1424 2024-05-24 08:41:31.000000 audio_searcher-0.1.2/README.md
+drwxr-xr-x   0 hamazakikotomi   (501) staff       (20)        0 2024-05-24 08:46:11.996508 audio_searcher-0.1.2/audio_searcher/
+-rw-r--r--   0 hamazakikotomi   (501) staff       (20)        0 2024-05-23 06:11:02.000000 audio_searcher-0.1.2/audio_searcher/__init__.py
+-rw-r--r--   0 hamazakikotomi   (501) staff       (20)     2070 2024-05-23 06:43:02.000000 audio_searcher-0.1.2/audio_searcher/audio_search.py
+drwxr-xr-x   0 hamazakikotomi   (501) staff       (20)        0 2024-05-24 08:46:11.997841 audio_searcher-0.1.2/audio_searcher.egg-info/
+-rw-r--r--   0 hamazakikotomi   (501) staff       (20)     1919 2024-05-24 08:46:11.000000 audio_searcher-0.1.2/audio_searcher.egg-info/PKG-INFO
+-rw-r--r--   0 hamazakikotomi   (501) staff       (20)      314 2024-05-24 08:46:11.000000 audio_searcher-0.1.2/audio_searcher.egg-info/SOURCES.txt
+-rw-r--r--   0 hamazakikotomi   (501) staff       (20)        1 2024-05-24 08:46:11.000000 audio_searcher-0.1.2/audio_searcher.egg-info/dependency_links.txt
+-rw-r--r--   0 hamazakikotomi   (501) staff       (20)       70 2024-05-24 08:46:11.000000 audio_searcher-0.1.2/audio_searcher.egg-info/entry_points.txt
+-rw-r--r--   0 hamazakikotomi   (501) staff       (20)       24 2024-05-24 08:46:11.000000 audio_searcher-0.1.2/audio_searcher.egg-info/requires.txt
+-rw-r--r--   0 hamazakikotomi   (501) staff       (20)       15 2024-05-24 08:46:11.000000 audio_searcher-0.1.2/audio_searcher.egg-info/top_level.txt
+-rw-r--r--   0 hamazakikotomi   (501) staff       (20)       38 2024-05-24 08:46:11.998323 audio_searcher-0.1.2/setup.cfg
+-rw-r--r--   0 hamazakikotomi   (501) staff       (20)      835 2024-05-24 08:41:52.000000 audio_searcher-0.1.2/setup.py
```

### Comparing `audio_searcher-0.1.1/audio_searcher/audio_search.py` & `audio_searcher-0.1.2/audio_searcher/audio_search.py`

 * *Files identical despite different names*

### Comparing `audio_searcher-0.1.1/setup.py` & `audio_searcher-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='audio_searcher',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'SpeechRecognition',
         'pydub'
     ],
     entry_points={
         'console_scripts': [
```

