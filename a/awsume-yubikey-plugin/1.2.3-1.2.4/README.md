# Comparing `tmp/awsume_yubikey_plugin-1.2.3-py3-none-any.whl.zip` & `tmp/awsume_yubikey_plugin-1.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3937 bytes, number of entries: 7
--rw-r--r--  2.0 unx     4409 b- defN 23-Nov-24 16:52 yubikey.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Nov-24 16:54 awsume_yubikey_plugin-1.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      257 b- defN 23-Nov-24 16:54 awsume_yubikey_plugin-1.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Nov-24 16:54 awsume_yubikey_plugin-1.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       27 b- defN 23-Nov-24 16:54 awsume_yubikey_plugin-1.2.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Nov-24 16:54 awsume_yubikey_plugin-1.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      630 b- defN 23-Nov-24 16:54 awsume_yubikey_plugin-1.2.3.dist-info/RECORD
-7 files, 6492 bytes uncompressed, 2797 bytes compressed:  56.9%
+Zip file size: 3971 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     4485 b- defN 24-May-24 02:53 yubikey.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-24 02:56 awsume_yubikey_plugin-1.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      257 b- defN 24-May-24 02:56 awsume_yubikey_plugin-1.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 02:56 awsume_yubikey_plugin-1.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       27 b- defN 24-May-24 02:56 awsume_yubikey_plugin-1.2.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-May-24 02:56 awsume_yubikey_plugin-1.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      630 b- defN 24-May-24 02:56 awsume_yubikey_plugin-1.2.4.dist-info/RECORD
+7 files, 6568 bytes uncompressed, 2831 bytes compressed:  56.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: yubikey.py
 Comment: 
 
-Filename: awsume_yubikey_plugin-1.2.3.dist-info/LICENSE
+Filename: awsume_yubikey_plugin-1.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: awsume_yubikey_plugin-1.2.3.dist-info/METADATA
+Filename: awsume_yubikey_plugin-1.2.4.dist-info/METADATA
 Comment: 
 
-Filename: awsume_yubikey_plugin-1.2.3.dist-info/WHEEL
+Filename: awsume_yubikey_plugin-1.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: awsume_yubikey_plugin-1.2.3.dist-info/entry_points.txt
+Filename: awsume_yubikey_plugin-1.2.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: awsume_yubikey_plugin-1.2.3.dist-info/top_level.txt
+Filename: awsume_yubikey_plugin-1.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: awsume_yubikey_plugin-1.2.3.dist-info/RECORD
+Filename: awsume_yubikey_plugin-1.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yubikey.py

```diff
@@ -105,15 +105,16 @@
         if target_profile_name != None:
             role_chain = profile_lib.get_role_chain(
                 config, arguments, profiles, target_profile_name
             )
             first_profile_name = role_chain[0]
             first_profile = profiles.get(first_profile_name)
             source_credentials = profile_lib.profile_to_credentials(first_profile)
-            cache_file_name = "aws-credentials-" + source_credentials.get("AccessKeyId")
+            access_key_id = source_credentials.get("AccessKeyId")
+            cache_file_name = f"aws-credentials-{access_key_id if access_key_id else 'undefined'}"
             cache_session = cache_lib.read_aws_cache(cache_file_name)
             valid_cache_session = cache_session and cache_lib.valid_cache_session(
                 cache_session
             )
 
             mfa_serial = profile_lib.get_mfa_serial(profiles, first_profile_name)
             if (
```

## Comparing `awsume_yubikey_plugin-1.2.3.dist-info/LICENSE` & `awsume_yubikey_plugin-1.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awsume_yubikey_plugin-1.2.3.dist-info/RECORD` & `awsume_yubikey_plugin-1.2.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-yubikey.py,sha256=2FyESRBFNbAjTTh_EWq_qfeLRmY_rgNaazTpAjcr4o4,4409
-awsume_yubikey_plugin-1.2.3.dist-info/LICENSE,sha256=GXqQzXtIJsqBbf6epfoCZhoK1gWglOFukxbIE0Bdx2E,1069
-awsume_yubikey_plugin-1.2.3.dist-info/METADATA,sha256=QgqqIyr2BB6XLJw3fsb9l4IaHsl_3kdncvhbNHkrw7g,257
-awsume_yubikey_plugin-1.2.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-awsume_yubikey_plugin-1.2.3.dist-info/entry_points.txt,sha256=gXcX3GCKhaRo-F30Yv05oSYZfZUL2Vk26vyK7yyO-6A,27
-awsume_yubikey_plugin-1.2.3.dist-info/top_level.txt,sha256=MdymlNd1fKepypXJ4zlAL9CKPREb-2RG8FIHgJ1OtAE,8
-awsume_yubikey_plugin-1.2.3.dist-info/RECORD,,
+yubikey.py,sha256=xPv_F1eZdhwOfilx93sj48Lnuz9wuBOVT4_aujJGBEo,4485
+awsume_yubikey_plugin-1.2.4.dist-info/LICENSE,sha256=GXqQzXtIJsqBbf6epfoCZhoK1gWglOFukxbIE0Bdx2E,1069
+awsume_yubikey_plugin-1.2.4.dist-info/METADATA,sha256=WKCK5bdaxOHZvqV_4HiZMq-x81oHlUdUdrm0z-OdX9U,257
+awsume_yubikey_plugin-1.2.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+awsume_yubikey_plugin-1.2.4.dist-info/entry_points.txt,sha256=gXcX3GCKhaRo-F30Yv05oSYZfZUL2Vk26vyK7yyO-6A,27
+awsume_yubikey_plugin-1.2.4.dist-info/top_level.txt,sha256=MdymlNd1fKepypXJ4zlAL9CKPREb-2RG8FIHgJ1OtAE,8
+awsume_yubikey_plugin-1.2.4.dist-info/RECORD,,
```

