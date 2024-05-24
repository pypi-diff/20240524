# Comparing `tmp/decomp2dbg-3.9.1.tar.gz` & `tmp/decomp2dbg-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decomp2dbg-3.9.1.tar", last modified: Thu May  9 04:03:02 2024, max compression
+gzip compressed data, was "decomp2dbg-3.9.2.tar", last modified: Fri May 24 06:54:56 2024, max compression
```

## Comparing `decomp2dbg-3.9.1.tar` & `decomp2dbg-3.9.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/d2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.493087 decomp2dbg-3.9.1/decomp2dbg/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.493087 decomp2dbg-3.9.1/decomp2dbg/clients/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/decompiler_pane.py
--rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/gdb_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/gef_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/pwndbg_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/symbol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decomp2dbg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-09 04:03:02.000000 decomp2dbg-3.9.1/decomp2dbg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-09 04:03:02.000000 decomp2dbg-3.9.1/decomp2dbg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:03:02.000000 decomp2dbg-3.9.1/decomp2dbg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 04:03:02.000000 decomp2dbg-3.9.1/decomp2dbg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-09 04:03:02.000000 decomp2dbg-3.9.1/decomp2dbg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 04:03:02.000000 decomp2dbg-3.9.1/decomp2dbg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decompilers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decompilers/d2d_angr/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_angr/d2d_angr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_angr/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decompilers/d2d_binja/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_binja/d2d_binja.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_binja/plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_binja/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decompilers/d2d_ida/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/server_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:56.207970 decomp2dbg-3.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-24 06:54:56.207970 decomp2dbg-3.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/d2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:56.199970 decomp2dbg-3.9.2/decomp2dbg/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decomp2dbg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decomp2dbg/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:56.203970 decomp2dbg-3.9.2/decomp2dbg/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decomp2dbg/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decomp2dbg/clients/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:56.203970 decomp2dbg-3.9.2/decomp2dbg/clients/gdb/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decomp2dbg/clients/gdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decomp2dbg/clients/gdb/decompiler_pane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11050 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decomp2dbg/clients/gdb/gdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decomp2dbg/clients/gdb/gef_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decomp2dbg/clients/gdb/pwndbg_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decomp2dbg/clients/gdb/symbol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decomp2dbg/clients/gdb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decomp2dbg/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decomp2dbg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:56.207970 decomp2dbg-3.9.2/decomp2dbg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-24 06:54:56.000000 decomp2dbg-3.9.2/decomp2dbg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-24 06:54:56.000000 decomp2dbg-3.9.2/decomp2dbg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 06:54:56.000000 decomp2dbg-3.9.2/decomp2dbg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-24 06:54:56.000000 decomp2dbg-3.9.2/decomp2dbg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-24 06:54:56.000000 decomp2dbg-3.9.2/decomp2dbg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 06:54:56.000000 decomp2dbg-3.9.2/decomp2dbg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:56.203970 decomp2dbg-3.9.2/decompilers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:56.203970 decomp2dbg-3.9.2/decompilers/d2d_angr/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decompilers/d2d_angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decompilers/d2d_angr/d2d_angr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decompilers/d2d_angr/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:56.207970 decomp2dbg-3.9.2/decompilers/d2d_binja/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decompilers/d2d_binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decompilers/d2d_binja/d2d_binja.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decompilers/d2d_binja/plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decompilers/d2d_binja/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:56.207970 decomp2dbg-3.9.2/decompilers/d2d_ida/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:56.207970 decomp2dbg-3.9.2/decompilers/d2d_ida/d2d_ida/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decompilers/d2d_ida/d2d_ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decompilers/d2d_ida/d2d_ida/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decompilers/d2d_ida/d2d_ida/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decompilers/d2d_ida/d2d_ida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/decompilers/server_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-24 06:54:56.207970 decomp2dbg-3.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-24 06:54:52.000000 decomp2dbg-3.9.2/setup.py
```

### Comparing `decomp2dbg-3.9.1/LICENSE` & `decomp2dbg-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/PKG-INFO` & `decomp2dbg-3.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decomp2dbg
-Version: 3.9.1
+Version: 3.9.2
 Summary: Symbol syncing framework for decompilers and debuggers
 Home-page: https://github.com/mahaloz/decomp2dbg
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.5
```

### Comparing `decomp2dbg-3.9.1/README.md` & `decomp2dbg-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/d2d.py` & `decomp2dbg-3.9.2/d2d.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decomp2dbg/__main__.py` & `decomp2dbg-3.9.2/decomp2dbg/__main__.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decomp2dbg/clients/client.py` & `decomp2dbg-3.9.2/decomp2dbg/clients/client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decomp2dbg/clients/gdb/decompiler_pane.py` & `decomp2dbg-3.9.2/decomp2dbg/clients/gdb/decompiler_pane.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decomp2dbg/clients/gdb/gdb_client.py` & `decomp2dbg-3.9.2/decomp2dbg/clients/gdb/gdb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,19 +130,18 @@
         func_data = self.function_data(addr)
         reg_vars = func_data.get("reg_vars", {})
         stack_vars = func_data.get("stack_vars", {})
 
         for name, var in reg_vars.items():
             type_str = self._clean_type_str(var['type'])
             reg_name = var['reg_name']
-            expr = f"""(({type_str}) (${reg_name})"""
+            expr = f"""(({type_str}) (${reg_name}))"""
 
             try:
-                val = gdb.parse_and_eval(expr)
-                gdb.execute(f"set ${name} = {val}")
+                gdb.execute(f"set ${name} = {expr}")
                 type_unknown = False
             except Exception:
                 type_unknown = True
 
             if type_unknown:
                 try:
                     gdb.execute(f"set ${name} = (${reg_name})")
```

### Comparing `decomp2dbg-3.9.1/decomp2dbg/clients/gdb/gef_client.py` & `decomp2dbg-3.9.2/decomp2dbg/clients/gdb/gef_client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decomp2dbg/clients/gdb/pwndbg_client.py` & `decomp2dbg-3.9.2/decomp2dbg/clients/gdb/pwndbg_client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decomp2dbg/clients/gdb/symbol_mapper.py` & `decomp2dbg-3.9.2/decomp2dbg/clients/gdb/symbol_mapper.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decomp2dbg/clients/gdb/utils.py` & `decomp2dbg-3.9.2/decomp2dbg/clients/gdb/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 from functools import lru_cache
 import functools
 import collections
 import re
 import tempfile
 import hashlib
+from pathlib import Path
 
 from elftools.elf.elffile import ELFFile
 
 from ...utils import gef_pystring, warn, err
 
 import gdb
 
@@ -187,38 +188,44 @@
 
 
 
 @lru_cache()
 def get_filepath() -> Optional[str]:
     """Return the local absolute path of the file currently debugged."""
     filename = gdb.current_progspace().filename
-
+    filepath = None
     if is_remote_debug():
         # if no filename specified, try downloading target from /proc
         if filename is None:
             pid_ = pid()
             if pid_ > 0:
-                return download_file(f"/proc/{pid_:d}/exe", use_cache=True)
-            return None
-
+                filepath = download_file(f"/proc/{pid_:d}/exe", use_cache=True)
         # if target is remote file, download
         elif filename.startswith("target:"):
             fname = filename[len("target:") :]
-            return download_file(fname, use_cache=True, local_name=fname)
+            filepath = download_file(fname, use_cache=True, local_name=fname)
 
         elif filename.startswith(".gnu_debugdata for target:"):
             fname = filename[len(".gnu_debugdata for target:") :]
-            return download_file(fname, use_cache=True, local_name=fname)
-
-        return filename
+            filepath = download_file(fname, use_cache=True, local_name=fname)
+        else:
+            filepath = filename
     else:
         if filename is not None:
-            return filename
-        # inferior probably did not have name, extract cmdline from info proc
-        return get_path_from_info_proc()
+            filepath = filename
+        else:
+            # inferior probably did not have name, extract cmdline from info proc
+            filepath = get_path_from_info_proc()
+
+    try:
+        filepath = Path(filepath).resolve()
+    except Exception:
+        err(f"Failed to resolve path in get_filepath(): {filepath}, this error is fatal.")
+
+    return str(filepath) if filepath else None
 
 
 def get_path_from_info_proc() -> Optional[str]:
     for x in gdb.execute("info proc", to_string=True).splitlines():
         if x.startswith("exe = "):
             return x.split(" = ")[1].replace("'", "")
     return None
```

### Comparing `decomp2dbg-3.9.1/decomp2dbg/installer.py` & `decomp2dbg-3.9.2/decomp2dbg/installer.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decomp2dbg/utils.py` & `decomp2dbg-3.9.2/decomp2dbg/utils.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decomp2dbg.egg-info/PKG-INFO` & `decomp2dbg-3.9.2/decomp2dbg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decomp2dbg
-Version: 3.9.1
+Version: 3.9.2
 Summary: Symbol syncing framework for decompilers and debuggers
 Home-page: https://github.com/mahaloz/decomp2dbg
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.5
```

### Comparing `decomp2dbg-3.9.1/decomp2dbg.egg-info/SOURCES.txt` & `decomp2dbg-3.9.2/decomp2dbg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decompilers/d2d_angr/d2d_angr.py` & `decomp2dbg-3.9.2/decompilers/d2d_angr/d2d_angr.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decompilers/d2d_angr/server.py` & `decomp2dbg-3.9.2/decompilers/d2d_angr/server.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decompilers/d2d_binja/d2d_binja.py` & `decomp2dbg-3.9.2/decompilers/d2d_binja/d2d_binja.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decompilers/d2d_binja/plugin.json` & `decomp2dbg-3.9.2/decompilers/d2d_binja/plugin.json`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decompilers/d2d_binja/server.py` & `decomp2dbg-3.9.2/decompilers/d2d_binja/server.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida/plugin.py` & `decomp2dbg-3.9.2/decompilers/d2d_ida/d2d_ida/plugin.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida/server.py` & `decomp2dbg-3.9.2/decompilers/d2d_ida/d2d_ida/server.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/decompilers/server_template.py` & `decomp2dbg-3.9.2/decompilers/server_template.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/setup.cfg` & `decomp2dbg-3.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.1/setup.py` & `decomp2dbg-3.9.2/setup.py`

 * *Files identical despite different names*

