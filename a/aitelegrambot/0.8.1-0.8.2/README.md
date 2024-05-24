# Comparing `tmp/aitelegrambot-0.8.1.tar.gz` & `tmp/aitelegrambot-0.8.2.tar.gz`

## Comparing `aitelegrambot-0.8.1.tar` & `aitelegrambot-0.8.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/.env.example
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/.envrc
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/CHANGELOG.md
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/Makefile
--rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/Makefile.venv
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/manifest.scm
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/docs/README.md
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/docs/commands.md
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/docs/setup.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/src/aitelegrambot/__init__.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/src/aitelegrambot/__main__.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/src/aitelegrambot/bot.py
--rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/src/aitelegrambot/commandhandlers.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/src/aitelegrambot/constants.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/.gitignore
--rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/LICENSE.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 aitelegrambot-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/.env.example
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/.envrc
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/CHANGELOG.md
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/Makefile
+-rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/Makefile.venv
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/manifest.scm
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/docs/README.md
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/docs/commands.md
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/docs/setup.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/src/aitelegrambot/__init__.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/src/aitelegrambot/__main__.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/src/aitelegrambot/bot.py
+-rw-r--r--   0        0        0     9972 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/src/aitelegrambot/commandhandlers.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/src/aitelegrambot/constants.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/.gitignore
+-rw-r--r--   0        0        0    34896 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/LICENSE.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 aitelegrambot-0.8.2/PKG-INFO
```

### Comparing `aitelegrambot-0.8.1/CHANGELOG.md` & `aitelegrambot-0.8.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -82,7 +82,11 @@
 
 - add current model indication in list_models command.
 - fix error in /help command.
 
 ## 0.8.1
 
 - remove debugging statements from /list_models command.
+
+## 0.8.2
+- fix BadRequest response error when using streaming inference.
+- add help message when user sends an empty message to /infer commands.
```

### Comparing `aitelegrambot-0.8.1/Makefile.venv` & `aitelegrambot-0.8.2/Makefile.venv`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.8.1/docs/commands.md` & `aitelegrambot-0.8.2/docs/commands.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.8.1/docs/setup.md` & `aitelegrambot-0.8.2/docs/setup.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.8.1/src/aitelegrambot/__main__.py` & `aitelegrambot-0.8.2/src/aitelegrambot/__main__.py`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.8.1/src/aitelegrambot/bot.py` & `aitelegrambot-0.8.2/src/aitelegrambot/bot.py`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.8.1/src/aitelegrambot/commandhandlers.py` & `aitelegrambot-0.8.2/src/aitelegrambot/commandhandlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         """
         Remove the command from query.
 
         Arguments:
         ==========
         raw_query: the raw query from telegram.
         """
-        return re.split(" ", raw_query, 1)[-1]
+        return re.split(" ", raw_query, 1)[1]
 
 
 class NormalCommandHandlers(CommandHandlers):
     """
     Class for handling normal commands.
     """
 
@@ -120,14 +120,21 @@
         Arguments:
         ==========
         update: The update to be processed.
         context: The context for the inference.
         """
         query: str = self.get_content(update.message.text)
 
+        if query == "":
+            await update.message.reply_text(
+                text=constants.MISTAKEN_CLICK,
+                parse_mode="Markdown"
+            )
+            return
+
         message: Message = await update.message.reply_text(
             text="wait...", parse_mode="Markdown"
         )
         await message.edit_text(
             text=self.ollama_state.client.chat(
                 model=self.ollama_state.model,
                 messages=[
@@ -149,15 +156,24 @@
         Performs inference on the given update.
 
         Arguments:
         ==========
         update: The update to be processed.
         context: The context for the inference.
         """
+        prev_msg_size: int = 0
         query: str = self.get_content(update.message.text)
+
+        if query == "":
+            await update.message.reply_text(
+                text=constants.MISTAKEN_CLICK,
+                parse_mode="Markdown"
+            )
+            return
+
         message: Message = await update.message.reply_text(
             text="wait...", parse_mode="Markdown"
         )
         message_stream: list[str] = []
         for message_chunk in self.ollama_state.client.chat(
             model=self.ollama_state.model,
             messages=[
@@ -165,24 +181,34 @@
                     "role": "user",
                     "content": query,
                 },
             ],
             stream=True,
         ):
             message_stream.append(message_chunk["message"]["content"])
+            cur_msg_size = len(message_stream)
+
+            # avoid BadRequest
+            if cur_msg_size == prev_msg_size:
+                continue
+
             is_message_rounded: bool = (
-                len(message_stream) % self.ollama_state.message_chunk_size == 0
+                cur_msg_size % self.ollama_state.message_chunk_size == 0
             )
-            if is_message_rounded:
+
+            is_last_chunk: bool = (
+                message_chunk["done"]
+            )
+
+            if is_message_rounded or is_last_chunk:
+                prev_msg_size = cur_msg_size
                 await message.edit_text(
                     text="".join(message_stream), parse_mode="Markdown"
                 )
                 time.sleep(2)
-        if not is_message_rounded:
-            await message.edit_text(text="".join(message_stream), parse_mode="Markdown")
 
 
 class AdministrationCommandHandlers(CommandHandlers):
     """
     Class for administrating Ollama by the Bot administrators.
     """
```

### Comparing `aitelegrambot-0.8.1/LICENSE.md` & `aitelegrambot-0.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aitelegrambot-0.8.1/pyproject.toml` & `aitelegrambot-0.8.2/pyproject.toml`

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
-version = "0.8.1"
+version = "0.8.2"
 dependencies = [
   "ollama",
   "python-telegram-bot",
   "python-dotenv",
 ]
 authors = [
   {name = "tusharhero", email = "tusharhero@sdf.org"},
```

### Comparing `aitelegrambot-0.8.1/PKG-INFO` & `aitelegrambot-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aitelegrambot
-Version: 0.8.1
+Version: 0.8.2
 Summary: aitelegrambot is a Telegram bot that uses the Ollama backend to run the LLM rationalAI (by default).
 Author-email: tusharhero <tusharhero@sdf.org>, alokosx <alokosx@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: ollama
 Requires-Dist: python-dotenv
```

