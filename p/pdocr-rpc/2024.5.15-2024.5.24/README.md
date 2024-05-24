# Comparing `tmp/pdocr_rpc-2024.5.15.tar.gz` & `tmp/pdocr_rpc-2024.5.24.tar.gz`

## Comparing `pdocr_rpc-2024.5.15.tar` & `pdocr_rpc-2024.5.24.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/pdocr_rpc/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/pdocr_rpc/__version__.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/pdocr_rpc/conf.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/pdocr_rpc/server.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/LICENSE
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/NOTICE
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/README.md
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/pyproject.toml
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.15/PKG-INFO
+-rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/pdocr_rpc/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/pdocr_rpc/__version__.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/pdocr_rpc/conf.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/pdocr_rpc/server.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/LICENSE
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/NOTICE
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/README.md
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/pyproject.toml
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 pdocr_rpc-2024.5.24/PKG-INFO
```

### Comparing `pdocr_rpc-2024.5.15/pdocr_rpc/__init__.py` & `pdocr_rpc-2024.5.24/pdocr_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.15/pdocr_rpc/conf.py` & `pdocr_rpc-2024.5.24/pdocr_rpc/conf.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.15/pdocr_rpc/server.py` & `pdocr_rpc-2024.5.24/pdocr_rpc/server.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.15/LICENSE` & `pdocr_rpc-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.15/NOTICE` & `pdocr_rpc-2024.5.24/NOTICE`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.15/README.md` & `pdocr_rpc-2024.5.24/README.md`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-2024.5.15/pyproject.toml` & `pdocr_rpc-2024.5.24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "pdocr-rpc"
 authors = [
   { name="mikigo", email="1964191531@qq.com" },
 ]
 description = "PaddleOCR-RPC"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
```

### Comparing `pdocr_rpc-2024.5.15/PKG-INFO` & `pdocr_rpc-2024.5.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pdocr-rpc
-Version: 2024.5.15
+Version: 2024.5.24
 Summary: PaddleOCR-RPC
 Project-URL: Source, https://github.com/linuxdeepin/pdocr-rpc
 Project-URL: Documentation, https://linuxdeepin.github.io/pdocr-rpc
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
 License-File: NOTICE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Requires-Dist: funnylog
 Requires-Dist: pillow; sys_platform == 'win32'
 Requires-Dist: pyscreenshot; sys_platform == 'linux'
 Provides-Extra: doc
 Requires-Dist: mkdocs-material; extra == 'doc'
 Provides-Extra: server
 Requires-Dist: paddleocr>=2.0.1; extra == 'server'
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: pdocr-rpc Version: 2024.5.15 Summary: PaddleOCR-RPC
+Metadata-Version: 2.1 Name: pdocr-rpc Version: 2024.5.24 Summary: PaddleOCR-RPC
 Project-URL: Source, https://github.com/linuxdeepin/pdocr-rpc Project-URL:
 Documentation, https://linuxdeepin.github.io/pdocr-rpc Author-email: mikigo
 <1964191531@qq.com> License-File: LICENSE License-File: NOTICE Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
-Python: >=3.7 Requires-Dist: funnylog Requires-Dist: pillow; sys_platform ==
+Python: >=3.6 Requires-Dist: funnylog Requires-Dist: pillow; sys_platform ==
 'win32' Requires-Dist: pyscreenshot; sys_platform == 'linux' Provides-Extra:
 doc Requires-Dist: mkdocs-material; extra == 'doc' Provides-Extra: server
 Requires-Dist: paddleocr>=2.0.1; extra == 'server' Requires-Dist: paddlepaddle;
 extra == 'server' Provides-Extra: test Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown # pdocr-rpc åºäº `PaddleOCR`
 å°è£ç `RPC` æå¡ï¼åå«å®¢æ·ç«¯åæå¡ç«¯ã
 å®¢æ·ç«¯æä¾äºä¸ä¸ªç®åæç¨çå½æ°
```

