# Comparing `tmp/hashy-0.3.2-py3-none-any.whl.zip` & `tmp/hashy-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 8115 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      472 b- defN 23-Dec-29 00:18 hashy/__init__.py
--rw-rw-rw-  2.0 fat      325 b- defN 24-Jan-01 05:44 hashy/__version__.py
+Zip file size: 9568 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat      473 b- defN 24-May-24 16:59 hashy/__init__.py
+-rw-rw-rw-  2.0 fat      325 b- defN 24-May-24 17:00 hashy/__version__.py
+-rw-rw-rw-  2.0 fat     4543 b- defN 24-Jan-02 01:22 hashy/_cachy.py
 -rw-rw-rw-  2.0 fat      511 b- defN 23-Apr-09 03:01 hashy/bytes.py
 -rw-rw-rw-  2.0 fat     4543 b- defN 24-Jan-01 05:39 hashy/cachy.py
 -rw-rw-rw-  2.0 fat     4104 b- defN 23-Apr-09 03:08 hashy/dls_hash.py
 -rw-rw-rw-  2.0 fat      815 b- defN 23-Apr-09 03:01 hashy/file_hash.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-09 03:01 hashy/py.typed
 -rw-rw-rw-  2.0 fat      519 b- defN 23-Apr-09 03:01 hashy/string_hash.py
--rw-rw-rw-  2.0 fat     1088 b- defN 24-Jan-01 05:57 hashy-0.3.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1088 b- defN 24-Jan-01 05:57 hashy-0.3.2.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1453 b- defN 24-Jan-01 05:57 hashy-0.3.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Jan-01 05:57 hashy-0.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Jan-01 05:57 hashy-0.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1047 b- defN 24-Jan-01 05:57 hashy-0.3.2.dist-info/RECORD
-14 files, 16063 bytes uncompressed, 6397 bytes compressed:  60.2%
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-May-24 17:00 hashy-0.4.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-May-24 17:00 hashy-0.4.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1529 b- defN 24-May-24 17:00 hashy-0.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-24 17:00 hashy-0.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-24 17:00 hashy-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1119 b- defN 24-May-24 17:00 hashy-0.4.0.dist-info/RECORD
+15 files, 20755 bytes uncompressed, 7744 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: hashy/__init__.py
 Comment: 
 
 Filename: hashy/__version__.py
 Comment: 
 
+Filename: hashy/_cachy.py
+Comment: 
+
 Filename: hashy/bytes.py
 Comment: 
 
 Filename: hashy/cachy.py
 Comment: 
 
 Filename: hashy/dls_hash.py
@@ -18,26 +21,26 @@
 
 Filename: hashy/py.typed
 Comment: 
 
 Filename: hashy/string_hash.py
 Comment: 
 
-Filename: hashy-0.3.2.dist-info/LICENSE
+Filename: hashy-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: hashy-0.3.2.dist-info/LICENSE.txt
+Filename: hashy-0.4.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: hashy-0.3.2.dist-info/METADATA
+Filename: hashy-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: hashy-0.3.2.dist-info/WHEEL
+Filename: hashy-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: hashy-0.3.2.dist-info/top_level.txt
+Filename: hashy-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: hashy-0.3.2.dist-info/RECORD
+Filename: hashy-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hashy/__init__.py

```diff
@@ -1,6 +1,6 @@
 from .__version__ import __application_name__, __author__, __version__
 from .file_hash import get_file_md5, get_file_sha256, get_file_sha512
 from .string_hash import get_string_md5, get_string_sha256, get_string_sha512
 from .dls_hash import dls_sort, get_dls_md5, get_dls_sha256, get_dls_sha512, convert_serializable_special_cases, json_dumps
 from .bytes import get_bytes_md5, get_bytes_sha512, get_bytes_sha256
-from .cachy import cachy, CacheCounters, get_counters
+from ._cachy import cachy, CacheCounters, get_counters
```

## hashy/__version__.py

```diff
@@ -1,8 +1,8 @@
 __application_name__ = "hashy"
 __title__ = __application_name__
 __author__ = "abel"
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 __author_email__ = "j@abel.co"
 __url__ = "https://github.com/jamesabel/hashy"
 __download_url__ = "https://github.com/jamesabel/hashy"
 __description__ = "simple hash library for string, file, dict, set and list"
```

## Comparing `hashy-0.3.2.dist-info/LICENSE` & `hashy-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hashy-0.3.2.dist-info/LICENSE.txt` & `hashy-0.4.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `hashy-0.3.2.dist-info/METADATA` & `hashy-0.4.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashy
-Version: 0.3.2
+Version: 0.4.0
 Summary: simple hash library for string, file, dict, set and list
 Home-page: https://github.com/jamesabel/hashy
 Download-URL: https://github.com/jamesabel/hashy
 Author: abel
 Author-email: j@abel.co
 License: MIT License
 Keywords: hash
@@ -36,15 +36,18 @@
 - Doesn't require arguments be frozen and/or pickle-able. Uses hashy to create a hash of the arguments.
 
 
 # Example
 
 ```
 
-from hashy import get_string_sha256
+from hashy import get_string_sha256, cachy
 
-print(get_string_sha256("a"))
+print(get_string_sha256("a"))  # prints ca978112ca1bbdcafac231b39a23dc4da786eff8147c4e72b9807785afee48bb
 
-# prints
-# ca978112ca1bbdcafac231b39a23dc4da786eff8147c4e72b9807785afee48bb
+@cachy()
+def func(a):
+    return a + a
+
+print(func(2))  # prints 4
 
 ```
```

## Comparing `hashy-0.3.2.dist-info/RECORD` & `hashy-0.4.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-hashy/__init__.py,sha256=QLP19wOEFyCwa9IQUdVReg6daYOVmnWVGSTebSWHwI4,472
-hashy/__version__.py,sha256=Yu0vv710uTE2So7HLFeJy0alg4_VFJM9KsnKRmHRx2w,325
+hashy/__init__.py,sha256=zciQ2skrxx8bPYRcSvXuRMtsfj1LH4chu4z_i-fvaW8,473
+hashy/__version__.py,sha256=LXwYCKVzkDbsx_NHSZ_EIu9-10NAUmZ9aGhglJe79kU,325
+hashy/_cachy.py,sha256=wcLO2C6Ft16Aaj7gOAvpy-BctTLYXmVvPWB2Amawar8,4543
 hashy/bytes.py,sha256=se7gVG9_ry5_q_QbxwjnJeyMP0mefxz9zhPQ8R50Ips,511
 hashy/cachy.py,sha256=wcLO2C6Ft16Aaj7gOAvpy-BctTLYXmVvPWB2Amawar8,4543
 hashy/dls_hash.py,sha256=l6s6VoMbY1iZxZ9iye2xty3AFDCW0gn4BsNK9Y_2z4c,4104
 hashy/file_hash.py,sha256=1TU3h_DG08X01rf65MUj36-aLIPaT5UgAWnNQEDmfvk,815
 hashy/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hashy/string_hash.py,sha256=lGq3Tx-_IpNTfQby0wg6QpJA6-WfLZGiqQQJKbfl3jk,519
-hashy-0.3.2.dist-info/LICENSE,sha256=wJpPh6rC_YhbTZ7ZIy1VjrqeLdJ8Pz0ppx2MUi7s8Dg,1088
-hashy-0.3.2.dist-info/LICENSE.txt,sha256=wJpPh6rC_YhbTZ7ZIy1VjrqeLdJ8Pz0ppx2MUi7s8Dg,1088
-hashy-0.3.2.dist-info/METADATA,sha256=-QykBDbtnA-J_ESPJTUXixTRrCnr5FKQafdpOHvk2CA,1453
-hashy-0.3.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-hashy-0.3.2.dist-info/top_level.txt,sha256=zBSfOfOk3tDVMuVpW9PM9DGWbIx0zV8BsNP-gb87swE,6
-hashy-0.3.2.dist-info/RECORD,,
+hashy-0.4.0.dist-info/LICENSE,sha256=wJpPh6rC_YhbTZ7ZIy1VjrqeLdJ8Pz0ppx2MUi7s8Dg,1088
+hashy-0.4.0.dist-info/LICENSE.txt,sha256=wJpPh6rC_YhbTZ7ZIy1VjrqeLdJ8Pz0ppx2MUi7s8Dg,1088
+hashy-0.4.0.dist-info/METADATA,sha256=1J373DyJ1SHfQ458u5kHukZkY_popg9U5z42JEsnBbo,1529
+hashy-0.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hashy-0.4.0.dist-info/top_level.txt,sha256=zBSfOfOk3tDVMuVpW9PM9DGWbIx0zV8BsNP-gb87swE,6
+hashy-0.4.0.dist-info/RECORD,,
```

