# Comparing `tmp/Jvav-1.9.1.tar.gz` & `tmp/Jvav-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-t87o_kqr/Jvav-1.9.1.tar", last modified: Fri Apr 26 15:54:33 2024, max compression
+gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-qc07b9l0/Jvav-1.9.2.tar", last modified: Fri May 24 08:30:18 2024, max compression
```

## Comparing `Jvav-1.9.1.tar` & `Jvav-1.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-26 15:54:33.000000 Jvav-1.9.1/
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/
--rw-r--r--   0 zh         (501) staff       (20)     4311 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)      295 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/SOURCES.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/dependency_links.txt
--rw-r--r--   0 zh         (501) staff       (20)       39 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/entry_points.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-1.9.1/Jvav.egg-info/not-zip-safe
--rw-r--r--   0 zh         (501) staff       (20)      495 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/requires.txt
--rw-r--r--   0 zh         (501) staff       (20)       11 2024-04-26 15:54:33.000000 Jvav-1.9.1/Jvav.egg-info/top_level.txt
--rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-1.9.1/LICENSE
--rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-1.9.1/MANIFEST.in
--rw-r--r--   0 zh         (501) staff       (20)     4311 2024-04-26 15:54:33.000000 Jvav-1.9.1/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)     3581 2024-04-21 15:00:39.000000 Jvav-1.9.1/README.md
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-04-26 15:54:33.000000 Jvav-1.9.1/jvav/
--rw-r--r--   0 zh         (501) staff       (20)      481 2024-04-26 15:54:07.000000 Jvav-1.9.1/jvav/__init__.py
--rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-1.9.1/jvav/cmd.py
--rw-r--r--   0 zh         (501) staff       (20)    74171 2024-04-26 15:52:16.000000 Jvav-1.9.1/jvav/utils.py
--rw-r--r--   0 zh         (501) staff       (20)      495 2024-04-22 03:22:14.000000 Jvav-1.9.1/requirements.txt
--rw-r--r--   0 zh         (501) staff       (20)       38 2024-04-26 15:54:33.000000 Jvav-1.9.1/setup.cfg
--rw-r--r--   0 zh         (501) staff       (20)     1345 2024-04-26 15:54:04.000000 Jvav-1.9.1/setup.py
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-05-24 08:30:18.000000 Jvav-1.9.2/
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/
+-rw-r--r--   0 zh         (501) staff       (20)     4311 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)      295 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/SOURCES.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/dependency_links.txt
+-rw-r--r--   0 zh         (501) staff       (20)       39 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/entry_points.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-1.9.2/Jvav.egg-info/not-zip-safe
+-rw-r--r--   0 zh         (501) staff       (20)      495 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/requires.txt
+-rw-r--r--   0 zh         (501) staff       (20)       11 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/top_level.txt
+-rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-1.9.2/LICENSE
+-rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-1.9.2/MANIFEST.in
+-rw-r--r--   0 zh         (501) staff       (20)     4311 2024-05-24 08:30:18.000000 Jvav-1.9.2/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)     3581 2024-04-21 15:00:39.000000 Jvav-1.9.2/README.md
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-05-24 08:30:18.000000 Jvav-1.9.2/jvav/
+-rw-r--r--   0 zh         (501) staff       (20)      481 2024-05-24 08:29:24.000000 Jvav-1.9.2/jvav/__init__.py
+-rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-1.9.2/jvav/cmd.py
+-rw-r--r--   0 zh         (501) staff       (20)    74172 2024-05-24 08:28:05.000000 Jvav-1.9.2/jvav/utils.py
+-rw-r--r--   0 zh         (501) staff       (20)      495 2024-04-22 03:22:14.000000 Jvav-1.9.2/requirements.txt
+-rw-r--r--   0 zh         (501) staff       (20)       38 2024-05-24 08:30:18.000000 Jvav-1.9.2/setup.cfg
+-rw-r--r--   0 zh         (501) staff       (20)     1345 2024-05-24 08:29:19.000000 Jvav-1.9.2/setup.py
```

### Comparing `Jvav-1.9.1/Jvav.egg-info/PKG-INFO` & `Jvav-1.9.2/Jvav.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.9.1
+Version: 1.9.2
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.9.1 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 1.9.2 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `Jvav-1.9.1/LICENSE` & `Jvav-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.1/PKG-INFO` & `Jvav-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.9.1
+Version: 1.9.2
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.9.1 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 1.9.2 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `Jvav-1.9.1/README.md` & `Jvav-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.1/jvav/cmd.py` & `Jvav-1.9.2/jvav/cmd.py`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.1/jvav/utils.py` & `Jvav-1.9.2/jvav/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         :return tuple[int, requests.Response] 状态码和请求返回值
         关于状态码:
         200: 成功
         404: 未找到
         502: 网络问题
         """
         if self.use_cache:
-            with requests_cache.CachedSession(cache_name="jvav_cache") as session:
+            with requests_cache.CachedSession(cache_name=".jvav_cache") as session:
                 return self._inner_send_req(url, session, headers, proxies, m, **args)
         else:
             with requests.Session() as session:
                 return self._inner_send_req(url, session, headers, proxies, m, **args)
 
     @staticmethod
     def get_soup(resp: requests.Response) -> BeautifulSoup:
```

### Comparing `Jvav-1.9.1/setup.py` & `Jvav-1.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requires = [i.strip() for i in r]
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="Jvav",
-    version="1.9.1",
+    version="1.9.2",
     description="Useful tools for Jav.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/akynazh/jvav",
     download_url="https://github.com/akynazh/jvav/releases/latest",
     author="akynazh",
     author_email="akynazh@gmail.com",
```

