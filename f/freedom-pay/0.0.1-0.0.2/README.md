# Comparing `tmp/freedom_pay-0.0.1-py3-none-any.whl.zip` & `tmp/freedom_pay-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4985 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 24-May-23 05:30 freedom_pay/__init__.py
--rw-rw-rw-  2.0 fat     8148 b- defN 24-May-23 06:09 freedom_pay/main.py
--rw-rw-rw-  2.0 fat     1422 b- defN 24-May-23 06:14 freedom_pay/utils.py
--rw-rw-rw-  2.0 fat     1057 b- defN 24-May-24 05:15 freedom_pay-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      603 b- defN 24-May-24 05:15 freedom_pay-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-24 05:15 freedom_pay-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-May-24 05:15 freedom_pay-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      635 b- defN 24-May-24 05:15 freedom_pay-0.0.1.dist-info/RECORD
-8 files, 11969 bytes uncompressed, 3873 bytes compressed:  67.6%
+Zip file size: 5021 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-23 05:30 freedom_package/__init__.py
+-rw-rw-rw-  2.0 fat     8148 b- defN 24-May-23 06:09 freedom_package/main.py
+-rw-rw-rw-  2.0 fat     1422 b- defN 24-May-23 06:14 freedom_package/utils.py
+-rw-rw-rw-  2.0 fat     1057 b- defN 24-May-24 05:13 freedom_pay-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      603 b- defN 24-May-24 05:13 freedom_pay-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-24 05:13 freedom_pay-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 24-May-24 05:13 freedom_pay-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      647 b- defN 24-May-24 05:13 freedom_pay-0.0.2.dist-info/RECORD
+8 files, 11985 bytes uncompressed, 3885 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: freedom_pay/__init__.py
+Filename: freedom_package/__init__.py
 Comment: 
 
-Filename: freedom_pay/main.py
+Filename: freedom_package/main.py
 Comment: 
 
-Filename: freedom_pay/utils.py
+Filename: freedom_package/utils.py
 Comment: 
 
-Filename: freedom_pay-0.0.1.dist-info/LICENSE
+Filename: freedom_pay-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: freedom_pay-0.0.1.dist-info/METADATA
+Filename: freedom_pay-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: freedom_pay-0.0.1.dist-info/WHEEL
+Filename: freedom_pay-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: freedom_pay-0.0.1.dist-info/top_level.txt
+Filename: freedom_pay-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: freedom_pay-0.0.1.dist-info/RECORD
+Filename: freedom_pay-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `freedom_pay/main.py` & `freedom_package/main.py`

 * *Files identical despite different names*

## Comparing `freedom_pay/utils.py` & `freedom_package/utils.py`

 * *Files identical despite different names*

## Comparing `freedom_pay-0.0.1.dist-info/LICENSE` & `freedom_pay-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `freedom_pay-0.0.1.dist-info/METADATA` & `freedom_pay-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freedom_pay
-Version: 0.0.1
+Version: 0.0.2
 Summary: wqewqewqewq
 Home-page: https://gitlab.com/erlan.kubanychbekov.000/freedompay_lib
 Author: erllan.000
 Author-email: erlan.kubanychbekov.000@gmail.com
 Project-URL: GitLab, https://gitlab.com/erlan.kubanychbekov.000/freedompay_lib
 Keywords: files speedfiles
 Classifier: Programming Language :: Python :: 3.11
```

