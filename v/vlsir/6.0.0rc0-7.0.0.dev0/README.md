# Comparing `tmp/vlsir-6.0.0rc0.tar.gz` & `tmp/vlsir-7.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlsir-6.0.0rc0.tar", last modified: Fri May 24 16:31:38 2024, max compression
+gzip compressed data, was "vlsir-7.0.0.dev0.tar", last modified: Fri May 24 17:31:47 2024, max compression
```

## Comparing `vlsir-6.0.0rc0.tar` & `vlsir-7.0.0.dev0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:38.239307 vlsir-6.0.0rc0/
--rw-r--r--   0 dan        (501) staff       (20)     2762 2023-04-26 23:15:43.000000 vlsir-6.0.0rc0/.gitignore
--rw-r--r--   0 dan        (501) staff       (20)     1521 2023-04-26 23:15:43.000000 vlsir-6.0.0rc0/LICENSE
--rw-r--r--   0 dan        (501) staff       (20)      415 2024-05-24 16:31:38.239097 vlsir-6.0.0rc0/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)       98 2023-06-26 21:21:08.000000 vlsir-6.0.0rc0/readme.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-24 16:31:38.239354 vlsir-6.0.0rc0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)     1629 2024-05-24 16:23:33.000000 vlsir-6.0.0rc0/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:38.234512 vlsir-6.0.0rc0/tests/
--rw-r--r--   0 dan        (501) staff       (20)        0 2023-04-26 23:15:43.000000 vlsir-6.0.0rc0/tests/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     1186 2023-06-28 18:09:23.000000 vlsir-6.0.0rc0/tests/test_vlsir.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:38.238062 vlsir-6.0.0rc0/vlsir/
--rw-r--r--   0 dan        (501) staff       (20)      679 2024-05-24 16:26:14.000000 vlsir-6.0.0rc0/vlsir/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     4919 2024-05-24 16:07:55.000000 vlsir-6.0.0rc0/vlsir/circuit_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)     5884 2023-08-30 20:52:59.000000 vlsir-6.0.0rc0/vlsir/geometry_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)     2092 2024-05-24 16:07:55.000000 vlsir-6.0.0rc0/vlsir/netlist_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)     8928 2023-08-30 20:52:59.000000 vlsir-6.0.0rc0/vlsir/raw_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)    14458 2024-05-24 16:07:55.000000 vlsir-6.0.0rc0/vlsir/spice_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)     2152 2024-05-24 16:07:55.000000 vlsir-6.0.0rc0/vlsir/tech_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)    17522 2023-08-30 20:52:59.000000 vlsir-6.0.0rc0/vlsir/tetris_pb2.py
--rw-r--r--   0 dan        (501) staff       (20)     3602 2024-05-24 16:07:55.000000 vlsir-6.0.0rc0/vlsir/utils_pb2.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:38.238882 vlsir-6.0.0rc0/vlsir.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)      415 2024-05-24 16:31:38.000000 vlsir-6.0.0rc0/vlsir.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      394 2024-05-24 16:31:38.000000 vlsir-6.0.0rc0/vlsir.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-24 16:31:38.000000 vlsir-6.0.0rc0/vlsir.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       72 2024-05-24 16:31:38.000000 vlsir-6.0.0rc0/vlsir.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       12 2024-05-24 16:31:38.000000 vlsir-6.0.0rc0/vlsir.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:31:47.805372 vlsir-7.0.0.dev0/
+-rw-r--r--   0 dan        (501) staff       (20)     2762 2023-04-26 23:15:43.000000 vlsir-7.0.0.dev0/.gitignore
+-rw-r--r--   0 dan        (501) staff       (20)     1521 2023-04-26 23:15:43.000000 vlsir-7.0.0.dev0/LICENSE
+-rw-r--r--   0 dan        (501) staff       (20)      487 2024-05-24 17:31:47.805093 vlsir-7.0.0.dev0/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)       98 2023-06-26 21:21:08.000000 vlsir-7.0.0.dev0/readme.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-24 17:31:47.805420 vlsir-7.0.0.dev0/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)     1564 2024-05-24 17:28:43.000000 vlsir-7.0.0.dev0/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:31:47.800699 vlsir-7.0.0.dev0/tests/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2023-04-26 23:15:43.000000 vlsir-7.0.0.dev0/tests/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     1186 2023-06-28 18:09:23.000000 vlsir-7.0.0.dev0/tests/test_vlsir.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:31:47.803368 vlsir-7.0.0.dev0/vlsir/
+-rw-r--r--   0 dan        (501) staff       (20)      681 2024-05-24 17:28:43.000000 vlsir-7.0.0.dev0/vlsir/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     4919 2024-05-24 16:07:55.000000 vlsir-7.0.0.dev0/vlsir/circuit_pb2.py
+-rw-r--r--   0 dan        (501) staff       (20)     5884 2023-08-30 20:52:59.000000 vlsir-7.0.0.dev0/vlsir/geometry_pb2.py
+-rw-r--r--   0 dan        (501) staff       (20)     2092 2024-05-24 16:07:55.000000 vlsir-7.0.0.dev0/vlsir/netlist_pb2.py
+-rw-r--r--   0 dan        (501) staff       (20)     8928 2023-08-30 20:52:59.000000 vlsir-7.0.0.dev0/vlsir/raw_pb2.py
+-rw-r--r--   0 dan        (501) staff       (20)    14458 2024-05-24 16:07:55.000000 vlsir-7.0.0.dev0/vlsir/spice_pb2.py
+-rw-r--r--   0 dan        (501) staff       (20)     2152 2024-05-24 16:07:55.000000 vlsir-7.0.0.dev0/vlsir/tech_pb2.py
+-rw-r--r--   0 dan        (501) staff       (20)    17522 2023-08-30 20:52:59.000000 vlsir-7.0.0.dev0/vlsir/tetris_pb2.py
+-rw-r--r--   0 dan        (501) staff       (20)     3602 2024-05-24 16:07:55.000000 vlsir-7.0.0.dev0/vlsir/utils_pb2.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:31:47.804583 vlsir-7.0.0.dev0/vlsir.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)      487 2024-05-24 17:31:47.000000 vlsir-7.0.0.dev0/vlsir.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      394 2024-05-24 17:31:47.000000 vlsir-7.0.0.dev0/vlsir.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-24 17:31:47.000000 vlsir-7.0.0.dev0/vlsir.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       31 2024-05-24 17:31:47.000000 vlsir-7.0.0.dev0/vlsir.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       12 2024-05-24 17:31:47.000000 vlsir-7.0.0.dev0/vlsir.egg-info/top_level.txt
```

### Comparing `vlsir-6.0.0rc0/.gitignore` & `vlsir-7.0.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `vlsir-6.0.0rc0/LICENSE` & `vlsir-7.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `vlsir-6.0.0rc0/setup.py` & `vlsir-7.0.0.dev0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pathlib
 
 # Get the long description from the README file
 here = pathlib.Path(__file__).parent.resolve()
 readme = here / "readme.md"
 long_description = "" if not readme.exists() else readme.read_text(encoding="utf-8")
 
-VLSIR_VERSION = "6.0.0rc0"
+VLSIR_VERSION = "7.0.0.dev0"
 
 setup(
     name="vlsir",
     version=VLSIR_VERSION,
     description="Python Bindings to the VLSIR Data Schemas for Chip Design",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -36,11 +36,9 @@
         # Note:
         # This version of protobuf differs pretty substantially from the ones before it;
         # Most binding-code is *not* generated per-schema, but is in the protobuf package,
         # And schema-derived types are generated on the fly.
         # So, versions before this will generally fail pretty hard.
         "protobuf~=4.23"
     ],
-    extras_require={
-        "dev": ["pytest==7.1", "coverage", "pytest-cov", "black==22.6", "twine"]
-    },
+    extras_require={"dev": ["vlsirdev"]},
 )
```

### Comparing `vlsir-6.0.0rc0/tests/test_vlsir.py` & `vlsir-7.0.0.dev0/tests/test_vlsir.py`

 * *Files identical despite different names*

### Comparing `vlsir-6.0.0rc0/vlsir/__init__.py` & `vlsir-7.0.0.dev0/vlsir/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 # VLSIR Python Bindings 
 
 Note while most modules in this package are protobuf-compiler generated, 
 *this* top-level namespace module is not! 
 """
 
-__version__ = "6.0.0rc0" # VLSIR_VERSION
+__version__ = "7.0.0.dev0" # VLSIR_VERSION
 
 # Schema
 from . import utils_pb2 as utils
 from . import spice_pb2 as spice
 from . import circuit_pb2 as circuit
 from . import netlist_pb2 as netlist
 from . import raw_pb2 as raw
```

### Comparing `vlsir-6.0.0rc0/vlsir/circuit_pb2.py` & `vlsir-7.0.0.dev0/vlsir/circuit_pb2.py`

 * *Files identical despite different names*

### Comparing `vlsir-6.0.0rc0/vlsir/geometry_pb2.py` & `vlsir-7.0.0.dev0/vlsir/geometry_pb2.py`

 * *Files identical despite different names*

### Comparing `vlsir-6.0.0rc0/vlsir/netlist_pb2.py` & `vlsir-7.0.0.dev0/vlsir/netlist_pb2.py`

 * *Files identical despite different names*

### Comparing `vlsir-6.0.0rc0/vlsir/raw_pb2.py` & `vlsir-7.0.0.dev0/vlsir/raw_pb2.py`

 * *Files identical despite different names*

### Comparing `vlsir-6.0.0rc0/vlsir/spice_pb2.py` & `vlsir-7.0.0.dev0/vlsir/spice_pb2.py`

 * *Files identical despite different names*

### Comparing `vlsir-6.0.0rc0/vlsir/tech_pb2.py` & `vlsir-7.0.0.dev0/vlsir/tech_pb2.py`

 * *Files identical despite different names*

### Comparing `vlsir-6.0.0rc0/vlsir/tetris_pb2.py` & `vlsir-7.0.0.dev0/vlsir/tetris_pb2.py`

 * *Files identical despite different names*

### Comparing `vlsir-6.0.0rc0/vlsir/utils_pb2.py` & `vlsir-7.0.0.dev0/vlsir/utils_pb2.py`

 * *Files identical despite different names*

