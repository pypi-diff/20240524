# Comparing `tmp/cela-0.0.1-py2.py3-none-any.whl.zip` & `tmp/cela-0.0.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6716 bytes, number of entries: 11
+Zip file size: 6719 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 24-May-23 03:25 services/__init__.py
 -rw-r--r--  2.0 unx     1111 b- defN 24-May-24 07:28 services/create.py
 -rw-r--r--  2.0 unx     1574 b- defN 24-May-24 02:57 services/init.py
 -rw-r--r--  2.0 unx     7067 b- defN 24-May-24 07:27 services/migrate.py
 -rw-r--r--  2.0 unx      994 b- defN 24-May-24 07:34 services/reset.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-24 08:58 cela-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3780 b- defN 24-May-24 08:58 cela-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-May-24 08:58 cela-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       35 b- defN 24-May-24 08:58 cela-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-24 08:58 cela-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      831 b- defN 24-May-24 08:58 cela-0.0.1.dist-info/RECORD
-11 files, 15511 bytes uncompressed, 5316 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 09:03 cela-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3780 b- defN 24-May-24 09:03 cela-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-24 09:03 cela-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 24-May-24 09:03 cela-0.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-24 09:03 cela-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 24-May-24 09:03 cela-0.0.2.dist-info/RECORD
+11 files, 15516 bytes uncompressed, 5319 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: services/migrate.py
 Comment: 
 
 Filename: services/reset.py
 Comment: 
 
-Filename: cela-0.0.1.dist-info/LICENSE
+Filename: cela-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: cela-0.0.1.dist-info/METADATA
+Filename: cela-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: cela-0.0.1.dist-info/WHEEL
+Filename: cela-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: cela-0.0.1.dist-info/entry_points.txt
+Filename: cela-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cela-0.0.1.dist-info/top_level.txt
+Filename: cela-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cela-0.0.1.dist-info/RECORD
+Filename: cela-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cela-0.0.1.dist-info/METADATA` & `cela-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cela
-Version: 0.0.1
+Version: 0.0.2
 Summary: A databases migration tools for all stacks.
 Author: celaraze
 Author-email: celaraze@qq.com
 License: MIT
 Keywords: database,migration,sql
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `cela-0.0.1.dist-info/RECORD` & `cela-0.0.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 services/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 services/create.py,sha256=fG7Bf6Ssdh1ycGx5HthD1HWIU4W3lB13rC4riPIhrjU,1111
 services/init.py,sha256=g_RoqUZqJWtOP3uUv0ihdr7qTO3auhkplKk3ussTNsA,1574
 services/migrate.py,sha256=0wSaW2jPlvt3NM8QyiYG3LnwWGP6KJW7GvpS5qlUQVg,7067
 services/reset.py,sha256=pxRGBzC-T7szt7Y3i-ISVEbk85q0cBAnRNCmHz6SdOU,994
-cela-0.0.1.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cela-0.0.1.dist-info/METADATA,sha256=m9GsB8ueuDHx0r7HgtiI2pMHRyc_QiCY_DinSZaE9JE,3780
-cela-0.0.1.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
-cela-0.0.1.dist-info/entry_points.txt,sha256=YYupJGhWBtzev1gDdcKKLTWC-HfR3mCCancRPwaxUzg,35
-cela-0.0.1.dist-info/top_level.txt,sha256=Xau8qVy0H_tHbGDNnS7i0vFz4WqB9lBwZHg0pGziYuM,9
-cela-0.0.1.dist-info/RECORD,,
+cela-0.0.2.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+cela-0.0.2.dist-info/METADATA,sha256=N-WLAohMG0MdyXORVmuWPC2bKn18wO7VAXDIfdNHQ-U,3780
+cela-0.0.2.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+cela-0.0.2.dist-info/entry_points.txt,sha256=LWM7Xlzng7LSBixy3ipdGeVdU83PNH--kdSwJ-16_To,40
+cela-0.0.2.dist-info/top_level.txt,sha256=Xau8qVy0H_tHbGDNnS7i0vFz4WqB9lBwZHg0pGziYuM,9
+cela-0.0.2.dist-info/RECORD,,
```

