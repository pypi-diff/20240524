# Comparing `tmp/nebulagraph_lite-0.2.3.tar.gz` & `tmp/nebulagraph_lite-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nebulagraph_lite-0.2.3.tar", last modified: Thu May 23 12:13:52 2024, max compression
+gzip compressed data, was "nebulagraph_lite-0.2.4.tar", last modified: Fri May 24 04:20:16 2024, max compression
```

## Comparing `nebulagraph_lite-0.2.3.tar` & `nebulagraph_lite-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/LICENSE
--rw-r--r--   0        0        0     7200 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/README.md
--rw-r--r--   0        0        0      859 2024-05-23 12:13:52.144414 nebulagraph_lite-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      129 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/src/nebulagraph_lite/__init__.py
--rw-r--r--   0        0        0     4446 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/src/nebulagraph_lite/cli.py
--rw-r--r--   0        0        0    27930 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/src/nebulagraph_lite/nebulagraph.py
--rw-r--r--   0        0        0     3625 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/src/nebulagraph_lite/utils.py
--rw-r--r--   0        0        0        0 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     4687 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/tests/e2e/jupyter/jupyter_test.ipynb
--rw-r--r--   0        0        0     3877 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/tests/e2e/jupyter/modelscope_test.ipynb
--rw-r--r--   0        0        0     7535 1970-01-01 00:00:00.000000 nebulagraph_lite-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 04:18:47.143566 nebulagraph_lite-0.2.4/LICENSE
+-rw-r--r--   0        0        0     7200 2024-05-24 04:18:47.143566 nebulagraph_lite-0.2.4/README.md
+-rw-r--r--   0        0        0      859 2024-05-24 04:20:15.608021 nebulagraph_lite-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      129 2024-05-24 04:18:47.143566 nebulagraph_lite-0.2.4/src/nebulagraph_lite/__init__.py
+-rw-r--r--   0        0        0     4446 2024-05-24 04:18:47.143566 nebulagraph_lite-0.2.4/src/nebulagraph_lite/cli.py
+-rw-r--r--   0        0        0    28084 2024-05-24 04:18:47.143566 nebulagraph_lite-0.2.4/src/nebulagraph_lite/nebulagraph.py
+-rw-r--r--   0        0        0     4160 2024-05-24 04:18:47.143566 nebulagraph_lite-0.2.4/src/nebulagraph_lite/utils.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:18:47.143566 nebulagraph_lite-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     4687 2024-05-24 04:18:47.143566 nebulagraph_lite-0.2.4/tests/e2e/jupyter/jupyter_test.ipynb
+-rw-r--r--   0        0        0     3877 2024-05-24 04:18:47.143566 nebulagraph_lite-0.2.4/tests/e2e/jupyter/modelscope_test.ipynb
+-rw-r--r--   0        0        0     7535 1970-01-01 00:00:00.000000 nebulagraph_lite-0.2.4/PKG-INFO
```

### Comparing `nebulagraph_lite-0.2.3/LICENSE` & `nebulagraph_lite-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nebulagraph_lite-0.2.3/README.md` & `nebulagraph_lite-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nebulagraph_lite-0.2.3/pyproject.toml` & `nebulagraph_lite-0.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 dependencies = [
     "udocker==1.3.13",
     "psutil>=5.9.6",
     "nebula3-python>=3.8.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.2.3"
+version = "0.2.4"
 
 [project.license]
 text = "Apache 2.0"
 
 [project.scripts]
 nebulagraph = "nebulagraph_lite.cli:main"
```

### Comparing `nebulagraph_lite-0.2.3/src/nebulagraph_lite/cli.py` & `nebulagraph_lite-0.2.4/src/nebulagraph_lite/cli.py`

 * *Files identical despite different names*

### Comparing `nebulagraph_lite-0.2.3/src/nebulagraph_lite/nebulagraph.py` & `nebulagraph_lite-0.2.4/src/nebulagraph_lite/nebulagraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -609,15 +609,16 @@
 
     def start(self, fresh=False):
         shoot = bool(fresh)
         self.udocker_init()
         # if on_modelscope, we should load the model first
         if self.on_modelscope:
             fancy_print(
-                f"Info: loading nebulagraph_lite model from {self.modelscope_file}..."
+                f"Info: loading nebulagraph_lite model from {self.modelscope_file}...",
+                color="light_green",
             )
             os.system(f"tar -xzf {self.modelscope_file} -C {self.base_path}")
 
             try:
                 self._run_udocker(
                     f"load -i {self.base_path}/nebulagraph_lite_meta.tar"
                 )
@@ -629,15 +630,18 @@
                 )
                 self._run_udocker(
                     f"load -i {self.base_path}/nebulagraph_lite_console.tar"
                 )
             except Exception as e:
                 if self._debug:
                     fancy_print(f"Info: [DEBUG] error when load model, {e}")
-            fancy_print(f"Info: nebulagraph_lite model loaded successfully!")
+            fancy_print(
+                f"Info: nebulagraph_lite model loaded successfully!",
+                color="light_blue",
+            )
         # async pull images
         if not self.on_modelscope:
             self.udocker_pull(
                 f"{self._container_image_prefix}vesoft/nebula-metad:v3"
             )
             self.udocker_pull_backgroud(
                 f"{self._container_image_prefix}vesoft/nebula-graphd:v3"
@@ -652,18 +656,20 @@
         time.sleep(20)
         self.activate_storaged()
         if not self.on_modelscope:
             self.udocker_pull(
                 f"{self._container_image_prefix}vesoft/nebula-console:v3"
             )
         time.sleep(20)
-        fancy_print("Info: loading basketballplayer dataset...")
+        fancy_print("Info: loading basketballplayer dataset...", color="green")
         self.load_basketballplayer_dataset()
         fancy_print(BANNER_ASCII)
-        fancy_print("[ OK ] nebulagraph_lite started successfully!", "purple")
+        fancy_print(
+            "[ OK ] nebulagraph_lite started successfully!", color="light_purple"
+        )
         self.docker_ps()
 
     def check_status(self):
         self._run_udocker_ps_filter("metad")
         self._run_udocker_ps_filter("graphd")
         self._run_udocker_ps_filter("storaged")
```

### Comparing `nebulagraph_lite-0.2.3/src/nebulagraph_lite/utils.py` & `nebulagraph_lite-0.2.4/src/nebulagraph_lite/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,25 +12,41 @@
     "blue": "#2f4b7c",
     "purple": "#665191",
     "magenta": "#a05195",
     "pink": "#d45087",
     "red": "#f95d6a",
     "orange": "#ff7c43",
     "yellow": "#ffa600",
+    "green": "#a8ff9f",
+    "light_green": "#baf278",
+    "light_blue": "#78caff",
+    "light_purple": "#d2a6ff",
+    "light_pink": "#ff94d2",
+    "light_red": "#ff79c6",
+    "light_orange": "#ffb47b",
+    "light_yellow": "#ffe8a1",
 }
 
 COLORS_rgb = {
     # "dark_blue": "38;2;0;63;92",
     "blue": "38;2;47;75;124",
     "purple": "38;2;102;81;145",
     "magenta": "38;2;160;81;149",
     "pink": "38;2;212;80;135",
     "red": "38;2;249;93;106",
     "orange": "38;2;255;124;67",
     "yellow": "38;2;255;166;0",
+    "green": "38;2;168;255;159",
+    "light_green": "38;2;186;252;78",
+    "light_blue": "38;2;120;198;255",
+    "light_purple": "38;2;210;161;255",
+    "light_pink": "38;2;255;148;181",
+    "light_red": "38;2;255;129;159",
+    "light_orange": "38;2;255;186;119",
+    "light_yellow": "38;2;255;239;0",
 }
 
 BANNER_ASCII = r"""
   _   _      _           _        ____                 _     
  | \ | | ___| |__  _   _| | __ _ / ___|_ __ __ _ _ __ | |__  
  |  \| |/ _ | '_ \| | | | |/ _` | |  _| '__/ _` | '_ \| '_ \ 
  | |\  |  __| |_) | |_| | | (_| | |_| | | | (_| | |_) | | | |
```

### Comparing `nebulagraph_lite-0.2.3/tests/e2e/jupyter/jupyter_test.ipynb` & `nebulagraph_lite-0.2.4/tests/e2e/jupyter/jupyter_test.ipynb`

 * *Files identical despite different names*

### Comparing `nebulagraph_lite-0.2.3/tests/e2e/jupyter/modelscope_test.ipynb` & `nebulagraph_lite-0.2.4/tests/e2e/jupyter/modelscope_test.ipynb`

 * *Files identical despite different names*

### Comparing `nebulagraph_lite-0.2.3/PKG-INFO` & `nebulagraph_lite-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebulagraph-lite
-Version: 0.2.3
+Version: 0.2.4
 Summary: Plug and play NebulaGraph with pip install.
 Author-Email: Wey Gu <weyl.gu@gmail.com>
 License: Apache 2.0
 Requires-Python: >=3.8
 Requires-Dist: udocker==1.3.13
 Requires-Dist: psutil>=5.9.6
 Requires-Dist: nebula3-python>=3.8.0
```

