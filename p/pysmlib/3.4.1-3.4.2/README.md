# Comparing `tmp/pysmlib-3.4.1.tar.gz` & `tmp/pysmlib-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmlib-3.4.1.tar", last modified: Tue Feb 14 14:51:00 2023, max compression
+gzip compressed data, was "pysmlib-3.4.2.tar", last modified: Fri May 24 08:45:33 2024, max compression
```

## Comparing `pysmlib-3.4.1.tar` & `pysmlib-3.4.2.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxrwxr-x   0 marcato   (1000) marcato   (1000)        0 2023-02-14 14:51:00.352615 pysmlib-3.4.1/
--rw-rw-r--   0 marcato   (1000) marcato   (1000)    35041 2020-03-20 14:41:04.000000 pysmlib-3.4.1/LICENSE.txt
--rw-rw-r--   0 marcato   (1000) marcato   (1000)       48 2020-03-20 14:41:04.000000 pysmlib-3.4.1/MANIFEST.in
--rw-rw-r--   0 marcato   (1000) marcato   (1000)     1722 2023-02-14 14:51:00.352615 pysmlib-3.4.1/PKG-INFO
--rw-r--r--   0 marcato   (1000) marcato   (1000)     1329 2023-01-20 14:57:15.000000 pysmlib-3.4.1/README.md
-drwxrwxr-x   0 marcato   (1000) marcato   (1000)        0 2023-02-14 14:51:00.352615 pysmlib-3.4.1/pysmlib.egg-info/
--rw-rw-r--   0 marcato   (1000) marcato   (1000)     1722 2023-02-14 14:51:00.000000 pysmlib-3.4.1/pysmlib.egg-info/PKG-INFO
--rw-rw-r--   0 marcato   (1000) marcato   (1000)      400 2023-02-14 14:51:00.000000 pysmlib-3.4.1/pysmlib.egg-info/SOURCES.txt
--rw-rw-r--   0 marcato   (1000) marcato   (1000)        1 2023-02-14 14:51:00.000000 pysmlib-3.4.1/pysmlib.egg-info/dependency_links.txt
--rw-rw-r--   0 marcato   (1000) marcato   (1000)        1 2018-03-19 16:43:19.000000 pysmlib-3.4.1/pysmlib.egg-info/not-zip-safe
--rw-rw-r--   0 marcato   (1000) marcato   (1000)        8 2023-02-14 14:51:00.000000 pysmlib-3.4.1/pysmlib.egg-info/requires.txt
--rw-rw-r--   0 marcato   (1000) marcato   (1000)        6 2023-02-14 14:51:00.000000 pysmlib-3.4.1/pysmlib.egg-info/top_level.txt
--rw-rw-r--   0 marcato   (1000) marcato   (1000)      223 2023-02-14 14:51:00.352615 pysmlib-3.4.1/setup.cfg
--rw-r--r--   0 marcato   (1000) marcato   (1000)     1105 2020-10-29 16:26:39.000000 pysmlib-3.4.1/setup.py
-drwxrwxr-x   0 marcato   (1000) marcato   (1000)        0 2023-02-14 14:51:00.352615 pysmlib-3.4.1/smlib/
--rw-r--r--   0 marcato   (1000) marcato   (1000)     1490 2023-01-18 18:32:43.000000 pysmlib-3.4.1/smlib/__init__.py
--rw-rw-r--   0 marcato   (1000) marcato   (1000)    18445 2020-03-20 14:41:04.000000 pysmlib-3.4.1/smlib/_version.py
--rw-r--r--   0 marcato   (1000) marcato   (1000)    11471 2023-02-03 12:19:49.000000 pysmlib-3.4.1/smlib/fsm.py
--rw-r--r--   0 marcato   (1000) marcato   (1000)     1709 2023-02-03 09:31:55.000000 pysmlib-3.4.1/smlib/fsmTemplate.py
--rw-r--r--   0 marcato   (1000) marcato   (1000)     1952 2023-01-18 16:11:03.000000 pysmlib-3.4.1/smlib/fsmWatchdog.py
--rw-rw-r--   0 marcato   (1000) marcato   (1000)    24106 2023-01-20 10:35:46.000000 pysmlib-3.4.1/smlib/io.py
--rw-rw-r--   0 marcato   (1000) marcato   (1000)     3693 2023-01-18 16:14:08.000000 pysmlib-3.4.1/smlib/loader.py
--rw-r--r--   0 marcato   (1000) marcato   (1000)     1969 2023-01-18 16:18:20.000000 pysmlib-3.4.1/smlib/logger.py
--rw-r--r--   0 marcato   (1000) marcato   (1000)     5498 2023-01-20 10:38:13.000000 pysmlib-3.4.1/smlib/timer.py
--rw-rw-r--   0 marcato   (1000) marcato   (1000)    68611 2020-03-20 14:41:04.000000 pysmlib-3.4.1/versioneer.py
+drwxrwxr-x   0 marcato   (1000) marcato   (1000)        0 2024-05-24 08:45:33.981943 pysmlib-3.4.2/
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)    35041 2018-03-06 21:02:33.000000 pysmlib-3.4.2/LICENSE.txt
+-rw-r--r--   0 marcato   (1000) marcato   (1000)       48 2020-03-20 13:10:18.000000 pysmlib-3.4.2/MANIFEST.in
+-rw-r--r--   0 marcato   (1000) marcato   (1000)     1745 2024-05-24 08:45:33.981943 pysmlib-3.4.2/PKG-INFO
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)     1329 2024-05-24 08:22:35.000000 pysmlib-3.4.2/README.md
+drwxrwxr-x   0 marcato   (1000) marcato   (1000)        0 2024-05-24 08:45:33.981943 pysmlib-3.4.2/pysmlib.egg-info/
+-rw-r--r--   0 marcato   (1000) marcato   (1000)     1745 2024-05-24 08:45:33.000000 pysmlib-3.4.2/pysmlib.egg-info/PKG-INFO
+-rw-r--r--   0 marcato   (1000) marcato   (1000)      479 2024-05-24 08:45:33.000000 pysmlib-3.4.2/pysmlib.egg-info/SOURCES.txt
+-rw-r--r--   0 marcato   (1000) marcato   (1000)        1 2024-05-24 08:45:33.000000 pysmlib-3.4.2/pysmlib.egg-info/dependency_links.txt
+-rw-r--r--   0 marcato   (1000) marcato   (1000)        1 2018-10-04 08:18:58.000000 pysmlib-3.4.2/pysmlib.egg-info/not-zip-safe
+-rw-r--r--   0 marcato   (1000) marcato   (1000)        8 2024-05-24 08:45:33.000000 pysmlib-3.4.2/pysmlib.egg-info/requires.txt
+-rw-r--r--   0 marcato   (1000) marcato   (1000)        6 2024-05-24 08:45:33.000000 pysmlib-3.4.2/pysmlib.egg-info/top_level.txt
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)      223 2024-05-24 08:45:33.981943 pysmlib-3.4.2/setup.cfg
+-rw-r--r--   0 marcato   (1000) marcato   (1000)     1105 2020-09-10 17:56:38.000000 pysmlib-3.4.2/setup.py
+drwxrwxr-x   0 marcato   (1000) marcato   (1000)        0 2024-05-24 08:45:33.977943 pysmlib-3.4.2/smlib/
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)     1490 2024-05-24 08:22:35.000000 pysmlib-3.4.2/smlib/__init__.py
+-rw-r--r--   0 marcato   (1000) marcato   (1000)    18445 2020-03-20 13:10:18.000000 pysmlib-3.4.2/smlib/_version.py
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)    11609 2024-05-24 08:22:35.000000 pysmlib-3.4.2/smlib/fsm.py
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)     1709 2024-05-24 08:22:35.000000 pysmlib-3.4.2/smlib/fsmTemplate.py
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)     1952 2024-05-24 08:22:35.000000 pysmlib-3.4.2/smlib/fsmWatchdog.py
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)    24316 2024-05-24 08:22:35.000000 pysmlib-3.4.2/smlib/io.py
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)     3693 2024-05-24 08:22:35.000000 pysmlib-3.4.2/smlib/loader.py
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)     1969 2024-05-24 08:22:35.000000 pysmlib-3.4.2/smlib/logger.py
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)     5498 2024-05-24 08:22:35.000000 pysmlib-3.4.2/smlib/timer.py
+drwxrwxr-x   0 marcato   (1000) marcato   (1000)        0 2024-05-24 08:45:33.977943 pysmlib-3.4.2/tests/
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)     5580 2024-05-24 08:22:35.000000 pysmlib-3.4.2/tests/test_io.py
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)     2402 2024-05-24 08:22:35.000000 pysmlib-3.4.2/tests/test_loader.py
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)     2981 2024-05-24 08:22:35.000000 pysmlib-3.4.2/tests/test_states.py
+-rw-rw-r--   0 marcato   (1000) marcato   (1000)     3140 2024-05-24 08:22:35.000000 pysmlib-3.4.2/tests/test_timer.py
+-rw-r--r--   0 marcato   (1000) marcato   (1000)    68611 2020-03-20 13:10:18.000000 pysmlib-3.4.2/versioneer.py
```

### Comparing `pysmlib-3.4.1/LICENSE.txt` & `pysmlib-3.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysmlib-3.4.1/PKG-INFO` & `pysmlib-3.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pysmlib
-Version: 3.4.1
+Version: 3.4.2
 Summary: Python Finite State Machines for EPICS
 Home-page: https://darcato.github.io/pysmlib/docs/html/
 Download-URL: https://github.com/darcato/pysmlib
 Author: Damiano Bortolato - Davide Marcato
 Author-email: davide.marcato@lnl.infn.it
 License: GPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: pyepics
 
 # pysmlib
 
 ## Python Finite State Machines for EPICS
 
 _Developers_: Damiano Bortolato - Davide Marcato @ Laboratori Nazionali di Legnaro - INFN
```

### Comparing `pysmlib-3.4.1/README.md` & `pysmlib-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pysmlib-3.4.1/pysmlib.egg-info/PKG-INFO` & `pysmlib-3.4.2/pysmlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pysmlib
-Version: 3.4.1
+Version: 3.4.2
 Summary: Python Finite State Machines for EPICS
 Home-page: https://darcato.github.io/pysmlib/docs/html/
 Download-URL: https://github.com/darcato/pysmlib
 Author: Damiano Bortolato - Davide Marcato
 Author-email: davide.marcato@lnl.infn.it
 License: GPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: pyepics
 
 # pysmlib
 
 ## Python Finite State Machines for EPICS
 
 _Developers_: Damiano Bortolato - Davide Marcato @ Laboratori Nazionali di Legnaro - INFN
```

### Comparing `pysmlib-3.4.1/setup.py` & `pysmlib-3.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `pysmlib-3.4.1/smlib/__init__.py` & `pysmlib-3.4.2/smlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmlib-3.4.1/smlib/_version.py` & `pysmlib-3.4.2/smlib/_version.py`

 * *Files identical despite different names*

### Comparing `pysmlib-3.4.1/smlib/fsm.py` & `pysmlib-3.4.2/smlib/fsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,19 @@
     The user must implement FSM states as methods of the class.
     '''
 
     def __init__(self, name:str, **args) -> None:
         super(fsmBase, self).__init__(name=name)
         self._name = name
         if 'tmgr' not in args:
+            self._private_tmgr = True
             self._tmgr = fsmTimers()
             self._tmgr.start()
         else:
+            self._private_tmgr = False
             self._tmgr = args['tmgr']
             if not self._tmgr.is_alive():
                 self._tmgr.start()
 
         self._timers = {}
         self._ios = args.get('ios', fsmIOs())
         self._logger = args.get('logger', fsmLogger())
@@ -181,14 +183,16 @@
     def kill(self) -> None:
         '''Stop the FSM thread'''
         self._cond.acquire()
         self._stop_thread = True
         self._cond.notify()
         self._cond.release()
         self.join()
+        if self._private_tmgr:
+            self._tmgr.kill()
 
     def trigger(self, **args) -> None:
         '''Enqueue an event to be processed by the FSM'''
         self._cond.acquire()
 #        self.logD("pushing event %s %d" %(repr(args), len(self._events)+1))
         self._events.append(args)  # append here also the shapshot of all ios
         if len(self._events) == 1:
```

### Comparing `pysmlib-3.4.1/smlib/fsmTemplate.py` & `pysmlib-3.4.2/smlib/fsmTemplate.py`

 * *Files identical despite different names*

### Comparing `pysmlib-3.4.1/smlib/fsmWatchdog.py` & `pysmlib-3.4.2/smlib/fsmWatchdog.py`

 * *Files identical despite different names*

### Comparing `pysmlib-3.4.1/smlib/io.py` & `pysmlib-3.4.2/smlib/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
     def __init__(self, name:str) -> None:
         self._name = name
         self._data = {}  # keep all infos arriving with change callback
         self._conn = False  # keeps all infos arriving with connection callback
 
         self._attached = set()  # set of finite state machines using this IO
-        self._pv = epics.PV(name, callback=self.chgcb, connection_callback=self.concb, auto_monitor=True)
         self._cond = threading.Condition()
+        self._pv = epics.PV(name, callback=self.chgcb, connection_callback=self.concb, auto_monitor=True)
 
     def ioname(self) -> str:
         '''Return the name of the PV.'''
         return self._name
 
     def attach(self, fsm: 'fsmBase') -> None:
         '''
@@ -80,23 +80,27 @@
         '''
         Wakes up all the finite state machines attached to this IO.
         The finite state machines will be triggered with the given callback name and data.
         '''
         for fsm in self._attached:
             fsm.trigger(iobj=self, inputname=self._name, reason=cbname, cbdata=cbdata)
 
-    def put(self, value, caller_fsm: 'fsmBase') -> bool:
+    def put(self, value, caller_fsm: 'fsmBase', use_complete=True) -> bool:
         '''
-        Put a value to the PV without wait for the PV processing to complete.
+        Put a value to the PV without wait for the PV processing to complete
+        if use_complete=True or issue regular PV put otherwise.
         Returns False if the put() fails to start, may still fail later.
         '''
         # cbdata contains the fsm obj to wake up when putCompleted
-        cbdata = {"fsm": caller_fsm}
         try:
-            self._pv.put(value, callback=self.putcb, use_complete=True, callback_data=cbdata)
+            if use_complete:
+                cbdata = {"fsm": caller_fsm}
+                self._pv.put(value, callback=self.putcb, use_complete=True, callback_data=cbdata)
+            else:
+                self._pv.put(value)
         except Exception as e:
             caller_fsm.logE("FAILED putting to pv %s  -- exception: %s" % (self._name, str(e)))
             return False
         return True
 
     def putComplete(self) -> bool:
         '''Return True if the most recent put() has completed.'''
@@ -350,18 +354,18 @@
         '''When the state is changed, the current callback is reset'''
         self._currcb = ""
 
     def ioname(self) -> str:
         '''Return the name of the io'''
         return self._name
 
-    def put(self, value) -> bool:
+    def put(self, value, use_complete=True) -> bool:
         '''Write a value to the io'''
         self._putComplete = False
-        return self._reflectedIO.put(value, self._fsm)
+        return self._reflectedIO.put(value, self._fsm, use_complete)
 
     # ----- METHODS THAT CATCH CHANGE ONLY if CHECKED WHEN TRIGGERED BY THE SAME CHANGE ------
     # ----- They return True if the fsm was woken up by this change in this cycle
 
     def putCompleting(self) -> bool:
         '''The current event is a put complete callback of this IO'''
         return self._currcb == 'putcomp'
```

### Comparing `pysmlib-3.4.1/smlib/loader.py` & `pysmlib-3.4.2/smlib/loader.py`

 * *Files identical despite different names*

### Comparing `pysmlib-3.4.1/smlib/logger.py` & `pysmlib-3.4.2/smlib/logger.py`

 * *Files identical despite different names*

### Comparing `pysmlib-3.4.1/smlib/timer.py` & `pysmlib-3.4.2/smlib/timer.py`

 * *Files identical despite different names*

### Comparing `pysmlib-3.4.1/versioneer.py` & `pysmlib-3.4.2/versioneer.py`

 * *Files identical despite different names*

