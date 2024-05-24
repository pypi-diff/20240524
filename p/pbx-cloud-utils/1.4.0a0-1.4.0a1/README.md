# Comparing `tmp/pbx_cloud_utils-1.4.0a0-py3-none-any.whl.zip` & `tmp/pbx_cloud_utils-1.4.0a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7605 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 24-May-24 10:54 cloud_utils/__init__.py
+Zip file size: 7600 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 12:03 cloud_utils/__init__.py
 -rw-r--r--  2.0 unx    12094 b- defN 24-May-23 08:46 cloud_utils/aio_storage.py
 -rw-r--r--  2.0 unx       57 b- defN 24-May-23 08:46 cloud_utils/const.py
 -rw-r--r--  2.0 unx      284 b- defN 24-May-23 08:46 cloud_utils/exceptions.py
--rw-r--r--  2.0 unx    10378 b- defN 24-May-24 10:25 cloud_utils/storage.py
+-rw-r--r--  2.0 unx    10438 b- defN 24-May-24 12:02 cloud_utils/storage.py
 -rw-r--r--  2.0 unx     1365 b- defN 24-May-23 08:46 cloud_utils/types.py
 -rw-r--r--  2.0 unx      346 b- defN 24-May-23 08:46 cloud_utils/utils.py
--rw-r--r--  2.0 unx      324 b- defN 24-May-24 10:54 pbx_cloud_utils-1.4.0a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 10:54 pbx_cloud_utils-1.4.0a0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-24 10:54 pbx_cloud_utils-1.4.0a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      887 b- defN 24-May-24 10:54 pbx_cloud_utils-1.4.0a0.dist-info/RECORD
-11 files, 25839 bytes uncompressed, 6099 bytes compressed:  76.4%
+-rw-r--r--  2.0 unx      324 b- defN 24-May-24 12:03 pbx_cloud_utils-1.4.0a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 12:03 pbx_cloud_utils-1.4.0a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-24 12:03 pbx_cloud_utils-1.4.0a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      887 b- defN 24-May-24 12:03 pbx_cloud_utils-1.4.0a1.dist-info/RECORD
+11 files, 25899 bytes uncompressed, 6094 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: cloud_utils/types.py
 Comment: 
 
 Filename: cloud_utils/utils.py
 Comment: 
 
-Filename: pbx_cloud_utils-1.4.0a0.dist-info/METADATA
+Filename: pbx_cloud_utils-1.4.0a1.dist-info/METADATA
 Comment: 
 
-Filename: pbx_cloud_utils-1.4.0a0.dist-info/WHEEL
+Filename: pbx_cloud_utils-1.4.0a1.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_cloud_utils-1.4.0a0.dist-info/top_level.txt
+Filename: pbx_cloud_utils-1.4.0a1.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_cloud_utils-1.4.0a0.dist-info/RECORD
+Filename: pbx_cloud_utils-1.4.0a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloud_utils/storage.py

```diff
@@ -141,15 +141,15 @@
             client_kwargs["ACL"] = acl
         if storage_class := kwargs.get("storage_class"):
             client_kwargs["StorageClass"] = storage_class
 
         try:
             self.client.put(**client_kwargs)
         except BotoError as e:
-            raise exceptions.StorageError(e)
+            raise exceptions.StorageError() from e
 
     def set_storage_class(self, storage_class: str) -> None:
         self.client.copy(
             {"Bucket": self.bucket_name, "Key": self.path},
             ExtraArgs={
                 "StorageClass": self.provider_storage_class_map[storage_class],
                 "MetadataDirective": "COPY",
@@ -225,17 +225,18 @@
 
     def __init__(self, client, gcs_client: gcs_storage.Bucket) -> None:
         super().__init__(client)
         self.gcs_client = gcs_client
 
     def set_storage_class(self, storage_class: str) -> None:
         destination_storage_class = self.provider_storage_class_map[storage_class]
-
-        blob = self.gcs_client.blob(self.path)
-        blob.update_storage_class(destination_storage_class)
+        try:
+            self.client.put(StorageClass=destination_storage_class)
+        except BotoError as e:
+            raise exceptions.StorageError() from e
 
     @property
     def _provider_storage_class(self) -> str:
         blob = self.gcs_client.get_blob(self.path)
         return blob.storage_class
```

