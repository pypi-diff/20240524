# Comparing `tmp/FM14_transform-0.0.8.tar.gz` & `tmp/FM14_transform-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FM14_transform-0.0.8.tar", last modified: Mon Mar 25 18:38:08 2024, max compression
+gzip compressed data, was "FM14_transform-0.0.9.tar", last modified: Mon Mar 25 18:54:38 2024, max compression
```

## Comparing `FM14_transform-0.0.8.tar` & `FM14_transform-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-25 18:38:08.543088 FM14_transform-0.0.8/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       43 2024-03-13 19:22:37.000000 FM14_transform-0.0.8/MANIFEST.in
--rw-r--r--   0 alexander.thompson  (1013) alexander.thompson  (1013)      739 2024-03-25 18:38:08.542088 FM14_transform-0.0.8/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      107 2024-03-13 19:29:01.000000 FM14_transform-0.0.8/README.md
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      939 2024-03-25 18:37:56.000000 FM14_transform-0.0.8/pyproject.toml
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       37 2024-03-13 19:26:05.000000 FM14_transform-0.0.8/requirements.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2024-03-25 18:38:08.543088 FM14_transform-0.0.8/setup.cfg
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-25 18:38:08.539088 FM14_transform-0.0.8/src/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-25 18:38:08.540088 FM14_transform-0.0.8/src/FM14_transform/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-02-05 19:59:27.000000 FM14_transform-0.0.8/src/FM14_transform/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    37155 2024-03-25 18:37:36.000000 FM14_transform-0.0.8/src/FM14_transform/bufr2geojson.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    57792 2024-03-25 16:13:22.000000 FM14_transform-0.0.8/src/FM14_transform/data2bufr.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-25 18:38:08.542088 FM14_transform-0.0.8/src/FM14_transform/resources/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8740 2024-03-11 21:15:37.000000 FM14_transform-0.0.8/src/FM14_transform/resources/307090_template.json
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-07 17:12:06.000000 FM14_transform-0.0.8/src/FM14_transform/resources/__init__.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-25 18:38:08.542088 FM14_transform-0.0.8/src/FM14_transform.egg-info/
--rw-r--r--   0 alexander.thompson  (1013) alexander.thompson  (1013)      739 2024-03-25 18:38:08.000000 FM14_transform-0.0.8/src/FM14_transform.egg-info/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      496 2024-03-25 18:38:08.000000 FM14_transform-0.0.8/src/FM14_transform.egg-info/SOURCES.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2024-03-25 18:38:08.000000 FM14_transform-0.0.8/src/FM14_transform.egg-info/dependency_links.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       55 2024-03-25 18:38:08.000000 FM14_transform-0.0.8/src/FM14_transform.egg-info/entry_points.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2024-03-25 18:38:08.000000 FM14_transform-0.0.8/src/FM14_transform.egg-info/requires.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       15 2024-03-25 18:38:08.000000 FM14_transform-0.0.8/src/FM14_transform.egg-info/top_level.txt
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-25 18:54:38.244907 FM14_transform-0.0.9/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       43 2024-03-13 19:22:37.000000 FM14_transform-0.0.9/MANIFEST.in
+-rw-r--r--   0 alexander.thompson  (1013) alexander.thompson  (1013)      739 2024-03-25 18:54:38.243908 FM14_transform-0.0.9/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      107 2024-03-13 19:29:01.000000 FM14_transform-0.0.9/README.md
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      939 2024-03-25 18:54:25.000000 FM14_transform-0.0.9/pyproject.toml
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       37 2024-03-13 19:26:05.000000 FM14_transform-0.0.9/requirements.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2024-03-25 18:54:38.244907 FM14_transform-0.0.9/setup.cfg
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-25 18:54:38.240908 FM14_transform-0.0.9/src/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-25 18:54:38.241907 FM14_transform-0.0.9/src/FM14_transform/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-02-05 19:59:27.000000 FM14_transform-0.0.9/src/FM14_transform/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    37167 2024-03-25 18:54:09.000000 FM14_transform-0.0.9/src/FM14_transform/bufr2geojson.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    57792 2024-03-25 16:13:22.000000 FM14_transform-0.0.9/src/FM14_transform/data2bufr.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-25 18:54:38.243908 FM14_transform-0.0.9/src/FM14_transform/resources/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8740 2024-03-11 21:15:37.000000 FM14_transform-0.0.9/src/FM14_transform/resources/307090_template.json
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-07 17:12:06.000000 FM14_transform-0.0.9/src/FM14_transform/resources/__init__.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-25 18:54:38.243908 FM14_transform-0.0.9/src/FM14_transform.egg-info/
+-rw-r--r--   0 alexander.thompson  (1013) alexander.thompson  (1013)      739 2024-03-25 18:54:38.000000 FM14_transform-0.0.9/src/FM14_transform.egg-info/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      496 2024-03-25 18:54:38.000000 FM14_transform-0.0.9/src/FM14_transform.egg-info/SOURCES.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2024-03-25 18:54:38.000000 FM14_transform-0.0.9/src/FM14_transform.egg-info/dependency_links.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       55 2024-03-25 18:54:38.000000 FM14_transform-0.0.9/src/FM14_transform.egg-info/entry_points.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2024-03-25 18:54:38.000000 FM14_transform-0.0.9/src/FM14_transform.egg-info/requires.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       15 2024-03-25 18:54:38.000000 FM14_transform-0.0.9/src/FM14_transform.egg-info/top_level.txt
```

### Comparing `FM14_transform-0.0.8/PKG-INFO` & `FM14_transform-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FM14_transform
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for converting FM14 SYNOP MOBIL TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,SYNOP MOBIL,FM-14,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `FM14_transform-0.0.8/pyproject.toml` & `FM14_transform-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FM14_transform"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Alexander Thompson", email="alexander.thompson@noaa.gov" },
 ]
 description = "Package for converting FM14 SYNOP MOBIL TAC messages or an individual METAR message to BUFR4"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `FM14_transform-0.0.8/src/FM14_transform/bufr2geojson.py` & `FM14_transform-0.0.9/src/FM14_transform/bufr2geojson.py`

 * *Files 1% similar despite different names*

```diff
@@ -740,15 +740,15 @@
                 if ((xx >= 4) and (xx < 8)) and (key == last_key):
                     append = True
                 self.set_qualifier(fxxyyy, key, value, description,
                                    attributes, append)
             elif xx == 31:
                 pass
             else:
-                if fxxyyy == "022067":
+                if fxxyyy in ["022067", "033024"]:
                     append = False
                     self.set_qualifier(fxxyyy, key, value, description,
                                        attributes, append)
                     continue
                 if value is not None or description is not None:
                     self.get_identification()
                     metadata = self.get_qualifiers()
```

### Comparing `FM14_transform-0.0.8/src/FM14_transform/data2bufr.py` & `FM14_transform-0.0.9/src/FM14_transform/data2bufr.py`

 * *Files identical despite different names*

### Comparing `FM14_transform-0.0.8/src/FM14_transform/resources/307090_template.json` & `FM14_transform-0.0.9/src/FM14_transform/resources/307090_template.json`

 * *Files identical despite different names*

### Comparing `FM14_transform-0.0.8/src/FM14_transform.egg-info/PKG-INFO` & `FM14_transform-0.0.9/src/FM14_transform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FM14_transform
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for converting FM14 SYNOP MOBIL TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,SYNOP MOBIL,FM-14,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

