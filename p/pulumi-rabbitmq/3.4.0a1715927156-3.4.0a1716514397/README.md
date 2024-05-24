# Comparing `tmp/pulumi_rabbitmq-3.4.0a1715927156.tar.gz` & `tmp/pulumi_rabbitmq-3.4.0a1716514397.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rabbitmq-3.4.0a1715927156.tar", last modified: Fri May 17 06:42:02 2024, max compression
+gzip compressed data, was "pulumi_rabbitmq-3.4.0a1716514397.tar", last modified: Fri May 24 01:39:16 2024, max compression
```

## Comparing `pulumi_rabbitmq-3.4.0a1715927156.tar` & `pulumi_rabbitmq-3.4.0a1716514397.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:42:02.969774 pulumi_rabbitmq-3.4.0a1715927156/
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-17 06:42:02.969774 pulumi_rabbitmq-3.4.0a1715927156/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:42:02.969774 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35649 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    20597 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:42:02.969774 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    11242 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)    15093 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/federation_upstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/get_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/get_v_host.py
--rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/operator_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    32119 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13046 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/shovel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/topic_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/v_host.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:42:02.969774 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-17 06:42:02.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-17 06:42:02.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:42:02.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 06:42:02.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 06:42:02.000000 pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-17 06:41:56.000000 pulumi_rabbitmq-3.4.0a1715927156/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:42:02.969774 pulumi_rabbitmq-3.4.0a1715927156/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:39:16.922335 pulumi_rabbitmq-3.4.0a1716514397/
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-24 01:39:16.922335 pulumi_rabbitmq-3.4.0a1716514397/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:39:16.918335 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35649 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20597 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:39:16.922335 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11242 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15093 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/federation_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/get_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/get_v_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/operator_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32119 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13046 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/shovel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/topic_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/v_host.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:39:16.922335 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-24 01:39:16.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-24 01:39:16.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:39:16.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 01:39:16.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 01:39:16.000000 pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-24 01:39:10.000000 pulumi_rabbitmq-3.4.0a1716514397/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 01:39:16.922335 pulumi_rabbitmq-3.4.0a1716514397/setup.cfg
```

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/PKG-INFO` & `pulumi_rabbitmq-3.4.0a1716514397/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rabbitmq
-Version: 3.4.0a1715927156
+Version: 3.4.0a1716514397
 Summary: A Pulumi package for creating and managing RabbitMQ resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rabbitmq
 Keywords: pulumi,rabbitmq
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/README.md` & `pulumi_rabbitmq-3.4.0a1716514397/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/__init__.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/_inputs.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/_utilities.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/binding.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/config/__init__.pyi` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/config/vars.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/exchange.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/exchange.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/federation_upstream.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/federation_upstream.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/get_exchange.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/get_exchange.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/get_user.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/get_v_host.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/get_v_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/operator_policy.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/operator_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/outputs.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/permissions.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/policy.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/provider.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/queue.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/shovel.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/shovel.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/topic_permissions.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/topic_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/user.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq/v_host.py` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq/v_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq.egg-info/PKG-INFO` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rabbitmq
-Version: 3.4.0a1715927156
+Version: 3.4.0a1716514397
 Summary: A Pulumi package for creating and managing RabbitMQ resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rabbitmq
 Keywords: pulumi,rabbitmq
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pulumi_rabbitmq.egg-info/SOURCES.txt` & `pulumi_rabbitmq-3.4.0a1716514397/pulumi_rabbitmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1715927156/pyproject.toml` & `pulumi_rabbitmq-3.4.0a1716514397/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_rabbitmq"
   description = "A Pulumi package for creating and managing RabbitMQ resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "rabbitmq"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.4.0a1715927156"
+  version = "3.4.0a1716514397"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-rabbitmq"
 
 [build-system]
```

