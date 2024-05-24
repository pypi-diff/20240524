# Comparing `tmp/AAIT-0.0.2.8.tar.gz` & `tmp/AAIT-0.0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAIT-0.0.2.8.tar", last modified: Fri May 24 09:04:12 2024, max compression
+gzip compressed data, was "AAIT-0.0.2.9.tar", last modified: Fri May 24 09:08:50 2024, max compression
```

## Comparing `AAIT-0.0.2.8.tar` & `AAIT-0.0.2.9.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 09:04:12.448537 AAIT-0.0.2.8/
-drwxrwxrwx   0        0        0        0 2024-05-24 09:04:12.444535 AAIT-0.0.2.8/AAIT.egg-info/
--rw-rw-rw-   0        0        0      236 2024-05-24 09:04:12.000000 AAIT-0.0.2.8/AAIT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2024-05-24 09:04:12.000000 AAIT-0.0.2.8/AAIT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 09:04:12.000000 AAIT-0.0.2.8/AAIT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-24 09:04:12.000000 AAIT-0.0.2.8/AAIT.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-24 09:04:12.000000 AAIT-0.0.2.8/AAIT.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       29 2024-05-24 09:04:12.000000 AAIT-0.0.2.8/AAIT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-24 09:04:12.000000 AAIT-0.0.2.8/AAIT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.8/License.txt
--rw-rw-rw-   0        0        0      236 2024-05-24 09:04:12.448537 AAIT-0.0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 09:04:12.445535 AAIT-0.0.2.8/orangecontrib/
-drwxrwxrwx   0        0        0        0 2024-05-24 09:04:12.445535 AAIT-0.0.2.8/orangecontrib/AAIT/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.8/orangecontrib/AAIT/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:04:12.446550 AAIT-0.0.2.8/orangecontrib/AAIT/llm/
--rw-rw-rw-   0        0        0     1043 2024-05-23 13:36:26.000000 AAIT-0.0.2.8/orangecontrib/AAIT/llm/embeddings.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:04:12.447537 AAIT-0.0.2.8/orangecontrib/AAIT/widgets/
--rw-rw-rw-   0        0        0      392 2024-05-23 18:26:14.000000 AAIT-0.0.2.8/orangecontrib/AAIT/widgets/__init__.py
--rw-rw-rw-   0        0        0     1930 2024-05-23 17:30:45.000000 AAIT-0.0.2.8/orangecontrib/AAIT/widgets/category.svg
--rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT-0.0.2.8/orangecontrib/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-24 09:04:12.448537 AAIT-0.0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1806 2024-05-24 09:03:20.000000 AAIT-0.0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:08:50.826450 AAIT-0.0.2.9/
+drwxrwxrwx   0        0        0        0 2024-05-24 09:08:50.819918 AAIT-0.0.2.9/AAIT.egg-info/
+-rw-rw-rw-   0        0        0      236 2024-05-24 09:08:50.000000 AAIT-0.0.2.9/AAIT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      605 2024-05-24 09:08:50.000000 AAIT-0.0.2.9/AAIT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 09:08:50.000000 AAIT-0.0.2.9/AAIT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-24 09:08:50.000000 AAIT-0.0.2.9/AAIT.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 09:08:50.000000 AAIT-0.0.2.9/AAIT.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       29 2024-05-24 09:08:50.000000 AAIT-0.0.2.9/AAIT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 09:08:50.000000 AAIT-0.0.2.9/AAIT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.9/License.txt
+-rw-rw-rw-   0        0        0      236 2024-05-24 09:08:50.825453 AAIT-0.0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 09:08:50.820431 AAIT-0.0.2.9/orangecontrib/
+drwxrwxrwx   0        0        0        0 2024-05-24 09:08:50.820431 AAIT-0.0.2.9/orangecontrib/AAIT/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.9/orangecontrib/AAIT/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:08:50.821444 AAIT-0.0.2.9/orangecontrib/AAIT/llm/
+-rw-rw-rw-   0        0        0        0 2024-05-24 09:07:42.000000 AAIT-0.0.2.9/orangecontrib/AAIT/llm/__init__.py
+-rw-rw-rw-   0        0        0     1043 2024-05-23 13:36:26.000000 AAIT-0.0.2.9/orangecontrib/AAIT/llm/embeddings.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:08:50.822450 AAIT-0.0.2.9/orangecontrib/AAIT/widgets/
+-rw-rw-rw-   0        0        0      392 2024-05-23 18:26:14.000000 AAIT-0.0.2.9/orangecontrib/AAIT/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:08:50.823450 AAIT-0.0.2.9/orangecontrib/AAIT/widgets/llm/
+-rw-rw-rw-   0        0        0     1351 2024-05-23 16:08:53.000000 AAIT-0.0.2.9/orangecontrib/AAIT/widgets/llm/OWEmbeddings.py
+-rw-rw-rw-   0        0        0        0 2024-05-24 09:07:58.000000 AAIT-0.0.2.9/orangecontrib/AAIT/widgets/llm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:08:50.823450 AAIT-0.0.2.9/orangecontrib/AAIT/widgets/llm/designer/
+-rw-rw-rw-   0        0        0      134 2024-05-23 11:59:32.000000 AAIT-0.0.2.9/orangecontrib/AAIT/widgets/llm/designer/owembeddings.ui
+drwxrwxrwx   0        0        0        0 2024-05-24 09:08:50.824450 AAIT-0.0.2.9/orangecontrib/AAIT/widgets/llm/icons/
+-rw-rw-rw-   0        0        0      755 2024-05-23 16:32:22.000000 AAIT-0.0.2.9/orangecontrib/AAIT/widgets/llm/icons/owembeddings.svg
+-rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT-0.0.2.9/orangecontrib/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-24 09:08:50.826450 AAIT-0.0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1757 2024-05-24 09:08:34.000000 AAIT-0.0.2.9/setup.py
```

### Comparing `AAIT-0.0.2.8/orangecontrib/AAIT/llm/embeddings.py` & `AAIT-0.0.2.9/orangecontrib/AAIT/llm/embeddings.py`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2.8/setup.py` & `AAIT-0.0.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Nom du package PyPI ('pip install NAME')
 NAME = "AAIT"
 
 # Version du package PyPI
-VERSION = "0.0.2.8" # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.0.2.9" # la version doit être supérieure à la précédente sinon la publication sera refusée
 
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
-	#"orangecontrib.AAIT.widgets.llm": ["icons/*", "designer/*"], # contenu du dossier 'icons' situé dans 'orangecontrib/hkh_bot/widgets'
-	"orangecontrib.AAIT": ["llm/*", "widgets/*"],
+	"orangecontrib.AAIT.widgets.llm": ["icons/*", "designer/*"], # contenu du dossier 'icons' situé dans 'orangecontrib/hkh_bot/widgets'
 }
 # /!\ les noms de fichier 'orangecontrib.hkh_bot.widgets' doivent correspondre à l'arborescence
 
 # Dépendances
 INSTALL_REQUIRES = ["sentence-transformers==2.5.1"]
 
 # Spécifie le dossier contenant les widgets et le nom de section qu'aura l'addon sur Orange
```

