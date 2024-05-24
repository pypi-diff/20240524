# Comparing `tmp/shift_forex_tester_data-0.1.1-py3-none-any.whl.zip` & `tmp/shift_forex_tester_data-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5515 bytes, number of entries: 11
--rw-r--r--  2.0 unx       63 b- defN 24-May-24 05:19 shiftdata/__init__.py
+Zip file size: 5551 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       63 b- defN 24-May-24 05:20 shiftdata/__init__.py
 -rw-r--r--  2.0 unx       47 b- defN 24-May-24 04:38 shiftdata/__main__.py
 -rw-r--r--  2.0 unx     1643 b- defN 24-May-24 04:38 shiftdata/_shift.py
 -rw-r--r--  2.0 unx     2385 b- defN 24-May-24 05:18 shiftdata/cli.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-24 04:38 shiftdata/py.typed
--rw-r--r--  2.0 unx     1070 b- defN 24-May-24 05:19 shift_forex_tester_data-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1817 b- defN 24-May-24 05:19 shift_forex_tester_data-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 05:19 shift_forex_tester_data-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 24-May-24 05:19 shift_forex_tester_data-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-May-24 05:19 shift_forex_tester_data-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      950 b- defN 24-May-24 05:19 shift_forex_tester_data-0.1.1.dist-info/RECORD
-11 files, 8125 bytes uncompressed, 3877 bytes compressed:  52.3%
+-rw-r--r--  2.0 unx     1070 b- defN 24-May-24 05:24 shift_forex_tester_data-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1993 b- defN 24-May-24 05:24 shift_forex_tester_data-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 05:24 shift_forex_tester_data-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 24-May-24 05:24 shift_forex_tester_data-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-May-24 05:24 shift_forex_tester_data-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      950 b- defN 24-May-24 05:24 shift_forex_tester_data-0.1.2.dist-info/RECORD
+11 files, 8301 bytes uncompressed, 3913 bytes compressed:  52.9%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: shiftdata/cli.py
 Comment: 
 
 Filename: shiftdata/py.typed
 Comment: 
 
-Filename: shift_forex_tester_data-0.1.1.dist-info/LICENSE
+Filename: shift_forex_tester_data-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: shift_forex_tester_data-0.1.1.dist-info/METADATA
+Filename: shift_forex_tester_data-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: shift_forex_tester_data-0.1.1.dist-info/WHEEL
+Filename: shift_forex_tester_data-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: shift_forex_tester_data-0.1.1.dist-info/entry_points.txt
+Filename: shift_forex_tester_data-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: shift_forex_tester_data-0.1.1.dist-info/top_level.txt
+Filename: shift_forex_tester_data-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: shift_forex_tester_data-0.1.1.dist-info/RECORD
+Filename: shift_forex_tester_data-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shiftdata/__init__.py

```diff
@@ -1,4 +1,4 @@
 from ._shift import shift_data  # noqa
 
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
```

## Comparing `shift_forex_tester_data-0.1.1.dist-info/LICENSE` & `shift_forex_tester_data-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `shift_forex_tester_data-0.1.1.dist-info/METADATA` & `shift_forex_tester_data-0.1.2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: shift-forex-tester-data
-Version: 0.1.1
+Version: 0.1.2
 Summary: Shift Forex Tester data time so that daily candle closes at the right price
-Author-email: Chew  <bachew@gmail.com>
+Project-URL: Homepage, https://github.com/bachew/shift-forex-tester-data
+Project-URL: Repository, https://github.com/bachew/shift-forex-tester-data
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs
 Requires-Dist: click
 Requires-Dist: python-dateutil
 
@@ -37,14 +38,20 @@
   --version                Show the version and exit.
   -c, --close TIME         Daily closing time  [required]
   -z, --timezone TIMEZONE  Closing time timezone  [default: America/New_York]
   --include-weekends       Do not remove Saturday and Sunday data
   -h, --help               Show this message and exit.
 ```
 
+To install:
+
+```console
+$ pip install shift-forex-tester-data
+```
+
 
 ## Development
 
 Development command:
 
 ```console
 $ bin/dev --help
```

## Comparing `shift_forex_tester_data-0.1.1.dist-info/RECORD` & `shift_forex_tester_data-0.1.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-shiftdata/__init__.py,sha256=AkLsXoomNF9NkB7ihIcvMJCRMSk6B35u4yfQj5hMC7c,63
+shiftdata/__init__.py,sha256=SxAocbb7DigfdtrDKJbyrIJc2hEuxAqm9q7FZkTuhL4,63
 shiftdata/__main__.py,sha256=BXqFnxEo8t9WOWamf1_rjjHnFTYpS4LwzTMR5tcULQ8,47
 shiftdata/_shift.py,sha256=KqRctnGhtgoerLbcSBcVSDNp0_dPkKk99ZXxqDRouSM,1643
 shiftdata/cli.py,sha256=QaKXq56AOTyBobC85b-HNNuiz4Ry6OY8z15zC1cbcTw,2385
 shiftdata/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-shift_forex_tester_data-0.1.1.dist-info/LICENSE,sha256=gioMNXTK5-bs-OjrkVcMoUysKqZFb180oo3Q0s7Qqpw,1070
-shift_forex_tester_data-0.1.1.dist-info/METADATA,sha256=3alNm4yqmC8NuSFKdXre58TwiOdElDDmX6pMzsEoTg0,1817
-shift_forex_tester_data-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-shift_forex_tester_data-0.1.1.dist-info/entry_points.txt,sha256=1nlljYJCuKfIFT1M0lOPsSpdCkrZ8yzKxi2X0hwztV8,48
-shift_forex_tester_data-0.1.1.dist-info/top_level.txt,sha256=46_AatiqqxR6sse0edYodP-AejchPpwfDxvEx8jG_NE,10
-shift_forex_tester_data-0.1.1.dist-info/RECORD,,
+shift_forex_tester_data-0.1.2.dist-info/LICENSE,sha256=gioMNXTK5-bs-OjrkVcMoUysKqZFb180oo3Q0s7Qqpw,1070
+shift_forex_tester_data-0.1.2.dist-info/METADATA,sha256=rmtvEfMoW-54I0G1XHAJPQERTdwz6q3sHkWBfsrP-nY,1993
+shift_forex_tester_data-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+shift_forex_tester_data-0.1.2.dist-info/entry_points.txt,sha256=1nlljYJCuKfIFT1M0lOPsSpdCkrZ8yzKxi2X0hwztV8,48
+shift_forex_tester_data-0.1.2.dist-info/top_level.txt,sha256=46_AatiqqxR6sse0edYodP-AejchPpwfDxvEx8jG_NE,10
+shift_forex_tester_data-0.1.2.dist-info/RECORD,,
```

