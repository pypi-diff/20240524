# Comparing `tmp/drawlib-0.1.7.tar.gz` & `tmp/drawlib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drawlib-0.1.7.tar", max compression
+gzip compressed data, was "drawlib-0.1.8.tar", max compression
```

## Comparing `drawlib-0.1.7.tar` & `drawlib-0.1.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    11344 2024-04-05 18:42:05.538150 drawlib-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0     2421 2024-05-04 15:36:12.546708 drawlib-0.1.7/README.md
--rw-r--r--   0        0        0       27 2024-03-29 11:45:48.926601 drawlib-0.1.7/drawlib/.pylintrc
--rw-r--r--   0        0        0     1039 2024-05-17 13:51:50.749671 drawlib-0.1.7/drawlib/__init__.py
--rw-r--r--   0        0        0      688 2024-05-21 13:52:08.835136 drawlib-0.1.7/drawlib/__main__.py
--rw-r--r--   0        0        0      777 2024-04-07 14:54:59.159171 drawlib-0.1.7/drawlib/apis.py
--rw-r--r--   0        0        0      407 2024-04-12 07:27:54.821931 drawlib-0.1.7/drawlib/assets/__init__.py
--rw-r--r--   0        0        0      407 2024-05-01 10:34:11.053352 drawlib-0.1.7/drawlib/assets/v0_1/__init__.py
--rw-r--r--   0        0        0      407 2024-04-12 07:28:01.917218 drawlib-0.1.7/drawlib/assets/v0_1/fonticons/__init__.py
--rw-r--r--   0        0        0      407 2024-04-13 15:48:11.439423 drawlib-0.1.7/drawlib/assets/v0_1/fonts/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-07 03:53:05.340986 drawlib-0.1.7/drawlib/v0_1/__init__.py
--rw-r--r--   0        0        0      663 2024-04-06 12:40:11.972278 drawlib-0.1.7/drawlib/v0_1/__main__.py
--rw-r--r--   0        0        0     2421 2024-05-21 13:50:32.945869 drawlib-0.1.7/drawlib/v0_1/apis.py
--rw-r--r--   0        0        0      763 2024-04-06 11:52:52.776827 drawlib-0.1.7/drawlib/v0_1/private/__init__.py
--rw-r--r--   0        0        0    12860 2024-05-21 14:42:32.950675 drawlib-0.1.7/drawlib/v0_1/private/command.py
--rw-r--r--   0        0        0      548 2024-04-07 14:22:07.928062 drawlib-0.1.7/drawlib/v0_1/private/core/__init__.py
--rw-r--r--   0        0        0    12776 2024-04-23 00:24:17.718876 drawlib-0.1.7/drawlib/v0_1/private/core/colors.py
--rw-r--r--   0        0        0    13598 2024-05-17 11:32:14.717753 drawlib-0.1.7/drawlib/v0_1/private/core/dimage.py
--rw-r--r--   0        0        0    23775 2024-05-17 13:15:29.707391 drawlib-0.1.7/drawlib/v0_1/private/core/fonts.py
--rw-r--r--   0        0        0    33160 2024-05-17 07:10:44.348191 drawlib-0.1.7/drawlib/v0_1/private/core/model.py
--rw-r--r--   0        0        0    18865 2024-05-19 04:26:51.380337 drawlib-0.1.7/drawlib/v0_1/private/core/theme.py
--rw-r--r--   0        0        0    12272 2024-05-19 00:50:29.097717 drawlib-0.1.7/drawlib/v0_1/private/core/theme_officials.py
--rw-r--r--   0        0        0    51534 2024-05-17 08:42:26.352080 drawlib-0.1.7/drawlib/v0_1/private/core/theme_styles.py
--rw-r--r--   0        0        0    28300 2024-05-17 11:42:16.612394 drawlib-0.1.7/drawlib/v0_1/private/core/util.py
--rw-r--r--   0        0        0      548 2024-04-27 02:06:25.820510 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/__init__.py
--rw-r--r--   0        0        0    15589 2024-05-17 11:33:32.642807 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/base.py
--rw-r--r--   0        0        0     7992 2024-05-17 04:55:01.315534 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/canvas.py
--rw-r--r--   0        0        0     4950 2024-05-17 04:01:16.413350 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/image.py
--rw-r--r--   0        0        0     6593 2024-05-17 04:01:22.784734 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/line.py
--rw-r--r--   0        0        0     4297 2024-05-17 04:01:28.386700 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/original_arrow.py
--rw-r--r--   0        0        0    12132 2024-05-17 12:08:03.060649 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/original_polygon.py
--rw-r--r--   0        0        0    16466 2024-05-17 04:01:43.093731 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/patches.py
--rw-r--r--   0        0        0     3264 2024-05-17 04:02:22.095588 drawlib-0.1.7/drawlib/v0_1/private/core_canvas/text.py
--rw-r--r--   0        0        0     2067 2024-05-03 16:29:49.262484 drawlib-0.1.7/drawlib/v0_1/private/download.py
--rw-r--r--   0        0        0      881 2024-05-02 13:00:20.440339 drawlib-0.1.7/drawlib/v0_1/private/dutil.py
--rw-r--r--   0        0        0      589 2024-04-13 03:31:11.518478 drawlib-0.1.7/drawlib/v0_1/private/icons/__init__.py
--rw-r--r--   0        0        0   902368 2024-05-17 00:56:51.813460 drawlib-0.1.7/drawlib/v0_1/private/icons/phosphor.py
--rw-r--r--   0        0        0     1998 2024-05-17 04:04:01.158522 drawlib-0.1.7/drawlib/v0_1/private/icons/util.py
--rw-r--r--   0        0        0     1206 2024-05-21 13:50:52.977426 drawlib-0.1.7/drawlib/v0_1/private/logging.py
--rw-r--r--   0        0        0     6689 2024-05-21 13:34:20.888010 drawlib-0.1.7/drawlib/v0_1/private/settings.py
--rw-r--r--   0        0        0      589 2024-04-25 02:41:30.472250 drawlib-0.1.7/drawlib/v0_1/private/smartarts/__init__.py
--rw-r--r--   0        0        0     3482 2024-05-17 07:07:04.377539 drawlib-0.1.7/drawlib/v0_1/private/smartarts/bubblespeech.py
--rw-r--r--   0        0        0      426 2024-04-14 23:53:18.451455 drawlib-0.1.7/drawlib/v0_1/private/smartarts/cycle.py
--rw-r--r--   0        0        0      686 2024-05-17 01:14:56.535422 drawlib-0.1.7/drawlib/v0_1/private/smartarts/dsart.py
--rw-r--r--   0        0        0      660 2024-04-14 23:53:28.113177 drawlib-0.1.7/drawlib/v0_1/private/smartarts/groups.py
--rw-r--r--   0        0        0      619 2024-04-14 23:53:33.993167 drawlib-0.1.7/drawlib/v0_1/private/smartarts/pyramid.py
--rw-r--r--   0        0        0     5905 2024-05-17 01:19:04.280798 drawlib-0.1.7/drawlib/v0_1/private/smartarts/sourcecode.py
--rw-r--r--   0        0        0      426 2024-04-14 23:53:43.397670 drawlib-0.1.7/drawlib/v0_1/private/smartarts/table.py
--rw-r--r--   0        0        0      651 2024-04-14 23:53:50.199157 drawlib-0.1.7/drawlib/v0_1/private/smartarts/tree.py
--rw-r--r--   0        0        0    10163 2024-05-20 09:07:41.448465 drawlib-0.1.7/drawlib/v0_1/private/util.py
--rw-r--r--   0        0        0      407 2024-05-17 07:28:29.821380 drawlib-0.1.7/drawlib/v0_1/private/validators/__init__.py
--rw-r--r--   0        0        0     7382 2024-05-17 07:25:34.994200 drawlib-0.1.7/drawlib/v0_1/private/validators/args.py
--rw-r--r--   0        0        0     1576 2024-05-17 07:25:58.475653 drawlib-0.1.7/drawlib/v0_1/private/validators/color.py
--rw-r--r--   0        0        0     3275 2024-05-17 08:44:34.098244 drawlib-0.1.7/drawlib/v0_1/private/validators/coordinate.py
--rw-r--r--   0        0        0      891 2024-05-17 08:44:42.485495 drawlib-0.1.7/drawlib/v0_1/private/validators/image.py
--rw-r--r--   0        0        0     1249 2024-05-17 08:44:59.932902 drawlib-0.1.7/drawlib/v0_1/private/validators/line.py
--rw-r--r--   0        0        0     1332 2024-05-17 08:45:07.566582 drawlib-0.1.7/drawlib/v0_1/private/validators/shape.py
--rw-r--r--   0        0        0      660 2024-05-17 07:27:28.907431 drawlib-0.1.7/drawlib/v0_1/private/validators/smartarts.py
--rw-r--r--   0        0        0     2276 2024-05-17 08:45:25.563109 drawlib-0.1.7/drawlib/v0_1/private/validators/style.py
--rw-r--r--   0        0        0      824 2024-05-17 07:27:54.398157 drawlib-0.1.7/drawlib/v0_1/private/validators/text.py
--rw-r--r--   0        0        0     2270 2024-05-17 08:45:46.188412 drawlib-0.1.7/drawlib/v0_1/private/validators/types.py
--rw-r--r--   0        0        0      712 2024-05-21 14:45:13.302199 drawlib-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 drawlib-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-05 18:42:05.538150 drawlib-0.1.8/LICENSE.txt
+-rw-r--r--   0        0        0     2421 2024-05-04 15:36:12.546708 drawlib-0.1.8/README.md
+-rw-r--r--   0        0        0       27 2024-03-29 11:45:48.926601 drawlib-0.1.8/drawlib/.pylintrc
+-rw-r--r--   0        0        0     1039 2024-05-21 14:46:50.727969 drawlib-0.1.8/drawlib/__init__.py
+-rw-r--r--   0        0        0      688 2024-05-21 13:52:08.835136 drawlib-0.1.8/drawlib/__main__.py
+-rw-r--r--   0        0        0      777 2024-04-07 14:54:59.159171 drawlib-0.1.8/drawlib/apis.py
+-rw-r--r--   0        0        0      407 2024-04-12 07:27:54.821931 drawlib-0.1.8/drawlib/assets/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-01 10:34:11.053352 drawlib-0.1.8/drawlib/assets/v0_1/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-12 07:28:01.917218 drawlib-0.1.8/drawlib/assets/v0_1/fonticons/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-13 15:48:11.439423 drawlib-0.1.8/drawlib/assets/v0_1/fonts/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-07 03:53:05.340986 drawlib-0.1.8/drawlib/v0_1/__init__.py
+-rw-r--r--   0        0        0      663 2024-04-06 12:40:11.972278 drawlib-0.1.8/drawlib/v0_1/__main__.py
+-rw-r--r--   0        0        0     2438 2024-05-24 01:25:55.873169 drawlib-0.1.8/drawlib/v0_1/apis.py
+-rw-r--r--   0        0        0      763 2024-04-06 11:52:52.776827 drawlib-0.1.8/drawlib/v0_1/private/__init__.py
+-rw-r--r--   0        0        0    12860 2024-05-21 14:42:32.950675 drawlib-0.1.8/drawlib/v0_1/private/command.py
+-rw-r--r--   0        0        0      548 2024-04-07 14:22:07.928062 drawlib-0.1.8/drawlib/v0_1/private/core/__init__.py
+-rw-r--r--   0        0        0    12776 2024-05-22 11:20:38.275207 drawlib-0.1.8/drawlib/v0_1/private/core/colors.py
+-rw-r--r--   0        0        0    13652 2024-05-24 15:37:46.743882 drawlib-0.1.8/drawlib/v0_1/private/core/dimage.py
+-rw-r--r--   0        0        0    23777 2024-05-24 01:28:49.886237 drawlib-0.1.8/drawlib/v0_1/private/core/fonts.py
+-rw-r--r--   0        0        0    33167 2024-05-24 01:28:33.651901 drawlib-0.1.8/drawlib/v0_1/private/core/model.py
+-rw-r--r--   0        0        0    18865 2024-05-19 04:26:51.380337 drawlib-0.1.8/drawlib/v0_1/private/core/theme.py
+-rw-r--r--   0        0        0    12976 2024-05-24 01:43:09.114237 drawlib-0.1.8/drawlib/v0_1/private/core/theme_officials.py
+-rw-r--r--   0        0        0    51534 2024-05-17 08:42:26.352080 drawlib-0.1.8/drawlib/v0_1/private/core/theme_styles.py
+-rw-r--r--   0        0        0    28300 2024-05-17 11:42:16.612394 drawlib-0.1.8/drawlib/v0_1/private/core/util.py
+-rw-r--r--   0        0        0      548 2024-04-27 02:06:25.820510 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/__init__.py
+-rw-r--r--   0        0        0    15548 2024-05-24 01:29:18.823658 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/base.py
+-rw-r--r--   0        0        0     7992 2024-05-17 04:55:01.315534 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/canvas.py
+-rw-r--r--   0        0        0     5309 2024-05-24 16:33:38.203652 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/image.py
+-rw-r--r--   0        0        0     6593 2024-05-17 04:01:22.784734 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/line.py
+-rw-r--r--   0        0        0     4297 2024-05-17 04:01:28.386700 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/original_arrow.py
+-rw-r--r--   0        0        0    12132 2024-05-17 12:08:03.060649 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/original_polygon.py
+-rw-r--r--   0        0        0    16466 2024-05-17 04:01:43.093731 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/patches.py
+-rw-r--r--   0        0        0     3264 2024-05-17 04:02:22.095588 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/text.py
+-rw-r--r--   0        0        0     2067 2024-05-03 16:29:49.262484 drawlib-0.1.8/drawlib/v0_1/private/download.py
+-rw-r--r--   0        0        0      881 2024-05-02 13:00:20.440339 drawlib-0.1.8/drawlib/v0_1/private/dutil.py
+-rw-r--r--   0        0        0      589 2024-04-13 03:31:11.518478 drawlib-0.1.8/drawlib/v0_1/private/icons/__init__.py
+-rw-r--r--   0        0        0   902368 2024-05-17 00:56:51.813460 drawlib-0.1.8/drawlib/v0_1/private/icons/phosphor.py
+-rw-r--r--   0        0        0     1998 2024-05-17 04:04:01.158522 drawlib-0.1.8/drawlib/v0_1/private/icons/util.py
+-rw-r--r--   0        0        0     1206 2024-05-21 13:50:52.977426 drawlib-0.1.8/drawlib/v0_1/private/logging.py
+-rw-r--r--   0        0        0     6689 2024-05-21 13:34:20.888010 drawlib-0.1.8/drawlib/v0_1/private/settings.py
+-rw-r--r--   0        0        0      589 2024-04-25 02:41:30.472250 drawlib-0.1.8/drawlib/v0_1/private/smartarts/__init__.py
+-rw-r--r--   0        0        0     3482 2024-05-17 07:07:04.377539 drawlib-0.1.8/drawlib/v0_1/private/smartarts/bubblespeech.py
+-rw-r--r--   0        0        0      426 2024-04-14 23:53:18.451455 drawlib-0.1.8/drawlib/v0_1/private/smartarts/cycle.py
+-rw-r--r--   0        0        0      686 2024-05-17 01:14:56.535422 drawlib-0.1.8/drawlib/v0_1/private/smartarts/dsart.py
+-rw-r--r--   0        0        0      660 2024-04-14 23:53:28.113177 drawlib-0.1.8/drawlib/v0_1/private/smartarts/groups.py
+-rw-r--r--   0        0        0      619 2024-04-14 23:53:33.993167 drawlib-0.1.8/drawlib/v0_1/private/smartarts/pyramid.py
+-rw-r--r--   0        0        0     5905 2024-05-17 01:19:04.280798 drawlib-0.1.8/drawlib/v0_1/private/smartarts/sourcecode.py
+-rw-r--r--   0        0        0      426 2024-04-14 23:53:43.397670 drawlib-0.1.8/drawlib/v0_1/private/smartarts/table.py
+-rw-r--r--   0        0        0      651 2024-04-14 23:53:50.199157 drawlib-0.1.8/drawlib/v0_1/private/smartarts/tree.py
+-rw-r--r--   0        0        0    10163 2024-05-20 09:07:41.448465 drawlib-0.1.8/drawlib/v0_1/private/util.py
+-rw-r--r--   0        0        0      407 2024-05-17 07:28:29.821380 drawlib-0.1.8/drawlib/v0_1/private/validators/__init__.py
+-rw-r--r--   0        0        0     7382 2024-05-17 07:25:34.994200 drawlib-0.1.8/drawlib/v0_1/private/validators/args.py
+-rw-r--r--   0        0        0     1576 2024-05-17 07:25:58.475653 drawlib-0.1.8/drawlib/v0_1/private/validators/color.py
+-rw-r--r--   0        0        0     3275 2024-05-17 08:44:34.098244 drawlib-0.1.8/drawlib/v0_1/private/validators/coordinate.py
+-rw-r--r--   0        0        0      891 2024-05-17 08:44:42.485495 drawlib-0.1.8/drawlib/v0_1/private/validators/image.py
+-rw-r--r--   0        0        0     1249 2024-05-17 08:44:59.932902 drawlib-0.1.8/drawlib/v0_1/private/validators/line.py
+-rw-r--r--   0        0        0     1332 2024-05-17 08:45:07.566582 drawlib-0.1.8/drawlib/v0_1/private/validators/shape.py
+-rw-r--r--   0        0        0      660 2024-05-17 07:27:28.907431 drawlib-0.1.8/drawlib/v0_1/private/validators/smartarts.py
+-rw-r--r--   0        0        0     2276 2024-05-17 08:45:25.563109 drawlib-0.1.8/drawlib/v0_1/private/validators/style.py
+-rw-r--r--   0        0        0      824 2024-05-17 07:27:54.398157 drawlib-0.1.8/drawlib/v0_1/private/validators/text.py
+-rw-r--r--   0        0        0     2270 2024-05-17 08:45:46.188412 drawlib-0.1.8/drawlib/v0_1/private/validators/types.py
+-rw-r--r--   0        0        0      712 2024-05-24 16:35:25.217531 drawlib-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 drawlib-0.1.8/PKG-INFO
```

### Comparing `drawlib-0.1.7/LICENSE.txt` & `drawlib-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/README.md` & `drawlib-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/__init__.py` & `drawlib-0.1.8/drawlib/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 - drawlib.v0_1: API v0.1 interface (latest)
 
 """
 
 from typing import Final
 
 # please update here when you release new version
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 
 # might not be changed
 LIB_NAME: Final[str] = "drawlib"
 AUTHOR: Final[str] = "Yuichi Ito"
 CONTACT: Final[str] = "yuichi@yuichi.com"
 __version__: Final[str] = VERSION
```

### Comparing `drawlib-0.1.7/drawlib/__main__.py` & `drawlib-0.1.8/drawlib/__main__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/apis.py` & `drawlib-0.1.8/drawlib/apis.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/__init__.py` & `drawlib-0.1.8/drawlib/v0_1/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/__main__.py` & `drawlib-0.1.8/drawlib/v0_1/__main__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/apis.py` & `drawlib-0.1.8/drawlib/v0_1/apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 #############
 ### Class ###
 #############
 
 from drawlib.v0_1.private.core.colors import (
     Colors,
     Colors140,
+    ColorsBase,
 )
 
 from drawlib.v0_1.private.core.model import (
     IconStyle,
     ImageStyle,
     LineStyle,
     LineArrowStyle,
@@ -48,15 +49,15 @@
     FontArabic,
     FontBrahmic,
     FontChinese,
     FontJapanese,
     FontKorean,
     FontMonoSpace,
     FontRoboto,
-    FontSanSerif,
+    FontSansSerif,
     FontSerif,
     FontSourceCode,
     FontThai,
 )
 
 from drawlib.v0_1.private.core.dimage import (
     Dimage,
```

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/__init__.py` & `drawlib-0.1.8/drawlib/v0_1/private/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/command.py` & `drawlib-0.1.8/drawlib/v0_1/private/command.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core/__init__.py` & `drawlib-0.1.8/drawlib/v0_1/private/core/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core/colors.py` & `drawlib-0.1.8/drawlib/v0_1/private/core/colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 Please don't use Enum for colors. Just RGB with tuple(int, int int) is good.
 
 """
 
 from typing import Final, Tuple, Optional
 
 
-class BaseColors:
+class ColorsBase:
     """Base class of Colors class
 
     Posses color ``Transparent`` and utility functions.
 
     """
 
     Transparent: Final[Tuple[int, int, int, float]] = (0, 0, 0, 0.0)
@@ -104,15 +104,15 @@
 
         """
 
         rgb = int(grayscale * 255)
         return (rgb, rgb, rgb, alpha)
 
 
-class Colors(BaseColors):
+class Colors(ColorsBase):
     """Web basic color class.
 
     Supports 16 of basic web colors.
     ``Transparent`` is also supported.
 
     """
 
@@ -130,15 +130,15 @@
     Red: Final[Tuple[int, int, int]] = (255, 0, 0)
     Silver: Final[Tuple[int, int, int]] = (192, 192, 192)
     Teal: Final[Tuple[int, int, int]] = (0, 128, 128)
     White: Final[Tuple[int, int, int]] = (255, 255, 255)
     Yellow: Final[Tuple[int, int, int]] = (255, 255, 0)
 
 
-class Colors140(BaseColors):
+class Colors140(ColorsBase):
     """Web colors class. CSS Color Module Level3.
 
     Supports 140 of "CSS Color Module Level3" web colors.
     ``Transparent`` is also supported.
 
     """
```

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core/fonts.py` & `drawlib-0.1.8/drawlib/v0_1/private/core/fonts.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 ### FONTS ###
 #############
 
 # Default
 # - Font: English + CJK
 #
 # Alphabet
-# - FontSanSerif
+# - FontSansSerif
 # - FontSans
 # - FontMonoSpace
 # - FontRoboto
 #
 # SourceCode
 # - FontSourcecode
 #
@@ -125,15 +125,15 @@
     )
     SERIF_BOLD = get_fontfile_tuple(
         "cjk_japanese_noto_serif/bold.otf",
         "ea7175c0325777d126622340f9c94a66",
     )
 
 
-class FontSanSerif(FontBase):
+class FontSansSerif(FontBase):
     """Drawlib Fonts.
 
     Drawlib avoid using system font since it depends on host OS.
     Using only internal font files and user provided font file.
 
     """
```

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core/model.py` & `drawlib-0.1.8/drawlib/v0_1/private/core/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     Final,
 )
 from drawlib.v0_1.private.core.fonts import (
     Font,
     FontArabic,
     FontBase,
     FontSerif,
-    FontSanSerif,
+    FontSansSerif,
     FontChinese,
     FontJapanese,
     FontKorean,
     FontMonoSpace,
     FontRoboto,
     FontSourceCode,
     FontFile,
@@ -657,15 +657,15 @@
     halign: Optional[Literal["left", "center", "right"]] = None
     valign: Optional[Literal["bottom", "center", "top"]] = None
     font: Union[
         Font,
         FontArabic,
         FontBase,
         FontSerif,
-        FontSanSerif,
+        FontSansSerif,
         FontChinese,
         FontJapanese,
         FontKorean,
         FontMonoSpace,
         FontRoboto,
         FontSourceCode,
         FontFile,
@@ -755,15 +755,15 @@
 
     @property  # type: ignore[no-redef]
     def font(self) -> Union[
         Font,
         FontArabic,
         FontBase,
         FontSerif,
-        FontSanSerif,
+        FontSansSerif,
         FontChinese,
         FontJapanese,
         FontKorean,
         FontMonoSpace,
         FontRoboto,
         FontSourceCode,
         FontFile,
@@ -776,15 +776,15 @@
     def font(
         self,
         value: Union[
             Font,
             FontArabic,
             FontBase,
             FontSerif,
-            FontSanSerif,
+            FontSansSerif,
             FontChinese,
             FontJapanese,
             FontKorean,
             FontMonoSpace,
             FontRoboto,
             FontSourceCode,
             FontFile,
@@ -882,15 +882,15 @@
     halign: Optional[Literal["left", "center", "right"]] = None
     valign: Optional[Literal["bottom", "center", "top"]] = None
     font: Union[
         Font,
         FontArabic,
         FontBase,
         FontSerif,
-        FontSanSerif,
+        FontSansSerif,
         FontChinese,
         FontJapanese,
         FontKorean,
         FontMonoSpace,
         FontRoboto,
         FontSourceCode,
         FontFile,
@@ -984,15 +984,15 @@
 
     @property  # type: ignore[no-redef]
     def font(self) -> Union[
         Font,
         FontArabic,
         FontBase,
         FontSerif,
-        FontSanSerif,
+        FontSansSerif,
         FontChinese,
         FontJapanese,
         FontKorean,
         FontMonoSpace,
         FontRoboto,
         FontSourceCode,
         FontFile,
@@ -1005,15 +1005,15 @@
     def font(
         self,
         value: Union[
             Font,
             FontArabic,
             FontBase,
             FontSerif,
-            FontSanSerif,
+            FontSansSerif,
             FontChinese,
             FontJapanese,
             FontKorean,
             FontMonoSpace,
             FontRoboto,
             FontSourceCode,
             FontFile,
```

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core/theme.py` & `drawlib-0.1.8/drawlib/v0_1/private/core/theme.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core/theme_officials.py` & `drawlib-0.1.8/drawlib/v0_1/private/core/theme_officials.py`

 * *Files 9% similar despite different names*

```diff
@@ -100,14 +100,38 @@
         shapestyle=default_styles[4],
         shapetextstyle=default_styles[5],
         textstyle=default_styles[6],
         named_styles=named_styles,
     )
 
 
+def get_flat_ui_palette_v1() -> _ThemeReturnValue:
+    # https://flatuicolors.com/palette/defo
+    turquoise = (26, 188, 156)
+    green_sea = (22, 160, 133)
+    emerald = (46, 204, 113)
+    nephritis = (39, 174, 96)
+    peter_river = (52, 152, 219)
+    belize_hole = (41, 128, 185)
+    amethyst = (155, 89, 182)
+    wisteria = (142, 68, 173)
+    wet_asphalt = (52, 73, 94)
+    midnight_blue = (44, 62, 80)
+    sun_flower = (241, 196, 15)
+    orange = (243, 156, 18)
+    carrot = (230, 126, 34)
+    pumpkin = (211, 84, 0)
+    alizarin = (231, 76, 60)
+    pomegranate = (192, 57, 43)
+    clouds = (236, 240, 241)
+    silver = (189, 195, 199)
+    concrete = (149, 165, 166)
+    asbestos = (127, 140, 141)
+
+
 def get_gray() -> _ThemeReturnValue:
     """Change theme to gray.
 
     Returns:
         None
 
     """
```

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core/theme_styles.py` & `drawlib-0.1.8/drawlib/v0_1/private/core/theme_styles.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core/util.py` & `drawlib-0.1.8/drawlib/v0_1/private/core/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/__init__.py` & `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/base.py` & `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     DEFAULT_WIDTH: Final[int] = 100
     DEFAULT_HEIGHT: Final[int] = 100
     DEFAULT_DPI: Final[int] = 100
     DEFAULT_GRID: Final[bool] = False
     DEFAULT_GRID_ONLY: Final[bool] = False
     DEFAULT_GRID_STYLE: Final[LineStyle] = LineStyle(width=1, color=Colors.Gray, style="dashed")
     DEFAULT_GRID_CENTERSTYLE: Final[LineStyle] = LineStyle(width=2, color=Colors.Gray, style="dashed")
-    SYSTEM_FONTS = ["serif", "sanserif"]
 
     @error_handler
     def __init__(self) -> None:
         """Initialize Canvas instance with default params.
 
         Not only first initialization, it is called from ``clear()``.
         Variables are updated on ``config()``.
```

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/canvas.py` & `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/image.py` & `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -123,14 +123,23 @@
                 y -= y_shift
             else:
                 raise ValueError(f'valign "{style.valign}" is not supported.')
 
         # create image drawing object
         pil_image = pimg.get_pil_image()
         im = numpy.array(pil_image)
+
+        # grayscale doesn't work fine on matplotlib. convert to RGBA.
+        if im.ndim == 3:
+            if im.shape[2] == 2:
+                gray = im[:, :, 0]
+                alpha = im[:, :, 1]
+                rgb_array = numpy.stack((gray, gray, gray), axis=-1)
+                im = numpy.concatenate((rgb_array, alpha[:, :, numpy.newaxis]), axis=-1)
+
         imagebox = offsetbox.OffsetImage(im, zoom=zoom)
         ab = offsetbox.AnnotationBbox(imagebox, (x, y), frameon=False)
 
         # draw later
         self._artists.append(ab)
 
         # border
```

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/line.py` & `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/line.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/original_arrow.py` & `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/original_arrow.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/original_polygon.py` & `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/original_polygon.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/patches.py` & `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/patches.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/core_canvas/text.py` & `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/text.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/download.py` & `drawlib-0.1.8/drawlib/v0_1/private/download.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/dutil.py` & `drawlib-0.1.8/drawlib/v0_1/private/dutil.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/icons/__init__.py` & `drawlib-0.1.8/drawlib/v0_1/private/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/icons/phosphor.py` & `drawlib-0.1.8/drawlib/v0_1/private/icons/phosphor.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/icons/util.py` & `drawlib-0.1.8/drawlib/v0_1/private/icons/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/logging.py` & `drawlib-0.1.8/drawlib/v0_1/private/logging.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/settings.py` & `drawlib-0.1.8/drawlib/v0_1/private/settings.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/smartarts/__init__.py` & `drawlib-0.1.8/drawlib/v0_1/private/smartarts/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/smartarts/bubblespeech.py` & `drawlib-0.1.8/drawlib/v0_1/private/smartarts/bubblespeech.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/smartarts/dsart.py` & `drawlib-0.1.8/drawlib/v0_1/private/smartarts/dsart.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/smartarts/groups.py` & `drawlib-0.1.8/drawlib/v0_1/private/smartarts/groups.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/smartarts/pyramid.py` & `drawlib-0.1.8/drawlib/v0_1/private/smartarts/pyramid.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/smartarts/sourcecode.py` & `drawlib-0.1.8/drawlib/v0_1/private/smartarts/sourcecode.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/smartarts/tree.py` & `drawlib-0.1.8/drawlib/v0_1/private/smartarts/tree.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/util.py` & `drawlib-0.1.8/drawlib/v0_1/private/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/validators/args.py` & `drawlib-0.1.8/drawlib/v0_1/private/validators/args.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/validators/color.py` & `drawlib-0.1.8/drawlib/v0_1/private/validators/color.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/validators/coordinate.py` & `drawlib-0.1.8/drawlib/v0_1/private/validators/coordinate.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/validators/image.py` & `drawlib-0.1.8/drawlib/v0_1/private/validators/image.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/validators/line.py` & `drawlib-0.1.8/drawlib/v0_1/private/validators/line.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/validators/shape.py` & `drawlib-0.1.8/drawlib/v0_1/private/validators/shape.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/validators/smartarts.py` & `drawlib-0.1.8/drawlib/v0_1/private/validators/smartarts.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/validators/style.py` & `drawlib-0.1.8/drawlib/v0_1/private/validators/style.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/validators/text.py` & `drawlib-0.1.8/drawlib/v0_1/private/validators/text.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/drawlib/v0_1/private/validators/types.py` & `drawlib-0.1.8/drawlib/v0_1/private/validators/types.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.7/pyproject.toml` & `drawlib-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "drawlib"
-version = "0.1.7"
+version = "0.1.8"
 description = "Python drawing library. Illustration as Code."
 homepage = "https://www.drawlib.com"
 repository = "https://github.com/yuichi110/drawlib"
 authors = [ "Yuichi Ito <yuichi@yuichi.com>",]
 readme = "README.md"
 
 [tool.black]
```

### Comparing `drawlib-0.1.7/PKG-INFO` & `drawlib-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drawlib
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python drawing library. Illustration as Code.
 Home-page: https://www.drawlib.com
 Author: Yuichi Ito
 Author-email: yuichi@yuichi.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

