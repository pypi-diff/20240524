# Comparing `tmp/neuro_all-24.5.0.tar.gz` & `tmp/neuro_all-24.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro_all-24.5.0.tar", max compression
+gzip compressed data, was "neuro_all-24.5.1.tar", max compression
```

## Comparing `neuro_all-24.5.0.tar` & `neuro_all-24.5.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2024-05-21 12:50:15.581942 neuro_all-24.5.0/LICENSE
--rw-r--r--   0        0        0      107 2024-05-21 12:50:15.581942 neuro_all-24.5.0/README.md
--rw-r--r--   0        0        0      462 2024-05-21 12:50:15.581942 neuro_all-24.5.0/neuro_all/__init__.py
--rw-r--r--   0        0        0     1657 2024-05-21 12:50:15.581942 neuro_all-24.5.0/pyproject.toml
--rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 neuro_all-24.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 15:46:25.622299 neuro_all-24.5.1/LICENSE
+-rw-r--r--   0        0        0      107 2024-05-24 15:46:25.622299 neuro_all-24.5.1/README.md
+-rw-r--r--   0        0        0      462 2024-05-24 15:46:25.622299 neuro_all-24.5.1/neuro_all/__init__.py
+-rw-r--r--   0        0        0     1657 2024-05-24 15:46:25.622299 neuro_all-24.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 neuro_all-24.5.1/PKG-INFO
```

### Comparing `neuro_all-24.5.0/LICENSE` & `neuro_all-24.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro_all-24.5.0/pyproject.toml` & `neuro_all-24.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neuro-all"
-version = "24.5.0"
+version = "24.5.1"
 description = "Combo package for installing all neu.ro command line tools by 'pipx install neuro-all' command"
 authors = ["Neu.ro Team <team@neu.ro>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://neu.ro"
 repository = "https://github.com/neuro-inc/neuro-all"
 keywords = [
@@ -40,15 +40,15 @@
 docker-credential-neuro = "neuro_cli.docker_credential_helper:main"
 neuro-extras = "neuro_extras:main"
 neuro-flow = "neuro_flow.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
 neuro-cli = "24.5.0"
-neuro-extras = "24.2.0"
+neuro-extras = "24.5.0"
 neuro-flow = "24.2.0"
 certifi = "2024.2.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "8.1.1"
 pre-commit = "^3.5.0"
 click = "^8.1.7"
```

### Comparing `neuro_all-24.5.0/PKG-INFO` & `neuro_all-24.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-all
-Version: 24.5.0
+Version: 24.5.1
 Summary: Combo package for installing all neu.ro command line tools by 'pipx install neuro-all' command
 Home-page: https://neu.ro
 License: Apache-2.0
 Keywords: neu.ro,mlops
 Author: Neu.ro Team
 Author-email: team@neu.ro
 Requires-Python: >=3.8.0,<4.0.0
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Dist: certifi (==2024.2.2)
 Requires-Dist: neuro-cli (==24.5.0)
-Requires-Dist: neuro-extras (==24.2.0)
+Requires-Dist: neuro-extras (==24.5.0)
 Requires-Dist: neuro-flow (==24.2.0)
 Project-URL: Repository, https://github.com/neuro-inc/neuro-all
 Description-Content-Type: text/markdown
 
 # neuro-all
 Combo package for installing all neu.ro command line tools by `pipx install neuro-all` command
```

