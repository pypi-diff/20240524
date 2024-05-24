# Comparing `tmp/bigtools-0.1.8.tar.gz` & `tmp/bigtools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigtools-0.1.8.tar", last modified: Mon Apr  1 08:08:40 2024, max compression
+gzip compressed data, was "bigtools-0.1.9.tar", last modified: Mon Apr  1 08:24:21 2024, max compression
```

## Comparing `bigtools-0.1.8.tar` & `bigtools-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-04-01 08:08:40.239048 bigtools-0.1.8/
--rw-r--r--   0 bo         (501) staff       (20)    11357 2023-09-26 10:32:13.000000 bigtools-0.1.8/LICENSE
--rw-r--r--   0 bo         (501) staff       (20)       64 2023-10-07 08:59:46.000000 bigtools-0.1.8/MANIFEST.in
--rw-r--r--   0 bo         (501) staff       (20)     4707 2024-04-01 08:08:40.238845 bigtools-0.1.8/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)     4011 2024-04-01 08:02:17.000000 bigtools-0.1.8/README.md
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-04-01 08:08:40.237671 bigtools-0.1.8/bigtools/
--rw-r--r--   0 bo         (501) staff       (20)     1025 2024-04-01 08:02:17.000000 bigtools-0.1.8/bigtools/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     1863 2024-04-01 08:00:00.000000 bigtools-0.1.8/bigtools/db_tools.py
--rw-r--r--   0 bo         (501) staff       (20)     2767 2023-12-11 10:34:58.000000 bigtools-0.1.8/bigtools/default_data.py
--rw-r--r--   0 bo         (501) staff       (20)     2240 2023-10-19 08:39:36.000000 bigtools-0.1.8/bigtools/hash_tools.py
--rw-r--r--   0 bo         (501) staff       (20)      299 2023-11-20 10:33:10.000000 bigtools-0.1.8/bigtools/jieba_tools.py
--rw-r--r--   0 bo         (501) staff       (20)     1609 2023-12-18 05:49:55.000000 bigtools-0.1.8/bigtools/log_tools.py
--rw-r--r--   0 bo         (501) staff       (20)     4967 2023-12-19 09:01:17.000000 bigtools-0.1.8/bigtools/more_tools.py
--rw-r--r--   0 bo         (501) staff       (20)      739 2023-12-18 03:49:56.000000 bigtools-0.1.8/bigtools/path_tools.py
--rw-r--r--   0 bo         (501) staff       (20)     3120 2023-11-30 03:43:41.000000 bigtools-0.1.8/bigtools/requests_tools.py
--rw-r--r--   0 bo         (501) staff       (20)      953 2023-11-15 09:38:35.000000 bigtools-0.1.8/bigtools/similarity_tools.py
--rw-r--r--   0 bo         (501) staff       (20)    25647 2023-11-15 10:15:48.000000 bigtools-0.1.8/bigtools/stopwords.py
--rw-r--r--   0 bo         (501) staff       (20)      473 2023-11-08 02:46:13.000000 bigtools-0.1.8/bigtools/yaml_tools.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-04-01 08:08:40.238527 bigtools-0.1.8/bigtools.egg-info/
--rw-r--r--   0 bo         (501) staff       (20)     4707 2024-04-01 08:08:40.000000 bigtools-0.1.8/bigtools.egg-info/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      507 2024-04-01 08:08:40.000000 bigtools-0.1.8/bigtools.egg-info/SOURCES.txt
--rw-r--r--   0 bo         (501) staff       (20)        1 2024-04-01 08:08:40.000000 bigtools-0.1.8/bigtools.egg-info/dependency_links.txt
--rw-r--r--   0 bo         (501) staff       (20)      130 2024-04-01 08:08:40.000000 bigtools-0.1.8/bigtools.egg-info/requires.txt
--rw-r--r--   0 bo         (501) staff       (20)        9 2024-04-01 08:08:40.000000 bigtools-0.1.8/bigtools.egg-info/top_level.txt
--rw-r--r--   0 bo         (501) staff       (20)      288 2024-04-01 08:02:17.000000 bigtools-0.1.8/requires.py
--rw-r--r--   0 bo         (501) staff       (20)       38 2024-04-01 08:08:40.239085 bigtools-0.1.8/setup.cfg
--rw-r--r--   0 bo         (501) staff       (20)      853 2023-12-14 03:20:56.000000 bigtools-0.1.8/setup.py
--rw-r--r--   0 bo         (501) staff       (20)       21 2024-04-01 08:08:29.000000 bigtools-0.1.8/version.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-04-01 08:24:21.034852 bigtools-0.1.9/
+-rw-r--r--   0 bo         (501) staff       (20)    11357 2023-09-26 10:32:13.000000 bigtools-0.1.9/LICENSE
+-rw-r--r--   0 bo         (501) staff       (20)       64 2023-10-07 08:59:46.000000 bigtools-0.1.9/MANIFEST.in
+-rw-r--r--   0 bo         (501) staff       (20)     4708 2024-04-01 08:24:21.034633 bigtools-0.1.9/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)     4012 2024-04-01 08:23:25.000000 bigtools-0.1.9/README.md
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-04-01 08:24:21.033609 bigtools-0.1.9/bigtools/
+-rw-r--r--   0 bo         (501) staff       (20)     1026 2024-04-01 08:23:25.000000 bigtools-0.1.9/bigtools/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     1864 2024-04-01 08:20:01.000000 bigtools-0.1.9/bigtools/db_tools.py
+-rw-r--r--   0 bo         (501) staff       (20)     2767 2023-12-11 10:34:58.000000 bigtools-0.1.9/bigtools/default_data.py
+-rw-r--r--   0 bo         (501) staff       (20)     2240 2023-10-19 08:39:36.000000 bigtools-0.1.9/bigtools/hash_tools.py
+-rw-r--r--   0 bo         (501) staff       (20)      299 2023-11-20 10:33:10.000000 bigtools-0.1.9/bigtools/jieba_tools.py
+-rw-r--r--   0 bo         (501) staff       (20)     1609 2023-12-18 05:49:55.000000 bigtools-0.1.9/bigtools/log_tools.py
+-rw-r--r--   0 bo         (501) staff       (20)     4967 2023-12-19 09:01:17.000000 bigtools-0.1.9/bigtools/more_tools.py
+-rw-r--r--   0 bo         (501) staff       (20)      739 2023-12-18 03:49:56.000000 bigtools-0.1.9/bigtools/path_tools.py
+-rw-r--r--   0 bo         (501) staff       (20)     3120 2023-11-30 03:43:41.000000 bigtools-0.1.9/bigtools/requests_tools.py
+-rw-r--r--   0 bo         (501) staff       (20)      953 2023-11-15 09:38:35.000000 bigtools-0.1.9/bigtools/similarity_tools.py
+-rw-r--r--   0 bo         (501) staff       (20)    25647 2023-11-15 10:15:48.000000 bigtools-0.1.9/bigtools/stopwords.py
+-rw-r--r--   0 bo         (501) staff       (20)      473 2023-11-08 02:46:13.000000 bigtools-0.1.9/bigtools/yaml_tools.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2024-04-01 08:24:21.034304 bigtools-0.1.9/bigtools.egg-info/
+-rw-r--r--   0 bo         (501) staff       (20)     4708 2024-04-01 08:24:20.000000 bigtools-0.1.9/bigtools.egg-info/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      507 2024-04-01 08:24:21.000000 bigtools-0.1.9/bigtools.egg-info/SOURCES.txt
+-rw-r--r--   0 bo         (501) staff       (20)        1 2024-04-01 08:24:20.000000 bigtools-0.1.9/bigtools.egg-info/dependency_links.txt
+-rw-r--r--   0 bo         (501) staff       (20)      130 2024-04-01 08:24:20.000000 bigtools-0.1.9/bigtools.egg-info/requires.txt
+-rw-r--r--   0 bo         (501) staff       (20)        9 2024-04-01 08:24:20.000000 bigtools-0.1.9/bigtools.egg-info/top_level.txt
+-rw-r--r--   0 bo         (501) staff       (20)      288 2024-04-01 08:02:17.000000 bigtools-0.1.9/requires.py
+-rw-r--r--   0 bo         (501) staff       (20)       38 2024-04-01 08:24:21.034897 bigtools-0.1.9/setup.cfg
+-rw-r--r--   0 bo         (501) staff       (20)      853 2023-12-14 03:20:56.000000 bigtools-0.1.9/setup.py
+-rw-r--r--   0 bo         (501) staff       (20)       21 2024-04-01 08:24:12.000000 bigtools-0.1.9/version.py
```

### Comparing `bigtools-0.1.8/LICENSE` & `bigtools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bigtools-0.1.8/PKG-INFO` & `bigtools-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigtools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for python
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: bananabo@foxmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -85,15 +85,15 @@
 data = ''
 response = requests.post(url=url, data=data, headers=ContentType.app_json_headers)
 print(response)
 ```
 ## 实现清单
 ### 1. 已实现的函数或类
 ```python3
-from bigtools.db_tools import mongo_client, MinioClinet
+from bigtools.db_tools import mongo_client, MinioOperate
 from bigtools.hash_tools import generate_hash_value, hash_object_dict
 from bigtools.jieba_tools import get_keywords_from_text
 from bigtools.log_tools import set_log, SetLog
 from bigtools.yaml_tools import load_yaml, load_all_yaml, write_yaml
 from bigtools.path_tools import check_make_dir, get_execution_dir, get_file_type, get_execution_file_name
 from bigtools.requests_tools import get_requests_session, DealException, download, save_response_data
 from bigtools.similarity_tools import cosine_similarity, edit_distance
```

### Comparing `bigtools-0.1.8/README.md` & `bigtools-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 data = ''
 response = requests.post(url=url, data=data, headers=ContentType.app_json_headers)
 print(response)
 ```
 ## 实现清单
 ### 1. 已实现的函数或类
 ```python3
-from bigtools.db_tools import mongo_client, MinioClinet
+from bigtools.db_tools import mongo_client, MinioOperate
 from bigtools.hash_tools import generate_hash_value, hash_object_dict
 from bigtools.jieba_tools import get_keywords_from_text
 from bigtools.log_tools import set_log, SetLog
 from bigtools.yaml_tools import load_yaml, load_all_yaml, write_yaml
 from bigtools.path_tools import check_make_dir, get_execution_dir, get_file_type, get_execution_file_name
 from bigtools.requests_tools import get_requests_session, DealException, download, save_response_data
 from bigtools.similarity_tools import cosine_similarity, edit_distance
```

### Comparing `bigtools-0.1.8/bigtools/__init__.py` & `bigtools-0.1.9/bigtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: UTF-8 -*-
 # @Time : 2023/9/26 18:34 
 # @Author : 刘洪波
 from bigtools.default_data import *
-from bigtools.db_tools import mongo_client, MinioClinet
+from bigtools.db_tools import mongo_client, MinioOperate
 from bigtools.hash_tools import generate_hash_value, hash_object_dict
 from bigtools.jieba_tools import get_keywords_from_text
 from bigtools.log_tools import set_log, SetLog
 from bigtools.yaml_tools import load_yaml, load_all_yaml, write_yaml
 from bigtools.path_tools import check_make_dir, get_execution_dir, get_file_type, get_execution_file_name
 from bigtools.requests_tools import get_requests_session, DealException, download, save_response_data
 from bigtools.similarity_tools import cosine_similarity, edit_distance
```

### Comparing `bigtools-0.1.8/bigtools/db_tools.py` & `bigtools-0.1.9/bigtools/db_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     elif password:
         raise ValueError('Please check user and password')
     if tz_aware:
         return MongoClient(uri, tz_aware=tz_aware, tzinfo=timezone(tzinfo))
     return MongoClient(uri)
 
 
-class MinioClinet(object):
+class MinioOperate(object):
     def __init__(self, minio_clinet: Minio):
         self.clinet = minio_clinet
 
     def create_bucket(self, bucket_name: str):
         """
         创建桶
         注：创建桶命名限制：小写字母，句点，连字符和数字是唯一允许使用的字符（使用大写字母、下划线等命名会报错），长度至少应为3个字符
```

### Comparing `bigtools-0.1.8/bigtools/default_data.py` & `bigtools-0.1.9/bigtools/default_data.py`

 * *Files identical despite different names*

### Comparing `bigtools-0.1.8/bigtools/hash_tools.py` & `bigtools-0.1.9/bigtools/hash_tools.py`

 * *Files identical despite different names*

### Comparing `bigtools-0.1.8/bigtools/log_tools.py` & `bigtools-0.1.9/bigtools/log_tools.py`

 * *Files identical despite different names*

### Comparing `bigtools-0.1.8/bigtools/more_tools.py` & `bigtools-0.1.9/bigtools/more_tools.py`

 * *Files identical despite different names*

### Comparing `bigtools-0.1.8/bigtools/path_tools.py` & `bigtools-0.1.9/bigtools/path_tools.py`

 * *Files identical despite different names*

### Comparing `bigtools-0.1.8/bigtools/requests_tools.py` & `bigtools-0.1.9/bigtools/requests_tools.py`

 * *Files identical despite different names*

### Comparing `bigtools-0.1.8/bigtools/similarity_tools.py` & `bigtools-0.1.9/bigtools/similarity_tools.py`

 * *Files identical despite different names*

### Comparing `bigtools-0.1.8/bigtools/stopwords.py` & `bigtools-0.1.9/bigtools/stopwords.py`

 * *Files identical despite different names*

### Comparing `bigtools-0.1.8/bigtools.egg-info/PKG-INFO` & `bigtools-0.1.9/bigtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigtools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for python
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: bananabo@foxmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -85,15 +85,15 @@
 data = ''
 response = requests.post(url=url, data=data, headers=ContentType.app_json_headers)
 print(response)
 ```
 ## 实现清单
 ### 1. 已实现的函数或类
 ```python3
-from bigtools.db_tools import mongo_client, MinioClinet
+from bigtools.db_tools import mongo_client, MinioOperate
 from bigtools.hash_tools import generate_hash_value, hash_object_dict
 from bigtools.jieba_tools import get_keywords_from_text
 from bigtools.log_tools import set_log, SetLog
 from bigtools.yaml_tools import load_yaml, load_all_yaml, write_yaml
 from bigtools.path_tools import check_make_dir, get_execution_dir, get_file_type, get_execution_file_name
 from bigtools.requests_tools import get_requests_session, DealException, download, save_response_data
 from bigtools.similarity_tools import cosine_similarity, edit_distance
```

### Comparing `bigtools-0.1.8/setup.py` & `bigtools-0.1.9/setup.py`

 * *Files identical despite different names*

