# Comparing `tmp/ryry_cli-2.1.tar.gz` & `tmp/ryry_cli-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryry_cli-2.1.tar", last modified: Fri May 24 08:29:01 2024, max compression
+gzip compressed data, was "ryry_cli-2.2.tar", last modified: Fri May 24 08:53:58 2024, max compression
```

## Comparing `ryry_cli-2.1.tar` & `ryry_cli-2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 08:29:01.837873 ryry_cli-2.1/
--rw-rw-rw-   0        0        0     1077 2024-05-21 11:01:18.000000 ryry_cli-2.1/LICENSE
--rw-rw-rw-   0        0        0     2071 2024-05-24 08:29:01.837873 ryry_cli-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2024-05-21 10:59:20.000000 ryry_cli-2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 08:29:01.827576 ryry_cli-2.1/ryry/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-2.1/ryry/__init__.py
--rw-rw-rw-   0        0        0      150 2024-05-24 08:29:00.000000 ryry_cli-2.1/ryry/constant.py
--rw-rw-rw-   0        0        0    10331 2024-05-24 06:07:58.000000 ryry_cli-2.1/ryry/main.py
--rw-rw-rw-   0        0        0     5894 2024-05-23 11:14:35.000000 ryry_cli-2.1/ryry/ryry_server_socket.py
--rw-rw-rw-   0        0        0     9198 2024-05-24 06:22:51.000000 ryry_cli-2.1/ryry/ryry_service.py
--rw-rw-rw-   0        0        0     8312 2024-05-24 08:20:20.000000 ryry_cli-2.1/ryry/ryry_webapi.py
--rw-rw-rw-   0        0        0    14478 2024-05-24 08:28:58.000000 ryry_cli-2.1/ryry/ryry_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:29:01.829575 ryry_cli-2.1/ryry/script_template/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-2.1/ryry/script_template/__init__.py
--rw-rw-rw-   0        0        0      893 2024-03-11 07:11:36.000000 ryry_cli-2.1/ryry/script_template/main.py
--rw-rw-rw-   0        0        0      495 2024-03-11 07:12:45.000000 ryry_cli-2.1/ryry/script_template/run.py
--rw-rw-rw-   0        0        0     2377 2024-05-24 08:21:24.000000 ryry_cli-2.1/ryry/server_func.py
--rw-rw-rw-   0        0        0     4375 2024-05-20 06:06:46.000000 ryry_cli-2.1/ryry/store.py
--rw-rw-rw-   0        0        0     8723 2024-05-21 10:52:24.000000 ryry_cli-2.1/ryry/task.py
--rw-rw-rw-   0        0        0    10277 2024-05-21 09:54:41.000000 ryry_cli-2.1/ryry/taskUtils.py
--rw-rw-rw-   0        0        0     3934 2024-05-22 14:20:29.000000 ryry_cli-2.1/ryry/upload.py
--rw-rw-rw-   0        0        0    10877 2024-05-24 08:17:57.000000 ryry_cli-2.1/ryry/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:29:01.836874 ryry_cli-2.1/ryry_cli.egg-info/
--rw-rw-rw-   0        0        0     2071 2024-05-24 08:29:01.000000 ryry_cli-2.1/ryry_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-05-24 08:29:01.000000 ryry_cli-2.1/ryry_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 08:29:01.000000 ryry_cli-2.1/ryry_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-24 08:29:01.000000 ryry_cli-2.1/ryry_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      167 2024-05-24 08:29:01.000000 ryry_cli-2.1/ryry_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-24 08:29:01.000000 ryry_cli-2.1/ryry_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 08:29:01.839379 ryry_cli-2.1/setup.cfg
--rw-rw-rw-   0        0        0     2296 2024-05-24 08:28:58.000000 ryry_cli-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 08:53:58.709639 ryry_cli-2.2/
+-rw-rw-rw-   0        0        0     1077 2024-05-21 11:01:18.000000 ryry_cli-2.2/LICENSE
+-rw-rw-rw-   0        0        0     2071 2024-05-24 08:53:58.708640 ryry_cli-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2024-05-21 10:59:20.000000 ryry_cli-2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 08:53:58.699075 ryry_cli-2.2/ryry/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-2.2/ryry/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-05-24 08:53:57.000000 ryry_cli-2.2/ryry/constant.py
+-rw-rw-rw-   0        0        0    10331 2024-05-24 06:07:58.000000 ryry_cli-2.2/ryry/main.py
+-rw-rw-rw-   0        0        0     5894 2024-05-23 11:14:35.000000 ryry_cli-2.2/ryry/ryry_server_socket.py
+-rw-rw-rw-   0        0        0     9198 2024-05-24 06:22:51.000000 ryry_cli-2.2/ryry/ryry_service.py
+-rw-rw-rw-   0        0        0     8312 2024-05-24 08:20:20.000000 ryry_cli-2.2/ryry/ryry_webapi.py
+-rw-rw-rw-   0        0        0    15772 2024-05-24 08:53:50.000000 ryry_cli-2.2/ryry/ryry_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-24 08:53:58.702075 ryry_cli-2.2/ryry/script_template/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-2.2/ryry/script_template/__init__.py
+-rw-rw-rw-   0        0        0      893 2024-03-11 07:11:36.000000 ryry_cli-2.2/ryry/script_template/main.py
+-rw-rw-rw-   0        0        0      495 2024-03-11 07:12:45.000000 ryry_cli-2.2/ryry/script_template/run.py
+-rw-rw-rw-   0        0        0     2377 2024-05-24 08:21:24.000000 ryry_cli-2.2/ryry/server_func.py
+-rw-rw-rw-   0        0        0     4375 2024-05-20 06:06:46.000000 ryry_cli-2.2/ryry/store.py
+-rw-rw-rw-   0        0        0     8723 2024-05-21 10:52:24.000000 ryry_cli-2.2/ryry/task.py
+-rw-rw-rw-   0        0        0    10277 2024-05-21 09:54:41.000000 ryry_cli-2.2/ryry/taskUtils.py
+-rw-rw-rw-   0        0        0     3934 2024-05-22 14:20:29.000000 ryry_cli-2.2/ryry/upload.py
+-rw-rw-rw-   0        0        0    10994 2024-05-24 08:50:57.000000 ryry_cli-2.2/ryry/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 08:53:58.708640 ryry_cli-2.2/ryry_cli.egg-info/
+-rw-rw-rw-   0        0        0     2071 2024-05-24 08:53:58.000000 ryry_cli-2.2/ryry_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2024-05-24 08:53:58.000000 ryry_cli-2.2/ryry_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 08:53:58.000000 ryry_cli-2.2/ryry_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-24 08:53:58.000000 ryry_cli-2.2/ryry_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      167 2024-05-24 08:53:58.000000 ryry_cli-2.2/ryry_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-24 08:53:58.000000 ryry_cli-2.2/ryry_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 08:53:58.710640 ryry_cli-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2296 2024-05-24 08:53:54.000000 ryry_cli-2.2/setup.py
```

### Comparing `ryry_cli-2.1/LICENSE` & `ryry_cli-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.1/PKG-INFO` & `ryry_cli-2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 2.1
+Version: 2.2
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-2.1/README.md` & `ryry_cli-2.2/README.md`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.1/ryry/main.py` & `ryry_cli-2.2/ryry/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.1/ryry/ryry_server_socket.py` & `ryry_cli-2.2/ryry/ryry_server_socket.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.1/ryry/ryry_service.py` & `ryry_cli-2.2/ryry/ryry_service.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.1/ryry/ryry_webapi.py` & `ryry_cli-2.2/ryry/ryry_webapi.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.1/ryry/ryry_widget.py` & `ryry_cli-2.2/ryry/ryry_widget.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,37 +37,47 @@
             return -1
         elif v1[i] > v2[i]:
             return 1
     return 0
 
 def _remote_package_version(py_package):
     remote_version = ""
-    result = subprocess.run(f"pip index versions {py_package} -i https://pypi.python.org/simple/", 
-                            stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
-    ss = result.stdout.decode(encoding="utf8", errors="ignore").split("\n")
-    for s in ss:
-        if "LATEST:" in s.strip():
-            remote_version = s.replace("LATEST:", "").strip()
+    for pip in ["pip3","pip"]:
+        result = subprocess.run(f"pip index versions {py_package} -i https://pypi.python.org/simple/", 
+                                stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+        ss = result.stdout.decode(encoding="utf8", errors="ignore").split("\n")
+        for s in ss:
+            if "LATEST:" in s.strip():
+                remote_version = s.replace("LATEST:", "").strip()
+                break
+        else:
+            continue
+        break
     return remote_version
 
 #real time version get
 def _local_package_version(py_package):
     find_str = "grep"
     if platform.system() == 'Windows':
         find_str = "findstr"
     local_version = ""
-    result = subprocess.run(f"pip list | {find_str} {py_package}", 
-                            stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
-    ss = result.stdout.decode(encoding="utf8", errors="ignore").split("\n")
-    for s in ss:
-        s = re.sub(r'\s+', ' ', s)
-        sl = s.strip().split(" ")
-        if len(sl) == 2:
-            if py_package.strip() == sl[0].strip():
-                local_version = sl[1].strip()
+    for pip in ["pip3","pip"]:
+        result = subprocess.run(f"{pip} list | {find_str} {py_package}", 
+                                stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+        ss = result.stdout.decode(encoding="utf8", errors="ignore").split("\n")
+        for s in ss:
+            s = re.sub(r'\s+', ' ', s)
+            sl = s.strip().split(" ")
+            if len(sl) == 2:
+                if py_package.strip() == sl[0].strip():
+                    local_version = sl[1].strip()
+                    break
+        else:
+            continue
+        break
     return local_version
 
 def _pypi_folder_name(name):
     import re
     return re.sub(r"[/,\-\s]", "", name)
 
 def GetWidgetConfig(path):
@@ -308,17 +318,19 @@
 )
 ''')
     try:
         #build
         subprocess.run(f"python {setup_py} sdist bdist_wheel", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, cwd=pip_dir, encoding="utf-8")
         #uninstall
         subprocess.run(f"pip uninstall {name} -y", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, encoding="utf-8")
+        subprocess.run(f"pip3 uninstall {name} -y", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, encoding="utf-8")
         #install
         whl = utils.firstExitWithDir(os.path.join(pip_dir, "dist"), "whl")
         subprocess.run(f"pip install {whl} --extra-index-url https://pypi.python.org/simple/", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, encoding="utf-8")
+        subprocess.run(f"pip3 install {whl} --extra-index-url https://pypi.python.org/simple/", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, encoding="utf-8")
         #upload
         ryry_webapi.uploadWidget(widget_id, name, whl, ".whl", local_version)
         print(f"发布 {name}_{local_version} -> 成功")
     except Exception as ex:
         print(ex)
     finally:
         shutil.rmtree(pip_dir)
@@ -361,28 +373,34 @@
                 try:
                     py_package = data["py_package"]
                     widgetid, remote_version, package_url = ryry_webapi.findWidget(py_package)
                     local_version = _local_package_version(py_package)
                     if compare_versions(remote_version, local_version) > 0:
                         #update
                         subprocess.run(f"pip uninstall {py_package} -y", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+                        subprocess.run(f"pip3 uninstall {py_package} -y", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
                         subprocess.run(f"pip install {package_url} -i https://pypi.python.org/simple/ --extra-index-url https://pypi.python.org/simple/", 
                             stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+                        subprocess.run(f"pip3 install {package_url} -i https://pypi.python.org/simple/ --extra-index-url https://pypi.python.org/simple/", 
+                            stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
                         widgetUpdateNotify(py_package, local_version, remote_version)
                 except Exception as ex:
                     print(ex)
                     continue
                
 def installWidget(name):
     widgetid, remote_version, package_url = ryry_webapi.findWidget(name)
     if len(widgetid) <= 0:
         print(f"{name} 不存在")
         return
     local_version = _local_package_version(name)
     if compare_versions(remote_version, local_version) > 0:
         #update
         subprocess.run(f"pip uninstall {name} -y", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+        subprocess.run(f"pip3 uninstall {name} -y", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
         subprocess.run(f"pip install {package_url} -i https://pypi.python.org/simple/ --extra-index-url https://pypi.python.org/simple/", 
             stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+        subprocess.run(f"pip3 install {package_url} -i https://pypi.python.org/simple/ --extra-index-url https://pypi.python.org/simple/", 
+            stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
         widgetInstallNotify(name, remote_version)
         addWidgetToEnv(name)
```

### Comparing `ryry_cli-2.1/ryry/script_template/main.py` & `ryry_cli-2.2/ryry/script_template/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.1/ryry/server_func.py` & `ryry_cli-2.2/ryry/server_func.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.1/ryry/store.py` & `ryry_cli-2.2/ryry/store.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.1/ryry/task.py` & `ryry_cli-2.2/ryry/task.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.1/ryry/taskUtils.py` & `ryry_cli-2.2/ryry/taskUtils.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.1/ryry/upload.py` & `ryry_cli-2.2/ryry/upload.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.1/ryry/utils.py` & `ryry_cli-2.2/ryry/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,15 +282,17 @@
             run_subprocess(f"apt-get update")
             run_subprocess(f"apt-get install -y at libopencv-features2d-dev=4.5.4+dfsg-9ubuntu4 systemctl")
         run_subprocess(f"systemctl start atd")
         with open(time_task_file, 'w') as f:
             if update_cli:
                 f.write(f'''#!/bin/bash
 pip uninstall ryry-cli -y 
+pip3 uninstall ryry-cli -y 
 pip install -U ryry-cli -i {simple} --extra-index-url https://pypi.python.org/simple/
+pip3 install -U ryry-cli -i {simple} --extra-index-url https://pypi.python.org/simple/
 nohup {restart_command} &''')
             else:
                 f.write(f'''#!/bin/bash
 nohup {restart_command} &''')
         ot = os.path.join(thisFileDir, "update_ryry.out")
         result = subprocess.run(f"at now + 1 minutes -f {time_task_file} > {ot}", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
         print(f"{result.stdout}\n{result.stderr}")
```

### Comparing `ryry_cli-2.1/ryry_cli.egg-info/PKG-INFO` & `ryry_cli-2.2/ryry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 2.1
+Version: 2.2
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-2.1/ryry_cli.egg-info/SOURCES.txt` & `ryry_cli-2.2/ryry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryry_cli-2.1/setup.py` & `ryry_cli-2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 import subprocess
 import datetime
 
-ryry_version = "2.1"
+ryry_version = "2.2"
 ryry_build_number = int(ryry_version.replace(".",""))
 cur_dir = os.path.dirname(os.path.abspath(__file__))
 constanspy = os.path.join(cur_dir, "ryry", "constant.py")
 try:
     # result = subprocess.run("git config user.email", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
     build_user = "Noh"
     # if result.returncode == 0:
```

