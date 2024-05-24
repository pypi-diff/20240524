# Comparing `tmp/sssekai-0.1.0.tar.gz` & `tmp/sssekai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sssekai-0.1.0.tar", last modified: Mon May  6 15:53:39 2024, max compression
+gzip compressed data, was "sssekai-0.1.1.tar", last modified: Fri May 24 12:52:02 2024, max compression
```

## Comparing `sssekai-0.1.0.tar` & `sssekai-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-06 15:53:39.116844 sssekai-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-06 15:53:34.000000 sssekai-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:53:39.116844 sssekai-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-06 15:53:34.000000 sssekai-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.112844 sssekai-0.1.0/sssekai/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.112844 sssekai-0.1.0/sssekai/abcache/
--rw-r--r--   0 runner    (1001) docker     (127)    13897 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/abcache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/sssekai/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/crypto/APIManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/crypto/AssetBundle.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/sssekai/entrypoint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/abcache.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/abdecrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/apidecrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/live2dextract.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/mitm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/mvdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/spineextract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/entrypoint/usmdemux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/sssekai/fmt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/fmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/fmt/moc3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/sssekai/unity/
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/unity/AnimationClip.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/unity/AssetBundle.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/unity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/sssekai/unity/constant/
--rw-r--r--   0 runner    (1001) docker     (127)    60945 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/unity/constant/SekaiLive2DPathNames.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:34.000000 sssekai-0.1.0/sssekai/unity/constant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:53:39.116844 sssekai-0.1.0/sssekai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-06 15:53:39.000000 sssekai-0.1.0/sssekai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-06 15:53:39.000000 sssekai-0.1.0/sssekai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:53:39.000000 sssekai-0.1.0/sssekai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 15:53:39.000000 sssekai-0.1.0/sssekai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:53:39.000000 sssekai-0.1.0/sssekai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 15:53:39.000000 sssekai-0.1.0/sssekai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.722165 sssekai-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-24 12:52:02.722165 sssekai-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-24 12:51:54.000000 sssekai-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:52:02.722165 sssekai-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-24 12:51:54.000000 sssekai-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.714165 sssekai-0.1.1/sssekai/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.718165 sssekai-0.1.1/sssekai/abcache/
+-rw-r--r--   0 runner    (1001) docker     (127)    16291 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/abcache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.718165 sssekai-0.1.1/sssekai/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/crypto/APIManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/crypto/AssetBundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.718165 sssekai-0.1.1/sssekai/entrypoint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/abcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/abdecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/apidecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/live2dextract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/mitm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/mvdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/spineextract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/entrypoint/usmdemux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.718165 sssekai-0.1.1/sssekai/fmt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/fmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/fmt/moc3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.718165 sssekai-0.1.1/sssekai/unity/
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/unity/AnimationClip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/unity/AssetBundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/unity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.722165 sssekai-0.1.1/sssekai/unity/constant/
+-rw-r--r--   0 runner    (1001) docker     (127)    60945 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/unity/constant/SekaiLive2DPathNames.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:51:54.000000 sssekai-0.1.1/sssekai/unity/constant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:52:02.722165 sssekai-0.1.1/sssekai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-24 12:52:02.000000 sssekai-0.1.1/sssekai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-24 12:52:02.000000 sssekai-0.1.1/sssekai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:52:02.000000 sssekai-0.1.1/sssekai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 12:52:02.000000 sssekai-0.1.1/sssekai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:52:02.000000 sssekai-0.1.1/sssekai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 12:52:02.000000 sssekai-0.1.1/sssekai.egg-info/top_level.txt
```

### Comparing `sssekai-0.1.0/PKG-INFO` & `sssekai-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sssekai
-Version: 0.1.0
+Version: 0.1.1
 Summary: Project SEKAI Asset Utility / PJSK 资源下载 + Live2D, Spine, USM 提取
 Home-page: https://github.com/mos9527/sssekai
 Author: greats3an
 Author-email: greats3an@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -62,26 +62,38 @@
 ### Examples
 - Caches the game data into `D:\Sekai`
   ```powershell
   sssekai abcache --cache-dir D:\Sekai
   ```
 - Download game data for a *very specific* version into `D:\Sekai`
   ```powershell
-  sssekai abcache --cache-dir D:\Sekai --platform android --version "3.5.0" --appHash "5e9fea31-2613-bd13-1723-9fe15156bd66" --assetHash "9a5e2be1-0502-24c6-389e-b79b6a24ec0b" --assetHostHash "cf2d2388"
+  sssekai abcache --cache-dir D:\Sekai --platform android --version "3.5.0" --appHash "5e9fea31-2613-bd13-1723-9fe15156bd66"
   ```
-  The fields, `platform`, `appHash`, `assetHash`, `assetHostHash` are **all** necessary to facilitate the download.
 
-  The table below contains the values you might need for that purpose.
-
-  *FYI the game used to actually send these values with before 3.5.0! Now they don't :(*
 ### Known Game Versions And Their Respective Hashes
 *NOTE: This table will probably remain not up-to-date and/or incomplete. PRs are welcome for additions.*
-|platform|version|appHash|assetHash|assetHostHash|
-|-|-|-|-|-|
-|android|3.5.0|5e9fea31-2613-bd13-1723-9fe15156bd66|9a5e2be1-0502-24c6-389e-b79b6a24ec0b|cf2d2388|
+
+|platform|version|appHash|
+|-|-|-|
+|android|3.6.0|7558547e-4753-6ebd-03ff-168494c32769|
+|ios|3.6.0|7558547e-4753-6ebd-03ff-168494c32769|
+|android|3.5.0|5e9fea31-2613-bd13-1723-9fe15156bd66|
+|ios|3.5.0|5e9fea31-2613-bd13-1723-9fe15156bd66|
+#### Bonus: How to extract appHash from Android releases
+- Acquire the game's APK file.
+- Run [dump_android_pjsk_appHash.py](https://github.com/mos9527/sssekai/blob/main/sssekai/scripts/dump_android_pjsk_appHash.py) on it. For example:
+```bash
+python dump_android_pjsk_appHash.py pjsk_360.apk
+```
+- Which prints
+```
+7558547e-4753-6ebd-03ff-168494c32769 production_android
+7558547e-4753-6ebd-03ff-168494c32769 production_android
+7558547e-4753-6ebd-03ff-168494c32769 production_ios
+```
 
 ## What Do These Files Do? (WIP)
 There's a *ton* of them. Like ~45GB with version 3.5.0.(!) I'll try to document my limited findings here whenever possible 
 ### Spine2D Related Files
 NOTE: You'll need Spine2D SDK 4.x to load these.
 |Path|Purpose (Assumed)|
 |-|-|
```

### Comparing `sssekai-0.1.0/README.md` & `sssekai-0.1.1/sssekai.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: sssekai
+Version: 0.1.1
+Summary: Project SEKAI Asset Utility / PJSK 资源下载 + Live2D, Spine, USM 提取
+Home-page: https://github.com/mos9527/sssekai
+Author: greats3an
+Author-email: greats3an@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: msgpack
+Requires-Dist: pycryptodome
+Requires-Dist: unitypy
+Requires-Dist: wannacri
+
 # sssekai
 Command-line tool (w/Python API support) for downloading/deobfuscating the game's assets, along with some other tools.
 
     usage: sssekai [-h]
                   {apidecrypt,abdecrypt,usmdemux,abcache,live2dextract,mitm} ...
 
     SSSekai Proejct SEKAI feat. Hatsune Miku (Android) Modding Tools
@@ -45,26 +62,38 @@
 ### Examples
 - Caches the game data into `D:\Sekai`
   ```powershell
   sssekai abcache --cache-dir D:\Sekai
   ```
 - Download game data for a *very specific* version into `D:\Sekai`
   ```powershell
-  sssekai abcache --cache-dir D:\Sekai --platform android --version "3.5.0" --appHash "5e9fea31-2613-bd13-1723-9fe15156bd66" --assetHash "9a5e2be1-0502-24c6-389e-b79b6a24ec0b" --assetHostHash "cf2d2388"
+  sssekai abcache --cache-dir D:\Sekai --platform android --version "3.5.0" --appHash "5e9fea31-2613-bd13-1723-9fe15156bd66"
   ```
-  The fields, `platform`, `appHash`, `assetHash`, `assetHostHash` are **all** necessary to facilitate the download.
-
-  The table below contains the values you might need for that purpose.
 
-  *FYI the game used to actually send these values with before 3.5.0! Now they don't :(*
 ### Known Game Versions And Their Respective Hashes
 *NOTE: This table will probably remain not up-to-date and/or incomplete. PRs are welcome for additions.*
-|platform|version|appHash|assetHash|assetHostHash|
-|-|-|-|-|-|
-|android|3.5.0|5e9fea31-2613-bd13-1723-9fe15156bd66|9a5e2be1-0502-24c6-389e-b79b6a24ec0b|cf2d2388|
+
+|platform|version|appHash|
+|-|-|-|
+|android|3.6.0|7558547e-4753-6ebd-03ff-168494c32769|
+|ios|3.6.0|7558547e-4753-6ebd-03ff-168494c32769|
+|android|3.5.0|5e9fea31-2613-bd13-1723-9fe15156bd66|
+|ios|3.5.0|5e9fea31-2613-bd13-1723-9fe15156bd66|
+#### Bonus: How to extract appHash from Android releases
+- Acquire the game's APK file.
+- Run [dump_android_pjsk_appHash.py](https://github.com/mos9527/sssekai/blob/main/sssekai/scripts/dump_android_pjsk_appHash.py) on it. For example:
+```bash
+python dump_android_pjsk_appHash.py pjsk_360.apk
+```
+- Which prints
+```
+7558547e-4753-6ebd-03ff-168494c32769 production_android
+7558547e-4753-6ebd-03ff-168494c32769 production_android
+7558547e-4753-6ebd-03ff-168494c32769 production_ios
+```
 
 ## What Do These Files Do? (WIP)
 There's a *ton* of them. Like ~45GB with version 3.5.0.(!) I'll try to document my limited findings here whenever possible 
 ### Spine2D Related Files
 NOTE: You'll need Spine2D SDK 4.x to load these.
 |Path|Purpose (Assumed)|
 |-|-|
@@ -106,8 +135,8 @@
 |live_pv/model/music_item|*PV Props. There aren't lots of those.|
 And strangly enough there's another folder *outside* live_pv that also contains 3D assets. I'll put it here.
 |Path|Purpose (Assumed)|
 |-|-|
 |model3d/model/stage_object|*PV Props, again. Those this time it's all instruments and it has the same aforementioned weighting issues.|
 
 # See Also
-https://github.com/mos9527/sssekai_blender_io
+https://github.com/mos9527/sssekai_blender_io
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sssekai-0.1.0/setup.py` & `sssekai-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.0/sssekai/__main__.py` & `sssekai-0.1.1/sssekai/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sssekai.entrypoint.mitm import main_mitm
 from sssekai.entrypoint.mvdata import main_mvdata
 from sssekai.entrypoint.usmdemux import main_usmdemux
 from sssekai.entrypoint.abcache import main_abcache
 from sssekai.entrypoint.live2dextract import main_live2dextract
 from sssekai.entrypoint.spineextract import main_spineextract
 from sssekai.unity import SEKAI_UNITY_VERSION
-from sssekai.abcache import DEFAULT_CACHE_DIR, DEFAULT_SEKAI_APP_PLATFORM, DEFAULT_SEKAI_APP_VERSION, DEFAULT_SEKAI_APP_HASH, DEFAULT_SEKAI_AB_HASH, DEFAULT_SEKAI_AB_HOST_HASH
+from sssekai.abcache import DEFAULT_CACHE_DIR, DEFAULT_SEKAI_APP_PLATFORM, DEFAULT_SEKAI_APP_VERSION, DEFAULT_SEKAI_APP_HASH
 def __main__():
     from tqdm.std import tqdm as tqdm_c
     class SemaphoreStdout:
         @staticmethod
         def write(__s):
             # Blocks tqdm's output until write on this stream is done
             # Solves cases where progress bars gets re-rendered when logs
@@ -54,16 +54,14 @@
 NOTE: The AssetBundles *cached* are NOT OBFUSCATED. They can be used as is by various Unity ripping tools (and sssekai by extension)
       that supports stripped Unity version (should be %s. the version is ripped).''' % SEKAI_UNITY_VERSION)
     abcache_parser.add_argument('--cache-dir', type=str, help='cache directory (default: %(default)s)',default=DEFAULT_CACHE_DIR)
     abcache_parser.add_argument('--skip-update',action='store_true',help='skip all updates and use cached assets as is.')
     abcache_parser.add_argument('--version', type=str, help='PJSK app version (default: %(default)s)', default=DEFAULT_SEKAI_APP_VERSION)
     abcache_parser.add_argument('--platform', type=str, help='PJSK app platform (default: %(default)s)', default=DEFAULT_SEKAI_APP_PLATFORM)
     abcache_parser.add_argument('--appHash', type=str, help='PJSK app hash (default: %(default)s)', default=DEFAULT_SEKAI_APP_HASH)
-    abcache_parser.add_argument('--assetHash', type=str, help='PJSK asset hash (default: %(default)s)', default=DEFAULT_SEKAI_AB_HASH)
-    abcache_parser.add_argument('--assetHostHash', type=str, help='PJSK asset host hash (default: %(default)s)', default=DEFAULT_SEKAI_AB_HOST_HASH)
     abcache_parser.add_argument('--open', action='store_true',help='open cache directory. this will skip all updates.')
     abcache_parser.set_defaults(func=main_abcache)
     # live2dextract
     live2dextract_parser = subparsers.add_parser('live2dextract', help='''Extract Sekai Live2D Models in a AssetBundle''')
     live2dextract_parser.add_argument('infile', type=str, help='input file')
     live2dextract_parser.add_argument('outdir', type=str, help='output directory')
     live2dextract_parser.add_argument('--no-anim',action='store_true',help='don\'t extract animation clips')
```

### Comparing `sssekai-0.1.0/sssekai/abcache/__init__.py` & `sssekai-0.1.1/sssekai/abcache/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from os import path, remove, makedirs, stat
 from typing import List, Mapping
 from dataclasses import dataclass, asdict
 from requests import Session
 from logging import getLogger
 from pathlib import Path
 from concurrent.futures import ThreadPoolExecutor
+
+from sssekai import __version__
+from sssekai.unity import SEKAI_UNITY_VERSION
 logger = getLogger('sssekai.abcache')
 
-from sssekai.crypto.APIManager import decrypt
+from sssekai.crypto.APIManager import decrypt, encrypt
 from sssekai.crypto.AssetBundle import decrypt_headaer_inplace, SEKAI_AB_MAGIC
-from msgpack import unpackb, dump, load
+from msgpack import unpackb, dump, load, packb
 from tqdm import tqdm
 DEFAULT_CACHE_DIR = '~/.sssekai/abcache'
 DOWNLOADER_WORKER_COUNT = 8
 DEFAULT_FILESIZE_MATCH_RATIO = 1.5
 
-DEFAULT_SEKAI_APP_VERSION = '3.5.0'
-DEFAULT_SEKAI_APP_HASH = '5e9fea31-2613-bd13-1723-9fe15156bd66'
-DEFAULT_SEKAI_AB_HASH = '9a5e2be1-0502-24c6-389e-b79b6a24ec0b'
-DEFAULT_SEKAI_AB_HOST_HASH = 'cf2d2388'
+DEFAULT_SEKAI_APP_VERSION = '3.6.0'
+DEFAULT_SEKAI_APP_HASH = '7558547e-4753-6ebd-03ff-168494c32769'
 DEFAULT_SEKAI_APP_PLATFORM = 'android'
 
 class AbCacheDownloader(ThreadPoolExecutor):
     session : Session
     progress : tqdm = None
     def _ensure_progress(self):
         if not self.progress:
@@ -63,16 +64,14 @@
 
 @dataclass
 class AbCacheConfig:
     cache_dir : str # absolute path to cache directory
     app_version : str = None
     app_platform : str = None
     app_hash : str  = None
-    ab_hash : str = None
-    ab_host_hash : str  = None
 
 @dataclass
 class AbCacheEntry(dict):
     bundleName: str
     cacheFileName: str
     cacheDirectoryName: str
     hash: str
@@ -146,39 +145,73 @@
     def list_app_versions(self) -> List[str]:
         return [av.appVersion for av in self.appVersions]
 @dataclass
 class SekaiGameVersionData:
     profile : str
     assetbundleHostHash : str
     domain : str
+@dataclass
+class SekaiUserRegistrationData:
+    userId : int
+    signature : str
+    platform : str
+    deviceModel : str
+    operatingSystem : str
+    registeredAt : int
+@dataclass
+class SekaiUserData:
+    userRegistration : SekaiUserRegistrationData
+    credential : str
+    updatedResources : dict
+@dataclass
+class SekaiUserAuthData:
+    sessionToken: str
+    appVersion: str
+    multiPlayVersion: str
+    dataVersion: str
+    assetVersion: str
+    removeAssetVersion: str
+    assetHash: str
+    appVersionStatus: str
+    isStreamingVirtualLiveForceOpenUser: bool
+    deviceId: str
+    updatedResources: dict
+    suiteMasterSplitPath: list
 class AbCache(Session):    
     downloader : AbCacheDownloader
 
     config : AbCacheConfig
     local_abcache_index : AbCacheIndex  = None
 
+    sekai_user_data : SekaiUserData = None
+    sekai_user_auth_data : SekaiUserAuthData = None
     sekai_abcache_index  : AbCacheIndex = None
     sekai_system_data : SekaiSystemData  = None
     sekai_gameversion_data : SekaiGameVersionData  = None
 
     @property
     def SEKAI_APP_VERSION(self): return self.config.app_version
     @property
-    def SEKAI_ASSET_VERSION(self): return self.sekai_system_data.get_app_version_by_app(self.SEKAI_APP_VERSION).assetVersion
-    @property
     def SEKAI_APP_HASH(self): return self.config.app_hash
+
     @property
-    def SEKAI_AB_HASH(self): return self.config.ab_hash
+    def SEKAI_ASSET_VERSION(self): return self.sekai_system_data.get_app_version_by_app(self.SEKAI_APP_VERSION).assetVersion
+    @property
+    def SEKAI_AB_HASH(self): return self.sekai_user_auth_data.assetHash
     @property
     def SEKAI_AB_HOST_HASH(self): return self.sekai_gameversion_data.assetbundleHostHash
     @property
     def SEKAI_API_ENDPOINT(self): return 'https://production-game-api.sekai.colorfulpalette.org'
     @property
     def SEKAI_API_SYSTEM_DATA(self): return self.SEKAI_API_ENDPOINT + '/api/system'
     @property
+    def SEKAI_API_USER(self): return self.SEKAI_API_ENDPOINT + '/api/user'
+    @property
+    def SEKAI_API_USER_AUTH(self): return f'{self.SEKAI_API_USER}/{self.sekai_user_data.userRegistration.userId}/auth?refreshUpdatedResources=False'
+    @property
     def SEKAI_API_GAMEVERSION_ENDPOINT(self): return 'https://game-version.sekai.colorfulpalette.org'
     @property
     def SEKAI_AB_INFO_ENDPOINT(self): return f'https://production-{self.SEKAI_AB_HOST_HASH}-assetbundle-info.sekai.colorfulpalette.org/'
     @property
     def SEKAI_AB_ENDPOINT(self): return f'https://production-{self.SEKAI_AB_HOST_HASH}-assetbundle.sekai.colorfulpalette.org/'
     @property
     def SEKAI_AB_BASE_PATH(self): return f'{self.SEKAI_ASSET_VERSION}/{self.SEKAI_AB_HASH}/{self.config.app_platform}/'
@@ -193,14 +226,44 @@
         logger.info('Updating signatures')
         resp = self.post(self.SEKAI_ISSUE_SIGNATURE_ENDPOINT)
         resp.raise_for_status()
         self.headers['Cookie'] = resp.headers['Set-Cookie'] 
         # HACK: Per RFC6265, Cookies should not be visible to subdomains since it's not set with Domain attribute (https://github.com/psf/requests/issues/2576)
         # But the other endpoints uses it nontheless. So we have to set it manually.
 
+    def update_user_data(self):
+        logger.info('Updating user data')
+        payload = {
+            "platform": self.headers['X-Platform'],
+            "deviceModel": self.headers['X-DeviceModel'],
+            "operatingSystem": self.headers['X-OperatingSystem'],
+        }
+        payload = packb(payload)
+        payload = encrypt(payload)
+        resp = self.post(self.SEKAI_API_USER, data=payload)
+        resp.raise_for_status()
+        data = decrypt(resp.content)
+        data = unpackb(data)
+        self.sekai_user_data = SekaiUserData(**data)
+        self.sekai_user_data.userRegistration = SekaiUserRegistrationData(**self.sekai_user_data.userRegistration)
+
+    def update_user_auth_data(self):
+        logger.info('Updating user auth data')
+        payload = {
+            "credential": self.sekai_user_data.credential,
+            "deviceId" : None
+        }
+        payload = packb(payload)
+        payload = encrypt(payload)        
+        resp = self.put(self.SEKAI_API_USER_AUTH, data=payload)
+        resp.raise_for_status()
+        data = decrypt(resp.content)
+        data = unpackb(data)        
+        self.sekai_user_auth_data = SekaiUserAuthData(**data)
+        
     def update_system_data(self):
         logger.info('Updating system data')
         resp = self.get(self.SEKAI_API_SYSTEM_DATA)
         resp.raise_for_status()
         data = decrypt(resp.content)
         data = unpackb(data)
         self.sekai_system_data = SekaiSystemData(**data)
@@ -278,30 +341,35 @@
         self.wait_for_downloads()
     
     def update_metadata(self):
         logger.info('Updating metadata')
         logger.debug('Cache directory: %s' % self.config.cache_dir)
         logger.debug('Set App version: %s (%s), hash=%s' % (self.config.app_version,self.config.app_platform, self.SEKAI_APP_HASH))
         self.update_signatures()
-        self.update_system_data()
         self.update_gameversion_data()               
+        self.update_user_data()
+        self.update_user_auth_data()
+        self.update_system_data()
         self.update_abcache_index()
         logger.debug('Sekai AssetBundle version: %s' % self.SEKAI_ASSET_VERSION)
         logger.debug('Sekai AssetBundle host hash: %s' % self.SEKAI_AB_HOST_HASH)
 
     def __init__(self, config : AbCacheConfig) -> None:
         super().__init__()
         self.config = config
+        self.config.app_platform = self.config.app_platform.lower()
         self.headers.update({
             'Accept': 'application/octet-stream',
             'Content-Type': 'application/octet-stream',
             'Accept-Encoding': 'deflate, gzip',
-            'User-Agent': 'UnityPlayer/2020.3.32f1 (UnityWebRequest/1.0, libcurl/7.80.0-DEV)',
-            'X-Platform': self.config.app_platform,
-            'X-Unity-Version': '2020.3.32f1',
+            'User-Agent': 'UnityPlayer/%s' % SEKAI_UNITY_VERSION,
+            'X-Platform': self.config.app_platform.capitalize(),
+            'X-DeviceModel': 'sssekai/%s' % __version__,
+            'X-OperatingSystem': self.config.app_platform.capitalize(),
+            'X-Unity-Version': SEKAI_UNITY_VERSION,
             'X-App-Version': self.SEKAI_APP_VERSION,
             'X-App-Hash': self.SEKAI_APP_HASH
         })
         self.downloader = AbCacheDownloader(self)
         makedirs(self.config.cache_dir,exist_ok=True)
         try:
             self.load()
```

### Comparing `sssekai-0.1.0/sssekai/crypto/APIManager.py` & `sssekai-0.1.1/sssekai/crypto/APIManager.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.0/sssekai/crypto/AssetBundle.py` & `sssekai-0.1.1/sssekai/crypto/AssetBundle.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.0/sssekai/entrypoint/abcache.py` & `sssekai-0.1.1/sssekai/entrypoint/abcache.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from sssekai.abcache import AbCache, AbCacheConfig,logger
 def main_abcache(args):
     cache_dir = args.cache_dir
     cache_dir = os.path.expanduser(cache_dir)
     cache_dir = os.path.abspath(cache_dir)
-    config = AbCacheConfig(cache_dir, args.version, args.platform, args.appHash, args.assetHash, args.assetHostHash)
+    config = AbCacheConfig(cache_dir, args.version, args.platform, args.appHash)
     if args.open:
         from os import startfile
         startfile(config.cache_dir)
         return
     cache = AbCache(config)
     if not args.skip_update:
         cache.update_metadata()
```

### Comparing `sssekai-0.1.0/sssekai/entrypoint/live2dextract.py` & `sssekai-0.1.1/sssekai/entrypoint/live2dextract.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.0/sssekai/entrypoint/mvdata.py` & `sssekai-0.1.1/sssekai/entrypoint/mvdata.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.0/sssekai/entrypoint/spineextract.py` & `sssekai-0.1.1/sssekai/entrypoint/spineextract.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.0/sssekai/entrypoint/usmdemux.py` & `sssekai-0.1.1/sssekai/entrypoint/usmdemux.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.0/sssekai/fmt/moc3.py` & `sssekai-0.1.1/sssekai/fmt/moc3.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.0/sssekai/unity/AnimationClip.py` & `sssekai-0.1.1/sssekai/unity/AnimationClip.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.0/sssekai/unity/constant/SekaiLive2DPathNames.py` & `sssekai-0.1.1/sssekai/unity/constant/SekaiLive2DPathNames.py`

 * *Files identical despite different names*

### Comparing `sssekai-0.1.0/sssekai.egg-info/PKG-INFO` & `sssekai-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: sssekai
-Version: 0.1.0
-Summary: Project SEKAI Asset Utility / PJSK 资源下载 + Live2D, Spine, USM 提取
-Home-page: https://github.com/mos9527/sssekai
-Author: greats3an
-Author-email: greats3an@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: msgpack
-Requires-Dist: pycryptodome
-Requires-Dist: unitypy
-Requires-Dist: wannacri
-
 # sssekai
 Command-line tool (w/Python API support) for downloading/deobfuscating the game's assets, along with some other tools.
 
     usage: sssekai [-h]
                   {apidecrypt,abdecrypt,usmdemux,abcache,live2dextract,mitm} ...
 
     SSSekai Proejct SEKAI feat. Hatsune Miku (Android) Modding Tools
@@ -62,26 +45,38 @@
 ### Examples
 - Caches the game data into `D:\Sekai`
   ```powershell
   sssekai abcache --cache-dir D:\Sekai
   ```
 - Download game data for a *very specific* version into `D:\Sekai`
   ```powershell
-  sssekai abcache --cache-dir D:\Sekai --platform android --version "3.5.0" --appHash "5e9fea31-2613-bd13-1723-9fe15156bd66" --assetHash "9a5e2be1-0502-24c6-389e-b79b6a24ec0b" --assetHostHash "cf2d2388"
+  sssekai abcache --cache-dir D:\Sekai --platform android --version "3.5.0" --appHash "5e9fea31-2613-bd13-1723-9fe15156bd66"
   ```
-  The fields, `platform`, `appHash`, `assetHash`, `assetHostHash` are **all** necessary to facilitate the download.
-
-  The table below contains the values you might need for that purpose.
 
-  *FYI the game used to actually send these values with before 3.5.0! Now they don't :(*
 ### Known Game Versions And Their Respective Hashes
 *NOTE: This table will probably remain not up-to-date and/or incomplete. PRs are welcome for additions.*
-|platform|version|appHash|assetHash|assetHostHash|
-|-|-|-|-|-|
-|android|3.5.0|5e9fea31-2613-bd13-1723-9fe15156bd66|9a5e2be1-0502-24c6-389e-b79b6a24ec0b|cf2d2388|
+
+|platform|version|appHash|
+|-|-|-|
+|android|3.6.0|7558547e-4753-6ebd-03ff-168494c32769|
+|ios|3.6.0|7558547e-4753-6ebd-03ff-168494c32769|
+|android|3.5.0|5e9fea31-2613-bd13-1723-9fe15156bd66|
+|ios|3.5.0|5e9fea31-2613-bd13-1723-9fe15156bd66|
+#### Bonus: How to extract appHash from Android releases
+- Acquire the game's APK file.
+- Run [dump_android_pjsk_appHash.py](https://github.com/mos9527/sssekai/blob/main/sssekai/scripts/dump_android_pjsk_appHash.py) on it. For example:
+```bash
+python dump_android_pjsk_appHash.py pjsk_360.apk
+```
+- Which prints
+```
+7558547e-4753-6ebd-03ff-168494c32769 production_android
+7558547e-4753-6ebd-03ff-168494c32769 production_android
+7558547e-4753-6ebd-03ff-168494c32769 production_ios
+```
 
 ## What Do These Files Do? (WIP)
 There's a *ton* of them. Like ~45GB with version 3.5.0.(!) I'll try to document my limited findings here whenever possible 
 ### Spine2D Related Files
 NOTE: You'll need Spine2D SDK 4.x to load these.
 |Path|Purpose (Assumed)|
 |-|-|
@@ -123,8 +118,8 @@
 |live_pv/model/music_item|*PV Props. There aren't lots of those.|
 And strangly enough there's another folder *outside* live_pv that also contains 3D assets. I'll put it here.
 |Path|Purpose (Assumed)|
 |-|-|
 |model3d/model/stage_object|*PV Props, again. Those this time it's all instruments and it has the same aforementioned weighting issues.|
 
 # See Also
-https://github.com/mos9527/sssekai_blender_io
+https://github.com/mos9527/sssekai_blender_io
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sssekai-0.1.0/sssekai.egg-info/SOURCES.txt` & `sssekai-0.1.1/sssekai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

