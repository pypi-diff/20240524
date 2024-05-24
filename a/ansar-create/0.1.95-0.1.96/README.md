# Comparing `tmp/ansar_create-0.1.95.tar.gz` & `tmp/ansar_create-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_create-0.1.95.tar", last modified: Fri May 24 09:59:45 2024, max compression
+gzip compressed data, was "ansar_create-0.1.96.tar", last modified: Fri May 24 13:35:05 2024, max compression
```

## Comparing `ansar_create-0.1.95.tar` & `ansar_create-0.1.96.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 09:59:45.976550 ansar_create-0.1.95/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:18.000000 ansar_create-0.1.95/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-24 09:59:45.976550 ansar_create-0.1.95/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      901 2023-06-17 21:18:11.000000 ansar_create-0.1.95/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      718 2024-05-22 01:10:14.000000 ansar_create-0.1.95/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-24 09:59:45.976550 ansar_create-0.1.95/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     2139 2024-05-22 01:10:05.000000 ansar_create-0.1.95/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 09:59:45.976550 ansar_create-0.1.95/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 09:59:45.976550 ansar_create-0.1.95/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 09:59:45.976550 ansar_create-0.1.95/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    13081 2024-01-02 02:57:04.000000 ansar_create-0.1.95/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8950 2024-02-25 02:39:34.000000 ansar_create-0.1.95/src/ansar/command/ansar_group.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 09:59:45.976550 ansar_create-0.1.95/src/ansar/create/
--rw-rw-r--   0 scott     (1000) scott     (1000)     5706 2024-05-24 09:59:42.000000 ansar_create-0.1.95/src/ansar/create/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2654 2023-07-13 04:39:47.000000 ansar_create-0.1.95/src/ansar/create/binding.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1989 2023-12-23 01:56:16.000000 ansar_create-0.1.95/src/ansar/create/coding.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1857 2024-01-19 15:16:48.000000 ansar_create-0.1.95/src/ansar/create/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    13837 2024-02-24 20:57:36.000000 ansar_create-0.1.95/src/ansar/create/home.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3590 2024-05-22 18:42:10.000000 ansar_create-0.1.95/src/ansar/create/latching.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7383 2024-03-24 15:57:41.000000 ansar_create-0.1.95/src/ansar/create/lifecycle.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     4061 2024-01-25 13:13:42.000000 ansar_create-0.1.95/src/ansar/create/locking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6164 2023-07-13 04:40:10.000000 ansar_create-0.1.95/src/ansar/create/log.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8495 2023-07-13 04:40:11.000000 ansar_create-0.1.95/src/ansar/create/machine.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    31879 2024-05-24 09:57:14.000000 ansar_create-0.1.95/src/ansar/create/object.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9071 2024-01-18 15:23:10.000000 ansar_create-0.1.95/src/ansar/create/pending.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    29529 2024-05-14 22:01:16.000000 ansar_create-0.1.95/src/ansar/create/point.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    80287 2024-05-14 16:43:56.000000 ansar_create-0.1.95/src/ansar/create/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    31841 2024-01-22 04:26:11.000000 ansar_create-0.1.95/src/ansar/create/processing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3099 2024-03-26 19:19:48.000000 ansar_create-0.1.95/src/ansar/create/properties.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3741 2024-03-07 07:59:16.000000 ansar_create-0.1.95/src/ansar/create/retry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5938 2024-02-27 14:04:16.000000 ansar_create-0.1.95/src/ansar/create/rolling.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7477 2023-12-23 15:53:02.000000 ansar_create-0.1.95/src/ansar/create/root.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14309 2024-05-22 19:30:42.000000 ansar_create-0.1.95/src/ansar/create/space.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    19885 2024-05-24 06:04:53.000000 ansar_create-0.1.95/src/ansar/create/storage.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3959 2024-01-15 15:55:19.000000 ansar_create-0.1.95/src/ansar/create/test.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5100 2024-01-26 08:38:29.000000 ansar_create-0.1.95/src/ansar/create/timing.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 09:59:45.976550 ansar_create-0.1.95/src/ansar_create.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-24 09:59:45.000000 ansar_create-0.1.95/src/ansar_create.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      986 2024-05-24 09:59:45.000000 ansar_create-0.1.95/src/ansar_create.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-24 09:59:45.000000 ansar_create-0.1.95/src/ansar_create.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      104 2024-05-24 09:59:45.000000 ansar_create-0.1.95/src/ansar_create.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       22 2024-05-24 09:59:45.000000 ansar_create-0.1.95/src/ansar_create.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-24 09:59:45.000000 ansar_create-0.1.95/src/ansar_create.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 13:35:05.755682 ansar_create-0.1.96/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:18.000000 ansar_create-0.1.96/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-24 13:35:05.755682 ansar_create-0.1.96/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      901 2023-06-17 21:18:11.000000 ansar_create-0.1.96/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      718 2024-05-22 01:10:14.000000 ansar_create-0.1.96/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-24 13:35:05.755682 ansar_create-0.1.96/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2139 2024-05-22 01:10:05.000000 ansar_create-0.1.96/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 13:35:05.751682 ansar_create-0.1.96/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 13:35:05.751682 ansar_create-0.1.96/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 13:35:05.751682 ansar_create-0.1.96/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13081 2024-01-02 02:57:04.000000 ansar_create-0.1.96/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8950 2024-02-25 02:39:34.000000 ansar_create-0.1.96/src/ansar/command/ansar_group.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 13:35:05.755682 ansar_create-0.1.96/src/ansar/create/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5706 2024-05-24 13:35:02.000000 ansar_create-0.1.96/src/ansar/create/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2654 2023-07-13 04:39:47.000000 ansar_create-0.1.96/src/ansar/create/binding.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1989 2023-12-23 01:56:16.000000 ansar_create-0.1.96/src/ansar/create/coding.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1857 2024-01-19 15:16:48.000000 ansar_create-0.1.96/src/ansar/create/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13837 2024-02-24 20:57:36.000000 ansar_create-0.1.96/src/ansar/create/home.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3590 2024-05-22 18:42:10.000000 ansar_create-0.1.96/src/ansar/create/latching.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7383 2024-03-24 15:57:41.000000 ansar_create-0.1.96/src/ansar/create/lifecycle.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4061 2024-01-25 13:13:42.000000 ansar_create-0.1.96/src/ansar/create/locking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6164 2023-07-13 04:40:10.000000 ansar_create-0.1.96/src/ansar/create/log.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8495 2023-07-13 04:40:11.000000 ansar_create-0.1.96/src/ansar/create/machine.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32000 2024-05-24 13:33:12.000000 ansar_create-0.1.96/src/ansar/create/object.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9071 2024-01-18 15:23:10.000000 ansar_create-0.1.96/src/ansar/create/pending.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    29529 2024-05-14 22:01:16.000000 ansar_create-0.1.96/src/ansar/create/point.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    80287 2024-05-14 16:43:56.000000 ansar_create-0.1.96/src/ansar/create/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    31841 2024-01-22 04:26:11.000000 ansar_create-0.1.96/src/ansar/create/processing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3099 2024-03-26 19:19:48.000000 ansar_create-0.1.96/src/ansar/create/properties.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3741 2024-03-07 07:59:16.000000 ansar_create-0.1.96/src/ansar/create/retry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5938 2024-02-27 14:04:16.000000 ansar_create-0.1.96/src/ansar/create/rolling.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7477 2023-12-23 15:53:02.000000 ansar_create-0.1.96/src/ansar/create/root.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14309 2024-05-22 19:30:42.000000 ansar_create-0.1.96/src/ansar/create/space.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    19885 2024-05-24 06:04:53.000000 ansar_create-0.1.96/src/ansar/create/storage.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3959 2024-01-15 15:55:19.000000 ansar_create-0.1.96/src/ansar/create/test.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5100 2024-01-26 08:38:29.000000 ansar_create-0.1.96/src/ansar/create/timing.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-24 13:35:05.755682 ansar_create-0.1.96/src/ansar_create.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-24 13:35:05.000000 ansar_create-0.1.96/src/ansar_create.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      986 2024-05-24 13:35:05.000000 ansar_create-0.1.96/src/ansar_create.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-24 13:35:05.000000 ansar_create-0.1.96/src/ansar_create.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      104 2024-05-24 13:35:05.000000 ansar_create-0.1.96/src/ansar_create.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       22 2024-05-24 13:35:05.000000 ansar_create-0.1.96/src/ansar_create.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-24 13:35:05.000000 ansar_create-0.1.96/src/ansar_create.egg-info/top_level.txt
```

### Comparing `ansar_create-0.1.95/LICENSE` & `ansar_create-0.1.96/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/PKG-INFO` & `ansar_create-0.1.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-create
-Version: 0.1.95
+Version: 0.1.96
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com>
 Project-URL: Documentation, https://ansar-create-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_create-0.1.95/README.md` & `ansar_create-0.1.96/README.md`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/pyproject.toml` & `ansar_create-0.1.96/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/setup.py` & `ansar_create-0.1.96/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/command/ansar_command.py` & `ansar_create-0.1.96/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/command/ansar_group.py` & `ansar_create-0.1.96/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/__init__.py` & `ansar_create-0.1.96/src/ansar/create/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-create.git
 Branch: main
-Commit: 12d75a5ba43b53bb92c192bd732dce0acf08a8ac
-Version: 0.1.94 (2024-05-24@21:59:42+NZST)
+Commit: 10ca442ee728473db3706a50fa7043064952ab92
+Version: 0.1.95 (2024-05-25@01:35:02+NZST)
 """
 
 from ansar.encode import *
 
 from .coding import cannot, lor
 from .space import NO_SUCH_ADDRESS
 from .space import create_an_object, find_object, destroy_an_object
```

### Comparing `ansar_create-0.1.95/src/ansar/create/binding.py` & `ansar_create-0.1.96/src/ansar/create/binding.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/coding.py` & `ansar_create-0.1.96/src/ansar/create/coding.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/grouping.py` & `ansar_create-0.1.96/src/ansar/create/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/home.py` & `ansar_create-0.1.96/src/ansar/create/home.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/latching.py` & `ansar_create-0.1.96/src/ansar/create/latching.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/lifecycle.py` & `ansar_create-0.1.96/src/ansar/create/lifecycle.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/locking.py` & `ansar_create-0.1.96/src/ansar/create/locking.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/log.py` & `ansar_create-0.1.96/src/ansar/create/log.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/machine.py` & `ansar_create-0.1.96/src/ansar/create/machine.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/object.py` & `ansar_create-0.1.96/src/ansar/create/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,14 +385,81 @@
 		r2,				 # Remainder from ls2, i.e. for passing to sub-component
 		word)			   # Non-flag arguments.
 
 	return executable, bundle, r1
 
 #
 #
+# OS_NAME = os.name
+# PLATFORM_RELEASE = platform.release()
+PLATFORM_SYSTEM = platform.system()
+
+if PLATFORM_SYSTEM.startswith('Linux'):
+	def platform_signal():
+		signal.signal(signal.SIGINT, catch_interrupt)
+		signal.signal(signal.SIGQUIT, interrupt_alias)
+		signal.signal(signal.SIGHUP, interrupt_alias)
+		signal.signal(signal.SIGTERM, interrupt_alias)
+
+		signal.signal(signal.SIGCHLD, ignore_signal)
+		signal.signal(signal.SIGTRAP, log_signal)
+		signal.signal(signal.SIGABRT, log_signal)
+		#signal.signal(signal.SIGKILL, log_signal)	... cant be caught.
+
+		signal.signal(signal.SIGPIPE, log_signal)
+		signal.signal(signal.SIGUSR1, catch_interrupt)
+		signal.signal(signal.SIGUSR2, catch_interrupt)
+		signal.signal(signal.SIGALRM, log_signal)
+		signal.signal(signal.SIGTTIN, log_signal)
+		#signal.signal(signal.SIGSTOP, log_signal)	... ditto.
+		signal.signal(signal.SIGTSTP, log_signal)
+		signal.signal(signal.SIGPWR, log_signal)
+	SIGNAL_KILL = signal.SIGKILL
+elif PLATFORM_SYSTEM == 'Darwin':
+	def platform_signal():
+		signal.signal(signal.SIGINT, catch_interrupt)
+		signal.signal(signal.SIGQUIT, interrupt_alias)
+		signal.signal(signal.SIGHUP, interrupt_alias)
+		signal.signal(signal.SIGTERM, interrupt_alias)
+
+		signal.signal(signal.SIGCHLD, ignore_signal)
+		signal.signal(signal.SIGTRAP, log_signal)
+		signal.signal(signal.SIGABRT, log_signal)
+		#signal.signal(signal.SIGKILL, log_signal)	... cant be caught.
+
+		signal.signal(signal.SIGPIPE, log_signal)
+		signal.signal(signal.SIGUSR1, catch_interrupt)
+		signal.signal(signal.SIGUSR2, catch_interrupt)
+		signal.signal(signal.SIGALRM, log_signal)
+		signal.signal(signal.SIGTTIN, log_signal)
+		#signal.signal(signal.SIGSTOP, log_signal)	... ditto.
+		signal.signal(signal.SIGTSTP, log_signal)
+		#signal.signal(signal.SIGPWR, log_signal)
+	SIGNAL_KILL = signal.SIGKILL
+else:
+	def platform_signal():
+		signal.signal(signal.SIGINT, catch_interrupt)
+		#signal.signal(signal.SIGBREAK, log_signal)		... cant be caught
+		#signal.signal(signal.SIGQUIT, interrupt_alias)	... not in windows
+		#signal.signal(signal.SIGHUP, interrupt_alias)
+		signal.signal(signal.SIGTERM, catch_interrupt)
+		signal.signal(signal.SIGFPE, interrupt_alias)
+		#signal.signal(signal.SIGCHLD, ignore_signal)
+		#signal.signal(signal.SIGTRAP, log_signal)
+		signal.signal(signal.SIGABRT, log_signal)
+		#signal.signal(signal.SIGKILL, log_signal)	... cant be caught.
+		#signal.signal(signal.SIGPIPE, log_signal)
+		#signal.signal(signal.SIGUSR1, catch_interrupt)
+		#signal.signal(signal.SIGUSR2, catch_interrupt)
+		#signal.signal(signal.SIGALRM, log_signal)
+		#signal.signal(signal.SIGTTIN, log_signal)
+		#signal.signal(signal.SIGSTOP, log_signal)	... ditto.
+		#signal.signal(signal.SIGTSTP, log_signal)
+	SIGNAL_KILL = signal.SIGBREAK
+
 def object_vector(self, object_type, settings, input, variables, fixed_value, key_value):
 	name_counts = ['"%s" (%d)' % (k, len(v)) for k, v in pt.thread_classes.items()]
 
 	executable = os.path.abspath(sys.argv[0])
 	self.trace('Executable "%s" as object process (%d)' % (executable, os.getpid()))
 	self.trace('Working folder "%s"' % (os.getcwd()))
 	self.trace('Running object "%s"' % (object_type.__art__.path,))
@@ -413,15 +480,15 @@
 		m = self.select(Completed, Stop, Pause, Resume)
 
 		if isinstance(m, Completed):
 			# Do a "fake" signaling. Sidestep all the platform machinery
 			# and just set a global. It does avoid any complexities
 			# arising from overlapping events. Spent far too much time
 			# trying to untangle signals, exceptions and interrupted i/o.
-			co.signal_received = signal.SIGINT
+			co.signal_received = SIGNAL_KILL
 			return m.value
 		elif isinstance(m, Stop):
 			# Received a Stop.
 			self.send(m, a)
 			m = self.select(Completed)
 			return m.value
 		
@@ -661,74 +728,14 @@
 			logs = select_logs(object_settings.debug_level)
 	except ar.CommandError as e:
 		f = ar.Failed(logs_open=(e, None))
 		raise ar.Incomplete(f)
 
 	return logs
 
-OS_NAME = os.name
-PLATFORM_SYSTEM = platform.system()
-PLATFORM_RELEASE = platform.release()
-
-if PLATFORM_SYSTEM.startswith('Linux'):
-	def platform_signal():
-		signal.signal(signal.SIGINT, catch_interrupt)
-		signal.signal(signal.SIGQUIT, interrupt_alias)
-		signal.signal(signal.SIGHUP, interrupt_alias)
-		signal.signal(signal.SIGTERM, interrupt_alias)
-		signal.signal(signal.SIGCHLD, ignore_signal)
-		signal.signal(signal.SIGTRAP, log_signal)
-		signal.signal(signal.SIGABRT, log_signal)
-		#signal.signal(signal.SIGKILL, log_signal)	... cant be caught.
-		signal.signal(signal.SIGPIPE, log_signal)
-		signal.signal(signal.SIGUSR1, catch_interrupt)
-		signal.signal(signal.SIGUSR2, catch_interrupt)
-		signal.signal(signal.SIGALRM, log_signal)
-		signal.signal(signal.SIGTTIN, log_signal)
-		#signal.signal(signal.SIGSTOP, log_signal)	... ditto.
-		signal.signal(signal.SIGTSTP, log_signal)
-		signal.signal(signal.SIGPWR, log_signal)
-elif PLATFORM_SYSTEM == 'Darwin':
-	def platform_signal():
-		signal.signal(signal.SIGINT, catch_interrupt)
-		signal.signal(signal.SIGQUIT, interrupt_alias)
-		signal.signal(signal.SIGHUP, interrupt_alias)
-		signal.signal(signal.SIGTERM, interrupt_alias)
-		signal.signal(signal.SIGCHLD, ignore_signal)
-		signal.signal(signal.SIGTRAP, log_signal)
-		signal.signal(signal.SIGABRT, log_signal)
-		#signal.signal(signal.SIGKILL, log_signal)	... cant be caught.
-		signal.signal(signal.SIGPIPE, log_signal)
-		signal.signal(signal.SIGUSR1, catch_interrupt)
-		signal.signal(signal.SIGUSR2, catch_interrupt)
-		signal.signal(signal.SIGALRM, log_signal)
-		signal.signal(signal.SIGTTIN, log_signal)
-		#signal.signal(signal.SIGSTOP, log_signal)	... ditto.
-		signal.signal(signal.SIGTSTP, log_signal)
-		#signal.signal(signal.SIGPWR, log_signal)
-else:
-	def platform_signal():
-		signal.signal(signal.SIGINT, catch_interrupt)
-		signal.signal(signal.SIGBREAK, interrupt_alias)
-		#signal.signal(signal.SIGQUIT, interrupt_alias)
-		#signal.signal(signal.SIGHUP, interrupt_alias)
-		signal.signal(signal.SIGTERM, catch_interrupt)
-		signal.signal(signal.SIGFPE, interrupt_alias)
-		#signal.signal(signal.SIGCHLD, ignore_signal)
-		#signal.signal(signal.SIGTRAP, log_signal)
-		signal.signal(signal.SIGABRT, log_signal)
-		#signal.signal(signal.SIGKILL, log_signal)	... cant be caught.
-		#signal.signal(signal.SIGPIPE, log_signal)
-		#signal.signal(signal.SIGUSR1, catch_interrupt)
-		#signal.signal(signal.SIGUSR2, catch_interrupt)
-		#signal.signal(signal.SIGALRM, log_signal)
-		#signal.signal(signal.SIGTTIN, log_signal)
-		#signal.signal(signal.SIGSTOP, log_signal)	... ditto.
-		#signal.signal(signal.SIGTSTP, log_signal)
-
 def is_signal(a, s):
 	v = getattr(signal, a, None)
 	if v is None:
 		return False
 	return v == s
 
 def run_object(start_vector, object_type, settings, input, variables, fixed_value, role, logs, homed, point_of_origin, key_value):
@@ -779,17 +786,17 @@
 			while co.signal_received is None:
 				time.sleep(0.1)
 				#signal.pause()
 			sr, co.signal_received = co.signal_received, None
 
 			# If it was keyboard then async object needs
 			# to be bumped.
-			if is_signal('SIGKILL', sr):
+			if sr == SIGNAL_KILL:
 				running = False
-			elif is_signal('SIGINT', sr):
+			elif sr == signal.SIGINT:
 				root.send(Stop(), a)
 				running = False
 			elif is_signal('SIGUSR1', sr):
 				root.send(Pause(), a)
 			elif is_signal('SIGUSR2', sr):
 				root.send(Resume(), a)
```

### Comparing `ansar_create-0.1.95/src/ansar/create/pending.py` & `ansar_create-0.1.96/src/ansar/create/pending.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/point.py` & `ansar_create-0.1.96/src/ansar/create/point.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/procedure.py` & `ansar_create-0.1.96/src/ansar/create/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/processing.py` & `ansar_create-0.1.96/src/ansar/create/processing.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/properties.py` & `ansar_create-0.1.96/src/ansar/create/properties.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/retry.py` & `ansar_create-0.1.96/src/ansar/create/retry.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/rolling.py` & `ansar_create-0.1.96/src/ansar/create/rolling.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/root.py` & `ansar_create-0.1.96/src/ansar/create/root.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/space.py` & `ansar_create-0.1.96/src/ansar/create/space.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/storage.py` & `ansar_create-0.1.96/src/ansar/create/storage.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/test.py` & `ansar_create-0.1.96/src/ansar/create/test.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar/create/timing.py` & `ansar_create-0.1.96/src/ansar/create/timing.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.95/src/ansar_create.egg-info/PKG-INFO` & `ansar_create-0.1.96/src/ansar_create.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-create
-Version: 0.1.95
+Version: 0.1.96
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com>
 Project-URL: Documentation, https://ansar-create-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_create-0.1.95/src/ansar_create.egg-info/SOURCES.txt` & `ansar_create-0.1.96/src/ansar_create.egg-info/SOURCES.txt`

 * *Files identical despite different names*

