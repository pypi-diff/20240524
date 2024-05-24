# Comparing `tmp/AAIT-0.0.2.4.tar.gz` & `tmp/AAIT-0.0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAIT-0.0.2.4.tar", last modified: Fri May 24 07:37:57 2024, max compression
+gzip compressed data, was "AAIT-0.0.2.5.tar", last modified: Fri May 24 08:18:18 2024, max compression
```

## Comparing `AAIT-0.0.2.4.tar` & `AAIT-0.0.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 07:37:57.731571 AAIT-0.0.2.4/
-drwxrwxrwx   0        0        0        0 2024-05-24 07:37:57.729206 AAIT-0.0.2.4/AAIT.egg-info/
--rw-rw-rw-   0        0        0      236 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       29 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-24 07:37:57.000000 AAIT-0.0.2.4/AAIT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.4/License.txt
--rw-rw-rw-   0        0        0      236 2024-05-24 07:37:57.730564 AAIT-0.0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 07:37:57.729514 AAIT-0.0.2.4/orangecontrib/
-drwxrwxrwx   0        0        0        0 2024-05-24 07:37:57.729514 AAIT-0.0.2.4/orangecontrib/AAIT/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.4/orangecontrib/AAIT/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:37:57.730564 AAIT-0.0.2.4/orangecontrib/AAIT/widgets/
--rw-rw-rw-   0        0        0      392 2024-05-23 18:26:14.000000 AAIT-0.0.2.4/orangecontrib/AAIT/widgets/__init__.py
--rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT-0.0.2.4/orangecontrib/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-24 07:37:57.731571 AAIT-0.0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1753 2024-05-24 07:37:52.000000 AAIT-0.0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 08:18:18.190281 AAIT-0.0.2.5/
+drwxrwxrwx   0        0        0        0 2024-05-24 08:18:18.187767 AAIT-0.0.2.5/AAIT.egg-info/
+-rw-rw-rw-   0        0        0      236 2024-05-24 08:18:18.000000 AAIT-0.0.2.5/AAIT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2024-05-24 08:18:18.000000 AAIT-0.0.2.5/AAIT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 08:18:18.000000 AAIT-0.0.2.5/AAIT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-24 08:18:18.000000 AAIT-0.0.2.5/AAIT.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 08:18:18.000000 AAIT-0.0.2.5/AAIT.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       29 2024-05-24 08:18:18.000000 AAIT-0.0.2.5/AAIT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 08:18:18.000000 AAIT-0.0.2.5/AAIT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.5/License.txt
+-rw-rw-rw-   0        0        0      236 2024-05-24 08:18:18.190281 AAIT-0.0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 08:18:18.187767 AAIT-0.0.2.5/orangecontrib/
+drwxrwxrwx   0        0        0        0 2024-05-24 08:18:18.188772 AAIT-0.0.2.5/orangecontrib/AAIT/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.5/orangecontrib/AAIT/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 08:18:18.189276 AAIT-0.0.2.5/orangecontrib/AAIT/widgets/
+-rw-rw-rw-   0        0        0      392 2024-05-23 18:26:14.000000 AAIT-0.0.2.5/orangecontrib/AAIT/widgets/__init__.py
+-rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT-0.0.2.5/orangecontrib/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-24 08:18:18.190281 AAIT-0.0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1757 2024-05-24 08:18:03.000000 AAIT-0.0.2.5/setup.py
```

### Comparing `AAIT-0.0.2.4/setup.py` & `AAIT-0.0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Nom du package PyPI ('pip install NAME')
 NAME = "AAIT"
 
 # Version du package PyPI
-VERSION = "0.0.2.4" # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.0.2.5" # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
 AUTHOR = ""
 AUTHOR_EMAIL = ""
 URL = ""
 DESCRIPTION = "LLM addons for Orange Data Mining !"
 LICENSE = ""
@@ -17,15 +17,15 @@
 KEYWORDS = ("orange3 add-on",)
 
 # Tous les packages python existants dans le projet
 PACKAGES = find_packages()
 
 # Fichiers additionnels aux fichiers .py (comme les icons ou des .ows)
 PACKAGE_DATA = {
-	"orangecontrib.AAIT.widgets": ["icons/*", "designer/*"], # contenu du dossier 'icons' situé dans 'orangecontrib/hkh_bot/widgets'
+	"orangecontrib.AAIT.widgets.llm": ["icons/*", "designer/*"], # contenu du dossier 'icons' situé dans 'orangecontrib/hkh_bot/widgets'
 }
 # /!\ les noms de fichier 'orangecontrib.hkh_bot.widgets' doivent correspondre à l'arborescence
 
 # Dépendances
 INSTALL_REQUIRES = ["sentence-transformers==2.5.1"]
 
 # Spécifie le dossier contenant les widgets et le nom de section qu'aura l'addon sur Orange
```

