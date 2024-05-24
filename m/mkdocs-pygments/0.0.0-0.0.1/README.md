# Comparing `tmp/mkdocs_pygments-0.0.0.tar.gz` & `tmp/mkdocs_pygments-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_pygments-0.0.0.tar", last modified: Fri May 17 18:00:02 2024, max compression
+gzip compressed data, was "mkdocs_pygments-0.0.1.tar", last modified: Fri May 24 13:13:18 2024, max compression
```

## Comparing `mkdocs_pygments-0.0.0.tar` & `mkdocs_pygments-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,8 @@
-drwxr-xr-x   0 pawamoy   (1000) users      (985)        0 2024-05-17 18:00:02.430339 mkdocs_pygments-0.0.0/
--rw-r--r--   0 pawamoy   (1000) users      (985)      504 2024-05-17 18:00:02.430339 mkdocs_pygments-0.0.0/PKG-INFO
--rw-r--r--   0 pawamoy   (1000) users      (985)      206 2024-05-17 17:59:56.000000 mkdocs_pygments-0.0.0/README.md
-drwxr-xr-x   0 pawamoy   (1000) users      (985)        0 2024-05-17 18:00:02.430339 mkdocs_pygments-0.0.0/mkdocs_pygments.egg-info/
--rw-r--r--   0 pawamoy   (1000) users      (985)      504 2024-05-17 18:00:02.000000 mkdocs_pygments-0.0.0/mkdocs_pygments.egg-info/PKG-INFO
--rw-r--r--   0 pawamoy   (1000) users      (985)      180 2024-05-17 18:00:02.000000 mkdocs_pygments-0.0.0/mkdocs_pygments.egg-info/SOURCES.txt
--rw-r--r--   0 pawamoy   (1000) users      (985)        1 2024-05-17 18:00:02.000000 mkdocs_pygments-0.0.0/mkdocs_pygments.egg-info/dependency_links.txt
--rw-r--r--   0 pawamoy   (1000) users      (985)        1 2024-05-17 18:00:02.000000 mkdocs_pygments-0.0.0/mkdocs_pygments.egg-info/top_level.txt
--rw-r--r--   0 pawamoy   (1000) users      (985)      306 2024-05-17 17:59:56.000000 mkdocs_pygments-0.0.0/pyproject.toml
--rw-r--r--   0 pawamoy   (1000) users      (985)       38 2024-05-17 18:00:02.430339 mkdocs_pygments-0.0.0/setup.cfg
+-rw-r--r--   0        0        0      754 2024-05-20 17:36:13.286685 mkdocs_pygments-0.0.1/LICENSE
+-rw-r--r--   0        0        0     2689 2024-05-20 17:36:13.553324 mkdocs_pygments-0.0.1/README.md
+-rw-r--r--   0        0        0     1817 2024-05-24 13:13:18.700727 mkdocs_pygments-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-05-20 17:36:14.219921 mkdocs_pygments-0.0.1/src/mkdocs_pygments/__init__.py
+-rw-r--r--   0        0        0     2846 2024-05-20 17:36:14.219921 mkdocs_pygments-0.0.1/src/mkdocs_pygments/debug.py
+-rw-r--r--   0        0        0      642 2024-05-24 13:09:46.166579 mkdocs_pygments-0.0.1/src/mkdocs_pygments/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-20 17:36:14.219921 mkdocs_pygments-0.0.1/src/mkdocs_pygments/py.typed
+-rw-r--r--   0        0        0     4169 1970-01-01 00:00:00.000000 mkdocs_pygments-0.0.1/PKG-INFO
```

