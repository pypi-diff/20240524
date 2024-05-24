# Comparing `tmp/secretscraper-1.3.9.5.tar.gz` & `tmp/secretscraper-1.3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.9.5.tar", max compression
+gzip compressed data, was "secretscraper-1.3.9.6.tar", max compression
```

## Comparing `secretscraper-1.3.9.5.tar` & `secretscraper-1.3.9.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.9.5/LICENSE
--rw-r--r--   0        0        0     9074 2024-05-24 03:17:08.607752 secretscraper-1.3.9.5/README.md
--rw-r--r--   0        0        0     1910 2024-05-24 05:23:19.508113 secretscraper-1.3.9.5/pyproject.toml
--rw-r--r--   0        0        0       45 2024-05-24 05:22:09.924148 secretscraper-1.3.9.5/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     7755 2024-04-30 09:48:52.854355 secretscraper-1.3.9.5/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.9.5/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2716 2024-05-24 03:03:31.799544 secretscraper-1.3.9.5/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.9.5/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    17291 2024-05-24 05:21:32.853650 secretscraper-1.3.9.5/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1503 2024-05-24 05:17:11.505719 secretscraper-1.3.9.5/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.9.5/src/secretscraper/exception.py
--rw-r--r--   0        0        0    14636 2024-05-24 03:03:31.805841 secretscraper-1.3.9.5/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.9.5/src/secretscraper/filter.py
--rw-r--r--   0        0        0     6774 2024-04-30 09:28:19.272007 secretscraper-1.3.9.5/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1910 2024-04-30 07:31:20.191193 secretscraper-1.3.9.5/src/secretscraper/log.py
--rw-r--r--   0        0        0     8822 2024-04-30 07:39:46.452140 secretscraper-1.3.9.5/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.9.5/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4596 2024-04-30 03:29:52.175016 secretscraper-1.3.9.5/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     3242 2024-05-24 05:21:32.849996 secretscraper-1.3.9.5/src/secretscraper/util.py
--rw-r--r--   0        0        0    10558 1970-01-01 00:00:00.000000 secretscraper-1.3.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.9.6/LICENSE
+-rw-r--r--   0        0        0     9074 2024-05-24 03:17:08.607752 secretscraper-1.3.9.6/README.md
+-rw-r--r--   0        0        0     1910 2024-05-24 05:59:47.808658 secretscraper-1.3.9.6/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-05-24 05:59:52.266448 secretscraper-1.3.9.6/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     7755 2024-04-30 09:48:52.854355 secretscraper-1.3.9.6/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.9.6/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2716 2024-05-24 03:03:31.799544 secretscraper-1.3.9.6/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.9.6/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    17291 2024-05-24 05:21:32.853650 secretscraper-1.3.9.6/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1503 2024-05-24 05:17:11.505719 secretscraper-1.3.9.6/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.9.6/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    14636 2024-05-24 03:03:31.805841 secretscraper-1.3.9.6/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.9.6/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6774 2024-04-30 09:28:19.272007 secretscraper-1.3.9.6/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1910 2024-04-30 07:31:20.191193 secretscraper-1.3.9.6/src/secretscraper/log.py
+-rw-r--r--   0        0        0     8822 2024-04-30 07:39:46.452140 secretscraper-1.3.9.6/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.9.6/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4596 2024-04-30 03:29:52.175016 secretscraper-1.3.9.6/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     3901 2024-05-24 05:59:07.971762 secretscraper-1.3.9.6/src/secretscraper/util.py
+-rw-r--r--   0        0        0    10558 1970-01-01 00:00:00.000000 secretscraper-1.3.9.6/PKG-INFO
```

### Comparing `secretscraper-1.3.9.5/LICENSE` & `secretscraper-1.3.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/README.md` & `secretscraper-1.3.9.6/README.md`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/pyproject.toml` & `secretscraper-1.3.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.9.5"
+version = "1.3.9.6"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
```

### Comparing `secretscraper-1.3.9.5/src/secretscraper/cmdline.py` & `secretscraper-1.3.9.6/src/secretscraper/cmdline.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/config/__init__.py` & `secretscraper-1.3.9.6/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/config/settings.yml` & `secretscraper-1.3.9.6/src/secretscraper/config/settings.yml`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/coroutinue.py` & `secretscraper-1.3.9.6/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/crawler.py` & `secretscraper-1.3.9.6/src/secretscraper/crawler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/entity.py` & `secretscraper-1.3.9.6/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/exception.py` & `secretscraper-1.3.9.6/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/facade.py` & `secretscraper-1.3.9.6/src/secretscraper/facade.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/filter.py` & `secretscraper-1.3.9.6/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/handler.py` & `secretscraper-1.3.9.6/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/log.py` & `secretscraper-1.3.9.6/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/output_formatter.py` & `secretscraper-1.3.9.6/src/secretscraper/output_formatter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/scanner.py` & `secretscraper-1.3.9.6/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/urlparser.py` & `secretscraper-1.3.9.6/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.5/src/secretscraper/util.py` & `secretscraper-1.3.9.6/src/secretscraper/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Common utility functions."""
 
 import re
 import typing
 from collections import namedtuple
+from pathlib import Path
 from urllib.parse import urlparse
-
+from threading import Thread
 import requests
 import tldextract
 from bs4 import BeautifulSoup
 
 # from dynaconf import LazySettings
 
 from .entity import URL
@@ -108,7 +109,26 @@
     """Get the response title"""
     bs = BeautifulSoup(response.text, "html.parser")
     titles = list()
     for t in bs.find_all('title'):
         text = t.get_text()
         titles.append(text.replace("\n", " ").replace("\r", " ").strip())
     return "|".join(titles)
+
+
+import http.server
+
+
+def start_local_test_http_server(host: str, port: int) -> tuple[Thread, http.server.HTTPServer]:
+    """Start local test server"""
+
+    DIR = str(
+        Path(__file__).parent.parent.parent.joinpath("tests").joinpath("resources").joinpath("local_server").absolute())
+
+    class Handler(http.server.SimpleHTTPRequestHandler):
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, directory=DIR, **kwargs)
+
+    httpd = http.server.HTTPServer((host, port), Handler)
+    thread = Thread(target=httpd.serve_forever)
+    thread.start()
+    return thread, httpd
```

### Comparing `secretscraper-1.3.9.5/PKG-INFO` & `secretscraper-1.3.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.9.5
+Version: 1.3.9.6
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

