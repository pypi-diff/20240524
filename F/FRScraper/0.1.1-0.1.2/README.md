# Comparing `tmp/frscraper-0.1.1.tar.gz` & `tmp/frscraper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frscraper-0.1.1.tar", last modified: Fri May 24 02:40:17 2024, max compression
+gzip compressed data, was "frscraper-0.1.2.tar", last modified: Fri May 24 02:46:06 2024, max compression
```

## Comparing `frscraper-0.1.1.tar` & `frscraper-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 02:40:17.743239 frscraper-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-05-24 02:40:17.738256 frscraper-0.1.1/FRScraper/
--rw-rw-rw-   0        0        0     9268 2024-05-22 01:30:37.000000 frscraper-0.1.1/FRScraper/FRScraper.py
--rw-rw-rw-   0        0        0        0 2023-03-10 22:31:23.000000 frscraper-0.1.1/FRScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 02:40:17.742242 frscraper-0.1.1/FRScraper.egg-info/
--rw-rw-rw-   0        0        0     3198 2024-05-24 02:40:17.000000 frscraper-0.1.1/FRScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-05-24 02:40:17.000000 frscraper-0.1.1/FRScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 02:40:17.000000 frscraper-0.1.1/FRScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-05-24 02:40:17.000000 frscraper-0.1.1/FRScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-24 02:40:17.000000 frscraper-0.1.1/FRScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1075 2023-03-12 19:02:09.000000 frscraper-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3198 2024-05-24 02:40:17.742242 frscraper-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2396 2024-05-24 02:38:21.000000 frscraper-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 02:40:17.743239 frscraper-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1319 2024-05-24 02:40:00.000000 frscraper-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 02:46:06.534997 frscraper-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-05-24 02:46:06.534000 frscraper-0.1.2/FRScraper.egg-info/
+-rw-rw-rw-   0        0        0     3198 2024-05-24 02:46:06.000000 frscraper-0.1.2/FRScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-24 02:46:06.000000 frscraper-0.1.2/FRScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 02:46:06.000000 frscraper-0.1.2/FRScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-24 02:46:06.000000 frscraper-0.1.2/FRScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 02:46:06.000000 frscraper-0.1.2/FRScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1075 2023-03-12 19:02:09.000000 frscraper-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3198 2024-05-24 02:46:06.534000 frscraper-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2396 2024-05-24 02:38:21.000000 frscraper-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 02:46:06.534997 frscraper-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1319 2024-05-24 02:45:59.000000 frscraper-0.1.2/setup.py
```

### Comparing `frscraper-0.1.1/FRScraper.egg-info/PKG-INFO` & `frscraper-0.1.2/FRScraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FRScraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python module for Football Reference scraping and easy access to football data from various leagues
 Home-page: https://github.com/GabrielPastorello/FRScraper
 Author: Gabriel Speranza Pastorello
 Author-email: gabriel.pastorello01@gmail.com
 License: MIT
 Keywords: football reference,scraper,premier league,la liga,ligue 1,serie a,bundesliga,eredivisie,football data
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FRScraper Version: 0.1.1 Summary: Python module for
+Metadata-Version: 2.1 Name: FRScraper Version: 0.1.2 Summary: Python module for
 Football Reference scraping and easy access to football data from various
 leagues Home-page: https://github.com/GabrielPastorello/FRScraper Author:
 Gabriel Speranza Pastorello Author-email: gabriel.pastorello01@gmail.com
 License: MIT Keywords: football reference,scraper,premier league,la liga,ligue
 1,serie a,bundesliga,eredivisie,football data Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
```

### Comparing `frscraper-0.1.1/LICENSE` & `frscraper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frscraper-0.1.1/PKG-INFO` & `frscraper-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FRScraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python module for Football Reference scraping and easy access to football data from various leagues
 Home-page: https://github.com/GabrielPastorello/FRScraper
 Author: Gabriel Speranza Pastorello
 Author-email: gabriel.pastorello01@gmail.com
 License: MIT
 Keywords: football reference,scraper,premier league,la liga,ligue 1,serie a,bundesliga,eredivisie,football data
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FRScraper Version: 0.1.1 Summary: Python module for
+Metadata-Version: 2.1 Name: FRScraper Version: 0.1.2 Summary: Python module for
 Football Reference scraping and easy access to football data from various
 leagues Home-page: https://github.com/GabrielPastorello/FRScraper Author:
 Gabriel Speranza Pastorello Author-email: gabriel.pastorello01@gmail.com
 License: MIT Keywords: football reference,scraper,premier league,la liga,ligue
 1,serie a,bundesliga,eredivisie,football data Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
```

### Comparing `frscraper-0.1.1/README.md` & `frscraper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `frscraper-0.1.1/setup.py` & `frscraper-0.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
             name='FRScraper',
-            version='0.1.1',
+            version='0.1.2',
             description='Python module for Football Reference scraping and easy access to football data from various leagues',
             long_description=long_description,
             long_description_content_type="text/markdown",
             url='https://github.com/GabrielPastorello/FRScraper',
             author='Gabriel Speranza Pastorello',
             author_email='gabriel.pastorello01@gmail.com',
             license='MIT',
```

