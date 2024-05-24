# Comparing `tmp/gs_engine-0.28.0a20240522-py2.py3-none-any.whl.zip` & `tmp/gs_engine-0.28.0a20240523-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12698 bytes, number of entries: 9
--rw-r--r--  2.0 unx      398 b- defN 24-May-22 19:02 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      593 b- defN 24-May-22 19:02 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx     1573 b- defN 24-May-22 19:02 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      204 b- defN 24-May-22 19:02 graphscope.runtime/conf/log4rs.yml
--rw-r--r--  2.0 unx      694 b- defN 24-May-22 19:02 graphscope_runtime/__init__.py
--rw-r--r--  2.0 unx    23359 b- defN 24-May-22 20:00 gs_engine-0.28.0a20240522.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-May-22 20:00 gs_engine-0.28.0a20240522.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-May-22 20:00 gs_engine-0.28.0a20240522.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      831 b- defN 24-May-22 20:00 gs_engine-0.28.0a20240522.dist-info/RECORD
-9 files, 27781 bytes uncompressed, 11236 bytes compressed:  59.6%
+Zip file size: 12699 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      398 b- defN 24-May-23 19:01 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      593 b- defN 24-May-23 19:01 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx     1573 b- defN 24-May-23 19:01 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      204 b- defN 24-May-23 19:01 graphscope.runtime/conf/log4rs.yml
+-rw-r--r--  2.0 unx      694 b- defN 24-May-23 19:01 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx    23359 b- defN 24-May-23 20:01 gs_engine-0.28.0a20240523.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-23 20:01 gs_engine-0.28.0a20240523.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-23 20:01 gs_engine-0.28.0a20240523.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 24-May-23 20:01 gs_engine-0.28.0a20240523.dist-info/RECORD
+9 files, 27781 bytes uncompressed, 11237 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
 Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: gs_engine-0.28.0a20240522.dist-info/METADATA
+Filename: gs_engine-0.28.0a20240523.dist-info/METADATA
 Comment: 
 
-Filename: gs_engine-0.28.0a20240522.dist-info/WHEEL
+Filename: gs_engine-0.28.0a20240523.dist-info/WHEEL
 Comment: 
 
-Filename: gs_engine-0.28.0a20240522.dist-info/top_level.txt
+Filename: gs_engine-0.28.0a20240523.dist-info/top_level.txt
 Comment: 
 
-Filename: gs_engine-0.28.0a20240522.dist-info/RECORD
+Filename: gs_engine-0.28.0a20240523.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gs_engine-0.28.0a20240522.dist-info/METADATA` & `gs_engine-0.28.0a20240523.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.28.0a20240522
+Version: 0.28.0a20240523
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `gs_engine-0.28.0a20240522.dist-info/RECORD` & `gs_engine-0.28.0a20240523.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
 graphscope.runtime/conf/frontend.vineyard.properties,sha256=A99pIMZorNr0hWMbPF2cX58Y1_LhfCICzgQlMcL1Xg0,593
 graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
 graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
 graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
-gs_engine-0.28.0a20240522.dist-info/METADATA,sha256=h-Rqe_E5Vf_E-bAewYHtKTQmaRxAi9y-N2bfHTYCXBc,23359
-gs_engine-0.28.0a20240522.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
-gs_engine-0.28.0a20240522.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
-gs_engine-0.28.0a20240522.dist-info/RECORD,,
+gs_engine-0.28.0a20240523.dist-info/METADATA,sha256=Kh_UtYVSNHMQmdBFFMx8q81CJP_AreKBbjZGZKMmc-4,23359
+gs_engine-0.28.0a20240523.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+gs_engine-0.28.0a20240523.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
+gs_engine-0.28.0a20240523.dist-info/RECORD,,
```

