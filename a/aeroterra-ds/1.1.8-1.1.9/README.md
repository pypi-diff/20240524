# Comparing `tmp/aeroterra_ds-1.1.8.tar.gz` & `tmp/aeroterra_ds-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeroterra_ds-1.1.8.tar", last modified: Thu May 23 19:28:52 2024, max compression
+gzip compressed data, was "aeroterra_ds-1.1.9.tar", last modified: Thu May 23 20:45:57 2024, max compression
```

## Comparing `aeroterra_ds-1.1.8.tar` & `aeroterra_ds-1.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 19:28:52.501031 aeroterra_ds-1.1.8/
--rw-rw-rw-   0        0        0     1325 2024-05-23 19:28:52.500031 aeroterra_ds-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-23 18:46:51.000000 aeroterra_ds-1.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 19:28:52.501031 aeroterra_ds-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-05-23 19:28:47.000000 aeroterra_ds-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:28:52.476565 aeroterra_ds-1.1.8/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 19:28:52.485922 aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/
--rw-rw-rw-   0        0        0     1325 2024-05-23 19:28:52.000000 aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-05-23 19:28:52.000000 aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 19:28:52.000000 aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-23 19:28:52.000000 aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 19:28:52.000000 aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 19:28:52.489939 aeroterra_ds-1.1.8/src/geometry/
--rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.1.8/src/geometry/__init__.py
--rw-rw-rw-   0        0        0     4267 2024-05-23 19:28:06.000000 aeroterra_ds-1.1.8/src/geometry/change_crs.py
--rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.1.8/src/geometry/geometry.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:28:52.498042 aeroterra_ds-1.1.8/src/layers/
--rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.1.8/src/layers/__init__.py
--rw-rw-rw-   0        0        0     1720 2024-04-29 14:04:32.000000 aeroterra_ds-1.1.8/src/layers/common.py
--rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.1.8/src/layers/constants.py
--rw-rw-rw-   0        0        0     5510 2024-05-23 18:49:59.000000 aeroterra_ds-1.1.8/src/layers/fields.py
--rw-rw-rw-   0        0        0    15183 2024-05-23 19:25:30.000000 aeroterra_ds-1.1.8/src/layers/layers.py
--rw-rw-rw-   0        0        0     6691 2024-04-29 14:04:39.000000 aeroterra_ds-1.1.8/src/layers/properties.py
--rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.1.8/src/layers/symbology.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:45:57.330740 aeroterra_ds-1.1.9/
+-rw-rw-rw-   0        0        0     1325 2024-05-23 20:45:57.329400 aeroterra_ds-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-23 18:46:51.000000 aeroterra_ds-1.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 20:45:57.331774 aeroterra_ds-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-05-23 20:45:51.000000 aeroterra_ds-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:45:57.297699 aeroterra_ds-1.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 20:45:57.315473 aeroterra_ds-1.1.9/src/aeroterra_ds.egg-info/
+-rw-rw-rw-   0        0        0     1325 2024-05-23 20:45:57.000000 aeroterra_ds-1.1.9/src/aeroterra_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-05-23 20:45:57.000000 aeroterra_ds-1.1.9/src/aeroterra_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 20:45:57.000000 aeroterra_ds-1.1.9/src/aeroterra_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-23 20:45:57.000000 aeroterra_ds-1.1.9/src/aeroterra_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 20:45:57.000000 aeroterra_ds-1.1.9/src/aeroterra_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 20:45:57.319324 aeroterra_ds-1.1.9/src/geometry/
+-rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.1.9/src/geometry/__init__.py
+-rw-rw-rw-   0        0        0     4267 2024-05-23 19:28:06.000000 aeroterra_ds-1.1.9/src/geometry/change_crs.py
+-rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.1.9/src/geometry/geometry.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:45:57.326374 aeroterra_ds-1.1.9/src/layers/
+-rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.1.9/src/layers/__init__.py
+-rw-rw-rw-   0        0        0     1720 2024-04-29 14:04:32.000000 aeroterra_ds-1.1.9/src/layers/common.py
+-rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.1.9/src/layers/constants.py
+-rw-rw-rw-   0        0        0     5510 2024-05-23 18:49:59.000000 aeroterra_ds-1.1.9/src/layers/fields.py
+-rw-rw-rw-   0        0        0    14951 2024-05-23 20:45:48.000000 aeroterra_ds-1.1.9/src/layers/layers.py
+-rw-rw-rw-   0        0        0     6691 2024-04-29 14:04:39.000000 aeroterra_ds-1.1.9/src/layers/properties.py
+-rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.1.9/src/layers/symbology.py
```

### Comparing `aeroterra_ds-1.1.8/PKG-INFO` & `aeroterra_ds-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra_ds
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.1.8/README.md` & `aeroterra_ds-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.8/setup.py` & `aeroterra_ds-1.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aeroterra_ds',
-    version='1.1.8',
+    version='1.1.9',
     author='Data Science',
     author_email='aeroterra_ds@aeroterra.com',
     description='Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://example.com',
     package_dir={'': "src"},
```

### Comparing `aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/PKG-INFO` & `aeroterra_ds-1.1.9/src/aeroterra_ds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra-ds
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.1.8/src/geometry/change_crs.py` & `aeroterra_ds-1.1.9/src/geometry/change_crs.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.8/src/geometry/geometry.py` & `aeroterra_ds-1.1.9/src/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.8/src/layers/common.py` & `aeroterra_ds-1.1.9/src/layers/common.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.8/src/layers/fields.py` & `aeroterra_ds-1.1.9/src/layers/fields.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.8/src/layers/layers.py` & `aeroterra_ds-1.1.9/src/layers/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,24 +301,24 @@
     Returns a SDF
     """
     object_id_col = get_objectid_field_aux(layer)
 
     total_data = None
     if out_crs is None:
         out_crs = get_layer_crs_aux(layer)
-    new_data = layer.query(out_sr=out_crs, result_record_count=READ_BATCH, return_all_records=False).sdf
+    new_data = layer.query(out_sr=out_crs).sdf
     while len(new_data) > 0:
         if total_data is None:
             total_data = new_data.copy()
         else:
             total_data = pd.concat([total_data, new_data])
 
         last_time = new_data[object_id_col].max()
         new_where = f"{object_id_col} > {last_time}"
-        new_data = layer.query(where = new_where, out_sr=out_crs, result_record_count=READ_BATCH, return_all_records=False).sdf
+        new_data = layer.query(where = new_where, out_sr=out_crs).sdf
 
     if total_data is None:
         return create_empty_gdf_aux(layer, crs=out_crs)
 
     return total_data
 
 
@@ -391,27 +391,27 @@
     object_id_col = get_objectid_field_aux(layer)
     
     basic_where = query
     if out_fields is None:
        out_fields = "*"
 
     total_data = None
-    new_data = layer.query(where = basic_where, geometry_filter=geo_filter, out_fields=out_fields, out_sr=out_crs, result_record_count=READ_BATCH, return_all_records=False).sdf
+    new_data = layer.query(where = basic_where, geometry_filter=geo_filter, out_fields=out_fields, out_sr=out_crs).sdf
     while len(new_data) > 0:
         if total_data is None:
             total_data = new_data.copy()
         else:
             total_data = pd.concat([total_data, new_data])
 
         last_time = new_data[object_id_col].max()
         if query:
             new_where = basic_where + f" AND {object_id_col} > {last_time}"
         else:
             new_where = f"{object_id_col} > {last_time}"
-        new_data = layer.query(where = new_where, geometry_filter=geo_filter, out_fields=out_fields, out_sr=out_crs, result_record_count=READ_BATCH, return_all_records=False).sdf
+        new_data = layer.query(where = new_where, geometry_filter=geo_filter, out_fields=out_fields, out_sr=out_crs).sdf
 
     if total_data is None:
         total_data = create_empty_gdf_aux(layer, crs=out_crs)
         if isinstance(out_fields, list):
             out_fields.append("SHAPE")
             total_data = total_data[out_fields]
         total_data = total_data.rename(columns = {"SHAPE": "geometry"})
```

### Comparing `aeroterra_ds-1.1.8/src/layers/properties.py` & `aeroterra_ds-1.1.9/src/layers/properties.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.8/src/layers/symbology.py` & `aeroterra_ds-1.1.9/src/layers/symbology.py`

 * *Files identical despite different names*

