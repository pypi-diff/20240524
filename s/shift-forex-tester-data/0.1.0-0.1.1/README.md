# Comparing `tmp/shift_forex_tester_data-0.1.0-py3-none-any.whl.zip` & `tmp/shift_forex_tester_data-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5467 bytes, number of entries: 11
--rw-rw-r--  2.0 unx       63 b- defN 24-May-05 04:36 shiftdata/__init__.py
--rw-rw-r--  2.0 unx       47 b- defN 24-May-05 04:11 shiftdata/__main__.py
--rw-rw-r--  2.0 unx     1643 b- defN 24-May-05 04:44 shiftdata/_shift.py
--rw-rw-r--  2.0 unx     2337 b- defN 24-May-05 04:48 shiftdata/cli.py
--rw-rw-r--  2.0 unx        0 b- defN 24-May-05 04:11 shiftdata/py.typed
--rw-rw-r--  2.0 unx     1070 b- defN 24-May-05 05:07 shift_forex_tester_data-0.1.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1658 b- defN 24-May-05 05:07 shift_forex_tester_data-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-05 05:07 shift_forex_tester_data-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 24-May-05 05:07 shift_forex_tester_data-0.1.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 24-May-05 05:07 shift_forex_tester_data-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      950 b- defN 24-May-05 05:07 shift_forex_tester_data-0.1.0.dist-info/RECORD
-11 files, 7918 bytes uncompressed, 3829 bytes compressed:  51.6%
+Zip file size: 5515 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       63 b- defN 24-May-24 05:19 shiftdata/__init__.py
+-rw-r--r--  2.0 unx       47 b- defN 24-May-24 04:38 shiftdata/__main__.py
+-rw-r--r--  2.0 unx     1643 b- defN 24-May-24 04:38 shiftdata/_shift.py
+-rw-r--r--  2.0 unx     2385 b- defN 24-May-24 05:18 shiftdata/cli.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 04:38 shiftdata/py.typed
+-rw-r--r--  2.0 unx     1070 b- defN 24-May-24 05:19 shift_forex_tester_data-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1817 b- defN 24-May-24 05:19 shift_forex_tester_data-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 05:19 shift_forex_tester_data-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 24-May-24 05:19 shift_forex_tester_data-0.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-May-24 05:19 shift_forex_tester_data-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      950 b- defN 24-May-24 05:19 shift_forex_tester_data-0.1.1.dist-info/RECORD
+11 files, 8125 bytes uncompressed, 3877 bytes compressed:  52.3%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: shiftdata/cli.py
 Comment: 
 
 Filename: shiftdata/py.typed
 Comment: 
 
-Filename: shift_forex_tester_data-0.1.0.dist-info/LICENSE
+Filename: shift_forex_tester_data-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: shift_forex_tester_data-0.1.0.dist-info/METADATA
+Filename: shift_forex_tester_data-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: shift_forex_tester_data-0.1.0.dist-info/WHEEL
+Filename: shift_forex_tester_data-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: shift_forex_tester_data-0.1.0.dist-info/entry_points.txt
+Filename: shift_forex_tester_data-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: shift_forex_tester_data-0.1.0.dist-info/top_level.txt
+Filename: shift_forex_tester_data-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: shift_forex_tester_data-0.1.0.dist-info/RECORD
+Filename: shift_forex_tester_data-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shiftdata/__init__.py

```diff
@@ -1,4 +1,4 @@
 from ._shift import shift_data  # noqa
 
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
```

## shiftdata/cli.py

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from . import __version__
 from ._shift import shift_data
 from click import argument, command, option
 from functools import wraps
 from datetime import time, tzinfo
 from pathlib import Path
 import click
@@ -50,15 +51,15 @@
 @option('-c', '--close', 'closing_time', required=True, type=CliTypes.time, help='Daily closing time')
 @option('-z', '--timezone', default='America/New_York', type=CliTypes.timezone, help='Closing time timezone')
 @option('--include-weekends', is_flag=True, default=False, help='Do not remove Saturday and Sunday data')
 @argument('input_file', type=Path)
 @argument('output_file', type=Path)
 def cli(closing_time, timezone, include_weekends, input_file, output_file):
     '''
-    Shift data time so that daily candle closes with price at CLOSING_TIME.
+    Shift Forex Tester data time so that daily candle closes with price at CLOSING_TIME.
 
     INPUT_FILE is Forex Tester exported data with defaut settings,
     OUTPUT_FILE has the same format and can be imported back into
     Forex Tester with default settings.
 
     Example:
```

## Comparing `shift_forex_tester_data-0.1.0.dist-info/LICENSE` & `shift_forex_tester_data-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `shift_forex_tester_data-0.1.0.dist-info/METADATA` & `shift_forex_tester_data-0.1.1.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: shift-forex-tester-data
-Version: 0.1.0
+Version: 0.1.1
+Summary: Shift Forex Tester data time so that daily candle closes at the right price
 Author-email: Chew  <bachew@gmail.com>
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs
 Requires-Dist: click
 Requires-Dist: python-dateutil
 
 # Shift Forex Tester data
 
 ```
 $ pip install shift-forex-tester-data
 $ shiftdata --help
 Usage: shiftdata [OPTIONS] INPUT_FILE OUTPUT_FILE
 
-  Shift data time so that daily candle closes with price at CLOSING_TIME.
+  Shift Forex Tester data time so that daily candle closes with price at daily closing time.
 
   INPUT_FILE is Forex Tester exported data with defaut settings, OUTPUT_FILE
   has the same format and can be imported back into Forex Tester with default
   settings.
 
   Example:
 
@@ -58,13 +59,19 @@
 
 To lint code:
 
 ```console
 $ dev lint
 ```
 
+To run unit test:
+
+```console
+$ bin/dev run pytest
+```
+
 To build library and upload to PyPI:
 
 ```console
 $ dev build
 $ dev upload
 ```
```

## Comparing `shift_forex_tester_data-0.1.0.dist-info/RECORD` & `shift_forex_tester_data-0.1.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-shiftdata/__init__.py,sha256=m3ov98Hw4bfhoEnfhyN_cnNXbWDJL07EKZt0oao3_F8,63
+shiftdata/__init__.py,sha256=AkLsXoomNF9NkB7ihIcvMJCRMSk6B35u4yfQj5hMC7c,63
 shiftdata/__main__.py,sha256=BXqFnxEo8t9WOWamf1_rjjHnFTYpS4LwzTMR5tcULQ8,47
 shiftdata/_shift.py,sha256=KqRctnGhtgoerLbcSBcVSDNp0_dPkKk99ZXxqDRouSM,1643
-shiftdata/cli.py,sha256=Cpow17hxYrEhzumQHXcvjPqPrRVIZFK1f_3KAOLgjzo,2337
+shiftdata/cli.py,sha256=QaKXq56AOTyBobC85b-HNNuiz4Ry6OY8z15zC1cbcTw,2385
 shiftdata/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-shift_forex_tester_data-0.1.0.dist-info/LICENSE,sha256=gioMNXTK5-bs-OjrkVcMoUysKqZFb180oo3Q0s7Qqpw,1070
-shift_forex_tester_data-0.1.0.dist-info/METADATA,sha256=Kt9VpXuoF1pn0HHwDUsqGlqqMRFoeMh9lJXanFCcnhs,1658
-shift_forex_tester_data-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-shift_forex_tester_data-0.1.0.dist-info/entry_points.txt,sha256=1nlljYJCuKfIFT1M0lOPsSpdCkrZ8yzKxi2X0hwztV8,48
-shift_forex_tester_data-0.1.0.dist-info/top_level.txt,sha256=46_AatiqqxR6sse0edYodP-AejchPpwfDxvEx8jG_NE,10
-shift_forex_tester_data-0.1.0.dist-info/RECORD,,
+shift_forex_tester_data-0.1.1.dist-info/LICENSE,sha256=gioMNXTK5-bs-OjrkVcMoUysKqZFb180oo3Q0s7Qqpw,1070
+shift_forex_tester_data-0.1.1.dist-info/METADATA,sha256=3alNm4yqmC8NuSFKdXre58TwiOdElDDmX6pMzsEoTg0,1817
+shift_forex_tester_data-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+shift_forex_tester_data-0.1.1.dist-info/entry_points.txt,sha256=1nlljYJCuKfIFT1M0lOPsSpdCkrZ8yzKxi2X0hwztV8,48
+shift_forex_tester_data-0.1.1.dist-info/top_level.txt,sha256=46_AatiqqxR6sse0edYodP-AejchPpwfDxvEx8jG_NE,10
+shift_forex_tester_data-0.1.1.dist-info/RECORD,,
```

