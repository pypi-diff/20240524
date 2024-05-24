# Comparing `tmp/ryry_cli-1.8.tar.gz` & `tmp/ryry_cli-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryry_cli-1.8.tar", last modified: Thu May 23 11:14:59 2024, max compression
+gzip compressed data, was "ryry_cli-2.0.tar", last modified: Fri May 24 08:20:41 2024, max compression
```

## Comparing `ryry_cli-1.8.tar` & `ryry_cli-2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 11:14:59.007159 ryry_cli-1.8/
--rw-rw-rw-   0        0        0     1077 2024-05-21 11:01:18.000000 ryry_cli-1.8/LICENSE
--rw-rw-rw-   0        0        0     2071 2024-05-23 11:14:59.005845 ryry_cli-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2024-05-21 10:59:20.000000 ryry_cli-1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 11:14:58.995835 ryry_cli-1.8/ryry/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.8/ryry/__init__.py
--rw-rw-rw-   0        0        0      150 2024-05-23 11:14:58.000000 ryry_cli-1.8/ryry/constant.py
--rw-rw-rw-   0        0        0    10438 2024-05-21 11:07:52.000000 ryry_cli-1.8/ryry/main.py
--rw-rw-rw-   0        0        0     5894 2024-05-23 11:14:35.000000 ryry_cli-1.8/ryry/ryry_server_socket.py
--rw-rw-rw-   0        0        0     9198 2024-05-21 08:19:13.000000 ryry_cli-1.8/ryry/ryry_service.py
--rw-rw-rw-   0        0        0     8210 2024-05-23 11:11:51.000000 ryry_cli-1.8/ryry/ryry_webapi.py
--rw-rw-rw-   0        0        0    14641 2024-05-23 11:14:53.000000 ryry_cli-1.8/ryry/ryry_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:14:58.998845 ryry_cli-1.8/ryry/script_template/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.8/ryry/script_template/__init__.py
--rw-rw-rw-   0        0        0      893 2024-03-11 07:11:36.000000 ryry_cli-1.8/ryry/script_template/main.py
--rw-rw-rw-   0        0        0      495 2024-03-11 07:12:45.000000 ryry_cli-1.8/ryry/script_template/run.py
--rw-rw-rw-   0        0        0     2374 2024-05-23 10:53:41.000000 ryry_cli-1.8/ryry/server_func.py
--rw-rw-rw-   0        0        0     4375 2024-05-20 06:06:46.000000 ryry_cli-1.8/ryry/store.py
--rw-rw-rw-   0        0        0     8723 2024-05-21 10:52:24.000000 ryry_cli-1.8/ryry/task.py
--rw-rw-rw-   0        0        0    10277 2024-05-21 09:54:41.000000 ryry_cli-1.8/ryry/taskUtils.py
--rw-rw-rw-   0        0        0     3934 2024-05-22 14:20:29.000000 ryry_cli-1.8/ryry/upload.py
--rw-rw-rw-   0        0        0    13198 2024-05-21 08:18:59.000000 ryry_cli-1.8/ryry/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:14:59.004845 ryry_cli-1.8/ryry_cli.egg-info/
--rw-rw-rw-   0        0        0     2071 2024-05-23 11:14:58.000000 ryry_cli-1.8/ryry_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-05-23 11:14:58.000000 ryry_cli-1.8/ryry_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 11:14:58.000000 ryry_cli-1.8/ryry_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-23 11:14:58.000000 ryry_cli-1.8/ryry_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      167 2024-05-23 11:14:58.000000 ryry_cli-1.8/ryry_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-23 11:14:58.000000 ryry_cli-1.8/ryry_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 11:14:59.007159 ryry_cli-1.8/setup.cfg
--rw-rw-rw-   0        0        0     2296 2024-05-23 11:14:53.000000 ryry_cli-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 08:20:41.001796 ryry_cli-2.0/
+-rw-rw-rw-   0        0        0     1077 2024-05-21 11:01:18.000000 ryry_cli-2.0/LICENSE
+-rw-rw-rw-   0        0        0     2071 2024-05-24 08:20:41.000795 ryry_cli-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2024-05-21 10:59:20.000000 ryry_cli-2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 08:20:40.992580 ryry_cli-2.0/ryry/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-2.0/ryry/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry/constant.py
+-rw-rw-rw-   0        0        0    10331 2024-05-24 06:07:58.000000 ryry_cli-2.0/ryry/main.py
+-rw-rw-rw-   0        0        0     5894 2024-05-23 11:14:35.000000 ryry_cli-2.0/ryry/ryry_server_socket.py
+-rw-rw-rw-   0        0        0     9198 2024-05-24 06:22:51.000000 ryry_cli-2.0/ryry/ryry_service.py
+-rw-rw-rw-   0        0        0     8312 2024-05-24 08:20:20.000000 ryry_cli-2.0/ryry/ryry_webapi.py
+-rw-rw-rw-   0        0        0    14441 2024-05-24 08:20:37.000000 ryry_cli-2.0/ryry/ryry_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-24 08:20:40.993584 ryry_cli-2.0/ryry/script_template/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-2.0/ryry/script_template/__init__.py
+-rw-rw-rw-   0        0        0      893 2024-03-11 07:11:36.000000 ryry_cli-2.0/ryry/script_template/main.py
+-rw-rw-rw-   0        0        0      495 2024-03-11 07:12:45.000000 ryry_cli-2.0/ryry/script_template/run.py
+-rw-rw-rw-   0        0        0     2380 2024-05-24 06:17:59.000000 ryry_cli-2.0/ryry/server_func.py
+-rw-rw-rw-   0        0        0     4375 2024-05-20 06:06:46.000000 ryry_cli-2.0/ryry/store.py
+-rw-rw-rw-   0        0        0     8723 2024-05-21 10:52:24.000000 ryry_cli-2.0/ryry/task.py
+-rw-rw-rw-   0        0        0    10277 2024-05-21 09:54:41.000000 ryry_cli-2.0/ryry/taskUtils.py
+-rw-rw-rw-   0        0        0     3934 2024-05-22 14:20:29.000000 ryry_cli-2.0/ryry/upload.py
+-rw-rw-rw-   0        0        0    10877 2024-05-24 08:17:57.000000 ryry_cli-2.0/ryry/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 08:20:40.999581 ryry_cli-2.0/ryry_cli.egg-info/
+-rw-rw-rw-   0        0        0     2071 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      167 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-24 08:20:40.000000 ryry_cli-2.0/ryry_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 08:20:41.001796 ryry_cli-2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2296 2024-05-24 08:20:37.000000 ryry_cli-2.0/setup.py
```

### Comparing `ryry_cli-1.8/LICENSE` & `ryry_cli-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.8/PKG-INFO` & `ryry_cli-2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 1.8
+Version: 2.0
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-1.8/README.md` & `ryry_cli-2.0/README.md`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.8/ryry/main.py` & `ryry_cli-2.0/ryry/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,33 +267,30 @@
         ryry_widget.addWidgetToEnv(work_path)
     elif command == 'remove':
         ryry_widget.remove(work_path)
     elif command == 'enable':
         ryry_widget.enable(work_path)
     elif command == 'disable':
         ryry_widget.disable(work_path)
-    elif command == 'pending_task':
-        ryry_widget.getTaskCount(work_path)
+    elif command == 'install':
+        ryry_widget.installWidget(work_path)
     else:
         print("Unknown command:", command)
 
 def main():
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
     if len(sys.argv) >= 2:
         module = sys.argv[1]
         if module == "widget":
             widget()
         elif module == "service":
             service()
         elif module == "status":
             status()
-        elif module == "report":
-            utils.reportLog()
-            print(f"report success")
         else:
             print(f"Unknown command:{module}")
             sys.exit(0)
     else:
         status()
 
 if __name__ == '__main__':
```

### Comparing `ryry_cli-1.8/ryry/ryry_server_socket.py` & `ryry_cli-2.0/ryry/ryry_server_socket.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.8/ryry/ryry_service.py` & `ryry_cli-2.0/ryry/ryry_service.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.8/ryry/ryry_webapi.py` & `ryry_cli-2.0/ryry/ryry_webapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,21 +225,23 @@
 
 def findWidget(name):
     req = {
         "name": name
     }
     r1, r2, r3 = _aigc_post("aigc/task/findWidget", req)
     if r1 != 0:
-        return 0
+        return "", "", ""
     for it in r3:
         widget_id = it["widget_id"]
         widget_name = it["name"]
+        version = it["version"]
+        package = it["package"]
         if widget_name.strip().lower() == name.strip().lower():
-            return widget_id
-    return 0
+            return widget_id, version, package
+    return "", "", ""
 
 def checkTask(checkUUID):
     req = {
         "task_uuid": checkUUID
     }
     r1, r2, r3 = _aigc_post("aigc/task/checkTask", req)
     if r1 != 0:
```

### Comparing `ryry_cli-1.8/ryry/ryry_widget.py` & `ryry_cli-2.0/ryry/ryry_widget.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,28 +81,14 @@
     for filename in os.listdir(path):
         pathname = os.path.join(path, filename) 
         if (os.path.isfile(pathname)) and filename in ["config.json", "config.json.py"]:
             with open(pathname, 'r', encoding='UTF-8') as f:
                 return json.load(f)
     return {}
 
-def folderIsH5(path):
-    configFileExist = False
-    iconFileExist = False
-    htmlFileExist = False
-    for filename in os.listdir(path):
-        pathname = os.path.join(path, filename) 
-        if (os.path.isfile(pathname)) and filename == "config.json":
-            configFileExist = True
-        if (os.path.isfile(pathname)) and filename == "icon.png":
-            iconFileExist = True
-        if (os.path.isfile(pathname)) and filename == "index.html":
-            htmlFileExist = True
-    return configFileExist and iconFileExist and htmlFileExist
-
 def PathIsEmpty(path):
     return len(os.listdir(path)) == 0
 
 def replaceIfNeed(dstDir, name, subfix):
     newsubfix = subfix + ".py"
     if name.find(newsubfix) != -1:
         os.rename(os.path.join(dstDir, name), os.path.join(dstDir, name.replace(newsubfix, subfix)))
@@ -125,15 +111,15 @@
         replaceIfNeed(dstDir, filename, ".png")
         replaceIfNeed(dstDir, filename, ".html")
 
 def setWidgetData(root, widgetid):
     data = GetWidgetConfig(root)
     data["widget_id"] = widgetid
     data["name"] = "Demo"
-    data["version"] = "1.8"
+    data["version"] = "2.0"
     data["device_keys"] = [
         utils.generate_unique_id()
     ]
     data["cmd"] = os.path.join(root, "main.py")
     with open(os.path.join(root, "config.json"), 'w') as f:
         json.dump(data, f)
 
@@ -169,15 +155,15 @@
 def addWidgetToEnv(root, mute=False):
     #maybe pip package
     try:
         package = pkg_resources.get_distribution(root)
         local_version = package.version
         name = package.project_name
         version = package.version
-        root = os.path.join(package.location, _pypi_folder_name(name))
+        root = os.path.join(package.location, name)
     except:
         pass
 
     if CheckWidgetDataInPath(root) == False:
         return
     data = GetWidgetConfig(root)
     widget_id = data["widget_id"]
@@ -218,45 +204,24 @@
         data = GetWidgetConfig(args)
         if "widget_id" not in data:
             print(f"path {args} is not widget folder!")
             return
         widget_id = data["widget_id"]
     store.disableWidget(widget_id)
     print(f"widget:{widget_id} updated")
-        
-def getTaskCount(args):
-    widget_id = args
-    if os.path.exists(args):
-        #find widgetid in args path
-        data = GetWidgetConfig(args)
-        if "widget_id" not in data:
-            print(f"path {args} is not widget folder!")
-            return
-        widget_id = data["widget_id"]
-    datas = ryry_webapi.GetTaskCount(widget_id)
-    for it in datas:
-        if it["widgetUUID"] == widget_id:
-            return it["taskCount"]
-    return -1
 
 def publishWidget(package_folder):
     if CheckWidgetDataInPath(package_folder) == False:
         return
         
     data = GetWidgetConfig(package_folder)
     widget_id = data["widget_id"]
     name = data["name"]
     local_version = data["version"]
     user_id = utils.generate_unique_id()
-
-    #override setting
-    remote_version = _remote_package_version(name)
-    if compare_versions(remote_version, local_version) >= 0:
-        print(f"version {local_version} must be larger than {remote_version}, publish abandon")
-        return
         
     #if in h5&script parent folder, add env path
     if len(package_folder) > 0:
         addWidgetToEnv(package_folder, True)
         
     #package python to private pip server
     requirements_txts = [
@@ -273,15 +238,15 @@
                         requirements += f"'{reals[:reals.index(';')]}',"  
                     elif "#" not in reals:
                         requirements += f"'{reals}',"
     pip_dir = os.path.join(os.path.dirname(package_folder), "tmp")
     if os.path.exists(pip_dir):
         shutil.rmtree(pip_dir)
     os.makedirs(pip_dir)
-    source_folder_name = _pypi_folder_name(name)
+    source_folder_name = name
     pip_source_dir = os.path.join(pip_dir, source_folder_name)
     shutil.copytree(package_folder, pip_source_dir)
     config_json_file = os.path.join(pip_source_dir, "config.json") 
     if os.path.exists(config_json_file):
         with open(config_json_file, 'r') as f:
             cc = json.load(f)
         cc["py_package"] = name
@@ -364,14 +329,25 @@
     ver = get_distribution("ryry-cli").version
     taskUtils.notifyWechatRobot({
         "msgtype": "text",
         "text": {
             "content": f"机器<{machine_name}[{device_id}]>[{ver}] widget:[{widgetName}]升级版本[{oldver}]->[{newver}]"
         }
     })
+    
+def widgetInstallNotify(widgetName, newver):
+    device_id = utils.generate_unique_id()
+    machine_name = socket.gethostname()
+    ver = get_distribution("ryry-cli").version
+    taskUtils.notifyWechatRobot({
+        "msgtype": "text",
+        "text": {
+            "content": f"机器<{machine_name}[{device_id}]>[{ver}] 安装widget:[{widgetName}][{newver}]"
+        }
+    })
 
 def UpdateWidgetFromPypi():
     map = store.widgetMap()
     for it in map:
         is_block = False
         if isinstance(map[it], (dict)):
             is_block = map[it]["isBlock"]
@@ -380,19 +356,33 @@
             path = map[it]
         path = os.path.dirname(path)
         if is_block == False and os.path.exists(path):
             data = GetWidgetConfig(path)
             if "py_package" in data and len(data["py_package"]) > 0:
                 try:
                     py_package = data["py_package"]
-                    remote_version = _remote_package_version(py_package)
+                    widgetid, remote_version, package_url = ryry_webapi.findWidget(py_package)
                     local_version = _local_package_version(py_package)
                     if compare_versions(remote_version, local_version) > 0:
                         #update
-                        subprocess.run(f"pip uninstall {py_package}", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
-                        subprocess.run(f"pip install -U {py_package} -i https://pypi.python.org/simple/ --extra-index-url https://pypi.python.org/simple/", 
+                        subprocess.run(f"pip uninstall {py_package} -y", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+                        subprocess.run(f"pip install {package_url} -i https://pypi.python.org/simple/ --extra-index-url https://pypi.python.org/simple/", 
                             stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
                         widgetUpdateNotify(py_package, local_version, remote_version)
                 except Exception as ex:
                     print(ex)
                     continue
-               
+               
+def installWidget(name):
+    widgetid, remote_version, package_url = ryry_webapi.findWidget(name)
+    if len(widgetid) <= 0:
+        print(f"{name} 不存在")
+        return
+    local_version = _local_package_version(name)
+    if compare_versions(remote_version, local_version) > 0:
+        #update
+        subprocess.run(f"pip uninstall {name} -y", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+        subprocess.run(f"pip install {package_url} -i https://pypi.python.org/simple/ --extra-index-url https://pypi.python.org/simple/", 
+            stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+        widgetInstallNotify(name, remote_version)
+        addWidgetToEnv(name)
+
```

### Comparing `ryry_cli-1.8/ryry/script_template/main.py` & `ryry_cli-2.0/ryry/script_template/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.8/ryry/server_func.py` & `ryry_cli-2.0/ryry/server_func.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         if self.call_back == None:
             raise Exception("need callback function")
         self.start()
     def run(self):
         self.checking = False
         self.result = False, "Unknow"
         if self.widgetid == None:
-            self.widgetid = ryry_webapi.findWidget(self.func)
+            self.widgetid, _, _ = ryry_webapi.findWidget(self.func)
         if len(self.widgetid) > 0:
             checkUUID = ryry_webapi.createTask(self.widgetid, self.params)
             checking = True
             checkCount = 0
             while checking or checkCount > 6000:
                 finish, success, data = ryry_webapi.checkTask(checkUUID)
                 if finish:
```

### Comparing `ryry_cli-1.8/ryry/store.py` & `ryry_cli-2.0/ryry/store.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.8/ryry/task.py` & `ryry_cli-2.0/ryry/task.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.8/ryry/taskUtils.py` & `ryry_cli-2.0/ryry/taskUtils.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.8/ryry/upload.py` & `ryry_cli-2.0/ryry/upload.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.8/ryry/utils.py` & `ryry_cli-2.0/ryry/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -164,74 +164,14 @@
             
         pynvml.nvmlShutdown()
     except Exception as e:
         data["gpu"]["count"] = 1
         data["gpu"]["list"].append(f"GPU0: Normal")
     return data
 
-def reportLog():
-    reason = ""
-    if len(sys.argv) >= 2:
-        reason = sys.argv[2].strip().replace("\n","").replace(",","").replace(" ","").replace(";","")
-    d = datetime.now().strftime('%Y_%m_%d_%H_%M_%S')
-    uid = generate_unique_id()
-
-    thisFileDir = os.path.dirname(os.path.abspath(__file__))
-    dist = os.path.join(thisFileDir, f"{uid}_{reason}_{d}.zip")
-    zip = zipfile.ZipFile(dist, "w", zipfile.ZIP_DEFLATED) 
-
-    for root,dirs,files in os.walk(thisFileDir):
-        for file in files:
-            if str(file).startswith("~$"):
-                continue
-            ext = file[file.rindex("."):]
-            if ext == ".log" or ext == ".json" or ".log." in file:
-                filepath = os.path.join(root, file)
-                zip.write(filepath, file)
-        if root != files:
-            break
-    zip.close()
-    ossurl = uploadOSS(dist)
-    os.remove(dist)
-    return ossurl
-
-def uploadOSS(file):
-    conn = http.client.HTTPSConnection("api.ryryai.com")
-    payload = json.dumps({
-        "sign": "f0463f490eb84133c0aab3a8576ed2fc"
-    })
-    headers = {
-        'Content-Type': 'application/json'
-    }
-    conn.request("POST", "/proxymsg/get_oss_config", payload, headers)
-    res = conn.getresponse()
-    data = json.loads(res.read().decode("utf-8"))
-    if data["code"] == 0:
-        AccessKeyId = data["data"]["AccessKeyId"]
-        AccessKeySecret = data["data"]["AccessKeySecret"]
-        SecurityToken = data["data"]["SecurityToken"]
-        BucketName = data["data"]["BucketName"]
-        Expiration = data["data"]["Expiration"]
-        Endpoint = data["data"]["Endpoint"]
-        CallbackUrl = data["data"]["CallbackUrl"]
-        cdn = data["data"]["cdn"]
-        
-        if len(AccessKeyId) > 0:  
-            import oss2
-            auth = oss2.StsAuth(AccessKeyId, AccessKeySecret, SecurityToken)
-            bucket = oss2.Bucket(auth, Endpoint, BucketName, connect_timeout=600)
-            with open(file, "rb") as f:
-                byte_data = f.read()
-            file_name = Path(file).name
-            publish_name = f"ryry/report/{file_name}" 
-            bucket.put_object(publish_name, byte_data)
-            return f"{cdn}{publish_name}" 
-    else:
-        print(f"get_oss_config fail: response={data}")
-
 def process_is_alive(pid: int) -> bool:
     try:
         process = psutil.Process(pid)
         pstatus = process.status()
         if pstatus == psutil.STATUS_RUNNING or pstatus == psutil.STATUS_SLEEPING:
             return True
         else:
```

### Comparing `ryry_cli-1.8/ryry_cli.egg-info/PKG-INFO` & `ryry_cli-2.0/ryry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 1.8
+Version: 2.0
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-1.8/ryry_cli.egg-info/SOURCES.txt` & `ryry_cli-2.0/ryry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.8/setup.py` & `ryry_cli-2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 import subprocess
 import datetime
 
-ryry_version = "1.8"
+ryry_version = "2.0"
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
-app_version="1.8"
+app_version="2.0"
 app_bulld_number=1
 app_bulld_anchor=""
 app_name="ryry-cli"
 ''')
 
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
```

