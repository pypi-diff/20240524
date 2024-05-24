# Comparing `tmp/logyca_azure_storage_blob-0.0.1rc1.tar.gz` & `tmp/logyca_azure_storage_blob-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logyca_azure_storage_blob-0.0.1rc1.tar", last modified: Fri May 24 17:11:03 2024, max compression
+gzip compressed data, was "logyca_azure_storage_blob-0.0.1rc2.tar", last modified: Fri May 24 17:15:47 2024, max compression
```

## Comparing `logyca_azure_storage_blob-0.0.1rc1.tar` & `logyca_azure_storage_blob-0.0.1rc2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 17:11:03.554536 logyca_azure_storage_blob-0.0.1rc1/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc1/LICENSE.txt
--rw-rw-rw-   0        0        0     5044 2024-05-24 17:11:03.554536 logyca_azure_storage_blob-0.0.1rc1/PKG-INFO
--rw-rw-rw-   0        0        0     3483 2024-05-24 17:10:04.000000 logyca_azure_storage_blob-0.0.1rc1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 17:11:03.521839 logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob/
--rw-rw-rw-   0        0        0      270 2024-05-24 17:06:46.000000 logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 17:11:03.554536 logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 17:11:03.554536 logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0    42730 2024-05-22 01:51:51.000000 logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py
-drwxrwxrwx   0        0        0        0 2024-05-24 17:11:03.554536 logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob.egg-info/
--rw-rw-rw-   0        0        0     5044 2024-05-24 17:11:03.000000 logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-05-24 17:11:03.000000 logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 17:11:03.000000 logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-24 17:11:03.000000 logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-24 17:11:03.000000 logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 17:11:03.569827 logyca_azure_storage_blob-0.0.1rc1/setup.cfg
--rw-rw-rw-   0        0        0     1877 2024-05-24 17:03:51.000000 logyca_azure_storage_blob-0.0.1rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 17:15:47.865635 logyca_azure_storage_blob-0.0.1rc2/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5044 2024-05-24 17:15:47.865635 logyca_azure_storage_blob-0.0.1rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     3483 2024-05-24 17:10:04.000000 logyca_azure_storage_blob-0.0.1rc2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 17:15:47.834658 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/
+-rw-rw-rw-   0        0        0      270 2024-05-24 17:06:46.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 17:15:47.850705 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 17:15:47.850705 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0    42586 2024-05-24 17:15:29.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py
+drwxrwxrwx   0        0        0        0 2024-05-24 17:15:47.850705 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob.egg-info/
+-rw-rw-rw-   0        0        0     5044 2024-05-24 17:15:47.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-05-24 17:15:47.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 17:15:47.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-24 17:15:47.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-24 17:15:47.000000 logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 17:15:47.865635 logyca_azure_storage_blob-0.0.1rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1877 2024-05-24 17:15:40.000000 logyca_azure_storage_blob-0.0.1rc2/setup.py
```

### Comparing `logyca_azure_storage_blob-0.0.1rc1/LICENSE.txt` & `logyca_azure_storage_blob-0.0.1rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logyca_azure_storage_blob-0.0.1rc1/PKG-INFO` & `logyca_azure_storage_blob-0.0.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logyca-azure-storage-blob
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: An integration package created by the company LOGYCA to interact with the blob container files in your Azure Storage account.
 Home-page: https://github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: postgres,driver database
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logyca-azure-storage-blob Version: 0.0.1rc1
+Metadata-Version: 2.1 Name: logyca-azure-storage-blob Version: 0.0.1rc2
 Summary: An integration package created by the company LOGYCA to interact with
 the blob container files in your Azure Storage account. Home-page: https://
 github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob Author:
 Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com License: MIT
 License Keywords: postgres,driver database Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `logyca_azure_storage_blob-0.0.1rc1/README.md` & `logyca_azure_storage_blob-0.0.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py` & `logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     def get_connect_status(self):
         '''Description
         :return bool: True if exist attribute sku_name in account_information, otherwise return False due to connection failure to the storage account
 
         ## Examples
 
         ```Python
-        from azure_storage_account_blob_management import AzureStorageAccountBlobManagement, SetCredentialsNameKey, SetCredentialsConnectionString
+        from logyca_azure_storage_blob import AzureStorageAccountBlobManagement, SetCredentialsNameKey, SetCredentialsConnectionString
 
         asabm=AzureStorageAccountBlobManagement(SetCredentialsNameKey(account_name="",key=""))
         print("SetCredentialsNameKey: Successfully connection") if asabm.get_connect_status() else print("SetCredentialsNameKey: Failed connection")
 
         asabm=AzureStorageAccountBlobManagement(SetCredentialsConnectionString(connection_string=""))
         print("SetCredentialsNameKey: Successfully connection") if asabm.get_connect_status() else print("SetCredentialsNameKey: Failed connection")
 
@@ -106,15 +106,15 @@
     def get_account_information(self):
         '''Description
         :return list: list of account information
 
         ## Examples
 
         ```Python
-        from azure_storage_account_blob_management import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
+        from logyca_azure_storage_blob import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
         import json
 
         asabm=AzureStorageAccountBlobManagement(SetCredentialsConnectionString(connection_string=""))
         data=asabm.get_account_information()
         print(json.dumps(data,indent=4))
         ```
         '''
@@ -153,15 +153,15 @@
         '''Description
         :param name:str         : Name of new container.
         :param public_access:str: Possible values None,container,blob.
         :return bool|str        : True if Ok, otherwise string message exception.
 
         ## Example
         ```Python
-        from azure_storage_account_blob_management import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
+        from logyca_azure_storage_blob import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
 
         asabm=AzureStorageAccountBlobManagement(SetCredentialsConnectionString(connection_string=""))
         status=asabm.container_create("name")
         if status is True:
             print("ok...")
         else:
             print(status)
@@ -179,15 +179,15 @@
     def container_delete(self,name:str)->bool|str:
         '''Description
         :param name:str     : Name of new container.
         :return bool|str    : True if Ok, otherwise string message exception.
 
         ## Example
         ```Python
-        from azure_storage_account_blob_management import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
+        from logyca_azure_storage_blob import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
 
         asabm=AzureStorageAccountBlobManagement(SetCredentialsConnectionString(connection_string=""))
         status=asabm.container_delete("name")
         if status is True:
             print("ok...")
         else:
             print(status)
@@ -208,15 +208,15 @@
     def container_blob_list(self,container_name:str)->list[BlobProperties]:
         '''Description
         :param container_name:str   : Name of container.
         :return list                : list of blobs in container name.
 
         ## Example
         ```Python
-        from azure_storage_account_blob_management import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
+        from logyca_azure_storage_blob import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
         from azure.storage.blob import BlobProperties
 
         asabm=AzureStorageAccountBlobManagement(SetCredentialsConnectionString(connection_string=""))
         blob_list=asabm.container_blob_list("container_name")
         if(isinstance(blob_list,list)):
             for blob in blob_list:
                 print("----------------------")
@@ -244,15 +244,15 @@
         :param blob_file:str                : Blob name with extention to get the info.
         :param container_name:str           : Name of container.
         :param container_folders:list[str]  : Subfolders where the blob file is located. Default root container.
         :return list                        : BlobProperties or Exception message
 
         ## Example
         ```Python
-        from azure_storage_account_blob_management import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
+        from logyca_azure_storage_blob import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
         from azure.storage.blob import BlobProperties
 
         asabm=AzureStorageAccountBlobManagement(SetCredentialsConnectionString(connection_string=""))
 
         # Example 1 - Small file
         # Container root path
         blob_file='upload.txt'
@@ -309,15 +309,15 @@
         :param verify_file_integrity:bool   : Enable checksum verification with content_md5
         :param print_charge_percentage:bool : prints data and percentage of progress of the process in the console.
         :return bool|str                    : True if Ok, otherwise string message exception.
 
         ## Examples
 
         ```Python
-        from azure_storage_account_blob_management import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
+        from logyca_azure_storage_blob import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
         from jaanca_chronometer import Chronometer # pip install jaanca-chronometer
         import os
 
         asabm=AzureStorageAccountBlobManagement(SetCredentialsConnectionString(connection_string=""))
         chronometer=Chronometer()
         folder_local_full_path=os.path.abspath(os.path.join(os.path.dirname(__file__),'files'))
         file='upload.txt'
@@ -403,15 +403,15 @@
         :param max_concurrency:int          : This argument defines the maximum number of parallel connections to use when the blob size exceeds 64 MiB.
         :param verify_file_integrity:bool   : Enable checksum verification with content_md5
         :return bool|str                    : True if Ok, otherwise string message exception.
 
         ## Examples
 
         ```Python
-        from azure_storage_account_blob_management import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
+        from logyca_azure_storage_blob import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
         from jaanca_chronometer import Chronometer # pip install jaanca-chronometer
         import os
         
         chronometer=Chronometer()
         asabm=AzureStorageAccountBlobManagement(SetCredentialsConnectionString(connection_string=""))
 
         # Container root path
@@ -490,15 +490,15 @@
         :param max_concurrency:int          : This argument defines the maximum number of parallel connections to use when the blob size exceeds 64 MiB.
         :param verify_file_integrity:bool   : Enable checksum verification with content_md5
         :return bool|str                    : True if Ok, otherwise string message exception.
 
         ## Examples
 
         ```Python
-        from azure_storage_account_blob_management import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
+        from logyca_azure_storage_blob import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
         from jaanca_chronometer import Chronometer # pip install jaanca-chronometer
         import os
 
         asabm=AzureStorageAccountBlobManagement(SetCredentialsConnectionString(connection_string=""))
         chronometer=Chronometer()
 
         # Container root path
@@ -571,15 +571,15 @@
         :param container_name:str           : Container name.
         :param container_folders:list[str]  : Subfolders to upload files to the container. Default root container.
         :return bool|str                    : True if Ok, otherwise string message exception.
 
         ## Examples
 
         ```Python
-        from azure_storage_account_blob_management import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
+        from logyca_azure_storage_blob import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
         import os
 
         asabm=AzureStorageAccountBlobManagement(SetCredentialsConnectionString(connection_string=""))
 
         # Container root path
         file='upload.txt'
         status=asabm.container_blob_delete(file,App.AzureStorageAccount.Containers.NAME_WITH_DATA)
@@ -673,15 +673,15 @@
         :param prefix_within_the_message:str    : Text to write to the file before the message, to differentiate messages. Suggested date and time.
         :param container_folders:list[str]      : Subfolders to upload files to the container. Default logs folder at the root of the container.
         :return bool|str                        : True if Ok, otherwise string message exception.
 
         ## Examples
 
         ```Python
-        from azure_storage_account_blob_management import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
+        from logyca_azure_storage_blob import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
 
         asabm=AzureStorageAccountBlobManagement(SetCredentialsConnectionString(connection_string=""))
 
         # Example 1 - INFO
         # Container root path
         preffix_name="app_worker"
         message = "text text...\ntext text...\ntext text...\ntext text...\n"
@@ -798,15 +798,15 @@
         :param container_name:str           : Container name.
         :param container_folders:list[str]  : Subfolders to upload files to the container. Default root container.
         :return bool|str                    : True if Ok, otherwise string message exception.
 
         ## Example
         
         ```Python
-        from azure_storage_account_blob_management import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
+        from logyca_azure_storage_blob import AzureStorageAccountBlobManagement, SetCredentialsConnectionString
         import os
 
         asabm=AzureStorageAccountBlobManagement(SetCredentialsConnectionString(connection_string=""))
         folder_local_full_path=os.path.abspath(os.path.join(os.path.dirname(__file__),'files'))
 
         # Example 1 - Small file
         # Container root path
```

### Comparing `logyca_azure_storage_blob-0.0.1rc1/logyca_azure_storage_blob.egg-info/PKG-INFO` & `logyca_azure_storage_blob-0.0.1rc2/logyca_azure_storage_blob.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logyca-azure-storage-blob
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: An integration package created by the company LOGYCA to interact with the blob container files in your Azure Storage account.
 Home-page: https://github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: postgres,driver database
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logyca-azure-storage-blob Version: 0.0.1rc1
+Metadata-Version: 2.1 Name: logyca-azure-storage-blob Version: 0.0.1rc2
 Summary: An integration package created by the company LOGYCA to interact with
 the blob container files in your Azure Storage account. Home-page: https://
 github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob Author:
 Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com License: MIT
 License Keywords: postgres,driver database Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `logyca_azure_storage_blob-0.0.1rc1/setup.py` & `logyca_azure_storage_blob-0.0.1rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="LOGYCA"
 PACKAGE_NAME = "logyca-azure-storage-blob"
-VERSION = "0.0.1rc1"
+VERSION = "0.0.1rc2"
 
 install_requires = ["azure.storage.blob>=12.20.0"]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'An integration package created by the company {COMPANY_NAME} to interact with the blob container files in your Azure Storage account.',
```

