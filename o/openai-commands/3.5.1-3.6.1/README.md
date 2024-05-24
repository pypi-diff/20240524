# Comparing `tmp/openai_commands-3.5.1.tar.gz` & `tmp/openai_commands-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_commands-3.5.1.tar", last modified: Fri May 24 02:52:27 2024, max compression
+gzip compressed data, was "openai_commands-3.6.1.tar", last modified: Fri May 24 02:53:39 2024, max compression
```

## Comparing `openai_commands-3.5.1.tar` & `openai_commands-3.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:52:27.767928 openai_commands-3.5.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-24 02:29:00.000000 openai_commands-3.5.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-24 02:29:00.000000 openai_commands-3.5.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     8461 2024-05-24 02:52:27.767240 openai_commands-3.5.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     6744 2024-05-24 02:35:54.000000 openai_commands-3.5.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:52:27.763592 openai_commands-3.5.1/openai_commands/
--rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-24 02:52:18.000000 openai_commands-3.5.1/openai_commands/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1249 2024-05-24 02:38:45.000000 openai_commands-3.5.1/openai_commands/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      481 2024-05-24 02:50:14.000000 openai_commands-3.5.1/openai_commands/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)       96 2024-05-24 02:38:46.000000 openai_commands-3.5.1/openai_commands/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-24 02:29:00.000000 openai_commands-3.5.1/openai_commands/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:52:27.766479 openai_commands-3.5.1/openai_commands.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     8461 2024-05-24 02:52:27.000000 openai_commands-3.5.1/openai_commands.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      393 2024-05-24 02:52:27.000000 openai_commands-3.5.1/openai_commands.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-24 02:52:27.000000 openai_commands-3.5.1/openai_commands.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      204 2024-05-24 02:52:27.000000 openai_commands-3.5.1/openai_commands.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       16 2024-05-24 02:52:27.000000 openai_commands-3.5.1/openai_commands.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-24 02:29:00.000000 openai_commands-3.5.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      264 2024-05-24 02:29:00.000000 openai_commands-3.5.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-24 02:52:27.768143 openai_commands-3.5.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-24 02:30:24.000000 openai_commands-3.5.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:53:39.484702 openai_commands-3.6.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-24 02:29:00.000000 openai_commands-3.6.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-24 02:29:00.000000 openai_commands-3.6.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     8444 2024-05-24 02:53:39.484184 openai_commands-3.6.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     6727 2024-05-24 02:53:20.000000 openai_commands-3.6.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:53:39.480818 openai_commands-3.6.1/openai_commands/
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-24 02:53:31.000000 openai_commands-3.6.1/openai_commands/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1249 2024-05-24 02:38:45.000000 openai_commands-3.6.1/openai_commands/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      481 2024-05-24 02:50:14.000000 openai_commands-3.6.1/openai_commands/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       96 2024-05-24 02:38:46.000000 openai_commands-3.6.1/openai_commands/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-24 02:29:00.000000 openai_commands-3.6.1/openai_commands/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-24 02:53:39.483458 openai_commands-3.6.1/openai_commands.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     8444 2024-05-24 02:53:39.000000 openai_commands-3.6.1/openai_commands.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      393 2024-05-24 02:53:39.000000 openai_commands-3.6.1/openai_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-24 02:53:39.000000 openai_commands-3.6.1/openai_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      204 2024-05-24 02:53:39.000000 openai_commands-3.6.1/openai_commands.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       16 2024-05-24 02:53:39.000000 openai_commands-3.6.1/openai_commands.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-24 02:29:00.000000 openai_commands-3.6.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      264 2024-05-24 02:29:00.000000 openai_commands-3.6.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-24 02:53:39.484775 openai_commands-3.6.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-24 02:30:24.000000 openai_commands-3.6.1/setup.py
```

### Comparing `openai_commands-3.5.1/LICENSE` & `openai_commands-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_commands-3.5.1/PKG-INFO` & `openai_commands-3.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_commands
-Version: 3.5.1
+Version: 3.6.1
 Summary: 🛠️ a command interface to the OpenAI API
 Home-page: https://github.com/kamangir/openai-commands
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -45,18 +45,14 @@
 
 Install [`awesome-bash-cli`](https://github.com/kamangir/awesome-bash-cli) (`abcli`), then,
 
 ```bash
 abcli git clone openai-commands install
 ```
 
-```bash
-...
-```
-
 ## Completion
 
 ```bash
 @openai complete "describe mathematics"
 ```
 
 > Mathematics is an abstract science that examines topics such as quantity, structure, space, change, and other topics in various ways. It involves the use of logic, algorithms, and formulas to solve problems. Mathematics can be used to study the natural world, to describe phenomena, and to make predictions about the future. It provides the foundation for the development of a wide range of disciplines in science, technology, engineering, economics, finance, and more.
```

### Comparing `openai_commands-3.5.1/README.md` & `openai_commands-3.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 
 Install [`awesome-bash-cli`](https://github.com/kamangir/awesome-bash-cli) (`abcli`), then,
 
 ```bash
 abcli git clone openai-commands install
 ```
 
-```bash
-...
-```
-
 ## Completion
 
 ```bash
 @openai complete "describe mathematics"
 ```
 
 > Mathematics is an abstract science that examines topics such as quantity, structure, space, change, and other topics in various ways. It involves the use of logic, algorithms, and formulas to solve problems. Mathematics can be used to study the natural world, to describe phenomena, and to make predictions about the future. It provides the foundation for the development of a wide range of disciplines in science, technology, engineering, economics, finance, and more.
```

### Comparing `openai_commands-3.5.1/openai_commands/__main__.py` & `openai_commands-3.6.1/openai_commands/__main__.py`

 * *Files identical despite different names*

### Comparing `openai_commands-3.5.1/openai_commands.egg-info/PKG-INFO` & `openai_commands-3.6.1/openai_commands.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_commands
-Version: 3.5.1
+Version: 3.6.1
 Summary: 🛠️ a command interface to the OpenAI API
 Home-page: https://github.com/kamangir/openai-commands
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -45,18 +45,14 @@
 
 Install [`awesome-bash-cli`](https://github.com/kamangir/awesome-bash-cli) (`abcli`), then,
 
 ```bash
 abcli git clone openai-commands install
 ```
 
-```bash
-...
-```
-
 ## Completion
 
 ```bash
 @openai complete "describe mathematics"
 ```
 
 > Mathematics is an abstract science that examines topics such as quantity, structure, space, change, and other topics in various ways. It involves the use of logic, algorithms, and formulas to solve problems. Mathematics can be used to study the natural world, to describe phenomena, and to make predictions about the future. It provides the foundation for the development of a wide range of disciplines in science, technology, engineering, economics, finance, and more.
```

