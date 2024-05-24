# Comparing `tmp/flexsolve-0.5.5.tar.gz` & `tmp/flexsolve-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexsolve-0.5.5.tar", last modified: Fri May 24 15:31:58 2024, max compression
+gzip compressed data, was "flexsolve-0.5.6.tar", last modified: Fri May 24 15:38:02 2024, max compression
```

## Comparing `flexsolve-0.5.5.tar` & `flexsolve-0.5.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 15:31:58.718469 flexsolve-0.5.5/
--rw-rw-rw-   0        0        0     1120 2023-09-22 17:18:37.000000 flexsolve-0.5.5/LICENSE.txt
--rw-rw-rw-   0        0        0      624 2023-09-22 17:18:37.000000 flexsolve-0.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0     9636 2024-05-24 15:31:58.718469 flexsolve-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     8206 2023-09-22 17:18:37.000000 flexsolve-0.5.5/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-24 15:31:58.624267 flexsolve-0.5.5/docs/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:31:58.640907 flexsolve-0.5.5/docs/images/
--rw-rw-rw-   0        0        0    58254 2023-09-22 17:18:37.000000 flexsolve-0.5.5/docs/images/bounded_solvers_example.png
--rw-rw-rw-   0        0        0    35388 2023-09-22 17:18:37.000000 flexsolve-0.5.5/docs/images/fixed_point_solvers_example.png
--rw-rw-rw-   0        0        0    44816 2023-09-22 17:18:37.000000 flexsolve-0.5.5/docs/images/general_solvers_example.png
-drwxrwxrwx   0        0        0        0 2024-05-24 15:31:58.687242 flexsolve-0.5.5/flexsolve/
--rw-rw-rw-   0        0        0      713 2024-05-24 15:31:45.000000 flexsolve-0.5.5/flexsolve/__init__.py
--rw-rw-rw-   0        0        0     7063 2023-09-22 17:18:37.000000 flexsolve-0.5.5/flexsolve/bounded_solvers.py
--rw-rw-rw-   0        0        0     4668 2024-05-24 15:31:45.000000 flexsolve-0.5.5/flexsolve/iterative_solvers.py
--rw-rw-rw-   0        0        0     4472 2023-09-22 17:18:37.000000 flexsolve-0.5.5/flexsolve/open_solvers.py
--rw-rw-rw-   0        0        0     1507 2023-09-22 17:18:37.000000 flexsolve-0.5.5/flexsolve/problem.py
--rw-rw-rw-   0        0        0     2816 2023-09-22 17:18:37.000000 flexsolve-0.5.5/flexsolve/problem_list.py
--rw-rw-rw-   0        0        0     6015 2023-09-22 17:18:37.000000 flexsolve-0.5.5/flexsolve/profiler.py
--rw-rw-rw-   0        0        0     6344 2023-09-22 17:18:37.000000 flexsolve-0.5.5/flexsolve/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:31:58.702877 flexsolve-0.5.5/flexsolve.egg-info/
--rw-rw-rw-   0        0        0     9636 2024-05-24 15:31:58.000000 flexsolve-0.5.5/flexsolve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      679 2024-05-24 15:31:58.000000 flexsolve-0.5.5/flexsolve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 15:31:58.000000 flexsolve-0.5.5/flexsolve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-24 15:31:58.000000 flexsolve-0.5.5/flexsolve.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-24 15:31:58.000000 flexsolve-0.5.5/flexsolve.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      277 2023-09-22 17:18:37.000000 flexsolve-0.5.5/pytest.ini
--rw-rw-rw-   0        0        0       42 2024-05-24 15:31:58.718469 flexsolve-0.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1936 2024-05-24 15:31:45.000000 flexsolve-0.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:31:58.718469 flexsolve-0.5.5/tests/
--rw-rw-rw-   0        0        0      363 2023-09-22 17:18:37.000000 flexsolve-0.5.5/tests/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-09-22 17:18:37.000000 flexsolve-0.5.5/tests/test_bounded_solvers.py
--rw-rw-rw-   0        0        0     5692 2023-09-22 17:18:37.000000 flexsolve-0.5.5/tests/test_fixedpoint_array_solvers.py
--rw-rw-rw-   0        0        0     9840 2023-09-22 17:18:37.000000 flexsolve-0.5.5/tests/test_scalar_solvers.py
--rw-rw-rw-   0        0        0     1521 2023-09-22 17:18:37.000000 flexsolve-0.5.5/tests/test_with_plots.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:38:02.292964 flexsolve-0.5.6/
+-rw-rw-rw-   0        0        0     1120 2023-09-22 17:18:37.000000 flexsolve-0.5.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      624 2023-09-22 17:18:37.000000 flexsolve-0.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     9636 2024-05-24 15:38:02.292964 flexsolve-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8206 2023-09-22 17:18:37.000000 flexsolve-0.5.6/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-24 15:38:02.264323 flexsolve-0.5.6/docs/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:38:02.277331 flexsolve-0.5.6/docs/images/
+-rw-rw-rw-   0        0        0    58254 2023-09-22 17:18:37.000000 flexsolve-0.5.6/docs/images/bounded_solvers_example.png
+-rw-rw-rw-   0        0        0    35388 2023-09-22 17:18:37.000000 flexsolve-0.5.6/docs/images/fixed_point_solvers_example.png
+-rw-rw-rw-   0        0        0    44816 2023-09-22 17:18:37.000000 flexsolve-0.5.6/docs/images/general_solvers_example.png
+drwxrwxrwx   0        0        0        0 2024-05-24 15:38:02.277331 flexsolve-0.5.6/flexsolve/
+-rw-rw-rw-   0        0        0      713 2024-05-24 15:37:31.000000 flexsolve-0.5.6/flexsolve/__init__.py
+-rw-rw-rw-   0        0        0     7063 2023-09-22 17:18:37.000000 flexsolve-0.5.6/flexsolve/bounded_solvers.py
+-rw-rw-rw-   0        0        0     4668 2024-05-24 15:31:45.000000 flexsolve-0.5.6/flexsolve/iterative_solvers.py
+-rw-rw-rw-   0        0        0     4472 2023-09-22 17:18:37.000000 flexsolve-0.5.6/flexsolve/open_solvers.py
+-rw-rw-rw-   0        0        0     1507 2023-09-22 17:18:37.000000 flexsolve-0.5.6/flexsolve/problem.py
+-rw-rw-rw-   0        0        0     2816 2023-09-22 17:18:37.000000 flexsolve-0.5.6/flexsolve/problem_list.py
+-rw-rw-rw-   0        0        0     6015 2023-09-22 17:18:37.000000 flexsolve-0.5.6/flexsolve/profiler.py
+-rw-rw-rw-   0        0        0     6344 2023-09-22 17:18:37.000000 flexsolve-0.5.6/flexsolve/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:38:02.292964 flexsolve-0.5.6/flexsolve.egg-info/
+-rw-rw-rw-   0        0        0     9636 2024-05-24 15:38:02.000000 flexsolve-0.5.6/flexsolve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      679 2024-05-24 15:38:02.000000 flexsolve-0.5.6/flexsolve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 15:38:02.000000 flexsolve-0.5.6/flexsolve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-24 15:38:02.000000 flexsolve-0.5.6/flexsolve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 15:38:02.000000 flexsolve-0.5.6/flexsolve.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      277 2023-09-22 17:18:37.000000 flexsolve-0.5.6/pytest.ini
+-rw-rw-rw-   0        0        0       42 2024-05-24 15:38:02.292964 flexsolve-0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1936 2024-05-24 15:37:25.000000 flexsolve-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:38:02.292964 flexsolve-0.5.6/tests/
+-rw-rw-rw-   0        0        0      363 2023-09-22 17:18:37.000000 flexsolve-0.5.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-09-22 17:18:37.000000 flexsolve-0.5.6/tests/test_bounded_solvers.py
+-rw-rw-rw-   0        0        0     5692 2023-09-22 17:18:37.000000 flexsolve-0.5.6/tests/test_fixedpoint_array_solvers.py
+-rw-rw-rw-   0        0        0     9840 2023-09-22 17:18:37.000000 flexsolve-0.5.6/tests/test_scalar_solvers.py
+-rw-rw-rw-   0        0        0     1521 2023-09-22 17:18:37.000000 flexsolve-0.5.6/tests/test_with_plots.py
```

### Comparing `flexsolve-0.5.5/LICENSE.txt` & `flexsolve-0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/MANIFEST.in` & `flexsolve-0.5.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/PKG-INFO` & `flexsolve-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexsolve
-Version: 0.5.5
+Version: 0.5.6
 Summary: Flexible function solvers
 Home-page: https://github.com/yoelcortes/flexsolve
 Download-URL: https://github.com/yoelcortes/flexsolve.git
 Author: Yoel Cortes-Pena
 Author-email: yoelcortes@gmail.com
 License: MIT
 Keywords: solve,equation,function,flexible
@@ -28,15 +28,15 @@
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 License-File: LICENSE.txt
 
 ========================================================
 flexsolve: Flexible function solvers
 ========================================================
 .. image:: http://img.shields.io/badge/license-MIT-blue.svg?style=flat
    :target: https://github.com/yoelcortes/flexsolve/blob/master/LICENSE.txt
```

### Comparing `flexsolve-0.5.5/README.rst` & `flexsolve-0.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/docs/images/bounded_solvers_example.png` & `flexsolve-0.5.6/docs/images/bounded_solvers_example.png`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/docs/images/fixed_point_solvers_example.png` & `flexsolve-0.5.6/docs/images/fixed_point_solvers_example.png`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/docs/images/general_solvers_example.png` & `flexsolve-0.5.6/docs/images/general_solvers_example.png`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/flexsolve/__init__.py` & `flexsolve-0.5.6/flexsolve/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 from .open_solvers import *
 from .bounded_solvers import *
 from .iterative_solvers import *
 from .problem_list import *
 from .problem import *
 from .profiler import *
 
-__version__ = '0.5.5'
+__version__ = '0.5.6'
```

### Comparing `flexsolve-0.5.5/flexsolve/bounded_solvers.py` & `flexsolve-0.5.6/flexsolve/bounded_solvers.py`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/flexsolve/iterative_solvers.py` & `flexsolve-0.5.6/flexsolve/iterative_solvers.py`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/flexsolve/open_solvers.py` & `flexsolve-0.5.6/flexsolve/open_solvers.py`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/flexsolve/problem.py` & `flexsolve-0.5.6/flexsolve/problem.py`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/flexsolve/problem_list.py` & `flexsolve-0.5.6/flexsolve/problem_list.py`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/flexsolve/profiler.py` & `flexsolve-0.5.6/flexsolve/profiler.py`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/flexsolve/utils.py` & `flexsolve-0.5.6/flexsolve/utils.py`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/flexsolve.egg-info/PKG-INFO` & `flexsolve-0.5.6/flexsolve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexsolve
-Version: 0.5.5
+Version: 0.5.6
 Summary: Flexible function solvers
 Home-page: https://github.com/yoelcortes/flexsolve
 Download-URL: https://github.com/yoelcortes/flexsolve.git
 Author: Yoel Cortes-Pena
 Author-email: yoelcortes@gmail.com
 License: MIT
 Keywords: solve,equation,function,flexible
@@ -28,15 +28,15 @@
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 License-File: LICENSE.txt
 
 ========================================================
 flexsolve: Flexible function solvers
 ========================================================
 .. image:: http://img.shields.io/badge/license-MIT-blue.svg?style=flat
    :target: https://github.com/yoelcortes/flexsolve/blob/master/LICENSE.txt
```

### Comparing `flexsolve-0.5.5/flexsolve.egg-info/SOURCES.txt` & `flexsolve-0.5.6/flexsolve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/setup.py` & `flexsolve-0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 """
 from distutils.core import setup
 
 setup(
     name='flexsolve',
     packages=['flexsolve'],
     license='MIT',
-    version='0.5.5',
+    version='0.5.6',
     description='Flexible function solvers',
     long_description=open('README.rst').read(),
     author='Yoel Cortes-Pena',
     install_requires=['numba>=0.50.0', 'llvmlite>=0.31', 'numpy'],
-    python_requires=">=3.6",
+    python_requires=">=3.9",
     package_data=
         {'flexsolve': []},
     platforms=['Windows', 'Mac', 'Linux'],
     author_email='yoelcortes@gmail.com',
     url='https://github.com/yoelcortes/flexsolve',
     download_url='https://github.com/yoelcortes/flexsolve.git',
     classifiers=['Development Status :: 3 - Alpha',
```

### Comparing `flexsolve-0.5.5/tests/test_bounded_solvers.py` & `flexsolve-0.5.6/tests/test_bounded_solvers.py`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/tests/test_fixedpoint_array_solvers.py` & `flexsolve-0.5.6/tests/test_fixedpoint_array_solvers.py`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/tests/test_scalar_solvers.py` & `flexsolve-0.5.6/tests/test_scalar_solvers.py`

 * *Files identical despite different names*

### Comparing `flexsolve-0.5.5/tests/test_with_plots.py` & `flexsolve-0.5.6/tests/test_with_plots.py`

 * *Files identical despite different names*

