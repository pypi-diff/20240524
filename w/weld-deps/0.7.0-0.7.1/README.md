# Comparing `tmp/weld_deps-0.7.0.tar.gz` & `tmp/weld_deps-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weld_deps-0.7.0.tar", max compression
+gzip compressed data, was "weld_deps-0.7.1.tar", max compression
```

## Comparing `weld_deps-0.7.0.tar` & `weld_deps-0.7.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2024-05-07 17:28:54.433695 weld_deps-0.7.0/LICENSE
--rw-r--r--   0        0        0      333 2024-05-07 17:29:13.065493 weld_deps-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       31 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/__init__.py
--rw-r--r--   0        0        0     6076 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/dep.py
--rw-r--r--   0        0        0      267 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/examples/pack1/beet.yaml
--rw-r--r--   0        0        0        0 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/examples/pack1/src/data/pack1/functions/test.mcfunction
--rw-r--r--   0        0        0      261 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/examples/pack_no_versions/beet.yaml
--rw-r--r--   0        0        0        0 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/examples/pack_no_versions/src/data/pack_not_found/functions/test.mcfunction
--rw-r--r--   0        0        0      262 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/examples/pack_not_found/beet.yaml
--rw-r--r--   0        0        0        0 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/examples/pack_not_found/src/data/pack_not_found/functions/test.mcfunction
--rw-r--r--   0        0        0     1858 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/main.py
--rw-r--r--   0        0        0     5124 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/utils.py
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 weld_deps-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-24 19:23:38.232109 weld_deps-0.7.1/LICENSE
+-rw-r--r--   0        0        0      332 2024-05-24 19:23:56.228227 weld_deps-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-24 19:23:38.232109 weld_deps-0.7.1/weld_deps/__init__.py
+-rw-r--r--   0        0        0     6076 2024-05-24 19:23:38.232109 weld_deps-0.7.1/weld_deps/dep.py
+-rw-r--r--   0        0        0      267 2024-05-24 19:23:38.232109 weld_deps-0.7.1/weld_deps/examples/pack1/beet.yaml
+-rw-r--r--   0        0        0        0 2024-05-24 19:23:38.232109 weld_deps-0.7.1/weld_deps/examples/pack1/src/data/pack1/functions/test.mcfunction
+-rw-r--r--   0        0        0      261 2024-05-24 19:23:38.232109 weld_deps-0.7.1/weld_deps/examples/pack_no_versions/beet.yaml
+-rw-r--r--   0        0        0        0 2024-05-24 19:23:38.232109 weld_deps-0.7.1/weld_deps/examples/pack_no_versions/src/data/pack_not_found/functions/test.mcfunction
+-rw-r--r--   0        0        0      262 2024-05-24 19:23:38.232109 weld_deps-0.7.1/weld_deps/examples/pack_not_found/beet.yaml
+-rw-r--r--   0        0        0        0 2024-05-24 19:23:38.232109 weld_deps-0.7.1/weld_deps/examples/pack_not_found/src/data/pack_not_found/functions/test.mcfunction
+-rw-r--r--   0        0        0     1858 2024-05-24 19:23:38.232109 weld_deps-0.7.1/weld_deps/main.py
+-rw-r--r--   0        0        0     5124 2024-05-24 19:23:38.232109 weld_deps-0.7.1/weld_deps/utils.py
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 weld_deps-0.7.1/PKG-INFO
```

### Comparing `weld_deps-0.7.0/LICENSE` & `weld_deps-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `weld_deps-0.7.0/weld_deps/dep.py` & `weld_deps-0.7.1/weld_deps/dep.py`

 * *Files identical despite different names*

### Comparing `weld_deps-0.7.0/weld_deps/main.py` & `weld_deps-0.7.1/weld_deps/main.py`

 * *Files identical despite different names*

### Comparing `weld_deps-0.7.0/weld_deps/utils.py` & `weld_deps-0.7.1/weld_deps/utils.py`

 * *Files identical despite different names*

