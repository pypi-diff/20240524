# Comparing `tmp/anyon-4.2.4-cp312-none-win_amd64.whl.zip` & `tmp/anyon-4.2.6-cp312-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 471345 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-28 05:53 anyon-4.2.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2334 b- defN 24-Apr-28 05:53 anyon-4.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-28 05:53 anyon-4.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-28 05:53 anyon-4.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      376 b- defN 24-Apr-28 05:53 anyon-4.2.4.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20992 b- defN 24-Apr-28 05:52 anyon/__init__.pyd
--rw-rw-rw-  2.0 fat    96256 b- defN 24-Apr-28 05:52 anyon/loader.pyd
--rw-rw-rw-  2.0 fat   121344 b- defN 24-Apr-28 05:52 anyon/remote.pyd
--rw-rw-rw-  2.0 fat   235008 b- defN 24-Apr-28 05:52 anyon/server.pyd
--rw-rw-rw-  2.0 fat    22016 b- defN 24-Apr-28 05:53 anyon/stage/__init__.pyd
--rw-rw-rw-  2.0 fat   251904 b- defN 24-Apr-28 05:53 anyon/stage/assembler.pyd
--rw-rw-rw-  2.0 fat   100352 b- defN 24-Apr-28 05:53 anyon/stage/calculator.pyd
--rw-rw-rw-  2.0 fat   140288 b- defN 24-Apr-28 05:53 anyon/stage/device.pyd
--rw-rw-rw-  2.0 fat    67584 b- defN 24-Apr-28 05:53 anyon/stage/processor.pyd
-14 files, 1059640 bytes uncompressed, 469585 bytes compressed:  55.7%
+Zip file size: 472431 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat     1084 b- defN 24-May-24 14:05 anyon-4.2.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2325 b- defN 24-May-24 14:05 anyon-4.2.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-24 14:05 anyon-4.2.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-May-24 14:05 anyon-4.2.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      376 b- defN 24-May-24 14:05 anyon-4.2.6.dist-info/RECORD
+-rw-rw-rw-  2.0 fat    21504 b- defN 24-May-24 14:04 anyon/__init__.pyd
+-rw-rw-rw-  2.0 fat    94208 b- defN 24-May-24 14:04 anyon/loader.pyd
+-rw-rw-rw-  2.0 fat   122368 b- defN 24-May-24 14:04 anyon/remote.pyd
+-rw-rw-rw-  2.0 fat   236032 b- defN 24-May-24 14:04 anyon/server.pyd
+-rw-rw-rw-  2.0 fat    22016 b- defN 24-May-24 14:05 anyon/stage/__init__.pyd
+-rw-rw-rw-  2.0 fat   248832 b- defN 24-May-24 14:05 anyon/stage/assembler.pyd
+-rw-rw-rw-  2.0 fat   101376 b- defN 24-May-24 14:05 anyon/stage/calculator.pyd
+-rw-rw-rw-  2.0 fat   142336 b- defN 24-May-24 14:05 anyon/stage/device.pyd
+-rw-rw-rw-  2.0 fat    68096 b- defN 24-May-24 14:05 anyon/stage/processor.pyd
+14 files, 1060654 bytes uncompressed, 470671 bytes compressed:  55.6%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: anyon-4.2.4.dist-info/LICENSE
+Filename: anyon-4.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: anyon-4.2.4.dist-info/METADATA
+Filename: anyon-4.2.6.dist-info/METADATA
 Comment: 
 
-Filename: anyon-4.2.4.dist-info/WHEEL
+Filename: anyon-4.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: anyon-4.2.4.dist-info/top_level.txt
+Filename: anyon-4.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: anyon-4.2.4.dist-info/RECORD
+Filename: anyon-4.2.6.dist-info/RECORD
 Comment: 
 
 Filename: anyon/__init__.pyd
 Comment: 
 
 Filename: anyon/loader.pyd
 Comment:
```

## Comparing `anyon-4.2.4.dist-info/LICENSE` & `anyon-4.2.6.dist-info/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## Comparing `anyon-4.2.4.dist-info/METADATA` & `anyon-4.2.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: anyon
-Version: 4.2.4
+Version: 4.2.6
 Summary: description
 Author-email: YL <fengyl@pku.edu.cn>
 License: MIT License
         
         Copyright (c) 2021 YL Feng
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
         
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: homepage, https://gitee.com
 Project-URL: documentation, https://gitee.com
 Project-URL: bugs, https://gitee.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

