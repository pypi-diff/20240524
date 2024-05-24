# Comparing `tmp/pybetterthreads-0.0.1.tar.gz` & `tmp/pybetterthreads-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybetterthreads-0.0.1.tar", last modified: Fri May 24 20:20:29 2024, max compression
+gzip compressed data, was "pybetterthreads-0.0.2.tar", last modified: Fri May 24 20:28:13 2024, max compression
```

## Comparing `pybetterthreads-0.0.1.tar` & `pybetterthreads-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 20:20:29.020679 pybetterthreads-0.0.1/
--rw-rw-rw-   0        0        0     1082 2024-05-24 19:54:45.000000 pybetterthreads-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3608 2024-05-24 20:20:29.019676 pybetterthreads-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-24 20:20:28.985538 pybetterthreads-0.0.1/PyBetterThreads/
--rw-rw-rw-   0        0        0      855 2024-05-24 18:59:50.000000 pybetterthreads-0.0.1/PyBetterThreads/BetterThread.py
--rw-rw-rw-   0        0        0      101 2024-05-24 20:16:19.000000 pybetterthreads-0.0.1/PyBetterThreads/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:20:29.016822 pybetterthreads-0.0.1/PyBetterThreads.egg-info/
--rw-rw-rw-   0        0        0     3608 2024-05-24 20:20:28.000000 pybetterthreads-0.0.1/PyBetterThreads.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-05-24 20:20:28.000000 pybetterthreads-0.0.1/PyBetterThreads.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 20:20:28.000000 pybetterthreads-0.0.1/PyBetterThreads.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-24 20:20:28.000000 pybetterthreads-0.0.1/PyBetterThreads.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2401 2024-05-24 20:15:58.000000 pybetterthreads-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 20:20:29.020679 pybetterthreads-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1574 2024-05-24 20:15:58.000000 pybetterthreads-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:28:13.995045 pybetterthreads-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2024-05-24 19:54:45.000000 pybetterthreads-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3619 2024-05-24 20:28:13.993380 pybetterthreads-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-24 20:28:13.975341 pybetterthreads-0.0.2/PyBetterThreads/
+-rw-rw-rw-   0        0        0      855 2024-05-24 18:59:50.000000 pybetterthreads-0.0.2/PyBetterThreads/BetterThread.py
+-rw-rw-rw-   0        0        0      101 2024-05-24 20:16:19.000000 pybetterthreads-0.0.2/PyBetterThreads/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:28:13.993380 pybetterthreads-0.0.2/PyBetterThreads.egg-info/
+-rw-rw-rw-   0        0        0     3619 2024-05-24 20:28:13.000000 pybetterthreads-0.0.2/PyBetterThreads.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-24 20:28:13.000000 pybetterthreads-0.0.2/PyBetterThreads.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 20:28:13.000000 pybetterthreads-0.0.2/PyBetterThreads.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-24 20:28:13.000000 pybetterthreads-0.0.2/PyBetterThreads.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2414 2024-05-24 20:27:48.000000 pybetterthreads-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 20:28:13.995045 pybetterthreads-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1574 2024-05-24 20:23:22.000000 pybetterthreads-0.0.2/setup.py
```

### Comparing `pybetterthreads-0.0.1/LICENSE` & `pybetterthreads-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybetterthreads-0.0.1/PKG-INFO` & `pybetterthreads-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBetterThreads
-Version: 0.0.1
+Version: 0.0.2
 Summary: Threads, but with more features!
 Home-page: https://github.com/theAbdoSabbagh/PyBetterThreads
 Author: theAbdoSabbagh
 License: MIT
 Project-URL: Documentation, https://github.com/theAbdoSabbagh/PyBetterThreads/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/theAbdoSabbagh/PyBetterThreads/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,17 +24,17 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyBetterThreads
 
-[![Downloads](https://static.pepy.tech/badge/betterthread)](https://pepy.tech/project/betterthread)
+[![Downloads](https://static.pepy.tech/badge/pybetterthreads)](https://pepy.tech/project/pybetterthreads)
 [![PyPi](https://img.shields.io/pypi/v/PyBetterThreads.svg)](https://pypi.python.org/pypi/PyBetterThreads)
-[![License](https://img.shields.io/github/license/theAbdoSabbagh/PyBetterThreads.svg?color=black)](https://github.com/theAbdoSabbagh/PyBetterThreads/main/LICENSE)
+[![License](https://img.shields.io/github/license/theAbdoSabbagh/PyBetterThreads.svg?color=black)](https://github.com/theAbdoSabbagh/PyBetterThreads/blob/main/LICENSE)
 
 PyBetterThreads is a Python library for adding more features to the threading module in Python. 
 
 PyBetterThreads makes it possible to return values from threads, and adds a finished signal so that the user can execute a function once the thread is finished. It is still in early development, and more features will be added soon.
 
 ## Installation
 You can install PyBetterThreads using pip:
```

### Comparing `pybetterthreads-0.0.1/PyBetterThreads/BetterThread.py` & `pybetterthreads-0.0.2/PyBetterThreads/BetterThread.py`

 * *Files identical despite different names*

### Comparing `pybetterthreads-0.0.1/PyBetterThreads.egg-info/PKG-INFO` & `pybetterthreads-0.0.2/PyBetterThreads.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBetterThreads
-Version: 0.0.1
+Version: 0.0.2
 Summary: Threads, but with more features!
 Home-page: https://github.com/theAbdoSabbagh/PyBetterThreads
 Author: theAbdoSabbagh
 License: MIT
 Project-URL: Documentation, https://github.com/theAbdoSabbagh/PyBetterThreads/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/theAbdoSabbagh/PyBetterThreads/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,17 +24,17 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyBetterThreads
 
-[![Downloads](https://static.pepy.tech/badge/betterthread)](https://pepy.tech/project/betterthread)
+[![Downloads](https://static.pepy.tech/badge/pybetterthreads)](https://pepy.tech/project/pybetterthreads)
 [![PyPi](https://img.shields.io/pypi/v/PyBetterThreads.svg)](https://pypi.python.org/pypi/PyBetterThreads)
-[![License](https://img.shields.io/github/license/theAbdoSabbagh/PyBetterThreads.svg?color=black)](https://github.com/theAbdoSabbagh/PyBetterThreads/main/LICENSE)
+[![License](https://img.shields.io/github/license/theAbdoSabbagh/PyBetterThreads.svg?color=black)](https://github.com/theAbdoSabbagh/PyBetterThreads/blob/main/LICENSE)
 
 PyBetterThreads is a Python library for adding more features to the threading module in Python. 
 
 PyBetterThreads makes it possible to return values from threads, and adds a finished signal so that the user can execute a function once the thread is finished. It is still in early development, and more features will be added soon.
 
 ## Installation
 You can install PyBetterThreads using pip:
```

### Comparing `pybetterthreads-0.0.1/README.md` & `pybetterthreads-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PyBetterThreads
 
-[![Downloads](https://static.pepy.tech/badge/betterthread)](https://pepy.tech/project/betterthread)
+[![Downloads](https://static.pepy.tech/badge/pybetterthreads)](https://pepy.tech/project/pybetterthreads)
 [![PyPi](https://img.shields.io/pypi/v/PyBetterThreads.svg)](https://pypi.python.org/pypi/PyBetterThreads)
-[![License](https://img.shields.io/github/license/theAbdoSabbagh/PyBetterThreads.svg?color=black)](https://github.com/theAbdoSabbagh/PyBetterThreads/main/LICENSE)
+[![License](https://img.shields.io/github/license/theAbdoSabbagh/PyBetterThreads.svg?color=black)](https://github.com/theAbdoSabbagh/PyBetterThreads/blob/main/LICENSE)
 
 PyBetterThreads is a Python library for adding more features to the threading module in Python. 
 
 PyBetterThreads makes it possible to return values from threads, and adds a finished signal so that the user can execute a function once the thread is finished. It is still in early development, and more features will be added soon.
 
 ## Installation
 You can install PyBetterThreads using pip:
@@ -51,8 +51,8 @@
 - [x] Execute a function once the thread is finished
 - [ ] More features coming soon!
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Star History
-[![Star History Chart](https://api.star-history.com/svg?repos=theAbdoSabbagh/PyBetterThreads&type=Date&theme=dark)](https://star-history.com/#theAbdoSabbagh/PyBetterThreads&Date&theme=dark)
+[![Star History Chart](https://api.star-history.com/svg?repos=theAbdoSabbagh/PyBetterThreads&type=Date&theme=dark)](https://star-history.com/#theAbdoSabbagh/PyBetterThreads&Date&theme=dark)
```

### Comparing `pybetterthreads-0.0.1/setup.py` & `pybetterthreads-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     name="PyBetterThreads",
     author="theAbdoSabbagh",
     url="https://github.com/theAbdoSabbagh/PyBetterThreads",
     project_urls={
         "Documentation": "https://github.com/theAbdoSabbagh/PyBetterThreads/blob/main/README.md",
         "Issue tracker": "https://github.com/theAbdoSabbagh/PyBetterThreads/issues",
     },
-    version="0.0.1",
+    version="0.0.2",
     packages=["PyBetterThreads"],
     license="MIT",
     description="Threads, but with more features!",
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     install_requires=[],
```

