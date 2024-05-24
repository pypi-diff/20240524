# Comparing `tmp/secretscraper-1.3.9.4.tar.gz` & `tmp/secretscraper-1.3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.9.4.tar", max compression
+gzip compressed data, was "secretscraper-1.3.9.5.tar", max compression
```

## Comparing `secretscraper-1.3.9.4.tar` & `secretscraper-1.3.9.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.9.4/LICENSE
--rw-r--r--   0        0        0     9074 2024-04-30 10:24:02.401501 secretscraper-1.3.9.4/README.md
--rw-r--r--   0        0        0     1910 2024-05-24 03:08:16.583332 secretscraper-1.3.9.4/pyproject.toml
--rw-r--r--   0        0        0       45 2024-05-24 03:07:23.229353 secretscraper-1.3.9.4/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     7755 2024-04-30 09:48:52.854355 secretscraper-1.3.9.4/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.9.4/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2716 2024-05-24 03:03:31.799544 secretscraper-1.3.9.4/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.9.4/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    17214 2024-04-30 08:49:48.323754 secretscraper-1.3.9.4/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.9.4/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.9.4/src/secretscraper/exception.py
--rw-r--r--   0        0        0    14636 2024-05-24 03:03:31.805841 secretscraper-1.3.9.4/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.9.4/src/secretscraper/filter.py
--rw-r--r--   0        0        0     6774 2024-04-30 09:28:19.272007 secretscraper-1.3.9.4/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1910 2024-04-30 07:31:20.191193 secretscraper-1.3.9.4/src/secretscraper/log.py
--rw-r--r--   0        0        0     8822 2024-04-30 07:39:46.452140 secretscraper-1.3.9.4/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.9.4/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4596 2024-04-30 03:29:52.175016 secretscraper-1.3.9.4/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     2862 2024-04-30 06:43:03.216699 secretscraper-1.3.9.4/src/secretscraper/util.py
--rw-r--r--   0        0        0    10558 1970-01-01 00:00:00.000000 secretscraper-1.3.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.9.5/LICENSE
+-rw-r--r--   0        0        0     9074 2024-05-24 03:17:08.607752 secretscraper-1.3.9.5/README.md
+-rw-r--r--   0        0        0     1910 2024-05-24 05:23:19.508113 secretscraper-1.3.9.5/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-05-24 05:22:09.924148 secretscraper-1.3.9.5/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     7755 2024-04-30 09:48:52.854355 secretscraper-1.3.9.5/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.9.5/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2716 2024-05-24 03:03:31.799544 secretscraper-1.3.9.5/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.9.5/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    17291 2024-05-24 05:21:32.853650 secretscraper-1.3.9.5/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1503 2024-05-24 05:17:11.505719 secretscraper-1.3.9.5/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.9.5/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    14636 2024-05-24 03:03:31.805841 secretscraper-1.3.9.5/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.9.5/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6774 2024-04-30 09:28:19.272007 secretscraper-1.3.9.5/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1910 2024-04-30 07:31:20.191193 secretscraper-1.3.9.5/src/secretscraper/log.py
+-rw-r--r--   0        0        0     8822 2024-04-30 07:39:46.452140 secretscraper-1.3.9.5/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.9.5/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4596 2024-04-30 03:29:52.175016 secretscraper-1.3.9.5/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     3242 2024-05-24 05:21:32.849996 secretscraper-1.3.9.5/src/secretscraper/util.py
+-rw-r--r--   0        0        0    10558 1970-01-01 00:00:00.000000 secretscraper-1.3.9.5/PKG-INFO
```

### Comparing `secretscraper-1.3.9.4/LICENSE` & `secretscraper-1.3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.4/README.md` & `secretscraper-1.3.9.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 - Support multiple targets, input target URLs from a file
 - Support local file scan
 - Scalable customization: header, proxy, timeout, cookie, scrape depth, follow redirect, etc.
 - Built-in regex to search for sensitive information
 - Flexible configuration in yaml format
 
 ## Prerequisite
-- Platform: Test on MaxOS, Ubuntu and Windows.
+- Platform: Test on MacOS, Ubuntu and Windows.
 - Python Version >= 3.9
 
 ## Usage
 
 ### Install
 
 ```bash
```

### Comparing `secretscraper-1.3.9.4/pyproject.toml` & `secretscraper-1.3.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.9.4"
+version = "1.3.9.5"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
```

### Comparing `secretscraper-1.3.9.4/src/secretscraper/cmdline.py` & `secretscraper-1.3.9.5/src/secretscraper/cmdline.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.4/src/secretscraper/config/__init__.py` & `secretscraper-1.3.9.5/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.4/src/secretscraper/config/settings.yml` & `secretscraper-1.3.9.5/src/secretscraper/config/settings.yml`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.4/src/secretscraper/coroutinue.py` & `secretscraper-1.3.9.5/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.4/src/secretscraper/crawler.py` & `secretscraper-1.3.9.5/src/secretscraper/crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from secretscraper.filter import URLFilter
 from secretscraper.handler import Handler
 from secretscraper.urlparser import URLParser
 from aiocache.serializers import PickleSerializer
 
 from .config import settings
 from .exception import CrawlerException
-from .util import Range
+from .util import Range, get_response_title
 
 logger = logging.getLogger(__name__)
 
 
 class Crawler:
     """Crawler interface"""
 
@@ -240,15 +240,15 @@
             logger.debug(f"Evading {url_node}")
             return
         logger.debug(f"Processing {url_node.url}")
         self.total_page += 1
         response = await self.fetch(url_node.url)
         if response is not None:  # and response.status == 200
             url_node.response_status = str(response.status_code)
-
+            url_node.title = get_response_title(response)
             response_text: str = response.text
             # try:
             #     response_text: str = await response.text(
             #         encoding="utf8", errors="ignore"
             #     )
             # except TimeoutError:
             #     logger.error(f"Timeout while reading response from {url_node.url}")
```

### Comparing `secretscraper-1.3.9.4/src/secretscraper/entity.py` & `secretscraper-1.3.9.5/src/secretscraper/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     """
 
     url: str = field(hash=False, compare=False)
     url_object: ParseResult = field(hash=True, compare=True)
     response_status: str = field(default="Unknown", hash=False, compare=False)
     depth: int = field(default=0, hash=False, compare=False)
     parent: typing.Optional["URLNode"] = field(default=None, hash=False, compare=False)
+    title:str = field(hash=False, compare=False, default="")
 
     def __post_init__(self):
         if self.parent is not None and self.depth <= self.parent.depth:
             raise ValueError(
                 f"URLNode: depth({self.depth}) must be greater than that of parent({self.parent.depth})"
             )
```

### Comparing `secretscraper-1.3.9.4/src/secretscraper/exception.py` & `secretscraper-1.3.9.5/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.4/src/secretscraper/facade.py` & `secretscraper-1.3.9.5/src/secretscraper/facade.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.4/src/secretscraper/filter.py` & `secretscraper-1.3.9.5/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.4/src/secretscraper/handler.py` & `secretscraper-1.3.9.5/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.4/src/secretscraper/log.py` & `secretscraper-1.3.9.5/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.4/src/secretscraper/output_formatter.py` & `secretscraper-1.3.9.5/src/secretscraper/output_formatter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.4/src/secretscraper/scanner.py` & `secretscraper-1.3.9.5/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.4/src/secretscraper/urlparser.py` & `secretscraper-1.3.9.5/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.4/src/secretscraper/util.py` & `secretscraper-1.3.9.5/src/secretscraper/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Common utility functions."""
 
 import re
 import typing
 from collections import namedtuple
 from urllib.parse import urlparse
+
+import requests
 import tldextract
+from bs4 import BeautifulSoup
 
 # from dynaconf import LazySettings
 
 from .entity import URL
 from .exception import SecretScraperException
 
 Range = namedtuple("Range", ["start", "end"])
@@ -95,7 +98,17 @@
 def is_hyperscan() -> bool:
     """Check if hyperscan is usable"""
     try:
         import hyperscan
         return True
     except ImportError:
         return False
+
+
+def get_response_title(response: requests.Response) -> str:
+    """Get the response title"""
+    bs = BeautifulSoup(response.text, "html.parser")
+    titles = list()
+    for t in bs.find_all('title'):
+        text = t.get_text()
+        titles.append(text.replace("\n", " ").replace("\r", " ").strip())
+    return "|".join(titles)
```

### Comparing `secretscraper-1.3.9.4/PKG-INFO` & `secretscraper-1.3.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.9.4
+Version: 1.3.9.5
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,15 @@
 - Support multiple targets, input target URLs from a file
 - Support local file scan
 - Scalable customization: header, proxy, timeout, cookie, scrape depth, follow redirect, etc.
 - Built-in regex to search for sensitive information
 - Flexible configuration in yaml format
 
 ## Prerequisite
-- Platform: Test on MaxOS, Ubuntu and Windows.
+- Platform: Test on MacOS, Ubuntu and Windows.
 - Python Version >= 3.9
 
 ## Usage
 
 ### Install
 
 ```bash
```

