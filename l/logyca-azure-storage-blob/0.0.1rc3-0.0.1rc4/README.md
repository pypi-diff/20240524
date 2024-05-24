# Comparing `tmp/logyca_azure_storage_blob-0.0.1rc3.tar.gz` & `tmp/logyca_azure_storage_blob-0.0.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logyca_azure_storage_blob-0.0.1rc3.tar", last modified: Fri May 24 20:25:06 2024, max compression
+gzip compressed data, was "logyca_azure_storage_blob-0.0.1rc4.tar", last modified: Fri May 24 20:28:56 2024, max compression
```

## Comparing `logyca_azure_storage_blob-0.0.1rc3.tar` & `logyca_azure_storage_blob-0.0.1rc4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 20:25:06.858213 logyca_azure_storage_blob-0.0.1rc3/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc3/LICENSE.txt
--rw-rw-rw-   0        0        0     8492 2024-05-24 20:25:06.858213 logyca_azure_storage_blob-0.0.1rc3/PKG-INFO
--rw-rw-rw-   0        0        0     6916 2024-05-24 20:24:15.000000 logyca_azure_storage_blob-0.0.1rc3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 20:25:06.827401 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/
--rw-rw-rw-   0        0        0      270 2024-05-24 17:06:46.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:25:06.850733 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:25:06.854557 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0    42586 2024-05-24 17:15:29.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:25:06.858213 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob.egg-info/
--rw-rw-rw-   0        0        0     8492 2024-05-24 20:25:06.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-05-24 20:25:06.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 20:25:06.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-24 20:25:06.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-24 20:25:06.000000 logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 20:25:06.858213 logyca_azure_storage_blob-0.0.1rc3/setup.cfg
--rw-rw-rw-   0        0        0     1890 2024-05-24 20:24:46.000000 logyca_azure_storage_blob-0.0.1rc3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:28:56.634471 logyca_azure_storage_blob-0.0.1rc4/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc4/LICENSE.txt
+-rw-rw-rw-   0        0        0     8573 2024-05-24 20:28:56.633474 logyca_azure_storage_blob-0.0.1rc4/PKG-INFO
+-rw-rw-rw-   0        0        0     7002 2024-05-24 20:28:00.000000 logyca_azure_storage_blob-0.0.1rc4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 20:28:56.606339 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/
+-rw-rw-rw-   0        0        0      270 2024-05-24 17:06:46.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:28:56.607425 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:28:56.627060 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0    42586 2024-05-24 17:15:29.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:28:56.630600 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/
+-rw-rw-rw-   0        0        0     8573 2024-05-24 20:28:56.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-05-24 20:28:56.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 20:28:56.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-24 20:28:56.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-24 20:28:56.000000 logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 20:28:56.636412 logyca_azure_storage_blob-0.0.1rc4/setup.cfg
+-rw-rw-rw-   0        0        0     1890 2024-05-24 20:28:42.000000 logyca_azure_storage_blob-0.0.1rc4/setup.py
```

### Comparing `logyca_azure_storage_blob-0.0.1rc3/LICENSE.txt` & `logyca_azure_storage_blob-0.0.1rc4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logyca_azure_storage_blob-0.0.1rc3/PKG-INFO` & `logyca_azure_storage_blob-0.0.1rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logyca-azure-storage-blob
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: An integration package created by the company LOGYCA to interact with the blob container files in your Azure Storage account.
 Home-page: https://github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: azure,blob,storage,upload,download
 Classifier: Development Status :: 4 - Beta
@@ -73,29 +73,31 @@
 
 ```Python
 # Check SQLAlchemy dependency that is installed
 pip install logyca_azure_storage_blob
 ```
 
 
-# Checksum â€“ File Integrity Verification
+# How azcopy performs file consistency validation
 
 Like azcopy, Microsoft's client for uploading large files to Blob, the md5 hash must be computed locally and uploaded to the blob properties along with the file, the blob service will commit this at the end of the process, returning an error if presents inconsistency in value.
 
 ## Calculates the MD5 hash of the file content and saves it as the Content-MD5 property of the blob:
 
 
 ```console
 azcopy --put-md5 #
 ```
 
 References:
 
     - https://learn.microsoft.com/en-us/azure/storage/common/storage-ref-azcopy-copy
 
+This library uses the concepts of the azcopy client for its implementation.
+
 ---
 
 # Test upload
 
 bandwith movistar: upload/download: 300 mbps
 
 ## Test 1, function: container_blob_upload_staging_blocks_commit with console output
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logyca-azure-storage-blob Version: 0.0.1rc3
+Metadata-Version: 2.1 Name: logyca-azure-storage-blob Version: 0.0.1rc4
 Summary: An integration package created by the company LOGYCA to interact with
 the blob container files in your Azure Storage account. Home-page: https://
 github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob Author:
 Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com License: MIT
 License Keywords: azure,blob,storage,upload,download Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
@@ -25,24 +25,25 @@
 --- # About us * _L_O_G_Y_C_A_ _C_o_m_p_a_n_y * _L_O_G_Y_C_A_ _Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l * _[_L_i_n_k_e_d_i_n_]*
 _[_T_w_i_t_t_e_r_]* _[_F_a_c_e_b_o_o_k_]--- # LOGYCA public libraries: To interact with the blob
 container files in your Azure Storage account. [Source code](https://
 github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob) |
 [Package (PyPI)](https://pypi.org/project/logyca-azure-storage-blob/) |
 [Samples](https://github.com/logyca/python-libraries/tree/main/logyca-azure-
 storage-blob/samples) --- To install the libraries ```Python # Check SQLAlchemy
-dependency that is installed pip install logyca_azure_storage_blob ``` #
-Checksum Ã¢â¬â File Integrity Verification Like azcopy, Microsoft's client
-for uploading large files to Blob, the md5 hash must be computed locally and
+dependency that is installed pip install logyca_azure_storage_blob ``` # How
+azcopy performs file consistency validation Like azcopy, Microsoft's client for
+uploading large files to Blob, the md5 hash must be computed locally and
 uploaded to the blob properties along with the file, the blob service will
 commit this at the end of the process, returning an error if presents
 inconsistency in value. ## Calculates the MD5 hash of the file content and
 saves it as the Content-MD5 property of the blob: ```console azcopy --put-md5 #
 ``` References: - https://learn.microsoft.com/en-us/azure/storage/common/
-storage-ref-azcopy-copy --- # Test upload bandwith movistar: upload/download:
-300 mbps ## Test 1, function: container_blob_upload_staging_blocks_commit with
+storage-ref-azcopy-copy This library uses the concepts of the azcopy client for
+its implementation. --- # Test upload bandwith movistar: upload/download: 300
+mbps ## Test 1, function: container_blob_upload_staging_blocks_commit with
 console output file: 20240126084440-backup.dump size: 2.03 GB parameters: -
 self.__chunk_size_bytes=4*1024*1024 # Defaults 4 MiB Elapsed time: 00:05:22
 Output: Upload process: file_to_upload[20240126084440-backup.dump], Chunks[42/
 522], Percentage[8.05%] Upload process: file_to_upload[20240126084440-
 backup.dump], Chunks[43/522], Percentage[8.24%] Upload process: file_to_upload
 [20240126084440-backup.dump], Chunks[44/522], Percentage[8.43%] Upload process:
 file_to_upload[20240126084440-backup.dump], Chunks[45/522], Percentage[8.62%]
```

### Comparing `logyca_azure_storage_blob-0.0.1rc3/README.md` & `logyca_azure_storage_blob-0.0.1rc4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,29 +39,31 @@
 
 ```Python
 # Check SQLAlchemy dependency that is installed
 pip install logyca_azure_storage_blob
 ```
 
 
-# Checksum – File Integrity Verification
+# How azcopy performs file consistency validation
 
 Like azcopy, Microsoft's client for uploading large files to Blob, the md5 hash must be computed locally and uploaded to the blob properties along with the file, the blob service will commit this at the end of the process, returning an error if presents inconsistency in value.
 
 ## Calculates the MD5 hash of the file content and saves it as the Content-MD5 property of the blob:
 
 
 ```console
 azcopy --put-md5 #
 ```
 
 References:
 
     - https://learn.microsoft.com/en-us/azure/storage/common/storage-ref-azcopy-copy
 
+This library uses the concepts of the azcopy client for its implementation.
+
 ---
 
 # Test upload
 
 bandwith movistar: upload/download: 300 mbps
 
 ## Test 1, function: container_blob_upload_staging_blocks_commit with console output
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -4,24 +4,25 @@
 --- # About us * _L_O_G_Y_C_A_ _C_o_m_p_a_n_y * _L_O_G_Y_C_A_ _Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l * _[_L_i_n_k_e_d_i_n_]*
 _[_T_w_i_t_t_e_r_]* _[_F_a_c_e_b_o_o_k_]--- # LOGYCA public libraries: To interact with the blob
 container files in your Azure Storage account. [Source code](https://
 github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob) |
 [Package (PyPI)](https://pypi.org/project/logyca-azure-storage-blob/) |
 [Samples](https://github.com/logyca/python-libraries/tree/main/logyca-azure-
 storage-blob/samples) --- To install the libraries ```Python # Check SQLAlchemy
-dependency that is installed pip install logyca_azure_storage_blob ``` #
-Checksum â File Integrity Verification Like azcopy, Microsoft's client for
+dependency that is installed pip install logyca_azure_storage_blob ``` # How
+azcopy performs file consistency validation Like azcopy, Microsoft's client for
 uploading large files to Blob, the md5 hash must be computed locally and
 uploaded to the blob properties along with the file, the blob service will
 commit this at the end of the process, returning an error if presents
 inconsistency in value. ## Calculates the MD5 hash of the file content and
 saves it as the Content-MD5 property of the blob: ```console azcopy --put-md5 #
 ``` References: - https://learn.microsoft.com/en-us/azure/storage/common/
-storage-ref-azcopy-copy --- # Test upload bandwith movistar: upload/download:
-300 mbps ## Test 1, function: container_blob_upload_staging_blocks_commit with
+storage-ref-azcopy-copy This library uses the concepts of the azcopy client for
+its implementation. --- # Test upload bandwith movistar: upload/download: 300
+mbps ## Test 1, function: container_blob_upload_staging_blocks_commit with
 console output file: 20240126084440-backup.dump size: 2.03 GB parameters: -
 self.__chunk_size_bytes=4*1024*1024 # Defaults 4 MiB Elapsed time: 00:05:22
 Output: Upload process: file_to_upload[20240126084440-backup.dump], Chunks[42/
 522], Percentage[8.05%] Upload process: file_to_upload[20240126084440-
 backup.dump], Chunks[43/522], Percentage[8.24%] Upload process: file_to_upload
 [20240126084440-backup.dump], Chunks[44/522], Percentage[8.43%] Upload process:
 file_to_upload[20240126084440-backup.dump], Chunks[45/522], Percentage[8.62%]
```

### Comparing `logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py` & `logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob/utils/helpers/azure_storage_account_blob_management.py`

 * *Files identical despite different names*

### Comparing `logyca_azure_storage_blob-0.0.1rc3/logyca_azure_storage_blob.egg-info/PKG-INFO` & `logyca_azure_storage_blob-0.0.1rc4/logyca_azure_storage_blob.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logyca-azure-storage-blob
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: An integration package created by the company LOGYCA to interact with the blob container files in your Azure Storage account.
 Home-page: https://github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: azure,blob,storage,upload,download
 Classifier: Development Status :: 4 - Beta
@@ -73,29 +73,31 @@
 
 ```Python
 # Check SQLAlchemy dependency that is installed
 pip install logyca_azure_storage_blob
 ```
 
 
-# Checksum â€“ File Integrity Verification
+# How azcopy performs file consistency validation
 
 Like azcopy, Microsoft's client for uploading large files to Blob, the md5 hash must be computed locally and uploaded to the blob properties along with the file, the blob service will commit this at the end of the process, returning an error if presents inconsistency in value.
 
 ## Calculates the MD5 hash of the file content and saves it as the Content-MD5 property of the blob:
 
 
 ```console
 azcopy --put-md5 #
 ```
 
 References:
 
     - https://learn.microsoft.com/en-us/azure/storage/common/storage-ref-azcopy-copy
 
+This library uses the concepts of the azcopy client for its implementation.
+
 ---
 
 # Test upload
 
 bandwith movistar: upload/download: 300 mbps
 
 ## Test 1, function: container_blob_upload_staging_blocks_commit with console output
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logyca-azure-storage-blob Version: 0.0.1rc3
+Metadata-Version: 2.1 Name: logyca-azure-storage-blob Version: 0.0.1rc4
 Summary: An integration package created by the company LOGYCA to interact with
 the blob container files in your Azure Storage account. Home-page: https://
 github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob Author:
 Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com License: MIT
 License Keywords: azure,blob,storage,upload,download Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
@@ -25,24 +25,25 @@
 --- # About us * _L_O_G_Y_C_A_ _C_o_m_p_a_n_y * _L_O_G_Y_C_A_ _Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l * _[_L_i_n_k_e_d_i_n_]*
 _[_T_w_i_t_t_e_r_]* _[_F_a_c_e_b_o_o_k_]--- # LOGYCA public libraries: To interact with the blob
 container files in your Azure Storage account. [Source code](https://
 github.com/logyca/python-libraries/tree/main/logyca-azure-storage-blob) |
 [Package (PyPI)](https://pypi.org/project/logyca-azure-storage-blob/) |
 [Samples](https://github.com/logyca/python-libraries/tree/main/logyca-azure-
 storage-blob/samples) --- To install the libraries ```Python # Check SQLAlchemy
-dependency that is installed pip install logyca_azure_storage_blob ``` #
-Checksum Ã¢â¬â File Integrity Verification Like azcopy, Microsoft's client
-for uploading large files to Blob, the md5 hash must be computed locally and
+dependency that is installed pip install logyca_azure_storage_blob ``` # How
+azcopy performs file consistency validation Like azcopy, Microsoft's client for
+uploading large files to Blob, the md5 hash must be computed locally and
 uploaded to the blob properties along with the file, the blob service will
 commit this at the end of the process, returning an error if presents
 inconsistency in value. ## Calculates the MD5 hash of the file content and
 saves it as the Content-MD5 property of the blob: ```console azcopy --put-md5 #
 ``` References: - https://learn.microsoft.com/en-us/azure/storage/common/
-storage-ref-azcopy-copy --- # Test upload bandwith movistar: upload/download:
-300 mbps ## Test 1, function: container_blob_upload_staging_blocks_commit with
+storage-ref-azcopy-copy This library uses the concepts of the azcopy client for
+its implementation. --- # Test upload bandwith movistar: upload/download: 300
+mbps ## Test 1, function: container_blob_upload_staging_blocks_commit with
 console output file: 20240126084440-backup.dump size: 2.03 GB parameters: -
 self.__chunk_size_bytes=4*1024*1024 # Defaults 4 MiB Elapsed time: 00:05:22
 Output: Upload process: file_to_upload[20240126084440-backup.dump], Chunks[42/
 522], Percentage[8.05%] Upload process: file_to_upload[20240126084440-
 backup.dump], Chunks[43/522], Percentage[8.24%] Upload process: file_to_upload
 [20240126084440-backup.dump], Chunks[44/522], Percentage[8.43%] Upload process:
 file_to_upload[20240126084440-backup.dump], Chunks[45/522], Percentage[8.62%]
```

### Comparing `logyca_azure_storage_blob-0.0.1rc3/setup.py` & `logyca_azure_storage_blob-0.0.1rc4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="LOGYCA"
 PACKAGE_NAME = "logyca-azure-storage-blob"
-VERSION = "0.0.1rc3"
+VERSION = "0.0.1rc4"
 
 install_requires = ["azure.storage.blob>=12.20.0"]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'An integration package created by the company {COMPANY_NAME} to interact with the blob container files in your Azure Storage account.',
```

