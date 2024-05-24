# Comparing `tmp/logyca_azure_storage_blob-0.0.1rc4.tar.gz` & `tmp/logyca_azure_storage_blob-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logyca_azure_storage_blob-0.0.1rc4.tar", last modified: Fri May 24 20:28:56 2024, max compression
+gzip compressed data, was "logyca_azure_storage_blob-0.1.0.tar", last modified: Fri May 24 20:40:29 2024, max compression
```

## Comparing `logyca_azure_storage_blob-0.0.1rc4.tar` & `logyca_azure_storage_blob-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 20:28:56.634471 logyca_azure_storage_blob-0.0.1rc4/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc4/LICENSE.txt
--rw-rw-rw-   0        0        0     8573 2024-05-24 20:28:56.633474 logyca_azure_storage_blob-0.0.1rc4/PKG-INFO
--rw-rw-rw-   0        0        0     7002 2024-05-24 20:28:00.000000 logyca_azure_storage_blob-0.0.1rc4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 20:28:56.606339 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/
--rw-rw-rw-   0        0        0      270 2024-05-24 17:06:46.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:28:56.607425 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:28:56.627060 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0    42586 2024-05-24 17:15:29.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:28:56.630600 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/
--rw-rw-rw-   0        0        0     8573 2024-05-24 20:28:56.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-05-24 20:28:56.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 20:28:56.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-24 20:28:56.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-24 20:28:56.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 20:28:56.636412 logyca_azure_storage_blob-0.0.1rc4/setup.cfg
--rw-rw-rw-   0        0        0     1890 2024-05-24 20:28:42.000000 logyca_azure_storage_blob-0.0.1rc4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:40:29.311086 logyca_azure_storage_blob-0.1.0/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     8570 2024-05-24 20:40:29.309097 logyca_azure_storage_blob-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7002 2024-05-24 20:28:00.000000 logyca_azure_storage_blob-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 20:40:29.277473 logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob/
+-rw-rw-rw-   0        0        0      270 2024-05-24 17:06:46.000000 logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:40:29.294074 logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:40:29.303322 logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0    42586 2024-05-24 17:15:29.000000 logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:40:29.307123 logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob.egg-info/
+-rw-rw-rw-   0        0        0     8570 2024-05-24 20:40:29.000000 logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-05-24 20:40:29.000000 logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 20:40:29.000000 logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-24 20:40:29.000000 logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-24 20:40:29.000000 logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 20:40:29.313057 logyca_azure_storage_blob-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1887 2024-05-24 20:39:53.000000 logyca_azure_storage_blob-0.1.0/setup.py
```

### Comparing `logyca_azure_storage_blob-0.0.1rc4/LICENSE.txt` & `logyca_azure_storage_blob-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logyca_azure_storage_blob-0.0.1rc4/PKG-INFO` & `logyca_azure_storage_blob-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logyca-azure-storage-blob
-Version: 0.0.1rc4
+Version: 0.1.0
 Summary: An integration package created by the company LOGYCA to interact with the blob container files in your Azure Storage account.
 Home-page: https://github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: azure,blob,storage,upload,download
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: logyca-azure-storage-blob Version: 0.0.1rc4
-Summary: An integration package created by the company LOGYCA to interact with
-the blob container files in your Azure Storage account. Home-page: https://
-github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob Author:
-Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com License: MIT
+Metadata-Version: 2.1 Name: logyca-azure-storage-blob Version: 0.1.0 Summary:
+An integration package created by the company LOGYCA to interact with the blob
+container files in your Azure Storage account. Home-page: https://github.com/
+logyca/python-libraries/tree/main/logyca-azure-storage-blob Author: Jaime
+Andres Cardona Carrillo Author-email: jacardona@outlook.com License: MIT
 License Keywords: azure,blob,storage,upload,download Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

### Comparing `logyca_azure_storage_blob-0.0.1rc4/README.md` & `logyca_azure_storage_blob-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py` & `logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py`

 * *Files identical despite different names*

### Comparing `logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/PKG-INFO` & `logyca_azure_storage_blob-0.1.0/logyca_azure_storage_blob.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logyca-azure-storage-blob
-Version: 0.0.1rc4
+Version: 0.1.0
 Summary: An integration package created by the company LOGYCA to interact with the blob container files in your Azure Storage account.
 Home-page: https://github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: azure,blob,storage,upload,download
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: logyca-azure-storage-blob Version: 0.0.1rc4
-Summary: An integration package created by the company LOGYCA to interact with
-the blob container files in your Azure Storage account. Home-page: https://
-github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob Author:
-Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com License: MIT
+Metadata-Version: 2.1 Name: logyca-azure-storage-blob Version: 0.1.0 Summary:
+An integration package created by the company LOGYCA to interact with the blob
+container files in your Azure Storage account. Home-page: https://github.com/
+logyca/python-libraries/tree/main/logyca-azure-storage-blob Author: Jaime
+Andres Cardona Carrillo Author-email: jacardona@outlook.com License: MIT
 License Keywords: azure,blob,storage,upload,download Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

### Comparing `logyca_azure_storage_blob-0.0.1rc4/setup.py` & `logyca_azure_storage_blob-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="LOGYCA"
 PACKAGE_NAME = "logyca-azure-storage-blob"
-VERSION = "0.0.1rc4"
+VERSION = "0.1.0"
 
 install_requires = ["azure.storage.blob>=12.20.0"]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'An integration package created by the company {COMPANY_NAME} to interact with the blob container files in your Azure Storage account.',
```

