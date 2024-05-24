# Comparing `tmp/syndicate-py-0.8.5.tar.gz` & `tmp/syndicate-py-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syndicate-py-0.8.5.tar", last modified: Fri Jul 22 15:06:15 2022, max compression
+gzip compressed data, was "syndicate-py-0.9.0.tar", last modified: Mon Feb  6 22:31:52 2023, max compression
```

## Comparing `syndicate-py-0.8.5.tar` & `syndicate-py-0.9.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2022-07-22 15:06:15.878956 syndicate-py-0.8.5/
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      137 2022-01-11 17:22:01.000000 syndicate-py-0.8.5/.envrc
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)       75 2022-01-05 16:29:43.000000 syndicate-py-0.8.5/.gitignore
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      497 2021-11-30 17:47:05.000000 syndicate-py-0.8.5/Makefile
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      649 2022-07-22 15:06:15.878956 syndicate-py-0.8.5/PKG-INFO
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      798 2021-08-23 15:04:30.000000 syndicate-py-0.8.5/README.md
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     3865 2022-01-05 16:29:43.000000 syndicate-py-0.8.5/bidi-gc.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1952 2022-01-05 16:29:43.000000 syndicate-py-0.8.5/chat.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      264 2022-01-07 15:04:18.000000 syndicate-py-0.8.5/inf.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)       21 2021-08-23 15:04:30.000000 syndicate-py-0.8.5/requirements.txt
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)       38 2022-07-22 15:06:15.878956 syndicate-py-0.8.5/setup.cfg
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      946 2022-07-22 15:02:29.000000 syndicate-py-0.8.5/setup.py
-drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2022-07-22 15:06:15.878956 syndicate-py-0.8.5/syndicate/
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1323 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/__init__.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)    17938 2022-07-22 15:02:05.000000 syndicate-py-0.8.5/syndicate/actor.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2313 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/dataflow.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      568 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/dataspace.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2105 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/during.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      591 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/gatekeeper.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      231 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/idgen.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      222 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/mapset.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      538 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/metapy.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2927 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/patterns.py
-drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2022-07-22 15:06:15.878956 syndicate-py-0.8.5/syndicate/protocols/
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      140 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/protocols/Makefile
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)    13977 2022-02-04 19:51:34.000000 syndicate-py-0.8.5/syndicate/protocols/schema-bundle.bin
-drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2022-07-22 15:06:15.878956 syndicate-py-0.8.5/syndicate/protocols/schemas/
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      114 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/dataspace.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      543 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/dataspacePatterns.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      158 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/gatekeeper.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      471 2022-01-16 23:22:44.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/protocol.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)       70 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/racketEvent.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      498 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/secureChatProtocol.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1691 2022-02-04 19:51:34.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/service.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      120 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/simpleChatProtocol.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      782 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/stream.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1592 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/sturdy.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      213 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/tcp.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      221 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/timer.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     3029 2022-02-04 19:51:34.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/trace.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      124 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/transportAddress.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)       92 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/protocols/schemas/worker.prs
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)    17246 2022-01-16 23:20:03.000000 syndicate-py-0.8.5/syndicate/relay.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      271 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/schema.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      648 2022-01-12 13:12:35.000000 syndicate-py-0.8.5/syndicate/transport.py
-drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2022-07-22 15:06:15.878956 syndicate-py-0.8.5/syndicate_py.egg-info/
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      649 2022-07-22 15:06:15.000000 syndicate-py-0.8.5/syndicate_py.egg-info/PKG-INFO
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1247 2022-07-22 15:06:15.000000 syndicate-py-0.8.5/syndicate_py.egg-info/SOURCES.txt
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)        1 2022-07-22 15:06:15.000000 syndicate-py-0.8.5/syndicate_py.egg-info/dependency_links.txt
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)       21 2022-07-22 15:06:15.000000 syndicate-py-0.8.5/syndicate_py.egg-info/requires.txt
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)       10 2022-07-22 15:06:15.000000 syndicate-py-0.8.5/syndicate_py.egg-info/top_level.txt
+drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2023-02-06 22:31:52.453699 syndicate-py-0.9.0/
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      137 2022-01-11 17:22:01.000000 syndicate-py-0.9.0/.envrc
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)       75 2022-01-05 16:29:43.000000 syndicate-py-0.9.0/.gitignore
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      552 2023-02-06 08:40:56.000000 syndicate-py-0.9.0/Makefile
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      649 2023-02-06 22:31:52.453699 syndicate-py-0.9.0/PKG-INFO
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      798 2023-02-06 16:35:14.000000 syndicate-py-0.9.0/README.md
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     3865 2023-02-06 16:35:14.000000 syndicate-py-0.9.0/bidi-gc.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      248 2023-02-06 22:31:06.000000 syndicate-py-0.9.0/chat.bin
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)       91 2023-02-06 08:40:56.000000 syndicate-py-0.9.0/chat.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2037 2023-02-06 16:35:14.000000 syndicate-py-0.9.0/chat.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      264 2022-01-07 15:04:18.000000 syndicate-py-0.9.0/inf.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)       21 2021-08-23 15:04:30.000000 syndicate-py-0.9.0/requirements.txt
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)       38 2023-02-06 22:31:52.453699 syndicate-py-0.9.0/setup.cfg
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      946 2023-02-06 22:31:22.000000 syndicate-py-0.9.0/setup.py
+drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2023-02-06 22:31:52.453699 syndicate-py-0.9.0/syndicate/
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1323 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/__init__.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)    17938 2022-07-22 15:02:05.000000 syndicate-py-0.9.0/syndicate/actor.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2313 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/dataflow.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      568 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/dataspace.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2105 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/during.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      591 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/gatekeeper.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      231 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/idgen.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      222 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/mapset.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      538 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/metapy.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2927 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/patterns.py
+drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2023-02-06 22:31:52.453699 syndicate-py-0.9.0/syndicate/protocols/
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      140 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/protocols/Makefile
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)    16075 2023-02-06 16:35:12.000000 syndicate-py-0.9.0/syndicate/protocols/schema-bundle.bin
+drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2023-02-06 22:31:52.453699 syndicate-py-0.9.0/syndicate/protocols/schemas/
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      114 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/dataspace.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      543 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/dataspacePatterns.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      158 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/gatekeeper.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1554 2023-02-06 08:40:56.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/http.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     3306 2023-02-06 08:40:56.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/noise.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      471 2022-01-16 23:22:44.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/protocol.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1691 2022-02-04 19:51:34.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/service.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      782 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/stream.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1691 2023-02-06 16:35:12.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/sturdy.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      213 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/tcp.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      227 2023-02-06 16:35:12.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/timer.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     3029 2022-02-04 19:51:34.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/trace.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      124 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/transportAddress.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)       92 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/protocols/schemas/worker.prs
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)    17246 2022-01-16 23:20:03.000000 syndicate-py-0.9.0/syndicate/relay.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      271 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/schema.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      648 2022-01-12 13:12:35.000000 syndicate-py-0.9.0/syndicate/transport.py
+drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2023-02-06 22:31:52.453699 syndicate-py-0.9.0/syndicate_py.egg-info/
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      649 2023-02-06 22:31:52.000000 syndicate-py-0.9.0/syndicate_py.egg-info/PKG-INFO
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1194 2023-02-06 22:31:52.000000 syndicate-py-0.9.0/syndicate_py.egg-info/SOURCES.txt
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)        1 2023-02-06 22:31:52.000000 syndicate-py-0.9.0/syndicate_py.egg-info/dependency_links.txt
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)       21 2023-02-06 22:31:52.000000 syndicate-py-0.9.0/syndicate_py.egg-info/requires.txt
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)       10 2023-02-06 22:31:52.000000 syndicate-py-0.9.0/syndicate_py.egg-info/top_level.txt
```

### Comparing `syndicate-py-0.8.5/PKG-INFO` & `syndicate-py-0.9.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syndicate-py
-Version: 0.8.5
+Version: 0.9.0
 Summary: Syndicated Actor model and Syndicate network protocol for Python 3
 Home-page: https://git.syndicate-lang.org/syndicate-lang/syndicate-py
 Author: Tony Garnock-Jones
 Author-email: tonyg@leastfixedpoint.com
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `syndicate-py-0.8.5/README.md` & `syndicate-py-0.9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 ## Running
 
 Start a Syndicate broker (such as
 [this one](https://git.syndicate-lang.org/syndicate-rs)) in one window.
 
 Find the line of broker output giving the root capability:
 
-    ... rootcap=<ref "syndicate" [] #x"a6480df5306611ddd0d3882b546e1977"> ...
+    ... rootcap=<ref "syndicate" [] #x"69ca300c1dbfa08fba692102dd82311a"> ...
 
 Then, run [chat.py](chat.py) several times in several separate windows:
 
     python chat.py \
         --address '<tcp "localhost" 8001>' \
-        --cap '<ref "syndicate" [] #x"a6480df5306611ddd0d3882b546e1977">'
+        --cap '<ref "syndicate" [] #x"69ca300c1dbfa08fba692102dd82311a">'
```

### Comparing `syndicate-py-0.8.5/bidi-gc.py` & `syndicate-py-0.9.0/bidi-gc.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 parser = argparse.ArgumentParser(description='Test bidirectional object reference GC.',
                                  formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 parser.add_argument('--address', metavar='\'<tcp "HOST" PORT>\'',
                     help='transport address of the server',
                     default='<ws "ws://localhost:9001/">')
 parser.add_argument('--cap', metavar='\'<ref ...>\'',
                     help='capability for the dataspace on the server',
-                    default='<ref "syndicate" [] #[pkgN9TBmEd3Q04grVG4Zdw==]>')
+                    default='<ref "syndicate" [] #[acowDB2/oI+6aSEC3YIxGg==]>')
 parser.add_argument('--start',
                     help='make this instance kick off the procedure',
                     action='store_true')
 args = parser.parse_args()
 
 #   A             B             DS
 # -----         -----         ------
```

### Comparing `syndicate-py-0.8.5/chat.py` & `syndicate-py-0.9.0/chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import sys
 import argparse
 import asyncio
 import random
 import syndicate
 from syndicate import patterns as P, actor, dataspace, turn
-from syndicate.schema import simpleChatProtocol, sturdy
+
+from syndicate.schema import sturdy
+
+from preserves.schema import load_schema_file
+simpleChatProtocol = load_schema_file('./chat.bin').chat
 
 parser = argparse.ArgumentParser(description='Simple dataspace-server-mediated text chat.',
                                  formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 parser.add_argument('--address', metavar='\'<tcp "HOST" PORT>\'',
                     help='transport address of the server',
                     default='<ws "ws://localhost:9001/">')
 parser.add_argument('--cap', metavar='\'<ref ...>\'',
                     help='capability for the dataspace on the server',
-                    default='<ref "syndicate" [] #[pkgN9TBmEd3Q04grVG4Zdw==]>')
+                    default='<ref "syndicate" [] #[acowDB2/oI+6aSEC3YIxGg==]>')
 args = parser.parse_args()
 
 Present = simpleChatProtocol.Present
 Says = simpleChatProtocol.Says
 
 @actor.run_system(name = 'chat', debug = False)
 def main():
```

### Comparing `syndicate-py-0.8.5/setup.py` & `syndicate-py-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 setup(
     name="syndicate-py",
-    version="0.8.5",
+    version="0.9.0",
     author="Tony Garnock-Jones",
     author_email="tonyg@leastfixedpoint.com",
     license="GNU General Public License v3 or later (GPLv3+)",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `syndicate-py-0.8.5/syndicate/__init__.py` & `syndicate-py-0.9.0/syndicate/__init__.py`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate/actor.py` & `syndicate-py-0.9.0/syndicate/actor.py`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate/dataflow.py` & `syndicate-py-0.9.0/syndicate/dataflow.py`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate/dataspace.py` & `syndicate-py-0.9.0/syndicate/dataspace.py`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate/during.py` & `syndicate-py-0.9.0/syndicate/during.py`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate/gatekeeper.py` & `syndicate-py-0.9.0/syndicate/gatekeeper.py`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate/metapy.py` & `syndicate-py-0.9.0/syndicate/metapy.py`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate/patterns.py` & `syndicate-py-0.9.0/syndicate/patterns.py`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate/protocols/schema-bundle.bin` & `syndicate-py-0.9.0/syndicate/protocols/schema-bundle.bin`

 * *Files 14% similar despite different names*

```diff
@@ -24,851 +24,982 @@
 00000170: 6564 b305 6c6f 6361 6cb4 b303 7265 66b5  ed..local...ref.
 00000180: 84b3 0854 6370 4c6f 6361 6c84 84b4 b305  ...TcpLocal.....
 00000190: 6e61 6d65 64b3 0672 656d 6f74 65b4 b303  named..remote...
 000001a0: 7265 66b5 84b3 0954 6370 5265 6d6f 7465  ref....TcpRemote
 000001b0: 8484 8484 8484 b30c 656d 6265 6464 6564  ........embedded
 000001c0: 5479 7065 b4b3 0372 6566 b5b3 0945 6e74  Type...ref...Ent
 000001d0: 6974 7952 6566 84b3 0343 6170 8484 84b5  ityRef...Cap....
-000001e0: b305 7469 6d65 7284 b4b3 0673 6368 656d  ..timer....schem
-000001f0: 61b7 b307 7665 7273 696f 6e91 b30b 6465  a...version...de
-00000200: 6669 6e69 7469 6f6e 73b7 b308 5365 7454  finitions...SetT
-00000210: 696d 6572 b4b3 0372 6563 b4b3 036c 6974  imer...rec...lit
-00000220: b309 7365 742d 7469 6d65 7284 b4b3 0574  ..set-timer....t
-00000230: 7570 6c65 b5b4 b305 6e61 6d65 64b3 056c  uple....named..l
-00000240: 6162 656c b303 616e 7984 b4b3 056e 616d  abel..any....nam
-00000250: 6564 b305 6d73 6563 73b4 b304 6174 6f6d  ed..msecs...atom
-00000260: b306 446f 7562 6c65 8484 b4b3 056e 616d  ..Double.....nam
-00000270: 6564 b304 6b69 6e64 b4b3 0372 6566 b584  ed..kind...ref..
-00000280: b309 5469 6d65 724b 696e 6484 8484 8484  ..TimerKind.....
-00000290: b309 4c61 7465 7254 6861 6eb4 b303 7265  ..LaterThan...re
-000002a0: 63b4 b303 6c69 74b3 0a6c 6174 6572 2d74  c...lit..later-t
-000002b0: 6861 6e84 b4b3 0574 7570 6c65 b5b4 b305  han....tuple....
-000002c0: 6e61 6d65 64b3 056d 7365 6373 b4b3 0461  named..msecs...a
-000002d0: 746f 6db3 0644 6f75 626c 6584 8484 8484  tom..Double.....
-000002e0: b309 5469 6d65 724b 696e 64b4 b302 6f72  ..TimerKind...or
-000002f0: b5b5 b108 7265 6c61 7469 7665 b4b3 036c  ....relative...l
-00000300: 6974 b308 7265 6c61 7469 7665 8484 b5b1  it..relative....
-00000310: 0861 6273 6f6c 7574 65b4 b303 6c69 74b3  .absolute...lit.
-00000320: 0861 6273 6f6c 7574 6584 84b5 b105 636c  .absolute.....cl
-00000330: 6561 72b4 b303 6c69 74b3 0563 6c65 6172  ear...lit..clear
-00000340: 8484 8484 b30c 5469 6d65 7245 7870 6972  ......TimerExpir
-00000350: 6564 b4b3 0372 6563 b4b3 036c 6974 b30d  ed...rec...lit..
-00000360: 7469 6d65 722d 6578 7069 7265 6484 b4b3  timer-expired...
-00000370: 0574 7570 6c65 b5b4 b305 6e61 6d65 64b3  .tuple....named.
-00000380: 056c 6162 656c b303 616e 7984 b4b3 056e  .label..any....n
-00000390: 616d 6564 b305 6d73 6563 73b4 b304 6174  amed..msecs...at
-000003a0: 6f6d b306 446f 7562 6c65 8484 8484 8484  om..Double......
-000003b0: b30c 656d 6265 6464 6564 5479 7065 8084  ..embeddedType..
-000003c0: 84b5 b305 7472 6163 6584 b4b3 0673 6368  ....trace....sch
-000003d0: 656d 61b7 b307 7665 7273 696f 6e91 b30b  ema...version...
-000003e0: 6465 6669 6e69 7469 6f6e 73b7 b303 4f69  definitions...Oi
-000003f0: 64b3 0361 6e79 b304 4e61 6d65 b4b3 026f  d..any..Name...o
-00000400: 72b5 b5b1 0961 6e6f 6e79 6d6f 7573 b4b3  r....anonymous..
-00000410: 0372 6563 b4b3 036c 6974 b309 616e 6f6e  .rec...lit..anon
-00000420: 796d 6f75 7384 b4b3 0574 7570 6c65 b584  ymous....tuple..
-00000430: 8484 84b5 b105 6e61 6d65 64b4 b303 7265  ......named...re
-00000440: 63b4 b303 6c69 74b3 056e 616d 6564 84b4  c...lit..named..
-00000450: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
-00000460: b304 6e61 6d65 b303 616e 7984 8484 8484  ..name..any.....
-00000470: 8484 b306 5461 7267 6574 b4b3 0372 6563  ....Target...rec
-00000480: b4b3 036c 6974 b306 656e 7469 7479 84b4  ...lit..entity..
-00000490: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
-000004a0: b305 6163 746f 72b4 b303 7265 66b5 84b3  ..actor...ref...
-000004b0: 0741 6374 6f72 4964 8484 b4b3 056e 616d  .ActorId.....nam
-000004c0: 6564 b305 6661 6365 74b4 b303 7265 66b5  ed..facet...ref.
-000004d0: 84b3 0746 6163 6574 4964 8484 b4b3 056e  ...FacetId.....n
-000004e0: 616d 6564 b303 6f69 64b4 b303 7265 66b5  amed..oid...ref.
-000004f0: 84b3 034f 6964 8484 8484 84b3 0654 6173  ...Oid.......Tas
-00000500: 6b49 64b3 0361 6e79 b306 5475 726e 4964  kId..any..TurnId
-00000510: b303 616e 79b3 0741 6374 6f72 4964 b303  ..any..ActorId..
-00000520: 616e 79b3 0746 6163 6574 4964 b303 616e  any..FacetId..an
-00000530: 79b3 0954 7572 6e43 6175 7365 b4b3 026f  y..TurnCause...o
-00000540: 72b5 b5b1 0474 7572 6eb4 b303 7265 63b4  r....turn...rec.
-00000550: b303 6c69 74b3 0963 6175 7365 642d 6279  ..lit..caused-by
-00000560: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
-00000570: 6564 b302 6964 b4b3 0372 6566 b584 b306  ed..id...ref....
-00000580: 5475 726e 4964 8484 8484 8484 b5b1 0763  TurnId.........c
-00000590: 6c65 616e 7570 b4b3 0372 6563 b4b3 036c  leanup...rec...l
-000005a0: 6974 b307 636c 6561 6e75 7084 b4b3 0574  it..cleanup....t
-000005b0: 7570 6c65 b584 8484 84b5 b111 6c69 6e6b  uple........link
-000005c0: 6564 5461 736b 5265 6c65 6173 65b4 b303  edTaskRelease...
-000005d0: 7265 63b4 b303 6c69 74b3 136c 696e 6b65  rec...lit..linke
-000005e0: 642d 7461 736b 2d72 656c 6561 7365 84b4  d-task-release..
-000005f0: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
-00000600: b302 6964 b4b3 0372 6566 b584 b306 5461  ..id...ref....Ta
-00000610: 736b 4964 8484 b4b3 056e 616d 6564 b306  skId.....named..
-00000620: 7265 6173 6f6e b4b3 0372 6566 b584 b317  reason...ref....
-00000630: 4c69 6e6b 6564 5461 736b 5265 6c65 6173  LinkedTaskReleas
-00000640: 6552 6561 736f 6e84 8484 8484 84b5 b112  eReason.........
-00000650: 7065 7269 6f64 6963 4163 7469 7661 7469  periodicActivati
-00000660: 6f6e b4b3 0372 6563 b4b3 036c 6974 b313  on...rec...lit..
-00000670: 7065 7269 6f64 6963 2d61 6374 6976 6174  periodic-activat
-00000680: 696f 6e84 b4b3 0574 7570 6c65 b5b4 b305  ion....tuple....
-00000690: 6e61 6d65 64b3 0670 6572 696f 64b4 b304  named..period...
-000006a0: 6174 6f6d b306 446f 7562 6c65 8484 8484  atom..Double....
-000006b0: 8484 b5b1 0564 656c 6179 b4b3 0372 6563  .....delay...rec
-000006c0: b4b3 036c 6974 b305 6465 6c61 7984 b4b3  ...lit..delay...
-000006d0: 0574 7570 6c65 b5b4 b305 6e61 6d65 64b3  .tuple....named.
-000006e0: 0b63 6175 7369 6e67 5475 726e b4b3 0372  .causingTurn...r
-000006f0: 6566 b584 b306 5475 726e 4964 8484 b4b3  ef....TurnId....
-00000700: 056e 616d 6564 b306 616d 6f75 6e74 b4b3  .named..amount..
-00000710: 0461 746f 6db3 0644 6f75 626c 6584 8484  .atom..Double...
-00000720: 8484 84b5 b108 6578 7465 726e 616c b4b3  ......external..
-00000730: 0372 6563 b4b3 036c 6974 b308 6578 7465  .rec...lit..exte
-00000740: 726e 616c 84b4 b305 7475 706c 65b5 b4b3  rnal....tuple...
-00000750: 056e 616d 6564 b30b 6465 7363 7269 7074  .named..descript
-00000760: 696f 6eb3 0361 6e79 8484 8484 8484 84b3  ion..any........
-00000770: 0954 7572 6e45 7665 6e74 b4b3 026f 72b5  .TurnEvent...or.
-00000780: b5b1 0661 7373 6572 74b4 b303 7265 63b4  ...assert...rec.
-00000790: b303 6c69 74b3 0661 7373 6572 7484 b4b3  ..lit..assert...
-000007a0: 0574 7570 6c65 b5b4 b305 6e61 6d65 64b3  .tuple....named.
-000007b0: 0961 7373 6572 7469 6f6e b4b3 0372 6566  .assertion...ref
-000007c0: b584 b314 4173 7365 7274 696f 6e44 6573  ....AssertionDes
-000007d0: 6372 6970 7469 6f6e 8484 b4b3 056e 616d  cription.....nam
-000007e0: 6564 b306 6861 6e64 6c65 b4b3 0372 6566  ed..handle...ref
-000007f0: b5b3 0870 726f 746f 636f 6c84 b306 4861  ...protocol...Ha
-00000800: 6e64 6c65 8484 8484 8484 b5b1 0772 6574  ndle.........ret
-00000810: 7261 6374 b4b3 0372 6563 b4b3 036c 6974  ract...rec...lit
-00000820: b307 7265 7472 6163 7484 b4b3 0574 7570  ..retract....tup
-00000830: 6c65 b5b4 b305 6e61 6d65 64b3 0668 616e  le....named..han
-00000840: 646c 65b4 b303 7265 66b5 b308 7072 6f74  dle...ref...prot
-00000850: 6f63 6f6c 84b3 0648 616e 646c 6584 8484  ocol...Handle...
-00000860: 8484 84b5 b107 6d65 7373 6167 65b4 b303  ......message...
-00000870: 7265 63b4 b303 6c69 74b3 076d 6573 7361  rec...lit..messa
-00000880: 6765 84b4 b305 7475 706c 65b5 b4b3 056e  ge....tuple....n
-00000890: 616d 6564 b304 626f 6479 b4b3 0372 6566  amed..body...ref
-000008a0: b584 b314 4173 7365 7274 696f 6e44 6573  ....AssertionDes
-000008b0: 6372 6970 7469 6f6e 8484 8484 8484 b5b1  cription........
-000008c0: 0473 796e 63b4 b303 7265 63b4 b303 6c69  .sync...rec...li
-000008d0: 74b3 0473 796e 6384 b4b3 0574 7570 6c65  t..sync....tuple
-000008e0: b5b4 b305 6e61 6d65 64b3 0470 6565 72b4  ....named..peer.
-000008f0: b303 7265 66b5 84b3 0654 6172 6765 7484  ..ref....Target.
-00000900: 8484 8484 84b5 b109 6272 6561 6b4c 696e  ........breakLin
-00000910: 6bb4 b303 7265 63b4 b303 6c69 74b3 0a62  k...rec...lit..b
-00000920: 7265 616b 2d6c 696e 6b84 b4b3 0574 7570  reak-link....tup
-00000930: 6c65 b5b4 b305 6e61 6d65 64b3 0673 6f75  le....named..sou
-00000940: 7263 65b4 b303 7265 66b5 84b3 0741 6374  rce...ref....Act
-00000950: 6f72 4964 8484 b4b3 056e 616d 6564 b306  orId.....named..
-00000960: 6861 6e64 6c65 b4b3 0372 6566 b5b3 0870  handle...ref...p
-00000970: 726f 746f 636f 6c84 b306 4861 6e64 6c65  rotocol...Handle
-00000980: 8484 8484 8484 8484 b30a 4578 6974 5374  ..........ExitSt
-00000990: 6174 7573 b4b3 026f 72b5 b5b1 026f 6bb4  atus...or....ok.
-000009a0: b303 6c69 74b3 026f 6b84 84b5 b105 4572  ..lit..ok.....Er
-000009b0: 726f 72b4 b303 7265 66b5 b308 7072 6f74  ror...ref...prot
-000009c0: 6f63 6f6c 84b3 0545 7272 6f72 8484 8484  ocol...Error....
-000009d0: b30a 5472 6163 6545 6e74 7279 b4b3 0372  ..TraceEntry...r
-000009e0: 6563 b4b3 036c 6974 b305 7472 6163 6584  ec...lit..trace.
-000009f0: b4b3 0574 7570 6c65 b5b4 b305 6e61 6d65  ...tuple....name
-00000a00: 64b3 0974 696d 6573 7461 6d70 b4b3 0461  d..timestamp...a
-00000a10: 746f 6db3 0644 6f75 626c 6584 84b4 b305  tom..Double.....
-00000a20: 6e61 6d65 64b3 0561 6374 6f72 b4b3 0372  named..actor...r
-00000a30: 6566 b584 b307 4163 746f 7249 6484 84b4  ef....ActorId...
-00000a40: b305 6e61 6d65 64b3 0469 7465 6db4 b303  ..named..item...
-00000a50: 7265 66b5 84b3 0f41 6374 6f72 4163 7469  ref....ActorActi
-00000a60: 7661 7469 6f6e 8484 8484 84b3 0f41 6374  vation.......Act
-00000a70: 6f72 4163 7469 7661 7469 6f6e b4b3 026f  orActivation...o
-00000a80: 72b5 b5b1 0573 7461 7274 b4b3 0372 6563  r....start...rec
-00000a90: b4b3 036c 6974 b305 7374 6172 7484 b4b3  ...lit..start...
-00000aa0: 0574 7570 6c65 b5b4 b305 6e61 6d65 64b3  .tuple....named.
-00000ab0: 0961 6374 6f72 4e61 6d65 b4b3 0372 6566  .actorName...ref
-00000ac0: b584 b304 4e61 6d65 8484 8484 8484 b5b1  ....Name........
-00000ad0: 0474 7572 6eb4 b303 7265 66b5 84b3 0f54  .turn...ref....T
-00000ae0: 7572 6e44 6573 6372 6970 7469 6f6e 8484  urnDescription..
-00000af0: b5b1 0473 746f 70b4 b303 7265 63b4 b303  ...stop...rec...
-00000b00: 6c69 74b3 0473 746f 7084 b4b3 0574 7570  lit..stop....tup
-00000b10: 6c65 b5b4 b305 6e61 6d65 64b3 0673 7461  le....named..sta
-00000b20: 7475 73b4 b303 7265 66b5 84b3 0a45 7869  tus...ref....Exi
-00000b30: 7453 7461 7475 7384 8484 8484 8484 84b3  tStatus.........
-00000b40: 0f46 6163 6574 5374 6f70 5265 6173 6f6e  .FacetStopReason
-00000b50: b4b3 026f 72b5 b5b1 0e65 7870 6c69 6369  ...or....explici
-00000b60: 7441 6374 696f 6eb4 b303 6c69 74b3 0f65  tAction...lit..e
-00000b70: 7870 6c69 6369 742d 6163 7469 6f6e 8484  xplicit-action..
-00000b80: b5b1 0569 6e65 7274 b4b3 036c 6974 b305  ...inert...lit..
-00000b90: 696e 6572 7484 84b5 b10e 7061 7265 6e74  inert.....parent
-00000ba0: 5374 6f70 7069 6e67 b4b3 036c 6974 b30f  Stopping...lit..
-00000bb0: 7061 7265 6e74 2d73 746f 7070 696e 6784  parent-stopping.
-00000bc0: 84b5 b10d 6163 746f 7253 746f 7070 696e  ....actorStoppin
-00000bd0: 67b4 b303 6c69 74b3 0e61 6374 6f72 2d73  g...lit..actor-s
-00000be0: 746f 7070 696e 6784 8484 84b3 0f54 7572  topping......Tur
-00000bf0: 6e44 6573 6372 6970 7469 6f6e b4b3 0372  nDescription...r
-00000c00: 6563 b4b3 036c 6974 b304 7475 726e 84b4  ec...lit..turn..
-00000c10: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
-00000c20: b302 6964 b4b3 0372 6566 b584 b306 5475  ..id...ref....Tu
-00000c30: 726e 4964 8484 b4b3 056e 616d 6564 b305  rnId.....named..
-00000c40: 6361 7573 65b4 b303 7265 66b5 84b3 0954  cause...ref....T
-00000c50: 7572 6e43 6175 7365 8484 b4b3 056e 616d  urnCause.....nam
-00000c60: 6564 b307 6163 7469 6f6e 73b4 b305 7365  ed..actions...se
-00000c70: 716f 66b4 b303 7265 66b5 84b3 1141 6374  qof...ref....Act
-00000c80: 696f 6e44 6573 6372 6970 7469 6f6e 8484  ionDescription..
-00000c90: 8484 8484 b311 4163 7469 6f6e 4465 7363  ......ActionDesc
-00000ca0: 7269 7074 696f 6eb4 b302 6f72 b5b5 b107  ription...or....
-00000cb0: 6465 7175 6575 65b4 b303 7265 63b4 b303  dequeue...rec...
-00000cc0: 6c69 74b3 0764 6571 7565 7565 84b4 b305  lit..dequeue....
-00000cd0: 7475 706c 65b5 b4b3 056e 616d 6564 b305  tuple....named..
-00000ce0: 6576 656e 74b4 b303 7265 66b5 84b3 1154  event...ref....T
-00000cf0: 6172 6765 7465 6454 7572 6e45 7665 6e74  argetedTurnEvent
-00000d00: 8484 8484 8484 b5b1 0765 6e71 7565 7565  .........enqueue
-00000d10: b4b3 0372 6563 b4b3 036c 6974 b307 656e  ...rec...lit..en
-00000d20: 7175 6575 6584 b4b3 0574 7570 6c65 b5b4  queue....tuple..
-00000d30: b305 6e61 6d65 64b3 0565 7665 6e74 b4b3  ..named..event..
-00000d40: 0372 6566 b584 b311 5461 7267 6574 6564  .ref....Targeted
-00000d50: 5475 726e 4576 656e 7484 8484 8484 84b5  TurnEvent.......
-00000d60: b10f 6465 7175 6575 6549 6e74 6572 6e61  ..dequeueInterna
-00000d70: 6cb4 b303 7265 63b4 b303 6c69 74b3 1064  l...rec...lit..d
-00000d80: 6571 7565 7565 2d69 6e74 6572 6e61 6c84  equeue-internal.
-00000d90: b4b3 0574 7570 6c65 b5b4 b305 6e61 6d65  ...tuple....name
-00000da0: 64b3 0565 7665 6e74 b4b3 0372 6566 b584  d..event...ref..
-00000db0: b311 5461 7267 6574 6564 5475 726e 4576  ..TargetedTurnEv
-00000dc0: 656e 7484 8484 8484 84b5 b10f 656e 7175  ent.........enqu
-00000dd0: 6575 6549 6e74 6572 6e61 6cb4 b303 7265  eueInternal...re
-00000de0: 63b4 b303 6c69 74b3 1065 6e71 7565 7565  c...lit..enqueue
-00000df0: 2d69 6e74 6572 6e61 6c84 b4b3 0574 7570  -internal....tup
-00000e00: 6c65 b5b4 b305 6e61 6d65 64b3 0565 7665  le....named..eve
-00000e10: 6e74 b4b3 0372 6566 b584 b311 5461 7267  nt...ref....Targ
-00000e20: 6574 6564 5475 726e 4576 656e 7484 8484  etedTurnEvent...
-00000e30: 8484 84b5 b105 7370 6177 6eb4 b303 7265  ......spawn...re
-00000e40: 63b4 b303 6c69 74b3 0573 7061 776e 84b4  c...lit..spawn..
-00000e50: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
-00000e60: b304 6c69 6e6b b4b3 0461 746f 6db3 0742  ..link...atom..B
-00000e70: 6f6f 6c65 616e 8484 b4b3 056e 616d 6564  oolean.....named
-00000e80: b302 6964 b4b3 0372 6566 b584 b307 4163  ..id...ref....Ac
-00000e90: 746f 7249 6484 8484 8484 84b5 b104 6c69  torId.........li
-00000ea0: 6e6b b4b3 0372 6563 b4b3 036c 6974 b304  nk...rec...lit..
-00000eb0: 6c69 6e6b 84b4 b305 7475 706c 65b5 b4b3  link....tuple...
-00000ec0: 056e 616d 6564 b30b 7061 7265 6e74 4163  .named..parentAc
-00000ed0: 746f 72b4 b303 7265 66b5 84b3 0741 6374  tor...ref....Act
-00000ee0: 6f72 4964 8484 b4b3 056e 616d 6564 b30d  orId.....named..
-00000ef0: 6368 696c 6454 6f50 6172 656e 74b4 b303  childToParent...
-00000f00: 7265 66b5 b308 7072 6f74 6f63 6f6c 84b3  ref...protocol..
-00000f10: 0648 616e 646c 6584 84b4 b305 6e61 6d65  .Handle.....name
-00000f20: 64b3 0a63 6869 6c64 4163 746f 72b4 b303  d..childActor...
-00000f30: 7265 66b5 84b3 0741 6374 6f72 4964 8484  ref....ActorId..
-00000f40: b4b3 056e 616d 6564 b30d 7061 7265 6e74  ...named..parent
-00000f50: 546f 4368 696c 64b4 b303 7265 66b5 b308  ToChild...ref...
-00000f60: 7072 6f74 6f63 6f6c 84b3 0648 616e 646c  protocol...Handl
-00000f70: 6584 8484 8484 84b5 b10a 6661 6365 7453  e.........facetS
-00000f80: 7461 7274 b4b3 0372 6563 b4b3 036c 6974  tart...rec...lit
-00000f90: b30b 6661 6365 742d 7374 6172 7484 b4b3  ..facet-start...
-00000fa0: 0574 7570 6c65 b5b4 b305 6e61 6d65 64b3  .tuple....named.
-00000fb0: 0470 6174 68b4 b305 7365 716f 66b4 b303  .path...seqof...
-00000fc0: 7265 66b5 84b3 0746 6163 6574 4964 8484  ref....FacetId..
-00000fd0: 8484 8484 84b5 b109 6661 6365 7453 746f  ........facetSto
-00000fe0: 70b4 b303 7265 63b4 b303 6c69 74b3 0a66  p...rec...lit..f
-00000ff0: 6163 6574 2d73 746f 7084 b4b3 0574 7570  acet-stop....tup
-00001000: 6c65 b5b4 b305 6e61 6d65 64b3 0470 6174  le....named..pat
-00001010: 68b4 b305 7365 716f 66b4 b303 7265 66b5  h...seqof...ref.
-00001020: 84b3 0746 6163 6574 4964 8484 84b4 b305  ...FacetId......
-00001030: 6e61 6d65 64b3 0672 6561 736f 6eb4 b303  named..reason...
-00001040: 7265 66b5 84b3 0f46 6163 6574 5374 6f70  ref....FacetStop
-00001050: 5265 6173 6f6e 8484 8484 8484 b5b1 0f6c  Reason.........l
-00001060: 696e 6b65 6454 6173 6b53 7461 7274 b4b3  inkedTaskStart..
-00001070: 0372 6563 b4b3 036c 6974 b311 6c69 6e6b  .rec...lit..link
-00001080: 6564 2d74 6173 6b2d 7374 6172 7484 b4b3  ed-task-start...
-00001090: 0574 7570 6c65 b5b4 b305 6e61 6d65 64b3  .tuple....named.
-000010a0: 0874 6173 6b4e 616d 65b4 b303 7265 66b5  .taskName...ref.
-000010b0: 84b3 044e 616d 6584 84b4 b305 6e61 6d65  ...Name.....name
-000010c0: 64b3 0269 64b4 b303 7265 66b5 84b3 0654  d..id...ref....T
-000010d0: 6173 6b49 6484 8484 8484 8484 84b3 1154  askId..........T
-000010e0: 6172 6765 7465 6454 7572 6e45 7665 6e74  argetedTurnEvent
-000010f0: b4b3 0372 6563 b4b3 036c 6974 b305 6576  ...rec...lit..ev
-00001100: 656e 7484 b4b3 0574 7570 6c65 b5b4 b305  ent....tuple....
-00001110: 6e61 6d65 64b3 0674 6172 6765 74b4 b303  named..target...
-00001120: 7265 66b5 84b3 0654 6172 6765 7484 84b4  ref....Target...
-00001130: b305 6e61 6d65 64b3 0664 6574 6169 6cb4  ..named..detail.
-00001140: b303 7265 66b5 84b3 0954 7572 6e45 7665  ..ref....TurnEve
-00001150: 6e74 8484 8484 84b3 1441 7373 6572 7469  nt.......Asserti
-00001160: 6f6e 4465 7363 7269 7074 696f 6eb4 b302  onDescription...
-00001170: 6f72 b5b5 b105 7661 6c75 65b4 b303 7265  or....value...re
-00001180: 63b4 b303 6c69 74b3 0576 616c 7565 84b4  c...lit..value..
-00001190: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
-000011a0: b305 7661 6c75 65b3 0361 6e79 8484 8484  ..value..any....
-000011b0: 84b5 b106 6f70 6171 7565 b4b3 0372 6563  ....opaque...rec
-000011c0: b4b3 036c 6974 b306 6f70 6171 7565 84b4  ...lit..opaque..
-000011d0: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
-000011e0: b30b 6465 7363 7269 7074 696f 6eb3 0361  ..description..a
-000011f0: 6e79 8484 8484 8484 84b3 174c 696e 6b65  ny.........Linke
-00001200: 6454 6173 6b52 656c 6561 7365 5265 6173  dTaskReleaseReas
-00001210: 6f6e b4b3 026f 72b5 b5b1 0963 616e 6365  on...or....cance
-00001220: 6c6c 6564 b4b3 036c 6974 b309 6361 6e63  lled...lit..canc
-00001230: 656c 6c65 6484 84b5 b106 6e6f 726d 616c  elled.....normal
-00001240: b4b3 036c 6974 b306 6e6f 726d 616c 8484  ...lit..normal..
-00001250: 8484 84b3 0c65 6d62 6564 6465 6454 7970  .....embeddedTyp
-00001260: 65b4 b303 7265 66b5 b309 456e 7469 7479  e...ref...Entity
-00001270: 5265 6684 b303 4361 7084 8484 b5b3 0673  Ref...Cap......s
-00001280: 7472 6561 6d84 b4b3 0673 6368 656d 61b7  tream....schema.
-00001290: b307 7665 7273 696f 6e91 b30b 6465 6669  ..version...defi
-000012a0: 6e69 7469 6f6e 73b7 b304 4d6f 6465 b4b3  nitions...Mode..
-000012b0: 026f 72b5 b5b1 0562 7974 6573 b4b3 036c  .or....bytes...l
-000012c0: 6974 b305 6279 7465 7384 84b5 b105 6c69  it..bytes.....li
-000012d0: 6e65 73b4 b303 7265 66b5 84b3 084c 696e  nes...ref....Lin
-000012e0: 654d 6f64 6584 84b5 b106 7061 636b 6574  eMode.....packet
-000012f0: b4b3 0372 6563 b4b3 036c 6974 b306 7061  ...rec...lit..pa
-00001300: 636b 6574 84b4 b305 7475 706c 65b5 b4b3  cket....tuple...
-00001310: 056e 616d 6564 b304 7369 7a65 b4b3 0461  .named..size...a
-00001320: 746f 6db3 0d53 6967 6e65 6449 6e74 6567  tom..SignedInteg
-00001330: 6572 8484 8484 8484 b5b1 066f 626a 6563  er.........objec
-00001340: 74b4 b303 7265 63b4 b303 6c69 74b3 066f  t...rec...lit..o
-00001350: 626a 6563 7484 b4b3 0574 7570 6c65 b5b4  bject....tuple..
-00001360: b305 6e61 6d65 64b3 0b64 6573 6372 6970  ..named..descrip
-00001370: 7469 6f6e b303 616e 7984 8484 8484 8484  tion..any.......
-00001380: b304 5369 6e6b b4b3 026f 72b5 b5b1 0673  ..Sink...or....s
-00001390: 6f75 7263 65b4 b303 7265 63b4 b303 6c69  ource...rec...li
-000013a0: 74b3 0673 6f75 7263 6584 b4b3 0574 7570  t..source....tup
-000013b0: 6c65 b5b4 b305 6e61 6d65 64b3 0a63 6f6e  le....named..con
-000013c0: 7472 6f6c 6c65 72b4 b308 656d 6265 6464  troller...embedd
-000013d0: 6564 b4b3 0372 6566 b584 b306 536f 7572  ed...ref....Sour
-000013e0: 6365 8484 8484 8484 84b5 b10b 5374 7265  ce..........Stre
-000013f0: 616d 4572 726f 72b4 b303 7265 66b5 84b3  amError...ref...
-00001400: 0b53 7472 6561 6d45 7272 6f72 8484 b5b1  .StreamError....
-00001410: 0464 6174 61b4 b303 7265 63b4 b303 6c69  .data...rec...li
-00001420: 74b3 0464 6174 6184 b4b3 0574 7570 6c65  t..data....tuple
-00001430: b5b4 b305 6e61 6d65 64b3 0770 6179 6c6f  ....named..paylo
-00001440: 6164 b303 616e 7984 b4b3 056e 616d 6564  ad..any....named
-00001450: b304 6d6f 6465 b4b3 0372 6566 b584 b304  ..mode...ref....
-00001460: 4d6f 6465 8484 8484 8484 b5b1 0365 6f66  Mode.........eof
-00001470: b4b3 0372 6563 b4b3 036c 6974 b303 656f  ...rec...lit..eo
-00001480: 6684 b4b3 0574 7570 6c65 b584 8484 8484  f....tuple......
-00001490: 84b3 0653 6f75 7263 65b4 b302 6f72 b5b5  ...Source...or..
-000014a0: b104 7369 6e6b b4b3 0372 6563 b4b3 036c  ..sink...rec...l
-000014b0: 6974 b304 7369 6e6b 84b4 b305 7475 706c  it..sink....tupl
-000014c0: 65b5 b4b3 056e 616d 6564 b30a 636f 6e74  e....named..cont
-000014d0: 726f 6c6c 6572 b4b3 0865 6d62 6564 6465  roller...embedde
-000014e0: 64b4 b303 7265 66b5 84b3 0453 696e 6b84  d...ref....Sink.
-000014f0: 8484 8484 8484 b5b1 0b53 7472 6561 6d45  .........StreamE
-00001500: 7272 6f72 b4b3 0372 6566 b584 b30b 5374  rror...ref....St
-00001510: 7265 616d 4572 726f 7284 84b5 b106 6372  reamError.....cr
-00001520: 6564 6974 b4b3 0372 6563 b4b3 036c 6974  edit...rec...lit
-00001530: b306 6372 6564 6974 84b4 b305 7475 706c  ..credit....tupl
-00001540: 65b5 b4b3 056e 616d 6564 b306 616d 6f75  e....named..amou
-00001550: 6e74 b4b3 0372 6566 b584 b30c 4372 6564  nt...ref....Cred
-00001560: 6974 416d 6f75 6e74 8484 b4b3 056e 616d  itAmount.....nam
-00001570: 6564 b304 6d6f 6465 b4b3 0372 6566 b584  ed..mode...ref..
-00001580: b304 4d6f 6465 8484 8484 8484 8484 b308  ..Mode..........
-00001590: 4c69 6e65 4d6f 6465 b4b3 026f 72b5 b5b1  LineMode...or...
-000015a0: 026c 66b4 b303 6c69 74b3 026c 6684 84b5  .lf...lit..lf...
-000015b0: b104 6372 6c66 b4b3 036c 6974 b304 6372  ..crlf...lit..cr
-000015c0: 6c66 8484 8484 b30b 5374 7265 616d 4572  lf......StreamEr
-000015d0: 726f 72b4 b303 7265 63b4 b303 6c69 74b3  ror...rec...lit.
-000015e0: 0565 7272 6f72 84b4 b305 7475 706c 65b5  .error....tuple.
-000015f0: b4b3 056e 616d 6564 b307 6d65 7373 6167  ...named..messag
-00001600: 65b4 b304 6174 6f6d b306 5374 7269 6e67  e...atom..String
-00001610: 8484 8484 84b3 0c43 7265 6469 7441 6d6f  .......CreditAmo
-00001620: 756e 74b4 b302 6f72 b5b5 b105 636f 756e  unt...or....coun
-00001630: 74b4 b304 6174 6f6d b30d 5369 676e 6564  t...atom..Signed
-00001640: 496e 7465 6765 7284 84b5 b109 756e 626f  Integer.....unbo
-00001650: 756e 6465 64b4 b303 6c69 74b3 0975 6e62  unded...lit..unb
-00001660: 6f75 6e64 6564 8484 8484 b310 5374 7265  ounded......Stre
-00001670: 616d 436f 6e6e 6563 7469 6f6e b4b3 0372  amConnection...r
-00001680: 6563 b4b3 036c 6974 b311 7374 7265 616d  ec...lit..stream
-00001690: 2d63 6f6e 6e65 6374 696f 6e84 b4b3 0574  -connection....t
-000016a0: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0673  uple....named..s
-000016b0: 6f75 7263 65b4 b308 656d 6265 6464 6564  ource...embedded
-000016c0: b4b3 0372 6566 b584 b306 536f 7572 6365  ...ref....Source
-000016d0: 8484 84b4 b305 6e61 6d65 64b3 0473 696e  ......named..sin
-000016e0: 6bb4 b308 656d 6265 6464 6564 b4b3 0372  k...embedded...r
-000016f0: 6566 b584 b304 5369 6e6b 8484 84b4 b305  ef....Sink......
-00001700: 6e61 6d65 64b3 0473 7065 63b3 0361 6e79  named..spec..any
-00001710: 8484 8484 b313 5374 7265 616d 4c69 7374  ......StreamList
-00001720: 656e 6572 4572 726f 72b4 b303 7265 63b4  enerError...rec.
-00001730: b303 6c69 74b3 1573 7472 6561 6d2d 6c69  ..lit..stream-li
-00001740: 7374 656e 6572 2d65 7272 6f72 84b4 b305  stener-error....
-00001750: 7475 706c 65b5 b4b3 056e 616d 6564 b304  tuple....named..
-00001760: 7370 6563 b303 616e 7984 b4b3 056e 616d  spec..any....nam
-00001770: 6564 b307 6d65 7373 6167 65b4 b304 6174  ed..message...at
-00001780: 6f6d b306 5374 7269 6e67 8484 8484 84b3  om..String......
-00001790: 1353 7472 6561 6d4c 6973 7465 6e65 7252  .StreamListenerR
-000017a0: 6561 6479 b4b3 0372 6563 b4b3 036c 6974  eady...rec...lit
-000017b0: b315 7374 7265 616d 2d6c 6973 7465 6e65  ..stream-listene
-000017c0: 722d 7265 6164 7984 b4b3 0574 7570 6c65  r-ready....tuple
-000017d0: b5b4 b305 6e61 6d65 64b3 0473 7065 63b3  ....named..spec.
-000017e0: 0361 6e79 8484 8484 84b3 0c65 6d62 6564  .any.......embed
-000017f0: 6465 6454 7970 65b4 b303 7265 66b5 b309  dedType...ref...
-00001800: 456e 7469 7479 5265 6684 b303 4361 7084  EntityRef...Cap.
-00001810: 8484 b5b3 0673 7475 7264 7984 b4b3 0673  .....sturdy....s
-00001820: 6368 656d 61b7 b307 7665 7273 696f 6e91  chema...version.
-00001830: b30b 6465 6669 6e69 7469 6f6e 73b7 b303  ..definitions...
-00001840: 4c69 74b4 b303 7265 63b4 b303 6c69 74b3  Lit...rec...lit.
-00001850: 036c 6974 84b4 b305 7475 706c 65b5 b4b3  .lit....tuple...
-00001860: 056e 616d 6564 b305 7661 6c75 65b3 0361  .named..value..a
-00001870: 6e79 8484 8484 b303 4f69 64b4 b304 6174  ny......Oid...at
-00001880: 6f6d b30d 5369 676e 6564 496e 7465 6765  om..SignedIntege
-00001890: 7284 b304 416c 7473 b4b3 0372 6563 b4b3  r...Alts...rec..
-000018a0: 036c 6974 b302 6f72 84b4 b305 7475 706c  .lit..or....tupl
-000018b0: 65b5 b4b3 056e 616d 6564 b30c 616c 7465  e....named..alte
-000018c0: 726e 6174 6976 6573 b4b3 0573 6571 6f66  rnatives...seqof
-000018d0: b4b3 0372 6566 b584 b307 5265 7772 6974  ...ref....Rewrit
-000018e0: 6584 8484 8484 84b3 0450 416e 64b4 b303  e........PAnd...
-000018f0: 7265 63b4 b303 6c69 74b3 0361 6e64 84b4  rec...lit..and..
-00001900: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
-00001910: b308 7061 7474 6572 6e73 b4b3 0573 6571  ..patterns...seq
-00001920: 6f66 b4b3 0372 6566 b584 b307 5061 7474  of...ref....Patt
-00001930: 6572 6e84 8484 8484 84b3 0450 4e6f 74b4  ern........PNot.
-00001940: b303 7265 63b4 b303 6c69 74b3 036e 6f74  ..rec...lit..not
-00001950: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
-00001960: 6564 b307 7061 7474 6572 6eb4 b303 7265  ed..pattern...re
-00001970: 66b5 84b3 0750 6174 7465 726e 8484 8484  f....Pattern....
-00001980: 84b3 0454 5265 66b4 b303 7265 63b4 b303  ...TRef...rec...
-00001990: 6c69 74b3 0372 6566 84b4 b305 7475 706c  lit..ref....tupl
-000019a0: 65b5 b4b3 056e 616d 6564 b307 6269 6e64  e....named..bind
-000019b0: 696e 67b4 b304 6174 6f6d b30d 5369 676e  ing...atom..Sign
-000019c0: 6564 496e 7465 6765 7284 8484 8484 b305  edInteger.......
-000019d0: 5041 746f 6db4 b302 6f72 b5b5 b107 426f  PAtom...or....Bo
-000019e0: 6f6c 6561 6eb4 b303 6c69 74b3 0742 6f6f  olean...lit..Boo
-000019f0: 6c65 616e 8484 b5b1 0546 6c6f 6174 b4b3  lean.....Float..
-00001a00: 036c 6974 b305 466c 6f61 7484 84b5 b106  .lit..Float.....
-00001a10: 446f 7562 6c65 b4b3 036c 6974 b306 446f  Double...lit..Do
-00001a20: 7562 6c65 8484 b5b1 0d53 6967 6e65 6449  uble.....SignedI
-00001a30: 6e74 6567 6572 b4b3 036c 6974 b30d 5369  nteger...lit..Si
-00001a40: 676e 6564 496e 7465 6765 7284 84b5 b106  gnedInteger.....
-00001a50: 5374 7269 6e67 b4b3 036c 6974 b306 5374  String...lit..St
-00001a60: 7269 6e67 8484 b5b1 0a42 7974 6553 7472  ring.....ByteStr
-00001a70: 696e 67b4 b303 6c69 74b3 0a42 7974 6553  ing...lit..ByteS
-00001a80: 7472 696e 6784 84b5 b106 5379 6d62 6f6c  tring.....Symbol
-00001a90: b4b3 036c 6974 b306 5379 6d62 6f6c 8484  ...lit..Symbol..
-00001aa0: 8484 b305 5042 696e 64b4 b303 7265 63b4  ....PBind...rec.
-00001ab0: b303 6c69 74b3 0462 696e 6484 b4b3 0574  ..lit..bind....t
-00001ac0: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0770  uple....named..p
-00001ad0: 6174 7465 726e b4b3 0372 6566 b584 b307  attern...ref....
-00001ae0: 5061 7474 6572 6e84 8484 8484 b306 4361  Pattern.......Ca
-00001af0: 7665 6174 b4b3 026f 72b5 b5b1 0752 6577  veat...or....Rew
-00001b00: 7269 7465 b4b3 0372 6566 b584 b307 5265  rite...ref....Re
-00001b10: 7772 6974 6584 84b5 b104 416c 7473 b4b3  write.....Alts..
-00001b20: 0372 6566 b584 b304 416c 7473 8484 8484  .ref....Alts....
-00001b30: b307 5061 7474 6572 6eb4 b302 6f72 b5b5  ..Pattern...or..
-00001b40: b108 5044 6973 6361 7264 b4b3 0372 6566  ..PDiscard...ref
-00001b50: b584 b308 5044 6973 6361 7264 8484 b5b1  ....PDiscard....
-00001b60: 0550 4174 6f6d b4b3 0372 6566 b584 b305  .PAtom...ref....
-00001b70: 5041 746f 6d84 84b5 b109 5045 6d62 6564  PAtom.....PEmbed
-00001b80: 6465 64b4 b303 7265 66b5 84b3 0950 456d  ded...ref....PEm
-00001b90: 6265 6464 6564 8484 b5b1 0550 4269 6e64  bedded.....PBind
-00001ba0: b4b3 0372 6566 b584 b305 5042 696e 6484  ...ref....PBind.
-00001bb0: 84b5 b104 5041 6e64 b4b3 0372 6566 b584  ....PAnd...ref..
-00001bc0: b304 5041 6e64 8484 b5b1 0450 4e6f 74b4  ..PAnd.....PNot.
-00001bd0: b303 7265 66b5 84b3 0450 4e6f 7484 84b5  ..ref....PNot...
-00001be0: b103 4c69 74b4 b303 7265 66b5 84b3 034c  ..Lit...ref....L
-00001bf0: 6974 8484 b5b1 0950 436f 6d70 6f75 6e64  it.....PCompound
-00001c00: b4b3 0372 6566 b584 b309 5043 6f6d 706f  ...ref....PCompo
-00001c10: 756e 6484 8484 84b3 0752 6577 7269 7465  und......Rewrite
-00001c20: b4b3 0372 6563 b4b3 036c 6974 b307 7265  ...rec...lit..re
-00001c30: 7772 6974 6584 b4b3 0574 7570 6c65 b5b4  write....tuple..
-00001c40: b305 6e61 6d65 64b3 0770 6174 7465 726e  ..named..pattern
-00001c50: b4b3 0372 6566 b584 b307 5061 7474 6572  ...ref....Patter
-00001c60: 6e84 84b4 b305 6e61 6d65 64b3 0874 656d  n.....named..tem
-00001c70: 706c 6174 65b4 b303 7265 66b5 84b3 0854  plate...ref....T
-00001c80: 656d 706c 6174 6584 8484 8484 b307 5769  emplate.......Wi
-00001c90: 7265 5265 66b4 b302 6f72 b5b5 b104 6d69  reRef...or....mi
-00001ca0: 6e65 b4b3 0574 7570 6c65 b5b4 b303 6c69  ne...tuple....li
-00001cb0: 7490 84b4 b305 6e61 6d65 64b3 036f 6964  t.....named..oid
-00001cc0: b4b3 0372 6566 b584 b303 4f69 6484 8484  ...ref....Oid...
-00001cd0: 8484 b5b1 0579 6f75 7273 b4b3 0b74 7570  .....yours...tup
-00001ce0: 6c65 5072 6566 6978 b5b4 b303 6c69 7491  lePrefix....lit.
-00001cf0: 84b4 b305 6e61 6d65 64b3 036f 6964 b4b3  ....named..oid..
-00001d00: 0372 6566 b584 b303 4f69 6484 8484 b4b3  .ref....Oid.....
-00001d10: 056e 616d 6564 b30b 6174 7465 6e75 6174  .named..attenuat
-00001d20: 696f 6eb4 b305 7365 716f 66b4 b303 7265  ion...seqof...re
-00001d30: 66b5 84b3 0643 6176 6561 7484 8484 8484  f....Caveat.....
-00001d40: 8484 b308 5044 6973 6361 7264 b4b3 0372  ....PDiscard...r
-00001d50: 6563 b4b3 036c 6974 b301 5f84 b4b3 0574  ec...lit.._....t
-00001d60: 7570 6c65 b584 8484 b308 5465 6d70 6c61  uple......Templa
-00001d70: 7465 b4b3 026f 72b5 b5b1 0a54 4174 7465  te...or....TAtte
-00001d80: 6e75 6174 65b4 b303 7265 66b5 84b3 0a54  nuate...ref....T
-00001d90: 4174 7465 6e75 6174 6584 84b5 b104 5452  Attenuate.....TR
-00001da0: 6566 b4b3 0372 6566 b584 b304 5452 6566  ef...ref....TRef
-00001db0: 8484 b5b1 034c 6974 b4b3 0372 6566 b584  .....Lit...ref..
-00001dc0: b303 4c69 7484 84b5 b109 5443 6f6d 706f  ..Lit.....TCompo
-00001dd0: 756e 64b4 b303 7265 66b5 84b3 0954 436f  und...ref....TCo
-00001de0: 6d70 6f75 6e64 8484 8484 b309 5043 6f6d  mpound......PCom
-00001df0: 706f 756e 64b4 b302 6f72 b5b5 b103 7265  pound...or....re
-00001e00: 63b4 b303 7265 63b4 b303 6c69 74b3 0372  c...rec...lit..r
-00001e10: 6563 84b4 b305 7475 706c 65b5 b4b3 056e  ec....tuple....n
-00001e20: 616d 6564 b305 6c61 6265 6cb3 0361 6e79  amed..label..any
-00001e30: 84b4 b305 6e61 6d65 64b3 0666 6965 6c64  ....named..field
-00001e40: 73b4 b305 7365 716f 66b4 b303 7265 66b5  s...seqof...ref.
-00001e50: 84b3 0750 6174 7465 726e 8484 8484 8484  ...Pattern......
-00001e60: 84b5 b103 6172 72b4 b303 7265 63b4 b303  ....arr...rec...
-00001e70: 6c69 74b3 0361 7272 84b4 b305 7475 706c  lit..arr....tupl
-00001e80: 65b5 b4b3 056e 616d 6564 b305 6974 656d  e....named..item
-00001e90: 73b4 b305 7365 716f 66b4 b303 7265 66b5  s...seqof...ref.
-00001ea0: 84b3 0750 6174 7465 726e 8484 8484 8484  ...Pattern......
-00001eb0: 84b5 b104 6469 6374 b4b3 0372 6563 b4b3  ....dict...rec..
-00001ec0: 036c 6974 b304 6469 6374 84b4 b305 7475  .lit..dict....tu
-00001ed0: 706c 65b5 b4b3 056e 616d 6564 b307 656e  ple....named..en
-00001ee0: 7472 6965 73b4 b306 6469 6374 6f66 b303  tries...dictof..
-00001ef0: 616e 79b4 b303 7265 66b5 84b3 0750 6174  any...ref....Pat
-00001f00: 7465 726e 8484 8484 8484 8484 84b3 0950  tern...........P
-00001f10: 456d 6265 6464 6564 b4b3 036c 6974 b308  Embedded...lit..
-00001f20: 456d 6265 6464 6564 84b3 0953 7475 7264  Embedded...Sturd
-00001f30: 7952 6566 b4b3 0372 6563 b4b3 036c 6974  yRef...rec...lit
-00001f40: b303 7265 6684 b4b3 0574 7570 6c65 b5b4  ..ref....tuple..
-00001f50: b305 6e61 6d65 64b3 036f 6964 b303 616e  ..named..oid..an
-00001f60: 7984 b4b3 056e 616d 6564 b30b 6361 7665  y....named..cave
-00001f70: 6174 4368 6169 6eb4 b305 7365 716f 66b4  atChain...seqof.
-00001f80: b303 7265 66b5 84b3 0b41 7474 656e 7561  ..ref....Attenua
-00001f90: 7469 6f6e 8484 84b4 b305 6e61 6d65 64b3  tion......named.
-00001fa0: 0373 6967 b4b3 0461 746f 6db3 0a42 7974  .sig...atom..Byt
-00001fb0: 6553 7472 696e 6784 8484 8484 b309 5443  eString.......TC
-00001fc0: 6f6d 706f 756e 64b4 b302 6f72 b5b5 b103  ompound...or....
-00001fd0: 7265 63b4 b303 7265 63b4 b303 6c69 74b3  rec...rec...lit.
-00001fe0: 0372 6563 84b4 b305 7475 706c 65b5 b4b3  .rec....tuple...
-00001ff0: 056e 616d 6564 b305 6c61 6265 6cb3 0361  .named..label..a
-00002000: 6e79 84b4 b305 6e61 6d65 64b3 0666 6965  ny....named..fie
-00002010: 6c64 73b4 b305 7365 716f 66b4 b303 7265  lds...seqof...re
-00002020: 66b5 84b3 0854 656d 706c 6174 6584 8484  f....Template...
-00002030: 8484 8484 b5b1 0361 7272 b4b3 0372 6563  .......arr...rec
-00002040: b4b3 036c 6974 b303 6172 7284 b4b3 0574  ...lit..arr....t
-00002050: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0569  uple....named..i
-00002060: 7465 6d73 b4b3 0573 6571 6f66 b4b3 0372  tems...seqof...r
-00002070: 6566 b584 b308 5465 6d70 6c61 7465 8484  ef....Template..
-00002080: 8484 8484 84b5 b104 6469 6374 b4b3 0372  ........dict...r
-00002090: 6563 b4b3 036c 6974 b304 6469 6374 84b4  ec...lit..dict..
-000020a0: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
-000020b0: b307 656e 7472 6965 73b4 b306 6469 6374  ..entries...dict
-000020c0: 6f66 b303 616e 79b4 b303 7265 66b5 84b3  of..any...ref...
-000020d0: 0854 656d 706c 6174 6584 8484 8484 8484  .Template.......
-000020e0: 8484 b30a 5441 7474 656e 7561 7465 b4b3  ....TAttenuate..
-000020f0: 0372 6563 b4b3 036c 6974 b309 6174 7465  .rec...lit..atte
-00002100: 6e75 6174 6584 b4b3 0574 7570 6c65 b5b4  nuate....tuple..
-00002110: b305 6e61 6d65 64b3 0874 656d 706c 6174  ..named..templat
-00002120: 65b4 b303 7265 66b5 84b3 0854 656d 706c  e...ref....Templ
-00002130: 6174 6584 84b4 b305 6e61 6d65 64b3 0b61  ate.....named..a
-00002140: 7474 656e 7561 7469 6f6e b4b3 0372 6566  ttenuation...ref
-00002150: b584 b30b 4174 7465 6e75 6174 696f 6e84  ....Attenuation.
-00002160: 8484 8484 b30b 4174 7465 6e75 6174 696f  ......Attenuatio
-00002170: 6eb4 b305 7365 716f 66b4 b303 7265 66b5  n...seqof...ref.
-00002180: 84b3 0643 6176 6561 7484 8484 b30c 656d  ...Caveat.....em
-00002190: 6265 6464 6564 5479 7065 b4b3 0372 6566  beddedType...ref
-000021a0: b5b3 0945 6e74 6974 7952 6566 84b3 0343  ...EntityRef...C
-000021b0: 6170 8484 84b5 b306 776f 726b 6572 84b4  ap......worker..
-000021c0: b306 7363 6865 6d61 b7b3 0776 6572 7369  ..schema...versi
-000021d0: 6f6e 91b3 0b64 6566 696e 6974 696f 6e73  on...definitions
-000021e0: b7b3 0849 6e73 7461 6e63 65b4 b303 7265  ...Instance...re
-000021f0: 63b4 b303 6c69 74b3 0849 6e73 7461 6e63  c...lit..Instanc
-00002200: 6584 b4b3 0574 7570 6c65 b5b4 b305 6e61  e....tuple....na
-00002210: 6d65 64b3 046e 616d 65b4 b304 6174 6f6d  med..name...atom
-00002220: b306 5374 7269 6e67 8484 b4b3 056e 616d  ..String.....nam
-00002230: 6564 b308 6172 6775 6d65 6e74 b303 616e  ed..argument..an
-00002240: 7984 8484 8484 b30c 656d 6265 6464 6564  y.......embedded
-00002250: 5479 7065 b4b3 0372 6566 b5b3 0945 6e74  Type...ref...Ent
-00002260: 6974 7952 6566 84b3 0343 6170 8484 84b5  ityRef...Cap....
-00002270: b307 7365 7276 6963 6584 b4b3 0673 6368  ..service....sch
-00002280: 656d 61b7 b307 7665 7273 696f 6e91 b30b  ema...version...
-00002290: 6465 6669 6e69 7469 6f6e 73b7 b305 5374  definitions...St
-000022a0: 6174 65b4 b302 6f72 b5b5 b107 7374 6172  ate...or....star
-000022b0: 7465 64b4 b303 6c69 74b3 0773 7461 7274  ted...lit..start
-000022c0: 6564 8484 b5b1 0572 6561 6479 b4b3 036c  ed.....ready...l
-000022d0: 6974 b305 7265 6164 7984 84b5 b106 6661  it..ready.....fa
-000022e0: 696c 6564 b4b3 036c 6974 b306 6661 696c  iled...lit..fail
-000022f0: 6564 8484 b5b1 0863 6f6d 706c 6574 65b4  ed.....complete.
-00002300: b303 6c69 74b3 0863 6f6d 706c 6574 6584  ..lit..complete.
-00002310: 84b5 b10b 7573 6572 4465 6669 6e65 64b3  ....userDefined.
-00002320: 0361 6e79 8484 84b3 0a52 756e 5365 7276  .any.....RunServ
-00002330: 6963 65b4 b303 7265 63b4 b303 6c69 74b3  ice...rec...lit.
-00002340: 0b72 756e 2d73 6572 7669 6365 84b4 b305  .run-service....
-00002350: 7475 706c 65b5 b4b3 056e 616d 6564 b30b  tuple....named..
-00002360: 7365 7276 6963 654e 616d 65b3 0361 6e79  serviceName..any
-00002370: 8484 8484 b30c 5365 7276 6963 6553 7461  ......ServiceSta
-00002380: 7465 b4b3 0372 6563 b4b3 036c 6974 b30d  te...rec...lit..
-00002390: 7365 7276 6963 652d 7374 6174 6584 b4b3  service-state...
-000023a0: 0574 7570 6c65 b5b4 b305 6e61 6d65 64b3  .tuple....named.
-000023b0: 0b73 6572 7669 6365 4e61 6d65 b303 616e  .serviceName..an
-000023c0: 7984 b4b3 056e 616d 6564 b305 7374 6174  y....named..stat
-000023d0: 65b4 b303 7265 66b5 84b3 0553 7461 7465  e...ref....State
-000023e0: 8484 8484 84b3 0d53 6572 7669 6365 4f62  .......ServiceOb
-000023f0: 6a65 6374 b4b3 0372 6563 b4b3 036c 6974  ject...rec...lit
-00002400: b30e 7365 7276 6963 652d 6f62 6a65 6374  ..service-object
-00002410: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
-00002420: 6564 b30b 7365 7276 6963 654e 616d 65b3  ed..serviceName.
-00002430: 0361 6e79 84b4 b305 6e61 6d65 64b3 066f  .any....named..o
-00002440: 626a 6563 74b3 0361 6e79 8484 8484 b30e  bject..any......
-00002450: 5265 7175 6972 6553 6572 7669 6365 b4b3  RequireService..
-00002460: 0372 6563 b4b3 036c 6974 b30f 7265 7175  .rec...lit..requ
-00002470: 6972 652d 7365 7276 6963 6584 b4b3 0574  ire-service....t
-00002480: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0b73  uple....named..s
-00002490: 6572 7669 6365 4e61 6d65 b303 616e 7984  erviceName..any.
-000024a0: 8484 84b3 0e52 6573 7461 7274 5365 7276  .....RestartServ
-000024b0: 6963 65b4 b303 7265 63b4 b303 6c69 74b3  ice...rec...lit.
-000024c0: 0f72 6573 7461 7274 2d73 6572 7669 6365  .restart-service
-000024d0: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
-000024e0: 6564 b30b 7365 7276 6963 654e 616d 65b3  ed..serviceName.
-000024f0: 0361 6e79 8484 8484 b311 5365 7276 6963  .any......Servic
-00002500: 6544 6570 656e 6465 6e63 79b4 b303 7265  eDependency...re
-00002510: 63b4 b303 6c69 74b3 0a64 6570 656e 6473  c...lit..depends
-00002520: 2d6f 6e84 b4b3 0574 7570 6c65 b5b4 b305  -on....tuple....
-00002530: 6e61 6d65 64b3 0864 6570 656e 6465 72b3  named..depender.
-00002540: 0361 6e79 84b4 b305 6e61 6d65 64b3 0864  .any....named..d
-00002550: 6570 656e 6465 65b4 b303 7265 66b5 84b3  ependee...ref...
-00002560: 0c53 6572 7669 6365 5374 6174 6584 8484  .ServiceState...
-00002570: 8484 84b3 0c65 6d62 6564 6465 6454 7970  .....embeddedTyp
-00002580: 65b4 b303 7265 66b5 b309 456e 7469 7479  e...ref...Entity
-00002590: 5265 6684 b303 4361 7084 8484 b5b3 0870  Ref...Cap......p
-000025a0: 726f 746f 636f 6c84 b4b3 0673 6368 656d  rotocol....schem
-000025b0: 61b7 b307 7665 7273 696f 6e91 b30b 6465  a...version...de
-000025c0: 6669 6e69 7469 6f6e 73b7 b303 4f69 64b4  finitions...Oid.
-000025d0: b304 6174 6f6d b30d 5369 676e 6564 496e  ..atom..SignedIn
-000025e0: 7465 6765 7284 b304 5379 6e63 b4b3 0372  teger...Sync...r
-000025f0: 6563 b4b3 036c 6974 b304 7379 6e63 84b4  ec...lit..sync..
-00002600: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
-00002610: b304 7065 6572 b4b3 0865 6d62 6564 6465  ..peer...embedde
-00002620: 64b4 b303 6c69 7481 8484 8484 8484 b304  d...lit.........
-00002630: 5475 726e b4b3 0573 6571 6f66 b4b3 0372  Turn...seqof...r
-00002640: 6566 b584 b309 5475 726e 4576 656e 7484  ef....TurnEvent.
-00002650: 84b3 0545 7272 6f72 b4b3 0372 6563 b4b3  ...Error...rec..
-00002660: 036c 6974 b305 6572 726f 7284 b4b3 0574  .lit..error....t
-00002670: 7570 6c65 b5b4 b305 6e61 6d65 64b3 076d  uple....named..m
-00002680: 6573 7361 6765 b4b3 0461 746f 6db3 0653  essage...atom..S
-00002690: 7472 696e 6784 84b4 b305 6e61 6d65 64b3  tring.....named.
-000026a0: 0664 6574 6169 6cb3 0361 6e79 8484 8484  .detail..any....
-000026b0: b305 4576 656e 74b4 b302 6f72 b5b5 b106  ..Event...or....
-000026c0: 4173 7365 7274 b4b3 0372 6566 b584 b306  Assert...ref....
-000026d0: 4173 7365 7274 8484 b5b1 0752 6574 7261  Assert.....Retra
-000026e0: 6374 b4b3 0372 6566 b584 b307 5265 7472  ct...ref....Retr
-000026f0: 6163 7484 84b5 b107 4d65 7373 6167 65b4  act.....Message.
-00002700: b303 7265 66b5 84b3 074d 6573 7361 6765  ..ref....Message
-00002710: 8484 b5b1 0453 796e 63b4 b303 7265 66b5  .....Sync...ref.
-00002720: 84b3 0453 796e 6384 8484 84b3 0641 7373  ...Sync......Ass
-00002730: 6572 74b4 b303 7265 63b4 b303 6c69 74b3  ert...rec...lit.
-00002740: 0661 7373 6572 7484 b4b3 0574 7570 6c65  .assert....tuple
-00002750: b5b4 b305 6e61 6d65 64b3 0961 7373 6572  ....named..asser
-00002760: 7469 6f6e b4b3 0372 6566 b584 b309 4173  tion...ref....As
-00002770: 7365 7274 696f 6e84 84b4 b305 6e61 6d65  sertion.....name
-00002780: 64b3 0668 616e 646c 65b4 b303 7265 66b5  d..handle...ref.
-00002790: 84b3 0648 616e 646c 6584 8484 8484 b306  ...Handle.......
-000027a0: 4861 6e64 6c65 b4b3 0461 746f 6db3 0d53  Handle...atom..S
-000027b0: 6967 6e65 6449 6e74 6567 6572 84b3 0650  ignedInteger...P
-000027c0: 6163 6b65 74b4 b302 6f72 b5b5 b104 5475  acket...or....Tu
-000027d0: 726e b4b3 0372 6566 b584 b304 5475 726e  rn...ref....Turn
-000027e0: 8484 b5b1 0545 7272 6f72 b4b3 0372 6566  .....Error...ref
-000027f0: b584 b305 4572 726f 7284 84b5 b109 4578  ....Error.....Ex
-00002800: 7465 6e73 696f 6eb4 b303 7265 66b5 84b3  tension...ref...
-00002810: 0945 7874 656e 7369 6f6e 8484 8484 b307  .Extension......
-00002820: 4d65 7373 6167 65b4 b303 7265 63b4 b303  Message...rec...
-00002830: 6c69 74b3 076d 6573 7361 6765 84b4 b305  lit..message....
-00002840: 7475 706c 65b5 b4b3 056e 616d 6564 b304  tuple....named..
-00002850: 626f 6479 b4b3 0372 6566 b584 b309 4173  body...ref....As
-00002860: 7365 7274 696f 6e84 8484 8484 b307 5265  sertion.......Re
-00002870: 7472 6163 74b4 b303 7265 63b4 b303 6c69  tract...rec...li
-00002880: 74b3 0772 6574 7261 6374 84b4 b305 7475  t..retract....tu
-00002890: 706c 65b5 b4b3 056e 616d 6564 b306 6861  ple....named..ha
-000028a0: 6e64 6c65 b4b3 0372 6566 b584 b306 4861  ndle...ref....Ha
-000028b0: 6e64 6c65 8484 8484 84b3 0941 7373 6572  ndle.......Asser
-000028c0: 7469 6f6e b303 616e 79b3 0945 7874 656e  tion..any..Exten
-000028d0: 7369 6f6e b4b3 0372 6563 b4b3 056e 616d  sion...rec...nam
-000028e0: 6564 b305 6c61 6265 6cb3 0361 6e79 84b4  ed..label..any..
-000028f0: b305 6e61 6d65 64b3 0666 6965 6c64 73b4  ..named..fields.
-00002900: b305 7365 716f 66b3 0361 6e79 8484 84b3  ..seqof..any....
-00002910: 0954 7572 6e45 7665 6e74 b4b3 0574 7570  .TurnEvent...tup
-00002920: 6c65 b5b4 b305 6e61 6d65 64b3 036f 6964  le....named..oid
-00002930: b4b3 0372 6566 b584 b303 4f69 6484 84b4  ...ref....Oid...
-00002940: b305 6e61 6d65 64b3 0565 7665 6e74 b4b3  ..named..event..
-00002950: 0372 6566 b584 b305 4576 656e 7484 8484  .ref....Event...
-00002960: 8484 b30c 656d 6265 6464 6564 5479 7065  ....embeddedType
-00002970: 8084 84b5 b309 6461 7461 7370 6163 6584  ......dataspace.
-00002980: b4b3 0673 6368 656d 61b7 b307 7665 7273  ...schema...vers
-00002990: 696f 6e91 b30b 6465 6669 6e69 7469 6f6e  ion...definition
-000029a0: 73b7 b307 4f62 7365 7276 65b4 b303 7265  s...Observe...re
-000029b0: 63b4 b303 6c69 74b3 074f 6273 6572 7665  c...lit..Observe
-000029c0: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
-000029d0: 6564 b307 7061 7474 6572 6eb4 b303 7265  ed..pattern...re
-000029e0: 66b5 b311 6461 7461 7370 6163 6550 6174  f...dataspacePat
-000029f0: 7465 726e 7384 b307 5061 7474 6572 6e84  terns...Pattern.
-00002a00: 84b4 b305 6e61 6d65 64b3 086f 6273 6572  ....named..obser
-00002a10: 7665 72b4 b308 656d 6265 6464 6564 b303  ver...embedded..
-00002a20: 616e 7984 8484 8484 84b3 0c65 6d62 6564  any........embed
-00002a30: 6465 6454 7970 65b4 b303 7265 66b5 b309  dedType...ref...
-00002a40: 456e 7469 7479 5265 6684 b303 4361 7084  EntityRef...Cap.
-00002a50: 8484 b5b3 0a67 6174 656b 6565 7065 7284  .....gatekeeper.
-00002a60: b4b3 0673 6368 656d 61b7 b307 7665 7273  ...schema...vers
-00002a70: 696f 6e91 b30b 6465 6669 6e69 7469 6f6e  ion...definition
-00002a80: 73b7 b304 4269 6e64 b4b3 0372 6563 b4b3  s...Bind...rec..
-00002a90: 036c 6974 b304 6269 6e64 84b4 b305 7475  .lit..bind....tu
-00002aa0: 706c 65b5 b4b3 056e 616d 6564 b303 6f69  ple....named..oi
-00002ab0: 64b3 0361 6e79 84b4 b305 6e61 6d65 64b3  d..any....named.
-00002ac0: 036b 6579 b4b3 0461 746f 6db3 0a42 7974  .key...atom..Byt
-00002ad0: 6553 7472 696e 6784 84b4 b305 6e61 6d65  eString.....name
-00002ae0: 64b3 0674 6172 6765 74b4 b308 656d 6265  d..target...embe
-00002af0: 6464 6564 b303 616e 7984 8484 8484 b307  dded..any.......
-00002b00: 5265 736f 6c76 65b4 b303 7265 63b4 b303  Resolve...rec...
-00002b10: 6c69 74b3 0772 6573 6f6c 7665 84b4 b305  lit..resolve....
-00002b20: 7475 706c 65b5 b4b3 056e 616d 6564 b309  tuple....named..
-00002b30: 7374 7572 6479 7265 66b4 b303 7265 66b5  sturdyref...ref.
-00002b40: b306 7374 7572 6479 84b3 0953 7475 7264  ..sturdy...Sturd
-00002b50: 7952 6566 8484 b4b3 056e 616d 6564 b308  yRef.....named..
-00002b60: 6f62 7365 7276 6572 b4b3 0865 6d62 6564  observer...embed
-00002b70: 6465 64b4 b308 656d 6265 6464 6564 b303  ded...embedded..
-00002b80: 616e 7984 8484 8484 8484 b30c 656d 6265  any.........embe
-00002b90: 6464 6564 5479 7065 b4b3 0372 6566 b5b3  ddedType...ref..
-00002ba0: 0945 6e74 6974 7952 6566 84b3 0343 6170  .EntityRef...Cap
-00002bb0: 8484 84b5 b30b 7261 636b 6574 4576 656e  ......racketEven
-00002bc0: 7484 b4b3 0673 6368 656d 61b7 b307 7665  t....schema...ve
-00002bd0: 7273 696f 6e91 b30b 6465 6669 6e69 7469  rsion...definiti
-00002be0: 6f6e 73b7 b30b 5261 636b 6574 4576 656e  ons...RacketEven
-00002bf0: 74b4 b303 7265 63b4 b303 6c69 74b3 0c72  t...rec...lit..r
-00002c00: 6163 6b65 742d 6576 656e 7484 b4b3 0574  acket-event....t
-00002c10: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0673  uple....named..s
-00002c20: 6f75 7263 65b4 b308 656d 6265 6464 6564  ource...embedded
-00002c30: b303 616e 7984 84b4 b305 6e61 6d65 64b3  ..any.....named.
-00002c40: 0565 7665 6e74 b4b3 0865 6d62 6564 6465  .event...embedde
-00002c50: 64b3 0361 6e79 8484 8484 8484 b30c 656d  d..any........em
-00002c60: 6265 6464 6564 5479 7065 8084 84b5 b310  beddedType......
-00002c70: 7472 616e 7370 6f72 7441 6464 7265 7373  transportAddress
-00002c80: 84b4 b306 7363 6865 6d61 b7b3 0776 6572  ....schema...ver
-00002c90: 7369 6f6e 91b3 0b64 6566 696e 6974 696f  sion...definitio
-00002ca0: 6e73 b7b3 0354 6370 b4b3 0372 6563 b4b3  ns...Tcp...rec..
-00002cb0: 036c 6974 b303 7463 7084 b4b3 0574 7570  .lit..tcp....tup
-00002cc0: 6c65 b5b4 b305 6e61 6d65 64b3 0468 6f73  le....named..hos
-00002cd0: 74b4 b304 6174 6f6d b306 5374 7269 6e67  t...atom..String
-00002ce0: 8484 b4b3 056e 616d 6564 b304 706f 7274  .....named..port
-00002cf0: b4b3 0461 746f 6db3 0d53 6967 6e65 6449  ...atom..SignedI
-00002d00: 6e74 6567 6572 8484 8484 84b3 0455 6e69  nteger.......Uni
-00002d10: 78b4 b303 7265 63b4 b303 6c69 74b3 0475  x...rec...lit..u
-00002d20: 6e69 7884 b4b3 0574 7570 6c65 b5b4 b305  nix....tuple....
-00002d30: 6e61 6d65 64b3 0470 6174 68b4 b304 6174  named..path...at
-00002d40: 6f6d b306 5374 7269 6e67 8484 8484 84b3  om..String......
-00002d50: 0553 7464 696f b4b3 0372 6563 b4b3 036c  .Stdio...rec...l
-00002d60: 6974 b305 7374 6469 6f84 b4b3 0574 7570  it..stdio....tup
-00002d70: 6c65 b584 8484 b309 5765 6253 6f63 6b65  le......WebSocke
-00002d80: 74b4 b303 7265 63b4 b303 6c69 74b3 0277  t...rec...lit..w
-00002d90: 7384 b4b3 0574 7570 6c65 b5b4 b305 6e61  s....tuple....na
-00002da0: 6d65 64b3 0375 726c b4b3 0461 746f 6db3  med..url...atom.
-00002db0: 0653 7472 696e 6784 8484 8484 84b3 0c65  .String........e
-00002dc0: 6d62 6564 6465 6454 7970 6580 8484 b5b3  mbeddedType.....
-00002dd0: 1164 6174 6173 7061 6365 5061 7474 6572  .dataspacePatter
-00002de0: 6e73 84b4 b306 7363 6865 6d61 b7b3 0776  ns....schema...v
-00002df0: 6572 7369 6f6e 91b3 0b64 6566 696e 6974  ersion...definit
-00002e00: 696f 6e73 b7b3 0444 4c69 74b4 b303 7265  ions...DLit...re
-00002e10: 63b4 b303 6c69 74b3 036c 6974 84b4 b305  c...lit..lit....
-00002e20: 7475 706c 65b5 b4b3 056e 616d 6564 b305  tuple....named..
-00002e30: 7661 6c75 65b4 b303 7265 66b5 84b3 0741  value...ref....A
-00002e40: 6e79 4174 6f6d 8484 8484 84b3 0544 4269  nyAtom.......DBi
-00002e50: 6e64 b4b3 0372 6563 b4b3 036c 6974 b304  nd...rec...lit..
-00002e60: 6269 6e64 84b4 b305 7475 706c 65b5 b4b3  bind....tuple...
-00002e70: 056e 616d 6564 b307 7061 7474 6572 6eb4  .named..pattern.
-00002e80: b303 7265 66b5 84b3 0750 6174 7465 726e  ..ref....Pattern
-00002e90: 8484 8484 84b3 0741 6e79 4174 6f6d b4b3  .......AnyAtom..
-00002ea0: 026f 72b5 b5b1 0462 6f6f 6cb4 b304 6174  .or....bool...at
-00002eb0: 6f6d b307 426f 6f6c 6561 6e84 84b5 b105  om..Boolean.....
-00002ec0: 666c 6f61 74b4 b304 6174 6f6d b305 466c  float...atom..Fl
-00002ed0: 6f61 7484 84b5 b106 646f 7562 6c65 b4b3  oat.....double..
-00002ee0: 0461 746f 6db3 0644 6f75 626c 6584 84b5  .atom..Double...
-00002ef0: b103 696e 74b4 b304 6174 6f6d b30d 5369  ..int...atom..Si
-00002f00: 676e 6564 496e 7465 6765 7284 84b5 b106  gnedInteger.....
-00002f10: 7374 7269 6e67 b4b3 0461 746f 6db3 0653  string...atom..S
-00002f20: 7472 696e 6784 84b5 b105 6279 7465 73b4  tring.....bytes.
-00002f30: b304 6174 6f6d b30a 4279 7465 5374 7269  ..atom..ByteStri
-00002f40: 6e67 8484 b5b1 0673 796d 626f 6cb4 b304  ng.....symbol...
-00002f50: 6174 6f6d b306 5379 6d62 6f6c 8484 b5b1  atom..Symbol....
-00002f60: 0865 6d62 6564 6465 64b4 b308 656d 6265  .embedded...embe
-00002f70: 6464 6564 b303 616e 7984 8484 84b3 0750  dded..any......P
-00002f80: 6174 7465 726e b4b3 026f 72b5 b5b1 0844  attern...or....D
-00002f90: 4469 7363 6172 64b4 b303 7265 66b5 84b3  Discard...ref...
-00002fa0: 0844 4469 7363 6172 6484 84b5 b105 4442  .DDiscard.....DB
-00002fb0: 696e 64b4 b303 7265 66b5 84b3 0544 4269  ind...ref....DBi
-00002fc0: 6e64 8484 b5b1 0444 4c69 74b4 b303 7265  nd.....DLit...re
-00002fd0: 66b5 84b3 0444 4c69 7484 84b5 b109 4443  f....DLit.....DC
-00002fe0: 6f6d 706f 756e 64b4 b303 7265 66b5 84b3  ompound...ref...
-00002ff0: 0944 436f 6d70 6f75 6e64 8484 8484 b308  .DCompound......
-00003000: 4444 6973 6361 7264 b4b3 0372 6563 b4b3  DDiscard...rec..
-00003010: 036c 6974 b301 5f84 b4b3 0574 7570 6c65  .lit.._....tuple
-00003020: b584 8484 b309 4443 6f6d 706f 756e 64b4  ......DCompound.
-00003030: b302 6f72 b5b5 b103 7265 63b4 b303 7265  ..or....rec...re
-00003040: 63b4 b303 6c69 74b3 0372 6563 84b4 b305  c...lit..rec....
-00003050: 7475 706c 65b5 b4b3 056e 616d 6564 b305  tuple....named..
-00003060: 6c61 6265 6cb3 0361 6e79 84b4 b305 6e61  label..any....na
-00003070: 6d65 64b3 0666 6965 6c64 73b4 b305 7365  med..fields...se
-00003080: 716f 66b4 b303 7265 66b5 84b3 0750 6174  qof...ref....Pat
-00003090: 7465 726e 8484 8484 8484 84b5 b103 6172  tern..........ar
-000030a0: 72b4 b303 7265 63b4 b303 6c69 74b3 0361  r...rec...lit..a
-000030b0: 7272 84b4 b305 7475 706c 65b5 b4b3 056e  rr....tuple....n
-000030c0: 616d 6564 b305 6974 656d 73b4 b305 7365  amed..items...se
-000030d0: 716f 66b4 b303 7265 66b5 84b3 0750 6174  qof...ref....Pat
-000030e0: 7465 726e 8484 8484 8484 84b5 b104 6469  tern..........di
-000030f0: 6374 b4b3 0372 6563 b4b3 036c 6974 b304  ct...rec...lit..
-00003100: 6469 6374 84b4 b305 7475 706c 65b5 b4b3  dict....tuple...
-00003110: 056e 616d 6564 b307 656e 7472 6965 73b4  .named..entries.
-00003120: b306 6469 6374 6f66 b303 616e 79b4 b303  ..dictof..any...
-00003130: 7265 66b5 84b3 0750 6174 7465 726e 8484  ref....Pattern..
-00003140: 8484 8484 8484 8484 b30c 656d 6265 6464  ..........embedd
-00003150: 6564 5479 7065 b4b3 0372 6566 b5b3 0945  edType...ref...E
-00003160: 6e74 6974 7952 6566 84b3 0343 6170 8484  ntityRef...Cap..
-00003170: 84b5 b312 7365 6375 7265 4368 6174 5072  ....secureChatPr
-00003180: 6f74 6f63 6f6c 84b4 b306 7363 6865 6d61  otocol....schema
-00003190: b7b3 0776 6572 7369 6f6e 91b3 0b64 6566  ...version...def
-000031a0: 696e 6974 696f 6e73 b7b3 044a 6f69 6eb4  initions...Join.
-000031b0: b303 7265 63b4 b303 6c69 74b3 0a6a 6f69  ..rec...lit..joi
-000031c0: 6e65 6455 7365 7284 b4b3 0574 7570 6c65  nedUser....tuple
-000031d0: b5b4 b305 6e61 6d65 64b3 0375 6964 b4b3  ....named..uid..
-000031e0: 0372 6566 b584 b306 5573 6572 4964 8484  .ref....UserId..
-000031f0: b4b3 056e 616d 6564 b306 6861 6e64 6c65  ...named..handle
-00003200: b4b3 0865 6d62 6564 6465 64b4 b303 7265  ...embedded...re
-00003210: 66b5 84b3 0753 6573 7369 6f6e 8484 8484  f....Session....
-00003220: 8484 b304 5361 7973 b4b3 0372 6563 b4b3  ....Says...rec..
-00003230: 036c 6974 b304 7361 7973 84b4 b305 7475  .lit..says....tu
-00003240: 706c 65b5 b4b3 056e 616d 6564 b303 7768  ple....named..wh
-00003250: 6fb4 b303 7265 66b5 84b3 0655 7365 7249  o...ref....UserI
-00003260: 6484 84b4 b305 6e61 6d65 64b3 0477 6861  d.....named..wha
-00003270: 74b4 b304 6174 6f6d b306 5374 7269 6e67  t...atom..String
-00003280: 8484 8484 84b3 0655 7365 7249 64b4 b304  .......UserId...
-00003290: 6174 6f6d b30d 5369 676e 6564 496e 7465  atom..SignedInte
-000032a0: 6765 7284 b307 5365 7373 696f 6eb4 b302  ger...Session...
-000032b0: 6f72 b5b5 b10c 6f62 7365 7276 6555 7365  or....observeUse
-000032c0: 7273 b4b3 0372 6563 b4b3 036c 6974 b307  rs...rec...lit..
-000032d0: 4f62 7365 7276 6584 b4b3 0574 7570 6c65  Observe....tuple
-000032e0: b5b4 b303 6c69 74b3 0475 7365 7284 b4b3  ....lit..user...
-000032f0: 056e 616d 6564 b308 6f62 7365 7276 6572  .named..observer
-00003300: b4b3 0865 6d62 6564 6465 64b4 b303 7265  ...embedded...re
-00003310: 66b5 84b3 0855 7365 7249 6e66 6f84 8484  f....UserInfo...
-00003320: 8484 8484 b5b1 0d6f 6273 6572 7665 5370  .......observeSp
-00003330: 6565 6368 b4b3 0372 6563 b4b3 036c 6974  eech...rec...lit
-00003340: b307 4f62 7365 7276 6584 b4b3 0574 7570  ..Observe....tup
-00003350: 6c65 b5b4 b303 6c69 74b3 0473 6179 7384  le....lit..says.
-00003360: b4b3 056e 616d 6564 b308 6f62 7365 7276  ...named..observ
-00003370: 6572 b4b3 0865 6d62 6564 6465 64b4 b303  er...embedded...
-00003380: 7265 66b5 84b3 0453 6179 7384 8484 8484  ref....Says.....
-00003390: 8484 b5b1 094e 6963 6b43 6c61 696d b4b3  .....NickClaim..
-000033a0: 0372 6566 b584 b309 4e69 636b 436c 6169  .ref....NickClai
-000033b0: 6d84 84b5 b104 5361 7973 b4b3 0372 6566  m.....Says...ref
-000033c0: b584 b304 5361 7973 8484 8484 b308 5573  ....Says......Us
-000033d0: 6572 496e 666f b4b3 0372 6563 b4b3 036c  erInfo...rec...l
-000033e0: 6974 b304 7573 6572 84b4 b305 7475 706c  it..user....tupl
-000033f0: 65b5 b4b3 056e 616d 6564 b303 7569 64b4  e....named..uid.
-00003400: b303 7265 66b5 84b3 0655 7365 7249 6484  ..ref....UserId.
-00003410: 84b4 b305 6e61 6d65 64b3 046e 616d 65b4  ....named..name.
-00003420: b304 6174 6f6d b306 5374 7269 6e67 8484  ..atom..String..
-00003430: 8484 84b3 094e 6963 6b43 6c61 696d b4b3  .....NickClaim..
-00003440: 0372 6563 b4b3 036c 6974 b309 636c 6169  .rec...lit..clai
-00003450: 6d4e 6963 6b84 b4b3 0574 7570 6c65 b5b4  mNick....tuple..
-00003460: b305 6e61 6d65 64b3 0375 6964 b4b3 0372  ..named..uid...r
-00003470: 6566 b584 b306 5573 6572 4964 8484 b4b3  ef....UserId....
-00003480: 056e 616d 6564 b304 6e61 6d65 b4b3 0461  .named..name...a
-00003490: 746f 6db3 0653 7472 696e 6784 84b4 b305  tom..String.....
-000034a0: 6e61 6d65 64b3 016b b4b3 0865 6d62 6564  named..k...embed
-000034b0: 6465 64b4 b303 7265 66b5 84b3 114e 6963  ded...ref....Nic
-000034c0: 6b43 6c61 696d 5265 7370 6f6e 7365 8484  kClaimResponse..
-000034d0: 8484 8484 b30c 4e69 636b 436f 6e66 6c69  ......NickConfli
-000034e0: 6374 b4b3 0372 6563 b4b3 036c 6974 b30c  ct...rec...lit..
-000034f0: 6e69 636b 436f 6e66 6c69 6374 84b4 b305  nickConflict....
-00003500: 7475 706c 65b5 8484 84b3 114e 6963 6b43  tuple......NickC
-00003510: 6c61 696d 5265 7370 6f6e 7365 b4b3 026f  laimResponse...o
-00003520: 72b5 b5b1 0474 7275 65b4 b303 6c69 7481  r....true...lit.
-00003530: 8484 b5b1 0c4e 6963 6b43 6f6e 666c 6963  .....NickConflic
-00003540: 74b4 b303 7265 66b5 84b3 0c4e 6963 6b43  t...ref....NickC
-00003550: 6f6e 666c 6963 7484 8484 8484 b30c 656d  onflict.......em
-00003560: 6265 6464 6564 5479 7065 b4b3 0372 6566  beddedType...ref
-00003570: b5b3 0945 6e74 6974 7952 6566 84b3 0343  ...EntityRef...C
-00003580: 6170 8484 84b5 b312 7369 6d70 6c65 4368  ap......simpleCh
-00003590: 6174 5072 6f74 6f63 6f6c 84b4 b306 7363  atProtocol....sc
-000035a0: 6865 6d61 b7b3 0776 6572 7369 6f6e 91b3  hema...version..
-000035b0: 0b64 6566 696e 6974 696f 6e73 b7b3 0453  .definitions...S
-000035c0: 6179 73b4 b303 7265 63b4 b303 6c69 74b3  ays...rec...lit.
-000035d0: 0453 6179 7384 b4b3 0574 7570 6c65 b5b4  .Says....tuple..
-000035e0: b305 6e61 6d65 64b3 0377 686f b4b3 0461  ..named..who...a
-000035f0: 746f 6db3 0653 7472 696e 6784 84b4 b305  tom..String.....
-00003600: 6e61 6d65 64b3 0477 6861 74b4 b304 6174  named..what...at
-00003610: 6f6d b306 5374 7269 6e67 8484 8484 84b3  om..String......
-00003620: 0750 7265 7365 6e74 b4b3 0372 6563 b4b3  .Present...rec..
-00003630: 036c 6974 b307 5072 6573 656e 7484 b4b3  .lit..Present...
-00003640: 0574 7570 6c65 b5b4 b305 6e61 6d65 64b3  .tuple....named.
-00003650: 0875 7365 726e 616d 65b4 b304 6174 6f6d  .username...atom
-00003660: b306 5374 7269 6e67 8484 8484 8484 b30c  ..String........
-00003670: 656d 6265 6464 6564 5479 7065 b4b3 0372  embeddedType...r
-00003680: 6566 b5b3 0945 6e74 6974 7952 6566 84b3  ef...EntityRef..
-00003690: 0343 6170 8484 8484 84                   .Cap.....
+000001e0: b304 6874 7470 84b4 b306 7363 6865 6d61  ..http....schema
+000001f0: b7b3 0776 6572 7369 6f6e 91b3 0b64 6566  ...version...def
+00000200: 696e 6974 696f 6e73 b7b3 0543 6875 6e6b  initions...Chunk
+00000210: b4b3 026f 72b5 b5b1 0673 7472 696e 67b4  ...or....string.
+00000220: b304 6174 6f6d b306 5374 7269 6e67 8484  ..atom..String..
+00000230: b5b1 0562 7974 6573 b4b3 0461 746f 6db3  ...bytes...atom.
+00000240: 0a42 7974 6553 7472 696e 6784 8484 84b3  .ByteString.....
+00000250: 0748 6561 6465 7273 b4b3 0664 6963 746f  .Headers...dicto
+00000260: 66b4 b304 6174 6f6d b306 5379 6d62 6f6c  f...atom..Symbol
+00000270: 84b4 b304 6174 6f6d b306 5374 7269 6e67  ....atom..String
+00000280: 8484 b308 4d69 6d65 5479 7065 b4b3 0461  ....MimeType...a
+00000290: 746f 6db3 0653 796d 626f 6c84 b30a 5175  tom..Symbol...Qu
+000002a0: 6572 7956 616c 7565 b4b3 026f 72b5 b5b1  eryValue...or...
+000002b0: 0673 7472 696e 67b4 b304 6174 6f6d b306  .string...atom..
+000002c0: 5374 7269 6e67 8484 b5b1 0466 696c 65b4  String.....file.
+000002d0: b303 7265 63b4 b303 6c69 74b3 0466 696c  ..rec...lit..fil
+000002e0: 6584 b4b3 0574 7570 6c65 b5b4 b305 6e61  e....tuple....na
+000002f0: 6d65 64b3 0866 696c 656e 616d 65b4 b304  med..filename...
+00000300: 6174 6f6d b306 5374 7269 6e67 8484 b4b3  atom..String....
+00000310: 056e 616d 6564 b307 6865 6164 6572 73b4  .named..headers.
+00000320: b303 7265 66b5 84b3 0748 6561 6465 7273  ..ref....Headers
+00000330: 8484 b4b3 056e 616d 6564 b304 626f 6479  .....named..body
+00000340: b4b3 0461 746f 6db3 0a42 7974 6553 7472  ...atom..ByteStr
+00000350: 696e 6784 8484 8484 8484 84b3 0b48 6f73  ing..........Hos
+00000360: 7450 6174 7465 726e b4b3 026f 72b5 b5b1  tPattern...or...
+00000370: 0468 6f73 74b4 b304 6174 6f6d b306 5374  .host...atom..St
+00000380: 7269 6e67 8484 b5b1 0361 6e79 b4b3 036c  ring.....any...l
+00000390: 6974 8084 8484 84b3 0b48 7474 7042 696e  it.......HttpBin
+000003a0: 6469 6e67 b4b3 0372 6563 b4b3 036c 6974  ding...rec...lit
+000003b0: b309 6874 7470 2d62 696e 6484 b4b3 0574  ..http-bind....t
+000003c0: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0468  uple....named..h
+000003d0: 6f73 74b4 b303 7265 66b5 84b3 0b48 6f73  ost...ref....Hos
+000003e0: 7450 6174 7465 726e 8484 b4b3 056e 616d  tPattern.....nam
+000003f0: 6564 b304 706f 7274 b4b3 0461 746f 6db3  ed..port...atom.
+00000400: 0d53 6967 6e65 6449 6e74 6567 6572 8484  .SignedInteger..
+00000410: b4b3 056e 616d 6564 b306 6d65 7468 6f64  ...named..method
+00000420: b4b3 0372 6566 b584 b30d 4d65 7468 6f64  ...ref....Method
+00000430: 5061 7474 6572 6e84 84b4 b305 6e61 6d65  Pattern.....name
+00000440: 64b3 0470 6174 68b4 b303 7265 66b5 84b3  d..path...ref...
+00000450: 0b50 6174 6850 6174 7465 726e 8484 b4b3  .PathPattern....
+00000460: 056e 616d 6564 b307 6861 6e64 6c65 72b4  .named..handler.
+00000470: b308 656d 6265 6464 6564 b4b3 0372 6566  ..embedded...ref
+00000480: b584 b30b 4874 7470 5265 7175 6573 7484  ....HttpRequest.
+00000490: 8484 8484 84b3 0b48 7474 7043 6f6e 7465  .......HttpConte
+000004a0: 7874 b4b3 0372 6563 b4b3 036c 6974 b307  xt...rec...lit..
+000004b0: 7265 7175 6573 7484 b4b3 0574 7570 6c65  request....tuple
+000004c0: b5b4 b305 6e61 6d65 64b3 0372 6571 b4b3  ....named..req..
+000004d0: 0372 6566 b584 b30b 4874 7470 5265 7175  .ref....HttpRequ
+000004e0: 6573 7484 84b4 b305 6e61 6d65 64b3 0372  est.....named..r
+000004f0: 6573 b4b3 0865 6d62 6564 6465 64b4 b303  es...embedded...
+00000500: 7265 66b5 84b3 0c48 7474 7052 6573 706f  ref....HttpRespo
+00000510: 6e73 6584 8484 8484 84b3 0b48 7474 7052  nse........HttpR
+00000520: 6571 7565 7374 b4b3 0372 6563 b4b3 036c  equest...rec...l
+00000530: 6974 b30c 6874 7470 2d72 6571 7565 7374  it..http-request
+00000540: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
+00000550: 6564 b30e 7365 7175 656e 6365 4e75 6d62  ed..sequenceNumb
+00000560: 6572 b4b3 0461 746f 6db3 0d53 6967 6e65  er...atom..Signe
+00000570: 6449 6e74 6567 6572 8484 b4b3 056e 616d  dInteger.....nam
+00000580: 6564 b304 686f 7374 b4b3 0461 746f 6db3  ed..host...atom.
+00000590: 0653 7472 696e 6784 84b4 b305 6e61 6d65  .String.....name
+000005a0: 64b3 0470 6f72 74b4 b304 6174 6f6d b30d  d..port...atom..
+000005b0: 5369 676e 6564 496e 7465 6765 7284 84b4  SignedInteger...
+000005c0: b305 6e61 6d65 64b3 066d 6574 686f 64b4  ..named..method.
+000005d0: b304 6174 6f6d b306 5379 6d62 6f6c 8484  ..atom..Symbol..
+000005e0: b4b3 056e 616d 6564 b304 7061 7468 b4b3  ...named..path..
+000005f0: 0573 6571 6f66 b4b3 0461 746f 6db3 0653  .seqof...atom..S
+00000600: 7472 696e 6784 8484 b4b3 056e 616d 6564  tring......named
+00000610: b307 6865 6164 6572 73b4 b303 7265 66b5  ..headers...ref.
+00000620: 84b3 0748 6561 6465 7273 8484 b4b3 056e  ...Headers.....n
+00000630: 616d 6564 b305 7175 6572 79b4 b306 6469  amed..query...di
+00000640: 6374 6f66 b4b3 0461 746f 6db3 0653 796d  ctof...atom..Sym
+00000650: 626f 6c84 b4b3 0573 6571 6f66 b4b3 0372  bol....seqof...r
+00000660: 6566 b584 b30a 5175 6572 7956 616c 7565  ef....QueryValue
+00000670: 8484 8484 b4b3 056e 616d 6564 b304 626f  .......named..bo
+00000680: 6479 b4b3 0372 6566 b584 b30b 5265 7175  dy...ref....Requ
+00000690: 6573 7442 6f64 7984 8484 8484 b30b 4874  estBody.......Ht
+000006a0: 7470 5365 7276 6963 65b4 b303 7265 63b4  tpService...rec.
+000006b0: b303 6c69 74b3 0c68 7474 702d 7365 7276  ..lit..http-serv
+000006c0: 6963 6584 b4b3 0574 7570 6c65 b5b4 b305  ice....tuple....
+000006d0: 6e61 6d65 64b3 0468 6f73 74b4 b303 7265  named..host...re
+000006e0: 66b5 84b3 0b48 6f73 7450 6174 7465 726e  f....HostPattern
+000006f0: 8484 b4b3 056e 616d 6564 b304 706f 7274  .....named..port
+00000700: b4b3 0461 746f 6db3 0d53 6967 6e65 6449  ...atom..SignedI
+00000710: 6e74 6567 6572 8484 b4b3 056e 616d 6564  nteger.....named
+00000720: b306 6d65 7468 6f64 b4b3 0372 6566 b584  ..method...ref..
+00000730: b30d 4d65 7468 6f64 5061 7474 6572 6e84  ..MethodPattern.
+00000740: 84b4 b305 6e61 6d65 64b3 0470 6174 68b4  ....named..path.
+00000750: b303 7265 66b5 84b3 0b50 6174 6850 6174  ..ref....PathPat
+00000760: 7465 726e 8484 8484 84b3 0b50 6174 6850  tern.......PathP
+00000770: 6174 7465 726e b4b3 0573 6571 6f66 b4b3  attern...seqof..
+00000780: 0372 6566 b584 b312 5061 7468 5061 7474  .ref....PathPatt
+00000790: 6572 6e45 6c65 6d65 6e74 8484 b30b 5265  ernElement....Re
+000007a0: 7175 6573 7442 6f64 79b4 b302 6f72 b5b5  questBody...or..
+000007b0: b107 7072 6573 656e 74b4 b304 6174 6f6d  ..present...atom
+000007c0: b30a 4279 7465 5374 7269 6e67 8484 b5b1  ..ByteString....
+000007d0: 0661 6273 656e 74b4 b303 6c69 7480 8484  .absent...lit...
+000007e0: 8484 b30c 4874 7470 4c69 7374 656e 6572  ....HttpListener
+000007f0: b4b3 0372 6563 b4b3 036c 6974 b30d 6874  ...rec...lit..ht
+00000800: 7470 2d6c 6973 7465 6e65 7284 b4b3 0574  tp-listener....t
+00000810: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0470  uple....named..p
+00000820: 6f72 74b4 b304 6174 6f6d b30d 5369 676e  ort...atom..Sign
+00000830: 6564 496e 7465 6765 7284 8484 8484 b30c  edInteger.......
+00000840: 4874 7470 5265 7370 6f6e 7365 b4b3 026f  HttpResponse...o
+00000850: 72b5 b5b1 0673 7461 7475 73b4 b303 7265  r....status...re
+00000860: 63b4 b303 6c69 74b3 0673 7461 7475 7384  c...lit..status.
+00000870: b4b3 0574 7570 6c65 b5b4 b305 6e61 6d65  ...tuple....name
+00000880: 64b3 0463 6f64 65b4 b304 6174 6f6d b30d  d..code...atom..
+00000890: 5369 676e 6564 496e 7465 6765 7284 84b4  SignedInteger...
+000008a0: b305 6e61 6d65 64b3 076d 6573 7361 6765  ..named..message
+000008b0: b4b3 0461 746f 6db3 0653 7472 696e 6784  ...atom..String.
+000008c0: 8484 8484 84b5 b106 6865 6164 6572 b4b3  ........header..
+000008d0: 0372 6563 b4b3 036c 6974 b306 6865 6164  .rec...lit..head
+000008e0: 6572 84b4 b305 7475 706c 65b5 b4b3 056e  er....tuple....n
+000008f0: 616d 6564 b304 6e61 6d65 b4b3 0461 746f  amed..name...ato
+00000900: 6db3 0653 796d 626f 6c84 84b4 b305 6e61  m..Symbol.....na
+00000910: 6d65 64b3 0576 616c 7565 b4b3 0461 746f  med..value...ato
+00000920: 6db3 0653 7472 696e 6784 8484 8484 84b5  m..String.......
+00000930: b105 6368 756e 6bb4 b303 7265 63b4 b303  ..chunk...rec...
+00000940: 6c69 74b3 0563 6875 6e6b 84b4 b305 7475  lit..chunk....tu
+00000950: 706c 65b5 b4b3 056e 616d 6564 b305 6368  ple....named..ch
+00000960: 756e 6bb4 b303 7265 66b5 84b3 0543 6875  unk...ref....Chu
+00000970: 6e6b 8484 8484 8484 b5b1 0464 6f6e 65b4  nk.........done.
+00000980: b303 7265 63b4 b303 6c69 74b3 0464 6f6e  ..rec...lit..don
+00000990: 6584 b4b3 0574 7570 6c65 b5b4 b305 6e61  e....tuple....na
+000009a0: 6d65 64b3 0563 6875 6e6b b4b3 0372 6566  med..chunk...ref
+000009b0: b584 b305 4368 756e 6b84 8484 8484 8484  ....Chunk.......
+000009c0: 84b3 0d4d 6574 686f 6450 6174 7465 726e  ...MethodPattern
+000009d0: b4b3 026f 72b5 b5b1 0361 6e79 b4b3 036c  ...or....any...l
+000009e0: 6974 8084 84b5 b108 7370 6563 6966 6963  it......specific
+000009f0: b4b3 0461 746f 6db3 0653 796d 626f 6c84  ...atom..Symbol.
+00000a00: 8484 84b3 1250 6174 6850 6174 7465 726e  .....PathPattern
+00000a10: 456c 656d 656e 74b4 b302 6f72 b5b5 b105  Element...or....
+00000a20: 6c61 6265 6cb4 b304 6174 6f6d b306 5374  label...atom..St
+00000a30: 7269 6e67 8484 b5b1 0877 696c 6463 6172  ring.....wildcar
+00000a40: 64b4 b303 6c69 74b3 015f 8484 b5b1 0472  d...lit.._.....r
+00000a50: 6573 74b4 b303 6c69 74b3 032e 2e2e 8484  est...lit.......
+00000a60: 8484 84b3 0c65 6d62 6564 6465 6454 7970  .....embeddedTyp
+00000a70: 6580 8484 b5b3 056e 6f69 7365 84b4 b306  e......noise....
+00000a80: 7363 6865 6d61 b7b3 0776 6572 7369 6f6e  schema...version
+00000a90: 91b3 0b64 6566 696e 6974 696f 6e73 b7b3  ...definitions..
+00000aa0: 0552 6f75 7465 b4b3 0372 6563 b4b3 036c  .Route...rec...l
+00000ab0: 6974 b305 726f 7574 6584 b4b3 0b74 7570  it..route....tup
+00000ac0: 6c65 5072 6566 6978 b5b4 b305 6e61 6d65  lePrefix....name
+00000ad0: 64b3 0a74 7261 6e73 706f 7274 73b4 b305  d..transports...
+00000ae0: 7365 716f 66b3 0361 6e79 8484 84b4 b305  seqof..any......
+00000af0: 6e61 6d65 64b3 0573 7465 7073 b4b3 0573  named..steps...s
+00000b00: 6571 6f66 b4b3 0372 6566 b584 b309 526f  eqof...ref....Ro
+00000b10: 7574 6553 7465 7084 8484 8484 b306 4163  uteStep.......Ac
+00000b20: 6365 7074 b4b3 0372 6563 b4b3 036c 6974  cept...rec...lit
+00000b30: b306 6163 6365 7074 84b4 b305 7475 706c  ..accept....tupl
+00000b40: 65b5 b4b3 056e 616d 6564 b310 7265 7370  e....named..resp
+00000b50: 6f6e 6465 7253 6573 7369 6f6e b4b3 0865  onderSession...e
+00000b60: 6d62 6564 6465 64b3 0361 6e79 8484 8484  mbedded..any....
+00000b70: 84b3 0650 6163 6b65 74b4 b302 6f72 b5b5  ...Packet...or..
+00000b80: b108 636f 6d70 6c65 7465 b4b3 0461 746f  ..complete...ato
+00000b90: 6db3 0a42 7974 6553 7472 696e 6784 84b5  m..ByteString...
+00000ba0: b10a 6672 6167 6d65 6e74 6564 b4b3 0573  ..fragmented...s
+00000bb0: 6571 6f66 b4b3 0461 746f 6db3 0a42 7974  eqof...atom..Byt
+00000bc0: 6553 7472 696e 6784 8484 8484 b307 436f  eString.......Co
+00000bd0: 6e6e 6563 74b4 b303 7265 63b4 b303 6c69  nnect...rec...li
+00000be0: 74b3 0763 6f6e 6e65 6374 84b4 b305 7475  t..connect....tu
+00000bf0: 706c 65b5 b4b3 056e 616d 6564 b30f 7365  ple....named..se
+00000c00: 7276 6963 6553 656c 6563 746f 72b3 0361  rviceSelector..a
+00000c10: 6e79 84b4 b305 6e61 6d65 64b3 1069 6e69  ny....named..ini
+00000c20: 7469 6174 6f72 5365 7373 696f 6eb4 b308  tiatorSession...
+00000c30: 656d 6265 6464 6564 b303 616e 7984 8484  embedded..any...
+00000c40: 8484 b309 4e6f 6973 6553 7065 63b4 b303  ....NoiseSpec...
+00000c50: 616e 64b5 b4b3 0464 6963 74b7 b303 6b65  and....dict...ke
+00000c60: 79b4 b305 6e61 6d65 64b3 036b 6579 b4b3  y...named..key..
+00000c70: 0461 746f 6db3 0a42 7974 6553 7472 696e  .atom..ByteStrin
+00000c80: 6784 84b3 0773 6572 7669 6365 b4b3 056e  g....service...n
+00000c90: 616d 6564 b307 7365 7276 6963 65b3 0361  amed..service..a
+00000ca0: 6e79 8484 84b4 b305 6e61 6d65 64b3 0870  ny......named..p
+00000cb0: 726f 746f 636f 6cb4 b303 7265 66b5 84b3  rotocol...ref...
+00000cc0: 0d4e 6f69 7365 5072 6f74 6f63 6f6c 8484  .NoiseProtocol..
+00000cd0: b4b3 056e 616d 6564 b30d 7072 6553 6861  ...named..preSha
+00000ce0: 7265 644b 6579 73b4 b303 7265 66b5 84b3  redKeys...ref...
+00000cf0: 124e 6f69 7365 5072 6553 6861 7265 644b  .NoisePreSharedK
+00000d00: 6579 7384 8484 84b3 094e 6f69 7365 5374  eys......NoiseSt
+00000d10: 6570 b4b3 0372 6563 b4b3 036c 6974 b305  ep...rec...lit..
+00000d20: 6e6f 6973 6584 b4b3 0574 7570 6c65 b5b4  noise....tuple..
+00000d30: b305 6e61 6d65 64b3 0473 7065 63b4 b303  ..named..spec...
+00000d40: 7265 66b5 84b3 094e 6f69 7365 5370 6563  ref....NoiseSpec
+00000d50: 8484 8484 84b3 0952 6f75 7465 5374 6570  .......RouteStep
+00000d60: b4b3 026f 72b5 b5b1 094e 6f69 7365 5374  ...or....NoiseSt
+00000d70: 6570 b4b3 0372 6566 b584 b309 4e6f 6973  ep...ref....Nois
+00000d80: 6553 7465 7084 84b5 b10e 4761 7465 6b65  eStep.....Gateke
+00000d90: 6570 6572 5374 6570 b4b3 0372 6566 b584  eperStep...ref..
+00000da0: b30e 4761 7465 6b65 6570 6572 5374 6570  ..GatekeeperStep
+00000db0: 8484 8484 b30d 4e6f 6973 6550 726f 746f  ......NoiseProto
+00000dc0: 636f 6cb4 b302 6f72 b5b5 b107 7072 6573  col...or....pres
+00000dd0: 656e 74b4 b304 6469 6374 b7b3 0870 726f  ent...dict...pro
+00000de0: 746f 636f 6cb4 b305 6e61 6d65 64b3 0870  tocol...named..p
+00000df0: 726f 746f 636f 6cb4 b304 6174 6f6d b306  rotocol...atom..
+00000e00: 5374 7269 6e67 8484 8484 84b5 b107 696e  String........in
+00000e10: 7661 6c69 64b4 b304 6469 6374 b7b3 0870  valid...dict...p
+00000e20: 726f 746f 636f 6cb4 b305 6e61 6d65 64b3  rotocol...named.
+00000e30: 0870 726f 746f 636f 6cb3 0361 6e79 8484  .protocol..any..
+00000e40: 8484 b5b1 0661 6273 656e 74b4 b304 6469  .....absent...di
+00000e50: 6374 b784 8484 8484 b30e 4761 7465 6b65  ct........Gateke
+00000e60: 6570 6572 5374 6570 b4b3 0372 6566 b5b3  eperStep...ref..
+00000e70: 0673 7475 7264 7984 b309 5374 7572 6479  .sturdy...Sturdy
+00000e80: 5265 6684 b30f 4465 6661 756c 7450 726f  Ref...DefaultPro
+00000e90: 746f 636f 6cb4 b303 6c69 74b1 214e 6f69  tocol...lit.!Noi
+00000ea0: 7365 5f4e 4b5f 3235 3531 395f 4368 6143  se_NK_25519_ChaC
+00000eb0: 6861 506f 6c79 5f42 4c41 4b45 3273 84b3  haPoly_BLAKE2s..
+00000ec0: 124e 6f69 7365 5072 6553 6861 7265 644b  .NoisePreSharedK
+00000ed0: 6579 73b4 b302 6f72 b5b5 b107 7072 6573  eys...or....pres
+00000ee0: 656e 74b4 b304 6469 6374 b7b3 0d70 7265  ent...dict...pre
+00000ef0: 5368 6172 6564 4b65 7973 b4b3 056e 616d  SharedKeys...nam
+00000f00: 6564 b30d 7072 6553 6861 7265 644b 6579  ed..preSharedKey
+00000f10: 73b4 b305 7365 716f 66b4 b304 6174 6f6d  s...seqof...atom
+00000f20: b30a 4279 7465 5374 7269 6e67 8484 8484  ..ByteString....
+00000f30: 8484 b5b1 0769 6e76 616c 6964 b4b3 0464  .....invalid...d
+00000f40: 6963 74b7 b30d 7072 6553 6861 7265 644b  ict...preSharedK
+00000f50: 6579 73b4 b305 6e61 6d65 64b3 0d70 7265  eys...named..pre
+00000f60: 5368 6172 6564 4b65 7973 b303 616e 7984  SharedKeys..any.
+00000f70: 8484 84b5 b106 6162 7365 6e74 b4b3 0464  ......absent...d
+00000f80: 6963 74b7 8484 8484 8484 b30c 656d 6265  ict.........embe
+00000f90: 6464 6564 5479 7065 8084 84b5 b305 7469  ddedType......ti
+00000fa0: 6d65 7284 b4b3 0673 6368 656d 61b7 b307  mer....schema...
+00000fb0: 7665 7273 696f 6e91 b30b 6465 6669 6e69  version...defini
+00000fc0: 7469 6f6e 73b7 b308 5365 7454 696d 6572  tions...SetTimer
+00000fd0: b4b3 0372 6563 b4b3 036c 6974 b309 7365  ...rec...lit..se
+00000fe0: 742d 7469 6d65 7284 b4b3 0574 7570 6c65  t-timer....tuple
+00000ff0: b5b4 b305 6e61 6d65 64b3 056c 6162 656c  ....named..label
+00001000: b303 616e 7984 b4b3 056e 616d 6564 b307  ..any....named..
+00001010: 7365 636f 6e64 73b4 b304 6174 6f6d b306  seconds...atom..
+00001020: 446f 7562 6c65 8484 b4b3 056e 616d 6564  Double.....named
+00001030: b304 6b69 6e64 b4b3 0372 6566 b584 b309  ..kind...ref....
+00001040: 5469 6d65 724b 696e 6484 8484 8484 b309  TimerKind.......
+00001050: 4c61 7465 7254 6861 6eb4 b303 7265 63b4  LaterThan...rec.
+00001060: b303 6c69 74b3 0a6c 6174 6572 2d74 6861  ..lit..later-tha
+00001070: 6e84 b4b3 0574 7570 6c65 b5b4 b305 6e61  n....tuple....na
+00001080: 6d65 64b3 0773 6563 6f6e 6473 b4b3 0461  med..seconds...a
+00001090: 746f 6db3 0644 6f75 626c 6584 8484 8484  tom..Double.....
+000010a0: b309 5469 6d65 724b 696e 64b4 b302 6f72  ..TimerKind...or
+000010b0: b5b5 b108 7265 6c61 7469 7665 b4b3 036c  ....relative...l
+000010c0: 6974 b308 7265 6c61 7469 7665 8484 b5b1  it..relative....
+000010d0: 0861 6273 6f6c 7574 65b4 b303 6c69 74b3  .absolute...lit.
+000010e0: 0861 6273 6f6c 7574 6584 84b5 b105 636c  .absolute.....cl
+000010f0: 6561 72b4 b303 6c69 74b3 0563 6c65 6172  ear...lit..clear
+00001100: 8484 8484 b30c 5469 6d65 7245 7870 6972  ......TimerExpir
+00001110: 6564 b4b3 0372 6563 b4b3 036c 6974 b30d  ed...rec...lit..
+00001120: 7469 6d65 722d 6578 7069 7265 6484 b4b3  timer-expired...
+00001130: 0574 7570 6c65 b5b4 b305 6e61 6d65 64b3  .tuple....named.
+00001140: 056c 6162 656c b303 616e 7984 b4b3 056e  .label..any....n
+00001150: 616d 6564 b307 7365 636f 6e64 73b4 b304  amed..seconds...
+00001160: 6174 6f6d b306 446f 7562 6c65 8484 8484  atom..Double....
+00001170: 8484 b30c 656d 6265 6464 6564 5479 7065  ....embeddedType
+00001180: 8084 84b5 b305 7472 6163 6584 b4b3 0673  ......trace....s
+00001190: 6368 656d 61b7 b307 7665 7273 696f 6e91  chema...version.
+000011a0: b30b 6465 6669 6e69 7469 6f6e 73b7 b303  ..definitions...
+000011b0: 4f69 64b3 0361 6e79 b304 4e61 6d65 b4b3  Oid..any..Name..
+000011c0: 026f 72b5 b5b1 0961 6e6f 6e79 6d6f 7573  .or....anonymous
+000011d0: b4b3 0372 6563 b4b3 036c 6974 b309 616e  ...rec...lit..an
+000011e0: 6f6e 796d 6f75 7384 b4b3 0574 7570 6c65  onymous....tuple
+000011f0: b584 8484 84b5 b105 6e61 6d65 64b4 b303  ........named...
+00001200: 7265 63b4 b303 6c69 74b3 056e 616d 6564  rec...lit..named
+00001210: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
+00001220: 6564 b304 6e61 6d65 b303 616e 7984 8484  ed..name..any...
+00001230: 8484 8484 b306 5461 7267 6574 b4b3 0372  ......Target...r
+00001240: 6563 b4b3 036c 6974 b306 656e 7469 7479  ec...lit..entity
+00001250: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
+00001260: 6564 b305 6163 746f 72b4 b303 7265 66b5  ed..actor...ref.
+00001270: 84b3 0741 6374 6f72 4964 8484 b4b3 056e  ...ActorId.....n
+00001280: 616d 6564 b305 6661 6365 74b4 b303 7265  amed..facet...re
+00001290: 66b5 84b3 0746 6163 6574 4964 8484 b4b3  f....FacetId....
+000012a0: 056e 616d 6564 b303 6f69 64b4 b303 7265  .named..oid...re
+000012b0: 66b5 84b3 034f 6964 8484 8484 84b3 0654  f....Oid.......T
+000012c0: 6173 6b49 64b3 0361 6e79 b306 5475 726e  askId..any..Turn
+000012d0: 4964 b303 616e 79b3 0741 6374 6f72 4964  Id..any..ActorId
+000012e0: b303 616e 79b3 0746 6163 6574 4964 b303  ..any..FacetId..
+000012f0: 616e 79b3 0954 7572 6e43 6175 7365 b4b3  any..TurnCause..
+00001300: 026f 72b5 b5b1 0474 7572 6eb4 b303 7265  .or....turn...re
+00001310: 63b4 b303 6c69 74b3 0963 6175 7365 642d  c...lit..caused-
+00001320: 6279 84b4 b305 7475 706c 65b5 b4b3 056e  by....tuple....n
+00001330: 616d 6564 b302 6964 b4b3 0372 6566 b584  amed..id...ref..
+00001340: b306 5475 726e 4964 8484 8484 8484 b5b1  ..TurnId........
+00001350: 0763 6c65 616e 7570 b4b3 0372 6563 b4b3  .cleanup...rec..
+00001360: 036c 6974 b307 636c 6561 6e75 7084 b4b3  .lit..cleanup...
+00001370: 0574 7570 6c65 b584 8484 84b5 b111 6c69  .tuple........li
+00001380: 6e6b 6564 5461 736b 5265 6c65 6173 65b4  nkedTaskRelease.
+00001390: b303 7265 63b4 b303 6c69 74b3 136c 696e  ..rec...lit..lin
+000013a0: 6b65 642d 7461 736b 2d72 656c 6561 7365  ked-task-release
+000013b0: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
+000013c0: 6564 b302 6964 b4b3 0372 6566 b584 b306  ed..id...ref....
+000013d0: 5461 736b 4964 8484 b4b3 056e 616d 6564  TaskId.....named
+000013e0: b306 7265 6173 6f6e b4b3 0372 6566 b584  ..reason...ref..
+000013f0: b317 4c69 6e6b 6564 5461 736b 5265 6c65  ..LinkedTaskRele
+00001400: 6173 6552 6561 736f 6e84 8484 8484 84b5  aseReason.......
+00001410: b112 7065 7269 6f64 6963 4163 7469 7661  ..periodicActiva
+00001420: 7469 6f6e b4b3 0372 6563 b4b3 036c 6974  tion...rec...lit
+00001430: b313 7065 7269 6f64 6963 2d61 6374 6976  ..periodic-activ
+00001440: 6174 696f 6e84 b4b3 0574 7570 6c65 b5b4  ation....tuple..
+00001450: b305 6e61 6d65 64b3 0670 6572 696f 64b4  ..named..period.
+00001460: b304 6174 6f6d b306 446f 7562 6c65 8484  ..atom..Double..
+00001470: 8484 8484 b5b1 0564 656c 6179 b4b3 0372  .......delay...r
+00001480: 6563 b4b3 036c 6974 b305 6465 6c61 7984  ec...lit..delay.
+00001490: b4b3 0574 7570 6c65 b5b4 b305 6e61 6d65  ...tuple....name
+000014a0: 64b3 0b63 6175 7369 6e67 5475 726e b4b3  d..causingTurn..
+000014b0: 0372 6566 b584 b306 5475 726e 4964 8484  .ref....TurnId..
+000014c0: b4b3 056e 616d 6564 b306 616d 6f75 6e74  ...named..amount
+000014d0: b4b3 0461 746f 6db3 0644 6f75 626c 6584  ...atom..Double.
+000014e0: 8484 8484 84b5 b108 6578 7465 726e 616c  ........external
+000014f0: b4b3 0372 6563 b4b3 036c 6974 b308 6578  ...rec...lit..ex
+00001500: 7465 726e 616c 84b4 b305 7475 706c 65b5  ternal....tuple.
+00001510: b4b3 056e 616d 6564 b30b 6465 7363 7269  ...named..descri
+00001520: 7074 696f 6eb3 0361 6e79 8484 8484 8484  ption..any......
+00001530: 84b3 0954 7572 6e45 7665 6e74 b4b3 026f  ...TurnEvent...o
+00001540: 72b5 b5b1 0661 7373 6572 74b4 b303 7265  r....assert...re
+00001550: 63b4 b303 6c69 74b3 0661 7373 6572 7484  c...lit..assert.
+00001560: b4b3 0574 7570 6c65 b5b4 b305 6e61 6d65  ...tuple....name
+00001570: 64b3 0961 7373 6572 7469 6f6e b4b3 0372  d..assertion...r
+00001580: 6566 b584 b314 4173 7365 7274 696f 6e44  ef....AssertionD
+00001590: 6573 6372 6970 7469 6f6e 8484 b4b3 056e  escription.....n
+000015a0: 616d 6564 b306 6861 6e64 6c65 b4b3 0372  amed..handle...r
+000015b0: 6566 b5b3 0870 726f 746f 636f 6c84 b306  ef...protocol...
+000015c0: 4861 6e64 6c65 8484 8484 8484 b5b1 0772  Handle.........r
+000015d0: 6574 7261 6374 b4b3 0372 6563 b4b3 036c  etract...rec...l
+000015e0: 6974 b307 7265 7472 6163 7484 b4b3 0574  it..retract....t
+000015f0: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0668  uple....named..h
+00001600: 616e 646c 65b4 b303 7265 66b5 b308 7072  andle...ref...pr
+00001610: 6f74 6f63 6f6c 84b3 0648 616e 646c 6584  otocol...Handle.
+00001620: 8484 8484 84b5 b107 6d65 7373 6167 65b4  ........message.
+00001630: b303 7265 63b4 b303 6c69 74b3 076d 6573  ..rec...lit..mes
+00001640: 7361 6765 84b4 b305 7475 706c 65b5 b4b3  sage....tuple...
+00001650: 056e 616d 6564 b304 626f 6479 b4b3 0372  .named..body...r
+00001660: 6566 b584 b314 4173 7365 7274 696f 6e44  ef....AssertionD
+00001670: 6573 6372 6970 7469 6f6e 8484 8484 8484  escription......
+00001680: b5b1 0473 796e 63b4 b303 7265 63b4 b303  ...sync...rec...
+00001690: 6c69 74b3 0473 796e 6384 b4b3 0574 7570  lit..sync....tup
+000016a0: 6c65 b5b4 b305 6e61 6d65 64b3 0470 6565  le....named..pee
+000016b0: 72b4 b303 7265 66b5 84b3 0654 6172 6765  r...ref....Targe
+000016c0: 7484 8484 8484 84b5 b109 6272 6561 6b4c  t.........breakL
+000016d0: 696e 6bb4 b303 7265 63b4 b303 6c69 74b3  ink...rec...lit.
+000016e0: 0a62 7265 616b 2d6c 696e 6b84 b4b3 0574  .break-link....t
+000016f0: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0673  uple....named..s
+00001700: 6f75 7263 65b4 b303 7265 66b5 84b3 0741  ource...ref....A
+00001710: 6374 6f72 4964 8484 b4b3 056e 616d 6564  ctorId.....named
+00001720: b306 6861 6e64 6c65 b4b3 0372 6566 b5b3  ..handle...ref..
+00001730: 0870 726f 746f 636f 6c84 b306 4861 6e64  .protocol...Hand
+00001740: 6c65 8484 8484 8484 8484 b30a 4578 6974  le..........Exit
+00001750: 5374 6174 7573 b4b3 026f 72b5 b5b1 026f  Status...or....o
+00001760: 6bb4 b303 6c69 74b3 026f 6b84 84b5 b105  k...lit..ok.....
+00001770: 4572 726f 72b4 b303 7265 66b5 b308 7072  Error...ref...pr
+00001780: 6f74 6f63 6f6c 84b3 0545 7272 6f72 8484  otocol...Error..
+00001790: 8484 b30a 5472 6163 6545 6e74 7279 b4b3  ....TraceEntry..
+000017a0: 0372 6563 b4b3 036c 6974 b305 7472 6163  .rec...lit..trac
+000017b0: 6584 b4b3 0574 7570 6c65 b5b4 b305 6e61  e....tuple....na
+000017c0: 6d65 64b3 0974 696d 6573 7461 6d70 b4b3  med..timestamp..
+000017d0: 0461 746f 6db3 0644 6f75 626c 6584 84b4  .atom..Double...
+000017e0: b305 6e61 6d65 64b3 0561 6374 6f72 b4b3  ..named..actor..
+000017f0: 0372 6566 b584 b307 4163 746f 7249 6484  .ref....ActorId.
+00001800: 84b4 b305 6e61 6d65 64b3 0469 7465 6db4  ....named..item.
+00001810: b303 7265 66b5 84b3 0f41 6374 6f72 4163  ..ref....ActorAc
+00001820: 7469 7661 7469 6f6e 8484 8484 84b3 0f41  tivation.......A
+00001830: 6374 6f72 4163 7469 7661 7469 6f6e b4b3  ctorActivation..
+00001840: 026f 72b5 b5b1 0573 7461 7274 b4b3 0372  .or....start...r
+00001850: 6563 b4b3 036c 6974 b305 7374 6172 7484  ec...lit..start.
+00001860: b4b3 0574 7570 6c65 b5b4 b305 6e61 6d65  ...tuple....name
+00001870: 64b3 0961 6374 6f72 4e61 6d65 b4b3 0372  d..actorName...r
+00001880: 6566 b584 b304 4e61 6d65 8484 8484 8484  ef....Name......
+00001890: b5b1 0474 7572 6eb4 b303 7265 66b5 84b3  ...turn...ref...
+000018a0: 0f54 7572 6e44 6573 6372 6970 7469 6f6e  .TurnDescription
+000018b0: 8484 b5b1 0473 746f 70b4 b303 7265 63b4  .....stop...rec.
+000018c0: b303 6c69 74b3 0473 746f 7084 b4b3 0574  ..lit..stop....t
+000018d0: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0673  uple....named..s
+000018e0: 7461 7475 73b4 b303 7265 66b5 84b3 0a45  tatus...ref....E
+000018f0: 7869 7453 7461 7475 7384 8484 8484 8484  xitStatus.......
+00001900: 84b3 0f46 6163 6574 5374 6f70 5265 6173  ...FacetStopReas
+00001910: 6f6e b4b3 026f 72b5 b5b1 0e65 7870 6c69  on...or....expli
+00001920: 6369 7441 6374 696f 6eb4 b303 6c69 74b3  citAction...lit.
+00001930: 0f65 7870 6c69 6369 742d 6163 7469 6f6e  .explicit-action
+00001940: 8484 b5b1 0569 6e65 7274 b4b3 036c 6974  .....inert...lit
+00001950: b305 696e 6572 7484 84b5 b10e 7061 7265  ..inert.....pare
+00001960: 6e74 5374 6f70 7069 6e67 b4b3 036c 6974  ntStopping...lit
+00001970: b30f 7061 7265 6e74 2d73 746f 7070 696e  ..parent-stoppin
+00001980: 6784 84b5 b10d 6163 746f 7253 746f 7070  g.....actorStopp
+00001990: 696e 67b4 b303 6c69 74b3 0e61 6374 6f72  ing...lit..actor
+000019a0: 2d73 746f 7070 696e 6784 8484 84b3 0f54  -stopping......T
+000019b0: 7572 6e44 6573 6372 6970 7469 6f6e b4b3  urnDescription..
+000019c0: 0372 6563 b4b3 036c 6974 b304 7475 726e  .rec...lit..turn
+000019d0: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
+000019e0: 6564 b302 6964 b4b3 0372 6566 b584 b306  ed..id...ref....
+000019f0: 5475 726e 4964 8484 b4b3 056e 616d 6564  TurnId.....named
+00001a00: b305 6361 7573 65b4 b303 7265 66b5 84b3  ..cause...ref...
+00001a10: 0954 7572 6e43 6175 7365 8484 b4b3 056e  .TurnCause.....n
+00001a20: 616d 6564 b307 6163 7469 6f6e 73b4 b305  amed..actions...
+00001a30: 7365 716f 66b4 b303 7265 66b5 84b3 1141  seqof...ref....A
+00001a40: 6374 696f 6e44 6573 6372 6970 7469 6f6e  ctionDescription
+00001a50: 8484 8484 8484 b311 4163 7469 6f6e 4465  ........ActionDe
+00001a60: 7363 7269 7074 696f 6eb4 b302 6f72 b5b5  scription...or..
+00001a70: b107 6465 7175 6575 65b4 b303 7265 63b4  ..dequeue...rec.
+00001a80: b303 6c69 74b3 0764 6571 7565 7565 84b4  ..lit..dequeue..
+00001a90: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
+00001aa0: b305 6576 656e 74b4 b303 7265 66b5 84b3  ..event...ref...
+00001ab0: 1154 6172 6765 7465 6454 7572 6e45 7665  .TargetedTurnEve
+00001ac0: 6e74 8484 8484 8484 b5b1 0765 6e71 7565  nt.........enque
+00001ad0: 7565 b4b3 0372 6563 b4b3 036c 6974 b307  ue...rec...lit..
+00001ae0: 656e 7175 6575 6584 b4b3 0574 7570 6c65  enqueue....tuple
+00001af0: b5b4 b305 6e61 6d65 64b3 0565 7665 6e74  ....named..event
+00001b00: b4b3 0372 6566 b584 b311 5461 7267 6574  ...ref....Target
+00001b10: 6564 5475 726e 4576 656e 7484 8484 8484  edTurnEvent.....
+00001b20: 84b5 b10f 6465 7175 6575 6549 6e74 6572  ....dequeueInter
+00001b30: 6e61 6cb4 b303 7265 63b4 b303 6c69 74b3  nal...rec...lit.
+00001b40: 1064 6571 7565 7565 2d69 6e74 6572 6e61  .dequeue-interna
+00001b50: 6c84 b4b3 0574 7570 6c65 b5b4 b305 6e61  l....tuple....na
+00001b60: 6d65 64b3 0565 7665 6e74 b4b3 0372 6566  med..event...ref
+00001b70: b584 b311 5461 7267 6574 6564 5475 726e  ....TargetedTurn
+00001b80: 4576 656e 7484 8484 8484 84b5 b10f 656e  Event.........en
+00001b90: 7175 6575 6549 6e74 6572 6e61 6cb4 b303  queueInternal...
+00001ba0: 7265 63b4 b303 6c69 74b3 1065 6e71 7565  rec...lit..enque
+00001bb0: 7565 2d69 6e74 6572 6e61 6c84 b4b3 0574  ue-internal....t
+00001bc0: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0565  uple....named..e
+00001bd0: 7665 6e74 b4b3 0372 6566 b584 b311 5461  vent...ref....Ta
+00001be0: 7267 6574 6564 5475 726e 4576 656e 7484  rgetedTurnEvent.
+00001bf0: 8484 8484 84b5 b105 7370 6177 6eb4 b303  ........spawn...
+00001c00: 7265 63b4 b303 6c69 74b3 0573 7061 776e  rec...lit..spawn
+00001c10: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
+00001c20: 6564 b304 6c69 6e6b b4b3 0461 746f 6db3  ed..link...atom.
+00001c30: 0742 6f6f 6c65 616e 8484 b4b3 056e 616d  .Boolean.....nam
+00001c40: 6564 b302 6964 b4b3 0372 6566 b584 b307  ed..id...ref....
+00001c50: 4163 746f 7249 6484 8484 8484 84b5 b104  ActorId.........
+00001c60: 6c69 6e6b b4b3 0372 6563 b4b3 036c 6974  link...rec...lit
+00001c70: b304 6c69 6e6b 84b4 b305 7475 706c 65b5  ..link....tuple.
+00001c80: b4b3 056e 616d 6564 b30b 7061 7265 6e74  ...named..parent
+00001c90: 4163 746f 72b4 b303 7265 66b5 84b3 0741  Actor...ref....A
+00001ca0: 6374 6f72 4964 8484 b4b3 056e 616d 6564  ctorId.....named
+00001cb0: b30d 6368 696c 6454 6f50 6172 656e 74b4  ..childToParent.
+00001cc0: b303 7265 66b5 b308 7072 6f74 6f63 6f6c  ..ref...protocol
+00001cd0: 84b3 0648 616e 646c 6584 84b4 b305 6e61  ...Handle.....na
+00001ce0: 6d65 64b3 0a63 6869 6c64 4163 746f 72b4  med..childActor.
+00001cf0: b303 7265 66b5 84b3 0741 6374 6f72 4964  ..ref....ActorId
+00001d00: 8484 b4b3 056e 616d 6564 b30d 7061 7265  .....named..pare
+00001d10: 6e74 546f 4368 696c 64b4 b303 7265 66b5  ntToChild...ref.
+00001d20: b308 7072 6f74 6f63 6f6c 84b3 0648 616e  ..protocol...Han
+00001d30: 646c 6584 8484 8484 84b5 b10a 6661 6365  dle.........face
+00001d40: 7453 7461 7274 b4b3 0372 6563 b4b3 036c  tStart...rec...l
+00001d50: 6974 b30b 6661 6365 742d 7374 6172 7484  it..facet-start.
+00001d60: b4b3 0574 7570 6c65 b5b4 b305 6e61 6d65  ...tuple....name
+00001d70: 64b3 0470 6174 68b4 b305 7365 716f 66b4  d..path...seqof.
+00001d80: b303 7265 66b5 84b3 0746 6163 6574 4964  ..ref....FacetId
+00001d90: 8484 8484 8484 84b5 b109 6661 6365 7453  ..........facetS
+00001da0: 746f 70b4 b303 7265 63b4 b303 6c69 74b3  top...rec...lit.
+00001db0: 0a66 6163 6574 2d73 746f 7084 b4b3 0574  .facet-stop....t
+00001dc0: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0470  uple....named..p
+00001dd0: 6174 68b4 b305 7365 716f 66b4 b303 7265  ath...seqof...re
+00001de0: 66b5 84b3 0746 6163 6574 4964 8484 84b4  f....FacetId....
+00001df0: b305 6e61 6d65 64b3 0672 6561 736f 6eb4  ..named..reason.
+00001e00: b303 7265 66b5 84b3 0f46 6163 6574 5374  ..ref....FacetSt
+00001e10: 6f70 5265 6173 6f6e 8484 8484 8484 b5b1  opReason........
+00001e20: 0f6c 696e 6b65 6454 6173 6b53 7461 7274  .linkedTaskStart
+00001e30: b4b3 0372 6563 b4b3 036c 6974 b311 6c69  ...rec...lit..li
+00001e40: 6e6b 6564 2d74 6173 6b2d 7374 6172 7484  nked-task-start.
+00001e50: b4b3 0574 7570 6c65 b5b4 b305 6e61 6d65  ...tuple....name
+00001e60: 64b3 0874 6173 6b4e 616d 65b4 b303 7265  d..taskName...re
+00001e70: 66b5 84b3 044e 616d 6584 84b4 b305 6e61  f....Name.....na
+00001e80: 6d65 64b3 0269 64b4 b303 7265 66b5 84b3  med..id...ref...
+00001e90: 0654 6173 6b49 6484 8484 8484 8484 84b3  .TaskId.........
+00001ea0: 1154 6172 6765 7465 6454 7572 6e45 7665  .TargetedTurnEve
+00001eb0: 6e74 b4b3 0372 6563 b4b3 036c 6974 b305  nt...rec...lit..
+00001ec0: 6576 656e 7484 b4b3 0574 7570 6c65 b5b4  event....tuple..
+00001ed0: b305 6e61 6d65 64b3 0674 6172 6765 74b4  ..named..target.
+00001ee0: b303 7265 66b5 84b3 0654 6172 6765 7484  ..ref....Target.
+00001ef0: 84b4 b305 6e61 6d65 64b3 0664 6574 6169  ....named..detai
+00001f00: 6cb4 b303 7265 66b5 84b3 0954 7572 6e45  l...ref....TurnE
+00001f10: 7665 6e74 8484 8484 84b3 1441 7373 6572  vent.......Asser
+00001f20: 7469 6f6e 4465 7363 7269 7074 696f 6eb4  tionDescription.
+00001f30: b302 6f72 b5b5 b105 7661 6c75 65b4 b303  ..or....value...
+00001f40: 7265 63b4 b303 6c69 74b3 0576 616c 7565  rec...lit..value
+00001f50: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
+00001f60: 6564 b305 7661 6c75 65b3 0361 6e79 8484  ed..value..any..
+00001f70: 8484 84b5 b106 6f70 6171 7565 b4b3 0372  ......opaque...r
+00001f80: 6563 b4b3 036c 6974 b306 6f70 6171 7565  ec...lit..opaque
+00001f90: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
+00001fa0: 6564 b30b 6465 7363 7269 7074 696f 6eb3  ed..description.
+00001fb0: 0361 6e79 8484 8484 8484 84b3 174c 696e  .any.........Lin
+00001fc0: 6b65 6454 6173 6b52 656c 6561 7365 5265  kedTaskReleaseRe
+00001fd0: 6173 6f6e b4b3 026f 72b5 b5b1 0963 616e  ason...or....can
+00001fe0: 6365 6c6c 6564 b4b3 036c 6974 b309 6361  celled...lit..ca
+00001ff0: 6e63 656c 6c65 6484 84b5 b106 6e6f 726d  ncelled.....norm
+00002000: 616c b4b3 036c 6974 b306 6e6f 726d 616c  al...lit..normal
+00002010: 8484 8484 84b3 0c65 6d62 6564 6465 6454  .......embeddedT
+00002020: 7970 65b4 b303 7265 66b5 b309 456e 7469  ype...ref...Enti
+00002030: 7479 5265 6684 b303 4361 7084 8484 b5b3  tyRef...Cap.....
+00002040: 0673 7472 6561 6d84 b4b3 0673 6368 656d  .stream....schem
+00002050: 61b7 b307 7665 7273 696f 6e91 b30b 6465  a...version...de
+00002060: 6669 6e69 7469 6f6e 73b7 b304 4d6f 6465  finitions...Mode
+00002070: b4b3 026f 72b5 b5b1 0562 7974 6573 b4b3  ...or....bytes..
+00002080: 036c 6974 b305 6279 7465 7384 84b5 b105  .lit..bytes.....
+00002090: 6c69 6e65 73b4 b303 7265 66b5 84b3 084c  lines...ref....L
+000020a0: 696e 654d 6f64 6584 84b5 b106 7061 636b  ineMode.....pack
+000020b0: 6574 b4b3 0372 6563 b4b3 036c 6974 b306  et...rec...lit..
+000020c0: 7061 636b 6574 84b4 b305 7475 706c 65b5  packet....tuple.
+000020d0: b4b3 056e 616d 6564 b304 7369 7a65 b4b3  ...named..size..
+000020e0: 0461 746f 6db3 0d53 6967 6e65 6449 6e74  .atom..SignedInt
+000020f0: 6567 6572 8484 8484 8484 b5b1 066f 626a  eger.........obj
+00002100: 6563 74b4 b303 7265 63b4 b303 6c69 74b3  ect...rec...lit.
+00002110: 066f 626a 6563 7484 b4b3 0574 7570 6c65  .object....tuple
+00002120: b5b4 b305 6e61 6d65 64b3 0b64 6573 6372  ....named..descr
+00002130: 6970 7469 6f6e b303 616e 7984 8484 8484  iption..any.....
+00002140: 8484 b304 5369 6e6b b4b3 026f 72b5 b5b1  ....Sink...or...
+00002150: 0673 6f75 7263 65b4 b303 7265 63b4 b303  .source...rec...
+00002160: 6c69 74b3 0673 6f75 7263 6584 b4b3 0574  lit..source....t
+00002170: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0a63  uple....named..c
+00002180: 6f6e 7472 6f6c 6c65 72b4 b308 656d 6265  ontroller...embe
+00002190: 6464 6564 b4b3 0372 6566 b584 b306 536f  dded...ref....So
+000021a0: 7572 6365 8484 8484 8484 84b5 b10b 5374  urce..........St
+000021b0: 7265 616d 4572 726f 72b4 b303 7265 66b5  reamError...ref.
+000021c0: 84b3 0b53 7472 6561 6d45 7272 6f72 8484  ...StreamError..
+000021d0: b5b1 0464 6174 61b4 b303 7265 63b4 b303  ...data...rec...
+000021e0: 6c69 74b3 0464 6174 6184 b4b3 0574 7570  lit..data....tup
+000021f0: 6c65 b5b4 b305 6e61 6d65 64b3 0770 6179  le....named..pay
+00002200: 6c6f 6164 b303 616e 7984 b4b3 056e 616d  load..any....nam
+00002210: 6564 b304 6d6f 6465 b4b3 0372 6566 b584  ed..mode...ref..
+00002220: b304 4d6f 6465 8484 8484 8484 b5b1 0365  ..Mode.........e
+00002230: 6f66 b4b3 0372 6563 b4b3 036c 6974 b303  of...rec...lit..
+00002240: 656f 6684 b4b3 0574 7570 6c65 b584 8484  eof....tuple....
+00002250: 8484 84b3 0653 6f75 7263 65b4 b302 6f72  .....Source...or
+00002260: b5b5 b104 7369 6e6b b4b3 0372 6563 b4b3  ....sink...rec..
+00002270: 036c 6974 b304 7369 6e6b 84b4 b305 7475  .lit..sink....tu
+00002280: 706c 65b5 b4b3 056e 616d 6564 b30a 636f  ple....named..co
+00002290: 6e74 726f 6c6c 6572 b4b3 0865 6d62 6564  ntroller...embed
+000022a0: 6465 64b4 b303 7265 66b5 84b3 0453 696e  ded...ref....Sin
+000022b0: 6b84 8484 8484 8484 b5b1 0b53 7472 6561  k..........Strea
+000022c0: 6d45 7272 6f72 b4b3 0372 6566 b584 b30b  mError...ref....
+000022d0: 5374 7265 616d 4572 726f 7284 84b5 b106  StreamError.....
+000022e0: 6372 6564 6974 b4b3 0372 6563 b4b3 036c  credit...rec...l
+000022f0: 6974 b306 6372 6564 6974 84b4 b305 7475  it..credit....tu
+00002300: 706c 65b5 b4b3 056e 616d 6564 b306 616d  ple....named..am
+00002310: 6f75 6e74 b4b3 0372 6566 b584 b30c 4372  ount...ref....Cr
+00002320: 6564 6974 416d 6f75 6e74 8484 b4b3 056e  editAmount.....n
+00002330: 616d 6564 b304 6d6f 6465 b4b3 0372 6566  amed..mode...ref
+00002340: b584 b304 4d6f 6465 8484 8484 8484 8484  ....Mode........
+00002350: b308 4c69 6e65 4d6f 6465 b4b3 026f 72b5  ..LineMode...or.
+00002360: b5b1 026c 66b4 b303 6c69 74b3 026c 6684  ...lf...lit..lf.
+00002370: 84b5 b104 6372 6c66 b4b3 036c 6974 b304  ....crlf...lit..
+00002380: 6372 6c66 8484 8484 b30b 5374 7265 616d  crlf......Stream
+00002390: 4572 726f 72b4 b303 7265 63b4 b303 6c69  Error...rec...li
+000023a0: 74b3 0565 7272 6f72 84b4 b305 7475 706c  t..error....tupl
+000023b0: 65b5 b4b3 056e 616d 6564 b307 6d65 7373  e....named..mess
+000023c0: 6167 65b4 b304 6174 6f6d b306 5374 7269  age...atom..Stri
+000023d0: 6e67 8484 8484 84b3 0c43 7265 6469 7441  ng.......CreditA
+000023e0: 6d6f 756e 74b4 b302 6f72 b5b5 b105 636f  mount...or....co
+000023f0: 756e 74b4 b304 6174 6f6d b30d 5369 676e  unt...atom..Sign
+00002400: 6564 496e 7465 6765 7284 84b5 b109 756e  edInteger.....un
+00002410: 626f 756e 6465 64b4 b303 6c69 74b3 0975  bounded...lit..u
+00002420: 6e62 6f75 6e64 6564 8484 8484 b310 5374  nbounded......St
+00002430: 7265 616d 436f 6e6e 6563 7469 6f6e b4b3  reamConnection..
+00002440: 0372 6563 b4b3 036c 6974 b311 7374 7265  .rec...lit..stre
+00002450: 616d 2d63 6f6e 6e65 6374 696f 6e84 b4b3  am-connection...
+00002460: 0574 7570 6c65 b5b4 b305 6e61 6d65 64b3  .tuple....named.
+00002470: 0673 6f75 7263 65b4 b308 656d 6265 6464  .source...embedd
+00002480: 6564 b4b3 0372 6566 b584 b306 536f 7572  ed...ref....Sour
+00002490: 6365 8484 84b4 b305 6e61 6d65 64b3 0473  ce......named..s
+000024a0: 696e 6bb4 b308 656d 6265 6464 6564 b4b3  ink...embedded..
+000024b0: 0372 6566 b584 b304 5369 6e6b 8484 84b4  .ref....Sink....
+000024c0: b305 6e61 6d65 64b3 0473 7065 63b3 0361  ..named..spec..a
+000024d0: 6e79 8484 8484 b313 5374 7265 616d 4c69  ny......StreamLi
+000024e0: 7374 656e 6572 4572 726f 72b4 b303 7265  stenerError...re
+000024f0: 63b4 b303 6c69 74b3 1573 7472 6561 6d2d  c...lit..stream-
+00002500: 6c69 7374 656e 6572 2d65 7272 6f72 84b4  listener-error..
+00002510: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
+00002520: b304 7370 6563 b303 616e 7984 b4b3 056e  ..spec..any....n
+00002530: 616d 6564 b307 6d65 7373 6167 65b4 b304  amed..message...
+00002540: 6174 6f6d b306 5374 7269 6e67 8484 8484  atom..String....
+00002550: 84b3 1353 7472 6561 6d4c 6973 7465 6e65  ...StreamListene
+00002560: 7252 6561 6479 b4b3 0372 6563 b4b3 036c  rReady...rec...l
+00002570: 6974 b315 7374 7265 616d 2d6c 6973 7465  it..stream-liste
+00002580: 6e65 722d 7265 6164 7984 b4b3 0574 7570  ner-ready....tup
+00002590: 6c65 b5b4 b305 6e61 6d65 64b3 0473 7065  le....named..spe
+000025a0: 63b3 0361 6e79 8484 8484 84b3 0c65 6d62  c..any.......emb
+000025b0: 6564 6465 6454 7970 65b4 b303 7265 66b5  eddedType...ref.
+000025c0: b309 456e 7469 7479 5265 6684 b303 4361  ..EntityRef...Ca
+000025d0: 7084 8484 b5b3 0673 7475 7264 7984 b4b3  p......sturdy...
+000025e0: 0673 6368 656d 61b7 b307 7665 7273 696f  .schema...versio
+000025f0: 6e91 b30b 6465 6669 6e69 7469 6f6e 73b7  n...definitions.
+00002600: b303 4c69 74b4 b303 7265 63b4 b303 6c69  ..Lit...rec...li
+00002610: 74b3 036c 6974 84b4 b305 7475 706c 65b5  t..lit....tuple.
+00002620: b4b3 056e 616d 6564 b305 7661 6c75 65b3  ...named..value.
+00002630: 0361 6e79 8484 8484 b303 4f69 64b4 b304  .any......Oid...
+00002640: 6174 6f6d b30d 5369 676e 6564 496e 7465  atom..SignedInte
+00002650: 6765 7284 b304 416c 7473 b4b3 0372 6563  ger...Alts...rec
+00002660: b4b3 036c 6974 b302 6f72 84b4 b305 7475  ...lit..or....tu
+00002670: 706c 65b5 b4b3 056e 616d 6564 b30c 616c  ple....named..al
+00002680: 7465 726e 6174 6976 6573 b4b3 0573 6571  ternatives...seq
+00002690: 6f66 b4b3 0372 6566 b584 b307 5265 7772  of...ref....Rewr
+000026a0: 6974 6584 8484 8484 84b3 0450 416e 64b4  ite........PAnd.
+000026b0: b303 7265 63b4 b303 6c69 74b3 0361 6e64  ..rec...lit..and
+000026c0: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
+000026d0: 6564 b308 7061 7474 6572 6e73 b4b3 0573  ed..patterns...s
+000026e0: 6571 6f66 b4b3 0372 6566 b584 b307 5061  eqof...ref....Pa
+000026f0: 7474 6572 6e84 8484 8484 84b3 0450 4e6f  ttern........PNo
+00002700: 74b4 b303 7265 63b4 b303 6c69 74b3 036e  t...rec...lit..n
+00002710: 6f74 84b4 b305 7475 706c 65b5 b4b3 056e  ot....tuple....n
+00002720: 616d 6564 b307 7061 7474 6572 6eb4 b303  amed..pattern...
+00002730: 7265 66b5 84b3 0750 6174 7465 726e 8484  ref....Pattern..
+00002740: 8484 84b3 0454 5265 66b4 b303 7265 63b4  .....TRef...rec.
+00002750: b303 6c69 74b3 0372 6566 84b4 b305 7475  ..lit..ref....tu
+00002760: 706c 65b5 b4b3 056e 616d 6564 b307 6269  ple....named..bi
+00002770: 6e64 696e 67b4 b304 6174 6f6d b30d 5369  nding...atom..Si
+00002780: 676e 6564 496e 7465 6765 7284 8484 8484  gnedInteger.....
+00002790: b305 5041 746f 6db4 b302 6f72 b5b5 b107  ..PAtom...or....
+000027a0: 426f 6f6c 6561 6eb4 b303 6c69 74b3 0742  Boolean...lit..B
+000027b0: 6f6f 6c65 616e 8484 b5b1 0546 6c6f 6174  oolean.....Float
+000027c0: b4b3 036c 6974 b305 466c 6f61 7484 84b5  ...lit..Float...
+000027d0: b106 446f 7562 6c65 b4b3 036c 6974 b306  ..Double...lit..
+000027e0: 446f 7562 6c65 8484 b5b1 0d53 6967 6e65  Double.....Signe
+000027f0: 6449 6e74 6567 6572 b4b3 036c 6974 b30d  dInteger...lit..
+00002800: 5369 676e 6564 496e 7465 6765 7284 84b5  SignedInteger...
+00002810: b106 5374 7269 6e67 b4b3 036c 6974 b306  ..String...lit..
+00002820: 5374 7269 6e67 8484 b5b1 0a42 7974 6553  String.....ByteS
+00002830: 7472 696e 67b4 b303 6c69 74b3 0a42 7974  tring...lit..Byt
+00002840: 6553 7472 696e 6784 84b5 b106 5379 6d62  eString.....Symb
+00002850: 6f6c b4b3 036c 6974 b306 5379 6d62 6f6c  ol...lit..Symbol
+00002860: 8484 8484 b305 5042 696e 64b4 b303 7265  ......PBind...re
+00002870: 63b4 b303 6c69 74b3 0462 696e 6484 b4b3  c...lit..bind...
+00002880: 0574 7570 6c65 b5b4 b305 6e61 6d65 64b3  .tuple....named.
+00002890: 0770 6174 7465 726e b4b3 0372 6566 b584  .pattern...ref..
+000028a0: b307 5061 7474 6572 6e84 8484 8484 b306  ..Pattern.......
+000028b0: 4361 7665 6174 b4b3 026f 72b5 b5b1 0752  Caveat...or....R
+000028c0: 6577 7269 7465 b4b3 0372 6566 b584 b307  ewrite...ref....
+000028d0: 5265 7772 6974 6584 84b5 b104 416c 7473  Rewrite.....Alts
+000028e0: b4b3 0372 6566 b584 b304 416c 7473 8484  ...ref....Alts..
+000028f0: b5b1 0652 656a 6563 74b4 b303 7265 66b5  ...Reject...ref.
+00002900: 84b3 0652 656a 6563 7484 84b5 b107 756e  ...Reject.....un
+00002910: 6b6e 6f77 6eb3 0361 6e79 8484 84b3 0652  known..any.....R
+00002920: 656a 6563 74b4 b303 7265 63b4 b303 6c69  eject...rec...li
+00002930: 74b3 0672 656a 6563 7484 b4b3 0574 7570  t..reject....tup
+00002940: 6c65 b5b4 b305 6e61 6d65 64b3 0770 6174  le....named..pat
+00002950: 7465 726e b4b3 0372 6566 b584 b307 5061  tern...ref....Pa
+00002960: 7474 6572 6e84 8484 8484 b307 5061 7474  ttern.......Patt
+00002970: 6572 6eb4 b302 6f72 b5b5 b108 5044 6973  ern...or....PDis
+00002980: 6361 7264 b4b3 0372 6566 b584 b308 5044  card...ref....PD
+00002990: 6973 6361 7264 8484 b5b1 0550 4174 6f6d  iscard.....PAtom
+000029a0: b4b3 0372 6566 b584 b305 5041 746f 6d84  ...ref....PAtom.
+000029b0: 84b5 b109 5045 6d62 6564 6465 64b4 b303  ....PEmbedded...
+000029c0: 7265 66b5 84b3 0950 456d 6265 6464 6564  ref....PEmbedded
+000029d0: 8484 b5b1 0550 4269 6e64 b4b3 0372 6566  .....PBind...ref
+000029e0: b584 b305 5042 696e 6484 84b5 b104 5041  ....PBind.....PA
+000029f0: 6e64 b4b3 0372 6566 b584 b304 5041 6e64  nd...ref....PAnd
+00002a00: 8484 b5b1 0450 4e6f 74b4 b303 7265 66b5  .....PNot...ref.
+00002a10: 84b3 0450 4e6f 7484 84b5 b103 4c69 74b4  ...PNot.....Lit.
+00002a20: b303 7265 66b5 84b3 034c 6974 8484 b5b1  ..ref....Lit....
+00002a30: 0950 436f 6d70 6f75 6e64 b4b3 0372 6566  .PCompound...ref
+00002a40: b584 b309 5043 6f6d 706f 756e 6484 8484  ....PCompound...
+00002a50: 84b3 0752 6577 7269 7465 b4b3 0372 6563  ...Rewrite...rec
+00002a60: b4b3 036c 6974 b307 7265 7772 6974 6584  ...lit..rewrite.
+00002a70: b4b3 0574 7570 6c65 b5b4 b305 6e61 6d65  ...tuple....name
+00002a80: 64b3 0770 6174 7465 726e b4b3 0372 6566  d..pattern...ref
+00002a90: b584 b307 5061 7474 6572 6e84 84b4 b305  ....Pattern.....
+00002aa0: 6e61 6d65 64b3 0874 656d 706c 6174 65b4  named..template.
+00002ab0: b303 7265 66b5 84b3 0854 656d 706c 6174  ..ref....Templat
+00002ac0: 6584 8484 8484 b307 5769 7265 5265 66b4  e.......WireRef.
+00002ad0: b302 6f72 b5b5 b104 6d69 6e65 b4b3 0574  ..or....mine...t
+00002ae0: 7570 6c65 b5b4 b303 6c69 7490 84b4 b305  uple....lit.....
+00002af0: 6e61 6d65 64b3 036f 6964 b4b3 0372 6566  named..oid...ref
+00002b00: b584 b303 4f69 6484 8484 8484 b5b1 0579  ....Oid........y
+00002b10: 6f75 7273 b4b3 0b74 7570 6c65 5072 6566  ours...tuplePref
+00002b20: 6978 b5b4 b303 6c69 7491 84b4 b305 6e61  ix....lit.....na
+00002b30: 6d65 64b3 036f 6964 b4b3 0372 6566 b584  med..oid...ref..
+00002b40: b303 4f69 6484 8484 b4b3 056e 616d 6564  ..Oid......named
+00002b50: b30b 6174 7465 6e75 6174 696f 6eb4 b305  ..attenuation...
+00002b60: 7365 716f 66b4 b303 7265 66b5 84b3 0643  seqof...ref....C
+00002b70: 6176 6561 7484 8484 8484 8484 b308 5044  aveat.........PD
+00002b80: 6973 6361 7264 b4b3 0372 6563 b4b3 036c  iscard...rec...l
+00002b90: 6974 b301 5f84 b4b3 0574 7570 6c65 b584  it.._....tuple..
+00002ba0: 8484 b308 5465 6d70 6c61 7465 b4b3 026f  ....Template...o
+00002bb0: 72b5 b5b1 0a54 4174 7465 6e75 6174 65b4  r....TAttenuate.
+00002bc0: b303 7265 66b5 84b3 0a54 4174 7465 6e75  ..ref....TAttenu
+00002bd0: 6174 6584 84b5 b104 5452 6566 b4b3 0372  ate.....TRef...r
+00002be0: 6566 b584 b304 5452 6566 8484 b5b1 034c  ef....TRef.....L
+00002bf0: 6974 b4b3 0372 6566 b584 b303 4c69 7484  it...ref....Lit.
+00002c00: 84b5 b109 5443 6f6d 706f 756e 64b4 b303  ....TCompound...
+00002c10: 7265 66b5 84b3 0954 436f 6d70 6f75 6e64  ref....TCompound
+00002c20: 8484 8484 b309 5043 6f6d 706f 756e 64b4  ......PCompound.
+00002c30: b302 6f72 b5b5 b103 7265 63b4 b303 7265  ..or....rec...re
+00002c40: 63b4 b303 6c69 74b3 0372 6563 84b4 b305  c...lit..rec....
+00002c50: 7475 706c 65b5 b4b3 056e 616d 6564 b305  tuple....named..
+00002c60: 6c61 6265 6cb3 0361 6e79 84b4 b305 6e61  label..any....na
+00002c70: 6d65 64b3 0666 6965 6c64 73b4 b305 7365  med..fields...se
+00002c80: 716f 66b4 b303 7265 66b5 84b3 0750 6174  qof...ref....Pat
+00002c90: 7465 726e 8484 8484 8484 84b5 b103 6172  tern..........ar
+00002ca0: 72b4 b303 7265 63b4 b303 6c69 74b3 0361  r...rec...lit..a
+00002cb0: 7272 84b4 b305 7475 706c 65b5 b4b3 056e  rr....tuple....n
+00002cc0: 616d 6564 b305 6974 656d 73b4 b305 7365  amed..items...se
+00002cd0: 716f 66b4 b303 7265 66b5 84b3 0750 6174  qof...ref....Pat
+00002ce0: 7465 726e 8484 8484 8484 84b5 b104 6469  tern..........di
+00002cf0: 6374 b4b3 0372 6563 b4b3 036c 6974 b304  ct...rec...lit..
+00002d00: 6469 6374 84b4 b305 7475 706c 65b5 b4b3  dict....tuple...
+00002d10: 056e 616d 6564 b307 656e 7472 6965 73b4  .named..entries.
+00002d20: b306 6469 6374 6f66 b303 616e 79b4 b303  ..dictof..any...
+00002d30: 7265 66b5 84b3 0750 6174 7465 726e 8484  ref....Pattern..
+00002d40: 8484 8484 8484 84b3 0950 456d 6265 6464  .........PEmbedd
+00002d50: 6564 b4b3 036c 6974 b308 456d 6265 6464  ed...lit..Embedd
+00002d60: 6564 84b3 0953 7475 7264 7952 6566 b4b3  ed...SturdyRef..
+00002d70: 0372 6563 b4b3 036c 6974 b303 7265 6684  .rec...lit..ref.
+00002d80: b4b3 0574 7570 6c65 b5b4 b305 6e61 6d65  ...tuple....name
+00002d90: 64b3 036f 6964 b303 616e 7984 b4b3 056e  d..oid..any....n
+00002da0: 616d 6564 b30b 6361 7665 6174 4368 6169  amed..caveatChai
+00002db0: 6eb4 b305 7365 716f 66b4 b303 7265 66b5  n...seqof...ref.
+00002dc0: 84b3 0643 6176 6561 7484 8484 b4b3 056e  ...Caveat......n
+00002dd0: 616d 6564 b303 7369 67b4 b304 6174 6f6d  amed..sig...atom
+00002de0: b30a 4279 7465 5374 7269 6e67 8484 8484  ..ByteString....
+00002df0: 84b3 0954 436f 6d70 6f75 6e64 b4b3 026f  ...TCompound...o
+00002e00: 72b5 b5b1 0372 6563 b4b3 0372 6563 b4b3  r....rec...rec..
+00002e10: 036c 6974 b303 7265 6384 b4b3 0574 7570  .lit..rec....tup
+00002e20: 6c65 b5b4 b305 6e61 6d65 64b3 056c 6162  le....named..lab
+00002e30: 656c b303 616e 7984 b4b3 056e 616d 6564  el..any....named
+00002e40: b306 6669 656c 6473 b4b3 0573 6571 6f66  ..fields...seqof
+00002e50: b4b3 0372 6566 b584 b308 5465 6d70 6c61  ...ref....Templa
+00002e60: 7465 8484 8484 8484 84b5 b103 6172 72b4  te..........arr.
+00002e70: b303 7265 63b4 b303 6c69 74b3 0361 7272  ..rec...lit..arr
+00002e80: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
+00002e90: 6564 b305 6974 656d 73b4 b305 7365 716f  ed..items...seqo
+00002ea0: 66b4 b303 7265 66b5 84b3 0854 656d 706c  f...ref....Templ
+00002eb0: 6174 6584 8484 8484 8484 b5b1 0464 6963  ate..........dic
+00002ec0: 74b4 b303 7265 63b4 b303 6c69 74b3 0464  t...rec...lit..d
+00002ed0: 6963 7484 b4b3 0574 7570 6c65 b5b4 b305  ict....tuple....
+00002ee0: 6e61 6d65 64b3 0765 6e74 7269 6573 b4b3  named..entries..
+00002ef0: 0664 6963 746f 66b3 0361 6e79 b4b3 0372  .dictof..any...r
+00002f00: 6566 b584 b308 5465 6d70 6c61 7465 8484  ef....Template..
+00002f10: 8484 8484 8484 84b3 0a54 4174 7465 6e75  .........TAttenu
+00002f20: 6174 65b4 b303 7265 63b4 b303 6c69 74b3  ate...rec...lit.
+00002f30: 0961 7474 656e 7561 7465 84b4 b305 7475  .attenuate....tu
+00002f40: 706c 65b5 b4b3 056e 616d 6564 b308 7465  ple....named..te
+00002f50: 6d70 6c61 7465 b4b3 0372 6566 b584 b308  mplate...ref....
+00002f60: 5465 6d70 6c61 7465 8484 b4b3 056e 616d  Template.....nam
+00002f70: 6564 b30b 6174 7465 6e75 6174 696f 6eb4  ed..attenuation.
+00002f80: b305 7365 716f 66b4 b303 7265 66b5 84b3  ..seqof...ref...
+00002f90: 0643 6176 6561 7484 8484 8484 8484 b30c  .Caveat.........
+00002fa0: 656d 6265 6464 6564 5479 7065 b4b3 0372  embeddedType...r
+00002fb0: 6566 b5b3 0945 6e74 6974 7952 6566 84b3  ef...EntityRef..
+00002fc0: 0343 6170 8484 84b5 b306 776f 726b 6572  .Cap......worker
+00002fd0: 84b4 b306 7363 6865 6d61 b7b3 0776 6572  ....schema...ver
+00002fe0: 7369 6f6e 91b3 0b64 6566 696e 6974 696f  sion...definitio
+00002ff0: 6e73 b7b3 0849 6e73 7461 6e63 65b4 b303  ns...Instance...
+00003000: 7265 63b4 b303 6c69 74b3 0849 6e73 7461  rec...lit..Insta
+00003010: 6e63 6584 b4b3 0574 7570 6c65 b5b4 b305  nce....tuple....
+00003020: 6e61 6d65 64b3 046e 616d 65b4 b304 6174  named..name...at
+00003030: 6f6d b306 5374 7269 6e67 8484 b4b3 056e  om..String.....n
+00003040: 616d 6564 b308 6172 6775 6d65 6e74 b303  amed..argument..
+00003050: 616e 7984 8484 8484 b30c 656d 6265 6464  any.......embedd
+00003060: 6564 5479 7065 b4b3 0372 6566 b5b3 0945  edType...ref...E
+00003070: 6e74 6974 7952 6566 84b3 0343 6170 8484  ntityRef...Cap..
+00003080: 84b5 b307 7365 7276 6963 6584 b4b3 0673  ....service....s
+00003090: 6368 656d 61b7 b307 7665 7273 696f 6e91  chema...version.
+000030a0: b30b 6465 6669 6e69 7469 6f6e 73b7 b305  ..definitions...
+000030b0: 5374 6174 65b4 b302 6f72 b5b5 b107 7374  State...or....st
+000030c0: 6172 7465 64b4 b303 6c69 74b3 0773 7461  arted...lit..sta
+000030d0: 7274 6564 8484 b5b1 0572 6561 6479 b4b3  rted.....ready..
+000030e0: 036c 6974 b305 7265 6164 7984 84b5 b106  .lit..ready.....
+000030f0: 6661 696c 6564 b4b3 036c 6974 b306 6661  failed...lit..fa
+00003100: 696c 6564 8484 b5b1 0863 6f6d 706c 6574  iled.....complet
+00003110: 65b4 b303 6c69 74b3 0863 6f6d 706c 6574  e...lit..complet
+00003120: 6584 84b5 b10b 7573 6572 4465 6669 6e65  e.....userDefine
+00003130: 64b3 0361 6e79 8484 84b3 0a52 756e 5365  d..any.....RunSe
+00003140: 7276 6963 65b4 b303 7265 63b4 b303 6c69  rvice...rec...li
+00003150: 74b3 0b72 756e 2d73 6572 7669 6365 84b4  t..run-service..
+00003160: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
+00003170: b30b 7365 7276 6963 654e 616d 65b3 0361  ..serviceName..a
+00003180: 6e79 8484 8484 b30c 5365 7276 6963 6553  ny......ServiceS
+00003190: 7461 7465 b4b3 0372 6563 b4b3 036c 6974  tate...rec...lit
+000031a0: b30d 7365 7276 6963 652d 7374 6174 6584  ..service-state.
+000031b0: b4b3 0574 7570 6c65 b5b4 b305 6e61 6d65  ...tuple....name
+000031c0: 64b3 0b73 6572 7669 6365 4e61 6d65 b303  d..serviceName..
+000031d0: 616e 7984 b4b3 056e 616d 6564 b305 7374  any....named..st
+000031e0: 6174 65b4 b303 7265 66b5 84b3 0553 7461  ate...ref....Sta
+000031f0: 7465 8484 8484 84b3 0d53 6572 7669 6365  te.......Service
+00003200: 4f62 6a65 6374 b4b3 0372 6563 b4b3 036c  Object...rec...l
+00003210: 6974 b30e 7365 7276 6963 652d 6f62 6a65  it..service-obje
+00003220: 6374 84b4 b305 7475 706c 65b5 b4b3 056e  ct....tuple....n
+00003230: 616d 6564 b30b 7365 7276 6963 654e 616d  amed..serviceNam
+00003240: 65b3 0361 6e79 84b4 b305 6e61 6d65 64b3  e..any....named.
+00003250: 066f 626a 6563 74b3 0361 6e79 8484 8484  .object..any....
+00003260: b30e 5265 7175 6972 6553 6572 7669 6365  ..RequireService
+00003270: b4b3 0372 6563 b4b3 036c 6974 b30f 7265  ...rec...lit..re
+00003280: 7175 6972 652d 7365 7276 6963 6584 b4b3  quire-service...
+00003290: 0574 7570 6c65 b5b4 b305 6e61 6d65 64b3  .tuple....named.
+000032a0: 0b73 6572 7669 6365 4e61 6d65 b303 616e  .serviceName..an
+000032b0: 7984 8484 84b3 0e52 6573 7461 7274 5365  y......RestartSe
+000032c0: 7276 6963 65b4 b303 7265 63b4 b303 6c69  rvice...rec...li
+000032d0: 74b3 0f72 6573 7461 7274 2d73 6572 7669  t..restart-servi
+000032e0: 6365 84b4 b305 7475 706c 65b5 b4b3 056e  ce....tuple....n
+000032f0: 616d 6564 b30b 7365 7276 6963 654e 616d  amed..serviceNam
+00003300: 65b3 0361 6e79 8484 8484 b311 5365 7276  e..any......Serv
+00003310: 6963 6544 6570 656e 6465 6e63 79b4 b303  iceDependency...
+00003320: 7265 63b4 b303 6c69 74b3 0a64 6570 656e  rec...lit..depen
+00003330: 6473 2d6f 6e84 b4b3 0574 7570 6c65 b5b4  ds-on....tuple..
+00003340: b305 6e61 6d65 64b3 0864 6570 656e 6465  ..named..depende
+00003350: 72b3 0361 6e79 84b4 b305 6e61 6d65 64b3  r..any....named.
+00003360: 0864 6570 656e 6465 65b4 b303 7265 66b5  .dependee...ref.
+00003370: 84b3 0c53 6572 7669 6365 5374 6174 6584  ...ServiceState.
+00003380: 8484 8484 84b3 0c65 6d62 6564 6465 6454  .......embeddedT
+00003390: 7970 65b4 b303 7265 66b5 b309 456e 7469  ype...ref...Enti
+000033a0: 7479 5265 6684 b303 4361 7084 8484 b5b3  tyRef...Cap.....
+000033b0: 0870 726f 746f 636f 6c84 b4b3 0673 6368  .protocol....sch
+000033c0: 656d 61b7 b307 7665 7273 696f 6e91 b30b  ema...version...
+000033d0: 6465 6669 6e69 7469 6f6e 73b7 b303 4f69  definitions...Oi
+000033e0: 64b4 b304 6174 6f6d b30d 5369 676e 6564  d...atom..Signed
+000033f0: 496e 7465 6765 7284 b304 5379 6e63 b4b3  Integer...Sync..
+00003400: 0372 6563 b4b3 036c 6974 b304 7379 6e63  .rec...lit..sync
+00003410: 84b4 b305 7475 706c 65b5 b4b3 056e 616d  ....tuple....nam
+00003420: 6564 b304 7065 6572 b4b3 0865 6d62 6564  ed..peer...embed
+00003430: 6465 64b4 b303 6c69 7481 8484 8484 8484  ded...lit.......
+00003440: b304 5475 726e b4b3 0573 6571 6f66 b4b3  ..Turn...seqof..
+00003450: 0372 6566 b584 b309 5475 726e 4576 656e  .ref....TurnEven
+00003460: 7484 84b3 0545 7272 6f72 b4b3 0372 6563  t....Error...rec
+00003470: b4b3 036c 6974 b305 6572 726f 7284 b4b3  ...lit..error...
+00003480: 0574 7570 6c65 b5b4 b305 6e61 6d65 64b3  .tuple....named.
+00003490: 076d 6573 7361 6765 b4b3 0461 746f 6db3  .message...atom.
+000034a0: 0653 7472 696e 6784 84b4 b305 6e61 6d65  .String.....name
+000034b0: 64b3 0664 6574 6169 6cb3 0361 6e79 8484  d..detail..any..
+000034c0: 8484 b305 4576 656e 74b4 b302 6f72 b5b5  ....Event...or..
+000034d0: b106 4173 7365 7274 b4b3 0372 6566 b584  ..Assert...ref..
+000034e0: b306 4173 7365 7274 8484 b5b1 0752 6574  ..Assert.....Ret
+000034f0: 7261 6374 b4b3 0372 6566 b584 b307 5265  ract...ref....Re
+00003500: 7472 6163 7484 84b5 b107 4d65 7373 6167  tract.....Messag
+00003510: 65b4 b303 7265 66b5 84b3 074d 6573 7361  e...ref....Messa
+00003520: 6765 8484 b5b1 0453 796e 63b4 b303 7265  ge.....Sync...re
+00003530: 66b5 84b3 0453 796e 6384 8484 84b3 0641  f....Sync......A
+00003540: 7373 6572 74b4 b303 7265 63b4 b303 6c69  ssert...rec...li
+00003550: 74b3 0661 7373 6572 7484 b4b3 0574 7570  t..assert....tup
+00003560: 6c65 b5b4 b305 6e61 6d65 64b3 0961 7373  le....named..ass
+00003570: 6572 7469 6f6e b4b3 0372 6566 b584 b309  ertion...ref....
+00003580: 4173 7365 7274 696f 6e84 84b4 b305 6e61  Assertion.....na
+00003590: 6d65 64b3 0668 616e 646c 65b4 b303 7265  med..handle...re
+000035a0: 66b5 84b3 0648 616e 646c 6584 8484 8484  f....Handle.....
+000035b0: b306 4861 6e64 6c65 b4b3 0461 746f 6db3  ..Handle...atom.
+000035c0: 0d53 6967 6e65 6449 6e74 6567 6572 84b3  .SignedInteger..
+000035d0: 0650 6163 6b65 74b4 b302 6f72 b5b5 b104  .Packet...or....
+000035e0: 5475 726e b4b3 0372 6566 b584 b304 5475  Turn...ref....Tu
+000035f0: 726e 8484 b5b1 0545 7272 6f72 b4b3 0372  rn.....Error...r
+00003600: 6566 b584 b305 4572 726f 7284 84b5 b109  ef....Error.....
+00003610: 4578 7465 6e73 696f 6eb4 b303 7265 66b5  Extension...ref.
+00003620: 84b3 0945 7874 656e 7369 6f6e 8484 8484  ...Extension....
+00003630: b307 4d65 7373 6167 65b4 b303 7265 63b4  ..Message...rec.
+00003640: b303 6c69 74b3 076d 6573 7361 6765 84b4  ..lit..message..
+00003650: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
+00003660: b304 626f 6479 b4b3 0372 6566 b584 b309  ..body...ref....
+00003670: 4173 7365 7274 696f 6e84 8484 8484 b307  Assertion.......
+00003680: 5265 7472 6163 74b4 b303 7265 63b4 b303  Retract...rec...
+00003690: 6c69 74b3 0772 6574 7261 6374 84b4 b305  lit..retract....
+000036a0: 7475 706c 65b5 b4b3 056e 616d 6564 b306  tuple....named..
+000036b0: 6861 6e64 6c65 b4b3 0372 6566 b584 b306  handle...ref....
+000036c0: 4861 6e64 6c65 8484 8484 84b3 0941 7373  Handle.......Ass
+000036d0: 6572 7469 6f6e b303 616e 79b3 0945 7874  ertion..any..Ext
+000036e0: 656e 7369 6f6e b4b3 0372 6563 b4b3 056e  ension...rec...n
+000036f0: 616d 6564 b305 6c61 6265 6cb3 0361 6e79  amed..label..any
+00003700: 84b4 b305 6e61 6d65 64b3 0666 6965 6c64  ....named..field
+00003710: 73b4 b305 7365 716f 66b3 0361 6e79 8484  s...seqof..any..
+00003720: 84b3 0954 7572 6e45 7665 6e74 b4b3 0574  ...TurnEvent...t
+00003730: 7570 6c65 b5b4 b305 6e61 6d65 64b3 036f  uple....named..o
+00003740: 6964 b4b3 0372 6566 b584 b303 4f69 6484  id...ref....Oid.
+00003750: 84b4 b305 6e61 6d65 64b3 0565 7665 6e74  ....named..event
+00003760: b4b3 0372 6566 b584 b305 4576 656e 7484  ...ref....Event.
+00003770: 8484 8484 b30c 656d 6265 6464 6564 5479  ......embeddedTy
+00003780: 7065 8084 84b5 b309 6461 7461 7370 6163  pe......dataspac
+00003790: 6584 b4b3 0673 6368 656d 61b7 b307 7665  e....schema...ve
+000037a0: 7273 696f 6e91 b30b 6465 6669 6e69 7469  rsion...definiti
+000037b0: 6f6e 73b7 b307 4f62 7365 7276 65b4 b303  ons...Observe...
+000037c0: 7265 63b4 b303 6c69 74b3 074f 6273 6572  rec...lit..Obser
+000037d0: 7665 84b4 b305 7475 706c 65b5 b4b3 056e  ve....tuple....n
+000037e0: 616d 6564 b307 7061 7474 6572 6eb4 b303  amed..pattern...
+000037f0: 7265 66b5 b311 6461 7461 7370 6163 6550  ref...dataspaceP
+00003800: 6174 7465 726e 7384 b307 5061 7474 6572  atterns...Patter
+00003810: 6e84 84b4 b305 6e61 6d65 64b3 086f 6273  n.....named..obs
+00003820: 6572 7665 72b4 b308 656d 6265 6464 6564  erver...embedded
+00003830: b303 616e 7984 8484 8484 84b3 0c65 6d62  ..any........emb
+00003840: 6564 6465 6454 7970 65b4 b303 7265 66b5  eddedType...ref.
+00003850: b309 456e 7469 7479 5265 6684 b303 4361  ..EntityRef...Ca
+00003860: 7084 8484 b5b3 0a67 6174 656b 6565 7065  p......gatekeepe
+00003870: 7284 b4b3 0673 6368 656d 61b7 b307 7665  r....schema...ve
+00003880: 7273 696f 6e91 b30b 6465 6669 6e69 7469  rsion...definiti
+00003890: 6f6e 73b7 b304 4269 6e64 b4b3 0372 6563  ons...Bind...rec
+000038a0: b4b3 036c 6974 b304 6269 6e64 84b4 b305  ...lit..bind....
+000038b0: 7475 706c 65b5 b4b3 056e 616d 6564 b303  tuple....named..
+000038c0: 6f69 64b3 0361 6e79 84b4 b305 6e61 6d65  oid..any....name
+000038d0: 64b3 036b 6579 b4b3 0461 746f 6db3 0a42  d..key...atom..B
+000038e0: 7974 6553 7472 696e 6784 84b4 b305 6e61  yteString.....na
+000038f0: 6d65 64b3 0674 6172 6765 74b4 b308 656d  med..target...em
+00003900: 6265 6464 6564 b303 616e 7984 8484 8484  bedded..any.....
+00003910: b307 5265 736f 6c76 65b4 b303 7265 63b4  ..Resolve...rec.
+00003920: b303 6c69 74b3 0772 6573 6f6c 7665 84b4  ..lit..resolve..
+00003930: b305 7475 706c 65b5 b4b3 056e 616d 6564  ..tuple....named
+00003940: b309 7374 7572 6479 7265 66b4 b303 7265  ..sturdyref...re
+00003950: 66b5 b306 7374 7572 6479 84b3 0953 7475  f...sturdy...Stu
+00003960: 7264 7952 6566 8484 b4b3 056e 616d 6564  rdyRef.....named
+00003970: b308 6f62 7365 7276 6572 b4b3 0865 6d62  ..observer...emb
+00003980: 6564 6465 64b4 b308 656d 6265 6464 6564  edded...embedded
+00003990: b303 616e 7984 8484 8484 8484 b30c 656d  ..any.........em
+000039a0: 6265 6464 6564 5479 7065 b4b3 0372 6566  beddedType...ref
+000039b0: b5b3 0945 6e74 6974 7952 6566 84b3 0343  ...EntityRef...C
+000039c0: 6170 8484 84b5 b310 7472 616e 7370 6f72  ap......transpor
+000039d0: 7441 6464 7265 7373 84b4 b306 7363 6865  tAddress....sche
+000039e0: 6d61 b7b3 0776 6572 7369 6f6e 91b3 0b64  ma...version...d
+000039f0: 6566 696e 6974 696f 6e73 b7b3 0354 6370  efinitions...Tcp
+00003a00: b4b3 0372 6563 b4b3 036c 6974 b303 7463  ...rec...lit..tc
+00003a10: 7084 b4b3 0574 7570 6c65 b5b4 b305 6e61  p....tuple....na
+00003a20: 6d65 64b3 0468 6f73 74b4 b304 6174 6f6d  med..host...atom
+00003a30: b306 5374 7269 6e67 8484 b4b3 056e 616d  ..String.....nam
+00003a40: 6564 b304 706f 7274 b4b3 0461 746f 6db3  ed..port...atom.
+00003a50: 0d53 6967 6e65 6449 6e74 6567 6572 8484  .SignedInteger..
+00003a60: 8484 84b3 0455 6e69 78b4 b303 7265 63b4  .....Unix...rec.
+00003a70: b303 6c69 74b3 0475 6e69 7884 b4b3 0574  ..lit..unix....t
+00003a80: 7570 6c65 b5b4 b305 6e61 6d65 64b3 0470  uple....named..p
+00003a90: 6174 68b4 b304 6174 6f6d b306 5374 7269  ath...atom..Stri
+00003aa0: 6e67 8484 8484 84b3 0553 7464 696f b4b3  ng.......Stdio..
+00003ab0: 0372 6563 b4b3 036c 6974 b305 7374 6469  .rec...lit..stdi
+00003ac0: 6f84 b4b3 0574 7570 6c65 b584 8484 b309  o....tuple......
+00003ad0: 5765 6253 6f63 6b65 74b4 b303 7265 63b4  WebSocket...rec.
+00003ae0: b303 6c69 74b3 0277 7384 b4b3 0574 7570  ..lit..ws....tup
+00003af0: 6c65 b5b4 b305 6e61 6d65 64b3 0375 726c  le....named..url
+00003b00: b4b3 0461 746f 6db3 0653 7472 696e 6784  ...atom..String.
+00003b10: 8484 8484 84b3 0c65 6d62 6564 6465 6454  .......embeddedT
+00003b20: 7970 6580 8484 b5b3 1164 6174 6173 7061  ype......dataspa
+00003b30: 6365 5061 7474 6572 6e73 84b4 b306 7363  cePatterns....sc
+00003b40: 6865 6d61 b7b3 0776 6572 7369 6f6e 91b3  hema...version..
+00003b50: 0b64 6566 696e 6974 696f 6e73 b7b3 0444  .definitions...D
+00003b60: 4c69 74b4 b303 7265 63b4 b303 6c69 74b3  Lit...rec...lit.
+00003b70: 036c 6974 84b4 b305 7475 706c 65b5 b4b3  .lit....tuple...
+00003b80: 056e 616d 6564 b305 7661 6c75 65b4 b303  .named..value...
+00003b90: 7265 66b5 84b3 0741 6e79 4174 6f6d 8484  ref....AnyAtom..
+00003ba0: 8484 84b3 0544 4269 6e64 b4b3 0372 6563  .....DBind...rec
+00003bb0: b4b3 036c 6974 b304 6269 6e64 84b4 b305  ...lit..bind....
+00003bc0: 7475 706c 65b5 b4b3 056e 616d 6564 b307  tuple....named..
+00003bd0: 7061 7474 6572 6eb4 b303 7265 66b5 84b3  pattern...ref...
+00003be0: 0750 6174 7465 726e 8484 8484 84b3 0741  .Pattern.......A
+00003bf0: 6e79 4174 6f6d b4b3 026f 72b5 b5b1 0462  nyAtom...or....b
+00003c00: 6f6f 6cb4 b304 6174 6f6d b307 426f 6f6c  ool...atom..Bool
+00003c10: 6561 6e84 84b5 b105 666c 6f61 74b4 b304  ean.....float...
+00003c20: 6174 6f6d b305 466c 6f61 7484 84b5 b106  atom..Float.....
+00003c30: 646f 7562 6c65 b4b3 0461 746f 6db3 0644  double...atom..D
+00003c40: 6f75 626c 6584 84b5 b103 696e 74b4 b304  ouble.....int...
+00003c50: 6174 6f6d b30d 5369 676e 6564 496e 7465  atom..SignedInte
+00003c60: 6765 7284 84b5 b106 7374 7269 6e67 b4b3  ger.....string..
+00003c70: 0461 746f 6db3 0653 7472 696e 6784 84b5  .atom..String...
+00003c80: b105 6279 7465 73b4 b304 6174 6f6d b30a  ..bytes...atom..
+00003c90: 4279 7465 5374 7269 6e67 8484 b5b1 0673  ByteString.....s
+00003ca0: 796d 626f 6cb4 b304 6174 6f6d b306 5379  ymbol...atom..Sy
+00003cb0: 6d62 6f6c 8484 b5b1 0865 6d62 6564 6465  mbol.....embedde
+00003cc0: 64b4 b308 656d 6265 6464 6564 b303 616e  d...embedded..an
+00003cd0: 7984 8484 84b3 0750 6174 7465 726e b4b3  y......Pattern..
+00003ce0: 026f 72b5 b5b1 0844 4469 7363 6172 64b4  .or....DDiscard.
+00003cf0: b303 7265 66b5 84b3 0844 4469 7363 6172  ..ref....DDiscar
+00003d00: 6484 84b5 b105 4442 696e 64b4 b303 7265  d.....DBind...re
+00003d10: 66b5 84b3 0544 4269 6e64 8484 b5b1 0444  f....DBind.....D
+00003d20: 4c69 74b4 b303 7265 66b5 84b3 0444 4c69  Lit...ref....DLi
+00003d30: 7484 84b5 b109 4443 6f6d 706f 756e 64b4  t.....DCompound.
+00003d40: b303 7265 66b5 84b3 0944 436f 6d70 6f75  ..ref....DCompou
+00003d50: 6e64 8484 8484 b308 4444 6973 6361 7264  nd......DDiscard
+00003d60: b4b3 0372 6563 b4b3 036c 6974 b301 5f84  ...rec...lit.._.
+00003d70: b4b3 0574 7570 6c65 b584 8484 b309 4443  ...tuple......DC
+00003d80: 6f6d 706f 756e 64b4 b302 6f72 b5b5 b103  ompound...or....
+00003d90: 7265 63b4 b303 7265 63b4 b303 6c69 74b3  rec...rec...lit.
+00003da0: 0372 6563 84b4 b305 7475 706c 65b5 b4b3  .rec....tuple...
+00003db0: 056e 616d 6564 b305 6c61 6265 6cb3 0361  .named..label..a
+00003dc0: 6e79 84b4 b305 6e61 6d65 64b3 0666 6965  ny....named..fie
+00003dd0: 6c64 73b4 b305 7365 716f 66b4 b303 7265  lds...seqof...re
+00003de0: 66b5 84b3 0750 6174 7465 726e 8484 8484  f....Pattern....
+00003df0: 8484 84b5 b103 6172 72b4 b303 7265 63b4  ......arr...rec.
+00003e00: b303 6c69 74b3 0361 7272 84b4 b305 7475  ..lit..arr....tu
+00003e10: 706c 65b5 b4b3 056e 616d 6564 b305 6974  ple....named..it
+00003e20: 656d 73b4 b305 7365 716f 66b4 b303 7265  ems...seqof...re
+00003e30: 66b5 84b3 0750 6174 7465 726e 8484 8484  f....Pattern....
+00003e40: 8484 84b5 b104 6469 6374 b4b3 0372 6563  ......dict...rec
+00003e50: b4b3 036c 6974 b304 6469 6374 84b4 b305  ...lit..dict....
+00003e60: 7475 706c 65b5 b4b3 056e 616d 6564 b307  tuple....named..
+00003e70: 656e 7472 6965 73b4 b306 6469 6374 6f66  entries...dictof
+00003e80: b303 616e 79b4 b303 7265 66b5 84b3 0750  ..any...ref....P
+00003e90: 6174 7465 726e 8484 8484 8484 8484 8484  attern..........
+00003ea0: b30c 656d 6265 6464 6564 5479 7065 b4b3  ..embeddedType..
+00003eb0: 0372 6566 b5b3 0945 6e74 6974 7952 6566  .ref...EntityRef
+00003ec0: 84b3 0343 6170 8484 8484 84              ...Cap.....
```

### Comparing `syndicate-py-0.8.5/syndicate/protocols/schemas/dataspacePatterns.prs` & `syndicate-py-0.9.0/syndicate/protocols/schemas/dataspacePatterns.prs`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate/protocols/schemas/service.prs` & `syndicate-py-0.9.0/syndicate/protocols/schemas/service.prs`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate/protocols/schemas/stream.prs` & `syndicate-py-0.9.0/syndicate/protocols/schemas/stream.prs`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate/protocols/schemas/sturdy.prs` & `syndicate-py-0.9.0/syndicate/protocols/schemas/sturdy.prs`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 version 1 .
 embeddedType EntityRef.Cap .
 
-; Each Attenuation is a stage. The sequence of Attenuations is run RIGHT-TO-LEFT.
-; That is, the newest Attenuations are at the right.
-SturdyRef = <ref @oid any @caveatChain [Attenuation ...] @sig bytes>.
-
-; An individual Attenuation is run RIGHT-TO-LEFT.
+; The sequence of Caveats is run RIGHT-TO-LEFT.
 ; That is, the newest Caveats are at the right.
-Attenuation = [Caveat ...].
+;
+; Let f = HMAC-BLAKE2s, e = canonical machine-oriented serialization of some preserves value,
+; and k = the original secret key for the ref.
+;
+; The `sig` is then f(f(f(f(k, e(oid)), ...), Caveat), ...).
+;
+SturdyRef = <ref @oid any @caveatChain [Caveat ...] @sig bytes>.
 
 ; embodies 1st-party caveats over assertion structure, but nothing else
 ; can add 3rd-party caveats and richer predicates later
-Caveat = Rewrite / Alts .
-Rewrite = <rewrite @pattern Pattern @template Template>.
+Caveat = Rewrite / Alts / Reject /@unknown any .
+Rewrite = <rewrite @pattern Pattern @template Template> .
+Reject = <reject @pattern Pattern> .
 Alts = <or @alternatives [Rewrite ...]>.
 
 Oid = int .
 WireRef = @mine [0 @oid Oid] / @yours [1 @oid Oid @attenuation Caveat ...].
 
 ;---------------------------------------------------------------------------
 
@@ -31,13 +34,13 @@
 PNot = <not @pattern Pattern>.
 PCompound =
     / @rec <rec @label any @fields [Pattern ...]>
     / @arr <arr @items [Pattern ...]>
     / @dict <dict @entries { any: Pattern ...:... }> .
 
 Template = TAttenuate / TRef / Lit / TCompound .
-TAttenuate = <attenuate @template Template @attenuation Attenuation>.
+TAttenuate = <attenuate @template Template @attenuation [Caveat ...]>.
 TRef = <ref @binding int>.
 TCompound =
     / @rec <rec @label any @fields [Template ...]>
     / @arr <arr @items [Template ...]>
     / @dict <dict @entries { any: Template ...:... }> .
```

### Comparing `syndicate-py-0.8.5/syndicate/protocols/schemas/trace.prs` & `syndicate-py-0.9.0/syndicate/protocols/schemas/trace.prs`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate/relay.py` & `syndicate-py-0.9.0/syndicate/relay.py`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate/transport.py` & `syndicate-py-0.9.0/syndicate/transport.py`

 * *Files identical despite different names*

### Comparing `syndicate-py-0.8.5/syndicate_py.egg-info/PKG-INFO` & `syndicate-py-0.9.0/syndicate_py.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syndicate-py
-Version: 0.8.5
+Version: 0.9.0
 Summary: Syndicated Actor model and Syndicate network protocol for Python 3
 Home-page: https://git.syndicate-lang.org/syndicate-lang/syndicate-py
 Author: Tony Garnock-Jones
 Author-email: tonyg@leastfixedpoint.com
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `syndicate-py-0.8.5/syndicate_py.egg-info/SOURCES.txt` & `syndicate-py-0.9.0/syndicate_py.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .envrc
 .gitignore
 Makefile
 README.md
 bidi-gc.py
+chat.bin
+chat.prs
 chat.py
 inf.py
 requirements.txt
 setup.py
 syndicate/__init__.py
 syndicate/actor.py
 syndicate/dataflow.py
@@ -21,19 +23,18 @@
 syndicate/schema.py
 syndicate/transport.py
 syndicate/protocols/Makefile
 syndicate/protocols/schema-bundle.bin
 syndicate/protocols/schemas/dataspace.prs
 syndicate/protocols/schemas/dataspacePatterns.prs
 syndicate/protocols/schemas/gatekeeper.prs
+syndicate/protocols/schemas/http.prs
+syndicate/protocols/schemas/noise.prs
 syndicate/protocols/schemas/protocol.prs
-syndicate/protocols/schemas/racketEvent.prs
-syndicate/protocols/schemas/secureChatProtocol.prs
 syndicate/protocols/schemas/service.prs
-syndicate/protocols/schemas/simpleChatProtocol.prs
 syndicate/protocols/schemas/stream.prs
 syndicate/protocols/schemas/sturdy.prs
 syndicate/protocols/schemas/tcp.prs
 syndicate/protocols/schemas/timer.prs
 syndicate/protocols/schemas/trace.prs
 syndicate/protocols/schemas/transportAddress.prs
 syndicate/protocols/schemas/worker.prs
```

