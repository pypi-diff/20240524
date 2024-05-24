# Comparing `tmp/limitloop-0.1.tar.gz` & `tmp/limitloop-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/limitloop-0.1.tar", last modified: Tue May 21 20:50:34 2019, max compression
+gzip compressed data, was "limitloop-0.2.tar", last modified: Fri May 24 16:48:46 2024, max compression
```

## Comparing `limitloop-0.1.tar` & `limitloop-0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 localuser  (1000) localuser  (1000)        0 2019-05-21 20:50:34.000000 limitloop-0.1/
--rw-rw-r--   0 localuser  (1000) localuser  (1000)     1136 2019-05-21 20:45:26.000000 limitloop-0.1/README.md
--rw-rw-r--   0 localuser  (1000) localuser  (1000)       19 2019-05-21 20:23:38.000000 limitloop-0.1/MANIFEST.in
--rw-rw-r--   0 localuser  (1000) localuser  (1000)       38 2019-05-21 20:50:34.000000 limitloop-0.1/setup.cfg
-drwxrwxr-x   0 localuser  (1000) localuser  (1000)        0 2019-05-21 20:50:34.000000 limitloop-0.1/limitloop/
--rw-rw-r--   0 localuser  (1000) localuser  (1000)     2528 2019-05-18 20:37:19.000000 limitloop-0.1/limitloop/limitloop.py
--rw-rw-r--   0 localuser  (1000) localuser  (1000)       48 2019-05-18 15:48:27.000000 limitloop-0.1/limitloop/__init__.py
--rw-rw-r--   0 localuser  (1000) localuser  (1000)      818 2019-05-21 20:28:22.000000 limitloop-0.1/setup.py
-drwxrwxr-x   0 localuser  (1000) localuser  (1000)        0 2019-05-21 20:50:34.000000 limitloop-0.1/limitloop.egg-info/
--rw-rw-r--   0 localuser  (1000) localuser  (1000)      207 2019-05-21 20:50:34.000000 limitloop-0.1/limitloop.egg-info/SOURCES.txt
--rw-rw-r--   0 localuser  (1000) localuser  (1000)       10 2019-05-21 20:50:34.000000 limitloop-0.1/limitloop.egg-info/top_level.txt
--rw-rw-r--   0 localuser  (1000) localuser  (1000)        1 2019-05-21 20:50:34.000000 limitloop-0.1/limitloop.egg-info/dependency_links.txt
--rw-rw-r--   0 localuser  (1000) localuser  (1000)     2005 2019-05-21 20:50:34.000000 limitloop-0.1/limitloop.egg-info/PKG-INFO
--rw-rw-r--   0 localuser  (1000) localuser  (1000)     2005 2019-05-21 20:50:34.000000 limitloop-0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-24 16:48:46.295332 limitloop-0.2/
+-rw-rw-rw-   0        0        0    32473 2024-05-24 16:26:53.000000 limitloop-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2024-05-24 16:26:53.000000 limitloop-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1686 2024-05-24 16:48:46.294337 limitloop-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1094 2024-05-24 16:26:53.000000 limitloop-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 16:48:46.273392 limitloop-0.2/limitloop/
+-rw-rw-rw-   0        0        0       48 2024-05-24 16:26:53.000000 limitloop-0.2/limitloop/__init__.py
+-rw-rw-rw-   0        0        0     2894 2024-05-24 16:26:53.000000 limitloop-0.2/limitloop/limitloop.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:48:46.292341 limitloop-0.2/limitloop.egg-info/
+-rw-rw-rw-   0        0        0     1686 2024-05-24 16:48:46.000000 limitloop-0.2/limitloop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2024-05-24 16:48:46.000000 limitloop-0.2/limitloop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 16:48:46.000000 limitloop-0.2/limitloop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 16:48:46.000000 limitloop-0.2/limitloop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 16:48:46.295332 limitloop-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      799 2024-05-24 16:26:53.000000 limitloop-0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `limitloop-0.1/README.md` & `limitloop-0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -30,9 +30,7 @@
 Hello, world!
 Hello, world!
 Hello, world!
 Hello, world!
 Hello, world!
 ```
 See the [API reference](api_reference.md) for more advanced usage.
-
-*TODO: Add more advanced usage examples*
```

### Comparing `limitloop-0.1/limitloop/limitloop.py` & `limitloop-0.2/limitloop/limitloop.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from time import perf_counter, sleep
 import math, threading
 
 class Loop(object):
+    #TODO: Add a `Loop.initialFrame` property
+    #TODO: Make constructor for Loop check if the method it's being passed contains a *kwarg* for the loop
+    #TODO: Add a constructor arg to pass loop object through kwargs with non-standard name
     def __init__(self, func, freq=30, saveArgs=False):
         self._running = False
         self._function = func
         self._frequency = freq
         self._saveArgs = saveArgs
         self._args = []
         self._kwargs = {}
@@ -39,14 +42,17 @@
         if self._running: raise RuntimeError('Loop.run cannot be called while the loop is already running')
         self._running = True
         frameTargetTime = self.targetTime()
         iteration=0
         while self._running:
             self._currentFrameStartTime = perf_counter()
             self._lastReturn = self._function(self, *self._args, **self._kwargs)
+            if not self.saveArgs:
+                self._args = []
+                self._kwargs = {}
             iteration += 1
             if iteration >= maxIterations and maxIterations > 0:
                 self.end()
             self._lastFrameTime = perf_counter() - self._currentFrameStartTime
             if(self._lastFrameTime < frameTargetTime):
                 sleep(frameTargetTime - self._lastFrameTime)
     
@@ -60,15 +66,15 @@
         if not self._running: raise RuntimeError('Loop.frameTime can only be called while the loop is running')
         return self._currentFrameStartTime - perf_counter()
     
     def targetTime(self):
         return 1/self._frequency
     
     def framesPerSecond(self):
-        return 1/self._lastFrameTime if self._lastFrameTime != 0 else 0
+        return min(self._frequency, 1/self._lastFrameTime if self._lastFrameTime != 0 else 0)
     
     def setArgs(self, *args, **kwargs):
         self._args = args
         self._kwargs = kwargs
     
     def lastReturn(self):
         return self._lastReturn
```

### Comparing `limitloop-0.1/setup.py` & `limitloop-0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 SHORT_DESC = 'Limitloop is a lightweight python module for running loops that depend on precise timing.'
 
 with open('README.md', 'r') as readme_file:
     readme_contents = readme_file.read()
 
 setup(
     name='limitloop',
-    version=0.1,
+    version=0.2,
     author='Alex Medeiros',
-    author_email='alex.daniel.medeiros@gmail.com',
-    url='https://github.com/Alex-Medeiros/limitloop',
+    author_email='senox13@gmail.com',
+    url='https://github.com/senox13/limitloop',
     description=SHORT_DESC,
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     packages=['limitloop'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

