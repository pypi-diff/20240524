# Comparing `tmp/myscale-telemetry-0.1.0.tar.gz` & `tmp/myscale-telemetry-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myscale-telemetry-0.1.0.tar", last modified: Fri May 24 05:22:28 2024, max compression
+gzip compressed data, was "myscale-telemetry-0.1.1.tar", last modified: Fri May 24 06:59:37 2024, max compression
```

## Comparing `myscale-telemetry-0.1.0.tar` & `myscale-telemetry-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 05:22:28.747638 myscale-telemetry-0.1.0/
--rw-r--r--   0 xuj        (501) staff       (20)     1064 2024-05-21 03:32:44.000000 myscale-telemetry-0.1.0/LICENSE
--rw-r--r--   0 xuj        (501) staff       (20)      416 2024-05-24 05:22:28.747516 myscale-telemetry-0.1.0/PKG-INFO
--rw-r--r--   0 xuj        (501) staff       (20)     5894 2024-05-24 05:19:23.000000 myscale-telemetry-0.1.0/README.md
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 05:22:28.746611 myscale-telemetry-0.1.0/myscale_telemetry/
--rw-r--r--   0 xuj        (501) staff       (20)        0 2024-05-21 05:08:28.000000 myscale-telemetry-0.1.0/myscale_telemetry/__init__.py
--rw-r--r--   0 xuj        (501) staff       (20)     5569 2024-05-21 05:09:24.000000 myscale-telemetry-0.1.0/myscale_telemetry/consumer.py
--rw-r--r--   0 xuj        (501) staff       (20)    21572 2024-05-24 04:42:34.000000 myscale-telemetry-0.1.0/myscale_telemetry/handler.py
--rw-r--r--   0 xuj        (501) staff       (20)     3671 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.0/myscale_telemetry/span_data.py
--rw-r--r--   0 xuj        (501) staff       (20)     6557 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.0/myscale_telemetry/task_manager.py
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 05:22:28.747354 myscale-telemetry-0.1.0/myscale_telemetry.egg-info/
--rw-r--r--   0 xuj        (501) staff       (20)      416 2024-05-24 05:22:28.000000 myscale-telemetry-0.1.0/myscale_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 xuj        (501) staff       (20)      384 2024-05-24 05:22:28.000000 myscale-telemetry-0.1.0/myscale_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 xuj        (501) staff       (20)        1 2024-05-24 05:22:28.000000 myscale-telemetry-0.1.0/myscale_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 xuj        (501) staff       (20)       85 2024-05-24 05:22:28.000000 myscale-telemetry-0.1.0/myscale_telemetry.egg-info/requires.txt
--rw-r--r--   0 xuj        (501) staff       (20)       18 2024-05-24 05:22:28.000000 myscale-telemetry-0.1.0/myscale_telemetry.egg-info/top_level.txt
--rw-r--r--   0 xuj        (501) staff       (20)       38 2024-05-24 05:22:28.747678 myscale-telemetry-0.1.0/setup.cfg
--rw-r--r--   0 xuj        (501) staff       (20)      676 2024-05-24 05:22:26.000000 myscale-telemetry-0.1.0/setup.py
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 06:59:37.702933 myscale-telemetry-0.1.1/
+-rw-r--r--   0 xuj        (501) staff       (20)     1064 2024-05-21 03:32:44.000000 myscale-telemetry-0.1.1/LICENSE
+-rw-r--r--   0 xuj        (501) staff       (20)     6351 2024-05-24 06:59:37.702807 myscale-telemetry-0.1.1/PKG-INFO
+-rw-r--r--   0 xuj        (501) staff       (20)     5894 2024-05-24 05:19:23.000000 myscale-telemetry-0.1.1/README.md
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 06:59:37.701800 myscale-telemetry-0.1.1/myscale_telemetry/
+-rw-r--r--   0 xuj        (501) staff       (20)        0 2024-05-21 05:08:28.000000 myscale-telemetry-0.1.1/myscale_telemetry/__init__.py
+-rw-r--r--   0 xuj        (501) staff       (20)     5569 2024-05-21 05:09:24.000000 myscale-telemetry-0.1.1/myscale_telemetry/consumer.py
+-rw-r--r--   0 xuj        (501) staff       (20)    21572 2024-05-24 04:42:34.000000 myscale-telemetry-0.1.1/myscale_telemetry/handler.py
+-rw-r--r--   0 xuj        (501) staff       (20)     3671 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.1/myscale_telemetry/span_data.py
+-rw-r--r--   0 xuj        (501) staff       (20)     6557 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.1/myscale_telemetry/task_manager.py
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 06:59:37.702581 myscale-telemetry-0.1.1/myscale_telemetry.egg-info/
+-rw-r--r--   0 xuj        (501) staff       (20)     6351 2024-05-24 06:59:37.000000 myscale-telemetry-0.1.1/myscale_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 xuj        (501) staff       (20)      384 2024-05-24 06:59:37.000000 myscale-telemetry-0.1.1/myscale_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 xuj        (501) staff       (20)        1 2024-05-24 06:59:37.000000 myscale-telemetry-0.1.1/myscale_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       85 2024-05-24 06:59:37.000000 myscale-telemetry-0.1.1/myscale_telemetry.egg-info/requires.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       18 2024-05-24 06:59:37.000000 myscale-telemetry-0.1.1/myscale_telemetry.egg-info/top_level.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       38 2024-05-24 06:59:37.702979 myscale-telemetry-0.1.1/setup.cfg
+-rw-r--r--   0 xuj        (501) staff       (20)      893 2024-05-24 06:59:36.000000 myscale-telemetry-0.1.1/setup.py
```

### Comparing `myscale-telemetry-0.1.0/LICENSE` & `myscale-telemetry-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.0/README.md` & `myscale-telemetry-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.0/myscale_telemetry/consumer.py` & `myscale-telemetry-0.1.1/myscale_telemetry/consumer.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.0/myscale_telemetry/handler.py` & `myscale-telemetry-0.1.1/myscale_telemetry/handler.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.0/myscale_telemetry/span_data.py` & `myscale-telemetry-0.1.1/myscale_telemetry/span_data.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.0/myscale_telemetry/task_manager.py` & `myscale-telemetry-0.1.1/myscale_telemetry/task_manager.py`

 * *Files identical despite different names*

