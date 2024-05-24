# Comparing `tmp/pbx_cloud_utils-1.3.0a0-py3-none-any.whl.zip` & `tmp/pbx_cloud_utils-1.4.0a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7589 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 24-May-15 07:01 cloud_utils/__init__.py
--rw-r--r--  2.0 unx    12094 b- defN 24-May-15 06:42 cloud_utils/aio_storage.py
--rw-r--r--  2.0 unx       57 b- defN 24-May-14 09:38 cloud_utils/const.py
--rw-r--r--  2.0 unx      284 b- defN 24-May-14 09:38 cloud_utils/exceptions.py
--rw-r--r--  2.0 unx    10262 b- defN 24-May-15 06:57 cloud_utils/storage.py
--rw-r--r--  2.0 unx     1365 b- defN 24-May-15 06:42 cloud_utils/types.py
--rw-r--r--  2.0 unx      346 b- defN 24-May-14 09:38 cloud_utils/utils.py
--rw-r--r--  2.0 unx      324 b- defN 24-May-15 07:01 pbx_cloud_utils-1.3.0a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-15 07:01 pbx_cloud_utils-1.3.0a0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-15 07:01 pbx_cloud_utils-1.3.0a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      887 b- defN 24-May-15 07:01 pbx_cloud_utils-1.3.0a0.dist-info/RECORD
-11 files, 25723 bytes uncompressed, 6083 bytes compressed:  76.4%
+Zip file size: 7605 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 10:54 cloud_utils/__init__.py
+-rw-r--r--  2.0 unx    12094 b- defN 24-May-23 08:46 cloud_utils/aio_storage.py
+-rw-r--r--  2.0 unx       57 b- defN 24-May-23 08:46 cloud_utils/const.py
+-rw-r--r--  2.0 unx      284 b- defN 24-May-23 08:46 cloud_utils/exceptions.py
+-rw-r--r--  2.0 unx    10378 b- defN 24-May-24 10:25 cloud_utils/storage.py
+-rw-r--r--  2.0 unx     1365 b- defN 24-May-23 08:46 cloud_utils/types.py
+-rw-r--r--  2.0 unx      346 b- defN 24-May-23 08:46 cloud_utils/utils.py
+-rw-r--r--  2.0 unx      324 b- defN 24-May-24 10:54 pbx_cloud_utils-1.4.0a0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 10:54 pbx_cloud_utils-1.4.0a0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-24 10:54 pbx_cloud_utils-1.4.0a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      887 b- defN 24-May-24 10:54 pbx_cloud_utils-1.4.0a0.dist-info/RECORD
+11 files, 25839 bytes uncompressed, 6099 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: cloud_utils/types.py
 Comment: 
 
 Filename: cloud_utils/utils.py
 Comment: 
 
-Filename: pbx_cloud_utils-1.3.0a0.dist-info/METADATA
+Filename: pbx_cloud_utils-1.4.0a0.dist-info/METADATA
 Comment: 
 
-Filename: pbx_cloud_utils-1.3.0a0.dist-info/WHEEL
+Filename: pbx_cloud_utils-1.4.0a0.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_cloud_utils-1.3.0a0.dist-info/top_level.txt
+Filename: pbx_cloud_utils-1.4.0a0.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_cloud_utils-1.3.0a0.dist-info/RECORD
+Filename: pbx_cloud_utils-1.4.0a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloud_utils/storage.py

```diff
@@ -135,14 +135,17 @@
 
     def upload(self, content: Iterable | IO, **kwargs: Any) -> None:
         client_kwargs = {"Body": content}
         if content_type := kwargs.get("content_type"):
             client_kwargs["ContentType"] = content_type
         if acl := kwargs.get("acl"):
             client_kwargs["ACL"] = acl
+        if storage_class := kwargs.get("storage_class"):
+            client_kwargs["StorageClass"] = storage_class
+
         try:
             self.client.put(**client_kwargs)
         except BotoError as e:
             raise exceptions.StorageError(e)
 
     def set_storage_class(self, storage_class: str) -> None:
         self.client.copy(
```

