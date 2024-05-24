# Comparing `tmp/scrapfly-sdk-0.8.8.tar.gz` & `tmp/scrapfly-sdk-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapfly-sdk-0.8.8.tar", last modified: Thu Jul 27 12:38:19 2023, max compression
+gzip compressed data, was "scrapfly-sdk-0.8.9.tar", last modified: Tue Sep 12 09:25:51 2023, max compression
```

## Comparing `scrapfly-sdk-0.8.8.tar` & `scrapfly-sdk-0.8.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/
--rw-r--r--   0 johann    (1000) johann    (1000)     1390 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.8/LICENSE
--rw-r--r--   0 johann    (1000) johann    (1000)     2727 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/PKG-INFO
--rw-r--r--   0 johann    (1000) johann    (1000)     1451 2023-02-21 22:10:41.000000 scrapfly-sdk-0.8.8/README.md
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-07-27 12:38:19.311485 scrapfly-sdk-0.8.8/scrapfly/
--rw-r--r--   0 johann    (1000) johann    (1000)     1336 2023-06-08 02:08:56.000000 scrapfly-sdk-0.8.8/scrapfly/__init__.py
--rw-r--r--   0 johann    (1000) johann    (1000)    16613 2022-06-14 19:45:38.000000 scrapfly-sdk-0.8.8/scrapfly/api_response.py
--rw-r--r--   0 johann    (1000) johann    (1000)    15969 2023-02-21 22:13:29.000000 scrapfly-sdk-0.8.8/scrapfly/client.py
--rw-r--r--   0 johann    (1000) johann    (1000)     7244 2023-06-08 02:00:48.000000 scrapfly-sdk-0.8.8/scrapfly/errors.py
--rw-r--r--   0 johann    (1000) johann    (1000)      653 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.8/scrapfly/frozen_dict.py
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/scrapfly/polyfill/
--rw-r--r--   0 johann    (1000) johann    (1000)        0 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.8/scrapfly/polyfill/__init__.py
--rw-r--r--   0 johann    (1000) johann    (1000)      556 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.8/scrapfly/polyfill/cached_property.py
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/scrapfly/reporter/
--rw-r--r--   0 johann    (1000) johann    (1000)      406 2021-12-18 23:00:36.000000 scrapfly-sdk-0.8.8/scrapfly/reporter/ChainReporter.py
--rw-r--r--   0 johann    (1000) johann    (1000)      214 2021-12-18 22:59:57.000000 scrapfly-sdk-0.8.8/scrapfly/reporter/NoopReporter.py
--rw-r--r--   0 johann    (1000) johann    (1000)      944 2021-12-19 00:22:06.000000 scrapfly-sdk-0.8.8/scrapfly/reporter/PrintReporter.py
--rw-r--r--   0 johann    (1000) johann    (1000)     1164 2022-04-30 01:02:19.000000 scrapfly-sdk-0.8.8/scrapfly/reporter/SentryReporter.py
--rw-r--r--   0 johann    (1000) johann    (1000)      792 2021-12-18 22:59:04.000000 scrapfly-sdk-0.8.8/scrapfly/reporter/__init__.py
--rw-r--r--   0 johann    (1000) johann    (1000)    11339 2023-02-24 16:27:20.000000 scrapfly-sdk-0.8.8/scrapfly/scrape_config.py
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/scrapfly/scrapy/
--rw-r--r--   0 johann    (1000) johann    (1000)      473 2022-05-16 00:35:14.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/__init__.py
--rw-r--r--   0 johann    (1000) johann    (1000)     4924 2022-05-13 14:57:24.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/downloader.py
--rw-r--r--   0 johann    (1000) johann    (1000)     3163 2023-06-08 02:00:48.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/middleware.py
--rw-r--r--   0 johann    (1000) johann    (1000)     1800 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/pipelines.py
--rw-r--r--   0 johann    (1000) johann    (1000)     1293 2022-04-05 19:53:12.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/request.py
--rw-r--r--   0 johann    (1000) johann    (1000)     3133 2022-04-05 19:58:38.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/response.py
--rw-r--r--   0 johann    (1000) johann    (1000)     8774 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/spider.py
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/
--rw-r--r--   0 johann    (1000) johann    (1000)     2727 2023-07-27 12:38:19.000000 scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/PKG-INFO
--rw-r--r--   0 johann    (1000) johann    (1000)      784 2023-07-27 12:38:19.000000 scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 johann    (1000) johann    (1000)        1 2023-07-27 12:38:19.000000 scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 johann    (1000) johann    (1000)      556 2023-07-27 12:38:19.000000 scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/requires.txt
--rw-r--r--   0 johann    (1000) johann    (1000)        9 2023-07-27 12:38:19.000000 scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/top_level.txt
--rw-r--r--   0 johann    (1000) johann    (1000)      272 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/setup.cfg
--rw-r--r--   0 johann    (1000) johann    (1000)     3323 2023-07-27 12:32:43.000000 scrapfly-sdk-0.8.8/setup.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-09-12 09:25:51.040212 scrapfly-sdk-0.8.9/
+-rw-r--r--   0 johann    (1000) johann    (1000)     1390 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.9/LICENSE
+-rw-r--r--   0 johann    (1000) johann    (1000)     2727 2023-09-12 09:25:51.040212 scrapfly-sdk-0.8.9/PKG-INFO
+-rw-r--r--   0 johann    (1000) johann    (1000)     1451 2023-02-21 22:10:41.000000 scrapfly-sdk-0.8.9/README.md
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-09-12 09:25:51.040212 scrapfly-sdk-0.8.9/scrapfly/
+-rw-r--r--   0 johann    (1000) johann    (1000)     1336 2023-07-27 12:38:25.000000 scrapfly-sdk-0.8.9/scrapfly/__init__.py
+-rw-r--r--   0 johann    (1000) johann    (1000)    17023 2023-09-12 09:17:56.000000 scrapfly-sdk-0.8.9/scrapfly/api_response.py
+-rw-r--r--   0 johann    (1000) johann    (1000)    15969 2023-02-21 22:13:29.000000 scrapfly-sdk-0.8.9/scrapfly/client.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     7244 2023-06-08 02:00:48.000000 scrapfly-sdk-0.8.9/scrapfly/errors.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      653 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.9/scrapfly/frozen_dict.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-09-12 09:25:51.040212 scrapfly-sdk-0.8.9/scrapfly/polyfill/
+-rw-r--r--   0 johann    (1000) johann    (1000)        0 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.9/scrapfly/polyfill/__init__.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      556 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.9/scrapfly/polyfill/cached_property.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-09-12 09:25:51.040212 scrapfly-sdk-0.8.9/scrapfly/reporter/
+-rw-r--r--   0 johann    (1000) johann    (1000)      406 2021-12-18 23:00:36.000000 scrapfly-sdk-0.8.9/scrapfly/reporter/ChainReporter.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      214 2021-12-18 22:59:57.000000 scrapfly-sdk-0.8.9/scrapfly/reporter/NoopReporter.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      944 2021-12-19 00:22:06.000000 scrapfly-sdk-0.8.9/scrapfly/reporter/PrintReporter.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     1164 2022-04-30 01:02:19.000000 scrapfly-sdk-0.8.9/scrapfly/reporter/SentryReporter.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      792 2021-12-18 22:59:04.000000 scrapfly-sdk-0.8.9/scrapfly/reporter/__init__.py
+-rw-r--r--   0 johann    (1000) johann    (1000)    11339 2023-02-24 16:27:20.000000 scrapfly-sdk-0.8.9/scrapfly/scrape_config.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-09-12 09:25:51.040212 scrapfly-sdk-0.8.9/scrapfly/scrapy/
+-rw-r--r--   0 johann    (1000) johann    (1000)      473 2022-05-16 00:35:14.000000 scrapfly-sdk-0.8.9/scrapfly/scrapy/__init__.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     4924 2022-05-13 14:57:24.000000 scrapfly-sdk-0.8.9/scrapfly/scrapy/downloader.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     3163 2023-06-08 02:00:48.000000 scrapfly-sdk-0.8.9/scrapfly/scrapy/middleware.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     1800 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.9/scrapfly/scrapy/pipelines.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     1293 2022-04-05 19:53:12.000000 scrapfly-sdk-0.8.9/scrapfly/scrapy/request.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     3133 2022-04-05 19:58:38.000000 scrapfly-sdk-0.8.9/scrapfly/scrapy/response.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     8774 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.9/scrapfly/scrapy/spider.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-09-12 09:25:51.040212 scrapfly-sdk-0.8.9/scrapfly_sdk.egg-info/
+-rw-r--r--   0 johann    (1000) johann    (1000)     2727 2023-09-12 09:25:51.000000 scrapfly-sdk-0.8.9/scrapfly_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 johann    (1000) johann    (1000)      784 2023-09-12 09:25:51.000000 scrapfly-sdk-0.8.9/scrapfly_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)        1 2023-09-12 09:25:51.000000 scrapfly-sdk-0.8.9/scrapfly_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)      556 2023-09-12 09:25:51.000000 scrapfly-sdk-0.8.9/scrapfly_sdk.egg-info/requires.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)        9 2023-09-12 09:25:51.000000 scrapfly-sdk-0.8.9/scrapfly_sdk.egg-info/top_level.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)      272 2023-09-12 09:25:51.040212 scrapfly-sdk-0.8.9/setup.cfg
+-rw-r--r--   0 johann    (1000) johann    (1000)     3323 2023-07-27 12:32:43.000000 scrapfly-sdk-0.8.9/setup.py
```

### Comparing `scrapfly-sdk-0.8.8/LICENSE` & `scrapfly-sdk-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/PKG-INFO` & `scrapfly-sdk-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapfly-sdk
-Version: 0.8.8
+Version: 0.8.9
 Summary: Scrapfly SDK for Scrapfly
 Home-page: https://github.com/scrapfly/python-sdk
 Author: Scrapfly
 Author-email: tech@scrapfly.io
 License: BSD
 Project-URL: Company, https://scrapfly.io
 Project-URL: Documentation, https://scrapfly.io/docs
```

### Comparing `scrapfly-sdk-0.8.8/README.md` & `scrapfly-sdk-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/__init__.py` & `scrapfly-sdk-0.8.9/scrapfly/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.8.8'
+__version__ = '0.8.9'
 
 from typing import Tuple
 from .errors import ScrapflyError
 from .errors import ScrapflyAspError
 from .errors import ScrapflyProxyError
 from .errors import ScrapflyScheduleError
 from .errors import ScrapflyScrapeError
```

### Comparing `scrapfly-sdk-0.8.8/scrapfly/api_response.py` & `scrapfly-sdk-0.8.9/scrapfly/api_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,15 +350,25 @@
 
         if self.response.status_code != 200:
             return None
 
         response = Response()
         response.status_code = self.scrape_result['status_code']
         response.reason = self.scrape_result['reason']
-        response._content = self.scrape_result['content'].encode('utf-8') if self.scrape_result['content'] else None
+
+        if self.scrape_result['content']:
+            if isinstance(self.scrape_result['content'], BytesIO):
+                response._content = self.scrape_result['content'].getvalue()
+            elif isinstance(self.scrape_result['content'], bytes):
+                response._content = self.scrape_result['content']
+            elif isinstance(self.scrape_result['content'], str):
+                response._content = self.scrape_result['content'].encode('utf-8')
+        else:
+            response._content = None
+        
         response.headers.update(self.scrape_result['response_headers'])
         response.url = self.scrape_result['url']
 
         response.request = Request(
             method=self.config['method'],
             url=self.config['url'],
             headers=self.scrape_result['request_headers'],
```

### Comparing `scrapfly-sdk-0.8.8/scrapfly/client.py` & `scrapfly-sdk-0.8.9/scrapfly/client.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/errors.py` & `scrapfly-sdk-0.8.9/scrapfly/errors.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/frozen_dict.py` & `scrapfly-sdk-0.8.9/scrapfly/frozen_dict.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/polyfill/cached_property.py` & `scrapfly-sdk-0.8.9/scrapfly/polyfill/cached_property.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/reporter/PrintReporter.py` & `scrapfly-sdk-0.8.9/scrapfly/reporter/PrintReporter.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/reporter/SentryReporter.py` & `scrapfly-sdk-0.8.9/scrapfly/reporter/SentryReporter.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/reporter/__init__.py` & `scrapfly-sdk-0.8.9/scrapfly/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/scrape_config.py` & `scrapfly-sdk-0.8.9/scrapfly/scrape_config.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/scrapy/downloader.py` & `scrapfly-sdk-0.8.9/scrapfly/scrapy/downloader.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/scrapy/middleware.py` & `scrapfly-sdk-0.8.9/scrapfly/scrapy/middleware.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/scrapy/pipelines.py` & `scrapfly-sdk-0.8.9/scrapfly/scrapy/pipelines.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/scrapy/request.py` & `scrapfly-sdk-0.8.9/scrapfly/scrapy/request.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/scrapy/response.py` & `scrapfly-sdk-0.8.9/scrapfly/scrapy/response.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly/scrapy/spider.py` & `scrapfly-sdk-0.8.9/scrapfly/scrapy/spider.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/PKG-INFO` & `scrapfly-sdk-0.8.9/scrapfly_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapfly-sdk
-Version: 0.8.8
+Version: 0.8.9
 Summary: Scrapfly SDK for Scrapfly
 Home-page: https://github.com/scrapfly/python-sdk
 Author: Scrapfly
 Author-email: tech@scrapfly.io
 License: BSD
 Project-URL: Company, https://scrapfly.io
 Project-URL: Documentation, https://scrapfly.io/docs
```

### Comparing `scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/SOURCES.txt` & `scrapfly-sdk-0.8.9/scrapfly_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/requires.txt` & `scrapfly-sdk-0.8.9/scrapfly_sdk.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 requests>=2.25.0
 python-dateutil<3.0.0,>=2.1
 loguru>=0.5
 urllib3>=1.26.0
 backoff>=1.10.0
 
 [all]
-brotlipy
-setuptools
 pdoc3
-scrapy>=2.4.0
-lxml
-pip
-bumpversion
-readme_renderer
-wheel
-isort
+setuptools
 colorama
-soupsieve
-extruct
+brotlipy
+msgpack
+wheel
+readme_renderer
 twine
 beautifulsoup4
+soupsieve
+scrapy>=2.4.0
+extruct
+pip
+lxml
 sentry-sdk
-msgpack
+bumpversion
+isort
 
 [concurrency]
 
 [deploy]
 bumpversion
 isort
 readme_renderer
```

### Comparing `scrapfly-sdk-0.8.8/setup.py` & `scrapfly-sdk-0.8.9/setup.py`

 * *Files identical despite different names*

