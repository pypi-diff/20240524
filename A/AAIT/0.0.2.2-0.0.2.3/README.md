# Comparing `tmp/AAIT-0.0.2.2.tar.gz` & `tmp/AAIT-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAIT-0.0.2.2.tar", last modified: Thu May 23 19:56:20 2024, max compression
+gzip compressed data, was "AAIT-0.0.2.3.tar", last modified: Thu May 23 19:59:34 2024, max compression
```

## Comparing `AAIT-0.0.2.2.tar` & `AAIT-0.0.2.3.tar`

### file list

```diff
@@ -1,33 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 19:56:20.873722 AAIT-0.0.2.2/
-drwxrwxrwx   0        0        0        0 2024-05-23 19:56:20.866206 AAIT-0.0.2.2/AAIT.egg-info/
--rw-rw-rw-   0        0        0      236 2024-05-23 19:56:20.000000 AAIT-0.0.2.2/AAIT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      811 2024-05-23 19:56:20.000000 AAIT-0.0.2.2/AAIT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 19:56:20.000000 AAIT-0.0.2.2/AAIT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-23 19:56:20.000000 AAIT-0.0.2.2/AAIT.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 19:56:20.000000 AAIT-0.0.2.2/AAIT.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       29 2024-05-23 19:56:20.000000 AAIT-0.0.2.2/AAIT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 19:56:20.000000 AAIT-0.0.2.2/AAIT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.2/License.txt
--rw-rw-rw-   0        0        0      236 2024-05-23 19:56:20.873722 AAIT-0.0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 19:56:20.866206 AAIT-0.0.2.2/orangecontrib/
-drwxrwxrwx   0        0        0        0 2024-05-23 19:56:20.867203 AAIT-0.0.2.2/orangecontrib/AAIT/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.2/orangecontrib/AAIT/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:56:20.868196 AAIT-0.0.2.2/orangecontrib/AAIT/examples/
--rw-rw-rw-   0        0        0     7856 2024-02-20 12:43:50.000000 AAIT-0.0.2.2/orangecontrib/AAIT/examples/example-chatbot.ows
--rw-rw-rw-   0        0        0      966 2024-03-06 08:40:04.000000 AAIT-0.0.2.2/orangecontrib/AAIT/execute_thread.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:56:20.869197 AAIT-0.0.2.2/orangecontrib/AAIT/widgets/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.2/orangecontrib/AAIT/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:56:20.872200 AAIT-0.0.2.2/orangecontrib/AAIT/widgets/icons/
--rw-rw-rw-   0        0        0      831 2024-01-18 15:57:45.000000 AAIT-0.0.2.2/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg
--rw-rw-rw-   0        0        0     1596 2024-01-18 15:57:45.000000 AAIT-0.0.2.2/orangecontrib/AAIT/widgets/icons/DocumentEater.svg
--rw-rw-rw-   0        0        0     4195 2024-01-18 15:57:45.000000 AAIT-0.0.2.2/orangecontrib/AAIT/widgets/icons/Embeddings.svg
--rw-rw-rw-   0        0        0     1357 2024-01-18 15:57:45.000000 AAIT-0.0.2.2/orangecontrib/AAIT/widgets/icons/LanguageModel.svg
--rw-rw-rw-   0        0        0      500 2024-01-18 15:57:45.000000 AAIT-0.0.2.2/orangecontrib/AAIT/widgets/icons/TextPreprocessing.svg
--rw-rw-rw-   0        0        0     1082 2024-02-19 21:08:44.000000 AAIT-0.0.2.2/orangecontrib/AAIT/widgets/icons/chatbot.svg
--rw-rw-rw-   0        0        0     8204 2024-03-12 21:47:18.000000 AAIT-0.0.2.2/orangecontrib/AAIT/widgets/owchatbot.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:56:20.872712 AAIT-0.0.2.2/orangecontrib/AAIT/widgets/widget_designer/
--rw-rw-rw-   0        0        0     2337 2024-03-04 19:45:00.000000 AAIT-0.0.2.2/orangecontrib/AAIT/widgets/widget_designer/owchatbot.ui
--rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT-0.0.2.2/orangecontrib/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-23 19:56:20.873722 AAIT-0.0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1800 2024-05-23 19:56:14.000000 AAIT-0.0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.184966 AAIT-0.0.2.3/
+drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.177449 AAIT-0.0.2.3/AAIT.egg-info/
+-rw-rw-rw-   0        0        0      236 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       29 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 19:59:34.000000 AAIT-0.0.2.3/AAIT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/License.txt
+-rw-rw-rw-   0        0        0      236 2024-05-23 19:59:34.183963 AAIT-0.0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.178452 AAIT-0.0.2.3/orangecontrib/
+drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.178452 AAIT-0.0.2.3/orangecontrib/AAIT/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.179452 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/
+-rw-rw-rw-   0        0        0     1351 2024-05-23 16:08:53.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/OWEmbeddings.py
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.180450 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/designer/
+-rw-rw-rw-   0        0        0      134 2024-05-23 11:59:32.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/designer/owembeddings.ui
+drwxrwxrwx   0        0        0        0 2024-05-23 19:59:34.183963 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/
+-rw-rw-rw-   0        0        0      831 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg
+-rw-rw-rw-   0        0        0     1596 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/DocumentEater.svg
+-rw-rw-rw-   0        0        0     4195 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/Embeddings.svg
+-rw-rw-rw-   0        0        0     1357 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/LanguageModel.svg
+-rw-rw-rw-   0        0        0      500 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/TextPreprocessing.svg
+-rw-rw-rw-   0        0        0     1082 2024-02-19 21:08:44.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/chatbot.svg
+-rw-rw-rw-   0        0        0      755 2024-05-23 16:32:22.000000 AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/owembeddings.svg
+-rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT-0.0.2.3/orangecontrib/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 19:59:34.184966 AAIT-0.0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1753 2024-05-23 19:59:28.000000 AAIT-0.0.2.3/setup.py
```

### Comparing `AAIT-0.0.2.2/AAIT.egg-info/SOURCES.txt` & `AAIT-0.0.2.3/AAIT.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 AAIT.egg-info/dependency_links.txt
 AAIT.egg-info/entry_points.txt
 AAIT.egg-info/namespace_packages.txt
 AAIT.egg-info/requires.txt
 AAIT.egg-info/top_level.txt
 orangecontrib/__init__.py
 orangecontrib/AAIT/__init__.py
-orangecontrib/AAIT/execute_thread.py
-orangecontrib/AAIT/examples/example-chatbot.ows
+orangecontrib/AAIT/widgets/OWEmbeddings.py
 orangecontrib/AAIT/widgets/__init__.py
-orangecontrib/AAIT/widgets/owchatbot.py
+orangecontrib/AAIT/widgets/designer/owembeddings.ui
 orangecontrib/AAIT/widgets/icons/Chatbotpy.svg
 orangecontrib/AAIT/widgets/icons/DocumentEater.svg
 orangecontrib/AAIT/widgets/icons/Embeddings.svg
 orangecontrib/AAIT/widgets/icons/LanguageModel.svg
 orangecontrib/AAIT/widgets/icons/TextPreprocessing.svg
 orangecontrib/AAIT/widgets/icons/chatbot.svg
-orangecontrib/AAIT/widgets/widget_designer/owchatbot.ui
+orangecontrib/AAIT/widgets/icons/owembeddings.svg
```

### Comparing `AAIT-0.0.2.2/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg` & `AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2.2/orangecontrib/AAIT/widgets/icons/DocumentEater.svg` & `AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/DocumentEater.svg`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2.2/orangecontrib/AAIT/widgets/icons/Embeddings.svg` & `AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/Embeddings.svg`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2.2/orangecontrib/AAIT/widgets/icons/LanguageModel.svg` & `AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/LanguageModel.svg`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2.2/orangecontrib/AAIT/widgets/icons/chatbot.svg` & `AAIT-0.0.2.3/orangecontrib/AAIT/widgets/icons/chatbot.svg`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2.2/setup.py` & `AAIT-0.0.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Nom du package PyPI ('pip install NAME')
 NAME = "AAIT"
 
 # Version du package PyPI
-VERSION = "0.0.2.2" # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.0.2.3" # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
 AUTHOR = ""
 AUTHOR_EMAIL = ""
 URL = ""
 DESCRIPTION = "LLM addons for Orange Data Mining !"
 LICENSE = ""
@@ -17,16 +17,15 @@
 KEYWORDS = ("orange3 add-on",)
 
 # Tous les packages python existants dans le projet
 PACKAGES = find_packages()
 
 # Fichiers additionnels aux fichiers .py (comme les icons ou des .ows)
 PACKAGE_DATA = {
-	"orangecontrib.AAIT.widgets": ["icons/*", "widget_designer/*"], # contenu du dossier 'icons' situé dans 'orangecontrib/hkh_bot/widgets'
-	"orangecontrib.AAIT": ["examples/*"],
+	"orangecontrib.AAIT.widgets": ["icons/*", "designer/*"], # contenu du dossier 'icons' situé dans 'orangecontrib/hkh_bot/widgets'
 }
 # /!\ les noms de fichier 'orangecontrib.hkh_bot.widgets' doivent correspondre à l'arborescence
 
 # Dépendances
 INSTALL_REQUIRES = ["sentence-transformers==2.5.1"]
 
 # Spécifie le dossier contenant les widgets et le nom de section qu'aura l'addon sur Orange
```

