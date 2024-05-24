# Comparing `tmp/ryry_cli-2.0.tar.gz` & `tmp/ryry_cli-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryry_cli-2.0.tar", last modified: Fri May 24 08:20:41 2024, max compression
+gzip compressed data, was "ryry_cli-2.1.tar", last modified: Fri May 24 08:29:01 2024, max compression
```

## Comparing `ryry_cli-2.0.tar` & `ryry_cli-2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 08:20:41.001796 ryry_cli-2.0/
--rw-rw-rw-   0        0        0     1077 2024-05-21 11:01:18.000000 ryry_cli-2.0/LICENSE
--rw-rw-rw-   0        0        0     2071 2024-05-24 08:20:41.000795 ryry_cli-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2024-05-21 10:59:20.000000 ryry_cli-2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 08:20:40.992580 ryry_cli-2.0/ryry/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-2.0/ryry/__init__.py
--rw-rw-rw-   0        0        0      150 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry/constant.py
--rw-rw-rw-   0        0        0    10331 2024-05-24 06:07:58.000000 ryry_cli-2.0/ryry/main.py
--rw-rw-rw-   0        0        0     5894 2024-05-23 11:14:35.000000 ryry_cli-2.0/ryry/ryry_server_socket.py
--rw-rw-rw-   0        0        0     9198 2024-05-24 06:22:51.000000 ryry_cli-2.0/ryry/ryry_service.py
--rw-rw-rw-   0        0        0     8312 2024-05-24 08:20:20.000000 ryry_cli-2.0/ryry/ryry_webapi.py
--rw-rw-rw-   0        0        0    14441 2024-05-24 08:20:37.000000 ryry_cli-2.0/ryry/ryry_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:20:40.993584 ryry_cli-2.0/ryry/script_template/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-2.0/ryry/script_template/__init__.py
--rw-rw-rw-   0        0        0      893 2024-03-11 07:11:36.000000 ryry_cli-2.0/ryry/script_template/main.py
--rw-rw-rw-   0        0        0      495 2024-03-11 07:12:45.000000 ryry_cli-2.0/ryry/script_template/run.py
--rw-rw-rw-   0        0        0     2380 2024-05-24 06:17:59.000000 ryry_cli-2.0/ryry/server_func.py
--rw-rw-rw-   0        0        0     4375 2024-05-20 06:06:46.000000 ryry_cli-2.0/ryry/store.py
--rw-rw-rw-   0        0        0     8723 2024-05-21 10:52:24.000000 ryry_cli-2.0/ryry/task.py
--rw-rw-rw-   0        0        0    10277 2024-05-21 09:54:41.000000 ryry_cli-2.0/ryry/taskUtils.py
--rw-rw-rw-   0        0        0     3934 2024-05-22 14:20:29.000000 ryry_cli-2.0/ryry/upload.py
--rw-rw-rw-   0        0        0    10877 2024-05-24 08:17:57.000000 ryry_cli-2.0/ryry/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:20:40.999581 ryry_cli-2.0/ryry_cli.egg-info/
--rw-rw-rw-   0        0        0     2071 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      167 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 08:20:41.001796 ryry_cli-2.0/setup.cfg
--rw-rw-rw-   0        0        0     2296 2024-05-24 08:20:37.000000 ryry_cli-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 08:29:01.837873 ryry_cli-2.1/
+-rw-rw-rw-   0        0        0     1077 2024-05-21 11:01:18.000000 ryry_cli-2.1/LICENSE
+-rw-rw-rw-   0        0        0     2071 2024-05-24 08:29:01.837873 ryry_cli-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2024-05-21 10:59:20.000000 ryry_cli-2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 08:29:01.827576 ryry_cli-2.1/ryry/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-2.1/ryry/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-05-24 08:29:00.000000 ryry_cli-2.1/ryry/constant.py
+-rw-rw-rw-   0        0        0    10331 2024-05-24 06:07:58.000000 ryry_cli-2.1/ryry/main.py
+-rw-rw-rw-   0        0        0     5894 2024-05-23 11:14:35.000000 ryry_cli-2.1/ryry/ryry_server_socket.py
+-rw-rw-rw-   0        0        0     9198 2024-05-24 06:22:51.000000 ryry_cli-2.1/ryry/ryry_service.py
+-rw-rw-rw-   0        0        0     8312 2024-05-24 08:20:20.000000 ryry_cli-2.1/ryry/ryry_webapi.py
+-rw-rw-rw-   0        0        0    14478 2024-05-24 08:28:58.000000 ryry_cli-2.1/ryry/ryry_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-24 08:29:01.829575 ryry_cli-2.1/ryry/script_template/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-2.1/ryry/script_template/__init__.py
+-rw-rw-rw-   0        0        0      893 2024-03-11 07:11:36.000000 ryry_cli-2.1/ryry/script_template/main.py
+-rw-rw-rw-   0        0        0      495 2024-03-11 07:12:45.000000 ryry_cli-2.1/ryry/script_template/run.py
+-rw-rw-rw-   0        0        0     2377 2024-05-24 08:21:24.000000 ryry_cli-2.1/ryry/server_func.py
+-rw-rw-rw-   0        0        0     4375 2024-05-20 06:06:46.000000 ryry_cli-2.1/ryry/store.py
+-rw-rw-rw-   0        0        0     8723 2024-05-21 10:52:24.000000 ryry_cli-2.1/ryry/task.py
+-rw-rw-rw-   0        0        0    10277 2024-05-21 09:54:41.000000 ryry_cli-2.1/ryry/taskUtils.py
+-rw-rw-rw-   0        0        0     3934 2024-05-22 14:20:29.000000 ryry_cli-2.1/ryry/upload.py
+-rw-rw-rw-   0        0        0    10877 2024-05-24 08:17:57.000000 ryry_cli-2.1/ryry/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 08:29:01.836874 ryry_cli-2.1/ryry_cli.egg-info/
+-rw-rw-rw-   0        0        0     2071 2024-05-24 08:29:01.000000 ryry_cli-2.1/ryry_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2024-05-24 08:29:01.000000 ryry_cli-2.1/ryry_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 08:29:01.000000 ryry_cli-2.1/ryry_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-24 08:29:01.000000 ryry_cli-2.1/ryry_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      167 2024-05-24 08:29:01.000000 ryry_cli-2.1/ryry_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-24 08:29:01.000000 ryry_cli-2.1/ryry_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 08:29:01.839379 ryry_cli-2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2296 2024-05-24 08:28:58.000000 ryry_cli-2.1/setup.py
```

### Comparing `ryry_cli-2.0/LICENSE` & `ryry_cli-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.0/PKG-INFO` & `ryry_cli-2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 2.0
+Version: 2.1
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-2.0/README.md` & `ryry_cli-2.1/README.md`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.0/ryry/main.py` & `ryry_cli-2.1/ryry/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.0/ryry/ryry_server_socket.py` & `ryry_cli-2.1/ryry/ryry_server_socket.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.0/ryry/ryry_service.py` & `ryry_cli-2.1/ryry/ryry_service.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.0/ryry/ryry_webapi.py` & `ryry_cli-2.1/ryry/ryry_webapi.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.0/ryry/ryry_widget.py` & `ryry_cli-2.1/ryry/ryry_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         replaceIfNeed(dstDir, filename, ".png")
         replaceIfNeed(dstDir, filename, ".html")
 
 def setWidgetData(root, widgetid):
     data = GetWidgetConfig(root)
     data["widget_id"] = widgetid
     data["name"] = "Demo"
-    data["version"] = "2.0"
+    data["version"] = "2.1"
     data["device_keys"] = [
         utils.generate_unique_id()
     ]
     data["cmd"] = os.path.join(root, "main.py")
     with open(os.path.join(root, "config.json"), 'w') as f:
         json.dump(data, f)
 
@@ -155,15 +155,15 @@
 def addWidgetToEnv(root, mute=False):
     #maybe pip package
     try:
         package = pkg_resources.get_distribution(root)
         local_version = package.version
         name = package.project_name
         version = package.version
-        root = os.path.join(package.location, name)
+        root = os.path.join(package.location, name.replace("-", "_"))
     except:
         pass
 
     if CheckWidgetDataInPath(root) == False:
         return
     data = GetWidgetConfig(root)
     widget_id = data["widget_id"]
@@ -238,15 +238,15 @@
                         requirements += f"'{reals[:reals.index(';')]}',"  
                     elif "#" not in reals:
                         requirements += f"'{reals}',"
     pip_dir = os.path.join(os.path.dirname(package_folder), "tmp")
     if os.path.exists(pip_dir):
         shutil.rmtree(pip_dir)
     os.makedirs(pip_dir)
-    source_folder_name = name
+    source_folder_name = _pypi_folder_name(name)
     pip_source_dir = os.path.join(pip_dir, source_folder_name)
     shutil.copytree(package_folder, pip_source_dir)
     config_json_file = os.path.join(pip_source_dir, "config.json") 
     if os.path.exists(config_json_file):
         with open(config_json_file, 'r') as f:
             cc = json.load(f)
         cc["py_package"] = name
```

### Comparing `ryry_cli-2.0/ryry/script_template/main.py` & `ryry_cli-2.1/ryry/script_template/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.0/ryry/server_func.py` & `ryry_cli-2.1/ryry/server_func.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,23 +24,23 @@
         self.result = False, "Unknow"
         if self.widgetid == None:
             self.widgetid, _, _ = ryry_webapi.findWidget(self.func)
         if len(self.widgetid) > 0:
             checkUUID = ryry_webapi.createTask(self.widgetid, self.params)
             checking = True
             checkCount = 0
-            while checking or checkCount > 6000:
+            while checking or checkCount > 600:
                 finish, success, data = ryry_webapi.checkTask(checkUUID)
                 if finish:
                     checking = False
                     if success:
                         self.call_back(self.idx, data)
                         return
                 checkCount += 1
-                time.sleep(0.1)
+                time.sleep(1)
         else:
             print(f"widget {self.func}-{self.widgetid} not found")
         self.call_back(self.idx, None)
 
 class Task:
     thread_data = {}
```

### Comparing `ryry_cli-2.0/ryry/store.py` & `ryry_cli-2.1/ryry/store.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.0/ryry/task.py` & `ryry_cli-2.1/ryry/task.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.0/ryry/taskUtils.py` & `ryry_cli-2.1/ryry/taskUtils.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.0/ryry/upload.py` & `ryry_cli-2.1/ryry/upload.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.0/ryry/utils.py` & `ryry_cli-2.1/ryry/utils.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.0/ryry_cli.egg-info/PKG-INFO` & `ryry_cli-2.1/ryry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 2.0
+Version: 2.1
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-2.0/ryry_cli.egg-info/SOURCES.txt` & `ryry_cli-2.1/ryry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.0/setup.py` & `ryry_cli-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 import subprocess
 import datetime
 
-ryry_version = "2.0"
+ryry_version = "2.1"
 ryry_build_number = int(ryry_version.replace(".",""))
 cur_dir = os.path.dirname(os.path.abspath(__file__))
 constanspy = os.path.join(cur_dir, "ryry", "constant.py")
 try:
     # result = subprocess.run("git config user.email", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
     build_user = "Noh"
     # if result.returncode == 0:
@@ -20,15 +20,15 @@
 app_bulld_number={ryry_build_number}
 app_bulld_anchor="{build_user}_{build_pts}"
 app_name="ryry-cli"
 ''')
 except:
     with open(constanspy, 'w') as f:
         f.write(f'''#!!!!! do not change this file !!!!!
-app_version="2.0"
+app_version="2.1"
 app_bulld_number=1
 app_bulld_anchor=""
 app_name="ryry-cli"
 ''')
 
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
```

