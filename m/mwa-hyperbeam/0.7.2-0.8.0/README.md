# Comparing `tmp/mwa_hyperbeam-0.7.2-cp39-cp39-manylinux_2_35_x86_64.whl.zip` & `tmp/mwa_hyperbeam-0.8.0-cp38-cp38-macosx_10_12_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1643022 bytes, number of entries: 8
--rw-r--r--  4.6 unx     2244 b- defN 24-May-14 04:01 mwa_hyperbeam-0.7.2.dist-info/METADATA
--rw-r--r--  4.6 unx      106 b- defN 24-May-14 04:01 mwa_hyperbeam-0.7.2.dist-info/WHEEL
--rw-r--r--  4.6 unx    15320 b- defN 24-May-14 04:01 mwa_hyperbeam-0.7.2.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx     2651 b- defN 24-May-14 04:01 mwa_hyperbeam-0.7.2.dist-info/license_files/LICENSE-erfa
--rw-r--r--  4.6 unx     5515 b- defN 24-May-14 04:01 mwa_hyperbeam-0.7.2.dist-info/license_files/COPYING-hdf5
--rw-r--r--  4.6 unx      135 b- defN 24-May-14 04:01 mwa_hyperbeam/__init__.py
--rwxr-xr-x  4.6 unx  4176328 b- defN 24-May-14 04:01 mwa_hyperbeam/mwa_hyperbeam.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      759 b- defN 24-May-14 04:01 mwa_hyperbeam-0.7.2.dist-info/RECORD
-8 files, 4203058 bytes uncompressed, 1641682 bytes compressed:  60.9%
+Zip file size: 1333231 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     2244 b- defN 24-May-24 06:44 mwa_hyperbeam-0.8.0.dist-info/METADATA
+-rw-r--r--  4.6 unx      104 b- defN 24-May-24 06:44 mwa_hyperbeam-0.8.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx    15320 b- defN 24-May-24 06:44 mwa_hyperbeam-0.8.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx     2651 b- defN 24-May-24 06:44 mwa_hyperbeam-0.8.0.dist-info/license_files/LICENSE-erfa
+-rw-r--r--  4.6 unx     5515 b- defN 24-May-24 06:44 mwa_hyperbeam-0.8.0.dist-info/license_files/COPYING-hdf5
+-rw-r--r--  4.6 unx      135 b- defN 24-May-24 06:44 mwa_hyperbeam/__init__.py
+-rwxr-xr-x  4.6 unx  3285632 b- defN 24-May-24 06:44 mwa_hyperbeam/mwa_hyperbeam.cpython-38-darwin.so
+-rw-r--r--  4.6 unx      749 b- defN 24-May-24 06:44 mwa_hyperbeam-0.8.0.dist-info/RECORD
+8 files, 3312350 bytes uncompressed, 1331911 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: mwa_hyperbeam-0.7.2.dist-info/METADATA
+Filename: mwa_hyperbeam-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: mwa_hyperbeam-0.7.2.dist-info/WHEEL
+Filename: mwa_hyperbeam-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: mwa_hyperbeam-0.7.2.dist-info/license_files/LICENSE
+Filename: mwa_hyperbeam-0.8.0.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: mwa_hyperbeam-0.7.2.dist-info/license_files/LICENSE-erfa
+Filename: mwa_hyperbeam-0.8.0.dist-info/license_files/LICENSE-erfa
 Comment: 
 
-Filename: mwa_hyperbeam-0.7.2.dist-info/license_files/COPYING-hdf5
+Filename: mwa_hyperbeam-0.8.0.dist-info/license_files/COPYING-hdf5
 Comment: 
 
 Filename: mwa_hyperbeam/__init__.py
 Comment: 
 
-Filename: mwa_hyperbeam/mwa_hyperbeam.cpython-39-x86_64-linux-gnu.so
+Filename: mwa_hyperbeam/mwa_hyperbeam.cpython-38-darwin.so
 Comment: 
 
-Filename: mwa_hyperbeam-0.7.2.dist-info/RECORD
+Filename: mwa_hyperbeam-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mwa_hyperbeam-0.7.2.dist-info/METADATA` & `mwa_hyperbeam-0.8.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mwa_hyperbeam
-Version: 0.7.2
+Version: 0.8.0
 Requires-Dist: numpy
 License-File: LICENSE
 License-File: LICENSE-erfa
 License-File: COPYING-hdf5
 Summary: Primary beam code for the Murchison Widefield Array (MWA) radio telescope.
 Home-Page: https://github.com/MWATelescope/mwa_hyperbeam
 Author: Christopher H. Jordan <christopherjordan87@gmail.com>, Jack L. B. Line <jack.line@curtin.edu.au>, Marcin Sokolowski <marcin.sokolowski@curtin.edu.au>, Dev Null <dev.null@curtin.edu.au
```

## Comparing `mwa_hyperbeam-0.7.2.dist-info/license_files/LICENSE` & `mwa_hyperbeam-0.8.0.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `mwa_hyperbeam-0.7.2.dist-info/license_files/LICENSE-erfa` & `mwa_hyperbeam-0.8.0.dist-info/license_files/LICENSE-erfa`

 * *Files identical despite different names*

## Comparing `mwa_hyperbeam-0.7.2.dist-info/license_files/COPYING-hdf5` & `mwa_hyperbeam-0.8.0.dist-info/license_files/COPYING-hdf5`

 * *Files identical despite different names*

## Comparing `mwa_hyperbeam-0.7.2.dist-info/RECORD` & `mwa_hyperbeam-0.8.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-mwa_hyperbeam-0.7.2.dist-info/METADATA,sha256=q0FmtOVUex2eUZEajansauq76n10iEJwhHOYnUaOXwY,2244
-mwa_hyperbeam-0.7.2.dist-info/WHEEL,sha256=9RtivweJjoiZDLVxZgJx2pt8BEU8vO9W0wI5bbL3eMQ,106
-mwa_hyperbeam-0.7.2.dist-info/license_files/LICENSE,sha256=SsQqx3BgJ-eLZ2wRa4I7PuuoDf4An8AELHC6UCBQV8o,15320
-mwa_hyperbeam-0.7.2.dist-info/license_files/LICENSE-erfa,sha256=sYWPmiY_IsQ4pFWjKUXaUaMaCuJaIQVdoTu37VfMO1E,2651
-mwa_hyperbeam-0.7.2.dist-info/license_files/COPYING-hdf5,sha256=ys-4ydiR5LBRQ5bjGfYmpV905D-ftTnuzRqlLaz4t-c,5515
+mwa_hyperbeam-0.8.0.dist-info/METADATA,sha256=eDyq5BqRaPthyDTc59Fz4d9WMMJQXL2VfNhFP6oyoZk,2244
+mwa_hyperbeam-0.8.0.dist-info/WHEEL,sha256=l7WELOTeYLkLPt92GG--_Y_8GH8Y47mJfaLTcAxZ59w,104
+mwa_hyperbeam-0.8.0.dist-info/license_files/LICENSE,sha256=SsQqx3BgJ-eLZ2wRa4I7PuuoDf4An8AELHC6UCBQV8o,15320
+mwa_hyperbeam-0.8.0.dist-info/license_files/LICENSE-erfa,sha256=sYWPmiY_IsQ4pFWjKUXaUaMaCuJaIQVdoTu37VfMO1E,2651
+mwa_hyperbeam-0.8.0.dist-info/license_files/COPYING-hdf5,sha256=ys-4ydiR5LBRQ5bjGfYmpV905D-ftTnuzRqlLaz4t-c,5515
 mwa_hyperbeam/__init__.py,sha256=3Noy2PyIXd-xOs7EiCb718Lu3xSG-2QjG9nUjfklaS4,135
-mwa_hyperbeam/mwa_hyperbeam.cpython-39-x86_64-linux-gnu.so,sha256=A2T54uBNo_6iJIvK_5RHyakS0kwWWOUbRZM8IjhLhVM,4176328
-mwa_hyperbeam-0.7.2.dist-info/RECORD,,
+mwa_hyperbeam/mwa_hyperbeam.cpython-38-darwin.so,sha256=ekjtKQfUQvbped4Qxle737r5dxPDkJ4k7w_Y1kJKcew,3285632
+mwa_hyperbeam-0.8.0.dist-info/RECORD,,
```

