# Comparing `tmp/rangekeeper-0.6.2a0.tar.gz` & `tmp/rangekeeper-0.6.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rangekeeper-0.6.2a0.tar", max compression
+gzip compressed data, was "rangekeeper-0.6.3a0.tar", max compression
```

## Comparing `rangekeeper-0.6.2a0.tar` & `rangekeeper-0.6.3a0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rwxr-xr-x   0        0        0     1278 2024-02-21 06:49:07.991928 rangekeeper-0.6.2a0/README.md
--rwxr-xr-x   0        0        0      867 2024-03-14 12:15:17.474461 rangekeeper-0.6.2a0/pyproject.toml
--rwxr-xr-x   0        0        0     1736 2024-03-11 11:25:34.053023 rangekeeper-0.6.2a0/rangekeeper/__init__.py
--rwxr-xr-x   0        0        0     4790 2024-02-21 01:07:19.996808 rangekeeper-0.6.2a0/rangekeeper/api.py
--rwxr-xr-x   0        0        0       43 2024-02-21 01:07:10.809379 rangekeeper-0.6.2a0/rangekeeper/conftest.py
--rwxr-xr-x   0        0        0     9159 2024-02-21 01:07:19.999563 rangekeeper-0.6.2a0/rangekeeper/distribution.py
--rwxr-xr-x   0        0        0    16279 2024-03-11 12:08:10.007129 rangekeeper-0.6.2a0/rangekeeper/duration.py
--rwxr-xr-x   0        0        0      207 2024-02-21 01:07:19.999847 rangekeeper-0.6.2a0/rangekeeper/dynamics/__init__.py
--rwxr-xr-x   0        0        0     2514 2024-03-11 12:27:45.422978 rangekeeper-0.6.2a0/rangekeeper/dynamics/black_swan.py
--rwxr-xr-x   0        0        0    16156 2024-03-11 12:23:40.018905 rangekeeper-0.6.2a0/rangekeeper/dynamics/cyclicality.py
--rwxr-xr-x   0        0        0     5943 2024-03-11 12:25:48.274916 rangekeeper-0.6.2a0/rangekeeper/dynamics/market.py
--rwxr-xr-x   0        0        0     1322 2024-03-11 12:27:22.748437 rangekeeper-0.6.2a0/rangekeeper/dynamics/noise.py
--rwxr-xr-x   0        0        0     2361 2024-02-21 01:07:20.001064 rangekeeper-0.6.2a0/rangekeeper/dynamics/trend.py
--rwxr-xr-x   0        0        0     5162 2024-03-11 12:21:27.731170 rangekeeper-0.6.2a0/rangekeeper/dynamics/volatility.py
--rwxr-xr-x   0        0        0     2974 2024-02-21 01:07:20.001647 rangekeeper-0.6.2a0/rangekeeper/extrapolation.py
--rwxr-xr-x   0        0        0    25912 2024-03-14 11:45:59.787163 rangekeeper-0.6.2a0/rangekeeper/flux.py
--rwxr-xr-x   0        0        0    27073 2024-03-14 12:15:09.555973 rangekeeper-0.6.2a0/rangekeeper/graph.py
--rwxr-xr-x   0        0        0     4138 2024-02-21 01:07:20.005350 rangekeeper-0.6.2a0/rangekeeper/measure.py
--rwxr-xr-x   0        0        0      199 2024-02-21 01:07:20.005614 rangekeeper-0.6.2a0/rangekeeper/models/__init__.py
--rwxr-xr-x   0        0        0     5254 2024-03-14 11:47:43.602903 rangekeeper-0.6.2a0/rangekeeper/models/deterministic.py
--rwxr-xr-x   0        0        0     6631 2024-03-14 11:47:43.600207 rangekeeper-0.6.2a0/rangekeeper/models/flexible.py
--rwxr-xr-x   0        0        0     5499 2024-03-14 11:47:43.592934 rangekeeper-0.6.2a0/rangekeeper/models/linear.py
--rwxr-xr-x   0        0        0     6389 2024-02-21 01:07:20.007936 rangekeeper-0.6.2a0/rangekeeper/models/linear_graph.py
--rwxr-xr-x   0        0        0     5864 2024-03-14 11:47:43.613547 rangekeeper-0.6.2a0/rangekeeper/models/probabilistic.py
--rw-r--r--   0        0        0      567 2023-11-21 12:49:29.650000 rangekeeper-0.6.2a0/rangekeeper/policy.py
--rwxr-xr-x   0        0        0     7085 2024-03-11 12:20:38.716014 rangekeeper-0.6.2a0/rangekeeper/projection.py
--rwxr-xr-x   0        0        0     6862 2024-03-11 12:58:06.844097 rangekeeper-0.6.2a0/rangekeeper/segmentation.py
--rwxr-xr-x   0        0        0     1167 2024-02-21 01:19:38.324065 rangekeeper-0.6.2a0/rangekeeper/space.py
--rwxr-xr-x   0        0        0     7314 2024-03-11 12:41:13.136975 rangekeeper-0.6.2a0/rangekeeper/span.py
--rw-r--r--   0        0        0     2571 1970-01-01 00:00:00.000000 rangekeeper-0.6.2a0/PKG-INFO
+-rwxr-xr-x   0        0        0     1278 2024-03-14 12:52:33.213049 rangekeeper-0.6.3a0/README.md
+-rwxr-xr-x   0        0        0      818 2024-05-24 03:30:55.759254 rangekeeper-0.6.3a0/pyproject.toml
+-rwxr-xr-x   0        0        0     1736 2024-03-14 12:52:33.214027 rangekeeper-0.6.3a0/rangekeeper/__init__.py
+-rwxr-xr-x   0        0        0     4790 2024-03-14 12:52:33.214176 rangekeeper-0.6.3a0/rangekeeper/api.py
+-rwxr-xr-x   0        0        0       43 2024-03-14 12:52:33.214303 rangekeeper-0.6.3a0/rangekeeper/conftest.py
+-rwxr-xr-x   0        0        0     9159 2024-03-14 12:52:33.214433 rangekeeper-0.6.3a0/rangekeeper/distribution.py
+-rwxr-xr-x   0        0        0    16279 2024-03-14 12:52:33.214640 rangekeeper-0.6.3a0/rangekeeper/duration.py
+-rwxr-xr-x   0        0        0      207 2024-03-14 12:52:33.214768 rangekeeper-0.6.3a0/rangekeeper/dynamics/__init__.py
+-rwxr-xr-x   0        0        0     2514 2024-03-14 12:52:33.214969 rangekeeper-0.6.3a0/rangekeeper/dynamics/black_swan.py
+-rwxr-xr-x   0        0        0    16156 2024-03-14 12:52:33.215119 rangekeeper-0.6.3a0/rangekeeper/dynamics/cyclicality.py
+-rwxr-xr-x   0        0        0     5943 2024-03-14 12:52:33.215332 rangekeeper-0.6.3a0/rangekeeper/dynamics/market.py
+-rwxr-xr-x   0        0        0     1322 2024-03-14 12:52:33.215541 rangekeeper-0.6.3a0/rangekeeper/dynamics/noise.py
+-rwxr-xr-x   0        0        0     2361 2024-03-14 12:52:33.215737 rangekeeper-0.6.3a0/rangekeeper/dynamics/trend.py
+-rwxr-xr-x   0        0        0     5162 2024-03-14 12:52:33.215880 rangekeeper-0.6.3a0/rangekeeper/dynamics/volatility.py
+-rwxr-xr-x   0        0        0     2974 2024-03-14 12:52:33.216084 rangekeeper-0.6.3a0/rangekeeper/extrapolation.py
+-rwxr-xr-x   0        0        0    25912 2024-03-14 12:52:33.216260 rangekeeper-0.6.3a0/rangekeeper/flux.py
+-rwxr-xr-x   0        0        0    27073 2024-03-14 12:52:33.216448 rangekeeper-0.6.3a0/rangekeeper/graph.py
+-rwxr-xr-x   0        0        0     4138 2024-03-14 12:52:33.216643 rangekeeper-0.6.3a0/rangekeeper/measure.py
+-rwxr-xr-x   0        0        0      199 2024-03-14 12:52:33.216790 rangekeeper-0.6.3a0/rangekeeper/models/__init__.py
+-rwxr-xr-x   0        0        0     5254 2024-03-14 12:52:33.216980 rangekeeper-0.6.3a0/rangekeeper/models/deterministic.py
+-rwxr-xr-x   0        0        0     6631 2024-03-14 12:52:33.217147 rangekeeper-0.6.3a0/rangekeeper/models/flexible.py
+-rwxr-xr-x   0        0        0     5499 2024-03-14 12:52:33.217300 rangekeeper-0.6.3a0/rangekeeper/models/linear.py
+-rwxr-xr-x   0        0        0     6389 2024-03-14 12:52:33.217434 rangekeeper-0.6.3a0/rangekeeper/models/linear_graph.py
+-rwxr-xr-x   0        0        0     5864 2024-03-14 12:52:33.217599 rangekeeper-0.6.3a0/rangekeeper/models/probabilistic.py
+-rw-r--r--   0        0        0      567 2024-03-14 12:52:33.217760 rangekeeper-0.6.3a0/rangekeeper/policy.py
+-rwxr-xr-x   0        0        0     7085 2024-03-14 12:52:33.217896 rangekeeper-0.6.3a0/rangekeeper/projection.py
+-rwxr-xr-x   0        0        0     6862 2024-03-14 12:52:33.218062 rangekeeper-0.6.3a0/rangekeeper/segmentation.py
+-rwxr-xr-x   0        0        0     1167 2024-03-14 12:52:33.218223 rangekeeper-0.6.3a0/rangekeeper/space.py
+-rwxr-xr-x   0        0        0     7314 2024-03-14 12:52:33.218380 rangekeeper-0.6.3a0/rangekeeper/span.py
+-rw-r--r--   0        0        0     2476 1970-01-01 00:00:00.000000 rangekeeper-0.6.3a0/PKG-INFO
```

### Comparing `rangekeeper-0.6.2a0/README.md` & `rangekeeper-0.6.3a0/README.md`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/pyproject.toml` & `rangekeeper-0.6.3a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 [tool.poetry]
 name = "Rangekeeper"
-version = "0.6.2-alpha"
+version = "0.6.3-alpha"
 description = "A Python library assisting financial modelling in scenario planning, decision-making, cashflow forecasting, and the like"
 authors = ["Daniel Fink <danfink@mit.edu>"]
 license = "MPL-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
-aenum = "^3.1.15"
-matplotlib = "^3.8.3"
-pandas = "^2.2.0"
-Pint = "^0.20.1"
+matplotlib = "^3.9.0"
+pandas = "^2.2.2"
+pint = "^0.23"
 pyxirr = "^0.10.3"
-scipy = "^1.12.0"
-networkx = "^3.2.1"
+scipy = "^1.13.1"
+networkx = "^3.3"
 py-moneyed = "^3.0"
-python-dateutil = "^2.9.0"
 tabulate = "^0.9.0"
-PyYAML = "^6.0.1"
-specklepy = "^2.18.1"
-numba = "^0.59.0"
-multiprocess = "^0.70.14"
+pyyaml = "^6.0.1"
+specklepy = "^2.19.0"
+numba = "^0.59.1"
+multiprocess = "^0.70.16"
 seaborn = "^0.13.2"
 pyvis = "^0.3.2"
-plotly = "^5.19.0"
+plotly = "^5.22.0"
 mpld3 = "^0.5.10"
-pyarrow = "^15.0.0"
+pyarrow = "^16.1.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^8.1.1"
+pytest = "^8.2.1"
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rangekeeper-0.6.2a0/rangekeeper/__init__.py` & `rangekeeper-0.6.3a0/rangekeeper/__init__.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/api.py` & `rangekeeper-0.6.3a0/rangekeeper/api.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/distribution.py` & `rangekeeper-0.6.3a0/rangekeeper/distribution.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/duration.py` & `rangekeeper-0.6.3a0/rangekeeper/duration.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/dynamics/black_swan.py` & `rangekeeper-0.6.3a0/rangekeeper/dynamics/black_swan.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/dynamics/cyclicality.py` & `rangekeeper-0.6.3a0/rangekeeper/dynamics/cyclicality.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/dynamics/market.py` & `rangekeeper-0.6.3a0/rangekeeper/dynamics/market.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/dynamics/noise.py` & `rangekeeper-0.6.3a0/rangekeeper/dynamics/noise.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/dynamics/trend.py` & `rangekeeper-0.6.3a0/rangekeeper/dynamics/trend.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/dynamics/volatility.py` & `rangekeeper-0.6.3a0/rangekeeper/dynamics/volatility.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/extrapolation.py` & `rangekeeper-0.6.3a0/rangekeeper/extrapolation.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/flux.py` & `rangekeeper-0.6.3a0/rangekeeper/flux.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/graph.py` & `rangekeeper-0.6.3a0/rangekeeper/graph.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/measure.py` & `rangekeeper-0.6.3a0/rangekeeper/measure.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/models/deterministic.py` & `rangekeeper-0.6.3a0/rangekeeper/models/deterministic.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/models/flexible.py` & `rangekeeper-0.6.3a0/rangekeeper/models/flexible.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/models/linear.py` & `rangekeeper-0.6.3a0/rangekeeper/models/linear.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/models/linear_graph.py` & `rangekeeper-0.6.3a0/rangekeeper/models/linear_graph.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/models/probabilistic.py` & `rangekeeper-0.6.3a0/rangekeeper/models/probabilistic.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/policy.py` & `rangekeeper-0.6.3a0/rangekeeper/policy.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/projection.py` & `rangekeeper-0.6.3a0/rangekeeper/projection.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/segmentation.py` & `rangekeeper-0.6.3a0/rangekeeper/segmentation.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/space.py` & `rangekeeper-0.6.3a0/rangekeeper/space.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/rangekeeper/span.py` & `rangekeeper-0.6.3a0/rangekeeper/span.py`

 * *Files identical despite different names*

### Comparing `rangekeeper-0.6.2a0/PKG-INFO` & `rangekeeper-0.6.3a0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: Rangekeeper
-Version: 0.6.2a0
+Version: 0.6.3a0
 Summary: A Python library assisting financial modelling in scenario planning, decision-making, cashflow forecasting, and the like
 License: MPL-2.0
 Author: Daniel Fink
 Author-email: danfink@mit.edu
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pint (>=0.20.1,<0.21.0)
-Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
-Requires-Dist: aenum (>=3.1.15,<4.0.0)
-Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
+Requires-Dist: matplotlib (>=3.9.0,<4.0.0)
 Requires-Dist: mpld3 (>=0.5.10,<0.6.0)
-Requires-Dist: multiprocess (>=0.70.14,<0.71.0)
-Requires-Dist: networkx (>=3.2.1,<4.0.0)
-Requires-Dist: numba (>=0.59.0,<0.60.0)
-Requires-Dist: pandas (>=2.2.0,<3.0.0)
-Requires-Dist: plotly (>=5.19.0,<6.0.0)
+Requires-Dist: multiprocess (>=0.70.16,<0.71.0)
+Requires-Dist: networkx (>=3.3,<4.0)
+Requires-Dist: numba (>=0.59.1,<0.60.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: pint (>=0.23,<0.24)
+Requires-Dist: plotly (>=5.22.0,<6.0.0)
 Requires-Dist: py-moneyed (>=3.0,<4.0)
-Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
-Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
+Requires-Dist: pyarrow (>=16.1.0,<17.0.0)
 Requires-Dist: pyvis (>=0.3.2,<0.4.0)
 Requires-Dist: pyxirr (>=0.10.3,<0.11.0)
-Requires-Dist: scipy (>=1.12.0,<2.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: scipy (>=1.13.1,<2.0.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
-Requires-Dist: specklepy (>=2.18.1,<3.0.0)
+Requires-Dist: specklepy (>=2.19.0,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Rangekeeper Source
 This directory holds the source code for the Rangekeeper Library
 
 ## Installation
```

