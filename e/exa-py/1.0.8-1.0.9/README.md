# Comparing `tmp/exa_py-1.0.8.tar.gz` & `tmp/exa_py-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exa_py-1.0.8.tar", last modified: Mon Feb  5 22:16:55 2024, max compression
+gzip compressed data, was "exa_py-1.0.9.tar", last modified: Tue Mar 12 17:58:06 2024, max compression
```

## Comparing `exa_py-1.0.8.tar` & `exa_py-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2024-02-05 22:16:55.170316 exa_py-1.0.8/
--rw-r--r--   0 jwang      (501) staff       (20)     2992 2024-02-05 22:16:55.170173 exa_py-1.0.8/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)     2301 2024-02-05 22:16:44.000000 exa_py-1.0.8/README.md
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2024-02-05 22:16:55.169384 exa_py-1.0.8/exa_py/
--rw-r--r--   0 jwang      (501) staff       (20)       29 2024-01-25 13:31:48.000000 exa_py-1.0.8/exa_py/__init__.py
--rw-r--r--   0 jwang      (501) staff       (20)    22932 2024-02-05 22:16:18.000000 exa_py-1.0.8/exa_py/api.py
--rw-r--r--   0 jwang      (501) staff       (20)        0 2024-01-25 13:31:48.000000 exa_py-1.0.8/exa_py/py.typed
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2024-02-05 22:16:55.169970 exa_py-1.0.8/exa_py.egg-info/
--rw-r--r--   0 jwang      (501) staff       (20)     2992 2024-02-05 22:16:55.000000 exa_py-1.0.8/exa_py.egg-info/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)      216 2024-02-05 22:16:55.000000 exa_py-1.0.8/exa_py.egg-info/SOURCES.txt
--rw-r--r--   0 jwang      (501) staff       (20)        1 2024-02-05 22:16:55.000000 exa_py-1.0.8/exa_py.egg-info/dependency_links.txt
--rw-r--r--   0 jwang      (501) staff       (20)        9 2024-02-05 22:16:55.000000 exa_py-1.0.8/exa_py.egg-info/requires.txt
--rw-r--r--   0 jwang      (501) staff       (20)        7 2024-02-05 22:16:55.000000 exa_py-1.0.8/exa_py.egg-info/top_level.txt
--rw-r--r--   0 jwang      (501) staff       (20)       38 2024-02-05 22:16:55.170361 exa_py-1.0.8/setup.cfg
--rw-r--r--   0 jwang      (501) staff       (20)      952 2024-02-05 22:16:00.000000 exa_py-1.0.8/setup.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2024-03-12 17:58:06.257119 exa_py-1.0.9/
+-rw-r--r--   0 jwang      (501) staff       (20)     2992 2024-03-12 17:58:06.256973 exa_py-1.0.9/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)     2301 2024-02-05 22:16:44.000000 exa_py-1.0.9/README.md
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2024-03-12 17:58:06.256157 exa_py-1.0.9/exa_py/
+-rw-r--r--   0 jwang      (501) staff       (20)       29 2024-01-25 13:31:48.000000 exa_py-1.0.9/exa_py/__init__.py
+-rw-r--r--   0 jwang      (501) staff       (20)    22932 2024-03-12 17:57:49.000000 exa_py-1.0.9/exa_py/api.py
+-rw-r--r--   0 jwang      (501) staff       (20)        0 2024-01-25 13:31:48.000000 exa_py-1.0.9/exa_py/py.typed
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2024-03-12 17:58:06.256785 exa_py-1.0.9/exa_py.egg-info/
+-rw-r--r--   0 jwang      (501) staff       (20)     2992 2024-03-12 17:58:06.000000 exa_py-1.0.9/exa_py.egg-info/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)      216 2024-03-12 17:58:06.000000 exa_py-1.0.9/exa_py.egg-info/SOURCES.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        1 2024-03-12 17:58:06.000000 exa_py-1.0.9/exa_py.egg-info/dependency_links.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       27 2024-03-12 17:58:06.000000 exa_py-1.0.9/exa_py.egg-info/requires.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        7 2024-03-12 17:58:06.000000 exa_py-1.0.9/exa_py.egg-info/top_level.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       38 2024-03-12 17:58:06.257173 exa_py-1.0.9/setup.cfg
+-rw-r--r--   0 jwang      (501) staff       (20)      981 2024-03-12 17:57:54.000000 exa_py-1.0.9/setup.py
```

### Comparing `exa_py-1.0.8/PKG-INFO` & `exa_py-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exa_py
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python SDK for Exa API.
 Home-page: https://github.com/exa-labs/exa-py
 Author: Exa
 Author-email: hello@exa.ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `exa_py-1.0.8/README.md` & `exa_py-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `exa_py-1.0.8/exa_py/api.py` & `exa_py-1.0.9/exa_py/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
 class Exa:
     """A client for interacting with Exa API."""
 
     def __init__(
         self,
         api_key: Optional[str],
         base_url: str = "https://api.exa.ai",
-        user_agent: str = "exa-py 1.0.7",
+        user_agent: str = "exa-py 1.0.9",
     ):
         """Initialize the Exa client with the provided API key and optional base URL and user agent.
 
         Args:
             api_key (str): The API key for authenticating with the Exa API.
             base_url (str, optional): The base URL for the Exa API. Defaults to "https://api.exa.ai".
         """
```

### Comparing `exa_py-1.0.8/exa_py.egg-info/PKG-INFO` & `exa_py-1.0.9/exa_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exa-py
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python SDK for Exa API.
 Home-page: https://github.com/exa-labs/exa-py
 Author: Exa
 Author-email: hello@exa.ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `exa_py-1.0.8/setup.py` & `exa_py-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="exa_py",
-    version="1.0.8",
+    version="1.0.9",
     description="Python SDK for Exa API.",
     long_description_content_type="text/markdown",
     long_description=open("README.md").read(),
     author="Exa",
     author_email="hello@exa.ai",
     package_data={"exa_py": ["py.typed"]},
     url="https://github.com/exa-labs/exa-py",
     packages=find_packages(),
     install_requires=[
         "requests",
+        "typing-extensions",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Typing :: Typed",
         "Programming Language :: Python :: 3.7",
```

