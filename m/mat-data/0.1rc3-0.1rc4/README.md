# Comparing `tmp/mat_data-0.1rc3.tar.gz` & `tmp/mat_data-0.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat_data-0.1rc3.tar", last modified: Wed May 22 19:27:31 2024, max compression
+gzip compressed data, was "mat_data-0.1rc4.tar", last modified: Fri May 24 17:52:46 2024, max compression
```

## Comparing `mat_data-0.1rc3.tar` & `mat_data-0.1rc4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-22 19:27:31.594889 mat_data-0.1rc3/
--rw-r--r--   0 tarlisportela   (501) staff       (20)       86 2024-05-18 00:08:05.000000 mat_data-0.1rc3/CHANGELOG.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2023-12-15 20:34:29.000000 mat_data-0.1rc3/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat_data-0.1rc3/MANIFEST.in
--rwx------   0 tarlisportela   (501) staff       (20)   164966 2024-05-21 20:11:32.000000 mat_data-0.1rc3/MAT-data-Tutorial.ipynb
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5628 2024-05-22 19:27:31.594682 mat_data-0.1rc3/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3302 2024-05-17 23:01:51.000000 mat_data-0.1rc3/README.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)      717 2023-12-16 03:29:23.000000 mat_data-0.1rc3/Steps to Build.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-22 19:27:31.540345 mat_data-0.1rc3/docs/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      638 2024-05-17 20:33:21.000000 mat_data-0.1rc3/docs/Makefile
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-22 19:27:31.536779 mat_data-0.1rc3/docs/build/
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-22 19:27:31.548377 mat_data-0.1rc3/docs/build/doctrees/
--rw-r--r--   0 tarlisportela   (501) staff       (20)   136470 2024-05-22 02:44:40.000000 mat_data-0.1rc3/docs/build/doctrees/converter.doctree
--rw-r--r--   0 tarlisportela   (501) staff       (20)    93301 2024-05-22 02:44:40.000000 mat_data-0.1rc3/docs/build/doctrees/dataset.doctree
--rw-r--r--   0 tarlisportela   (501) staff       (20)  1472114 2024-05-22 02:44:40.000000 mat_data-0.1rc3/docs/build/doctrees/environment.pickle
--rw-r--r--   0 tarlisportela   (501) staff       (20)    69348 2024-05-22 02:44:40.000000 mat_data-0.1rc3/docs/build/doctrees/generator.doctree
--rw-r--r--   0 tarlisportela   (501) staff       (20)   959687 2024-05-20 20:33:48.000000 mat_data-0.1rc3/docs/build/doctrees/index.doctree
--rw-r--r--   0 tarlisportela   (501) staff       (20)   173971 2024-05-22 02:44:40.000000 mat_data-0.1rc3/docs/build/doctrees/preprocess.doctree
--rw-r--r--   0 tarlisportela   (501) staff       (20)      804 2024-05-17 20:33:21.000000 mat_data-0.1rc3/docs/make.bat
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-22 19:27:31.550133 mat_data-0.1rc3/docs/source/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1262 2024-05-22 02:52:46.000000 mat_data-0.1rc3/docs/source/conf.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)       66 2024-05-17 21:13:53.000000 mat_data-0.1rc3/docs/source/converter.rst
--rw-r--r--   0 tarlisportela   (501) staff       (20)       60 2024-05-17 21:13:51.000000 mat_data-0.1rc3/docs/source/dataset.rst
--rw-r--r--   0 tarlisportela   (501) staff       (20)       66 2024-05-17 21:29:32.000000 mat_data-0.1rc3/docs/source/generator.rst
--rw-r--r--   0 tarlisportela   (501) staff       (20)      623 2024-05-17 22:49:52.000000 mat_data-0.1rc3/docs/source/index.rst
--rw-r--r--   0 tarlisportela   (501) staff       (20)       77 2024-05-17 21:29:23.000000 mat_data-0.1rc3/docs/source/preprocess.rst
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-22 19:27:31.593951 mat_data-0.1rc3/mat_data.egg-info/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5628 2024-05-22 19:27:31.000000 mat_data-0.1rc3/mat_data.egg-info/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1166 2024-05-22 19:27:31.000000 mat_data-0.1rc3/mat_data.egg-info/SOURCES.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-05-22 19:27:31.000000 mat_data-0.1rc3/mat_data.egg-info/dependency_links.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)      175 2024-05-22 19:27:31.000000 mat_data-0.1rc3/mat_data.egg-info/requires.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        8 2024-05-22 19:27:31.000000 mat_data-0.1rc3/mat_data.egg-info/top_level.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-22 19:27:31.552256 mat_data-0.1rc3/matdata/
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2023-12-15 20:34:29.000000 mat_data-0.1rc3/matdata/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3302 2024-05-17 23:01:51.000000 mat_data-0.1rc3/matdata/README.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)      770 2024-05-17 21:07:30.000000 mat_data-0.1rc3/matdata/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-22 19:27:31.537135 mat_data-0.1rc3/matdata/assets/
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-22 19:27:31.586861 mat_data-0.1rc3/matdata/assets/sample/
--rw-rw-r--   0 tarlisportela   (501) staff       (20)  7716732 2021-02-10 16:01:46.000000 mat_data-0.1rc3/matdata/assets/sample/Foursquare_Sample.csv
--rw-r--r--   0 tarlisportela   (501) staff       (20)  1775017 2024-05-17 19:06:55.000000 mat_data-0.1rc3/matdata/assets/sample/data.parquet
--rw-r--r--   0 tarlisportela   (501) staff       (20)  7619562 2024-05-17 19:06:54.000000 mat_data-0.1rc3/matdata/assets/sample/joined.csv
--rw-r--r--   0 tarlisportela   (501) staff       (20)  2283111 2024-05-17 19:06:46.000000 mat_data-0.1rc3/matdata/assets/sample/test.csv
--rw-r--r--   0 tarlisportela   (501) staff       (20)   494642 2024-05-17 19:06:46.000000 mat_data-0.1rc3/matdata/assets/sample/test.parquet
--rw-r--r--   0 tarlisportela   (501) staff       (20)  5336514 2024-05-17 19:06:45.000000 mat_data-0.1rc3/matdata/assets/sample/train.csv
--rw-r--r--   0 tarlisportela   (501) staff       (20)  1075420 2024-05-17 19:06:46.000000 mat_data-0.1rc3/matdata/assets/sample/train.parquet
--rw-r--r--   0 tarlisportela   (501) staff       (20)    24732 2024-05-22 19:25:13.000000 mat_data-0.1rc3/matdata/converter.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    20722 2024-05-22 19:26:47.000000 mat_data-0.1rc3/matdata/dataset.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    26560 2024-05-17 22:09:55.000000 mat_data-0.1rc3/matdata/generator.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-22 19:27:31.591786 mat_data-0.1rc3/matdata/inc/
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_data-0.1rc3/matdata/inc/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    54373 2024-05-17 21:34:31.000000 mat_data-0.1rc3/matdata/inc/ts_io.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    47145 2024-05-22 19:21:08.000000 mat_data-0.1rc3/matdata/preprocess.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-22 19:27:31.592106 mat_data-0.1rc3/matdata/util/
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_data-0.1rc3/matdata/util/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1384 2024-05-17 21:33:27.000000 mat_data-0.1rc3/matdata/util/movelets.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2192 2024-05-22 02:16:48.000000 mat_data-0.1rc3/pyproject.toml
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-22 19:27:31.593000 mat_data-0.1rc3/scripts/
--rwx------   0 tarlisportela   (501) staff       (20)     3986 2024-05-20 22:17:59.000000 mat_data-0.1rc3/scripts/MAT-GetData.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-05-22 19:27:31.594956 mat_data-0.1rc3/setup.cfg
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2092 2024-05-20 12:38:21.000000 mat_data-0.1rc3/setup.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:52:46.834464 mat_data-0.1rc4/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       86 2024-05-18 00:08:05.000000 mat_data-0.1rc4/CHANGELOG.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2023-12-15 20:34:29.000000 mat_data-0.1rc4/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat_data-0.1rc4/MANIFEST.in
+-rwx------   0 tarlisportela   (501) staff       (20)   164966 2024-05-21 20:11:32.000000 mat_data-0.1rc4/MAT-data-Tutorial.ipynb
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5628 2024-05-24 17:52:46.834208 mat_data-0.1rc4/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3302 2024-05-17 23:01:51.000000 mat_data-0.1rc4/README.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      717 2023-12-16 03:29:23.000000 mat_data-0.1rc4/Steps to Build.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:52:46.775744 mat_data-0.1rc4/docs/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      638 2024-05-17 20:33:21.000000 mat_data-0.1rc4/docs/Makefile
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:52:46.771993 mat_data-0.1rc4/docs/build/
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:52:46.783852 mat_data-0.1rc4/docs/build/doctrees/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   136470 2024-05-22 02:44:40.000000 mat_data-0.1rc4/docs/build/doctrees/converter.doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    93301 2024-05-22 02:44:40.000000 mat_data-0.1rc4/docs/build/doctrees/dataset.doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  1472114 2024-05-22 02:44:40.000000 mat_data-0.1rc4/docs/build/doctrees/environment.pickle
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    69348 2024-05-22 02:44:40.000000 mat_data-0.1rc4/docs/build/doctrees/generator.doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   959687 2024-05-20 20:33:48.000000 mat_data-0.1rc4/docs/build/doctrees/index.doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   173971 2024-05-22 02:44:40.000000 mat_data-0.1rc4/docs/build/doctrees/preprocess.doctree
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      804 2024-05-17 20:33:21.000000 mat_data-0.1rc4/docs/make.bat
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:52:46.785709 mat_data-0.1rc4/docs/source/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1262 2024-05-22 02:52:46.000000 mat_data-0.1rc4/docs/source/conf.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       66 2024-05-17 21:13:53.000000 mat_data-0.1rc4/docs/source/converter.rst
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       60 2024-05-17 21:13:51.000000 mat_data-0.1rc4/docs/source/dataset.rst
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       66 2024-05-17 21:29:32.000000 mat_data-0.1rc4/docs/source/generator.rst
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      623 2024-05-17 22:49:52.000000 mat_data-0.1rc4/docs/source/index.rst
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       77 2024-05-17 21:29:23.000000 mat_data-0.1rc4/docs/source/preprocess.rst
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:52:46.833443 mat_data-0.1rc4/mat_data.egg-info/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5628 2024-05-24 17:52:46.000000 mat_data-0.1rc4/mat_data.egg-info/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1166 2024-05-24 17:52:46.000000 mat_data-0.1rc4/mat_data.egg-info/SOURCES.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-05-24 17:52:46.000000 mat_data-0.1rc4/mat_data.egg-info/dependency_links.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      175 2024-05-24 17:52:46.000000 mat_data-0.1rc4/mat_data.egg-info/requires.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        8 2024-05-24 17:52:46.000000 mat_data-0.1rc4/mat_data.egg-info/top_level.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:52:46.789140 mat_data-0.1rc4/matdata/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2023-12-15 20:34:29.000000 mat_data-0.1rc4/matdata/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3302 2024-05-17 23:01:51.000000 mat_data-0.1rc4/matdata/README.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      770 2024-05-17 21:07:30.000000 mat_data-0.1rc4/matdata/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:52:46.772371 mat_data-0.1rc4/matdata/assets/
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:52:46.826128 mat_data-0.1rc4/matdata/assets/sample/
+-rw-rw-r--   0 tarlisportela   (501) staff       (20)  7716732 2021-02-10 16:01:46.000000 mat_data-0.1rc4/matdata/assets/sample/Foursquare_Sample.csv
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  1775017 2024-05-17 19:06:55.000000 mat_data-0.1rc4/matdata/assets/sample/data.parquet
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  7619562 2024-05-17 19:06:54.000000 mat_data-0.1rc4/matdata/assets/sample/joined.csv
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  2283111 2024-05-17 19:06:46.000000 mat_data-0.1rc4/matdata/assets/sample/test.csv
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   494642 2024-05-17 19:06:46.000000 mat_data-0.1rc4/matdata/assets/sample/test.parquet
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  5336514 2024-05-17 19:06:45.000000 mat_data-0.1rc4/matdata/assets/sample/train.csv
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  1075420 2024-05-17 19:06:46.000000 mat_data-0.1rc4/matdata/assets/sample/train.parquet
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    24732 2024-05-22 19:25:13.000000 mat_data-0.1rc4/matdata/converter.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    20722 2024-05-22 19:26:47.000000 mat_data-0.1rc4/matdata/dataset.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    26560 2024-05-17 22:09:55.000000 mat_data-0.1rc4/matdata/generator.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:52:46.830784 mat_data-0.1rc4/matdata/inc/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_data-0.1rc4/matdata/inc/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    54373 2024-05-17 21:34:31.000000 mat_data-0.1rc4/matdata/inc/ts_io.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    47145 2024-05-22 19:21:08.000000 mat_data-0.1rc4/matdata/preprocess.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:52:46.832877 mat_data-0.1rc4/matdata/util/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_data-0.1rc4/matdata/util/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1384 2024-05-17 21:33:27.000000 mat_data-0.1rc4/matdata/util/movelets.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2192 2024-05-24 17:51:26.000000 mat_data-0.1rc4/pyproject.toml
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:52:46.833134 mat_data-0.1rc4/scripts/
+-rwx------   0 tarlisportela   (501) staff       (20)     3986 2024-05-20 22:17:59.000000 mat_data-0.1rc4/scripts/MAT-GetData.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-05-24 17:52:46.834538 mat_data-0.1rc4/setup.cfg
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2092 2024-05-20 12:38:21.000000 mat_data-0.1rc4/setup.py
```

### Comparing `mat_data-0.1rc3/LICENSE` & `mat_data-0.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/MAT-data-Tutorial.ipynb` & `mat_data-0.1rc4/MAT-data-Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/PKG-INFO` & `mat_data-0.1rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat-data
-Version: 0.1rc3
+Version: 0.1rc4
 Summary: MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining
 Home-page: https://github.com/mat-analysis/mat-data
 Author: Tarlis Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/mat-analysis/mat-data
```

### Comparing `mat_data-0.1rc3/README.md` & `mat_data-0.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/Steps to Build.txt` & `mat_data-0.1rc4/Steps to Build.txt`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/docs/Makefile` & `mat_data-0.1rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/docs/build/doctrees/converter.doctree` & `mat_data-0.1rc4/docs/build/doctrees/converter.doctree`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/docs/build/doctrees/dataset.doctree` & `mat_data-0.1rc4/docs/build/doctrees/dataset.doctree`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/docs/build/doctrees/environment.pickle` & `mat_data-0.1rc4/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/docs/build/doctrees/generator.doctree` & `mat_data-0.1rc4/docs/build/doctrees/generator.doctree`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/docs/build/doctrees/index.doctree` & `mat_data-0.1rc4/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/docs/build/doctrees/preprocess.doctree` & `mat_data-0.1rc4/docs/build/doctrees/preprocess.doctree`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/docs/make.bat` & `mat_data-0.1rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/docs/source/conf.py` & `mat_data-0.1rc4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/docs/source/index.rst` & `mat_data-0.1rc4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/mat_data.egg-info/PKG-INFO` & `mat_data-0.1rc4/mat_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat-data
-Version: 0.1rc3
+Version: 0.1rc4
 Summary: MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining
 Home-page: https://github.com/mat-analysis/mat-data
 Author: Tarlis Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/mat-analysis/mat-data
```

### Comparing `mat_data-0.1rc3/mat_data.egg-info/SOURCES.txt` & `mat_data-0.1rc4/mat_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/LICENSE` & `mat_data-0.1rc4/matdata/LICENSE`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/README.md` & `mat_data-0.1rc4/matdata/README.md`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/__init__.py` & `mat_data-0.1rc4/matdata/__init__.py`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/assets/sample/Foursquare_Sample.csv` & `mat_data-0.1rc4/matdata/assets/sample/Foursquare_Sample.csv`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/assets/sample/data.parquet` & `mat_data-0.1rc4/matdata/assets/sample/data.parquet`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/assets/sample/joined.csv` & `mat_data-0.1rc4/matdata/assets/sample/joined.csv`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/assets/sample/test.csv` & `mat_data-0.1rc4/matdata/assets/sample/test.csv`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/assets/sample/test.parquet` & `mat_data-0.1rc4/matdata/assets/sample/test.parquet`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/assets/sample/train.csv` & `mat_data-0.1rc4/matdata/assets/sample/train.csv`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/assets/sample/train.parquet` & `mat_data-0.1rc4/matdata/assets/sample/train.parquet`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/converter.py` & `mat_data-0.1rc4/matdata/converter.py`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/dataset.py` & `mat_data-0.1rc4/matdata/dataset.py`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/generator.py` & `mat_data-0.1rc4/matdata/generator.py`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/inc/ts_io.py` & `mat_data-0.1rc4/matdata/inc/ts_io.py`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/preprocess.py` & `mat_data-0.1rc4/matdata/preprocess.py`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/matdata/util/movelets.py` & `mat_data-0.1rc4/matdata/util/movelets.py`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/pyproject.toml` & `mat_data-0.1rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 [project]
 name = "mat-data"
-version = "0.1rc3"
+version = "0.1rc4"
 description = "MAT-data: Data Preprocessing for Multiple Aspect Trajectory Data Mining"
 authors = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
 maintainers = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
```

### Comparing `mat_data-0.1rc3/scripts/MAT-GetData.py` & `mat_data-0.1rc4/scripts/MAT-GetData.py`

 * *Files identical despite different names*

### Comparing `mat_data-0.1rc3/setup.py` & `mat_data-0.1rc4/setup.py`

 * *Files identical despite different names*

