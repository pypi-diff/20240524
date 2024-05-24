# Comparing `tmp/logyca_azure_storage_blob-0.0.1rc2.tar.gz` & `tmp/logyca_azure_storage_blob-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logyca_azure_storage_blob-0.0.1rc2.tar", last modified: Fri May 24 17:15:47 2024, max compression
+gzip compressed data, was "logyca_azure_storage_blob-0.0.1rc3.tar", last modified: Fri May 24 20:25:06 2024, max compression
```

## Comparing `logyca_azure_storage_blob-0.0.1rc2.tar` & `logyca_azure_storage_blob-0.0.1rc3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 17:15:47.865635 logyca_azure_storage_blob-0.0.1rc2/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc2/LICENSE.txt
--rw-rw-rw-   0        0        0     5044 2024-05-24 17:15:47.865635 logyca_azure_storage_blob-0.0.1rc2/PKG-INFO
--rw-rw-rw-   0        0        0     3483 2024-05-24 17:10:04.000000 logyca_azure_storage_blob-0.0.1rc2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 17:15:47.834658 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/
--rw-rw-rw-   0        0        0      270 2024-05-24 17:06:46.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 17:15:47.850705 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 17:15:47.850705 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0    42586 2024-05-24 17:15:29.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py
-drwxrwxrwx   0        0        0        0 2024-05-24 17:15:47.850705 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob.egg-info/
--rw-rw-rw-   0        0        0     5044 2024-05-24 17:15:47.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-05-24 17:15:47.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 17:15:47.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-24 17:15:47.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-24 17:15:47.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 17:15:47.865635 logyca_azure_storage_blob-0.0.1rc2/setup.cfg
--rw-rw-rw-   0        0        0     1877 2024-05-24 17:15:40.000000 logyca_azure_storage_blob-0.0.1rc2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:25:06.858213 logyca_azure_storage_blob-0.0.1rc3/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc3/LICENSE.txt
+-rw-rw-rw-   0        0        0     8492 2024-05-24 20:25:06.858213 logyca_azure_storage_blob-0.0.1rc3/PKG-INFO
+-rw-rw-rw-   0        0        0     6916 2024-05-24 20:24:15.000000 logyca_azure_storage_blob-0.0.1rc3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 20:25:06.827401 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/
+-rw-rw-rw-   0        0        0      270 2024-05-24 17:06:46.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:25:06.850733 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:25:06.854557 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0    42586 2024-05-24 17:15:29.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:25:06.858213 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob.egg-info/
+-rw-rw-rw-   0        0        0     8492 2024-05-24 20:25:06.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-05-24 20:25:06.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 20:25:06.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-24 20:25:06.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-24 20:25:06.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 20:25:06.858213 logyca_azure_storage_blob-0.0.1rc3/setup.cfg
+-rw-rw-rw-   0        0        0     1890 2024-05-24 20:24:46.000000 logyca_azure_storage_blob-0.0.1rc3/setup.py
```

### Comparing `logyca_azure_storage_blob-0.0.1rc2/LICENSE.txt` & `logyca_azure_storage_blob-0.0.1rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py` & `logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py`

 * *Files identical despite different names*

### Comparing `logyca_azure_storage_blob-0.0.1rc2/setup.py` & `logyca_azure_storage_blob-0.0.1rc3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="LOGYCA"
 PACKAGE_NAME = "logyca-azure-storage-blob"
-VERSION = "0.0.1rc2"
+VERSION = "0.0.1rc3"
 
 install_requires = ["azure.storage.blob>=12.20.0"]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'An integration package created by the company {COMPANY_NAME} to interact with the blob container files in your Azure Storage account.',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     author='Jaime Andres Cardona Carrillo',
     author_email='jacardona@outlook.com',
     url='https://github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob',
-    keywords="postgres, driver database",
+    keywords="azure, blob, storage, upload, download",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

