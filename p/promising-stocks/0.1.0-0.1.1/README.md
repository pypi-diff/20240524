# Comparing `tmp/promising_stocks-0.1.0.tar.gz` & `tmp/promising_stocks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promising_stocks-0.1.0.tar", last modified: Fri May 24 09:39:56 2024, max compression
+gzip compressed data, was "promising_stocks-0.1.1.tar", last modified: Fri May 24 10:12:26 2024, max compression
```

## Comparing `promising_stocks-0.1.0.tar` & `promising_stocks-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-24 09:39:56.944418 promising_stocks-0.1.0/
--rw-r--r--   0 ryota      (501) staff       (20)       11 2024-05-24 09:15:33.000000 promising_stocks-0.1.0/LICENSE
--rw-r--r--   0 ryota      (501) staff       (20)      506 2024-05-24 09:39:56.944310 promising_stocks-0.1.0/PKG-INFO
--rw-r--r--   0 ryota      (501) staff       (20)       41 2024-05-24 09:14:55.000000 promising_stocks-0.1.0/README.md
-drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-24 09:39:56.943599 promising_stocks-0.1.0/promising_stocks/
--rw-r--r--   0 ryota      (501) staff       (20)      151 2024-05-24 09:12:18.000000 promising_stocks-0.1.0/promising_stocks/__init__.py
--rw-r--r--   0 ryota      (501) staff       (20)      302 2024-05-24 09:32:31.000000 promising_stocks-0.1.0/promising_stocks/main.py
-drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-24 09:39:56.944147 promising_stocks-0.1.0/promising_stocks.egg-info/
--rw-r--r--   0 ryota      (501) staff       (20)      506 2024-05-24 09:39:56.000000 promising_stocks-0.1.0/promising_stocks.egg-info/PKG-INFO
--rw-r--r--   0 ryota      (501) staff       (20)      240 2024-05-24 09:39:56.000000 promising_stocks-0.1.0/promising_stocks.egg-info/SOURCES.txt
--rw-r--r--   0 ryota      (501) staff       (20)        1 2024-05-24 09:39:56.000000 promising_stocks-0.1.0/promising_stocks.egg-info/dependency_links.txt
--rw-r--r--   0 ryota      (501) staff       (20)       17 2024-05-24 09:39:56.000000 promising_stocks-0.1.0/promising_stocks.egg-info/top_level.txt
--rw-r--r--   0 ryota      (501) staff       (20)       38 2024-05-24 09:39:56.944459 promising_stocks-0.1.0/setup.cfg
--rw-r--r--   0 ryota      (501) staff       (20)      623 2024-05-24 09:39:53.000000 promising_stocks-0.1.0/setup.py
+drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-24 10:12:26.524151 promising_stocks-0.1.1/
+-rw-r--r--   0 ryota      (501) staff       (20)       11 2024-05-24 09:15:33.000000 promising_stocks-0.1.1/LICENSE
+-rw-r--r--   0 ryota      (501) staff       (20)      506 2024-05-24 10:12:26.524039 promising_stocks-0.1.1/PKG-INFO
+-rw-r--r--   0 ryota      (501) staff       (20)       41 2024-05-24 09:14:55.000000 promising_stocks-0.1.1/README.md
+drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-24 10:12:26.523313 promising_stocks-0.1.1/promising_stocks/
+-rw-r--r--   0 ryota      (501) staff       (20)       88 2024-05-24 10:12:13.000000 promising_stocks-0.1.1/promising_stocks/__init__.py
+-rw-r--r--   0 ryota      (501) staff       (20)      302 2024-05-24 09:32:31.000000 promising_stocks-0.1.1/promising_stocks/main.py
+drwxr-xr-x   0 ryota      (501) staff       (20)        0 2024-05-24 10:12:26.523875 promising_stocks-0.1.1/promising_stocks.egg-info/
+-rw-r--r--   0 ryota      (501) staff       (20)      506 2024-05-24 10:12:26.000000 promising_stocks-0.1.1/promising_stocks.egg-info/PKG-INFO
+-rw-r--r--   0 ryota      (501) staff       (20)      240 2024-05-24 10:12:26.000000 promising_stocks-0.1.1/promising_stocks.egg-info/SOURCES.txt
+-rw-r--r--   0 ryota      (501) staff       (20)        1 2024-05-24 10:12:26.000000 promising_stocks-0.1.1/promising_stocks.egg-info/dependency_links.txt
+-rw-r--r--   0 ryota      (501) staff       (20)       17 2024-05-24 10:12:26.000000 promising_stocks-0.1.1/promising_stocks.egg-info/top_level.txt
+-rw-r--r--   0 ryota      (501) staff       (20)       38 2024-05-24 10:12:26.524191 promising_stocks-0.1.1/setup.cfg
+-rw-r--r--   0 ryota      (501) staff       (20)      623 2024-05-24 10:12:14.000000 promising_stocks-0.1.1/setup.py
```

### Comparing `promising_stocks-0.1.0/setup.py` & `promising_stocks-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='promising_stocks',
-    version='0.1.0',
+    version='0.1.1',
     author='ryotatakasaki226',
     author_email='s2222022@stu.musashino-u.ac.jp',
     description='A brief description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ryotatakasaki226/pr_st.git',
     packages=find_packages(),
```

