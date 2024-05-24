# Comparing `tmp/pypods-0.1.3.tar.gz` & `tmp/pypods-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypods-0.1.3.tar", last modified: Thu May 23 06:36:44 2024, max compression
+gzip compressed data, was "pypods-0.2.0.tar", last modified: Fri May 24 21:24:51 2024, max compression
```

## Comparing `pypods-0.1.3.tar` & `pypods-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-23 06:36:44.890968 pypods-0.1.3/
--rw-r--r--   0 rohandeshpande   (501) staff       (20)     1058 2024-05-19 02:45:24.000000 pypods-0.1.3/LICENSE
--rw-r--r--   0 rohandeshpande   (501) staff       (20)     4719 2024-05-23 06:36:44.890846 pypods-0.1.3/PKG-INFO
--rw-r--r--   0 rohandeshpande   (501) staff       (20)     4200 2024-05-23 06:34:05.000000 pypods-0.1.3/README.md
-drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-23 06:36:44.889803 pypods-0.1.3/pypods/
--rw-r--r--   0 rohandeshpande   (501) staff       (20)       53 2024-05-23 06:35:55.000000 pypods-0.1.3/pypods/__init__.py
--rw-r--r--   0 rohandeshpande   (501) staff       (20)      414 2024-05-20 17:24:37.000000 pypods-0.1.3/pypods/errors.py
--rw-r--r--   0 rohandeshpande   (501) staff       (20)     1624 2024-05-20 20:52:13.000000 pypods-0.1.3/pypods/ns.py
--rw-r--r--   0 rohandeshpande   (501) staff       (20)     8193 2024-05-23 05:39:22.000000 pypods-0.1.3/pypods/pods.py
-drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-23 06:36:44.890668 pypods-0.1.3/pypods/template/
--rw-r--r--   0 rohandeshpande   (501) staff       (20)     1386 2024-05-20 20:56:47.000000 pypods-0.1.3/pypods/template/pod.py
-drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-23 06:36:44.890529 pypods-0.1.3/pypods.egg-info/
--rw-r--r--   0 rohandeshpande   (501) staff       (20)     4719 2024-05-23 06:36:44.000000 pypods-0.1.3/pypods.egg-info/PKG-INFO
--rw-r--r--   0 rohandeshpande   (501) staff       (20)      262 2024-05-23 06:36:44.000000 pypods-0.1.3/pypods.egg-info/SOURCES.txt
--rw-r--r--   0 rohandeshpande   (501) staff       (20)        1 2024-05-23 06:36:44.000000 pypods-0.1.3/pypods.egg-info/dependency_links.txt
--rw-r--r--   0 rohandeshpande   (501) staff       (20)        5 2024-05-23 06:36:44.000000 pypods-0.1.3/pypods.egg-info/requires.txt
--rw-r--r--   0 rohandeshpande   (501) staff       (20)        7 2024-05-23 06:36:44.000000 pypods-0.1.3/pypods.egg-info/top_level.txt
--rw-r--r--   0 rohandeshpande   (501) staff       (20)       38 2024-05-23 06:36:44.891017 pypods-0.1.3/setup.cfg
--rw-r--r--   0 rohandeshpande   (501) staff       (20)      823 2024-05-23 06:25:43.000000 pypods-0.1.3/setup.py
+drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-24 21:24:51.007037 pypods-0.2.0/
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     1058 2024-05-19 02:45:24.000000 pypods-0.2.0/LICENSE
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     7708 2024-05-24 21:24:51.006901 pypods-0.2.0/PKG-INFO
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     7189 2024-05-24 19:37:20.000000 pypods-0.2.0/README.md
+drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-24 21:24:51.005545 pypods-0.2.0/pypods/
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)       53 2024-05-24 21:24:32.000000 pypods-0.2.0/pypods/__init__.py
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)      414 2024-05-24 21:23:49.000000 pypods-0.2.0/pypods/errors.py
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     1624 2024-05-24 15:18:55.000000 pypods-0.2.0/pypods/ns.py
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     8816 2024-05-24 21:21:41.000000 pypods-0.2.0/pypods/pods.py
+drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-24 21:24:51.006457 pypods-0.2.0/pypods/template/
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     1386 2024-05-20 20:56:47.000000 pypods-0.2.0/pypods/template/pod.py
+drwxr-xr-x   0 rohandeshpande   (501) staff       (20)        0 2024-05-24 21:24:51.006306 pypods-0.2.0/pypods.egg-info/
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)     7708 2024-05-24 21:24:50.000000 pypods-0.2.0/pypods.egg-info/PKG-INFO
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)      262 2024-05-24 21:24:50.000000 pypods-0.2.0/pypods.egg-info/SOURCES.txt
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)        1 2024-05-24 21:24:50.000000 pypods-0.2.0/pypods.egg-info/dependency_links.txt
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)        5 2024-05-24 21:24:50.000000 pypods-0.2.0/pypods.egg-info/requires.txt
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)        7 2024-05-24 21:24:50.000000 pypods-0.2.0/pypods.egg-info/top_level.txt
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)       38 2024-05-24 21:24:51.007095 pypods-0.2.0/setup.cfg
+-rw-r--r--   0 rohandeshpande   (501) staff       (20)      823 2024-05-23 06:25:43.000000 pypods-0.2.0/setup.py
```

### Comparing `pypods-0.1.3/LICENSE` & `pypods-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypods-0.1.3/pypods/ns.py` & `pypods-0.2.0/pypods/ns.py`

 * *Files identical despite different names*

### Comparing `pypods-0.1.3/pypods/pods.py` & `pypods-0.2.0/pypods/pods.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,29 @@
 
 from pypods.ns import *
 from pypods.errors import PyPodNotStartedError, PyPodResponseError
 
 from bson import dumps, loads
 
 VENV_BIN = "Scripts" if os.name == 'nt' else "bin"
+
+class Object(object):
+    """
+        The pod_name attribute in PodLoader will be assigned Object() in the client's namespace
+        so that we can add attributes to the pod_name. Why we need attributes?
+
+        Let's say the pod_name is hello_world and hello_world has a function foo.
+        
+        If a client loads the hello_world pod then the client can call hello_world.foo() rather
+        than just foo().
+
+        The intention of this approach is to scope the pod's functions using the pod as a wrapper. 
+        Scoping will avoid polluting the client's namespace with similar function names but from different pods.
+    """
+    pass
 class PodLoader:
     """
     This class is for managing the lifecycle and interactions of a client with a specific pod.
     It loads and unloads pod functions into a namespace, sends data to the pod for processing,
     and handles responses and errors.
     """
 
@@ -32,17 +47,14 @@
 
         Args:
             pod_name (str): The name of the pod associated with this loader.
             namespace (dict): The namespace dictionary where pod functions are loaded.
         """
         self.pod_name = pod_name
         self.namespace = namespace
-        self.loaded_functions = []
-        self.create_pod()
-
     def create_pod(self) -> None:
         """
         Create a new pod by setting up the necessary directory structure and dependencies.
         """
         # All pods are stored inside PODS_DIRECTORY
         # Create PODS_DIRECTORY if not exist and pod_name directory if not exist.
         pod_path = join(PODS_DIRECTORY, self.pod_name)
@@ -92,28 +104,30 @@
                 ]
             )
 
     def load_pod(self) -> None:
         """
         Load functions from the pod into the client's namespace.
         """
+        if not str.isidentifier(self.pod_name):
+            raise ValueError(f"pod_name: {self.pod_name} should be a valid python identifier")
+        self.create_pod()
+        self.namespace[self.pod_name] = Object()
+
         pod_ns = get_pod_namespace(self.pod_name)
         for function_name in pod_ns:
             args, kwargs = pod_ns[function_name]
-            pod_function_name = self.create_a_function(function_name, *args, **kwargs)
-            self.loaded_functions.append(pod_function_name)
+            self.create_a_function(function_name, *args, **kwargs)
 
     def unload_pod(self) -> None:
         """
-        Unload functions loaded from the pod from the client's namespace.
+        Unload pod object from the client's namespace.
         """
-        for loaded_function in self.loaded_functions:
-            if loaded_function not in self.namespace:
-                continue
-            del self.namespace[loaded_function]
+        if self.pod_name in self.namespace:
+            del self.namespace[self.pod_name]
 
     def send_data(self, data: bytes) -> None:
         """
         Send data to the pod for processing and handle the response.
 
         Args:
             data (bytes): The data to be sent to the pod.
@@ -161,17 +175,15 @@
                     raise PyPodResponseError(error)
                 function_output = loads(stdout)["response"]
             except PyPodResponseError as e:
                 raise PyPodResponseError(f"PyPodResponseError: {e}")
             except Exception as e:
                 raise Exception(f"Unknown error: {e}")
             return function_output
-
-        self.namespace[func_name] = rpc_proxy_function
-        return func_name
+        self.namespace[self.pod_name].__setattr__(func_name, rpc_proxy_function)
 
 
 class PodListener:
     """
     The PodListener class provides functionalities to interact with standard input and
     output streams, specifically tailored for handling serialized data in a structured format. It
     can read from stdin, write to stdout, and log errors to stderr, all using BSON serialization.
@@ -192,15 +204,15 @@
             data = sys.stdin.buffer.read()
             func_param = loads(data)
             if not isinstance(func_param, dict) or not {
                 "name",
                 "args",
                 "kwargs",
             }.issubset(func_param):
-                raise ValueError("Corrupt pod input!")
+                raise Exception("Corrupt pod input!")
         except Exception as e:
             func_param = None
             self.write_stderr(str(e))
         return func_param
 
     def write_stdout(self, data: Any) -> None:
         """
@@ -222,8 +234,8 @@
 
         Args:
             error (str): Error message to be serialized and written.
         """
         if not isinstance(error, str):
             raise TypeError("Error message should be of type string.")
         sys.stderr.buffer.write(dumps({"error": error}))
-        sys.stderr.flush()
+        sys.stderr.buffer.flush()
```

### Comparing `pypods-0.1.3/pypods/template/pod.py` & `pypods-0.2.0/pypods/template/pod.py`

 * *Files identical despite different names*

### Comparing `pypods-0.1.3/setup.py` & `pypods-0.2.0/setup.py`

 * *Files identical despite different names*

