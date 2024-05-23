# Comparing `tmp/unray-1.0.3.tar.gz` & `tmp/unray-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unray-1.0.3.tar", last modified: Thu May 23 21:47:17 2024, max compression
+gzip compressed data, was "unray-1.0.4.tar", last modified: Thu May 23 21:58:10 2024, max compression
```

## Comparing `unray-1.0.3.tar` & `unray-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 21:47:17.376823 unray-1.0.3/
--rw-rw-rw-   0        0        0     1116 2024-05-23 21:39:25.000000 unray-1.0.3/LICENSE
--rw-rw-rw-   0        0        0    10541 2024-05-23 21:47:17.375247 unray-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     9895 2024-05-23 21:39:25.000000 unray-1.0.3/README.md
--rw-rw-rw-   0        0        0      751 2024-05-23 21:40:01.000000 unray-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 21:47:17.376823 unray-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-23 21:47:17.316948 unray-1.0.3/src/
--rw-rw-rw-   0        0        0       32 2024-05-23 21:39:25.000000 unray-1.0.3/src/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 21:47:17.323265 unray-1.0.3/src/unray/
--rw-rw-rw-   0        0        0        2 2024-05-23 21:39:25.000000 unray-1.0.3/src/unray/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 21:47:17.365726 unray-1.0.3/src/unray/envs/
--rw-rw-rw-   0        0        0        0 2024-05-23 21:39:25.000000 unray-1.0.3/src/unray/envs/__init__.py
--rw-rw-rw-   0        0        0     1491 2024-05-23 21:39:40.000000 unray-1.0.3/src/unray/envs/base_env.py
-drwxrwxrwx   0        0        0        0 2024-05-23 21:47:17.369249 unray-1.0.3/src/unray/envs/bridge/
--rw-rw-rw-   0        0        0     5487 2024-05-23 21:39:25.000000 unray-1.0.3/src/unray/envs/bridge/TCP_IP_Connector.py
--rw-rw-rw-   0        0        0        0 2024-05-23 21:39:25.000000 unray-1.0.3/src/unray/envs/bridge/__init__.py
--rw-rw-rw-   0        0        0    19426 2024-05-23 21:39:40.000000 unray-1.0.3/src/unray/envs/bridge_env.py
--rw-rw-rw-   0        0        0      110 2024-05-23 21:39:25.000000 unray-1.0.3/src/unray/envs/spaces.py
--rw-rw-rw-   0        0        0     1007 2024-05-23 21:39:25.000000 unray-1.0.3/src/unray/gui.py
--rw-rw-rw-   0        0        0     1374 2024-05-23 21:39:40.000000 unray-1.0.3/src/unray/unray_config.py
-drwxrwxrwx   0        0        0        0 2024-05-23 21:47:17.371242 unray-1.0.3/src/unray.egg-info/
--rw-rw-rw-   0        0        0    10541 2024-05-23 21:47:17.000000 unray-1.0.3/src/unray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2024-05-23 21:47:17.000000 unray-1.0.3/src/unray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 21:47:17.000000 unray-1.0.3/src/unray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-23 21:47:17.000000 unray-1.0.3/src/unray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 21:58:10.734801 unray-1.0.4/
+-rw-rw-rw-   0        0        0     1116 2024-05-23 21:39:25.000000 unray-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0    10541 2024-05-23 21:58:10.728451 unray-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9895 2024-05-23 21:39:25.000000 unray-1.0.4/README.md
+-rw-rw-rw-   0        0        0      751 2024-05-23 21:57:20.000000 unray-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 21:58:10.734801 unray-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 21:58:10.625163 unray-1.0.4/src/
+-rw-rw-rw-   0        0        0       32 2024-05-23 21:39:25.000000 unray-1.0.4/src/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:58:10.637644 unray-1.0.4/src/unray/
+-rw-rw-rw-   0        0        0        2 2024-05-23 21:39:25.000000 unray-1.0.4/src/unray/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:58:10.708573 unray-1.0.4/src/unray/envs/
+-rw-rw-rw-   0        0        0        0 2024-05-23 21:39:25.000000 unray-1.0.4/src/unray/envs/__init__.py
+-rw-rw-rw-   0        0        0     1483 2024-05-23 21:55:41.000000 unray-1.0.4/src/unray/envs/base_env.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:58:10.719834 unray-1.0.4/src/unray/envs/bridge/
+-rw-rw-rw-   0        0        0     5487 2024-05-23 21:39:25.000000 unray-1.0.4/src/unray/envs/bridge/TCP_IP_Connector.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 21:39:25.000000 unray-1.0.4/src/unray/envs/bridge/__init__.py
+-rw-rw-rw-   0        0        0    19422 2024-05-23 21:56:01.000000 unray-1.0.4/src/unray/envs/bridge_env.py
+-rw-rw-rw-   0        0        0      110 2024-05-23 21:39:25.000000 unray-1.0.4/src/unray/envs/spaces.py
+-rw-rw-rw-   0        0        0     1007 2024-05-23 21:39:25.000000 unray-1.0.4/src/unray/gui.py
+-rw-rw-rw-   0        0        0     1370 2024-05-23 21:55:53.000000 unray-1.0.4/src/unray/unray_config.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:58:10.724887 unray-1.0.4/src/unray.egg-info/
+-rw-rw-rw-   0        0        0    10541 2024-05-23 21:58:10.000000 unray-1.0.4/src/unray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-05-23 21:58:10.000000 unray-1.0.4/src/unray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 21:58:10.000000 unray-1.0.4/src/unray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-23 21:58:10.000000 unray-1.0.4/src/unray.egg-info/top_level.txt
```

### Comparing `unray-1.0.3/LICENSE` & `unray-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unray-1.0.3/PKG-INFO` & `unray-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unray
-Version: 1.0.3
+Version: 1.0.4
 Summary: Framework for trainning Reinforcement Learning envs with RLlib and Unreal Eninge 5
 Author-email: Valentina Hernández <vahernandezmo@unal.edu.co>, Andrés Morales <amoralesma@unal.edu.co>
 Project-URL: Homepage, https://github.com/Nullspace-Colombia/unray-bridge/
 Project-URL: Issues, https://github.com/Nullspace-Colombia/unray-bridge/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `unray-1.0.3/README.md` & `unray-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `unray-1.0.3/pyproject.toml` & `unray-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unray"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Valentina Hernández", email="vahernandezmo@unal.edu.co" },
   { name="Andrés Morales", email="amoralesma@unal.edu.co" },
     
 ]
 description = "Framework for trainning Reinforcement Learning envs with RLlib and Unreal Eninge 5"
 readme = "README.md"
```

### Comparing `unray-1.0.3/src/unray/envs/base_env.py` & `unray-1.0.4/src/unray/envs/base_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from src.unray.envs.bridge_env import BridgeEnv
-from src.unray.envs.bridge_env import MultiAgentBridgeEnv
+from unray.envs.bridge_env import BridgeEnv
+from unray.envs.bridge_env import MultiAgentBridgeEnv
 
 class SingleAgentEnv():
     def __init__(self, config, env_name, isTuner = False, ip = 'localhost' , port = 9443, ID=1):
         self.env_ip = ip
         self.env_port = port
         self.env_config = config
         self.name = env_name
```

### Comparing `unray-1.0.3/src/unray/envs/bridge/TCP_IP_Connector.py` & `unray-1.0.4/src/unray/envs/bridge/TCP_IP_Connector.py`

 * *Files identical despite different names*

### Comparing `unray-1.0.3/src/unray/envs/bridge_env.py` & `unray-1.0.4/src/unray/envs/bridge_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     @version: 0.1V
     
     @file bridge_env.py 
 
 """
 from .bridge.TCP_IP_Connector import ClientHandler
-from src.unray.envs.spaces import BridgeSpaces
+from unray.envs.spaces import BridgeSpaces
 from gymnasium import Env as gymEnv
 from ray.rllib.env.multi_agent_env import MultiAgentEnv
 import numpy as np
 from socket import socket
 from src.unray.envs.bridge.TCP_IP_Connector import ClientHandler
 
 class BridgeEnv(gymEnv):
```

### Comparing `unray-1.0.3/src/unray/gui.py` & `unray-1.0.4/src/unray/gui.py`

 * *Files identical despite different names*

### Comparing `unray-1.0.3/src/unray/unray_config.py` & `unray-1.0.4/src/unray/unray_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ray.tune.registry import register_env
-from src.unray.gui import print_title
+from unray.gui import print_title
 
 class UnrayConfig():
     def __init__(self):
         print_title()
         pass
         
     def get_ID(self, worker):
```

### Comparing `unray-1.0.3/src/unray.egg-info/PKG-INFO` & `unray-1.0.4/src/unray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unray
-Version: 1.0.3
+Version: 1.0.4
 Summary: Framework for trainning Reinforcement Learning envs with RLlib and Unreal Eninge 5
 Author-email: Valentina Hernández <vahernandezmo@unal.edu.co>, Andrés Morales <amoralesma@unal.edu.co>
 Project-URL: Homepage, https://github.com/Nullspace-Colombia/unray-bridge/
 Project-URL: Issues, https://github.com/Nullspace-Colombia/unray-bridge/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

