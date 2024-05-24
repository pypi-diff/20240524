# Comparing `tmp/qtharmony-0.3.3.tar.gz` & `tmp/qtharmony-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.3.3.tar", max compression
+gzip compressed data, was "qtharmony-0.3.4.tar", max compression
```

## Comparing `qtharmony-0.3.3.tar` & `qtharmony-0.3.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.3.3/LICENSE
--rw-r--r--   0        0        0     2340 2024-05-14 07:15:03.814438 qtharmony-0.3.3/README.md
--rw-r--r--   0        0        0      332 2024-05-19 17:59:47.817516 qtharmony-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.3.3/qtharmony/__init__.py
--rw-r--r--   0        0        0       22 2024-05-14 15:55:11.674548 qtharmony-0.3.3/qtharmony/config/__init__.py
--rw-r--r--   0        0        0      233 2024-05-14 15:55:11.674548 qtharmony-0.3.3/qtharmony/config/config.py
--rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.3.3/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      628 2024-05-14 15:55:11.674548 qtharmony-0.3.3/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0      120 2024-05-14 15:55:11.674548 qtharmony-0.3.3/qtharmony/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-14 15:55:11.674548 qtharmony-0.3.3/qtharmony/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-14 15:55:11.674548 qtharmony-0.3.3/qtharmony/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-14 15:55:11.674548 qtharmony-0.3.3/qtharmony/core/font.py
--rw-r--r--   0        0        0      876 2024-05-14 15:55:11.674548 qtharmony-0.3.3/qtharmony/core/load.py
--rw-r--r--   0        0        0     2097 2024-05-19 17:59:31.518295 qtharmony-0.3.3/qtharmony/core/sizes.py
--rw-r--r--   0        0        0     1235 2024-05-14 15:55:11.674548 qtharmony-0.3.3/qtharmony/core/stylesheet.py
--rw-r--r--   0        0        0       80 2024-05-14 15:55:11.674548 qtharmony-0.3.3/qtharmony/core/theme/__init__.py
--rw-r--r--   0        0        0     1295 2024-05-14 15:55:11.674548 qtharmony-0.3.3/qtharmony/core/theme/theme_builder.py
--rw-r--r--   0        0        0     2345 2024-05-14 15:55:11.674548 qtharmony-0.3.3/qtharmony/core/theme/theme_manager.py
--rw-r--r--   0        0        0       34 2024-05-19 17:59:31.518295 qtharmony-0.3.3/qtharmony/gui/icon.py
--rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.3.3/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0     5411 2024-05-19 17:59:31.518295 qtharmony-0.3.3/qtharmony/resources/themes/dark-default.json
--rw-r--r--   0        0        0     4611 2024-05-12 12:26:40.223721 qtharmony-0.3.3/qtharmony/resources/themes/dark-green.json
--rw-r--r--   0        0        0     4563 2024-05-12 11:50:16.451713 qtharmony-0.3.3/qtharmony/resources/themes/light-default.json
--rw-r--r--   0        0        0     4560 2024-05-12 12:20:22.144106 qtharmony-0.3.3/qtharmony/resources/themes/light-green.json
--rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.3.3/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.3.3/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.3.3/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0      583 2024-05-19 17:59:31.518295 qtharmony-0.3.3/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     2931 2024-05-19 17:59:31.518295 qtharmony-0.3.3/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0     2674 2024-05-19 15:13:06.504362 qtharmony-0.3.3/qtharmony/widgets/basic/check_box.py
--rw-r--r--   0        0        0     2672 2024-05-19 15:13:06.504362 qtharmony-0.3.3/qtharmony/widgets/basic/digital_entry.py
--rw-r--r--   0        0        0     3646 2024-05-19 15:13:06.504362 qtharmony-0.3.3/qtharmony/widgets/basic/drop_down_menu.py
--rw-r--r--   0        0        0     2676 2024-05-19 15:13:06.504362 qtharmony-0.3.3/qtharmony/widgets/basic/entry.py
--rw-r--r--   0        0        0     1028 2024-05-19 15:13:06.504362 qtharmony-0.3.3/qtharmony/widgets/basic/frame.py
--rw-r--r--   0        0        0     2872 2024-05-19 17:59:31.518295 qtharmony-0.3.3/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0     3463 2024-05-19 17:59:31.518295 qtharmony-0.3.3/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0      389 2024-05-19 17:59:31.518295 qtharmony-0.3.3/qtharmony/widgets/basic/picture.py
--rw-r--r--   0        0        0     2072 2024-05-19 15:13:06.507695 qtharmony-0.3.3/qtharmony/widgets/basic/radio_button.py
--rw-r--r--   0        0        0     1178 2024-05-19 17:59:31.518295 qtharmony-0.3.3/qtharmony/widgets/basic/scrollbar.py
--rw-r--r--   0        0        0     2395 2024-05-19 15:13:06.507695 qtharmony-0.3.3/qtharmony/widgets/basic/splitter.py
--rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.3.3/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.3.3/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.3.3/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.3.3/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.3.3/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.3.3/qtharmony/widgets/basic/styles/frame.css
--rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.3.3/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.3.3/qtharmony/widgets/basic/styles/label.css
--rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.3.3/qtharmony/widgets/basic/styles/path_entry.css
--rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.3.3/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0      840 2024-05-19 17:59:31.518295 qtharmony-0.3.3/qtharmony/widgets/basic/styles/scrollbar.css
--rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.3.3/qtharmony/widgets/basic/styles/splitter.css
--rw-r--r--   0        0        0        0 2024-05-19 17:59:31.521628 qtharmony-0.3.3/qtharmony/widgets/basic/styles/text_box.css
--rw-r--r--   0        0        0        0 2024-05-19 15:13:06.507695 qtharmony-0.3.3/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     1703 2024-05-19 17:59:31.521628 qtharmony-0.3.3/qtharmony/widgets/basic/text_box.py
--rw-r--r--   0        0        0     1460 2024-05-19 15:13:06.514361 qtharmony-0.3.3/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0     4047 2024-05-19 17:59:31.521628 qtharmony-0.3.3/qtharmony/widgets/custom/path_entry.py
--rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.3.3/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     2679 2024-05-14 15:55:11.677882 qtharmony-0.3.3/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.3.3/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 qtharmony-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2340 2024-05-14 07:15:03.814438 qtharmony-0.3.4/README.md
+-rw-r--r--   0        0        0      332 2024-05-24 17:32:26.932939 qtharmony-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.3.4/qtharmony/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-14 15:55:11.674548 qtharmony-0.3.4/qtharmony/config/__init__.py
+-rw-r--r--   0        0        0      233 2024-05-14 15:55:11.674548 qtharmony-0.3.4/qtharmony/config/config.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.3.4/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      628 2024-05-14 15:55:11.674548 qtharmony-0.3.4/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0      120 2024-05-14 15:55:11.674548 qtharmony-0.3.4/qtharmony/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-14 15:55:11.674548 qtharmony-0.3.4/qtharmony/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-14 15:55:11.674548 qtharmony-0.3.4/qtharmony/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-14 15:55:11.674548 qtharmony-0.3.4/qtharmony/core/font.py
+-rw-r--r--   0        0        0      876 2024-05-14 15:55:11.674548 qtharmony-0.3.4/qtharmony/core/load.py
+-rw-r--r--   0        0        0     2097 2024-05-19 17:59:31.518295 qtharmony-0.3.4/qtharmony/core/sizes.py
+-rw-r--r--   0        0        0     1235 2024-05-14 15:55:11.674548 qtharmony-0.3.4/qtharmony/core/stylesheet.py
+-rw-r--r--   0        0        0       80 2024-05-14 15:55:11.674548 qtharmony-0.3.4/qtharmony/core/theme/__init__.py
+-rw-r--r--   0        0        0     1295 2024-05-14 15:55:11.674548 qtharmony-0.3.4/qtharmony/core/theme/theme_builder.py
+-rw-r--r--   0        0        0     2345 2024-05-14 15:55:11.674548 qtharmony-0.3.4/qtharmony/core/theme/theme_manager.py
+-rw-r--r--   0        0        0       34 2024-05-19 17:59:31.518295 qtharmony-0.3.4/qtharmony/gui/icon.py
+-rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.3.4/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0     5411 2024-05-19 17:59:31.518295 qtharmony-0.3.4/qtharmony/resources/themes/dark-default.json
+-rw-r--r--   0        0        0     4611 2024-05-12 12:26:40.223721 qtharmony-0.3.4/qtharmony/resources/themes/dark-green.json
+-rw-r--r--   0        0        0     5643 2024-05-24 17:24:34.344708 qtharmony-0.3.4/qtharmony/resources/themes/light-default.json
+-rw-r--r--   0        0        0     4560 2024-05-12 12:20:22.144106 qtharmony-0.3.4/qtharmony/resources/themes/light-green.json
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.3.4/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.3.4/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.3.4/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0      583 2024-05-19 17:59:31.518295 qtharmony-0.3.4/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     2931 2024-05-19 17:59:31.518295 qtharmony-0.3.4/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0     2674 2024-05-19 15:13:06.504362 qtharmony-0.3.4/qtharmony/widgets/basic/check_box.py
+-rw-r--r--   0        0        0     2672 2024-05-19 15:13:06.504362 qtharmony-0.3.4/qtharmony/widgets/basic/digital_entry.py
+-rw-r--r--   0        0        0     3646 2024-05-19 15:13:06.504362 qtharmony-0.3.4/qtharmony/widgets/basic/drop_down_menu.py
+-rw-r--r--   0        0        0     2676 2024-05-19 15:13:06.504362 qtharmony-0.3.4/qtharmony/widgets/basic/entry.py
+-rw-r--r--   0        0        0     1028 2024-05-19 15:13:06.504362 qtharmony-0.3.4/qtharmony/widgets/basic/frame.py
+-rw-r--r--   0        0        0     2872 2024-05-19 17:59:31.518295 qtharmony-0.3.4/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     3463 2024-05-19 17:59:31.518295 qtharmony-0.3.4/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0      389 2024-05-19 17:59:31.518295 qtharmony-0.3.4/qtharmony/widgets/basic/picture.py
+-rw-r--r--   0        0        0     2072 2024-05-19 15:13:06.507695 qtharmony-0.3.4/qtharmony/widgets/basic/radio_button.py
+-rw-r--r--   0        0        0     1178 2024-05-19 17:59:31.518295 qtharmony-0.3.4/qtharmony/widgets/basic/scrollbar.py
+-rw-r--r--   0        0        0     2395 2024-05-19 15:13:06.507695 qtharmony-0.3.4/qtharmony/widgets/basic/splitter.py
+-rw-r--r--   0        0        0       61 2024-05-12 07:41:31.423989 qtharmony-0.3.4/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      115 2024-05-12 06:38:54.304789 qtharmony-0.3.4/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0       63 2024-05-12 06:38:54.304789 qtharmony-0.3.4/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      147 2024-05-12 11:50:16.451713 qtharmony-0.3.4/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      108 2024-05-12 11:50:16.451713 qtharmony-0.3.4/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0        0 2024-05-12 11:50:16.451713 qtharmony-0.3.4/qtharmony/widgets/basic/styles/frame.css
+-rw-r--r--   0        0        0       60 2024-05-12 06:38:54.308122 qtharmony-0.3.4/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.3.4/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0        0 2024-05-12 06:38:54.308122 qtharmony-0.3.4/qtharmony/widgets/basic/styles/path_entry.css
+-rw-r--r--   0        0        0       67 2024-05-12 06:38:54.318122 qtharmony-0.3.4/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0      840 2024-05-19 17:59:31.518295 qtharmony-0.3.4/qtharmony/widgets/basic/styles/scrollbar.css
+-rw-r--r--   0        0        0        0 2024-05-12 07:41:31.423989 qtharmony-0.3.4/qtharmony/widgets/basic/styles/splitter.css
+-rw-r--r--   0        0        0        0 2024-05-19 17:59:31.521628 qtharmony-0.3.4/qtharmony/widgets/basic/styles/text_box.css
+-rw-r--r--   0        0        0        0 2024-05-19 15:13:06.507695 qtharmony-0.3.4/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     1703 2024-05-19 17:59:31.521628 qtharmony-0.3.4/qtharmony/widgets/basic/text_box.py
+-rw-r--r--   0        0        0     1460 2024-05-19 15:13:06.514361 qtharmony-0.3.4/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0     4047 2024-05-19 17:59:31.521628 qtharmony-0.3.4/qtharmony/widgets/custom/path_entry.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.3.4/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     2679 2024-05-14 15:55:11.677882 qtharmony-0.3.4/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.3.4/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 qtharmony-0.3.4/PKG-INFO
```

### Comparing `qtharmony-0.3.3/LICENSE` & `qtharmony-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/README.md` & `qtharmony-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/constructor/initialize.py` & `qtharmony-0.3.4/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/core/dialog.py` & `qtharmony-0.3.4/qtharmony/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/core/font.py` & `qtharmony-0.3.4/qtharmony/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/core/load.py` & `qtharmony-0.3.4/qtharmony/core/load.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/core/sizes.py` & `qtharmony-0.3.4/qtharmony/core/sizes.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/core/stylesheet.py` & `qtharmony-0.3.4/qtharmony/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/core/theme/theme_builder.py` & `qtharmony-0.3.4/qtharmony/core/theme/theme_builder.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/core/theme/theme_manager.py` & `qtharmony-0.3.4/qtharmony/core/theme/theme_manager.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/resources/themes/dark-default.json` & `qtharmony-0.3.4/qtharmony/resources/themes/dark-default.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/resources/themes/dark-green.json` & `qtharmony-0.3.4/qtharmony/resources/themes/dark-green.json`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/resources/themes/light-default.json` & `qtharmony-0.3.4/qtharmony/resources/themes/light-green.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9638227513227512%*

 * *Differences: {"'CheckBox'": "{'::indicator': {'border': '1px solid #00b300'}, '::indicator:checked:enabled': "*

 * *               "{'background-color': '#00b300'}}",*

 * * "'DigitalEntry'": "{':hover': {'border-color': '#00b300'}, ':focus': {'border-color': '#00b300'}}",*

 * * "'DropDownMenu'": "{':hover': {'border-color': '#00b300'}}",*

 * * "'Entry'": "{':hover': {'border-color': '#00b300'}, ':focus': {'border-color': '#00b300'}}",*

 * * "'Frame'": "{'': {'background-color': '#f5fff5'}}",*

 * * "'GroupBox'": "{'': {'background-color': '#f5fff5'}, […]*

```diff
@@ -1,21 +1,21 @@
 {
     "CheckBox": {
         "": {
             "color": "#333333"
         },
         "::indicator": {
-            "border": "1px solid #0166fc",
+            "border": "1px solid #00b300",
             "border-radius": "3px"
         },
         "::indicator:checked:disabled": {
             "background-color": "#d3d3d3"
         },
         "::indicator:checked:enabled": {
-            "background-color": "#0166fc"
+            "background-color": "#00b300"
         },
         "::indicator:disabled": {
             "border-color": "#a9a9a9"
         },
         ":disabled": {
             "color": "#a9a9a9"
         },
@@ -25,18 +25,18 @@
         "": {
             "background-color": "#ffffff",
             "border": "1px solid #d3d3d3",
             "border-radius": "6px",
             "color": "#333333"
         },
         ":focus": {
-            "border-color": "#405cf5"
+            "border-color": "#00b300"
         },
         ":hover": {
-            "border-color": "#6185DF"
+            "border-color": "#00b300"
         },
         "object-name": "QSpinBox#digital-entry"
     },
     "DropDownMenu": {
         "": {
             "background-color": "#ffffff",
             "border": "1px solid #d3d3d3",
@@ -50,15 +50,15 @@
             "border": "none"
         },
         ":disabled": {
             "background-color": "#d3d3d3",
             "color": "#a9a9a9"
         },
         ":hover": {
-            "border-color": "#6185DF"
+            "border-color": "#00b300"
         },
         "object-name": "QComboBox#drop-down-menu"
     },
     "Entry": {
         "": {
             "background-color": "#ffffff",
             "border": "1px solid #d3d3d3",
@@ -66,97 +66,97 @@
             "color": "#333333"
         },
         ":disabled": {
             "background-color": "#d3d3d3",
             "color": "#a9a9a9"
         },
         ":focus": {
-            "border-color": "#405cf5"
+            "border-color": "#00b300"
         },
         ":hover": {
-            "border-color": "#6185DF"
+            "border-color": "#00b300"
         },
         "object-name": "QLineEdit#entry"
     },
     "Frame": {
         "": {
-            "background-color": "#f5f5f5",
+            "background-color": "#f5fff5",
             "border": "1px solid #d3d3d3",
             "border-radius": "6px"
         },
         "object-name": "Frame#frame"
     },
     "GroupBox": {
         "": {
-            "background-color": "#f5f5f5",
+            "background-color": "#f5fff5",
             "border": "1px solid #d3d3d3",
             "border-radius": "6px"
         },
         "::title": {
-            "background-color": "#e6e6e6",
+            "background-color": "#e6ffe6",
             "border-radius": "6px",
             "color": "#333333",
-            "margin-top": "0px",
+            "margin-top": "0",
             "min-height": "30px",
             "padding-left": "20px",
             "padding-right": "20px",
             "subcontrol-position": "top"
         },
         "object-name": "QGroupBox#group-box"
     },
     "Info": {
         "author": null,
-        "name": "Light-Default"
+        "name": "Light-Green"
     },
     "Label": {
         "": {
             "color": "#333333"
         },
         "object-name": "QLabel#label"
     },
     "MainWindow": {
         "": {
-            "background-color": "#f5f5f5",
+            "background-color": "#f5fff5",
             "border": "none",
             "border-radius": "0px"
         },
         "object-name": "QMainWindow#main-window"
     },
     "PushButton": {
         "": {
-            "background-color": "#405cf5",
+            "background-color": "#00b300",
             "border": "none",
             "border-radius": "6px",
             "color": "#ffffff"
         },
         ":disabled": {
             "background-color": "#d3d3d3",
             "color": "#a9a9a9"
         },
         ":hover": {
-            "background-color": "#3045B8"
+            "background-color": "#008000"
         },
         ":pressed": {
-            "background-color": "#283A9A"
+            "background-color": "#006400"
         },
         "object-name": "QPushButton#button"
     },
     "RadioButton": {
         "": {
             "color": "#333333"
         },
         "::indicator": {
-            "border": "1px solid #0166fc",
+            "border": "1px solid #00b300",
             "border-radius": "7px"
         },
         "::indicator:checked:disabled": {
             "background-color": "#d3d3d3"
         },
         "::indicator:checked:enabled": {
-            "background-color": "#0166fc"
+            "background-color": "#00b300"
         },
         "::indicator:disabled": {
             "border-color": "#a9a9a9"
         },
         ":disabled": {
             "color": "#a9a9a9"
         },
```

### Comparing `qtharmony-0.3.3/qtharmony/resources/themes/light-green.json` & `qtharmony-0.3.4/qtharmony/resources/themes/light-default.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7520866402116403%*

 * *Differences: {"'CheckBox'": "{'::indicator': {'border': '1px solid #b0c4de'}, '::indicator:checked:enabled': "*

 * *               "{'background-color': '#b0c4de'}, '::indicator:checked:disabled': "*

 * *               "{'background-color': 'lightgray'}, ':disabled': {'color': 'gray'}, "*

 * *               "'::indicator:disabled': {'border-color': 'gray'}}",*

 * * "'DigitalEntry'": "{'': {'background-color': '#f5f5f5', 'border': '1px solid #adb5bd'}, ':hover': "*

 * *                   "{'border-color': '#b0c4de'}, ':focus': {'border-color': ' […]*

```diff
@@ -1,168 +1,209 @@
 {
     "CheckBox": {
         "": {
             "color": "#333333"
         },
         "::indicator": {
-            "border": "1px solid #00b300",
+            "border": "1px solid #b0c4de",
             "border-radius": "3px"
         },
         "::indicator:checked:disabled": {
-            "background-color": "#d3d3d3"
+            "background-color": "lightgray"
         },
         "::indicator:checked:enabled": {
-            "background-color": "#00b300"
+            "background-color": "#b0c4de"
         },
         "::indicator:disabled": {
-            "border-color": "#a9a9a9"
+            "border-color": "gray"
         },
         ":disabled": {
-            "color": "#a9a9a9"
+            "color": "gray"
         },
         "object-name": "QCheckBox#check-box"
     },
     "DigitalEntry": {
         "": {
-            "background-color": "#ffffff",
-            "border": "1px solid #d3d3d3",
+            "background-color": "#f5f5f5",
+            "border": "1px solid #adb5bd",
             "border-radius": "6px",
             "color": "#333333"
         },
         ":focus": {
-            "border-color": "#00b300"
+            "border-color": "#f0f0f0"
         },
         ":hover": {
-            "border-color": "#00b300"
+            "border-color": "#b0c4de"
         },
         "object-name": "QSpinBox#digital-entry"
     },
     "DropDownMenu": {
         "": {
-            "background-color": "#ffffff",
-            "border": "1px solid #d3d3d3",
+            "background-color": "#f5f5f5",
+            "border": "none",
             "border-radius": "6px",
             "color": "#333333"
         },
         " QAbstractItemView": {
-            "background-color": "#ffffff"
+            "background-color": "#f5f5f5"
         },
         "::drop-down": {
             "border": "none"
         },
         ":disabled": {
-            "background-color": "#d3d3d3",
-            "color": "#a9a9a9"
+            "background-color": "lightgray",
+            "color": "gray"
         },
         ":hover": {
-            "border-color": "#00b300"
+            "border-color": "#b0c4de"
         },
         "object-name": "QComboBox#drop-down-menu"
     },
     "Entry": {
         "": {
-            "background-color": "#ffffff",
-            "border": "1px solid #d3d3d3",
+            "background-color": "#f5f5f5",
+            "border": "none",
             "border-radius": "6px",
             "color": "#333333"
         },
         ":disabled": {
-            "background-color": "#d3d3d3",
-            "color": "#a9a9a9"
+            "background-color": "lightgray",
+            "color": "gray"
         },
         ":focus": {
-            "border-color": "#00b300"
+            "border-color": "#f0f0f0"
         },
         ":hover": {
-            "border-color": "#00b300"
+            "border-color": "#b0c4de"
         },
         "object-name": "QLineEdit#entry"
     },
     "Frame": {
         "": {
-            "background-color": "#f5fff5",
-            "border": "1px solid #d3d3d3",
+            "background-color": "#f0f0f0",
+            "border": "none",
             "border-radius": "6px"
         },
         "object-name": "Frame#frame"
     },
     "GroupBox": {
         "": {
-            "background-color": "#f5fff5",
-            "border": "1px solid #d3d3d3",
+            "background-color": "#f0f0f0",
+            "border": "none",
             "border-radius": "6px"
         },
         "::title": {
-            "background-color": "#e6ffe6",
+            "background-color": "#e0e0e0",
             "border-radius": "6px",
             "color": "#333333",
-            "margin-top": "0",
+            "margin-top": "5px",
             "min-height": "30px",
             "padding-left": "20px",
             "padding-right": "20px",
             "subcontrol-position": "top"
         },
         "object-name": "QGroupBox#group-box"
     },
     "Info": {
         "author": null,
-        "name": "Light-Green"
+        "name": "Light-Default"
     },
     "Label": {
         "": {
             "color": "#333333"
         },
         "object-name": "QLabel#label"
     },
     "MainWindow": {
         "": {
-            "background-color": "#f5fff5",
+            "background-color": "#f5f5f5",
             "border": "none",
             "border-radius": "0px"
         },
         "object-name": "QMainWindow#main-window"
     },
     "PushButton": {
         "": {
-            "background-color": "#00b300",
+            "background-color": "#f0f0f0",
             "border": "none",
-            "border-radius": "6px",
-            "color": "#ffffff"
+            "border-radius": "6px"
         },
         ":disabled": {
-            "background-color": "#d3d3d3",
-            "color": "#a9a9a9"
+            "background-color": "lightgray",
+            "color": "gray"
         },
         ":hover": {
-            "background-color": "#008000"
+            "background-color": "#d9d9d9"
         },
         ":pressed": {
-            "background-color": "#006400"
+            "background-color": "#c0c0c0"
         },
         "object-name": "QPushButton#button"
     },
     "RadioButton": {
         "": {
             "color": "#333333"
         },
         "::indicator": {
-            "border": "1px solid #00b300",
+            "border": "1px solid #b0c4de",
             "border-radius": "7px"
         },
         "::indicator:checked:disabled": {
-            "background-color": "#d3d3d3"
+            "background-color": "lightgray"
         },
         "::indicator:checked:enabled": {
-            "background-color": "#00b300"
+            "background-color": "#b0c4de"
         },
         "::indicator:disabled": {
-            "border-color": "#a9a9a9"
+            "border-color": "gray"
         },
         ":disabled": {
-            "color": "#a9a9a9"
+            "color": "gray"
         },
         "object-name": "QRadioButton#radio-button"
     },
+    "ScrollBar": {
+        "": {
+            "background-color": "#e0e0e0",
+            "border-radius": "4px",
+            "width": "10px"
+        },
+        "::add-page, ::sub-page": {
+            "background": "#e0e0e0",
+            "border": "none"
+        },
+        ":handle": {
+            "background-color": "#c0c0c0",
+            "border-radius": "4px"
+        },
+        ":handle:hover": {
+            "background-color": "#a0a0a0"
+        },
+        ":handle:pressed": {
+            "background-color": "#808080"
+        },
+        "object-name": "QScrollBar#scroll-bar"
+    },
     "Splitter": {
         "object-name": "QSplitter#splitter"
+    },
+    "TextBox": {
+        "": {
+            "background-color": "#e0e0e0",
+            "border-radius": "6px",
+            "color": "black",
+            "padding": "5px"
+        },
+        "object-name": "QPlainTextEdit#text-box"
+    },
+    "WidgetsList": {
+        "": {
+            "background-color": "#e0e0e0",
+            "border": "none",
+            "border-radius": "6px"
+        },
+        "::item": {
+            "min-height": "100px"
+        },
+        "object-name": "QListWidget#widgets-list"
     }
 }
```

### Comparing `qtharmony-0.3.3/qtharmony/resources/ui/Icon.png` & `qtharmony-0.3.4/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/resources/ui/Logo.png` & `qtharmony-0.3.4/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.3.4/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/__init__.py` & `qtharmony-0.3.4/qtharmony/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/button.py` & `qtharmony-0.3.4/qtharmony/widgets/basic/button.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/check_box.py` & `qtharmony-0.3.4/qtharmony/widgets/basic/check_box.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/digital_entry.py` & `qtharmony-0.3.4/qtharmony/widgets/basic/digital_entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/drop_down_menu.py` & `qtharmony-0.3.4/qtharmony/widgets/basic/drop_down_menu.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/entry.py` & `qtharmony-0.3.4/qtharmony/widgets/basic/entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/frame.py` & `qtharmony-0.3.4/qtharmony/widgets/basic/frame.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/groups.py` & `qtharmony-0.3.4/qtharmony/widgets/basic/groups.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/label.py` & `qtharmony-0.3.4/qtharmony/widgets/basic/label.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/radio_button.py` & `qtharmony-0.3.4/qtharmony/widgets/basic/radio_button.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/scrollbar.py` & `qtharmony-0.3.4/qtharmony/widgets/basic/scrollbar.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/splitter.py` & `qtharmony-0.3.4/qtharmony/widgets/basic/splitter.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/styles/scrollbar.css` & `qtharmony-0.3.4/qtharmony/widgets/basic/styles/scrollbar.css`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/text_box.py` & `qtharmony-0.3.4/qtharmony/widgets/basic/text_box.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/basic/widgets_list.py` & `qtharmony-0.3.4/qtharmony/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/widgets/custom/path_entry.py` & `qtharmony-0.3.4/qtharmony/widgets/custom/path_entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/qtharmony/windows/main_window.py` & `qtharmony-0.3.4/qtharmony/windows/main_window.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.3.3/PKG-INFO` & `qtharmony-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.3.3
+Version: 0.3.4
 Summary: 
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

