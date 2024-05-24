# Comparing `tmp/geodeticengine-1.0.8.tar.gz` & `tmp/geodeticengine-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodeticengine-1.0.8.tar", last modified: Mon Apr  8 06:56:32 2024, max compression
+gzip compressed data, was "geodeticengine-1.0.9.tar", last modified: Wed Apr 10 13:11:45 2024, max compression
```

## Comparing `geodeticengine-1.0.8.tar` & `geodeticengine-1.0.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      141 2024-01-31 13:29:55.000000 geodeticengine-1.0.8/.gitignore
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6830 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6263 2024-03-18 10:31:33.000000 geodeticengine-1.0.8/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      750 2024-04-08 06:51:37.000000 geodeticengine-1.0.8/pyproject.toml
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      117 2024-01-31 13:29:55.000000 geodeticengine-1.0.8/requirements.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/setup.cfg
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/src/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.514186 geodeticengine-1.0.8/src/examples/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/src/examples/data/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1313 2023-12-01 10:18:18.000000 geodeticengine-1.0.8/src/examples/data/feature.geojson
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3475 2023-12-01 10:18:18.000000 geodeticengine-1.0.8/src/examples/data/transformed_feature.geojson
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/src/geodeticengine/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2674 2024-04-08 06:50:15.000000 geodeticengine-1.0.8/src/geodeticengine/AuthBearerToken.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4342 2024-03-18 10:27:01.000000 geodeticengine-1.0.8/src/geodeticengine/CoordTrans.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      972 2024-04-08 06:50:15.000000 geodeticengine-1.0.8/src/geodeticengine/CrsSearch.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1076 2024-04-08 06:50:15.000000 geodeticengine-1.0.8/src/geodeticengine/CtSearch.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3579 2024-01-31 13:29:55.000000 geodeticengine-1.0.8/src/geodeticengine/MsalCredential.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      211 2024-04-08 06:50:15.000000 geodeticengine-1.0.8/src/geodeticengine/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4729 2024-04-08 06:50:15.000000 geodeticengine-1.0.8/src/geodeticengine/ege_api.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4839 2024-01-31 13:29:55.000000 geodeticengine-1.0.8/src/geodeticengine/utils.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/src/geodeticengine.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6830 2024-04-08 06:56:31.000000 geodeticengine-1.0.8/src/geodeticengine.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      649 2024-04-08 06:56:32.000000 geodeticengine-1.0.8/src/geodeticengine.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-04-08 06:56:31.000000 geodeticengine-1.0.8/src/geodeticengine.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       55 2024-04-08 06:56:31.000000 geodeticengine-1.0.8/src/geodeticengine.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       41 2024-04-08 06:56:31.000000 geodeticengine-1.0.8/src/geodeticengine.egg-info/top_level.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1864 2024-04-08 06:50:15.000000 geodeticengine-1.0.8/src/test_script.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-08 06:56:32.518185 geodeticengine-1.0.8/src/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     7730 2024-01-31 13:29:55.000000 geodeticengine-1.0.8/src/tests/test_CoordTrans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:11:45.671635 geodeticengine-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10982 2024-04-10 13:11:45.671635 geodeticengine-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10414 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-10 13:11:40.000000 geodeticengine-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:11:45.671635 geodeticengine-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:11:45.667635 geodeticengine-1.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/src/example_scripts.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:11:45.663635 geodeticengine-1.0.9/src/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:11:45.667635 geodeticengine-1.0.9/src/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/src/examples/data/feature.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/src/examples/data/transformed_feature.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:11:45.667635 geodeticengine-1.0.9/src/geodeticengine/
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/src/geodeticengine/AuthBearerToken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/src/geodeticengine/CoordTrans.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/src/geodeticengine/CrsSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/src/geodeticengine/CtSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/src/geodeticengine/MsalCredential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 13:11:40.000000 geodeticengine-1.0.9/src/geodeticengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/src/geodeticengine/ege_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/src/geodeticengine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:11:45.671635 geodeticengine-1.0.9/src/geodeticengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10982 2024-04-10 13:11:44.000000 geodeticengine-1.0.9/src/geodeticengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-10 13:11:45.000000 geodeticengine-1.0.9/src/geodeticengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:11:44.000000 geodeticengine-1.0.9/src/geodeticengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 13:11:44.000000 geodeticengine-1.0.9/src/geodeticengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 13:11:44.000000 geodeticengine-1.0.9/src/geodeticengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/src/test_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:11:45.667635 geodeticengine-1.0.9/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-04-10 13:11:20.000000 geodeticengine-1.0.9/src/tests/test_CoordTrans.py
```

### Comparing `geodeticengine-1.0.8/pyproject.toml` & `geodeticengine-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools","setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geodeticengine"
-version = "1.0.8"
+version = "1.0.9"
 
 description=" Library for transformation and conversion of coordinates used in Equinor."
 requires-python = ">=3.9"
 
 readme = "README.md"
 
 classifiers=[
```

### Comparing `geodeticengine-1.0.8/src/examples/data/feature.geojson` & `geodeticengine-1.0.9/src/examples/data/feature.geojson`

 * *Files identical despite different names*

### Comparing `geodeticengine-1.0.8/src/examples/data/transformed_feature.geojson` & `geodeticengine-1.0.9/src/examples/data/transformed_feature.geojson`

 * *Files identical despite different names*

### Comparing `geodeticengine-1.0.8/src/geodeticengine/AuthBearerToken.py` & `geodeticengine-1.0.9/src/geodeticengine/AuthBearerToken.py`

 * *Files identical despite different names*

### Comparing `geodeticengine-1.0.8/src/geodeticengine/CoordTrans.py` & `geodeticengine-1.0.9/src/geodeticengine/CoordTrans.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import numpy as np
 from pyproj import Transformer, network
 from geodeticengine.ege_api import EGE
 
 network.set_network_enabled(active=True)
 
 
-EGE = EGE()
-
 class CoordTrans():
     """
     Class for transforming coordinates using Equinor Geodetic Engine.
     Takes in CRS and CT info both using autority code and Equinor alias.
 
     """
     def __init__(self, crs_from:str, crs_to:str, ct_from:str=None, ct_to:str=None, points:list[float]=None):
@@ -35,15 +33,15 @@
         Validates the input parameters.
 
         Examples:
         >>> ct = CoordTrans(crs_from="ST_ED50_G4230", crs_to="EPSG:4326",  ct_from="EPSG:1612", points=[[10,60]])
         >>> ct.validate_input(ct.crs_from)
         [{'code': 4230, 'name': 'ST_ED50_G4230', 'naming_system': 'Equinor', 'authority': 'EPSG', 'uom': 'degree', 'coord_sys': 'ellipsoidal', 'type': 'geographic 2D', 'is_alias': True, 'alias': [{'name': 'ED50', 'naming_system': 'EPSG'}, {'name': 'GCS_European_1950', 'naming_system': 'ESRI'}], 'deprecations': []}]
         """
-        response = EGE.validate_input(entity).get('results')
+        response = EGE().validate_input(entity).get('results')
         if response is None:
             raise ValueError(f"{entity} is not a valid entity")
         return response
 
 
     def __strip_input(self, user_input):
         """Strips input strings"""
@@ -77,15 +75,15 @@
         crs_from = self.crs_from
         if self.ct_from:
             crs_from = f"({self.crs_from},{self.ct_from})"
 
         crs_to = self.crs_to
         if self.ct_to:
             crs_to = f"({self.crs_to},{self.ct_to})"
-        response = EGE.get_pipeline(crs_from, crs_to)
+        response = EGE().get_pipeline(crs_from, crs_to)
         return response['pipeline']
 
 
     def transform_from_pipeline(self, coordinates, pipeline) -> list:
         """
         Transform a list of points using PROJ pipeline and return a list
         of transformed coordinates.
```

### Comparing `geodeticengine-1.0.8/src/geodeticengine/CrsSearch.py` & `geodeticengine-1.0.9/src/geodeticengine/CrsSearch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from geodeticengine.ege_api import EGE
 
-EGE = EGE()
 
 class CrsSearch():
     """
     Class to query Equinor named CRSs based on polygon filter, crs types, target crs and usage scopes.
     The polygon filter must be defined with a list of WGS84 longitude, latitude coordinates.
 
     """
-    def __init__(self,types:list[str], polygon_coords:list[float], target_crs:str):
+    def __init__(self,types:list[str], target_crs:str=None,
+                 polygon_coords:list[float]=None):
         """
         Examples:
         >>> crs_search = CrsSearch(types=["bound projected","projected"], polygon_coords=[[1.278828871805691,58.07568845044884],[3.690287338364835,59.20344381800123],[2.274239008972083,60.12176489296384],[-0.1274790229401068, 59.8722761692493]], target_crs="ST_WGS84_G4326")
         """
         self.types = types
         self.polygon_coords = polygon_coords
         self.target_crs = target_crs
 
     def get_entities(self):
-        return EGE.crs_search(self.types, self.polygon_coords, self.target_crs)
+        return EGE().crs_search(self.types, self.polygon_coords, self.target_crs)
 
 if __name__ == "__main__":
     import doctest
     doctest.testmod()
```

### Comparing `geodeticengine-1.0.8/src/geodeticengine/CtSearch.py` & `geodeticengine-1.0.9/src/geodeticengine/CtSearch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from geodeticengine.ege_api import EGE
 
-EGE = EGE()
 
 class CtSearch():
     """
     Class to query Equinor named CRSs based on polygon filter, crs types, target crs and usage scopes.
     The polygon filter must be defined with a list of WGS84 longitude, latitude coordinates.
 
     """
-    def __init__(self,types:list[str], polygon_coords:list[float], source_crs:str, target_crs:str):
+    def __init__(self,types:list[str], source_crs:str=None, target_crs:str=None,
+                 polygon_coords:list[float]=None):
         """
         Examples:
         >>> ct_query = CtSearch(types=["transformation","concatenated operation"], polygon_coords=[[1.278828871805691,58.07568845044884],[3.690287338364835,59.20344381800123],[2.274239008972083,60.12176489296384],[-0.1274790229401068,59.8722761692493]], source_crs="ST_ED50_G4230", target_crs="ST_WGS84_G4326")
         """
         self.types = types
         self.polygon_coords = polygon_coords
         self.source_crs = source_crs
         self.target_crs = target_crs
 
     def get_entities(self):
-        return EGE.ct_search(self.types, self.polygon_coords, self.source_crs, self.target_crs)
+        return EGE().ct_search(self.types, self.polygon_coords, self.source_crs, self.target_crs)
 
 if __name__ == "__main__":
     import doctest
     doctest.testmod()
```

### Comparing `geodeticengine-1.0.8/src/geodeticengine/MsalCredential.py` & `geodeticengine-1.0.9/src/geodeticengine/MsalCredential.py`

 * *Files identical despite different names*

### Comparing `geodeticengine-1.0.8/src/geodeticengine/utils.py` & `geodeticengine-1.0.9/src/geodeticengine/utils.py`

 * *Files identical despite different names*

### Comparing `geodeticengine-1.0.8/src/geodeticengine.egg-info/SOURCES.txt` & `geodeticengine-1.0.9/src/geodeticengine.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 README.md
 pyproject.toml
 requirements.txt
+src/example_scripts.ipynb
 src/test_script.py
 src/examples/data/feature.geojson
 src/examples/data/transformed_feature.geojson
 src/geodeticengine/AuthBearerToken.py
 src/geodeticengine/CoordTrans.py
 src/geodeticengine/CrsSearch.py
 src/geodeticengine/CtSearch.py
```

### Comparing `geodeticengine-1.0.8/src/test_script.py` & `geodeticengine-1.0.9/src/test_script.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,12 +38,12 @@
 ct = CoordTrans(crs_from=crs_from, crs_to=crs_to, points=points)
 print(f"Transformed coordinates:{ct.transform_pointlist()}")
 
 # Get transformation pipeline
 pipeline =  ct.get_pipeline()
 print(f"Transformation pipeline: {pipeline}")
 
-#crs_query = CrsSearch(types=["bound projected","projected"], polygon_coords=[[1.278828871805691,58.07568845044884],[3.690287338364835,59.20344381800123],[2.274239008972083,60.12176489296384],[-0.1274790229401068, 59.8722761692493]], target_crs="ST_WGS84_G4326")
-#print(crs_query.get_entities())
+crs_query = CrsSearch(types=["bound projected","projected"], polygon_coords=[[1.278828871805691,58.07568845044884],[3.690287338364835,59.20344381800123],[2.274239008972083,60.12176489296384],[-0.1274790229401068, 59.8722761692493]], target_crs="ST_WGS84_G4326")
+print(crs_query.get_entities())
 
-#ct_query = CtSearch(types=["transformation","concatenated operation"], polygon_coords=[[1.278828871805691,58.07568845044884],[3.690287338364835,59.20344381800123],[2.274239008972083,60.12176489296384],[-0.1274790229401068,59.8722761692493]], source_crs="ST_ED50_G4230", target_crs="ST_WGS84_G4326")
-#print(ct_query.get_entities())
+ct_query = CtSearch(types=["transformation","concatenated operation"], polygon_coords=[[1.278828871805691,58.07568845044884],[3.690287338364835,59.20344381800123],[2.274239008972083,60.12176489296384],[-0.1274790229401068,59.8722761692493]], source_crs="ST_ED50_G4230", target_crs="ST_WGS84_G4326")
+print(ct_query.get_entities())
```

### Comparing `geodeticengine-1.0.8/src/tests/test_CoordTrans.py` & `geodeticengine-1.0.9/src/tests/test_CoordTrans.py`

 * *Files identical despite different names*

