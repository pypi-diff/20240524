# Comparing `tmp/eyegestures-1.4.5.tar.gz` & `tmp/eyegestures-2.0.0.tar.gz`

## Comparing `eyegestures-1.4.5.tar` & `eyegestures-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/Fixation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/__init__.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/calibration.py
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/eye.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/eyegestures.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/face.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/gazeContexter.py
--rw-r--r--   0        0        0     9767 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/gazeEstimator.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/gevent.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/processing.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/scalling_test.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/screenTracker_test.py
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/utils.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/screenTracker/clusters.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/screenTracker/dataPoints.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/screenTracker/heatmap.py
--rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 eyegestures-1.4.5/eyeGestures/screenTracker/screenTracker.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eyegestures-1.4.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 eyegestures-1.4.5/LICENSE
--rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 eyegestures-1.4.5/README.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 eyegestures-1.4.5/pyproject.toml
--rw-r--r--   0        0        0    51749 2020-02-02 00:00:00.000000 eyegestures-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/Fixation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/__init__.py
+-rw-r--r--   0        0        0     6689 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/calibration_v1.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/calibration_v2.py
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/eye.py
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/eyegestures.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/face.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/gazeContexter.py
+-rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/gazeEstimator.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/gevent.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/processing.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/scalling_test.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/screenTracker_test.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/utils.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/screenTracker/clusters.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/screenTracker/dataPoints.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/screenTracker/heatmap.py
+-rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 eyegestures-2.0.0/eyeGestures/screenTracker/screenTracker.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eyegestures-2.0.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 eyegestures-2.0.0/LICENSE
+-rw-r--r--   0        0        0     6973 2020-02-02 00:00:00.000000 eyegestures-2.0.0/README.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 eyegestures-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    48245 2020-02-02 00:00:00.000000 eyegestures-2.0.0/PKG-INFO
```

### Comparing `eyegestures-1.4.5/eyeGestures/Fixation.py` & `eyegestures-2.0.0/eyeGestures/Fixation.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.4.5/eyeGestures/eye.py` & `eyegestures-2.0.0/eyeGestures/eye.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.4.5/eyeGestures/face.py` & `eyegestures-2.0.0/eyeGestures/face.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.4.5/eyeGestures/gazeContexter.py` & `eyegestures-2.0.0/eyeGestures/gazeContexter.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.4.5/eyeGestures/gazeEstimator.py` & `eyegestures-2.0.0/eyeGestures/gazeEstimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,29 +220,27 @@
             # this should prevent of sudden movement down when blinking - not perfect yet
 
             if fix > fixation_freeze:
                 r = freeze_radius
                 if not isInside(self.freezed_point[0], self.freezed_point[1], r, self.point_screen[0], self.point_screen[1]):
                     self.freezed_point = self.point_screen
 
-                event = Gevent(compound_point,
-                               self.freezed_point,
+                event = Gevent(self.freezed_point,
                                blink,
                                fix,
                                l_eye,
                                r_eye,
                                display,
                                context.roi,
                                context.edges,
                                context.cluster_boundaries,
                                context_id)
             else:
                 self.freezed_point = self.point_screen
-                event = Gevent(compound_point,
-                               self.point_screen,
+                event = Gevent(self.point_screen,
                                blink,
                                fix,
                                l_eye,
                                r_eye,
                                display,
                                context.roi,
                                context.edges,
```

### Comparing `eyegestures-1.4.5/eyeGestures/processing.py` & `eyegestures-2.0.0/eyeGestures/processing.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.4.5/eyeGestures/scalling_test.py` & `eyegestures-2.0.0/eyeGestures/scalling_test.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.4.5/eyeGestures/screenTracker_test.py` & `eyegestures-2.0.0/eyeGestures/screenTracker_test.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.4.5/eyeGestures/utils.py` & `eyegestures-2.0.0/eyeGestures/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,16 @@
 
         if self.stream:
             self.prev_frame = None
 
             self.__openCam(name)
 
             self.q = queue.Queue()
-            self.t = threading.Thread(target=self.__reader).start()
+            self.t = threading.Thread(target=self.__reader)
+            self.t.start()
         else:
             self.frames = []
             with open(name, 'rb') as file:
                 self.frames = pickle.load(file)
 
     def __openCam(self, name):
         if isinstance(name, int):
@@ -189,7 +190,9 @@
             frame = self.frames.pop(0)
             self.frames.pop(0)
             return ((len(self.frames) >= 1), frame)
 
     def close(self):
         """Function closing stream"""
         self.run = False
+        self.t.join()
+        self.cap.release()
```

### Comparing `eyegestures-1.4.5/eyeGestures/screenTracker/clusters.py` & `eyegestures-2.0.0/eyeGestures/screenTracker/clusters.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.4.5/eyeGestures/screenTracker/dataPoints.py` & `eyegestures-2.0.0/eyeGestures/screenTracker/dataPoints.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.4.5/eyeGestures/screenTracker/heatmap.py` & `eyegestures-2.0.0/eyeGestures/screenTracker/heatmap.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.4.5/eyeGestures/screenTracker/screenTracker.py` & `eyegestures-2.0.0/eyeGestures/screenTracker/screenTracker.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.4.5/LICENSE` & `eyegestures-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eyegestures-1.4.5/pyproject.toml` & `eyegestures-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "test_app.py",
   "test.py",
   "tools/*"
 ]
 
 [project]
 name = "eyeGestures"
-version = "1.4.5"
+version = "2.0.0"
 authors = [
   { name="Piotr Walas", email="piotr.walas@eyegestures.com" },
 ]
 maintainers = [
   { name="Piotr Walas", email="piotr.walas@eyegestures.com" }
 ]
 description = "Package for eye tracking algorithm allowing for development of gaze controlled computer interface"
```

### Comparing `eyegestures-1.4.5/PKG-INFO` & `eyegestures-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: eyeGestures
-Version: 1.4.5
+Version: 2.0.0
 Summary: Package for eye tracking algorithm allowing for development of gaze controlled computer interface
 Project-URL: Homepage, https://github.com/NativeSensors/EyeGestures
 Project-URL: Issues, https://github.com/NativeSensors/EyeGestures/Issues
 Author-email: Piotr Walas <piotr.walas@eyegestures.com>
 Maintainer-email: Piotr Walas <piotr.walas@eyegestures.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -684,227 +684,136 @@
 Keywords: eye,eyetracking,gaze,gazetracking,tracking
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
+<p align="center">
+  <picture>
+    <source srcset="https://github.com/NativeSensors/EyeGestures/assets/40773550/ddfc8b96-5a7e-4487-9307-6fbd62e8915e" media="(prefers-color-scheme: light)"/>   
+    <source srcset="https://github.com/NativeSensors/EyeGestures/assets/40773550/6d42b8a2-24ea-4cbc-bdb0-ad688ee26c36" media="(prefers-color-scheme: dark)"/>    
+   <img width="300px" height="300px"/>
+  </picture>
+</p>
+
+## EYEGESTURES
+
+
+EyeGestures is open source eyetracking software/library using native webcams and phone camers for achieving its goal. The aim of library is to bring accessibility of eyetracking and eyedriven interfaces without requirement of obtaining expensive hardware.
 
+Our [Mission](https://github.com/NativeSensors/EyeGestures/blob/Engine_v2/MISSION.md)! 
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eyeGestures)
+<a href="https://polar.sh/NativeSensors"><img src="https://polar.sh/embed/seeks-funding-shield.svg?org=NativeSensors" /></a>
+### 💜 Sponsors: 
 
 ```
 For enterprise avoiding GPL3 licensing there is commercial license!
 ```
 We offer custom integration and managed services. For businesses requiring invoices message us `contact@eyegestures.com`.
 
-### 💜 Sponsors: 
-
 ```
 Sponsor us and we can add your link, banner or other promo materials!
 ```
 <!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
 
 
 
 <!-- POLAR-END id=eizdelwu -->
 
-## 👁️ EyeGestures
-
-EyeGestures is open source eyetracking software/library using native webcams and phone camers for achieving its goal. The aim of library is to bring accessibility of eyetracking and eyedriven interfaces without requirement of obtaining expensive hardware.
-
 <p align="center">
   <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/2ad25252-e96e-47d4-b25f-c47ba7f0f4f3" width="300" height="150">
 <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/f3132843-063a-439a-8e1c-2385ddfdccda" width="300
 " height="150">
 </p>
 <p align="center">
-<img src="https://github.com/NativeSensors/EyeGestures/assets/40773550/84aa7436-6153-49bc-b8e6-ccda535f25e6)" width="600
-" height="300">
+  <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/3b38d73d-bb6f-4f31-b67d-231ac4cd04cb" width="300" height="150">
+  <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/1715b4df-7ac3-479e-b51a-f6d800ea8ea5" width="300" height="150">
 </p>
 
-### ⭐ Mission
-
-There is no one-size-fits-all solution, and we believe that diversifying interfaces brings accessibility to digital spaces. Designing eye-driven interfaces provides greater control over computers for those unable to fully utilize their capabilities due to various disabilities, while also offering an additional means of computer control for all users.
-
-Such technology should not be hindered by expensive eye-tracking hardware, particularly when it is essential for individuals to navigate the digital realm and operate their computers. Many current consumer electronics devices feature built-in native cameras, and ongoing research suggests that achieving eye tracking with reasonable accuracy using these native cameras is feasible.
-
-Our mission is to democratize eye-tracking technology, making it accessible to as many people as possible.
-
-While our technology is not flawless, we are committed to continuous improvement and strive for excellence.
-
-### 📢 Announcements:
-
-<a href="https://polar.sh/NativeSensors/posts"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/posts.svg?org=NativeSensors&darkmode"><img alt="Posts on Polar" src="https://polar.sh/embed/posts.svg?org=NativeSensors"></picture></a>
-
-### 📇 Find us:
-- [RSS](https://polar.sh/NativeSensors/rss?auth=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJwYXRfaWQiOiJkMDYxMDFiOC0xYzYyLTQ1MTYtYjg3YS03NTFhOTM3OTIxZmUiLCJzY29wZXMiOiJhcnRpY2xlczpyZWFkIiwidHlwZSI6ImF1dGgiLCJleHAiOjE3NDMxNjg3ODh9.djoi5ARWHr-xFW_XJ6Fwal3JUT1fAbvx4Npl-daBC5U)
-- [discord](https://discord.gg/FV3RYTuV)
-- [twitter](https://twitter.com/PW4ltz)
-- email: contact@eyegestures.com
-
-Follow us on polar (it costs nothing but you help project!):
-
-<a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
-
-### 🔥 Web Demos:
-
-- [Main page](https://eyegestures.com/)
-- [Game demo](https://eyegestures.com/game)
-- [Cinema demo](https://eyegestures.com/cinema)
-- [Restaurant](https://eyegestures.com/restaurant)
+<p align="center">
+  <a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
+</p>
 
 ### 💻 Install
 ```
 python3 -m pip install eyeGestures
 ```
 
-Note: you may need to change version of package `eyegestures-X.X.X`.
-
 ### ⚙️ Run 
 ```
 python3 examples/simple_example.py
 ```
 
 ### 🪟 Run Windows App 
 ```
 python3 apps/win_app.py
 ```
 
 Or download it from [`releases`](https://github.com/NativeSensors/EyeGestures/releases/tag/1.3.4_App_0.0.3)
 
-### 🔧 Develop 
+### 🔧 How to use [WiP - adding Enginge V2]:
 
-To begin, you instantiate an EyeGestures object with initial Region of Interest (RoI) parameters. These parameters define a preliminary focus area for the tracker within a virtual 500x500 screen space, which helps in locating the user's gaze more efficiently.
-
-Main `EyeGesture` object provides general configuration initial conditions: 
+#### Using EyeGesture Engine V2 - Machine Learning Approach:
 
 ```python
-EyeGestures(  
-  roi_x = 285
-  roi_y = 115
-  roi_width = 80
-  roi_height = 15
-)
-```  
+from eyeGestures.utils import VideoCapture
+from eyeGestures.eyegestures import EyeGestures_v2
 
-The tracker operates within a virtual screen measuring 500x500, where it maps the positions of the pupils and other critical facial features to deduce the user's gaze direction. Within this space, the Region of Interest (RoI) serves as a representation of the user's display, inferred through a combination of eye movement and edge detection during calibration.
+# Initialize gesture engine and video capture
+gestures = EyeGestures_v2()
+cap = VideoCapture(0)  
 
-After locating the RoI within the 500x500 space, its dimensions are adjusted to fit the resolution used in the estimate function, typically described as `display_width` by `display_height`.
+# Process each frame
+point, calibration_point, blink, fixation, acceptance_radius, calibration_radius = gestures.step(frame, calibrate, screen_width, screen_height)
+# point: x, y positions of cursor
+# calibration_point: x, y position of current calibration point
+# acceptance_radius: precision required for calibration
+# calibration_radius: radius for data collection during calibration
+```
 
-Calibration aims to precisely determine the RoI's dimensions. Prior to calibration, the tracker relies on initial optional parameters, including:
+<!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
 
-- `roi_x`: The initial x-coordinate of the RoI (ranging from 0 to 500).
-- `roi_y`: The initial y-coordinate of the RoI (ranging from 0 to 500).
-- `roi_width`: The initial width of the RoI before calibration (ranging from 0 to 500 - x).
-- `roi_height`: The initial height of the RoI before calibration (ranging from 0 to 500 - x).
 
-Next part is obtaining estimations from camera frames (if you cannot get estimations, you may try to change color coding or rotation of image - check `simple_example.py`).
 
-```python
-event = gestures.estimate(
-    image = frame,
-    context = "main",
-    calibration = True, # set calibration - switch to False to stop calibration
-    display_width = screen_width,
-    display_height = screen_height,
-    display_offset_x = 0, 
-    display_offset_y = 0, 
-    fixation_freeze = 0.8,
-    freeze_radius = 10)
-```
-
-- `image` - is cv2 image frame
-- `context` - is name given to contect. If name changes then different tracker context is used. Tracker rembers previous points to estimate new one, but those points are assinged to single context. By changing names or passing new ones you can switch and create contextes.
-- `calibration` - if `True` then every few seconds tracker is recalibrating, if `False` then tracker setting is frozen. The best approach is to enable calibration when one of the edges is reached. 
-- `display_width` - width of display/screen used.
-- `display_height` - height of display/screen used.
-- `display_offset_x` - offset of x for display/screen used. Use it when having two displays and app is covering all screens, but you want to limit your cursor tracker to only specific display.
-- `display_offset_y` - offset of y for display/screen used. Use it when having two displays and app is covering all screens, but you want to limit your cursor tracker to only specific display.
-- `fixation_freeze` - threshold of user fixation on one point (it goes from 0.0 to 1.0). If threshold is crossed point is frozen till user breaks `freeze_radius` in pixels.
-- `freeze_radius` - distance cursor can move to reach fixation and freezing, if cursor movements are greater than distance then fixation measurement goes down to `0.0`.
-
-```
-Gevent event
-```
-
-`Gevent` is returned element having all data necessary to use tracker:
- 
-- `point_screen` is point coordinates on screen
-- `blink` is boolean value describing blink event. If `0` no blink occured, if `1` blink occured.
-- `fixation` value from `0.0` to `1.0` describing level of user fixation.
+<!-- POLAR-END id=eizdelwu -->
 
-Entire program: 
+#### Using EyeGesture Engine V1 - Model-Based Approach:
 
 ```python
-import VideoCapture #change it to opencv for real applications
 from eyeGestures.utils import VideoCapture
-from eyeGestures.eyegestures import EyeGestures
+from eyeGestures.eyegestures import EyeGestures_v1
 
-gestures = EyeGestures(
-  roi_x = 285
-  roi_y = 115
-  roi_width = 80
-  roi_height = 15
-)
+# Initialize gesture engine with RoI parameters
+gestures = EyeGestures_v1()
 
 cap = VideoCapture(0)  
+ret, frame = cap.read()
 
-# Main game loop
-running = True
-while running:
-
-    # Generate new random position for the cursor
-    ret, frame = cap.read()     
-
-    event = gestures.estimate(
-        frame,
-        "main",
-        True, # set calibration - switch to False to stop calibration
-        screen_width,
-        screen_height,
-        0, 0, 0.8,10)
-
-    cursor_x, cursor_y = event.point_screen[0],event.point_screen[1]
-
+# Obtain estimations from camera frames
+event = gestures.estimate(
+    frame,
+    "main",
+    True,  # set calibration - switch to False to stop calibration
+    screen_width,
+    screen_height,
+    0, 0, 0.8, 10
+)
+cursor_x, cursor_y = event.point[0], event.point[1]
 ```
 
+Feel free to copy and paste the relevant code snippets for your project.
 
-### 🌐 Web Embedd [Paid API]
-
-For now more info can be found here: https://eyegestures.com/user_portal
-
-```html
-// ... rest of html client ...
-
-<script>
-// ... your code ...
-
-function onTile(id, fix, blink) {
-  // ... do something here ...
-}
-
-function onCalibration() {
-  // ... do something here ...
-}
-</script>
-<script src="https://cdnjs.cloudflare.com/ajax/libs/socket.io/4.0.0/socket.io.js"></script>
-<script src="https://eyegestures.com/eyeTiles.min.js"></script>
-<script>
-  EyeTilesAPI(
-    key = "YOUR_API_KEY",
-    tiles = [1, 2, 1],
-    fixThresh = 0.1,
-    fixRadius = 500,
-    sightGrid = true,
-    onTile = onTile,
-    onCalibration = onCalibration,
-  );
-</script>    
-```
+### 🔥 Web Demos:
+
+- [Main page](https://eyegestures.com/)
+- [Game demo](https://eyegestures.com/game)
+- [Cinema demo](https://eyegestures.com/cinema)
+- [Restaurant](https://eyegestures.com/restaurant)
 
 ### rules of using
 
 If you are building publicly available product, and have no commercial license, please mention us somewhere in your interface. 
 
 **Promo Materials:**
 
@@ -914,14 +823,27 @@
 ">
 
 https://github.com/NativeSensors/EyeGestures/assets/40773550/6a7c74b5-b069-4eec-bc96-3a6bb4159b37
 
 <img src="https://github.com/NativeSensors/EyeGestures/assets/40773550/6a7c74b5-b069-4eec-bc96-3a6bb4159b37" width="200
 ">
 
+### 📇 Find us:
+- [RSS](https://polar.sh/NativeSensors/rss?auth=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJwYXRfaWQiOiJkMDYxMDFiOC0xYzYyLTQ1MTYtYjg3YS03NTFhOTM3OTIxZmUiLCJzY29wZXMiOiJhcnRpY2xlczpyZWFkIiwidHlwZSI6ImF1dGgiLCJleHAiOjE3NDMxNjg3ODh9.djoi5ARWHr-xFW_XJ6Fwal3JUT1fAbvx4Npl-daBC5U)
+- [discord](https://discord.gg/FV3RYTuV)
+- [twitter](https://twitter.com/PW4ltz)
+- email: contact@eyegestures.com
+
+Follow us on polar (it costs nothing but you help project!):
+
+<a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
+
+### 📢 Announcements:
+
+<a href="https://polar.sh/NativeSensors/posts"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/posts.svg?org=NativeSensors&darkmode"><img alt="Posts on Polar" src="https://polar.sh/embed/posts.svg?org=NativeSensors"></picture></a>
 
 ### 💻 Contributors
 
 <a href="https://github.com/OWNER/REPO/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=NativeSensors/EyeGestures" />
 </a>
```

