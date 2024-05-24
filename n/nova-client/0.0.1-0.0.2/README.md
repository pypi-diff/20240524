# Comparing `tmp/nova_client-0.0.1.tar.gz` & `tmp/nova_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nova_client-0.0.1.tar", last modified: Fri May 24 17:00:52 2024, max compression
+gzip compressed data, was "nova_client-0.0.2.tar", last modified: Fri May 24 17:07:41 2024, max compression
```

## Comparing `nova_client-0.0.1.tar` & `nova_client-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 palle      (501) staff       (20)        0 2024-05-24 17:00:52.955167 nova_client-0.0.1/
--rw-r--r--   0 palle      (501) staff       (20)        0 2023-10-06 15:42:52.000000 nova_client-0.0.1/.flake8
--rw-r--r--   0 palle      (501) staff       (20)       76 2024-05-09 15:20:25.000000 nova_client-0.0.1/.gitignore
--rw-r--r--   0 palle      (501) staff       (20)     1443 2024-04-12 16:34:38.000000 nova_client-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 palle      (501) staff       (20)     1085 2024-05-24 16:59:59.000000 nova_client-0.0.1/LICENSE
--rw-r--r--   0 palle      (501) staff       (20)     2127 2024-05-24 17:00:52.954910 nova_client-0.0.1/PKG-INFO
--rw-r--r--   0 palle      (501) staff       (20)     1294 2024-05-24 16:58:07.000000 nova_client-0.0.1/README.md
--rw-r--r--   0 palle      (501) staff       (20)     1137 2024-05-09 14:09:15.000000 nova_client-0.0.1/pyproject.toml
--rw-r--r--   0 palle      (501) staff       (20)       38 2024-05-24 17:00:52.955211 nova_client-0.0.1/setup.cfg
-drwxr-xr-x   0 palle      (501) staff       (20)        0 2024-05-24 17:00:52.950135 nova_client-0.0.1/src/
-drwxr-xr-x   0 palle      (501) staff       (20)        0 2024-05-24 17:00:52.952410 nova_client-0.0.1/src/nova_client/
--rw-r--r--   0 palle      (501) staff       (20)      130 2024-05-24 16:58:37.000000 nova_client-0.0.1/src/nova_client/__init__.py
--rw-r--r--   0 palle      (501) staff       (20)     4996 2024-05-24 13:02:49.000000 nova_client-0.0.1/src/nova_client/adapter.py
--rw-r--r--   0 palle      (501) staff       (20)     5027 2024-05-24 12:48:39.000000 nova_client-0.0.1/src/nova_client/chat_session_client.py
--rw-r--r--   0 palle      (501) staff       (20)      415 2024-05-09 15:17:52.000000 nova_client-0.0.1/src/nova_client/client.py
-drwxr-xr-x   0 palle      (501) staff       (20)        0 2024-05-24 17:00:52.953585 nova_client-0.0.1/src/nova_client/models/
--rw-r--r--   0 palle      (501) staff       (20)        0 2024-05-09 15:07:51.000000 nova_client-0.0.1/src/nova_client/models/__init__.py
--rw-r--r--   0 palle      (501) staff       (20)     1546 2024-05-09 15:09:09.000000 nova_client-0.0.1/src/nova_client/models/requests.py
--rw-r--r--   0 palle      (501) staff       (20)     2402 2024-05-24 16:54:30.000000 nova_client-0.0.1/src/nova_client/models/responses.py
-drwxr-xr-x   0 palle      (501) staff       (20)        0 2024-05-24 17:00:52.953912 nova_client-0.0.1/src/nova_client.egg-info/
--rw-r--r--   0 palle      (501) staff       (20)     2127 2024-05-24 17:00:52.000000 nova_client-0.0.1/src/nova_client.egg-info/PKG-INFO
--rw-r--r--   0 palle      (501) staff       (20)      495 2024-05-24 17:00:52.000000 nova_client-0.0.1/src/nova_client.egg-info/SOURCES.txt
--rw-r--r--   0 palle      (501) staff       (20)        1 2024-05-24 17:00:52.000000 nova_client-0.0.1/src/nova_client.egg-info/dependency_links.txt
--rw-r--r--   0 palle      (501) staff       (20)      256 2024-05-24 17:00:52.000000 nova_client-0.0.1/src/nova_client.egg-info/requires.txt
--rw-r--r--   0 palle      (501) staff       (20)       12 2024-05-24 17:00:52.000000 nova_client-0.0.1/src/nova_client.egg-info/top_level.txt
+drwxr-xr-x   0 palle      (501) staff       (20)        0 2024-05-24 17:07:41.368631 nova_client-0.0.2/
+-rw-r--r--   0 palle      (501) staff       (20)        0 2023-10-06 15:42:52.000000 nova_client-0.0.2/.flake8
+-rw-r--r--   0 palle      (501) staff       (20)       76 2024-05-09 15:20:25.000000 nova_client-0.0.2/.gitignore
+-rw-r--r--   0 palle      (501) staff       (20)     1443 2024-04-12 16:34:38.000000 nova_client-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 palle      (501) staff       (20)     1085 2024-05-24 16:59:59.000000 nova_client-0.0.2/LICENSE
+-rw-r--r--   0 palle      (501) staff       (20)     2127 2024-05-24 17:07:41.368359 nova_client-0.0.2/PKG-INFO
+-rw-r--r--   0 palle      (501) staff       (20)     1294 2024-05-24 16:58:07.000000 nova_client-0.0.2/README.md
+-rw-r--r--   0 palle      (501) staff       (20)     1137 2024-05-24 17:06:51.000000 nova_client-0.0.2/pyproject.toml
+-rw-r--r--   0 palle      (501) staff       (20)       38 2024-05-24 17:07:41.368672 nova_client-0.0.2/setup.cfg
+drwxr-xr-x   0 palle      (501) staff       (20)        0 2024-05-24 17:07:41.363256 nova_client-0.0.2/src/
+drwxr-xr-x   0 palle      (501) staff       (20)        0 2024-05-24 17:07:41.365598 nova_client-0.0.2/src/nova_client/
+-rw-r--r--   0 palle      (501) staff       (20)      130 2024-05-24 17:06:56.000000 nova_client-0.0.2/src/nova_client/__init__.py
+-rw-r--r--   0 palle      (501) staff       (20)     4996 2024-05-24 13:02:49.000000 nova_client-0.0.2/src/nova_client/adapter.py
+-rw-r--r--   0 palle      (501) staff       (20)     5027 2024-05-24 12:48:39.000000 nova_client-0.0.2/src/nova_client/chat_session_client.py
+-rw-r--r--   0 palle      (501) staff       (20)      415 2024-05-09 15:17:52.000000 nova_client-0.0.2/src/nova_client/client.py
+drwxr-xr-x   0 palle      (501) staff       (20)        0 2024-05-24 17:07:41.367051 nova_client-0.0.2/src/nova_client/models/
+-rw-r--r--   0 palle      (501) staff       (20)        0 2024-05-09 15:07:51.000000 nova_client-0.0.2/src/nova_client/models/__init__.py
+-rw-r--r--   0 palle      (501) staff       (20)     1546 2024-05-09 15:09:09.000000 nova_client-0.0.2/src/nova_client/models/requests.py
+-rw-r--r--   0 palle      (501) staff       (20)     2402 2024-05-24 16:54:30.000000 nova_client-0.0.2/src/nova_client/models/responses.py
+drwxr-xr-x   0 palle      (501) staff       (20)        0 2024-05-24 17:07:41.367361 nova_client-0.0.2/src/nova_client.egg-info/
+-rw-r--r--   0 palle      (501) staff       (20)     2127 2024-05-24 17:07:41.000000 nova_client-0.0.2/src/nova_client.egg-info/PKG-INFO
+-rw-r--r--   0 palle      (501) staff       (20)      495 2024-05-24 17:07:41.000000 nova_client-0.0.2/src/nova_client.egg-info/SOURCES.txt
+-rw-r--r--   0 palle      (501) staff       (20)        1 2024-05-24 17:07:41.000000 nova_client-0.0.2/src/nova_client.egg-info/dependency_links.txt
+-rw-r--r--   0 palle      (501) staff       (20)      256 2024-05-24 17:07:41.000000 nova_client-0.0.2/src/nova_client.egg-info/requires.txt
+-rw-r--r--   0 palle      (501) staff       (20)       12 2024-05-24 17:07:41.000000 nova_client-0.0.2/src/nova_client.egg-info/top_level.txt
```

### Comparing `nova_client-0.0.1/.pre-commit-config.yaml` & `nova_client-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nova_client-0.0.1/LICENSE` & `nova_client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nova_client-0.0.1/PKG-INFO` & `nova_client-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nova-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: NOVA Machine to Machine Client
 Author-email: Serapion GmbH <dev@serapion.net>
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic<3.0.0,>=2.0.0
 Requires-Dist: aiohttp<4.0.0,>=3.8.5
 Provides-Extra: dev
 Requires-Dist: pytest<8.0.0,>=7.4.2; extra == "dev"
 Requires-Dist: pytest-asyncio<1.0.0,>=0.21.0; extra == "dev"
```

### Comparing `nova_client-0.0.1/README.md` & `nova_client-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nova_client-0.0.1/pyproject.toml` & `nova_client-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "nova-client"
 authors = [
     {name = "Serapion GmbH", email = "dev@serapion.net"},
 ]
 description = "NOVA Machine to Machine Client"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["version"]
 dependencies = [
     "pydantic>=2.0.0,<3.0.0",
     "aiohttp>=3.8.5,<4.0.0",
```

### Comparing `nova_client-0.0.1/src/nova_client/adapter.py` & `nova_client-0.0.2/src/nova_client/adapter.py`

 * *Files identical despite different names*

### Comparing `nova_client-0.0.1/src/nova_client/chat_session_client.py` & `nova_client-0.0.2/src/nova_client/chat_session_client.py`

 * *Files identical despite different names*

### Comparing `nova_client-0.0.1/src/nova_client/models/requests.py` & `nova_client-0.0.2/src/nova_client/models/requests.py`

 * *Files identical despite different names*

### Comparing `nova_client-0.0.1/src/nova_client/models/responses.py` & `nova_client-0.0.2/src/nova_client/models/responses.py`

 * *Files identical despite different names*

### Comparing `nova_client-0.0.1/src/nova_client.egg-info/PKG-INFO` & `nova_client-0.0.2/src/nova_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nova-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: NOVA Machine to Machine Client
 Author-email: Serapion GmbH <dev@serapion.net>
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic<3.0.0,>=2.0.0
 Requires-Dist: aiohttp<4.0.0,>=3.8.5
 Provides-Extra: dev
 Requires-Dist: pytest<8.0.0,>=7.4.2; extra == "dev"
 Requires-Dist: pytest-asyncio<1.0.0,>=0.21.0; extra == "dev"
```

