# Comparing `tmp/kub-0.0.2.tar.gz` & `tmp/kub-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "kub-0.1.0.tar", max compression
```

## Comparing `kub-0.0.2.tar` & `kub-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 kub-0.0.2/.DS_Store
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 kub-0.0.2/src/KUB/KUB.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kub-0.0.2/src/KUB/__init__.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 kub-0.0.2/LICENSE
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 kub-0.0.2/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 kub-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 kub-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-26 02:01:01.716187 kub-0.1.0/LICENSE
+-rw-r--r--   0        0        0       46 2023-08-26 02:01:01.716427 kub-0.1.0/README.md
+-rw-r--r--   0        0        0      327 2024-04-28 17:41:41.705060 kub-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7642 2024-05-24 14:03:48.796275 kub-0.1.0/src/kub/KUB.py
+-rw-r--r--   0        0        0        0 2023-08-26 12:23:34.125444 kub-0.1.0/src/kub/__init__.py
+-rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 kub-0.1.0/PKG-INFO
```

### Comparing `kub-0.0.2/LICENSE` & `kub-0.1.0/LICENSE`

 * *Files identical despite different names*

