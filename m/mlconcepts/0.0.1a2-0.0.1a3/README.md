# Comparing `tmp/mlconcepts-0.0.1a2.tar.gz` & `tmp/mlconcepts-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlconcepts-0.0.1a2.tar", last modified: Fri May 24 13:24:28 2024, max compression
+gzip compressed data, was "mlconcepts-0.0.1a3.tar", last modified: Fri May 24 15:55:13 2024, max compression
```

## Comparing `mlconcepts-0.0.1a2.tar` & `mlconcepts-0.0.1a3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:24:28.806451 mlconcepts-0.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-24 13:24:14.026425 mlconcepts-0.0.1a2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-24 13:24:28.794451 mlconcepts-0.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-24 13:24:14.000000 mlconcepts-0.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:24:28.806451 mlconcepts-0.0.1a2/include/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-24 13:24:14.026425 mlconcepts-0.0.1a2/include/BasicMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    20601 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/Bitset.h
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/Bitstream.h
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/CNClassifier.h
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/ContextConcepts.h
--rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/ContextSelector.h
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/Dataset.h
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/EigenDataset.h
--rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/FeatureAssigner.h
--rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/GradientDescent.h
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/Model.h
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/PartialContext.h
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/Settings.h
--rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/StandardConceptifier.h
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/SupervisedOutlierDetectionModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/include/UnsupervisedOutlierDetectionModel.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:24:28.810451 mlconcepts-0.0.1a2/mlconcepts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-24 13:24:28.000000 mlconcepts-0.0.1a2/mlconcepts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-24 13:24:28.810451 mlconcepts-0.0.1a2/mlconcepts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:24:28.000000 mlconcepts-0.0.1a2/mlconcepts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:24:28.000000 mlconcepts-0.0.1a2/mlconcepts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 13:24:28.000000 mlconcepts-0.0.1a2/mlconcepts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 13:24:28.000000 mlconcepts-0.0.1a2/mlconcepts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-24 13:24:14.000000 mlconcepts-0.0.1a2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-24 13:24:14.000000 mlconcepts-0.0.1a2/rename_dist.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-24 13:24:28.798451 mlconcepts-0.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-24 13:24:14.000000 mlconcepts-0.0.1a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:24:28.798451 mlconcepts-0.0.1a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:24:28.798451 mlconcepts-0.0.1a2/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:24:28.802451 mlconcepts-0.0.1a2/src/python/mlconcepts/
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python/mlconcepts/ExplanationData.py
--rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python/mlconcepts/SODModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10383 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python/mlconcepts/UODModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python/mlconcepts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:24:28.802451 mlconcepts-0.0.1a2/src/python/mlconcepts/data/
--rw-r--r--   0 runner    (1001) docker     (127)    16712 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python/mlconcepts/data/Dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python/mlconcepts/data/NumpyLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python/mlconcepts/data/PandasLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python/mlconcepts/data/PathLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python/mlconcepts/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python/mlconcepts/data/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:24:28.802451 mlconcepts-0.0.1a2/src/python/mlconcepts/mlconceptscore/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python/mlconcepts/mlconceptscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python/mlconcepts/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-24 13:24:14.030425 mlconcepts-0.0.1a2/src/python_mlconcepts.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:24:28.806451 mlconcepts-0.0.1a2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-24 13:24:14.034425 mlconcepts-0.0.1a2/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-24 13:24:14.034425 mlconcepts-0.0.1a2/tests/tests.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-24 13:24:14.034425 mlconcepts-0.0.1a2/tests/tests_partial_context.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:55:13.584955 mlconcepts-0.0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-05-24 15:55:02.160950 mlconcepts-0.0.1a3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-24 15:55:13.572955 mlconcepts-0.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-24 15:55:02.000000 mlconcepts-0.0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:55:13.584955 mlconcepts-0.0.1a3/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/BasicMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20601 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/Bitset.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/Bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/CNClassifier.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/ContextConcepts.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/ContextSelector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/Dataset.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/EigenDataset.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/FeatureAssigner.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/GradientDescent.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/Model.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/PartialContext.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/StandardConceptifier.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/SupervisedOutlierDetectionModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/include/UnsupervisedOutlierDetectionModel.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:55:13.588955 mlconcepts-0.0.1a3/mlconcepts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-24 15:55:13.000000 mlconcepts-0.0.1a3/mlconcepts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-24 15:55:13.588955 mlconcepts-0.0.1a3/mlconcepts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:55:13.000000 mlconcepts-0.0.1a3/mlconcepts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:55:13.000000 mlconcepts-0.0.1a3/mlconcepts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 15:55:13.000000 mlconcepts-0.0.1a3/mlconcepts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 15:55:13.000000 mlconcepts-0.0.1a3/mlconcepts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-24 15:55:02.000000 mlconcepts-0.0.1a3/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-24 15:55:02.000000 mlconcepts-0.0.1a3/rename_dist.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-24 15:55:13.572955 mlconcepts-0.0.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-24 15:55:02.000000 mlconcepts-0.0.1a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:55:13.572955 mlconcepts-0.0.1a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:55:13.572955 mlconcepts-0.0.1a3/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:55:13.576955 mlconcepts-0.0.1a3/src/python/mlconcepts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python/mlconcepts/ExplanationData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python/mlconcepts/SODModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10383 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python/mlconcepts/UODModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python/mlconcepts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:55:13.576955 mlconcepts-0.0.1a3/src/python/mlconcepts/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    16712 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python/mlconcepts/data/Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python/mlconcepts/data/NumpyLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python/mlconcepts/data/PandasLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python/mlconcepts/data/PathLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python/mlconcepts/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python/mlconcepts/data/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:55:13.576955 mlconcepts-0.0.1a3/src/python/mlconcepts/mlconceptscore/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python/mlconcepts/mlconceptscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python/mlconcepts/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/src/python_mlconcepts.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:55:13.584955 mlconcepts-0.0.1a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/tests/tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-24 15:55:02.164950 mlconcepts-0.0.1a3/tests/tests_partial_context.cpp
```

### Comparing `mlconcepts-0.0.1a2/CMakeLists.txt` & `mlconcepts-0.0.1a3/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                                 WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR})
         endif()
         include_directories("eigen-3.4.0")
 else()
     include_directories( ${EIGEN3_INCLUDE_DIRS} )
 endif ()
 
-find_package(Python COMPONENTS Interpreter Development)
+find_package(Python COMPONENTS Interpreter Development.Module)
 find_package(pybind11 CONFIG REQUIRED)
 
 include(CTest)
 include_directories("include")
 
 
 # Python module
```

### Comparing `mlconcepts-0.0.1a2/PKG-INFO` & `mlconcepts-0.0.1a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlconcepts
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: A small library implementing several interpretable machine learning algorithms based on FCA.
 Home-page: https://github.com/xeredent/libmlconcepts
 Author: Mattia Panettiere
 Author-email: mattia.panettiere@gmail.com
 License: BSD3
 Project-URL: Source, https://github.com/xeredent/libmlconcepts
 Project-URL: Tracker, https://github.com/xeredent/libmlconcepts/issues
```

### Comparing `mlconcepts-0.0.1a2/README.md` & `mlconcepts-0.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/BasicMath.h` & `mlconcepts-0.0.1a3/include/BasicMath.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/Bitset.h` & `mlconcepts-0.0.1a3/include/Bitset.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/Bitstream.h` & `mlconcepts-0.0.1a3/include/Bitstream.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/CNClassifier.h` & `mlconcepts-0.0.1a3/include/CNClassifier.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/ContextConcepts.h` & `mlconcepts-0.0.1a3/include/ContextConcepts.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/ContextSelector.h` & `mlconcepts-0.0.1a3/include/ContextSelector.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/Dataset.h` & `mlconcepts-0.0.1a3/include/Dataset.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/EigenDataset.h` & `mlconcepts-0.0.1a3/include/EigenDataset.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/FeatureAssigner.h` & `mlconcepts-0.0.1a3/include/FeatureAssigner.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/GradientDescent.h` & `mlconcepts-0.0.1a3/include/GradientDescent.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/Model.h` & `mlconcepts-0.0.1a3/include/Model.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/PartialContext.h` & `mlconcepts-0.0.1a3/include/PartialContext.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/Settings.h` & `mlconcepts-0.0.1a3/include/Settings.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/StandardConceptifier.h` & `mlconcepts-0.0.1a3/include/StandardConceptifier.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/SupervisedOutlierDetectionModel.h` & `mlconcepts-0.0.1a3/include/SupervisedOutlierDetectionModel.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/include/UnsupervisedOutlierDetectionModel.h` & `mlconcepts-0.0.1a3/include/UnsupervisedOutlierDetectionModel.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/mlconcepts.egg-info/PKG-INFO` & `mlconcepts-0.0.1a3/mlconcepts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlconcepts
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: A small library implementing several interpretable machine learning algorithms based on FCA.
 Home-page: https://github.com/xeredent/libmlconcepts
 Author: Mattia Panettiere
 Author-email: mattia.panettiere@gmail.com
 License: BSD3
 Project-URL: Source, https://github.com/xeredent/libmlconcepts
 Project-URL: Tracker, https://github.com/xeredent/libmlconcepts/issues
```

### Comparing `mlconcepts-0.0.1a2/mlconcepts.egg-info/SOURCES.txt` & `mlconcepts-0.0.1a3/mlconcepts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/setup.cfg` & `mlconcepts-0.0.1a3/setup.cfg`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/setup.py` & `mlconcepts-0.0.1a3/setup.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/src/python/mlconcepts/ExplanationData.py` & `mlconcepts-0.0.1a3/src/python/mlconcepts/ExplanationData.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/src/python/mlconcepts/SODModel.py` & `mlconcepts-0.0.1a3/src/python/mlconcepts/SODModel.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/src/python/mlconcepts/UODModel.py` & `mlconcepts-0.0.1a3/src/python/mlconcepts/UODModel.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/src/python/mlconcepts/data/Dataset.py` & `mlconcepts-0.0.1a3/src/python/mlconcepts/data/Dataset.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/src/python/mlconcepts/data/NumpyLoader.py` & `mlconcepts-0.0.1a3/src/python/mlconcepts/data/NumpyLoader.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/src/python/mlconcepts/data/PandasLoader.py` & `mlconcepts-0.0.1a3/src/python/mlconcepts/data/PandasLoader.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/src/python/mlconcepts/data/PathLoader.py` & `mlconcepts-0.0.1a3/src/python/mlconcepts/data/PathLoader.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/src/python/mlconcepts/data/__init__.py` & `mlconcepts-0.0.1a3/src/python/mlconcepts/data/__init__.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/src/python/mlconcepts/data/test_data.py` & `mlconcepts-0.0.1a3/src/python/mlconcepts/data/test_data.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/src/python/mlconcepts/test_models.py` & `mlconcepts-0.0.1a3/src/python/mlconcepts/test_models.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/src/python_mlconcepts.cpp` & `mlconcepts-0.0.1a3/src/python_mlconcepts.cpp`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a2/tests/tests_partial_context.cpp` & `mlconcepts-0.0.1a3/tests/tests_partial_context.cpp`

 * *Files identical despite different names*

