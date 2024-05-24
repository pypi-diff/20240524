# Comparing `tmp/statsforecast-1.7.4.tar.gz` & `tmp/statsforecast-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statsforecast-1.7.4.tar", last modified: Mon Apr  8 16:44:27 2024, max compression
+gzip compressed data, was "statsforecast-1.7.5.tar", last modified: Fri May 24 17:17:45 2024, max compression
```

## Comparing `statsforecast-1.7.4.tar` & `statsforecast-1.7.5.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:27.718387 statsforecast-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-08 16:44:21.000000 statsforecast-1.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-08 16:44:21.000000 statsforecast-1.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    27435 2024-04-08 16:44:27.718387 statsforecast-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24960 2024-04-08 16:44:21.000000 statsforecast-1.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:27.710387 statsforecast-1.7.4/action_files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/test_fit_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/test_ray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/test_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-08 16:44:21.000000 statsforecast-1.7.4/action_files/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-08 16:44:21.000000 statsforecast-1.7.4/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:44:27.718387 statsforecast-1.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-08 16:44:21.000000 statsforecast-1.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:27.710387 statsforecast-1.7.4/statsforecast/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    99387 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/_modidx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:27.714387 statsforecast-1.7.4/statsforecast/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/adapters/prophet.py
--rw-r--r--   0 runner    (1001) docker     (127)    85815 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/arima.py
--rw-r--r--   0 runner    (1001) docker     (127)    22508 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/ces.py
--rw-r--r--   0 runner    (1001) docker     (127)    61494 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:27.714387 statsforecast-1.7.4/statsforecast/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16721 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/distributed/fugue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/distributed/multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    48393 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/ets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/garch.py
--rw-r--r--   0 runner    (1001) docker     (127)   212642 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/mstl.py
--rw-r--r--   0 runner    (1001) docker     (127)    29166 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/tbats.py
--rw-r--r--   0 runner    (1001) docker     (127)    20374 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/theta.py
--rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-04-08 16:44:21.000000 statsforecast-1.7.4/statsforecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:44:27.714387 statsforecast-1.7.4/statsforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27435 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 16:44:27.000000 statsforecast-1.7.4/statsforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:17:45.094132 statsforecast-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-24 17:17:40.000000 statsforecast-1.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-24 17:17:40.000000 statsforecast-1.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    27519 2024-05-24 17:17:45.094132 statsforecast-1.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24960 2024-05-24 17:17:40.000000 statsforecast-1.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:17:45.082132 statsforecast-1.7.5/action_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 17:17:40.000000 statsforecast-1.7.5/action_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-24 17:17:40.000000 statsforecast-1.7.5/action_files/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-24 17:17:40.000000 statsforecast-1.7.5/action_files/imports_with_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-24 17:17:40.000000 statsforecast-1.7.5/action_files/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-24 17:17:40.000000 statsforecast-1.7.5/action_files/test_fit_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-24 17:17:40.000000 statsforecast-1.7.5/action_files/test_ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-24 17:17:40.000000 statsforecast-1.7.5/action_files/test_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-24 17:17:40.000000 statsforecast-1.7.5/action_files/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-24 17:17:41.000000 statsforecast-1.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-24 17:17:41.000000 statsforecast-1.7.5/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 17:17:45.094132 statsforecast-1.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-24 17:17:41.000000 statsforecast-1.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:17:45.086132 statsforecast-1.7.5/statsforecast/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103565 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/_modidx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:17:45.090132 statsforecast-1.7.5/statsforecast/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/adapters/prophet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85908 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/arima.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22509 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/ces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63258 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:17:45.090132 statsforecast-1.7.5/statsforecast/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16721 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/distributed/fugue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/distributed/multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48363 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/ets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/garch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28079 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/mfles.py
+-rw-r--r--   0 runner    (1001) docker     (127)   237388 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/mstl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29029 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/tbats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/theta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-05-24 17:17:41.000000 statsforecast-1.7.5/statsforecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:17:45.090132 statsforecast-1.7.5/statsforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27519 2024-05-24 17:17:45.000000 statsforecast-1.7.5/statsforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-24 17:17:45.000000 statsforecast-1.7.5/statsforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:17:45.000000 statsforecast-1.7.5/statsforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-24 17:17:45.000000 statsforecast-1.7.5/statsforecast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:17:44.000000 statsforecast-1.7.5/statsforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-24 17:17:45.000000 statsforecast-1.7.5/statsforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 17:17:45.000000 statsforecast-1.7.5/statsforecast.egg-info/top_level.txt
```

### Comparing `statsforecast-1.7.4/LICENSE` & `statsforecast-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/PKG-INFO` & `statsforecast-1.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statsforecast
-Version: 1.7.4
+Version: 1.7.5
 Summary: Time series forecasting suite using statistical models
 Home-page: https://github.com/Nixtla/statsforecast/
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series forecasting arima ets
 Classifier: Development Status :: 3 - Alpha
@@ -15,45 +15,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloudpickle
-Requires-Dist: coreforecast>=0.0.7
+Requires-Dist: coreforecast>=0.0.9
 Requires-Dist: numba>=0.55.0
 Requires-Dist: numpy>=1.21.6
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: statsmodels>=0.13.2
 Requires-Dist: tqdm
 Requires-Dist: fugue>=0.8.1
-Requires-Dist: utilsforecast>=0.0.24
+Requires-Dist: utilsforecast>=0.1.4
 Requires-Dist: threadpoolctl
 Provides-Extra: dev
 Requires-Dist: pmdarima; extra == "dev"
-Requires-Dist: fugue[ray]>=0.8.1; extra == "dev"
+Requires-Dist: pyarrow; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: scikit-learn; extra == "dev"
+Requires-Dist: fugue[spark]>=0.8.1; extra == "dev"
+Requires-Dist: ray<2.8; extra == "dev"
+Requires-Dist: pandas[plot]; extra == "dev"
+Requires-Dist: datasetsforecast; extra == "dev"
 Requires-Dist: nbdev_plotly; extra == "dev"
-Requires-Dist: plotly-resampler; extra == "dev"
-Requires-Dist: polars; extra == "dev"
-Requires-Dist: plotly; extra == "dev"
-Requires-Dist: pyarrow; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: nbdev; extra == "dev"
-Requires-Dist: protobuf<4.0.0,>=3.15.3; extra == "dev"
-Requires-Dist: fugue[dask]>=0.8.1; extra == "dev"
+Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
+Requires-Dist: setuptools<70; extra == "dev"
 Requires-Dist: prophet; extra == "dev"
-Requires-Dist: datasetsforecast; extra == "dev"
+Requires-Dist: protobuf<4.0.0,>=3.15.3; extra == "dev"
+Requires-Dist: fugue[ray]>=0.8.1; extra == "dev"
 Requires-Dist: supersmoother; extra == "dev"
-Requires-Dist: pandas[plot]; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: ray<2.8; extra == "dev"
-Requires-Dist: fugue[spark]>=0.8.1; extra == "dev"
+Requires-Dist: fugue[dask]>=0.8.1; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
+Requires-Dist: plotly; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: plotly-resampler; extra == "dev"
+Requires-Dist: polars; extra == "dev"
 Provides-Extra: dask
 Requires-Dist: fugue[dask]>=0.8.1; extra == "dask"
 Provides-Extra: ray
 Requires-Dist: fugue[ray]>=0.8.1; extra == "ray"
 Requires-Dist: protobuf<4.0.0,>=3.15.3; extra == "ray"
 Requires-Dist: ray<2.8; extra == "ray"
 Provides-Extra: spark
```

### Comparing `statsforecast-1.7.4/README.md` & `statsforecast-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/action_files/conftest.py` & `statsforecast-1.7.5/action_files/conftest.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/action_files/test_dask.py` & `statsforecast-1.7.5/action_files/test_dask.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/action_files/test_fit_predict.py` & `statsforecast-1.7.5/action_files/test_fit_predict.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/action_files/test_ray.py` & `statsforecast-1.7.5/action_files/test_ray.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/action_files/test_spark.py` & `statsforecast-1.7.5/action_files/test_spark.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/action_files/utils.py` & `statsforecast-1.7.5/action_files/utils.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/settings.ini` & `statsforecast-1.7.5/settings.ini`

 * *Files 17% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 user = Nixtla
 description = Time series forecasting suite using statistical models
 keywords = time-series forecasting arima ets 
 author = Nixtla
 author_email = business@nixtla.io
 copyright = Nixtla Inc.
 branch = main
-version = 1.7.4
+version = 1.7.5
 min_python = 3.8
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 2
-requirements = cloudpickle coreforecast>=0.0.7 numba>=0.55.0 numpy>=1.21.6 pandas>=1.3.5 scipy>=1.7.3 statsmodels>=0.13.2 tqdm fugue>=0.8.1 utilsforecast>=0.0.24 threadpoolctl
+requirements = cloudpickle coreforecast>=0.0.9 numba>=0.55.0 numpy>=1.21.6 pandas>=1.3.5 scipy>=1.7.3 statsmodels>=0.13.2 tqdm fugue>=0.8.1 utilsforecast>=0.1.4 threadpoolctl
 polars_requirements = polars
 ray_requirements = fugue[ray]>=0.8.1 protobuf>=3.15.3,<4.0.0 ray<2.8
 dask_requirements = fugue[dask]>=0.8.1
 spark_requirements = fugue[spark]>=0.8.1
 plotly_requirements = plotly plotly-resampler
-dev_requirements = nbdev black mypy flake8 pandas[plot] pmdarima prophet pyarrow scikit-learn datasetsforecast supersmoother nbdev_plotly
+dev_requirements = nbdev black mypy pandas[plot] pmdarima prophet pyarrow ruff scikit-learn setuptools<70 datasetsforecast supersmoother nbdev_plotly pre-commit
 nbs_path = nbs
 doc_path = _docs
 recursive = True
 doc_host =  https://%(user)s.github.io
 doc_baseurl = /%(lib_name)s/
 git_url = https://github.com/%(user)s/statsforecast/
 lib_path = %(lib_name)s
```

### Comparing `statsforecast-1.7.4/setup.py` & `statsforecast-1.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/statsforecast/_modidx.py` & `statsforecast-1.7.5/statsforecast/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,24 @@
             'statsforecast.core': { 'statsforecast.core.GroupedArray': ('src/core/core.html#groupedarray', 'statsforecast/core.py'),
                                     'statsforecast.core.GroupedArray.__eq__': ( 'src/core/core.html#groupedarray.__eq__',
                                                                                 'statsforecast/core.py'),
                                     'statsforecast.core.GroupedArray._get_cols': ( 'src/core/core.html#groupedarray._get_cols',
                                                                                    'statsforecast/core.py'),
                                     'statsforecast.core.GroupedArray._output_fcst': ( 'src/core/core.html#groupedarray._output_fcst',
                                                                                       'statsforecast/core.py'),
+                                    'statsforecast.core.GroupedArray._single_threaded_cross_validation': ( 'src/core/core.html#groupedarray._single_threaded_cross_validation',
+                                                                                                           'statsforecast/core.py'),
+                                    'statsforecast.core.GroupedArray._single_threaded_fit': ( 'src/core/core.html#groupedarray._single_threaded_fit',
+                                                                                              'statsforecast/core.py'),
+                                    'statsforecast.core.GroupedArray._single_threaded_fit_predict': ( 'src/core/core.html#groupedarray._single_threaded_fit_predict',
+                                                                                                      'statsforecast/core.py'),
+                                    'statsforecast.core.GroupedArray._single_threaded_forecast': ( 'src/core/core.html#groupedarray._single_threaded_forecast',
+                                                                                                   'statsforecast/core.py'),
+                                    'statsforecast.core.GroupedArray._single_threaded_predict': ( 'src/core/core.html#groupedarray._single_threaded_predict',
+                                                                                                  'statsforecast/core.py'),
                                     'statsforecast.core.GroupedArray.cross_validation': ( 'src/core/core.html#groupedarray.cross_validation',
                                                                                           'statsforecast/core.py'),
                                     'statsforecast.core.GroupedArray.fit': ('src/core/core.html#groupedarray.fit', 'statsforecast/core.py'),
                                     'statsforecast.core.GroupedArray.fit_predict': ( 'src/core/core.html#groupedarray.fit_predict',
                                                                                      'statsforecast/core.py'),
                                     'statsforecast.core.GroupedArray.forecast': ( 'src/core/core.html#groupedarray.forecast',
                                                                                   'statsforecast/core.py'),
@@ -266,161 +276,193 @@
             'statsforecast.garch': { 'statsforecast.garch.garch_cons': ('src/garch.html#garch_cons', 'statsforecast/garch.py'),
                                      'statsforecast.garch.garch_forecast': ('src/garch.html#garch_forecast', 'statsforecast/garch.py'),
                                      'statsforecast.garch.garch_loglik': ('src/garch.html#garch_loglik', 'statsforecast/garch.py'),
                                      'statsforecast.garch.garch_model': ('src/garch.html#garch_model', 'statsforecast/garch.py'),
                                      'statsforecast.garch.garch_sigma2': ('src/garch.html#garch_sigma2', 'statsforecast/garch.py'),
                                      'statsforecast.garch.generate_garch_data': ( 'src/garch.html#generate_garch_data',
                                                                                   'statsforecast/garch.py')},
+            'statsforecast.mfles': { 'statsforecast.mfles.MFLES': ('src/mfles.html#mfles', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.MFLES.__init__': ('src/mfles.html#mfles.__init__', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.MFLES.fit': ('src/mfles.html#mfles.fit', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.MFLES.optimize': ('src/mfles.html#mfles.optimize', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.MFLES.predict': ('src/mfles.html#mfles.predict', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.MFLES.seasonal_decompose': ( 'src/mfles.html#mfles.seasonal_decompose',
+                                                                                       'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.OLS': ('src/mfles.html#ols', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.OLS.fit': ('src/mfles.html#ols.fit', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.OLS.predict': ('src/mfles.html#ols.predict', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.Zeros': ('src/mfles.html#zeros', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.Zeros.predict': ('src/mfles.html#zeros.predict', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles._ols': ('src/mfles.html#_ols', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.calc_cov': ('src/mfles.html#calc_cov', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.calc_mae': ('src/mfles.html#calc_mae', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.calc_mape': ('src/mfles.html#calc_mape', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.calc_mse': ('src/mfles.html#calc_mse', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.calc_rsq': ('src/mfles.html#calc_rsq', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.calc_seas_strength': ( 'src/mfles.html#calc_seas_strength',
+                                                                                 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.calc_smape': ('src/mfles.html#calc_smape', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.calc_trend_strength': ( 'src/mfles.html#calc_trend_strength',
+                                                                                  'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.cap_outliers': ('src/mfles.html#cap_outliers', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.cross_validation': ('src/mfles.html#cross_validation', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.default_configs': ('src/mfles.html#default_configs', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.fast_ols': ('src/mfles.html#fast_ols', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.get_basis': ('src/mfles.html#get_basis', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.get_fourier_series': ( 'src/mfles.html#get_fourier_series',
+                                                                                 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.get_future_basis': ('src/mfles.html#get_future_basis', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.get_seasonality_weights': ( 'src/mfles.html#get_seasonality_weights',
+                                                                                      'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.lasso_nb': ('src/mfles.html#lasso_nb', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.logic_check': ('src/mfles.html#logic_check', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.logic_layer': ('src/mfles.html#logic_layer', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.median': ('src/mfles.html#median', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.ols': ('src/mfles.html#ols', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.ses_ensemble': ('src/mfles.html#ses_ensemble', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.set_fourier': ('src/mfles.html#set_fourier', 'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.siegel_repeated_medians': ( 'src/mfles.html#siegel_repeated_medians',
+                                                                                      'statsforecast/mfles.py'),
+                                     'statsforecast.mfles.wls': ('src/mfles.html#wls', 'statsforecast/mfles.py')},
             'statsforecast.models': { 'statsforecast.models.ADIDA': ('src/core/models.html#adida', 'statsforecast/models.py'),
                                       'statsforecast.models.ADIDA.__init__': ( 'src/core/models.html#adida.__init__',
                                                                                'statsforecast/models.py'),
-                                      'statsforecast.models.ADIDA.__repr__': ( 'src/core/models.html#adida.__repr__',
-                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.ADIDA.fit': ('src/core/models.html#adida.fit', 'statsforecast/models.py'),
                                       'statsforecast.models.ADIDA.forecast': ( 'src/core/models.html#adida.forecast',
                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.ADIDA.predict': ( 'src/core/models.html#adida.predict',
                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.ADIDA.predict_in_sample': ( 'src/core/models.html#adida.predict_in_sample',
                                                                                         'statsforecast/models.py'),
                                       'statsforecast.models.ARCH': ('src/core/models.html#arch', 'statsforecast/models.py'),
                                       'statsforecast.models.ARCH.__init__': ( 'src/core/models.html#arch.__init__',
                                                                               'statsforecast/models.py'),
-                                      'statsforecast.models.ARCH.__repr__': ( 'src/core/models.html#arch.__repr__',
-                                                                              'statsforecast/models.py'),
                                       'statsforecast.models.ARIMA': ('src/core/models.html#arima', 'statsforecast/models.py'),
                                       'statsforecast.models.ARIMA.__init__': ( 'src/core/models.html#arima.__init__',
                                                                                'statsforecast/models.py'),
-                                      'statsforecast.models.ARIMA.__repr__': ( 'src/core/models.html#arima.__repr__',
-                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.ARIMA.fit': ('src/core/models.html#arima.fit', 'statsforecast/models.py'),
                                       'statsforecast.models.ARIMA.forecast': ( 'src/core/models.html#arima.forecast',
                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.ARIMA.forward': ( 'src/core/models.html#arima.forward',
                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.ARIMA.predict': ( 'src/core/models.html#arima.predict',
                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.ARIMA.predict_in_sample': ( 'src/core/models.html#arima.predict_in_sample',
                                                                                         'statsforecast/models.py'),
                                       'statsforecast.models.AutoARIMA': ('src/core/models.html#autoarima', 'statsforecast/models.py'),
                                       'statsforecast.models.AutoARIMA.__init__': ( 'src/core/models.html#autoarima.__init__',
                                                                                    'statsforecast/models.py'),
-                                      'statsforecast.models.AutoARIMA.__repr__': ( 'src/core/models.html#autoarima.__repr__',
-                                                                                   'statsforecast/models.py'),
                                       'statsforecast.models.AutoARIMA.fit': ( 'src/core/models.html#autoarima.fit',
                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.AutoARIMA.forecast': ( 'src/core/models.html#autoarima.forecast',
                                                                                    'statsforecast/models.py'),
                                       'statsforecast.models.AutoARIMA.forward': ( 'src/core/models.html#autoarima.forward',
                                                                                   'statsforecast/models.py'),
                                       'statsforecast.models.AutoARIMA.predict': ( 'src/core/models.html#autoarima.predict',
                                                                                   'statsforecast/models.py'),
                                       'statsforecast.models.AutoARIMA.predict_in_sample': ( 'src/core/models.html#autoarima.predict_in_sample',
                                                                                             'statsforecast/models.py'),
                                       'statsforecast.models.AutoCES': ('src/core/models.html#autoces', 'statsforecast/models.py'),
                                       'statsforecast.models.AutoCES.__init__': ( 'src/core/models.html#autoces.__init__',
                                                                                  'statsforecast/models.py'),
-                                      'statsforecast.models.AutoCES.__repr__': ( 'src/core/models.html#autoces.__repr__',
-                                                                                 'statsforecast/models.py'),
                                       'statsforecast.models.AutoCES.fit': ('src/core/models.html#autoces.fit', 'statsforecast/models.py'),
                                       'statsforecast.models.AutoCES.forecast': ( 'src/core/models.html#autoces.forecast',
                                                                                  'statsforecast/models.py'),
                                       'statsforecast.models.AutoCES.forward': ( 'src/core/models.html#autoces.forward',
                                                                                 'statsforecast/models.py'),
                                       'statsforecast.models.AutoCES.predict': ( 'src/core/models.html#autoces.predict',
                                                                                 'statsforecast/models.py'),
                                       'statsforecast.models.AutoCES.predict_in_sample': ( 'src/core/models.html#autoces.predict_in_sample',
                                                                                           'statsforecast/models.py'),
                                       'statsforecast.models.AutoETS': ('src/core/models.html#autoets', 'statsforecast/models.py'),
                                       'statsforecast.models.AutoETS.__init__': ( 'src/core/models.html#autoets.__init__',
                                                                                  'statsforecast/models.py'),
-                                      'statsforecast.models.AutoETS.__repr__': ( 'src/core/models.html#autoets.__repr__',
-                                                                                 'statsforecast/models.py'),
                                       'statsforecast.models.AutoETS.fit': ('src/core/models.html#autoets.fit', 'statsforecast/models.py'),
                                       'statsforecast.models.AutoETS.forecast': ( 'src/core/models.html#autoets.forecast',
                                                                                  'statsforecast/models.py'),
                                       'statsforecast.models.AutoETS.forward': ( 'src/core/models.html#autoets.forward',
                                                                                 'statsforecast/models.py'),
                                       'statsforecast.models.AutoETS.predict': ( 'src/core/models.html#autoets.predict',
                                                                                 'statsforecast/models.py'),
                                       'statsforecast.models.AutoETS.predict_in_sample': ( 'src/core/models.html#autoets.predict_in_sample',
                                                                                           'statsforecast/models.py'),
+                                      'statsforecast.models.AutoMFLES': ('src/core/models.html#automfles', 'statsforecast/models.py'),
+                                      'statsforecast.models.AutoMFLES.__init__': ( 'src/core/models.html#automfles.__init__',
+                                                                                   'statsforecast/models.py'),
+                                      'statsforecast.models.AutoMFLES._fit': ( 'src/core/models.html#automfles._fit',
+                                                                               'statsforecast/models.py'),
+                                      'statsforecast.models.AutoMFLES.fit': ( 'src/core/models.html#automfles.fit',
+                                                                              'statsforecast/models.py'),
+                                      'statsforecast.models.AutoMFLES.forecast': ( 'src/core/models.html#automfles.forecast',
+                                                                                   'statsforecast/models.py'),
+                                      'statsforecast.models.AutoMFLES.predict': ( 'src/core/models.html#automfles.predict',
+                                                                                  'statsforecast/models.py'),
+                                      'statsforecast.models.AutoMFLES.predict_in_sample': ( 'src/core/models.html#automfles.predict_in_sample',
+                                                                                            'statsforecast/models.py'),
                                       'statsforecast.models.AutoRegressive': ( 'src/core/models.html#autoregressive',
                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.AutoRegressive.__init__': ( 'src/core/models.html#autoregressive.__init__',
                                                                                         'statsforecast/models.py'),
-                                      'statsforecast.models.AutoRegressive.__repr__': ( 'src/core/models.html#autoregressive.__repr__',
-                                                                                        'statsforecast/models.py'),
                                       'statsforecast.models.AutoTBATS': ('src/core/models.html#autotbats', 'statsforecast/models.py'),
                                       'statsforecast.models.AutoTBATS.__init__': ( 'src/core/models.html#autotbats.__init__',
                                                                                    'statsforecast/models.py'),
                                       'statsforecast.models.AutoTheta': ('src/core/models.html#autotheta', 'statsforecast/models.py'),
                                       'statsforecast.models.AutoTheta.__init__': ( 'src/core/models.html#autotheta.__init__',
                                                                                    'statsforecast/models.py'),
-                                      'statsforecast.models.AutoTheta.__repr__': ( 'src/core/models.html#autotheta.__repr__',
-                                                                                   'statsforecast/models.py'),
                                       'statsforecast.models.AutoTheta.fit': ( 'src/core/models.html#autotheta.fit',
                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.AutoTheta.forecast': ( 'src/core/models.html#autotheta.forecast',
                                                                                    'statsforecast/models.py'),
                                       'statsforecast.models.AutoTheta.forward': ( 'src/core/models.html#autotheta.forward',
                                                                                   'statsforecast/models.py'),
                                       'statsforecast.models.AutoTheta.predict': ( 'src/core/models.html#autotheta.predict',
                                                                                   'statsforecast/models.py'),
                                       'statsforecast.models.AutoTheta.predict_in_sample': ( 'src/core/models.html#autotheta.predict_in_sample',
                                                                                             'statsforecast/models.py'),
                                       'statsforecast.models.ConstantModel': ( 'src/core/models.html#constantmodel',
                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.ConstantModel.__init__': ( 'src/core/models.html#constantmodel.__init__',
                                                                                        'statsforecast/models.py'),
-                                      'statsforecast.models.ConstantModel.__repr__': ( 'src/core/models.html#constantmodel.__repr__',
-                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models.ConstantModel.fit': ( 'src/core/models.html#constantmodel.fit',
                                                                                   'statsforecast/models.py'),
                                       'statsforecast.models.ConstantModel.forecast': ( 'src/core/models.html#constantmodel.forecast',
                                                                                        'statsforecast/models.py'),
                                       'statsforecast.models.ConstantModel.forward': ( 'src/core/models.html#constantmodel.forward',
                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models.ConstantModel.predict': ( 'src/core/models.html#constantmodel.predict',
                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models.ConstantModel.predict_in_sample': ( 'src/core/models.html#constantmodel.predict_in_sample',
                                                                                                 'statsforecast/models.py'),
                                       'statsforecast.models.CrostonClassic': ( 'src/core/models.html#crostonclassic',
                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.CrostonClassic.__init__': ( 'src/core/models.html#crostonclassic.__init__',
                                                                                         'statsforecast/models.py'),
-                                      'statsforecast.models.CrostonClassic.__repr__': ( 'src/core/models.html#crostonclassic.__repr__',
-                                                                                        'statsforecast/models.py'),
                                       'statsforecast.models.CrostonClassic.fit': ( 'src/core/models.html#crostonclassic.fit',
                                                                                    'statsforecast/models.py'),
                                       'statsforecast.models.CrostonClassic.forecast': ( 'src/core/models.html#crostonclassic.forecast',
                                                                                         'statsforecast/models.py'),
                                       'statsforecast.models.CrostonClassic.predict': ( 'src/core/models.html#crostonclassic.predict',
                                                                                        'statsforecast/models.py'),
                                       'statsforecast.models.CrostonClassic.predict_in_sample': ( 'src/core/models.html#crostonclassic.predict_in_sample',
                                                                                                  'statsforecast/models.py'),
                                       'statsforecast.models.CrostonOptimized': ( 'src/core/models.html#crostonoptimized',
                                                                                  'statsforecast/models.py'),
                                       'statsforecast.models.CrostonOptimized.__init__': ( 'src/core/models.html#crostonoptimized.__init__',
                                                                                           'statsforecast/models.py'),
-                                      'statsforecast.models.CrostonOptimized.__repr__': ( 'src/core/models.html#crostonoptimized.__repr__',
-                                                                                          'statsforecast/models.py'),
                                       'statsforecast.models.CrostonOptimized.fit': ( 'src/core/models.html#crostonoptimized.fit',
                                                                                      'statsforecast/models.py'),
                                       'statsforecast.models.CrostonOptimized.forecast': ( 'src/core/models.html#crostonoptimized.forecast',
                                                                                           'statsforecast/models.py'),
                                       'statsforecast.models.CrostonOptimized.predict': ( 'src/core/models.html#crostonoptimized.predict',
                                                                                          'statsforecast/models.py'),
                                       'statsforecast.models.CrostonOptimized.predict_in_sample': ( 'src/core/models.html#crostonoptimized.predict_in_sample',
                                                                                                    'statsforecast/models.py'),
                                       'statsforecast.models.CrostonSBA': ('src/core/models.html#crostonsba', 'statsforecast/models.py'),
                                       'statsforecast.models.CrostonSBA.__init__': ( 'src/core/models.html#crostonsba.__init__',
                                                                                     'statsforecast/models.py'),
-                                      'statsforecast.models.CrostonSBA.__repr__': ( 'src/core/models.html#crostonsba.__repr__',
-                                                                                    'statsforecast/models.py'),
                                       'statsforecast.models.CrostonSBA.fit': ( 'src/core/models.html#crostonsba.fit',
                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.CrostonSBA.forecast': ( 'src/core/models.html#crostonsba.forecast',
                                                                                     'statsforecast/models.py'),
                                       'statsforecast.models.CrostonSBA.predict': ( 'src/core/models.html#crostonsba.predict',
                                                                                    'statsforecast/models.py'),
                                       'statsforecast.models.CrostonSBA.predict_in_sample': ( 'src/core/models.html#crostonsba.predict_in_sample',
@@ -430,84 +472,80 @@
                                       'statsforecast.models.DynamicOptimizedTheta.__init__': ( 'src/core/models.html#dynamicoptimizedtheta.__init__',
                                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.DynamicTheta': ('src/core/models.html#dynamictheta', 'statsforecast/models.py'),
                                       'statsforecast.models.DynamicTheta.__init__': ( 'src/core/models.html#dynamictheta.__init__',
                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models.ETS': ('src/core/models.html#ets', 'statsforecast/models.py'),
                                       'statsforecast.models.ETS.__init__': ('src/core/models.html#ets.__init__', 'statsforecast/models.py'),
-                                      'statsforecast.models.ETS.__repr__': ('src/core/models.html#ets.__repr__', 'statsforecast/models.py'),
                                       'statsforecast.models.ETS._warn': ('src/core/models.html#ets._warn', 'statsforecast/models.py'),
                                       'statsforecast.models.GARCH': ('src/core/models.html#garch', 'statsforecast/models.py'),
                                       'statsforecast.models.GARCH.__init__': ( 'src/core/models.html#garch.__init__',
                                                                                'statsforecast/models.py'),
-                                      'statsforecast.models.GARCH.__repr__': ( 'src/core/models.html#garch.__repr__',
-                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.GARCH.fit': ('src/core/models.html#garch.fit', 'statsforecast/models.py'),
                                       'statsforecast.models.GARCH.forecast': ( 'src/core/models.html#garch.forecast',
                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.GARCH.predict': ( 'src/core/models.html#garch.predict',
                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.GARCH.predict_in_sample': ( 'src/core/models.html#garch.predict_in_sample',
                                                                                         'statsforecast/models.py'),
                                       'statsforecast.models.HistoricAverage': ( 'src/core/models.html#historicaverage',
                                                                                 'statsforecast/models.py'),
                                       'statsforecast.models.HistoricAverage.__init__': ( 'src/core/models.html#historicaverage.__init__',
                                                                                          'statsforecast/models.py'),
-                                      'statsforecast.models.HistoricAverage.__repr__': ( 'src/core/models.html#historicaverage.__repr__',
-                                                                                         'statsforecast/models.py'),
                                       'statsforecast.models.HistoricAverage.fit': ( 'src/core/models.html#historicaverage.fit',
                                                                                     'statsforecast/models.py'),
                                       'statsforecast.models.HistoricAverage.forecast': ( 'src/core/models.html#historicaverage.forecast',
                                                                                          'statsforecast/models.py'),
                                       'statsforecast.models.HistoricAverage.predict': ( 'src/core/models.html#historicaverage.predict',
                                                                                         'statsforecast/models.py'),
                                       'statsforecast.models.HistoricAverage.predict_in_sample': ( 'src/core/models.html#historicaverage.predict_in_sample',
                                                                                                   'statsforecast/models.py'),
                                       'statsforecast.models.Holt': ('src/core/models.html#holt', 'statsforecast/models.py'),
                                       'statsforecast.models.Holt.__init__': ( 'src/core/models.html#holt.__init__',
                                                                               'statsforecast/models.py'),
-                                      'statsforecast.models.Holt.__repr__': ( 'src/core/models.html#holt.__repr__',
-                                                                              'statsforecast/models.py'),
                                       'statsforecast.models.HoltWinters': ('src/core/models.html#holtwinters', 'statsforecast/models.py'),
                                       'statsforecast.models.HoltWinters.__init__': ( 'src/core/models.html#holtwinters.__init__',
                                                                                      'statsforecast/models.py'),
-                                      'statsforecast.models.HoltWinters.__repr__': ( 'src/core/models.html#holtwinters.__repr__',
-                                                                                     'statsforecast/models.py'),
                                       'statsforecast.models.IMAPA': ('src/core/models.html#imapa', 'statsforecast/models.py'),
                                       'statsforecast.models.IMAPA.__init__': ( 'src/core/models.html#imapa.__init__',
                                                                                'statsforecast/models.py'),
-                                      'statsforecast.models.IMAPA.__repr__': ( 'src/core/models.html#imapa.__repr__',
-                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.IMAPA.fit': ('src/core/models.html#imapa.fit', 'statsforecast/models.py'),
                                       'statsforecast.models.IMAPA.forecast': ( 'src/core/models.html#imapa.forecast',
                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.IMAPA.predict': ( 'src/core/models.html#imapa.predict',
                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.IMAPA.predict_in_sample': ( 'src/core/models.html#imapa.predict_in_sample',
                                                                                         'statsforecast/models.py'),
+                                      'statsforecast.models.MFLES': ('src/core/models.html#mfles', 'statsforecast/models.py'),
+                                      'statsforecast.models.MFLES.__init__': ( 'src/core/models.html#mfles.__init__',
+                                                                               'statsforecast/models.py'),
+                                      'statsforecast.models.MFLES._fit': ('src/core/models.html#mfles._fit', 'statsforecast/models.py'),
+                                      'statsforecast.models.MFLES.fit': ('src/core/models.html#mfles.fit', 'statsforecast/models.py'),
+                                      'statsforecast.models.MFLES.forecast': ( 'src/core/models.html#mfles.forecast',
+                                                                               'statsforecast/models.py'),
+                                      'statsforecast.models.MFLES.predict': ( 'src/core/models.html#mfles.predict',
+                                                                              'statsforecast/models.py'),
+                                      'statsforecast.models.MFLES.predict_in_sample': ( 'src/core/models.html#mfles.predict_in_sample',
+                                                                                        'statsforecast/models.py'),
                                       'statsforecast.models.MSTL': ('src/core/models.html#mstl', 'statsforecast/models.py'),
                                       'statsforecast.models.MSTL.__init__': ( 'src/core/models.html#mstl.__init__',
                                                                               'statsforecast/models.py'),
-                                      'statsforecast.models.MSTL.__repr__': ( 'src/core/models.html#mstl.__repr__',
-                                                                              'statsforecast/models.py'),
                                       'statsforecast.models.MSTL.fit': ('src/core/models.html#mstl.fit', 'statsforecast/models.py'),
                                       'statsforecast.models.MSTL.forecast': ( 'src/core/models.html#mstl.forecast',
                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.MSTL.forward': ('src/core/models.html#mstl.forward', 'statsforecast/models.py'),
                                       'statsforecast.models.MSTL.predict': ('src/core/models.html#mstl.predict', 'statsforecast/models.py'),
                                       'statsforecast.models.MSTL.predict_in_sample': ( 'src/core/models.html#mstl.predict_in_sample',
                                                                                        'statsforecast/models.py'),
                                       'statsforecast.models.NaNModel': ('src/core/models.html#nanmodel', 'statsforecast/models.py'),
                                       'statsforecast.models.NaNModel.__init__': ( 'src/core/models.html#nanmodel.__init__',
                                                                                   'statsforecast/models.py'),
                                       'statsforecast.models.Naive': ('src/core/models.html#naive', 'statsforecast/models.py'),
                                       'statsforecast.models.Naive.__init__': ( 'src/core/models.html#naive.__init__',
                                                                                'statsforecast/models.py'),
-                                      'statsforecast.models.Naive.__repr__': ( 'src/core/models.html#naive.__repr__',
-                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.Naive.fit': ('src/core/models.html#naive.fit', 'statsforecast/models.py'),
                                       'statsforecast.models.Naive.forecast': ( 'src/core/models.html#naive.forecast',
                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.Naive.forward': ( 'src/core/models.html#naive.forward',
                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.Naive.predict': ( 'src/core/models.html#naive.predict',
                                                                               'statsforecast/models.py'),
@@ -517,149 +555,144 @@
                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.OptimizedTheta.__init__': ( 'src/core/models.html#optimizedtheta.__init__',
                                                                                         'statsforecast/models.py'),
                                       'statsforecast.models.RandomWalkWithDrift': ( 'src/core/models.html#randomwalkwithdrift',
                                                                                     'statsforecast/models.py'),
                                       'statsforecast.models.RandomWalkWithDrift.__init__': ( 'src/core/models.html#randomwalkwithdrift.__init__',
                                                                                              'statsforecast/models.py'),
-                                      'statsforecast.models.RandomWalkWithDrift.__repr__': ( 'src/core/models.html#randomwalkwithdrift.__repr__',
-                                                                                             'statsforecast/models.py'),
                                       'statsforecast.models.RandomWalkWithDrift.fit': ( 'src/core/models.html#randomwalkwithdrift.fit',
                                                                                         'statsforecast/models.py'),
                                       'statsforecast.models.RandomWalkWithDrift.forecast': ( 'src/core/models.html#randomwalkwithdrift.forecast',
                                                                                              'statsforecast/models.py'),
                                       'statsforecast.models.RandomWalkWithDrift.predict': ( 'src/core/models.html#randomwalkwithdrift.predict',
                                                                                             'statsforecast/models.py'),
                                       'statsforecast.models.RandomWalkWithDrift.predict_in_sample': ( 'src/core/models.html#randomwalkwithdrift.predict_in_sample',
                                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalExponentialSmoothing': ( 'src/core/models.html#seasonalexponentialsmoothing',
                                                                                              'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalExponentialSmoothing.__init__': ( 'src/core/models.html#seasonalexponentialsmoothing.__init__',
                                                                                                       'statsforecast/models.py'),
-                                      'statsforecast.models.SeasonalExponentialSmoothing.__repr__': ( 'src/core/models.html#seasonalexponentialsmoothing.__repr__',
-                                                                                                      'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalExponentialSmoothing.fit': ( 'src/core/models.html#seasonalexponentialsmoothing.fit',
                                                                                                  'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalExponentialSmoothing.forecast': ( 'src/core/models.html#seasonalexponentialsmoothing.forecast',
                                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalExponentialSmoothing.predict': ( 'src/core/models.html#seasonalexponentialsmoothing.predict',
                                                                                                      'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalExponentialSmoothing.predict_in_sample': ( 'src/core/models.html#seasonalexponentialsmoothing.predict_in_sample',
                                                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalExponentialSmoothingOptimized': ( 'src/core/models.html#seasonalexponentialsmoothingoptimized',
                                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalExponentialSmoothingOptimized.__init__': ( 'src/core/models.html#seasonalexponentialsmoothingoptimized.__init__',
                                                                                                                'statsforecast/models.py'),
-                                      'statsforecast.models.SeasonalExponentialSmoothingOptimized.__repr__': ( 'src/core/models.html#seasonalexponentialsmoothingoptimized.__repr__',
-                                                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalExponentialSmoothingOptimized.fit': ( 'src/core/models.html#seasonalexponentialsmoothingoptimized.fit',
                                                                                                           'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalExponentialSmoothingOptimized.forecast': ( 'src/core/models.html#seasonalexponentialsmoothingoptimized.forecast',
                                                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalExponentialSmoothingOptimized.predict': ( 'src/core/models.html#seasonalexponentialsmoothingoptimized.predict',
                                                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalExponentialSmoothingOptimized.predict_in_sample': ( 'src/core/models.html#seasonalexponentialsmoothingoptimized.predict_in_sample',
                                                                                                                         'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalNaive': ( 'src/core/models.html#seasonalnaive',
                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalNaive.__init__': ( 'src/core/models.html#seasonalnaive.__init__',
                                                                                        'statsforecast/models.py'),
-                                      'statsforecast.models.SeasonalNaive.__repr__': ( 'src/core/models.html#seasonalnaive.__repr__',
-                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalNaive.fit': ( 'src/core/models.html#seasonalnaive.fit',
                                                                                   'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalNaive.forecast': ( 'src/core/models.html#seasonalnaive.forecast',
                                                                                        'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalNaive.predict': ( 'src/core/models.html#seasonalnaive.predict',
                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalNaive.predict_in_sample': ( 'src/core/models.html#seasonalnaive.predict_in_sample',
                                                                                                 'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalWindowAverage': ( 'src/core/models.html#seasonalwindowaverage',
                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalWindowAverage.__init__': ( 'src/core/models.html#seasonalwindowaverage.__init__',
                                                                                                'statsforecast/models.py'),
-                                      'statsforecast.models.SeasonalWindowAverage.__repr__': ( 'src/core/models.html#seasonalwindowaverage.__repr__',
-                                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalWindowAverage.fit': ( 'src/core/models.html#seasonalwindowaverage.fit',
                                                                                           'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalWindowAverage.forecast': ( 'src/core/models.html#seasonalwindowaverage.forecast',
                                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalWindowAverage.predict': ( 'src/core/models.html#seasonalwindowaverage.predict',
                                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.SeasonalWindowAverage.predict_in_sample': ( 'src/core/models.html#seasonalwindowaverage.predict_in_sample',
                                                                                                         'statsforecast/models.py'),
                                       'statsforecast.models.SimpleExponentialSmoothing': ( 'src/core/models.html#simpleexponentialsmoothing',
                                                                                            'statsforecast/models.py'),
                                       'statsforecast.models.SimpleExponentialSmoothing.__init__': ( 'src/core/models.html#simpleexponentialsmoothing.__init__',
                                                                                                     'statsforecast/models.py'),
-                                      'statsforecast.models.SimpleExponentialSmoothing.__repr__': ( 'src/core/models.html#simpleexponentialsmoothing.__repr__',
-                                                                                                    'statsforecast/models.py'),
                                       'statsforecast.models.SimpleExponentialSmoothing.fit': ( 'src/core/models.html#simpleexponentialsmoothing.fit',
                                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.SimpleExponentialSmoothing.forecast': ( 'src/core/models.html#simpleexponentialsmoothing.forecast',
                                                                                                     'statsforecast/models.py'),
                                       'statsforecast.models.SimpleExponentialSmoothing.predict': ( 'src/core/models.html#simpleexponentialsmoothing.predict',
                                                                                                    'statsforecast/models.py'),
                                       'statsforecast.models.SimpleExponentialSmoothing.predict_in_sample': ( 'src/core/models.html#simpleexponentialsmoothing.predict_in_sample',
                                                                                                              'statsforecast/models.py'),
                                       'statsforecast.models.SimpleExponentialSmoothingOptimized': ( 'src/core/models.html#simpleexponentialsmoothingoptimized',
                                                                                                     'statsforecast/models.py'),
                                       'statsforecast.models.SimpleExponentialSmoothingOptimized.__init__': ( 'src/core/models.html#simpleexponentialsmoothingoptimized.__init__',
                                                                                                              'statsforecast/models.py'),
-                                      'statsforecast.models.SimpleExponentialSmoothingOptimized.__repr__': ( 'src/core/models.html#simpleexponentialsmoothingoptimized.__repr__',
-                                                                                                             'statsforecast/models.py'),
                                       'statsforecast.models.SimpleExponentialSmoothingOptimized.fit': ( 'src/core/models.html#simpleexponentialsmoothingoptimized.fit',
                                                                                                         'statsforecast/models.py'),
                                       'statsforecast.models.SimpleExponentialSmoothingOptimized.forecast': ( 'src/core/models.html#simpleexponentialsmoothingoptimized.forecast',
                                                                                                              'statsforecast/models.py'),
                                       'statsforecast.models.SimpleExponentialSmoothingOptimized.predict': ( 'src/core/models.html#simpleexponentialsmoothingoptimized.predict',
                                                                                                             'statsforecast/models.py'),
                                       'statsforecast.models.SimpleExponentialSmoothingOptimized.predict_in_sample': ( 'src/core/models.html#simpleexponentialsmoothingoptimized.predict_in_sample',
                                                                                                                       'statsforecast/models.py'),
+                                      'statsforecast.models.SklearnModel': ('src/core/models.html#sklearnmodel', 'statsforecast/models.py'),
+                                      'statsforecast.models.SklearnModel.__init__': ( 'src/core/models.html#sklearnmodel.__init__',
+                                                                                      'statsforecast/models.py'),
+                                      'statsforecast.models.SklearnModel.fit': ( 'src/core/models.html#sklearnmodel.fit',
+                                                                                 'statsforecast/models.py'),
+                                      'statsforecast.models.SklearnModel.forecast': ( 'src/core/models.html#sklearnmodel.forecast',
+                                                                                      'statsforecast/models.py'),
+                                      'statsforecast.models.SklearnModel.forward': ( 'src/core/models.html#sklearnmodel.forward',
+                                                                                     'statsforecast/models.py'),
+                                      'statsforecast.models.SklearnModel.predict': ( 'src/core/models.html#sklearnmodel.predict',
+                                                                                     'statsforecast/models.py'),
+                                      'statsforecast.models.SklearnModel.predict_in_sample': ( 'src/core/models.html#sklearnmodel.predict_in_sample',
+                                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.TBATS': ('src/core/models.html#tbats', 'statsforecast/models.py'),
                                       'statsforecast.models.TBATS.__init__': ( 'src/core/models.html#tbats.__init__',
                                                                                'statsforecast/models.py'),
-                                      'statsforecast.models.TBATS.__repr__': ( 'src/core/models.html#tbats.__repr__',
-                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.TBATS.fit': ('src/core/models.html#tbats.fit', 'statsforecast/models.py'),
                                       'statsforecast.models.TBATS.forecast': ( 'src/core/models.html#tbats.forecast',
                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.TBATS.predict': ( 'src/core/models.html#tbats.predict',
                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.TBATS.predict_in_sample': ( 'src/core/models.html#tbats.predict_in_sample',
                                                                                         'statsforecast/models.py'),
                                       'statsforecast.models.TSB': ('src/core/models.html#tsb', 'statsforecast/models.py'),
                                       'statsforecast.models.TSB.__init__': ('src/core/models.html#tsb.__init__', 'statsforecast/models.py'),
-                                      'statsforecast.models.TSB.__repr__': ('src/core/models.html#tsb.__repr__', 'statsforecast/models.py'),
                                       'statsforecast.models.TSB.fit': ('src/core/models.html#tsb.fit', 'statsforecast/models.py'),
                                       'statsforecast.models.TSB.forecast': ('src/core/models.html#tsb.forecast', 'statsforecast/models.py'),
                                       'statsforecast.models.TSB.predict': ('src/core/models.html#tsb.predict', 'statsforecast/models.py'),
                                       'statsforecast.models.TSB.predict_in_sample': ( 'src/core/models.html#tsb.predict_in_sample',
                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models.Theta': ('src/core/models.html#theta', 'statsforecast/models.py'),
                                       'statsforecast.models.Theta.__init__': ( 'src/core/models.html#theta.__init__',
                                                                                'statsforecast/models.py'),
                                       'statsforecast.models.WindowAverage': ( 'src/core/models.html#windowaverage',
                                                                               'statsforecast/models.py'),
                                       'statsforecast.models.WindowAverage.__init__': ( 'src/core/models.html#windowaverage.__init__',
                                                                                        'statsforecast/models.py'),
-                                      'statsforecast.models.WindowAverage.__repr__': ( 'src/core/models.html#windowaverage.__repr__',
-                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models.WindowAverage.fit': ( 'src/core/models.html#windowaverage.fit',
                                                                                   'statsforecast/models.py'),
                                       'statsforecast.models.WindowAverage.forecast': ( 'src/core/models.html#windowaverage.forecast',
                                                                                        'statsforecast/models.py'),
                                       'statsforecast.models.WindowAverage.predict': ( 'src/core/models.html#windowaverage.predict',
                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models.WindowAverage.predict_in_sample': ( 'src/core/models.html#windowaverage.predict_in_sample',
                                                                                                 'statsforecast/models.py'),
                                       'statsforecast.models.ZeroModel': ('src/core/models.html#zeromodel', 'statsforecast/models.py'),
                                       'statsforecast.models.ZeroModel.__init__': ( 'src/core/models.html#zeromodel.__init__',
                                                                                    'statsforecast/models.py'),
                                       'statsforecast.models._TS': ('src/core/models.html#_ts', 'statsforecast/models.py'),
+                                      'statsforecast.models._TS.__repr__': ('src/core/models.html#_ts.__repr__', 'statsforecast/models.py'),
                                       'statsforecast.models._TS._add_conformal_intervals': ( 'src/core/models.html#_ts._add_conformal_intervals',
                                                                                              'statsforecast/models.py'),
                                       'statsforecast.models._TS._add_predict_conformal_intervals': ( 'src/core/models.html#_ts._add_predict_conformal_intervals',
                                                                                                      'statsforecast/models.py'),
                                       'statsforecast.models._TS._conformal_method': ( 'src/core/models.html#_ts._conformal_method',
                                                                                       'statsforecast/models.py'),
                                       'statsforecast.models._TS._conformity_scores': ( 'src/core/models.html#_ts._conformity_scores',
```

### Comparing `statsforecast-1.7.4/statsforecast/adapters/prophet.py` & `statsforecast-1.7.5/statsforecast/adapters/prophet.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,20 +213,17 @@
         self.history_dates = pd.to_datetime(
             pd.Series(df["ds"].unique(), name="ds")
         ).sort_values()
 
         history = self.setup_dataframe(history, initialize_scales=True)
         self.history = history
         self.set_auto_seasonalities()
-        (
-            seasonal_features,
-            prior_scales,
-            component_cols,
-            modes,
-        ) = self.make_all_seasonality_features(history)
+        seasonal_features, prior_scales, component_cols, modes = (
+            self.make_all_seasonality_features(history)
+        )
         self.train_component_cols = component_cols
         self.component_modes = modes
         if disable_seasonal_features:
             seas = tuple(self.seasonalities.keys())
             seasonal_features = seasonal_features.loc[
                 :, ~seasonal_features.columns.str.startswith(seas)
             ]
```

### Comparing `statsforecast-1.7.4/statsforecast/arima.py` & `statsforecast-1.7.5/statsforecast/arima.py`

 * *Files 0% similar despite different names*

```diff
@@ -886,14 +886,18 @@
         par[mask] = p
         phi, theta = arima_transpar(par, arma, False)
 
         if ncxreg > 0:
             x -= np.dot(xreg, par[narma + np.arange(ncxreg)])
 
         res, resid = arima_css(x, arma, phi, theta, ncond)
+        if math.isinf(res):
+            import sys
+
+            return sys.float_info.max
         if res <= 0.0:
             return -math.inf
         return 0.5 * math.log(res)
 
     coef = np.array(fixed)
     # parscale definition, think about it, scipy doesn't use it
     if method == "CSS":
@@ -1100,14 +1104,15 @@
 def checkarima(obj):
     if obj["var_coef"] is None:
         return False
     return any(np.isnan(np.sqrt(np.diag(obj["var_coef"]))))
 
 # %% ../nbs/src/arima.ipynb 44
 def predict_arima(model, n_ahead, newxreg=None, se_fit=True):
+
     myNCOL = lambda x: x.shape[1] if x is not None else 0
     # rsd = model['residuals']
     # xreg = model['xreg']
     # ncxreg = myNCOL(xreg)
 
     # n = len(rsd)
     arma = model["arma"]
@@ -2049,16 +2054,16 @@
             stationary,
             ic,
             trace,
             approximation,
             method=method,
             xreg=xreg,
             offset=offset,
-            allowdrift=allowdrift,
-            allowmean=allowmean,
+            allow_drift=allowdrift,
+            allow_mean=allowmean,
             period=m,
         )
         bestfit["lambda"] = blambda
         bestfit["x"] = origx
         if trace:
             print(f"Best model: {arima_string(bestfit, padding=True)}\n\n")
         return bestfit
```

### Comparing `statsforecast-1.7.4/statsforecast/ces.py` & `statsforecast-1.7.5/statsforecast/ces.py`

 * *Files 0% similar despite different names*

```diff
@@ -675,14 +675,15 @@
         f=forecast,
         **obj["par"]
     )
     return forecast
 
 # %% ../nbs/src/ces.ipynb 31
 def _simulate_pred_intervals(model, h, level):
+
     np.random.seed(1)
     nsim = 5000
     y_path = np.zeros([nsim, h])
 
     for k in range(nsim):
         e = np.random.normal(0, np.sqrt(model["sigma2"]), model["states"].shape)
         states = model["states"]
```

### Comparing `statsforecast-1.7.4/statsforecast/core.py` & `statsforecast-1.7.5/statsforecast/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import numpy as np
 import pandas as pd
 import utilsforecast.processing as ufp
 from fugue.execution.factory import (
     make_execution_engine,
     try_get_context_execution_engine,
 )
+from threadpoolctl import threadpool_limits
 from tqdm.autonotebook import tqdm
 from triad import conditional_dispatcher
 from utilsforecast.compat import DataFrame, pl_DataFrame, pl_Series
 from utilsforecast.grouped_array import GroupedArray as BaseGroupedArray
 from utilsforecast.validation import ensure_time_dtype, validate_freq
 
 from .utils import ConformalIntervals
@@ -37,14 +38,15 @@
         format="%(asctime)s %(name)s %(levelname)s: %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 logger = logging.getLogger(__name__)
 
 # %% ../nbs/src/core/core.ipynb 10
 class GroupedArray(BaseGroupedArray):
+
     def __eq__(self, other):
         if not hasattr(other, "data") or not hasattr(other, "indptr"):
             return False
         return np.allclose(self.data, other.data) and np.array_equal(
             self.indptr, other.indptr
         )
 
@@ -212,17 +214,19 @@
                     cols_m_fitted = [
                         key
                         for key in res_i.keys()
                         if any(key.startswith(m) for m in matches_fitted)
                     ]
                     fitted_i = np.vstack([res_i[key] for key in cols_m_fitted]).T
                     cols_m_fitted = [
-                        f"{repr(model)}"
-                        if col == "fitted"
-                        else f"{repr(model)}-{col.replace('fitted-', '')}"
+                        (
+                            f"{repr(model)}"
+                            if col == "fitted"
+                            else f"{repr(model)}-{col.replace('fitted-', '')}"
+                        )
                         for col in cols_m_fitted
                     ]
                     fitted_vals[
                         self.indptr[i] : self.indptr[i + 1],
                         (cuts[i_model] + 1) : (cuts[i_model + 1] + 1),
                     ] = fitted_i
                     cols_fitted += cols_m_fitted
@@ -382,14 +386,78 @@
     def split_fm(self, fm, n_chunks):
         return [
             fm[idxs]
             for idxs in np.array_split(range(self.n_groups), n_chunks)
             if idxs.size
         ]
 
+    def _single_threaded_fit(self, models, fallback_model=None):
+        with threadpool_limits(limits=1):
+            return self.fit(models=models, fallback_model=fallback_model)
+
+    def _single_threaded_predict(self, fm, h, X=None, level=tuple()):
+        with threadpool_limits(limits=1):
+            return self.predict(fm=fm, h=h, X=X, level=level)
+
+    def _single_threaded_fit_predict(self, models, h, X=None, level=tuple()):
+        with threadpool_limits(limits=1):
+            return self.fit_predict(models=models, h=h, X=X, level=level)
+
+    def _single_threaded_forecast(
+        self,
+        models,
+        h,
+        fallback_model=None,
+        fitted=False,
+        X=None,
+        level=tuple(),
+        verbose=False,
+        target_col="y",
+    ):
+        with threadpool_limits(limits=1):
+            return self.forecast(
+                models=models,
+                h=h,
+                fallback_model=fallback_model,
+                fitted=fitted,
+                X=X,
+                level=level,
+                verbose=verbose,
+                target_col=target_col,
+            )
+
+    def _single_threaded_cross_validation(
+        self,
+        models,
+        h,
+        test_size,
+        fallback_model=None,
+        step_size=1,
+        input_size=None,
+        fitted=False,
+        level=tuple(),
+        refit=True,
+        verbose=False,
+        target_col="y",
+    ):
+        with threadpool_limits(limits=1):
+            return self.cross_validation(
+                models=models,
+                h=h,
+                test_size=test_size,
+                fallback_model=fallback_model,
+                step_size=step_size,
+                input_size=input_size,
+                fitted=fitted,
+                level=level,
+                refit=refit,
+                verbose=verbose,
+                target_col=target_col,
+            )
+
 # %% ../nbs/src/core/core.ipynb 24
 def _get_n_jobs(n_groups, n_jobs):
     if n_jobs == -1 or (n_jobs is None):
         actual_n_jobs = os.cpu_count()
     else:
         actual_n_jobs = n_jobs
     return min(n_groups, actual_n_jobs)
@@ -673,16 +741,15 @@
         if X is None:
             return X, level
         expected_shape = (h * len(self.ga), self.ga.data.shape[1] + 1)
         if X.shape != expected_shape:
             raise ValueError(
                 f"Expected X to have shape {expected_shape}, but got {X.shape}"
             )
-        first_col = [c for c in X.columns if c not in (self.id_col, self.time_col)][0]
-        _, _, data, indptr, _ = ufp.process_df(X, self.id_col, self.time_col, first_col)
+        _, _, data, indptr, _ = ufp.process_df(X, self.id_col, self.time_col, None)
         return GroupedArray(data, indptr), level
 
     def _validate_exog(self, X_df: Optional[DataFrame] = None) -> None:
         if not any(m.uses_exog for m in self.models) or not self._exog:
             return
         err_msg = (
             f"Models require the following exogenous features {self._exog} "
@@ -970,26 +1037,26 @@
             raise ValueError("you must define `n_windows` or `test_size`")
         if test_size is None:
             test_size = h + step_size * (n_windows - 1)
         if prediction_intervals is not None and level is None:
             raise ValueError(
                 "You must specify `level` when using `prediction_intervals`"
             )
-        if not isinstance(refit, bool):
+        if refit != True:
             no_forward = [m for m in self.models if not hasattr(m, "forward")]
             if no_forward:
                 raise ValueError(
-                    "Can only use integer refit with models that implement the forward method. "
+                    "Can only use integer refit or refit=False with models that implement the forward method. "
                     f"The following models do not implement the forward method: {no_forward}."
                 )
             if self.fallback_model is not None and not hasattr(
                 self.fallback_model, "forward"
             ):
                 raise ValueError(
-                    "Can only use integer refit with a fallback model that implements the forward method."
+                    "Can only use integer refit or refit=False with a fallback model that implements the forward method."
                 )
         self.__dict__.pop("cv_fitted_values_", None)
         self._prepare_fit(
             df=df,
             sort_df=sort_df,
             id_col=id_col,
             time_col=time_col,
@@ -1113,15 +1180,15 @@
     def _fit_parallel(self):
         gas = self.ga.split(self.n_jobs)
         Pool, pool_kwargs = self._get_pool()
         with Pool(self.n_jobs, **pool_kwargs) as executor:
             futures = []
             for ga in gas:
                 future = executor.apply_async(
-                    ga.fit, (self.models, self.fallback_model)
+                    ga._single_threaded_fit, (self.models, self.fallback_model)
                 )
                 futures.append(future)
             fm = np.vstack([f.get() for f in futures])
         return fm
 
     def _get_gas_Xs(self, X):
         gas = self.ga.split(self.n_jobs)
@@ -1139,21 +1206,16 @@
         fms = self.ga.split_fm(self.fitted_, self.n_jobs)
         Pool, pool_kwargs = self._get_pool()
         # compute parallel forecasts
         with Pool(self.n_jobs, **pool_kwargs) as executor:
             futures = []
             for ga, fm, X_ in zip(gas, fms, Xs):
                 future = executor.apply_async(
-                    ga.predict,
-                    (
-                        fm,
-                        h,
-                        X_,
-                        level,
-                    ),
+                    ga._single_threaded_predict,
+                    (fm, h, X_, level),
                 )
                 futures.append(future)
             out = [f.get() for f in futures]
             fcsts, cols = list(zip(*out))
             fcsts = np.vstack(fcsts)
             cols = cols[0]
         return fcsts, cols
@@ -1163,21 +1225,16 @@
         gas, Xs = self._get_gas_Xs(X=X)
         Pool, pool_kwargs = self._get_pool()
         # compute parallel forecasts
         with Pool(self.n_jobs, **pool_kwargs) as executor:
             futures = []
             for ga, X_ in zip(gas, Xs):
                 future = executor.apply_async(
-                    ga.fit_predict,
-                    (
-                        self.models,
-                        h,
-                        X_,
-                        level,
-                    ),
+                    ga._single_threaded_fit_predict,
+                    (self.models, h, X_, level),
                 )
                 futures.append(future)
             out = [f.get() for f in futures]
             fm, fcsts, cols = list(zip(*out))
             fm = np.vstack(fm)
             fcsts = np.vstack(fcsts)
             cols = cols[0]
@@ -1189,15 +1246,15 @@
         Pool, pool_kwargs = self._get_pool()
         # compute parallel forecasts
         result = {}
         with Pool(self.n_jobs, **pool_kwargs) as executor:
             futures = []
             for ga, X_ in zip(gas, Xs):
                 future = executor.apply_async(
-                    ga.forecast,
+                    ga._single_threaded_forecast,
                     tuple(),
                     dict(
                         models=self.models,
                         h=h,
                         fallback_model=self.fallback_model,
                         fitted=fitted,
                         X=X_,
@@ -1228,15 +1285,15 @@
         Pool, pool_kwargs = self._get_pool()
         # compute parallel forecasts
         result = {}
         with Pool(self.n_jobs, **pool_kwargs) as executor:
             futures = []
             for ga in gas:
                 future = executor.apply_async(
-                    ga.cross_validation,
+                    ga._single_threaded_cross_validation,
                     tuple(),
                     dict(
                         models=self.models,
                         h=h,
                         test_size=test_size,
                         fallback_model=self.fallback_model,
                         step_size=step_size,
```

### Comparing `statsforecast-1.7.4/statsforecast/distributed/fugue.py` & `statsforecast-1.7.5/statsforecast/distributed/fugue.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/statsforecast/distributed/multiprocess.py` & `statsforecast-1.7.5/statsforecast/distributed/multiprocess.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/statsforecast/ets.py` & `statsforecast-1.7.5/statsforecast/ets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1315,14 +1315,15 @@
     m = obj["m"]
     etsforecast(x=states, m=m, trend=ttype, season=stype, phi=phi, h=h, f=forecast)
     return forecast
 
 # %% ../nbs/src/ets.ipynb 36
 # @njit(nogil=NOGIL, cache=CACHE)
 def _compute_sigmah(pf, h, sigma, cvals):
+
     theta = np.full(h, np.nan)
     theta[0] = pf[0] ** 2
 
     for k in range(1, h):
         sum_val = 0
         for j in range(1, k + 1):
             val = cvals[j - 1] ** 2 * theta[k - j]
@@ -1346,14 +1347,15 @@
     seasonality,
     damped,
     alpha,
     beta,
     gamma,
     phi,
 ):
+
     if damped == "N":
         damped_val = False
     else:
         damped_val = True
 
     p = len(last_state)
 
@@ -1456,19 +1458,15 @@
 
     # parameters
     alpha = model["par"][0]
     beta = model["par"][1]
     gamma = model["par"][2]
     phi = model["par"][3]
 
-    exp1 = (
-        alpha**2
-        + alpha * beta * steps
-        + (1 / 6) * beta**2 * steps * (2 * steps - 1)
-    )
+    exp1 = alpha**2 + alpha * beta * steps + (1 / 6) * beta**2 * steps * (2 * steps - 1)
     exp2 = (beta * phi * steps) / (1 - phi) ** 2
     exp3 = 2 * alpha * (1 - phi) + beta * phi
     exp4 = (beta * phi * (1 - phi**steps)) / ((1 - phi) ** 2 * (1 - phi**2))
     exp5 = 2 * alpha * (1 - phi**2) + beta * phi * (1 + 2 * phi - phi**steps)
 
     compute_intervals = True
     # Class 1 models
```

### Comparing `statsforecast-1.7.4/statsforecast/feature_engineering.py` & `statsforecast-1.7.5/statsforecast/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/statsforecast/garch.py` & `statsforecast-1.7.5/statsforecast/garch.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from scipy.optimize import minimize
 
 from .utils import CACHE, NOGIL
 
 # %% ../nbs/src/garch.ipynb 7
 @njit(nogil=NOGIL, cache=CACHE)
 def generate_garch_data(n, w, alpha, beta):
+
     np.random.seed(1)
 
     y = np.zeros(n)
     sigma2 = np.zeros(n)
 
     p = len(alpha)
     q = len(beta)
@@ -52,14 +53,15 @@
         y[k] = np.random.normal(loc=0, scale=np.sqrt(sigma2[k]))
 
     return y
 
 # %% ../nbs/src/garch.ipynb 12
 @njit(nogil=NOGIL, cache=CACHE)
 def garch_sigma2(x0, x, p, q):
+
     w = x0[0]
     alpha = x0[1 : (p + 1)]
     beta = x0[(p + 1) :]
 
     sigma2 = np.full((len(x),), np.nan)
     sigma2[0] = np.var(x)  # sigma2 can be initialized with the unconditional variance
 
@@ -81,14 +83,15 @@
     # Constraints for GARCH model
     # alpha+beta < 1
     return 1 - (x0[1:].sum())
 
 # %% ../nbs/src/garch.ipynb 16
 @njit(nogil=NOGIL, cache=CACHE)
 def garch_loglik(x0, x, p, q):
+
     sigma2 = garch_sigma2(x0, x, p, q)
     z = x - np.nanmean(x)
     loglik = 0
 
     for k in range(max(p, q), len(z)):
         if sigma2[k] == 0:
             sigma2[k] = 1e-10
@@ -96,14 +99,15 @@
             np.log(2 * np.pi) + np.log(sigma2[k]) + (z[k] ** 2) / sigma2[k]
         )
 
     return -loglik
 
 # %% ../nbs/src/garch.ipynb 18
 def garch_model(x, p, q):
+
     np.random.seed(1)
     x0 = np.repeat(0.1, p + q + 1)
     bnds = ((0, None),) * len(x0)
     cons = {"type": "ineq", "fun": garch_cons}
     opt = minimize(
         garch_loglik, x0, args=(x, p, q), method="SLSQP", bounds=bnds, constraints=cons
     )
@@ -126,14 +130,15 @@
         "fitted": fitted,
     }
 
     return res
 
 # %% ../nbs/src/garch.ipynb 22
 def garch_forecast(mod, h):
+
     np.random.seed(1)
 
     p = mod["p"]
     q = mod["q"]
 
     w = mod["coeff"][0]
     alpha = mod["coeff"][1 : (p + 1)]
```

### Comparing `statsforecast-1.7.4/statsforecast/models.py` & `statsforecast-1.7.5/statsforecast/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,41 +2,44 @@
 
 # %% auto 0
 __all__ = ['AutoARIMA', 'AutoETS', 'ETS', 'AutoCES', 'AutoTheta', 'ARIMA', 'AutoRegressive', 'SimpleExponentialSmoothing',
            'SimpleExponentialSmoothingOptimized', 'SeasonalExponentialSmoothing',
            'SeasonalExponentialSmoothingOptimized', 'Holt', 'HoltWinters', 'HistoricAverage', 'Naive',
            'RandomWalkWithDrift', 'SeasonalNaive', 'WindowAverage', 'SeasonalWindowAverage', 'ADIDA', 'CrostonClassic',
            'CrostonOptimized', 'CrostonSBA', 'IMAPA', 'TSB', 'MSTL', 'TBATS', 'AutoTBATS', 'Theta', 'OptimizedTheta',
-           'DynamicTheta', 'DynamicOptimizedTheta', 'GARCH', 'ARCH', 'ConstantModel', 'ZeroModel', 'NaNModel']
+           'DynamicTheta', 'DynamicOptimizedTheta', 'GARCH', 'ARCH', 'SklearnModel', 'MFLES', 'AutoMFLES',
+           'ConstantModel', 'ZeroModel', 'NaNModel']
 
 # %% ../nbs/src/core/models.ipynb 5
 import warnings
 from math import trunc
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 from numba import njit
 from scipy.optimize import minimize
 from scipy.special import inv_boxcox
 
 from statsforecast.arima import (
     Arima,
     auto_arima_f,
-    forecast_arima,
     fitted_arima,
+    forecast_arima,
     forward_arima,
+    is_constant,
 )
 from .ces import auto_ces, forecast_ces, forward_ces
 from statsforecast.ets import (
     _PHI_LOWER,
     _PHI_UPPER,
     ets_f,
     forecast_ets,
     forward_ets,
 )
+from .mfles import MFLES as _MFLES
 from .mstl import mstl
 from .theta import auto_theta, forecast_theta, forward_theta
 from .garch import garch_model, garch_forecast
 from .tbats import tbats_selection, tbats_forecast, _compute_sigmah
 from statsforecast.utils import (
     _calculate_sigma,
     _calculate_intervals,
@@ -112,14 +115,17 @@
     uses_exog = False
 
     def new(self):
         b = type(self).__new__(type(self))
         b.__dict__.update(self.__dict__)
         return b
 
+    def __repr__(self):
+        return self.alias
+
     def _conformity_scores(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ) -> np.ndarray:
         n_windows = self.prediction_intervals.n_windows  # type: ignore[attr-defined]
         h = self.prediction_intervals.h  # type: ignore[attr-defined]
@@ -320,17 +326,14 @@
         self.allowmean = allowmean
         self.blambda = blambda
         self.biasadj = biasadj
         self.season_length = season_length
         self.alias = alias
         self.prediction_intervals = prediction_intervals
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the AutoARIMA model.
 
@@ -654,17 +657,14 @@
                 raise ValueError("phi must be `None` or float.")
             if not _PHI_LOWER <= phi <= _PHI_UPPER:
                 raise ValueError(f"Valid range for phi is [{_PHI_LOWER}, {_PHI_UPPER}]")
         self.phi = phi
         self.alias = alias
         self.prediction_intervals = prediction_intervals
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the Exponential Smoothing model.
 
@@ -883,17 +883,14 @@
             model=model,
             damped=damped,
             phi=phi,
             alias=alias,
             prediction_intervals=prediction_intervals,
         )
 
-    def __repr__(self):
-        return self.alias
-
 # %% ../nbs/src/core/models.ipynb 53
 class AutoCES(_TS):
     """Complex Exponential Smoothing model.
 
     Automatically selects the best Complex Exponential Smoothing
     model using an information criterion. Default is Akaike Information Criterion (AICc), while particular
     models are estimated using maximum likelihood.
@@ -932,17 +929,14 @@
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         self.season_length = season_length
         self.model = model
         self.alias = alias
         self.prediction_intervals = prediction_intervals
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the Complex Exponential Smoothing model.
 
@@ -957,14 +951,20 @@
             Optional exogenous of shape (t, n_x).
 
         Returns
         -------
         self :
             Complex Exponential Smoothing fitted model.
         """
+        if is_constant(y):
+            model = Naive(
+                alias=self.alias, prediction_intervals=self.prediction_intervals
+            )
+            model.fit(y=y, X=X)
+            return model
         self.model_ = auto_ces(y, m=self.season_length, model=self.model)
         self.model_["actual_residuals"] = y - self.model_["fitted"]
         self._store_cs(y=y, X=X)
         return self
 
     def predict(
         self, h: int, X: Optional[np.ndarray] = None, level: Optional[List[int]] = None
@@ -1051,14 +1051,21 @@
             Whether or not to return insample predictions.
 
         Returns
         -------
         forecasts : dict
             Dictionary with entries `mean` for point predictions and `level_*` for probabilistic predictions.
         """
+        if is_constant(y):
+            model = Naive(
+                alias=self.alias, prediction_intervals=self.prediction_intervals
+            )
+            return model.forecast(
+                y=y, h=h, X=X, X_future=X_future, level=level, fitted=fitted
+            )
         mod = auto_ces(y, m=self.season_length, model=self.model)
         fcst = forecast_ces(mod, h, level=level)
         keys = ["mean"]
         if fitted:
             keys.append("fitted")
         res = {key: fcst[key] for key in keys}
         if level is not None:
@@ -1170,17 +1177,14 @@
     ):
         self.season_length = season_length
         self.decomposition_type = decomposition_type
         self.model = model
         self.alias = alias
         self.prediction_intervals = prediction_intervals
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the AutoTheta model.
 
@@ -1428,17 +1432,14 @@
         self.blambda = blambda
         self.biasadj = biasadj
         self.method = method
         self.fixed = fixed
         self.alias = alias
         self.prediction_intervals = prediction_intervals
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """
         Fit the model to a time series (numpy array) `y`
@@ -1723,17 +1724,14 @@
             biasadj=biasadj,
             method=method,
             alias=alias,
             fixed=fixed,
             prediction_intervals=prediction_intervals,
         )
 
-    def __repr__(self):
-        return self.alias
-
 # %% ../nbs/src/core/models.ipynb 117
 @njit(nogil=NOGIL, cache=CACHE)
 def _ses_fcst_mse(x: np.ndarray, alpha: float) -> Tuple[float, float, np.ndarray]:
     """Perform simple exponential smoothing on a series.
 
     This function returns the one step ahead prediction
     as well as the mean squared error of the fit.
@@ -1847,17 +1845,14 @@
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         self.alpha = alpha
         self.alias = alias
         self.prediction_intervals = prediction_intervals
         self.only_conformal_intervals = True
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the SimpleExponentialSmoothing model.
 
@@ -2006,30 +2001,26 @@
 
     Parameters
     ----------
     alias: str
         Custom name of the model.
     prediction_intervals : Optional[ConformalIntervals]
         Information to compute conformal prediction intervals.
-        By default, the model will compute the native prediction
-        intervals.
+        This is required for generating future prediction intervals.
     """
 
     def __init__(
         self,
         alias: str = "SESOpt",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         self.alias = alias
         self.prediction_intervals = prediction_intervals
         self.only_conformal_intervals = True
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the SimpleExponentialSmoothingOptimized model.
 
@@ -2079,15 +2070,15 @@
         res = {"mean": mean}
         if level is None:
             return res
         level = sorted(level)
         if self.prediction_intervals is not None:
             res = self._add_predict_conformal_intervals(res, level)
         else:
-            raise Exception("You must pass `prediction_intervals` to " "compute them.")
+            raise Exception("You must pass `prediction_intervals` to compute them.")
         return res
 
     def predict_in_sample(self):
         """Access fitted SimpleExponentialSmoothingOptimized insample predictions.
 
         Parameters
         ----------
@@ -2197,16 +2188,15 @@
         Smoothing parameter.
     season_length : int
         Number of observations per unit of time. Ex: 24 Hourly data.
     alias : str
         Custom name of the model.
     prediction_intervals : Optional[ConformalIntervals]
         Information to compute conformal prediction intervals.
-        By default, the model will compute the native prediction
-        intervals.
+        This is required for generating future prediction intervals.
     """
 
     def __init__(
         self,
         season_length: int,
         alpha: float,
         alias: str = "SeasonalES",
@@ -2214,17 +2204,14 @@
     ):
         self.season_length = season_length
         self.alpha = alpha
         self.alias = alias
         self.prediction_intervals = prediction_intervals
         self.only_conformal_intervals = True
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the SeasonalExponentialSmoothing model.
 
@@ -2372,14 +2359,15 @@
     fcst = {"mean": out}
     if fitted:
         fcst["fitted"] = fitted_vals
     return fcst
 
 # %% ../nbs/src/core/models.ipynb 161
 class SeasonalExponentialSmoothingOptimized(_TS):
+
     def __init__(
         self,
         season_length: int,
         alias: str = "SeasESOpt",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         """SeasonalExponentialSmoothingOptimized model.
@@ -2405,25 +2393,21 @@
         ----------
         season_length : int
             Number of observations per unit of time. Ex: 24 Hourly data.
         alias : str
             Custom name of the model.
         prediction_intervals : Optional[ConformalIntervals]
             Information to compute conformal prediction intervals.
-            By default, the model will compute the native prediction
-            intervals.
+            This is required for generating future prediction intervals.
         """
         self.season_length = season_length
         self.alias = alias
         self.prediction_intervals = prediction_intervals
         self.only_conformal_intervals = True
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the SeasonalExponentialSmoothingOptimized model.
 
@@ -2577,26 +2561,24 @@
     def __init__(
         self,
         season_length: int = 1,
         error_type: str = "A",
         alias: str = "Holt",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
+
         self.season_length = season_length
         self.error_type = error_type
         self.alias = alias
         self.prediction_intervals = prediction_intervals
         model = error_type + "AN"
         super().__init__(
             season_length, model, alias=alias, prediction_intervals=prediction_intervals
         )
 
-    def __repr__(self):
-        return self.alias
-
 # %% ../nbs/src/core/models.ipynb 188
 class HoltWinters(AutoETS):
     """Holt-Winters' method.
 
     Also known as triple exponential smoothing, Holt-Winters' method is an extension of exponential smoothing for series that contain both trend and seasonality.
     This implementation returns the corresponding `ETS` model with additive (A) or multiplicative (M) errors (so either 'AAA' or 'MAM').
 
@@ -2629,31 +2611,29 @@
         self.error_type = error_type
         self.alias = alias
         model = error_type + "A" + error_type
         super().__init__(
             season_length, model, alias=alias, prediction_intervals=prediction_intervals
         )
 
-    def __repr__(self):
-        return self.alias
-
 # %% ../nbs/src/core/models.ipynb 203
 def _historic_average(
     y: np.ndarray,  # time series
     h: int,  # forecasting horizon
     fitted: bool,  # fitted values
 ) -> Dict[str, np.ndarray]:
     fcst = {"mean": _repeat_val(val=y.mean(), h=h)}
     if fitted:
         fitted_vals = _repeat_val(val=y.mean(), h=len(y))
         fcst["fitted"] = fitted_vals
     return fcst
 
 # %% ../nbs/src/core/models.ipynb 204
 class HistoricAverage(_TS):
+
     def __init__(
         self,
         alias: str = "HistoricAverage",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         """HistoricAverage model.
 
@@ -2673,17 +2653,14 @@
             Information to compute conformal prediction intervals.
             By default, the model will compute the native prediction
             intervals.
         """
         self.alias = alias
         self.prediction_intervals = prediction_intervals
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the HistoricAverage model.
 
@@ -2824,14 +2801,15 @@
                 sigmah = sigma * np.sqrt(1 + (1 / len(y)))
                 res = _add_fitted_pi(res=res, se=sigmah, level=level)
 
         return res
 
 # %% ../nbs/src/core/models.ipynb 217
 class Naive(_TS):
+
     def __init__(
         self,
         alias: str = "Naive",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         """Naive model.
 
@@ -2850,17 +2828,14 @@
             Information to compute conformal prediction intervals.
             By default, the model will compute the native prediction
             intervals.
         """
         self.alias = alias
         self.prediction_intervals = prediction_intervals
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the Naive model.
 
@@ -3052,14 +3027,15 @@
         fitted_vals = np.full(y.size, np.nan, dtype=np.float32)
         fitted_vals[1:] = (slope + y[:-1]).astype(np.float32)
         fcst["fitted"] = fitted_vals
     return fcst
 
 # %% ../nbs/src/core/models.ipynb 234
 class RandomWalkWithDrift(_TS):
+
     def __init__(
         self,
         alias: str = "RWD",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         """RandomWalkWithDrift model.
 
@@ -3083,17 +3059,14 @@
             Information to compute conformal prediction intervals.
             By default, the model will compute the native prediction
             intervals.
         """
         self.alias = alias
         self.prediction_intervals = prediction_intervals
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the RandomWalkWithDrift model.
 
@@ -3230,14 +3203,15 @@
                 sigma = _calculate_sigma(residuals, len(residuals) - 1)
                 res = _add_fitted_pi(res=res, se=sigma, level=level)
 
         return res
 
 # %% ../nbs/src/core/models.ipynb 249
 class SeasonalNaive(_TS):
+
     def __init__(
         self,
         season_length: int,
         alias: str = "SeasonalNaive",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         """Seasonal naive model.
@@ -3259,17 +3233,14 @@
             By default, the model will compute the native prediction
             intervals.
         """
         self.season_length = season_length
         self.alias = alias
         self.prediction_intervals = prediction_intervals
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the SeasonalNaive model.
 
@@ -3433,14 +3404,15 @@
         return {"mean": np.full(h, np.nan, np.float32)}
     wavg = y[-window_size:].mean()
     mean = _repeat_val(val=wavg, h=h)
     return {"mean": mean}
 
 # %% ../nbs/src/core/models.ipynb 265
 class WindowAverage(_TS):
+
     def __init__(
         self,
         window_size: int,
         alias: str = "WindowAverage",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         """WindowAverage model.
@@ -3458,25 +3430,21 @@
         ----------
         window_size : int
             Size of truncated series on which average is estimated.
         alias : str
             Custom name of the model.
         prediction_intervals : Optional[ConformalIntervals]
             Information to compute conformal prediction intervals.
-            By default, the model will compute the native prediction
-            intervals.
+            This is required for generating future prediction intervals.
         """
         self.window_size = window_size
         self.alias = alias
         self.prediction_intervals = prediction_intervals
         self.only_conformal_intervals = True
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the WindowAverage model.
 
@@ -3587,15 +3555,15 @@
         res = dict(res)
         if level is None:
             return res
         level = sorted(level)
         if self.prediction_intervals is not None:
             res = self._add_conformal_intervals(fcst=res, y=y, X=X, level=level)
         else:
-            raise Exception("You must pass `prediction_intervals` to " "compute them.")
+            raise Exception("You must pass `prediction_intervals` to compute them.")
         return res
 
 # %% ../nbs/src/core/models.ipynb 276
 def _seasonal_window_average(
     y: np.ndarray,
     h: int,
     fitted: bool,
@@ -3609,14 +3577,15 @@
         return {"mean": np.full(h, np.nan, np.float32)}
     season_avgs = y[-min_samples:].reshape(window_size, season_length).mean(axis=0)
     out = _repeat_val_seas(season_vals=season_avgs, h=h)
     return {"mean": out}
 
 # %% ../nbs/src/core/models.ipynb 277
 class SeasonalWindowAverage(_TS):
+
     def __init__(
         self,
         season_length: int,
         window_size: int,
         alias: str = "SeasWA",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
@@ -3634,26 +3603,22 @@
             Size of truncated series on which average is estimated.
         seasonal_length : int
             Number of observations per cycle.
         alias : str
             Custom name of the model.
         prediction_intervals : Optional[ConformalIntervals]
             Information to compute conformal prediction intervals.
-            By default, the model will compute the native prediction
-            intervals.
+            This is required for generating future prediction intervals.
         """
         self.season_length = season_length
         self.window_size = window_size
         self.alias = alias
         self.prediction_intervals = prediction_intervals
         self.only_conformal_intervals = True
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the SeasonalWindowAverage model.
 
@@ -3865,14 +3830,15 @@
             sums_fitted[i] = _chunk_forecast(y[: i + 1], agg_lvl)
 
         res["fitted"] = np.append(np.nan, sums_fitted / fitted_aggregation_levels)
     return res
 
 # %% ../nbs/src/core/models.ipynb 290
 class ADIDA(_TS):
+
     def __init__(
         self,
         alias: str = "ADIDA",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         """ADIDA model.
 
@@ -3898,17 +3864,14 @@
             By default, the model will compute the native prediction
             intervals.
         """
         self.alias = alias
         self.prediction_intervals = prediction_intervals
         self.only_conformal_intervals = True
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the ADIDA model.
 
@@ -4062,14 +4025,15 @@
         ydf = _expand_fitted_demand(np.append(ydf, ydp), y)
         yif = _expand_fitted_intervals(np.append(yif, yip), y)
         out["fitted"] = ydf / yif
     return out
 
 # %% ../nbs/src/core/models.ipynb 303
 class CrostonClassic(_TS):
+
     def __init__(
         self,
         alias: str = "CrostonClassic",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         """CrostonClassic model.
 
@@ -4094,17 +4058,14 @@
             By default, the model will compute the native prediction
             intervals.
         """
         self.alias = alias
         self.prediction_intervals = prediction_intervals
         self.only_conformal_intervals = True
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the CrostonClassic model.
 
@@ -4268,14 +4229,15 @@
         ydf = _expand_fitted_demand(ydf, y)
         yif = _expand_fitted_intervals(yif, y)
         out["fitted"] = ydf / yif
     return out
 
 # %% ../nbs/src/core/models.ipynb 315
 class CrostonOptimized(_TS):
+
     def __init__(
         self,
         alias: str = "CrostonOptimized",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         """CrostonOptimized model.
 
@@ -4294,24 +4256,20 @@
 
         Parameters
         ----------
         alias : str
             Custom name of the model.
         prediction_intervals : Optional[ConformalIntervals]
             Information to compute conformal prediction intervals.
-            By default, the model will compute the native prediction
-            intervals.
+            This is required for generating future prediction intervals.
         """
         self.alias = alias
         self.prediction_intervals = prediction_intervals
         self.only_conformal_intervals = True
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the CrostonOptimized model.
 
@@ -4442,14 +4400,15 @@
     out["mean"] *= 0.95
     if fitted:
         out["fitted"] *= 0.95
     return out
 
 # %% ../nbs/src/core/models.ipynb 327
 class CrostonSBA(_TS):
+
     def __init__(
         self,
         alias: str = "CrostonSBA",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         """CrostonSBA model.
 
@@ -4475,17 +4434,14 @@
             By default, the model will compute the native prediction
             intervals.
         """
         self.alias = alias
         self.prediction_intervals = prediction_intervals
         self.only_conformal_intervals = True
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the CrostonSBA model.
 
@@ -4642,14 +4598,15 @@
         for i in range(y.size - 1):
             fitted_vals[i + 1] = _imapa(y[: i + 1], h=1, fitted=False)["mean"].item()
         res["fitted"] = fitted_vals
     return res
 
 # %% ../nbs/src/core/models.ipynb 339
 class IMAPA(_TS):
+
     def __init__(
         self,
         alias: str = "IMAPA",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         """IMAPA model.
 
@@ -4671,17 +4628,14 @@
             By default, the model will compute the native prediction
             intervals.
         """
         self.alias = alias
         self.prediction_intervals = prediction_intervals
         self.only_conformal_intervals = True
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the IMAPA model.
 
@@ -4832,14 +4786,15 @@
     if fitted:
         ydft = _expand_fitted_demand(np.append(ydft, ydf), y)
         res["fitted"] = ypft * ydft
     return res
 
 # %% ../nbs/src/core/models.ipynb 351
 class TSB(_TS):
+
     def __init__(
         self,
         alpha_d: float,
         alpha_p: float,
         alias: str = "TSB",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
@@ -4872,26 +4827,22 @@
             Smoothing parameter for demand.
         alpha_p : float
             Smoothing parameter for probability.
         alias : str
             Custom name of the model.
         prediction_intervals : Optional[ConformalIntervals]
             Information to compute conformal prediction intervals.
-            By default, the model will compute the native prediction
-            intervals.
+            This is required for generating future prediction intervals.
         """
         self.alpha_d = alpha_d
         self.alpha_p = alpha_p
         self.alias = alias
         self.prediction_intervals = prediction_intervals
         self.only_conformal_intervals = True
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the TSB model.
 
@@ -4938,15 +4889,15 @@
         res = {"mean": mean}
         if level is None:
             return res
         level = sorted(level)
         if self.prediction_intervals is not None:
             res = self._add_predict_conformal_intervals(res, level)
         else:
-            raise Exception("You must pass `prediction_intervals` to " "compute them.")
+            raise Exception("You must pass `prediction_intervals` to compute them.")
         return res
 
     def predict_in_sample(self, level: Optional[List[int]] = None):
         """Access fitted TSB insample predictions.
 
         Parameters
         ----------
@@ -5060,14 +5011,15 @@
         self,
         season_length: Union[int, List[int]],
         trend_forecaster=AutoETS(model="ZZN"),
         stl_kwargs: Optional[Dict] = None,
         alias: str = "MSTL",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
+
         # check ETS model doesnt have seasonality
         if repr(trend_forecaster) == "AutoETS":
             if trend_forecaster.model[2] != "N":
                 raise Exception(
                     "Trend forecaster should not adjust " "seasonal models."
                 )
         # check if trend forecaster has season_length=1
@@ -5089,17 +5041,14 @@
 
         if self.trend_forecaster.prediction_intervals is None and (
             self.prediction_intervals is not None
         ):
             self.trend_forecaster.prediction_intervals = prediction_intervals
         self.stl_kwargs = dict() if stl_kwargs is None else stl_kwargs
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the MSTL model.
 
@@ -5361,17 +5310,14 @@
         self.bc_lower_bound = bc_lower_bound
         self.bc_upper_bound = bc_upper_bound
         self.use_trend = use_trend
         self.use_damped_trend = use_damped_trend
         self.use_arma_errors = use_arma_errors
         self.alias = alias
 
-    def __repr__(self):
-        return self.alias
-
     def fit(self, y: np.ndarray, X: Optional[np.ndarray] = None):
         """Fit TBATS model.
 
         Fit TBATS model to a time series (numpy array) `y`.
 
         Parameters
         ----------
@@ -5782,17 +5728,14 @@
         self.q = q
         if q != 0:
             self.alias = alias + "(" + str(p) + "," + str(q) + ")"
         else:
             self.alias = alias + "(" + str(p) + ")"
         self.prediction_intervals = prediction_intervals
 
-    def __repr__(self):
-        return self.alias
-
     def fit(self, y: np.ndarray, X: Optional[np.ndarray] = None):
         """Fit GARCH model.
 
         Fit GARCH model to a time series (numpy array) `y`.
 
         Parameters
         ----------
@@ -5963,19 +5906,700 @@
         alias: str = "ARCH",
         prediction_intervals: Optional[ConformalIntervals] = None,
     ):
         self.p = p
         self.alias = alias
         super().__init__(p, q=0, alias=alias)
 
-    def __repr__(self):
-        return self.alias
-
 # %% ../nbs/src/core/models.ipynb 479
+class SklearnModel(_TS):
+    """scikit-learn model wrapper
+
+    Parameters
+    ----------
+    model : sklearn.base.BaseEstimator
+        scikit-learn estimator
+    prediction_intervals : Optional[ConformalIntervals]
+        Information to compute conformal prediction intervals.
+        This is required for generating future prediction intervals.
+    alias : str, optional (default=None)
+        Custom name of the model. If `None` will use the model's class.
+    """
+
+    def __init__(
+        self,
+        model,
+        prediction_intervals: Optional[ConformalIntervals] = None,
+        alias: Optional[str] = None,
+    ):
+        self.model = model
+        self.prediction_intervals = prediction_intervals
+        self.alias = alias if alias is not None else model.__class__.__name__
+
+    def fit(
+        self,
+        y: np.ndarray,
+        X: np.ndarray,
+    ) -> "SklearnModel":
+        """Fit the model.
+
+        Parameters
+        ----------
+        y : numpy.array
+            Clean time series of shape (t, ).
+        X : array-like
+            Exogenous of shape (t, n_x).
+
+        Returns
+        -------
+        self : SklearnModel
+            Fitted SklearnModel object.
+        """
+        from sklearn.base import clone
+
+        self.model_ = {"model": clone(self.model)}
+        self.model_["model"].fit(X, y)
+        self._store_cs(y=y, X=X)
+        self.model_["fitted"] = self.model_["model"].predict(X)
+        residuals = y - self.model_["fitted"]
+        self.model_["sigma"] = _calculate_sigma(residuals, y.size)
+        return self
+
+    def predict(
+        self,
+        h: int,
+        X: np.ndarray,
+        level: Optional[List[int]] = None,
+    ) -> Dict[str, Any]:
+        """Predict with fitted SklearnModel.
+
+        Parameters
+        ----------
+        h : int
+            Forecast horizon.
+        X : array-like
+            Exogenous of shape (h, n_x).
+        level: List[int]
+            Confidence levels (0-100) for prediction intervals.
+
+        Returns
+        -------
+        forecasts : dict
+            Dictionary with entries `mean` for point predictions and `level_*` for probabilistic predictions.
+        """
+        res = {"mean": self.model_["model"].predict(X)}
+        if level is None:
+            return res
+        level = sorted(level)
+        if self.prediction_intervals is not None:
+            res = self._add_predict_conformal_intervals(res, level)
+        else:
+            raise Exception("You must pass `prediction_intervals` to compute them.")
+        return res
+
+    def predict_in_sample(self, level: Optional[List[int]] = None) -> Dict[str, Any]:
+        """Access fitted SklearnModel insample predictions.
+
+        Parameters
+        ----------
+        level : List[int]
+            Confidence levels (0-100) for prediction intervals.
+
+        Returns
+        -------
+        forecasts : dict
+            Dictionary with entries `fitted` for point predictions and `level_*` for probabilistic predictions.
+        """
+        res = {"fitted": self.model_["fitted"]}
+        if level is not None:
+            level = sorted(level)
+            res = _add_fitted_pi(res=res, se=self.model_["sigma"], level=level)
+        return res
+
+    def forecast(
+        self,
+        y: np.ndarray,
+        h: int,
+        X: np.ndarray,
+        X_future: np.ndarray,
+        level: Optional[List[int]] = None,
+        fitted: bool = False,
+    ) -> Dict[str, Any]:
+        """Memory Efficient SklearnModel predictions.
+
+        This method avoids memory burden due from object storage.
+        It is analogous to `fit_predict` without storing information.
+        It assumes you know the forecast horizon in advance.
+
+        Parameters
+        ----------
+        y : numpy.array
+            Clean time series of shape (t, ).
+        h : int
+            Forecast horizon.
+        X : array-like
+            Insample exogenous of shape (t, n_x).
+        X_future : array-like
+            Exogenous of shape (h, n_x).
+        level : List[int]
+            Confidence levels (0-100) for prediction intervals.
+        fitted : bool
+            Whether or not to return insample predictions.
+
+        Returns
+        -------
+        forecasts : dict
+            Dictionary with entries `mean` for point predictions and `level_*` for probabilistic predictions.
+        """
+        from sklearn.base import clone
+
+        model = clone(self.model)
+        model.fit(X, y)
+        res = {"mean": model.predict(X_future)}
+        if fitted:
+            res["fitted"] = model.predict(X)
+        if level is not None:
+            level = sorted(level)
+            if self.prediction_intervals is not None:
+                res = self._add_conformal_intervals(fcst=res, y=y, X=X, level=level)
+            else:
+                raise Exception("You must pass `prediction_intervals` to compute them.")
+            if fitted:
+                residuals = y - res["fitted"]
+                sigma = _calculate_sigma(residuals, y.size)
+                res = _add_fitted_pi(res=res, se=sigma, level=level)
+        return res
+
+    def forward(
+        self,
+        y: np.ndarray,
+        h: int,
+        X: np.ndarray,
+        X_future: np.ndarray,
+        level: Optional[List[int]] = None,
+        fitted: bool = False,
+    ):
+        """Apply fitted SklearnModel to a new/updated time series.
+
+        Parameters
+        ----------
+        y : numpy.array
+            Clean time series of shape (t, ).
+        h : int
+            Forecast horizon.
+        X : array-like
+            Insample exogenous of shape (t, n_x).
+        X_future : array-like
+            Exogenous of shape (h, n_x).
+        level : List[float]
+            Confidence levels for prediction intervals.
+        fitted : bool
+            Whether or not returns insample predictions.
+
+        Returns
+        -------
+        forecasts : dict
+            Dictionary with entries `constant` for point predictions and `level_*` for probabilistic predictions.
+        """
+        if not hasattr(self, "model_"):
+            raise Exception("You have to use the `fit` method first")
+        res = {"mean": self.model_["model"].predict(X_future)}
+        if fitted:
+            res["fitted"] = self.model_["model"].predict(X)
+        if level is not None:
+            level = sorted(level)
+            if self.prediction_intervals is not None:
+                res = self._add_conformal_intervals(fcst=res, y=y, X=X, level=level)
+            else:
+                raise Exception("You must pass `prediction_intervals` to compute them.")
+            if fitted:
+                se = _calculate_sigma(y - res["fitted"], y.size)
+                res = _add_fitted_pi(res=res, se=se, level=level)
+        return res
+
+# %% ../nbs/src/core/models.ipynb 489
+class MFLES(_TS):
+    """MFLES model.
+
+    A method to forecast time series based on Gradient Boosted Time Series Decomposition
+    which treats traditional decomposition as the base estimator in the boosting
+    process. Unlike normal gradient boosting, slight learning rates are applied at the
+    component level (trend/seasonality/exogenous).
+
+    The method derives its name from some of the underlying estimators that can
+    enter into the boosting procedure, specifically: a simple Median, Fourier
+    functions for seasonality, a simple/piecewise Linear trend, and Exponential
+    Smoothing.
+
+    Parameters
+    ----------
+    season_length : int or list of int, optional (default=None)
+        Number of observations per unit of time. Ex: 24 Hourly data.
+    fourier_order : int, optional (default=None)
+        How many fourier sin/cos pairs to create, the larger the number the more complex of a seasonal pattern can be fitted.
+        A lower number leads to smoother results.
+        This is auto-set based on seasonal_period.
+    max_rounds : int (default=50)
+        The max number of boosting rounds. The boosting will auto-stop but depending on other parameters such as rs_lr you may want more rounds.
+        Generally more rounds means a smoother fit.
+    ma : int, optional (default=None)
+        The moving average order to use, this is auto-set based on internal logic.
+        Passing 4 would fit a 4 period moving average on the residual component.
+    alpha : float (default=1.0)
+        The alpha which is used in fitting the underlying LASSO when using piecewise functions.
+    decay : float (default=-1.0)
+        Effects the slopes of the piecewise-linear basis function.
+    changepoints : boolean (default=True)
+        Whether to fit for changepoints if all other logic allows for it. If False, MFLES will not ever fit a piecewise trend.
+    n_changepoints : int or float (default=0.25)
+        Number (if int) or proportion (if float) of changepoint knots to place. The default of 0.25 will place 0.25 * (series length) number of knots.
+    seasonal_lr : float (default=0.9)
+        A shrinkage parameter (0 < seasonal_lr <= 1) which penalizes the seasonal fit.
+        A value of 0.9 will flatly multiply the seasonal fit by 0.9 each boosting round, this can be used to allow more signal to the exogenous component.
+    trend_lr : float (default=0.9)
+        A shrinkage parameter (0 < trend_lr <= 1) which penalizes the linear trend fit
+        A value of 0.9 will flatly multiply the linear fit by 0.9 each boosting round, this can be used to allow more signal to the seasonality or exogenous components.
+    exogenous_lr : float (default=1.0)
+        The shrinkage parameter (0 < exogenous_lr <= 1) which controls how much of the exogenous signal is carried to the next round.
+    residuals_lr : float (default=1.0)
+        A shrinkage parameter (0 < residuals_lr <= 1) which penalizes the residual smoothing.
+        A value of 0.9 will flatly multiply the residual fit by 0.9 each boosting round, this can be used to allow more signal to the seasonality or linear components.
+    cov_threshold : float (default=0.7)
+        The deseasonalized cov is used to auto-set some logic, lowering the cov_threshold will result in simpler and less complex residual smoothing.
+        If you pass something like 1000 then there will be no safeguards applied.
+    moving_medians : bool (default=False)
+        The default behavior is to fit an initial median to the time series. If True, then it will fit a median per seasonal period.
+    min_alpha : float (default=0.05)
+        The minimum alpha in the SES ensemble.
+    max_alpha : float (default=1.0)
+        The maximum alpha used in the SES ensemble.
+    trend_penalty : bool (default=True)
+        Whether to apply a simple penalty to the linear trend component, very useful for dealing with the potentially dangerous piecewise trend.
+    multiplicative : bool, optional (default=None)
+        Auto-set based on internal logic. If True, it will simply take the log of the time series.
+    smoother : bool (default=False)
+        If True, then a simple exponential ensemble will be used rather than auto settings.
+    robust : bool, optional (default=None)
+        If True then MFLES will fit using more reserved methods, i.e. not using piecewise trend or moving average residual smoother.
+        Auto-set based on internal logic.
+    verbose : bool (default=False)
+        Print debugging information.
+    prediction_intervals : Optional[ConformalIntervals]
+        Information to compute conformal prediction intervals.
+        This is required for generating future prediction intervals.
+    alias : str (default='MFLES')
+        Custom name of the model.
+    """
+
+    def __init__(
+        self,
+        season_length: Optional[Union[int, List[int]]] = None,
+        fourier_order: Optional[int] = None,
+        max_rounds: int = 50,
+        ma: Optional[int] = None,
+        alpha: float = 1.0,
+        decay: float = -1.0,
+        changepoints: bool = True,
+        n_changepoints: Union[float, int] = 0.25,
+        seasonal_lr: float = 0.9,
+        trend_lr: float = 0.9,
+        exogenous_lr: float = 1.0,
+        residuals_lr: float = 1.0,
+        cov_threshold: float = 0.7,
+        moving_medians: bool = False,
+        min_alpha: float = 0.05,
+        max_alpha: float = 1.0,
+        trend_penalty: bool = True,
+        multiplicative: Optional[bool] = None,
+        smoother: bool = False,
+        robust: Optional[bool] = None,
+        verbose: bool = False,
+        prediction_intervals: Optional[ConformalIntervals] = None,
+        alias: str = "MFLES",
+    ):
+        try:
+            import sklearn  # noqa: F401
+        except ImportError:
+            raise ImportError("MFLES requires scikit-learn.") from None
+        self.season_length = season_length
+        self.fourier_order = fourier_order
+        self.max_rounds = max_rounds
+        self.ma = ma
+        self.alpha = alpha
+        self.decay = decay
+        self.changepoints = changepoints
+        self.n_changepoints = n_changepoints
+        self.seasonal_lr = seasonal_lr
+        self.trend_lr = trend_lr
+        self.exogenous_lr = exogenous_lr
+        self.residuals_lr = residuals_lr
+        self.cov_threshold = cov_threshold
+        self.moving_medians = moving_medians
+        self.min_alpha = min_alpha
+        self.max_alpha = max_alpha
+        self.trend_penalty = trend_penalty
+        self.multiplicative = multiplicative
+        self.smoother = smoother
+        self.robust = robust
+        self.verbose = verbose
+        self.prediction_intervals = prediction_intervals
+        self.alias = alias
+
+    def _fit(self, y: np.ndarray, X: Optional[np.ndarray]) -> Dict[str, Any]:
+        model = _MFLES(verbose=self.verbose, robust=self.robust)
+        fitted = model.fit(
+            y=y,
+            X=X,
+            seasonal_period=self.season_length,
+            fourier_order=self.fourier_order,
+            ma=self.ma,
+            alpha=self.alpha,
+            decay=self.decay,
+            n_changepoints=self.n_changepoints,
+            seasonal_lr=self.seasonal_lr,
+            linear_lr=self.trend_lr,
+            exogenous_lr=self.exogenous_lr,
+            rs_lr=self.residuals_lr,
+            cov_threshold=self.cov_threshold,
+            moving_medians=self.moving_medians,
+            max_rounds=self.max_rounds,
+            min_alpha=self.min_alpha,
+            max_alpha=self.max_alpha,
+            trend_penalty=self.trend_penalty,
+            multiplicative=self.multiplicative,
+            changepoints=self.changepoints,
+            smoother=self.smoother,
+        )
+        return {"model": model, "fitted": fitted}
+
+    def fit(self, y: np.ndarray, X: Optional[np.ndarray] = None) -> "MFLES":
+        """Fit the model
+
+        Parameters
+        ----------
+        y : numpy.array
+            Clean time series of shape (t, ).
+        X : array-like, optional (default=None)
+            Exogenous of shape (t, n_x).
+
+        Returns
+        -------
+        self : MFLES
+            Fitted MFLES object.
+        """
+        self.model_ = self._fit(y=y, X=X)
+        self._store_cs(y=y, X=X)
+        residuals = y - self.model_["fitted"]
+        self.model_["sigma"] = _calculate_sigma(residuals, y.size)
+        return self
+
+    def predict(
+        self,
+        h: int,
+        X: Optional[np.ndarray] = None,
+        level: Optional[List[int]] = None,
+    ) -> Dict[str, Any]:
+        """Predict with fitted MFLES.
+
+        Parameters
+        ----------
+        h : int
+            Forecast horizon.
+        X : array-like, optional (default=None)
+            Exogenous of shape (h, n_x).
+        level: List[int]
+            Confidence levels (0-100) for prediction intervals.
+
+        Returns
+        -------
+        forecasts : dict
+            Dictionary with entries `mean` for point predictions and `level_*` for probabilistic predictions.
+        """
+        res = {"mean": self.model_["model"].predict(forecast_horizon=h, X=X)}
+        if level is None:
+            return res
+        level = sorted(level)
+        if self.prediction_intervals is not None:
+            res = self._add_predict_conformal_intervals(res, level)
+        else:
+            raise Exception("You must pass `prediction_intervals` to compute them.")
+        return res
+
+    def predict_in_sample(self, level: Optional[List[int]] = None) -> Dict[str, Any]:
+        """Access fitted SklearnModel insample predictions.
+
+        Parameters
+        ----------
+        level : List[int]
+            Confidence levels (0-100) for prediction intervals.
+
+        Returns
+        -------
+        forecasts : dict
+            Dictionary with entries `fitted` for point predictions and `level_*` for probabilistic predictions.
+        """
+        res = {"fitted": self.model_["fitted"]}
+        if level is not None:
+            level = sorted(level)
+            res = _add_fitted_pi(res=res, se=self.model_["sigma"], level=level)
+        return res
+
+    def forecast(
+        self,
+        y: np.ndarray,
+        h: int,
+        X: Optional[np.ndarray] = None,
+        X_future: Optional[np.ndarray] = None,
+        level: Optional[List[int]] = None,
+        fitted: bool = False,
+    ) -> Dict[str, Any]:
+        """Memory Efficient MFLES predictions.
+
+        This method avoids memory burden due from object storage.
+        It is analogous to `fit_predict` without storing information.
+        It assumes you know the forecast horizon in advance.
+
+        Parameters
+        ----------
+        y : numpy.array
+            Clean time series of shape (t, ).
+        h : int
+            Forecast horizon.
+        X : array-like
+            Insample exogenous of shape (t, n_x).
+        X_future : array-like
+            Exogenous of shape (h, n_x).
+        level : List[int]
+            Confidence levels (0-100) for prediction intervals.
+        fitted : bool
+            Whether or not to return insample predictions.
+
+        Returns
+        -------
+        forecasts : dict
+            Dictionary with entries `mean` for point predictions and `level_*` for probabilistic predictions.
+        """
+        model = self._fit(y=y, X=X)
+        res = {"mean": model["model"].predict(forecast_horizon=h, X=X_future)}
+        if fitted:
+            res["fitted"] = model["fitted"]
+        if level is not None:
+            level = sorted(level)
+            if self.prediction_intervals is not None:
+                res = self._add_conformal_intervals(fcst=res, y=y, X=X, level=level)
+            else:
+                raise Exception("You must pass `prediction_intervals` to compute them.")
+            if fitted:
+                residuals = y - res["fitted"]
+                sigma = _calculate_sigma(residuals, y.size)
+                res = _add_fitted_pi(res=res, se=sigma, level=level)
+        return res
+
+# %% ../nbs/src/core/models.ipynb 497
+class AutoMFLES(_TS):
+    """AutoMFLES
+
+    Parameters
+    ----------
+    test_size : int
+        Forecast horizon used during cross validation.
+    season_length : int or list of int, optional (default=None)
+        Number of observations per unit of time. Ex: 24 Hourly data.
+    n_windows : int (default=2)
+        Number of windows used for cross validation.
+    config : dict, optional (default=None)
+        Mapping from parameter name (from the init arguments of MFLES) to a list of values to try.
+        If `None`, will use defaults.
+    step_size : int, optional (default=None)
+        Step size between each cross validation window. If `None` will be set to test_size.
+    metric : str (default='smape')
+        Metric used to select the best model. Possible options are: 'smape', 'mape', 'mse' and 'mae'.
+    verbose : bool (default=False)
+        Print debugging information.
+    prediction_intervals : Optional[ConformalIntervals]
+        Information to compute conformal prediction intervals.
+        This is required for generating future prediction intervals.
+    alias : str (default='AutoMFLES')
+        Custom name of the model.
+    """
+
+    def __init__(
+        self,
+        test_size: int,
+        season_length: Optional[Union[int, List[int]]] = None,
+        n_windows: int = 2,
+        config: Optional[Dict[str, Any]] = None,
+        step_size: Optional[int] = None,
+        metric: str = "smape",
+        verbose: bool = False,
+        prediction_intervals: Optional[ConformalIntervals] = None,
+        alias: str = "AutoMFLES",
+    ):
+        try:
+            import sklearn  # noqa: F401
+        except ImportError:
+            raise ImportError("MFLES requires scikit-learn.") from None
+        self.season_length = season_length
+        self.n_windows = n_windows
+        self.test_size = test_size
+        self.config = config
+        self.step_size = step_size if step_size is not None else test_size
+        self.metric = metric
+        self.verbose = verbose
+        self.prediction_intervals = prediction_intervals
+        self.alias = alias
+
+    def _fit(self, y: np.ndarray, X: Optional[np.ndarray] = None) -> Dict[str, Any]:
+        model = _MFLES(verbose=self.verbose)
+        optim_params = model.optimize(
+            y=y,
+            X=X,
+            test_size=self.test_size,
+            n_steps=self.n_windows,
+            step_size=self.step_size,
+            seasonal_period=self.season_length,
+            metric=self.metric,
+            params=self.config,
+        )
+        # the seasonal_period may've been found during the optimization
+        seasonal_period = optim_params.pop("seasonal_period", self.season_length)
+        fitted = model.fit(
+            y=y,
+            X=X,
+            seasonal_period=seasonal_period,
+            **optim_params,
+        )
+        return {"model": model, "fitted": fitted}
+
+    def fit(self, y: np.ndarray, X: Optional[np.ndarray] = None) -> "AutoMFLES":
+        """Fit the model
+
+        Parameters
+        ----------
+        y : numpy.array
+            Clean time series of shape (t, ).
+        X : array-like, optional (default=None)
+            Exogenous of shape (t, n_x).
+
+        Returns
+        -------
+        self : AutoMFLES
+            Fitted AutoMFLES object.
+        """
+        self.model_ = self._fit(y=y, X=X)
+        self._store_cs(y=y, X=X)
+        residuals = y - self.model_["fitted"]
+        self.model_["sigma"] = _calculate_sigma(residuals, y.size)
+        return self
+
+    def predict(
+        self,
+        h: int,
+        X: Optional[np.ndarray] = None,
+        level: Optional[List[int]] = None,
+    ) -> Dict[str, Any]:
+        """Predict with fitted AutoMFLES.
+
+        Parameters
+        ----------
+        h : int
+            Forecast horizon.
+        X : array-like, optional (default=None)
+            Exogenous of shape (h, n_x).
+        level: List[int]
+            Confidence levels (0-100) for prediction intervals.
+
+        Returns
+        -------
+        forecasts : dict
+            Dictionary with entries `mean` for point predictions and `level_*` for probabilistic predictions.
+        """
+        res = {"mean": self.model_["model"].predict(forecast_horizon=h, X=X)}
+        if level is None:
+            return res
+        level = sorted(level)
+        if self.prediction_intervals is not None:
+            res = self._add_predict_conformal_intervals(res, level)
+        else:
+            raise Exception("You must pass `prediction_intervals` to compute them.")
+        return res
+
+    def predict_in_sample(self, level: Optional[List[int]] = None) -> Dict[str, Any]:
+        """Access fitted AutoMFLES insample predictions.
+
+        Parameters
+        ----------
+        level : List[int]
+            Confidence levels (0-100) for prediction intervals.
+
+        Returns
+        -------
+        forecasts : dict
+            Dictionary with entries `fitted` for point predictions and `level_*` for probabilistic predictions.
+        """
+        res = {"fitted": self.model_["fitted"]}
+        if level is not None:
+            level = sorted(level)
+            res = _add_fitted_pi(res=res, se=self.model_["sigma"], level=level)
+        return res
+
+    def forecast(
+        self,
+        y: np.ndarray,
+        h: int,
+        X: Optional[np.ndarray] = None,
+        X_future: Optional[np.ndarray] = None,
+        level: Optional[List[int]] = None,
+        fitted: bool = False,
+    ) -> Dict[str, Any]:
+        """Memory Efficient AutoMFLES predictions.
+
+        This method avoids memory burden due from object storage.
+        It is analogous to `fit_predict` without storing information.
+        It assumes you know the forecast horizon in advance.
+
+        Parameters
+        ----------
+        y : numpy.array
+            Clean time series of shape (t, ).
+        h : int
+            Forecast horizon.
+        X : array-like
+            Insample exogenous of shape (t, n_x).
+        X_future : array-like
+            Exogenous of shape (h, n_x).
+        level : List[int]
+            Confidence levels (0-100) for prediction intervals.
+        fitted : bool
+            Whether or not to return insample predictions.
+
+        Returns
+        -------
+        forecasts : dict
+            Dictionary with entries `mean` for point predictions and `level_*` for probabilistic predictions.
+        """
+        model = self._fit(y=y, X=X)
+        res = {"mean": model["model"].predict(forecast_horizon=h, X=X_future)}
+        if fitted:
+            res["fitted"] = model["fitted"]
+        if level is not None:
+            level = sorted(level)
+            if self.prediction_intervals is not None:
+                res = self._add_conformal_intervals(fcst=res, y=y, X=X, level=level)
+            else:
+                raise Exception("You must pass `prediction_intervals` to compute them.")
+            if fitted:
+                residuals = y - res["fitted"]
+                sigma = _calculate_sigma(residuals, y.size)
+                res = _add_fitted_pi(res=res, se=sigma, level=level)
+        return res
+
+# %% ../nbs/src/core/models.ipynb 501
 class ConstantModel(_TS):
+
     def __init__(self, constant: float, alias: str = "ConstantModel"):
         """Constant Model.
 
         Returns Constant values.
 
         Parameters
         ----------
@@ -5983,17 +6607,14 @@
             Custom value to return as forecast.
         alias: str
             Custom name of the model.
         """
         self.constant = constant
         self.alias = alias
 
-    def __repr__(self):
-        return self.alias
-
     def fit(
         self,
         y: np.ndarray,
         X: Optional[np.ndarray] = None,
     ):
         """Fit the Constant model.
 
@@ -6151,30 +6772,32 @@
             Dictionary with entries `constant` for point predictions and `level_*` for probabilistic predictions.
         """
         res = self.forecast(
             y=y, h=h, X=X, X_future=X_future, level=level, fitted=fitted
         )
         return res
 
-# %% ../nbs/src/core/models.ipynb 493
+# %% ../nbs/src/core/models.ipynb 515
 class ZeroModel(ConstantModel):
+
     def __init__(self, alias: str = "ZeroModel"):
         """Returns Zero forecasts.
 
         Returns Zero values.
 
         Parameters
         ----------
         alias: str
             Custom name of the model.
         """
         super().__init__(constant=0, alias=alias)
 
-# %% ../nbs/src/core/models.ipynb 507
+# %% ../nbs/src/core/models.ipynb 529
 class NaNModel(ConstantModel):
+
     def __init__(self, alias: str = "NaNModel"):
         """NaN Model.
 
         Returns NaN values.
 
         Parameters
         ----------
```

### Comparing `statsforecast-1.7.4/statsforecast/mstl.py` & `statsforecast-1.7.5/statsforecast/mstl.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/statsforecast/tbats.py` & `statsforecast-1.7.5/statsforecast/tbats.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 import pandas as pd
 import scipy.linalg
 from coreforecast.scalers import boxcox, boxcox_lambda, inv_boxcox
 from numba import njit
 from numpy.polynomial.polynomial import Polynomial
 from scipy.optimize import minimize
-from threadpoolctl import threadpool_limits
+
 from .arima import auto_arima_f
 from .utils import NOGIL, CACHE
 
 # %% ../nbs/src/tbats.ipynb 7
 def find_harmonics(y, m):
 
     # Compute a 2 x m moving average to estimate the trend
@@ -983,29 +983,28 @@
         T = [[False, False]]
 
     A = [use_arma_errors]
 
     combinations = [(b, t, a) for b, t, a in product(B, T, A)]
 
     mod = {"aic": np.inf}
-    with threadpool_limits(limits=1):
-        for boxcox_var, (trend, damped_trend), arma_errors in combinations:
-            new_mod = tbats_model(
-                y,
-                seasonal_periods,
-                k_vector,
-                boxcox_var,
-                bc_lower_bound,
-                bc_upper_bound,
-                trend,
-                damped_trend,
-                arma_errors,
-            )
-            if new_mod["aic"] < mod["aic"]:
-                mod = new_mod
+    for boxcox_var, (trend, damped_trend), arma_errors in combinations:
+        new_mod = tbats_model(
+            y,
+            seasonal_periods,
+            k_vector,
+            boxcox_var,
+            bc_lower_bound,
+            bc_upper_bound,
+            trend,
+            damped_trend,
+            arma_errors,
+        )
+        if new_mod["aic"] < mod["aic"]:
+            mod = new_mod
 
     return mod
 
 # %% ../nbs/src/tbats.ipynb 42
 def tbats_forecast(mod, h):  # this function is the same as bats_forecast
     fcst = np.zeros(h)
     xx = np.zeros((h, mod["x"].shape[1]))
```

### Comparing `statsforecast-1.7.4/statsforecast/theta.py` & `statsforecast-1.7.5/statsforecast/theta.py`

 * *Files 0% similar despite different names*

```diff
@@ -616,15 +616,15 @@
             initial_smoothed=np.mean(y) / 2,
             alpha=0.5,
             theta=2.0,
         )
     # seasonal decomposition if needed
     decompose = False
     # seasonal test
-    if m >= 4:
+    if m >= 4 and len(y) >= 2 * m:
         r = acf(y, nlags=m, fft=False)[1:]
         stat = np.sqrt((1 + 2 * np.sum(r[:-1] ** 2)) / len(y))
         decompose = np.abs(r[-1]) / stat > norm.ppf(0.95)
 
     data_positive = min(y) > 0
     if decompose:
         # change decomposition type if data is not positive
```

### Comparing `statsforecast-1.7.4/statsforecast/utils.py` & `statsforecast-1.7.5/statsforecast/utils.py`

 * *Files identical despite different names*

### Comparing `statsforecast-1.7.4/statsforecast.egg-info/PKG-INFO` & `statsforecast-1.7.5/statsforecast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statsforecast
-Version: 1.7.4
+Version: 1.7.5
 Summary: Time series forecasting suite using statistical models
 Home-page: https://github.com/Nixtla/statsforecast/
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series forecasting arima ets
 Classifier: Development Status :: 3 - Alpha
@@ -15,45 +15,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloudpickle
-Requires-Dist: coreforecast>=0.0.7
+Requires-Dist: coreforecast>=0.0.9
 Requires-Dist: numba>=0.55.0
 Requires-Dist: numpy>=1.21.6
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: statsmodels>=0.13.2
 Requires-Dist: tqdm
 Requires-Dist: fugue>=0.8.1
-Requires-Dist: utilsforecast>=0.0.24
+Requires-Dist: utilsforecast>=0.1.4
 Requires-Dist: threadpoolctl
 Provides-Extra: dev
 Requires-Dist: pmdarima; extra == "dev"
-Requires-Dist: fugue[ray]>=0.8.1; extra == "dev"
+Requires-Dist: pyarrow; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: scikit-learn; extra == "dev"
+Requires-Dist: fugue[spark]>=0.8.1; extra == "dev"
+Requires-Dist: ray<2.8; extra == "dev"
+Requires-Dist: pandas[plot]; extra == "dev"
+Requires-Dist: datasetsforecast; extra == "dev"
 Requires-Dist: nbdev_plotly; extra == "dev"
-Requires-Dist: plotly-resampler; extra == "dev"
-Requires-Dist: polars; extra == "dev"
-Requires-Dist: plotly; extra == "dev"
-Requires-Dist: pyarrow; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: nbdev; extra == "dev"
-Requires-Dist: protobuf<4.0.0,>=3.15.3; extra == "dev"
-Requires-Dist: fugue[dask]>=0.8.1; extra == "dev"
+Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
+Requires-Dist: setuptools<70; extra == "dev"
 Requires-Dist: prophet; extra == "dev"
-Requires-Dist: datasetsforecast; extra == "dev"
+Requires-Dist: protobuf<4.0.0,>=3.15.3; extra == "dev"
+Requires-Dist: fugue[ray]>=0.8.1; extra == "dev"
 Requires-Dist: supersmoother; extra == "dev"
-Requires-Dist: pandas[plot]; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: ray<2.8; extra == "dev"
-Requires-Dist: fugue[spark]>=0.8.1; extra == "dev"
+Requires-Dist: fugue[dask]>=0.8.1; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
+Requires-Dist: plotly; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: plotly-resampler; extra == "dev"
+Requires-Dist: polars; extra == "dev"
 Provides-Extra: dask
 Requires-Dist: fugue[dask]>=0.8.1; extra == "dask"
 Provides-Extra: ray
 Requires-Dist: fugue[ray]>=0.8.1; extra == "ray"
 Requires-Dist: protobuf<4.0.0,>=3.15.3; extra == "ray"
 Requires-Dist: ray<2.8; extra == "ray"
 Provides-Extra: spark
```

### Comparing `statsforecast-1.7.4/statsforecast.egg-info/SOURCES.txt` & `statsforecast-1.7.5/statsforecast.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 settings.ini
 setup.py
 action_files/__init__.py
 action_files/conftest.py
+action_files/imports_with_code.py
 action_files/test_dask.py
 action_files/test_fit_predict.py
 action_files/test_ray.py
 action_files/test_spark.py
 action_files/utils.py
 statsforecast/__init__.py
 statsforecast/_modidx.py
 statsforecast/arima.py
 statsforecast/ces.py
 statsforecast/core.py
 statsforecast/ets.py
 statsforecast/feature_engineering.py
 statsforecast/garch.py
+statsforecast/mfles.py
 statsforecast/models.py
 statsforecast/mstl.py
 statsforecast/tbats.py
 statsforecast/theta.py
 statsforecast/utils.py
 statsforecast.egg-info/PKG-INFO
 statsforecast.egg-info/SOURCES.txt
```

### Comparing `statsforecast-1.7.4/statsforecast.egg-info/requires.txt` & `statsforecast-1.7.5/statsforecast.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 cloudpickle
-coreforecast>=0.0.7
+coreforecast>=0.0.9
 numba>=0.55.0
 numpy>=1.21.6
 pandas>=1.3.5
 scipy>=1.7.3
 statsmodels>=0.13.2
 tqdm
 fugue>=0.8.1
-utilsforecast>=0.0.24
+utilsforecast>=0.1.4
 threadpoolctl
 
 [dask]
 fugue[dask]>=0.8.1
 
 [dev]
 pmdarima
-fugue[ray]>=0.8.1
+pyarrow
+pre-commit
 scikit-learn
+fugue[spark]>=0.8.1
+ray<2.8
+pandas[plot]
+datasetsforecast
 nbdev_plotly
-plotly-resampler
-polars
-plotly
-pyarrow
-flake8
-nbdev
-protobuf<4.0.0,>=3.15.3
-fugue[dask]>=0.8.1
+black
 mypy
+setuptools<70
 prophet
-datasetsforecast
+protobuf<4.0.0,>=3.15.3
+fugue[ray]>=0.8.1
 supersmoother
-pandas[plot]
-black
-ray<2.8
-fugue[spark]>=0.8.1
+fugue[dask]>=0.8.1
+nbdev
+plotly
+ruff
+plotly-resampler
+polars
 
 [plotly]
 plotly
 plotly-resampler
 
 [polars]
 polars
```

