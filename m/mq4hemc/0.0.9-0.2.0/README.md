# Comparing `tmp/mq4hemc-0.0.9.tar.gz` & `tmp/mq4hemc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mq4hemc-0.0.9.tar", last modified: Thu May  2 15:54:45 2024, max compression
+gzip compressed data, was "mq4hemc-0.2.0.tar", last modified: Fri May 24 12:30:36 2024, max compression
```

## Comparing `mq4hemc-0.0.9.tar` & `mq4hemc-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-02 15:54:45.056076 mq4hemc-0.0.9/
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     3101 2024-05-02 12:01:36.000000 mq4hemc-0.0.9/.gitignore
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     1077 2024-04-30 09:39:00.000000 mq4hemc-0.0.9/LICENSE
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      952 2024-05-02 15:49:59.000000 mq4hemc-0.0.9/Makefile
--rw-r--r--   0 oshevchenko  (1000) oshevchenko  (1000)     3444 2024-05-02 15:54:45.056076 mq4hemc-0.0.9/PKG-INFO
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     2954 2024-05-02 11:59:52.000000 mq4hemc-0.0.9/README.md
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      244 2024-05-02 09:34:00.000000 mq4hemc-0.0.9/poetry.lock
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      161 2024-05-02 15:48:47.000000 mq4hemc-0.0.9/pyproject.toml
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      672 2024-05-02 14:23:44.000000 mq4hemc-0.0.9/pyproject.toml.in
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      659 2024-05-02 09:41:02.000000 mq4hemc-0.0.9/requirements.txt
-drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-02 15:54:45.052076 mq4hemc-0.0.9/scripts/
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     1120 2024-05-02 15:29:08.000000 mq4hemc-0.0.9/scripts/generate-pyproject.py
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      632 2024-05-02 15:54:45.056076 mq4hemc-0.0.9/setup.cfg
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)       38 2024-05-02 15:33:15.000000 mq4hemc-0.0.9/setup.py
-drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-02 15:54:45.052076 mq4hemc-0.0.9/src/
-drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-02 15:54:45.052076 mq4hemc-0.0.9/src/mq4hemc/
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      155 2024-05-02 08:01:43.000000 mq4hemc-0.0.9/src/mq4hemc/__init__.py
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     1215 2024-05-02 08:02:58.000000 mq4hemc-0.0.9/src/mq4hemc/hemc_observer.py
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     3973 2024-05-02 08:22:35.000000 mq4hemc-0.0.9/src/mq4hemc/hemc_queue.py
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     1752 2024-05-02 08:04:40.000000 mq4hemc-0.0.9/src/mq4hemc/hemc_service.py
-drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-02 15:54:45.056076 mq4hemc-0.0.9/src/mq4hemc.egg-info/
--rw-r--r--   0 oshevchenko  (1000) oshevchenko  (1000)     3444 2024-05-02 15:54:45.000000 mq4hemc-0.0.9/src/mq4hemc.egg-info/PKG-INFO
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      484 2024-05-02 15:54:45.000000 mq4hemc-0.0.9/src/mq4hemc.egg-info/SOURCES.txt
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)        1 2024-05-02 15:54:45.000000 mq4hemc-0.0.9/src/mq4hemc.egg-info/dependency_links.txt
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)        8 2024-05-02 15:54:45.000000 mq4hemc-0.0.9/src/mq4hemc.egg-info/top_level.txt
-drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-02 15:54:45.056076 mq4hemc-0.0.9/tests/
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     3728 2024-05-02 11:23:22.000000 mq4hemc-0.0.9/tests/test_mq4hemc.py
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     2807 2024-05-02 11:22:48.000000 mq4hemc-0.0.9/tests/test_observer.py
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     1747 2024-05-02 11:39:26.000000 mq4hemc-0.0.9/tests/test_readme.py
--rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     3588 2024-05-02 11:23:02.000000 mq4hemc-0.0.9/tests/test_real_use.py
+drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-24 12:30:36.037952 mq4hemc-0.2.0/
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     3108 2024-05-03 09:20:46.000000 mq4hemc-0.2.0/.gitignore
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     1077 2024-05-03 09:20:46.000000 mq4hemc-0.2.0/LICENSE
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      968 2024-05-24 12:20:45.000000 mq4hemc-0.2.0/Makefile
+-rw-r--r--   0 oshevchenko  (1000) oshevchenko  (1000)     4413 2024-05-24 12:30:36.037952 mq4hemc-0.2.0/PKG-INFO
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     3882 2024-05-03 15:34:53.000000 mq4hemc-0.2.0/README.md
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      202 2024-05-03 09:20:46.000000 mq4hemc-0.2.0/pyproject.toml
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      659 2024-05-03 09:43:10.000000 mq4hemc-0.2.0/requirements.txt
+drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-24 12:30:36.037952 mq4hemc-0.2.0/scripts/
+-rwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)      702 2024-05-03 09:20:46.000000 mq4hemc-0.2.0/scripts/create_setup_py.sh
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     1120 2024-05-03 09:20:46.000000 mq4hemc-0.2.0/scripts/generate-pyproject.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      634 2024-05-24 12:30:36.037952 mq4hemc-0.2.0/setup.cfg
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     2565 2024-05-03 15:16:04.000000 mq4hemc-0.2.0/setup_git.txt
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      583 2024-05-03 15:11:46.000000 mq4hemc-0.2.0/setup_pypi.txt
+drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-24 12:30:36.033952 mq4hemc-0.2.0/src/
+drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-24 12:30:36.037952 mq4hemc-0.2.0/src/mq4hemc/
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      192 2024-05-24 12:20:45.000000 mq4hemc-0.2.0/src/mq4hemc/__init__.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      411 2024-05-24 12:30:35.000000 mq4hemc-0.2.0/src/mq4hemc/_version.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     2161 2024-05-24 12:20:45.000000 mq4hemc-0.2.0/src/mq4hemc/hemc_observer.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     3973 2024-05-24 12:20:45.000000 mq4hemc-0.2.0/src/mq4hemc/hemc_queue.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     1741 2024-05-07 05:45:05.000000 mq4hemc-0.2.0/src/mq4hemc/hemc_service.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      647 2024-05-07 06:56:49.000000 mq4hemc-0.2.0/src/mq4hemc/hemc_tick.py
+drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-24 12:30:36.037952 mq4hemc-0.2.0/src/mq4hemc.egg-info/
+-rw-r--r--   0 oshevchenko  (1000) oshevchenko  (1000)     4413 2024-05-24 12:30:36.000000 mq4hemc-0.2.0/src/mq4hemc.egg-info/PKG-INFO
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)      550 2024-05-24 12:30:36.000000 mq4hemc-0.2.0/src/mq4hemc.egg-info/SOURCES.txt
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)        1 2024-05-24 12:30:36.000000 mq4hemc-0.2.0/src/mq4hemc.egg-info/dependency_links.txt
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)        8 2024-05-24 12:30:36.000000 mq4hemc-0.2.0/src/mq4hemc.egg-info/top_level.txt
+drwxrwxr-x   0 oshevchenko  (1000) oshevchenko  (1000)        0 2024-05-24 12:30:36.037952 mq4hemc-0.2.0/tests/
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     3728 2024-05-03 09:20:46.000000 mq4hemc-0.2.0/tests/test_mq4hemc.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     4594 2024-05-07 05:45:05.000000 mq4hemc-0.2.0/tests/test_observer.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     2754 2024-05-07 06:58:52.000000 mq4hemc-0.2.0/tests/test_readme.py
+-rw-rw-r--   0 oshevchenko  (1000) oshevchenko  (1000)     3588 2024-05-03 09:20:46.000000 mq4hemc-0.2.0/tests/test_real_use.py
```

### Comparing `mq4hemc-0.0.9/.gitignore` & `mq4hemc-0.2.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -155,8 +155,10 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 .vscode
-pyproject.toml
+_version.py
+setup.py
+
```

### Comparing `mq4hemc-0.0.9/LICENSE` & `mq4hemc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mq4hemc-0.0.9/Makefile` & `mq4hemc-0.2.0/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 	$(VENV_BIN_PATH)/python3 -m pip install --upgrade pip
 	$(VENV_BIN_PATH)/python3 -m pip install -r requirements.txt
 	$(VENV_BIN_PATH)/python3 -m pip install --upgrade build
 	$(VENV_BIN_PATH)/python3 -m pip install --upgrade twine
 
 build:
 	rm -rf dist
+	rm -f setup.py
 	$(VENV_BIN_PATH)/python3 -m build
 
 build_old:
 	rm -rf dist
 	rm -f pyproject.toml
 	$(VENV_BIN_PATH)/python3 ./scripts/generate-pyproject.py pyproject.setup.toml.in
 	$(VENV_BIN_PATH)/python3 -m build
```

### Comparing `mq4hemc-0.0.9/PKG-INFO` & `mq4hemc-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,20 @@
-Metadata-Version: 2.1
-Name: mq4hemc
-Version: 0.0.9
-Summary: Message Queue related Python library
-Home-page: https://github.com/oshevchenko/mq4hemc
-Author: Oleksandr Shevchenko
-Author-email: shevchenko.adb@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Message Queue Based Service
 ```py
 from mq4hemc import HemcMessage, HemcService
 ```
 `HemcService` - a class to create a separate thread which is extracting messages
 from the message queue and passes them to user callback for processing.
 It has a thread-safe methods to add messages to the queue synchronously
 (wait until processed) and asynchronously.
 
 
 `HemcMessage` - a dataclass to inherit from to create a custom message.
 
-## Example of usage
+## Usage
 Define a custom class for the messages:
 ```py
 @dataclass
 class BigHemcMessage(HemcMessage):
     payload: dict = field(default_factory=dict)
 ```
 Create a service which is running in a separate thread and processes
@@ -89,7 +74,45 @@
 2024-05-02 14:39:29 - test_mq4hemc - INFO - Processed message 'test0'
 2024-05-02 14:39:30 - test_mq4hemc - INFO - Processed message 'test1'
 2024-05-02 14:39:31 - test_mq4hemc - INFO - Processed message 'test2'
 2024-05-02 14:39:32 - test_mq4hemc - INFO - Processed message 'test_sync'
 2024-05-02 14:39:32 - test_mq4hemc - INFO - Message test_sync processed, reply: test_sync
 2024-05-02 14:39:32 - test_mq4hemc - INFO - Service stopped.
 ```
+## Yocto recipes
+Use the following bitbake recipes `python3-mq4hemc_0.0.20.bb` to install **mq4hemc** package:
+
+### From github.com:
+```
+DESCRIPTION = "Message Queue Based Service"
+HOMEPAGE = "https://github.com/oshevchenko/mq4hemc"
+LICENSE = "MIT"
+LIC_FILES_CHKSUM = "file://LICENSE;md5=bd6d2057bbfc3f9442bc4dfd9a7c4580"
+
+SRC_URI = "git://github.com/oshevchenko/mq4hemc.git;protocol=https"
+SRCREV = "75a10cfbf3e16c6a2491b2295d4d4d63f4a952f1"
+
+S = "${WORKDIR}/git"
+
+inherit setuptools3
+
+do_configure:prepend() {
+    cp ${S}/setup_git.txt ${S}/setup.py
+}
+```
+### From PyPi
+```
+DESCRIPTION = "Message Queue Based Service"
+HOMEPAGE = "https://github.com/oshevchenko/mq4hemc"
+LICENSE = "MIT"
+LIC_FILES_CHKSUM = "file://LICENSE;md5=bd6d2057bbfc3f9442bc4dfd9a7c4580"
+
+PYPI_PACKAGE = "mq4hemc"
+
+SRC_URI[md5sum] = "5317fbdc5cc857b70f622005730ef66f"
+
+inherit pypi setuptools3
+
+do_configure:prepend() {
+    cp ${S}/setup_pypi.txt ${S}/setup.py
+}
+```
```

### Comparing `mq4hemc-0.0.9/requirements.txt` & `mq4hemc-0.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `mq4hemc-0.0.9/scripts/generate-pyproject.py` & `mq4hemc-0.2.0/scripts/generate-pyproject.py`

 * *Files identical despite different names*

### Comparing `mq4hemc-0.0.9/src/mq4hemc/hemc_queue.py` & `mq4hemc-0.2.0/src/mq4hemc/hemc_queue.py`

 * *Files identical despite different names*

### Comparing `mq4hemc-0.0.9/src/mq4hemc/hemc_service.py` & `mq4hemc-0.2.0/src/mq4hemc/hemc_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,53 @@
 import threading
 from mq4hemc import HemcQueue, HemcQueueSender, HemcMessage
 
+
 class HemcService(threading.Thread):
-    def __init__(self, process_cb = None):
+    def __init__(self, process_cb=None):
         # Initialize the message queue
-        self._message_queue = HemcQueue(process_item_cb = self._process_item)
+        self._message_queue = HemcQueue(process_item_cb=self._process_item)
         self._running = False
         self._process_cb = None
         if process_cb is not None:
             if not callable(process_cb):
                 raise ValueError("process_cb must be a callable function!")
             self._process_cb = process_cb
         threading.Thread.__init__(self)
 
-
     def _process_item(self, item: HemcMessage):
         ret = None
         if item.type != "__stop__" and self._process_cb is not None:
             ret = self._process_cb(item)
         return ret
 
-
     def _get_sender(self):
         return HemcQueueSender(self._message_queue)
 
-
     def start(self) -> None:
         if self._running:
             return
         self._running = True
         return super().start()
 
-
     def send_sync_msg(self, message: HemcMessage):
         return self._get_sender().send_wait_reply(message)
 
-
     def send_async_msg(self, message: HemcMessage):
         return self._get_sender().send(message)
 
-
     def stop(self):
         self._running = False
         message = HemcMessage()
         message.type = "__stop__"
         self.send_async_msg(message)
 
-
     def register_process_cb(self, process_cb):
         if not callable(process_cb):
             raise ValueError("process_cb must be a callable function!")
         self._process_cb = process_cb
 
-
     def run(self):
         # The main execution loop of the thread.
         while self._running:
             # Get message from the queue and process it
             self._message_queue.get_process()
```

### Comparing `mq4hemc-0.0.9/tests/test_mq4hemc.py` & `mq4hemc-0.2.0/tests/test_mq4hemc.py`

 * *Files identical despite different names*

### Comparing `mq4hemc-0.0.9/tests/test_real_use.py` & `mq4hemc-0.2.0/tests/test_real_use.py`

 * *Files identical despite different names*

