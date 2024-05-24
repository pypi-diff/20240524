# Comparing `tmp/rembg-2.0.56.tar.gz` & `tmp/rembg-2.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.56.tar", last modified: Tue Mar 12 22:54:56 2024, max compression
+gzip compressed data, was "rembg-2.0.57.tar", last modified: Fri May 24 00:30:31 2024, max compression
```

## Comparing `rembg-2.0.56.tar` & `rembg-2.0.57.tar`

### file list

```diff
@@ -1,43 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 22:54:56.436858 rembg-2.0.56/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-12 22:53:55.000000 rembg-2.0.56/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-12 22:53:55.000000 rembg-2.0.56/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14024 2024-03-12 22:54:56.436858 rembg-2.0.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-03-12 22:53:55.000000 rembg-2.0.56/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-12 22:53:55.000000 rembg-2.0.56/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 22:54:56.436858 rembg-2.0.56/rembg/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-12 22:54:56.436858 rembg-2.0.56/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 22:54:56.432858 rembg-2.0.56/rembg/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/commands/b_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/commands/d_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/commands/i_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/commands/p_command.py
--rw-r--r--   0 runner    (1001) docker     (127)    10477 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/commands/s_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/session_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 22:54:56.436858 rembg-2.0.56/rembg/sessions/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/sessions/dis_anime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/sessions/dis_general_use.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/sessions/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/sessions/silueta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/sessions/u2net.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/sessions/u2net_cloth_seg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/sessions/u2net_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/sessions/u2net_human_seg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-12 22:53:55.000000 rembg-2.0.56/rembg/sessions/u2netp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 22:54:56.432858 rembg-2.0.56/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14024 2024-03-12 22:54:56.000000 rembg-2.0.56/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-12 22:54:56.000000 rembg-2.0.56/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 22:54:56.000000 rembg-2.0.56/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-12 22:54:56.000000 rembg-2.0.56/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-12 22:54:56.000000 rembg-2.0.56/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-12 22:54:56.000000 rembg-2.0.56/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-12 22:54:56.436858 rembg-2.0.56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-12 22:53:55.000000 rembg-2.0.56/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 22:54:56.436858 rembg-2.0.56/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-12 22:53:55.000000 rembg-2.0.56/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-03-12 22:53:55.000000 rembg-2.0.56/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:30:31.602099 rembg-2.0.57/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-24 00:29:40.000000 rembg-2.0.57/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-24 00:29:40.000000 rembg-2.0.57/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-05-24 00:30:31.602099 rembg-2.0.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-05-24 00:29:40.000000 rembg-2.0.57/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-24 00:29:40.000000 rembg-2.0.57/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:30:31.606099 rembg-2.0.57/rembg/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-24 00:30:31.606099 rembg-2.0.57/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10395 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:30:31.602099 rembg-2.0.57/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/commands/b_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/commands/d_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10477 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:30:31.602099 rembg-2.0.57/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/sessions/dis_anime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/sessions/dis_general_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/sessions/u2net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-24 00:29:40.000000 rembg-2.0.57/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:30:31.602099 rembg-2.0.57/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-05-24 00:30:31.000000 rembg-2.0.57/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-24 00:30:31.000000 rembg-2.0.57/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 00:30:31.000000 rembg-2.0.57/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-24 00:30:31.000000 rembg-2.0.57/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 00:30:31.000000 rembg-2.0.57/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 00:30:31.000000 rembg-2.0.57/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-24 00:30:31.606099 rembg-2.0.57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-24 00:29:40.000000 rembg-2.0.57/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-05-24 00:29:40.000000 rembg-2.0.57/versioneer.py
```

### Comparing `rembg-2.0.56/LICENSE.txt` & `rembg-2.0.57/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.56/PKG-INFO` & `rembg-2.0.57/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.56
+Version: 2.0.57
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
+License: UNKNOWN
 Keywords: remove,background,u2net
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -18,63 +20,62 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <3.13
 Description-Content-Type: text/markdown
+Provides-Extra: cli
 Provides-Extra: dev
 Provides-Extra: gpu
-Provides-Extra: cli
 License-File: LICENSE.txt
 
 # Rembg
 
 [![Downloads](https://img.shields.io/pypi/dm/rembg.svg)](https://img.shields.io/pypi/dm/rembg.svg)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://img.shields.io/badge/License-MIT-blue.svg)
 [![Hugging Face Spaces](https://img.shields.io/badge/🤗%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/KenjieDec/RemBG)
 [![Streamlit App](https://img.shields.io/badge/🎈%20Streamlit%20Community-Cloud-blue)](https://bgremoval.streamlit.app/)
 
-
 Rembg is a tool to remove images background.
 
 <p style="display: flex;align-items: center;justify-content: center;">
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-1.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-1.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-2.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-2.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-3.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-3.out.png" width="100" />
+  <img alt="example car-1" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-1.jpg" width="100" />
+  <img alt="example car-1.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-1.out.png" width="100" />
+  <img alt="example car-2" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-2.jpg" width="100" />
+  <img alt="example car-2.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-2.out.png" width="100" />
+  <img alt="example car-3" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-3.jpg" width="100" />
+  <img alt="example car-3.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-3.out.png" width="100" />
 </p>
 
 <p style="display: flex;align-items: center;justify-content: center;">
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-1.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-1.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-2.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-2.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-3.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-3.out.png" width="100" />
+  <img alt="example animal-1" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-1.jpg" width="100" />
+  <img alt="example animal-1.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-1.out.png" width="100" />
+  <img alt="example animal-2" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-2.jpg" width="100" />
+  <img alt="example animal-2.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-2.out.png" width="100" />
+  <img alt="example animal-3" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-3.jpg" width="100" />
+  <img alt="example animal-3.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-3.out.png" width="100" />
 </p>
 
 <p style="display: flex;align-items: center;justify-content: center;">
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-1.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-1.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-2.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-2.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-3.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-3.out.png" width="100" />
+  <img alt="example girl-1" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-1.jpg" width="100" />
+  <img alt="example girl-1.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-1.out.png" width="100" />
+  <img alt="example girl-2" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-2.jpg" width="100" />
+  <img alt="example girl-2.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-2.out.png" width="100" />
+  <img alt="example girl-3" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-3.jpg" width="100" />
+  <img alt="example girl-3.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-3.out.png" width="100" />
 </p>
 
 <p style="display: flex;align-items: center;justify-content: center;">
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-1.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-1.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-2.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-2.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-3.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-3.out.png" width="100" />
+  <img alt="example anime-girl-1" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-1.jpg" width="100" />
+  <img alt="example anime-girl-1.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-1.out.png" width="100" />
+  <img alt="example anime-girl-2" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-2.jpg" width="100" />
+  <img alt="example anime-girl-2.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-2.out.png" width="100" />
+  <img alt="example anime-girl-3" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-3.jpg" width="100" />
+  <img alt="example anime-girl-3.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-3.out.png" width="100" />
 </p>
 
 **If this project has helped you, please consider making a [donation](https://www.buymeacoffee.com/danielgatis).**
 
 ## Sponsor
 
 <table>
@@ -94,15 +95,15 @@
       </p>
     </td>
   </tr>
 </table>
 
 ## Requirements
 
-```
+```text
 python: >3.7, <3.13
 ```
 
 ## Installation
 
 CPU support:
 
@@ -111,159 +112,158 @@
 pip install rembg[cli] # for library + cli
 ```
 
 GPU support:
 
 First of all, you need to check if your system supports the `onnxruntime-gpu`.
 
-Go to https://onnxruntime.ai and check the installation matrix.
+Go to <https://onnxruntime.ai> and check the installation matrix.
 
 <p style="display: flex;align-items: center;justify-content: center;">
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/onnxruntime-installation-matrix.png" width="400" />
+  <img alt="onnxruntime-installation-matrix" src="https://raw.githubusercontent.com/danielgatis/rembg/master/onnxruntime-installation-matrix.png" width="400" />
 </p>
 
 If yes, just run:
 
 ```bash
 pip install rembg[gpu] # for library
 pip install rembg[gpu,cli] # for library + cli
 ```
 
 ## Usage as a cli
 
 After the installation step you can use rembg just typing `rembg` in your terminal window.
 
 The `rembg` command has 4 subcommands, one for each input type:
+
 - `i` for files
 - `p` for folders
 - `s` for http server
 - `b` for RGB24 pixel binary stream
 
 You can get help about the main command using:
 
-```
+```shell
 rembg --help
 ```
 
 As well, about all the subcommands using:
 
-```
+```shell
 rembg <COMMAND> --help
 ```
 
 ### rembg `i`
 
 Used when input and output are files.
 
 Remove the background from a remote image
 
-```
+```shell
 curl -s http://input.png | rembg i > output.png
 ```
 
 Remove the background from a local file
 
-```
+```shell
 rembg i path/to/input.png path/to/output.png
 ```
 
 Remove the background specifying a model
 
-```
+```shell
 rembg i -m u2netp path/to/input.png path/to/output.png
 ```
 
 Remove the background returning only the mask
 
-```
+```shell
 rembg i -om path/to/input.png path/to/output.png
 ```
 
-
 Remove the background applying an alpha matting
 
-```
+```shell
 rembg i -a path/to/input.png path/to/output.png
 ```
 
 Passing extras parameters
 
-```
+```shell
 SAM example
 
 rembg i -m sam -x '{ "sam_prompt": [{"type": "point", "data": [724, 740], "label": 1}] }' examples/plants-1.jpg examples/plants-1.out.png
 ```
 
-```
+```shell
 Custom model example
 
 rembg i -m u2net_custom -x '{"model_path": "~/.u2net/u2net.onnx"}' path/to/input.png path/to/output.png
 ```
 
 ### rembg `p`
 
 Used when input and output are folders.
 
 Remove the background from all images in a folder
 
-```
+```shell
 rembg p path/to/input path/to/output
 ```
 
 Same as before, but watching for new/changed files to process
 
-```
+```shell
 rembg p -w path/to/input path/to/output
 ```
 
 ### rembg `s`
 
 Used to start http server.
 
-```
+```shell
 rembg s --host 0.0.0.0 --port 7000 --log_level info
 ```
 
 To see the complete endpoints documentation, go to: `http://localhost:7000/api`.
 
 Remove the background from an image url
 
-```
+```shell
 curl -s "http://localhost:7000/api/remove?url=http://input.png" -o output.png
 ```
 
 Remove the background from an uploaded image
 
-```
+```shell
 curl -s -F file=@/path/to/input.jpg "http://localhost:7000/api/remove"  -o output.png
 ```
 
 ### rembg `b`
 
 Process a sequence of RGB24 images from stdin. This is intended to be used with another program, such as FFMPEG, that outputs RGB24 pixel data to stdout, which is piped into the stdin of this program, although nothing prevents you from manually typing in images at stdin.
 
-```
+```shell
 rembg b image_width image_height -o output_specifier
 ```
 
 Arguments:
 
 - image_width : width of input image(s)
 - image_height : height of input image(s)
 - output_specifier: printf-style specifier for output filenames, for example if `output-%03u.png`, then output files will be named `output-000.png`, `output-001.png`, `output-002.png`, etc. Output files will be saved in PNG format regardless of the extension specified. You can omit it to write results to stdout.
 
 Example usage with FFMPEG:
 
-```
+```shell
 ffmpeg -i input.mp4 -ss 10 -an -f rawvideo -pix_fmt rgb24 pipe:1 | rembg b 1280 720 -o folder/output-%03u.png
 ```
 
 The width and height values must match the dimension of output images from FFMPEG. Note for FFMPEG, the "`-an -f rawvideo -pix_fmt rgb24 pipe:1`" part is required for the whole thing to work.
 
-
 ## Usage as a library
 
 Input and output as bytes
 
 ```python
 from rembg import remove
 
@@ -319,69 +319,76 @@
 
     with open(input_path, 'rb') as i:
         with open(output_path, 'wb') as o:
             input = i.read()
             output = remove(input, session=session)
             o.write(output)
 ```
+
 To see a full list of examples on how to use rembg, go to the [examples](USAGE.md) page.
+
 ## Usage as a docker
 
 Just replace the `rembg` command for `docker run danielgatis/rembg`.
 
 Try this:
 
-```
+```shell
 docker run -v path/to/input:/rembg danielgatis/rembg i input.png path/to/output/output.png
 ```
 
 ## Models
 
 All models are downloaded and saved in the user home folder in the `.u2net` directory.
 
 The available models are:
 
--   u2net ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use cases.
--   u2netp ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A lightweight version of u2net model.
--   u2net_human_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human segmentation.
--   u2net_cloth_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths Parsing from human portrait. Here clothes are parsed into 3 category: Upper body, Lower body and Full body.
--   silueta ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is reduced to 43Mb.
--   isnet-general-use ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-trained model for general use cases.
--   isnet-anime ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-anime.onnx), [source](https://github.com/SkyTNT/anime-segmentation)): A high-accuracy segmentation for anime character.
--   sam ([download encoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A pre-trained model for any use cases.
+- u2net ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use cases.
+- u2netp ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A lightweight version of u2net model.
+- u2net_human_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human segmentation.
+- u2net_cloth_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths Parsing from human portrait. Here clothes are parsed into 3 category: Upper body, Lower body and Full body.
+- silueta ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is reduced to 43Mb.
+- isnet-general-use ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-trained model for general use cases.
+- isnet-anime ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-anime.onnx), [source](https://github.com/SkyTNT/anime-segmentation)): A high-accuracy segmentation for anime character.
+- sam ([download encoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A pre-trained model for any use cases.
 
 ### How to train your own model
 
 If You need more fine tuned models try this:
-https://github.com/danielgatis/rembg/issues/193#issuecomment-1055534289
-
+<https://github.com/danielgatis/rembg/issues/193#issuecomment-1055534289>
 
 ## Some video tutorials
 
-- https://www.youtube.com/watch?v=3xqwpXjxyMQ
-- https://www.youtube.com/watch?v=dFKRGXdkGJU
-- https://www.youtube.com/watch?v=Ai-BS_T7yjE
-- https://www.youtube.com/watch?v=D7W-C0urVcQ
+- <https://www.youtube.com/watch?v=3xqwpXjxyMQ>
+- <https://www.youtube.com/watch?v=dFKRGXdkGJU>
+- <https://www.youtube.com/watch?v=Ai-BS_T7yjE>
+- <https://www.youtube.com/watch?v=D7W-C0urVcQ>
 
 ## References
 
-- https://arxiv.org/pdf/2005.09007.pdf
-- https://github.com/NathanUA/U-2-Net
-- https://github.com/pymatting/pymatting
+- <https://arxiv.org/pdf/2005.09007.pdf>
+- <https://github.com/NathanUA/U-2-Net>
+- <https://github.com/pymatting/pymatting>
 
 ## FAQ
 
 ### When will this library provide support for Python version 3.xx?
 
 This library directly depends on the [onnxruntime](https://pypi.org/project/onnxruntime) library. Therefore, we can only update the Python version when [onnxruntime](https://pypi.org/project/onnxruntime) provides support for that specific version.
 
 ## Buy me a coffee
 
 Liked some of my work? Buy me a coffee (or more likely a beer)
 
-<a href="https://www.buymeacoffee.com/danielgatis" target="_blank"><img src="https://bmc-cdn.nyc3.digitaloceanspaces.com/BMC-button-images/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;"></a>
+<a href="https://www.buymeacoffee.com/danielgatis" target="_blank"><img src="https://bmc-cdn.nyc3.digitaloceanspaces.com/BMC-button-images/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;"></a> <!-- markdownlint-disable MD033 -->
+
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=danielgatis/rembg&type=Date)](https://star-history.com/#danielgatis/rembg&Date)
 
 ## License
 
 Copyright (c) 2020-present [Daniel Gatis](https://github.com/danielgatis)
 
 Licensed under [MIT License](./LICENSE.txt)
+
+
```

### Comparing `rembg-2.0.56/README.md` & `rembg-2.0.57/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,784 +24,841 @@
 00000170: 6c69 7420 4170 705d 2868 7474 7073 3a2f  lit App](https:/
 00000180: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
 00000190: 6261 6467 652f f09f 8e88 2532 3053 7472  badge/....%20Str
 000001a0: 6561 6d6c 6974 2532 3043 6f6d 6d75 6e69  eamlit%20Communi
 000001b0: 7479 2d43 6c6f 7564 2d62 6c75 6529 5d28  ty-Cloud-blue)](
 000001c0: 6874 7470 733a 2f2f 6267 7265 6d6f 7661  https://bgremova
 000001d0: 6c2e 7374 7265 616d 6c69 742e 6170 702f  l.streamlit.app/
-000001e0: 290a 0a0a 5265 6d62 6720 6973 2061 2074  )...Rembg is a t
-000001f0: 6f6f 6c20 746f 2072 656d 6f76 6520 696d  ool to remove im
-00000200: 6167 6573 2062 6163 6b67 726f 756e 642e  ages background.
-00000210: 0a0a 3c70 2073 7479 6c65 3d22 6469 7370  ..<p style="disp
-00000220: 6c61 793a 2066 6c65 783b 616c 6967 6e2d  lay: flex;align-
-00000230: 6974 656d 733a 2063 656e 7465 723b 6a75  items: center;ju
-00000240: 7374 6966 792d 636f 6e74 656e 743a 2063  stify-content: c
-00000250: 656e 7465 723b 223e 0a20 203c 696d 6720  enter;">.  <img 
-00000260: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00000270: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000280: 6e74 2e63 6f6d 2f64 616e 6965 6c67 6174  nt.com/danielgat
-00000290: 6973 2f72 656d 6267 2f6d 6173 7465 722f  is/rembg/master/
-000002a0: 6578 616d 706c 6573 2f63 6172 2d31 2e6a  examples/car-1.j
-000002b0: 7067 2220 7769 6474 683d 2231 3030 2220  pg" width="100" 
-000002c0: 2f3e 0a20 203c 696d 6720 7372 633d 2268  />.  <img src="h
-000002d0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-000002e0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-000002f0: 2f64 616e 6965 6c67 6174 6973 2f72 656d  /danielgatis/rem
-00000300: 6267 2f6d 6173 7465 722f 6578 616d 706c  bg/master/exampl
-00000310: 6573 2f63 6172 2d31 2e6f 7574 2e70 6e67  es/car-1.out.png
-00000320: 2220 7769 6474 683d 2231 3030 2220 2f3e  " width="100" />
-00000330: 0a20 203c 696d 6720 7372 633d 2268 7474  .  <img src="htt
-00000340: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00000350: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f64  sercontent.com/d
-00000360: 616e 6965 6c67 6174 6973 2f72 656d 6267  anielgatis/rembg
-00000370: 2f6d 6173 7465 722f 6578 616d 706c 6573  /master/examples
-00000380: 2f63 6172 2d32 2e6a 7067 2220 7769 6474  /car-2.jpg" widt
-00000390: 683d 2231 3030 2220 2f3e 0a20 203c 696d  h="100" />.  <im
-000003a0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-000003b0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-000003c0: 7465 6e74 2e63 6f6d 2f64 616e 6965 6c67  tent.com/danielg
-000003d0: 6174 6973 2f72 656d 6267 2f6d 6173 7465  atis/rembg/maste
-000003e0: 722f 6578 616d 706c 6573 2f63 6172 2d32  r/examples/car-2
-000003f0: 2e6f 7574 2e70 6e67 2220 7769 6474 683d  .out.png" width=
-00000400: 2231 3030 2220 2f3e 0a20 203c 696d 6720  "100" />.  <img 
-00000410: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00000420: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000430: 6e74 2e63 6f6d 2f64 616e 6965 6c67 6174  nt.com/danielgat
-00000440: 6973 2f72 656d 6267 2f6d 6173 7465 722f  is/rembg/master/
-00000450: 6578 616d 706c 6573 2f63 6172 2d33 2e6a  examples/car-3.j
-00000460: 7067 2220 7769 6474 683d 2231 3030 2220  pg" width="100" 
-00000470: 2f3e 0a20 203c 696d 6720 7372 633d 2268  />.  <img src="h
-00000480: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00000490: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-000004a0: 2f64 616e 6965 6c67 6174 6973 2f72 656d  /danielgatis/rem
-000004b0: 6267 2f6d 6173 7465 722f 6578 616d 706c  bg/master/exampl
-000004c0: 6573 2f63 6172 2d33 2e6f 7574 2e70 6e67  es/car-3.out.png
-000004d0: 2220 7769 6474 683d 2231 3030 2220 2f3e  " width="100" />
-000004e0: 0a3c 2f70 3e0a 0a3c 7020 7374 796c 653d  .</p>..<p style=
-000004f0: 2264 6973 706c 6179 3a20 666c 6578 3b61  "display: flex;a
-00000500: 6c69 676e 2d69 7465 6d73 3a20 6365 6e74  lign-items: cent
-00000510: 6572 3b6a 7573 7469 6679 2d63 6f6e 7465  er;justify-conte
-00000520: 6e74 3a20 6365 6e74 6572 3b22 3e0a 2020  nt: center;">.  
-00000530: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000540: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00000550: 636f 6e74 656e 742e 636f 6d2f 6461 6e69  content.com/dani
-00000560: 656c 6761 7469 732f 7265 6d62 672f 6d61  elgatis/rembg/ma
-00000570: 7374 6572 2f65 7861 6d70 6c65 732f 616e  ster/examples/an
-00000580: 696d 616c 2d31 2e6a 7067 2220 7769 6474  imal-1.jpg" widt
-00000590: 683d 2231 3030 2220 2f3e 0a20 203c 696d  h="100" />.  <im
-000005a0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-000005b0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-000005c0: 7465 6e74 2e63 6f6d 2f64 616e 6965 6c67  tent.com/danielg
-000005d0: 6174 6973 2f72 656d 6267 2f6d 6173 7465  atis/rembg/maste
-000005e0: 722f 6578 616d 706c 6573 2f61 6e69 6d61  r/examples/anima
-000005f0: 6c2d 312e 6f75 742e 706e 6722 2077 6964  l-1.out.png" wid
-00000600: 7468 3d22 3130 3022 202f 3e0a 2020 3c69  th="100" />.  <i
-00000610: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000620: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00000630: 6e74 656e 742e 636f 6d2f 6461 6e69 656c  ntent.com/daniel
-00000640: 6761 7469 732f 7265 6d62 672f 6d61 7374  gatis/rembg/mast
-00000650: 6572 2f65 7861 6d70 6c65 732f 616e 696d  er/examples/anim
-00000660: 616c 2d32 2e6a 7067 2220 7769 6474 683d  al-2.jpg" width=
-00000670: 2231 3030 2220 2f3e 0a20 203c 696d 6720  "100" />.  <img 
-00000680: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00000690: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-000006a0: 6e74 2e63 6f6d 2f64 616e 6965 6c67 6174  nt.com/danielgat
-000006b0: 6973 2f72 656d 6267 2f6d 6173 7465 722f  is/rembg/master/
-000006c0: 6578 616d 706c 6573 2f61 6e69 6d61 6c2d  examples/animal-
-000006d0: 322e 6f75 742e 706e 6722 2077 6964 7468  2.out.png" width
-000006e0: 3d22 3130 3022 202f 3e0a 2020 3c69 6d67  ="100" />.  <img
-000006f0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00000700: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000710: 656e 742e 636f 6d2f 6461 6e69 656c 6761  ent.com/danielga
-00000720: 7469 732f 7265 6d62 672f 6d61 7374 6572  tis/rembg/master
-00000730: 2f65 7861 6d70 6c65 732f 616e 696d 616c  /examples/animal
-00000740: 2d33 2e6a 7067 2220 7769 6474 683d 2231  -3.jpg" width="1
-00000750: 3030 2220 2f3e 0a20 203c 696d 6720 7372  00" />.  <img sr
-00000760: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
-00000770: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00000780: 2e63 6f6d 2f64 616e 6965 6c67 6174 6973  .com/danielgatis
-00000790: 2f72 656d 6267 2f6d 6173 7465 722f 6578  /rembg/master/ex
-000007a0: 616d 706c 6573 2f61 6e69 6d61 6c2d 332e  amples/animal-3.
-000007b0: 6f75 742e 706e 6722 2077 6964 7468 3d22  out.png" width="
-000007c0: 3130 3022 202f 3e0a 3c2f 703e 0a0a 3c70  100" />.</p>..<p
-000007d0: 2073 7479 6c65 3d22 6469 7370 6c61 793a   style="display:
-000007e0: 2066 6c65 783b 616c 6967 6e2d 6974 656d   flex;align-item
-000007f0: 733a 2063 656e 7465 723b 6a75 7374 6966  s: center;justif
-00000800: 792d 636f 6e74 656e 743a 2063 656e 7465  y-content: cente
-00000810: 723b 223e 0a20 203c 696d 6720 7372 633d  r;">.  <img src=
-00000820: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00000830: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000840: 6f6d 2f64 616e 6965 6c67 6174 6973 2f72  om/danielgatis/r
-00000850: 656d 6267 2f6d 6173 7465 722f 6578 616d  embg/master/exam
-00000860: 706c 6573 2f67 6972 6c2d 312e 6a70 6722  ples/girl-1.jpg"
-00000870: 2077 6964 7468 3d22 3130 3022 202f 3e0a   width="100" />.
-00000880: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000890: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-000008a0: 6572 636f 6e74 656e 742e 636f 6d2f 6461  ercontent.com/da
-000008b0: 6e69 656c 6761 7469 732f 7265 6d62 672f  nielgatis/rembg/
-000008c0: 6d61 7374 6572 2f65 7861 6d70 6c65 732f  master/examples/
-000008d0: 6769 726c 2d31 2e6f 7574 2e70 6e67 2220  girl-1.out.png" 
-000008e0: 7769 6474 683d 2231 3030 2220 2f3e 0a20  width="100" />. 
-000008f0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000900: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00000910: 7263 6f6e 7465 6e74 2e63 6f6d 2f64 616e  rcontent.com/dan
-00000920: 6965 6c67 6174 6973 2f72 656d 6267 2f6d  ielgatis/rembg/m
-00000930: 6173 7465 722f 6578 616d 706c 6573 2f67  aster/examples/g
-00000940: 6972 6c2d 322e 6a70 6722 2077 6964 7468  irl-2.jpg" width
-00000950: 3d22 3130 3022 202f 3e0a 2020 3c69 6d67  ="100" />.  <img
-00000960: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00000970: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000980: 656e 742e 636f 6d2f 6461 6e69 656c 6761  ent.com/danielga
-00000990: 7469 732f 7265 6d62 672f 6d61 7374 6572  tis/rembg/master
-000009a0: 2f65 7861 6d70 6c65 732f 6769 726c 2d32  /examples/girl-2
-000009b0: 2e6f 7574 2e70 6e67 2220 7769 6474 683d  .out.png" width=
-000009c0: 2231 3030 2220 2f3e 0a20 203c 696d 6720  "100" />.  <img 
-000009d0: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-000009e0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-000009f0: 6e74 2e63 6f6d 2f64 616e 6965 6c67 6174  nt.com/danielgat
-00000a00: 6973 2f72 656d 6267 2f6d 6173 7465 722f  is/rembg/master/
-00000a10: 6578 616d 706c 6573 2f67 6972 6c2d 332e  examples/girl-3.
-00000a20: 6a70 6722 2077 6964 7468 3d22 3130 3022  jpg" width="100"
-00000a30: 202f 3e0a 2020 3c69 6d67 2073 7263 3d22   />.  <img src="
-00000a40: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00000a50: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00000a60: 6d2f 6461 6e69 656c 6761 7469 732f 7265  m/danielgatis/re
-00000a70: 6d62 672f 6d61 7374 6572 2f65 7861 6d70  mbg/master/examp
-00000a80: 6c65 732f 6769 726c 2d33 2e6f 7574 2e70  les/girl-3.out.p
-00000a90: 6e67 2220 7769 6474 683d 2231 3030 2220  ng" width="100" 
-00000aa0: 2f3e 0a3c 2f70 3e0a 0a3c 7020 7374 796c  />.</p>..<p styl
-00000ab0: 653d 2264 6973 706c 6179 3a20 666c 6578  e="display: flex
-00000ac0: 3b61 6c69 676e 2d69 7465 6d73 3a20 6365  ;align-items: ce
-00000ad0: 6e74 6572 3b6a 7573 7469 6679 2d63 6f6e  nter;justify-con
-00000ae0: 7465 6e74 3a20 6365 6e74 6572 3b22 3e0a  tent: center;">.
-00000af0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000b00: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00000b10: 6572 636f 6e74 656e 742e 636f 6d2f 6461  ercontent.com/da
-00000b20: 6e69 656c 6761 7469 732f 7265 6d62 672f  nielgatis/rembg/
-00000b30: 6d61 7374 6572 2f65 7861 6d70 6c65 732f  master/examples/
-00000b40: 616e 696d 652d 6769 726c 2d31 2e6a 7067  anime-girl-1.jpg
-00000b50: 2220 7769 6474 683d 2231 3030 2220 2f3e  " width="100" />
-00000b60: 0a20 203c 696d 6720 7372 633d 2268 7474  .  <img src="htt
-00000b70: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00000b80: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f64  sercontent.com/d
-00000b90: 616e 6965 6c67 6174 6973 2f72 656d 6267  anielgatis/rembg
-00000ba0: 2f6d 6173 7465 722f 6578 616d 706c 6573  /master/examples
-00000bb0: 2f61 6e69 6d65 2d67 6972 6c2d 312e 6f75  /anime-girl-1.ou
-00000bc0: 742e 706e 6722 2077 6964 7468 3d22 3130  t.png" width="10
-00000bd0: 3022 202f 3e0a 2020 3c69 6d67 2073 7263  0" />.  <img src
-00000be0: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00000bf0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00000c00: 636f 6d2f 6461 6e69 656c 6761 7469 732f  com/danielgatis/
-00000c10: 7265 6d62 672f 6d61 7374 6572 2f65 7861  rembg/master/exa
-00000c20: 6d70 6c65 732f 616e 696d 652d 6769 726c  mples/anime-girl
-00000c30: 2d32 2e6a 7067 2220 7769 6474 683d 2231  -2.jpg" width="1
-00000c40: 3030 2220 2f3e 0a20 203c 696d 6720 7372  00" />.  <img sr
-00000c50: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
-00000c60: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00000c70: 2e63 6f6d 2f64 616e 6965 6c67 6174 6973  .com/danielgatis
-00000c80: 2f72 656d 6267 2f6d 6173 7465 722f 6578  /rembg/master/ex
-00000c90: 616d 706c 6573 2f61 6e69 6d65 2d67 6972  amples/anime-gir
-00000ca0: 6c2d 322e 6f75 742e 706e 6722 2077 6964  l-2.out.png" wid
-00000cb0: 7468 3d22 3130 3022 202f 3e0a 2020 3c69  th="100" />.  <i
-00000cc0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000cd0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00000ce0: 6e74 656e 742e 636f 6d2f 6461 6e69 656c  ntent.com/daniel
-00000cf0: 6761 7469 732f 7265 6d62 672f 6d61 7374  gatis/rembg/mast
-00000d00: 6572 2f65 7861 6d70 6c65 732f 616e 696d  er/examples/anim
-00000d10: 652d 6769 726c 2d33 2e6a 7067 2220 7769  e-girl-3.jpg" wi
-00000d20: 6474 683d 2231 3030 2220 2f3e 0a20 203c  dth="100" />.  <
-00000d30: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000d40: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00000d50: 6f6e 7465 6e74 2e63 6f6d 2f64 616e 6965  ontent.com/danie
-00000d60: 6c67 6174 6973 2f72 656d 6267 2f6d 6173  lgatis/rembg/mas
-00000d70: 7465 722f 6578 616d 706c 6573 2f61 6e69  ter/examples/ani
-00000d80: 6d65 2d67 6972 6c2d 332e 6f75 742e 706e  me-girl-3.out.pn
-00000d90: 6722 2077 6964 7468 3d22 3130 3022 202f  g" width="100" /
-00000da0: 3e0a 3c2f 703e 0a0a 2a2a 4966 2074 6869  >.</p>..**If thi
-00000db0: 7320 7072 6f6a 6563 7420 6861 7320 6865  s project has he
-00000dc0: 6c70 6564 2079 6f75 2c20 706c 6561 7365  lped you, please
-00000dd0: 2063 6f6e 7369 6465 7220 6d61 6b69 6e67   consider making
-00000de0: 2061 205b 646f 6e61 7469 6f6e 5d28 6874   a [donation](ht
-00000df0: 7470 733a 2f2f 7777 772e 6275 796d 6561  tps://www.buymea
-00000e00: 636f 6666 6565 2e63 6f6d 2f64 616e 6965  coffee.com/danie
-00000e10: 6c67 6174 6973 292e 2a2a 0a0a 2323 2053  lgatis).**..## S
-00000e20: 706f 6e73 6f72 0a0a 3c74 6162 6c65 3e0a  ponsor..<table>.
-00000e30: 2020 3c74 723e 0a20 2020 203c 7464 2061    <tr>.    <td a
-00000e40: 6c69 676e 3d22 6365 6e74 6572 2220 7665  lign="center" ve
-00000e50: 7274 6963 616c 2d61 6c69 676e 3d22 6365  rtical-align="ce
-00000e60: 6e74 6572 223e 0a20 2020 2020 203c 6120  nter">.      <a 
-00000e70: 6872 6566 3d22 6874 7470 733a 2f2f 7068  href="https://ph
-00000e80: 6f74 6f72 6f6f 6d2e 636f 6d2f 6170 692f  otoroom.com/api/
-00000e90: 7265 6d6f 7665 2d62 6163 6b67 726f 756e  remove-backgroun
-00000ea0: 643f 7574 6d5f 736f 7572 6365 3d72 656d  d?utm_source=rem
-00000eb0: 6267 2675 746d 5f6d 6564 6975 6d3d 6769  bg&utm_medium=gi
-00000ec0: 7468 7562 5f77 6562 7061 6765 2675 746d  thub_webpage&utm
-00000ed0: 5f63 616d 7061 6967 6e3d 7370 6f6e 736f  _campaign=sponso
-00000ee0: 7222 203e 0a20 2020 2020 2020 203c 696d  r" >.        <im
-00000ef0: 6720 7372 633d 2268 7474 7073 3a2f 2f66  g src="https://f
-00000f00: 6f6e 742d 6364 6e2e 7068 6f74 6f72 6f6f  ont-cdn.photoroo
-00000f10: 6d2e 636f 6d2f 6d65 6469 612f 6170 692d  m.com/media/api-
-00000f20: 6c6f 676f 2e70 6e67 2220 7769 6474 683d  logo.png" width=
-00000f30: 2231 3230 7078 3b22 2061 6c74 3d22 556e  "120px;" alt="Un
-00000f40: 7370 6c61 7368 2220 2f3e 0a20 2020 2020  splash" />.     
-00000f50: 203c 2f61 3e0a 2020 2020 3c2f 7464 3e0a   </a>.    </td>.
-00000f60: 2020 2020 3c74 6420 616c 6967 6e3d 2263      <td align="c
-00000f70: 656e 7465 7222 2076 6572 7469 6361 6c2d  enter" vertical-
-00000f80: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00000f90: 2020 2020 2020 3c62 3e50 686f 746f 526f        <b>PhotoRo
-00000fa0: 6f6d 2052 656d 6f76 6520 4261 636b 6772  om Remove Backgr
-00000fb0: 6f75 6e64 2041 5049 3c2f 623e 0a20 2020  ound API</b>.   
-00000fc0: 2020 203c 6272 202f 3e0a 2020 2020 2020     <br />.      
-00000fd0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000fe0: 2f70 686f 746f 726f 6f6d 2e63 6f6d 2f61  /photoroom.com/a
-00000ff0: 7069 2f72 656d 6f76 652d 6261 636b 6772  pi/remove-backgr
-00001000: 6f75 6e64 3f75 746d 5f73 6f75 7263 653d  ound?utm_source=
-00001010: 7265 6d62 6726 7574 6d5f 6d65 6469 756d  rembg&utm_medium
-00001020: 3d67 6974 6875 625f 7765 6270 6167 6526  =github_webpage&
-00001030: 7574 6d5f 6361 6d70 6169 676e 3d73 706f  utm_campaign=spo
-00001040: 6e73 6f72 223e 6874 7470 733a 2f2f 7068  nsor">https://ph
-00001050: 6f74 6f72 6f6f 6d2e 636f 6d2f 6170 693c  otoroom.com/api<
-00001060: 2f61 3e0a 2020 2020 2020 3c62 7220 2f3e  /a>.      <br />
-00001070: 0a20 2020 2020 203c 7020 7769 6474 683d  .      <p width=
-00001080: 2232 3030 7078 223e 0a20 2020 2020 2020  "200px">.       
-00001090: 2046 6173 7420 616e 6420 6163 6375 7261   Fast and accura
-000010a0: 7465 2062 6163 6b67 726f 756e 6420 7265  te background re
-000010b0: 6d6f 7665 7220 4150 493c 6272 2f3e 0a20  mover API<br/>. 
-000010c0: 2020 2020 203c 2f70 3e0a 2020 2020 3c2f       </p>.    </
-000010d0: 7464 3e0a 2020 3c2f 7472 3e0a 3c2f 7461  td>.  </tr>.</ta
-000010e0: 626c 653e 0a0a 2323 2052 6571 7569 7265  ble>..## Require
-000010f0: 6d65 6e74 730a 0a60 6060 0a70 7974 686f  ments..```.pytho
-00001100: 6e3a 203e 332e 372c 203c 332e 3133 0a60  n: >3.7, <3.13.`
-00001110: 6060 0a0a 2323 2049 6e73 7461 6c6c 6174  ``..## Installat
-00001120: 696f 6e0a 0a43 5055 2073 7570 706f 7274  ion..CPU support
-00001130: 3a0a 0a60 6060 6261 7368 0a70 6970 2069  :..```bash.pip i
-00001140: 6e73 7461 6c6c 2072 656d 6267 2023 2066  nstall rembg # f
-00001150: 6f72 206c 6962 7261 7279 0a70 6970 2069  or library.pip i
-00001160: 6e73 7461 6c6c 2072 656d 6267 5b63 6c69  nstall rembg[cli
-00001170: 5d20 2320 666f 7220 6c69 6272 6172 7920  ] # for library 
-00001180: 2b20 636c 690a 6060 600a 0a47 5055 2073  + cli.```..GPU s
-00001190: 7570 706f 7274 3a0a 0a46 6972 7374 206f  upport:..First o
-000011a0: 6620 616c 6c2c 2079 6f75 206e 6565 6420  f all, you need 
-000011b0: 746f 2063 6865 636b 2069 6620 796f 7572  to check if your
-000011c0: 2073 7973 7465 6d20 7375 7070 6f72 7473   system supports
-000011d0: 2074 6865 2060 6f6e 6e78 7275 6e74 696d   the `onnxruntim
-000011e0: 652d 6770 7560 2e0a 0a47 6f20 746f 2068  e-gpu`...Go to h
-000011f0: 7474 7073 3a2f 2f6f 6e6e 7872 756e 7469  ttps://onnxrunti
-00001200: 6d65 2e61 6920 616e 6420 6368 6563 6b20  me.ai and check 
-00001210: 7468 6520 696e 7374 616c 6c61 7469 6f6e  the installation
-00001220: 206d 6174 7269 782e 0a0a 3c70 2073 7479   matrix...<p sty
-00001230: 6c65 3d22 6469 7370 6c61 793a 2066 6c65  le="display: fle
-00001240: 783b 616c 6967 6e2d 6974 656d 733a 2063  x;align-items: c
-00001250: 656e 7465 723b 6a75 7374 6966 792d 636f  enter;justify-co
-00001260: 6e74 656e 743a 2063 656e 7465 723b 223e  ntent: center;">
-00001270: 0a20 203c 696d 6720 7372 633d 2268 7474  .  <img src="htt
-00001280: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00001290: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f64  sercontent.com/d
-000012a0: 616e 6965 6c67 6174 6973 2f72 656d 6267  anielgatis/rembg
-000012b0: 2f6d 6173 7465 722f 6f6e 6e78 7275 6e74  /master/onnxrunt
-000012c0: 696d 652d 696e 7374 616c 6c61 7469 6f6e  ime-installation
-000012d0: 2d6d 6174 7269 782e 706e 6722 2077 6964  -matrix.png" wid
-000012e0: 7468 3d22 3430 3022 202f 3e0a 3c2f 703e  th="400" />.</p>
-000012f0: 0a0a 4966 2079 6573 2c20 6a75 7374 2072  ..If yes, just r
-00001300: 756e 3a0a 0a60 6060 6261 7368 0a70 6970  un:..```bash.pip
-00001310: 2069 6e73 7461 6c6c 2072 656d 6267 5b67   install rembg[g
-00001320: 7075 5d20 2320 666f 7220 6c69 6272 6172  pu] # for librar
-00001330: 790a 7069 7020 696e 7374 616c 6c20 7265  y.pip install re
-00001340: 6d62 675b 6770 752c 636c 695d 2023 2066  mbg[gpu,cli] # f
-00001350: 6f72 206c 6962 7261 7279 202b 2063 6c69  or library + cli
-00001360: 0a60 6060 0a0a 2323 2055 7361 6765 2061  .```..## Usage a
-00001370: 7320 6120 636c 690a 0a41 6674 6572 2074  s a cli..After t
-00001380: 6865 2069 6e73 7461 6c6c 6174 696f 6e20  he installation 
-00001390: 7374 6570 2079 6f75 2063 616e 2075 7365  step you can use
-000013a0: 2072 656d 6267 206a 7573 7420 7479 7069   rembg just typi
-000013b0: 6e67 2060 7265 6d62 6760 2069 6e20 796f  ng `rembg` in yo
-000013c0: 7572 2074 6572 6d69 6e61 6c20 7769 6e64  ur terminal wind
-000013d0: 6f77 2e0a 0a54 6865 2060 7265 6d62 6760  ow...The `rembg`
-000013e0: 2063 6f6d 6d61 6e64 2068 6173 2034 2073   command has 4 s
-000013f0: 7562 636f 6d6d 616e 6473 2c20 6f6e 6520  ubcommands, one 
-00001400: 666f 7220 6561 6368 2069 6e70 7574 2074  for each input t
-00001410: 7970 653a 0a2d 2060 6960 2066 6f72 2066  ype:.- `i` for f
-00001420: 696c 6573 0a2d 2060 7060 2066 6f72 2066  iles.- `p` for f
-00001430: 6f6c 6465 7273 0a2d 2060 7360 2066 6f72  olders.- `s` for
-00001440: 2068 7474 7020 7365 7276 6572 0a2d 2060   http server.- `
-00001450: 6260 2066 6f72 2052 4742 3234 2070 6978  b` for RGB24 pix
-00001460: 656c 2062 696e 6172 7920 7374 7265 616d  el binary stream
-00001470: 0a0a 596f 7520 6361 6e20 6765 7420 6865  ..You can get he
-00001480: 6c70 2061 626f 7574 2074 6865 206d 6169  lp about the mai
-00001490: 6e20 636f 6d6d 616e 6420 7573 696e 673a  n command using:
-000014a0: 0a0a 6060 600a 7265 6d62 6720 2d2d 6865  ..```.rembg --he
-000014b0: 6c70 0a60 6060 0a0a 4173 2077 656c 6c2c  lp.```..As well,
-000014c0: 2061 626f 7574 2061 6c6c 2074 6865 2073   about all the s
-000014d0: 7562 636f 6d6d 616e 6473 2075 7369 6e67  ubcommands using
-000014e0: 3a0a 0a60 6060 0a72 656d 6267 203c 434f  :..```.rembg <CO
-000014f0: 4d4d 414e 443e 202d 2d68 656c 700a 6060  MMAND> --help.``
-00001500: 600a 0a23 2323 2072 656d 6267 2060 6960  `..### rembg `i`
-00001510: 0a0a 5573 6564 2077 6865 6e20 696e 7075  ..Used when inpu
-00001520: 7420 616e 6420 6f75 7470 7574 2061 7265  t and output are
-00001530: 2066 696c 6573 2e0a 0a52 656d 6f76 6520   files...Remove 
-00001540: 7468 6520 6261 636b 6772 6f75 6e64 2066  the background f
-00001550: 726f 6d20 6120 7265 6d6f 7465 2069 6d61  rom a remote ima
-00001560: 6765 0a0a 6060 600a 6375 726c 202d 7320  ge..```.curl -s 
-00001570: 6874 7470 3a2f 2f69 6e70 7574 2e70 6e67  http://input.png
-00001580: 207c 2072 656d 6267 2069 203e 206f 7574   | rembg i > out
-00001590: 7075 742e 706e 670a 6060 600a 0a52 656d  put.png.```..Rem
-000015a0: 6f76 6520 7468 6520 6261 636b 6772 6f75  ove the backgrou
-000015b0: 6e64 2066 726f 6d20 6120 6c6f 6361 6c20  nd from a local 
-000015c0: 6669 6c65 0a0a 6060 600a 7265 6d62 6720  file..```.rembg 
-000015d0: 6920 7061 7468 2f74 6f2f 696e 7075 742e  i path/to/input.
-000015e0: 706e 6720 7061 7468 2f74 6f2f 6f75 7470  png path/to/outp
-000015f0: 7574 2e70 6e67 0a60 6060 0a0a 5265 6d6f  ut.png.```..Remo
-00001600: 7665 2074 6865 2062 6163 6b67 726f 756e  ve the backgroun
-00001610: 6420 7370 6563 6966 7969 6e67 2061 206d  d specifying a m
-00001620: 6f64 656c 0a0a 6060 600a 7265 6d62 6720  odel..```.rembg 
-00001630: 6920 2d6d 2075 326e 6574 7020 7061 7468  i -m u2netp path
-00001640: 2f74 6f2f 696e 7075 742e 706e 6720 7061  /to/input.png pa
-00001650: 7468 2f74 6f2f 6f75 7470 7574 2e70 6e67  th/to/output.png
-00001660: 0a60 6060 0a0a 5265 6d6f 7665 2074 6865  .```..Remove the
-00001670: 2062 6163 6b67 726f 756e 6420 7265 7475   background retu
-00001680: 726e 696e 6720 6f6e 6c79 2074 6865 206d  rning only the m
-00001690: 6173 6b0a 0a60 6060 0a72 656d 6267 2069  ask..```.rembg i
-000016a0: 202d 6f6d 2070 6174 682f 746f 2f69 6e70   -om path/to/inp
-000016b0: 7574 2e70 6e67 2070 6174 682f 746f 2f6f  ut.png path/to/o
-000016c0: 7574 7075 742e 706e 670a 6060 600a 0a0a  utput.png.```...
-000016d0: 5265 6d6f 7665 2074 6865 2062 6163 6b67  Remove the backg
-000016e0: 726f 756e 6420 6170 706c 7969 6e67 2061  round applying a
-000016f0: 6e20 616c 7068 6120 6d61 7474 696e 670a  n alpha matting.
-00001700: 0a60 6060 0a72 656d 6267 2069 202d 6120  .```.rembg i -a 
-00001710: 7061 7468 2f74 6f2f 696e 7075 742e 706e  path/to/input.pn
-00001720: 6720 7061 7468 2f74 6f2f 6f75 7470 7574  g path/to/output
-00001730: 2e70 6e67 0a60 6060 0a0a 5061 7373 696e  .png.```..Passin
-00001740: 6720 6578 7472 6173 2070 6172 616d 6574  g extras paramet
-00001750: 6572 730a 0a60 6060 0a53 414d 2065 7861  ers..```.SAM exa
-00001760: 6d70 6c65 0a0a 7265 6d62 6720 6920 2d6d  mple..rembg i -m
-00001770: 2073 616d 202d 7820 277b 2022 7361 6d5f   sam -x '{ "sam_
-00001780: 7072 6f6d 7074 223a 205b 7b22 7479 7065  prompt": [{"type
-00001790: 223a 2022 706f 696e 7422 2c20 2264 6174  ": "point", "dat
-000017a0: 6122 3a20 5b37 3234 2c20 3734 305d 2c20  a": [724, 740], 
-000017b0: 226c 6162 656c 223a 2031 7d5d 207d 2720  "label": 1}] }' 
-000017c0: 6578 616d 706c 6573 2f70 6c61 6e74 732d  examples/plants-
-000017d0: 312e 6a70 6720 6578 616d 706c 6573 2f70  1.jpg examples/p
-000017e0: 6c61 6e74 732d 312e 6f75 742e 706e 670a  lants-1.out.png.
-000017f0: 6060 600a 0a60 6060 0a43 7573 746f 6d20  ```..```.Custom 
-00001800: 6d6f 6465 6c20 6578 616d 706c 650a 0a72  model example..r
-00001810: 656d 6267 2069 202d 6d20 7532 6e65 745f  embg i -m u2net_
-00001820: 6375 7374 6f6d 202d 7820 277b 226d 6f64  custom -x '{"mod
-00001830: 656c 5f70 6174 6822 3a20 227e 2f2e 7532  el_path": "~/.u2
-00001840: 6e65 742f 7532 6e65 742e 6f6e 6e78 227d  net/u2net.onnx"}
-00001850: 2720 7061 7468 2f74 6f2f 696e 7075 742e  ' path/to/input.
-00001860: 706e 6720 7061 7468 2f74 6f2f 6f75 7470  png path/to/outp
-00001870: 7574 2e70 6e67 0a60 6060 0a0a 2323 2320  ut.png.```..### 
-00001880: 7265 6d62 6720 6070 600a 0a55 7365 6420  rembg `p`..Used 
-00001890: 7768 656e 2069 6e70 7574 2061 6e64 206f  when input and o
-000018a0: 7574 7075 7420 6172 6520 666f 6c64 6572  utput are folder
-000018b0: 732e 0a0a 5265 6d6f 7665 2074 6865 2062  s...Remove the b
-000018c0: 6163 6b67 726f 756e 6420 6672 6f6d 2061  ackground from a
-000018d0: 6c6c 2069 6d61 6765 7320 696e 2061 2066  ll images in a f
-000018e0: 6f6c 6465 720a 0a60 6060 0a72 656d 6267  older..```.rembg
-000018f0: 2070 2070 6174 682f 746f 2f69 6e70 7574   p path/to/input
-00001900: 2070 6174 682f 746f 2f6f 7574 7075 740a   path/to/output.
-00001910: 6060 600a 0a53 616d 6520 6173 2062 6566  ```..Same as bef
-00001920: 6f72 652c 2062 7574 2077 6174 6368 696e  ore, but watchin
-00001930: 6720 666f 7220 6e65 772f 6368 616e 6765  g for new/change
-00001940: 6420 6669 6c65 7320 746f 2070 726f 6365  d files to proce
-00001950: 7373 0a0a 6060 600a 7265 6d62 6720 7020  ss..```.rembg p 
-00001960: 2d77 2070 6174 682f 746f 2f69 6e70 7574  -w path/to/input
-00001970: 2070 6174 682f 746f 2f6f 7574 7075 740a   path/to/output.
-00001980: 6060 600a 0a23 2323 2072 656d 6267 2060  ```..### rembg `
-00001990: 7360 0a0a 5573 6564 2074 6f20 7374 6172  s`..Used to star
-000019a0: 7420 6874 7470 2073 6572 7665 722e 0a0a  t http server...
-000019b0: 6060 600a 7265 6d62 6720 7320 2d2d 686f  ```.rembg s --ho
-000019c0: 7374 2030 2e30 2e30 2e30 202d 2d70 6f72  st 0.0.0.0 --por
-000019d0: 7420 3730 3030 202d 2d6c 6f67 5f6c 6576  t 7000 --log_lev
-000019e0: 656c 2069 6e66 6f0a 6060 600a 0a54 6f20  el info.```..To 
-000019f0: 7365 6520 7468 6520 636f 6d70 6c65 7465  see the complete
-00001a00: 2065 6e64 706f 696e 7473 2064 6f63 756d   endpoints docum
-00001a10: 656e 7461 7469 6f6e 2c20 676f 2074 6f3a  entation, go to:
-00001a20: 2060 6874 7470 3a2f 2f6c 6f63 616c 686f   `http://localho
-00001a30: 7374 3a37 3030 302f 6170 6960 2e0a 0a52  st:7000/api`...R
-00001a40: 656d 6f76 6520 7468 6520 6261 636b 6772  emove the backgr
-00001a50: 6f75 6e64 2066 726f 6d20 616e 2069 6d61  ound from an ima
-00001a60: 6765 2075 726c 0a0a 6060 600a 6375 726c  ge url..```.curl
-00001a70: 202d 7320 2268 7474 703a 2f2f 6c6f 6361   -s "http://loca
-00001a80: 6c68 6f73 743a 3730 3030 2f61 7069 2f72  lhost:7000/api/r
-00001a90: 656d 6f76 653f 7572 6c3d 6874 7470 3a2f  emove?url=http:/
-00001aa0: 2f69 6e70 7574 2e70 6e67 2220 2d6f 206f  /input.png" -o o
-00001ab0: 7574 7075 742e 706e 670a 6060 600a 0a52  utput.png.```..R
-00001ac0: 656d 6f76 6520 7468 6520 6261 636b 6772  emove the backgr
-00001ad0: 6f75 6e64 2066 726f 6d20 616e 2075 706c  ound from an upl
-00001ae0: 6f61 6465 6420 696d 6167 650a 0a60 6060  oaded image..```
-00001af0: 0a63 7572 6c20 2d73 202d 4620 6669 6c65  .curl -s -F file
-00001b00: 3d40 2f70 6174 682f 746f 2f69 6e70 7574  =@/path/to/input
-00001b10: 2e6a 7067 2022 6874 7470 3a2f 2f6c 6f63  .jpg "http://loc
-00001b20: 616c 686f 7374 3a37 3030 302f 6170 692f  alhost:7000/api/
-00001b30: 7265 6d6f 7665 2220 202d 6f20 6f75 7470  remove"  -o outp
-00001b40: 7574 2e70 6e67 0a60 6060 0a0a 2323 2320  ut.png.```..### 
-00001b50: 7265 6d62 6720 6062 600a 0a50 726f 6365  rembg `b`..Proce
-00001b60: 7373 2061 2073 6571 7565 6e63 6520 6f66  ss a sequence of
-00001b70: 2052 4742 3234 2069 6d61 6765 7320 6672   RGB24 images fr
-00001b80: 6f6d 2073 7464 696e 2e20 5468 6973 2069  om stdin. This i
-00001b90: 7320 696e 7465 6e64 6564 2074 6f20 6265  s intended to be
-00001ba0: 2075 7365 6420 7769 7468 2061 6e6f 7468   used with anoth
-00001bb0: 6572 2070 726f 6772 616d 2c20 7375 6368  er program, such
-00001bc0: 2061 7320 4646 4d50 4547 2c20 7468 6174   as FFMPEG, that
-00001bd0: 206f 7574 7075 7473 2052 4742 3234 2070   outputs RGB24 p
-00001be0: 6978 656c 2064 6174 6120 746f 2073 7464  ixel data to std
-00001bf0: 6f75 742c 2077 6869 6368 2069 7320 7069  out, which is pi
-00001c00: 7065 6420 696e 746f 2074 6865 2073 7464  ped into the std
-00001c10: 696e 206f 6620 7468 6973 2070 726f 6772  in of this progr
-00001c20: 616d 2c20 616c 7468 6f75 6768 206e 6f74  am, although not
-00001c30: 6869 6e67 2070 7265 7665 6e74 7320 796f  hing prevents yo
-00001c40: 7520 6672 6f6d 206d 616e 7561 6c6c 7920  u from manually 
-00001c50: 7479 7069 6e67 2069 6e20 696d 6167 6573  typing in images
-00001c60: 2061 7420 7374 6469 6e2e 0a0a 6060 600a   at stdin...```.
-00001c70: 7265 6d62 6720 6220 696d 6167 655f 7769  rembg b image_wi
-00001c80: 6474 6820 696d 6167 655f 6865 6967 6874  dth image_height
-00001c90: 202d 6f20 6f75 7470 7574 5f73 7065 6369   -o output_speci
-00001ca0: 6669 6572 0a60 6060 0a0a 4172 6775 6d65  fier.```..Argume
-00001cb0: 6e74 733a 0a0a 2d20 696d 6167 655f 7769  nts:..- image_wi
-00001cc0: 6474 6820 3a20 7769 6474 6820 6f66 2069  dth : width of i
-00001cd0: 6e70 7574 2069 6d61 6765 2873 290a 2d20  nput image(s).- 
-00001ce0: 696d 6167 655f 6865 6967 6874 203a 2068  image_height : h
-00001cf0: 6569 6768 7420 6f66 2069 6e70 7574 2069  eight of input i
-00001d00: 6d61 6765 2873 290a 2d20 6f75 7470 7574  mage(s).- output
-00001d10: 5f73 7065 6369 6669 6572 3a20 7072 696e  _specifier: prin
-00001d20: 7466 2d73 7479 6c65 2073 7065 6369 6669  tf-style specifi
-00001d30: 6572 2066 6f72 206f 7574 7075 7420 6669  er for output fi
-00001d40: 6c65 6e61 6d65 732c 2066 6f72 2065 7861  lenames, for exa
-00001d50: 6d70 6c65 2069 6620 606f 7574 7075 742d  mple if `output-
-00001d60: 2530 3375 2e70 6e67 602c 2074 6865 6e20  %03u.png`, then 
-00001d70: 6f75 7470 7574 2066 696c 6573 2077 696c  output files wil
-00001d80: 6c20 6265 206e 616d 6564 2060 6f75 7470  l be named `outp
-00001d90: 7574 2d30 3030 2e70 6e67 602c 2060 6f75  ut-000.png`, `ou
-00001da0: 7470 7574 2d30 3031 2e70 6e67 602c 2060  tput-001.png`, `
-00001db0: 6f75 7470 7574 2d30 3032 2e70 6e67 602c  output-002.png`,
-00001dc0: 2065 7463 2e20 4f75 7470 7574 2066 696c   etc. Output fil
-00001dd0: 6573 2077 696c 6c20 6265 2073 6176 6564  es will be saved
-00001de0: 2069 6e20 504e 4720 666f 726d 6174 2072   in PNG format r
-00001df0: 6567 6172 646c 6573 7320 6f66 2074 6865  egardless of the
-00001e00: 2065 7874 656e 7369 6f6e 2073 7065 6369   extension speci
-00001e10: 6669 6564 2e20 596f 7520 6361 6e20 6f6d  fied. You can om
-00001e20: 6974 2069 7420 746f 2077 7269 7465 2072  it it to write r
-00001e30: 6573 756c 7473 2074 6f20 7374 646f 7574  esults to stdout
-00001e40: 2e0a 0a45 7861 6d70 6c65 2075 7361 6765  ...Example usage
-00001e50: 2077 6974 6820 4646 4d50 4547 3a0a 0a60   with FFMPEG:..`
-00001e60: 6060 0a66 666d 7065 6720 2d69 2069 6e70  ``.ffmpeg -i inp
-00001e70: 7574 2e6d 7034 202d 7373 2031 3020 2d61  ut.mp4 -ss 10 -a
-00001e80: 6e20 2d66 2072 6177 7669 6465 6f20 2d70  n -f rawvideo -p
-00001e90: 6978 5f66 6d74 2072 6762 3234 2070 6970  ix_fmt rgb24 pip
-00001ea0: 653a 3120 7c20 7265 6d62 6720 6220 3132  e:1 | rembg b 12
-00001eb0: 3830 2037 3230 202d 6f20 666f 6c64 6572  80 720 -o folder
-00001ec0: 2f6f 7574 7075 742d 2530 3375 2e70 6e67  /output-%03u.png
-00001ed0: 0a60 6060 0a0a 5468 6520 7769 6474 6820  .```..The width 
-00001ee0: 616e 6420 6865 6967 6874 2076 616c 7565  and height value
-00001ef0: 7320 6d75 7374 206d 6174 6368 2074 6865  s must match the
-00001f00: 2064 696d 656e 7369 6f6e 206f 6620 6f75   dimension of ou
-00001f10: 7470 7574 2069 6d61 6765 7320 6672 6f6d  tput images from
-00001f20: 2046 464d 5045 472e 204e 6f74 6520 666f   FFMPEG. Note fo
-00001f30: 7220 4646 4d50 4547 2c20 7468 6520 2260  r FFMPEG, the "`
-00001f40: 2d61 6e20 2d66 2072 6177 7669 6465 6f20  -an -f rawvideo 
-00001f50: 2d70 6978 5f66 6d74 2072 6762 3234 2070  -pix_fmt rgb24 p
-00001f60: 6970 653a 3160 2220 7061 7274 2069 7320  ipe:1`" part is 
-00001f70: 7265 7175 6972 6564 2066 6f72 2074 6865  required for the
-00001f80: 2077 686f 6c65 2074 6869 6e67 2074 6f20   whole thing to 
-00001f90: 776f 726b 2e0a 0a0a 2323 2055 7361 6765  work....## Usage
-00001fa0: 2061 7320 6120 6c69 6272 6172 790a 0a49   as a library..I
-00001fb0: 6e70 7574 2061 6e64 206f 7574 7075 7420  nput and output 
-00001fc0: 6173 2062 7974 6573 0a0a 6060 6070 7974  as bytes..```pyt
-00001fd0: 686f 6e0a 6672 6f6d 2072 656d 6267 2069  hon.from rembg i
-00001fe0: 6d70 6f72 7420 7265 6d6f 7665 0a0a 696e  mport remove..in
-00001ff0: 7075 745f 7061 7468 203d 2027 696e 7075  put_path = 'inpu
-00002000: 742e 706e 6727 0a6f 7574 7075 745f 7061  t.png'.output_pa
-00002010: 7468 203d 2027 6f75 7470 7574 2e70 6e67  th = 'output.png
-00002020: 270a 0a77 6974 6820 6f70 656e 2869 6e70  '..with open(inp
-00002030: 7574 5f70 6174 682c 2027 7262 2729 2061  ut_path, 'rb') a
-00002040: 7320 693a 0a20 2020 2077 6974 6820 6f70  s i:.    with op
-00002050: 656e 286f 7574 7075 745f 7061 7468 2c20  en(output_path, 
-00002060: 2777 6227 2920 6173 206f 3a0a 2020 2020  'wb') as o:.    
-00002070: 2020 2020 696e 7075 7420 3d20 692e 7265      input = i.re
-00002080: 6164 2829 0a20 2020 2020 2020 206f 7574  ad().        out
-00002090: 7075 7420 3d20 7265 6d6f 7665 2869 6e70  put = remove(inp
-000020a0: 7574 290a 2020 2020 2020 2020 6f2e 7772  ut).        o.wr
-000020b0: 6974 6528 6f75 7470 7574 290a 6060 600a  ite(output).```.
-000020c0: 0a49 6e70 7574 2061 6e64 206f 7574 7075  .Input and outpu
-000020d0: 7420 6173 2061 2050 494c 2069 6d61 6765  t as a PIL image
-000020e0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-000020f0: 2072 656d 6267 2069 6d70 6f72 7420 7265   rembg import re
-00002100: 6d6f 7665 0a66 726f 6d20 5049 4c20 696d  move.from PIL im
-00002110: 706f 7274 2049 6d61 6765 0a0a 696e 7075  port Image..inpu
-00002120: 745f 7061 7468 203d 2027 696e 7075 742e  t_path = 'input.
-00002130: 706e 6727 0a6f 7574 7075 745f 7061 7468  png'.output_path
-00002140: 203d 2027 6f75 7470 7574 2e70 6e67 270a   = 'output.png'.
-00002150: 0a69 6e70 7574 203d 2049 6d61 6765 2e6f  .input = Image.o
-00002160: 7065 6e28 696e 7075 745f 7061 7468 290a  pen(input_path).
-00002170: 6f75 7470 7574 203d 2072 656d 6f76 6528  output = remove(
-00002180: 696e 7075 7429 0a6f 7574 7075 742e 7361  input).output.sa
-00002190: 7665 286f 7574 7075 745f 7061 7468 290a  ve(output_path).
-000021a0: 6060 600a 0a49 6e70 7574 2061 6e64 206f  ```..Input and o
-000021b0: 7574 7075 7420 6173 2061 206e 756d 7079  utput as a numpy
-000021c0: 2061 7272 6179 0a0a 6060 6070 7974 686f   array..```pytho
-000021d0: 6e0a 6672 6f6d 2072 656d 6267 2069 6d70  n.from rembg imp
-000021e0: 6f72 7420 7265 6d6f 7665 0a69 6d70 6f72  ort remove.impor
-000021f0: 7420 6376 320a 0a69 6e70 7574 5f70 6174  t cv2..input_pat
-00002200: 6820 3d20 2769 6e70 7574 2e70 6e67 270a  h = 'input.png'.
-00002210: 6f75 7470 7574 5f70 6174 6820 3d20 276f  output_path = 'o
-00002220: 7574 7075 742e 706e 6727 0a0a 696e 7075  utput.png'..inpu
-00002230: 7420 3d20 6376 322e 696d 7265 6164 2869  t = cv2.imread(i
-00002240: 6e70 7574 5f70 6174 6829 0a6f 7574 7075  nput_path).outpu
-00002250: 7420 3d20 7265 6d6f 7665 2869 6e70 7574  t = remove(input
-00002260: 290a 6376 322e 696d 7772 6974 6528 6f75  ).cv2.imwrite(ou
-00002270: 7470 7574 5f70 6174 682c 206f 7574 7075  tput_path, outpu
-00002280: 7429 0a60 6060 0a0a 486f 7720 746f 2069  t).```..How to i
-00002290: 7465 7261 7465 206f 7665 7220 6669 6c65  terate over file
-000022a0: 7320 696e 2061 2070 6572 666f 726d 6174  s in a performat
-000022b0: 6963 2077 6179 0a0a 6060 6070 7974 686f  ic way..```pytho
-000022c0: 6e0a 6672 6f6d 2070 6174 686c 6962 2069  n.from pathlib i
-000022d0: 6d70 6f72 7420 5061 7468 0a66 726f 6d20  mport Path.from 
-000022e0: 7265 6d62 6720 696d 706f 7274 2072 656d  rembg import rem
-000022f0: 6f76 652c 206e 6577 5f73 6573 7369 6f6e  ove, new_session
-00002300: 0a0a 7365 7373 696f 6e20 3d20 6e65 775f  ..session = new_
-00002310: 7365 7373 696f 6e28 290a 0a66 6f72 2066  session()..for f
-00002320: 696c 6520 696e 2050 6174 6828 2770 6174  ile in Path('pat
-00002330: 682f 746f 2f66 6f6c 6465 7227 292e 676c  h/to/folder').gl
-00002340: 6f62 2827 2a2e 706e 6727 293a 0a20 2020  ob('*.png'):.   
-00002350: 2069 6e70 7574 5f70 6174 6820 3d20 7374   input_path = st
-00002360: 7228 6669 6c65 290a 2020 2020 6f75 7470  r(file).    outp
-00002370: 7574 5f70 6174 6820 3d20 7374 7228 6669  ut_path = str(fi
-00002380: 6c65 2e70 6172 656e 7420 2f20 2866 696c  le.parent / (fil
-00002390: 652e 7374 656d 202b 2022 2e6f 7574 2e70  e.stem + ".out.p
-000023a0: 6e67 2229 290a 0a20 2020 2077 6974 6820  ng"))..    with 
-000023b0: 6f70 656e 2869 6e70 7574 5f70 6174 682c  open(input_path,
-000023c0: 2027 7262 2729 2061 7320 693a 0a20 2020   'rb') as i:.   
-000023d0: 2020 2020 2077 6974 6820 6f70 656e 286f       with open(o
-000023e0: 7574 7075 745f 7061 7468 2c20 2777 6227  utput_path, 'wb'
-000023f0: 2920 6173 206f 3a0a 2020 2020 2020 2020  ) as o:.        
-00002400: 2020 2020 696e 7075 7420 3d20 692e 7265      input = i.re
-00002410: 6164 2829 0a20 2020 2020 2020 2020 2020  ad().           
-00002420: 206f 7574 7075 7420 3d20 7265 6d6f 7665   output = remove
-00002430: 2869 6e70 7574 2c20 7365 7373 696f 6e3d  (input, session=
-00002440: 7365 7373 696f 6e29 0a20 2020 2020 2020  session).       
-00002450: 2020 2020 206f 2e77 7269 7465 286f 7574       o.write(out
-00002460: 7075 7429 0a60 6060 0a54 6f20 7365 6520  put).```.To see 
-00002470: 6120 6675 6c6c 206c 6973 7420 6f66 2065  a full list of e
-00002480: 7861 6d70 6c65 7320 6f6e 2068 6f77 2074  xamples on how t
-00002490: 6f20 7573 6520 7265 6d62 672c 2067 6f20  o use rembg, go 
-000024a0: 746f 2074 6865 205b 6578 616d 706c 6573  to the [examples
-000024b0: 5d28 5553 4147 452e 6d64 2920 7061 6765  ](USAGE.md) page
-000024c0: 2e0a 2323 2055 7361 6765 2061 7320 6120  ..## Usage as a 
-000024d0: 646f 636b 6572 0a0a 4a75 7374 2072 6570  docker..Just rep
-000024e0: 6c61 6365 2074 6865 2060 7265 6d62 6760  lace the `rembg`
-000024f0: 2063 6f6d 6d61 6e64 2066 6f72 2060 646f   command for `do
-00002500: 636b 6572 2072 756e 2064 616e 6965 6c67  cker run danielg
-00002510: 6174 6973 2f72 656d 6267 602e 0a0a 5472  atis/rembg`...Tr
-00002520: 7920 7468 6973 3a0a 0a60 6060 0a64 6f63  y this:..```.doc
-00002530: 6b65 7220 7275 6e20 2d76 2070 6174 682f  ker run -v path/
-00002540: 746f 2f69 6e70 7574 3a2f 7265 6d62 6720  to/input:/rembg 
-00002550: 6461 6e69 656c 6761 7469 732f 7265 6d62  danielgatis/remb
-00002560: 6720 6920 696e 7075 742e 706e 6720 7061  g i input.png pa
-00002570: 7468 2f74 6f2f 6f75 7470 7574 2f6f 7574  th/to/output/out
-00002580: 7075 742e 706e 670a 6060 600a 0a23 2320  put.png.```..## 
-00002590: 4d6f 6465 6c73 0a0a 416c 6c20 6d6f 6465  Models..All mode
-000025a0: 6c73 2061 7265 2064 6f77 6e6c 6f61 6465  ls are downloade
-000025b0: 6420 616e 6420 7361 7665 6420 696e 2074  d and saved in t
-000025c0: 6865 2075 7365 7220 686f 6d65 2066 6f6c  he user home fol
-000025d0: 6465 7220 696e 2074 6865 2060 2e75 326e  der in the `.u2n
-000025e0: 6574 6020 6469 7265 6374 6f72 792e 0a0a  et` directory...
-000025f0: 5468 6520 6176 6169 6c61 626c 6520 6d6f  The available mo
-00002600: 6465 6c73 2061 7265 3a0a 0a2d 2020 2075  dels are:..-   u
-00002610: 326e 6574 2028 5b64 6f77 6e6c 6f61 645d  2net ([download]
-00002620: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002630: 636f 6d2f 6461 6e69 656c 6761 7469 732f  com/danielgatis/
-00002640: 7265 6d62 672f 7265 6c65 6173 6573 2f64  rembg/releases/d
-00002650: 6f77 6e6c 6f61 642f 7630 2e30 2e30 2f75  ownload/v0.0.0/u
-00002660: 326e 6574 2e6f 6e6e 7829 2c20 5b73 6f75  2net.onnx), [sou
-00002670: 7263 655d 2868 7474 7073 3a2f 2f67 6974  rce](https://git
-00002680: 6875 622e 636f 6d2f 7875 6562 696e 7169  hub.com/xuebinqi
-00002690: 6e2f 552d 322d 4e65 7429 293a 2041 2070  n/U-2-Net)): A p
-000026a0: 7265 2d74 7261 696e 6564 206d 6f64 656c  re-trained model
-000026b0: 2066 6f72 2067 656e 6572 616c 2075 7365   for general use
-000026c0: 2063 6173 6573 2e0a 2d20 2020 7532 6e65   cases..-   u2ne
-000026d0: 7470 2028 5b64 6f77 6e6c 6f61 645d 2868  tp ([download](h
-000026e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000026f0: 6d2f 6461 6e69 656c 6761 7469 732f 7265  m/danielgatis/re
-00002700: 6d62 672f 7265 6c65 6173 6573 2f64 6f77  mbg/releases/dow
-00002710: 6e6c 6f61 642f 7630 2e30 2e30 2f75 326e  nload/v0.0.0/u2n
-00002720: 6574 702e 6f6e 6e78 292c 205b 736f 7572  etp.onnx), [sour
-00002730: 6365 5d28 6874 7470 733a 2f2f 6769 7468  ce](https://gith
-00002740: 7562 2e63 6f6d 2f78 7565 6269 6e71 696e  ub.com/xuebinqin
-00002750: 2f55 2d32 2d4e 6574 2929 3a20 4120 6c69  /U-2-Net)): A li
-00002760: 6768 7477 6569 6768 7420 7665 7273 696f  ghtweight versio
-00002770: 6e20 6f66 2075 326e 6574 206d 6f64 656c  n of u2net model
-00002780: 2e0a 2d20 2020 7532 6e65 745f 6875 6d61  ..-   u2net_huma
-00002790: 6e5f 7365 6720 285b 646f 776e 6c6f 6164  n_seg ([download
-000027a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000027b0: 2e63 6f6d 2f64 616e 6965 6c67 6174 6973  .com/danielgatis
-000027c0: 2f72 656d 6267 2f72 656c 6561 7365 732f  /rembg/releases/
-000027d0: 646f 776e 6c6f 6164 2f76 302e 302e 302f  download/v0.0.0/
-000027e0: 7532 6e65 745f 6875 6d61 6e5f 7365 672e  u2net_human_seg.
-000027f0: 6f6e 6e78 292c 205b 736f 7572 6365 5d28  onnx), [source](
-00002800: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002810: 6f6d 2f78 7565 6269 6e71 696e 2f55 2d32  om/xuebinqin/U-2
-00002820: 2d4e 6574 2929 3a20 4120 7072 652d 7472  -Net)): A pre-tr
-00002830: 6169 6e65 6420 6d6f 6465 6c20 666f 7220  ained model for 
-00002840: 6875 6d61 6e20 7365 676d 656e 7461 7469  human segmentati
-00002850: 6f6e 2e0a 2d20 2020 7532 6e65 745f 636c  on..-   u2net_cl
-00002860: 6f74 685f 7365 6720 285b 646f 776e 6c6f  oth_seg ([downlo
-00002870: 6164 5d28 6874 7470 733a 2f2f 6769 7468  ad](https://gith
-00002880: 7562 2e63 6f6d 2f64 616e 6965 6c67 6174  ub.com/danielgat
-00002890: 6973 2f72 656d 6267 2f72 656c 6561 7365  is/rembg/release
-000028a0: 732f 646f 776e 6c6f 6164 2f76 302e 302e  s/download/v0.0.
-000028b0: 302f 7532 6e65 745f 636c 6f74 685f 7365  0/u2net_cloth_se
-000028c0: 672e 6f6e 6e78 292c 205b 736f 7572 6365  g.onnx), [source
-000028d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000028e0: 2e63 6f6d 2f6c 6576 696e 6461 6268 692f  .com/levindabhi/
-000028f0: 636c 6f74 682d 7365 676d 656e 7461 7469  cloth-segmentati
-00002900: 6f6e 2929 3a20 4120 7072 652d 7472 6169  on)): A pre-trai
-00002910: 6e65 6420 6d6f 6465 6c20 666f 7220 436c  ned model for Cl
-00002920: 6f74 6873 2050 6172 7369 6e67 2066 726f  oths Parsing fro
-00002930: 6d20 6875 6d61 6e20 706f 7274 7261 6974  m human portrait
-00002940: 2e20 4865 7265 2063 6c6f 7468 6573 2061  . Here clothes a
-00002950: 7265 2070 6172 7365 6420 696e 746f 2033  re parsed into 3
-00002960: 2063 6174 6567 6f72 793a 2055 7070 6572   category: Upper
-00002970: 2062 6f64 792c 204c 6f77 6572 2062 6f64   body, Lower bod
-00002980: 7920 616e 6420 4675 6c6c 2062 6f64 792e  y and Full body.
-00002990: 0a2d 2020 2073 696c 7565 7461 2028 5b64  .-   silueta ([d
-000029a0: 6f77 6e6c 6f61 645d 2868 7474 7073 3a2f  ownload](https:/
-000029b0: 2f67 6974 6875 622e 636f 6d2f 6461 6e69  /github.com/dani
-000029c0: 656c 6761 7469 732f 7265 6d62 672f 7265  elgatis/rembg/re
-000029d0: 6c65 6173 6573 2f64 6f77 6e6c 6f61 642f  leases/download/
-000029e0: 7630 2e30 2e30 2f73 696c 7565 7461 2e6f  v0.0.0/silueta.o
-000029f0: 6e6e 7829 2c20 5b73 6f75 7263 655d 2868  nnx), [source](h
-00002a00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002a10: 6d2f 7875 6562 696e 7169 6e2f 552d 322d  m/xuebinqin/U-2-
-00002a20: 4e65 742f 6973 7375 6573 2f32 3935 2929  Net/issues/295))
-00002a30: 3a20 5361 6d65 2061 7320 7532 6e65 7420  : Same as u2net 
-00002a40: 6275 7420 7468 6520 7369 7a65 2069 7320  but the size is 
-00002a50: 7265 6475 6365 6420 746f 2034 334d 622e  reduced to 43Mb.
-00002a60: 0a2d 2020 2069 736e 6574 2d67 656e 6572  .-   isnet-gener
-00002a70: 616c 2d75 7365 2028 5b64 6f77 6e6c 6f61  al-use ([downloa
-00002a80: 645d 2868 7474 7073 3a2f 2f67 6974 6875  d](https://githu
-00002a90: 622e 636f 6d2f 6461 6e69 656c 6761 7469  b.com/danielgati
-00002aa0: 732f 7265 6d62 672f 7265 6c65 6173 6573  s/rembg/releases
-00002ab0: 2f64 6f77 6e6c 6f61 642f 7630 2e30 2e30  /download/v0.0.0
-00002ac0: 2f69 736e 6574 2d67 656e 6572 616c 2d75  /isnet-general-u
-00002ad0: 7365 2e6f 6e6e 7829 2c20 5b73 6f75 7263  se.onnx), [sourc
-00002ae0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00002af0: 622e 636f 6d2f 7875 6562 696e 7169 6e2f  b.com/xuebinqin/
-00002b00: 4449 5329 293a 2041 206e 6577 2070 7265  DIS)): A new pre
-00002b10: 2d74 7261 696e 6564 206d 6f64 656c 2066  -trained model f
-00002b20: 6f72 2067 656e 6572 616c 2075 7365 2063  or general use c
-00002b30: 6173 6573 2e0a 2d20 2020 6973 6e65 742d  ases..-   isnet-
-00002b40: 616e 696d 6520 285b 646f 776e 6c6f 6164  anime ([download
-00002b50: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00002b60: 2e63 6f6d 2f64 616e 6965 6c67 6174 6973  .com/danielgatis
-00002b70: 2f72 656d 6267 2f72 656c 6561 7365 732f  /rembg/releases/
-00002b80: 646f 776e 6c6f 6164 2f76 302e 302e 302f  download/v0.0.0/
-00002b90: 6973 6e65 742d 616e 696d 652e 6f6e 6e78  isnet-anime.onnx
-00002ba0: 292c 205b 736f 7572 6365 5d28 6874 7470  ), [source](http
-00002bb0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
-00002bc0: 6b79 544e 542f 616e 696d 652d 7365 676d  kyTNT/anime-segm
-00002bd0: 656e 7461 7469 6f6e 2929 3a20 4120 6869  entation)): A hi
-00002be0: 6768 2d61 6363 7572 6163 7920 7365 676d  gh-accuracy segm
-00002bf0: 656e 7461 7469 6f6e 2066 6f72 2061 6e69  entation for ani
-00002c00: 6d65 2063 6861 7261 6374 6572 2e0a 2d20  me character..- 
-00002c10: 2020 7361 6d20 285b 646f 776e 6c6f 6164    sam ([download
-00002c20: 2065 6e63 6f64 6572 5d28 6874 7470 733a   encoder](https:
-00002c30: 2f2f 6769 7468 7562 2e63 6f6d 2f64 616e  //github.com/dan
-00002c40: 6965 6c67 6174 6973 2f72 656d 6267 2f72  ielgatis/rembg/r
-00002c50: 656c 6561 7365 732f 646f 776e 6c6f 6164  eleases/download
-00002c60: 2f76 302e 302e 302f 7669 745f 622d 656e  /v0.0.0/vit_b-en
-00002c70: 636f 6465 722d 7175 616e 742e 6f6e 6e78  coder-quant.onnx
-00002c80: 292c 205b 646f 776e 6c6f 6164 2064 6563  ), [download dec
-00002c90: 6f64 6572 5d28 6874 7470 733a 2f2f 6769  oder](https://gi
-00002ca0: 7468 7562 2e63 6f6d 2f64 616e 6965 6c67  thub.com/danielg
-00002cb0: 6174 6973 2f72 656d 6267 2f72 656c 6561  atis/rembg/relea
-00002cc0: 7365 732f 646f 776e 6c6f 6164 2f76 302e  ses/download/v0.
-00002cd0: 302e 302f 7669 745f 622d 6465 636f 6465  0.0/vit_b-decode
-00002ce0: 722d 7175 616e 742e 6f6e 6e78 292c 205b  r-quant.onnx), [
-00002cf0: 736f 7572 6365 5d28 6874 7470 733a 2f2f  source](https://
-00002d00: 6769 7468 7562 2e63 6f6d 2f66 6163 6562  github.com/faceb
-00002d10: 6f6f 6b72 6573 6561 7263 682f 7365 676d  ookresearch/segm
-00002d20: 656e 742d 616e 7974 6869 6e67 2929 3a20  ent-anything)): 
-00002d30: 4120 7072 652d 7472 6169 6e65 6420 6d6f  A pre-trained mo
-00002d40: 6465 6c20 666f 7220 616e 7920 7573 6520  del for any use 
-00002d50: 6361 7365 732e 0a0a 2323 2320 486f 7720  cases...### How 
-00002d60: 746f 2074 7261 696e 2079 6f75 7220 6f77  to train your ow
-00002d70: 6e20 6d6f 6465 6c0a 0a49 6620 596f 7520  n model..If You 
-00002d80: 6e65 6564 206d 6f72 6520 6669 6e65 2074  need more fine t
-00002d90: 756e 6564 206d 6f64 656c 7320 7472 7920  uned models try 
-00002da0: 7468 6973 3a0a 6874 7470 733a 2f2f 6769  this:.https://gi
-00002db0: 7468 7562 2e63 6f6d 2f64 616e 6965 6c67  thub.com/danielg
-00002dc0: 6174 6973 2f72 656d 6267 2f69 7373 7565  atis/rembg/issue
-00002dd0: 732f 3139 3323 6973 7375 6563 6f6d 6d65  s/193#issuecomme
-00002de0: 6e74 2d31 3035 3535 3334 3238 390a 0a0a  nt-1055534289...
-00002df0: 2323 2053 6f6d 6520 7669 6465 6f20 7475  ## Some video tu
-00002e00: 746f 7269 616c 730a 0a2d 2068 7474 7073  torials..- https
-00002e10: 3a2f 2f77 7777 2e79 6f75 7475 6265 2e63  ://www.youtube.c
-00002e20: 6f6d 2f77 6174 6368 3f76 3d33 7871 7770  om/watch?v=3xqwp
-00002e30: 586a 7879 4d51 0a2d 2068 7474 7073 3a2f  XjxyMQ.- https:/
-00002e40: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
-00002e50: 2f77 6174 6368 3f76 3d64 464b 5247 5864  /watch?v=dFKRGXd
-00002e60: 6b47 4a55 0a2d 2068 7474 7073 3a2f 2f77  kGJU.- https://w
-00002e70: 7777 2e79 6f75 7475 6265 2e63 6f6d 2f77  ww.youtube.com/w
-00002e80: 6174 6368 3f76 3d41 692d 4253 5f54 3779  atch?v=Ai-BS_T7y
-00002e90: 6a45 0a2d 2068 7474 7073 3a2f 2f77 7777  jE.- https://www
-00002ea0: 2e79 6f75 7475 6265 2e63 6f6d 2f77 6174  .youtube.com/wat
-00002eb0: 6368 3f76 3d44 3757 2d43 3075 7256 6351  ch?v=D7W-C0urVcQ
-00002ec0: 0a0a 2323 2052 6566 6572 656e 6365 730a  ..## References.
-00002ed0: 0a2d 2068 7474 7073 3a2f 2f61 7278 6976  .- https://arxiv
-00002ee0: 2e6f 7267 2f70 6466 2f32 3030 352e 3039  .org/pdf/2005.09
-00002ef0: 3030 372e 7064 660a 2d20 6874 7470 733a  007.pdf.- https:
-00002f00: 2f2f 6769 7468 7562 2e63 6f6d 2f4e 6174  //github.com/Nat
-00002f10: 6861 6e55 412f 552d 322d 4e65 740a 2d20  hanUA/U-2-Net.- 
-00002f20: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002f30: 6f6d 2f70 796d 6174 7469 6e67 2f70 796d  om/pymatting/pym
-00002f40: 6174 7469 6e67 0a0a 2323 2046 4151 0a0a  atting..## FAQ..
-00002f50: 2323 2320 5768 656e 2077 696c 6c20 7468  ### When will th
-00002f60: 6973 206c 6962 7261 7279 2070 726f 7669  is library provi
-00002f70: 6465 2073 7570 706f 7274 2066 6f72 2050  de support for P
-00002f80: 7974 686f 6e20 7665 7273 696f 6e20 332e  ython version 3.
-00002f90: 7878 3f0a 0a54 6869 7320 6c69 6272 6172  xx?..This librar
-00002fa0: 7920 6469 7265 6374 6c79 2064 6570 656e  y directly depen
-00002fb0: 6473 206f 6e20 7468 6520 5b6f 6e6e 7872  ds on the [onnxr
-00002fc0: 756e 7469 6d65 5d28 6874 7470 733a 2f2f  untime](https://
-00002fd0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00002fe0: 2f6f 6e6e 7872 756e 7469 6d65 2920 6c69  /onnxruntime) li
-00002ff0: 6272 6172 792e 2054 6865 7265 666f 7265  brary. Therefore
-00003000: 2c20 7765 2063 616e 206f 6e6c 7920 7570  , we can only up
-00003010: 6461 7465 2074 6865 2050 7974 686f 6e20  date the Python 
-00003020: 7665 7273 696f 6e20 7768 656e 205b 6f6e  version when [on
-00003030: 6e78 7275 6e74 696d 655d 2868 7474 7073  nxruntime](https
-00003040: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00003050: 6563 742f 6f6e 6e78 7275 6e74 696d 6529  ect/onnxruntime)
-00003060: 2070 726f 7669 6465 7320 7375 7070 6f72   provides suppor
-00003070: 7420 666f 7220 7468 6174 2073 7065 6369  t for that speci
-00003080: 6669 6320 7665 7273 696f 6e2e 0a0a 2323  fic version...##
-00003090: 2042 7579 206d 6520 6120 636f 6666 6565   Buy me a coffee
-000030a0: 0a0a 4c69 6b65 6420 736f 6d65 206f 6620  ..Liked some of 
-000030b0: 6d79 2077 6f72 6b3f 2042 7579 206d 6520  my work? Buy me 
-000030c0: 6120 636f 6666 6565 2028 6f72 206d 6f72  a coffee (or mor
-000030d0: 6520 6c69 6b65 6c79 2061 2062 6565 7229  e likely a beer)
-000030e0: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-000030f0: 3a2f 2f77 7777 2e62 7579 6d65 6163 6f66  ://www.buymeacof
-00003100: 6665 652e 636f 6d2f 6461 6e69 656c 6761  fee.com/danielga
-00003110: 7469 7322 2074 6172 6765 743d 225f 626c  tis" target="_bl
-00003120: 616e 6b22 3e3c 696d 6720 7372 633d 2268  ank"><img src="h
-00003130: 7474 7073 3a2f 2f62 6d63 2d63 646e 2e6e  ttps://bmc-cdn.n
-00003140: 7963 332e 6469 6769 7461 6c6f 6365 616e  yc3.digitalocean
-00003150: 7370 6163 6573 2e63 6f6d 2f42 4d43 2d62  spaces.com/BMC-b
-00003160: 7574 746f 6e2d 696d 6167 6573 2f63 7573  utton-images/cus
-00003170: 746f 6d5f 696d 6167 6573 2f6f 7261 6e67  tom_images/orang
-00003180: 655f 696d 672e 706e 6722 2061 6c74 3d22  e_img.png" alt="
-00003190: 4275 7920 4d65 2041 2043 6f66 6665 6522  Buy Me A Coffee"
-000031a0: 2073 7479 6c65 3d22 6865 6967 6874 3a20   style="height: 
-000031b0: 6175 746f 2021 696d 706f 7274 616e 743b  auto !important;
-000031c0: 7769 6474 683a 2061 7574 6f20 2169 6d70  width: auto !imp
-000031d0: 6f72 7461 6e74 3b22 3e3c 2f61 3e0a 0a23  ortant;"></a>..#
-000031e0: 2320 4c69 6365 6e73 650a 0a43 6f70 7972  # License..Copyr
-000031f0: 6967 6874 2028 6329 2032 3032 302d 7072  ight (c) 2020-pr
-00003200: 6573 656e 7420 5b44 616e 6965 6c20 4761  esent [Daniel Ga
-00003210: 7469 735d 2868 7474 7073 3a2f 2f67 6974  tis](https://git
-00003220: 6875 622e 636f 6d2f 6461 6e69 656c 6761  hub.com/danielga
-00003230: 7469 7329 0a0a 4c69 6365 6e73 6564 2075  tis)..Licensed u
-00003240: 6e64 6572 205b 4d49 5420 4c69 6365 6e73  nder [MIT Licens
-00003250: 655d 282e 2f4c 4943 454e 5345 2e74 7874  e](./LICENSE.txt
-00003260: 290a                                     ).
+000001e0: 290a 0a52 656d 6267 2069 7320 6120 746f  )..Rembg is a to
+000001f0: 6f6c 2074 6f20 7265 6d6f 7665 2069 6d61  ol to remove ima
+00000200: 6765 7320 6261 636b 6772 6f75 6e64 2e0a  ges background..
+00000210: 0a3c 7020 7374 796c 653d 2264 6973 706c  .<p style="displ
+00000220: 6179 3a20 666c 6578 3b61 6c69 676e 2d69  ay: flex;align-i
+00000230: 7465 6d73 3a20 6365 6e74 6572 3b6a 7573  tems: center;jus
+00000240: 7469 6679 2d63 6f6e 7465 6e74 3a20 6365  tify-content: ce
+00000250: 6e74 6572 3b22 3e0a 2020 3c69 6d67 2061  nter;">.  <img a
+00000260: 6c74 3d22 6578 616d 706c 6520 6361 722d  lt="example car-
+00000270: 3122 2073 7263 3d22 6874 7470 733a 2f2f  1" src="https://
+00000280: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00000290: 6e74 656e 742e 636f 6d2f 6461 6e69 656c  ntent.com/daniel
+000002a0: 6761 7469 732f 7265 6d62 672f 6d61 7374  gatis/rembg/mast
+000002b0: 6572 2f65 7861 6d70 6c65 732f 6361 722d  er/examples/car-
+000002c0: 312e 6a70 6722 2077 6964 7468 3d22 3130  1.jpg" width="10
+000002d0: 3022 202f 3e0a 2020 3c69 6d67 2061 6c74  0" />.  <img alt
+000002e0: 3d22 6578 616d 706c 6520 6361 722d 312e  ="example car-1.
+000002f0: 6f75 7422 2073 7263 3d22 6874 7470 733a  out" src="https:
+00000300: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00000310: 636f 6e74 656e 742e 636f 6d2f 6461 6e69  content.com/dani
+00000320: 656c 6761 7469 732f 7265 6d62 672f 6d61  elgatis/rembg/ma
+00000330: 7374 6572 2f65 7861 6d70 6c65 732f 6361  ster/examples/ca
+00000340: 722d 312e 6f75 742e 706e 6722 2077 6964  r-1.out.png" wid
+00000350: 7468 3d22 3130 3022 202f 3e0a 2020 3c69  th="100" />.  <i
+00000360: 6d67 2061 6c74 3d22 6578 616d 706c 6520  mg alt="example 
+00000370: 6361 722d 3222 2073 7263 3d22 6874 7470  car-2" src="http
+00000380: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000390: 6572 636f 6e74 656e 742e 636f 6d2f 6461  ercontent.com/da
+000003a0: 6e69 656c 6761 7469 732f 7265 6d62 672f  nielgatis/rembg/
+000003b0: 6d61 7374 6572 2f65 7861 6d70 6c65 732f  master/examples/
+000003c0: 6361 722d 322e 6a70 6722 2077 6964 7468  car-2.jpg" width
+000003d0: 3d22 3130 3022 202f 3e0a 2020 3c69 6d67  ="100" />.  <img
+000003e0: 2061 6c74 3d22 6578 616d 706c 6520 6361   alt="example ca
+000003f0: 722d 322e 6f75 7422 2073 7263 3d22 6874  r-2.out" src="ht
+00000400: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000410: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000420: 6461 6e69 656c 6761 7469 732f 7265 6d62  danielgatis/remb
+00000430: 672f 6d61 7374 6572 2f65 7861 6d70 6c65  g/master/example
+00000440: 732f 6361 722d 322e 6f75 742e 706e 6722  s/car-2.out.png"
+00000450: 2077 6964 7468 3d22 3130 3022 202f 3e0a   width="100" />.
+00000460: 2020 3c69 6d67 2061 6c74 3d22 6578 616d    <img alt="exam
+00000470: 706c 6520 6361 722d 3322 2073 7263 3d22  ple car-3" src="
+00000480: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+00000490: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+000004a0: 6d2f 6461 6e69 656c 6761 7469 732f 7265  m/danielgatis/re
+000004b0: 6d62 672f 6d61 7374 6572 2f65 7861 6d70  mbg/master/examp
+000004c0: 6c65 732f 6361 722d 332e 6a70 6722 2077  les/car-3.jpg" w
+000004d0: 6964 7468 3d22 3130 3022 202f 3e0a 2020  idth="100" />.  
+000004e0: 3c69 6d67 2061 6c74 3d22 6578 616d 706c  <img alt="exampl
+000004f0: 6520 6361 722d 332e 6f75 7422 2073 7263  e car-3.out" src
+00000500: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+00000510: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000520: 636f 6d2f 6461 6e69 656c 6761 7469 732f  com/danielgatis/
+00000530: 7265 6d62 672f 6d61 7374 6572 2f65 7861  rembg/master/exa
+00000540: 6d70 6c65 732f 6361 722d 332e 6f75 742e  mples/car-3.out.
+00000550: 706e 6722 2077 6964 7468 3d22 3130 3022  png" width="100"
+00000560: 202f 3e0a 3c2f 703e 0a0a 3c70 2073 7479   />.</p>..<p sty
+00000570: 6c65 3d22 6469 7370 6c61 793a 2066 6c65  le="display: fle
+00000580: 783b 616c 6967 6e2d 6974 656d 733a 2063  x;align-items: c
+00000590: 656e 7465 723b 6a75 7374 6966 792d 636f  enter;justify-co
+000005a0: 6e74 656e 743a 2063 656e 7465 723b 223e  ntent: center;">
+000005b0: 0a20 203c 696d 6720 616c 743d 2265 7861  .  <img alt="exa
+000005c0: 6d70 6c65 2061 6e69 6d61 6c2d 3122 2073  mple animal-1" s
+000005d0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+000005e0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+000005f0: 742e 636f 6d2f 6461 6e69 656c 6761 7469  t.com/danielgati
+00000600: 732f 7265 6d62 672f 6d61 7374 6572 2f65  s/rembg/master/e
+00000610: 7861 6d70 6c65 732f 616e 696d 616c 2d31  xamples/animal-1
+00000620: 2e6a 7067 2220 7769 6474 683d 2231 3030  .jpg" width="100
+00000630: 2220 2f3e 0a20 203c 696d 6720 616c 743d  " />.  <img alt=
+00000640: 2265 7861 6d70 6c65 2061 6e69 6d61 6c2d  "example animal-
+00000650: 312e 6f75 7422 2073 7263 3d22 6874 7470  1.out" src="http
+00000660: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000670: 6572 636f 6e74 656e 742e 636f 6d2f 6461  ercontent.com/da
+00000680: 6e69 656c 6761 7469 732f 7265 6d62 672f  nielgatis/rembg/
+00000690: 6d61 7374 6572 2f65 7861 6d70 6c65 732f  master/examples/
+000006a0: 616e 696d 616c 2d31 2e6f 7574 2e70 6e67  animal-1.out.png
+000006b0: 2220 7769 6474 683d 2231 3030 2220 2f3e  " width="100" />
+000006c0: 0a20 203c 696d 6720 616c 743d 2265 7861  .  <img alt="exa
+000006d0: 6d70 6c65 2061 6e69 6d61 6c2d 3222 2073  mple animal-2" s
+000006e0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+000006f0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000700: 742e 636f 6d2f 6461 6e69 656c 6761 7469  t.com/danielgati
+00000710: 732f 7265 6d62 672f 6d61 7374 6572 2f65  s/rembg/master/e
+00000720: 7861 6d70 6c65 732f 616e 696d 616c 2d32  xamples/animal-2
+00000730: 2e6a 7067 2220 7769 6474 683d 2231 3030  .jpg" width="100
+00000740: 2220 2f3e 0a20 203c 696d 6720 616c 743d  " />.  <img alt=
+00000750: 2265 7861 6d70 6c65 2061 6e69 6d61 6c2d  "example animal-
+00000760: 322e 6f75 7422 2073 7263 3d22 6874 7470  2.out" src="http
+00000770: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000780: 6572 636f 6e74 656e 742e 636f 6d2f 6461  ercontent.com/da
+00000790: 6e69 656c 6761 7469 732f 7265 6d62 672f  nielgatis/rembg/
+000007a0: 6d61 7374 6572 2f65 7861 6d70 6c65 732f  master/examples/
+000007b0: 616e 696d 616c 2d32 2e6f 7574 2e70 6e67  animal-2.out.png
+000007c0: 2220 7769 6474 683d 2231 3030 2220 2f3e  " width="100" />
+000007d0: 0a20 203c 696d 6720 616c 743d 2265 7861  .  <img alt="exa
+000007e0: 6d70 6c65 2061 6e69 6d61 6c2d 3322 2073  mple animal-3" s
+000007f0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00000800: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000810: 742e 636f 6d2f 6461 6e69 656c 6761 7469  t.com/danielgati
+00000820: 732f 7265 6d62 672f 6d61 7374 6572 2f65  s/rembg/master/e
+00000830: 7861 6d70 6c65 732f 616e 696d 616c 2d33  xamples/animal-3
+00000840: 2e6a 7067 2220 7769 6474 683d 2231 3030  .jpg" width="100
+00000850: 2220 2f3e 0a20 203c 696d 6720 616c 743d  " />.  <img alt=
+00000860: 2265 7861 6d70 6c65 2061 6e69 6d61 6c2d  "example animal-
+00000870: 332e 6f75 7422 2073 7263 3d22 6874 7470  3.out" src="http
+00000880: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000890: 6572 636f 6e74 656e 742e 636f 6d2f 6461  ercontent.com/da
+000008a0: 6e69 656c 6761 7469 732f 7265 6d62 672f  nielgatis/rembg/
+000008b0: 6d61 7374 6572 2f65 7861 6d70 6c65 732f  master/examples/
+000008c0: 616e 696d 616c 2d33 2e6f 7574 2e70 6e67  animal-3.out.png
+000008d0: 2220 7769 6474 683d 2231 3030 2220 2f3e  " width="100" />
+000008e0: 0a3c 2f70 3e0a 0a3c 7020 7374 796c 653d  .</p>..<p style=
+000008f0: 2264 6973 706c 6179 3a20 666c 6578 3b61  "display: flex;a
+00000900: 6c69 676e 2d69 7465 6d73 3a20 6365 6e74  lign-items: cent
+00000910: 6572 3b6a 7573 7469 6679 2d63 6f6e 7465  er;justify-conte
+00000920: 6e74 3a20 6365 6e74 6572 3b22 3e0a 2020  nt: center;">.  
+00000930: 3c69 6d67 2061 6c74 3d22 6578 616d 706c  <img alt="exampl
+00000940: 6520 6769 726c 2d31 2220 7372 633d 2268  e girl-1" src="h
+00000950: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000960: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000970: 2f64 616e 6965 6c67 6174 6973 2f72 656d  /danielgatis/rem
+00000980: 6267 2f6d 6173 7465 722f 6578 616d 706c  bg/master/exampl
+00000990: 6573 2f67 6972 6c2d 312e 6a70 6722 2077  es/girl-1.jpg" w
+000009a0: 6964 7468 3d22 3130 3022 202f 3e0a 2020  idth="100" />.  
+000009b0: 3c69 6d67 2061 6c74 3d22 6578 616d 706c  <img alt="exampl
+000009c0: 6520 6769 726c 2d31 2e6f 7574 2220 7372  e girl-1.out" sr
+000009d0: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+000009e0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+000009f0: 2e63 6f6d 2f64 616e 6965 6c67 6174 6973  .com/danielgatis
+00000a00: 2f72 656d 6267 2f6d 6173 7465 722f 6578  /rembg/master/ex
+00000a10: 616d 706c 6573 2f67 6972 6c2d 312e 6f75  amples/girl-1.ou
+00000a20: 742e 706e 6722 2077 6964 7468 3d22 3130  t.png" width="10
+00000a30: 3022 202f 3e0a 2020 3c69 6d67 2061 6c74  0" />.  <img alt
+00000a40: 3d22 6578 616d 706c 6520 6769 726c 2d32  ="example girl-2
+00000a50: 2220 7372 633d 2268 7474 7073 3a2f 2f72  " src="https://r
+00000a60: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00000a70: 7465 6e74 2e63 6f6d 2f64 616e 6965 6c67  tent.com/danielg
+00000a80: 6174 6973 2f72 656d 6267 2f6d 6173 7465  atis/rembg/maste
+00000a90: 722f 6578 616d 706c 6573 2f67 6972 6c2d  r/examples/girl-
+00000aa0: 322e 6a70 6722 2077 6964 7468 3d22 3130  2.jpg" width="10
+00000ab0: 3022 202f 3e0a 2020 3c69 6d67 2061 6c74  0" />.  <img alt
+00000ac0: 3d22 6578 616d 706c 6520 6769 726c 2d32  ="example girl-2
+00000ad0: 2e6f 7574 2220 7372 633d 2268 7474 7073  .out" src="https
+00000ae0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000af0: 7263 6f6e 7465 6e74 2e63 6f6d 2f64 616e  rcontent.com/dan
+00000b00: 6965 6c67 6174 6973 2f72 656d 6267 2f6d  ielgatis/rembg/m
+00000b10: 6173 7465 722f 6578 616d 706c 6573 2f67  aster/examples/g
+00000b20: 6972 6c2d 322e 6f75 742e 706e 6722 2077  irl-2.out.png" w
+00000b30: 6964 7468 3d22 3130 3022 202f 3e0a 2020  idth="100" />.  
+00000b40: 3c69 6d67 2061 6c74 3d22 6578 616d 706c  <img alt="exampl
+00000b50: 6520 6769 726c 2d33 2220 7372 633d 2268  e girl-3" src="h
+00000b60: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000b70: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000b80: 2f64 616e 6965 6c67 6174 6973 2f72 656d  /danielgatis/rem
+00000b90: 6267 2f6d 6173 7465 722f 6578 616d 706c  bg/master/exampl
+00000ba0: 6573 2f67 6972 6c2d 332e 6a70 6722 2077  es/girl-3.jpg" w
+00000bb0: 6964 7468 3d22 3130 3022 202f 3e0a 2020  idth="100" />.  
+00000bc0: 3c69 6d67 2061 6c74 3d22 6578 616d 706c  <img alt="exampl
+00000bd0: 6520 6769 726c 2d33 2e6f 7574 2220 7372  e girl-3.out" sr
+00000be0: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00000bf0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000c00: 2e63 6f6d 2f64 616e 6965 6c67 6174 6973  .com/danielgatis
+00000c10: 2f72 656d 6267 2f6d 6173 7465 722f 6578  /rembg/master/ex
+00000c20: 616d 706c 6573 2f67 6972 6c2d 332e 6f75  amples/girl-3.ou
+00000c30: 742e 706e 6722 2077 6964 7468 3d22 3130  t.png" width="10
+00000c40: 3022 202f 3e0a 3c2f 703e 0a0a 3c70 2073  0" />.</p>..<p s
+00000c50: 7479 6c65 3d22 6469 7370 6c61 793a 2066  tyle="display: f
+00000c60: 6c65 783b 616c 6967 6e2d 6974 656d 733a  lex;align-items:
+00000c70: 2063 656e 7465 723b 6a75 7374 6966 792d   center;justify-
+00000c80: 636f 6e74 656e 743a 2063 656e 7465 723b  content: center;
+00000c90: 223e 0a20 203c 696d 6720 616c 743d 2265  ">.  <img alt="e
+00000ca0: 7861 6d70 6c65 2061 6e69 6d65 2d67 6972  xample anime-gir
+00000cb0: 6c2d 3122 2073 7263 3d22 6874 7470 733a  l-1" src="https:
+00000cc0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00000cd0: 636f 6e74 656e 742e 636f 6d2f 6461 6e69  content.com/dani
+00000ce0: 656c 6761 7469 732f 7265 6d62 672f 6d61  elgatis/rembg/ma
+00000cf0: 7374 6572 2f65 7861 6d70 6c65 732f 616e  ster/examples/an
+00000d00: 696d 652d 6769 726c 2d31 2e6a 7067 2220  ime-girl-1.jpg" 
+00000d10: 7769 6474 683d 2231 3030 2220 2f3e 0a20  width="100" />. 
+00000d20: 203c 696d 6720 616c 743d 2265 7861 6d70   <img alt="examp
+00000d30: 6c65 2061 6e69 6d65 2d67 6972 6c2d 312e  le anime-girl-1.
+00000d40: 6f75 7422 2073 7263 3d22 6874 7470 733a  out" src="https:
+00000d50: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00000d60: 636f 6e74 656e 742e 636f 6d2f 6461 6e69  content.com/dani
+00000d70: 656c 6761 7469 732f 7265 6d62 672f 6d61  elgatis/rembg/ma
+00000d80: 7374 6572 2f65 7861 6d70 6c65 732f 616e  ster/examples/an
+00000d90: 696d 652d 6769 726c 2d31 2e6f 7574 2e70  ime-girl-1.out.p
+00000da0: 6e67 2220 7769 6474 683d 2231 3030 2220  ng" width="100" 
+00000db0: 2f3e 0a20 203c 696d 6720 616c 743d 2265  />.  <img alt="e
+00000dc0: 7861 6d70 6c65 2061 6e69 6d65 2d67 6972  xample anime-gir
+00000dd0: 6c2d 3222 2073 7263 3d22 6874 7470 733a  l-2" src="https:
+00000de0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00000df0: 636f 6e74 656e 742e 636f 6d2f 6461 6e69  content.com/dani
+00000e00: 656c 6761 7469 732f 7265 6d62 672f 6d61  elgatis/rembg/ma
+00000e10: 7374 6572 2f65 7861 6d70 6c65 732f 616e  ster/examples/an
+00000e20: 696d 652d 6769 726c 2d32 2e6a 7067 2220  ime-girl-2.jpg" 
+00000e30: 7769 6474 683d 2231 3030 2220 2f3e 0a20  width="100" />. 
+00000e40: 203c 696d 6720 616c 743d 2265 7861 6d70   <img alt="examp
+00000e50: 6c65 2061 6e69 6d65 2d67 6972 6c2d 322e  le anime-girl-2.
+00000e60: 6f75 7422 2073 7263 3d22 6874 7470 733a  out" src="https:
+00000e70: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00000e80: 636f 6e74 656e 742e 636f 6d2f 6461 6e69  content.com/dani
+00000e90: 656c 6761 7469 732f 7265 6d62 672f 6d61  elgatis/rembg/ma
+00000ea0: 7374 6572 2f65 7861 6d70 6c65 732f 616e  ster/examples/an
+00000eb0: 696d 652d 6769 726c 2d32 2e6f 7574 2e70  ime-girl-2.out.p
+00000ec0: 6e67 2220 7769 6474 683d 2231 3030 2220  ng" width="100" 
+00000ed0: 2f3e 0a20 203c 696d 6720 616c 743d 2265  />.  <img alt="e
+00000ee0: 7861 6d70 6c65 2061 6e69 6d65 2d67 6972  xample anime-gir
+00000ef0: 6c2d 3322 2073 7263 3d22 6874 7470 733a  l-3" src="https:
+00000f00: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00000f10: 636f 6e74 656e 742e 636f 6d2f 6461 6e69  content.com/dani
+00000f20: 656c 6761 7469 732f 7265 6d62 672f 6d61  elgatis/rembg/ma
+00000f30: 7374 6572 2f65 7861 6d70 6c65 732f 616e  ster/examples/an
+00000f40: 696d 652d 6769 726c 2d33 2e6a 7067 2220  ime-girl-3.jpg" 
+00000f50: 7769 6474 683d 2231 3030 2220 2f3e 0a20  width="100" />. 
+00000f60: 203c 696d 6720 616c 743d 2265 7861 6d70   <img alt="examp
+00000f70: 6c65 2061 6e69 6d65 2d67 6972 6c2d 332e  le anime-girl-3.
+00000f80: 6f75 7422 2073 7263 3d22 6874 7470 733a  out" src="https:
+00000f90: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00000fa0: 636f 6e74 656e 742e 636f 6d2f 6461 6e69  content.com/dani
+00000fb0: 656c 6761 7469 732f 7265 6d62 672f 6d61  elgatis/rembg/ma
+00000fc0: 7374 6572 2f65 7861 6d70 6c65 732f 616e  ster/examples/an
+00000fd0: 696d 652d 6769 726c 2d33 2e6f 7574 2e70  ime-girl-3.out.p
+00000fe0: 6e67 2220 7769 6474 683d 2231 3030 2220  ng" width="100" 
+00000ff0: 2f3e 0a3c 2f70 3e0a 0a2a 2a49 6620 7468  />.</p>..**If th
+00001000: 6973 2070 726f 6a65 6374 2068 6173 2068  is project has h
+00001010: 656c 7065 6420 796f 752c 2070 6c65 6173  elped you, pleas
+00001020: 6520 636f 6e73 6964 6572 206d 616b 696e  e consider makin
+00001030: 6720 6120 5b64 6f6e 6174 696f 6e5d 2868  g a [donation](h
+00001040: 7474 7073 3a2f 2f77 7777 2e62 7579 6d65  ttps://www.buyme
+00001050: 6163 6f66 6665 652e 636f 6d2f 6461 6e69  acoffee.com/dani
+00001060: 656c 6761 7469 7329 2e2a 2a0a 0a23 2320  elgatis).**..## 
+00001070: 5370 6f6e 736f 720a 0a3c 7461 626c 653e  Sponsor..<table>
+00001080: 0a20 203c 7472 3e0a 2020 2020 3c74 6420  .  <tr>.    <td 
+00001090: 616c 6967 6e3d 2263 656e 7465 7222 2076  align="center" v
+000010a0: 6572 7469 6361 6c2d 616c 6967 6e3d 2263  ertical-align="c
+000010b0: 656e 7465 7222 3e0a 2020 2020 2020 3c61  enter">.      <a
+000010c0: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+000010d0: 686f 746f 726f 6f6d 2e63 6f6d 2f61 7069  hotoroom.com/api
+000010e0: 2f72 656d 6f76 652d 6261 636b 6772 6f75  /remove-backgrou
+000010f0: 6e64 3f75 746d 5f73 6f75 7263 653d 7265  nd?utm_source=re
+00001100: 6d62 6726 7574 6d5f 6d65 6469 756d 3d67  mbg&utm_medium=g
+00001110: 6974 6875 625f 7765 6270 6167 6526 7574  ithub_webpage&ut
+00001120: 6d5f 6361 6d70 6169 676e 3d73 706f 6e73  m_campaign=spons
+00001130: 6f72 2220 3e0a 2020 2020 2020 2020 3c69  or" >.        <i
+00001140: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00001150: 666f 6e74 2d63 646e 2e70 686f 746f 726f  font-cdn.photoro
+00001160: 6f6d 2e63 6f6d 2f6d 6564 6961 2f61 7069  om.com/media/api
+00001170: 2d6c 6f67 6f2e 706e 6722 2077 6964 7468  -logo.png" width
+00001180: 3d22 3132 3070 783b 2220 616c 743d 2255  ="120px;" alt="U
+00001190: 6e73 706c 6173 6822 202f 3e0a 2020 2020  nsplash" />.    
+000011a0: 2020 3c2f 613e 0a20 2020 203c 2f74 643e    </a>.    </td>
+000011b0: 0a20 2020 203c 7464 2061 6c69 676e 3d22  .    <td align="
+000011c0: 6365 6e74 6572 2220 7665 7274 6963 616c  center" vertical
+000011d0: 2d61 6c69 676e 3d22 6365 6e74 6572 223e  -align="center">
+000011e0: 0a20 2020 2020 203c 623e 5068 6f74 6f52  .      <b>PhotoR
+000011f0: 6f6f 6d20 5265 6d6f 7665 2042 6163 6b67  oom Remove Backg
+00001200: 726f 756e 6420 4150 493c 2f62 3e0a 2020  round API</b>.  
+00001210: 2020 2020 3c62 7220 2f3e 0a20 2020 2020      <br />.     
+00001220: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00001230: 2f2f 7068 6f74 6f72 6f6f 6d2e 636f 6d2f  //photoroom.com/
+00001240: 6170 692f 7265 6d6f 7665 2d62 6163 6b67  api/remove-backg
+00001250: 726f 756e 643f 7574 6d5f 736f 7572 6365  round?utm_source
+00001260: 3d72 656d 6267 2675 746d 5f6d 6564 6975  =rembg&utm_mediu
+00001270: 6d3d 6769 7468 7562 5f77 6562 7061 6765  m=github_webpage
+00001280: 2675 746d 5f63 616d 7061 6967 6e3d 7370  &utm_campaign=sp
+00001290: 6f6e 736f 7222 3e68 7474 7073 3a2f 2f70  onsor">https://p
+000012a0: 686f 746f 726f 6f6d 2e63 6f6d 2f61 7069  hotoroom.com/api
+000012b0: 3c2f 613e 0a20 2020 2020 203c 6272 202f  </a>.      <br /
+000012c0: 3e0a 2020 2020 2020 3c70 2077 6964 7468  >.      <p width
+000012d0: 3d22 3230 3070 7822 3e0a 2020 2020 2020  ="200px">.      
+000012e0: 2020 4661 7374 2061 6e64 2061 6363 7572    Fast and accur
+000012f0: 6174 6520 6261 636b 6772 6f75 6e64 2072  ate background r
+00001300: 656d 6f76 6572 2041 5049 3c62 722f 3e0a  emover API<br/>.
+00001310: 2020 2020 2020 3c2f 703e 0a20 2020 203c        </p>.    <
+00001320: 2f74 643e 0a20 203c 2f74 723e 0a3c 2f74  /td>.  </tr>.</t
+00001330: 6162 6c65 3e0a 0a23 2320 5265 7175 6972  able>..## Requir
+00001340: 656d 656e 7473 0a0a 6060 6074 6578 740a  ements..```text.
+00001350: 7079 7468 6f6e 3a20 3e33 2e37 2c20 3c33  python: >3.7, <3
+00001360: 2e31 330a 6060 600a 0a23 2320 496e 7374  .13.```..## Inst
+00001370: 616c 6c61 7469 6f6e 0a0a 4350 5520 7375  allation..CPU su
+00001380: 7070 6f72 743a 0a0a 6060 6062 6173 680a  pport:..```bash.
+00001390: 7069 7020 696e 7374 616c 6c20 7265 6d62  pip install remb
+000013a0: 6720 2320 666f 7220 6c69 6272 6172 790a  g # for library.
+000013b0: 7069 7020 696e 7374 616c 6c20 7265 6d62  pip install remb
+000013c0: 675b 636c 695d 2023 2066 6f72 206c 6962  g[cli] # for lib
+000013d0: 7261 7279 202b 2063 6c69 0a60 6060 0a0a  rary + cli.```..
+000013e0: 4750 5520 7375 7070 6f72 743a 0a0a 4669  GPU support:..Fi
+000013f0: 7273 7420 6f66 2061 6c6c 2c20 796f 7520  rst of all, you 
+00001400: 6e65 6564 2074 6f20 6368 6563 6b20 6966  need to check if
+00001410: 2079 6f75 7220 7379 7374 656d 2073 7570   your system sup
+00001420: 706f 7274 7320 7468 6520 606f 6e6e 7872  ports the `onnxr
+00001430: 756e 7469 6d65 2d67 7075 602e 0a0a 476f  untime-gpu`...Go
+00001440: 2074 6f20 3c68 7474 7073 3a2f 2f6f 6e6e   to <https://onn
+00001450: 7872 756e 7469 6d65 2e61 693e 2061 6e64  xruntime.ai> and
+00001460: 2063 6865 636b 2074 6865 2069 6e73 7461   check the insta
+00001470: 6c6c 6174 696f 6e20 6d61 7472 6978 2e0a  llation matrix..
+00001480: 0a3c 7020 7374 796c 653d 2264 6973 706c  .<p style="displ
+00001490: 6179 3a20 666c 6578 3b61 6c69 676e 2d69  ay: flex;align-i
+000014a0: 7465 6d73 3a20 6365 6e74 6572 3b6a 7573  tems: center;jus
+000014b0: 7469 6679 2d63 6f6e 7465 6e74 3a20 6365  tify-content: ce
+000014c0: 6e74 6572 3b22 3e0a 2020 3c69 6d67 2061  nter;">.  <img a
+000014d0: 6c74 3d22 6f6e 6e78 7275 6e74 696d 652d  lt="onnxruntime-
+000014e0: 696e 7374 616c 6c61 7469 6f6e 2d6d 6174  installation-mat
+000014f0: 7269 7822 2073 7263 3d22 6874 7470 733a  rix" src="https:
+00001500: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00001510: 636f 6e74 656e 742e 636f 6d2f 6461 6e69  content.com/dani
+00001520: 656c 6761 7469 732f 7265 6d62 672f 6d61  elgatis/rembg/ma
+00001530: 7374 6572 2f6f 6e6e 7872 756e 7469 6d65  ster/onnxruntime
+00001540: 2d69 6e73 7461 6c6c 6174 696f 6e2d 6d61  -installation-ma
+00001550: 7472 6978 2e70 6e67 2220 7769 6474 683d  trix.png" width=
+00001560: 2234 3030 2220 2f3e 0a3c 2f70 3e0a 0a49  "400" />.</p>..I
+00001570: 6620 7965 732c 206a 7573 7420 7275 6e3a  f yes, just run:
+00001580: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
+00001590: 7374 616c 6c20 7265 6d62 675b 6770 755d  stall rembg[gpu]
+000015a0: 2023 2066 6f72 206c 6962 7261 7279 0a70   # for library.p
+000015b0: 6970 2069 6e73 7461 6c6c 2072 656d 6267  ip install rembg
+000015c0: 5b67 7075 2c63 6c69 5d20 2320 666f 7220  [gpu,cli] # for 
+000015d0: 6c69 6272 6172 7920 2b20 636c 690a 6060  library + cli.``
+000015e0: 600a 0a23 2320 5573 6167 6520 6173 2061  `..## Usage as a
+000015f0: 2063 6c69 0a0a 4166 7465 7220 7468 6520   cli..After the 
+00001600: 696e 7374 616c 6c61 7469 6f6e 2073 7465  installation ste
+00001610: 7020 796f 7520 6361 6e20 7573 6520 7265  p you can use re
+00001620: 6d62 6720 6a75 7374 2074 7970 696e 6720  mbg just typing 
+00001630: 6072 656d 6267 6020 696e 2079 6f75 7220  `rembg` in your 
+00001640: 7465 726d 696e 616c 2077 696e 646f 772e  terminal window.
+00001650: 0a0a 5468 6520 6072 656d 6267 6020 636f  ..The `rembg` co
+00001660: 6d6d 616e 6420 6861 7320 3420 7375 6263  mmand has 4 subc
+00001670: 6f6d 6d61 6e64 732c 206f 6e65 2066 6f72  ommands, one for
+00001680: 2065 6163 6820 696e 7075 7420 7479 7065   each input type
+00001690: 3a0a 0a2d 2060 6960 2066 6f72 2066 696c  :..- `i` for fil
+000016a0: 6573 0a2d 2060 7060 2066 6f72 2066 6f6c  es.- `p` for fol
+000016b0: 6465 7273 0a2d 2060 7360 2066 6f72 2068  ders.- `s` for h
+000016c0: 7474 7020 7365 7276 6572 0a2d 2060 6260  ttp server.- `b`
+000016d0: 2066 6f72 2052 4742 3234 2070 6978 656c   for RGB24 pixel
+000016e0: 2062 696e 6172 7920 7374 7265 616d 0a0a   binary stream..
+000016f0: 596f 7520 6361 6e20 6765 7420 6865 6c70  You can get help
+00001700: 2061 626f 7574 2074 6865 206d 6169 6e20   about the main 
+00001710: 636f 6d6d 616e 6420 7573 696e 673a 0a0a  command using:..
+00001720: 6060 6073 6865 6c6c 0a72 656d 6267 202d  ```shell.rembg -
+00001730: 2d68 656c 700a 6060 600a 0a41 7320 7765  -help.```..As we
+00001740: 6c6c 2c20 6162 6f75 7420 616c 6c20 7468  ll, about all th
+00001750: 6520 7375 6263 6f6d 6d61 6e64 7320 7573  e subcommands us
+00001760: 696e 673a 0a0a 6060 6073 6865 6c6c 0a72  ing:..```shell.r
+00001770: 656d 6267 203c 434f 4d4d 414e 443e 202d  embg <COMMAND> -
+00001780: 2d68 656c 700a 6060 600a 0a23 2323 2072  -help.```..### r
+00001790: 656d 6267 2060 6960 0a0a 5573 6564 2077  embg `i`..Used w
+000017a0: 6865 6e20 696e 7075 7420 616e 6420 6f75  hen input and ou
+000017b0: 7470 7574 2061 7265 2066 696c 6573 2e0a  tput are files..
+000017c0: 0a52 656d 6f76 6520 7468 6520 6261 636b  .Remove the back
+000017d0: 6772 6f75 6e64 2066 726f 6d20 6120 7265  ground from a re
+000017e0: 6d6f 7465 2069 6d61 6765 0a0a 6060 6073  mote image..```s
+000017f0: 6865 6c6c 0a63 7572 6c20 2d73 2068 7474  hell.curl -s htt
+00001800: 703a 2f2f 696e 7075 742e 706e 6720 7c20  p://input.png | 
+00001810: 7265 6d62 6720 6920 3e20 6f75 7470 7574  rembg i > output
+00001820: 2e70 6e67 0a60 6060 0a0a 5265 6d6f 7665  .png.```..Remove
+00001830: 2074 6865 2062 6163 6b67 726f 756e 6420   the background 
+00001840: 6672 6f6d 2061 206c 6f63 616c 2066 696c  from a local fil
+00001850: 650a 0a60 6060 7368 656c 6c0a 7265 6d62  e..```shell.remb
+00001860: 6720 6920 7061 7468 2f74 6f2f 696e 7075  g i path/to/inpu
+00001870: 742e 706e 6720 7061 7468 2f74 6f2f 6f75  t.png path/to/ou
+00001880: 7470 7574 2e70 6e67 0a60 6060 0a0a 5265  tput.png.```..Re
+00001890: 6d6f 7665 2074 6865 2062 6163 6b67 726f  move the backgro
+000018a0: 756e 6420 7370 6563 6966 7969 6e67 2061  und specifying a
+000018b0: 206d 6f64 656c 0a0a 6060 6073 6865 6c6c   model..```shell
+000018c0: 0a72 656d 6267 2069 202d 6d20 7532 6e65  .rembg i -m u2ne
+000018d0: 7470 2070 6174 682f 746f 2f69 6e70 7574  tp path/to/input
+000018e0: 2e70 6e67 2070 6174 682f 746f 2f6f 7574  .png path/to/out
+000018f0: 7075 742e 706e 670a 6060 600a 0a52 656d  put.png.```..Rem
+00001900: 6f76 6520 7468 6520 6261 636b 6772 6f75  ove the backgrou
+00001910: 6e64 2072 6574 7572 6e69 6e67 206f 6e6c  nd returning onl
+00001920: 7920 7468 6520 6d61 736b 0a0a 6060 6073  y the mask..```s
+00001930: 6865 6c6c 0a72 656d 6267 2069 202d 6f6d  hell.rembg i -om
+00001940: 2070 6174 682f 746f 2f69 6e70 7574 2e70   path/to/input.p
+00001950: 6e67 2070 6174 682f 746f 2f6f 7574 7075  ng path/to/outpu
+00001960: 742e 706e 670a 6060 600a 0a52 656d 6f76  t.png.```..Remov
+00001970: 6520 7468 6520 6261 636b 6772 6f75 6e64  e the background
+00001980: 2061 7070 6c79 696e 6720 616e 2061 6c70   applying an alp
+00001990: 6861 206d 6174 7469 6e67 0a0a 6060 6073  ha matting..```s
+000019a0: 6865 6c6c 0a72 656d 6267 2069 202d 6120  hell.rembg i -a 
+000019b0: 7061 7468 2f74 6f2f 696e 7075 742e 706e  path/to/input.pn
+000019c0: 6720 7061 7468 2f74 6f2f 6f75 7470 7574  g path/to/output
+000019d0: 2e70 6e67 0a60 6060 0a0a 5061 7373 696e  .png.```..Passin
+000019e0: 6720 6578 7472 6173 2070 6172 616d 6574  g extras paramet
+000019f0: 6572 730a 0a60 6060 7368 656c 6c0a 5341  ers..```shell.SA
+00001a00: 4d20 6578 616d 706c 650a 0a72 656d 6267  M example..rembg
+00001a10: 2069 202d 6d20 7361 6d20 2d78 2027 7b20   i -m sam -x '{ 
+00001a20: 2273 616d 5f70 726f 6d70 7422 3a20 5b7b  "sam_prompt": [{
+00001a30: 2274 7970 6522 3a20 2270 6f69 6e74 222c  "type": "point",
+00001a40: 2022 6461 7461 223a 205b 3732 342c 2037   "data": [724, 7
+00001a50: 3430 5d2c 2022 6c61 6265 6c22 3a20 317d  40], "label": 1}
+00001a60: 5d20 7d27 2065 7861 6d70 6c65 732f 706c  ] }' examples/pl
+00001a70: 616e 7473 2d31 2e6a 7067 2065 7861 6d70  ants-1.jpg examp
+00001a80: 6c65 732f 706c 616e 7473 2d31 2e6f 7574  les/plants-1.out
+00001a90: 2e70 6e67 0a60 6060 0a0a 6060 6073 6865  .png.```..```she
+00001aa0: 6c6c 0a43 7573 746f 6d20 6d6f 6465 6c20  ll.Custom model 
+00001ab0: 6578 616d 706c 650a 0a72 656d 6267 2069  example..rembg i
+00001ac0: 202d 6d20 7532 6e65 745f 6375 7374 6f6d   -m u2net_custom
+00001ad0: 202d 7820 277b 226d 6f64 656c 5f70 6174   -x '{"model_pat
+00001ae0: 6822 3a20 227e 2f2e 7532 6e65 742f 7532  h": "~/.u2net/u2
+00001af0: 6e65 742e 6f6e 6e78 227d 2720 7061 7468  net.onnx"}' path
+00001b00: 2f74 6f2f 696e 7075 742e 706e 6720 7061  /to/input.png pa
+00001b10: 7468 2f74 6f2f 6f75 7470 7574 2e70 6e67  th/to/output.png
+00001b20: 0a60 6060 0a0a 2323 2320 7265 6d62 6720  .```..### rembg 
+00001b30: 6070 600a 0a55 7365 6420 7768 656e 2069  `p`..Used when i
+00001b40: 6e70 7574 2061 6e64 206f 7574 7075 7420  nput and output 
+00001b50: 6172 6520 666f 6c64 6572 732e 0a0a 5265  are folders...Re
+00001b60: 6d6f 7665 2074 6865 2062 6163 6b67 726f  move the backgro
+00001b70: 756e 6420 6672 6f6d 2061 6c6c 2069 6d61  und from all ima
+00001b80: 6765 7320 696e 2061 2066 6f6c 6465 720a  ges in a folder.
+00001b90: 0a60 6060 7368 656c 6c0a 7265 6d62 6720  .```shell.rembg 
+00001ba0: 7020 7061 7468 2f74 6f2f 696e 7075 7420  p path/to/input 
+00001bb0: 7061 7468 2f74 6f2f 6f75 7470 7574 0a60  path/to/output.`
+00001bc0: 6060 0a0a 5361 6d65 2061 7320 6265 666f  ``..Same as befo
+00001bd0: 7265 2c20 6275 7420 7761 7463 6869 6e67  re, but watching
+00001be0: 2066 6f72 206e 6577 2f63 6861 6e67 6564   for new/changed
+00001bf0: 2066 696c 6573 2074 6f20 7072 6f63 6573   files to proces
+00001c00: 730a 0a60 6060 7368 656c 6c0a 7265 6d62  s..```shell.remb
+00001c10: 6720 7020 2d77 2070 6174 682f 746f 2f69  g p -w path/to/i
+00001c20: 6e70 7574 2070 6174 682f 746f 2f6f 7574  nput path/to/out
+00001c30: 7075 740a 6060 600a 0a23 2323 2072 656d  put.```..### rem
+00001c40: 6267 2060 7360 0a0a 5573 6564 2074 6f20  bg `s`..Used to 
+00001c50: 7374 6172 7420 6874 7470 2073 6572 7665  start http serve
+00001c60: 722e 0a0a 6060 6073 6865 6c6c 0a72 656d  r...```shell.rem
+00001c70: 6267 2073 202d 2d68 6f73 7420 302e 302e  bg s --host 0.0.
+00001c80: 302e 3020 2d2d 706f 7274 2037 3030 3020  0.0 --port 7000 
+00001c90: 2d2d 6c6f 675f 6c65 7665 6c20 696e 666f  --log_level info
+00001ca0: 0a60 6060 0a0a 546f 2073 6565 2074 6865  .```..To see the
+00001cb0: 2063 6f6d 706c 6574 6520 656e 6470 6f69   complete endpoi
+00001cc0: 6e74 7320 646f 6375 6d65 6e74 6174 696f  nts documentatio
+00001cd0: 6e2c 2067 6f20 746f 3a20 6068 7474 703a  n, go to: `http:
+00001ce0: 2f2f 6c6f 6361 6c68 6f73 743a 3730 3030  //localhost:7000
+00001cf0: 2f61 7069 602e 0a0a 5265 6d6f 7665 2074  /api`...Remove t
+00001d00: 6865 2062 6163 6b67 726f 756e 6420 6672  he background fr
+00001d10: 6f6d 2061 6e20 696d 6167 6520 7572 6c0a  om an image url.
+00001d20: 0a60 6060 7368 656c 6c0a 6375 726c 202d  .```shell.curl -
+00001d30: 7320 2268 7474 703a 2f2f 6c6f 6361 6c68  s "http://localh
+00001d40: 6f73 743a 3730 3030 2f61 7069 2f72 656d  ost:7000/api/rem
+00001d50: 6f76 653f 7572 6c3d 6874 7470 3a2f 2f69  ove?url=http://i
+00001d60: 6e70 7574 2e70 6e67 2220 2d6f 206f 7574  nput.png" -o out
+00001d70: 7075 742e 706e 670a 6060 600a 0a52 656d  put.png.```..Rem
+00001d80: 6f76 6520 7468 6520 6261 636b 6772 6f75  ove the backgrou
+00001d90: 6e64 2066 726f 6d20 616e 2075 706c 6f61  nd from an uploa
+00001da0: 6465 6420 696d 6167 650a 0a60 6060 7368  ded image..```sh
+00001db0: 656c 6c0a 6375 726c 202d 7320 2d46 2066  ell.curl -s -F f
+00001dc0: 696c 653d 402f 7061 7468 2f74 6f2f 696e  ile=@/path/to/in
+00001dd0: 7075 742e 6a70 6720 2268 7474 703a 2f2f  put.jpg "http://
+00001de0: 6c6f 6361 6c68 6f73 743a 3730 3030 2f61  localhost:7000/a
+00001df0: 7069 2f72 656d 6f76 6522 2020 2d6f 206f  pi/remove"  -o o
+00001e00: 7574 7075 742e 706e 670a 6060 600a 0a23  utput.png.```..#
+00001e10: 2323 2072 656d 6267 2060 6260 0a0a 5072  ## rembg `b`..Pr
+00001e20: 6f63 6573 7320 6120 7365 7175 656e 6365  ocess a sequence
+00001e30: 206f 6620 5247 4232 3420 696d 6167 6573   of RGB24 images
+00001e40: 2066 726f 6d20 7374 6469 6e2e 2054 6869   from stdin. Thi
+00001e50: 7320 6973 2069 6e74 656e 6465 6420 746f  s is intended to
+00001e60: 2062 6520 7573 6564 2077 6974 6820 616e   be used with an
+00001e70: 6f74 6865 7220 7072 6f67 7261 6d2c 2073  other program, s
+00001e80: 7563 6820 6173 2046 464d 5045 472c 2074  uch as FFMPEG, t
+00001e90: 6861 7420 6f75 7470 7574 7320 5247 4232  hat outputs RGB2
+00001ea0: 3420 7069 7865 6c20 6461 7461 2074 6f20  4 pixel data to 
+00001eb0: 7374 646f 7574 2c20 7768 6963 6820 6973  stdout, which is
+00001ec0: 2070 6970 6564 2069 6e74 6f20 7468 6520   piped into the 
+00001ed0: 7374 6469 6e20 6f66 2074 6869 7320 7072  stdin of this pr
+00001ee0: 6f67 7261 6d2c 2061 6c74 686f 7567 6820  ogram, although 
+00001ef0: 6e6f 7468 696e 6720 7072 6576 656e 7473  nothing prevents
+00001f00: 2079 6f75 2066 726f 6d20 6d61 6e75 616c   you from manual
+00001f10: 6c79 2074 7970 696e 6720 696e 2069 6d61  ly typing in ima
+00001f20: 6765 7320 6174 2073 7464 696e 2e0a 0a60  ges at stdin...`
+00001f30: 6060 7368 656c 6c0a 7265 6d62 6720 6220  ``shell.rembg b 
+00001f40: 696d 6167 655f 7769 6474 6820 696d 6167  image_width imag
+00001f50: 655f 6865 6967 6874 202d 6f20 6f75 7470  e_height -o outp
+00001f60: 7574 5f73 7065 6369 6669 6572 0a60 6060  ut_specifier.```
+00001f70: 0a0a 4172 6775 6d65 6e74 733a 0a0a 2d20  ..Arguments:..- 
+00001f80: 696d 6167 655f 7769 6474 6820 3a20 7769  image_width : wi
+00001f90: 6474 6820 6f66 2069 6e70 7574 2069 6d61  dth of input ima
+00001fa0: 6765 2873 290a 2d20 696d 6167 655f 6865  ge(s).- image_he
+00001fb0: 6967 6874 203a 2068 6569 6768 7420 6f66  ight : height of
+00001fc0: 2069 6e70 7574 2069 6d61 6765 2873 290a   input image(s).
+00001fd0: 2d20 6f75 7470 7574 5f73 7065 6369 6669  - output_specifi
+00001fe0: 6572 3a20 7072 696e 7466 2d73 7479 6c65  er: printf-style
+00001ff0: 2073 7065 6369 6669 6572 2066 6f72 206f   specifier for o
+00002000: 7574 7075 7420 6669 6c65 6e61 6d65 732c  utput filenames,
+00002010: 2066 6f72 2065 7861 6d70 6c65 2069 6620   for example if 
+00002020: 606f 7574 7075 742d 2530 3375 2e70 6e67  `output-%03u.png
+00002030: 602c 2074 6865 6e20 6f75 7470 7574 2066  `, then output f
+00002040: 696c 6573 2077 696c 6c20 6265 206e 616d  iles will be nam
+00002050: 6564 2060 6f75 7470 7574 2d30 3030 2e70  ed `output-000.p
+00002060: 6e67 602c 2060 6f75 7470 7574 2d30 3031  ng`, `output-001
+00002070: 2e70 6e67 602c 2060 6f75 7470 7574 2d30  .png`, `output-0
+00002080: 3032 2e70 6e67 602c 2065 7463 2e20 4f75  02.png`, etc. Ou
+00002090: 7470 7574 2066 696c 6573 2077 696c 6c20  tput files will 
+000020a0: 6265 2073 6176 6564 2069 6e20 504e 4720  be saved in PNG 
+000020b0: 666f 726d 6174 2072 6567 6172 646c 6573  format regardles
+000020c0: 7320 6f66 2074 6865 2065 7874 656e 7369  s of the extensi
+000020d0: 6f6e 2073 7065 6369 6669 6564 2e20 596f  on specified. Yo
+000020e0: 7520 6361 6e20 6f6d 6974 2069 7420 746f  u can omit it to
+000020f0: 2077 7269 7465 2072 6573 756c 7473 2074   write results t
+00002100: 6f20 7374 646f 7574 2e0a 0a45 7861 6d70  o stdout...Examp
+00002110: 6c65 2075 7361 6765 2077 6974 6820 4646  le usage with FF
+00002120: 4d50 4547 3a0a 0a60 6060 7368 656c 6c0a  MPEG:..```shell.
+00002130: 6666 6d70 6567 202d 6920 696e 7075 742e  ffmpeg -i input.
+00002140: 6d70 3420 2d73 7320 3130 202d 616e 202d  mp4 -ss 10 -an -
+00002150: 6620 7261 7776 6964 656f 202d 7069 785f  f rawvideo -pix_
+00002160: 666d 7420 7267 6232 3420 7069 7065 3a31  fmt rgb24 pipe:1
+00002170: 207c 2072 656d 6267 2062 2031 3238 3020   | rembg b 1280 
+00002180: 3732 3020 2d6f 2066 6f6c 6465 722f 6f75  720 -o folder/ou
+00002190: 7470 7574 2d25 3033 752e 706e 670a 6060  tput-%03u.png.``
+000021a0: 600a 0a54 6865 2077 6964 7468 2061 6e64  `..The width and
+000021b0: 2068 6569 6768 7420 7661 6c75 6573 206d   height values m
+000021c0: 7573 7420 6d61 7463 6820 7468 6520 6469  ust match the di
+000021d0: 6d65 6e73 696f 6e20 6f66 206f 7574 7075  mension of outpu
+000021e0: 7420 696d 6167 6573 2066 726f 6d20 4646  t images from FF
+000021f0: 4d50 4547 2e20 4e6f 7465 2066 6f72 2046  MPEG. Note for F
+00002200: 464d 5045 472c 2074 6865 2022 602d 616e  FMPEG, the "`-an
+00002210: 202d 6620 7261 7776 6964 656f 202d 7069   -f rawvideo -pi
+00002220: 785f 666d 7420 7267 6232 3420 7069 7065  x_fmt rgb24 pipe
+00002230: 3a31 6022 2070 6172 7420 6973 2072 6571  :1`" part is req
+00002240: 7569 7265 6420 666f 7220 7468 6520 7768  uired for the wh
+00002250: 6f6c 6520 7468 696e 6720 746f 2077 6f72  ole thing to wor
+00002260: 6b2e 0a0a 2323 2055 7361 6765 2061 7320  k...## Usage as 
+00002270: 6120 6c69 6272 6172 790a 0a49 6e70 7574  a library..Input
+00002280: 2061 6e64 206f 7574 7075 7420 6173 2062   and output as b
+00002290: 7974 6573 0a0a 6060 6070 7974 686f 6e0a  ytes..```python.
+000022a0: 6672 6f6d 2072 656d 6267 2069 6d70 6f72  from rembg impor
+000022b0: 7420 7265 6d6f 7665 0a0a 696e 7075 745f  t remove..input_
+000022c0: 7061 7468 203d 2027 696e 7075 742e 706e  path = 'input.pn
+000022d0: 6727 0a6f 7574 7075 745f 7061 7468 203d  g'.output_path =
+000022e0: 2027 6f75 7470 7574 2e70 6e67 270a 0a77   'output.png'..w
+000022f0: 6974 6820 6f70 656e 2869 6e70 7574 5f70  ith open(input_p
+00002300: 6174 682c 2027 7262 2729 2061 7320 693a  ath, 'rb') as i:
+00002310: 0a20 2020 2077 6974 6820 6f70 656e 286f  .    with open(o
+00002320: 7574 7075 745f 7061 7468 2c20 2777 6227  utput_path, 'wb'
+00002330: 2920 6173 206f 3a0a 2020 2020 2020 2020  ) as o:.        
+00002340: 696e 7075 7420 3d20 692e 7265 6164 2829  input = i.read()
+00002350: 0a20 2020 2020 2020 206f 7574 7075 7420  .        output 
+00002360: 3d20 7265 6d6f 7665 2869 6e70 7574 290a  = remove(input).
+00002370: 2020 2020 2020 2020 6f2e 7772 6974 6528          o.write(
+00002380: 6f75 7470 7574 290a 6060 600a 0a49 6e70  output).```..Inp
+00002390: 7574 2061 6e64 206f 7574 7075 7420 6173  ut and output as
+000023a0: 2061 2050 494c 2069 6d61 6765 0a0a 6060   a PIL image..``
+000023b0: 6070 7974 686f 6e0a 6672 6f6d 2072 656d  `python.from rem
+000023c0: 6267 2069 6d70 6f72 7420 7265 6d6f 7665  bg import remove
+000023d0: 0a66 726f 6d20 5049 4c20 696d 706f 7274  .from PIL import
+000023e0: 2049 6d61 6765 0a0a 696e 7075 745f 7061   Image..input_pa
+000023f0: 7468 203d 2027 696e 7075 742e 706e 6727  th = 'input.png'
+00002400: 0a6f 7574 7075 745f 7061 7468 203d 2027  .output_path = '
+00002410: 6f75 7470 7574 2e70 6e67 270a 0a69 6e70  output.png'..inp
+00002420: 7574 203d 2049 6d61 6765 2e6f 7065 6e28  ut = Image.open(
+00002430: 696e 7075 745f 7061 7468 290a 6f75 7470  input_path).outp
+00002440: 7574 203d 2072 656d 6f76 6528 696e 7075  ut = remove(inpu
+00002450: 7429 0a6f 7574 7075 742e 7361 7665 286f  t).output.save(o
+00002460: 7574 7075 745f 7061 7468 290a 6060 600a  utput_path).```.
+00002470: 0a49 6e70 7574 2061 6e64 206f 7574 7075  .Input and outpu
+00002480: 7420 6173 2061 206e 756d 7079 2061 7272  t as a numpy arr
+00002490: 6179 0a0a 6060 6070 7974 686f 6e0a 6672  ay..```python.fr
+000024a0: 6f6d 2072 656d 6267 2069 6d70 6f72 7420  om rembg import 
+000024b0: 7265 6d6f 7665 0a69 6d70 6f72 7420 6376  remove.import cv
+000024c0: 320a 0a69 6e70 7574 5f70 6174 6820 3d20  2..input_path = 
+000024d0: 2769 6e70 7574 2e70 6e67 270a 6f75 7470  'input.png'.outp
+000024e0: 7574 5f70 6174 6820 3d20 276f 7574 7075  ut_path = 'outpu
+000024f0: 742e 706e 6727 0a0a 696e 7075 7420 3d20  t.png'..input = 
+00002500: 6376 322e 696d 7265 6164 2869 6e70 7574  cv2.imread(input
+00002510: 5f70 6174 6829 0a6f 7574 7075 7420 3d20  _path).output = 
+00002520: 7265 6d6f 7665 2869 6e70 7574 290a 6376  remove(input).cv
+00002530: 322e 696d 7772 6974 6528 6f75 7470 7574  2.imwrite(output
+00002540: 5f70 6174 682c 206f 7574 7075 7429 0a60  _path, output).`
+00002550: 6060 0a0a 486f 7720 746f 2069 7465 7261  ``..How to itera
+00002560: 7465 206f 7665 7220 6669 6c65 7320 696e  te over files in
+00002570: 2061 2070 6572 666f 726d 6174 6963 2077   a performatic w
+00002580: 6179 0a0a 6060 6070 7974 686f 6e0a 6672  ay..```python.fr
+00002590: 6f6d 2070 6174 686c 6962 2069 6d70 6f72  om pathlib impor
+000025a0: 7420 5061 7468 0a66 726f 6d20 7265 6d62  t Path.from remb
+000025b0: 6720 696d 706f 7274 2072 656d 6f76 652c  g import remove,
+000025c0: 206e 6577 5f73 6573 7369 6f6e 0a0a 7365   new_session..se
+000025d0: 7373 696f 6e20 3d20 6e65 775f 7365 7373  ssion = new_sess
+000025e0: 696f 6e28 290a 0a66 6f72 2066 696c 6520  ion()..for file 
+000025f0: 696e 2050 6174 6828 2770 6174 682f 746f  in Path('path/to
+00002600: 2f66 6f6c 6465 7227 292e 676c 6f62 2827  /folder').glob('
+00002610: 2a2e 706e 6727 293a 0a20 2020 2069 6e70  *.png'):.    inp
+00002620: 7574 5f70 6174 6820 3d20 7374 7228 6669  ut_path = str(fi
+00002630: 6c65 290a 2020 2020 6f75 7470 7574 5f70  le).    output_p
+00002640: 6174 6820 3d20 7374 7228 6669 6c65 2e70  ath = str(file.p
+00002650: 6172 656e 7420 2f20 2866 696c 652e 7374  arent / (file.st
+00002660: 656d 202b 2022 2e6f 7574 2e70 6e67 2229  em + ".out.png")
+00002670: 290a 0a20 2020 2077 6974 6820 6f70 656e  )..    with open
+00002680: 2869 6e70 7574 5f70 6174 682c 2027 7262  (input_path, 'rb
+00002690: 2729 2061 7320 693a 0a20 2020 2020 2020  ') as i:.       
+000026a0: 2077 6974 6820 6f70 656e 286f 7574 7075   with open(outpu
+000026b0: 745f 7061 7468 2c20 2777 6227 2920 6173  t_path, 'wb') as
+000026c0: 206f 3a0a 2020 2020 2020 2020 2020 2020   o:.            
+000026d0: 696e 7075 7420 3d20 692e 7265 6164 2829  input = i.read()
+000026e0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+000026f0: 7075 7420 3d20 7265 6d6f 7665 2869 6e70  put = remove(inp
+00002700: 7574 2c20 7365 7373 696f 6e3d 7365 7373  ut, session=sess
+00002710: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
+00002720: 206f 2e77 7269 7465 286f 7574 7075 7429   o.write(output)
+00002730: 0a60 6060 0a0a 546f 2073 6565 2061 2066  .```..To see a f
+00002740: 756c 6c20 6c69 7374 206f 6620 6578 616d  ull list of exam
+00002750: 706c 6573 206f 6e20 686f 7720 746f 2075  ples on how to u
+00002760: 7365 2072 656d 6267 2c20 676f 2074 6f20  se rembg, go to 
+00002770: 7468 6520 5b65 7861 6d70 6c65 735d 2855  the [examples](U
+00002780: 5341 4745 2e6d 6429 2070 6167 652e 0a0a  SAGE.md) page...
+00002790: 2323 2055 7361 6765 2061 7320 6120 646f  ## Usage as a do
+000027a0: 636b 6572 0a0a 4a75 7374 2072 6570 6c61  cker..Just repla
+000027b0: 6365 2074 6865 2060 7265 6d62 6760 2063  ce the `rembg` c
+000027c0: 6f6d 6d61 6e64 2066 6f72 2060 646f 636b  ommand for `dock
+000027d0: 6572 2072 756e 2064 616e 6965 6c67 6174  er run danielgat
+000027e0: 6973 2f72 656d 6267 602e 0a0a 5472 7920  is/rembg`...Try 
+000027f0: 7468 6973 3a0a 0a60 6060 7368 656c 6c0a  this:..```shell.
+00002800: 646f 636b 6572 2072 756e 202d 7620 7061  docker run -v pa
+00002810: 7468 2f74 6f2f 696e 7075 743a 2f72 656d  th/to/input:/rem
+00002820: 6267 2064 616e 6965 6c67 6174 6973 2f72  bg danielgatis/r
+00002830: 656d 6267 2069 2069 6e70 7574 2e70 6e67  embg i input.png
+00002840: 2070 6174 682f 746f 2f6f 7574 7075 742f   path/to/output/
+00002850: 6f75 7470 7574 2e70 6e67 0a60 6060 0a0a  output.png.```..
+00002860: 2323 204d 6f64 656c 730a 0a41 6c6c 206d  ## Models..All m
+00002870: 6f64 656c 7320 6172 6520 646f 776e 6c6f  odels are downlo
+00002880: 6164 6564 2061 6e64 2073 6176 6564 2069  aded and saved i
+00002890: 6e20 7468 6520 7573 6572 2068 6f6d 6520  n the user home 
+000028a0: 666f 6c64 6572 2069 6e20 7468 6520 602e  folder in the `.
+000028b0: 7532 6e65 7460 2064 6972 6563 746f 7279  u2net` directory
+000028c0: 2e0a 0a54 6865 2061 7661 696c 6162 6c65  ...The available
+000028d0: 206d 6f64 656c 7320 6172 653a 0a0a 2d20   models are:..- 
+000028e0: 7532 6e65 7420 285b 646f 776e 6c6f 6164  u2net ([download
+000028f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002900: 2e63 6f6d 2f64 616e 6965 6c67 6174 6973  .com/danielgatis
+00002910: 2f72 656d 6267 2f72 656c 6561 7365 732f  /rembg/releases/
+00002920: 646f 776e 6c6f 6164 2f76 302e 302e 302f  download/v0.0.0/
+00002930: 7532 6e65 742e 6f6e 6e78 292c 205b 736f  u2net.onnx), [so
+00002940: 7572 6365 5d28 6874 7470 733a 2f2f 6769  urce](https://gi
+00002950: 7468 7562 2e63 6f6d 2f78 7565 6269 6e71  thub.com/xuebinq
+00002960: 696e 2f55 2d32 2d4e 6574 2929 3a20 4120  in/U-2-Net)): A 
+00002970: 7072 652d 7472 6169 6e65 6420 6d6f 6465  pre-trained mode
+00002980: 6c20 666f 7220 6765 6e65 7261 6c20 7573  l for general us
+00002990: 6520 6361 7365 732e 0a2d 2075 326e 6574  e cases..- u2net
+000029a0: 7020 285b 646f 776e 6c6f 6164 5d28 6874  p ([download](ht
+000029b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000029c0: 2f64 616e 6965 6c67 6174 6973 2f72 656d  /danielgatis/rem
+000029d0: 6267 2f72 656c 6561 7365 732f 646f 776e  bg/releases/down
+000029e0: 6c6f 6164 2f76 302e 302e 302f 7532 6e65  load/v0.0.0/u2ne
+000029f0: 7470 2e6f 6e6e 7829 2c20 5b73 6f75 7263  tp.onnx), [sourc
+00002a00: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00002a10: 622e 636f 6d2f 7875 6562 696e 7169 6e2f  b.com/xuebinqin/
+00002a20: 552d 322d 4e65 7429 293a 2041 206c 6967  U-2-Net)): A lig
+00002a30: 6874 7765 6967 6874 2076 6572 7369 6f6e  htweight version
+00002a40: 206f 6620 7532 6e65 7420 6d6f 6465 6c2e   of u2net model.
+00002a50: 0a2d 2075 326e 6574 5f68 756d 616e 5f73  .- u2net_human_s
+00002a60: 6567 2028 5b64 6f77 6e6c 6f61 645d 2868  eg ([download](h
+00002a70: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002a80: 6d2f 6461 6e69 656c 6761 7469 732f 7265  m/danielgatis/re
+00002a90: 6d62 672f 7265 6c65 6173 6573 2f64 6f77  mbg/releases/dow
+00002aa0: 6e6c 6f61 642f 7630 2e30 2e30 2f75 326e  nload/v0.0.0/u2n
+00002ab0: 6574 5f68 756d 616e 5f73 6567 2e6f 6e6e  et_human_seg.onn
+00002ac0: 7829 2c20 5b73 6f75 7263 655d 2868 7474  x), [source](htt
+00002ad0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002ae0: 7875 6562 696e 7169 6e2f 552d 322d 4e65  xuebinqin/U-2-Ne
+00002af0: 7429 293a 2041 2070 7265 2d74 7261 696e  t)): A pre-train
+00002b00: 6564 206d 6f64 656c 2066 6f72 2068 756d  ed model for hum
+00002b10: 616e 2073 6567 6d65 6e74 6174 696f 6e2e  an segmentation.
+00002b20: 0a2d 2075 326e 6574 5f63 6c6f 7468 5f73  .- u2net_cloth_s
+00002b30: 6567 2028 5b64 6f77 6e6c 6f61 645d 2868  eg ([download](h
+00002b40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002b50: 6d2f 6461 6e69 656c 6761 7469 732f 7265  m/danielgatis/re
+00002b60: 6d62 672f 7265 6c65 6173 6573 2f64 6f77  mbg/releases/dow
+00002b70: 6e6c 6f61 642f 7630 2e30 2e30 2f75 326e  nload/v0.0.0/u2n
+00002b80: 6574 5f63 6c6f 7468 5f73 6567 2e6f 6e6e  et_cloth_seg.onn
+00002b90: 7829 2c20 5b73 6f75 7263 655d 2868 7474  x), [source](htt
+00002ba0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002bb0: 6c65 7669 6e64 6162 6869 2f63 6c6f 7468  levindabhi/cloth
+00002bc0: 2d73 6567 6d65 6e74 6174 696f 6e29 293a  -segmentation)):
+00002bd0: 2041 2070 7265 2d74 7261 696e 6564 206d   A pre-trained m
+00002be0: 6f64 656c 2066 6f72 2043 6c6f 7468 7320  odel for Cloths 
+00002bf0: 5061 7273 696e 6720 6672 6f6d 2068 756d  Parsing from hum
+00002c00: 616e 2070 6f72 7472 6169 742e 2048 6572  an portrait. Her
+00002c10: 6520 636c 6f74 6865 7320 6172 6520 7061  e clothes are pa
+00002c20: 7273 6564 2069 6e74 6f20 3320 6361 7465  rsed into 3 cate
+00002c30: 676f 7279 3a20 5570 7065 7220 626f 6479  gory: Upper body
+00002c40: 2c20 4c6f 7765 7220 626f 6479 2061 6e64  , Lower body and
+00002c50: 2046 756c 6c20 626f 6479 2e0a 2d20 7369   Full body..- si
+00002c60: 6c75 6574 6120 285b 646f 776e 6c6f 6164  lueta ([download
+00002c70: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002c80: 2e63 6f6d 2f64 616e 6965 6c67 6174 6973  .com/danielgatis
+00002c90: 2f72 656d 6267 2f72 656c 6561 7365 732f  /rembg/releases/
+00002ca0: 646f 776e 6c6f 6164 2f76 302e 302e 302f  download/v0.0.0/
+00002cb0: 7369 6c75 6574 612e 6f6e 6e78 292c 205b  silueta.onnx), [
+00002cc0: 736f 7572 6365 5d28 6874 7470 733a 2f2f  source](https://
+00002cd0: 6769 7468 7562 2e63 6f6d 2f78 7565 6269  github.com/xuebi
+00002ce0: 6e71 696e 2f55 2d32 2d4e 6574 2f69 7373  nqin/U-2-Net/iss
+00002cf0: 7565 732f 3239 3529 293a 2053 616d 6520  ues/295)): Same 
+00002d00: 6173 2075 326e 6574 2062 7574 2074 6865  as u2net but the
+00002d10: 2073 697a 6520 6973 2072 6564 7563 6564   size is reduced
+00002d20: 2074 6f20 3433 4d62 2e0a 2d20 6973 6e65   to 43Mb..- isne
+00002d30: 742d 6765 6e65 7261 6c2d 7573 6520 285b  t-general-use ([
+00002d40: 646f 776e 6c6f 6164 5d28 6874 7470 733a  download](https:
+00002d50: 2f2f 6769 7468 7562 2e63 6f6d 2f64 616e  //github.com/dan
+00002d60: 6965 6c67 6174 6973 2f72 656d 6267 2f72  ielgatis/rembg/r
+00002d70: 656c 6561 7365 732f 646f 776e 6c6f 6164  eleases/download
+00002d80: 2f76 302e 302e 302f 6973 6e65 742d 6765  /v0.0.0/isnet-ge
+00002d90: 6e65 7261 6c2d 7573 652e 6f6e 6e78 292c  neral-use.onnx),
+00002da0: 205b 736f 7572 6365 5d28 6874 7470 733a   [source](https:
+00002db0: 2f2f 6769 7468 7562 2e63 6f6d 2f78 7565  //github.com/xue
+00002dc0: 6269 6e71 696e 2f44 4953 2929 3a20 4120  binqin/DIS)): A 
+00002dd0: 6e65 7720 7072 652d 7472 6169 6e65 6420  new pre-trained 
+00002de0: 6d6f 6465 6c20 666f 7220 6765 6e65 7261  model for genera
+00002df0: 6c20 7573 6520 6361 7365 732e 0a2d 2069  l use cases..- i
+00002e00: 736e 6574 2d61 6e69 6d65 2028 5b64 6f77  snet-anime ([dow
+00002e10: 6e6c 6f61 645d 2868 7474 7073 3a2f 2f67  nload](https://g
+00002e20: 6974 6875 622e 636f 6d2f 6461 6e69 656c  ithub.com/daniel
+00002e30: 6761 7469 732f 7265 6d62 672f 7265 6c65  gatis/rembg/rele
+00002e40: 6173 6573 2f64 6f77 6e6c 6f61 642f 7630  ases/download/v0
+00002e50: 2e30 2e30 2f69 736e 6574 2d61 6e69 6d65  .0.0/isnet-anime
+00002e60: 2e6f 6e6e 7829 2c20 5b73 6f75 7263 655d  .onnx), [source]
+00002e70: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00002e80: 636f 6d2f 536b 7954 4e54 2f61 6e69 6d65  com/SkyTNT/anime
+00002e90: 2d73 6567 6d65 6e74 6174 696f 6e29 293a  -segmentation)):
+00002ea0: 2041 2068 6967 682d 6163 6375 7261 6379   A high-accuracy
+00002eb0: 2073 6567 6d65 6e74 6174 696f 6e20 666f   segmentation fo
+00002ec0: 7220 616e 696d 6520 6368 6172 6163 7465  r anime characte
+00002ed0: 722e 0a2d 2073 616d 2028 5b64 6f77 6e6c  r..- sam ([downl
+00002ee0: 6f61 6420 656e 636f 6465 725d 2868 7474  oad encoder](htt
+00002ef0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002f00: 6461 6e69 656c 6761 7469 732f 7265 6d62  danielgatis/remb
+00002f10: 672f 7265 6c65 6173 6573 2f64 6f77 6e6c  g/releases/downl
+00002f20: 6f61 642f 7630 2e30 2e30 2f76 6974 5f62  oad/v0.0.0/vit_b
+00002f30: 2d65 6e63 6f64 6572 2d71 7561 6e74 2e6f  -encoder-quant.o
+00002f40: 6e6e 7829 2c20 5b64 6f77 6e6c 6f61 6420  nnx), [download 
+00002f50: 6465 636f 6465 725d 2868 7474 7073 3a2f  decoder](https:/
+00002f60: 2f67 6974 6875 622e 636f 6d2f 6461 6e69  /github.com/dani
+00002f70: 656c 6761 7469 732f 7265 6d62 672f 7265  elgatis/rembg/re
+00002f80: 6c65 6173 6573 2f64 6f77 6e6c 6f61 642f  leases/download/
+00002f90: 7630 2e30 2e30 2f76 6974 5f62 2d64 6563  v0.0.0/vit_b-dec
+00002fa0: 6f64 6572 2d71 7561 6e74 2e6f 6e6e 7829  oder-quant.onnx)
+00002fb0: 2c20 5b73 6f75 7263 655d 2868 7474 7073  , [source](https
+00002fc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6661  ://github.com/fa
+00002fd0: 6365 626f 6f6b 7265 7365 6172 6368 2f73  cebookresearch/s
+00002fe0: 6567 6d65 6e74 2d61 6e79 7468 696e 6729  egment-anything)
+00002ff0: 293a 2041 2070 7265 2d74 7261 696e 6564  ): A pre-trained
+00003000: 206d 6f64 656c 2066 6f72 2061 6e79 2075   model for any u
+00003010: 7365 2063 6173 6573 2e0a 0a23 2323 2048  se cases...### H
+00003020: 6f77 2074 6f20 7472 6169 6e20 796f 7572  ow to train your
+00003030: 206f 776e 206d 6f64 656c 0a0a 4966 2059   own model..If Y
+00003040: 6f75 206e 6565 6420 6d6f 7265 2066 696e  ou need more fin
+00003050: 6520 7475 6e65 6420 6d6f 6465 6c73 2074  e tuned models t
+00003060: 7279 2074 6869 733a 0a3c 6874 7470 733a  ry this:.<https:
+00003070: 2f2f 6769 7468 7562 2e63 6f6d 2f64 616e  //github.com/dan
+00003080: 6965 6c67 6174 6973 2f72 656d 6267 2f69  ielgatis/rembg/i
+00003090: 7373 7565 732f 3139 3323 6973 7375 6563  ssues/193#issuec
+000030a0: 6f6d 6d65 6e74 2d31 3035 3535 3334 3238  omment-105553428
+000030b0: 393e 0a0a 2323 2053 6f6d 6520 7669 6465  9>..## Some vide
+000030c0: 6f20 7475 746f 7269 616c 730a 0a2d 203c  o tutorials..- <
+000030d0: 6874 7470 733a 2f2f 7777 772e 796f 7574  https://www.yout
+000030e0: 7562 652e 636f 6d2f 7761 7463 683f 763d  ube.com/watch?v=
+000030f0: 3378 7177 7058 6a78 794d 513e 0a2d 203c  3xqwpXjxyMQ>.- <
+00003100: 6874 7470 733a 2f2f 7777 772e 796f 7574  https://www.yout
+00003110: 7562 652e 636f 6d2f 7761 7463 683f 763d  ube.com/watch?v=
+00003120: 6446 4b52 4758 646b 474a 553e 0a2d 203c  dFKRGXdkGJU>.- <
+00003130: 6874 7470 733a 2f2f 7777 772e 796f 7574  https://www.yout
+00003140: 7562 652e 636f 6d2f 7761 7463 683f 763d  ube.com/watch?v=
+00003150: 4169 2d42 535f 5437 796a 453e 0a2d 203c  Ai-BS_T7yjE>.- <
+00003160: 6874 7470 733a 2f2f 7777 772e 796f 7574  https://www.yout
+00003170: 7562 652e 636f 6d2f 7761 7463 683f 763d  ube.com/watch?v=
+00003180: 4437 572d 4330 7572 5663 513e 0a0a 2323  D7W-C0urVcQ>..##
+00003190: 2052 6566 6572 656e 6365 730a 0a2d 203c   References..- <
+000031a0: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+000031b0: 672f 7064 662f 3230 3035 2e30 3930 3037  g/pdf/2005.09007
+000031c0: 2e70 6466 3e0a 2d20 3c68 7474 7073 3a2f  .pdf>.- <https:/
+000031d0: 2f67 6974 6875 622e 636f 6d2f 4e61 7468  /github.com/Nath
+000031e0: 616e 5541 2f55 2d32 2d4e 6574 3e0a 2d20  anUA/U-2-Net>.- 
+000031f0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+00003200: 636f 6d2f 7079 6d61 7474 696e 672f 7079  com/pymatting/py
+00003210: 6d61 7474 696e 673e 0a0a 2323 2046 4151  matting>..## FAQ
+00003220: 0a0a 2323 2320 5768 656e 2077 696c 6c20  ..### When will 
+00003230: 7468 6973 206c 6962 7261 7279 2070 726f  this library pro
+00003240: 7669 6465 2073 7570 706f 7274 2066 6f72  vide support for
+00003250: 2050 7974 686f 6e20 7665 7273 696f 6e20   Python version 
+00003260: 332e 7878 3f0a 0a54 6869 7320 6c69 6272  3.xx?..This libr
+00003270: 6172 7920 6469 7265 6374 6c79 2064 6570  ary directly dep
+00003280: 656e 6473 206f 6e20 7468 6520 5b6f 6e6e  ends on the [onn
+00003290: 7872 756e 7469 6d65 5d28 6874 7470 733a  xruntime](https:
+000032a0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+000032b0: 6374 2f6f 6e6e 7872 756e 7469 6d65 2920  ct/onnxruntime) 
+000032c0: 6c69 6272 6172 792e 2054 6865 7265 666f  library. Therefo
+000032d0: 7265 2c20 7765 2063 616e 206f 6e6c 7920  re, we can only 
+000032e0: 7570 6461 7465 2074 6865 2050 7974 686f  update the Pytho
+000032f0: 6e20 7665 7273 696f 6e20 7768 656e 205b  n version when [
+00003300: 6f6e 6e78 7275 6e74 696d 655d 2868 7474  onnxruntime](htt
+00003310: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+00003320: 6f6a 6563 742f 6f6e 6e78 7275 6e74 696d  oject/onnxruntim
+00003330: 6529 2070 726f 7669 6465 7320 7375 7070  e) provides supp
+00003340: 6f72 7420 666f 7220 7468 6174 2073 7065  ort for that spe
+00003350: 6369 6669 6320 7665 7273 696f 6e2e 0a0a  cific version...
+00003360: 2323 2042 7579 206d 6520 6120 636f 6666  ## Buy me a coff
+00003370: 6565 0a0a 4c69 6b65 6420 736f 6d65 206f  ee..Liked some o
+00003380: 6620 6d79 2077 6f72 6b3f 2042 7579 206d  f my work? Buy m
+00003390: 6520 6120 636f 6666 6565 2028 6f72 206d  e a coffee (or m
+000033a0: 6f72 6520 6c69 6b65 6c79 2061 2062 6565  ore likely a bee
+000033b0: 7229 0a0a 3c61 2068 7265 663d 2268 7474  r)..<a href="htt
+000033c0: 7073 3a2f 2f77 7777 2e62 7579 6d65 6163  ps://www.buymeac
+000033d0: 6f66 6665 652e 636f 6d2f 6461 6e69 656c  offee.com/daniel
+000033e0: 6761 7469 7322 2074 6172 6765 743d 225f  gatis" target="_
+000033f0: 626c 616e 6b22 3e3c 696d 6720 7372 633d  blank"><img src=
+00003400: 2268 7474 7073 3a2f 2f62 6d63 2d63 646e  "https://bmc-cdn
+00003410: 2e6e 7963 332e 6469 6769 7461 6c6f 6365  .nyc3.digitaloce
+00003420: 616e 7370 6163 6573 2e63 6f6d 2f42 4d43  anspaces.com/BMC
+00003430: 2d62 7574 746f 6e2d 696d 6167 6573 2f63  -button-images/c
+00003440: 7573 746f 6d5f 696d 6167 6573 2f6f 7261  ustom_images/ora
+00003450: 6e67 655f 696d 672e 706e 6722 2061 6c74  nge_img.png" alt
+00003460: 3d22 4275 7920 4d65 2041 2043 6f66 6665  ="Buy Me A Coffe
+00003470: 6522 2073 7479 6c65 3d22 6865 6967 6874  e" style="height
+00003480: 3a20 6175 746f 2021 696d 706f 7274 616e  : auto !importan
+00003490: 743b 7769 6474 683a 2061 7574 6f20 2169  t;width: auto !i
+000034a0: 6d70 6f72 7461 6e74 3b22 3e3c 2f61 3e20  mportant;"></a> 
+000034b0: 3c21 2d2d 206d 6172 6b64 6f77 6e6c 696e  <!-- markdownlin
+000034c0: 742d 6469 7361 626c 6520 4d44 3033 3320  t-disable MD033 
+000034d0: 2d2d 3e0a 0a23 2320 5374 6172 2048 6973  -->..## Star His
+000034e0: 746f 7279 0a0a 5b21 5b53 7461 7220 4869  tory..[![Star Hi
+000034f0: 7374 6f72 7920 4368 6172 745d 2868 7474  story Chart](htt
+00003500: 7073 3a2f 2f61 7069 2e73 7461 722d 6869  ps://api.star-hi
+00003510: 7374 6f72 792e 636f 6d2f 7376 673f 7265  story.com/svg?re
+00003520: 706f 733d 6461 6e69 656c 6761 7469 732f  pos=danielgatis/
+00003530: 7265 6d62 6726 7479 7065 3d44 6174 6529  rembg&type=Date)
+00003540: 5d28 6874 7470 733a 2f2f 7374 6172 2d68  ](https://star-h
+00003550: 6973 746f 7279 2e63 6f6d 2f23 6461 6e69  istory.com/#dani
+00003560: 656c 6761 7469 732f 7265 6d62 6726 4461  elgatis/rembg&Da
+00003570: 7465 290a 0a23 2320 4c69 6365 6e73 650a  te)..## License.
+00003580: 0a43 6f70 7972 6967 6874 2028 6329 2032  .Copyright (c) 2
+00003590: 3032 302d 7072 6573 656e 7420 5b44 616e  020-present [Dan
+000035a0: 6965 6c20 4761 7469 735d 2868 7474 7073  iel Gatis](https
+000035b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6461  ://github.com/da
+000035c0: 6e69 656c 6761 7469 7329 0a0a 4c69 6365  nielgatis)..Lice
+000035d0: 6e73 6564 2075 6e64 6572 205b 4d49 5420  nsed under [MIT 
+000035e0: 4c69 6365 6e73 655d 282e 2f4c 4943 454e  License](./LICEN
+000035f0: 5345 2e74 7874 290a                      SE.txt).
```

### Comparing `rembg-2.0.56/rembg/bg.py` & `rembg-2.0.57/rembg/bg.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import io
 from enum import Enum
-from typing import Any, List, Optional, Tuple, Union
+from typing import Any, List, Optional, Tuple, Union, cast
 
 import numpy as np
 import onnxruntime as ort
 from cv2 import (
     BORDER_DEFAULT,
     MORPH_ELLIPSE,
     MORPH_OPEN,
@@ -51,34 +51,34 @@
 
     The function returns a PIL image representing the cutout of the foreground object
     from the original image.
     """
     if img.mode == "RGBA" or img.mode == "CMYK":
         img = img.convert("RGB")
 
-    img = np.asarray(img)
-    mask = np.asarray(mask)
+    img_array = np.asarray(img)
+    mask_array = np.asarray(mask)
 
-    is_foreground = mask > foreground_threshold
-    is_background = mask < background_threshold
+    is_foreground = mask_array > foreground_threshold
+    is_background = mask_array < background_threshold
 
     structure = None
     if erode_structure_size > 0:
         structure = np.ones(
             (erode_structure_size, erode_structure_size), dtype=np.uint8
         )
 
     is_foreground = binary_erosion(is_foreground, structure=structure)
     is_background = binary_erosion(is_background, structure=structure, border_value=1)
 
-    trimap = np.full(mask.shape, dtype=np.uint8, fill_value=128)
+    trimap = np.full(mask_array.shape, dtype=np.uint8, fill_value=128)
     trimap[is_foreground] = 255
     trimap[is_background] = 0
 
-    img_normalized = img / 255.0
+    img_normalized = img_array / 255.0
     trimap_normalized = trimap / 255.0
 
     alpha = estimate_alpha_cf(img_normalized, trimap_normalized)
     foreground = estimate_foreground_ml(img_normalized, alpha)
     cutout = stack_images(foreground, alpha)
 
     cutout = np.clip(cutout * 255, 0, 255).astype(np.uint8)
@@ -188,15 +188,15 @@
 
     Args:
         img (PILImage): The image to be fixed.
 
     Returns:
         PILImage: The fixed image.
     """
-    return ImageOps.exif_transpose(img)
+    return cast(PILImage, ImageOps.exif_transpose(img))
 
 
 def download_models() -> None:
     """
     Download models for image processing.
     """
     for session in sessions_class:
```

### Comparing `rembg-2.0.56/rembg/commands/b_command.py` & `rembg-2.0.57/rembg/commands/b_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import io
 import json
 import os
 import sys
 from typing import IO
 
 import click
-from PIL import Image
+from PIL.Image import Image as PILImage
 
 from ..bg import remove
 from ..session_factory import new_session
 from ..sessions import sessions_names
 
 
 @click.command(  # type: ignore
@@ -130,15 +130,15 @@
         output_dir = os.path.dirname(
             os.path.abspath(os.path.expanduser(output_specifier))
         )
 
         if not os.path.isdir(output_dir):
             os.makedirs(output_dir, exist_ok=True)
 
-    def img_to_byte_array(img: Image) -> bytes:
+    def img_to_byte_array(img: PILImage) -> bytes:
         buff = io.BytesIO()
         img.save(buff, format="PNG")
         return buff.getvalue()
 
     async def connect_stdin_stdout():
         loop = asyncio.get_event_loop()
         reader = asyncio.StreamReader()
@@ -158,15 +158,15 @@
         idx = 0
         while True:
             try:
                 img_bytes = await reader.readexactly(bytes_per_img)
                 if not img_bytes:
                     break
 
-                img = Image.frombytes("RGB", (image_width, image_height), img_bytes)
+                img = PILImage.frombytes("RGB", (image_width, image_height), img_bytes)
                 output = remove(img, session=session, **kwargs)
 
                 if output_specifier:
                     output.save((output_specifier % idx), format="PNG")
                 else:
                     writer.write(img_to_byte_array(output))
```

### Comparing `rembg-2.0.56/rembg/commands/i_command.py` & `rembg-2.0.57/rembg/commands/i_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.56/rembg/commands/p_command.py` & `rembg-2.0.57/rembg/commands/p_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,17 +182,17 @@
                 each_input.unlink()
 
         except Exception as e:
             print(e)
 
     inputs = list(input.glob("**/*"))
     if not watch:
-        inputs = tqdm(inputs)
+        inputs_tqdm = tqdm(inputs)
 
-    for each_input in inputs:
+    for each_input in inputs_tqdm:
         if not each_input.is_dir():
             process(each_input)
 
     if watch:
         should_watch = True
         observer = Observer()
```

### Comparing `rembg-2.0.56/rembg/commands/s_command.py` & `rembg-2.0.57/rembg/commands/s_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.56/rembg/session_factory.py` & `rembg-2.0.57/rembg/session_factory.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.56/rembg/sessions/__init__.py` & `rembg-2.0.57/rembg/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.56/rembg/sessions/base.py` & `rembg-2.0.57/rembg/sessions/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         img: PILImage,
         mean: Tuple[float, float, float],
         std: Tuple[float, float, float],
         size: Tuple[int, int],
         *args,
         **kwargs
     ) -> Dict[str, np.ndarray]:
-        im = img.convert("RGB").resize(size, Image.LANCZOS)
+        im = img.convert("RGB").resize(size, Image.Resampling.LANCZOS)
 
         im_ary = np.array(im)
         im_ary = im_ary / np.max(im_ary)
 
         tmpImg = np.zeros((im_ary.shape[0], im_ary.shape[1], 3))
         tmpImg[:, :, 0] = (im_ary[:, :, 0] - mean[0]) / std[0]
         tmpImg[:, :, 1] = (im_ary[:, :, 1] - mean[1]) / std[1]
```

### Comparing `rembg-2.0.56/rembg/sessions/dis_anime.py` & `rembg-2.0.57/rembg/sessions/dis_anime.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         ma = np.max(pred)
         mi = np.min(pred)
 
         pred = (pred - mi) / (ma - mi)
         pred = np.squeeze(pred)
 
         mask = Image.fromarray((pred * 255).astype("uint8"), mode="L")
-        mask = mask.resize(img.size, Image.LANCZOS)
+        mask = mask.resize(img.size, Image.Resampling.LANCZOS)
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         """
         Download the pre-trained models.
```

### Comparing `rembg-2.0.56/rembg/sessions/dis_general_use.py` & `rembg-2.0.57/rembg/sessions/dis_general_use.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         ma = np.max(pred)
         mi = np.min(pred)
 
         pred = (pred - mi) / (ma - mi)
         pred = np.squeeze(pred)
 
         mask = Image.fromarray((pred * 255).astype("uint8"), mode="L")
-        mask = mask.resize(img.size, Image.LANCZOS)
+        mask = mask.resize(img.size, Image.Resampling.LANCZOS)
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         """
         Downloads the pre-trained model file.
```

### Comparing `rembg-2.0.56/rembg/sessions/sam.py` & `rembg-2.0.57/rembg/sessions/sam.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from copy import deepcopy
-from typing import List
+from typing import Dict, List, Tuple
 
 import cv2
 import numpy as np
 import onnxruntime as ort
 import pooch
 from jsonschema import validate
 from PIL import Image
@@ -79,62 +79,54 @@
     Args:
         model_name (str): The name of the model.
         sess_opts (ort.SessionOptions): The session options.
         *args: Variable length argument list.
         **kwargs: Arbitrary keyword arguments.
     """
 
-    def __init__(self, model_name: str, sess_opts: ort.SessionOptions, *args, **kwargs):
+    def __init__(
+        self,
+        model_name: str,
+        sess_opts: ort.SessionOptions,
+        providers=None,
+        *args,
+        **kwargs,
+    ):
         """
         Initialize a new SamSession with the given model name and session options.
 
         Args:
             model_name (str): The name of the model.
             sess_opts (ort.SessionOptions): The session options.
             *args: Variable length argument list.
             **kwargs: Arbitrary keyword arguments.
         """
         self.model_name = model_name
+
+        valid_providers = []
+        available_providers = ort.get_available_providers()
+
+        for provider in providers or []:
+            if provider in available_providers:
+                valid_providers.append(provider)
+        else:
+            valid_providers.extend(available_providers)
+
         paths = self.__class__.download_models(*args, **kwargs)
         self.encoder = ort.InferenceSession(
             str(paths[0]),
-            providers=ort.get_available_providers(),
+            providers=valid_providers,
             sess_options=sess_opts,
         )
         self.decoder = ort.InferenceSession(
             str(paths[1]),
-            providers=ort.get_available_providers(),
+            providers=valid_providers,
             sess_options=sess_opts,
         )
 
-    def normalize(
-        self,
-        img: np.ndarray,
-        mean=(),
-        std=(),
-        size=(),
-        *args,
-        **kwargs,
-    ):
-        """
-        Normalize the input image by subtracting the mean and dividing by the standard deviation.
-
-        Args:
-            img (np.ndarray): The input image.
-            mean (tuple, optional): The mean values for normalization. Defaults to ().
-            std (tuple, optional): The standard deviation values for normalization. Defaults to ().
-            size (tuple, optional): The target size of the image. Defaults to ().
-            *args: Variable length argument list.
-            **kwargs: Arbitrary keyword arguments.
-
-        Returns:
-            np.ndarray: The normalized image.
-        """
-        return img
-
     def predict(
         self,
         img: PILImage,
         *args,
         **kwargs,
     ) -> List[PILImage]:
         """
@@ -249,16 +241,15 @@
         inv_transform_matrix = np.linalg.inv(transform_matrix)
         masks = transform_masks(masks, original_size, inv_transform_matrix)
 
         mask = np.zeros((masks.shape[2], masks.shape[3], 3), dtype=np.uint8)
         for m in masks[0, :, :, :]:
             mask[m > 0.0] = [255, 255, 255]
 
-        mask = Image.fromarray(mask).convert("L")
-        return [mask]
+        return [Image.fromarray(mask).convert("L")]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         """
         Class method to download ONNX model files.
 
         This method is responsible for downloading two ONNX model files from specified URLs and saving them locally. The downloaded files are saved with the naming convention 'name_encoder.onnx' and 'name_decoder.onnx', where 'name' is the value returned by the 'name' method.
```

### Comparing `rembg-2.0.56/rembg/sessions/silueta.py` & `rembg-2.0.57/rembg/sessions/silueta.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         ma = np.max(pred)
         mi = np.min(pred)
 
         pred = (pred - mi) / (ma - mi)
         pred = np.squeeze(pred)
 
         mask = Image.fromarray((pred * 255).astype("uint8"), mode="L")
-        mask = mask.resize(img.size, Image.LANCZOS)
+        mask = mask.resize(img.size, Image.Resampling.LANCZOS)
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         """
         Download the pre-trained model file.
```

### Comparing `rembg-2.0.56/rembg/sessions/u2net.py` & `rembg-2.0.57/rembg/sessions/u2net.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         ma = np.max(pred)
         mi = np.min(pred)
 
         pred = (pred - mi) / (ma - mi)
         pred = np.squeeze(pred)
 
         mask = Image.fromarray((pred * 255).astype("uint8"), mode="L")
-        mask = mask.resize(img.size, Image.LANCZOS)
+        mask = mask.resize(img.size, Image.Resampling.LANCZOS)
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         """
         Downloads the U2net model file from a specific URL and saves it.
```

### Comparing `rembg-2.0.56/rembg/sessions/u2net_cloth_seg.py` & `rembg-2.0.57/rembg/sessions/u2net_cloth_seg.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         pred = ort_outs
         pred = log_softmax(pred[0], 1)
         pred = np.argmax(pred, axis=1, keepdims=True)
         pred = np.squeeze(pred, 0)
         pred = np.squeeze(pred, 0)
 
         mask = Image.fromarray(pred.astype("uint8"), mode="L")
-        mask = mask.resize(img.size, Image.LANCZOS)
+        mask = mask.resize(img.size, Image.Resampling.LANCZOS)
 
         masks = []
 
         cloth_category = kwargs.get("cc") or kwargs.get("cloth_category")
 
         def upper_cloth():
             mask1 = mask.copy()
```

### Comparing `rembg-2.0.56/rembg/sessions/u2net_custom.py` & `rembg-2.0.57/rembg/sessions/u2net_custom.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         ma = np.max(pred)
         mi = np.min(pred)
 
         pred = (pred - mi) / (ma - mi)
         pred = np.squeeze(pred)
 
         mask = Image.fromarray((pred * 255).astype("uint8"), mode="L")
-        mask = mask.resize(img.size, Image.LANCZOS)
+        mask = mask.resize(img.size, Image.Resampling.LANCZOS)
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         """
         Download the model files.
```

### Comparing `rembg-2.0.56/rembg/sessions/u2net_human_seg.py` & `rembg-2.0.57/rembg/sessions/u2net_human_seg.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         ma = np.max(pred)
         mi = np.min(pred)
 
         pred = (pred - mi) / (ma - mi)
         pred = np.squeeze(pred)
 
         mask = Image.fromarray((pred * 255).astype("uint8"), mode="L")
-        mask = mask.resize(img.size, Image.LANCZOS)
+        mask = mask.resize(img.size, Image.Resampling.LANCZOS)
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         """
         Downloads the U2Net model weights.
```

### Comparing `rembg-2.0.56/rembg/sessions/u2netp.py` & `rembg-2.0.57/rembg/sessions/u2netp.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         ma = np.max(pred)
         mi = np.min(pred)
 
         pred = (pred - mi) / (ma - mi)
         pred = np.squeeze(pred)
 
         mask = Image.fromarray((pred * 255).astype("uint8"), mode="L")
-        mask = mask.resize(img.size, Image.LANCZOS)
+        mask = mask.resize(img.size, Image.Resampling.LANCZOS)
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         """
         Downloads the U2netp model.
```

### Comparing `rembg-2.0.56/rembg.egg-info/PKG-INFO` & `rembg-2.0.57/rembg.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.56
+Version: 2.0.57
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
+License: UNKNOWN
 Keywords: remove,background,u2net
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -18,63 +20,62 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <3.13
 Description-Content-Type: text/markdown
+Provides-Extra: cli
 Provides-Extra: dev
 Provides-Extra: gpu
-Provides-Extra: cli
 License-File: LICENSE.txt
 
 # Rembg
 
 [![Downloads](https://img.shields.io/pypi/dm/rembg.svg)](https://img.shields.io/pypi/dm/rembg.svg)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://img.shields.io/badge/License-MIT-blue.svg)
 [![Hugging Face Spaces](https://img.shields.io/badge/🤗%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/KenjieDec/RemBG)
 [![Streamlit App](https://img.shields.io/badge/🎈%20Streamlit%20Community-Cloud-blue)](https://bgremoval.streamlit.app/)
 
-
 Rembg is a tool to remove images background.
 
 <p style="display: flex;align-items: center;justify-content: center;">
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-1.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-1.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-2.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-2.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-3.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-3.out.png" width="100" />
+  <img alt="example car-1" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-1.jpg" width="100" />
+  <img alt="example car-1.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-1.out.png" width="100" />
+  <img alt="example car-2" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-2.jpg" width="100" />
+  <img alt="example car-2.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-2.out.png" width="100" />
+  <img alt="example car-3" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-3.jpg" width="100" />
+  <img alt="example car-3.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/car-3.out.png" width="100" />
 </p>
 
 <p style="display: flex;align-items: center;justify-content: center;">
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-1.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-1.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-2.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-2.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-3.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-3.out.png" width="100" />
+  <img alt="example animal-1" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-1.jpg" width="100" />
+  <img alt="example animal-1.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-1.out.png" width="100" />
+  <img alt="example animal-2" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-2.jpg" width="100" />
+  <img alt="example animal-2.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-2.out.png" width="100" />
+  <img alt="example animal-3" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-3.jpg" width="100" />
+  <img alt="example animal-3.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/animal-3.out.png" width="100" />
 </p>
 
 <p style="display: flex;align-items: center;justify-content: center;">
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-1.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-1.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-2.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-2.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-3.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-3.out.png" width="100" />
+  <img alt="example girl-1" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-1.jpg" width="100" />
+  <img alt="example girl-1.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-1.out.png" width="100" />
+  <img alt="example girl-2" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-2.jpg" width="100" />
+  <img alt="example girl-2.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-2.out.png" width="100" />
+  <img alt="example girl-3" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-3.jpg" width="100" />
+  <img alt="example girl-3.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/girl-3.out.png" width="100" />
 </p>
 
 <p style="display: flex;align-items: center;justify-content: center;">
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-1.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-1.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-2.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-2.out.png" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-3.jpg" width="100" />
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-3.out.png" width="100" />
+  <img alt="example anime-girl-1" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-1.jpg" width="100" />
+  <img alt="example anime-girl-1.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-1.out.png" width="100" />
+  <img alt="example anime-girl-2" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-2.jpg" width="100" />
+  <img alt="example anime-girl-2.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-2.out.png" width="100" />
+  <img alt="example anime-girl-3" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-3.jpg" width="100" />
+  <img alt="example anime-girl-3.out" src="https://raw.githubusercontent.com/danielgatis/rembg/master/examples/anime-girl-3.out.png" width="100" />
 </p>
 
 **If this project has helped you, please consider making a [donation](https://www.buymeacoffee.com/danielgatis).**
 
 ## Sponsor
 
 <table>
@@ -94,15 +95,15 @@
       </p>
     </td>
   </tr>
 </table>
 
 ## Requirements
 
-```
+```text
 python: >3.7, <3.13
 ```
 
 ## Installation
 
 CPU support:
 
@@ -111,159 +112,158 @@
 pip install rembg[cli] # for library + cli
 ```
 
 GPU support:
 
 First of all, you need to check if your system supports the `onnxruntime-gpu`.
 
-Go to https://onnxruntime.ai and check the installation matrix.
+Go to <https://onnxruntime.ai> and check the installation matrix.
 
 <p style="display: flex;align-items: center;justify-content: center;">
-  <img src="https://raw.githubusercontent.com/danielgatis/rembg/master/onnxruntime-installation-matrix.png" width="400" />
+  <img alt="onnxruntime-installation-matrix" src="https://raw.githubusercontent.com/danielgatis/rembg/master/onnxruntime-installation-matrix.png" width="400" />
 </p>
 
 If yes, just run:
 
 ```bash
 pip install rembg[gpu] # for library
 pip install rembg[gpu,cli] # for library + cli
 ```
 
 ## Usage as a cli
 
 After the installation step you can use rembg just typing `rembg` in your terminal window.
 
 The `rembg` command has 4 subcommands, one for each input type:
+
 - `i` for files
 - `p` for folders
 - `s` for http server
 - `b` for RGB24 pixel binary stream
 
 You can get help about the main command using:
 
-```
+```shell
 rembg --help
 ```
 
 As well, about all the subcommands using:
 
-```
+```shell
 rembg <COMMAND> --help
 ```
 
 ### rembg `i`
 
 Used when input and output are files.
 
 Remove the background from a remote image
 
-```
+```shell
 curl -s http://input.png | rembg i > output.png
 ```
 
 Remove the background from a local file
 
-```
+```shell
 rembg i path/to/input.png path/to/output.png
 ```
 
 Remove the background specifying a model
 
-```
+```shell
 rembg i -m u2netp path/to/input.png path/to/output.png
 ```
 
 Remove the background returning only the mask
 
-```
+```shell
 rembg i -om path/to/input.png path/to/output.png
 ```
 
-
 Remove the background applying an alpha matting
 
-```
+```shell
 rembg i -a path/to/input.png path/to/output.png
 ```
 
 Passing extras parameters
 
-```
+```shell
 SAM example
 
 rembg i -m sam -x '{ "sam_prompt": [{"type": "point", "data": [724, 740], "label": 1}] }' examples/plants-1.jpg examples/plants-1.out.png
 ```
 
-```
+```shell
 Custom model example
 
 rembg i -m u2net_custom -x '{"model_path": "~/.u2net/u2net.onnx"}' path/to/input.png path/to/output.png
 ```
 
 ### rembg `p`
 
 Used when input and output are folders.
 
 Remove the background from all images in a folder
 
-```
+```shell
 rembg p path/to/input path/to/output
 ```
 
 Same as before, but watching for new/changed files to process
 
-```
+```shell
 rembg p -w path/to/input path/to/output
 ```
 
 ### rembg `s`
 
 Used to start http server.
 
-```
+```shell
 rembg s --host 0.0.0.0 --port 7000 --log_level info
 ```
 
 To see the complete endpoints documentation, go to: `http://localhost:7000/api`.
 
 Remove the background from an image url
 
-```
+```shell
 curl -s "http://localhost:7000/api/remove?url=http://input.png" -o output.png
 ```
 
 Remove the background from an uploaded image
 
-```
+```shell
 curl -s -F file=@/path/to/input.jpg "http://localhost:7000/api/remove"  -o output.png
 ```
 
 ### rembg `b`
 
 Process a sequence of RGB24 images from stdin. This is intended to be used with another program, such as FFMPEG, that outputs RGB24 pixel data to stdout, which is piped into the stdin of this program, although nothing prevents you from manually typing in images at stdin.
 
-```
+```shell
 rembg b image_width image_height -o output_specifier
 ```
 
 Arguments:
 
 - image_width : width of input image(s)
 - image_height : height of input image(s)
 - output_specifier: printf-style specifier for output filenames, for example if `output-%03u.png`, then output files will be named `output-000.png`, `output-001.png`, `output-002.png`, etc. Output files will be saved in PNG format regardless of the extension specified. You can omit it to write results to stdout.
 
 Example usage with FFMPEG:
 
-```
+```shell
 ffmpeg -i input.mp4 -ss 10 -an -f rawvideo -pix_fmt rgb24 pipe:1 | rembg b 1280 720 -o folder/output-%03u.png
 ```
 
 The width and height values must match the dimension of output images from FFMPEG. Note for FFMPEG, the "`-an -f rawvideo -pix_fmt rgb24 pipe:1`" part is required for the whole thing to work.
 
-
 ## Usage as a library
 
 Input and output as bytes
 
 ```python
 from rembg import remove
 
@@ -319,69 +319,76 @@
 
     with open(input_path, 'rb') as i:
         with open(output_path, 'wb') as o:
             input = i.read()
             output = remove(input, session=session)
             o.write(output)
 ```
+
 To see a full list of examples on how to use rembg, go to the [examples](USAGE.md) page.
+
 ## Usage as a docker
 
 Just replace the `rembg` command for `docker run danielgatis/rembg`.
 
 Try this:
 
-```
+```shell
 docker run -v path/to/input:/rembg danielgatis/rembg i input.png path/to/output/output.png
 ```
 
 ## Models
 
 All models are downloaded and saved in the user home folder in the `.u2net` directory.
 
 The available models are:
 
--   u2net ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use cases.
--   u2netp ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A lightweight version of u2net model.
--   u2net_human_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human segmentation.
--   u2net_cloth_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths Parsing from human portrait. Here clothes are parsed into 3 category: Upper body, Lower body and Full body.
--   silueta ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is reduced to 43Mb.
--   isnet-general-use ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-trained model for general use cases.
--   isnet-anime ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-anime.onnx), [source](https://github.com/SkyTNT/anime-segmentation)): A high-accuracy segmentation for anime character.
--   sam ([download encoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A pre-trained model for any use cases.
+- u2net ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use cases.
+- u2netp ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A lightweight version of u2net model.
+- u2net_human_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human segmentation.
+- u2net_cloth_seg ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths Parsing from human portrait. Here clothes are parsed into 3 category: Upper body, Lower body and Full body.
+- silueta ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is reduced to 43Mb.
+- isnet-general-use ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-trained model for general use cases.
+- isnet-anime ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-anime.onnx), [source](https://github.com/SkyTNT/anime-segmentation)): A high-accuracy segmentation for anime character.
+- sam ([download encoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A pre-trained model for any use cases.
 
 ### How to train your own model
 
 If You need more fine tuned models try this:
-https://github.com/danielgatis/rembg/issues/193#issuecomment-1055534289
-
+<https://github.com/danielgatis/rembg/issues/193#issuecomment-1055534289>
 
 ## Some video tutorials
 
-- https://www.youtube.com/watch?v=3xqwpXjxyMQ
-- https://www.youtube.com/watch?v=dFKRGXdkGJU
-- https://www.youtube.com/watch?v=Ai-BS_T7yjE
-- https://www.youtube.com/watch?v=D7W-C0urVcQ
+- <https://www.youtube.com/watch?v=3xqwpXjxyMQ>
+- <https://www.youtube.com/watch?v=dFKRGXdkGJU>
+- <https://www.youtube.com/watch?v=Ai-BS_T7yjE>
+- <https://www.youtube.com/watch?v=D7W-C0urVcQ>
 
 ## References
 
-- https://arxiv.org/pdf/2005.09007.pdf
-- https://github.com/NathanUA/U-2-Net
-- https://github.com/pymatting/pymatting
+- <https://arxiv.org/pdf/2005.09007.pdf>
+- <https://github.com/NathanUA/U-2-Net>
+- <https://github.com/pymatting/pymatting>
 
 ## FAQ
 
 ### When will this library provide support for Python version 3.xx?
 
 This library directly depends on the [onnxruntime](https://pypi.org/project/onnxruntime) library. Therefore, we can only update the Python version when [onnxruntime](https://pypi.org/project/onnxruntime) provides support for that specific version.
 
 ## Buy me a coffee
 
 Liked some of my work? Buy me a coffee (or more likely a beer)
 
-<a href="https://www.buymeacoffee.com/danielgatis" target="_blank"><img src="https://bmc-cdn.nyc3.digitaloceanspaces.com/BMC-button-images/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;"></a>
+<a href="https://www.buymeacoffee.com/danielgatis" target="_blank"><img src="https://bmc-cdn.nyc3.digitaloceanspaces.com/BMC-button-images/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;"></a> <!-- markdownlint-disable MD033 -->
+
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=danielgatis/rembg&type=Date)](https://star-history.com/#danielgatis/rembg&Date)
 
 ## License
 
 Copyright (c) 2020-present [Daniel Gatis](https://github.com/danielgatis)
 
 Licensed under [MIT License](./LICENSE.txt)
+
+
```

### Comparing `rembg-2.0.56/rembg.egg-info/SOURCES.txt` & `rembg-2.0.57/rembg.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -28,9 +28,8 @@
 rembg/sessions/dis_general_use.py
 rembg/sessions/sam.py
 rembg/sessions/silueta.py
 rembg/sessions/u2net.py
 rembg/sessions/u2net_cloth_seg.py
 rembg/sessions/u2net_custom.py
 rembg/sessions/u2net_human_seg.py
-rembg/sessions/u2netp.py
-tests/test_remove.py
+rembg/sessions/u2netp.py
```

### Comparing `rembg-2.0.56/setup.py` & `rembg-2.0.57/setup.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.56/versioneer.py` & `rembg-2.0.57/versioneer.py`

 * *Files identical despite different names*

