# Comparing `tmp/ibmpairs-3.1.1.tar.gz` & `tmp/ibmpairs-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibmpairs-3.1.1.tar", last modified: Thu Mar 28 17:40:50 2024, max compression
+gzip compressed data, was "ibmpairs-3.1.2.tar", last modified: Fri May 24 15:41:57 2024, max compression
```

## Comparing `ibmpairs-3.1.1.tar` & `ibmpairs-3.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 staylor    (501) staff       (20)        0 2024-03-28 17:40:50.625130 ibmpairs-3.1.1/
--rw-r--r--   0 staylor    (501) staff       (20)     6217 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/CONTRIBUTING.md
--rw-r--r--   0 staylor    (501) staff       (20)     1488 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/LICENSE
--rw-r--r--   0 staylor    (501) staff       (20)      480 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/MAINTAINERS.md
--rw-r--r--   0 staylor    (501) staff       (20)      281 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/MANIFEST.in
--rw-r--r--   0 staylor    (501) staff       (20)     3280 2024-03-28 17:40:50.625201 ibmpairs-3.1.1/PKG-INFO
--rw-r--r--   0 staylor    (501) staff       (20)     2529 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/README.md
-drwxr-xr-x   0 staylor    (501) staff       (20)        0 2024-03-28 17:40:50.623971 ibmpairs-3.1.1/ibmpairs/
--rw-r--r--   0 staylor    (501) staff       (20)    73724 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/ibmpairs/authentication.py
--rw-r--r--   0 staylor    (501) staff       (20)   412824 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/ibmpairs/catalog.py
--rw-r--r--   0 staylor    (501) staff       (20)    45646 2024-03-28 17:37:27.000000 ibmpairs-3.1.1/ibmpairs/client.py
--rw-r--r--   0 staylor    (501) staff       (20)    16086 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/ibmpairs/common.py
--rw-r--r--   0 staylor    (501) staff       (20)     1112 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/ibmpairs/config.py
--rw-r--r--   0 staylor    (501) staff       (20)     5766 2024-03-28 17:37:27.000000 ibmpairs-3.1.1/ibmpairs/constants.py
--rw-r--r--   0 staylor    (501) staff       (20)    17970 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/ibmpairs/dashboard.py
-drwxr-xr-x   0 staylor    (501) staff       (20)        0 2024-03-28 17:40:50.624945 ibmpairs-3.1.1/ibmpairs/external/
--rw-r--r--   0 staylor    (501) staff       (20)   102439 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/ibmpairs/external/ibm.py
--rw-r--r--   0 staylor    (501) staff       (20)      391 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/ibmpairs/logger.py
--rw-r--r--   0 staylor    (501) staff       (20)    29033 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/ibmpairs/messages.py
--rw-r--r--   0 staylor    (501) staff       (20)   165355 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/ibmpairs/paw.py
--rw-r--r--   0 staylor    (501) staff       (20)   407921 2024-03-28 17:37:27.000000 ibmpairs-3.1.1/ibmpairs/query.py
--rw-r--r--   0 staylor    (501) staff       (20)   164229 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/ibmpairs/upload.py
--rw-r--r--   0 staylor    (501) staff       (20)    11334 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/ibmpairs/utils.py
--rw-r--r--   0 staylor    (501) staff       (20)       42 2024-03-28 17:40:50.000000 ibmpairs-3.1.1/ibmpairs/version.py
-drwxr-xr-x   0 staylor    (501) staff       (20)        0 2024-03-28 17:40:50.624807 ibmpairs-3.1.1/ibmpairs.egg-info/
--rw-r--r--   0 staylor    (501) staff       (20)     3280 2024-03-28 17:40:50.000000 ibmpairs-3.1.1/ibmpairs.egg-info/PKG-INFO
--rw-r--r--   0 staylor    (501) staff       (20)      619 2024-03-28 17:40:50.000000 ibmpairs-3.1.1/ibmpairs.egg-info/SOURCES.txt
--rw-r--r--   0 staylor    (501) staff       (20)        1 2024-03-28 17:40:50.000000 ibmpairs-3.1.1/ibmpairs.egg-info/dependency_links.txt
--rw-r--r--   0 staylor    (501) staff       (20)        1 2024-03-28 17:40:50.000000 ibmpairs-3.1.1/ibmpairs.egg-info/not-zip-safe
--rw-r--r--   0 staylor    (501) staff       (20)      273 2024-03-28 17:40:50.000000 ibmpairs-3.1.1/ibmpairs.egg-info/requires.txt
--rw-r--r--   0 staylor    (501) staff       (20)        9 2024-03-28 17:40:50.000000 ibmpairs-3.1.1/ibmpairs.egg-info/top_level.txt
--rw-r--r--   0 staylor    (501) staff       (20)       60 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/requirements-development.txt
--rw-r--r--   0 staylor    (501) staff       (20)      270 2024-03-28 17:30:45.000000 ibmpairs-3.1.1/requirements.txt
--rw-r--r--   0 staylor    (501) staff       (20)      103 2024-03-28 17:40:50.625420 ibmpairs-3.1.1/setup.cfg
--rwxr-xr-x   0 staylor    (501) staff       (20)     1838 2024-03-28 17:37:27.000000 ibmpairs-3.1.1/setup.py
+drwxr-xr-x   0 staylor    (501) staff       (20)        0 2024-05-24 15:41:57.879564 ibmpairs-3.1.2/
+-rw-r--r--   0 staylor    (501) staff       (20)     6217 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/CONTRIBUTING.md
+-rw-r--r--   0 staylor    (501) staff       (20)     1488 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/LICENSE
+-rw-r--r--   0 staylor    (501) staff       (20)      480 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/MAINTAINERS.md
+-rw-r--r--   0 staylor    (501) staff       (20)      281 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/MANIFEST.in
+-rw-r--r--   0 staylor    (501) staff       (20)     3961 2024-05-24 15:41:57.879472 ibmpairs-3.1.2/PKG-INFO
+-rw-r--r--   0 staylor    (501) staff       (20)     2550 2024-05-24 15:35:37.000000 ibmpairs-3.1.2/README.md
+drwxr-xr-x   0 staylor    (501) staff       (20)        0 2024-05-24 15:41:57.877122 ibmpairs-3.1.2/ibmpairs/
+-rw-r--r--   0 staylor    (501) staff       (20)    73724 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/ibmpairs/authentication.py
+-rw-r--r--   0 staylor    (501) staff       (20)   412825 2024-05-24 15:35:37.000000 ibmpairs-3.1.2/ibmpairs/catalog.py
+-rw-r--r--   0 staylor    (501) staff       (20)    45646 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/ibmpairs/client.py
+-rw-r--r--   0 staylor    (501) staff       (20)    16086 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/ibmpairs/common.py
+-rw-r--r--   0 staylor    (501) staff       (20)     1112 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/ibmpairs/config.py
+-rw-r--r--   0 staylor    (501) staff       (20)     5766 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/ibmpairs/constants.py
+-rw-r--r--   0 staylor    (501) staff       (20)    17970 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/ibmpairs/dashboard.py
+drwxr-xr-x   0 staylor    (501) staff       (20)        0 2024-05-24 15:41:57.878117 ibmpairs-3.1.2/ibmpairs/external/
+-rw-r--r--   0 staylor    (501) staff       (20)   102439 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/ibmpairs/external/ibm.py
+-rw-r--r--   0 staylor    (501) staff       (20)      391 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/ibmpairs/logger.py
+-rw-r--r--   0 staylor    (501) staff       (20)    29033 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/ibmpairs/messages.py
+-rw-r--r--   0 staylor    (501) staff       (20)   165355 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/ibmpairs/paw.py
+-rw-r--r--   0 staylor    (501) staff       (20)   408727 2024-05-24 15:35:37.000000 ibmpairs-3.1.2/ibmpairs/query.py
+-rw-r--r--   0 staylor    (501) staff       (20)   164229 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/ibmpairs/upload.py
+-rw-r--r--   0 staylor    (501) staff       (20)    11334 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/ibmpairs/utils.py
+-rw-r--r--   0 staylor    (501) staff       (20)       42 2024-05-24 15:41:57.000000 ibmpairs-3.1.2/ibmpairs/version.py
+drwxr-xr-x   0 staylor    (501) staff       (20)        0 2024-05-24 15:41:57.879059 ibmpairs-3.1.2/ibmpairs.egg-info/
+-rw-r--r--   0 staylor    (501) staff       (20)     3961 2024-05-24 15:41:57.000000 ibmpairs-3.1.2/ibmpairs.egg-info/PKG-INFO
+-rw-r--r--   0 staylor    (501) staff       (20)      619 2024-05-24 15:41:57.000000 ibmpairs-3.1.2/ibmpairs.egg-info/SOURCES.txt
+-rw-r--r--   0 staylor    (501) staff       (20)        1 2024-05-24 15:41:57.000000 ibmpairs-3.1.2/ibmpairs.egg-info/dependency_links.txt
+-rw-r--r--   0 staylor    (501) staff       (20)        1 2024-05-24 15:41:57.000000 ibmpairs-3.1.2/ibmpairs.egg-info/not-zip-safe
+-rw-r--r--   0 staylor    (501) staff       (20)      273 2024-05-24 15:41:57.000000 ibmpairs-3.1.2/ibmpairs.egg-info/requires.txt
+-rw-r--r--   0 staylor    (501) staff       (20)        9 2024-05-24 15:41:57.000000 ibmpairs-3.1.2/ibmpairs.egg-info/top_level.txt
+-rw-r--r--   0 staylor    (501) staff       (20)       60 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/requirements-development.txt
+-rw-r--r--   0 staylor    (501) staff       (20)      270 2024-05-24 15:31:33.000000 ibmpairs-3.1.2/requirements.txt
+-rw-r--r--   0 staylor    (501) staff       (20)      103 2024-05-24 15:41:57.879813 ibmpairs-3.1.2/setup.cfg
+-rwxr-xr-x   0 staylor    (501) staff       (20)     1838 2024-05-24 15:35:37.000000 ibmpairs-3.1.2/setup.py
```

### Comparing `ibmpairs-3.1.1/CONTRIBUTING.md` & `ibmpairs-3.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/LICENSE` & `ibmpairs-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/PKG-INFO` & `ibmpairs-3.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,19 @@
-Metadata-Version: 2.1
-Name: ibmpairs
-Version: 3.1.1
-Summary: open source Python modules for the IBM PAIRS Geoscope platform
-Home-page: https://ibmpairs.mybluemix.net
-Author: Physical Analytics, IBM Research
-Author-email: pairs@us.ibm.com
-Maintainer: cmalbrec
-License: BSD-Clause-3
-Project-URL: Documentation, https://pairs.res.ibm.com/tutorial
-Project-URL: Source, https://github.com/ibm/ibmpairs
-Project-URL: Tracker, https://github.com/ibm/ibmpairs/issues
-Keywords: IBM PAIRS GIS BigGeoData
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: GIS
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # IBM Environmental Intelligence Suite (EIS): Geospatial Analytics open source modules
 
 [![Build Status](https://travis-ci.org/IBM/ibmpairs.svg?branch=master)](https://travis-ci.org/IBM/ibmpairs)
 [![PyPI Package](https://badge.fury.io/py/ibmpairs.svg)](https://pypi.org/project/ibmpairs/)
 
 
 This repository provides an interface to the geo-spatial big data platform
 [IBM EIS: Geospatial Analytics](https://www.ibm.com/products/environmental-intelligence-suite).
 
 E.g. the `query` module in the subdirectory `ibmpairs` serves as a wrapper employing the IBM EIS: 
 Geospatial Analytics core RESTful API served through the host reachable via
-[https://pairs.res.ibm.com](https://pairs.res.ibm.com/manual/api-doc/).
+[https://api.ibm.com/geospatial/run/na/core/v3/](https://pairs.res.ibm.com/manual/api-doc/).
 
 
 # General Notes
 
 If you like to contribute, please read [CONTRIBUTING.md](https://github.com/ibm/ibmpairs/blob/master/CONTRIBUTING.md)
 first. A list of maintainers is recorded in [MAINTAINERS.md](https://github.com/ibm/ibmpairs/blob/master/MAINTAINERS.md).
 
@@ -102,8 +82,8 @@
     --name ibmpairs \
     ibmpairs:latest
 ```
 or:
 ```Bash
 docker-compose up ibmpairs
 ```
-to run.
+to run.
```

### Comparing `ibmpairs-3.1.1/ibmpairs/authentication.py` & `ibmpairs-3.1.2/ibmpairs/authentication.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/ibmpairs/catalog.py` & `ibmpairs-3.1.2/ibmpairs/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -7477,15 +7477,15 @@
         :rtype: string
         """
 
         return json.dumps(self.to_dict_data_layer_put())
         
     #
     def display(self,
-                columns: List[str] = ['dataset_id', 'id', 'name', 'description_short', 'description_long', 'level', 'type', 'unit']
+                columns: List[str] = ['dataset_id', 'id', 'name', 'description_short', 'description_long', 'level', 'type', 'units']
                ):
                 
         """
         A method to return a pandas.DataFrame object of a get result.
         
         :param columns: The columns to be returned in the pandas.DataFrame object, defaults to ['dataset_id', 'id', 'name', 'description_short', 'description_long', 'level', 'type', 'unit']
         :type columns:  List[str]
```

### Comparing `ibmpairs-3.1.1/ibmpairs/client.py` & `ibmpairs-3.1.2/ibmpairs/client.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/ibmpairs/common.py` & `ibmpairs-3.1.2/ibmpairs/common.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/ibmpairs/config.py` & `ibmpairs-3.1.2/ibmpairs/config.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/ibmpairs/constants.py` & `ibmpairs-3.1.2/ibmpairs/constants.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/ibmpairs/dashboard.py` & `ibmpairs-3.1.2/ibmpairs/dashboard.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/ibmpairs/external/ibm.py` & `ibmpairs-3.1.2/ibmpairs/external/ibm.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/ibmpairs/messages.py` & `ibmpairs-3.1.2/ibmpairs/messages.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/ibmpairs/paw.py` & `ibmpairs-3.1.2/ibmpairs/paw.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/ibmpairs/query.py` & `ibmpairs-3.1.2/ibmpairs/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -2880,14 +2880,15 @@
     #_ex_percent: int
     #_flag: bool
     #_hadoop_id: str
     #_ready: bool
     #_rt_status: str
     #_pd_status: str
     #_status_code: int
+    #_message: str
     
     """
     A representation of a Query Job.
     
     :param id:          Query ID.
     :type id:           str
     :param status:      Query status.
@@ -2914,14 +2915,16 @@
     :type ready:        bool
     :param rt_status:   RT status.
     :type rt_status:    str
     :param pd_status:   PD status.
     :type pd_status:    str
     :param status_code: Status code.
     :type status_code:  int
+    :param message:     Query message.
+    :type message:      str
     """
 
     #
     def __str__(self):
                                                     
         """
         The method creates a string representation of the internal class structure.
@@ -2960,15 +2963,16 @@
                  nickname: str    = None, 
                  ex_percent: int  = None, 
                  flag: bool       = None, 
                  hadoop_id: str   = None, 
                  ready: bool      = None, 
                  rt_status: str   = None, 
                  pd_status: str   = None, 
-                 status_code: int = None
+                 status_code: int = None,
+                 message: str     = None
                 ):
         self._id          = id
         self._status      = status
         self._start       = start
         self._sw_lat      = sw_lat
         self._sw_lon      = sw_lon
         self._ne_lat      = ne_lat
@@ -2977,14 +2981,15 @@
         self._ex_percent  = ex_percent
         self._flag        = flag
         self._hadoop_id   = hadoop_id
         self._ready       = ready
         self._rt_status   = rt_status
         self._pd_status   = pd_status
         self._status_code = status_code
+        self._message     = message
 
     #
     def get_id(self):
         return self._id
 
     #
     def set_id(self, id):
@@ -3204,14 +3209,29 @@
     def del_status_code(self): 
         del self._status_code
 
     #    
     status_code = property(get_status_code, set_status_code, del_status_code)
     
     #
+    def get_message(self):
+        return self._message
+  
+    #
+    def set_message(self, message):
+        self._message = common.check_str(message)
+      
+    #
+    def del_message(self): 
+        del self._message
+      
+    #
+    message = property(get_message, set_message, del_message)
+    
+    #
     def from_dict(query_job_dict: Any):
 
         """
         Create a QueryJob object from a dictionary.
         
         :param query_job_dict:    A dictionary that contains the keys of a QueryJob.
         :type query_job_dict:     Any             
@@ -3230,14 +3250,15 @@
         ex_percent  = None
         flag        = None
         hadoop_id   = None
         ready       = None
         rt_status   = None
         pd_status   = None
         status_code = None
+        message     = None
         
         common.check_dict(query_job_dict)
         if "id" in query_job_dict:
             if query_job_dict.get("id") is not None:
                 id = common.check_str(query_job_dict.get("id"))
         if "status" in query_job_dict:
             if query_job_dict.get("status") is not None:
@@ -3304,29 +3325,33 @@
                 pd_status = common.check_str(query_job_dict.get("pd_status"))
         if "statusCode" in query_job_dict:
             if query_job_dict.get("statusCode") is not None:
                 status_code = common.check_int(query_job_dict.get("statusCode"))
         elif "status_code" in query_job_dict:
             if query_job_dict.get("status_code") is not None:
                 status_code = common.check_int(query_job_dict.get("status_code"))
+        if "message" in query_job_dict:
+            if query_job_dict.get("message") is not None:
+                message = common.check_str(query_job_dict.get("message"))
         return QueryJob(id          = id,
                         status      = status,
                         start       = start,
                         sw_lat      = sw_lat,
                         sw_lon      = sw_lon,
                         ne_lat      = ne_lat,
                         ne_lon      = ne_lon,
                         nickname    = nickname,
                         ex_percent  = ex_percent,
                         flag        = flag,
                         hadoop_id   = hadoop_id,
                         ready       = ready,
                         rt_status   = rt_status,
                         pd_status   = pd_status,
-                        status_code = status_code
+                        status_code = status_code,
+                        message     = message
                        )
 
     #
     def to_dict(self):
         
         """
         Create a dictionary from the objects structure. 
@@ -3361,14 +3386,16 @@
             query_job_dict["ready"] = self._ready
         if self._rt_status is not None:
             query_job_dict["rt_status"] = self._rt_status
         if self._pd_status is not None:
             query_job_dict["pd_status"] = self._pd_status
         if self._status_code is not None:
             query_job_dict["status_code"] = self._status_code
+        if self._message is not None:
+            query_job_dict["message"] = self._message
         return query_job_dict
         
     #
     def from_json(query_job_json: Any):
 
         """
         Create a QueryJob object from json (dictonary or str).
```

### Comparing `ibmpairs-3.1.1/ibmpairs/upload.py` & `ibmpairs-3.1.2/ibmpairs/upload.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/ibmpairs/utils.py` & `ibmpairs-3.1.2/ibmpairs/utils.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/ibmpairs.egg-info/SOURCES.txt` & `ibmpairs-3.1.2/ibmpairs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibmpairs-3.1.1/setup.py` & `ibmpairs-3.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 # define package version
-version = '3.1.1'
+version = '3.1.2'
 # ... and record it for ibmpairs package
 with open("ibmpairs/version.py", 'w') as f:
     f.write('# generated by setup.py\nversion = "{}"\n'.format(version))
 
 def readme():
     try:
         with open('README.md') as f:
```

