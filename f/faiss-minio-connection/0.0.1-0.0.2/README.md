# Comparing `tmp/faiss-minio-connection-0.0.1.tar.gz` & `tmp/faiss-minio-connection-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faiss-minio-connection-0.0.1.tar", last modified: Thu May 23 22:06:34 2024, max compression
+gzip compressed data, was "faiss-minio-connection-0.0.2.tar", last modified: Fri May 24 11:21:31 2024, max compression
```

## Comparing `faiss-minio-connection-0.0.1.tar` & `faiss-minio-connection-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 22:06:34.130781 faiss-minio-connection-0.0.1/
--rw-rw-rw-   0        0        0      534 2024-05-23 22:06:34.130781 faiss-minio-connection-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-23 20:56:33.000000 faiss-minio-connection-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 22:06:33.875779 faiss-minio-connection-0.0.1/faiss_minio/
--rw-rw-rw-   0        0        0       26 2024-05-23 20:53:42.000000 faiss-minio-connection-0.0.1/faiss_minio/__init__.py
--rw-rw-rw-   0        0        0     6952 2024-05-23 20:32:29.000000 faiss-minio-connection-0.0.1/faiss_minio/faiss_minio.py
-drwxrwxrwx   0        0        0        0 2024-05-23 22:06:34.086780 faiss-minio-connection-0.0.1/faiss_minio_connection.egg-info/
--rw-rw-rw-   0        0        0      534 2024-05-23 22:06:33.000000 faiss-minio-connection-0.0.1/faiss_minio_connection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-05-23 22:06:33.000000 faiss-minio-connection-0.0.1/faiss_minio_connection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 22:06:33.000000 faiss-minio-connection-0.0.1/faiss_minio_connection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2024-05-23 22:06:33.000000 faiss-minio-connection-0.0.1/faiss_minio_connection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-23 22:06:33.000000 faiss-minio-connection-0.0.1/faiss_minio_connection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 22:06:34.174726 faiss-minio-connection-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1122 2024-05-23 22:06:27.000000 faiss-minio-connection-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:21:31.166613 faiss-minio-connection-0.0.2/
+-rw-rw-rw-   0        0        0      534 2024-05-24 11:21:31.166613 faiss-minio-connection-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2873 2024-05-24 11:19:42.000000 faiss-minio-connection-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 11:21:31.010050 faiss-minio-connection-0.0.2/faiss_minio/
+-rw-rw-rw-   0        0        0       26 2024-05-23 20:53:42.000000 faiss-minio-connection-0.0.2/faiss_minio/__init__.py
+-rw-rw-rw-   0        0        0     6952 2024-05-23 20:32:29.000000 faiss-minio-connection-0.0.2/faiss_minio/faiss_minio.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:21:31.143563 faiss-minio-connection-0.0.2/faiss_minio_connection.egg-info/
+-rw-rw-rw-   0        0        0      534 2024-05-24 11:21:30.000000 faiss-minio-connection-0.0.2/faiss_minio_connection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2024-05-24 11:21:30.000000 faiss-minio-connection-0.0.2/faiss_minio_connection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 11:21:30.000000 faiss-minio-connection-0.0.2/faiss_minio_connection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2024-05-24 11:21:30.000000 faiss-minio-connection-0.0.2/faiss_minio_connection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-24 11:21:30.000000 faiss-minio-connection-0.0.2/faiss_minio_connection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 11:21:31.200796 faiss-minio-connection-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2024-05-24 11:21:26.000000 faiss-minio-connection-0.0.2/setup.py
```

### Comparing `faiss-minio-connection-0.0.1/PKG-INFO` & `faiss-minio-connection-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faiss-minio-connection
-Version: 0.0.1
+Version: 0.0.2
 Summary: Combining FAISS work with S3 cloud storage.
 Home-page: https://github.com/Ilya-Akulov/FAISS-Minio
 Author: ilya_a
 Author-email: iakulpypi@mail.ru
 Project-URL: GitHub, https://github.com/Ilya-Akulov/FAISS-Minio
 Keywords: FAISS Minio
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `faiss-minio-connection-0.0.1/faiss_minio/faiss_minio.py` & `faiss-minio-connection-0.0.2/faiss_minio/faiss_minio.py`

 * *Files identical despite different names*

### Comparing `faiss-minio-connection-0.0.1/faiss_minio_connection.egg-info/PKG-INFO` & `faiss-minio-connection-0.0.2/faiss_minio_connection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faiss-minio-connection
-Version: 0.0.1
+Version: 0.0.2
 Summary: Combining FAISS work with S3 cloud storage.
 Home-page: https://github.com/Ilya-Akulov/FAISS-Minio
 Author: ilya_a
 Author-email: iakulpypi@mail.ru
 Project-URL: GitHub, https://github.com/Ilya-Akulov/FAISS-Minio
 Keywords: FAISS Minio
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `faiss-minio-connection-0.0.1/setup.py` & `faiss-minio-connection-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 
 def readme():
-  with open('README.md', 'r') as f:
-    return f.read()
+    with open('README.md', 'r', encoding='UTF8') as f:
+        f.read()
 
 
 setup(
   name='faiss-minio-connection',
-  version='0.0.1',
+  version='0.0.2',
   author='ilya_a',
   author_email='iakulpypi@mail.ru',
   description='Combining FAISS work with S3 cloud storage.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Ilya-Akulov/FAISS-Minio',
   packages=find_packages(),
```

