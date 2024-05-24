# Comparing `tmp/autoutils-0.9.1.tar.gz` & `tmp/autoutils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoutils-0.9.1.tar", max compression
+gzip compressed data, was "autoutils-1.0.0.tar", max compression
```

## Comparing `autoutils-0.9.1.tar` & `autoutils-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-07-25 01:56:35.774830 autoutils-0.9.1/LICENSE
--rw-r--r--   0        0        0       11 2023-07-25 01:56:35.774830 autoutils-0.9.1/README.md
--rw-r--r--   0        0        0        0 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/__init__.py
--rw-r--r--   0        0        0     3081 2024-02-05 11:39:08.521097 autoutils-0.9.1/autoutils/api.py
--rw-r--r--   0        0        0     8739 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/color.py
--rw-r--r--   0        0        0     3411 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/file.py
--rw-r--r--   0        0        0    20748 2023-11-13 09:24:49.207147 autoutils-0.9.1/autoutils/log.py
--rw-r--r--   0        0        0        0 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/matrixcli/__init__.py
--rw-r--r--   0        0        0    35272 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/matrixcli/api.py
--rw-r--r--   0        0        0     7437 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/matrixcli/client.py
--rw-r--r--   0        0        0     1765 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/matrixcli/errors.py
--rw-r--r--   0        0        0    24836 2023-07-25 01:56:35.778830 autoutils-0.9.1/autoutils/matrixcli/room.py
--rw-r--r--   0        0        0     1509 2023-07-25 01:56:35.778830 autoutils-0.9.1/autoutils/matrixcli/user.py
--rw-r--r--   0        0        0     3253 2023-07-25 01:56:35.778830 autoutils-0.9.1/autoutils/redis.py
--rw-r--r--   0        0        0     4243 2023-07-25 01:56:35.778830 autoutils-0.9.1/autoutils/script.py
--rw-r--r--   0        0        0    12052 2023-11-25 06:17:00.273785 autoutils-0.9.1/autoutils/server.py
--rw-r--r--   0        0        0     6437 2023-07-25 01:56:35.778830 autoutils-0.9.1/autoutils/thread.py
--rw-r--r--   0        0        0      808 2024-02-05 11:06:58.808667 autoutils-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 autoutils-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-24 09:51:08.459971 autoutils-1.0.0/LICENSE
+-rw-r--r--   0        0        0       11 2024-05-24 09:51:08.459971 autoutils-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 09:51:08.460971 autoutils-1.0.0/autoutils/__init__.py
+-rw-r--r--   0        0        0     3281 2024-05-24 10:52:59.841928 autoutils-1.0.0/autoutils/api.py
+-rw-r--r--   0        0        0     3411 2024-05-24 10:55:16.337935 autoutils-1.0.0/autoutils/file.py
+-rw-r--r--   0        0        0     4243 2024-05-24 09:51:08.464971 autoutils-1.0.0/autoutils/script.py
+-rw-r--r--   0        0        0     6437 2024-05-24 09:51:08.465971 autoutils-1.0.0/autoutils/thread.py
+-rw-r--r--   0        0        0      656 2024-05-24 21:11:40.972749 autoutils-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 autoutils-1.0.0/PKG-INFO
```

### Comparing `autoutils-0.9.1/LICENSE` & `autoutils-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.1/autoutils/api.py` & `autoutils-1.0.0/autoutils/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,63 +19,69 @@
 
     def __post_init__(self):
         if self.response is not None:
             self.status_code = self.response.status_code
 
     @property
     def json_response(self) -> Optional[Union[List, Dict]]:
-        if not self.response:
+        if self.response is None:
             return None
         try:
             return self.response.json()
         except json.JSONDecodeError:
             pass
 
 
 @dataclasses.dataclass
 class BaseApi:
     name: str
     base_url: str
-    token: str
     connection_timeout: int = 60
     validate_cert: bool = True
     user_agent: str = "autoutils"
     retry_count: int = 1
     retry_delay: int = 3
     token_name: str = "Bearer"
     supported_http_methods: List[str] = None
+    token: str = None
     proxies: dict = None
+    username: str = None
+    password: str = None
 
     def __post_init__(self):
         if not self.supported_http_methods:
             self.supported_http_methods = ["GET", "PUT", "DELETE", "POST", "PATCH"]
         self.session = Session()
 
-    def _send(self, method: str, path: str, content: dict = None, files=None,
-              query_params: dict = None, is_json=True):
+    def send(self, method: str, path: str, content: dict = None, files=None,
+             query_params: dict = None, is_json=True):
         method = method.upper()
         if method not in self.supported_http_methods:
             raise Exception(f"Unsupported HTTP method: {method}")
         if query_params is None:
             query_params = {}
         headers = {
             "User-Agent": self.user_agent,
-            "Authorization": f"{self.token_name} {self.token}"
         }
+        if self.token:
+            headers["Authorization"] = f"{self.token_name} {self.token}"
+
         endpoint = self.base_url + path
         logger.info(f"{self.name} api: method {method} with url {endpoint} start")
         if is_json:
             send_data = {
                 "json": content
             }
         else:
             send_data = {
                 "data": content,
                 "files": files
             }
+        if self.username and self.password:
+            send_data["auth"] = (self.username, self.password)
         retry_count = 0
         while retry_count < self.retry_count:
             try:
                 response = self.session.request(
                     method, endpoint,
                     params=query_params,
                     headers=headers,
```

### Comparing `autoutils-0.9.1/autoutils/file.py` & `autoutils-1.0.0/autoutils/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     Returns:
         (bool) : job state
     """
     if address is None:
         return False
 
-    if type(data) == str and file_mode in [FileModes.APPEND, FileModes.NORMAL]:
+    if type(data) is str and file_mode in [FileModes.APPEND, FileModes.NORMAL]:
         data = [data]
 
     mode = "w"
     if file_mode == FileModes.APPEND:
         mode = "a+"
     elif file_mode in [FileModes.OBJECT, FileModes.FILE]:
         mode = "wb"
```

### Comparing `autoutils-0.9.1/autoutils/script.py` & `autoutils-1.0.0/autoutils/script.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.1/autoutils/thread.py` & `autoutils-1.0.0/autoutils/thread.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.1/pyproject.toml` & `autoutils-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoutils"
-version = "0.9.1"
+version = "1.0.0"
 description = "Some Good Function"
 authors = ["Reza Zeiny <rezazeiny1998@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rezazeiny/autoutils"
 repository = "https://github.com/rezazeiny/autoutils"
 keywords = ["autoutils"]
@@ -15,23 +15,15 @@
 ]
 include = [
     "LICENSE",
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.6"
-persiantools = "~=2.0"
-redis = "^4.0"
+python = "~=3.12"
 requests = "^2.0"
-urllib3 = "^1.0"
-sshtunnel = "~=0.1"
-paramiko = "^2.0"
 func-timeout = "^4.0"
-blessings = "^1.0"
-pytz = "~=2022.1"
-kafka-python = "^2.0.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

