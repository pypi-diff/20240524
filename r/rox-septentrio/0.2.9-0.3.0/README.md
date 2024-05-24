# Comparing `tmp/rox_septentrio-0.2.9.tar.gz` & `tmp/rox_septentrio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rox_septentrio-0.2.9.tar", last modified: Thu May 16 14:43:07 2024, max compression
+gzip compressed data, was "rox_septentrio-0.3.0.tar", last modified: Fri May 24 12:34:18 2024, max compression
```

## Comparing `rox_septentrio-0.2.9.tar` & `rox_septentrio-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:43:07.574217 rox_septentrio-0.2.9/
--rw-rw-rw-   0 root         (0) root         (0)     1106 2024-05-16 14:42:43.000000 rox_septentrio-0.2.9/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2994 2024-05-16 14:43:07.574217 rox_septentrio-0.2.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2089 2024-05-16 14:42:43.000000 rox_septentrio-0.2.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-16 14:42:43.000000 rox_septentrio-0.2.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 14:43:07.574217 rox_septentrio-0.2.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:43:07.569217 rox_septentrio-0.2.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:43:07.572217 rox_septentrio-0.2.9/src/rox_septentrio/
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-16 14:42:43.000000 rox_septentrio-0.2.9/src/rox_septentrio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-16 14:42:43.000000 rox_septentrio-0.2.9/src/rox_septentrio/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2024-05-16 14:42:43.000000 rox_septentrio-0.2.9/src/rox_septentrio/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1773 2024-05-16 14:42:43.000000 rox_septentrio-0.2.9/src/rox_septentrio/converters.py
--rw-rw-rw-   0 root         (0) root         (0)     2214 2024-05-16 14:42:43.000000 rox_septentrio-0.2.9/src/rox_septentrio/gps_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2486 2024-05-16 14:42:43.000000 rox_septentrio-0.2.9/src/rox_septentrio/nmea.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 14:42:43.000000 rox_septentrio-0.2.9/src/rox_septentrio/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-16 14:42:43.000000 rox_septentrio-0.2.9/src/rox_septentrio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:43:07.573217 rox_septentrio-0.2.9/src/rox_septentrio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2994 2024-05-16 14:43:07.000000 rox_septentrio-0.2.9/src/rox_septentrio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      569 2024-05-16 14:43:07.000000 rox_septentrio-0.2.9/src/rox_septentrio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 14:43:07.000000 rox_septentrio-0.2.9/src/rox_septentrio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-16 14:43:07.000000 rox_septentrio-0.2.9/src/rox_septentrio.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       87 2024-05-16 14:43:07.000000 rox_septentrio-0.2.9/src/rox_septentrio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-16 14:43:07.000000 rox_septentrio-0.2.9/src/rox_septentrio.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 14:43:07.573217 rox_septentrio-0.2.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)      444 2024-05-16 14:42:43.000000 rox_septentrio-0.2.9/tests/test_messages.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-05-16 14:42:43.000000 rox_septentrio-0.2.9/tests/test_smoke.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:34:18.322800 rox_septentrio-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2994 2024-05-24 12:34:18.322800 rox_septentrio-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2089 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 12:34:18.322800 rox_septentrio-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:34:18.317800 rox_septentrio-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:34:18.319800 rox_septentrio-0.3.0/src/rox_septentrio/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2000 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/converters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/gps_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2486 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/nmea.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:34:18.321800 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2994 2024-05-24 12:34:18.000000 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      593 2024-05-24 12:34:18.000000 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 12:34:18.000000 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-24 12:34:18.000000 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2024-05-24 12:34:18.000000 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-24 12:34:18.000000 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:34:18.321800 rox_septentrio-0.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/tests/test_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/tests/test_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/tests/test_smoke.py
```

### Comparing `rox_septentrio-0.2.9/LICENCE` & `rox_septentrio-0.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.2.9/PKG-INFO` & `rox_septentrio-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rox-septentrio
-Version: 0.2.9
+Version: 0.3.0
 Summary: Driver for Septentrio GPS, posting messages to mqtt
 Author-email: Jev Kuznetsov <jev@roxautomation.com>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/roxautomation/components/septentrio-gps
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `rox_septentrio-0.2.9/README.md` & `rox_septentrio-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.2.9/pyproject.toml` & `rox_septentrio-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #-----------------pyproject.toml configuration----------------
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rox-septentrio"
-version = "0.2.9"
+version = "0.3.0"
 description = "Driver for Septentrio GPS, posting messages to mqtt"
 authors = [
     {name = "Jev Kuznetsov", email = "jev@roxautomation.com"},
 ]
 license = {text = "MIT"}
 readme = "README.md"
 classifiers = [
```

### Comparing `rox_septentrio-0.2.9/src/rox_septentrio/config.py` & `rox_septentrio-0.3.0/src/rox_septentrio/config.py`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.2.9/src/rox_septentrio/converters.py` & `rox_septentrio-0.3.0/src/rox_septentrio/converters.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,29 +24,32 @@
     h = -1j * cmath.rect(1, angle_rad)
     return degrees(-cmath.phase(h))  # type: ignore
 
 
 class GpsConverter:
     """coordinate converter (lat,lon) to (xEast,yNorth). wrapper around pymap3d"""
 
-    def __init__(self) -> None:
+    def __init__(self, gps_ref: tuple[float, float] | None = None) -> None:
         """create converter, try to get reference from GPS_REF env variable"""
-        # get gps reference from environment variable
-        var = os.environ.get("GPS_REF")
-        if var is None:
-            gps_ref = (51.0, 6.0)
-            warnings.warn(
-                f"GPS_REF environment variable not set, using default {gps_ref}"
-            )
+        if gps_ref is not None:
+            self.gps_ref = gps_ref
         else:
-            gps_ref = tuple(float(x) for x in var.split(","))  # type: ignore
-            if len(gps_ref) != 2:
-                raise ValueError(f"invalid GPS_REF: {var}")
+            # get gps reference from environment variable
+            var = os.environ.get("GPS_REF")
+            if var is None:  # not set, use default fallback.
+                new_gps_ref = (51.0, 6.0)
+                warnings.warn(
+                    f"GPS_REF environment variable not set, using default {new_gps_ref}"
+                )
+            else:
+                new_gps_ref = tuple(float(x) for x in var.split(","))  # type: ignore
+                if len(new_gps_ref) != 2:
+                    raise ValueError(f"invalid GPS_REF: {var}")
 
-        self.gps_ref = gps_ref
+            self.gps_ref = new_gps_ref
 
     def latlon_to_enu(self, latlon: Tuple[float, float]) -> Tuple[float, float]:
         x, y, _ = geodetic2enu(
             latlon[0], latlon[1], 0, self.gps_ref[0], self.gps_ref[1], 0
         )
         return float(x), float(y)
```

### Comparing `rox_septentrio-0.2.9/src/rox_septentrio/gps_node.py` & `rox_septentrio-0.3.0/src/rox_septentrio/gps_node.py`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.2.9/src/rox_septentrio/nmea.py` & `rox_septentrio-0.3.0/src/rox_septentrio/nmea.py`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.2.9/src/rox_septentrio.egg-info/PKG-INFO` & `rox_septentrio-0.3.0/src/rox_septentrio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rox-septentrio
-Version: 0.2.9
+Version: 0.3.0
 Summary: Driver for Septentrio GPS, posting messages to mqtt
 Author-email: Jev Kuznetsov <jev@roxautomation.com>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/roxautomation/components/septentrio-gps
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `rox_septentrio-0.2.9/src/rox_septentrio.egg-info/SOURCES.txt` & `rox_septentrio-0.3.0/src/rox_septentrio.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,9 +11,10 @@
 src/rox_septentrio/version.py
 src/rox_septentrio.egg-info/PKG-INFO
 src/rox_septentrio.egg-info/SOURCES.txt
 src/rox_septentrio.egg-info/dependency_links.txt
 src/rox_septentrio.egg-info/entry_points.txt
 src/rox_septentrio.egg-info/requires.txt
 src/rox_septentrio.egg-info/top_level.txt
+tests/test_converter.py
 tests/test_messages.py
 tests/test_smoke.py
```

