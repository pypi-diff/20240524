# Comparing `tmp/AAIT-0.0.2.6.tar.gz` & `tmp/AAIT-0.0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAIT-0.0.2.6.tar", last modified: Fri May 24 08:47:13 2024, max compression
+gzip compressed data, was "AAIT-0.0.2.7.tar", last modified: Fri May 24 09:01:43 2024, max compression
```

## Comparing `AAIT-0.0.2.6.tar` & `AAIT-0.0.2.7.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 08:47:13.007996 AAIT-0.0.2.6/
-drwxrwxrwx   0        0        0        0 2024-05-24 08:47:13.004996 AAIT-0.0.2.6/AAIT.egg-info/
--rw-rw-rw-   0        0        0      236 2024-05-24 08:47:12.000000 AAIT-0.0.2.6/AAIT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2024-05-24 08:47:12.000000 AAIT-0.0.2.6/AAIT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 08:47:12.000000 AAIT-0.0.2.6/AAIT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-24 08:47:12.000000 AAIT-0.0.2.6/AAIT.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-24 08:47:12.000000 AAIT-0.0.2.6/AAIT.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       29 2024-05-24 08:47:12.000000 AAIT-0.0.2.6/AAIT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-24 08:47:12.000000 AAIT-0.0.2.6/AAIT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.6/License.txt
--rw-rw-rw-   0        0        0      236 2024-05-24 08:47:13.006996 AAIT-0.0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 08:47:13.005997 AAIT-0.0.2.6/orangecontrib/
-drwxrwxrwx   0        0        0        0 2024-05-24 08:47:13.005997 AAIT-0.0.2.6/orangecontrib/AAIT/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.6/orangecontrib/AAIT/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:47:13.005997 AAIT-0.0.2.6/orangecontrib/AAIT/widgets/
--rw-rw-rw-   0        0        0      392 2024-05-23 18:26:14.000000 AAIT-0.0.2.6/orangecontrib/AAIT/widgets/__init__.py
--rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT-0.0.2.6/orangecontrib/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-24 08:47:13.007996 AAIT-0.0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1761 2024-05-24 08:47:04.000000 AAIT-0.0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:43.537672 AAIT-0.0.2.7/
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:43.533673 AAIT-0.0.2.7/AAIT.egg-info/
+-rw-rw-rw-   0        0        0      236 2024-05-24 09:01:43.000000 AAIT-0.0.2.7/AAIT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2024-05-24 09:01:43.000000 AAIT-0.0.2.7/AAIT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 09:01:43.000000 AAIT-0.0.2.7/AAIT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-24 09:01:43.000000 AAIT-0.0.2.7/AAIT.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 09:01:43.000000 AAIT-0.0.2.7/AAIT.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       29 2024-05-24 09:01:43.000000 AAIT-0.0.2.7/AAIT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 09:01:43.000000 AAIT-0.0.2.7/AAIT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.7/License.txt
+-rw-rw-rw-   0        0        0      236 2024-05-24 09:01:43.536672 AAIT-0.0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:43.534672 AAIT-0.0.2.7/orangecontrib/
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:43.534672 AAIT-0.0.2.7/orangecontrib/AAIT/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.7/orangecontrib/AAIT/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:43.535672 AAIT-0.0.2.7/orangecontrib/AAIT/llm/
+-rw-rw-rw-   0        0        0     1043 2024-05-23 13:36:26.000000 AAIT-0.0.2.7/orangecontrib/AAIT/llm/embeddings.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:43.535672 AAIT-0.0.2.7/orangecontrib/AAIT/widgets/
+-rw-rw-rw-   0        0        0      392 2024-05-23 18:26:14.000000 AAIT-0.0.2.7/orangecontrib/AAIT/widgets/__init__.py
+-rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT-0.0.2.7/orangecontrib/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-24 09:01:43.537672 AAIT-0.0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1792 2024-05-24 09:01:37.000000 AAIT-0.0.2.7/setup.py
```

### Comparing `AAIT-0.0.2.6/setup.py` & `AAIT-0.0.2.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Nom du package PyPI ('pip install NAME')
 NAME = "AAIT"
 
 # Version du package PyPI
-VERSION = "0.0.2.6" # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.0.2.7" # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
 AUTHOR = ""
 AUTHOR_EMAIL = ""
 URL = ""
 DESCRIPTION = "LLM addons for Orange Data Mining !"
 LICENSE = ""
@@ -18,24 +18,25 @@
 
 # Tous les packages python existants dans le projet
 PACKAGES = find_packages()
 
 # Fichiers additionnels aux fichiers .py (comme les icons ou des .ows)
 PACKAGE_DATA = {
 	"orangecontrib.AAIT.widgets.llm": ["icons/*", "designer/*"], # contenu du dossier 'icons' situé dans 'orangecontrib/hkh_bot/widgets'
+	"orangecontrib.AAIT": ["llm/*"],
 }
 # /!\ les noms de fichier 'orangecontrib.hkh_bot.widgets' doivent correspondre à l'arborescence
 
 # Dépendances
 INSTALL_REQUIRES = ["sentence-transformers==2.5.1"]
 
 # Spécifie le dossier contenant les widgets et le nom de section qu'aura l'addon sur Orange
 ENTRY_POINTS = {
 	"orange.widgets": (
-		"AAIT = orangecontrib.AAIT.widgets.llm", # 'HKH-Bot' sera le nom de la section Orange contenant les widgets
+		"AAIT = orangecontrib.AAIT.widgets", # 'HKH-Bot' sera le nom de la section Orange contenant les widgets
 	)
 }
 # /!\ les noms de fichier 'orangecontrib.hkh_bot.widgets' doivent correspondre à l'arborescence
 
 NAMESPACE_PACKAGES = ["orangecontrib"]
 
 setup(name=NAME,
```

