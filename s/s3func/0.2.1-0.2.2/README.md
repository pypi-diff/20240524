# Comparing `tmp/s3func-0.2.1.tar.gz` & `tmp/s3func-0.2.2.tar.gz`

## Comparing `s3func-0.2.1.tar` & `s3func-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 s3func-0.2.1/s3func/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 s3func-0.2.1/s3func/b2.py
--rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 s3func-0.2.1/s3func/http_url.py
--rw-r--r--   0        0        0    24660 2020-02-02 00:00:00.000000 s3func-0.2.1/s3func/s3.py
--rw-r--r--   0        0        0    12801 2020-02-02 00:00:00.000000 s3func-0.2.1/s3func/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 s3func-0.2.1/s3func/tests/__init__.py
--rw-r--r--   0        0        0   285095 2020-02-02 00:00:00.000000 s3func-0.2.1/s3func/tests/stns_data.blt
--rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 s3func-0.2.1/s3func/tests/test_s3func.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 s3func-0.2.1/.gitignore
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 s3func-0.2.1/LICENSE
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 s3func-0.2.1/README.md
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 s3func-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 s3func-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 s3func-0.2.2/s3func/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 s3func-0.2.2/s3func/b2.py
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 s3func-0.2.2/s3func/http_url.py
+-rw-r--r--   0        0        0    24851 2020-02-02 00:00:00.000000 s3func-0.2.2/s3func/s3.py
+-rw-r--r--   0        0        0    12801 2020-02-02 00:00:00.000000 s3func-0.2.2/s3func/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 s3func-0.2.2/s3func/tests/__init__.py
+-rw-r--r--   0        0        0    30884 2020-02-02 00:00:00.000000 s3func-0.2.2/s3func/tests/put_object_timings.csv
+-rw-r--r--   0        0        0   285095 2020-02-02 00:00:00.000000 s3func-0.2.2/s3func/tests/stns_data.blt
+-rw-r--r--   0        0        0     9168 2020-02-02 00:00:00.000000 s3func-0.2.2/s3func/tests/test_s3func.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 s3func-0.2.2/.gitignore
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 s3func-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 s3func-0.2.2/README.md
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 s3func-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 s3func-0.2.2/PKG-INFO
```

### Comparing `s3func-0.2.1/s3func/b2.py` & `s3func-0.2.2/s3func/b2.py`

 * *Files identical despite different names*

### Comparing `s3func-0.2.1/s3func/http_url.py` & `s3func-0.2.2/s3func/http_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # import requests
 import urllib.parse
 from urllib3.util import Retry, Timeout
 # from requests import Session
 # from requests.adapters import HTTPAdapter
 import urllib3
 
-from . import utils
-# import utils
+# from . import utils
+import utils
 
 #######################################################
 ### Parameters
 
 
 
 ##################################################
```

### Comparing `s3func-0.2.1/s3func/s3.py` & `s3func-0.2.2/s3func/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 from time import sleep
 from timeit import default_timer
 import datetime
 
 # from . import http_url
 # import http_url
 
-from . import utils
-# import utils
+# from . import utils
+import utils
 
 #######################################################
 ### Parameters
 
 
 md5_locks = {
     'shared': 'cfcd208495d565ef66e7dff9f98764da',
@@ -534,42 +534,46 @@
 
         """
         _ = delete_object(self._s3_client, self._bucket, self._obj_lock_key, self._version_id)
         self._version_id = ''
         self._last_modified = None
 
 
-    def _put_object(self, body):
+    def _put_lock_object(self, body):
         """
 
         """
         counter = 0
         while True:
             counter += 1
             start_time = datetime.datetime.now(datetime.timezone.utc)
             resp = put_object(self._s3_client, self._bucket, self._obj_lock_key, body)
+            return_time = datetime.datetime.now(datetime.timezone.utc)
             if resp.status != 200:
                 raise urllib3.exceptions.HTTPError(str(resp.error)[1:-1])
             # header_time = datetime.datetime.strptime(resp.headers['ResponseMetadata']['HTTPHeaders']['date'], '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc)
-            # to_header_time = (header_time - start_time).total_seconds()
-            mod_time = resp.metadata['last_modified']
-            to_mod_time = (mod_time - start_time).total_seconds()
+            # total_time = (header_time - start_time).total_seconds()
+            # mod_time = resp.metadata['last_modified']
+            # total_time = (mod_time - start_time).total_seconds()
+            total_time = (return_time - start_time).total_seconds()
+            # print(total_time)
 
-            if to_mod_time < 2.5:
-                diff_time = 2.5 - to_mod_time
+            self._version_id = resp.metadata['version_id']
+            self._last_modified = resp.metadata['last_modified']
+
+            if total_time <= 3:
+                diff_time = 3 - total_time
                 sleep(diff_time)
                 break
             else:
+                # print(counter)
                 self._delete_lock_object()
                 if counter == 5:
                     raise urllib3.exceptions.HTTPError('put_object takes too long to complete.')
 
-        self._version_id = resp.metadata['version_id']
-        self._last_modified = resp.metadata['last_modified']
-
 
     def other_locks(self):
         """
         Method to list all of the other locks that might also be on the object.
 
         Returns
         -------
@@ -601,15 +605,15 @@
             delete_objects(self._s3_client, self._bucket, obj_keys)
 
         return obj_keys
 
 
     def locked(self):
         """
-        Checks to see if there's a lock on the object. 
+        Checks to see if there's a lock on the object.
 
         Returns
         -------
         bool
         """
         objs = self._list_object_versions(self._s3_client, self._bucket, self._obj_lock_key)
         if objs:
@@ -619,33 +623,33 @@
 
 
     def aquire(self, blocking=True, timeout=-1, exclusive=True):
         """
         Acquire a lock, blocking or non-blocking.
 
         When invoked with the blocking argument set to True (the default), block until the lock is unlocked, then set it to locked and return True.
-        
+
         When invoked with the blocking argument set to False, do not block. If a call with blocking set to True would block, return False immediately; otherwise, set the lock to locked and return True.
-        
+
         When invoked with the timeout argument set to a positive value, block for at most the number of seconds specified by timeout and as long as the lock cannot be acquired. A timeout argument of -1 specifies an unbounded wait. It is forbidden to specify a timeout when blocking is False.
 
         When the exclusive argument is True (the default), an exclusive lock is made. If False, then a shared lock is made. These are equivalent to the exclusive and shared locks in the linux flock command.
-        
+
         The return value is True if the lock is acquired successfully, False if not (for example if the timeout expired).
 
         Returns
         -------
         bool
         """
         if self._last_modified is None:
             if exclusive:
                 body = b'1'
             else:
                 body = b'0'
-            self._put_object(body)
+            self._put_lock_object(body)
             objs = self.other_locks()
             objs2 = self._check_for_older_versions(objs, self._last_modified, self._version_id)
 
             if objs2:
                 start_time = default_timer()
 
                 while blocking:
```

### Comparing `s3func-0.2.1/s3func/utils.py` & `s3func-0.2.2/s3func/utils.py`

 * *Files identical despite different names*

### Comparing `s3func-0.2.1/s3func/tests/stns_data.blt` & `s3func-0.2.2/s3func/tests/stns_data.blt`

 * *Files identical despite different names*

### Comparing `s3func-0.2.1/s3func/tests/test_s3func.py` & `s3func-0.2.2/s3func/tests/test_s3func.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 #################################################
 ### Parameters
 
 script_path = pathlib.Path(os.path.realpath(os.path.dirname(__file__)))
 package_path = str(script_path.parent)
 
-# if package_path not in sys.path:
-#     sys.path.insert(0, package_path)
-# import s3, http_url # For running without a package
+if package_path not in sys.path:
+    sys.path.insert(0, package_path)
+import s3, http_url # For running without a package
 
 try:
     with open(script_path.joinpath('s3_config.toml'), "rb") as f:
         conn_config = toml.load(f)['connection_config']
 except:
     conn_config = {
         'service_name': 's3',
@@ -39,14 +39,15 @@
 flag = "w"
 buffer_size = 524288
 read_timeout = 60
 threads = 10
 object_lock = False
 file_name = 'stns_data.blt'
 obj_key = uuid.uuid4().hex
+obj_key = 'manual_test_key'
 base_url = 'https://b2.tethys-ts.xyz/file/' + bucket + '/'
 url = base_url +  obj_key
 
 s3_client = s3.client(conn_config)
 
 
 ################################################
@@ -308,15 +309,16 @@
         with s3lock:
             mod_date = s3lock._last_modified
             others = s3lock.other_locks()
             if others:
                 for other_one in others:
                     other_mod_date = other_one['last_modified']
                     if other_mod_date < mod_date:
-                        raise ValueError('Other mod date was earlier.')
+                        print(('Other mod date was earlier.'))
+                        # raise ValueError('Other mod date was earlier.')
 
 
 def resp_delay_test(n):
     """
 
     """
     s3lock = s3.S3Lock(s3_client, bucket, obj_key)
@@ -342,15 +344,20 @@
     # header_time_mean = to_header_time/n
     # return_time_mean = to_return_time/n
 
     return to_mod_time, to_header_time, to_return_time
 
 
 
+# def _save_test_results(to_mod_time, to_header_time, to_return_time):
+#     """
 
+#     """
+#     df1 = pd.DataFrame(zip(to_mod_time, to_header_time, to_return_time), columns=['to_mod_time', 'to_header_time', 'to_return_time'])
+#     df1.to_csv('put_object_timings.csv')
```

### Comparing `s3func-0.2.1/.gitignore` & `s3func-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `s3func-0.2.1/LICENSE` & `s3func-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `s3func-0.2.1/README.md` & `s3func-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `s3func-0.2.1/pyproject.toml` & `s3func-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `s3func-0.2.1/PKG-INFO` & `s3func-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: s3func
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple functions for working with S3
 Project-URL: Documentation, https://mullenkamp.github.io/s3func/
 Project-URL: Source, https://github.com/mullenkamp/s3func
 Author-email: s3func <mullenkamp1@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: s3func Version: 0.2.1 Summary: Simple functions for
+Metadata-Version: 2.3 Name: s3func Version: 0.2.2 Summary: Simple functions for
 working with S3 Project-URL: Documentation, https://mullenkamp.github.io/
 s3func/ Project-URL: Source, https://github.com/mullenkamp/s3func Author-email:
 s3func
 gmail.com> License-File: LICENSE Classifier: Programming Language :: Python ::
 3 :: Only Requires-Python: >=3.9 Requires-Dist: boto3 Requires-Dist: pydantic
 Requires-Dist: urllib3>=2 Description-Content-Type: text/markdown # s3func
                      SSiimmppllee ffuunnccttiioonnss ffoorr wwoorrkkiinngg wwiitthh SS33
```

