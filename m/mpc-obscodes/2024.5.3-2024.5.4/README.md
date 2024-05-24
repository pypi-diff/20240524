# Comparing `tmp/mpc_obscodes-2024.5.3.tar.gz` & `tmp/mpc_obscodes-2024.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2024.5.3.tar", last modified: Fri May  3 02:24:06 2024, max compression
+gzip compressed data, was "mpc_obscodes-2024.5.4.tar", last modified: Sat May  4 02:22:39 2024, max compression
```

## Comparing `mpc_obscodes-2024.5.3.tar` & `mpc_obscodes-2024.5.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:24:06.184181 mpc_obscodes-2024.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-03 02:24:06.184181 mpc_obscodes-2024.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:24:06.180181 mpc_obscodes-2024.5.3/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)   254258 2024-05-03 02:24:00.000000 mpc_obscodes-2024.5.3/mpc_obscodes/obscodes_extended.json
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 02:24:00.000000 mpc_obscodes-2024.5.3/mpc_obscodes/obscodes_extended.md5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:24:06.180181 mpc_obscodes-2024.5.3/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:24:06.180181 mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-03 02:24:06.000000 mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-03 02:24:06.000000 mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:24:06.000000 mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 02:24:06.000000 mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 02:24:06.000000 mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-03 02:24:00.000000 mpc_obscodes-2024.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:24:06.184181 mpc_obscodes-2024.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:22:39.569850 mpc_obscodes-2024.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-04 02:22:39.569850 mpc_obscodes-2024.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:22:39.565850 mpc_obscodes-2024.5.4/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)   254259 2024-05-04 02:22:33.000000 mpc_obscodes-2024.5.4/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-04 02:22:33.000000 mpc_obscodes-2024.5.4/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:22:39.569850 mpc_obscodes-2024.5.4/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-04 02:22:31.000000 mpc_obscodes-2024.5.4/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:22:39.569850 mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-04 02:22:39.000000 mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-04 02:22:39.000000 mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 02:22:39.000000 mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 02:22:39.000000 mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 02:22:39.000000 mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-04 02:22:33.000000 mpc_obscodes-2024.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 02:22:39.569850 mpc_obscodes-2024.5.4/setup.cfg
```

### Comparing `mpc_obscodes-2024.5.3/PKG-INFO` & `mpc_obscodes-2024.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2024.5.3
+Version: 2024.5.4
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

### Comparing `mpc_obscodes-2024.5.3/README.md` & `mpc_obscodes-2024.5.4/README.md`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.5.3/mpc_obscodes/compare.py` & `mpc_obscodes-2024.5.4/mpc_obscodes/compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.5.3/mpc_obscodes/fetch.py` & `mpc_obscodes-2024.5.4/mpc_obscodes/fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.5.3/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2024.5.4/mpc_obscodes/obscodes_extended.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992790373906125%*

 * *Differences: {"'266'": "{'Longitude': 204.52396, 'cos': 0.941711, 'sin': 0.337239}",*

 * * "'267'": "{'Longitude': 204.5311, 'cos': 0.941718, 'sin': 0.337237}",*

 * * "'T09'": "{'Longitude': 204.52396, 'cos': 0.941711, 'sin': 0.337239}",*

 * * "'T11'": "{'Longitude': 204.52965, 'cos': 0.941734, 'sin': 0.337191}",*

 * * "'T12'": "{'Longitude': 204.53054, 'cos': 0.941733, 'sin': 0.337201}",*

 * * "'T13'": "{'Longitude': 204.52797, 'cos': 0.941707, 'sin': 0.337251}",*

 * * "'T14'": "{'Longitude': 204.5311, 'cos': 0.941718, 'sin': 0.337237}",*

 * * "'T15'":  […]*

```diff
@@ -1559,24 +1559,24 @@
     "262": {
         "Longitude": 289.26626,
         "Name": "European Southern Observatory, La Silla-DSS",
         "cos": 0.87344,
         "sin": -0.486052
     },
     "266": {
-        "Longitude": 204.52344,
+        "Longitude": 204.52396,
         "Name": "New Horizons KBO Search-Subaru",
-        "cos": 0.941701,
-        "sin": 0.337237
+        "cos": 0.941711,
+        "sin": 0.337239
     },
     "267": {
-        "Longitude": 204.53044,
+        "Longitude": 204.5311,
         "Name": "New Horizons KBO Search-CFHT",
-        "cos": 0.941705,
-        "sin": 0.337234
+        "cos": 0.941718,
+        "sin": 0.337237
     },
     "268": {
         "Longitude": 289.30803,
         "Name": "New Horizons KBO Search-Magellan/Clay",
         "cos": 0.875516,
         "sin": -0.482342
     },
@@ -12962,75 +12962,75 @@
     "T08": {
         "Longitude": 204.42395,
         "Name": "ATLAS-MLO, Mauna Loa",
         "cos": 0.94329,
         "sin": 0.332467
     },
     "T09": {
-        "Longitude": 204.52398,
+        "Longitude": 204.52396,
         "Name": "Subaru Telescope, Maunakea",
-        "cos": 0.941706,
-        "sin": 0.337237
+        "cos": 0.941711,
+        "sin": 0.337239
     },
     "T10": {
         "Longitude": 204.52241,
         "Name": "Submillimeter Array, Maunakea (SMA)",
         "cos": 0.941706,
         "sin": 0.337212
     },
     "T11": {
-        "Longitude": 204.53036,
+        "Longitude": 204.52965,
         "Name": "United Kingdom Infrared Telescope, Maunakea",
-        "cos": 0.941731,
-        "sin": 0.337198
+        "cos": 0.941734,
+        "sin": 0.337191
     },
     "T12": {
-        "Longitude": 204.53057,
+        "Longitude": 204.53054,
         "Name": "University of Hawaii 88-inch telescope, Maunakea",
-        "cos": 0.941729,
-        "sin": 0.337199
+        "cos": 0.941733,
+        "sin": 0.337201
     },
     "T13": {
-        "Longitude": 204.52771,
+        "Longitude": 204.52797,
         "Name": "NASA Infrared Telescope Facility, Maunakea",
-        "cos": 0.941691,
-        "sin": 0.337263
+        "cos": 0.941707,
+        "sin": 0.337251
     },
     "T14": {
-        "Longitude": 204.53113,
+        "Longitude": 204.5311,
         "Name": "Canada-France-Hawaii Telescope, Maunakea",
-        "cos": 0.941714,
-        "sin": 0.337236
+        "cos": 0.941718,
+        "sin": 0.337237
     },
     "T15": {
-        "Longitude": 204.53094,
+        "Longitude": 204.53093,
         "Name": "Gemini North Observatory, Maunakea",
-        "cos": 0.941727,
+        "cos": 0.941728,
         "sin": 0.337214
     },
     "T16": {
-        "Longitude": 204.5257,
+        "Longitude": 204.52526,
         "Name": "W. M. Keck Observatory, Keck 1, Maunakea",
-        "cos": 0.941703,
-        "sin": 0.33725
+        "cos": 0.941708,
+        "sin": 0.337246
     },
     "T17": {
-        "Longitude": 204.5258,
+        "Longitude": 204.52574,
         "Name": "W. M. Keck Observatory, Keck 2, Maunakea",
-        "cos": 0.9417,
+        "cos": 0.941704,
         "sin": 0.337256
     },
     "T35": {
         "Longitude": 210.3902,
         "Name": "Astronomical Society of Tahiti",
         "cos": 0.953686,
         "sin": -0.299837
     },
     "U52": {
-        "Longitude": 237.45111,
+        "Longitude": 237.451,
         "Name": "Shasta Valley Observatory, Grenada",
         "cos": 0.74924,
         "sin": 0.66027
     },
     "U53": {
         "Longitude": 237.1603,
         "Name": "Murray Hill Observatory, Beaverton",
```

### Comparing `mpc_obscodes-2024.5.3/mpc_obscodes/tests/test_compare.py` & `mpc_obscodes-2024.5.4/mpc_obscodes/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.5.3/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2024.5.4/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.5.3/mpc_obscodes/tests/test_mpc_obscodes.py` & `mpc_obscodes-2024.5.4/mpc_obscodes/tests/test_mpc_obscodes.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/PKG-INFO` & `mpc_obscodes-2024.5.4/mpc_obscodes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2024.5.3
+Version: 2024.5.4
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

### Comparing `mpc_obscodes-2024.5.3/pyproject.toml` & `mpc_obscodes-2024.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2024.05.03"
+version = "2024.05.04"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```

