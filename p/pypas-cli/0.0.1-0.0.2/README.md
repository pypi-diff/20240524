# Comparing `tmp/pypas_cli-0.0.1.tar.gz` & `tmp/pypas_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypas_cli-0.0.1.tar", last modified: Sun Apr 28 19:08:24 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pypas_cli-0.0.1.tar` & `pypas_cli-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2024-04-28 19:08:24.459674 pypas_cli-0.0.1/
--rw-r--r--   0 sdelquin   (501) staff       (20)     1080 2024-04-28 18:56:18.000000 pypas_cli-0.0.1/LICENSE
--rw-r--r--   0 sdelquin   (501) staff       (20)      270 2024-04-28 19:08:24.459472 pypas_cli-0.0.1/PKG-INFO
--rw-r--r--   0 sdelquin   (501) staff       (20)       12 2024-04-28 18:56:54.000000 pypas_cli-0.0.1/README.md
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2024-04-28 19:08:24.458617 pypas_cli-0.0.1/pypas/
--rw-r--r--   0 sdelquin   (501) staff       (20)        7 2024-04-28 19:01:29.000000 pypas_cli-0.0.1/pypas/core.py
-drwxr-xr-x   0 sdelquin   (501) staff       (20)        0 2024-04-28 19:08:24.459302 pypas_cli-0.0.1/pypas_cli.egg-info/
--rw-r--r--   0 sdelquin   (501) staff       (20)      270 2024-04-28 19:08:24.000000 pypas_cli-0.0.1/pypas_cli.egg-info/PKG-INFO
--rw-r--r--   0 sdelquin   (501) staff       (20)      172 2024-04-28 19:08:24.000000 pypas_cli-0.0.1/pypas_cli.egg-info/SOURCES.txt
--rw-r--r--   0 sdelquin   (501) staff       (20)        1 2024-04-28 19:08:24.000000 pypas_cli-0.0.1/pypas_cli.egg-info/dependency_links.txt
--rw-r--r--   0 sdelquin   (501) staff       (20)        6 2024-04-28 19:08:24.000000 pypas_cli-0.0.1/pypas_cli.egg-info/top_level.txt
--rw-r--r--   0 sdelquin   (501) staff       (20)       38 2024-04-28 19:08:24.459715 pypas_cli-0.0.1/setup.cfg
--rw-r--r--   0 sdelquin   (501) staff       (20)      588 2024-04-28 19:00:45.000000 pypas_cli-0.0.1/setup.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pypas_cli-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pypas_cli-0.0.2/justfile
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypas_cli-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pypas_cli-0.0.2/src/pypas/core.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pypas_cli-0.0.2/src/pypas/main.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pypas_cli-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pypas_cli-0.0.2/LICENSE
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.2/README.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pypas_cli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 pypas_cli-0.0.2/PKG-INFO
```

### Comparing `pypas_cli-0.0.1/LICENSE` & `pypas_cli-0.0.2/LICENSE`

 * *Files identical despite different names*

