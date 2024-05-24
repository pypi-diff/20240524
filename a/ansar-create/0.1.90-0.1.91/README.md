# Comparing `tmp/ansar_create-0.1.90.tar.gz` & `tmp/ansar_create-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_create-0.1.90.tar", last modified: Wed May 22 19:32:26 2024, max compression
+gzip compressed data, was "ansar_create-0.1.91.tar", last modified: Fri May 24 06:42:04 2024, max compression
```

## Comparing `ansar_create-0.1.90.tar` & `ansar_create-0.1.91.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 19:32:26.085633 ansar_create-0.1.90/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:18.000000 ansar_create-0.1.90/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-22 19:32:26.085633 ansar_create-0.1.90/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      901 2023-06-17 21:18:11.000000 ansar_create-0.1.90/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      718 2024-05-22 01:10:14.000000 ansar_create-0.1.90/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-22 19:32:26.085633 ansar_create-0.1.90/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     2139 2024-05-22 01:10:05.000000 ansar_create-0.1.90/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 19:32:26.081633 ansar_create-0.1.90/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 19:32:26.081633 ansar_create-0.1.90/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 19:32:26.081633 ansar_create-0.1.90/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    13081 2024-01-02 02:57:04.000000 ansar_create-0.1.90/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8950 2024-02-25 02:39:34.000000 ansar_create-0.1.90/src/ansar/command/ansar_group.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 19:32:26.085633 ansar_create-0.1.90/src/ansar/create/
--rw-rw-r--   0 scott     (1000) scott     (1000)     5706 2024-05-22 19:32:22.000000 ansar_create-0.1.90/src/ansar/create/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2654 2023-07-13 04:39:47.000000 ansar_create-0.1.90/src/ansar/create/binding.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1989 2023-12-23 01:56:16.000000 ansar_create-0.1.90/src/ansar/create/coding.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1857 2024-01-19 15:16:48.000000 ansar_create-0.1.90/src/ansar/create/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    13837 2024-02-24 20:57:36.000000 ansar_create-0.1.90/src/ansar/create/home.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3590 2024-05-22 18:42:10.000000 ansar_create-0.1.90/src/ansar/create/latching.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7383 2024-03-24 15:57:41.000000 ansar_create-0.1.90/src/ansar/create/lifecycle.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     4061 2024-01-25 13:13:42.000000 ansar_create-0.1.90/src/ansar/create/locking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6164 2023-07-13 04:40:10.000000 ansar_create-0.1.90/src/ansar/create/log.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8495 2023-07-13 04:40:11.000000 ansar_create-0.1.90/src/ansar/create/machine.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    29887 2024-05-21 15:14:05.000000 ansar_create-0.1.90/src/ansar/create/object.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9071 2024-01-18 15:23:10.000000 ansar_create-0.1.90/src/ansar/create/pending.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    29529 2024-05-14 22:01:16.000000 ansar_create-0.1.90/src/ansar/create/point.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    80287 2024-05-14 16:43:56.000000 ansar_create-0.1.90/src/ansar/create/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    31841 2024-01-22 04:26:11.000000 ansar_create-0.1.90/src/ansar/create/processing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3099 2024-03-26 19:19:48.000000 ansar_create-0.1.90/src/ansar/create/properties.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3741 2024-03-07 07:59:16.000000 ansar_create-0.1.90/src/ansar/create/retry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5938 2024-02-27 14:04:16.000000 ansar_create-0.1.90/src/ansar/create/rolling.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7477 2023-12-23 15:53:02.000000 ansar_create-0.1.90/src/ansar/create/root.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14309 2024-05-22 19:30:42.000000 ansar_create-0.1.90/src/ansar/create/space.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    19735 2024-03-22 18:43:09.000000 ansar_create-0.1.90/src/ansar/create/storage.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3959 2024-01-15 15:55:19.000000 ansar_create-0.1.90/src/ansar/create/test.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5100 2024-01-26 08:38:29.000000 ansar_create-0.1.90/src/ansar/create/timing.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 19:32:26.085633 ansar_create-0.1.90/src/ansar_create.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-22 19:32:26.000000 ansar_create-0.1.90/src/ansar_create.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      986 2024-05-22 19:32:26.000000 ansar_create-0.1.90/src/ansar_create.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-22 19:32:26.000000 ansar_create-0.1.90/src/ansar_create.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      104 2024-05-22 19:32:26.000000 ansar_create-0.1.90/src/ansar_create.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       22 2024-05-22 19:32:26.000000 ansar_create-0.1.90/src/ansar_create.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-22 19:32:26.000000 ansar_create-0.1.90/src/ansar_create.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 06:42:04.717087 ansar_create-0.1.91/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:18.000000 ansar_create-0.1.91/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-24 06:42:04.717087 ansar_create-0.1.91/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      901 2023-06-17 21:18:11.000000 ansar_create-0.1.91/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      718 2024-05-22 01:10:14.000000 ansar_create-0.1.91/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-24 06:42:04.717087 ansar_create-0.1.91/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2139 2024-05-22 01:10:05.000000 ansar_create-0.1.91/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 06:42:04.713087 ansar_create-0.1.91/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 06:42:04.713087 ansar_create-0.1.91/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 06:42:04.713087 ansar_create-0.1.91/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13081 2024-01-02 02:57:04.000000 ansar_create-0.1.91/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8950 2024-02-25 02:39:34.000000 ansar_create-0.1.91/src/ansar/command/ansar_group.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 06:42:04.717087 ansar_create-0.1.91/src/ansar/create/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5706 2024-05-24 06:42:01.000000 ansar_create-0.1.91/src/ansar/create/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2654 2023-07-13 04:39:47.000000 ansar_create-0.1.91/src/ansar/create/binding.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1989 2023-12-23 01:56:16.000000 ansar_create-0.1.91/src/ansar/create/coding.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1857 2024-01-19 15:16:48.000000 ansar_create-0.1.91/src/ansar/create/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13837 2024-02-24 20:57:36.000000 ansar_create-0.1.91/src/ansar/create/home.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3590 2024-05-22 18:42:10.000000 ansar_create-0.1.91/src/ansar/create/latching.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7383 2024-03-24 15:57:41.000000 ansar_create-0.1.91/src/ansar/create/lifecycle.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4061 2024-01-25 13:13:42.000000 ansar_create-0.1.91/src/ansar/create/locking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6164 2023-07-13 04:40:10.000000 ansar_create-0.1.91/src/ansar/create/log.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8495 2023-07-13 04:40:11.000000 ansar_create-0.1.91/src/ansar/create/machine.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    29887 2024-05-21 15:14:05.000000 ansar_create-0.1.91/src/ansar/create/object.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9071 2024-01-18 15:23:10.000000 ansar_create-0.1.91/src/ansar/create/pending.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    29529 2024-05-14 22:01:16.000000 ansar_create-0.1.91/src/ansar/create/point.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    80287 2024-05-14 16:43:56.000000 ansar_create-0.1.91/src/ansar/create/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    31841 2024-01-22 04:26:11.000000 ansar_create-0.1.91/src/ansar/create/processing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3099 2024-03-26 19:19:48.000000 ansar_create-0.1.91/src/ansar/create/properties.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3741 2024-03-07 07:59:16.000000 ansar_create-0.1.91/src/ansar/create/retry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5938 2024-02-27 14:04:16.000000 ansar_create-0.1.91/src/ansar/create/rolling.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7477 2023-12-23 15:53:02.000000 ansar_create-0.1.91/src/ansar/create/root.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14309 2024-05-22 19:30:42.000000 ansar_create-0.1.91/src/ansar/create/space.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    19885 2024-05-24 06:04:53.000000 ansar_create-0.1.91/src/ansar/create/storage.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3959 2024-01-15 15:55:19.000000 ansar_create-0.1.91/src/ansar/create/test.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5100 2024-01-26 08:38:29.000000 ansar_create-0.1.91/src/ansar/create/timing.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 06:42:04.717087 ansar_create-0.1.91/src/ansar_create.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-24 06:42:04.000000 ansar_create-0.1.91/src/ansar_create.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      986 2024-05-24 06:42:04.000000 ansar_create-0.1.91/src/ansar_create.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-24 06:42:04.000000 ansar_create-0.1.91/src/ansar_create.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      104 2024-05-24 06:42:04.000000 ansar_create-0.1.91/src/ansar_create.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       22 2024-05-24 06:42:04.000000 ansar_create-0.1.91/src/ansar_create.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-24 06:42:04.000000 ansar_create-0.1.91/src/ansar_create.egg-info/top_level.txt
```

### Comparing `ansar_create-0.1.90/LICENSE` & `ansar_create-0.1.91/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/PKG-INFO` & `ansar_create-0.1.91/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-create
-Version: 0.1.90
+Version: 0.1.91
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com>
 Project-URL: Documentation, https://ansar-create-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_create-0.1.90/README.md` & `ansar_create-0.1.91/README.md`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/pyproject.toml` & `ansar_create-0.1.91/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/setup.py` & `ansar_create-0.1.91/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/command/ansar_command.py` & `ansar_create-0.1.91/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/command/ansar_group.py` & `ansar_create-0.1.91/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/__init__.py` & `ansar_create-0.1.91/src/ansar/create/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-create.git
 Branch: main
-Commit: 0baa77f34643b453d19c36da74ec735af0fa6344
-Version: 0.1.89 (2024-05-23@07:32:22+NZST)
+Commit: 921efe6856646de0da6dea67eacc3e7575a1ebdb
+Version: 0.1.90 (2024-05-24@18:42:01+NZST)
 """
 
 from ansar.encode import *
 
 from .coding import cannot, lor
 from .space import NO_SUCH_ADDRESS
 from .space import create_an_object, find_object, destroy_an_object
```

### Comparing `ansar_create-0.1.90/src/ansar/create/binding.py` & `ansar_create-0.1.91/src/ansar/create/binding.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/coding.py` & `ansar_create-0.1.91/src/ansar/create/coding.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/grouping.py` & `ansar_create-0.1.91/src/ansar/create/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/home.py` & `ansar_create-0.1.91/src/ansar/create/home.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/latching.py` & `ansar_create-0.1.91/src/ansar/create/latching.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/lifecycle.py` & `ansar_create-0.1.91/src/ansar/create/lifecycle.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/locking.py` & `ansar_create-0.1.91/src/ansar/create/locking.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/log.py` & `ansar_create-0.1.91/src/ansar/create/log.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/machine.py` & `ansar_create-0.1.91/src/ansar/create/machine.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/object.py` & `ansar_create-0.1.91/src/ansar/create/object.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/pending.py` & `ansar_create-0.1.91/src/ansar/create/pending.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/point.py` & `ansar_create-0.1.91/src/ansar/create/point.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/procedure.py` & `ansar_create-0.1.91/src/ansar/create/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/processing.py` & `ansar_create-0.1.91/src/ansar/create/processing.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/properties.py` & `ansar_create-0.1.91/src/ansar/create/properties.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/retry.py` & `ansar_create-0.1.91/src/ansar/create/retry.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/rolling.py` & `ansar_create-0.1.91/src/ansar/create/rolling.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/root.py` & `ansar_create-0.1.91/src/ansar/create/root.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/space.py` & `ansar_create-0.1.91/src/ansar/create/space.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/storage.py` & `ansar_create-0.1.91/src/ansar/create/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 """Movement of files to home processes and back.
 
 """
 __docformat__ = 'restructuredtext'
 
 import os
 import stat
-import pwd
-import grp
+#import pwd
+#import grp
 import uuid
 import shutil
 import datetime
 
 __all__ = [
 	'DELTA_FILE_ADD', 'DELTA_FILE_UPDATE', 'DELTA_FILE_UGM', 'DELTA_FILE_REMOVE',
 	'DELTA_FOLDER_ADD', 'DELTA_FOLDER_UPDATE', 'DELTA_FOLDER_UGM', 'DELTA_FOLDER_REMOVE',
@@ -70,18 +70,19 @@
 	"""Attributes of a folder/file in a storage hierarchy."""
 	def __init__(self, user=None, group=None, mode=None):
 		self.user = user
 		self.group = group
 		self.mode = mode
 
 	def __str__(self):
-		user = pwd.getpwuid(self.user)
-		group = grp.getgrgid(self.group)
-		rwx = stat.filemode(self.mode)
-		return f'StorageAttributes(owner={user.pw_name}, group={group.gr_name}, permissions={rwx})'
+	#	user = pwd.getpwuid(self.user)
+	#	group = grp.getgrgid(self.group)
+	#	rwx = stat.filemode(self.mode)
+	#	return f'StorageAttributes(owner={user.pw_name}, group={group.gr_name}, permissions={rwx})'
+		return f'StorageAttributes(owner={self.user}, group={self.group}, permissions={self.mode})'
 
 
 STORAGE_ATTRIBUTES_SCHEMA = {
 	'user': int,
 	'group': int,
 	'mode': int,
 }
@@ -187,27 +188,29 @@
 	# Small optimization to reduce hits on the
 	# platform dbs.
 	def lookup(s):
 		# User ids <---> names
 		try:
 			t = user_name[s.st_uid]	 # Already seen?
 		except KeyError:
-			try:
-				t = pwd.getpwuid(s.st_uid).pw_name	# Nope - lookup.
-			except KeyError:
-				t = None				# Not defined.
+			t = None				# Not defined.
+			#try:
+			#	t = pwd.getpwuid(s.st_uid).pw_name	# Nope - lookup.
+			#except KeyError:
+			#	t = None				# Not defined.
 			user_name[s.st_uid] = t	 # Remember results.
 		# Group ids <---> names
 		try:
 			t = group_name[s.st_gid]
 		except KeyError:
-			try:
-				t = grp.getgrgid(s.st_gid).gr_name
-			except KeyError:
-				t = None
+			t = None
+			#try:
+			#	t = grp.getgrgid(s.st_gid).gr_name
+			#except KeyError:
+			#	t = None
 			group_name[s.st_gid] = t
 		a = StorageAttributes(user=s.st_uid, group=s.st_gid, mode=s.st_mode)
 		return a
 
 	s = os.stat(path)
 	d = datetime.datetime.fromtimestamp(s.st_mtime, tz=ar.UTC)
 	a = lookup(s)
```

### Comparing `ansar_create-0.1.90/src/ansar/create/test.py` & `ansar_create-0.1.91/src/ansar/create/test.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar/create/timing.py` & `ansar_create-0.1.91/src/ansar/create/timing.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.90/src/ansar_create.egg-info/PKG-INFO` & `ansar_create-0.1.91/src/ansar_create.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-create
-Version: 0.1.90
+Version: 0.1.91
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com>
 Project-URL: Documentation, https://ansar-create-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_create-0.1.90/src/ansar_create.egg-info/SOURCES.txt` & `ansar_create-0.1.91/src/ansar_create.egg-info/SOURCES.txt`

 * *Files identical despite different names*

