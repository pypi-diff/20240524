# Comparing `tmp/oxaigen-0.0.1.0.tar.gz` & `tmp/oxaigen-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxaigen-0.0.1.0.tar", max compression
+gzip compressed data, was "oxaigen-0.0.1.1.tar", max compression
```

## Comparing `oxaigen-0.0.1.0.tar` & `oxaigen-0.0.1.1.tar`

### file list

```diff
@@ -1,20 +1,24 @@
--rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.1.0/README.md
--rw-r--r--   0        0        0      112 2024-05-21 18:27:06.168091 oxaigen-0.0.1.0/oxaigen/__init__.py
--rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.1.0/oxaigen/src/__init__.py
--rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.1.0/oxaigen/src/asset/__init__.py
--rw-r--r--   0        0        0     7244 2024-05-22 15:29:14.166261 oxaigen-0.0.1.0/oxaigen/src/asset/asset.py
--rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.1.0/oxaigen/src/authentication/__init__.py
--rw-r--r--   0        0        0     2655 2024-05-22 12:57:53.116060 oxaigen-0.0.1.0/oxaigen/src/authentication/authentication.py
--rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.1.0/oxaigen/src/config.py
--rw-r--r--   0        0        0      118 2024-05-22 13:30:36.758916 oxaigen-0.0.1.0/oxaigen/src/constant.py
--rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.1.0/oxaigen/src/main.py
--rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.1.0/oxaigen/src/storage/__init__.py
--rw-r--r--   0        0        0     4850 2024-05-22 15:41:08.118946 oxaigen-0.0.1.0/oxaigen/src/storage/data_storage.py
--rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.1.0/oxaigen/src/util/__init__.py
--rw-r--r--   0        0        0     2258 2024-05-22 13:27:42.721239 oxaigen-0.0.1.0/oxaigen/src/util/api.py
--rw-r--r--   0        0        0      906 2024-05-22 12:57:41.116790 oxaigen-0.0.1.0/oxaigen/src/util/exception.py
--rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.1.0/oxaigen/src/util/logging.py
--rw-r--r--   0        0        0     4117 2024-05-22 13:16:05.444588 oxaigen-0.0.1.0/oxaigen/src/util/token.py
--rw-r--r--   0        0        0      816 2024-05-22 15:51:43.862669 oxaigen-0.0.1.0/oxaigen/src/util/util.py
--rw-r--r--   0        0        0      825 2024-05-22 15:52:01.536724 oxaigen-0.0.1.0/pyproject.toml
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 oxaigen-0.0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.1.1/README.md
+-rw-r--r--   0        0        0      212 2024-05-24 12:04:21.512609 oxaigen-0.0.1.1/oxaigen/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.1.1/oxaigen/src/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.1.1/oxaigen/src/asset/__init__.py
+-rw-r--r--   0        0        0     7244 2024-05-22 15:29:14.166261 oxaigen-0.0.1.1/oxaigen/src/asset/asset.py
+-rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.1.1/oxaigen/src/authentication/__init__.py
+-rw-r--r--   0        0        0     2655 2024-05-22 12:57:53.116060 oxaigen-0.0.1.1/oxaigen/src/authentication/authentication.py
+-rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.1.1/oxaigen/src/config.py
+-rw-r--r--   0        0        0      118 2024-05-22 13:30:36.758916 oxaigen-0.0.1.1/oxaigen/src/constant.py
+-rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.1.1/oxaigen/src/main.py
+-rw-r--r--   0        0        0      153 2024-05-24 12:04:02.433557 oxaigen-0.0.1.1/oxaigen/src/orchestration/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 11:56:11.573962 oxaigen-0.0.1.1/oxaigen/src/orchestration/resources/__init__.py
+-rw-r--r--   0        0        0     1746 2024-05-24 12:03:45.176346 oxaigen-0.0.1.1/oxaigen/src/orchestration/resources/db_io_manager.py
+-rw-r--r--   0        0        0     2785 2024-05-24 11:57:43.284892 oxaigen-0.0.1.1/oxaigen/src/orchestration/resources/dbt_translator.py
+-rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.1.1/oxaigen/src/storage/__init__.py
+-rw-r--r--   0        0        0     4850 2024-05-22 15:41:08.118946 oxaigen-0.0.1.1/oxaigen/src/storage/data_storage.py
+-rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.1.1/oxaigen/src/util/__init__.py
+-rw-r--r--   0        0        0     2258 2024-05-22 13:27:42.721239 oxaigen-0.0.1.1/oxaigen/src/util/api.py
+-rw-r--r--   0        0        0      906 2024-05-22 12:57:41.116790 oxaigen-0.0.1.1/oxaigen/src/util/exception.py
+-rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.1.1/oxaigen/src/util/logging.py
+-rw-r--r--   0        0        0     4117 2024-05-22 13:16:05.444588 oxaigen-0.0.1.1/oxaigen/src/util/token.py
+-rw-r--r--   0        0        0      816 2024-05-22 15:51:43.862669 oxaigen-0.0.1.1/oxaigen/src/util/util.py
+-rw-r--r--   0        0        0      820 2024-05-24 12:05:07.538266 oxaigen-0.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 oxaigen-0.0.1.1/PKG-INFO
```

### Comparing `oxaigen-0.0.1.0/oxaigen/src/asset/asset.py` & `oxaigen-0.0.1.1/oxaigen/src/asset/asset.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.1.0/oxaigen/src/authentication/authentication.py` & `oxaigen-0.0.1.1/oxaigen/src/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.1.0/oxaigen/src/config.py` & `oxaigen-0.0.1.1/oxaigen/src/config.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.1.0/oxaigen/src/storage/data_storage.py` & `oxaigen-0.0.1.1/oxaigen/src/storage/data_storage.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.1.0/oxaigen/src/util/api.py` & `oxaigen-0.0.1.1/oxaigen/src/util/api.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.1.0/oxaigen/src/util/exception.py` & `oxaigen-0.0.1.1/oxaigen/src/util/exception.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.1.0/oxaigen/src/util/token.py` & `oxaigen-0.0.1.1/oxaigen/src/util/token.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.1.0/oxaigen/src/util/util.py` & `oxaigen-0.0.1.1/oxaigen/src/util/util.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.1.0/pyproject.toml` & `oxaigen-0.0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "oxaigen"
-version = "0.0.1.0"
+version = "0.0.1.1"
 description = "Oxaigen Python SDK"
-authors = ["Luca Roggeveen Name <luca@oxaigen.com>"]
+authors = ["Luca Roggeveen <luca@oxaigen.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.12"
 pydantic = "==2.7.1"
 pandas = "^2.1.0"
 mlflow = "^2.10.2"
```

### Comparing `oxaigen-0.0.1.0/PKG-INFO` & `oxaigen-0.0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: oxaigen
-Version: 0.0.1.0
+Version: 0.0.1.1
 Summary: Oxaigen Python SDK
-Author: Luca Roggeveen Name
+Author: Luca Roggeveen
 Author-email: luca@oxaigen.com
 Requires-Python: >=3.10.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.34.44,<2.0.0)
 Requires-Dist: mlflow (>=2.10.2,<3.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
```

