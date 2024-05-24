# Comparing `tmp/c4m_flexio-0.4.3.tar.gz` & `tmp/c4m_flexio-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_flexio-0.4.3.tar", last modified: Mon May 13 15:31:32 2024, max compression
+gzip compressed data, was "c4m_flexio-0.4.4.tar", last modified: Fri May 24 09:57:54 2024, max compression
```

## Comparing `c4m_flexio-0.4.3.tar` & `c4m_flexio-0.4.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      992 2024-04-29 12:19:56.775201 c4m_flexio-0.4.3/LICENSE.md
--rw-r--r--   0        0        0     2813 2024-05-13 15:26:22.107061 c4m_flexio-0.4.3/README.md
--rw-r--r--   0        0        0      170 2024-04-29 09:44:39.473491 c4m_flexio-0.4.3/c4m/flexio/__init__.py
--rw-r--r--   0        0        0    18938 2024-04-29 09:49:22.507719 c4m_flexio-0.4.3/c4m/flexio/_helpers.py
--rw-r--r--   0        0        0   106512 2024-05-13 14:44:22.044766 c4m_flexio-0.4.3/c4m/flexio/cell.py
--rw-r--r--   0        0        0   236164 2024-05-08 14:45:54.124023 c4m_flexio-0.4.3/c4m/flexio/factory.py
--rw-r--r--   0        0        0    37990 2024-04-29 09:49:14.995766 c4m_flexio-0.4.3/c4m/flexio/specification.py
--rw-r--r--   0        0        0      706 2024-05-13 15:31:32.425533 c4m_flexio-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     3152 1970-01-01 00:00:00.000000 c4m_flexio-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      992 2024-05-21 16:32:45.122863 c4m_flexio-0.4.4/LICENSE.md
+-rw-r--r--   0        0        0     2958 2024-05-24 09:48:44.314177 c4m_flexio-0.4.4/README.md
+-rw-r--r--   0        0        0      170 2024-05-21 16:32:45.122863 c4m_flexio-0.4.4/c4m/flexio/__init__.py
+-rw-r--r--   0        0        0    18938 2024-05-21 16:32:45.122863 c4m_flexio-0.4.4/c4m/flexio/_helpers.py
+-rw-r--r--   0        0        0   106573 2024-05-21 16:45:20.491928 c4m_flexio-0.4.4/c4m/flexio/cell.py
+-rw-r--r--   0        0        0   236164 2024-05-21 16:32:45.122863 c4m_flexio-0.4.4/c4m/flexio/factory.py
+-rw-r--r--   0        0        0    37990 2024-05-21 16:32:45.122863 c4m_flexio-0.4.4/c4m/flexio/specification.py
+-rw-r--r--   0        0        0      706 2024-05-24 09:57:54.349282 c4m_flexio-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3297 1970-01-01 00:00:00.000000 c4m_flexio-0.4.4/PKG-INFO
```

### Comparing `c4m_flexio-0.4.3/LICENSE.md` & `c4m_flexio-0.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.4.3/README.md` & `c4m_flexio-0.4.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,28 @@
+Metadata-Version: 2.1
+Name: c4m-flexio
+Version: 0.4.4
+Summary: PDKMaster based scalable IO library
+Author: Chips4Makers contributors
+License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
+Requires-Python: ~=3.8
+Requires-Dist: PDKMaster<0.12.0,>=0.10.2
+Requires-Dist: c4m-flexcell~=0.4.2
+Description-Content-Type: text/markdown
+
 # Flexible, scalable, IO library
 
 A IO library is a collection of cells that allows to do the input and output from on-chip signals to outside the chip. Typically these libraries with a fixed set of cells with a fixed layout and functionality and provided by the foundry or a third party.
 
 Purpose of c4m-flexio library is to have a library that is easily scalable between different technologies using the [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) framework. It will also be configurable to adapt the cells to one's needs.
 
 ## Release history
 
+* [v0.4.4](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.4):
+  * IOPadVdd needed another fix as a guard was wrongly connected to vdd
 * [v0.4.3](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.3):
   * Critical fix for IOPadVdd layout.
   * make this repo part of project Arrakeen; use common setup like license, DCO check etc.
 * [v0.4.2](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.2):
   Several features for IHP SG13G2 support: RCClamp in IOPadVdd, custom layout manipulation
   suport, prefix all cell names.
 * v0.4.1:
```

### Comparing `c4m_flexio-0.4.3/c4m/flexio/_helpers.py` & `c4m_flexio-0.4.4/c4m/flexio/_helpers.py`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.4.3/c4m/flexio/cell.py` & `c4m_flexio-0.4.4/c4m/flexio/cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1901,20 +1901,21 @@
             shape = _geo.Rect.from_rect(
                 rect=bb,
                 top=max(bb.top, padm2_bounds.bottom),
                 bottom=min(bb.bottom, padm2_bounds.top),
             )
             layouter.add_wire(wire=metal2, net=pad, shape=shape)
 
-            y = bb.top
-            layouter.add_wire(
-                net=pad, wire=via1, y=y,
-                bottom_left=shape.left, bottom_right=shape.right, bottom_enclosure="tall",
-                top_left=shape.left, top_right=shape.right, top_enclosure="tall",
-            )
+            if pad == nets["iovdd"]:
+                y = bb.top
+                layouter.add_wire(
+                    net=pad, wire=via1, y=y,
+                    bottom_left=shape.left, bottom_right=shape.right, bottom_enclosure="tall",
+                    top_left=shape.left, top_right=shape.right, top_enclosure="tall",
+                )
 
         # Draw guardring around pad and connect to iovdd track
         bottom = cast(_geo._Rectangular, l_nclamp.boundary).top
         top = iovdd_trackspec.bottom - comp.guardring_space
         c_guard = fab.guardring(
             type_="n", width=spec.monocell_width, height=(top - bottom),
         )
```

### Comparing `c4m_flexio-0.4.3/c4m/flexio/factory.py` & `c4m_flexio-0.4.4/c4m/flexio/factory.py`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.4.3/c4m/flexio/specification.py` & `c4m_flexio-0.4.4/c4m/flexio/specification.py`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.4.3/pyproject.toml` & `c4m_flexio-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 dependencies = [
     "PDKMaster>=0.10.2,<0.12.0",
     "c4m-flexcell~=0.4.2",
 ]
 requires-python = "~=3.8"
 readme = "README.md"
-version = "0.4.3"
+version = "0.4.4"
 
 [project.license]
 text = "GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `c4m_flexio-0.4.3/PKG-INFO` & `c4m_flexio-0.4.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,17 @@
-Metadata-Version: 2.1
-Name: c4m-flexio
-Version: 0.4.3
-Summary: PDKMaster based scalable IO library
-Author: Chips4Makers contributors
-License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
-Requires-Python: ~=3.8
-Requires-Dist: PDKMaster<0.12.0,>=0.10.2
-Requires-Dist: c4m-flexcell~=0.4.2
-Description-Content-Type: text/markdown
-
 # Flexible, scalable, IO library
 
 A IO library is a collection of cells that allows to do the input and output from on-chip signals to outside the chip. Typically these libraries with a fixed set of cells with a fixed layout and functionality and provided by the foundry or a third party.
 
 Purpose of c4m-flexio library is to have a library that is easily scalable between different technologies using the [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) framework. It will also be configurable to adapt the cells to one's needs.
 
 ## Release history
 
+* [v0.4.4](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.4):
+  * IOPadVdd needed another fix as a guard was wrongly connected to vdd
 * [v0.4.3](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.3):
   * Critical fix for IOPadVdd layout.
   * make this repo part of project Arrakeen; use common setup like license, DCO check etc.
 * [v0.4.2](https://gitlab.com/Chips4Makers/c4m-flexio/-/commits/v0.4.2):
   Several features for IHP SG13G2 support: RCClamp in IOPadVdd, custom layout manipulation
   suport, prefix all cell names.
 * v0.4.1:
```

