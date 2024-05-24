# Comparing `tmp/eth_gtd_cli-0.0.68.tar.gz` & `tmp/eth_gtd_cli-0.0.69.tar.gz`

## Comparing `eth_gtd_cli-0.0.68.tar` & `eth_gtd_cli-0.0.69.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.68/deploy.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.68/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.68/src/ETH_GTD_cli/auth.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.68/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.68/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.68/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.68/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.68/LICENSE
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.68/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.68/pyproject.toml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.68/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.69/deploy.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.69/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.69/src/ETH_GTD_cli/auth.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.69/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.69/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0     8793 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.69/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.69/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.69/LICENSE
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.69/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.69/pyproject.toml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.69/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.68/src/ETH_GTD_cli/auth.py` & `eth_gtd_cli-0.0.69/src/ETH_GTD_cli/auth.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.68/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.69/src/ETH_GTD_cli/helper.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.68/src/ETH_GTD_cli/main.py` & `eth_gtd_cli-0.0.69/src/ETH_GTD_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,9 +241,15 @@
         response.raise_for_status()
         response = client.delete(f"{API_URL}/project/clear")
         response.raise_for_status()
         print("Data wiped.")
     else:
         print("Operation cancelled.")
 
+@app.command('claim')
+def claim():
+    response = client.post(f"{API_URL}/user/claimAdmin")
+    response.raise_for_status()
+    print("Admin claimed.")
+
 if __name__ == "__main__":
     app()
```

### Comparing `eth_gtd_cli-0.0.68/LICENSE` & `eth_gtd_cli-0.0.69/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.68/pyproject.toml` & `eth_gtd_cli-0.0.69/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.68"
+version = "0.0.69"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
 description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `eth_gtd_cli-0.0.68/PKG-INFO` & `eth_gtd_cli-0.0.69/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ETH_GTD_cli
-Version: 0.0.68
+Version: 0.0.69
 Summary: A CLI for the ETH project Grand Tour
 Project-URL: Homepage, https://github.com/leggedrobotics/GrandTourDatasets
 Project-URL: Issues, https://github.com/leggedrobotics/GrandTourDatasets/issues
 Author-email: Johann Schwabe <jschwab@ethz.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

