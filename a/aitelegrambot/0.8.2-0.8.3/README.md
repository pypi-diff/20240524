# Comparing `tmp/aitelegrambot-0.8.2.tar.gz` & `tmp/aitelegrambot-0.8.3.tar.gz`

## Comparing `aitelegrambot-0.8.2.tar` & `aitelegrambot-0.8.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/.env.example
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/.envrc
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/CHANGELOG.md
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/Makefile
--rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/Makefile.venv
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/manifest.scm
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/docs/README.md
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/docs/commands.md
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/docs/setup.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/src/aitelegrambot/__init__.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/src/aitelegrambot/__main__.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/src/aitelegrambot/bot.py
--rw-r--r--   0        0        0     9972 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/src/aitelegrambot/commandhandlers.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/src/aitelegrambot/constants.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/.gitignore
--rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/LICENSE.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/.env.example
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/.envrc
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/CHANGELOG.md
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/Makefile
+-rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/Makefile.venv
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/manifest.scm
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/docs/README.md
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/docs/commands.md
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/docs/setup.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/src/aitelegrambot/__init__.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/src/aitelegrambot/__main__.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/src/aitelegrambot/bot.py
+-rw-r--r--   0        0        0     9972 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/src/aitelegrambot/commandhandlers.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/src/aitelegrambot/constants.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/.gitignore
+-rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/LICENSE.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 aitelegrambot-0.8.3/PKG-INFO
```

### Comparing `aitelegrambot-0.8.2/CHANGELOG.md` & `aitelegrambot-0.8.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -86,7 +86,10 @@
 ## 0.8.1
 
 - remove debugging statements from /list_models command.
 
 ## 0.8.2
 - fix BadRequest response error when using streaming inference.
 - add help message when user sends an empty message to /infer commands.
+
+## 0.8.3
+- Fix error in /infer command.
```

### Comparing `aitelegrambot-0.8.2/Makefile.venv` & `aitelegrambot-0.8.3/Makefile.venv`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.8.2/docs/commands.md` & `aitelegrambot-0.8.3/docs/commands.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.8.2/docs/setup.md` & `aitelegrambot-0.8.3/docs/setup.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.8.2/src/aitelegrambot/__main__.py` & `aitelegrambot-0.8.3/src/aitelegrambot/__main__.py`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.8.2/src/aitelegrambot/bot.py` & `aitelegrambot-0.8.3/src/aitelegrambot/bot.py`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.8.2/src/aitelegrambot/commandhandlers.py` & `aitelegrambot-0.8.3/src/aitelegrambot/commandhandlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         """
         Remove the command from query.
 
         Arguments:
         ==========
         raw_query: the raw query from telegram.
         """
-        return re.split(" ", raw_query, 1)[1]
+        return re.split(" ", raw_query, 1)[0]
 
 
 class NormalCommandHandlers(CommandHandlers):
     """
     Class for handling normal commands.
     """
```

### Comparing `aitelegrambot-0.8.2/src/aitelegrambot/constants.py` & `aitelegrambot-0.8.3/src/aitelegrambot/constants.py`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.8.2/LICENSE.md` & `aitelegrambot-0.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.8.2/pyproject.toml` & `aitelegrambot-0.8.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [tool.hatch.build.targets.wheel]
 packages = ["src/aitelegrambot"]
 [project]
 name = "aitelegrambot"
-version = "0.8.2"
+version = "0.8.3"
 dependencies = [
   "ollama",
   "python-telegram-bot",
   "python-dotenv",
 ]
 authors = [
   {name = "tusharhero", email = "tusharhero@sdf.org"},
```

### Comparing `aitelegrambot-0.8.2/PKG-INFO` & `aitelegrambot-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aitelegrambot
-Version: 0.8.2
+Version: 0.8.3
 Summary: aitelegrambot is a Telegram bot that uses the Ollama backend to run the LLM rationalAI (by default).
 Author-email: tusharhero <tusharhero@sdf.org>, alokosx <alokosx@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: ollama
 Requires-Dist: python-dotenv
```

