# Comparing `tmp/surena-0.1.2.tar.gz` & `tmp/surena-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surena-0.1.2.tar", max compression
+gzip compressed data, was "surena-0.1.3.tar", max compression
```

## Comparing `surena-0.1.2.tar` & `surena-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1079 2024-05-23 09:51:16.801806 surena-0.1.2/LICENSE
--rw-r--r--   0        0        0     3508 2024-05-23 09:51:16.801806 surena-0.1.2/README.md
--rw-r--r--   0        0        0     1801 2024-05-23 09:51:16.801806 surena-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      421 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/__main__.py
--rw-r--r--   0        0        0      122 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/cli/commands/__init__.py
--rw-r--r--   0        0        0      996 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/cli/commands/docker_host.py
--rw-r--r--   0        0        0     6181 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/cli/commands/get_docker_host.py
--rw-r--r--   0        0        0      170 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/cli/options/__init__.py
--rw-r--r--   0        0        0      454 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/cli/options/port.py
--rw-r--r--   0        0        0     1046 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/cli/options/required_if_option_has_specific_value.py
--rw-r--r--   0        0        0       46 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/models/commons/__init__.py
--rw-r--r--   0        0        0      387 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/models/commons/countdown.py
--rw-r--r--   0        0        0      121 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/models/docker_host/__init__.py
--rw-r--r--   0        0        0     4654 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/models/docker_host/docker_host.py
--rw-r--r--   0        0        0      287 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/models/docker_host/ubuntu.Dockerfile
--rw-r--r--   0        0        0      677 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/models/spy_container/WARNING.surena
--rw-r--r--   0        0        0        0 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/models/spy_container/__init__.py
--rw-r--r--   0        0        0     6569 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/models/spy_container/spy_container.py
--rw-r--r--   0        0        0       43 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/models/ssh/__init__.py
--rw-r--r--   0        0        0     1611 2024-05-23 09:51:16.801806 surena-0.1.2/src/surena/models/ssh/client.py
--rw-r--r--   0        0        0     4198 1970-01-01 00:00:00.000000 surena-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-24 10:18:35.655343 surena-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3508 2024-05-24 10:18:35.655343 surena-0.1.3/README.md
+-rw-r--r--   0        0        0     1801 2024-05-24 10:18:35.659344 surena-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      421 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/__main__.py
+-rw-r--r--   0        0        0      122 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/cli/commands/__init__.py
+-rw-r--r--   0        0        0      996 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/cli/commands/docker_host.py
+-rw-r--r--   0        0        0     6181 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/cli/commands/get_docker_host.py
+-rw-r--r--   0        0        0      170 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/cli/options/__init__.py
+-rw-r--r--   0        0        0      454 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/cli/options/port.py
+-rw-r--r--   0        0        0     1046 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/cli/options/required_if_option_has_specific_value.py
+-rw-r--r--   0        0        0       46 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/models/commons/__init__.py
+-rw-r--r--   0        0        0      387 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/models/commons/countdown.py
+-rw-r--r--   0        0        0      121 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/models/docker_host/__init__.py
+-rw-r--r--   0        0        0     4654 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/models/docker_host/docker_host.py
+-rw-r--r--   0        0        0      287 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/models/docker_host/ubuntu.Dockerfile
+-rw-r--r--   0        0        0      677 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/models/spy_container/WARNING.surena
+-rw-r--r--   0        0        0        0 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/models/spy_container/__init__.py
+-rw-r--r--   0        0        0     6569 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/models/spy_container/spy_container.py
+-rw-r--r--   0        0        0       43 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/models/ssh/__init__.py
+-rw-r--r--   0        0        0     1634 2024-05-24 10:18:35.659344 surena-0.1.3/src/surena/models/ssh/client.py
+-rw-r--r--   0        0        0     4198 1970-01-01 00:00:00.000000 surena-0.1.3/PKG-INFO
```

### Comparing `surena-0.1.2/LICENSE` & `surena-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `surena-0.1.2/README.md` & `surena-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `surena-0.1.2/pyproject.toml` & `surena-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surena"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Mohammad Norouzzadegan <Norouzzadegan@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "surena", from = "src" },
 ]
```

### Comparing `surena-0.1.2/src/surena/cli/commands/docker_host.py` & `surena-0.1.3/src/surena/cli/commands/docker_host.py`

 * *Files identical despite different names*

### Comparing `surena-0.1.2/src/surena/cli/commands/get_docker_host.py` & `surena-0.1.3/src/surena/cli/commands/get_docker_host.py`

 * *Files identical despite different names*

### Comparing `surena-0.1.2/src/surena/cli/options/required_if_option_has_specific_value.py` & `surena-0.1.3/src/surena/cli/options/required_if_option_has_specific_value.py`

 * *Files identical despite different names*

### Comparing `surena-0.1.2/src/surena/models/docker_host/docker_host.py` & `surena-0.1.3/src/surena/models/docker_host/docker_host.py`

 * *Files identical despite different names*

### Comparing `surena-0.1.2/src/surena/models/spy_container/WARNING.surena` & `surena-0.1.3/src/surena/models/spy_container/WARNING.surena`

 * *Files identical despite different names*

### Comparing `surena-0.1.2/src/surena/models/spy_container/spy_container.py` & `surena-0.1.3/src/surena/models/spy_container/spy_container.py`

 * *Files identical despite different names*

### Comparing `surena-0.1.2/src/surena/models/ssh/client.py` & `surena-0.1.3/src/surena/models/ssh/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,11 +31,11 @@
                 "to enable support for GatewayPorts in SSH. After that, please restart the SSH "
                 "service on the remote server. Then, please run Surena."
             )
 
     def get_free_port(self) -> int:
         while True:
             free_port = random.randint(35000, 60000)
-            exit_status = self.execute_command(f"lsof -i:{free_port}")
+            exit_status = self.execute_command(f"(lsof -i :{free_port}) && exit 1 || exit 0")
             if exit_status == 0:
                 break
         return free_port
```

### Comparing `surena-0.1.2/PKG-INFO` & `surena-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surena
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Mohammad Norouzzadegan
 Author-email: Norouzzadegan@gmail.com
 Requires-Python: >=3.8.10,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

