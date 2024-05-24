# Comparing `tmp/eth_gtd_cli-0.0.72.tar.gz` & `tmp/eth_gtd_cli-0.0.73.tar.gz`

## Comparing `eth_gtd_cli-0.0.72.tar` & `eth_gtd_cli-0.0.73.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.72/deploy.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.72/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.72/src/ETH_GTD_cli/auth.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.72/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.72/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0     9137 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.72/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.72/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.72/LICENSE
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.72/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.72/pyproject.toml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.72/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.73/deploy.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.73/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.73/src/ETH_GTD_cli/auth.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.73/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.73/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.73/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.73/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.73/LICENSE
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.73/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.73/pyproject.toml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.73/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.72/src/ETH_GTD_cli/auth.py` & `eth_gtd_cli-0.0.73/src/ETH_GTD_cli/auth.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.72/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.73/src/ETH_GTD_cli/helper.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.72/src/ETH_GTD_cli/main.py` & `eth_gtd_cli-0.0.73/src/ETH_GTD_cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,14 +255,14 @@
 
 
 @user.command('list')
 def users():
     response = client.get(f"{API_URL}/user/all")
     response.raise_for_status()
     data = response.json()
-    table = Table("Name", "Email", "Role")
+    table = Table("Name", "Email", "Role", "googleId")
     for user in data:
-        table.add_row(user["name"], user["email"], user["role"])
+        table.add_row(user["name"], user["email"], user["role"], user["googleId"])
     print(table)
 
 if __name__ == "__main__":
     app()
```

### Comparing `eth_gtd_cli-0.0.72/LICENSE` & `eth_gtd_cli-0.0.73/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.72/pyproject.toml` & `eth_gtd_cli-0.0.73/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.72"
+version = "0.0.73"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
 description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `eth_gtd_cli-0.0.72/PKG-INFO` & `eth_gtd_cli-0.0.73/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ETH_GTD_cli
-Version: 0.0.72
+Version: 0.0.73
 Summary: A CLI for the ETH project Grand Tour
 Project-URL: Homepage, https://github.com/leggedrobotics/GrandTourDatasets
 Project-URL: Issues, https://github.com/leggedrobotics/GrandTourDatasets/issues
 Author-email: Johann Schwabe <jschwab@ethz.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

