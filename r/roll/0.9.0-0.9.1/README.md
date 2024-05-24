# Comparing `tmp/roll-0.9.0.tar.gz` & `tmp/roll-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/roll-0.9.0.tar", last modified: Mon Jun  4 17:30:12 2018, max compression
+gzip compressed data, was "dist/roll-0.9.1.tar", last modified: Mon Jun 11 21:11:11 2018, max compression
```

## Comparing `roll-0.9.0.tar` & `roll-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2018-06-04 17:30:12.000000 roll-0.9.0/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1066 2018-06-04 17:30:12.000000 roll-0.9.0/PKG-INFO
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2018-06-04 17:30:12.000000 roll-0.9.0/roll/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1711 2017-09-13 19:44:56.000000 roll-0.9.0/roll/worker.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4430 2018-05-17 09:48:41.000000 roll-0.9.0/roll/extensions.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22005 2018-05-28 13:40:41.000000 roll-0.9.0/roll/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7911 2018-05-28 13:30:40.000000 roll-0.9.0/roll/testing.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      288 2017-10-30 15:28:54.000000 roll-0.9.0/README.md
--rw-r--r--   0 ybon      (1000) ybon      (1000)      104 2018-06-04 17:27:20.000000 roll-0.9.0/requirements.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)       38 2018-06-04 17:30:12.000000 roll-0.9.0/setup.cfg
--rw-r--r--   0 ybon      (1000) ybon      (1000)       43 2017-08-25 15:50:42.000000 roll-0.9.0/MANIFEST.in
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2018-06-04 17:30:12.000000 roll-0.9.0/roll.egg-info/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1066 2018-06-04 17:30:12.000000 roll-0.9.0/roll.egg-info/PKG-INFO
--rw-r--r--   0 ybon      (1000) ybon      (1000)        1 2018-06-04 17:30:12.000000 roll-0.9.0/roll.egg-info/dependency_links.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)       32 2018-06-04 17:30:12.000000 roll-0.9.0/roll.egg-info/entry_points.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)        5 2018-06-04 17:30:12.000000 roll-0.9.0/roll.egg-info/top_level.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)      284 2018-06-04 17:30:12.000000 roll-0.9.0/roll.egg-info/SOURCES.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)      134 2018-06-04 17:30:12.000000 roll-0.9.0/roll.egg-info/requires.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2306 2018-06-04 17:14:22.000000 roll-0.9.0/setup.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2018-06-11 21:11:11.000000 roll-0.9.1/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1066 2018-06-11 21:11:11.000000 roll-0.9.1/PKG-INFO
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2018-06-11 21:11:11.000000 roll-0.9.1/roll/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1711 2017-09-13 19:44:56.000000 roll-0.9.1/roll/worker.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4430 2018-05-17 09:48:41.000000 roll-0.9.1/roll/extensions.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22372 2018-06-11 10:32:45.000000 roll-0.9.1/roll/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7911 2018-05-28 13:30:40.000000 roll-0.9.1/roll/testing.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      288 2017-10-30 15:28:54.000000 roll-0.9.1/README.md
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      104 2018-06-04 17:27:20.000000 roll-0.9.1/requirements.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       38 2018-06-11 21:11:11.000000 roll-0.9.1/setup.cfg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       43 2017-08-25 15:50:42.000000 roll-0.9.1/MANIFEST.in
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2018-06-11 21:11:11.000000 roll-0.9.1/roll.egg-info/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1066 2018-06-11 21:11:11.000000 roll-0.9.1/roll.egg-info/PKG-INFO
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        1 2018-06-11 21:11:11.000000 roll-0.9.1/roll.egg-info/dependency_links.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       32 2018-06-11 21:11:11.000000 roll-0.9.1/roll.egg-info/entry_points.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        5 2018-06-11 21:11:11.000000 roll-0.9.1/roll.egg-info/top_level.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      284 2018-06-11 21:11:11.000000 roll-0.9.1/roll.egg-info/SOURCES.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      134 2018-06-11 21:11:11.000000 roll-0.9.1/roll.egg-info/requires.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2306 2018-06-11 21:10:35.000000 roll-0.9.1/setup.py
```

### Comparing `roll-0.9.0/PKG-INFO` & `roll-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roll
-Version: 0.9.0
+Version: 0.9.1
 Summary: Roll is a pico framework with performances and aesthetic in mind.
 Home-page: https://github.com/pyrates/roll
 Author: Pyrates
 Author-email: yohan.boniface@data.gouv.fr
 License: WTFPL
 Description: # Let’s roll.
         
@@ -24,9 +24,9 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: test
```

### Comparing `roll-0.9.0/roll/worker.py` & `roll-0.9.1/roll/worker.py`

 * *Files identical despite different names*

### Comparing `roll-0.9.0/roll/extensions.py` & `roll-0.9.1/roll/extensions.py`

 * *Files identical despite different names*

### Comparing `roll-0.9.0/roll/__init__.py` & `roll-0.9.1/roll/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -515,17 +515,26 @@
             for cookie in self.response.cookies.values():
                 payload += b'Set-Cookie: %b\r\n' % str(cookie).encode()
         for key, value in self.response.headers.items():
             payload += b'%b: %b\r\n' % (key.encode(), str(value).encode())
         payload += b'\r\n'
         if self.response.body and not bodyless:
             payload += self.response.body
-        self.transport.write(payload)
-        if not self.parser.should_keep_alive():
-            self.transport.close()
+        if self.transport.is_closing():
+            # Request has been aborted, thus socket as been closed, thus
+            # transport has been closed?
+            return
+        try:
+            self.transport.write(payload)
+        except RuntimeError:  # transport may still be closed during write.
+            # TODO: Pass into error hook when write is async.
+            pass
+        else:
+            if not self.parser.should_keep_alive():
+                self.transport.close()
 
 
 Route = namedtuple('Route', ['payload', 'vars'])
 
 
 class Roll(dict):
     """Deal with routes dispatching and events listening.
```

### Comparing `roll-0.9.0/roll/testing.py` & `roll-0.9.1/roll/testing.py`

 * *Files identical despite different names*

### Comparing `roll-0.9.0/roll.egg-info/PKG-INFO` & `roll-0.9.1/roll.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roll
-Version: 0.9.0
+Version: 0.9.1
 Summary: Roll is a pico framework with performances and aesthetic in mind.
 Home-page: https://github.com/pyrates/roll
 Author: Pyrates
 Author-email: yohan.boniface@data.gouv.fr
 License: WTFPL
 Description: # Let’s roll.
         
@@ -24,9 +24,9 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: test
```

### Comparing `roll-0.9.0/setup.py` & `roll-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     ext_modules = [
         Extension('roll', ['roll/__init__.py']),
         Extension('roll.extensions', ['roll/extensions.py']),
         Extension('roll.worker', ['roll/worker.py']),
     ]
     cmdclass = {'build_ext': build_ext}
 
-VERSION = (0, 9, 0)
+VERSION = (0, 9, 1)
 
 __author__ = 'Pyrates'
 __contact__ = "yohan.boniface@data.gouv.fr"
 __homepage__ = "https://github.com/pyrates/roll"
 __version__ = ".".join(map(str, VERSION))
 
 setup(
```

