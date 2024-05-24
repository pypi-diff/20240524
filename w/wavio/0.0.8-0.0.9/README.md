# Comparing `tmp/wavio-0.0.8.tar.gz` & `tmp/wavio-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wavio-0.0.8.tar", last modified: Sat Oct  7 22:49:44 2023, max compression
+gzip compressed data, was "wavio-0.0.9.tar", last modified: Fri May 24 02:12:18 2024, max compression
```

## Comparing `wavio-0.0.8.tar` & `wavio-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 22:49:44.733109 wavio-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2023-10-07 22:49:44.733109 wavio-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2023-10-07 22:49:34.000000 wavio-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-07 22:49:44.733109 wavio-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2023-10-07 22:49:34.000000 wavio-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 22:49:44.733109 wavio-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2023-10-07 22:49:34.000000 wavio-0.0.8/tests/test_wavio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 22:49:44.733109 wavio-0.0.8/wavio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2023-10-07 22:49:44.000000 wavio-0.0.8/wavio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-10-07 22:49:44.000000 wavio-0.0.8/wavio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-07 22:49:44.000000 wavio-0.0.8/wavio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-07 22:49:44.000000 wavio-0.0.8/wavio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-07 22:49:44.000000 wavio-0.0.8/wavio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17669 2023-10-07 22:49:34.000000 wavio-0.0.8/wavio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:12:18.826414 wavio-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-24 02:12:18.826414 wavio-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-24 02:12:14.000000 wavio-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 02:12:18.826414 wavio-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-24 02:12:14.000000 wavio-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:12:18.826414 wavio-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11458 2024-05-24 02:12:14.000000 wavio-0.0.9/tests/test_wavio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:12:18.826414 wavio-0.0.9/wavio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-24 02:12:18.000000 wavio-0.0.9/wavio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-24 02:12:18.000000 wavio-0.0.9/wavio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:12:18.000000 wavio-0.0.9/wavio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-24 02:12:18.000000 wavio-0.0.9/wavio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 02:12:18.000000 wavio-0.0.9/wavio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17789 2024-05-24 02:12:14.000000 wavio-0.0.9/wavio.py
```

### Comparing `wavio-0.0.8/PKG-INFO` & `wavio-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: wavio
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python module for reading and writing WAV files using numpy arrays.
 Home-page: https://github.com/WarrenWeckesser/wavio
 Author: Warren Weckesser
 License: BSD
 Keywords: wav numpy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy>=1.19.0
 
 wavio
 =====
 
 ``wavio`` is a Python module that defines two functions:
```

### Comparing `wavio-0.0.8/README.md` & `wavio-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wavio-0.0.8/setup.py` & `wavio-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     with open("wavio.py", "r") as f:
         for line in f:
             s = [w.strip() for w in line.split("=", 1)]
             if len(s) == 2 and s[0] == "__version__":
                 return s[1][1:-1]
 
 
-# Get the long description from README.rst.
+# Get the long description from README.md.
 _here = path.abspath(path.dirname(__file__))
 with open(path.join(_here, 'README.md')) as f:
     _long_description = f.read()
 
 setup(
     name='wavio',
     version=get_wavio_version(),
@@ -39,14 +39,15 @@
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     keywords="wav numpy",
     py_modules=["wavio"],
     install_requires=[
         'numpy >= 1.19.0',
     ],
 )
```

### Comparing `wavio-0.0.8/tests/test_wavio.py` & `wavio-0.0.9/tests/test_wavio.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,16 @@
             os.chdir(d)
             # Negative values will be clipped.
             data = np.array([-2**7, -2**3, -1, 0, 1, 2**3, 2**7-1],
                             dtype=np.int8)
             wavio.write(filename, data, 44100, clip='ignore')
 
             check_basic(filename, nchannels=1, sampwidth=1, framerate=44100)
-            expected_data = data.clip(0, 255).astype(np.uint8)
+            int8max = np.iinfo(np.int8).max  # A long way to spell 127.
+            expected_data = data.clip(0, int8max).astype(np.uint8)
             check_wavio_read(filename, rate=44100, sampwidth=1,
                              dtype=np.uint8, shape=(len(data), 1),
                              data=expected_data)
 
     def test_unsigned8bit_full_range_round_trip(self):
         # Regression test for github issue 5.
         filename = 'testdata.wav'
```

### Comparing `wavio-0.0.8/wavio.egg-info/PKG-INFO` & `wavio-0.0.9/wavio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: wavio
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python module for reading and writing WAV files using numpy arrays.
 Home-page: https://github.com/WarrenWeckesser/wavio
 Author: Warren Weckesser
 License: BSD
 Keywords: wav numpy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy>=1.19.0
 
 wavio
 =====
 
 ``wavio`` is a Python module that defines two functions:
```

### Comparing `wavio-0.0.8/wavio.py` & `wavio-0.0.9/wavio.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 """
 
 import warnings as _warnings
 import wave as _wave
 import numpy as _np
 
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 
 class ClippedDataWarning(UserWarning):
 
     def __init__(self, message=None):
         if message is None:
             message = ('Some data values were clipped when converted to the '
@@ -442,15 +442,17 @@
                              'input is an integer array.  No shifting or '
                              'scaling is done to integer input values.')
         if (data.min() < outmin or data.max() > outmax):
             if clip == "warn":
                 _warnings.warn(ClippedDataWarning())
             elif clip == "raise":
                 raise ClippedDataError()
-        data = data.clip(outmin, outmax).astype(outdtype)
+        clip_min = max(outmin, _np.iinfo(data.dtype).min)
+        clip_max = min(outmax, _np.iinfo(data.dtype).max)
+        data = data.clip(clip_min, clip_max).astype(outdtype)
     elif _np.issubdtype(data.dtype, _np.floating):
         data = _float_to_integer(data, sampwidth, scale=scale, clip=clip)
     else:
         raise TypeError(f'unsupported input array data type: {data.dtype}')
 
     # At this point, `data` has been converted to have one of the following:
     #    sampwidth   dtype
```

