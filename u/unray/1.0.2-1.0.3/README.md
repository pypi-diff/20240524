# Comparing `tmp/unray-1.0.2.tar.gz` & `tmp/unray-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unray-1.0.2.tar", last modified: Thu Feb 22 00:06:25 2024, max compression
+gzip compressed data, was "unray-1.0.3.tar", last modified: Thu May 23 21:47:17 2024, max compression
```

## Comparing `unray-1.0.2.tar` & `unray-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-02-22 00:06:25.962471 unray-1.0.2/
--rw-rw-rw-   0        0        0     1116 2024-02-21 23:50:34.000000 unray-1.0.2/LICENSE
--rw-rw-rw-   0        0        0    10541 2024-02-22 00:06:25.960470 unray-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     9895 2024-02-21 23:50:34.000000 unray-1.0.2/README.md
--rw-rw-rw-   0        0        0      747 2024-02-22 00:06:04.000000 unray-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-22 00:06:25.962471 unray-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-22 00:06:25.928208 unray-1.0.2/src/
--rw-rw-rw-   0        0        0       32 2024-02-21 23:50:34.000000 unray-1.0.2/src/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-22 00:06:25.933213 unray-1.0.2/src/unray/
--rw-rw-rw-   0        0        0        2 2024-02-21 23:50:34.000000 unray-1.0.2/src/unray/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-22 00:06:25.954437 unray-1.0.2/src/unray/envs/
--rw-rw-rw-   0        0        0        0 2024-02-21 23:50:34.000000 unray-1.0.2/src/unray/envs/__init__.py
--rw-rw-rw-   0        0        0     1217 2024-02-22 00:02:47.000000 unray-1.0.2/src/unray/envs/base_env.py
-drwxrwxrwx   0        0        0        0 2024-02-22 00:06:25.957010 unray-1.0.2/src/unray/envs/bridge/
--rw-rw-rw-   0        0        0     5487 2024-02-21 23:50:34.000000 unray-1.0.2/src/unray/envs/bridge/TCP_IP_Connector.py
--rw-rw-rw-   0        0        0        0 2024-02-21 23:50:34.000000 unray-1.0.2/src/unray/envs/bridge/__init__.py
--rw-rw-rw-   0        0        0    19234 2024-02-22 00:04:06.000000 unray-1.0.2/src/unray/envs/bridge_env.py
--rw-rw-rw-   0        0        0      110 2024-02-21 23:50:34.000000 unray-1.0.2/src/unray/envs/spaces.py
--rw-rw-rw-   0        0        0     1007 2024-02-21 23:50:34.000000 unray-1.0.2/src/unray/gui.py
--rw-rw-rw-   0        0        0     1275 2024-02-21 23:53:47.000000 unray-1.0.2/src/unray/unray_config.py
-drwxrwxrwx   0        0        0        0 2024-02-22 00:06:25.958465 unray-1.0.2/src/unray.egg-info/
--rw-rw-rw-   0        0        0    10541 2024-02-22 00:06:25.000000 unray-1.0.2/src/unray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2024-02-22 00:06:25.000000 unray-1.0.2/src/unray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-22 00:06:25.000000 unray-1.0.2/src/unray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-02-22 00:06:25.000000 unray-1.0.2/src/unray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 21:47:17.376823 unray-1.0.3/
+-rw-rw-rw-   0        0        0     1116 2024-05-23 21:39:25.000000 unray-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0    10541 2024-05-23 21:47:17.375247 unray-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9895 2024-05-23 21:39:25.000000 unray-1.0.3/README.md
+-rw-rw-rw-   0        0        0      751 2024-05-23 21:40:01.000000 unray-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 21:47:17.376823 unray-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 21:47:17.316948 unray-1.0.3/src/
+-rw-rw-rw-   0        0        0       32 2024-05-23 21:39:25.000000 unray-1.0.3/src/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:47:17.323265 unray-1.0.3/src/unray/
+-rw-rw-rw-   0        0        0        2 2024-05-23 21:39:25.000000 unray-1.0.3/src/unray/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:47:17.365726 unray-1.0.3/src/unray/envs/
+-rw-rw-rw-   0        0        0        0 2024-05-23 21:39:25.000000 unray-1.0.3/src/unray/envs/__init__.py
+-rw-rw-rw-   0        0        0     1491 2024-05-23 21:39:40.000000 unray-1.0.3/src/unray/envs/base_env.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:47:17.369249 unray-1.0.3/src/unray/envs/bridge/
+-rw-rw-rw-   0        0        0     5487 2024-05-23 21:39:25.000000 unray-1.0.3/src/unray/envs/bridge/TCP_IP_Connector.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 21:39:25.000000 unray-1.0.3/src/unray/envs/bridge/__init__.py
+-rw-rw-rw-   0        0        0    19426 2024-05-23 21:39:40.000000 unray-1.0.3/src/unray/envs/bridge_env.py
+-rw-rw-rw-   0        0        0      110 2024-05-23 21:39:25.000000 unray-1.0.3/src/unray/envs/spaces.py
+-rw-rw-rw-   0        0        0     1007 2024-05-23 21:39:25.000000 unray-1.0.3/src/unray/gui.py
+-rw-rw-rw-   0        0        0     1374 2024-05-23 21:39:40.000000 unray-1.0.3/src/unray/unray_config.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:47:17.371242 unray-1.0.3/src/unray.egg-info/
+-rw-rw-rw-   0        0        0    10541 2024-05-23 21:47:17.000000 unray-1.0.3/src/unray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-05-23 21:47:17.000000 unray-1.0.3/src/unray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 21:47:17.000000 unray-1.0.3/src/unray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-23 21:47:17.000000 unray-1.0.3/src/unray.egg-info/top_level.txt
```

### Comparing `unray-1.0.2/LICENSE` & `unray-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unray-1.0.2/PKG-INFO` & `unray-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: unray
-Version: 1.0.2
+Version: 1.0.3
 Summary: Framework for trainning Reinforcement Learning envs with RLlib and Unreal Eninge 5
-Author-email: Andrés Morales <amoralesma@unal.edu.co>, Valentina Hernández <vahernandezmo@unal.edu.co>
+Author-email: Valentina Hernández <vahernandezmo@unal.edu.co>, Andrés Morales <amoralesma@unal.edu.co>
 Project-URL: Homepage, https://github.com/Nullspace-Colombia/unray-bridge/
 Project-URL: Issues, https://github.com/Nullspace-Colombia/unray-bridge/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unray-1.0.2/README.md` & `unray-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `unray-1.0.2/pyproject.toml` & `unray-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unray"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
+  { name="Valentina Hernández", email="vahernandezmo@unal.edu.co" },
   { name="Andrés Morales", email="amoralesma@unal.edu.co" },
-    { name="Valentina Hernández", email="vahernandezmo@unal.edu.co" },
+    
 ]
 description = "Framework for trainning Reinforcement Learning envs with RLlib and Unreal Eninge 5"
 readme = "README.md"
 requires-python = ">=3.8"
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `unray-1.0.2/src/unray/envs/base_env.py` & `unray-1.0.3/src/unray/envs/base_env.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,51 @@
-from unray.envs.bridge_env import BridgeEnv
-from unray.envs.bridge_env import MultiAgentBridgeEnv
+from src.unray.envs.bridge_env import BridgeEnv
+from src.unray.envs.bridge_env import MultiAgentBridgeEnv
 
 class SingleAgentEnv():
-    def __init__(self, config, env_name, ip = 'localhost' , port = 9443, ID=1):
+    def __init__(self, config, env_name, isTuner = False, ip = 'localhost' , port = 9443, ID=1):
         self.env_ip = ip
         self.env_port = port
         self.env_config = config
         self.name = env_name
         self.ID = ID
+        self.isTuner = isTuner
 
     def get_env(self):
         return lambda config: BridgeEnv(
             name = self.name, 
             ip = self.env_ip,
             port = self.env_port,
             config = self.env_config,
             first_connection = False,
-            ID = self.ID
+            ID = self.ID,
+            isTuner = self.isTuner,
         )
     
     def get_name(self):
         return self.name
 
+    def isTuner(self):
+        return self.isTuner
+    
 class MultiAgentEnv(SingleAgentEnv):
-    def __init__(self, config, env_name, ip='localhost', port=9443, ID = 1):
-        super().__init__(config, env_name, ip, port, ID)
+    def __init__(self, config, env_name, isTuner=False, ip='localhost', port=9443, ID = 1):
+        super().__init__(config, env_name, isTuner, ip, port, ID)
 
     def get_env(self):
         return lambda config: MultiAgentBridgeEnv(
             name = self.name, 
             ip = self.env_ip,
             port = self.env_port,
             config = self.env_config,
             first_connection = False,
             ID = self.ID,
+            isTuner = self.isTuner,
         )
     
     def get_name(self):
         return self.name
+    
+    def isTuner(self):
+        return self.isTuner
```

### Comparing `unray-1.0.2/src/unray/envs/bridge/TCP_IP_Connector.py` & `unray-1.0.3/src/unray/envs/bridge/TCP_IP_Connector.py`

 * *Files identical despite different names*

### Comparing `unray-1.0.2/src/unray/envs/bridge_env.py` & `unray-1.0.3/src/unray/envs/bridge_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 
     @version: 0.1V
     
     @file bridge_env.py 
 
 """
 from .bridge.TCP_IP_Connector import ClientHandler
-from unray.envs.spaces import BridgeSpaces
+from src.unray.envs.spaces import BridgeSpaces
 from gymnasium import Env as gymEnv
 from ray.rllib.env.multi_agent_env import MultiAgentEnv
 import numpy as np
 from socket import socket
-from unray.envs.bridge.TCP_IP_Connector import ClientHandler
+from src.unray.envs.bridge.TCP_IP_Connector import ClientHandler
 
 class BridgeEnv(gymEnv): 
     """
         Base class for custom UE5 Conenction. 
     """
     # 1. Custom gymenv metadata for viz. 
     metadata = {
@@ -44,15 +44,16 @@
                  name, 
                  ip, 
                  port, 
                  config, 
                  first_connection = False, 
                  validation = False, 
                  multiagent = False,
-                 ID = int):
+                 ID = int,
+                 isTuner = False):
                  
         
         self.ip = ip # IP Address for IP Connection 
         self.port = port 
         self.ID = ID
 
         self.client_handler = ClientHandler(ip, port + ID)
@@ -74,14 +75,17 @@
         except: 
             raise ValueError("No correct space selected")
 
         self.obs = self.observation_space.sample()
 
         self.create_handler()
 
+        if isTuner:
+            self.connect_socket()
+
     
     def step(self, action): 
 
         #if not self.has_connection:
         #    self.connect()
 
         action=np.array(action,dtype=np.single)
@@ -307,15 +311,16 @@
                  ip: str, 
                  port: int, 
                  config: dict, 
                  first_connection = False, 
                  validation = False, 
                  multiagent = False, 
                  #Paralell
-                 ID = int):
+                 ID = int,
+                 isTuner = False):
         
         # gui 
         self.ID = ID
         self.client_handler = ClientHandler(ip, port + ID)
 
         # Connection stage 
         ## Worker will wait until de client handler connect to the UE5 instance Socket Server (SS)
@@ -380,14 +385,16 @@
       
 
         self.has_connection = True
         self.has_handler = True
 
         self.obs_dict = self.get_dict_template()
         self.dummy_action = self.get_dict_template()
+        if isTuner:
+            self.connect_socket()
         
 
     def get_amount_agents(self) -> int: 
         """
             Get Amount Agents
             ---
             Returns de amount of agents in the multiagent environment.
```

### Comparing `unray-1.0.2/src/unray/gui.py` & `unray-1.0.3/src/unray/gui.py`

 * *Files identical despite different names*

### Comparing `unray-1.0.2/src/unray/unray_config.py` & `unray-1.0.3/src/unray/unray_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from ray.tune.registry import register_env
-from unray.gui import print_title
+from src.unray.gui import print_title
 
 class UnrayConfig():
     def __init__(self):
         print_title()
         pass
         
     def get_ID(self, worker):
         return worker.env.get_ID()
 
     def set_ID(self, worker):
         ID = worker.worker_index
         worker.env.set_ID(ID)
 
-
     def configure_algo(self, config, env_t):
         
         env_name = env_t.get_name()
         if config.num_rollout_workers > 0:
             num_workers = config.num_rollout_workers
             config.rollouts(num_rollout_workers=0)
         else:
@@ -40,7 +39,10 @@
             
         else:
             print("CONNECTING LOCAL WORKER")
             algo.workers.local_worker().env.connect_socket()
 
         return algo
 
+    def configure_tune(self, env_t):
+        register_env(env_t.get_name(), env_t.get_env())
+
```

### Comparing `unray-1.0.2/src/unray.egg-info/PKG-INFO` & `unray-1.0.3/src/unray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: unray
-Version: 1.0.2
+Version: 1.0.3
 Summary: Framework for trainning Reinforcement Learning envs with RLlib and Unreal Eninge 5
-Author-email: Andrés Morales <amoralesma@unal.edu.co>, Valentina Hernández <vahernandezmo@unal.edu.co>
+Author-email: Valentina Hernández <vahernandezmo@unal.edu.co>, Andrés Morales <amoralesma@unal.edu.co>
 Project-URL: Homepage, https://github.com/Nullspace-Colombia/unray-bridge/
 Project-URL: Issues, https://github.com/Nullspace-Colombia/unray-bridge/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

