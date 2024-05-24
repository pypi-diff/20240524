# Comparing `tmp/dzidb-1.2.7-py3-none-any.whl.zip` & `tmp/dzidb-1.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 28689 bytes, number of entries: 15
+Zip file size: 28809 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-22 01:16 dzidb/__init__.py
--rw-rw-rw-  2.0 fat     8700 b- defN 24-May-23 09:38 dzidb/__main__.py
+-rw-rw-rw-  2.0 fat     8948 b- defN 24-May-23 10:22 dzidb/__main__.py
 -rw-rw-rw-  2.0 fat    59153 b- defN 24-May-09 10:04 wda/__init__.py
 -rw-rw-rw-  2.0 fat     1209 b- defN 24-May-09 10:04 wda/_proto.py
 -rw-rw-rw-  2.0 fat     2393 b- defN 24-May-09 10:04 wda/exceptions.py
 -rw-rw-rw-  2.0 fat     3558 b- defN 24-May-09 10:04 wda/requests_usbmux.py
 -rw-rw-rw-  2.0 fat     7613 b- defN 24-May-09 10:04 wda/usbmux.py
 -rw-rw-rw-  2.0 fat     1348 b- defN 24-May-09 10:04 wda/utils.py
 -rw-rw-rw-  2.0 fat     1458 b- defN 24-May-09 10:04 wda/xcui_element_types.py
--rw-rw-rw-  2.0 fat     1088 b- defN 24-May-23 09:41 dzidb-1.2.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1565 b- defN 24-May-23 09:41 dzidb-1.2.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 09:41 dzidb-1.2.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       47 b- defN 24-May-23 09:41 dzidb-1.2.7.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       10 b- defN 24-May-23 09:41 dzidb-1.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1131 b- defN 24-May-23 09:41 dzidb-1.2.7.dist-info/RECORD
-15 files, 89365 bytes uncompressed, 26851 bytes compressed:  70.0%
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-May-23 10:26 dzidb-1.2.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1565 b- defN 24-May-23 10:26 dzidb-1.2.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 10:26 dzidb-1.2.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       47 b- defN 24-May-23 10:26 dzidb-1.2.8.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-23 10:26 dzidb-1.2.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1131 b- defN 24-May-23 10:26 dzidb-1.2.8.dist-info/RECORD
+15 files, 89613 bytes uncompressed, 26971 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: wda/utils.py
 Comment: 
 
 Filename: wda/xcui_element_types.py
 Comment: 
 
-Filename: dzidb-1.2.7.dist-info/LICENSE
+Filename: dzidb-1.2.8.dist-info/LICENSE
 Comment: 
 
-Filename: dzidb-1.2.7.dist-info/METADATA
+Filename: dzidb-1.2.8.dist-info/METADATA
 Comment: 
 
-Filename: dzidb-1.2.7.dist-info/WHEEL
+Filename: dzidb-1.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: dzidb-1.2.7.dist-info/entry_points.txt
+Filename: dzidb-1.2.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: dzidb-1.2.7.dist-info/top_level.txt
+Filename: dzidb-1.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: dzidb-1.2.7.dist-info/RECORD
+Filename: dzidb-1.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dzidb/__main__.py

```diff
@@ -1,9 +1,10 @@
 import argparse
 import json
+import os
 from collections import namedtuple
 
 import wda
 import tidevice
 
 
 def cmd_devices(args):
@@ -34,16 +35,20 @@
             print(f"{device['udid']}\tdevice")
     #json_result = json.dumps(result)
     #print(json_result)
 
 
 def cmd_screencap(args):
     c = wda.USBClient(args.udid)
-    filename = args.filename
-    c.screenshot().save(filename)
+    # 规范化路径，确保使用/作为分隔符
+    normalized_path = os.path.normpath(args.fileName)
+    # 使用os.path.basename()获取文件名
+    file_name = os.path.basename(normalized_path)
+    fileName = os.path.join(args.filePath, file_name)
+    c.screenshot().save(fileName)
 
 
 def cmd_input_tap(args):
     c = wda.USBClient(args.udid)
 
     # 这里x，y必须得是int
     c.click(args.x, args.y, args.duration)
@@ -84,36 +89,36 @@
          command="devices",
          flags=[
              dict(args=['-l'],
                   action='store_true',
                   help='output one entry per line')
          ],
          help="show connected iOS devices"),
-    dict(action=cmd_screencap,
+    dict(action=cmd_pull,
          command="screencap",
          flags=[
              dict(args=['-p'],
                   action='store_true',
                   help='output the screenshot in png format'),
              dict(args=['filename'],
                   metavar='FILENAME',
                   help='local output file path')
          ],
          help="capture the screen of an iOS device"),
-    dict(action=cmd_pull,
+    dict(action=cmd_screencap,
          command="pull",
          flags=[
-             dict(args=['str1'],
+             dict(args=['fileName'],
                   type=str,
                   help='useless'),
-             dict(args=['str2'],
-                  type=str,
-                  help='useless')
+             dict(args=['filePath'],
+                  metavar='FILENAME',
+                  help='local output file path')
          ],
-         help="capture the screen of an iOS device"),
+         help="useless"),
     dict(action=None,  # 顶级命令不需要动作函数
          command="input",
          subcommands=[
              dict(action=cmd_input_tap,
                   command="tap",
                   flags=[
                       dict(args=['x'],
```

## Comparing `dzidb-1.2.7.dist-info/LICENSE` & `dzidb-1.2.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dzidb-1.2.7.dist-info/METADATA` & `dzidb-1.2.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dzidb
-Version: 1.2.7
+Version: 1.2.8
 Summary: A custom adb-like tool
 Home-page: https://github.com/yourusername/dzidb
 Author: Your Name
 Author-email: your.email@example.com
 License: MIT License
 
 Copyright (c) [year] [fullname]
```

## Comparing `dzidb-1.2.7.dist-info/RECORD` & `dzidb-1.2.8.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 dzidb/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dzidb/__main__.py,sha256=k_p9yLfcToa-YHkTTIYCCICSeGR0MAF4BtfMxwJM0Vg,8700
+dzidb/__main__.py,sha256=g4ONm1fDh_J7SIRqg18xrC89aypp8odfGLzlpPfXibo,8948
 wda/__init__.py,sha256=3vJ4t3KIEt2LjeEncBW0cgEg5GEB0Epi4XqJfWZhdF0,59153
 wda/_proto.py,sha256=aB7uLSTHQrUFfjUMc5sAAOzcA3uXlvcCFHKOt1cLdHM,1209
 wda/exceptions.py,sha256=dMtuNsK6xhqa3hFyA9x3y1U-5bf9tNOaL_z6TK4Gx1E,2393
 wda/requests_usbmux.py,sha256=PjAxc58UJxlaEZXWKGaO4sNxqVOQoqhJsaut30qyvBw,3558
 wda/usbmux.py,sha256=TfjGKdEK0qjFEVjOjz-2Dy8K3O7QfRizlI1JQAJBEQQ,7613
 wda/utils.py,sha256=Kq3FQpVLOSoL60fdggDxBCPMZV0QqpKlchjx1EO8_Eo,1348
 wda/xcui_element_types.py,sha256=vO6-TpBW9SYgtPKFxYKY1nwA75HkXTUu4x0Dpb9lD8s,1458
-dzidb-1.2.7.dist-info/LICENSE,sha256=Qv2ilebwoUtMJnRsZwRy729xS5JZQzLauJ0tQzkAkTA,1088
-dzidb-1.2.7.dist-info/METADATA,sha256=YaAS7LplYW3ZshfmuLMs5Z6UuiNoiSzE21UvlJdB8IQ,1565
-dzidb-1.2.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dzidb-1.2.7.dist-info/entry_points.txt,sha256=Y-Bau_Qd8PJuVHkZakLOOGDdOuVJCXwr7pBiLwu3TAA,47
-dzidb-1.2.7.dist-info/top_level.txt,sha256=37YHSzY14b9-V1M1c7jJKJURLYPA2w9_Bgu0IuJX69Y,10
-dzidb-1.2.7.dist-info/RECORD,,
+dzidb-1.2.8.dist-info/LICENSE,sha256=Qv2ilebwoUtMJnRsZwRy729xS5JZQzLauJ0tQzkAkTA,1088
+dzidb-1.2.8.dist-info/METADATA,sha256=mLZtDLxlrcpcht98NiMRIdJzi_n5Pc7xCEIHeQEChvw,1565
+dzidb-1.2.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dzidb-1.2.8.dist-info/entry_points.txt,sha256=Y-Bau_Qd8PJuVHkZakLOOGDdOuVJCXwr7pBiLwu3TAA,47
+dzidb-1.2.8.dist-info/top_level.txt,sha256=37YHSzY14b9-V1M1c7jJKJURLYPA2w9_Bgu0IuJX69Y,10
+dzidb-1.2.8.dist-info/RECORD,,
```

