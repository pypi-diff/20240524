# Comparing `tmp/faostat-1.0.2.tar.gz` & `tmp/faostat-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faostat-1.0.2.tar", last modified: Tue Oct 10 07:20:29 2023, max compression
+gzip compressed data, was "faostat-1.1.1.tar", last modified: Fri May 24 15:24:56 2024, max compression
```

## Comparing `faostat-1.0.2.tar` & `faostat-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-10-10 07:20:29.345200 faostat-1.0.2/
--rw-rw-rw-   0        0        0     1102 2023-10-10 07:17:55.000000 faostat-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       85 2023-10-10 07:17:55.000000 faostat-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     9561 2023-10-10 07:20:29.345200 faostat-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8505 2023-10-10 07:17:55.000000 faostat-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-10-10 07:20:29.329561 faostat-1.0.2/faostat/
--rw-rw-rw-   0        0        0      551 2023-10-10 07:17:56.000000 faostat-1.0.2/faostat/__init__.py
--rw-rw-rw-   0        0        0    10902 2023-10-10 07:17:56.000000 faostat-1.0.2/faostat/faostat.py
-drwxrwxrwx   0        0        0        0 2023-10-10 07:20:29.329561 faostat-1.0.2/faostat.egg-info/
--rw-rw-rw-   0        0        0     9561 2023-10-10 07:20:29.000000 faostat-1.0.2/faostat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-10-10 07:20:29.000000 faostat-1.0.2/faostat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-10 07:20:29.000000 faostat-1.0.2/faostat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-10-10 07:20:29.000000 faostat-1.0.2/faostat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-10-10 07:20:29.000000 faostat-1.0.2/faostat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-10 07:20:29.345200 faostat-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1615 2023-10-10 07:17:55.000000 faostat-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:24:56.050810 faostat-1.1.1/
+-rw-rw-rw-   0        0        0     1102 2024-05-24 13:20:54.000000 faostat-1.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       85 2024-03-05 16:39:44.000000 faostat-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    15852 2024-05-24 15:24:56.050810 faostat-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14796 2024-05-24 09:38:47.000000 faostat-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 15:24:55.997435 faostat-1.1.1/faostat/
+-rw-rw-rw-   0        0        0      796 2024-04-22 13:43:37.000000 faostat-1.1.1/faostat/__init__.py
+-rw-rw-rw-   0        0        0    14640 2024-05-24 09:07:53.000000 faostat-1.1.1/faostat/faostat.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:24:56.035184 faostat-1.1.1/faostat.egg-info/
+-rw-rw-rw-   0        0        0    15852 2024-05-24 15:24:55.000000 faostat-1.1.1/faostat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-24 15:24:55.000000 faostat-1.1.1/faostat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 15:24:55.000000 faostat-1.1.1/faostat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-24 15:24:55.000000 faostat-1.1.1/faostat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-24 15:24:55.000000 faostat-1.1.1/faostat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 15:24:56.050810 faostat-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2024-05-24 13:20:25.000000 faostat-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:24:56.035184 faostat-1.1.1/test/
+-rw-rw-rw-   0        0        0     1056 2024-03-19 15:44:24.000000 faostat-1.1.1/test/test.py
```

### Comparing `faostat-1.0.2/LICENSE.txt` & `faostat-1.1.1/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Noemi Emanuela Cazzaniga
+Copyright (c) 2024 Noemi Emanuela Cazzaniga
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `faostat-1.0.2/setup.py` & `faostat-1.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 """
-@author: Noemi E. Cazzaniga - 2023
+@author: Noemi E. Cazzaniga - 2024
 @email: noemi.cazzaniga@polimi.it
 """
 
 
 from setuptools import setup, find_packages
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_descr = f.read()
 
 setup(name='faostat',
-      version='1.0.2',
+      version='1.1.1',
       license='MIT',
-      date='2023',
+      date='2024',
       description="Faostat Python Package",
       long_description=long_descr,
       long_description_content_type='text/markdown',
       author='Noemi Emanuela Cazzaniga',
       author_email='noemi.cazzaniga@polimi.it',
       keywords='faostat statistics data economics science',
       classifiers=[
```

