# Comparing `tmp/pypomes_cloud-0.1.4.tar.gz` & `tmp/pypomes_cloud-0.1.5.tar.gz`

## Comparing `pypomes_cloud-0.1.4.tar` & `pypomes_cloud-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.4/src/pypomes_cloud/__init__.py
--rw-r--r--   0        0        0     9351 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.4/src/pypomes_cloud/azure_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.4/README.md
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.5/src/pypomes_cloud/__init__.py
+-rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.5/src/pypomes_cloud/azure_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.5/README.md
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 pypomes_cloud-0.1.5/PKG-INFO
```

### Comparing `pypomes_cloud-0.1.4/src/pypomes_cloud/__init__.py` & `pypomes_cloud-0.1.5/src/pypomes_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_cloud-0.1.4/src/pypomes_cloud/azure_pomes.py` & `pypomes_cloud-0.1.5/src/pypomes_cloud/azure_pomes.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,46 +2,51 @@
 import sys
 from azure.storage.blob import BlobClient, BlobServiceClient, BlobProperties
 from typing import Final
 from logging import Logger
 from pypomes_core import APP_PREFIX, env_get_str, exc_format
 
 # connection string to Azure
-AZURE_CONNECTION_STRING: Final[str] = env_get_str(f"{APP_PREFIX}_AZURE_CONNECTION_STRING")
+AZURE_CONNECTION_STRING: Final[str] = env_get_str(key=f"{APP_PREFIX}_AZURE_CONNECTION_STRING")
 
 #  storage bucket name
-AZURE_STORAGE_BUCKET: Final[str] = env_get_str(f"{APP_PREFIX}_AZURE_STORAGE_BUCKET")
+AZURE_STORAGE_BUCKET: Final[str] = env_get_str(key=f"{APP_PREFIX}_AZURE_STORAGE_BUCKET")
 
 
-def azure_verify(errors: list[str] | None, logger: Logger = None) -> bool:
+def azure_verify(errors: list[str] | None,
+                 logger: Logger = None) -> bool:
     """
     Verify whether a connection to the Azure cloud services is possible.
 
     :param errors: incidental errors
     :param logger: optional logger
     :return: True if a connection is possible, or False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     err_msg: str | None = None
     try:
-        client: BlobServiceClient = BlobServiceClient.from_connection_string(AZURE_CONNECTION_STRING)
+        client: BlobServiceClient = \
+            BlobServiceClient.from_connection_string(conn_str=AZURE_CONNECTION_STRING)
         client.close()
         result = True
     except Exception as e:
-        err_msg = __azure_except_msg(e)
+        err_msg = exc_format(exc=e,
+                             exc_info=sys.exc_info())
 
     __azure_log(errors, err_msg, logger, "Verified connection")
 
     return result
 
 
-def azure_blob_exists(errors: list[str] | None, blob_path: str,
-                      bucket_name: str = AZURE_STORAGE_BUCKET, logger: Logger = None) -> bool:
+def azure_blob_exists(errors: list[str] | None,
+                      blob_path: str,
+                      bucket_name: str = AZURE_STORAGE_BUCKET,
+                      logger: Logger = None) -> bool:
     """
     Verify whether the file referred to by *blob_path*, within *bucket_name*, exists.
 
     :param errors: incidental errors
     :param blob_path: file path within the bucket
     :param bucket_name: name of bucket (defaults to AZURE_STORAGE_BUCKET)
     :param logger: optional logger
@@ -55,23 +60,26 @@
         with BlobClient.from_connection_string(
             conn_str=AZURE_CONNECTION_STRING,
             container_name=bucket_name,
             blob_name=blob_path
         ) as client:
             result = client.exists()
     except Exception as e:
-        err_msg = __azure_except_msg(e)
+        err_msg = exc_format(exc=e,
+                             exc_info=sys.exc_info())
 
     __azure_log(errors, err_msg, logger, f"Checked if blob '{blob_path}' exists")
 
     return result
 
 
-def azure_blob_retrieve(errors: list[str] | None, blob_path: str,
-                        bucket_name: str = AZURE_STORAGE_BUCKET, logger: Logger = None) -> bytes:
+def azure_blob_retrieve(errors: list[str] | None,
+                        blob_path: str,
+                        bucket_name: str = AZURE_STORAGE_BUCKET,
+                        logger: Logger = None) -> bytes:
     """
     Obtem e retorna o conteúdo *raw* do arquivo apontado por *blob_path*, dentro de *bucket_name*.
 
     :param errors: incidental errors
     :param blob_path: file path within the bucket
     :param bucket_name: name of bucket (defaults to AZURE_STORAGE_BUCKET)
     :param logger: optional logger
@@ -88,23 +96,26 @@
             blob_name=blob_path
         ) as client:
             stream: io.BytesIO = io.BytesIO()
             client.download_blob().readinto(stream)
             stream.seek(0)
             result = stream.read()
     except Exception as e:
-        err_msg = __azure_except_msg(e)
+        err_msg = exc_format(exc=e,
+                             exc_info=sys.exc_info())
 
     __azure_log(errors, err_msg, logger, f"Retrieved blob '{blob_path}'")
 
     return result
 
 
-def azure_blob_store(errors: list[str] | None, content: bytes, blob_path: str,
-                     bucket_name: str = AZURE_STORAGE_BUCKET, logger: Logger = None) -> bool:
+def azure_blob_store(errors: list[str] | None,
+                     content: bytes, blob_path: str,
+                     bucket_name: str = AZURE_STORAGE_BUCKET,
+                     logger: Logger = None) -> bool:
     """
     Armazena o conteúdo *content* no caminho apontado por *blob_path*, dentro de *bucket_name*.
 
     :param errors: incidental errors
     :param content: conteúdo a ser armazenado
     :param blob_path: file path within the bucket
     :param bucket_name: name of bucket (defaults to AZURE_STORAGE_BUCKET)
@@ -126,23 +137,26 @@
             client.upload_blob(data=stream,
                                blob_type="BlockBlob",
                                length=len(content),
                                overwrite=True)
             result = True
     except Exception as e:
         result = False
-        err_msg = __azure_except_msg(e)
+        err_msg = exc_format(exc=e,
+                             exc_info=sys.exc_info())
 
     __azure_log(errors, err_msg, logger, f"Stored blob '{blob_path}'")
 
     return result
 
 
-def azure_blob_delete(errors: list[str] | None, blob_path: str,
-                      bucket_name: str = AZURE_STORAGE_BUCKET, logger: Logger = None) -> bool:
+def azure_blob_delete(errors: list[str] | None,
+                      blob_path: str,
+                      bucket_name: str = AZURE_STORAGE_BUCKET,
+                      logger: Logger = None) -> bool:
     """
     Remove o arquivo apontado por *blob_path*, dentro de *bucket_name*, e todos os seus *snapshots*.
 
     :param errors: incidental errors
     :param blob_path: file path within the bucket
     :param bucket_name: name of bucket (defaults to AZURE_STORAGE_BUCKET)
     :param logger: optional logger
@@ -158,23 +172,26 @@
             container_name=bucket_name,
             blob_name=blob_path
         ) as client:
             client.delete_blob(delete_snapshots="include")
             result = True
     except Exception as e:
         result = False
-        err_msg = __azure_except_msg(e)
+        err_msg = exc_format(exc=e,
+                             exc_info=sys.exc_info())
 
     __azure_log(errors, err_msg, logger, f"Deleted blob '{blob_path}'")
 
     return result
 
 
-def azure_blob_get_mimetype(errors: list[str] | None, blob_path: str,
-                            bucket_name: str = AZURE_STORAGE_BUCKET, logger: Logger = None) -> str:
+def azure_blob_get_mimetype(errors: list[str] | None,
+                            blob_path: str,
+                            bucket_name: str = AZURE_STORAGE_BUCKET,
+                            logger: Logger = None) -> str:
     """
     Return the mimetype of the file referred to by *file_path*, within  *bucket_name*.
 
     :param errors: incidental errors
     :param blob_path: file path within the bucket
     :param bucket_name: name of bucket (defaults to AZURE_STORAGE_BUCKET)
     :param logger: optional logger
@@ -189,45 +206,38 @@
             conn_str=AZURE_CONNECTION_STRING,
             container_name=bucket_name,
             blob_name=blob_path
         ) as client:
             props: BlobProperties = client.get_blob_properties()
             result = props.get("content_settings").get("content_type")
     except Exception as e:
-        err_msg = __azure_except_msg(e)
+        err_msg = exc_format(exc=e,
+                             exc_info=sys.exc_info())
 
     __azure_log(errors, err_msg, logger, f"Got mimetype for blob '{blob_path}'")
 
     return result
 
 
-def __azure_except_msg(exception: Exception) -> str:
-    """
-    Format and return the error message in the exception raised on acessing Azure.
-
-    :param exception: the raised exception
-    :return: the formatted error message
-    """
-    # TODO
-    return exc_format(exception, sys.exc_info())
-
-
-def __azure_log(errors: list[str] | None, err_msg: str, logger: Logger, debug_msg: str) -> None:
+def __azure_log(errors: list[str],
+                err_msg: str,
+                logger: Logger,
+                debug_msg: str) -> None:
     """
     Log *err_msg* and add it to *errors*, or log *debug_msg*, whatever is applicable.
 
     :param errors: incidental errors
     :param err_msg: the error message
     :param logger: optional logger
     :param debug_msg: a debug message
     """
     if err_msg:
         if logger:
             logger.error(err_msg)
-        if errors is not None:
+        if isinstance(errors, list):
             errors.append(err_msg)
     elif logger:
         logger.debug(debug_msg)
 
 
 # test Azure operations
 if __name__ == "__main__":
```

### Comparing `pypomes_cloud-0.1.4/LICENSE` & `pypomes_cloud-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_cloud-0.1.4/pyproject.toml` & `pypomes_cloud-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = [
-    "hatchling"
+    "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_cloud"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (cloud storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -20,15 +20,15 @@
 ]
 dependencies = [
     "azure-common>=1.1.28",
     "azure-core>=1.29.2",
     "azure-identity>=1.14.0",
     "azure-storage-blob>=12.17.0",
     "pip>=23.2.1",
-    "pypomes_core>=0.3.3",
+    "pypomes_core>=1.0.6",
     "setuptools>=68.0.0",
     "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Cloud"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-Cloud/issues"
```

### Comparing `pypomes_cloud-0.1.4/PKG-INFO` & `pypomes_cloud-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pypomes_cloud
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of Python pomes, pennyeach (cloud storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Cloud
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Cloud/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: azure-common>=1.1.28
 Requires-Dist: azure-core>=1.29.2
 Requires-Dist: azure-identity>=1.14.0
 Requires-Dist: azure-storage-blob>=12.17.0
 Requires-Dist: pip>=23.2.1
-Requires-Dist: pypomes-core>=0.3.3
+Requires-Dist: pypomes-core>=1.0.6
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.41.0
```

