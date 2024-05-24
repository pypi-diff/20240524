# Comparing `tmp/pyperclip_plus-0.1-py3-none-any.whl.zip` & `tmp/pyperclip_plus-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,8 @@
-Zip file size: 1223 bytes, number of entries: 4
--rw-r--r--  2.0 unx      699 b- defN 24-May-24 08:34 pyperclip_plus-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 08:34 pyperclip_plus-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-May-24 08:34 pyperclip_plus-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      316 b- defN 24-May-24 08:34 pyperclip_plus-0.1.dist-info/RECORD
-4 files, 1108 bytes uncompressed, 601 bytes compressed:  45.8%
+Zip file size: 2172 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       47 b- defN 24-May-24 09:26 pyperclip_plus/__init__.py
+-rw-r--r--  2.0 unx     1422 b- defN 24-May-24 09:23 pyperclip_plus/clipboard_manager.py
+-rw-r--r--  2.0 unx      701 b- defN 24-May-24 09:41 pyperclip_plus-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 09:41 pyperclip_plus-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-24 09:41 pyperclip_plus-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      498 b- defN 24-May-24 09:41 pyperclip_plus-0.1.1.dist-info/RECORD
+6 files, 2775 bytes uncompressed, 1260 bytes compressed:  54.6%
```

## zipnote {}

```diff
@@ -1,13 +1,19 @@
-Filename: pyperclip_plus-0.1.dist-info/METADATA
+Filename: pyperclip_plus/__init__.py
 Comment: 
 
-Filename: pyperclip_plus-0.1.dist-info/WHEEL
+Filename: pyperclip_plus/clipboard_manager.py
 Comment: 
 
-Filename: pyperclip_plus-0.1.dist-info/top_level.txt
+Filename: pyperclip_plus-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pyperclip_plus-0.1.dist-info/RECORD
+Filename: pyperclip_plus-0.1.1.dist-info/WHEEL
+Comment: 
+
+Filename: pyperclip_plus-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: pyperclip_plus-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyperclip_plus-0.1.dist-info/METADATA` & `pyperclip_plus-0.1.1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperclip-plus
-Version: 0.1
+Version: 0.1.1
 Summary: An enhanced clipboard management tool
 Home-page: https://github.com/yourusername/pyperclip_plus
 Author: Your Name
 Author-email: your.email@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

