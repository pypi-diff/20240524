# Comparing `tmp/chloris_app_sdk-1.0.8.tar.gz` & `tmp/chloris_app_sdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chloris_app_sdk-1.0.8.tar", last modified: Wed Apr  3 14:47:54 2024, max compression
+gzip compressed data, was "chloris_app_sdk-1.0.9.tar", last modified: Fri Apr 12 18:12:15 2024, max compression
```

## Comparing `chloris_app_sdk-1.0.8.tar` & `chloris_app_sdk-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-04-03 14:47:54.082259 chloris_app_sdk-1.0.8/
--rw-r--r--   0 jay       (1000) jay       (1000)     1079 2024-01-30 16:22:16.000000 chloris_app_sdk-1.0.8/LICENSE
--rw-r--r--   0 jay       (1000) jay       (1000)     2816 2024-04-03 14:47:54.082259 chloris_app_sdk-1.0.8/PKG-INFO
--rw-r--r--   0 jay       (1000) jay       (1000)     2493 2024-01-30 21:42:42.000000 chloris_app_sdk-1.0.8/README.md
--rw-r--r--   0 jay       (1000) jay       (1000)      100 2024-01-29 15:28:34.000000 chloris_app_sdk-1.0.8/pyproject.toml
--rw-r--r--   0 jay       (1000) jay       (1000)      506 2024-04-03 14:47:54.082259 chloris_app_sdk-1.0.8/setup.cfg
--rw-r--r--   0 jay       (1000) jay       (1000)       39 2024-01-29 15:27:09.000000 chloris_app_sdk-1.0.8/setup.py
-drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-04-03 14:47:54.072259 chloris_app_sdk-1.0.8/src/
-drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-04-03 14:47:54.072259 chloris_app_sdk-1.0.8/src/chloris_app_sdk/
--rw-r--r--   0 jay       (1000) jay       (1000)       37 2024-01-30 15:35:13.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk/__init__.py
--rw-r--r--   0 jay       (1000) jay       (1000)    34876 2024-04-02 18:50:16.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk/client.py
--rw-r--r--   0 jay       (1000) jay       (1000)     2111 2024-01-30 15:37:10.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk/utils.py
-drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-04-03 14:47:54.082259 chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/
--rw-r--r--   0 jay       (1000) jay       (1000)     2816 2024-04-03 14:47:54.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/PKG-INFO
--rw-r--r--   0 jay       (1000) jay       (1000)      356 2024-04-03 14:47:54.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 jay       (1000) jay       (1000)        1 2024-04-03 14:47:54.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 jay       (1000) jay       (1000)       14 2024-04-03 14:47:54.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/requires.txt
--rw-r--r--   0 jay       (1000) jay       (1000)       16 2024-04-03 14:47:54.000000 chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-04-12 18:12:15.057739 chloris_app_sdk-1.0.9/
+-rw-r--r--   0 jay       (1000) jay       (1000)     1079 2024-01-30 16:22:16.000000 chloris_app_sdk-1.0.9/LICENSE
+-rw-r--r--   0 jay       (1000) jay       (1000)     2816 2024-04-12 18:12:15.057739 chloris_app_sdk-1.0.9/PKG-INFO
+-rw-r--r--   0 jay       (1000) jay       (1000)     2493 2024-01-30 21:42:42.000000 chloris_app_sdk-1.0.9/README.md
+-rw-r--r--   0 jay       (1000) jay       (1000)      100 2024-01-29 15:28:34.000000 chloris_app_sdk-1.0.9/pyproject.toml
+-rw-r--r--   0 jay       (1000) jay       (1000)      506 2024-04-12 18:12:15.057739 chloris_app_sdk-1.0.9/setup.cfg
+-rw-r--r--   0 jay       (1000) jay       (1000)       39 2024-01-29 15:27:09.000000 chloris_app_sdk-1.0.9/setup.py
+drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-04-12 18:12:15.057739 chloris_app_sdk-1.0.9/src/
+drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-04-12 18:12:15.057739 chloris_app_sdk-1.0.9/src/chloris_app_sdk/
+-rw-r--r--   0 jay       (1000) jay       (1000)       37 2024-01-30 15:35:13.000000 chloris_app_sdk-1.0.9/src/chloris_app_sdk/__init__.py
+-rw-r--r--   0 jay       (1000) jay       (1000)    35323 2024-04-12 18:06:45.000000 chloris_app_sdk-1.0.9/src/chloris_app_sdk/client.py
+-rw-r--r--   0 jay       (1000) jay       (1000)     2111 2024-01-30 15:37:10.000000 chloris_app_sdk-1.0.9/src/chloris_app_sdk/utils.py
+drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2024-04-12 18:12:15.057739 chloris_app_sdk-1.0.9/src/chloris_app_sdk.egg-info/
+-rw-r--r--   0 jay       (1000) jay       (1000)     2816 2024-04-12 18:12:15.000000 chloris_app_sdk-1.0.9/src/chloris_app_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 jay       (1000) jay       (1000)      356 2024-04-12 18:12:15.000000 chloris_app_sdk-1.0.9/src/chloris_app_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jay       (1000) jay       (1000)        1 2024-04-12 18:12:15.000000 chloris_app_sdk-1.0.9/src/chloris_app_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jay       (1000) jay       (1000)       14 2024-04-12 18:12:15.000000 chloris_app_sdk-1.0.9/src/chloris_app_sdk.egg-info/requires.txt
+-rw-r--r--   0 jay       (1000) jay       (1000)       16 2024-04-12 18:12:15.000000 chloris_app_sdk-1.0.9/src/chloris_app_sdk.egg-info/top_level.txt
```

### Comparing `chloris_app_sdk-1.0.8/LICENSE` & `chloris_app_sdk-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chloris_app_sdk-1.0.8/PKG-INFO` & `chloris_app_sdk-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chloris_app_sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package created with a setuptools tutorial.  See article link for more details.
 Home-page: https://app.chloris.earth/docs/index.html
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: urllib3
```

### Comparing `chloris_app_sdk-1.0.8/README.md` & `chloris_app_sdk-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `chloris_app_sdk-1.0.8/src/chloris_app_sdk/client.py` & `chloris_app_sdk-1.0.9/src/chloris_app_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,22 +146,32 @@
 
         Returns: The boto3 cognito idp client.
         """
         if self._cognito_idp_client is None:
             self._cognito_idp_client = boto3.client("cognito-idp", config=Config(region_name=self._aws_resources["awsRegion"]))
         return self._cognito_idp_client
 
-    def _get_s3_client(self ) -> Any:
+    def _get_s3_client(self) -> Any:
         """
         Get the boto3 s3 client, creating it if needed.
 
         Returns: The boto3 s3 client.
         """
+        # check if the credentials are expired
+        if self._sts_credentials_expired():
+            self._s3_client = None
+        # get new client if needed
         if self._s3_client is None:
-            self._s3_client = boto3.client("s3", config=Config(region_name=self._aws_resources["awsRegion"]))
+            credentials = self._get_sts_temporary_credentials()
+            self._s3_client = boto3.client(
+                "s3",
+                aws_access_key_id=credentials["AccessKeyId"],
+                aws_secret_access_key=credentials["SecretKey"],
+                aws_session_token=credentials["SessionToken"],
+                config=Config(region_name=self._aws_resources["awsRegion"], ))
         return self._s3_client
 
     def _get_s3_bucket_resource(self) -> Any:
         """
         Get the boto3 s3 bucket resource, creating it if needed.
 
         Returns: The boto3 s3 bucket resource.
@@ -306,15 +316,14 @@
         # Poll S3 with exponential backoff up to 15 minutes for the boundary to be normalized
         boundary_path = self._wait_for_boundary_normalization(upload_id)
         if boundary_path is None:
             raise ValueError("Could not process your file in the time allowed, please simplify your boundary and try again.")
         return boundary_path
 
 
-
     def _upload_boundary_file(self, file: Union[str, os.PathLike], exclude_geometry_path: str = None) -> str:
         """
         Upload a geospatial boundary to the Chloris S3 bucket, and wait for it to be normalized.
 
           Compared to `_upload_boundary_remote_geojson()`, this function is more flexible in the types of files
           it can upload, but more applies stricter sparseness and complexity limits.
 
@@ -340,15 +349,15 @@
         #    This is important because the normalization process may have changed the boundary in unexpected ways,
         #    as it attempts fix some common polygon issues and reading from certain
         #    formats (such as KML) can produce visual artifacts.
 
         if not isinstance(file, str):
             file = str(file)
         if file.endswith(".shp"):
-            files =[]
+            files = []
             # if the file is a shapefile, upload all the files in the shapefile
             for shp_ext in [".dbf", ".prj", ".shx"]:
                 if os.path.exists(file.replace(".shp", shp_ext)):
                     files.append(file.replace(".shp", shp_ext))
             files.append(file)
         else:
             files = [file]
@@ -438,15 +447,14 @@
         """
         # clone the reporting unit entry
         reporting_unit_entry = dict(reporting_unit_entry)
         # remove the downloads/stats/layersConfig fields since the API doesn't accept them
         reporting_unit_entry.pop("downloads", None)
         reporting_unit_entry.pop("stats", None)
         reporting_unit_entry.pop("layersConfig", None)
-
         response = self._http_pool.request(
             "PUT",
             self.api_endpoint + f"reportingUnit",
             headers={
                 "Content-Type": "application/json",
                 "Authorization": "Bearer " + self._get_id_token(),
             },
```

### Comparing `chloris_app_sdk-1.0.8/src/chloris_app_sdk/utils.py` & `chloris_app_sdk-1.0.9/src/chloris_app_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `chloris_app_sdk-1.0.8/src/chloris_app_sdk.egg-info/PKG-INFO` & `chloris_app_sdk-1.0.9/src/chloris_app_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chloris_app_sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package created with a setuptools tutorial.  See article link for more details.
 Home-page: https://app.chloris.earth/docs/index.html
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: urllib3
```

