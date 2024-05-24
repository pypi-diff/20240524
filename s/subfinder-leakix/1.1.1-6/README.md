# Comparing `tmp/subfinder-leakix-1.1.1.tar.gz` & `tmp/subfinder-leakix-6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subfinder-leakix-1.1.1.tar", last modified: Fri May 24 16:01:36 2024, max compression
+gzip compressed data, was "subfinder-leakix-6.tar", last modified: Thu May 23 01:24:24 2024, max compression
```

## Comparing `subfinder-leakix-1.1.1.tar` & `subfinder-leakix-6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:01:36.974320 subfinder-leakix-1.1.1/
--rw-r--r--   0 root         (0) root         (0)       45 2024-05-22 23:44:05.000000 subfinder-leakix-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      483 2024-05-24 16:01:36.974320 subfinder-leakix-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      240 2024-05-23 10:56:28.000000 subfinder-leakix-1.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 16:01:36.974320 subfinder-leakix-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      441 2024-05-24 16:01:33.000000 subfinder-leakix-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:01:36.974320 subfinder-leakix-1.1.1/subfinder_leakix.egg-info/
--rw-r--r--   0 root         (0) root         (0)      483 2024-05-24 16:01:36.000000 subfinder-leakix-1.1.1/subfinder_leakix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      225 2024-05-24 16:01:36.000000 subfinder-leakix-1.1.1/subfinder_leakix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 16:01:36.000000 subfinder-leakix-1.1.1/subfinder_leakix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-24 16:01:36.000000 subfinder-leakix-1.1.1/subfinder_leakix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 16:01:36.000000 subfinder-leakix-1.1.1/subfinder_leakix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 01:24:24.969324 subfinder-leakix-6/
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-22 23:44:05.000000 subfinder-leakix-6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-23 01:24:24.969324 subfinder-leakix-6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-22 23:55:30.000000 subfinder-leakix-6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 01:24:24.969324 subfinder-leakix-6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1038 2024-05-23 01:24:20.000000 subfinder-leakix-6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 01:24:24.969324 subfinder-leakix-6/subfinder_leakix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-23 01:24:24.000000 subfinder-leakix-6/subfinder_leakix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      268 2024-05-23 01:24:24.000000 subfinder-leakix-6/subfinder_leakix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 01:24:24.000000 subfinder-leakix-6/subfinder_leakix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 01:24:24.000000 subfinder-leakix-6/subfinder_leakix.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-23 01:24:24.000000 subfinder-leakix-6/subfinder_leakix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 01:24:24.000000 subfinder-leakix-6/subfinder_leakix.egg-info/top_level.txt
```

