# Comparing `tmp/mlf-api-0.2.1.tar.gz` & `tmp/mlf-api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlf-api-0.2.1.tar", last modified: Fri Mar 22 19:03:47 2024, max compression
+gzip compressed data, was "mlf-api-0.2.2.tar", last modified: Fri May 24 21:49:51 2024, max compression
```

## Comparing `mlf-api-0.2.1.tar` & `mlf-api-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 19:03:47.496775 mlf-api-0.2.1/
--rw-rw-rw-   0        0        0     1095 2024-03-15 17:49:15.000000 mlf-api-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      165 2024-03-22 19:03:47.495774 mlf-api-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-03-15 17:49:15.000000 mlf-api-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 19:03:47.473771 mlf-api-0.2.1/mlf_api/
--rw-rw-rw-   0        0        0       30 2024-03-15 17:50:45.000000 mlf-api-0.2.1/mlf_api/__init__.py
--rw-rw-rw-   0        0        0      768 2024-03-22 19:01:50.000000 mlf-api-0.2.1/mlf_api/inverse_kinematics.py
--rw-rw-rw-   0        0        0     2582 2024-03-22 13:58:37.000000 mlf-api-0.2.1/mlf_api/robot.py
--rw-rw-rw-   0        0        0      735 2024-03-15 17:50:45.000000 mlf-api-0.2.1/mlf_api/signaling.py
--rw-rw-rw-   0        0        0     2258 2024-03-15 17:50:45.000000 mlf-api-0.2.1/mlf_api/videoShow.py
--rw-rw-rw-   0        0        0     3841 2024-03-15 17:50:45.000000 mlf-api-0.2.1/mlf_api/webRTC.py
-drwxrwxrwx   0        0        0        0 2024-03-22 19:03:47.493774 mlf-api-0.2.1/mlf_api.egg-info/
--rw-rw-rw-   0        0        0      165 2024-03-22 19:03:47.000000 mlf-api-0.2.1/mlf_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-03-22 19:03:47.000000 mlf-api-0.2.1/mlf_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 19:03:47.000000 mlf-api-0.2.1/mlf_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-03-22 19:03:47.000000 mlf-api-0.2.1/mlf_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-22 19:03:47.000000 mlf-api-0.2.1/mlf_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 19:03:47.496775 mlf-api-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      309 2024-03-22 19:03:32.000000 mlf-api-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 21:49:51.662406 mlf-api-0.2.2/
+-rw-rw-rw-   0        0        0     1095 2024-03-15 17:49:15.000000 mlf-api-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      165 2024-05-24 21:49:51.661404 mlf-api-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-03-15 17:49:15.000000 mlf-api-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 21:49:51.651405 mlf-api-0.2.2/mlf_api/
+-rw-rw-rw-   0        0        0       30 2024-03-15 17:50:45.000000 mlf-api-0.2.2/mlf_api/__init__.py
+-rw-rw-rw-   0        0        0      768 2024-03-22 19:01:50.000000 mlf-api-0.2.2/mlf_api/inverse_kinematics.py
+-rw-rw-rw-   0        0        0     2862 2024-05-24 21:27:19.000000 mlf-api-0.2.2/mlf_api/robot.py
+-rw-rw-rw-   0        0        0      735 2024-03-15 17:50:45.000000 mlf-api-0.2.2/mlf_api/signaling.py
+-rw-rw-rw-   0        0        0     2258 2024-03-15 17:50:45.000000 mlf-api-0.2.2/mlf_api/videoShow.py
+-rw-rw-rw-   0        0        0     3841 2024-03-15 17:50:45.000000 mlf-api-0.2.2/mlf_api/webRTC.py
+drwxrwxrwx   0        0        0        0 2024-05-24 21:49:51.660406 mlf-api-0.2.2/mlf_api.egg-info/
+-rw-rw-rw-   0        0        0      165 2024-05-24 21:49:51.000000 mlf-api-0.2.2/mlf_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-05-24 21:49:51.000000 mlf-api-0.2.2/mlf_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 21:49:51.000000 mlf-api-0.2.2/mlf_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-05-24 21:49:51.000000 mlf-api-0.2.2/mlf_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-24 21:49:51.000000 mlf-api-0.2.2/mlf_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 21:49:51.662406 mlf-api-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      309 2024-05-24 21:39:53.000000 mlf-api-0.2.2/setup.py
```

### Comparing `mlf-api-0.2.1/LICENSE` & `mlf-api-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlf-api-0.2.1/README.md` & `mlf-api-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mlf-api-0.2.1/mlf_api/inverse_kinematics.py` & `mlf-api-0.2.2/mlf_api/inverse_kinematics.py`

 * *Files identical despite different names*

### Comparing `mlf-api-0.2.1/mlf_api/robot.py` & `mlf-api-0.2.2/mlf_api/robot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+import json
 from .webRTC import WebRTCController
 from .videoShow import VideoShow
 
 from .inverse_kinematics import inverse_kinematics
 
 
 class RobotClient:
@@ -12,63 +13,69 @@
     HOME_Q2 = 90
 
     def __init__(self, address, port=5000, portVideo=8080):
         self.address = address
         self.port = port
         self.base_url = f"http://{address}:{port}"
         self.connected = False
+        self.session = requests.Session()
         self.webRTCUser = WebRTCController(self.address)
 
     def connect(self):
         if self.connected:
             print("already connected :)")
             return
 
         url = f"{self.base_url}/connect"
-        response = requests.get(url)
+        response = self.session.get(url)
         if response.status_code == 200:
             self.connected = True
             print(response.text)
 
     def move_xyz(self, x, y, z, eff_off = [56, 0, 0], q3=120):
         eff_off_x, eff_off_y, eff_off_z = eff_off
         q0, q1, q2 = inverse_kinematics(x, y, z, eff_off_x, eff_off_z)
         params = {"q0": q0, "q1": q1, "q2": q2, "q3": q3}
         url = f"{self.base_url}/set_joints"
-        response = requests.get(url, params=params)
+        response = self.session.get(url, params=params)
         print(response.text)
         
 
     def set_joints(self, q0=0, q1=0, q2=90, q3=120):
         params = {"q0": q0, "q1": q1, "q2": q2, "q3": q3}
         url = f"{self.base_url}/set_joints"
-        response = requests.get(url, params=params)
+        response = self.session.get(url, params=params)
         print(response.text)
 
     def set_relay_status(self, state=1, relay=1):
         params = {"state": state, "n_relay": relay}
         url = f"{self.base_url}/set_relay_status"
-        response = requests.get(url, params=params)
+        response = self.session.get(url, params=params)
         print(response.text)
     
     def connectWebRTC(self):
         self.webRTCUser.connect()
 
     def set_extra_servo(self, q=0):
         params = {"q": q}
         url = f"{self.base_url}/set_extra_servo"
-        response = requests.get(url, params=params)
+        response = self.session.get(url, params=params)
         print(response.text)
 
     def set_gripper_servo(self, q=120):
         params = {"q": q}
         url = f"{self.base_url}/set_gripper_servo"
-        response = requests.get(url, params=params)
+        response = self.session.get(url, params=params)
         print(response.text)
     
+    def get_weight(self):
+        url = f"{self.base_url}/get_weight"
+        response = self.session.get(url)
+        json_data = json.loads(response.text)
+        return json_data['weight'][0]
 
     def closeWebRTC(self):
         self.webRTCUser.close()
         
 
     def showVideo(self, process= lambda frame : (frame, None)):
         self.webRTCUser.showVideo(process)
```

### Comparing `mlf-api-0.2.1/mlf_api/signaling.py` & `mlf-api-0.2.2/mlf_api/signaling.py`

 * *Files identical despite different names*

### Comparing `mlf-api-0.2.1/mlf_api/videoShow.py` & `mlf-api-0.2.2/mlf_api/videoShow.py`

 * *Files identical despite different names*

### Comparing `mlf-api-0.2.1/mlf_api/webRTC.py` & `mlf-api-0.2.2/mlf_api/webRTC.py`

 * *Files identical despite different names*

