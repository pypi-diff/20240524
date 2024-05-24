# Comparing `tmp/pyredlight-0.2.0.tar.gz` & `tmp/pyredlight-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyredlight-0.2.0.tar", max compression
+gzip compressed data, was "pyredlight-0.3.0.tar", max compression
```

## Comparing `pyredlight-0.2.0.tar` & `pyredlight-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1506 2024-02-03 08:18:01.163838 pyredlight-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     6566 2024-02-03 08:18:01.163838 pyredlight-0.2.0/README.md
--rw-r--r--   0        0        0      842 2024-02-03 08:18:25.972018 pyredlight-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      134 2024-02-03 08:18:01.163838 pyredlight-0.2.0/pyredlight/__init__.py
--rw-r--r--   0        0        0      617 2024-02-03 08:18:01.163838 pyredlight-0.2.0/pyredlight/fastapi.py
--rw-r--r--   0        0        0     2959 2024-02-03 08:18:01.163838 pyredlight-0.2.0/pyredlight/limits.py
--rw-r--r--   0        0        0      364 2024-02-03 08:18:01.163838 pyredlight-0.2.0/pyredlight/redis.py
--rw-r--r--   0        0        0     7456 1970-01-01 00:00:00.000000 pyredlight-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1506 2024-05-24 13:22:39.301340 pyredlight-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     6566 2024-05-24 13:22:39.301340 pyredlight-0.3.0/README.md
+-rw-r--r--   0        0        0      842 2024-05-24 13:23:07.141586 pyredlight-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      134 2024-05-24 13:22:39.301340 pyredlight-0.3.0/pyredlight/__init__.py
+-rw-r--r--   0        0        0      912 2024-05-24 13:22:39.301340 pyredlight-0.3.0/pyredlight/fastapi.py
+-rw-r--r--   0        0        0     2959 2024-05-24 13:22:39.301340 pyredlight-0.3.0/pyredlight/limits.py
+-rw-r--r--   0        0        0      364 2024-05-24 13:22:39.301340 pyredlight-0.3.0/pyredlight/redis.py
+-rw-r--r--   0        0        0     7456 1970-01-01 00:00:00.000000 pyredlight-0.3.0/PKG-INFO
```

### Comparing `pyredlight-0.2.0/LICENSE.md` & `pyredlight-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyredlight-0.2.0/README.md` & `pyredlight-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyredlight-0.2.0/pyproject.toml` & `pyredlight-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyredlight"
-version = "0.2.0"
+version = "0.3.0"
 description = "Redis transaction based rate limiter"
 authors = ["Janne Enberg <janne.enberg@lietu.net>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/cocreators-ee/pyredlight/"
 repository = "https://github.com/cocreators-ee/pyredlight/"
 documentation = "https://github.com/cocreators-ee/pyredlight/"
```

### Comparing `pyredlight-0.2.0/pyredlight/limits.py` & `pyredlight-0.3.0/pyredlight/limits.py`

 * *Files identical despite different names*

### Comparing `pyredlight-0.2.0/PKG-INFO` & `pyredlight-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyredlight
-Version: 0.2.0
+Version: 0.3.0
 Summary: Redis transaction based rate limiter
 Home-page: https://github.com/cocreators-ee/pyredlight/
 License: BSD-3-Clause
 Keywords: rate,limit,limiter,limiting,async
 Author: Janne Enberg
 Author-email: janne.enberg@lietu.net
 Requires-Python: >=3.8,<4
```

