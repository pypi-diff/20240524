# Comparing `tmp/ansar_connect-0.1.257.tar.gz` & `tmp/ansar_connect-0.1.258.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.257.tar", last modified: Wed May 22 19:33:27 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.258.tar", last modified: Fri May 24 06:43:29 2024, max compression
```

## Comparing `ansar_connect-0.1.257.tar` & `ansar_connect-0.1.258.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 19:33:27.657091 ansar_connect-0.1.257/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.257/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1303 2024-05-22 19:33:27.657091 ansar_connect-0.1.257/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)      538 2024-05-21 07:49:27.000000 ansar_connect-0.1.257/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-22 19:33:13.000000 ansar_connect-0.1.257/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-22 19:33:27.657091 ansar_connect-0.1.257/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-22 19:33:04.000000 ansar_connect-0.1.257/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 19:33:27.653091 ansar_connect-0.1.257/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 19:33:27.653091 ansar_connect-0.1.257/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 19:33:27.653091 ansar_connect-0.1.257/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.257/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.257/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.257/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.257/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 19:33:27.657091 ansar_connect-0.1.257/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-22 19:33:24.000000 ansar_connect-0.1.257/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.257/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    88788 2024-05-18 21:19:19.000000 ansar_connect-0.1.257/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.257/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.257/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.257/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    15853 2024-05-20 01:19:54.000000 ansar_connect-0.1.257/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.257/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.257/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.257/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9679 2024-05-21 15:14:21.000000 ansar_connect-0.1.257/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.257/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.257/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.257/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    42334 2024-05-19 21:19:26.000000 ansar_connect-0.1.257/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.257/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.257/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.257/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.257/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 19:33:27.657091 ansar_connect-0.1.257/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1303 2024-05-22 19:33:27.000000 ansar_connect-0.1.257/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-22 19:33:27.000000 ansar_connect-0.1.257/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-22 19:33:27.000000 ansar_connect-0.1.257/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-22 19:33:27.000000 ansar_connect-0.1.257/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-22 19:33:27.000000 ansar_connect-0.1.257/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-22 19:33:27.000000 ansar_connect-0.1.257/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 06:43:29.724232 ansar_connect-0.1.258/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.258/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-24 06:43:29.724232 ansar_connect-0.1.258/PKG-INFO
+-rwxrwxr-x   0 scott     (1000) scott     (1000)      577 2024-05-23 01:07:25.000000 ansar_connect-0.1.258/README.md
+-rwxrwxr-x   0 scott     (1000) scott     (1000)      764 2024-05-24 06:42:45.000000 ansar_connect-0.1.258/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-24 06:43:29.724232 ansar_connect-0.1.258/setup.cfg
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2251 2024-05-24 06:42:37.000000 ansar_connect-0.1.258/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 06:43:29.724232 ansar_connect-0.1.258/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 06:43:29.724232 ansar_connect-0.1.258/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 06:43:29.724232 ansar_connect-0.1.258/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.258/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.258/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.258/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.258/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 06:43:29.724232 ansar_connect-0.1.258/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-24 06:43:26.000000 ansar_connect-0.1.258/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.258/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    88764 2024-05-24 02:37:42.000000 ansar_connect-0.1.258/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.258/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.258/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.258/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    15853 2024-05-20 01:19:54.000000 ansar_connect-0.1.258/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.258/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.258/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.258/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9679 2024-05-21 15:14:21.000000 ansar_connect-0.1.258/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.258/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.258/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.258/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    42334 2024-05-19 21:19:26.000000 ansar_connect-0.1.258/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.258/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.258/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.258/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.258/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 06:43:29.724232 ansar_connect-0.1.258/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1342 2024-05-24 06:43:29.000000 ansar_connect-0.1.258/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-24 06:43:29.000000 ansar_connect-0.1.258/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-24 06:43:29.000000 ansar_connect-0.1.258/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-24 06:43:29.000000 ansar_connect-0.1.258/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-24 06:43:29.000000 ansar_connect-0.1.258/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-24 06:43:29.000000 ansar_connect-0.1.258/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.257/LICENSE` & `ansar_connect-0.1.258/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/PKG-INFO` & `ansar_connect-0.1.258/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.257
+Version: 0.1.258
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,20 +12,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi>=1.16.0
 Requires-Dist: PyNaCl>=1.5.0
-Requires-Dist: ansar-create>=0.1.90
+Requires-Dist: ansar-create>=0.1.91
 
 # ansar-connect
 
 The **ansar-connect** library implements clear and concise network messaging for a wide range
 of networking requirements. From multi-processing within a single host through to messaging
 beween different LANs on the Internet. There is a single send method that does it all.
 
 ## Features
 
-- Implements full-duplex, network messaging over asynchronous sockets,
+- Implements bi-directional, asynchronous network messaging,
+- Provides a synchronous request-response layer,
 - Inherits the data sophistication of **ansar.encode**,
 - Seamlessly extends the asynchronous runtime from **ansar.create**, to span local and wide-area networks.
```

### Comparing `ansar_connect-0.1.257/README.md` & `ansar_connect-0.1.258/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,10 +2,11 @@
 
 The **ansar-connect** library implements clear and concise network messaging for a wide range
 of networking requirements. From multi-processing within a single host through to messaging
 beween different LANs on the Internet. There is a single send method that does it all.
 
 ## Features
 
-- Implements full-duplex, network messaging over asynchronous sockets,
+- Implements bi-directional, asynchronous network messaging,
+- Provides a synchronous request-response layer,
 - Inherits the data sophistication of **ansar.encode**,
 - Seamlessly extends the asynchronous runtime from **ansar.create**, to span local and wide-area networks.
```

### Comparing `ansar_connect-0.1.257/pyproject.toml` & `ansar_connect-0.1.258/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 	"Operating System :: OS Independent",
 	"Topic :: Software Development :: Libraries"
 ]
 dynamic = ["description", "version", "scripts"]
 dependencies = [
     "cffi>=1.16.0",
     "PyNaCl>=1.5.0",
-    "ansar-create>=0.1.90"
+    "ansar-create>=0.1.91"
 ]
 
 [project.urls]
 Documentation = "https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html"
```

### Comparing `ansar_connect-0.1.257/setup.py` & `ansar_connect-0.1.258/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 with open("DOC_LATEST_LINK", "r", encoding="utf-8") as f:
     d = f.read()
 DOC_LINK = d[:-1]
 
 REQUIRES = [
     "cffi>=1.16.0",
     "PyNaCl>=1.5.0",
-    "ansar-create>=0.1.90",
+    "ansar-create>=0.1.91",
 ]
 
 setuptools.setup(
     name=PACKAGE,
     version=VERSION,
     author="Scott Woods",
     author_email="scott.18.ansar@gmail.com.com",
```

### Comparing `ansar_connect-0.1.257/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.258/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.258/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.258/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.258/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/__init__.py` & `ansar_connect-0.1.258/src/ansar/connect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 37d7c5c1b2743e0b23aab91e58f8746d36bfdb0d
-Version: 0.1.256 (2024-05-23@07:33:24+NZST)
+Commit: 26c45591ce4ad7ded2745b69d9c35490197d43e6
+Version: 0.1.257 (2024-05-24@18:43:26+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.257/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.258/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/directory.py` & `ansar_connect-0.1.258/src/ansar/connect/directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1888,15 +1888,15 @@
 def SubscriberLoop_CONNECTION_PEERING_T2(self, message):
 	route_key = self.route.route_key
 	name = key_service(route_key)
 	reason = 'timed out on peer'
 	self.trace(f'Cannot loop to {name} ({reason})')
 	na = NotAvailable(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=self.route.route_key, reason=message.reason,
+		route_key=self.route.route_key, reason=reason,
 		agent_address=self.parent_address)
 	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
@@ -2058,15 +2058,15 @@
 def SubscriberLoop_RELAY_PEERING_T2(self, message):
 	route_key = self.route.route_key
 	name = key_service(route_key)
 	reason = 'timed out on peer'
 	self.trace(f'Cannot relay to {name} ({reason})')
 	na = NotAvailable(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=self.route.route_key, reason=message.reason,
+		route_key=self.route.route_key, reason=reason,
 		agent_address=self.parent_address)
 	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
@@ -2090,15 +2090,15 @@
 def SubscriberLoop_RELAY_LOOPING_T1(self, message):
 	route_key = self.route.route_key
 	name = key_service(route_key)
 	reason = 'loop time exceeded'
 	self.trace(f'Cannot relay to {name} ({reason})')
 	na = NotAvailable(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=self.route.route_key, reason=message.reason,
+		route_key=self.route.route_key, reason=reason,
 		agent_address=self.parent_address)
 	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_loop()
 	self.close_relay()
 	self.close_peer()
```

### Comparing `ansar_connect-0.1.257/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.258/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.258/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/group_if.py` & `ansar_connect-0.1.258/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/grouping.py` & `ansar_connect-0.1.258/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/moving.py` & `ansar_connect-0.1.258/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/networking.py` & `ansar_connect-0.1.258/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.258/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/node.py` & `ansar_connect-0.1.258/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.258/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/procedure.py` & `ansar_connect-0.1.258/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/product.py` & `ansar_connect-0.1.258/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/socketry.py` & `ansar_connect-0.1.258/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/standard.py` & `ansar_connect-0.1.258/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/transporting.py` & `ansar_connect-0.1.258/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.258/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar/connect/wan.py` & `ansar_connect-0.1.258/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.257/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.258/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.257
+Version: 0.1.258
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,20 +12,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi>=1.16.0
 Requires-Dist: PyNaCl>=1.5.0
-Requires-Dist: ansar-create>=0.1.90
+Requires-Dist: ansar-create>=0.1.91
 
 # ansar-connect
 
 The **ansar-connect** library implements clear and concise network messaging for a wide range
 of networking requirements. From multi-processing within a single host through to messaging
 beween different LANs on the Internet. There is a single send method that does it all.
 
 ## Features
 
-- Implements full-duplex, network messaging over asynchronous sockets,
+- Implements bi-directional, asynchronous network messaging,
+- Provides a synchronous request-response layer,
 - Inherits the data sophistication of **ansar.encode**,
 - Seamlessly extends the asynchronous runtime from **ansar.create**, to span local and wide-area networks.
```

### Comparing `ansar_connect-0.1.257/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.258/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

