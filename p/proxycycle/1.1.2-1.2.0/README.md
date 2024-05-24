# Comparing `tmp/proxycycle-1.1.2.tar.gz` & `tmp/proxycycle-1.2.0.tar.gz`

## Comparing `proxycycle-1.1.2.tar` & `proxycycle-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 proxycycle-1.1.2/.vscode/settings.json
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 proxycycle-1.1.2/src/proxycycle/Proxy.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 proxycycle-1.1.2/src/proxycycle/ProxySet.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 proxycycle-1.1.2/src/proxycycle/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 proxycycle-1.1.2/src/proxycycle/api/__init__.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 proxycycle-1.1.2/src/proxycycle/api/proxyscrape.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 proxycycle-1.1.2/src/proxycycle/enums/__init__.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 proxycycle-1.1.2/src/proxycycle/enums/anonymity_level.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 proxycycle-1.1.2/src/proxycycle/enums/scheme.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 proxycycle-1.1.2/tests/Proxy.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 proxycycle-1.1.2/tests/ProxySet.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 proxycycle-1.1.2/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 proxycycle-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 proxycycle-1.1.2/README.md
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 proxycycle-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 proxycycle-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 proxycycle-1.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 proxycycle-1.2.0/src/proxycycle/Proxy.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 proxycycle-1.2.0/src/proxycycle/ProxySet.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 proxycycle-1.2.0/src/proxycycle/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 proxycycle-1.2.0/src/proxycycle/api/__init__.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 proxycycle-1.2.0/src/proxycycle/api/proxyscrape.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 proxycycle-1.2.0/src/proxycycle/cli/fetch_proxy.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 proxycycle-1.2.0/src/proxycycle/enums/__init__.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 proxycycle-1.2.0/src/proxycycle/enums/anonymity_level.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 proxycycle-1.2.0/src/proxycycle/enums/scheme.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 proxycycle-1.2.0/tests/Proxy.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 proxycycle-1.2.0/tests/ProxySet.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 proxycycle-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 proxycycle-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 proxycycle-1.2.0/README.md
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 proxycycle-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 proxycycle-1.2.0/PKG-INFO
```

### Comparing `proxycycle-1.1.2/src/proxycycle/Proxy.py` & `proxycycle-1.2.0/src/proxycycle/Proxy.py`

 * *Files identical despite different names*

### Comparing `proxycycle-1.1.2/src/proxycycle/ProxySet.py` & `proxycycle-1.2.0/src/proxycycle/ProxySet.py`

 * *Files identical despite different names*

### Comparing `proxycycle-1.1.2/src/proxycycle/api/proxyscrape.py` & `proxycycle-1.2.0/src/proxycycle/api/proxyscrape.py`

 * *Files identical despite different names*

### Comparing `proxycycle-1.1.2/tests/Proxy.py` & `proxycycle-1.2.0/tests/Proxy.py`

 * *Files identical despite different names*

### Comparing `proxycycle-1.1.2/tests/ProxySet.py` & `proxycycle-1.2.0/tests/ProxySet.py`

 * *Files identical despite different names*

### Comparing `proxycycle-1.1.2/LICENSE.txt` & `proxycycle-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `proxycycle-1.1.2/README.md` & `proxycycle-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `proxycycle-1.1.2/pyproject.toml` & `proxycycle-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "proxycycle"
-version = "1.1.2"
+version = "1.2.0"
 description = "A Library to easily load/fetch proxy servers."
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Vbrawl", email = "greninjagr@gmail.com" },
@@ -68,7 +68,10 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[project.scripts]
+fetch-proxy = "proxycycle.cli.fetch_proxy:fetch_proxy"
```

### Comparing `proxycycle-1.1.2/PKG-INFO` & `proxycycle-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: proxycycle
-Version: 1.1.2
+Version: 1.2.0
 Summary: A Library to easily load/fetch proxy servers.
 Project-URL: Documentation, https://github.com/Vbrawl/proxycycle#readme
 Project-URL: Issues, https://github.com/Vbrawl/proxycycle/issues
 Project-URL: Source, https://github.com/Vbrawl/proxycycle
 Author-email: Vbrawl <greninjagr@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

