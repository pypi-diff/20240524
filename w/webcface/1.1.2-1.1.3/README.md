# Comparing `tmp/webcface-1.1.2.tar.gz` & `tmp/webcface-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcface-1.1.2.tar", max compression
+gzip compressed data, was "webcface-1.1.3.tar", max compression
```

## Comparing `webcface-1.1.2.tar` & `webcface-1.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1069 2024-03-09 06:13:45.146310 webcface-1.1.2/LICENSE
--rw-r--r--   0        0        0      667 2024-03-09 06:13:45.146310 webcface-1.1.2/README.md
--rw-r--r--   0        0        0      857 2024-03-09 06:13:45.150310 webcface-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      787 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/__init__.py
--rw-r--r--   0        0        0     7773 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/canvas2d.py
--rw-r--r--   0        0        0     1914 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/canvas2d_base.py
--rw-r--r--   0        0        0     6518 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/canvas3d.py
--rw-r--r--   0        0        0     1888 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/canvas3d_base.py
--rw-r--r--   0        0        0     7922 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/client.py
--rw-r--r--   0        0        0    12357 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/client_data.py
--rw-r--r--   0        0        0    14680 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/client_impl.py
--rw-r--r--   0        0        0     1008 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/field.py
--rw-r--r--   0        0        0     8342 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/func.py
--rw-r--r--   0        0        0     7258 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/func_info.py
--rw-r--r--   0        0        0     8783 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/geometries.py
--rw-r--r--   0        0        0     2105 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/log.py
--rw-r--r--   0        0        0     1930 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/log_handler.py
--rw-r--r--   0        0        0     9658 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/member.py
--rw-r--r--   0        0        0    22138 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/message.py
--rw-r--r--   0        0        0     2895 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/text.py
--rw-r--r--   0        0        0     5233 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/transform.py
--rw-r--r--   0        0        0     3677 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/value.py
--rw-r--r--   0        0        0     9166 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/view.py
--rw-r--r--   0        0        0      640 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/view_base.py
--rw-r--r--   0        0        0     1487 2024-03-09 06:13:45.150310 webcface-1.1.2/webcface/view_components.py
--rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 webcface-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-24 09:08:14.483312 webcface-1.1.3/LICENSE
+-rw-r--r--   0        0        0      667 2024-05-24 09:08:14.483312 webcface-1.1.3/README.md
+-rw-r--r--   0        0        0      857 2024-05-24 09:08:14.483312 webcface-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      787 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/__init__.py
+-rw-r--r--   0        0        0     7773 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/canvas2d.py
+-rw-r--r--   0        0        0     1914 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/canvas2d_base.py
+-rw-r--r--   0        0        0     6518 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/canvas3d.py
+-rw-r--r--   0        0        0     1888 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/canvas3d_base.py
+-rw-r--r--   0        0        0     8021 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/client.py
+-rw-r--r--   0        0        0    12357 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/client_data.py
+-rw-r--r--   0        0        0    14680 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/client_impl.py
+-rw-r--r--   0        0        0     1008 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/field.py
+-rw-r--r--   0        0        0     8342 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/func.py
+-rw-r--r--   0        0        0     7258 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/func_info.py
+-rw-r--r--   0        0        0     8783 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/geometries.py
+-rw-r--r--   0        0        0     2105 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/log.py
+-rw-r--r--   0        0        0     1930 2024-05-24 09:08:14.483312 webcface-1.1.3/webcface/log_handler.py
+-rw-r--r--   0        0        0     9658 2024-05-24 09:08:14.487312 webcface-1.1.3/webcface/member.py
+-rw-r--r--   0        0        0    22138 2024-05-24 09:08:14.487312 webcface-1.1.3/webcface/message.py
+-rw-r--r--   0        0        0     2895 2024-05-24 09:08:14.487312 webcface-1.1.3/webcface/text.py
+-rw-r--r--   0        0        0     5233 2024-05-24 09:08:14.487312 webcface-1.1.3/webcface/transform.py
+-rw-r--r--   0        0        0     3677 2024-05-24 09:08:14.487312 webcface-1.1.3/webcface/value.py
+-rw-r--r--   0        0        0     9166 2024-05-24 09:08:14.487312 webcface-1.1.3/webcface/view.py
+-rw-r--r--   0        0        0      640 2024-05-24 09:08:14.487312 webcface-1.1.3/webcface/view_base.py
+-rw-r--r--   0        0        0     1487 2024-05-24 09:08:14.487312 webcface-1.1.3/webcface/view_components.py
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 webcface-1.1.3/PKG-INFO
```

### Comparing `webcface-1.1.2/LICENSE` & `webcface-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/README.md` & `webcface-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/pyproject.toml` & `webcface-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webcface"
-version = "1.1.2"
+version = "1.1.3"
 description = "WebCFace Client for Python"
 authors = ["na-trium-144 <100704180+na-trium-144@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/na-trium-144/webcface-python"
 documentation = "https://na-trium-144.github.io/webcface-python/"
```

### Comparing `webcface-1.1.2/webcface/__init__.py` & `webcface-1.1.3/webcface/__init__.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/canvas2d.py` & `webcface-1.1.3/webcface/canvas2d.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/canvas2d_base.py` & `webcface-1.1.3/webcface/canvas2d_base.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/canvas3d.py` & `webcface-1.1.3/webcface/canvas3d.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/canvas3d_base.py` & `webcface-1.1.3/webcface/canvas3d_base.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/client.py` & `webcface-1.1.3/webcface/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,29 +88,31 @@
                     on_error=on_error,
                     on_close=on_close,
                 )
                 try:
                     self._ws.run_forever()
                 except Exception as e:
                     data.logger_internal.debug(f"WebSocket Error: {e}")
-                time.sleep(1)
+                if not self._closing:
+                    time.sleep(0.1)
             data.logger_internal.debug(f"reconnect_thread end")
 
 
         self._reconnect_thread = threading.Thread(target=reconnect, daemon=True)
 
         def msg_send():
             data = self._data_check()
             while self._reconnect_thread.is_alive():
                 while (
                     not self.connected or not data.has_msg()
                 ) and self._reconnect_thread.is_alive():
-                    with self._connection_cv:
-                        self._connection_cv.wait(timeout=1)
-                    data.wait_msg(timeout=1)
+                    if not self.connected:
+                        with self._connection_cv:
+                            self._connection_cv.wait(timeout=0.1)
+                    data.wait_msg(timeout=0.1)
                 msgs = self._data_check().pop_msg()
                 if msgs is not None and self._ws is not None and self.connected:
                     try:
                         data.logger_internal.debug("Sending message")
                         self._ws.send(webcface.message.pack(msgs))
                     except Exception as e:
                         data.logger_internal.error(f"Error Sending message {e}")
```

### Comparing `webcface-1.1.2/webcface/client_data.py` & `webcface-1.1.3/webcface/client_data.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/client_impl.py` & `webcface-1.1.3/webcface/client_impl.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/field.py` & `webcface-1.1.3/webcface/field.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/func.py` & `webcface-1.1.3/webcface/func.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/func_info.py` & `webcface-1.1.3/webcface/func_info.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/geometries.py` & `webcface-1.1.3/webcface/geometries.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/log.py` & `webcface-1.1.3/webcface/log.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/log_handler.py` & `webcface-1.1.3/webcface/log_handler.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/member.py` & `webcface-1.1.3/webcface/member.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/message.py` & `webcface-1.1.3/webcface/message.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/text.py` & `webcface-1.1.3/webcface/text.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/transform.py` & `webcface-1.1.3/webcface/transform.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/value.py` & `webcface-1.1.3/webcface/value.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/view.py` & `webcface-1.1.3/webcface/view.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/view_base.py` & `webcface-1.1.3/webcface/view_base.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/webcface/view_components.py` & `webcface-1.1.3/webcface/view_components.py`

 * *Files identical despite different names*

### Comparing `webcface-1.1.2/PKG-INFO` & `webcface-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcface
-Version: 1.1.2
+Version: 1.1.3
 Summary: WebCFace Client for Python
 Home-page: https://github.com/na-trium-144/webcface-python
 License: MIT
 Author: na-trium-144
 Author-email: 100704180+na-trium-144@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

