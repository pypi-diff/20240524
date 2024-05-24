# Comparing `tmp/matterdelta-1.4.0.tar.gz` & `tmp/matterdelta-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matterdelta-1.4.0.tar", last modified: Sat Apr 27 21:12:05 2024, max compression
+gzip compressed data, was "matterdelta-1.5.0.tar", last modified: Fri May 24 19:41:37 2024, max compression
```

## Comparing `matterdelta-1.4.0.tar` & `matterdelta-1.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:05.066473 matterdelta-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:05.062473 matterdelta-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:05.066473 matterdelta-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-27 21:11:53.000000 matterdelta-1.4.0/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-27 21:11:53.000000 matterdelta-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-27 21:11:53.000000 matterdelta-1.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-27 21:12:05.066473 matterdelta-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-27 21:11:53.000000 matterdelta-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:05.066473 matterdelta-1.4.0/matterdelta/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-27 21:11:53.000000 matterdelta-1.4.0/matterdelta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-27 21:11:53.000000 matterdelta-1.4.0/matterdelta/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 21:12:04.000000 matterdelta-1.4.0/matterdelta/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-27 21:11:53.000000 matterdelta-1.4.0/matterdelta/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-27 21:11:53.000000 matterdelta-1.4.0/matterdelta/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:05.066473 matterdelta-1.4.0/matterdelta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-27 21:12:05.000000 matterdelta-1.4.0/matterdelta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-27 21:12:05.000000 matterdelta-1.4.0/matterdelta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 21:12:05.000000 matterdelta-1.4.0/matterdelta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-27 21:12:05.000000 matterdelta-1.4.0/matterdelta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-27 21:12:05.000000 matterdelta-1.4.0/matterdelta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 21:12:05.000000 matterdelta-1.4.0/matterdelta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-27 21:11:53.000000 matterdelta-1.4.0/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-27 21:11:53.000000 matterdelta-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 21:12:05.066473 matterdelta-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:41:37.359733 matterdelta-1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:41:37.355733 matterdelta-1.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:41:37.355733 matterdelta-1.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-24 19:41:27.000000 matterdelta-1.5.0/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-24 19:41:27.000000 matterdelta-1.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-24 19:41:27.000000 matterdelta-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-24 19:41:37.359733 matterdelta-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-24 19:41:27.000000 matterdelta-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:41:37.355733 matterdelta-1.5.0/matterdelta/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-24 19:41:27.000000 matterdelta-1.5.0/matterdelta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-24 19:41:27.000000 matterdelta-1.5.0/matterdelta/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-24 19:41:27.000000 matterdelta-1.5.0/matterdelta/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-24 19:41:27.000000 matterdelta-1.5.0/matterdelta/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:41:37.359733 matterdelta-1.5.0/matterdelta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 19:41:37.000000 matterdelta-1.5.0/matterdelta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-24 19:41:27.000000 matterdelta-1.5.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-24 19:41:27.000000 matterdelta-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 19:41:37.359733 matterdelta-1.5.0/setup.cfg
```

### Comparing `matterdelta-1.4.0/.github/workflows/python-ci.yml` & `matterdelta-1.5.0/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `matterdelta-1.4.0/LICENSE.txt` & `matterdelta-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `matterdelta-1.4.0/PKG-INFO` & `matterdelta-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matterdelta
-Version: 1.4.0
+Version: 1.5.0
 Summary: Matterbridge API plugin for Delta Chat
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/matterdelta
 Keywords: deltachat,bot,matterbridge,bridge
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `matterdelta-1.4.0/README.md` & `matterdelta-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `matterdelta-1.4.0/matterdelta/api.py` & `matterdelta-1.5.0/matterdelta/api.py`

 * *Files identical despite different names*

### Comparing `matterdelta-1.4.0/matterdelta/hooks.py` & `matterdelta-1.5.0/matterdelta/hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 """Event Hooks"""
 
 from argparse import Namespace
 
 from deltabot_cli import BotCli
-from deltachat2 import Bot, ChatType, CoreEvent, EventType, MsgData, NewMsgEvent, events
+from deltachat2 import (
+    Bot,
+    ChatType,
+    CoreEvent,
+    EventType,
+    JsonRpcError,
+    MsgData,
+    NewMsgEvent,
+    events,
+)
+from deltachat2.types import SpecialContactId
 from rich.logging import RichHandler
 
 from ._version import __version__
 from .api import dc2mb, init_api
 
 cli = BotCli("matterdelta")
 cli.add_generic_option("-v", "--version", action="version", version=__version__)
@@ -21,15 +31,15 @@
 @cli.on_init
 def _on_init(bot: Bot, args: Namespace) -> None:
     bot.logger.handlers = [
         RichHandler(show_path=False, omit_repeated_times=False, show_time=args.no_time)
     ]
     for accid in bot.rpc.get_all_account_ids():
         if not bot.rpc.get_config(accid, "displayname"):
-            bot.rpc.set_config(accid, "displayname", "Matterbridge Bot")
+            bot.rpc.set_config(accid, "displayname", "Bridge Bot")
             status = "I am a Delta Chat bot, send me /help for more info"
             bot.rpc.set_config(accid, "selfstatus", status)
             bot.rpc.set_config(accid, "delete_device_after", str(60 * 60 * 24 * 30))
 
 
 @cli.on_start
 def _on_start(bot: Bot, args: Namespace) -> None:
@@ -56,15 +66,20 @@
 def _bridge(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     if bot.has_command(event.command):
         return
     msg = event.msg
     chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
     if chat.chat_type == ChatType.SINGLE and not msg.is_bot:
         bot.rpc.markseen_msgs(accid, [msg.id])
-        _send_help(bot, accid, msg.chat_id)
+        try:
+            community = bot.rpc.get_config(accid, "is_community") == "1"
+        except JsonRpcError:
+            community = False
+        if not community or msg.from_id > SpecialContactId.LAST_SPECIAL:
+            _send_help(bot, accid, msg.chat_id)
     else:
         dc2mb(bot, accid, msg)
 
 
 @cli.on(events.NewMessage(command="/id"))
 def _id(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     msg = event.msg
```

### Comparing `matterdelta-1.4.0/matterdelta.egg-info/PKG-INFO` & `matterdelta-1.5.0/matterdelta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matterdelta
-Version: 1.4.0
+Version: 1.5.0
 Summary: Matterbridge API plugin for Delta Chat
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/matterdelta
 Keywords: deltachat,bot,matterbridge,bridge
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `matterdelta-1.4.0/pyproject.toml` & `matterdelta-1.5.0/pyproject.toml`

 * *Files identical despite different names*

