# Comparing `tmp/cv_smart_house_camera-0.1.5.tar.gz` & `tmp/cv_smart_house_camera-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cv_smart_house_camera-0.1.5.tar", max compression
+gzip compressed data, was "cv_smart_house_camera-0.1.6.tar", max compression
```

## Comparing `cv_smart_house_camera-0.1.5.tar` & `cv_smart_house_camera-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     4243 2024-05-21 19:08:04.266273 cv_smart_house_camera-0.1.5/cv_smart_house_camera/__init__.py
--rw-r--r--   0        0        0      733 2024-05-20 13:14:13.260707 cv_smart_house_camera-0.1.5/cv_smart_house_camera/cam_capture.py
--rw-r--r--   0        0        0       48 2024-05-20 12:13:33.324485 cv_smart_house_camera-0.1.5/cv_smart_house_camera/constants.py
--rw-r--r--   0        0        0       85 2024-05-18 16:24:24.102931 cv_smart_house_camera-0.1.5/cv_smart_house_camera/data/frames.py
--rw-r--r--   0        0        0     1113 2024-05-21 19:07:52.163784 cv_smart_house_camera-0.1.5/cv_smart_house_camera/generate_code.py
--rw-r--r--   0        0        0      292 2024-05-20 12:05:00.597313 cv_smart_house_camera-0.1.5/cv_smart_house_camera/helpers/poetry_install.py
--rw-r--r--   0        0        0      183 2024-05-20 18:00:07.621973 cv_smart_house_camera-0.1.5/cv_smart_house_camera/modules/modules_list.py
--rw-r--r--   0        0        0     1771 2024-05-20 17:54:20.117074 cv_smart_house_camera-0.1.5/cv_smart_house_camera/modules/modules_processing.py
--rw-r--r--   0        0        0     3543 2024-05-21 18:56:28.902217 cv_smart_house_camera-0.1.5/cv_smart_house_camera/proto_services/camera_service_pb2.py
--rw-r--r--   0        0        0     5512 2024-05-21 18:56:28.902217 cv_smart_house_camera-0.1.5/cv_smart_house_camera/proto_services/camera_service_twirp.py
--rw-r--r--   0        0        0      141 2024-05-19 14:26:26.476002 cv_smart_house_camera-0.1.5/cv_smart_house_camera/utils/get_local_ip.py
--rw-r--r--   0        0        0      515 2024-05-20 12:20:23.424894 cv_smart_house_camera-0.1.5/cv_smart_house_camera/utils/get_modules_from_toml.py
--rw-r--r--   0        0        0      683 2024-05-21 19:07:36.442842 cv_smart_house_camera-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 13:48:56.985064 cv_smart_house_camera-0.1.5/README.md
--rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 cv_smart_house_camera-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      244 2024-05-24 09:03:04.476722 cv_smart_house_camera-0.1.6/cv_smart_house_camera/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-20 13:14:13.260707 cv_smart_house_camera-0.1.6/cv_smart_house_camera/cam_capture.py
+-rw-r--r--   0        0        0       91 2024-05-24 08:38:56.068779 cv_smart_house_camera-0.1.6/cv_smart_house_camera/constants.py
+-rw-r--r--   0        0        0       85 2024-05-18 16:24:24.102931 cv_smart_house_camera-0.1.6/cv_smart_house_camera/data/frames.py
+-rw-r--r--   0        0        0      976 2024-05-24 09:01:56.589663 cv_smart_house_camera-0.1.6/cv_smart_house_camera/generate_code.py
+-rw-r--r--   0        0        0      347 2024-05-24 09:19:21.154139 cv_smart_house_camera-0.1.6/cv_smart_house_camera/helpers/poetry_install.py
+-rw-r--r--   0        0        0      271 2024-05-24 09:08:20.156939 cv_smart_house_camera-0.1.6/cv_smart_house_camera/main.py
+-rw-r--r--   0        0        0      778 2024-05-24 08:39:21.579651 cv_smart_house_camera-0.1.6/cv_smart_house_camera/modules/modules_list.py
+-rw-r--r--   0        0        0     1771 2024-05-20 17:54:20.117074 cv_smart_house_camera-0.1.6/cv_smart_house_camera/modules/modules_processing.py
+-rw-r--r--   0        0        0     3543 2024-05-24 08:47:27.279619 cv_smart_house_camera-0.1.6/cv_smart_house_camera/proto_services/camera_service_pb2.py
+-rw-r--r--   0        0        0     5512 2024-05-24 08:47:27.279619 cv_smart_house_camera-0.1.6/cv_smart_house_camera/proto_services/camera_service_twirp.py
+-rw-r--r--   0        0        0     4697 2024-05-24 09:22:47.376868 cv_smart_house_camera-0.1.6/cv_smart_house_camera/server.py
+-rw-r--r--   0        0        0      141 2024-05-19 14:26:26.476002 cv_smart_house_camera-0.1.6/cv_smart_house_camera/utils/get_local_ip.py
+-rw-r--r--   0        0        0      515 2024-05-20 12:20:23.424894 cv_smart_house_camera-0.1.6/cv_smart_house_camera/utils/get_modules_from_toml.py
+-rw-r--r--   0        0        0      660 2024-05-24 09:24:09.524311 cv_smart_house_camera-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 13:48:56.985064 cv_smart_house_camera-0.1.6/README.md
+-rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 cv_smart_house_camera-0.1.6/PKG-INFO
```

### Comparing `cv_smart_house_camera-0.1.5/cv_smart_house_camera/__init__.py` & `cv_smart_house_camera-0.1.6/cv_smart_house_camera/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,85 @@
 import logging
 import toml
 import uvicorn
 from threading import Thread
 from cv_smart_house_camera.cam_capture import cam_capture
 from twirp.asgi import TwirpASGIApp
-from  cv_smart_house_camera.proto_services.camera_service_twirp import CameraServiceServer
 import  cv_smart_house_camera.proto_services.camera_service_pb2 as camera_service
+from cv_smart_house_camera.proto_services.camera_service_twirp import CameraServiceServer 
 from cv_smart_house_camera.data.frames import modules_result
 from cv_smart_house_camera.modules.modules_list import modules as modules_list
 from starlette.middleware.cors import CORSMiddleware
 
 from cv_smart_house_camera.helpers.poetry_install import poetry_install
 from cv_smart_house_camera.generate_code import generate_code
 from google.protobuf.empty_pb2 import Empty
 from cv_smart_house_camera.constants import PORT
 from cv_smart_house_camera.utils.get_local_ip import get_local_ip
+import uuid
 
 class CameraService(object):
+
+    def __init__(self, poetry_path:str):
+        self.poetry_path = poetry_path
+
     def IsCameraAlive(self, ctx, request):
         return camera_service.IsCameraAliveResponse(is_alive=True)
         
 
     def InstallModules(self, ctx, request):
-        # Add packages from array to the project.
-        with open('pyproject.toml', 'r') as file:
-            pyproject_data = toml.load(file)
-
-        for package in request.modules:
-            pyproject_data['tool']['poetry']['dependencies'][package.name] = package.version
-
-        with open('pyproject.toml', 'w') as file:
-            toml.dump(pyproject_data, file)
-
-        generate_code()
-
-        return Empty()
+        try:
+            # Add packages from array to the project.
+            with open('pyproject.toml', 'r') as file:
+                pyproject_data = toml.load(file)
+
+            for package in request.modules:
+                pyproject_data['tool']['poetry']['dependencies'][package.name] = package.version
+
+            with open('pyproject.toml', 'w') as file:
+                toml.dump(pyproject_data, file)
+
+            # Install packages.
+            poetry_install(self.poetry_path)
+            generate_code()
+
+            return Empty()
+        except Exception as e:
+            print(e)
+            raise Exception("Error installing modules")
     
     def UninstallModules(self, ctx, request):
-        # Remove packages from array from the project.
-        original_names = []
-
-        #find original_name of the package
-        for module in request.modules:
-            for installed_module in modules_list:
-                if installed_module.get("name") == module:
-                    original_names.append(installed_module.get("package_name"))
-
-        with open('pyproject.toml', 'r') as file:
-            pyproject_data = toml.load(file)
-
-        for package in original_names:
-            del pyproject_data['tool']['poetry']['dependencies'][package]
-
-        with open('pyproject.toml', 'w') as file:
-            toml.dump(pyproject_data, file)
-
-        generate_code()
-
-        return Empty()
-    
+        try:
+            # Remove packages from array from the project.
+            original_names = []
+
+            #find original_name of the package
+            for module in request.modules:
+                for installed_module in modules_list:
+                    if installed_module.get("name") == module:
+                        original_names.append(installed_module.get("package_name"))
+
+            with open('pyproject.toml', 'r') as file:
+                pyproject_data = toml.load(file)
+
+            for package in original_names:
+                del pyproject_data['tool']['poetry']['dependencies'][package]
+
+            with open('pyproject.toml', 'w') as file:
+                toml.dump(pyproject_data, file)
+
+            # Install packages.
+            poetry_install(self.poetry_path)
+            generate_code()
+
+            return Empty()
+        except Exception as e:
+            print(e)
+            raise Exception("Error uninstalling modules")
+        
     def GetInstalledModules(self, ctx, request):
         formatted_modules = []
 
         for module in modules_list:
             formatted_modules.append(camera_service.InstalledModule(name = module.get("name"), package_name = module.get("package_name"), options = module.get("options")))
 
         return camera_service.InstalledModules(modules=formatted_modules)
@@ -72,56 +89,46 @@
         if module_result is None or module_result.get("ok") == False:
             raise Exception(f"Module {request.module} failed processing")
         
         frame = module_result.get("frame")
 
         return camera_service.Frame(frame=frame)
 
-app = TwirpASGIApp()
-service = CameraServiceServer(service=CameraService())
-app.add_service(service)
 
-# Wrap the app with CORSMiddleware
-app = CORSMiddleware(
-    app,
-    allow_origins=["*"],
-    allow_methods=["*"],
-    allow_headers=["*"],
-)
-
-def run_server():
-    uvicorn.run(app=app, host=get_local_ip(), port=PORT)
 
 def configure_camera_server(services: list = [], 
                             modules: list = [],
+                            poetry_path:str="poetry",
                             allow_origins=[],
                             allow_methods=[],
                             allow_headers=[]):
     logging.basicConfig()
-
-    # Install packages.
-    poetry_install()
+    poetry_install(poetry_path=poetry_path)
 
     # Add modules to the list
     for module in modules:
-        module["package_name"] = "internal"
+        module["package_name"] = "internal_"+str(uuid.uuid4())
         modules_list.append(module)
 
     app = TwirpASGIApp()
-    services.append(CameraServiceServer(service=CameraService()))
+    services.append(CameraServiceServer(service=CameraService(poetry_path)))
 
     for service in services:
         app.add_service(service)
 
 
 
     # Wrap the app with CORSMiddleware
     app = CORSMiddleware(
     app,
     allow_origins=allow_origins,
     allow_methods=allow_methods,
     allow_headers=allow_headers,
     )
 
+
+    def run_server():
+        uvicorn.run(app=app, host=get_local_ip(), port=PORT)
+        
     thread = Thread(target = run_server, args = ())
     thread.start()
     cam_capture()
```

### Comparing `cv_smart_house_camera-0.1.5/cv_smart_house_camera/cam_capture.py` & `cv_smart_house_camera-0.1.6/cv_smart_house_camera/cam_capture.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.5/cv_smart_house_camera/generate_code.py` & `cv_smart_house_camera-0.1.6/cv_smart_house_camera/generate_code.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 from cv_smart_house_camera.utils.get_modules_from_toml import get_modules_from_toml
 
+import os
+
+# Define the path
+path = '.\\.tmp'
+file_path = os.path.join(path, 'modules_list.py')
+
+# Check if the directory exists and create it if it doesn't
+if not os.path.exists(path):
+    os.makedirs(path)
+
+
+
+
 def generate_code():
     modules = get_modules_from_toml()
     import_code = []
-    original_frame_processing = "def original_frame_processing(frame, frame_number):\n\treturn"
-    modules_list = ['{ "name": "Original Frame", "package_name": "internal", "processing": original_frame_processing }']
+    modules_list = []
 
 
 
     for package, version in modules:
         import_statement = f"import {package}"
         import_code.append(import_statement)
         module_item = f"""{{ "name": {package}.name, "package_name": "{package}", "processing": {package}.processing, "options": {package}.options }}"""
 
         modules_list.append(module_item)
 
-    # with open('.\\cv_smart_house_camera\\modules\\modules_list.py', 'w') as out_file:
-    with open('.\\.venv\\Lib\\site-packages\\cv_smart_house_camera\\modules\\modules_list.py', 'w') as out_file:
-        out_file.write('\n'.join([*import_code, "\n", original_frame_processing, "\n" "modules = [", ", ".join(modules_list), "]"]))
+    # Write to the file
+    with open(file_path, 'w') as out_file:
+        out_file.write('\n'.join([*import_code, "\n", "modules = [", ", ".join(modules_list), "]"]))
 
 if __name__ == "__main__":
     generate_code()
```

### Comparing `cv_smart_house_camera-0.1.5/cv_smart_house_camera/modules/modules_processing.py` & `cv_smart_house_camera-0.1.6/cv_smart_house_camera/modules/modules_processing.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.5/cv_smart_house_camera/proto_services/camera_service_pb2.py` & `cv_smart_house_camera-0.1.6/cv_smart_house_camera/proto_services/camera_service_pb2.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.5/cv_smart_house_camera/proto_services/camera_service_twirp.py` & `cv_smart_house_camera-0.1.6/cv_smart_house_camera/proto_services/camera_service_twirp.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.5/cv_smart_house_camera/utils/get_modules_from_toml.py` & `cv_smart_house_camera-0.1.6/cv_smart_house_camera/utils/get_modules_from_toml.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.5/pyproject.toml` & `cv_smart_house_camera-0.1.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cv-smart-house-camera"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = [ "Your Name <you@example.com>",]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 flask = "^3.0.3"
@@ -21,9 +21,9 @@
 protobuf = "^5.26.1"
 uvicorn = "^0.29.0"
 starlette = "^0.37.2"
 aiohttp = "^3.9.5"
 aiortc = "^1.8.0"
 
 [tool.poetry.scripts]
-start = "cv_smart_house_camera.__init__:configure_camera_server"
+start = "cv_smart_house_camera.main:main"
 compile = "compile_proto:compile_proto_files"
```

### Comparing `cv_smart_house_camera-0.1.5/PKG-INFO` & `cv_smart_house_camera-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cv-smart-house-camera
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
```

