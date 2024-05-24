# Comparing `tmp/yuvio-1.4.0.tar.gz` & `tmp/yuvio-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuvio-1.4.0.tar", last modified: Thu Sep 14 18:01:53 2023, max compression
+gzip compressed data, was "/home/fa94ciqu/Development/yuvio/dist/.tmp-3wn40exy/yuvio-1.4.1.tar", last modified: Fri May 24 14:05:03 2024, max compression
```

## Comparing `yuvio-1.4.0.tar` & `yuvio-1.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 labradon   (501) staff       (20)        0 2023-09-14 18:01:53.048299 yuvio-1.4.0/
--rw-r--r--   0 labradon   (501) staff       (20)     1070 2021-03-19 06:40:29.000000 yuvio-1.4.0/LICENSE
--rw-r--r--   0 labradon   (501) staff       (20)     6236 2023-09-14 18:01:53.048094 yuvio-1.4.0/PKG-INFO
--rw-r--r--   0 labradon   (501) staff       (20)     5234 2023-09-14 17:59:54.000000 yuvio-1.4.0/README.md
--rw-r--r--   0 labradon   (501) staff       (20)      104 2021-10-19 14:30:43.000000 yuvio-1.4.0/pyproject.toml
--rw-r--r--   0 labradon   (501) staff       (20)      988 2023-09-14 18:01:53.048942 yuvio-1.4.0/setup.cfg
-drwxr-xr-x   0 labradon   (501) staff       (20)        0 2023-09-14 18:01:53.034699 yuvio-1.4.0/yuvio/
--rw-r--r--   0 labradon   (501) staff       (20)      341 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/__init__.py
-drwxr-xr-x   0 labradon   (501) staff       (20)        0 2023-09-14 18:01:53.041761 yuvio-1.4.0/yuvio/core/
--rw-r--r--   0 labradon   (501) staff       (20)      170 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/core/__init__.py
--rw-r--r--   0 labradon   (501) staff       (20)     6565 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/core/colorspace.py
--rw-r--r--   0 labradon   (501) staff       (20)     2565 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/core/format.py
--rw-r--r--   0 labradon   (501) staff       (20)     6302 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/core/functions.py
--rw-r--r--   0 labradon   (501) staff       (20)     2868 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/core/reader.py
--rw-r--r--   0 labradon   (501) staff       (20)     1670 2022-05-14 13:04:43.000000 yuvio-1.4.0/yuvio/core/writer.py
--rw-r--r--   0 labradon   (501) staff       (20)     2281 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/core/yuv.py
-drwxr-xr-x   0 labradon   (501) staff       (20)        0 2023-09-14 18:01:53.047242 yuvio-1.4.0/yuvio/formats/
--rw-r--r--   0 labradon   (501) staff       (20)     1120 2023-03-07 20:53:34.000000 yuvio-1.4.0/yuvio/formats/__init__.py
--rw-r--r--   0 labradon   (501) staff       (20)     4438 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/formats/gray.py
--rw-r--r--   0 labradon   (501) staff       (20)      960 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/formats/nv12.py
--rw-r--r--   0 labradon   (501) staff       (20)     3447 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/formats/v210.py
--rw-r--r--   0 labradon   (501) staff       (20)     5523 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/formats/yuv420p.py
--rw-r--r--   0 labradon   (501) staff       (20)     5414 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/formats/yuv422p.py
--rw-r--r--   0 labradon   (501) staff       (20)     5304 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/formats/yuv444p.py
--rw-r--r--   0 labradon   (501) staff       (20)     2224 2023-09-14 17:59:54.000000 yuvio-1.4.0/yuvio/formats/yuyv422.py
-drwxr-xr-x   0 labradon   (501) staff       (20)        0 2023-09-14 18:01:53.036735 yuvio-1.4.0/yuvio.egg-info/
--rw-r--r--   0 labradon   (501) staff       (20)     6236 2023-09-14 18:01:53.000000 yuvio-1.4.0/yuvio.egg-info/PKG-INFO
--rw-r--r--   0 labradon   (501) staff       (20)      549 2023-09-14 18:01:53.000000 yuvio-1.4.0/yuvio.egg-info/SOURCES.txt
--rw-r--r--   0 labradon   (501) staff       (20)        1 2023-09-14 18:01:53.000000 yuvio-1.4.0/yuvio.egg-info/dependency_links.txt
--rw-r--r--   0 labradon   (501) staff       (20)       13 2023-09-14 18:01:53.000000 yuvio-1.4.0/yuvio.egg-info/requires.txt
--rw-r--r--   0 labradon   (501) staff       (20)        6 2023-09-14 18:01:53.000000 yuvio-1.4.0/yuvio.egg-info/top_level.txt
+drwxr-xr-x   0 fa94ciqu (68084661) domain users (68000513)        0 2024-05-24 14:05:03.289959 yuvio-1.4.1/
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     1070 2021-11-18 07:45:34.000000 yuvio-1.4.1/LICENSE
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     6236 2024-05-24 14:05:03.289959 yuvio-1.4.1/PKG-INFO
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     5234 2023-09-15 06:49:47.000000 yuvio-1.4.1/README.md
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)      104 2021-11-18 07:45:34.000000 yuvio-1.4.1/pyproject.toml
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)      988 2024-05-24 14:05:03.289959 yuvio-1.4.1/setup.cfg
+drwxr-xr-x   0 fa94ciqu (68084661) domain users (68000513)        0 2024-05-24 14:05:03.287959 yuvio-1.4.1/yuvio/
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)      341 2023-09-15 06:49:47.000000 yuvio-1.4.1/yuvio/__init__.py
+drwxr-xr-x   0 fa94ciqu (68084661) domain users (68000513)        0 2024-05-24 14:05:03.288959 yuvio-1.4.1/yuvio/core/
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)      170 2023-09-15 06:49:47.000000 yuvio-1.4.1/yuvio/core/__init__.py
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     6565 2024-05-24 14:01:42.000000 yuvio-1.4.1/yuvio/core/colorspace.py
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     2565 2023-09-15 06:49:47.000000 yuvio-1.4.1/yuvio/core/format.py
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     6302 2023-09-15 06:49:47.000000 yuvio-1.4.1/yuvio/core/functions.py
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     3010 2024-05-24 12:55:54.000000 yuvio-1.4.1/yuvio/core/reader.py
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     1812 2024-05-24 12:56:14.000000 yuvio-1.4.1/yuvio/core/writer.py
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     2281 2023-09-15 06:49:47.000000 yuvio-1.4.1/yuvio/core/yuv.py
+drwxr-xr-x   0 fa94ciqu (68084661) domain users (68000513)        0 2024-05-24 14:05:03.289959 yuvio-1.4.1/yuvio/formats/
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     1120 2022-12-09 15:17:37.000000 yuvio-1.4.1/yuvio/formats/__init__.py
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     4438 2023-09-15 06:49:47.000000 yuvio-1.4.1/yuvio/formats/gray.py
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)      960 2023-09-15 06:49:47.000000 yuvio-1.4.1/yuvio/formats/nv12.py
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     3447 2023-09-15 06:49:47.000000 yuvio-1.4.1/yuvio/formats/v210.py
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     5523 2023-09-15 06:49:47.000000 yuvio-1.4.1/yuvio/formats/yuv420p.py
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     5414 2023-09-15 06:49:47.000000 yuvio-1.4.1/yuvio/formats/yuv422p.py
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     5304 2023-09-15 06:49:47.000000 yuvio-1.4.1/yuvio/formats/yuv444p.py
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     2224 2023-09-15 06:49:47.000000 yuvio-1.4.1/yuvio/formats/yuyv422.py
+drwxr-xr-x   0 fa94ciqu (68084661) domain users (68000513)        0 2024-05-24 14:05:03.289959 yuvio-1.4.1/yuvio.egg-info/
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)     6236 2024-05-24 14:05:03.000000 yuvio-1.4.1/yuvio.egg-info/PKG-INFO
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)      549 2024-05-24 14:05:03.000000 yuvio-1.4.1/yuvio.egg-info/SOURCES.txt
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)        1 2024-05-24 14:05:03.000000 yuvio-1.4.1/yuvio.egg-info/dependency_links.txt
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)       13 2024-05-24 14:05:03.000000 yuvio-1.4.1/yuvio.egg-info/requires.txt
+-rw-r--r--   0 fa94ciqu (68084661) domain users (68000513)        6 2024-05-24 14:05:03.000000 yuvio-1.4.1/yuvio.egg-info/top_level.txt
```

### Comparing `yuvio-1.4.0/LICENSE` & `yuvio-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/PKG-INFO` & `yuvio-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuvio
-Version: 1.4.0
+Version: 1.4.1
 Summary: Read and write uncompressed yuv/ycbcr image and video files
 Home-page: https://github.com/labradon/yuvio
 Author: Andy Regensky
 Author-email: info@andyregensky.dev
 Project-URL: Bug Tracker, https://github.com/labradon/yuvio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `yuvio-1.4.0/README.md` & `yuvio-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/setup.cfg` & `yuvio-1.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = yuvio
-version = 1.4.0
+version = 1.4.1
 author = Andy Regensky
 author_email = info@andyregensky.dev
 description = Read and write uncompressed yuv/ycbcr image and video files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/labradon/yuvio
 project_urls =
```

### Comparing `yuvio-1.4.0/yuvio/core/colorspace.py` & `yuvio-1.4.1/yuvio/core/colorspace.py`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/yuvio/core/format.py` & `yuvio-1.4.1/yuvio/core/format.py`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/yuvio/core/functions.py` & `yuvio-1.4.1/yuvio/core/functions.py`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/yuvio/core/reader.py` & `yuvio-1.4.1/yuvio/core/reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,27 @@
 from . import Format
 
 
 class Reader:
 
     def __init__(self, file: Union[Path, str, io.RawIOBase, io.BufferedIOBase], format: Format):
         if isinstance(file, io.RawIOBase) or isinstance(file, io.BufferedIOBase):
+            self._close = False
             self._file = file
         else:
+            self._close = True
             self._file = open(Path(file).expanduser().resolve(), 'rb')
         self._format = format
         self._length = self._length_from_stream()
         self._iter_idx = 0
 
+    def __del__(self):
+        if self._close:
+            self._file.close()
+
     def __len__(self):
         return self._length
 
     def __iter__(self):
         for i in range(self._length):
             yield self.read(i, count=1)[0]
```

### Comparing `yuvio-1.4.0/yuvio/core/writer.py` & `yuvio-1.4.1/yuvio/core/writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,25 @@
 from . import Format
 
 
 class Writer:
 
     def __init__(self, file, format: Format):
         if isinstance(file, IOBase):
+            self._close = False
             self._file = file
         else:
+            self._close = True
             self._file = open(Path(file).expanduser().resolve(), 'wb')
         self._format = format
 
+    def __del__(self):
+        if self._close:
+            self._file.close()
+
     def write(self, yuv_frames: Union[List[YUVFrame], YUVFrame]):
         if isinstance(yuv_frames, YUVFrame):
             yuv_frames = [yuv_frames]
         frame_count = len(yuv_frames)
         if frame_count == 0:
             return
```

### Comparing `yuvio-1.4.0/yuvio/core/yuv.py` & `yuvio-1.4.1/yuvio/core/yuv.py`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/yuvio/formats/__init__.py` & `yuvio-1.4.1/yuvio/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/yuvio/formats/gray.py` & `yuvio-1.4.1/yuvio/formats/gray.py`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/yuvio/formats/nv12.py` & `yuvio-1.4.1/yuvio/formats/nv12.py`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/yuvio/formats/v210.py` & `yuvio-1.4.1/yuvio/formats/v210.py`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/yuvio/formats/yuv420p.py` & `yuvio-1.4.1/yuvio/formats/yuv420p.py`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/yuvio/formats/yuv422p.py` & `yuvio-1.4.1/yuvio/formats/yuv422p.py`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/yuvio/formats/yuv444p.py` & `yuvio-1.4.1/yuvio/formats/yuv444p.py`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/yuvio/formats/yuyv422.py` & `yuvio-1.4.1/yuvio/formats/yuyv422.py`

 * *Files identical despite different names*

### Comparing `yuvio-1.4.0/yuvio.egg-info/PKG-INFO` & `yuvio-1.4.1/yuvio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuvio
-Version: 1.4.0
+Version: 1.4.1
 Summary: Read and write uncompressed yuv/ycbcr image and video files
 Home-page: https://github.com/labradon/yuvio
 Author: Andy Regensky
 Author-email: info@andyregensky.dev
 Project-URL: Bug Tracker, https://github.com/labradon/yuvio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `yuvio-1.4.0/yuvio.egg-info/SOURCES.txt` & `yuvio-1.4.1/yuvio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

