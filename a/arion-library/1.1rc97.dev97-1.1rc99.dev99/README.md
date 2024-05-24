# Comparing `tmp/arion_library-1.1rc97.dev97.tar.gz` & `tmp/arion_library-1.1rc99.dev99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc97.dev97.tar", last modified: Thu May  2 09:58:33 2024, max compression
+gzip compressed data, was "arion_library-1.1rc99.dev99.tar", last modified: Tue May 21 10:40:10 2024, max compression
```

## Comparing `arion_library-1.1rc97.dev97.tar` & `arion_library-1.1rc99.dev99.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.220380 arion_library-1.1rc97.dev97/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.212380 arion_library-1.1rc97.dev97/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 09:58:33.000000 arion_library-1.1rc97.dev97/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-02 09:58:33.000000 arion_library-1.1rc97.dev97/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:58:33.000000 arion_library-1.1rc97.dev97/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 09:58:33.000000 arion_library-1.1rc97.dev97/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 09:58:33.000000 arion_library-1.1rc97.dev97/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.212380 arion_library-1.1rc97.dev97/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.212380 arion_library-1.1rc97.dev97/processors/Cegid_Web_Services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/Cegid_Web_Services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.212380 arion_library-1.1rc97.dev97/processors/Cegid_Web_Services/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/Cegid_Web_Services/lib/Convert_Soap_Rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/Cegid_Web_Services/lib/Handle_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/Cegid_Web_Services/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.212380 arion_library-1.1rc97.dev97/processors/Cegid_Web_Services/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/Cegid_Web_Services/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/Cegid_Web_Services/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/Cegid_Web_Services/tests/test_methods_handle_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.212380 arion_library-1.1rc97.dev97/processors/FTP_connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/FTP_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.212380 arion_library-1.1rc97.dev97/processors/FTP_connector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/FTP_connector/lib/FTPconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/FTP_connector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/FTP_connector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/FTP_connector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/FTP_connector/tests/test_ftp_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/OracleConnector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/OracleConnector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/OracleConnector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/OracleConnector/lib/OracleDatabase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/OracleConnector/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/OracleConnector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/OracleConnector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/OracleConnector/tests/test_oracle_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/Shopify_connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/Shopify_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/Shopify_connector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/Shopify_connector/lib/ShopifyConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/Shopify_connector/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6890 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/Shopify_connector/lib/shopifyConnect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/Shopify_connector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/Shopify_connector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/Shopify_connector/tests/test_shopify_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3101 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:58:33.216380 arion_library-1.1rc97.dev97/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-02 09:57:39.000000 arion_library-1.1rc97.dev97/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:58:33.220380 arion_library-1.1rc97.dev97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-02 09:58:31.000000 arion_library-1.1rc97.dev97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.957689 arion_library-1.1rc99.dev99/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 10:40:10.000000 arion_library-1.1rc99.dev99/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-21 10:40:10.000000 arion_library-1.1rc99.dev99/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 10:40:10.000000 arion_library-1.1rc99.dev99/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-21 10:40:10.000000 arion_library-1.1rc99.dev99/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 10:40:10.000000 arion_library-1.1rc99.dev99/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.957689 arion_library-1.1rc99.dev99/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.957689 arion_library-1.1rc99.dev99/processors/Cegid_Web_Services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/Cegid_Web_Services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.957689 arion_library-1.1rc99.dev99/processors/Cegid_Web_Services/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/Cegid_Web_Services/lib/Convert_Soap_Rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/Cegid_Web_Services/lib/Handle_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/Cegid_Web_Services/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.957689 arion_library-1.1rc99.dev99/processors/Cegid_Web_Services/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/Cegid_Web_Services/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/Cegid_Web_Services/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/Cegid_Web_Services/tests/test_methods_handle_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.957689 arion_library-1.1rc99.dev99/processors/FTP_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/FTP_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.957689 arion_library-1.1rc99.dev99/processors/FTP_connector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/FTP_connector/lib/FTPconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/FTP_connector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.957689 arion_library-1.1rc99.dev99/processors/FTP_connector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/FTP_connector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/FTP_connector/tests/test_ftp_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.957689 arion_library-1.1rc99.dev99/processors/OracleConnector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/OracleConnector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.957689 arion_library-1.1rc99.dev99/processors/OracleConnector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/OracleConnector/lib/OracleDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/OracleConnector/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.957689 arion_library-1.1rc99.dev99/processors/OracleConnector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/OracleConnector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/OracleConnector/tests/test_oracle_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.957689 arion_library-1.1rc99.dev99/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/Shopify_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/Shopify_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/Shopify_connector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/Shopify_connector/lib/ShopifyConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/Shopify_connector/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6890 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/Shopify_connector/lib/shopifyConnect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/Shopify_connector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/Shopify_connector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/Shopify_connector/tests/test_shopify_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3101 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-21 10:39:27.000000 arion_library-1.1rc99.dev99/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 10:40:10.961689 arion_library-1.1rc99.dev99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-21 10:40:09.000000 arion_library-1.1rc99.dev99/setup.py
```

### Comparing `arion_library-1.1rc97.dev97/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc99.dev99/arion_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/Cegid_Web_Services/lib/Convert_Soap_Rest.py` & `arion_library-1.1rc99.dev99/processors/Cegid_Web_Services/lib/Convert_Soap_Rest.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/Cegid_Web_Services/lib/Handle_error_response.py` & `arion_library-1.1rc99.dev99/processors/Cegid_Web_Services/lib/Handle_error_response.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/Cegid_Web_Services/tests/test_methods.py` & `arion_library-1.1rc99.dev99/processors/Cegid_Web_Services/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/FTP_connector/lib/FTPconnector.py` & `arion_library-1.1rc99.dev99/processors/FTP_connector/lib/FTPconnector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/OracleConnector/lib/OracleDatabase.py` & `arion_library-1.1rc99.dev99/processors/OracleConnector/lib/OracleDatabase.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/OracleConnector/tests/test_oracle_connector.py` & `arion_library-1.1rc99.dev99/processors/OracleConnector/tests/test_oracle_connector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc99.dev99/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc99.dev99/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/Shopify_connector/lib/ShopifyConnector.py` & `arion_library-1.1rc99.dev99/processors/Shopify_connector/lib/ShopifyConnector.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/Shopify_connector/lib/shopifyConnect.py` & `arion_library-1.1rc99.dev99/processors/Shopify_connector/lib/shopifyConnect.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc99.dev99/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc99.dev99/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc99.dev99/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc99.dev99/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc99.dev99/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc99.dev99/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc99.dev99/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc99.dev99/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc97.dev97/setup.py` & `arion_library-1.1rc99.dev99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='arion_library',
-    version='1.1rc97.dev97',  
+    version='1.1rc99.dev99',  
     author='Heni Nechi',  
     author_email='h.nechi@arion-tech.com',  
     url='https://github.com/Ariontech/ArionLibrary.git',  
     packages=find_packages(),  
     python_requires='>=3.8',  
     install_requires=['pyodbc', 'pytest', 'pysftp==0.2.9', 'ShopifyAPI==12.5.0', 'requests==2.31.0', 'azure-core==1.29.6', 'azure-data-tables==12.5.0', 'azure-storage-blob==12.19.1', 'python-dotenv==1.0.1', 'pytest==8.1.1', 'pandas==2.0.3', 'pytest'],
 )
```

