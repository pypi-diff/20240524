# Comparing `tmp/AAIT-0.0.2.3.tar.gz` & `tmp/AAIT-0.0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAIT-0.0.2.3.tar", last modified: Thu May 23 19:59:34 2024, max compression
+gzip compressed data, was "AAIT-0.0.2.4.tar", last modified: Fri May 24 07:37:57 2024, max compression
```

## Comparing `AAIT-0.0.2.3.tar` & `AAIT-0.0.2.4.tar`

### file list

```diff
@@ -1,31 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.184966 AAIT-0.0.2.3/
-drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.177449 AAIT-0.0.2.3/AAIT.egg-info/
--rw-rw-rw-   0        0        0      236 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      775 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       29 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/License.txt
--rw-rw-rw-   0        0        0      236 2024-05-23 19:59:34.183963 AAIT-0.0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.178452 AAIT-0.0.2.3/orangecontrib/
-drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.178452 AAIT-0.0.2.3/orangecontrib/AAIT/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.179452 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/
--rw-rw-rw-   0        0        0     1351 2024-05-23 16:08:53.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/OWEmbeddings.py
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.180450 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/designer/
--rw-rw-rw-   0        0        0      134 2024-05-23 11:59:32.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/designer/owembeddings.ui
-drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.183963 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/
--rw-rw-rw-   0        0        0      831 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg
--rw-rw-rw-   0        0        0     1596 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/DocumentEater.svg
--rw-rw-rw-   0        0        0     4195 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/Embeddings.svg
--rw-rw-rw-   0        0        0     1357 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/LanguageModel.svg
--rw-rw-rw-   0        0        0      500 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/TextPreprocessing.svg
--rw-rw-rw-   0        0        0     1082 2024-02-19 21:08:44.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/chatbot.svg
--rw-rw-rw-   0        0        0      755 2024-05-23 16:32:22.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/owembeddings.svg
--rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-23 19:59:34.184966 AAIT-0.0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1753 2024-05-23 19:59:28.000000 AAIT-0.0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:37:57.731571 AAIT-0.0.2.4/
+drwxrwxrwx   0        0        0        0 2024-05-24 07:37:57.729206 AAIT-0.0.2.4/AAIT.egg-info/
+-rw-rw-rw-   0        0        0      236 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       29 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.4/License.txt
+-rw-rw-rw-   0        0        0      236 2024-05-24 07:37:57.730564 AAIT-0.0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 07:37:57.729514 AAIT-0.0.2.4/orangecontrib/
+drwxrwxrwx   0        0        0        0 2024-05-24 07:37:57.729514 AAIT-0.0.2.4/orangecontrib/AAIT/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.4/orangecontrib/AAIT/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:37:57.730564 AAIT-0.0.2.4/orangecontrib/AAIT/widgets/
+-rw-rw-rw-   0        0        0      392 2024-05-23 18:26:14.000000 AAIT-0.0.2.4/orangecontrib/AAIT/widgets/__init__.py
+-rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT-0.0.2.4/orangecontrib/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-24 07:37:57.731571 AAIT-0.0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1753 2024-05-24 07:37:52.000000 AAIT-0.0.2.4/setup.py
```

### Comparing `AAIT-0.0.2.3/setup.py` & `AAIT-0.0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Nom du package PyPI ('pip install NAME')
 NAME = "AAIT"
 
 # Version du package PyPI
-VERSION = "0.0.2.3" # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.0.2.4" # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
 AUTHOR = ""
 AUTHOR_EMAIL = ""
 URL = ""
 DESCRIPTION = "LLM addons for Orange Data Mining !"
 LICENSE = ""
```

