# Comparing `tmp/eth_gtd_cli-0.0.65.tar.gz` & `tmp/eth_gtd_cli-0.0.66.tar.gz`

## Comparing `eth_gtd_cli-0.0.65.tar` & `eth_gtd_cli-0.0.66.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.65/deploy.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.65/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.65/src/ETH_GTD_cli/auth.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.65/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.65/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.65/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.65/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.65/LICENSE
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.65/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.65/pyproject.toml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.65/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.66/deploy.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.66/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.66/src/ETH_GTD_cli/auth.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.66/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.66/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.66/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.66/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.66/LICENSE
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.66/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.66/pyproject.toml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.66/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.65/src/ETH_GTD_cli/auth.py` & `eth_gtd_cli-0.0.66/src/ETH_GTD_cli/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,18 @@
         new_access_token = response.cookies.get('authtoken')
         new_tokens = {'access_token': new_access_token, 'refresh_token': refresh_token}
         save_token(new_tokens)
         self.cookies.set('authtoken', new_access_token)
 
     def request(self, method, url, *args, **kwargs):
         response = super().request(method, url, *args, **kwargs)
+        if (url == f"{API_URL}/auth/refresh-token") and response.status_code == 401:
+            print("Refresh token expired. Please login again.")
+            response.status_code = 403
+            exit(1)
         if response.status_code == 401:
             print("Token expired, refreshing token...")
             self.refresh_token()
             response = super().request(method, url, *args, **kwargs)
         return response
```

### Comparing `eth_gtd_cli-0.0.65/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.66/src/ETH_GTD_cli/helper.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.65/src/ETH_GTD_cli/main.py` & `eth_gtd_cli-0.0.66/src/ETH_GTD_cli/main.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.65/LICENSE` & `eth_gtd_cli-0.0.66/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.65/pyproject.toml` & `eth_gtd_cli-0.0.66/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.65"
+version = "0.0.66"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
 description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `eth_gtd_cli-0.0.65/PKG-INFO` & `eth_gtd_cli-0.0.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ETH_GTD_cli
-Version: 0.0.65
+Version: 0.0.66
 Summary: A CLI for the ETH project Grand Tour
 Project-URL: Homepage, https://github.com/leggedrobotics/GrandTourDatasets
 Project-URL: Issues, https://github.com/leggedrobotics/GrandTourDatasets/issues
 Author-email: Johann Schwabe <jschwab@ethz.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

