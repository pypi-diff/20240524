# Comparing `tmp/centralcli-5.0.0.tar.gz` & `tmp/centralcli-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "centralcli-5.0.0.tar", max compression
+gzip compressed data, was "centralcli-5.1.0.tar", max compression
```

## Comparing `centralcli-5.0.0.tar` & `centralcli-5.1.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1067 2023-08-30 16:01:18.948011 centralcli-5.0.0/LICENSE
--rw-r--r--   0        0        0    12115 2023-08-30 16:01:34.228021 centralcli-5.0.0/README.md
--rw-r--r--   0        0        0     5728 2024-05-09 16:23:40.007449 centralcli-5.0.0/centralcli/__init__.py
--rw-r--r--   0        0        0     1265 2023-09-08 18:43:03.749878 centralcli-5.0.0/centralcli/boilerplate/README.md
--rw-r--r--   0        0        0  1156267 2024-05-14 22:05:46.978274 centralcli-5.0.0/centralcli/boilerplate/allcalls.py
--rw-r--r--   0        0        0    11951 2024-05-05 02:42:27.903512 centralcli-5.0.0/centralcli/caas.py
--rw-r--r--   0        0        0   119848 2024-05-22 05:46:59.633976 centralcli-5.0.0/centralcli/cache.py
--rw-r--r--   0        0        0   223765 2024-05-21 15:57:32.608161 centralcli-5.0.0/centralcli/central.py
--rw-r--r--   0        0        0    60186 2024-05-21 21:30:40.222990 centralcli-5.0.0/centralcli/cleaner.py
--rw-r--r--   0        0        0    47378 2024-05-16 22:07:24.060368 centralcli-5.0.0/centralcli/cli.py
--rw-r--r--   0        0        0    29011 2024-05-13 14:28:13.658447 centralcli-5.0.0/centralcli/cliadd.py
--rw-r--r--   0        0        0     5388 2024-04-29 15:32:55.074272 centralcli-5.0.0/centralcli/cliassign.py
--rw-r--r--   0        0        0   100595 2024-05-21 03:28:12.531138 centralcli-5.0.0/centralcli/clibatch.py
--rw-r--r--   0        0        0    17190 2024-04-30 19:53:43.301938 centralcli-5.0.0/centralcli/clicaas.py
--rw-r--r--   0        0        0     2995 2023-08-30 16:01:18.958011 centralcli-5.0.0/centralcli/cliclone.py
--rw-r--r--   0        0        0    27093 2024-05-17 03:06:34.436222 centralcli-5.0.0/centralcli/clicommon.py
--rw-r--r--   0        0        0    25379 2024-05-09 15:50:25.995104 centralcli-5.0.0/centralcli/clidel.py
--rw-r--r--   0        0        0     3249 2024-04-23 01:56:25.646381 centralcli-5.0.0/centralcli/clidelfirmware.py
--rw-r--r--   0        0        0     1800 2024-05-21 03:46:04.962340 centralcli-5.0.0/centralcli/cliexport.py
--rw-r--r--   0        0        0     4765 2023-08-30 16:01:18.958011 centralcli-5.0.0/centralcli/clikick.py
--rw-r--r--   0        0        0      453 2024-05-01 03:52:02.285371 centralcli-5.0.0/centralcli/clioptions.py
--rw-r--r--   0        0        0     5608 2024-04-29 16:14:15.397597 centralcli-5.0.0/centralcli/clirefresh.py
--rw-r--r--   0        0        0     5316 2024-04-30 21:44:22.507322 centralcli-5.0.0/centralcli/clirename.py
--rw-r--r--   0        0        0      712 2024-04-22 23:50:21.991969 centralcli-5.0.0/centralcli/cliset.py
--rw-r--r--   0        0        0     3624 2024-04-23 01:57:48.666559 centralcli-5.0.0/centralcli/clisetfirmware.py
--rw-r--r--   0        0        0   161485 2024-05-22 05:44:01.033732 centralcli-5.0.0/centralcli/clishow.py
--rw-r--r--   0        0        0     8253 2024-05-01 05:18:45.977716 centralcli-5.0.0/centralcli/clishowaudit.py
--rw-r--r--   0        0        0     3943 2023-08-30 16:01:18.958011 centralcli-5.0.0/centralcli/clishowbranch.py
--rw-r--r--   0        0        0     5377 2024-05-21 02:55:20.859375 centralcli-5.0.0/centralcli/clishowcloudauth.py
--rw-r--r--   0        0        0     7356 2024-05-16 00:21:38.288411 centralcli-5.0.0/centralcli/clishowfirmware.py
--rw-r--r--   0        0        0     6273 2024-05-21 16:39:45.228432 centralcli-5.0.0/centralcli/clishowmpsk.py
--rw-r--r--   0        0        0    12980 2023-08-30 16:01:18.958011 centralcli-5.0.0/centralcli/clishowospf.py
--rw-r--r--   0        0        0    10809 2024-04-22 23:42:36.251725 centralcli-5.0.0/centralcli/clishowoverlay.py
--rw-r--r--   0        0        0     4956 2024-04-24 18:44:09.045709 centralcli-5.0.0/centralcli/clishowtshoot.py
--rw-r--r--   0        0        0    21550 2023-08-30 16:01:18.958011 centralcli-5.0.0/centralcli/clishowwids.py
--rw-r--r--   0        0        0     8451 2024-04-29 13:56:13.138575 centralcli-5.0.0/centralcli/clitest.py
--rw-r--r--   0        0        0    21213 2024-05-22 05:12:36.481093 centralcli-5.0.0/centralcli/clitshoot.py
--rw-r--r--   0        0        0     5888 2023-10-17 20:00:18.020614 centralcli-5.0.0/centralcli/cliunassign.py
--rw-r--r--   0        0        0    24517 2024-05-09 15:12:16.482928 centralcli-5.0.0/centralcli/cliupdate.py
--rw-r--r--   0        0        0     9005 2024-05-16 00:24:57.059018 centralcli-5.0.0/centralcli/cliupgrade.py
--rw-r--r--   0        0        0    26011 2024-05-22 00:32:11.959887 centralcli-5.0.0/centralcli/config.py
--rw-r--r--   0        0        0    41189 2024-05-21 15:42:11.777045 centralcli-5.0.0/centralcli/constants.py
--rw-r--r--   0        0        0      487 2024-04-23 00:38:18.706030 centralcli-5.0.0/centralcli/exceptions.py
--rw-r--r--   0        0        0     7253 2024-05-11 04:41:47.617937 centralcli-5.0.0/centralcli/logger.py
--rw-r--r--   0        0        0    19371 2024-05-21 14:06:48.814985 centralcli-5.0.0/centralcli/models.py
--rw-r--r--   0        0        0     3488 2023-10-26 00:01:09.236218 centralcli-5.0.0/centralcli/objects.py
--rw-r--r--   0        0        0    18371 2024-05-21 21:57:27.529879 centralcli-5.0.0/centralcli/render.py
--rw-r--r--   0        0        0    42257 2024-05-20 21:53:27.311619 centralcli-5.0.0/centralcli/response.py
--rw-r--r--   0        0        0       96 2021-10-13 20:41:19.000000 centralcli-5.0.0/centralcli/setup.py
--rw-r--r--   0        0        0     1150 2023-08-30 16:01:18.958011 centralcli-5.0.0/centralcli/static/favicon.ico
--rw-r--r--   0        0        0    15720 2024-05-21 03:27:38.321124 centralcli-5.0.0/centralcli/strings.py
--rw-r--r--   0        0        0    32263 2024-05-16 22:03:20.378955 centralcli-5.0.0/centralcli/utils.py
--rw-r--r--   0        0        0     5407 2023-08-30 16:01:18.958011 centralcli-5.0.0/centralcli/vscodeargs.py
--rw-r--r--   0        0        0    15335 2023-08-30 16:01:18.958011 centralcli-5.0.0/centralcli/wh2snow.py
--rw-r--r--   0        0        0    16108 2023-11-17 17:52:25.095728 centralcli-5.0.0/centralcli/wh_proxy.py
--rw-r--r--   0        0        0      393 2023-08-30 16:01:18.958011 centralcli-5.0.0/centralcli/wh_proxy_service.py
--rw-r--r--   0        0        0     2256 2024-05-22 05:51:33.224382 centralcli-5.0.0/pyproject.toml
--rw-r--r--   0        0        0    14176 1970-01-01 00:00:00.000000 centralcli-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-30 16:01:18.948011 centralcli-5.1.0/LICENSE
+-rw-r--r--   0        0        0    12115 2023-08-30 16:01:34.228021 centralcli-5.1.0/README.md
+-rw-r--r--   0        0        0     5732 2024-05-23 01:49:09.584685 centralcli-5.1.0/centralcli/__init__.py
+-rw-r--r--   0        0        0     1265 2023-09-08 18:43:03.749878 centralcli-5.1.0/centralcli/boilerplate/README.md
+-rw-r--r--   0        0        0  1156267 2024-05-14 22:05:46.978274 centralcli-5.1.0/centralcli/boilerplate/allcalls.py
+-rw-r--r--   0        0        0    11951 2024-05-05 02:42:27.903512 centralcli-5.1.0/centralcli/caas.py
+-rw-r--r--   0        0        0   127668 2024-05-23 14:23:35.674415 centralcli-5.1.0/centralcli/cache.py
+-rw-r--r--   0        0        0   224129 2024-05-23 03:18:49.474339 centralcli-5.1.0/centralcli/central.py
+-rw-r--r--   0        0        0    61017 2024-05-23 13:42:07.252386 centralcli-5.1.0/centralcli/cleaner.py
+-rw-r--r--   0        0        0    47385 2024-05-23 01:52:13.545370 centralcli-5.1.0/centralcli/cli.py
+-rw-r--r--   0        0        0    29011 2024-05-13 14:28:13.658447 centralcli-5.1.0/centralcli/cliadd.py
+-rw-r--r--   0        0        0     5388 2024-04-29 15:32:55.074272 centralcli-5.1.0/centralcli/cliassign.py
+-rw-r--r--   0        0        0   100595 2024-05-21 03:28:12.531138 centralcli-5.1.0/centralcli/clibatch.py
+-rw-r--r--   0        0        0    17190 2024-04-30 19:53:43.301938 centralcli-5.1.0/centralcli/clicaas.py
+-rw-r--r--   0        0        0     2747 2024-05-23 16:22:36.443011 centralcli-5.1.0/centralcli/cliclone.py
+-rw-r--r--   0        0        0    27658 2024-05-23 19:37:43.991489 centralcli-5.1.0/centralcli/clicommon.py
+-rw-r--r--   0        0        0    25379 2024-05-09 15:50:25.995104 centralcli-5.1.0/centralcli/clidel.py
+-rw-r--r--   0        0        0     3249 2024-04-23 01:56:25.646381 centralcli-5.1.0/centralcli/clidelfirmware.py
+-rw-r--r--   0        0        0     1800 2024-05-21 03:46:04.962340 centralcli-5.1.0/centralcli/cliexport.py
+-rw-r--r--   0        0        0     4765 2023-08-30 16:01:18.958011 centralcli-5.1.0/centralcli/clikick.py
+-rw-r--r--   0        0        0      453 2024-05-01 03:52:02.285371 centralcli-5.1.0/centralcli/clioptions.py
+-rw-r--r--   0        0        0     5608 2024-04-29 16:14:15.397597 centralcli-5.1.0/centralcli/clirefresh.py
+-rw-r--r--   0        0        0     5316 2024-04-30 21:44:22.507322 centralcli-5.1.0/centralcli/clirename.py
+-rw-r--r--   0        0        0      712 2024-04-22 23:50:21.991969 centralcli-5.1.0/centralcli/cliset.py
+-rw-r--r--   0        0        0     3624 2024-04-23 01:57:48.666559 centralcli-5.1.0/centralcli/clisetfirmware.py
+-rw-r--r--   0        0        0   167971 2024-05-24 01:09:26.968727 centralcli-5.1.0/centralcli/clishow.py
+-rw-r--r--   0        0        0     8253 2024-05-01 05:18:45.977716 centralcli-5.1.0/centralcli/clishowaudit.py
+-rw-r--r--   0        0        0     3943 2023-08-30 16:01:18.958011 centralcli-5.1.0/centralcli/clishowbranch.py
+-rw-r--r--   0        0        0     5377 2024-05-21 02:55:20.859375 centralcli-5.1.0/centralcli/clishowcloudauth.py
+-rw-r--r--   0        0        0     7356 2024-05-16 00:21:38.288411 centralcli-5.1.0/centralcli/clishowfirmware.py
+-rw-r--r--   0        0        0     6273 2024-05-21 16:39:45.228432 centralcli-5.1.0/centralcli/clishowmpsk.py
+-rw-r--r--   0        0        0    12980 2023-08-30 16:01:18.958011 centralcli-5.1.0/centralcli/clishowospf.py
+-rw-r--r--   0        0        0    10809 2024-04-22 23:42:36.251725 centralcli-5.1.0/centralcli/clishowoverlay.py
+-rw-r--r--   0        0        0     5316 2024-05-24 00:39:27.647050 centralcli-5.1.0/centralcli/clishowtshoot.py
+-rw-r--r--   0        0        0    21550 2023-08-30 16:01:18.958011 centralcli-5.1.0/centralcli/clishowwids.py
+-rw-r--r--   0        0        0     8451 2024-04-29 13:56:13.138575 centralcli-5.1.0/centralcli/clitest.py
+-rw-r--r--   0        0        0    21257 2024-05-24 01:24:50.065379 centralcli-5.1.0/centralcli/clitshoot.py
+-rw-r--r--   0        0        0     5888 2023-10-17 20:00:18.020614 centralcli-5.1.0/centralcli/cliunassign.py
+-rw-r--r--   0        0        0    24501 2024-05-22 18:12:15.824110 centralcli-5.1.0/centralcli/cliupdate.py
+-rw-r--r--   0        0        0     9014 2024-05-24 00:25:44.943374 centralcli-5.1.0/centralcli/cliupgrade.py
+-rw-r--r--   0        0        0    26011 2024-05-22 00:32:11.959887 centralcli-5.1.0/centralcli/config.py
+-rw-r--r--   0        0        0    41602 2024-05-23 14:52:37.387568 centralcli-5.1.0/centralcli/constants.py
+-rw-r--r--   0        0        0      487 2024-04-23 00:38:18.706030 centralcli-5.1.0/centralcli/exceptions.py
+-rw-r--r--   0        0        0     7162 2024-05-23 15:11:02.348775 centralcli-5.1.0/centralcli/logger.py
+-rw-r--r--   0        0        0    19704 2024-05-23 02:06:35.868059 centralcli-5.1.0/centralcli/models.py
+-rw-r--r--   0        0        0     3488 2023-10-26 00:01:09.236218 centralcli-5.1.0/centralcli/objects.py
+-rw-r--r--   0        0        0    18625 2024-05-23 18:49:21.540816 centralcli-5.1.0/centralcli/render.py
+-rw-r--r--   0        0        0    42257 2024-05-20 21:53:27.311619 centralcli-5.1.0/centralcli/response.py
+-rw-r--r--   0        0        0       96 2021-10-13 20:41:19.000000 centralcli-5.1.0/centralcli/setup.py
+-rw-r--r--   0        0        0     1150 2023-08-30 16:01:18.958011 centralcli-5.1.0/centralcli/static/favicon.ico
+-rw-r--r--   0        0        0    15720 2024-05-21 03:27:38.321124 centralcli-5.1.0/centralcli/strings.py
+-rw-r--r--   0        0        0    32263 2024-05-16 22:03:20.378955 centralcli-5.1.0/centralcli/utils.py
+-rw-r--r--   0        0        0     5407 2023-08-30 16:01:18.958011 centralcli-5.1.0/centralcli/vscodeargs.py
+-rw-r--r--   0        0        0    15335 2023-08-30 16:01:18.958011 centralcli-5.1.0/centralcli/wh2snow.py
+-rw-r--r--   0        0        0    16108 2023-11-17 17:52:25.095728 centralcli-5.1.0/centralcli/wh_proxy.py
+-rw-r--r--   0        0        0      393 2023-08-30 16:01:18.958011 centralcli-5.1.0/centralcli/wh_proxy_service.py
+-rw-r--r--   0        0        0     2256 2024-05-24 01:29:35.096835 centralcli-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0    14176 1970-01-01 00:00:00.000000 centralcli-5.1.0/PKG-INFO
```

### Comparing `centralcli-5.0.0/LICENSE` & `centralcli-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/README.md` & `centralcli-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/__init__.py` & `centralcli-5.1.0/centralcli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,17 +136,17 @@
 os.environ["LESS"] = "-RX +G"
 
 if os.environ.get("TERM_PROGRAM") == "vscode":
     from .vscodeargs import vscode_arg_handler
     vscode_arg_handler()
 
 raw_out = False
-if "-vv" in sys.argv:
+if "--raw" in sys.argv:
     raw_out = True
-    _ = sys.argv.pop(sys.argv.index("-vv"))
+    _ = sys.argv.pop(sys.argv.index("--raw"))
 if "--debug-limit" in sys.argv:
     _idx = sys.argv.index("--debug-limit")
     _ = sys.argv.pop(sys.argv.index("--debug-limit"))
     if len(sys.argv) - 1 >= _idx and sys.argv[_idx].isdigit():
         config.limit = int(sys.argv[_idx])
         _ = sys.argv.pop(_idx)
     else:
```

### Comparing `centralcli-5.0.0/centralcli/boilerplate/README.md` & `centralcli-5.1.0/centralcli/boilerplate/README.md`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/boilerplate/allcalls.py` & `centralcli-5.1.0/centralcli/boilerplate/allcalls.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/caas.py` & `centralcli-5.1.0/centralcli/caas.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/cache.py` & `centralcli-5.1.0/centralcli/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 
 from __future__ import annotations
 
 import asyncio
 import time
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Literal, Sequence, Set, Union, Generator, Tuple
+from typing import Any, Dict, Iterable, List, Literal, Sequence, Set, Union, Generator, Tuple, Callable
 
 import typer
 from rich import print
 from rich.console import Console
 from tinydb import Query, TinyDB
-from tinydb.table import Table
+from tinydb.table import Table, Document
 from copy import deepcopy
 
 from centralcli import CentralApi, Response, cleaner, config, constants, log, models, render, utils
 
 try:
     import readline  # noqa imported for backspace support during prompt.
 except Exception:
     pass
 
-# TODO remove after TESTING NEW string matching lookup
 try:
     from fuzzywuzzy import process  # type: ignore noqa
     FUZZ = True
 except Exception:
     FUZZ = False
-    pass
 
 # Used to debug completion
 err_console = Console(stderr=True)
 emoji_console = Console()
 console = Console(emoji=False)
 TinyDB.default_table_name = "devices"
 
@@ -63,19 +61,19 @@
     """
     return LIB_DEV_TYPE.get(dev_type, dev_type)
 
 
 class CentralObject:
     def __init__(
         self,
-        db: Literal["dev", "site", "template", "group", "label"],
+        db: Literal["dev", "site", "template", "group", "label", "mpsk", "portal"],
         data: Union[list, Dict[str, Any]],
     ) -> Union[list, Dict[str, Any]]:
-        self.is_dev, self.is_template, self.is_group, self.is_site, self.is_label = False, False, False, False, False
-        data = None if not data else data
+        self.is_dev, self.is_template, self.is_group, self.is_site, self.is_label, self.is_mpsk, self.is_portal = False, False, False, False, False, False, False
+        data: Dict | List[dict] = None if not data else data
         setattr(self, f"is_{db}", True)
         self.cache = db
 
         if isinstance(data, list):
             if len(data) > 1:
                 raise ValueError(f"CentralObject expects a single item. Got list of {len(data)}")
             elif data:
@@ -87,14 +85,15 @@
         # TODO maybe pydantic model
         if self.is_dev and self.data:
             self.name = self.data["name"] = self.data.get("name", self.data["serial"])
             self.status = self.data["status"] = self.data.get("status")
             self.ip = self.data["ip"] = self.data.get("ip")
             self.site = self.data["site"] = self.data.get("site")
             self.swack_id = self.data["swack_id"] = self.data.get("swack_id")
+            self.serial: str = self.data.get("serial")
 
     def __bool__(self):
         return bool(self.data)
 
     def __repr__(self):
         _ = f"<{self.__module__}.{type(self).__name__} ({self.cache}|{self.get('name', bool(self))}) object at {hex(id(self))}>"
         return _
@@ -210,26 +209,30 @@
         self,
         dev: Response = None,
         inv: Response = None,
         site: Response = None,
         template: Response = None,
         group: Response = None,
         label: Response = None,
+        mpsk: Response = None,
+        portal: Response = None,
     ) -> None:
         self._dev = dev
         self._inv = inv
         self._site = site
         self._template = template
         self._group = group
         self._label = label
+        self._mpsk = mpsk
+        self._portal = portal
 
     def update_rl(self, resp: Response) -> Response:
         """Returns provided Response object with the RateLimit info from the most recent API call.
         """
-        _last_rl = sorted([r.rl for r in [self._dev, self._inv, self._site, self._template, self._group] if r is not None], key=lambda k: k.remain_day)
+        _last_rl = sorted([r.rl for r in [self._dev, self._inv, self._site, self._template, self._group, self._label, self._mpsk, self._portal] if r is not None], key=lambda k: k.remain_day)
         if _last_rl:
             resp.rl = _last_rl[0]
         return resp
 
     @property
     def dev(self):
         return self.update_rl(self._dev)
@@ -274,14 +277,30 @@
     def label(self):
         return self.update_rl(self._label)
 
     @label.setter
     def label(self, resp: Response):
         self._label = resp
 
+    @property
+    def mpsk(self):
+        return self.update_rl(self._mpsk)
+
+    @mpsk.setter
+    def mpsk(self, resp: Response):
+        self._mpsk = resp
+
+    @property
+    def portal(self):
+        return self.update_rl(self._portal)
+
+    @portal.setter
+    def portal(self, resp: Response):
+        self._portal = resp
+
 
 class Cache:
     def __init__(
         self,
         central: CentralApi = None,
         data: Union[List[dict], dict] = None,
         refresh: bool = False,
@@ -305,14 +324,15 @@
             # vs the actual log id in form 'audit_trail_2021_2,...'
             # it is updated anytime show logs is ran.
             self.LogDB: Table = self.DevDB.table("logs")
             self.EventDB: Table = self.DevDB.table("events")
             self.HookConfigDB: Table = self.DevDB.table("wh_config")
             self.HookDataDB: Table = self.DevDB.table("wh_data")
             self.MpskDB: Table = self.DevDB.table("mpsk")  # Only updated when show mpsk networks is ran or as needed when show named-mpsk <SSID> is ran
+            self.PortalDB: Table = self.DevDB.table("portal")  # Only updated when show portals is ran or as needed
             self._tables = [self.DevDB, self.InvDB, self.SiteDB, self.GroupDB, self.TemplateDB, self.LabelDB, self.LicenseDB, self.ClientDB]
             self.Q = Query()
             if data:
                 self.insert(data)
             if central:
                 self.check_fresh(refresh)
 
@@ -326,15 +346,16 @@
 
     @property
     def devices(self) -> list:
         return self.DevDB.all()
 
     @property
     def device_types(self) -> Set[str]:
-        return set([d["type"] if d["type"] not in ["cx", "sw"] else "switch" for d in self.DevDB.all()])
+        db = self.InvDB if self.InvDB else self.DevDB
+        return set([d["type"] for d in db.all()])
 
     @property
     def devices_by_serial(self) -> dict:
         return {d["serial"]: d for d in self.devices}
 
     @property
     def inventory(self) -> list:
@@ -375,14 +396,18 @@
         return self.ClientDB.all()
 
     @property
     def mpsk(self) -> list:
         return self.MpskDB.all()
 
     @property
+    def portals(self) -> list:
+        return self.PortalDB.all()
+
+    @property
     def logs(self) -> list:
         return self.LogDB.all()
 
     @property
     def events(self) -> list:
         return self.EventDB.all()
 
@@ -724,15 +749,48 @@
         match = self.get_mpsk_identifier(
             incomplete,
             completion=True,
         )
         out = []
         args = args or ctx.params.values()  # HACK as args stopped working
         if match:
-            # remove devices that are already on the command line
+            # remove items that are already on the command line
+            match = [m for m in match if m.name not in args]
+            for m in sorted(match, key=lambda i: i.name):
+                if m.name.startswith(incomplete):
+                    out += [tuple([m.name, m.id])]
+                elif m.id.startswith(incomplete):
+                    out += [tuple([m.id, m.name])]
+                else:
+                    out += [tuple([m.name, m.help_text])]  # failsafe, shouldn't hit
+
+        for m in out:
+            yield m
+
+    # TODO one common completion that is referenced by multiple xx_completions passing in ctx and the get__identifier func/args
+    def portal_completion(
+        self,
+        ctx: typer.Context,
+        incomplete: str,
+        args: List[str] = None,
+    ):
+        # Prevents exception during completion when config missing or invalid
+        if not config.valid:
+            err_console.print(":warning:  Invalid config")
+            return
+
+        match = self.get_name_id_identifier(
+            "portal",
+            incomplete,
+            completion=True,
+        )
+        out = []
+        args = args or ctx.params.values()  # HACK as args stopped working
+        if match:
+            # remove items that are already on the command line
             match = [m for m in match if m.name not in args]
             for m in sorted(match, key=lambda i: i.name):
                 if m.name.startswith(incomplete):
                     out += [tuple([m.name, m.id])]
                 elif m.id.startswith(incomplete):
                     out += [tuple([m.id, m.name])]
                 else:
@@ -1954,16 +2012,18 @@
         else:
             data = [*self.hook_active, *data]
             self.HookDataDB.truncate()
             return self.HookDataDB.insert_multiple(data)
 
     async def update_mpsk_db(self, data: List[Dict[str, Any]] = None) -> bool:
         if data:
-            data = models.CacheMpskNetworks(data)
-            data = data.dict()
+            if isinstance(data, list):
+                data = {"items": data}
+            data = models.CacheMpskNetworks(**data)
+            data = data.dict()["items"]
             self.MpskDB.truncate()
             return self.MpskDB.insert_multiple(data)
         else:
             resp = await self.central.cloudauth_get_mpsk_networks()
             if resp.ok:
                 if resp.output:
                     _update_data = utils.listify(deepcopy(resp.output))
@@ -1973,15 +2033,40 @@
                     self.MpskDB.truncate()
                     update_res = self.MpskDB.insert_multiple(_update_data)
                     if False in update_res:
                         log.error("Tiny DB returned an error during MPSK db update", caption=True)
 
                 # TODO change updated from  list of funcs to class with bool attributes or something
                 self.updated.append(self.central.cloudauth_get_mpsk_networks)
-                self.responses.dev = resp
+                self.responses.mpsk = resp
+            return resp
+
+    async def update_portal_db(self, data: List[Dict[str, Any]] = None) -> bool:
+        if data:
+            if isinstance(data, list):
+                data = {"portals": data}
+            data = models.CachePortals(**data)
+            data = data.dict()["portals"]
+            self.PortalDB.truncate()
+            return self.PortalDB.insert_multiple(data)
+        else:
+            resp = await self.central.get_portals()
+            if resp.ok:
+                if resp.output:
+                    _update_data = utils.listify(deepcopy(resp.output))
+                    _update_data = models.CachePortals(**resp.raw)
+                    _update_data = _update_data.dict()["portals"]
+
+                    self.PortalDB.truncate()
+                    update_res = self.PortalDB.insert_multiple(_update_data)
+                    if False in update_res:
+                        log.error("Tiny DB returned an error during Portal db update", caption=True)
+
+                self.updated.append(self.central.get_portals)
+                self.responses.portal = resp
             return resp
 
     # TODO cache.groups cache.devices etc change to Response object with data in output.  So they can be leveraged in commands with all attributes
     async def _check_fresh(
         self,
         dev_db: bool = False,
         inv_db: bool = False,
@@ -2909,8 +2994,109 @@
             print(f":warning:  [cyan]{query_str}[/] appears to be invalid")
             print(f"\n[bright_green]Valid MPSK Networks[/]:\n--\n{valid_mpsk}\n--\n")
             raise typer.Exit(1)
         else:
             if not completion:
                 log.error(
                     f"Central API CLI Cache unable to gather label data from provided identifier {query_str}", show=not silent
-                )
+                )
+
+
+    def get_name_id_identifier(
+        self,
+        cache_name: Literal["dev", "site", "template", "group", "label", "mpsk", "portal"],
+        query_str: str,
+        retry: bool = True,
+        completion: bool = False,
+        silent: bool = False,
+    ) -> CentralObject | List[CentralObject]:
+        cache_details = CacheDetails(self)
+        this: CacheAttributes = getattr(cache_details, cache_name)
+        db_all = this.db.all()
+        db = this.db
+        """Allows Case insensitive ssid match"""
+        retry = False if completion else retry
+        for _ in range(0, 2):
+            if query_str == "":
+                match = db_all
+            else:
+                match = db.search((self.Q.name == query_str))
+
+            # case insensitive
+            if not match:
+                match = db.search(
+                    self.Q.name.test(lambda v: v.lower() == query_str.lower())
+                )
+
+            # case insensitive startswith
+            if not match:
+                match = db.search(
+                    self.Q.name.test(lambda v: v.lower().startswith(query_str.lower()))
+                )
+
+            # case insensitive ignore -_
+            if not match:
+                if "_" in query_str or "-" in query_str:
+                    match = db.search(
+                        self.Q.name.test(
+                            lambda v: v.lower().strip("-_") == query_str.lower().strip("_-")
+                        )
+                    )
+
+            # case insensitive startswith search for mspk id
+            if not match:
+                match = db.search(
+                    self.Q.id.test(
+                        lambda v: v.lower().startswith(query_str.lower())
+                    )
+                )
+
+            if not match and retry and this.already_updated_func not in self.updated:
+                if FUZZ:
+                    fuzz_resp = process.extract(query_str, [item["name"] for item in db_all], limit=1)
+                    if fuzz_resp:
+                        fuzz_match, fuzz_confidence = fuzz_resp[0]
+                        confirm_str = render.rich_capture(f"[bright_red]{query_str}[/] not found in cache.  Did you mean [green3]{fuzz_match}[/]?")
+                        if fuzz_confidence >= 70 and typer.confirm(confirm_str):
+                            match = self.db.search(self.Q.name == fuzz_match)
+                if not match:
+                    err_console.print(f":warning:  [bright_red]No Match found for[/] [cyan]{query_str}[/].  Updating {cache_name} Cache")
+                    asyncio.run(this.cache_update_func())
+                _ += 1
+            if match:
+                match = [CentralObject(this.name, g) for g in match]
+                break
+
+        if completion:
+            return match or []
+
+        if match:
+            if len(match) > 1:
+                match = self.handle_multi_match(match, query_str=query_str, query_type=this.name,)
+
+            return match[0]
+
+        elif retry:
+            log.error(f"Central API CLI Cache unable to gather label data from provided identifier {query_str}", show=True)
+            valid = "\n".join([f'[cyan]{m["name"]}[/]' for m in db_all])
+            print(f":warning:  [cyan]{query_str}[/] appears to be invalid")
+            print(f"\n[bright_green]Valid Names[/]:\n--\n{valid}\n--\n")
+            raise typer.Exit(1)
+        else:
+            if not completion:
+                log.error(
+                    f"Central API CLI Cache unable to gather label data from provided identifier {query_str}", show=not silent
+                )
+
+class CacheAttributes:
+    def __init__(self, name: Literal["dev", "site", "template", "group", "label", "mpsk", "portal"], db: Table, already_updated_func: Callable, cache_update_func: Callable) -> None:
+        self.name = name
+        self.db = db
+        self.already_updated_func = already_updated_func
+        self.cache_update_func = cache_update_func
+
+class CacheDetails:
+    def __init__(self, cache = Cache):
+        self.dev = CacheAttributes(name="dev", db=cache.DevDB, already_updated_func=cache.central.get_all_devicesv2, cache_update_func=cache.update_dev_db)
+        self.site = CacheAttributes(name="site", db=cache.SiteDB, already_updated_func=cache.central.get_all_sites, cache_update_func=cache.update_site_db)
+        self.portal = CacheAttributes(name="portal", db=cache.PortalDB, already_updated_func=cache.central.get_portals, cache_update_func=cache.update_portal_db)
+        self.mpsk = CacheAttributes(name="mpsk", db=cache.MpskDB, already_updated_func=cache.central.cloudauth_get_mpsk_networks, cache_update_func=cache.update_mpsk_db)
```

### Comparing `centralcli-5.0.0/centralcli/central.py` & `centralcli-5.1.0/centralcli/central.py`

 * *Files 1% similar despite different names*

```diff
@@ -12327,1660 +12327,1683 @@
 00030260: 2027 6f66 6673 6574 273a 206f 6666 7365   'offset': offse
 00030270: 742c 0a20 2020 2020 2020 2020 2020 2027  t,.            '
 00030280: 6c69 6d69 7427 3a20 6c69 6d69 740a 2020  limit': limit.  
 00030290: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
 000302a0: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
 000302b0: 6c66 2e67 6574 2875 726c 2c20 7061 7261  lf.get(url, para
 000302c0: 6d73 3d70 6172 616d 7329 0a0a 2020 2020  ms=params)..    
-000302d0: 6173 796e 6320 6465 6620 6765 745f 7669  async def get_vi
-000302e0: 7369 746f 7273 280a 2020 2020 2020 2020  sitors(.        
-000302f0: 7365 6c66 2c0a 2020 2020 2020 2020 706f  self,.        po
-00030300: 7274 616c 5f69 643a 2073 7472 2c0a 2020  rtal_id: str,.  
-00030310: 2020 2020 2020 736f 7274 3a20 7374 7220        sort: str 
-00030320: 3d20 272b 6e61 6d65 272c 0a20 2020 2020  = '+name',.     
-00030330: 2020 2066 696c 7465 725f 6279 3a20 7374     filter_by: st
-00030340: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00030350: 2020 6669 6c74 6572 5f76 616c 7565 3a20    filter_value: 
-00030360: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00030370: 2020 2020 6f66 6673 6574 3a20 696e 7420      offset: int 
-00030380: 3d20 302c 0a20 2020 2020 2020 206c 696d  = 0,.        lim
-00030390: 6974 3a20 696e 7420 3d20 3130 302c 0a20  it: int = 100,. 
-000303a0: 2020 2029 202d 3e20 5265 7370 6f6e 7365     ) -> Response
-000303b0: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
-000303c0: 2061 6c6c 2076 6973 6974 6f72 7320 6372   all visitors cr
-000303d0: 6561 7465 6420 6167 6169 6e73 7420 6120  eated against a 
-000303e0: 706f 7274 616c 2e0a 0a20 2020 2020 2020  portal...       
-000303f0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00030400: 2020 2070 6f72 7461 6c5f 6964 2028 7374     portal_id (st
-00030410: 7229 3a20 506f 7274 616c 2049 4420 6f66  r): Portal ID of
-00030420: 2074 6865 2073 706c 6173 6820 7061 6765   the splash page
-00030430: 0a20 2020 2020 2020 2020 2020 2073 6f72  .            sor
-00030440: 7420 2873 7472 2c20 6f70 7469 6f6e 616c  t (str, optional
-00030450: 293a 202b 2069 7320 666f 7220 6173 6365  ): + is for asce
-00030460: 6e64 696e 6720 2061 6e64 202d 2066 6f72  nding  and - for
-00030470: 2064 6573 6365 6e64 696e 6720 6f72 6465   descending orde
-00030480: 7220 2c20 736f 7274 7320 6279 206e 616d  r , sorts by nam
-00030490: 6520 666f 720a 2020 2020 2020 2020 2020  e for.          
-000304a0: 2020 2020 2020 6e6f 7720 2056 616c 6964        now  Valid
-000304b0: 2056 616c 7565 733a 202b 6e61 6d65 2c20   Values: +name, 
-000304c0: 2d6e 616d 650a 2020 2020 2020 2020 2020  -name.          
-000304d0: 2020 6669 6c74 6572 5f62 7920 2873 7472    filter_by (str
-000304e0: 2c20 6f70 7469 6f6e 616c 293a 2066 696c  , optional): fil
-000304f0: 7465 7220 6279 2065 6d61 696c 206f 7220  ter by email or 
-00030500: 6e61 6d65 2020 5661 6c69 6420 5661 6c75  name  Valid Valu
-00030510: 6573 3a20 6e61 6d65 2c20 656d 6169 6c0a  es: name, email.
-00030520: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
-00030530: 6572 5f76 616c 7565 2028 7374 722c 206f  er_value (str, o
-00030540: 7074 696f 6e61 6c29 3a20 6669 6c74 6572  ptional): filter
-00030550: 2076 616c 7565 0a20 2020 2020 2020 2020   value.         
-00030560: 2020 206f 6666 7365 7420 2869 6e74 2c20     offset (int, 
-00030570: 6f70 7469 6f6e 616c 293a 2053 7461 7274  optional): Start
-00030580: 696e 6720 696e 6465 7820 6f66 2065 6c65  ing index of ele
-00030590: 6d65 6e74 2066 6f72 2061 2070 6167 696e  ment for a pagin
-000305a0: 6174 6564 2071 7565 7279 2044 6566 6175  ated query Defau
-000305b0: 6c74 7320 746f 2030 2e0a 2020 2020 2020  lts to 0..      
-000305c0: 2020 2020 2020 6c69 6d69 7420 2869 6e74        limit (int
-000305d0: 2c20 6f70 7469 6f6e 616c 293a 204e 756d  , optional): Num
-000305e0: 6265 7220 6f66 2069 7465 6d73 2072 6571  ber of items req
-000305f0: 7569 7265 6420 7065 7220 7175 6572 7920  uired per query 
-00030600: 4465 6661 756c 7473 2074 6f20 3130 302e  Defaults to 100.
-00030610: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00030620: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00030630: 6573 706f 6e73 653a 2043 656e 7472 616c  esponse: Central
-00030640: 4150 4920 5265 7370 6f6e 7365 206f 626a  API Response obj
-00030650: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
-00030660: 2020 2020 2020 2020 7572 6c20 3d20 6622          url = f"
-00030670: 2f67 7565 7374 2f76 312f 706f 7274 616c  /guest/v1/portal
-00030680: 732f 7b70 6f72 7461 6c5f 6964 7d2f 7669  s/{portal_id}/vi
-00030690: 7369 746f 7273 220a 0a20 2020 2020 2020  sitors"..       
-000306a0: 2070 6172 616d 7320 3d20 7b0a 2020 2020   params = {.    
-000306b0: 2020 2020 2020 2020 2773 6f72 7427 3a20          'sort': 
-000306c0: 736f 7274 2c0a 2020 2020 2020 2020 2020  sort,.          
-000306d0: 2020 2766 696c 7465 725f 6279 273a 2066    'filter_by': f
-000306e0: 696c 7465 725f 6279 2c0a 2020 2020 2020  ilter_by,.      
-000306f0: 2020 2020 2020 2766 696c 7465 725f 7661        'filter_va
-00030700: 6c75 6527 3a20 6669 6c74 6572 5f76 616c  lue': filter_val
-00030710: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00030720: 276f 6666 7365 7427 3a20 6f66 6673 6574  'offset': offset
-00030730: 2c0a 2020 2020 2020 2020 2020 2020 276c  ,.            'l
-00030740: 696d 6974 273a 206c 696d 6974 0a20 2020  imit': limit.   
-00030750: 2020 2020 207d 0a20 2020 2020 2020 2070       }.        p
-00030760: 6172 616d 7320 3d20 7574 696c 732e 7374  arams = utils.st
-00030770: 7269 705f 6e6f 6e65 2870 6172 616d 7329  rip_none(params)
-00030780: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00030790: 2061 7761 6974 2073 656c 662e 6765 7428   await self.get(
-000307a0: 7572 6c2c 2070 6172 616d 733d 7061 7261  url, params=para
-000307b0: 6d73 290a 0a0a 2020 2020 6173 796e 6320  ms)...    async 
-000307c0: 6465 6620 6164 645f 7669 7369 746f 7228  def add_visitor(
-000307d0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000307e0: 2020 2020 2020 2070 6f72 7461 6c5f 6964         portal_id
-000307f0: 3a20 7374 722c 0a20 2020 2020 2020 206e  : str,.        n
-00030800: 616d 653a 2073 7472 2c0a 2020 2020 2020  ame: str,.      
-00030810: 2020 2320 6964 3a20 7374 722c 0a20 2020    # id: str,.   
-00030820: 2020 2020 2070 6173 7377 6f72 643a 2073       password: s
-00030830: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-00030840: 2020 202a 2c0a 2020 2020 2020 2020 636f     *,.        co
-00030850: 6d70 616e 795f 6e61 6d65 3a20 7374 7220  mpany_name: str 
-00030860: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00030870: 7068 6f6e 653a 2073 7472 207c 204e 6f6e  phone: str | Non
-00030880: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
-00030890: 2020 656d 6169 6c3a 2073 7472 207c 204e    email: str | N
-000308a0: 6f6e 6520 3d20 4e6f 6e65 2c0a 2020 2020  one = None,.    
-000308b0: 2020 2020 7661 6c69 645f 666f 7265 7665      valid_foreve
-000308c0: 723a 2062 6f6f 6c20 3d20 4661 6c73 652c  r: bool = False,
-000308d0: 0a20 2020 2020 2020 2076 616c 6964 5f64  .        valid_d
-000308e0: 6179 733a 2069 6e74 203d 2033 2c0a 2020  ays: int = 3,.  
-000308f0: 2020 2020 2020 7661 6c69 645f 686f 7572        valid_hour
-00030900: 733a 2069 6e74 203d 2030 2c0a 2020 2020  s: int = 0,.    
-00030910: 2020 2020 7661 6c69 645f 6d69 6e75 7465      valid_minute
-00030920: 733a 2069 6e74 203d 2030 2c0a 2020 2020  s: int = 0,.    
-00030930: 2020 2020 6e6f 7469 6679 3a20 626f 6f6c      notify: bool
-00030940: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0a   | None = None,.
-00030950: 2020 2020 2020 2020 6e6f 7469 6679 5f74          notify_t
-00030960: 6f3a 2063 6f6e 7374 616e 7473 2e4e 6f74  o: constants.Not
-00030970: 6966 7954 6f41 7267 7320 7c20 4e6f 6e65  ifyToArgs | None
-00030980: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00030990: 2069 735f 656e 6162 6c65 643a 2062 6f6f   is_enabled: boo
-000309a0: 6c20 3d20 5472 7565 2c0a 2020 2020 2020  l = True,.      
-000309b0: 2020 2320 7374 6174 7573 3a20 626f 6f6c    # status: bool
-000309c0: 2c0a 2020 2020 2020 2020 2320 6372 6561  ,.        # crea
-000309d0: 7465 645f 6174 3a20 7374 722c 0a20 2020  ted_at: str,.   
-000309e0: 2020 2020 2023 2065 7870 6972 655f 6174       # expire_at
-000309f0: 3a20 7374 722c 0a20 2020 2029 202d 3e20  : str,.    ) -> 
-00030a00: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
-00030a10: 2020 2222 2243 7265 6174 6520 6120 6e65    """Create a ne
-00030a20: 7720 6775 6573 7420 7669 7369 746f 7220  w guest visitor 
-00030a30: 6f66 2061 2070 6f72 7461 6c2e 0a0a 2020  of a portal...  
-00030a40: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00030a50: 2020 2020 2020 2020 706f 7274 616c 5f69          portal_i
-00030a60: 6420 2873 7472 293a 2050 6f72 7461 6c20  d (str): Portal 
-00030a70: 4944 206f 6620 7468 6520 7370 6c61 7368  ID of the splash
-00030a80: 2070 6167 650a 2020 2020 2020 2020 2020   page.          
-00030a90: 2020 6e61 6d65 2028 7374 7229 3a20 5669    name (str): Vi
-00030aa0: 7369 746f 7220 6163 636f 756e 7420 6e61  sitor account na
-00030ab0: 6d65 0a20 2020 2020 2020 2020 2020 2070  me.            p
-00030ac0: 6173 7377 6f72 6420 2873 7472 293a 2050  assword (str): P
-00030ad0: 6173 7377 6f72 640a 2020 2020 2020 2020  assword.        
-00030ae0: 2020 2020 636f 6d70 616e 795f 6e61 6d65      company_name
-00030af0: 2028 7374 7229 3a20 436f 6d70 616e 7920   (str): Company 
-00030b00: 6e61 6d65 206f 6620 7468 6520 7669 7369  name of the visi
-00030b10: 746f 720a 2020 2020 2020 2020 2020 2020  tor.            
-00030b20: 7068 6f6e 6520 2873 7472 293a 2050 686f  phone (str): Pho
-00030b30: 6e65 206e 756d 6265 7220 6f66 2074 6865  ne number of the
-00030b40: 2076 6973 6974 6f72 3b20 466f 726d 6174   visitor; Format
-00030b50: 205b 2b43 6f75 6e74 7279 436f 6465 5d5b   [+CountryCode][
-00030b60: 5068 6f6e 654e 756d 6265 725d 0a20 2020  PhoneNumber].   
-00030b70: 2020 2020 2020 2020 2065 6d61 696c 2028           email (
-00030b80: 7374 7229 3a20 456d 6169 6c20 6164 6472  str): Email addr
-00030b90: 6573 7320 6f66 2074 6865 2076 6973 6974  ess of the visit
-00030ba0: 6f72 0a20 2020 2020 2020 2020 2020 2076  or.            v
-00030bb0: 616c 6964 5f66 6f72 6576 6572 2028 626f  alid_forever (bo
-00030bc0: 6f6c 293a 2056 6973 6974 6f72 2061 6363  ol): Visitor acc
-00030bd0: 6f75 6e74 2077 696c 6c20 6e6f 7420 6578  ount will not ex
-00030be0: 7069 7265 2077 6865 6e20 7468 6973 2069  pire when this i
-00030bf0: 7320 7365 7420 746f 2074 7275 650a 2020  s set to true.  
-00030c00: 2020 2020 2020 2020 2020 7661 6c69 645f            valid_
-00030c10: 6461 7973 2028 696e 7429 3a20 4163 636f  days (int): Acco
-00030c20: 756e 7420 7661 6c69 6469 7479 2069 6e20  unt validity in 
-00030c30: 6461 7973 0a20 2020 2020 2020 2020 2020  days.           
-00030c40: 2076 616c 6964 5f68 6f75 7273 2028 696e   valid_hours (in
-00030c50: 7429 3a20 4163 636f 756e 7420 7661 6c69  t): Account vali
-00030c60: 6469 7479 2069 6e20 686f 7572 730a 2020  dity in hours.  
-00030c70: 2020 2020 2020 2020 2020 7661 6c69 645f            valid_
-00030c80: 6d69 6e75 7465 7320 2869 6e74 293a 2041  minutes (int): A
-00030c90: 6363 6f75 6e74 2076 616c 6964 6974 7920  ccount validity 
-00030ca0: 696e 206d 696e 7574 6573 0a20 2020 2020  in minutes.     
-00030cb0: 2020 2020 2020 206e 6f74 6966 7920 2862         notify (b
-00030cc0: 6f6f 6c29 3a20 466c 6167 2074 6f20 6e6f  ool): Flag to no
-00030cd0: 7469 6679 2074 6865 2070 6173 7377 6f72  tify the passwor
-00030ce0: 6420 7669 6120 656d 6169 6c20 6f72 206e  d via email or n
-00030cf0: 756d 6265 720a 2020 2020 2020 2020 2020  umber.          
-00030d00: 2020 6e6f 7469 6679 5f74 6f20 2873 7472    notify_to (str
-00030d10: 293a 204e 6f74 6966 7920 746f 2065 6d61  ): Notify to ema
-00030d20: 696c 206f 7220 7068 6f6e 652e 2044 6566  il or phone. Def
-00030d30: 7561 6c74 2069 7320 7068 6f6e 6520 7768  ualt is phone wh
-00030d40: 656e 2069 7420 6973 2070 726f 7669 6465  en it is provide
-00030d50: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00030d60: 2020 6f74 6865 7277 6973 6520 656d 6169    otherwise emai
-00030d70: 6c2e 2020 5661 6c69 6420 5661 6c75 6573  l.  Valid Values
-00030d80: 3a20 656d 6169 6c2c 2070 686f 6e65 0a20  : email, phone. 
-00030d90: 2020 2020 2020 2020 2020 2069 735f 656e             is_en
-00030da0: 6162 6c65 6420 2862 6f6f 6c29 3a20 456e  abled (bool): En
-00030db0: 6162 6c65 206f 7220 6469 7361 626c 6520  able or disable 
-00030dc0: 7468 6520 7669 7369 746f 7220 6163 636f  the visitor acco
-00030dd0: 756e 740a 2020 2020 2020 2020 2020 2020  unt.            
-00030de0: 2320 6964 2028 7374 7229 3a20 4e41 2066  # id (str): NA f
-00030df0: 6f72 2076 6973 6974 6f72 2070 6f73 742f  or visitor post/
-00030e00: 7075 7420 6d65 7468 6f64 2e20 4944 206f  put method. ID o
-00030e10: 6620 7468 6520 7669 7369 746f 720a 2020  f the visitor.  
-00030e20: 2020 2020 2020 2020 2020 2320 7374 6174            # stat
-00030e30: 7573 2028 626f 6f6c 293a 2054 6869 7320  us (bool): This 
-00030e40: 6669 656c 6420 7072 6f76 6964 6573 2073  field provides s
-00030e50: 7461 7475 7320 6f66 2074 6865 2061 6363  tatus of the acc
-00030e60: 6f75 6e74 2e20 5265 7475 726e 7320 7472  ount. Returns tr
-00030e70: 7565 2077 6865 6e20 656e 6162 6c65 6420  ue when enabled 
-00030e80: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-00030e90: 2320 2020 2020 6e6f 7420 6578 7069 7265  #     not expire
-00030ea0: 642e 204e 4120 666f 7220 7669 7369 746f  d. NA for visito
-00030eb0: 7220 706f 7374 2f70 7574 206d 6574 686f  r post/put metho
-00030ec0: 642e 2054 6869 7320 6973 206f 7074 696f  d. This is optio
-00030ed0: 6e61 6c20 6669 656c 6473 2e0a 2020 2020  nal fields..    
-00030ee0: 2020 2020 2020 2020 2320 6372 6561 7465          # create
-00030ef0: 645f 6174 2028 7374 7229 3a20 5468 6973  d_at (str): This
-00030f00: 2066 6965 6c64 2069 6e64 6963 6174 6573   field indicates
-00030f10: 2074 6865 2063 7265 6174 6564 2064 6174   the created dat
-00030f20: 6520 7469 6d65 7374 616d 7020 7661 6c75  e timestamp valu
-00030f30: 652e 2049 7420 6973 2067 656e 6572 6174  e. It is generat
-00030f40: 6564 0a20 2020 2020 2020 2020 2020 2023  ed.            #
-00030f50: 2020 2020 2077 6869 6c65 2063 7265 6174       while creat
-00030f60: 696e 6720 7669 7369 746f 722e 204e 4120  ing visitor. NA 
-00030f70: 666f 7220 7669 7369 746f 7220 706f 7374  for visitor post
-00030f80: 2f70 7574 206d 6574 686f 642e 2054 6869  /put method. Thi
-00030f90: 7320 6973 206f 7074 696f 6e61 6c20 6669  s is optional fi
-00030fa0: 656c 642e 0a20 2020 2020 2020 2020 2020  eld..           
-00030fb0: 2023 2065 7870 6972 655f 6174 2028 7374   # expire_at (st
-00030fc0: 7229 3a20 5468 6973 2066 6965 6c64 2069  r): This field i
-00030fd0: 6e64 6963 6174 6573 2065 7870 6972 7920  ndicates expiry 
-00030fe0: 7469 6d65 2074 696d 6573 7461 6d70 2076  time timestamp v
-00030ff0: 616c 7565 2e20 4974 2069 7320 6765 6e65  alue. It is gene
-00031000: 7261 7465 6420 6261 7365 640a 2020 2020  rated based.    
-00031010: 2020 2020 2020 2020 2320 2020 2020 6f6e          #     on
-00031020: 2074 6865 2076 616c 6964 5f74 696c 6c20   the valid_till 
-00031030: 7661 6c75 6520 616e 6420 6372 6561 7465  value and create
-00031040: 645f 6174 2074 696d 652e 204e 4120 666f  d_at time. NA fo
-00031050: 7220 7669 7369 746f 7220 706f 7374 2f70  r visitor post/p
-00031060: 7574 206d 6574 686f 642e 2054 6869 7320  ut method. This 
-00031070: 6973 0a20 2020 2020 2020 2020 2020 2023  is.            #
-00031080: 2020 2020 206f 7074 696f 6e61 6c20 6669       optional fi
-00031090: 656c 640a 0a20 2020 2020 2020 2052 6574  eld..        Ret
-000310a0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-000310b0: 2020 5265 7370 6f6e 7365 3a20 4365 6e74    Response: Cent
-000310c0: 7261 6c41 5049 2052 6573 706f 6e73 6520  ralAPI Response 
-000310d0: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
-000310e0: 2222 0a20 2020 2020 2020 2075 726c 203d  "".        url =
-000310f0: 2066 222f 6775 6573 742f 7631 2f70 6f72   f"/guest/v1/por
-00031100: 7461 6c73 2f7b 706f 7274 616c 5f69 647d  tals/{portal_id}
-00031110: 2f76 6973 6974 6f72 7322 0a0a 2020 2020  /visitors"..    
-00031120: 2020 2020 7573 6572 5f64 6174 6120 3d20      user_data = 
-00031130: 7b0a 2020 2020 2020 2020 2020 2020 2770  {.            'p
-00031140: 686f 6e65 273a 2070 686f 6e65 2c0a 2020  hone': phone,.  
-00031150: 2020 2020 2020 2020 2020 2765 6d61 696c            'email
-00031160: 273a 2065 6d61 696c 0a20 2020 2020 2020  ': email.       
-00031170: 207d 0a20 2020 2020 2020 2023 2041 5049   }.        # API
-00031180: 2072 6571 7569 7265 7320 7068 6f6e 6520   requires phone 
-00031190: 616e 6420 656d 6169 6c2c 2062 7574 2061  and email, but a
-000311a0: 6c6c 6f77 7320 4e6f 6e65 2f6e 756c 6c20  llows None/null 
-000311b0: 6173 2076 616c 7565 2064 6570 656e 6469  as value dependi
-000311c0: 6e67 206f 6e20 686f 7720 706f 7274 616c  ng on how portal
-000311d0: 2069 7320 636f 6e66 6967 7572 6564 0a20   is configured. 
-000311e0: 2020 2020 2020 2023 2075 7365 725f 6461         # user_da
-000311f0: 7461 203d 2075 7469 6c73 2e73 7472 6970  ta = utils.strip
-00031200: 5f6e 6f6e 6528 7573 6572 5f64 6174 6129  _none(user_data)
-00031210: 0a0a 2020 2020 2020 2020 6a73 6f6e 5f64  ..        json_d
-00031220: 6174 6120 3d20 7b0a 2020 2020 2020 2020  ata = {.        
-00031230: 2020 2020 276e 616d 6527 3a20 6e61 6d65      'name': name
-00031240: 2c0a 2020 2020 2020 2020 2020 2020 2763  ,.            'c
-00031250: 6f6d 7061 6e79 5f6e 616d 6527 3a20 636f  ompany_name': co
-00031260: 6d70 616e 795f 6e61 6d65 2c0a 2020 2020  mpany_name,.    
-00031270: 2020 2020 2020 2020 2769 735f 656e 6162          'is_enab
-00031280: 6c65 6427 3a20 6973 5f65 6e61 626c 6564  led': is_enabled
-00031290: 2c0a 2020 2020 2020 2020 2020 2020 2776  ,.            'v
-000312a0: 616c 6964 5f74 696c 6c5f 6e6f 5f6c 696d  alid_till_no_lim
-000312b0: 6974 273a 2076 616c 6964 5f66 6f72 6576  it': valid_forev
-000312c0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-000312d0: 2776 616c 6964 5f74 696c 6c5f 6461 7973  'valid_till_days
-000312e0: 273a 2076 616c 6964 5f64 6179 732c 0a20  ': valid_days,. 
-000312f0: 2020 2020 2020 2020 2020 2027 7661 6c69             'vali
-00031300: 645f 7469 6c6c 5f68 6f75 7273 273a 2076  d_till_hours': v
-00031310: 616c 6964 5f68 6f75 7273 2c0a 2020 2020  alid_hours,.    
-00031320: 2020 2020 2020 2020 2776 616c 6964 5f74          'valid_t
-00031330: 696c 6c5f 6d69 6e75 7465 7327 3a20 7661  ill_minutes': va
-00031340: 6c69 645f 6d69 6e75 7465 732c 0a20 2020  lid_minutes,.   
-00031350: 2020 2020 2020 2020 2027 6e6f 7469 6679           'notify
-00031360: 273a 206e 6f74 6966 792c 0a20 2020 2020  ': notify,.     
-00031370: 2020 2020 2020 2027 6e6f 7469 6679 5f74         'notify_t
-00031380: 6f27 3a20 6e6f 7469 6679 5f74 6f2c 0a20  o': notify_to,. 
-00031390: 2020 2020 2020 2020 2020 2027 7061 7373             'pass
-000313a0: 776f 7264 273a 2070 6173 7377 6f72 640a  word': password.
-000313b0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000313c0: 2020 6a73 6f6e 5f64 6174 6120 3d20 7574    json_data = ut
-000313d0: 696c 732e 7374 7269 705f 6e6f 6e65 286a  ils.strip_none(j
-000313e0: 736f 6e5f 6461 7461 290a 2020 2020 2020  son_data).      
-000313f0: 2020 6966 2075 7365 725f 6461 7461 3a0a    if user_data:.
-00031400: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
-00031410: 5f64 6174 615b 2275 7365 7222 5d20 3d20  _data["user"] = 
-00031420: 7573 6572 5f64 6174 610a 0a20 2020 2020  user_data..     
-00031430: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00031440: 7365 6c66 2e70 6f73 7428 7572 6c2c 206a  self.post(url, j
-00031450: 736f 6e5f 6461 7461 3d6a 736f 6e5f 6461  son_data=json_da
-00031460: 7461 290a 0a20 2020 2023 2054 4f44 4f20  ta)..    # TODO 
-00031470: 7661 6c69 6461 7465 2049 5020 6164 6472  validate IP addr
-00031480: 6573 7320 666f 726d 6174 0a20 2020 2061  ess format.    a
-00031490: 7379 6e63 2064 6566 2075 7064 6174 655f  sync def update_
-000314a0: 6378 5f70 726f 7065 7274 6965 7328 0a20  cx_properties(. 
-000314b0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000314c0: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-000314d0: 7365 7269 616c 3a20 7374 7220 3d20 4e6f  serial: str = No
-000314e0: 6e65 2c0a 2020 2020 2020 2020 6772 6f75  ne,.        grou
-000314f0: 703a 2073 7472 203d 204e 6f6e 652c 0a20  p: str = None,. 
-00031500: 2020 2020 2020 206e 616d 653a 2073 7472         name: str
-00031510: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00031520: 2063 6f6e 7461 6374 3a20 7374 7220 3d20   contact: str = 
-00031530: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c6f  None,.        lo
-00031540: 6361 7469 6f6e 3a20 7374 7220 3d20 4e6f  cation: str = No
-00031550: 6e65 2c0a 2020 2020 2020 2020 7469 6d65  ne,.        time
-00031560: 7a6f 6e65 3a20 636f 6e73 7461 6e74 732e  zone: constants.
-00031570: 545a 4442 203d 204e 6f6e 652c 0a20 2020  TZDB = None,.   
-00031580: 2020 2020 206d 676d 745f 7672 663a 2062       mgmt_vrf: b
-00031590: 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020 2020  ool = None,.    
-000315a0: 2020 2020 646e 735f 7365 7276 6572 733a      dns_servers:
-000315b0: 204c 6973 745b 7374 725d 203d 205b 5d2c   List[str] = [],
-000315c0: 0a20 2020 2020 2020 206e 7470 5f73 6572  .        ntp_ser
-000315d0: 7665 7273 3a20 4c69 7374 5b73 7472 5d20  vers: List[str] 
-000315e0: 3d20 5b5d 2c0a 2020 2020 2020 2020 6164  = [],.        ad
-000315f0: 6d69 6e5f 7573 6572 3a20 7374 7220 3d20  min_user: str = 
-00031600: 4e6f 6e65 2c0a 2020 2020 2020 2020 6164  None,.        ad
-00031610: 6d69 6e5f 7061 7373 3a20 7374 7220 3d20  min_pass: str = 
-00031620: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 2052  None,.    ) -> R
-00031630: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
-00031640: 2022 2222 5570 6461 7465 2050 726f 7065   """Update Prope
-00031650: 7274 6965 7320 2841 7275 6261 4f53 2d43  rties (ArubaOS-C
-00031660: 5829 2e0a 0a20 2020 2020 2020 2041 7267  X)...        Arg
-00031670: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00031680: 6572 6961 6c20 2873 7472 2c20 6f70 7469  erial (str, opti
-00031690: 6f6e 616c 293a 2044 6576 6963 6520 7365  onal): Device se
-000316a0: 7269 616c 206e 756d 6265 722e 0a20 2020  rial number..   
-000316b0: 2020 2020 2020 2020 2020 2020 204d 616e               Man
-000316c0: 6461 746f 7279 2066 6f72 2064 6576 6963  datory for devic
-000316d0: 6520 6c65 7665 6c20 636f 6e66 6967 7572  e level configur
-000316e0: 6174 696f 6e2e 0a20 2020 2020 2020 2020  ation..         
-000316f0: 2020 2020 2020 2031 2061 6e64 206f 6e6c         1 and onl
-00031700: 7920 3120 6f66 2073 6572 6961 6c20 6f72  y 1 of serial or
-00031710: 2067 726f 7570 2061 7265 2072 6571 7569   group are requi
-00031720: 7265 640a 2020 2020 2020 2020 2020 2020  red.            
-00031730: 6772 6f75 7020 2873 7472 2c20 6f70 7469  group (str, opti
-00031740: 6f6e 616c 293a 2047 726f 7570 206e 616d  onal): Group nam
-00031750: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
-00031760: 2020 204d 616e 6461 746f 7279 2066 6f72     Mandatory for
-00031770: 2067 726f 7570 206c 6576 656c 2063 6f6e   group level con
-00031780: 6669 6775 7261 7469 6f6e 2e0a 2020 2020  figuration..    
-00031790: 2020 2020 2020 2020 2020 2020 3120 616e              1 an
-000317a0: 6420 6f6e 6c79 2031 206f 6620 7365 7269  d only 1 of seri
-000317b0: 616c 206f 7220 6772 6f75 7020 6172 6520  al or group are 
-000317c0: 7265 7175 6972 6564 0a20 2020 2020 2020  required.       
-000317d0: 2020 2020 206e 616d 6520 2873 7472 293a       name (str):
-000317e0: 204f 6e6c 7920 636f 6e66 6967 7572 6162   Only configurab
-000317f0: 6c65 2061 7420 6465 7669 6365 2d6c 6576  le at device-lev
-00031800: 656c 2e0a 2020 2020 2020 2020 2020 2020  el..            
-00031810: 636f 6e74 6163 7420 2873 7472 293a 2050  contact (str): P
-00031820: 6174 7465 726e 3a20 225e 5b5e 223f 5d2a  attern: "^[^"?]*
-00031830: 2422 0a20 2020 2020 2020 2020 2020 206c  $".            l
-00031840: 6f63 6174 696f 6e20 2873 7472 293a 2050  ocation (str): P
-00031850: 6174 7465 726e 3a20 225e 5b5e 223f 5d2a  attern: "^[^"?]*
-00031860: 2422 0a20 2020 2020 2020 2020 2020 2074  $".            t
-00031870: 696d 657a 6f6e 6520 2873 7472 293a 2074  imezone (str): t
-00031880: 696d 657a 6f6e 6520 2056 616c 6964 2056  imezone  Valid V
-00031890: 616c 7565 733a 2075 7365 2074 7a20 6461  alues: use tz da
-000318a0: 7461 6261 7365 2066 6f72 6d61 7420 6c69  tabase format li
-000318b0: 6b65 2022 416d 6572 6963 612f 4368 6963  ke "America/Chic
-000318c0: 6167 6f22 0a20 2020 2020 2020 2020 2020  ago".           
-000318d0: 206d 676d 745f 7672 6620 2862 6f6f 6c29   mgmt_vrf (bool)
-000318e0: 3a20 5573 6520 6d67 6d74 2056 5246 2c20  : Use mgmt VRF, 
-000318f0: 696e 6469 6361 7465 7320 5652 4620 666f  indicates VRF fo
-00031900: 7220 646e 735f 7365 7276 6572 7320 616e  r dns_servers an
-00031910: 6420 6e74 705f 7365 7276 6572 732c 2069  d ntp_servers, i
-00031920: 6620 4661 6c73 6520 6f72 206e 6f74 2070  f False or not p
-00031930: 726f 7669 6465 6420 6465 6661 756c 7420  rovided default 
-00031940: 5652 4620 6973 2075 7365 642e 0a20 2020  VRF is used..   
-00031950: 2020 2020 2020 2020 2064 6e73 5f73 6572           dns_ser
-00031960: 7665 7273 2028 4c69 7374 5b73 7472 5d29  vers (List[str])
-00031970: 3a20 6970 7634 2f69 7076 3620 6164 6472  : ipv4/ipv6 addr
-00031980: 6573 730a 2020 2020 2020 2020 2020 2020  ess.            
-00031990: 6e74 705f 7365 7276 6572 7320 284c 6973  ntp_servers (Lis
-000319a0: 745b 7374 725d 293a 2069 7076 342f 6970  t[str]): ipv4/ip
-000319b0: 7636 2061 6464 7265 7373 0a20 2020 2020  v6 address.     
-000319c0: 2020 2020 2020 2061 646d 696e 5f75 7365         admin_use
-000319d0: 7220 2873 7472 293a 206c 6f63 616c 2061  r (str): local a
-000319e0: 646d 696e 2075 7365 720a 2020 2020 2020  dmin user.      
-000319f0: 2020 2020 2020 6164 6d69 6e5f 7061 7373        admin_pass
-00031a00: 2028 7374 7229 3a20 6c6f 6361 6c20 6164   (str): local ad
-00031a10: 6d69 6e20 7061 7373 776f 7264 0a0a 2020  min password..  
-00031a20: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00031a30: 2020 2020 2020 2020 2020 2052 6573 706f             Respo
-00031a40: 6e73 653a 2043 656e 7472 616c 4150 4920  nse: CentralAPI 
-00031a50: 5265 7370 6f6e 7365 206f 626a 6563 740a  Response object.
-00031a60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00031a70: 2020 2020 7572 6c20 3d20 222f 636f 6e66      url = "/conf
-00031a80: 6967 7572 6174 696f 6e2f 7631 2f73 7769  iguration/v1/swi
-00031a90: 7463 682f 6378 2f70 726f 7065 7274 6965  tch/cx/propertie
-00031aa0: 7322 0a0a 2020 2020 2020 2020 7061 7261  s"..        para
-00031ab0: 6d73 203d 207b 0a20 2020 2020 2020 2020  ms = {.         
-00031ac0: 2020 2027 6465 7669 6365 5f73 6572 6961     'device_seria
-00031ad0: 6c27 3a20 7365 7269 616c 2c0a 2020 2020  l': serial,.    
-00031ae0: 2020 2020 2020 2020 2767 726f 7570 5f6e          'group_n
-00031af0: 616d 6527 3a20 6772 6f75 700a 2020 2020  ame': group.    
-00031b00: 2020 2020 7d0a 0a20 2020 2020 2020 206a      }..        j
-00031b10: 736f 6e5f 6461 7461 203d 207b 0a20 2020  son_data = {.   
-00031b20: 2020 2020 2020 2020 2027 6e61 6d65 273a           'name':
-00031b30: 206e 616d 652c 0a20 2020 2020 2020 2020   name,.         
-00031b40: 2020 2027 636f 6e74 6163 7427 3a20 636f     'contact': co
-00031b50: 6e74 6163 742c 0a20 2020 2020 2020 2020  ntact,.         
-00031b60: 2020 2027 6c6f 6361 7469 6f6e 273a 206c     'location': l
-00031b70: 6f63 6174 696f 6e2c 0a20 2020 2020 2020  ocation,.       
-00031b80: 2020 2020 2027 7469 6d65 7a6f 6e65 273a       'timezone':
-00031b90: 2074 696d 657a 6f6e 652c 0a20 2020 2020   timezone,.     
-00031ba0: 2020 2020 2020 2027 646e 735f 7365 7276         'dns_serv
-00031bb0: 6572 7327 3a20 646e 735f 7365 7276 6572  ers': dns_server
-00031bc0: 732c 0a20 2020 2020 2020 2020 2020 2027  s,.            '
-00031bd0: 6e74 705f 7365 7276 6572 7327 3a20 6e74  ntp_servers': nt
-00031be0: 705f 7365 7276 6572 732c 0a20 2020 2020  p_servers,.     
-00031bf0: 2020 2020 2020 2027 6164 6d69 6e5f 7573         'admin_us
-00031c00: 6572 6e61 6d65 273a 2061 646d 696e 5f75  ername': admin_u
-00031c10: 7365 722c 0a20 2020 2020 2020 2020 2020  ser,.           
-00031c20: 2027 6164 6d69 6e5f 7061 7373 776f 7264   'admin_password
-00031c30: 273a 2061 646d 696e 5f70 6173 730a 2020  ': admin_pass.  
-00031c40: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00031c50: 6966 206d 676d 745f 7672 6620 6973 206e  if mgmt_vrf is n
-00031c60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00031c70: 2020 2020 206a 736f 6e5f 6461 7461 5b22       json_data["
-00031c80: 7672 6622 5d20 3d20 226d 676d 7422 2069  vrf"] = "mgmt" i
-00031c90: 6620 6d67 6d74 5f76 7266 2065 6c73 6520  f mgmt_vrf else 
-00031ca0: 2264 6566 6175 6c74 220a 2020 2020 2020  "default".      
-00031cb0: 2020 656c 6966 2064 6e73 5f73 6572 7665    elif dns_serve
-00031cc0: 7273 206f 7220 6e74 705f 7365 7276 6572  rs or ntp_server
-00031cd0: 733a 0a20 2020 2020 2020 2020 2020 206a  s:.            j
-00031ce0: 736f 6e5f 6461 7461 5b22 7672 6622 5d20  son_data["vrf"] 
-00031cf0: 3d20 2264 6566 6175 6c74 220a 0a20 2020  = "default"..   
-00031d00: 2020 2020 2069 6620 6c65 6e28 5b78 2066       if len([x f
-00031d10: 6f72 2078 2069 6e20 5b61 646d 696e 5f75  or x in [admin_u
-00031d20: 7365 722c 2061 646d 696e 5f70 6173 735d  ser, admin_pass]
-00031d30: 2069 6620 7820 6973 206e 6f74 204e 6f6e   if x is not Non
-00031d40: 655d 2920 3d3d 2031 3a0a 2020 2020 2020  e]) == 1:.      
-00031d50: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00031d60: 6545 7272 6f72 2822 4966 2065 6974 6865  eError("If eithe
-00031d70: 7220 6164 6d69 6e5f 7573 6572 206f 7220  r admin_user or 
-00031d80: 6164 6d69 6e5f 7061 7373 2061 7265 2062  admin_pass are b
-00031d90: 696e 6720 7570 6461 7465 642c 202a 626f  ing updated, *bo
-00031da0: 7468 2a20 7368 6f75 6c64 2062 6520 7072  th* should be pr
-00031db0: 6f76 6964 6564 2e22 290a 0a20 2020 2020  ovided.")..     
-00031dc0: 2020 2069 6620 6c65 6e28 5b78 2066 6f72     if len([x for
-00031dd0: 2078 2069 6e20 5b73 6572 6961 6c2c 2067   x in [serial, g
-00031de0: 726f 7570 5d20 6966 2078 2069 7320 6e6f  roup] if x is no
-00031df0: 7420 4e6f 6e65 5d29 203d 3d20 323a 0a20  t None]) == 2:. 
-00031e00: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00031e10: 2056 616c 7565 4572 726f 7228 2270 726f   ValueError("pro
-00031e20: 7669 6465 2073 6572 6961 6c20 746f 2075  vide serial to u
-00031e30: 7064 6174 6520 6465 7669 6365 206c 6576  pdate device lev
-00031e40: 656c 2070 726f 7065 7274 6965 732c 206f  el properties, o
-00031e50: 7220 6772 6f75 7020 746f 2075 7064 6174  r group to updat
-00031e60: 6520 6174 2074 6865 2067 726f 7570 206c  e at the group l
-00031e70: 6576 656c 2e20 2050 726f 7669 6469 6e67  evel.  Providing
-00031e80: 2062 6f74 6820 6973 2069 6e76 616c 6964   both is invalid
-00031e90: 2e22 290a 0a20 2020 2020 2020 206a 736f  .")..        jso
-00031ea0: 6e5f 6461 7461 203d 2075 7469 6c73 2e73  n_data = utils.s
-00031eb0: 7472 6970 5f6e 6f6e 6528 6a73 6f6e 5f64  trip_none(json_d
-00031ec0: 6174 612c 2073 7472 6970 5f65 6d70 7479  ata, strip_empty
-00031ed0: 5f6f 626a 3d54 7275 6529 0a0a 2020 2020  _obj=True)..    
-00031ee0: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-00031ef0: 2073 656c 662e 706f 7374 2875 726c 2c20   self.post(url, 
-00031f00: 6a73 6f6e 5f64 6174 613d 6a73 6f6e 5f64  json_data=json_d
-00031f10: 6174 612c 2070 6172 616d 733d 7061 7261  ata, params=para
-00031f20: 6d73 290a 0a20 2020 2061 7379 6e63 2064  ms)..    async d
-00031f30: 6566 2067 6574 5f6f 7370 665f 6172 6561  ef get_ospf_area
-00031f40: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00031f50: 2020 2020 2020 2020 6465 7669 6365 3a20          device: 
-00031f60: 7374 722c 0a20 2020 2020 2020 206d 6172  str,.        mar
-00031f70: 6b65 723a 2073 7472 203d 204e 6f6e 652c  ker: str = None,
-00031f80: 0a20 2020 2020 2020 206c 696d 6974 3a20  .        limit: 
-00031f90: 696e 7420 3d20 3130 302c 0a20 2020 2029  int = 100,.    )
-00031fa0: 202d 3e20 5265 7370 6f6e 7365 3a0a 2020   -> Response:.  
-00031fb0: 2020 2020 2020 2222 224c 6973 7420 4f53        """List OS
-00031fc0: 5046 2041 7265 6120 496e 666f 726d 6174  PF Area Informat
-00031fd0: 696f 6e2e 0a0a 2020 2020 2020 2020 4172  ion...        Ar
-00031fe0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00031ff0: 6465 7669 6365 2028 7374 7229 3a20 4465  device (str): De
-00032000: 7669 6365 2073 6572 6961 6c20 6e75 6d62  vice serial numb
-00032010: 6572 0a20 2020 2020 2020 2020 2020 206d  er.            m
-00032020: 6172 6b65 7220 2873 7472 2c20 6f70 7469  arker (str, opti
-00032030: 6f6e 616c 293a 204f 7061 7175 6520 6861  onal): Opaque ha
-00032040: 6e64 6c65 2074 6f20 6665 7463 6820 6e65  ndle to fetch ne
-00032050: 7874 2070 6167 650a 2020 2020 2020 2020  xt page.        
-00032060: 2020 2020 6c69 6d69 7420 2869 6e74 2c20      limit (int, 
-00032070: 6f70 7469 6f6e 616c 293a 2070 6167 6520  optional): page 
-00032080: 7369 7a65 2044 6566 6175 6c74 7320 746f  size Defaults to
-00032090: 2031 3030 2e0a 0a20 2020 2020 2020 2052   100...        R
-000320a0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-000320b0: 2020 2020 5265 7370 6f6e 7365 3a20 4365      Response: Ce
-000320c0: 6e74 7261 6c41 5049 2052 6573 706f 6e73  ntralAPI Respons
-000320d0: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
-000320e0: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
-000320f0: 203d 2022 2f61 7069 2f72 6f75 7469 6e67   = "/api/routing
-00032100: 2f76 312f 6f73 7066 2f61 7265 6122 0a0a  /v1/ospf/area"..
-00032110: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
-00032120: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-00032130: 6465 7669 6365 273a 2064 6576 6963 652c  device': device,
-00032140: 0a20 2020 2020 2020 2020 2020 2027 6d61  .            'ma
-00032150: 726b 6572 273a 206d 6172 6b65 722c 0a20  rker': marker,. 
-00032160: 2020 2020 2020 2020 2020 2027 6c69 6d69             'limi
-00032170: 7427 3a20 6c69 6d69 740a 2020 2020 2020  t': limit.      
-00032180: 2020 7d0a 0a20 2020 2020 2020 2072 6574    }..        ret
-00032190: 7572 6e20 6177 6169 7420 7365 6c66 2e67  urn await self.g
-000321a0: 6574 2875 726c 2c20 7061 7261 6d73 3d70  et(url, params=p
-000321b0: 6172 616d 7329 0a0a 2020 2020 6173 796e  arams)..    asyn
-000321c0: 6320 6465 6620 6765 745f 6f73 7066 5f69  c def get_ospf_i
-000321d0: 6e74 6572 6661 6365 280a 2020 2020 2020  nterface(.      
-000321e0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000321f0: 6465 7669 6365 3a20 7374 722c 0a20 2020  device: str,.   
-00032200: 2020 2020 206d 6172 6b65 723a 2073 7472       marker: str
-00032210: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00032220: 206c 696d 6974 3a20 696e 7420 3d20 3130   limit: int = 10
-00032230: 302c 0a20 2020 2029 202d 3e20 5265 7370  0,.    ) -> Resp
-00032240: 6f6e 7365 3a0a 2020 2020 2020 2020 2222  onse:.        ""
-00032250: 224c 6973 7420 4f53 5046 2049 6e74 6572  "List OSPF Inter
-00032260: 6661 6365 2049 6e66 6f72 6d61 7469 6f6e  face Information
-00032270: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00032280: 0a20 2020 2020 2020 2020 2020 2064 6576  .            dev
-00032290: 6963 6520 2873 7472 293a 2044 6576 6963  ice (str): Devic
-000322a0: 6520 7365 7269 616c 206e 756d 6265 720a  e serial number.
-000322b0: 2020 2020 2020 2020 2020 2020 6d61 726b              mark
-000322c0: 6572 2028 7374 722c 206f 7074 696f 6e61  er (str, optiona
-000322d0: 6c29 3a20 4f70 6171 7565 2068 616e 646c  l): Opaque handl
-000322e0: 6520 746f 2066 6574 6368 206e 6578 7420  e to fetch next 
-000322f0: 7061 6765 0a20 2020 2020 2020 2020 2020  page.           
-00032300: 206c 696d 6974 2028 696e 742c 206f 7074   limit (int, opt
-00032310: 696f 6e61 6c29 3a20 7061 6765 2073 697a  ional): page siz
-00032320: 6520 4465 6661 756c 7473 2074 6f20 3130  e Defaults to 10
-00032330: 302e 0a0a 2020 2020 2020 2020 5265 7475  0...        Retu
-00032340: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00032350: 2052 6573 706f 6e73 653a 2043 656e 7472   Response: Centr
-00032360: 616c 4150 4920 5265 7370 6f6e 7365 206f  alAPI Response o
-00032370: 626a 6563 740a 2020 2020 2020 2020 2222  bject.        ""
-00032380: 220a 2020 2020 2020 2020 7572 6c20 3d20  ".        url = 
-00032390: 222f 6170 692f 726f 7574 696e 672f 7631  "/api/routing/v1
-000323a0: 2f6f 7370 662f 696e 7465 7266 6163 6522  /ospf/interface"
-000323b0: 0a0a 2020 2020 2020 2020 7061 7261 6d73  ..        params
-000323c0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-000323d0: 2027 6465 7669 6365 273a 2064 6576 6963   'device': devic
-000323e0: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
-000323f0: 6d61 726b 6572 273a 206d 6172 6b65 722c  marker': marker,
-00032400: 0a20 2020 2020 2020 2020 2020 2027 6c69  .            'li
-00032410: 6d69 7427 3a20 6c69 6d69 740a 2020 2020  mit': limit.    
-00032420: 2020 2020 7d0a 0a20 2020 2020 2020 2072      }..        r
-00032430: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-00032440: 2e67 6574 2875 726c 2c20 7061 7261 6d73  .get(url, params
-00032450: 3d70 6172 616d 7329 0a0a 2020 2020 6173  =params)..    as
-00032460: 796e 6320 6465 6620 6765 745f 6f73 7066  ync def get_ospf
-00032470: 5f6e 6569 6768 626f 7228 0a20 2020 2020  _neighbor(.     
-00032480: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00032490: 2064 6576 6963 653a 2073 7472 2c0a 2020   device: str,.  
-000324a0: 2020 2020 2020 6d61 726b 6572 3a20 7374        marker: st
-000324b0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-000324c0: 2020 6c69 6d69 743a 2069 6e74 203d 2031    limit: int = 1
-000324d0: 3030 2c0a 2020 2020 2920 2d3e 2052 6573  00,.    ) -> Res
-000324e0: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
-000324f0: 2222 4c69 7374 204f 5350 4620 6e65 6967  ""List OSPF neig
-00032500: 6862 6f72 2049 6e66 6f72 6d61 7469 6f6e  hbor Information
-00032510: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00032520: 0a20 2020 2020 2020 2020 2020 2064 6576  .            dev
-00032530: 6963 6520 2873 7472 293a 2044 6576 6963  ice (str): Devic
-00032540: 6520 7365 7269 616c 206e 756d 6265 720a  e serial number.
-00032550: 2020 2020 2020 2020 2020 2020 6d61 726b              mark
-00032560: 6572 2028 7374 722c 206f 7074 696f 6e61  er (str, optiona
-00032570: 6c29 3a20 4f70 6171 7565 2068 616e 646c  l): Opaque handl
-00032580: 6520 746f 2066 6574 6368 206e 6578 7420  e to fetch next 
-00032590: 7061 6765 0a20 2020 2020 2020 2020 2020  page.           
-000325a0: 206c 696d 6974 2028 696e 742c 206f 7074   limit (int, opt
-000325b0: 696f 6e61 6c29 3a20 7061 6765 2073 697a  ional): page siz
-000325c0: 6520 4465 6661 756c 7473 2074 6f20 3130  e Defaults to 10
-000325d0: 302e 0a0a 2020 2020 2020 2020 5265 7475  0...        Retu
-000325e0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-000325f0: 2052 6573 706f 6e73 653a 2043 656e 7472   Response: Centr
-00032600: 616c 4150 4920 5265 7370 6f6e 7365 206f  alAPI Response o
-00032610: 626a 6563 740a 2020 2020 2020 2020 2222  bject.        ""
-00032620: 220a 2020 2020 2020 2020 7572 6c20 3d20  ".        url = 
-00032630: 222f 6170 692f 726f 7574 696e 672f 7631  "/api/routing/v1
-00032640: 2f6f 7370 662f 6e65 6967 6862 6f72 220a  /ospf/neighbor".
-00032650: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-00032660: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00032670: 2764 6576 6963 6527 3a20 6465 7669 6365  'device': device
-00032680: 2c0a 2020 2020 2020 2020 2020 2020 276d  ,.            'm
-00032690: 6172 6b65 7227 3a20 6d61 726b 6572 2c0a  arker': marker,.
-000326a0: 2020 2020 2020 2020 2020 2020 276c 696d              'lim
-000326b0: 6974 273a 206c 696d 6974 0a20 2020 2020  it': limit.     
-000326c0: 2020 207d 0a0a 2020 2020 2020 2020 7265     }..        re
-000326d0: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
-000326e0: 6765 7428 7572 6c2c 2070 6172 616d 733d  get(url, params=
-000326f0: 7061 7261 6d73 290a 0a20 2020 2061 7379  params)..    asy
-00032700: 6e63 2064 6566 2067 6574 5f6f 7370 665f  nc def get_ospf_
-00032710: 6461 7461 6261 7365 280a 2020 2020 2020  database(.      
-00032720: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00032730: 6465 7669 6365 3a20 7374 722c 0a20 2020  device: str,.   
-00032740: 2020 2020 206d 6172 6b65 723a 2073 7472       marker: str
-00032750: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00032760: 206c 696d 6974 3a20 696e 7420 3d20 3130   limit: int = 10
-00032770: 302c 0a20 2020 2029 202d 3e20 5265 7370  0,.    ) -> Resp
-00032780: 6f6e 7365 3a0a 2020 2020 2020 2020 2222  onse:.        ""
-00032790: 224c 6973 7420 4f53 5046 204c 696e 6b20  "List OSPF Link 
-000327a0: 5374 6174 6520 4461 7461 6261 7365 2049  State Database I
-000327b0: 6e66 6f72 6d61 7469 6f6e 2e0a 0a20 2020  nformation...   
-000327c0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-000327d0: 2020 2020 2020 2064 6576 6963 6520 2873         device (s
-000327e0: 7472 293a 2044 6576 6963 6520 7365 7269  tr): Device seri
-000327f0: 616c 206e 756d 6265 720a 2020 2020 2020  al number.      
-00032800: 2020 2020 2020 6d61 726b 6572 2028 7374        marker (st
-00032810: 722c 206f 7074 696f 6e61 6c29 3a20 4f70  r, optional): Op
-00032820: 6171 7565 2068 616e 646c 6520 746f 2066  aque handle to f
-00032830: 6574 6368 206e 6578 7420 7061 6765 0a20  etch next page. 
-00032840: 2020 2020 2020 2020 2020 206c 696d 6974             limit
-00032850: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
-00032860: 3a20 7061 6765 2073 697a 6520 4465 6661  : page size Defa
-00032870: 756c 7473 2074 6f20 3130 302e 0a0a 2020  ults to 100...  
-00032880: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00032890: 2020 2020 2020 2020 2020 2052 6573 706f             Respo
-000328a0: 6e73 653a 2043 656e 7472 616c 4150 4920  nse: CentralAPI 
-000328b0: 5265 7370 6f6e 7365 206f 626a 6563 740a  Response object.
-000328c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000328d0: 2020 2020 7572 6c20 3d20 222f 6170 692f      url = "/api/
-000328e0: 726f 7574 696e 672f 7631 2f6f 7370 662f  routing/v1/ospf/
-000328f0: 6461 7461 6261 7365 220a 0a20 2020 2020  database"..     
-00032900: 2020 2070 6172 616d 7320 3d20 7b0a 2020     params = {.  
-00032910: 2020 2020 2020 2020 2020 2764 6576 6963            'devic
-00032920: 6527 3a20 6465 7669 6365 2c0a 2020 2020  e': device,.    
-00032930: 2020 2020 2020 2020 276d 6172 6b65 7227          'marker'
-00032940: 3a20 6d61 726b 6572 2c0a 2020 2020 2020  : marker,.      
-00032950: 2020 2020 2020 276c 696d 6974 273a 206c        'limit': l
-00032960: 696d 6974 0a20 2020 2020 2020 207d 0a0a  imit.        }..
-00032970: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00032980: 7761 6974 2073 656c 662e 6765 7428 7572  wait self.get(ur
-00032990: 6c2c 2070 6172 616d 733d 7061 7261 6d73  l, params=params
-000329a0: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-000329b0: 2067 6574 5f6f 7665 726c 6179 5f63 6f6e   get_overlay_con
-000329c0: 6e65 6374 696f 6e28 0a20 2020 2020 2020  nection(.       
-000329d0: 2073 656c 662c 0a20 2020 2020 2020 2064   self,.        d
-000329e0: 6576 6963 653a 2073 7472 2c0a 2020 2020  evice: str,.    
-000329f0: 2020 2020 6d61 726b 6572 3a20 7374 7220      marker: str 
-00032a00: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00032a10: 6c69 6d69 743a 2069 6e74 203d 2031 3030  limit: int = 100
-00032a20: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
-00032a30: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
-00032a40: 4765 7420 696e 666f 726d 6174 696f 6e20  Get information 
-00032a50: 6162 6f75 7420 6f76 6572 6c61 7920 636f  about overlay co
-00032a60: 6e74 726f 6c20 636f 6e6e 6563 7469 6f6e  ntrol connection
-00032a70: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00032a80: 0a20 2020 2020 2020 2020 2020 2064 6576  .            dev
-00032a90: 6963 6520 2873 7472 293a 2044 6576 6963  ice (str): Devic
-00032aa0: 6520 7365 7269 616c 206e 756d 6265 720a  e serial number.
-00032ab0: 2020 2020 2020 2020 2020 2020 6d61 726b              mark
-00032ac0: 6572 2028 7374 722c 206f 7074 696f 6e61  er (str, optiona
-00032ad0: 6c29 3a20 4f70 6171 7565 2068 616e 646c  l): Opaque handl
-00032ae0: 6520 746f 2066 6574 6368 206e 6578 7420  e to fetch next 
-00032af0: 7061 6765 0a20 2020 2020 2020 2020 2020  page.           
-00032b00: 206c 696d 6974 2028 696e 742c 206f 7074   limit (int, opt
-00032b10: 696f 6e61 6c29 3a20 7061 6765 2073 697a  ional): page siz
-00032b20: 6520 4465 6661 756c 7473 2074 6f20 3130  e Defaults to 10
-00032b30: 302e 0a0a 2020 2020 2020 2020 5265 7475  0...        Retu
-00032b40: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00032b50: 2052 6573 706f 6e73 653a 2043 656e 7472   Response: Centr
-00032b60: 616c 4150 4920 5265 7370 6f6e 7365 206f  alAPI Response o
-00032b70: 626a 6563 740a 2020 2020 2020 2020 2222  bject.        ""
-00032b80: 220a 2020 2020 2020 2020 7572 6c20 3d20  ".        url = 
-00032b90: 222f 6170 692f 726f 7574 696e 672f 7631  "/api/routing/v1
-00032ba0: 2f6f 7665 726c 6179 2f63 6f6e 6e65 6374  /overlay/connect
-00032bb0: 696f 6e22 0a0a 2020 2020 2020 2020 7061  ion"..        pa
-00032bc0: 7261 6d73 203d 207b 0a20 2020 2020 2020  rams = {.       
-00032bd0: 2020 2020 2027 6465 7669 6365 273a 2064       'device': d
-00032be0: 6576 6963 652c 0a20 2020 2020 2020 2020  evice,.         
-00032bf0: 2020 2027 6d61 726b 6572 273a 206d 6172     'marker': mar
-00032c00: 6b65 722c 0a20 2020 2020 2020 2020 2020  ker,.           
-00032c10: 2027 6c69 6d69 7427 3a20 6c69 6d69 740a   'limit': limit.
-00032c20: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00032c30: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00032c40: 7365 6c66 2e67 6574 2875 726c 2c20 7061  self.get(url, pa
-00032c50: 7261 6d73 3d70 6172 616d 7329 0a0a 2020  rams=params)..  
-00032c60: 2020 6173 796e 6320 6465 6620 7265 7365    async def rese
-00032c70: 745f 6f76 6572 6c61 795f 636f 6e6e 6563  t_overlay_connec
-00032c80: 7469 6f6e 280a 2020 2020 2020 2020 7365  tion(.        se
-00032c90: 6c66 2c0a 2020 2020 2020 2020 6465 7669  lf,.        devi
-00032ca0: 6365 3a20 7374 722c 0a20 2020 2029 202d  ce: str,.    ) -
-00032cb0: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
-00032cc0: 2020 2020 2222 2252 6573 6574 206f 7665      """Reset ove
-00032cd0: 726c 6179 2063 6f6e 7472 6f6c 2063 6f6e  rlay control con
-00032ce0: 6e65 6374 696f 6e2e 0a0a 2020 2020 2020  nection...      
-00032cf0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00032d00: 2020 2020 6465 7669 6365 2028 7374 7229      device (str)
-00032d10: 3a20 4465 7669 6365 2073 6572 6961 6c20  : Device serial 
-00032d20: 6e75 6d62 6572 0a0a 2020 2020 2020 2020  number..        
-00032d30: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00032d40: 2020 2020 2052 6573 706f 6e73 653a 2043       Response: C
-00032d50: 656e 7472 616c 4150 4920 5265 7370 6f6e  entralAPI Respon
-00032d60: 7365 206f 626a 6563 740a 2020 2020 2020  se object.      
-00032d70: 2020 2222 220a 2020 2020 2020 2020 7572    """.        ur
-00032d80: 6c20 3d20 222f 6170 692f 726f 7574 696e  l = "/api/routin
-00032d90: 672f 7631 2f6f 7665 726c 6179 2f63 6f6e  g/v1/overlay/con
-00032da0: 6e65 6374 696f 6e2f 7265 7365 7422 0a0a  nection/reset"..
-00032db0: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
-00032dc0: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-00032dd0: 6465 7669 6365 273a 2064 6576 6963 650a  device': device.
-00032de0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00032df0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00032e00: 7365 6c66 2e70 7574 2875 726c 2c20 7061  self.put(url, pa
-00032e10: 7261 6d73 3d70 6172 616d 7329 0a0a 2020  rams=params)..  
-00032e20: 2020 6173 796e 6320 6465 6620 6765 745f    async def get_
-00032e30: 6f76 6572 6c61 795f 726f 7574 6573 5f6c  overlay_routes_l
-00032e40: 6561 726e 6564 280a 2020 2020 2020 2020  earned(.        
-00032e50: 7365 6c66 2c0a 2020 2020 2020 2020 6465  self,.        de
-00032e60: 7669 6365 3a20 7374 722c 0a20 2020 2020  vice: str,.     
-00032e70: 2020 202a 2c0a 2020 2020 2020 2020 6265     *,.        be
-00032e80: 7374 3a20 626f 6f6c 203d 2046 616c 7365  st: bool = False
-00032e90: 2c0a 2020 2020 2020 2020 6d61 726b 6572  ,.        marker
-00032ea0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00032eb0: 2020 2020 2020 6c69 6d69 743a 2069 6e74        limit: int
-00032ec0: 203d 2031 3030 2c0a 2020 2020 2920 2d3e   = 100,.    ) ->
-00032ed0: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
-00032ee0: 2020 2022 2222 4c69 7374 206f 6620 6c65     """List of le
-00032ef0: 6172 6e65 6420 726f 7574 6573 2066 726f  arned routes fro
-00032f00: 6d20 6f76 6572 6c61 792e 0a0a 2020 2020  m overlay...    
-00032f10: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00032f20: 2020 2020 2020 6465 7669 6365 2028 7374        device (st
-00032f30: 7229 3a20 4465 7669 6365 2073 6572 6961  r): Device seria
-00032f40: 6c20 6e75 6d62 6572 0a20 2020 2020 2020  l number.       
-00032f50: 2020 2020 2062 6573 7420 2862 6f6f 6c29       best (bool)
-00032f60: 3a20 5265 7475 726e 206f 6e6c 7920 6265  : Return only be
-00032f70: 7374 202f 2070 7265 6665 7272 6564 2072  st / preferred r
-00032f80: 6f75 7465 730a 2020 2020 2020 2020 2020  outes.          
-00032f90: 2020 6d61 726b 6572 2028 7374 722c 206f    marker (str, o
-00032fa0: 7074 696f 6e61 6c29 3a20 4f70 6171 7565  ptional): Opaque
-00032fb0: 2068 616e 646c 6520 746f 2066 6574 6368   handle to fetch
-00032fc0: 206e 6578 7420 7061 6765 0a20 2020 2020   next page.     
-00032fd0: 2020 2020 2020 206c 696d 6974 2028 696e         limit (in
-00032fe0: 742c 206f 7074 696f 6e61 6c29 3a20 7061  t, optional): pa
-00032ff0: 6765 2073 697a 6520 4465 6661 756c 7473  ge size Defaults
-00033000: 2074 6f20 3130 302e 0a0a 2020 2020 2020   to 100...      
-00033010: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00033020: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
-00033030: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
-00033040: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
-00033050: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00033060: 7572 6c20 3d20 222f 6170 692f 726f 7574  url = "/api/rout
-00033070: 696e 672f 7631 2f6f 7665 726c 6179 2f72  ing/v1/overlay/r
-00033080: 6f75 7465 2f6c 6561 726e 6564 220a 2020  oute/learned".  
-00033090: 2020 2020 2020 6966 2062 6573 743a 0a20        if best:. 
-000330a0: 2020 2020 2020 2020 2020 2075 726c 203d             url =
-000330b0: 2066 277b 7572 6c7d 2f62 6573 7427 0a0a   f'{url}/best'..
-000330c0: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
-000330d0: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-000330e0: 6465 7669 6365 273a 2064 6576 6963 652c  device': device,
-000330f0: 0a20 2020 2020 2020 2020 2020 2027 6d61  .            'ma
-00033100: 726b 6572 273a 206d 6172 6b65 722c 0a20  rker': marker,. 
-00033110: 2020 2020 2020 2020 2020 2027 6c69 6d69             'limi
-00033120: 7427 3a20 6c69 6d69 740a 2020 2020 2020  t': limit.      
-00033130: 2020 7d0a 0a20 2020 2020 2020 2072 6574    }..        ret
-00033140: 7572 6e20 6177 6169 7420 7365 6c66 2e67  urn await self.g
-00033150: 6574 2875 726c 2c20 7061 7261 6d73 3d70  et(url, params=p
-00033160: 6172 616d 7329 0a0a 2020 2020 6173 796e  arams)..    asyn
-00033170: 6320 6465 6620 6765 745f 6f76 6572 6c61  c def get_overla
-00033180: 795f 726f 7574 6573 5f61 6476 6572 7469  y_routes_adverti
-00033190: 7365 6428 0a20 2020 2020 2020 2073 656c  sed(.        sel
-000331a0: 662c 0a20 2020 2020 2020 2064 6576 6963  f,.        devic
-000331b0: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
-000331c0: 6d61 726b 6572 3a20 7374 7220 3d20 4e6f  marker: str = No
-000331d0: 6e65 2c0a 2020 2020 2020 2020 6c69 6d69  ne,.        limi
-000331e0: 743a 2069 6e74 203d 2031 3030 2c0a 2020  t: int = 100,.  
-000331f0: 2020 2920 2d3e 2052 6573 706f 6e73 653a    ) -> Response:
-00033200: 0a20 2020 2020 2020 2022 2222 4c69 7374  .        """List
-00033210: 206f 6620 6164 7665 7274 6973 6564 2072   of advertised r
-00033220: 6f75 7465 7320 746f 206f 7665 726c 6179  outes to overlay
-00033230: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00033240: 0a20 2020 2020 2020 2020 2020 2064 6576  .            dev
-00033250: 6963 6520 2873 7472 293a 2044 6576 6963  ice (str): Devic
-00033260: 6520 7365 7269 616c 206e 756d 6265 720a  e serial number.
-00033270: 2020 2020 2020 2020 2020 2020 6d61 726b              mark
-00033280: 6572 2028 7374 722c 206f 7074 696f 6e61  er (str, optiona
-00033290: 6c29 3a20 4f70 6171 7565 2068 616e 646c  l): Opaque handl
-000332a0: 6520 746f 2066 6574 6368 206e 6578 7420  e to fetch next 
-000332b0: 7061 6765 0a20 2020 2020 2020 2020 2020  page.           
-000332c0: 206c 696d 6974 2028 696e 742c 206f 7074   limit (int, opt
-000332d0: 696f 6e61 6c29 3a20 7061 6765 2073 697a  ional): page siz
-000332e0: 6520 4465 6661 756c 7473 2074 6f20 3130  e Defaults to 10
-000332f0: 302e 0a0a 2020 2020 2020 2020 5265 7475  0...        Retu
-00033300: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00033310: 2052 6573 706f 6e73 653a 2043 656e 7472   Response: Centr
-00033320: 616c 4150 4920 5265 7370 6f6e 7365 206f  alAPI Response o
-00033330: 626a 6563 740a 2020 2020 2020 2020 2222  bject.        ""
-00033340: 220a 2020 2020 2020 2020 7572 6c20 3d20  ".        url = 
-00033350: 222f 6170 692f 726f 7574 696e 672f 7631  "/api/routing/v1
-00033360: 2f6f 7665 726c 6179 2f72 6f75 7465 2f61  /overlay/route/a
-00033370: 6476 6572 7469 7365 6422 0a0a 2020 2020  dvertised"..    
-00033380: 2020 2020 7061 7261 6d73 203d 207b 0a20      params = {. 
-00033390: 2020 2020 2020 2020 2020 2027 6465 7669             'devi
-000333a0: 6365 273a 2064 6576 6963 652c 0a20 2020  ce': device,.   
-000333b0: 2020 2020 2020 2020 2027 6d61 726b 6572           'marker
-000333c0: 273a 206d 6172 6b65 722c 0a20 2020 2020  ': marker,.     
-000333d0: 2020 2020 2020 2027 6c69 6d69 7427 3a20         'limit': 
-000333e0: 6c69 6d69 740a 2020 2020 2020 2020 7d0a  limit.        }.
-000333f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00033400: 6177 6169 7420 7365 6c66 2e67 6574 2875  await self.get(u
-00033410: 726c 2c20 7061 7261 6d73 3d70 6172 616d  rl, params=param
-00033420: 7329 0a0a 2020 2020 6173 796e 6320 6465  s)..    async de
-00033430: 6620 6765 745f 6f76 6572 6c61 795f 696e  f get_overlay_in
-00033440: 7465 7266 6163 6573 280a 2020 2020 2020  terfaces(.      
-00033450: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00033460: 6465 7669 6365 3a20 7374 722c 0a20 2020  device: str,.   
-00033470: 2020 2020 206d 6172 6b65 723a 2073 7472       marker: str
-00033480: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00033490: 206c 696d 6974 3a20 696e 7420 3d20 3130   limit: int = 10
-000334a0: 302c 0a20 2020 2029 202d 3e20 5265 7370  0,.    ) -> Resp
-000334b0: 6f6e 7365 3a0a 2020 2020 2020 2020 2222  onse:.        ""
-000334c0: 224c 6973 7420 6f66 206f 7665 726c 6179  "List of overlay
-000334d0: 2069 6e74 6572 6661 6365 7320 2874 756e   interfaces (tun
-000334e0: 6e65 6c73 292e 0a0a 2020 2020 2020 2020  nels)...        
-000334f0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00033500: 2020 6465 7669 6365 2028 7374 7229 3a20    device (str): 
-00033510: 4465 7669 6365 2073 6572 6961 6c20 6e75  Device serial nu
-00033520: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
-00033530: 206d 6172 6b65 7220 2873 7472 2c20 6f70   marker (str, op
-00033540: 7469 6f6e 616c 293a 204f 7061 7175 6520  tional): Opaque 
-00033550: 6861 6e64 6c65 2074 6f20 6665 7463 6820  handle to fetch 
-00033560: 6e65 7874 2070 6167 650a 2020 2020 2020  next page.      
-00033570: 2020 2020 2020 6c69 6d69 7420 2869 6e74        limit (int
-00033580: 2c20 6f70 7469 6f6e 616c 293a 2070 6167  , optional): pag
-00033590: 6520 7369 7a65 2044 6566 6175 6c74 7320  e size Defaults 
-000335a0: 746f 2031 3030 2e0a 0a20 2020 2020 2020  to 100...       
-000335b0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-000335c0: 2020 2020 2020 5265 7370 6f6e 7365 3a20        Response: 
-000335d0: 4365 6e74 7261 6c41 5049 2052 6573 706f  CentralAPI Respo
-000335e0: 6e73 6520 6f62 6a65 6374 0a20 2020 2020  nse object.     
-000335f0: 2020 2022 2222 0a20 2020 2020 2020 2075     """.        u
-00033600: 726c 203d 2022 2f61 7069 2f72 6f75 7469  rl = "/api/routi
-00033610: 6e67 2f76 312f 6f76 6572 6c61 792f 696e  ng/v1/overlay/in
-00033620: 7465 7266 6163 6522 0a0a 2020 2020 2020  terface"..      
-00033630: 2020 7061 7261 6d73 203d 207b 0a20 2020    params = {.   
-00033640: 2020 2020 2020 2020 2027 6465 7669 6365           'device
-00033650: 273a 2064 6576 6963 652c 0a20 2020 2020  ': device,.     
-00033660: 2020 2020 2020 2027 6d61 726b 6572 273a         'marker':
-00033670: 206d 6172 6b65 722c 0a20 2020 2020 2020   marker,.       
-00033680: 2020 2020 2027 6c69 6d69 7427 3a20 6c69       'limit': li
-00033690: 6d69 740a 2020 2020 2020 2020 7d0a 0a20  mit.        }.. 
-000336a0: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
-000336b0: 6169 7420 7365 6c66 2e67 6574 2875 726c  ait self.get(url
-000336c0: 2c20 7061 7261 6d73 3d70 6172 616d 7329  , params=params)
-000336d0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-000336e0: 6765 745f 6465 6e79 6c69 7374 5f63 6c69  get_denylist_cli
-000336f0: 656e 7473 280a 2020 2020 2020 2020 7365  ents(.        se
-00033700: 6c66 2c0a 2020 2020 2020 2020 7365 7269  lf,.        seri
-00033710: 616c 3a20 7374 722c 0a20 2020 2029 202d  al: str,.    ) -
-00033720: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
-00033730: 2020 2020 2222 2247 6574 2061 6c6c 2064      """Get all d
-00033740: 656e 796c 6973 7420 636c 6965 6e74 206d  enylist client m
-00033750: 6163 2061 6464 7265 7373 2069 6e20 6465  ac address in de
-00033760: 7669 6365 2e0a 0a20 2020 2020 2020 2041  vice...        A
-00033770: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00033780: 2073 6572 6961 6c20 2873 7472 293a 2044   serial (str): D
-00033790: 6576 6963 6520 6964 206f 6620 7669 7274  evice id of virt
-000337a0: 7561 6c20 636f 6e74 726f 6c6c 6572 2028  ual controller (
-000337b0: 414f 5338 2049 4150 2920 6f72 2073 6572  AOS8 IAP) or ser
-000337c0: 6961 6c20 6f66 2041 4f53 3130 2061 702e  ial of AOS10 ap.
-000337d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000337e0: 2045 7861 6d70 6c65 3a31 3462 3337 3433   Example:14b3743
-000337f0: 6330 3166 3830 3830 6266 6130 3763 6130  c01f8080bfa07ca0
-00033800: 3533 6566 3165 3839 3564 6639 6330 3638  53ef1e895df9c068
-00033810: 3066 6535 6131 3762 6664 350a 0a20 2020  0fe5a17bfd5..   
-00033820: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00033830: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
-00033840: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
-00033850: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
-00033860: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00033870: 2020 2075 726c 203d 2066 222f 636f 6e66     url = f"/conf
-00033880: 6967 7572 6174 696f 6e2f 7631 2f73 7761  iguration/v1/swa
-00033890: 726d 2f7b 7365 7269 616c 7d2f 626c 6163  rm/{serial}/blac
-000338a0: 6b6c 6973 7469 6e67 220a 0a20 2020 2020  klisting"..     
-000338b0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-000338c0: 7365 6c66 2e67 6574 2875 726c 290a 0a0a  self.get(url)...
-000338d0: 2020 2020 6173 796e 6320 6465 6620 6765      async def ge
-000338e0: 745f 6175 746f 5f73 7562 7363 7269 6265  t_auto_subscribe
-000338f0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00033900: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
-00033910: 653a 0a20 2020 2020 2020 2022 2222 4765  e:.        """Ge
-00033920: 7420 7468 6520 7365 7276 6963 6573 2077  t the services w
-00033930: 6869 6368 2068 6176 6520 6175 746f 2073  hich have auto s
-00033940: 7562 7363 7269 6265 2065 6e61 626c 6564  ubscribe enabled
-00033950: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00033960: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00033970: 5265 7370 6f6e 7365 3a20 4365 6e74 7261  Response: Centra
-00033980: 6c41 5049 2052 6573 706f 6e73 6520 6f62  lAPI Response ob
-00033990: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
-000339a0: 0a20 2020 2020 2020 2075 726c 203d 2022  .        url = "
-000339b0: 2f70 6c61 7466 6f72 6d2f 6c69 6365 6e73  /platform/licens
-000339c0: 696e 672f 7631 2f63 7573 746f 6d65 722f  ing/v1/customer/
-000339d0: 7365 7474 696e 6773 2f61 7574 6f6c 6963  settings/autolic
-000339e0: 656e 7365 220a 0a20 2020 2020 2020 2072  ense"..        r
-000339f0: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-00033a00: 2e67 6574 2875 726c 290a 0a20 2020 2061  .get(url)..    a
-00033a10: 7379 6e63 2064 6566 2065 6e61 626c 655f  sync def enable_
-00033a20: 6175 746f 5f73 7562 7363 7269 6265 280a  auto_subscribe(.
-00033a30: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00033a40: 2020 2020 2020 7365 7276 6963 6573 3a20        services: 
-00033a50: 4c69 7374 5b73 7472 5d20 7c20 7374 722c  List[str] | str,
-00033a60: 0a20 2020 2029 202d 3e20 5265 7370 6f6e  .    ) -> Respon
-00033a70: 7365 3a0a 2020 2020 2020 2020 2222 2253  se:.        """S
-00033a80: 7461 6e64 616c 6f6e 6520 4375 7374 6f6d  tandalone Custom
-00033a90: 6572 2041 5049 3a20 4173 7369 676e 206c  er API: Assign l
-00033aa0: 6963 656e 7365 7320 746f 2061 6c6c 2064  icenses to all d
-00033ab0: 6576 6963 6573 2061 6e64 2065 6e61 626c  evices and enabl
-00033ac0: 6520 6175 746f 2073 7562 7363 7269 6265  e auto subscribe
-00033ad0: 2066 6f72 0a20 2020 2020 2020 2067 6976   for.        giv
-00033ae0: 656e 2073 6572 7669 6365 732e 0a0a 2020  en services...  
-00033af0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00033b00: 2020 2020 2020 2020 7365 7276 6963 6573          services
-00033b10: 2028 4c69 7374 5b73 7472 5d29 3a20 6c69   (List[str]): li
-00033b20: 7374 206f 6620 7365 7276 6963 6573 2065  st of services e
-00033b30: 2e67 2e20 5b27 7061 272c 2027 7563 6327  .g. ['pa', 'ucc'
-00033b40: 2c20 666f 756e 6461 7469 6f6e 5f61 702c  , foundation_ap,
-00033b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00033b60: 2061 6476 616e 6365 645f 7377 6974 6368   advanced_switch
-00033b70: 5f36 3230 302c 2066 6f75 6e64 6174 696f  _6200, foundatio
-00033b80: 6e5f 3730 5858 2065 7463 202e 2e2e 5d2e  n_70XX etc ...].
-00033b90: 2043 6865 636b 0a20 2020 2020 2020 2020   Check.         
-00033ba0: 2020 2020 2020 202f 706c 6174 666f 726d         /platform
-00033bb0: 2f6c 6963 656e 7369 6e67 2f76 312f 7365  /licensing/v1/se
-00033bc0: 7276 6963 6573 2f63 6f6e 6669 6720 4150  rvices/config AP
-00033bd0: 4920 7265 7370 6f6e 7365 2074 6f20 6b6e  I response to kn
-00033be0: 6f77 2074 6865 206c 6973 7420 6f66 2073  ow the list of s
-00033bf0: 7570 706f 7274 6564 0a20 2020 2020 2020  upported.       
-00033c00: 2020 2020 2020 2020 2073 6572 7669 6365           service
-00033c10: 732e 0a0a 2020 2020 2020 2020 5265 7475  s...        Retu
-00033c20: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00033c30: 2052 6573 706f 6e73 653a 2043 656e 7472   Response: Centr
-00033c40: 616c 4150 4920 5265 7370 6f6e 7365 206f  alAPI Response o
-00033c50: 626a 6563 740a 2020 2020 2020 2020 2222  bject.        ""
-00033c60: 220a 2020 2020 2020 2020 7572 6c20 3d20  ".        url = 
-00033c70: 222f 706c 6174 666f 726d 2f6c 6963 656e  "/platform/licen
-00033c80: 7369 6e67 2f76 312f 6375 7374 6f6d 6572  sing/v1/customer
-00033c90: 2f73 6574 7469 6e67 732f 6175 746f 6c69  /settings/autoli
-00033ca0: 6365 6e73 6522 0a0a 2020 2020 2020 2020  cense"..        
-00033cb0: 6966 2069 7369 6e73 7461 6e63 6528 7365  if isinstance(se
-00033cc0: 7276 6963 6573 2c20 7374 7229 3a0a 2020  rvices, str):.  
-00033cd0: 2020 2020 2020 2020 2020 7365 7276 6963            servic
-00033ce0: 6573 203d 205b 7365 7276 6963 6573 5d0a  es = [services].
-00033cf0: 0a20 2020 2020 2020 206a 736f 6e5f 6461  .        json_da
-00033d00: 7461 203d 207b 0a20 2020 2020 2020 2020  ta = {.         
-00033d10: 2020 2027 7365 7276 6963 6573 273a 2073     'services': s
-00033d20: 6572 7669 6365 730a 2020 2020 2020 2020  ervices.        
-00033d30: 7d0a 0a20 2020 2020 2020 2072 6574 7572  }..        retur
-00033d40: 6e20 6177 6169 7420 7365 6c66 2e70 6f73  n await self.pos
-00033d50: 7428 7572 6c2c 206a 736f 6e5f 6461 7461  t(url, json_data
-00033d60: 3d6a 736f 6e5f 6461 7461 290a 0a20 2020  =json_data)..   
-00033d70: 2061 7379 6e63 2064 6566 2064 6973 6162   async def disab
-00033d80: 6c65 5f61 7574 6f5f 7375 6273 6372 6962  le_auto_subscrib
-00033d90: 6528 0a20 2020 2020 2020 2073 656c 662c  e(.        self,
-00033da0: 0a20 2020 2020 2020 2073 6572 7669 6365  .        service
-00033db0: 733a 204c 6973 745b 7374 725d 207c 2073  s: List[str] | s
-00033dc0: 7472 2c0a 2020 2020 2920 2d3e 2052 6573  tr,.    ) -> Res
-00033dd0: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
-00033de0: 2222 5374 616e 6461 6c6f 6e65 2043 7573  ""Standalone Cus
-00033df0: 746f 6d65 7220 4150 493a 2044 6973 6162  tomer API: Disab
-00033e00: 6c65 2061 7574 6f20 6c69 6365 6e73 696e  le auto licensin
-00033e10: 6720 666f 7220 6769 7665 6e20 7365 7276  g for given serv
-00033e20: 6963 6573 2e0a 0a20 2020 2020 2020 2041  ices...        A
-00033e30: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00033e40: 2073 6572 7669 6365 7320 284c 6973 745b   services (List[
-00033e50: 7374 725d 293a 206c 6973 7420 6f66 2073  str]): list of s
-00033e60: 6572 7669 6365 7320 652e 672e 205b 2770  ervices e.g. ['p
-00033e70: 6127 2c20 2775 6363 272c 2066 6f75 6e64  a', 'ucc', found
-00033e80: 6174 696f 6e5f 6170 2c0a 2020 2020 2020  ation_ap,.      
-00033e90: 2020 2020 2020 2020 2020 6164 7661 6e63            advanc
-00033ea0: 6564 5f73 7769 7463 685f 3632 3030 2c20  ed_switch_6200, 
-00033eb0: 666f 756e 6461 7469 6f6e 5f37 3058 5820  foundation_70XX 
-00033ec0: 6574 6320 2e2e 2e5d 2e20 4368 6563 6b0a  etc ...]. Check.
-00033ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033ee0: 2f70 6c61 7466 6f72 6d2f 6c69 6365 6e73  /platform/licens
-00033ef0: 696e 672f 7631 2f73 6572 7669 6365 732f  ing/v1/services/
-00033f00: 636f 6e66 6967 2041 5049 2072 6573 706f  config API respo
-00033f10: 6e73 6520 746f 206b 6e6f 7720 7468 6520  nse to know the 
-00033f20: 6c69 7374 206f 6620 7375 7070 6f72 7465  list of supporte
-00033f30: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00033f40: 2020 7365 7276 6963 6573 2e0a 0a20 2020    services...   
-00033f50: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00033f60: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
-00033f70: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
-00033f80: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
-00033f90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00033fa0: 2020 2075 726c 203d 2022 2f70 6c61 7466     url = "/platf
-00033fb0: 6f72 6d2f 6c69 6365 6e73 696e 672f 7631  orm/licensing/v1
-00033fc0: 2f63 7573 746f 6d65 722f 7365 7474 696e  /customer/settin
-00033fd0: 6773 2f61 7574 6f6c 6963 656e 7365 220a  gs/autolicense".
-00033fe0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00033ff0: 7374 616e 6365 2873 6572 7669 6365 732c  stance(services,
-00034000: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
-00034010: 2020 2073 6572 7669 6365 7320 3d20 5b73     services = [s
-00034020: 6572 7669 6365 735d 0a0a 2020 2020 2020  ervices]..      
-00034030: 2020 6a73 6f6e 5f64 6174 6120 3d20 7b0a    json_data = {.
-00034040: 2020 2020 2020 2020 2020 2020 2773 6572              'ser
-00034050: 7669 6365 7327 3a20 7365 7276 6963 6573  vices': services
-00034060: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-00034070: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-00034080: 2073 656c 662e 6465 6c65 7465 2875 726c   self.delete(url
-00034090: 2c20 6a73 6f6e 5f64 6174 613d 6a73 6f6e  , json_data=json
-000340a0: 5f64 6174 6129 0a0a 2020 2020 2320 2f2f  _data)..    # //
-000340b0: 202d 2d20 4e6f 7420 7573 6564 2062 7920   -- Not used by 
-000340c0: 636f 6d6d 616e 6473 2079 6574 2e20 2075  commands yet.  u
-000340d0: 6e64 6f63 756d 656e 7465 6420 6b6d 7320  ndocumented kms 
-000340e0: 6170 6920 2d2d 202f 2f0a 2020 2020 6173  api -- //.    as
-000340f0: 796e 6320 6465 6620 6b6d 735f 6765 745f  ync def kms_get_
-00034100: 7379 6e63 6564 5f61 7073 2873 656c 662c  synced_aps(self,
-00034110: 206d 6163 3a20 7374 7229 202d 3e20 5265   mac: str) -> Re
-00034120: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
-00034130: 7572 6c20 3d20 6622 2f6b 6579 6d67 6d74  url = f"/keymgmt
-00034140: 2f76 312f 7379 6e63 6564 6170 6c69 7374  /v1/syncedaplist
-00034150: 2f7b 6d61 637d 220a 2020 2020 2020 2020  /{mac}".        
-00034160: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
-00034170: 662e 6765 7428 7572 6c29 0a0a 2020 2020  f.get(url)..    
-00034180: 6173 796e 6320 6465 6620 6b6d 735f 6765  async def kms_ge
-00034190: 745f 636c 6965 6e74 5f72 6563 6f72 6428  t_client_record(
-000341a0: 7365 6c66 2c20 6d61 633a 2073 7472 2920  self, mac: str) 
-000341b0: 2d3e 2052 6573 706f 6e73 653a 0a20 2020  -> Response:.   
-000341c0: 2020 2020 2075 726c 203d 2066 222f 6b65       url = f"/ke
-000341d0: 796d 676d 742f 7631 2f6b 6579 6361 6368  ymgmt/v1/keycach
-000341e0: 652f 7b6d 6163 7d22 0a20 2020 2020 2020  e/{mac}".       
-000341f0: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-00034200: 6c66 2e67 6574 2875 726c 290a 0a20 2020  lf.get(url)..   
-00034210: 2061 7379 6e63 2064 6566 206b 6d73 5f67   async def kms_g
-00034220: 6574 5f68 6173 6828 7365 6c66 2920 2d3e  et_hash(self) ->
-00034230: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
-00034240: 2020 2075 726c 203d 2022 2f6b 6579 6d67     url = "/keymg
-00034250: 6d74 2f76 312f 6b65 7968 6173 6822 0a20  mt/v1/keyhash". 
-00034260: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
-00034270: 6169 7420 7365 6c66 2e67 6574 2875 726c  ait self.get(url
-00034280: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-00034290: 206b 6d73 5f67 6574 5f61 705f 7374 6174   kms_get_ap_stat
-000342a0: 6528 7365 6c66 2c20 7365 7269 616c 3a20  e(self, serial: 
-000342b0: 7374 7229 202d 3e20 5265 7370 6f6e 7365  str) -> Response
-000342c0: 3a0a 2020 2020 2020 2020 7572 6c20 3d20  :.        url = 
-000342d0: 6622 2f6b 6579 6d67 6d74 2f76 312f 5374  f"/keymgmt/v1/St
-000342e0: 6174 732f 6170 2f7b 7365 7269 616c 7d22  ats/ap/{serial}"
-000342f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00034300: 6177 6169 7420 7365 6c66 2e67 6574 2875  await self.get(u
-00034310: 726c 290a 0a20 2020 2023 2042 6164 2065  rl)..    # Bad e
-00034320: 6e64 706f 696e 7420 5552 4c20 3430 340a  ndpoint URL 404.
-00034330: 2020 2020 6173 796e 6320 6465 6620 6b6d      async def km
-00034340: 735f 6765 745f 6865 616c 7468 2873 656c  s_get_health(sel
-00034350: 6629 202d 3e20 5265 7370 6f6e 7365 3a0a  f) -> Response:.
-00034360: 2020 2020 2020 2020 7572 6c20 3d20 222f          url = "/
-00034370: 6b65 796d 676d 742f 7631 2f68 6561 6c74  keymgmt/v1/healt
-00034380: 6822 0a20 2020 2020 2020 2072 6574 7572  h".        retur
-00034390: 6e20 6177 6169 7420 7365 6c66 2e67 6574  n await self.get
-000343a0: 2875 726c 290a 0a20 2020 2061 7379 6e63  (url)..    async
-000343b0: 2064 6566 2063 6c6f 7564 6175 7468 5f67   def cloudauth_g
-000343c0: 6574 5f72 6567 6973 7465 7265 645f 6d61  et_registered_ma
-000343d0: 6373 280a 2020 2020 2020 2020 7365 6c66  cs(.        self
-000343e0: 2c0a 2020 2020 2020 2020 7365 6172 6368  ,.        search
-000343f0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00034400: 2020 2020 2020 736f 7274 3a20 7374 7220        sort: str 
-00034410: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00034420: 6669 6c65 6e61 6d65 3a20 7374 7220 3d20  filename: str = 
-00034430: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 2052  None,.    ) -> R
-00034440: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
-00034450: 2022 2222 4665 7463 6820 616c 6c20 4d61   """Fetch all Ma
-00034460: 6320 5265 6769 7374 7261 7469 6f6e 7320  c Registrations 
-00034470: 6173 2061 2043 5356 2066 696c 652e 0a0a  as a CSV file...
-00034480: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00034490: 2020 2020 2020 2020 2020 7365 6172 6368            search
-000344a0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-000344b0: 3a20 4669 6c74 6572 2074 6865 204d 6163  : Filter the Mac
-000344c0: 2052 6567 6973 7472 6174 696f 6e73 2062   Registrations b
-000344d0: 7920 4d61 6320 4164 6472 6573 7320 616e  y Mac Address an
-000344e0: 6420 436c 6965 6e74 204e 616d 652e 0a20  d Client Name.. 
-000344f0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-00034500: 6f65 7320 6120 2763 6f6e 7461 696e 7327  oes a 'contains'
-00034510: 206d 6174 6368 2e0a 2020 2020 2020 2020   match..        
-00034520: 2020 2020 736f 7274 2028 7374 722c 206f      sort (str, o
-00034530: 7074 696f 6e61 6c29 3a20 536f 7274 206f  ptional): Sort o
-00034540: 7264 6572 2020 5661 6c69 6420 5661 6c75  rder  Valid Valu
-00034550: 6573 3a20 2b6e 616d 652c 202d 6e61 6d65  es: +name, -name
-00034560: 2c20 2b64 6973 706c 6179 5f6e 616d 652c  , +display_name,
-00034570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00034580: 202d 6469 7370 6c61 795f 6e61 6d65 0a20   -display_name. 
-00034590: 2020 2020 2020 2020 2020 2066 696c 656e             filen
-000345a0: 616d 6520 2873 7472 2c20 6f70 7469 6f6e  ame (str, option
-000345b0: 616c 293a 2053 7567 6765 7374 2061 2066  al): Suggest a f
-000345c0: 696c 6520 6e61 6d65 2066 6f72 2074 6865  ile name for the
-000345d0: 2064 6f77 6e6c 6f61 6469 6e67 2066 696c   downloading fil
-000345e0: 6520 7669 6120 636f 6e74 656e 740a 2020  e via content.  
-000345f0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00034600: 7370 6f73 6974 696f 6e20 6865 6164 6572  sposition header
-00034610: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00034620: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00034630: 5265 7370 6f6e 7365 3a20 4365 6e74 7261  Response: Centra
-00034640: 6c41 5049 2052 6573 706f 6e73 6520 6f62  lAPI Response ob
-00034650: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
-00034660: 0a20 2020 2020 2020 2075 726c 203d 2022  .        url = "
-00034670: 2f63 6c6f 7564 6175 7468 2f61 7069 2f76  /cloudauth/api/v
-00034680: 332f 6275 6c6b 2f6d 6163 220a 0a20 2020  3/bulk/mac"..   
-00034690: 2020 2020 2070 6172 616d 7320 3d20 7b0a       params = {.
-000346a0: 2020 2020 2020 2020 2020 2020 2773 6561              'sea
-000346b0: 7263 6827 3a20 7365 6172 6368 2c0a 2020  rch': search,.  
-000346c0: 2020 2020 2020 2020 2020 2773 6f72 7427            'sort'
-000346d0: 3a20 736f 7274 2c0a 2020 2020 2020 2020  : sort,.        
-000346e0: 2020 2020 2766 696c 656e 616d 6527 3a20      'filename': 
-000346f0: 6669 6c65 6e61 6d65 0a20 2020 2020 2020  filename.       
-00034700: 207d 0a0a 2020 2020 2020 2020 7265 7370   }..        resp
-00034710: 203d 2061 7761 6974 2073 656c 662e 6765   = await self.ge
-00034720: 7428 7572 6c2c 2070 6172 616d 733d 7061  t(url, params=pa
-00034730: 7261 6d73 290a 0a20 2020 2020 2020 2069  rams)..        i
-00034740: 6620 7265 7370 3a0a 2020 2020 2020 2020  f resp:.        
-00034750: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00034760: 2020 2020 2020 2020 2064 7320 3d20 7461           ds = ta
-00034770: 626c 6962 2e44 6174 6173 6574 2829 2e6c  blib.Dataset().l
-00034780: 6f61 6428 7265 7370 2e6f 7574 7075 7429  oad(resp.output)
-00034790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000347a0: 2072 6573 702e 6f75 7470 7574 203d 2079   resp.output = y
-000347b0: 616d 6c2e 6c6f 6164 2864 732e 6a73 6f6e  aml.load(ds.json
-000347c0: 2c20 4c6f 6164 6572 3d79 616d 6c2e 5361  , Loader=yaml.Sa
-000347d0: 6665 4c6f 6164 6572 290a 2020 2020 2020  feLoader).      
-000347e0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-000347f0: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
-00034800: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00034810: 2e65 7272 6f72 2866 2263 6c6f 7564 6175  .error(f"cloudau
-00034820: 7468 5f67 6574 5f72 6567 6973 7465 7265  th_get_registere
-00034830: 645f 6d61 6373 2063 6175 6768 7420 7b65  d_macs caught {e
-00034840: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
-00034850: 655f 5f7d 2074 7279 696e 6720 746f 2063  e__} trying to c
-00034860: 6f6e 7665 7274 2063 7376 2072 6574 7572  onvert csv retur
-00034870: 6e20 6672 6f6d 2041 5049 2074 6f20 6469  n from API to di
-00034880: 6374 2e22 2c20 6361 7074 696f 6e3d 5472  ct.", caption=Tr
-00034890: 7565 290a 0a20 2020 2020 2020 2072 6574  ue)..        ret
-000348a0: 7572 6e20 7265 7370 0a0a 2020 2020 6173  urn resp..    as
-000348b0: 796e 6320 6465 6620 636c 6f75 6461 7574  ync def cloudaut
-000348c0: 685f 7570 6c6f 6164 5f66 6978 6d65 280a  h_upload_fixme(.
-000348d0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000348e0: 2020 2020 2020 7570 6c6f 6164 5f74 7970        upload_typ
-000348f0: 653a 2043 6c6f 7564 4175 7468 5570 6c6f  e: CloudAuthUplo
-00034900: 6164 5479 7065 2c0a 2020 2020 2020 2020  adType,.        
-00034910: 6669 6c65 3a20 556e 696f 6e5b 5061 7468  file: Union[Path
-00034920: 2c20 7374 725d 2c0a 2020 2020 2020 2020  , str],.        
-00034930: 7373 6964 3a20 7374 7220 3d20 4e6f 6e65  ssid: str = None
-00034940: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
-00034950: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
-00034960: 5570 6c6f 6164 2066 696c 652e 0a0a 2020  Upload file...  
-00034970: 2020 2020 2020 5468 6973 2064 6f65 736e        This doesn
-00034980: 2774 2077 6f72 6b20 7374 696c 6c20 736f  't work still so
-00034990: 7274 696e 6720 7468 6520 666f 726d 6174  rting the format
-000349a0: 206f 6620 466f 726d 4461 7461 0a0a 2020   of FormData..  
-000349b0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-000349c0: 2020 2020 2020 2020 7570 6c6f 6164 5f74          upload_t
-000349d0: 7970 6520 2843 6c6f 7564 4175 7468 5570  ype (CloudAuthUp
-000349e0: 6c6f 6164 5479 7065 293a 2054 7970 6520  loadType): Type 
-000349f0: 6f66 2066 696c 6520 7570 6c6f 6164 2020  of file upload  
-00034a00: 5661 6c69 6420 5661 6c75 6573 3a20 6d70  Valid Values: mp
-00034a10: 736b 2c20 6d61 630a 2020 2020 2020 2020  sk, mac.        
-00034a20: 2020 2020 6669 6c65 2028 556e 696f 6e5b      file (Union[
-00034a30: 5061 7468 2c20 7374 725d 293a 2054 6865  Path, str]): The
-00034a40: 2063 7376 2066 696c 6520 746f 2075 706c   csv file to upl
-00034a50: 6f61 640a 2020 2020 2020 2020 2020 2020  oad.            
-00034a60: 7373 6964 2028 7374 722c 206f 7074 696f  ssid (str, optio
-00034a70: 6e61 6c29 3a20 4d50 534b 206e 6574 776f  nal): MPSK netwo
-00034a80: 726b 2053 5349 442c 2072 6571 7569 7265  rk SSID, require
-00034a90: 6420 6966 207b 7570 6c6f 6164 5f74 7970  d if {upload_typ
-00034aa0: 657d 203d 2027 6d70 736b 270a 0a20 2020  e} = 'mpsk'..   
-00034ab0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00034ac0: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
-00034ad0: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
-00034ae0: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
-00034af0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00034b00: 2020 2075 726c 203d 2066 222f 636c 6f75     url = f"/clou
-00034b10: 6461 7574 682f 6170 692f 7633 2f62 756c  dauth/api/v3/bul
-00034b20: 6b2f 7b75 706c 6f61 645f 7479 7065 7d22  k/{upload_type}"
-00034b30: 0a20 2020 2020 2020 2066 696c 6520 3d20  .        file = 
-00034b40: 6669 6c65 2069 6620 6973 696e 7374 616e  file if isinstan
-00034b50: 6365 2866 696c 652c 2050 6174 6829 2065  ce(file, Path) e
-00034b60: 6c73 6520 5061 7468 2873 7472 2866 696c  lse Path(str(fil
-00034b70: 6529 290a 2020 2020 2020 2020 2320 6461  e)).        # da
-00034b80: 7461 203d 206d 756c 7469 7061 7274 6966  ta = multipartif
-00034b90: 7928 6669 6c65 2e72 6561 645f 6279 7465  y(file.read_byte
-00034ba0: 7328 2929 0a20 2020 2020 2020 2023 2064  s()).        # d
-00034bb0: 6174 6120 3d20 6169 6f68 7474 702e 466f  ata = aiohttp.Fo
-00034bc0: 726d 4461 7461 2866 696c 652e 6f70 656e  rmData(file.open
-00034bd0: 2829 290a 0a20 2020 2020 2020 2070 6172  ())..        par
-00034be0: 616d 7320 3d20 7b0a 2020 2020 2020 2020  ams = {.        
-00034bf0: 2020 2020 2773 7369 6427 3a20 7373 6964      'ssid': ssid
-00034c00: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-00034c10: 2020 2066 696c 6573 203d 207b 2022 6669     files = { "fi
-00034c20: 6c65 223a 2028 6669 6c65 2e6e 616d 652c  le": (file.name,
-00034c30: 2066 696c 652e 6f70 656e 2822 7262 2229   file.open("rb")
-00034c40: 2c20 2274 6578 742f 6373 7622 2920 7d0a  , "text/csv") }.
-00034c50: 2020 2020 2020 2020 666f 726d 5f64 6174          form_dat
-00034c60: 6120 3d20 6169 6f68 7474 702e 466f 726d  a = aiohttp.Form
-00034c70: 4461 7461 2866 696c 6573 290a 2020 2020  Data(files).    
-00034c80: 2020 2020 2320 6669 6c65 7320 3d20 7b66      # files = {f
-00034c90: 277b 7570 6c6f 6164 5f74 7970 657d 5f69  '{upload_type}_i
-00034ca0: 6d70 6f72 7427 3a20 2866 277b 7570 6c6f  mport': (f'{uplo
-00034cb0: 6164 5f74 7970 657d 5f69 6d70 6f72 742e  ad_type}_import.
-00034cc0: 6373 7627 2c20 6669 6c65 2e72 6561 645f  csv', file.read_
-00034cd0: 6279 7465 7328 2929 7d0a 2020 2020 2020  bytes())}.      
-00034ce0: 2020 6865 6164 6572 7320 3d20 7b0a 2020    headers = {.  
-00034cf0: 2020 2020 2020 2020 2020 2243 6f6e 7465            "Conte
-00034d00: 6e74 2d54 7970 6522 3a20 226d 756c 7469  nt-Type": "multi
-00034d10: 7061 7274 2f66 6f72 6d2d 6461 7461 222c  part/form-data",
-00034d20: 0a20 2020 2020 2020 2020 2020 2027 4163  .            'Ac
-00034d30: 6365 7074 273a 2027 6170 706c 6963 6174  cept': 'applicat
-00034d40: 696f 6e2f 6a73 6f6e 270a 2020 2020 2020  ion/json'.      
-00034d50: 2020 7d0a 2020 2020 2020 2020 6865 6164    }.        head
-00034d60: 6572 7320 3d20 7b2a 2a68 6561 6465 7273  ers = {**headers
-00034d70: 2c20 2a2a 6469 6374 2861 696f 6874 7470  , **dict(aiohttp
-00034d80: 2e46 6f72 6d44 6174 6128 6669 6c65 7329  .FormData(files)
-00034d90: 2e5f 7772 6974 6572 2e5f 6865 6164 6572  ._writer._header
-00034da0: 7329 7d0a 0a20 2020 2020 2020 2072 6574  s)}..        ret
-00034db0: 7572 6e20 6177 6169 7420 7365 6c66 2e70  urn await self.p
-00034dc0: 6f73 7428 7572 6c2c 2068 6561 6465 7273  ost(url, headers
-00034dd0: 3d68 6561 6465 7273 2c20 7061 7261 6d73  =headers, params
-00034de0: 3d70 6172 616d 732c 2070 6179 6c6f 6164  =params, payload
-00034df0: 3d66 6f72 6d5f 6461 7461 290a 0a20 2020  =form_data)..   
-00034e00: 2061 7379 6e63 2064 6566 2063 6c6f 7564   async def cloud
-00034e10: 6175 7468 5f75 706c 6f61 6428 0a20 2020  auth_upload(.   
-00034e20: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00034e30: 2020 2075 706c 6f61 645f 7479 7065 3a20     upload_type: 
-00034e40: 436c 6f75 6441 7574 6855 706c 6f61 6454  CloudAuthUploadT
-00034e50: 7970 652c 0a20 2020 2020 2020 2066 696c  ype,.        fil
-00034e60: 653a 2055 6e69 6f6e 5b50 6174 682c 2073  e: Union[Path, s
-00034e70: 7472 5d2c 0a20 2020 2020 2020 2073 7369  tr],.        ssi
-00034e80: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-00034e90: 2020 2029 202d 3e20 5265 7370 6f6e 7365     ) -> Response
-00034ea0: 3a0a 0a20 2020 2020 2020 2022 2222 5570  :..        """Up
-00034eb0: 6c6f 6164 2066 696c 652e 0a0a 2020 2020  load file...    
-00034ec0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00034ed0: 2020 2020 2020 7570 6c6f 6164 5f74 7970        upload_typ
-00034ee0: 6520 2843 6c6f 7564 4175 7468 5570 6c6f  e (CloudAuthUplo
-00034ef0: 6164 5479 7065 293a 2054 7970 6520 6f66  adType): Type of
-00034f00: 2066 696c 6520 7570 6c6f 6164 2020 5661   file upload  Va
-00034f10: 6c69 6420 5661 6c75 6573 3a20 6d70 736b  lid Values: mpsk
-00034f20: 2c20 6d61 630a 2020 2020 2020 2020 2020  , mac.          
-00034f30: 2020 6669 6c65 2028 556e 696f 6e5b 5061    file (Union[Pa
-00034f40: 7468 2c20 7374 725d 293a 2054 6865 2063  th, str]): The c
-00034f50: 7376 2066 696c 6520 746f 2075 706c 6f61  sv file to uploa
-00034f60: 640a 2020 2020 2020 2020 2020 2020 7373  d.            ss
-00034f70: 6964 2028 7374 722c 206f 7074 696f 6e61  id (str, optiona
-00034f80: 6c29 3a20 4d50 534b 206e 6574 776f 726b  l): MPSK network
-00034f90: 2053 5349 442c 2072 6571 7569 7265 6420   SSID, required 
-00034fa0: 6966 207b 7570 6c6f 6164 5f74 7970 657d  if {upload_type}
-00034fb0: 203d 2027 6d70 736b 270a 0a20 2020 2020   = 'mpsk'..     
-00034fc0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00034fd0: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
-00034fe0: 3a20 4365 6e74 7261 6c41 5049 2052 6573  : CentralAPI Res
-00034ff0: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
-00035000: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00035010: 2075 726c 203d 2066 222f 636c 6f75 6461   url = f"/clouda
-00035020: 7574 682f 6170 692f 7633 2f62 756c 6b2f  uth/api/v3/bulk/
-00035030: 7b75 706c 6f61 645f 7479 7065 7d22 0a20  {upload_type}". 
-00035040: 2020 2020 2020 2066 696c 6520 3d20 6669         file = fi
-00035050: 6c65 2069 6620 6973 696e 7374 616e 6365  le if isinstance
-00035060: 2866 696c 652c 2050 6174 6829 2065 6c73  (file, Path) els
-00035070: 6520 5061 7468 2873 7472 2866 696c 6529  e Path(str(file)
-00035080: 290a 2020 2020 2020 2020 7061 7261 6d73  ).        params
-00035090: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-000350a0: 2027 7373 6964 273a 2073 7369 640a 2020   'ssid': ssid.  
-000350b0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-000350c0: 2023 2048 4143 4b20 6e65 6564 2074 6f20   # HACK need to 
-000350d0: 6d61 6b65 2074 6865 2061 626f 7665 2061  make the above a
-000350e0: 7379 6e63 2066 756e 6374 696f 6e20 776f  sync function wo
-000350f0: 726b 0a20 2020 2020 2020 2069 6d70 6f72  rk.        impor
-00035100: 7420 7265 7175 6573 7473 0a20 2020 2020  t requests.     
-00035110: 2020 2068 6561 6465 7273 203d 207b 0a20     headers = {. 
-00035120: 2020 2020 2020 2020 2020 2022 4175 7468             "Auth
-00035130: 6f72 697a 6174 696f 6e22 3a20 6622 4265  orization": f"Be
-00035140: 6172 6572 207b 7365 6c66 2e61 7574 682e  arer {self.auth.
-00035150: 6365 6e74 7261 6c5f 696e 666f 5b27 746f  central_info['to
-00035160: 6b65 6e27 5d5b 2761 6363 6573 735f 746f  ken']['access_to
-00035170: 6b65 6e27 5d7d 222c 0a20 2020 2020 2020  ken']}",.       
-00035180: 2020 2020 2027 4163 6365 7074 273a 2027       'Accept': '
-00035190: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-000351a0: 270a 2020 2020 2020 2020 7d0a 0a20 2020  '.        }..   
-000351b0: 2020 2020 2066 696c 6573 203d 207b 2022       files = { "
-000351c0: 6669 6c65 223a 2028 6669 6c65 2e6e 616d  file": (file.nam
-000351d0: 652c 2066 696c 652e 6f70 656e 2822 7262  e, file.open("rb
-000351e0: 2229 2c20 2274 6578 742f 6373 7622 2920  "), "text/csv") 
-000351f0: 7d0a 2020 2020 2020 2020 7572 6c3d 6622  }.        url=f"
-00035200: 7b73 656c 662e 6175 7468 2e63 656e 7472  {self.auth.centr
-00035210: 616c 5f69 6e66 6f5b 2762 6173 655f 7572  al_info['base_ur
-00035220: 6c27 5d7d 7b75 726c 7d22 0a0a 2020 2020  l']}{url}"..    
-00035230: 2020 2020 666f 7220 5f20 696e 2072 616e      for _ in ran
-00035240: 6765 2832 293a 0a20 2020 2020 2020 2020  ge(2):.         
-00035250: 2020 205f 7265 7370 203d 2072 6571 7565     _resp = reque
-00035260: 7374 732e 7265 7175 6573 7428 2250 4f53  sts.request("POS
-00035270: 5422 2c20 7572 6c3d 7572 6c2c 2070 6172  T", url=url, par
-00035280: 616d 733d 7061 7261 6d73 2c20 6669 6c65  ams=params, file
-00035290: 733d 6669 6c65 732c 2068 6561 6465 7273  s=files, headers
-000352a0: 3d68 6561 6465 7273 290a 2020 2020 2020  =headers).      
-000352b0: 2020 2020 2020 6f75 7470 7574 203d 2066        output = f
-000352c0: 225b 7b5f 7265 7370 2e72 6561 736f 6e7d  "[{_resp.reason}
-000352d0: 5d22 202b 2022 2022 202b 205f 7265 7370  ]" + " " + _resp
-000352e0: 2e74 6578 742e 6c73 7472 6970 2827 5b5c  .text.lstrip('[\
-000352f0: 6e20 2227 292e 7273 7472 6970 2827 225c  n "').rstrip('"\
-00035300: 6e5d 2729 0a20 2020 2020 2020 2020 2020  n]').           
-00035310: 2023 204d 616b 6520 7265 7175 6573 7473   # Make requests
-00035320: 2052 6573 706f 6e73 6520 6c6f 6f6b 206c   Response look l
-00035330: 696b 6520 6169 6f68 7474 702e 436c 6965  ike aiohttp.Clie
-00035340: 6e74 5265 7370 6f6e 7365 0a20 2020 2020  ntResponse.     
-00035350: 2020 2020 2020 205f 7265 7370 2e73 7461         _resp.sta
-00035360: 7475 732c 205f 7265 7370 2e6d 6574 686f  tus, _resp.metho
-00035370: 642c 205f 7265 7370 2e75 726c 203d 205f  d, _resp.url = _
-00035380: 7265 7370 2e73 7461 7475 735f 636f 6465  resp.status_code
-00035390: 2c20 2250 4f53 5422 2c20 5552 4c28 5f72  , "POST", URL(_r
-000353a0: 6573 702e 7572 6c29 0a20 2020 2020 2020  esp.url).       
-000353b0: 2020 2020 2072 6573 7020 3d20 5265 7370       resp = Resp
-000353c0: 6f6e 7365 285f 7265 7370 2c20 6f75 7470  onse(_resp, outp
-000353d0: 7574 3d6f 7574 7075 742c 2065 7272 6f72  ut=output, error
-000353e0: 3d4e 6f6e 6520 6966 205f 7265 7370 2e6f  =None if _resp.o
-000353f0: 6b20 656c 7365 205f 7265 7370 2e72 6561  k else _resp.rea
-00035400: 736f 6e2c 2075 726c 3d55 524c 2875 726c  son, url=URL(url
-00035410: 292c 2065 6c61 7073 6564 3d72 6f75 6e64  ), elapsed=round
-00035420: 285f 7265 7370 2e65 6c61 7073 6564 2e74  (_resp.elapsed.t
-00035430: 6f74 616c 5f73 6563 6f6e 6473 2829 2c20  otal_seconds(), 
-00035440: 3229 2c20 7374 6174 7573 5f63 6f64 653d  2), status_code=
-00035450: 5f72 6573 702e 7374 6174 7573 5f63 6f64  _resp.status_cod
-00035460: 652c 2072 6c5f 7374 723d 222d 2229 0a20  e, rl_str="-"). 
-00035470: 2020 2020 2020 2020 2020 2069 6620 2269             if "i
-00035480: 6e76 616c 6964 5f74 6f6b 656e 2220 696e  nvalid_token" in
-00035490: 2072 6573 702e 6f75 7470 7574 3a0a 2020   resp.output:.  
-000354a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000354b0: 6c66 2e72 6566 7265 7368 5f74 6f6b 656e  lf.refresh_token
-000354c0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-000354d0: 2020 2068 6561 6465 7273 5b22 4175 7468     headers["Auth
-000354e0: 6f72 697a 6174 696f 6e22 5d20 3d20 6622  orization"] = f"
-000354f0: 4265 6172 6572 207b 7365 6c66 2e61 7574  Bearer {self.aut
-00035500: 682e 6365 6e74 7261 6c5f 696e 666f 5b27  h.central_info['
-00035510: 746f 6b65 6e27 5d5b 2761 6363 6573 735f  token']['access_
-00035520: 746f 6b65 6e27 5d7d 220a 2020 2020 2020  token']}".      
-00035530: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00035540: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00035550: 6b0a 2020 2020 2020 2020 7265 7475 726e  k.        return
-00035560: 2072 6573 700a 0a20 2020 2061 7379 6e63   resp..    async
-00035570: 2064 6566 2063 6c6f 7564 6175 7468 5f75   def cloudauth_u
-00035580: 706c 6f61 645f 7374 6174 7573 280a 2020  pload_status(.  
-00035590: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000355a0: 2020 2020 7570 6c6f 6164 5f74 7970 653a      upload_type:
-000355b0: 2043 6c6f 7564 4175 7468 5570 6c6f 6164   CloudAuthUpload
-000355c0: 5479 7065 2c0a 2020 2020 2020 2020 7373  Type,.        ss
-000355d0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-000355e0: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
-000355f0: 653a 0a20 2020 2020 2020 2022 2222 5265  e:.        """Re
-00035600: 6164 2075 706c 6f61 6420 7374 6174 7573  ad upload status
-00035610: 206f 6620 6c61 7374 2066 696c 6520 7570   of last file up
-00035620: 6c6f 6164 2e0a 0a20 2020 2020 2020 2041  load...        A
-00035630: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00035640: 2075 706c 6f61 645f 7479 7065 2028 436c   upload_type (Cl
-00035650: 6f75 6441 7574 6855 706c 6f61 6454 7970  oudAuthUploadTyp
-00035660: 6529 3a20 5479 7065 206f 6620 6669 6c65  e): Type of file
-00035670: 2075 706c 6f61 6420 2056 616c 6964 2056   upload  Valid V
-00035680: 616c 7565 733a 206d 7073 6b2c 206d 6163  alues: mpsk, mac
-00035690: 0a20 2020 2020 2020 2020 2020 2073 7369  .            ssi
-000356a0: 6420 2873 7472 2c20 6f70 7469 6f6e 616c  d (str, optional
-000356b0: 293a 204d 5053 4b20 6e65 7477 6f72 6b20  ): MPSK network 
-000356c0: 5353 4944 2c20 7265 7175 6972 6564 2069  SSID, required i
-000356d0: 6620 7b75 706c 6f61 645f 7479 7065 7d20  f {upload_type} 
-000356e0: 3d20 276d 7073 6b27 0a0a 2020 2020 2020  = 'mpsk'..      
-000356f0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00035700: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
-00035710: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
-00035720: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
-00035730: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00035740: 7572 6c20 3d20 6622 2f63 6c6f 7564 6175  url = f"/cloudau
-00035750: 7468 2f61 7069 2f76 332f 6275 6c6b 2f7b  th/api/v3/bulk/{
-00035760: 7570 6c6f 6164 5f74 7970 657d 2f73 7461  upload_type}/sta
-00035770: 7475 7322 0a0a 2020 2020 2020 2020 7061  tus"..        pa
-00035780: 7261 6d73 203d 207b 0a20 2020 2020 2020  rams = {.       
-00035790: 2020 2020 2027 7373 6964 273a 2073 7369       'ssid': ssi
-000357a0: 640a 2020 2020 2020 2020 7d0a 0a20 2020  d.        }..   
-000357b0: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
-000357c0: 7420 7365 6c66 2e67 6574 2875 726c 2c20  t self.get(url, 
-000357d0: 7061 7261 6d73 3d70 6172 616d 7329 0a0a  params=params)..
-000357e0: 2020 2020 6173 796e 6320 6465 6620 636c      async def cl
-000357f0: 6f75 6461 7574 685f 6765 745f 6d70 736b  oudauth_get_mpsk
-00035800: 5f6e 6574 776f 726b 7328 0a20 2020 2020  _networks(.     
-00035810: 2020 2073 656c 662c 0a20 2020 2029 202d     self,.    ) -
-00035820: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
-00035830: 2020 2020 2222 2252 6561 6420 616c 6c20      """Read all 
-00035840: 636f 6e66 6967 7572 6564 204d 5053 4b20  configured MPSK 
-00035850: 6e65 7477 6f72 6b73 2e0a 0a20 2020 2020  networks...     
-00035860: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00035870: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
-00035880: 3a20 4365 6e74 7261 6c41 5049 2052 6573  : CentralAPI Res
-00035890: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
-000358a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000358b0: 2075 726c 203d 2022 2f63 6c6f 7564 4175   url = "/cloudAu
-000358c0: 7468 2f61 7069 2f76 322f 6d70 736b 220a  th/api/v2/mpsk".
-000358d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000358e0: 6177 6169 7420 7365 6c66 2e67 6574 2875  await self.get(u
-000358f0: 726c 290a 0a20 2020 2061 7379 6e63 2064  rl)..    async d
-00035900: 6566 2063 6c6f 7564 6175 7468 5f67 6574  ef cloudauth_get
-00035910: 5f6e 616d 6564 6d70 736b 280a 2020 2020  _namedmpsk(.    
-00035920: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00035930: 2020 6d70 736b 5f69 643a 2073 7472 2c0a    mpsk_id: str,.
-00035940: 2020 2020 2020 2020 6e61 6d65 3a20 7374          name: st
-00035950: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00035960: 2020 726f 6c65 3a20 7374 7220 3d20 4e6f    role: str = No
-00035970: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
-00035980: 7573 3a20 7374 7220 3d20 4e6f 6e65 2c0a  us: str = None,.
-00035990: 2020 2020 2020 2020 6375 7273 6f72 3a20          cursor: 
-000359a0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000359b0: 2020 2020 736f 7274 3a20 7374 7220 3d20      sort: str = 
-000359c0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c69  None,.        li
-000359d0: 6d69 743a 2069 6e74 203d 2031 3030 2c0a  mit: int = 100,.
-000359e0: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
-000359f0: 653a 0a20 2020 2020 2020 2022 2222 5265  e:.        """Re
-00035a00: 6164 2061 6c6c 206e 616d 6564 204d 5053  ad all named MPS
-00035a10: 4b2e 0a0a 2020 2020 2020 2020 4172 6773  K...        Args
-00035a20: 3a0a 2020 2020 2020 2020 2020 2020 6d70  :.            mp
-00035a30: 736b 5f69 6420 2873 7472 293a 2054 6865  sk_id (str): The
-00035a40: 204d 5053 4b20 636f 6e66 6967 7572 6174   MPSK configurat
-00035a50: 696f 6e20 4944 0a20 2020 2020 2020 2020  ion ID.         
-00035a60: 2020 206e 616d 6520 2873 7472 2c20 6f70     name (str, op
-00035a70: 7469 6f6e 616c 293a 2046 696c 7465 7220  tional): Filter 
-00035a80: 6279 206e 616d 6520 6f66 2074 6865 206e  by name of the n
-00035a90: 616d 6564 204d 5053 4b2e 2044 6f65 7320  amed MPSK. Does 
-00035aa0: 6120 2763 6f6e 7461 696e 7327 206d 6174  a 'contains' mat
-00035ab0: 6368 2e0a 2020 2020 2020 2020 2020 2020  ch..            
-00035ac0: 726f 6c65 2028 7374 722c 206f 7074 696f  role (str, optio
-00035ad0: 6e61 6c29 3a20 4669 6c74 6572 2062 7920  nal): Filter by 
-00035ae0: 726f 6c65 206f 6620 7468 6520 6e61 6d65  role of the name
-00035af0: 6420 4d50 534b 2e20 446f 6573 2061 6e20  d MPSK. Does an 
-00035b00: 2765 7175 616c 7327 206d 6174 6368 2e0a  'equals' match..
-00035b10: 2020 2020 2020 2020 2020 2020 7374 6174              stat
-00035b20: 7573 2028 7374 722c 206f 7074 696f 6e61  us (str, optiona
-00035b30: 6c29 3a20 4669 6c74 6572 2062 7920 7374  l): Filter by st
-00035b40: 6174 7573 206f 6620 7468 6520 6e61 6d65  atus of the name
-00035b50: 6420 4d50 534b 2e20 446f 6573 2061 6e20  d MPSK. Does an 
-00035b60: 2765 7175 616c 7327 206d 6174 6368 2e0a  'equals' match..
-00035b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035b80: 5661 6c69 6420 5661 6c75 6573 3a20 656e  Valid Values: en
-00035b90: 6162 6c65 642c 2064 6973 6162 6c65 640a  abled, disabled.
-00035ba0: 2020 2020 2020 2020 2020 2020 6375 7273              curs
-00035bb0: 6f72 2028 7374 722c 206f 7074 696f 6e61  or (str, optiona
-00035bc0: 6c29 3a20 466f 7220 6375 7273 6f72 2062  l): For cursor b
-00035bd0: 6173 6564 2070 6167 696e 6174 696f 6e2e  ased pagination.
-00035be0: 0a20 2020 2020 2020 2020 2020 2073 6f72  .            sor
-00035bf0: 7420 2873 7472 2c20 6f70 7469 6f6e 616c  t (str, optional
-00035c00: 293a 2053 6f72 7420 6f72 6465 7220 2056  ): Sort order  V
-00035c10: 616c 6964 2056 616c 7565 733a 202b 6e61  alid Values: +na
-00035c20: 6d65 2c20 2d6e 616d 652c 202b 726f 6c65  me, -name, +role
-00035c30: 2c20 2d72 6f6c 652c 202b 7374 6174 7573  , -role, +status
-00035c40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00035c50: 2020 2d73 7461 7475 730a 2020 2020 2020    -status.      
-00035c60: 2020 2020 2020 6c69 6d69 7420 2869 6e74        limit (int
-00035c70: 2c20 6f70 7469 6f6e 616c 293a 204e 756d  , optional): Num
-00035c80: 6265 7220 6f66 2069 7465 6d73 2074 6f20  ber of items to 
-00035c90: 6265 2066 6574 6368 6564 2044 6566 6175  be fetched Defau
-00035ca0: 6c74 7320 746f 2031 3030 2e0a 0a20 2020  lts to 100...   
-00035cb0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00035cc0: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
-00035cd0: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
-00035ce0: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
-00035cf0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00035d00: 2020 2075 726c 203d 2066 222f 636c 6f75     url = f"/clou
-00035d10: 6441 7574 682f 6170 692f 7632 2f6d 7073  dAuth/api/v2/mps
-00035d20: 6b2f 7b6d 7073 6b5f 6964 7d2f 6e61 6d65  k/{mpsk_id}/name
-00035d30: 644d 5053 4b22 0a0a 2020 2020 2020 2020  dMPSK"..        
-00035d40: 7061 7261 6d73 203d 207b 0a20 2020 2020  params = {.     
-00035d50: 2020 2020 2020 2027 6e61 6d65 273a 206e         'name': n
-00035d60: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-00035d70: 2027 726f 6c65 273a 2072 6f6c 652c 0a20   'role': role,. 
-00035d80: 2020 2020 2020 2020 2020 2027 7374 6174             'stat
-00035d90: 7573 273a 2073 7461 7475 732c 0a20 2020  us': status,.   
-00035da0: 2020 2020 2020 2020 2027 6375 7273 6f72           'cursor
-00035db0: 273a 2063 7572 736f 722c 0a20 2020 2020  ': cursor,.     
-00035dc0: 2020 2020 2020 2027 736f 7274 273a 2073         'sort': s
-00035dd0: 6f72 742c 0a20 2020 2020 2020 2020 2020  ort,.           
-00035de0: 2027 6c69 6d69 7427 3a20 6c69 6d69 740a   'limit': limit.
-00035df0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00035e00: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00035e10: 7365 6c66 2e67 6574 2875 726c 2c20 7061  self.get(url, pa
-00035e20: 7261 6d73 3d70 6172 616d 7329 0a0a 2020  rams=params)..  
-00035e30: 2020 6173 796e 6320 6465 6620 636c 6f75    async def clou
-00035e40: 6461 7574 685f 646f 776e 6c6f 6164 5f6d  dauth_download_m
-00035e50: 7073 6b5f 6373 7628 0a20 2020 2020 2020  psk_csv(.       
-00035e60: 2073 656c 662c 0a20 2020 2020 2020 2073   self,.        s
-00035e70: 7369 643a 2073 7472 2c0a 2020 2020 2020  sid: str,.      
-00035e80: 2020 6669 6c65 6e61 6d65 3a20 7374 7220    filename: str 
-00035e90: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00035ea0: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
-00035eb0: 2c0a 2020 2020 2020 2020 726f 6c65 3a20  ,.        role: 
-00035ec0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00035ed0: 2020 2020 7374 6174 7573 3a20 7374 7220      status: str 
-00035ee0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00035ef0: 736f 7274 3a20 7374 7220 3d20 4e6f 6e65  sort: str = None
-00035f00: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
-00035f10: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
-00035f20: 4665 7463 6820 616c 6c20 4e61 6d65 6420  Fetch all Named 
-00035f30: 4d50 534b 2061 7320 6120 4353 5620 6669  MPSK as a CSV fi
-00035f40: 6c65 2e0a 0a20 2020 2020 2020 2041 7267  le...        Arg
-00035f50: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00035f60: 7369 6420 2873 7472 293a 2043 6f6e 6669  sid (str): Confi
-00035f70: 6775 7265 6420 4d50 534b 2053 5349 4420  gured MPSK SSID 
-00035f80: 666f 7220 7768 6963 6820 4e61 6d65 6420  for which Named 
-00035f90: 4d50 534b 7320 6172 6520 746f 2062 6520  MPSKs are to be 
-00035fa0: 646f 776e 6c6f 6164 6564 2e0a 2020 2020  downloaded..    
-00035fb0: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
-00035fc0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-00035fd0: 3a20 5375 6767 6573 7420 6120 6669 6c65  : Suggest a file
-00035fe0: 206e 616d 6520 666f 7220 7468 6520 646f   name for the do
-00035ff0: 776e 6c6f 6164 696e 6720 6669 6c65 2076  wnloading file v
-00036000: 6961 2063 6f6e 7465 6e74 0a20 2020 2020  ia content.     
-00036010: 2020 2020 2020 2020 2020 2064 6973 706f             dispo
-00036020: 7369 7469 6f6e 2068 6561 6465 722e 0a20  sition header.. 
-00036030: 2020 2020 2020 2020 2020 206e 616d 6520             name 
-00036040: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
-00036050: 2046 696c 7465 7220 6279 206e 616d 6520   Filter by name 
-00036060: 6f66 2074 6865 206e 616d 6564 204d 5053  of the named MPS
-00036070: 4b2e 2044 6f65 7320 6120 2763 6f6e 7461  K. Does a 'conta
-00036080: 696e 7327 206d 6174 6368 2e0a 2020 2020  ins' match..    
-00036090: 2020 2020 2020 2020 726f 6c65 2028 7374          role (st
-000360a0: 722c 206f 7074 696f 6e61 6c29 3a20 4669  r, optional): Fi
-000360b0: 6c74 6572 2062 7920 726f 6c65 206f 6620  lter by role of 
-000360c0: 7468 6520 6e61 6d65 6420 4d50 534b 2e20  the named MPSK. 
-000360d0: 446f 6573 2061 6e20 2765 7175 616c 7327  Does an 'equals'
-000360e0: 206d 6174 6368 2e0a 2020 2020 2020 2020   match..        
-000360f0: 2020 2020 7374 6174 7573 2028 7374 722c      status (str,
-00036100: 206f 7074 696f 6e61 6c29 3a20 4669 6c74   optional): Filt
-00036110: 6572 2062 7920 7374 6174 7573 206f 6620  er by status of 
-00036120: 7468 6520 6e61 6d65 6420 4d50 534b 2e20  the named MPSK. 
-00036130: 446f 6573 2061 6e20 2765 7175 616c 7327  Does an 'equals'
-00036140: 206d 6174 6368 2e0a 2020 2020 2020 2020   match..        
-00036150: 2020 2020 2020 2020 5661 6c69 6420 5661          Valid Va
-00036160: 6c75 6573 3a20 656e 6162 6c65 642c 2064  lues: enabled, d
-00036170: 6973 6162 6c65 640a 2020 2020 2020 2020  isabled.        
-00036180: 2020 2020 736f 7274 2028 7374 722c 206f      sort (str, o
-00036190: 7074 696f 6e61 6c29 3a20 536f 7274 206f  ptional): Sort o
-000361a0: 7264 6572 2020 5661 6c69 6420 5661 6c75  rder  Valid Valu
-000361b0: 6573 3a20 2b6e 616d 652c 202d 6e61 6d65  es: +name, -name
-000361c0: 2c20 2b72 6f6c 652c 202d 726f 6c65 2c20  , +role, -role, 
-000361d0: 2b73 7461 7475 732c 0a20 2020 2020 2020  +status,.       
-000361e0: 2020 2020 2020 2020 202d 7374 6174 7573           -status
-000361f0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00036200: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00036210: 6573 706f 6e73 653a 2043 656e 7472 616c  esponse: Central
-00036220: 4150 4920 5265 7370 6f6e 7365 206f 626a  API Response obj
-00036230: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
-00036240: 2020 2020 2020 2020 7572 6c20 3d20 222f          url = "/
-00036250: 636c 6f75 6441 7574 682f 6170 692f 7632  cloudAuth/api/v2
-00036260: 2f64 6f77 6e6c 6f61 642f 6d70 736b 220a  /download/mpsk".
-00036270: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-00036280: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00036290: 2773 7369 6427 3a20 7373 6964 2c0a 2020  'ssid': ssid,.  
-000362a0: 2020 2020 2020 2020 2020 2766 696c 656e            'filen
-000362b0: 616d 6527 3a20 6669 6c65 6e61 6d65 2c0a  ame': filename,.
-000362c0: 2020 2020 2020 2020 2020 2020 276e 616d              'nam
-000362d0: 6527 3a20 6e61 6d65 2c0a 2020 2020 2020  e': name,.      
-000362e0: 2020 2020 2020 2772 6f6c 6527 3a20 726f        'role': ro
-000362f0: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
-00036300: 2773 7461 7475 7327 3a20 7374 6174 7573  'status': status
-00036310: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
-00036320: 6f72 7427 3a20 736f 7274 0a20 2020 2020  ort': sort.     
-00036330: 2020 207d 0a0a 2020 2020 2020 2020 7265     }..        re
-00036340: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
-00036350: 6765 7428 7572 6c2c 2070 6172 616d 733d  get(url, params=
-00036360: 7061 7261 6d73 290a 0a20 2020 2061 7379  params)..    asy
-00036370: 6e63 2064 6566 2067 6574 5f75 7365 725f  nc def get_user_
-00036380: 6163 636f 756e 7473 280a 2020 2020 2020  accounts(.      
-00036390: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000363a0: 6170 705f 6e61 6d65 3a20 7374 7220 3d20  app_name: str = 
-000363b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7479  None,.        ty
-000363c0: 7065 3a20 7374 7220 3d20 4e6f 6e65 2c0a  pe: str = None,.
-000363d0: 2020 2020 2020 2020 7374 6174 7573 3a20          status: 
-000363e0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000363f0: 2020 2020 6f72 6465 725f 6279 3a20 7374      order_by: st
-00036400: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00036410: 2020 6f66 6673 6574 3a20 696e 7420 3d20    offset: int = 
-00036420: 302c 0a20 2020 2020 2020 206c 696d 6974  0,.        limit
-00036430: 3a20 696e 7420 3d20 3130 302c 0a20 2020  : int = 100,.   
-00036440: 2029 202d 3e20 5265 7370 6f6e 7365 3a0a   ) -> Response:.
-00036450: 2020 2020 2020 2020 2222 224c 6973 7420          """List 
-00036460: 7573 6572 2061 6363 6f75 6e74 732e 0a0a  user accounts...
-00036470: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00036480: 2020 2020 2020 2020 2020 6170 705f 6e61            app_na
-00036490: 6d65 2028 7374 722c 206f 7074 696f 6e61  me (str, optiona
-000364a0: 6c29 3a20 4170 706e 616d 6520 6e6d 7320  l): Appname nms 
-000364b0: 746f 2066 696c 7465 7220 4172 7562 6120  to filter Aruba 
-000364c0: 4365 6e74 7261 6c20 7573 6572 732c 2061  Central users, a
-000364d0: 6e64 2061 6363 6f75 6e74 5f73 6574 7469  nd account_setti
-000364e0: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
-000364f0: 2020 2074 6f20 6669 6c74 6572 2048 5045     to filter HPE
-00036500: 2047 7265 656e 4c61 6b65 2045 6467 6520   GreenLake Edge 
-00036510: 746f 2043 6c6f 7564 2050 6c61 7466 6f72  to Cloud Platfor
-00036520: 6d20 2843 4353 2920 6170 706c 6963 6174  m (CCS) applicat
-00036530: 696f 6e20 7573 6572 7320 2056 616c 6964  ion users  Valid
-00036540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00036550: 2056 616c 7565 733a 206e 6d73 2c20 6163   Values: nms, ac
-00036560: 636f 756e 745f 7365 7474 696e 670a 2020  count_setting.  
-00036570: 2020 2020 2020 2020 2020 7479 7065 2028            type (
-00036580: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
-00036590: 4669 6c74 6572 2062 6173 6564 206f 6e20  Filter based on 
-000365a0: 7379 7374 656d 206f 7220 6665 6465 7261  system or federa
-000365b0: 7465 6420 7573 6572 2020 5661 6c69 6420  ted user  Valid 
-000365c0: 5661 6c75 6573 3a20 7379 7374 656d 2c0a  Values: system,.
-000365d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000365e0: 6665 6465 7261 7465 640a 2020 2020 2020  federated.      
-000365f0: 2020 2020 2020 7374 6174 7573 2028 7374        status (st
-00036600: 722c 206f 7074 696f 6e61 6c29 3a20 4669  r, optional): Fi
-00036610: 6c74 6572 2075 7365 7220 6261 7365 6420  lter user based 
-00036620: 6f6e 2073 7461 7475 7320 2869 6e70 726f  on status (inpro
-00036630: 6772 6573 732c 2066 6169 6c65 6429 2020  gress, failed)  
-00036640: 5661 6c69 6420 5661 6c75 6573 3a0a 2020  Valid Values:.  
-00036650: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00036660: 7072 6f67 7265 7373 2c20 6661 696c 6564  progress, failed
-00036670: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
-00036680: 6572 5f62 7920 2873 7472 2c20 6f70 7469  er_by (str, opti
-00036690: 6f6e 616c 293a 2053 6f72 7420 6f72 6465  onal): Sort orde
-000366a0: 7269 6e67 2028 6173 6365 6e64 696e 6720  ring (ascending 
-000366b0: 6f72 2064 6573 6365 6e64 696e 6729 2e20  or descending). 
-000366c0: 2b75 7365 726e 616d 6520 7369 676e 6966  +username signif
-000366d0: 6965 730a 2020 2020 2020 2020 2020 2020  ies.            
-000366e0: 2020 2020 6173 6365 6e64 696e 6720 6f72      ascending or
-000366f0: 6465 7220 6f66 2075 7365 726e 616d 652e  der of username.
-00036700: 2020 5661 6c69 6420 5661 6c75 6573 3a20    Valid Values: 
-00036710: 2b75 7365 726e 616d 652c 202d 7573 6572  +username, -user
-00036720: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
-00036730: 206f 6666 7365 7420 2869 6e74 2c20 6f70   offset (int, op
-00036740: 7469 6f6e 616c 293a 205a 6572 6f20 6261  tional): Zero ba
-00036750: 7365 6420 6f66 6673 6574 2074 6f20 7374  sed offset to st
-00036760: 6172 7420 6672 6f6d 2044 6566 6175 6c74  art from Default
-00036770: 7320 746f 2030 2e0a 2020 2020 2020 2020  s to 0..        
-00036780: 2020 2020 6c69 6d69 7420 2869 6e74 2c20      limit (int, 
-00036790: 6f70 7469 6f6e 616c 293a 204d 6178 696d  optional): Maxim
-000367a0: 756d 206e 756d 6265 7220 6f66 2069 7465  um number of ite
-000367b0: 6d73 2074 6f20 7265 7475 726e 2044 6566  ms to return Def
-000367c0: 6175 6c74 7320 746f 2031 3030 2e0a 0a20  aults to 100... 
-000367d0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-000367e0: 2020 2020 2020 2020 2020 2020 5265 7370              Resp
-000367f0: 6f6e 7365 3a20 4365 6e74 7261 6c41 5049  onse: CentralAPI
-00036800: 2052 6573 706f 6e73 6520 6f62 6a65 6374   Response object
-00036810: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00036820: 2020 2020 2075 726c 203d 2022 2f70 6c61       url = "/pla
-00036830: 7466 6f72 6d2f 7262 6163 2f76 312f 7573  tform/rbac/v1/us
-00036840: 6572 7322 0a0a 2020 2020 2020 2020 7061  ers"..        pa
-00036850: 7261 6d73 203d 207b 0a20 2020 2020 2020  rams = {.       
-00036860: 2020 2020 2027 6170 705f 6e61 6d65 273a       'app_name':
-00036870: 2061 7070 5f6e 616d 652c 0a20 2020 2020   app_name,.     
-00036880: 2020 2020 2020 2027 7479 7065 273a 2074         'type': t
-00036890: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
-000368a0: 2027 7374 6174 7573 273a 2073 7461 7475   'status': statu
-000368b0: 732c 0a20 2020 2020 2020 2020 2020 2027  s,.            '
-000368c0: 6f72 6465 725f 6279 273a 206f 7264 6572  order_by': order
-000368d0: 5f62 792c 0a20 2020 2020 2020 2020 2020  _by,.           
-000368e0: 2027 6f66 6673 6574 273a 206f 6666 7365   'offset': offse
-000368f0: 742c 0a20 2020 2020 2020 2020 2020 2027  t,.            '
-00036900: 6c69 6d69 7427 3a20 6c69 6d69 740a 2020  limit': limit.  
-00036910: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-00036920: 2023 2054 4f44 4f20 7468 6973 206e 6565   # TODO this nee
-00036930: 6473 2061 2066 6169 7220 616d 6f75 6e74  ds a fair amount
-00036940: 206f 6620 6d61 7373 6167 696e 6720 746f   of massaging to
-00036950: 2074 7572 6e20 696e 746f 2061 2063 6f6d   turn into a com
-00036960: 6d61 6e64 2c20 6974 2773 206e 6573 7465  mand, it's neste
-00036970: 6420 6469 6374 730a 2020 2020 2020 2020  d dicts.        
-00036980: 2320 6578 616d 706c 6520 7265 7370 6f6e  # example respon
-00036990: 7365 2069 6e20 7072 6976 6174 6520 7673  se in private vs
-000369a0: 636f 6465 2064 6972 2e0a 2020 2020 2020  code dir..      
-000369b0: 2020 7265 7370 203d 2061 7761 6974 2073    resp = await s
-000369c0: 656c 662e 6765 7428 7572 6c2c 2070 6172  elf.get(url, par
-000369d0: 616d 733d 7061 7261 6d73 290a 2020 2020  ams=params).    
-000369e0: 2020 2020 7265 7475 726e 2072 6573 700a      return resp.
-000369f0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00036a00: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
-00036a10: 7061 7373 0a                             pass.
+000302d0: 6173 796e 6320 6465 6620 6765 745f 706f  async def get_po
+000302e0: 7274 616c 5f70 726f 6669 6c65 280a 2020  rtal_profile(.  
+000302f0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00030300: 2020 2020 706f 7274 616c 5f69 643a 2073      portal_id: s
+00030310: 7472 2c0a 2020 2020 2920 2d3e 2052 6573  tr,.    ) -> Res
+00030320: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
+00030330: 2222 4765 7420 6775 6573 7420 706f 7274  ""Get guest port
+00030340: 616c 2070 726f 6669 6c65 2e0a 0a20 2020  al profile...   
+00030350: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00030360: 2020 2020 2020 2070 6f72 7461 6c5f 6964         portal_id
+00030370: 2028 7374 7229 3a20 506f 7274 616c 2049   (str): Portal I
+00030380: 4420 6f66 2074 6865 2073 706c 6173 6820  D of the splash 
+00030390: 7061 6765 0a0a 2020 2020 2020 2020 5265  page..        Re
+000303a0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+000303b0: 2020 2052 6573 706f 6e73 653a 2043 656e     Response: Cen
+000303c0: 7472 616c 4150 4920 5265 7370 6f6e 7365  tralAPI Response
+000303d0: 206f 626a 6563 740a 2020 2020 2020 2020   object.        
+000303e0: 2222 220a 2020 2020 2020 2020 7572 6c20  """.        url 
+000303f0: 3d20 6622 2f67 7565 7374 2f76 312f 706f  = f"/guest/v1/po
+00030400: 7274 616c 732f 7b70 6f72 7461 6c5f 6964  rtals/{portal_id
+00030410: 7d22 0a0a 2020 2020 2020 2020 7265 7475  }"..        retu
+00030420: 726e 2061 7761 6974 2073 656c 662e 6765  rn await self.ge
+00030430: 7428 7572 6c29 0a0a 2020 2020 6173 796e  t(url)..    asyn
+00030440: 6320 6465 6620 6765 745f 7669 7369 746f  c def get_visito
+00030450: 7273 280a 2020 2020 2020 2020 7365 6c66  rs(.        self
+00030460: 2c0a 2020 2020 2020 2020 706f 7274 616c  ,.        portal
+00030470: 5f69 643a 2073 7472 2c0a 2020 2020 2020  _id: str,.      
+00030480: 2020 736f 7274 3a20 7374 7220 3d20 272b    sort: str = '+
+00030490: 6e61 6d65 272c 0a20 2020 2020 2020 2066  name',.        f
+000304a0: 696c 7465 725f 6279 3a20 7374 7220 3d20  ilter_by: str = 
+000304b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6669  None,.        fi
+000304c0: 6c74 6572 5f76 616c 7565 3a20 7374 7220  lter_value: str 
+000304d0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000304e0: 6f66 6673 6574 3a20 696e 7420 3d20 302c  offset: int = 0,
+000304f0: 0a20 2020 2020 2020 206c 696d 6974 3a20  .        limit: 
+00030500: 696e 7420 3d20 3130 302c 0a20 2020 2029  int = 100,.    )
+00030510: 202d 3e20 5265 7370 6f6e 7365 3a0a 2020   -> Response:.  
+00030520: 2020 2020 2020 2222 2247 6574 2061 6c6c        """Get all
+00030530: 2076 6973 6974 6f72 7320 6372 6561 7465   visitors create
+00030540: 6420 6167 6169 6e73 7420 6120 706f 7274  d against a port
+00030550: 616c 2e0a 0a20 2020 2020 2020 2041 7267  al...        Arg
+00030560: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+00030570: 6f72 7461 6c5f 6964 2028 7374 7229 3a20  ortal_id (str): 
+00030580: 506f 7274 616c 2049 4420 6f66 2074 6865  Portal ID of the
+00030590: 2073 706c 6173 6820 7061 6765 0a20 2020   splash page.   
+000305a0: 2020 2020 2020 2020 2073 6f72 7420 2873           sort (s
+000305b0: 7472 2c20 6f70 7469 6f6e 616c 293a 202b  tr, optional): +
+000305c0: 2069 7320 666f 7220 6173 6365 6e64 696e   is for ascendin
+000305d0: 6720 2061 6e64 202d 2066 6f72 2064 6573  g  and - for des
+000305e0: 6365 6e64 696e 6720 6f72 6465 7220 2c20  cending order , 
+000305f0: 736f 7274 7320 6279 206e 616d 6520 666f  sorts by name fo
+00030600: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+00030610: 2020 6e6f 7720 2056 616c 6964 2056 616c    now  Valid Val
+00030620: 7565 733a 202b 6e61 6d65 2c20 2d6e 616d  ues: +name, -nam
+00030630: 650a 2020 2020 2020 2020 2020 2020 6669  e.            fi
+00030640: 6c74 6572 5f62 7920 2873 7472 2c20 6f70  lter_by (str, op
+00030650: 7469 6f6e 616c 293a 2066 696c 7465 7220  tional): filter 
+00030660: 6279 2065 6d61 696c 206f 7220 6e61 6d65  by email or name
+00030670: 2020 5661 6c69 6420 5661 6c75 6573 3a20    Valid Values: 
+00030680: 6e61 6d65 2c20 656d 6169 6c0a 2020 2020  name, email.    
+00030690: 2020 2020 2020 2020 6669 6c74 6572 5f76          filter_v
+000306a0: 616c 7565 2028 7374 722c 206f 7074 696f  alue (str, optio
+000306b0: 6e61 6c29 3a20 6669 6c74 6572 2076 616c  nal): filter val
+000306c0: 7565 0a20 2020 2020 2020 2020 2020 206f  ue.            o
+000306d0: 6666 7365 7420 2869 6e74 2c20 6f70 7469  ffset (int, opti
+000306e0: 6f6e 616c 293a 2053 7461 7274 696e 6720  onal): Starting 
+000306f0: 696e 6465 7820 6f66 2065 6c65 6d65 6e74  index of element
+00030700: 2066 6f72 2061 2070 6167 696e 6174 6564   for a paginated
+00030710: 2071 7565 7279 2044 6566 6175 6c74 7320   query Defaults 
+00030720: 746f 2030 2e0a 2020 2020 2020 2020 2020  to 0..          
+00030730: 2020 6c69 6d69 7420 2869 6e74 2c20 6f70    limit (int, op
+00030740: 7469 6f6e 616c 293a 204e 756d 6265 7220  tional): Number 
+00030750: 6f66 2069 7465 6d73 2072 6571 7569 7265  of items require
+00030760: 6420 7065 7220 7175 6572 7920 4465 6661  d per query Defa
+00030770: 756c 7473 2074 6f20 3130 302e 0a0a 2020  ults to 100...  
+00030780: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00030790: 2020 2020 2020 2020 2020 2052 6573 706f             Respo
+000307a0: 6e73 653a 2043 656e 7472 616c 4150 4920  nse: CentralAPI 
+000307b0: 5265 7370 6f6e 7365 206f 626a 6563 740a  Response object.
+000307c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000307d0: 2020 2020 7572 6c20 3d20 6622 2f67 7565      url = f"/gue
+000307e0: 7374 2f76 312f 706f 7274 616c 732f 7b70  st/v1/portals/{p
+000307f0: 6f72 7461 6c5f 6964 7d2f 7669 7369 746f  ortal_id}/visito
+00030800: 7273 220a 0a20 2020 2020 2020 2070 6172  rs"..        par
+00030810: 616d 7320 3d20 7b0a 2020 2020 2020 2020  ams = {.        
+00030820: 2020 2020 2773 6f72 7427 3a20 736f 7274      'sort': sort
+00030830: 2c0a 2020 2020 2020 2020 2020 2020 2766  ,.            'f
+00030840: 696c 7465 725f 6279 273a 2066 696c 7465  ilter_by': filte
+00030850: 725f 6279 2c0a 2020 2020 2020 2020 2020  r_by,.          
+00030860: 2020 2766 696c 7465 725f 7661 6c75 6527    'filter_value'
+00030870: 3a20 6669 6c74 6572 5f76 616c 7565 2c0a  : filter_value,.
+00030880: 2020 2020 2020 2020 2020 2020 276f 6666              'off
+00030890: 7365 7427 3a20 6f66 6673 6574 2c0a 2020  set': offset,.  
+000308a0: 2020 2020 2020 2020 2020 276c 696d 6974            'limit
+000308b0: 273a 206c 696d 6974 0a20 2020 2020 2020  ': limit.       
+000308c0: 207d 0a20 2020 2020 2020 2070 6172 616d   }.        param
+000308d0: 7320 3d20 7574 696c 732e 7374 7269 705f  s = utils.strip_
+000308e0: 6e6f 6e65 2870 6172 616d 7329 0a0a 2020  none(params)..  
+000308f0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+00030900: 6974 2073 656c 662e 6765 7428 7572 6c2c  it self.get(url,
+00030910: 2070 6172 616d 733d 7061 7261 6d73 290a   params=params).
+00030920: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00030930: 6164 645f 7669 7369 746f 7228 0a20 2020  add_visitor(.   
+00030940: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00030950: 2020 2070 6f72 7461 6c5f 6964 3a20 7374     portal_id: st
+00030960: 722c 0a20 2020 2020 2020 206e 616d 653a  r,.        name:
+00030970: 2073 7472 2c0a 2020 2020 2020 2020 2320   str,.        # 
+00030980: 6964 3a20 7374 722c 0a20 2020 2020 2020  id: str,.       
+00030990: 2070 6173 7377 6f72 643a 2073 7472 203d   password: str =
+000309a0: 204e 6f6e 652c 0a20 2020 2020 2020 202a   None,.        *
+000309b0: 2c0a 2020 2020 2020 2020 636f 6d70 616e  ,.        compan
+000309c0: 795f 6e61 6d65 3a20 7374 7220 3d20 4e6f  y_name: str = No
+000309d0: 6e65 2c0a 2020 2020 2020 2020 7068 6f6e  ne,.        phon
+000309e0: 653a 2073 7472 207c 204e 6f6e 6520 3d20  e: str | None = 
+000309f0: 4e6f 6e65 2c0a 2020 2020 2020 2020 656d  None,.        em
+00030a00: 6169 6c3a 2073 7472 207c 204e 6f6e 6520  ail: str | None 
+00030a10: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00030a20: 7661 6c69 645f 666f 7265 7665 723a 2062  valid_forever: b
+00030a30: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+00030a40: 2020 2020 2076 616c 6964 5f64 6179 733a       valid_days:
+00030a50: 2069 6e74 203d 2033 2c0a 2020 2020 2020   int = 3,.      
+00030a60: 2020 7661 6c69 645f 686f 7572 733a 2069    valid_hours: i
+00030a70: 6e74 203d 2030 2c0a 2020 2020 2020 2020  nt = 0,.        
+00030a80: 7661 6c69 645f 6d69 6e75 7465 733a 2069  valid_minutes: i
+00030a90: 6e74 203d 2030 2c0a 2020 2020 2020 2020  nt = 0,.        
+00030aa0: 6e6f 7469 6679 3a20 626f 6f6c 207c 204e  notify: bool | N
+00030ab0: 6f6e 6520 3d20 4e6f 6e65 2c0a 2020 2020  one = None,.    
+00030ac0: 2020 2020 6e6f 7469 6679 5f74 6f3a 2063      notify_to: c
+00030ad0: 6f6e 7374 616e 7473 2e4e 6f74 6966 7954  onstants.NotifyT
+00030ae0: 6f41 7267 7320 7c20 4e6f 6e65 203d 204e  oArgs | None = N
+00030af0: 6f6e 652c 0a20 2020 2020 2020 2069 735f  one,.        is_
+00030b00: 656e 6162 6c65 643a 2062 6f6f 6c20 3d20  enabled: bool = 
+00030b10: 5472 7565 2c0a 2020 2020 2020 2020 2320  True,.        # 
+00030b20: 7374 6174 7573 3a20 626f 6f6c 2c0a 2020  status: bool,.  
+00030b30: 2020 2020 2020 2320 6372 6561 7465 645f        # created_
+00030b40: 6174 3a20 7374 722c 0a20 2020 2020 2020  at: str,.       
+00030b50: 2023 2065 7870 6972 655f 6174 3a20 7374   # expire_at: st
+00030b60: 722c 0a20 2020 2029 202d 3e20 5265 7370  r,.    ) -> Resp
+00030b70: 6f6e 7365 3a0a 2020 2020 2020 2020 2222  onse:.        ""
+00030b80: 2243 7265 6174 6520 6120 6e65 7720 6775  "Create a new gu
+00030b90: 6573 7420 7669 7369 746f 7220 6f66 2061  est visitor of a
+00030ba0: 2070 6f72 7461 6c2e 0a0a 2020 2020 2020   portal...      
+00030bb0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00030bc0: 2020 2020 706f 7274 616c 5f69 6420 2873      portal_id (s
+00030bd0: 7472 293a 2050 6f72 7461 6c20 4944 206f  tr): Portal ID o
+00030be0: 6620 7468 6520 7370 6c61 7368 2070 6167  f the splash pag
+00030bf0: 650a 2020 2020 2020 2020 2020 2020 6e61  e.            na
+00030c00: 6d65 2028 7374 7229 3a20 5669 7369 746f  me (str): Visito
+00030c10: 7220 6163 636f 756e 7420 6e61 6d65 0a20  r account name. 
+00030c20: 2020 2020 2020 2020 2020 2070 6173 7377             passw
+00030c30: 6f72 6420 2873 7472 293a 2050 6173 7377  ord (str): Passw
+00030c40: 6f72 640a 2020 2020 2020 2020 2020 2020  ord.            
+00030c50: 636f 6d70 616e 795f 6e61 6d65 2028 7374  company_name (st
+00030c60: 7229 3a20 436f 6d70 616e 7920 6e61 6d65  r): Company name
+00030c70: 206f 6620 7468 6520 7669 7369 746f 720a   of the visitor.
+00030c80: 2020 2020 2020 2020 2020 2020 7068 6f6e              phon
+00030c90: 6520 2873 7472 293a 2050 686f 6e65 206e  e (str): Phone n
+00030ca0: 756d 6265 7220 6f66 2074 6865 2076 6973  umber of the vis
+00030cb0: 6974 6f72 3b20 466f 726d 6174 205b 2b43  itor; Format [+C
+00030cc0: 6f75 6e74 7279 436f 6465 5d5b 5068 6f6e  ountryCode][Phon
+00030cd0: 654e 756d 6265 725d 0a20 2020 2020 2020  eNumber].       
+00030ce0: 2020 2020 2065 6d61 696c 2028 7374 7229       email (str)
+00030cf0: 3a20 456d 6169 6c20 6164 6472 6573 7320  : Email address 
+00030d00: 6f66 2074 6865 2076 6973 6974 6f72 0a20  of the visitor. 
+00030d10: 2020 2020 2020 2020 2020 2076 616c 6964             valid
+00030d20: 5f66 6f72 6576 6572 2028 626f 6f6c 293a  _forever (bool):
+00030d30: 2056 6973 6974 6f72 2061 6363 6f75 6e74   Visitor account
+00030d40: 2077 696c 6c20 6e6f 7420 6578 7069 7265   will not expire
+00030d50: 2077 6865 6e20 7468 6973 2069 7320 7365   when this is se
+00030d60: 7420 746f 2074 7275 650a 2020 2020 2020  t to true.      
+00030d70: 2020 2020 2020 7661 6c69 645f 6461 7973        valid_days
+00030d80: 2028 696e 7429 3a20 4163 636f 756e 7420   (int): Account 
+00030d90: 7661 6c69 6469 7479 2069 6e20 6461 7973  validity in days
+00030da0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00030db0: 6964 5f68 6f75 7273 2028 696e 7429 3a20  id_hours (int): 
+00030dc0: 4163 636f 756e 7420 7661 6c69 6469 7479  Account validity
+00030dd0: 2069 6e20 686f 7572 730a 2020 2020 2020   in hours.      
+00030de0: 2020 2020 2020 7661 6c69 645f 6d69 6e75        valid_minu
+00030df0: 7465 7320 2869 6e74 293a 2041 6363 6f75  tes (int): Accou
+00030e00: 6e74 2076 616c 6964 6974 7920 696e 206d  nt validity in m
+00030e10: 696e 7574 6573 0a20 2020 2020 2020 2020  inutes.         
+00030e20: 2020 206e 6f74 6966 7920 2862 6f6f 6c29     notify (bool)
+00030e30: 3a20 466c 6167 2074 6f20 6e6f 7469 6679  : Flag to notify
+00030e40: 2074 6865 2070 6173 7377 6f72 6420 7669   the password vi
+00030e50: 6120 656d 6169 6c20 6f72 206e 756d 6265  a email or numbe
+00030e60: 720a 2020 2020 2020 2020 2020 2020 6e6f  r.            no
+00030e70: 7469 6679 5f74 6f20 2873 7472 293a 204e  tify_to (str): N
+00030e80: 6f74 6966 7920 746f 2065 6d61 696c 206f  otify to email o
+00030e90: 7220 7068 6f6e 652e 2044 6566 7561 6c74  r phone. Defualt
+00030ea0: 2069 7320 7068 6f6e 6520 7768 656e 2069   is phone when i
+00030eb0: 7420 6973 2070 726f 7669 6465 640a 2020  t is provided.  
+00030ec0: 2020 2020 2020 2020 2020 2020 2020 6f74                ot
+00030ed0: 6865 7277 6973 6520 656d 6169 6c2e 2020  herwise email.  
+00030ee0: 5661 6c69 6420 5661 6c75 6573 3a20 656d  Valid Values: em
+00030ef0: 6169 6c2c 2070 686f 6e65 0a20 2020 2020  ail, phone.     
+00030f00: 2020 2020 2020 2069 735f 656e 6162 6c65         is_enable
+00030f10: 6420 2862 6f6f 6c29 3a20 456e 6162 6c65  d (bool): Enable
+00030f20: 206f 7220 6469 7361 626c 6520 7468 6520   or disable the 
+00030f30: 7669 7369 746f 7220 6163 636f 756e 740a  visitor account.
+00030f40: 2020 2020 2020 2020 2020 2020 2320 6964              # id
+00030f50: 2028 7374 7229 3a20 4e41 2066 6f72 2076   (str): NA for v
+00030f60: 6973 6974 6f72 2070 6f73 742f 7075 7420  isitor post/put 
+00030f70: 6d65 7468 6f64 2e20 4944 206f 6620 7468  method. ID of th
+00030f80: 6520 7669 7369 746f 720a 2020 2020 2020  e visitor.      
+00030f90: 2020 2020 2020 2320 7374 6174 7573 2028        # status (
+00030fa0: 626f 6f6c 293a 2054 6869 7320 6669 656c  bool): This fiel
+00030fb0: 6420 7072 6f76 6964 6573 2073 7461 7475  d provides statu
+00030fc0: 7320 6f66 2074 6865 2061 6363 6f75 6e74  s of the account
+00030fd0: 2e20 5265 7475 726e 7320 7472 7565 2077  . Returns true w
+00030fe0: 6865 6e20 656e 6162 6c65 6420 616e 640a  hen enabled and.
+00030ff0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00031000: 2020 6e6f 7420 6578 7069 7265 642e 204e    not expired. N
+00031010: 4120 666f 7220 7669 7369 746f 7220 706f  A for visitor po
+00031020: 7374 2f70 7574 206d 6574 686f 642e 2054  st/put method. T
+00031030: 6869 7320 6973 206f 7074 696f 6e61 6c20  his is optional 
+00031040: 6669 656c 6473 2e0a 2020 2020 2020 2020  fields..        
+00031050: 2020 2020 2320 6372 6561 7465 645f 6174      # created_at
+00031060: 2028 7374 7229 3a20 5468 6973 2066 6965   (str): This fie
+00031070: 6c64 2069 6e64 6963 6174 6573 2074 6865  ld indicates the
+00031080: 2063 7265 6174 6564 2064 6174 6520 7469   created date ti
+00031090: 6d65 7374 616d 7020 7661 6c75 652e 2049  mestamp value. I
+000310a0: 7420 6973 2067 656e 6572 6174 6564 0a20  t is generated. 
+000310b0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+000310c0: 2077 6869 6c65 2063 7265 6174 696e 6720   while creating 
+000310d0: 7669 7369 746f 722e 204e 4120 666f 7220  visitor. NA for 
+000310e0: 7669 7369 746f 7220 706f 7374 2f70 7574  visitor post/put
+000310f0: 206d 6574 686f 642e 2054 6869 7320 6973   method. This is
+00031100: 206f 7074 696f 6e61 6c20 6669 656c 642e   optional field.
+00031110: 0a20 2020 2020 2020 2020 2020 2023 2065  .            # e
+00031120: 7870 6972 655f 6174 2028 7374 7229 3a20  xpire_at (str): 
+00031130: 5468 6973 2066 6965 6c64 2069 6e64 6963  This field indic
+00031140: 6174 6573 2065 7870 6972 7920 7469 6d65  ates expiry time
+00031150: 2074 696d 6573 7461 6d70 2076 616c 7565   timestamp value
+00031160: 2e20 4974 2069 7320 6765 6e65 7261 7465  . It is generate
+00031170: 6420 6261 7365 640a 2020 2020 2020 2020  d based.        
+00031180: 2020 2020 2320 2020 2020 6f6e 2074 6865      #     on the
+00031190: 2076 616c 6964 5f74 696c 6c20 7661 6c75   valid_till valu
+000311a0: 6520 616e 6420 6372 6561 7465 645f 6174  e and created_at
+000311b0: 2074 696d 652e 204e 4120 666f 7220 7669   time. NA for vi
+000311c0: 7369 746f 7220 706f 7374 2f70 7574 206d  sitor post/put m
+000311d0: 6574 686f 642e 2054 6869 7320 6973 0a20  ethod. This is. 
+000311e0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+000311f0: 206f 7074 696f 6e61 6c20 6669 656c 640a   optional field.
+00031200: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00031210: 3a0a 2020 2020 2020 2020 2020 2020 5265  :.            Re
+00031220: 7370 6f6e 7365 3a20 4365 6e74 7261 6c41  sponse: CentralA
+00031230: 5049 2052 6573 706f 6e73 6520 6f62 6a65  PI Response obje
+00031240: 6374 0a20 2020 2020 2020 2022 2222 0a20  ct.        """. 
+00031250: 2020 2020 2020 2075 726c 203d 2066 222f         url = f"/
+00031260: 6775 6573 742f 7631 2f70 6f72 7461 6c73  guest/v1/portals
+00031270: 2f7b 706f 7274 616c 5f69 647d 2f76 6973  /{portal_id}/vis
+00031280: 6974 6f72 7322 0a0a 2020 2020 2020 2020  itors"..        
+00031290: 7573 6572 5f64 6174 6120 3d20 7b0a 2020  user_data = {.  
+000312a0: 2020 2020 2020 2020 2020 2770 686f 6e65            'phone
+000312b0: 273a 2070 686f 6e65 2c0a 2020 2020 2020  ': phone,.      
+000312c0: 2020 2020 2020 2765 6d61 696c 273a 2065        'email': e
+000312d0: 6d61 696c 0a20 2020 2020 2020 207d 0a20  mail.        }. 
+000312e0: 2020 2020 2020 2023 2041 5049 2072 6571         # API req
+000312f0: 7569 7265 7320 7068 6f6e 6520 616e 6420  uires phone and 
+00031300: 656d 6169 6c2c 2062 7574 2061 6c6c 6f77  email, but allow
+00031310: 7320 4e6f 6e65 2f6e 756c 6c20 6173 2076  s None/null as v
+00031320: 616c 7565 2064 6570 656e 6469 6e67 206f  alue depending o
+00031330: 6e20 686f 7720 706f 7274 616c 2069 7320  n how portal is 
+00031340: 636f 6e66 6967 7572 6564 0a20 2020 2020  configured.     
+00031350: 2020 2023 2075 7365 725f 6461 7461 203d     # user_data =
+00031360: 2075 7469 6c73 2e73 7472 6970 5f6e 6f6e   utils.strip_non
+00031370: 6528 7573 6572 5f64 6174 6129 0a0a 2020  e(user_data)..  
+00031380: 2020 2020 2020 6a73 6f6e 5f64 6174 6120        json_data 
+00031390: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+000313a0: 276e 616d 6527 3a20 6e61 6d65 2c0a 2020  'name': name,.  
+000313b0: 2020 2020 2020 2020 2020 2763 6f6d 7061            'compa
+000313c0: 6e79 5f6e 616d 6527 3a20 636f 6d70 616e  ny_name': compan
+000313d0: 795f 6e61 6d65 2c0a 2020 2020 2020 2020  y_name,.        
+000313e0: 2020 2020 2769 735f 656e 6162 6c65 6427      'is_enabled'
+000313f0: 3a20 6973 5f65 6e61 626c 6564 2c0a 2020  : is_enabled,.  
+00031400: 2020 2020 2020 2020 2020 2776 616c 6964            'valid
+00031410: 5f74 696c 6c5f 6e6f 5f6c 696d 6974 273a  _till_no_limit':
+00031420: 2076 616c 6964 5f66 6f72 6576 6572 2c0a   valid_forever,.
+00031430: 2020 2020 2020 2020 2020 2020 2776 616c              'val
+00031440: 6964 5f74 696c 6c5f 6461 7973 273a 2076  id_till_days': v
+00031450: 616c 6964 5f64 6179 732c 0a20 2020 2020  alid_days,.     
+00031460: 2020 2020 2020 2027 7661 6c69 645f 7469         'valid_ti
+00031470: 6c6c 5f68 6f75 7273 273a 2076 616c 6964  ll_hours': valid
+00031480: 5f68 6f75 7273 2c0a 2020 2020 2020 2020  _hours,.        
+00031490: 2020 2020 2776 616c 6964 5f74 696c 6c5f      'valid_till_
+000314a0: 6d69 6e75 7465 7327 3a20 7661 6c69 645f  minutes': valid_
+000314b0: 6d69 6e75 7465 732c 0a20 2020 2020 2020  minutes,.       
+000314c0: 2020 2020 2027 6e6f 7469 6679 273a 206e       'notify': n
+000314d0: 6f74 6966 792c 0a20 2020 2020 2020 2020  otify,.         
+000314e0: 2020 2027 6e6f 7469 6679 5f74 6f27 3a20     'notify_to': 
+000314f0: 6e6f 7469 6679 5f74 6f2c 0a20 2020 2020  notify_to,.     
+00031500: 2020 2020 2020 2027 7061 7373 776f 7264         'password
+00031510: 273a 2070 6173 7377 6f72 640a 2020 2020  ': password.    
+00031520: 2020 2020 7d0a 2020 2020 2020 2020 6a73      }.        js
+00031530: 6f6e 5f64 6174 6120 3d20 7574 696c 732e  on_data = utils.
+00031540: 7374 7269 705f 6e6f 6e65 286a 736f 6e5f  strip_none(json_
+00031550: 6461 7461 290a 2020 2020 2020 2020 6966  data).        if
+00031560: 2075 7365 725f 6461 7461 3a0a 2020 2020   user_data:.    
+00031570: 2020 2020 2020 2020 6a73 6f6e 5f64 6174          json_dat
+00031580: 615b 2275 7365 7222 5d20 3d20 7573 6572  a["user"] = user
+00031590: 5f64 6174 610a 0a20 2020 2020 2020 2072  _data..        r
+000315a0: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+000315b0: 2e70 6f73 7428 7572 6c2c 206a 736f 6e5f  .post(url, json_
+000315c0: 6461 7461 3d6a 736f 6e5f 6461 7461 290a  data=json_data).
+000315d0: 0a20 2020 2023 2054 4f44 4f20 7661 6c69  .    # TODO vali
+000315e0: 6461 7465 2049 5020 6164 6472 6573 7320  date IP address 
+000315f0: 666f 726d 6174 0a20 2020 2061 7379 6e63  format.    async
+00031600: 2064 6566 2075 7064 6174 655f 6378 5f70   def update_cx_p
+00031610: 726f 7065 7274 6965 7328 0a20 2020 2020  roperties(.     
+00031620: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00031630: 202a 2c0a 2020 2020 2020 2020 7365 7269   *,.        seri
+00031640: 616c 3a20 7374 7220 3d20 4e6f 6e65 2c0a  al: str = None,.
+00031650: 2020 2020 2020 2020 6772 6f75 703a 2073          group: s
+00031660: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+00031670: 2020 206e 616d 653a 2073 7472 203d 204e     name: str = N
+00031680: 6f6e 652c 0a20 2020 2020 2020 2063 6f6e  one,.        con
+00031690: 7461 6374 3a20 7374 7220 3d20 4e6f 6e65  tact: str = None
+000316a0: 2c0a 2020 2020 2020 2020 6c6f 6361 7469  ,.        locati
+000316b0: 6f6e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  on: str = None,.
+000316c0: 2020 2020 2020 2020 7469 6d65 7a6f 6e65          timezone
+000316d0: 3a20 636f 6e73 7461 6e74 732e 545a 4442  : constants.TZDB
+000316e0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000316f0: 206d 676d 745f 7672 663a 2062 6f6f 6c20   mgmt_vrf: bool 
+00031700: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00031710: 646e 735f 7365 7276 6572 733a 204c 6973  dns_servers: Lis
+00031720: 745b 7374 725d 203d 205b 5d2c 0a20 2020  t[str] = [],.   
+00031730: 2020 2020 206e 7470 5f73 6572 7665 7273       ntp_servers
+00031740: 3a20 4c69 7374 5b73 7472 5d20 3d20 5b5d  : List[str] = []
+00031750: 2c0a 2020 2020 2020 2020 6164 6d69 6e5f  ,.        admin_
+00031760: 7573 6572 3a20 7374 7220 3d20 4e6f 6e65  user: str = None
+00031770: 2c0a 2020 2020 2020 2020 6164 6d69 6e5f  ,.        admin_
+00031780: 7061 7373 3a20 7374 7220 3d20 4e6f 6e65  pass: str = None
+00031790: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
+000317a0: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
+000317b0: 5570 6461 7465 2050 726f 7065 7274 6965  Update Propertie
+000317c0: 7320 2841 7275 6261 4f53 2d43 5829 2e0a  s (ArubaOS-CX)..
+000317d0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+000317e0: 2020 2020 2020 2020 2020 2073 6572 6961             seria
+000317f0: 6c20 2873 7472 2c20 6f70 7469 6f6e 616c  l (str, optional
+00031800: 293a 2044 6576 6963 6520 7365 7269 616c  ): Device serial
+00031810: 206e 756d 6265 722e 0a20 2020 2020 2020   number..       
+00031820: 2020 2020 2020 2020 204d 616e 6461 746f           Mandato
+00031830: 7279 2066 6f72 2064 6576 6963 6520 6c65  ry for device le
+00031840: 7665 6c20 636f 6e66 6967 7572 6174 696f  vel configuratio
+00031850: 6e2e 0a20 2020 2020 2020 2020 2020 2020  n..             
+00031860: 2020 2031 2061 6e64 206f 6e6c 7920 3120     1 and only 1 
+00031870: 6f66 2073 6572 6961 6c20 6f72 2067 726f  of serial or gro
+00031880: 7570 2061 7265 2072 6571 7569 7265 640a  up are required.
+00031890: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
+000318a0: 7020 2873 7472 2c20 6f70 7469 6f6e 616c  p (str, optional
+000318b0: 293a 2047 726f 7570 206e 616d 652e 0a20  ): Group name.. 
+000318c0: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+000318d0: 616e 6461 746f 7279 2066 6f72 2067 726f  andatory for gro
+000318e0: 7570 206c 6576 656c 2063 6f6e 6669 6775  up level configu
+000318f0: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
+00031900: 2020 2020 2020 2020 3120 616e 6420 6f6e          1 and on
+00031910: 6c79 2031 206f 6620 7365 7269 616c 206f  ly 1 of serial o
+00031920: 7220 6772 6f75 7020 6172 6520 7265 7175  r group are requ
+00031930: 6972 6564 0a20 2020 2020 2020 2020 2020  ired.           
+00031940: 206e 616d 6520 2873 7472 293a 204f 6e6c   name (str): Onl
+00031950: 7920 636f 6e66 6967 7572 6162 6c65 2061  y configurable a
+00031960: 7420 6465 7669 6365 2d6c 6576 656c 2e0a  t device-level..
+00031970: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00031980: 6163 7420 2873 7472 293a 2050 6174 7465  act (str): Patte
+00031990: 726e 3a20 225e 5b5e 223f 5d2a 2422 0a20  rn: "^[^"?]*$". 
+000319a0: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
+000319b0: 696f 6e20 2873 7472 293a 2050 6174 7465  ion (str): Patte
+000319c0: 726e 3a20 225e 5b5e 223f 5d2a 2422 0a20  rn: "^[^"?]*$". 
+000319d0: 2020 2020 2020 2020 2020 2074 696d 657a             timez
+000319e0: 6f6e 6520 2873 7472 293a 2074 696d 657a  one (str): timez
+000319f0: 6f6e 6520 2056 616c 6964 2056 616c 7565  one  Valid Value
+00031a00: 733a 2075 7365 2074 7a20 6461 7461 6261  s: use tz databa
+00031a10: 7365 2066 6f72 6d61 7420 6c69 6b65 2022  se format like "
+00031a20: 416d 6572 6963 612f 4368 6963 6167 6f22  America/Chicago"
+00031a30: 0a20 2020 2020 2020 2020 2020 206d 676d  .            mgm
+00031a40: 745f 7672 6620 2862 6f6f 6c29 3a20 5573  t_vrf (bool): Us
+00031a50: 6520 6d67 6d74 2056 5246 2c20 696e 6469  e mgmt VRF, indi
+00031a60: 6361 7465 7320 5652 4620 666f 7220 646e  cates VRF for dn
+00031a70: 735f 7365 7276 6572 7320 616e 6420 6e74  s_servers and nt
+00031a80: 705f 7365 7276 6572 732c 2069 6620 4661  p_servers, if Fa
+00031a90: 6c73 6520 6f72 206e 6f74 2070 726f 7669  lse or not provi
+00031aa0: 6465 6420 6465 6661 756c 7420 5652 4620  ded default VRF 
+00031ab0: 6973 2075 7365 642e 0a20 2020 2020 2020  is used..       
+00031ac0: 2020 2020 2064 6e73 5f73 6572 7665 7273       dns_servers
+00031ad0: 2028 4c69 7374 5b73 7472 5d29 3a20 6970   (List[str]): ip
+00031ae0: 7634 2f69 7076 3620 6164 6472 6573 730a  v4/ipv6 address.
+00031af0: 2020 2020 2020 2020 2020 2020 6e74 705f              ntp_
+00031b00: 7365 7276 6572 7320 284c 6973 745b 7374  servers (List[st
+00031b10: 725d 293a 2069 7076 342f 6970 7636 2061  r]): ipv4/ipv6 a
+00031b20: 6464 7265 7373 0a20 2020 2020 2020 2020  ddress.         
+00031b30: 2020 2061 646d 696e 5f75 7365 7220 2873     admin_user (s
+00031b40: 7472 293a 206c 6f63 616c 2061 646d 696e  tr): local admin
+00031b50: 2075 7365 720a 2020 2020 2020 2020 2020   user.          
+00031b60: 2020 6164 6d69 6e5f 7061 7373 2028 7374    admin_pass (st
+00031b70: 7229 3a20 6c6f 6361 6c20 6164 6d69 6e20  r): local admin 
+00031b80: 7061 7373 776f 7264 0a0a 2020 2020 2020  password..      
+00031b90: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00031ba0: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
+00031bb0: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
+00031bc0: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
+00031bd0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00031be0: 7572 6c20 3d20 222f 636f 6e66 6967 7572  url = "/configur
+00031bf0: 6174 696f 6e2f 7631 2f73 7769 7463 682f  ation/v1/switch/
+00031c00: 6378 2f70 726f 7065 7274 6965 7322 0a0a  cx/properties"..
+00031c10: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
+00031c20: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
+00031c30: 6465 7669 6365 5f73 6572 6961 6c27 3a20  device_serial': 
+00031c40: 7365 7269 616c 2c0a 2020 2020 2020 2020  serial,.        
+00031c50: 2020 2020 2767 726f 7570 5f6e 616d 6527      'group_name'
+00031c60: 3a20 6772 6f75 700a 2020 2020 2020 2020  : group.        
+00031c70: 7d0a 0a20 2020 2020 2020 206a 736f 6e5f  }..        json_
+00031c80: 6461 7461 203d 207b 0a20 2020 2020 2020  data = {.       
+00031c90: 2020 2020 2027 6e61 6d65 273a 206e 616d       'name': nam
+00031ca0: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
+00031cb0: 636f 6e74 6163 7427 3a20 636f 6e74 6163  contact': contac
+00031cc0: 742c 0a20 2020 2020 2020 2020 2020 2027  t,.            '
+00031cd0: 6c6f 6361 7469 6f6e 273a 206c 6f63 6174  location': locat
+00031ce0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00031cf0: 2027 7469 6d65 7a6f 6e65 273a 2074 696d   'timezone': tim
+00031d00: 657a 6f6e 652c 0a20 2020 2020 2020 2020  ezone,.         
+00031d10: 2020 2027 646e 735f 7365 7276 6572 7327     'dns_servers'
+00031d20: 3a20 646e 735f 7365 7276 6572 732c 0a20  : dns_servers,. 
+00031d30: 2020 2020 2020 2020 2020 2027 6e74 705f             'ntp_
+00031d40: 7365 7276 6572 7327 3a20 6e74 705f 7365  servers': ntp_se
+00031d50: 7276 6572 732c 0a20 2020 2020 2020 2020  rvers,.         
+00031d60: 2020 2027 6164 6d69 6e5f 7573 6572 6e61     'admin_userna
+00031d70: 6d65 273a 2061 646d 696e 5f75 7365 722c  me': admin_user,
+00031d80: 0a20 2020 2020 2020 2020 2020 2027 6164  .            'ad
+00031d90: 6d69 6e5f 7061 7373 776f 7264 273a 2061  min_password': a
+00031da0: 646d 696e 5f70 6173 730a 2020 2020 2020  dmin_pass.      
+00031db0: 2020 7d0a 2020 2020 2020 2020 6966 206d    }.        if m
+00031dc0: 676d 745f 7672 6620 6973 206e 6f74 204e  gmt_vrf is not N
+00031dd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00031de0: 206a 736f 6e5f 6461 7461 5b22 7672 6622   json_data["vrf"
+00031df0: 5d20 3d20 226d 676d 7422 2069 6620 6d67  ] = "mgmt" if mg
+00031e00: 6d74 5f76 7266 2065 6c73 6520 2264 6566  mt_vrf else "def
+00031e10: 6175 6c74 220a 2020 2020 2020 2020 656c  ault".        el
+00031e20: 6966 2064 6e73 5f73 6572 7665 7273 206f  if dns_servers o
+00031e30: 7220 6e74 705f 7365 7276 6572 733a 0a20  r ntp_servers:. 
+00031e40: 2020 2020 2020 2020 2020 206a 736f 6e5f             json_
+00031e50: 6461 7461 5b22 7672 6622 5d20 3d20 2264  data["vrf"] = "d
+00031e60: 6566 6175 6c74 220a 0a20 2020 2020 2020  efault"..       
+00031e70: 2069 6620 6c65 6e28 5b78 2066 6f72 2078   if len([x for x
+00031e80: 2069 6e20 5b61 646d 696e 5f75 7365 722c   in [admin_user,
+00031e90: 2061 646d 696e 5f70 6173 735d 2069 6620   admin_pass] if 
+00031ea0: 7820 6973 206e 6f74 204e 6f6e 655d 2920  x is not None]) 
+00031eb0: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
+00031ec0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00031ed0: 6f72 2822 4966 2065 6974 6865 7220 6164  or("If either ad
+00031ee0: 6d69 6e5f 7573 6572 206f 7220 6164 6d69  min_user or admi
+00031ef0: 6e5f 7061 7373 2061 7265 2062 696e 6720  n_pass are bing 
+00031f00: 7570 6461 7465 642c 202a 626f 7468 2a20  updated, *both* 
+00031f10: 7368 6f75 6c64 2062 6520 7072 6f76 6964  should be provid
+00031f20: 6564 2e22 290a 0a20 2020 2020 2020 2069  ed.")..        i
+00031f30: 6620 6c65 6e28 5b78 2066 6f72 2078 2069  f len([x for x i
+00031f40: 6e20 5b73 6572 6961 6c2c 2067 726f 7570  n [serial, group
+00031f50: 5d20 6966 2078 2069 7320 6e6f 7420 4e6f  ] if x is not No
+00031f60: 6e65 5d29 203d 3d20 323a 0a20 2020 2020  ne]) == 2:.     
+00031f70: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00031f80: 7565 4572 726f 7228 2270 726f 7669 6465  ueError("provide
+00031f90: 2073 6572 6961 6c20 746f 2075 7064 6174   serial to updat
+00031fa0: 6520 6465 7669 6365 206c 6576 656c 2070  e device level p
+00031fb0: 726f 7065 7274 6965 732c 206f 7220 6772  roperties, or gr
+00031fc0: 6f75 7020 746f 2075 7064 6174 6520 6174  oup to update at
+00031fd0: 2074 6865 2067 726f 7570 206c 6576 656c   the group level
+00031fe0: 2e20 2050 726f 7669 6469 6e67 2062 6f74  .  Providing bot
+00031ff0: 6820 6973 2069 6e76 616c 6964 2e22 290a  h is invalid.").
+00032000: 0a20 2020 2020 2020 206a 736f 6e5f 6461  .        json_da
+00032010: 7461 203d 2075 7469 6c73 2e73 7472 6970  ta = utils.strip
+00032020: 5f6e 6f6e 6528 6a73 6f6e 5f64 6174 612c  _none(json_data,
+00032030: 2073 7472 6970 5f65 6d70 7479 5f6f 626a   strip_empty_obj
+00032040: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
+00032050: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+00032060: 662e 706f 7374 2875 726c 2c20 6a73 6f6e  f.post(url, json
+00032070: 5f64 6174 613d 6a73 6f6e 5f64 6174 612c  _data=json_data,
+00032080: 2070 6172 616d 733d 7061 7261 6d73 290a   params=params).
+00032090: 0a20 2020 2061 7379 6e63 2064 6566 2067  .    async def g
+000320a0: 6574 5f6f 7370 665f 6172 6561 280a 2020  et_ospf_area(.  
+000320b0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000320c0: 2020 2020 6465 7669 6365 3a20 7374 722c      device: str,
+000320d0: 0a20 2020 2020 2020 206d 6172 6b65 723a  .        marker:
+000320e0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000320f0: 2020 2020 206c 696d 6974 3a20 696e 7420       limit: int 
+00032100: 3d20 3130 302c 0a20 2020 2029 202d 3e20  = 100,.    ) -> 
+00032110: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
+00032120: 2020 2222 224c 6973 7420 4f53 5046 2041    """List OSPF A
+00032130: 7265 6120 496e 666f 726d 6174 696f 6e2e  rea Information.
+00032140: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00032150: 2020 2020 2020 2020 2020 2020 6465 7669              devi
+00032160: 6365 2028 7374 7229 3a20 4465 7669 6365  ce (str): Device
+00032170: 2073 6572 6961 6c20 6e75 6d62 6572 0a20   serial number. 
+00032180: 2020 2020 2020 2020 2020 206d 6172 6b65             marke
+00032190: 7220 2873 7472 2c20 6f70 7469 6f6e 616c  r (str, optional
+000321a0: 293a 204f 7061 7175 6520 6861 6e64 6c65  ): Opaque handle
+000321b0: 2074 6f20 6665 7463 6820 6e65 7874 2070   to fetch next p
+000321c0: 6167 650a 2020 2020 2020 2020 2020 2020  age.            
+000321d0: 6c69 6d69 7420 2869 6e74 2c20 6f70 7469  limit (int, opti
+000321e0: 6f6e 616c 293a 2070 6167 6520 7369 7a65  onal): page size
+000321f0: 2044 6566 6175 6c74 7320 746f 2031 3030   Defaults to 100
+00032200: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00032210: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00032220: 5265 7370 6f6e 7365 3a20 4365 6e74 7261  Response: Centra
+00032230: 6c41 5049 2052 6573 706f 6e73 6520 6f62  lAPI Response ob
+00032240: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
+00032250: 0a20 2020 2020 2020 2075 726c 203d 2022  .        url = "
+00032260: 2f61 7069 2f72 6f75 7469 6e67 2f76 312f  /api/routing/v1/
+00032270: 6f73 7066 2f61 7265 6122 0a0a 2020 2020  ospf/area"..    
+00032280: 2020 2020 7061 7261 6d73 203d 207b 0a20      params = {. 
+00032290: 2020 2020 2020 2020 2020 2027 6465 7669             'devi
+000322a0: 6365 273a 2064 6576 6963 652c 0a20 2020  ce': device,.   
+000322b0: 2020 2020 2020 2020 2027 6d61 726b 6572           'marker
+000322c0: 273a 206d 6172 6b65 722c 0a20 2020 2020  ': marker,.     
+000322d0: 2020 2020 2020 2027 6c69 6d69 7427 3a20         'limit': 
+000322e0: 6c69 6d69 740a 2020 2020 2020 2020 7d0a  limit.        }.
+000322f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00032300: 6177 6169 7420 7365 6c66 2e67 6574 2875  await self.get(u
+00032310: 726c 2c20 7061 7261 6d73 3d70 6172 616d  rl, params=param
+00032320: 7329 0a0a 2020 2020 6173 796e 6320 6465  s)..    async de
+00032330: 6620 6765 745f 6f73 7066 5f69 6e74 6572  f get_ospf_inter
+00032340: 6661 6365 280a 2020 2020 2020 2020 7365  face(.        se
+00032350: 6c66 2c0a 2020 2020 2020 2020 6465 7669  lf,.        devi
+00032360: 6365 3a20 7374 722c 0a20 2020 2020 2020  ce: str,.       
+00032370: 206d 6172 6b65 723a 2073 7472 203d 204e   marker: str = N
+00032380: 6f6e 652c 0a20 2020 2020 2020 206c 696d  one,.        lim
+00032390: 6974 3a20 696e 7420 3d20 3130 302c 0a20  it: int = 100,. 
+000323a0: 2020 2029 202d 3e20 5265 7370 6f6e 7365     ) -> Response
+000323b0: 3a0a 2020 2020 2020 2020 2222 224c 6973  :.        """Lis
+000323c0: 7420 4f53 5046 2049 6e74 6572 6661 6365  t OSPF Interface
+000323d0: 2049 6e66 6f72 6d61 7469 6f6e 2e0a 0a20   Information... 
+000323e0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+000323f0: 2020 2020 2020 2020 2064 6576 6963 6520           device 
+00032400: 2873 7472 293a 2044 6576 6963 6520 7365  (str): Device se
+00032410: 7269 616c 206e 756d 6265 720a 2020 2020  rial number.    
+00032420: 2020 2020 2020 2020 6d61 726b 6572 2028          marker (
+00032430: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+00032440: 4f70 6171 7565 2068 616e 646c 6520 746f  Opaque handle to
+00032450: 2066 6574 6368 206e 6578 7420 7061 6765   fetch next page
+00032460: 0a20 2020 2020 2020 2020 2020 206c 696d  .            lim
+00032470: 6974 2028 696e 742c 206f 7074 696f 6e61  it (int, optiona
+00032480: 6c29 3a20 7061 6765 2073 697a 6520 4465  l): page size De
+00032490: 6661 756c 7473 2074 6f20 3130 302e 0a0a  faults to 100...
+000324a0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+000324b0: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
+000324c0: 706f 6e73 653a 2043 656e 7472 616c 4150  ponse: CentralAP
+000324d0: 4920 5265 7370 6f6e 7365 206f 626a 6563  I Response objec
+000324e0: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
+000324f0: 2020 2020 2020 7572 6c20 3d20 222f 6170        url = "/ap
+00032500: 692f 726f 7574 696e 672f 7631 2f6f 7370  i/routing/v1/osp
+00032510: 662f 696e 7465 7266 6163 6522 0a0a 2020  f/interface"..  
+00032520: 2020 2020 2020 7061 7261 6d73 203d 207b        params = {
+00032530: 0a20 2020 2020 2020 2020 2020 2027 6465  .            'de
+00032540: 7669 6365 273a 2064 6576 6963 652c 0a20  vice': device,. 
+00032550: 2020 2020 2020 2020 2020 2027 6d61 726b             'mark
+00032560: 6572 273a 206d 6172 6b65 722c 0a20 2020  er': marker,.   
+00032570: 2020 2020 2020 2020 2027 6c69 6d69 7427           'limit'
+00032580: 3a20 6c69 6d69 740a 2020 2020 2020 2020  : limit.        
+00032590: 7d0a 0a20 2020 2020 2020 2072 6574 7572  }..        retur
+000325a0: 6e20 6177 6169 7420 7365 6c66 2e67 6574  n await self.get
+000325b0: 2875 726c 2c20 7061 7261 6d73 3d70 6172  (url, params=par
+000325c0: 616d 7329 0a0a 2020 2020 6173 796e 6320  ams)..    async 
+000325d0: 6465 6620 6765 745f 6f73 7066 5f6e 6569  def get_ospf_nei
+000325e0: 6768 626f 7228 0a20 2020 2020 2020 2073  ghbor(.        s
+000325f0: 656c 662c 0a20 2020 2020 2020 2064 6576  elf,.        dev
+00032600: 6963 653a 2073 7472 2c0a 2020 2020 2020  ice: str,.      
+00032610: 2020 6d61 726b 6572 3a20 7374 7220 3d20    marker: str = 
+00032620: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c69  None,.        li
+00032630: 6d69 743a 2069 6e74 203d 2031 3030 2c0a  mit: int = 100,.
+00032640: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
+00032650: 653a 0a20 2020 2020 2020 2022 2222 4c69  e:.        """Li
+00032660: 7374 204f 5350 4620 6e65 6967 6862 6f72  st OSPF neighbor
+00032670: 2049 6e66 6f72 6d61 7469 6f6e 2e0a 0a20   Information... 
+00032680: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00032690: 2020 2020 2020 2020 2064 6576 6963 6520           device 
+000326a0: 2873 7472 293a 2044 6576 6963 6520 7365  (str): Device se
+000326b0: 7269 616c 206e 756d 6265 720a 2020 2020  rial number.    
+000326c0: 2020 2020 2020 2020 6d61 726b 6572 2028          marker (
+000326d0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+000326e0: 4f70 6171 7565 2068 616e 646c 6520 746f  Opaque handle to
+000326f0: 2066 6574 6368 206e 6578 7420 7061 6765   fetch next page
+00032700: 0a20 2020 2020 2020 2020 2020 206c 696d  .            lim
+00032710: 6974 2028 696e 742c 206f 7074 696f 6e61  it (int, optiona
+00032720: 6c29 3a20 7061 6765 2073 697a 6520 4465  l): page size De
+00032730: 6661 756c 7473 2074 6f20 3130 302e 0a0a  faults to 100...
+00032740: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00032750: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
+00032760: 706f 6e73 653a 2043 656e 7472 616c 4150  ponse: CentralAP
+00032770: 4920 5265 7370 6f6e 7365 206f 626a 6563  I Response objec
+00032780: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
+00032790: 2020 2020 2020 7572 6c20 3d20 222f 6170        url = "/ap
+000327a0: 692f 726f 7574 696e 672f 7631 2f6f 7370  i/routing/v1/osp
+000327b0: 662f 6e65 6967 6862 6f72 220a 0a20 2020  f/neighbor"..   
+000327c0: 2020 2020 2070 6172 616d 7320 3d20 7b0a       params = {.
+000327d0: 2020 2020 2020 2020 2020 2020 2764 6576              'dev
+000327e0: 6963 6527 3a20 6465 7669 6365 2c0a 2020  ice': device,.  
+000327f0: 2020 2020 2020 2020 2020 276d 6172 6b65            'marke
+00032800: 7227 3a20 6d61 726b 6572 2c0a 2020 2020  r': marker,.    
+00032810: 2020 2020 2020 2020 276c 696d 6974 273a          'limit':
+00032820: 206c 696d 6974 0a20 2020 2020 2020 207d   limit.        }
+00032830: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00032840: 2061 7761 6974 2073 656c 662e 6765 7428   await self.get(
+00032850: 7572 6c2c 2070 6172 616d 733d 7061 7261  url, params=para
+00032860: 6d73 290a 0a20 2020 2061 7379 6e63 2064  ms)..    async d
+00032870: 6566 2067 6574 5f6f 7370 665f 6461 7461  ef get_ospf_data
+00032880: 6261 7365 280a 2020 2020 2020 2020 7365  base(.        se
+00032890: 6c66 2c0a 2020 2020 2020 2020 6465 7669  lf,.        devi
+000328a0: 6365 3a20 7374 722c 0a20 2020 2020 2020  ce: str,.       
+000328b0: 206d 6172 6b65 723a 2073 7472 203d 204e   marker: str = N
+000328c0: 6f6e 652c 0a20 2020 2020 2020 206c 696d  one,.        lim
+000328d0: 6974 3a20 696e 7420 3d20 3130 302c 0a20  it: int = 100,. 
+000328e0: 2020 2029 202d 3e20 5265 7370 6f6e 7365     ) -> Response
+000328f0: 3a0a 2020 2020 2020 2020 2222 224c 6973  :.        """Lis
+00032900: 7420 4f53 5046 204c 696e 6b20 5374 6174  t OSPF Link Stat
+00032910: 6520 4461 7461 6261 7365 2049 6e66 6f72  e Database Infor
+00032920: 6d61 7469 6f6e 2e0a 0a20 2020 2020 2020  mation...       
+00032930: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00032940: 2020 2064 6576 6963 6520 2873 7472 293a     device (str):
+00032950: 2044 6576 6963 6520 7365 7269 616c 206e   Device serial n
+00032960: 756d 6265 720a 2020 2020 2020 2020 2020  umber.          
+00032970: 2020 6d61 726b 6572 2028 7374 722c 206f    marker (str, o
+00032980: 7074 696f 6e61 6c29 3a20 4f70 6171 7565  ptional): Opaque
+00032990: 2068 616e 646c 6520 746f 2066 6574 6368   handle to fetch
+000329a0: 206e 6578 7420 7061 6765 0a20 2020 2020   next page.     
+000329b0: 2020 2020 2020 206c 696d 6974 2028 696e         limit (in
+000329c0: 742c 206f 7074 696f 6e61 6c29 3a20 7061  t, optional): pa
+000329d0: 6765 2073 697a 6520 4465 6661 756c 7473  ge size Defaults
+000329e0: 2074 6f20 3130 302e 0a0a 2020 2020 2020   to 100...      
+000329f0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00032a00: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
+00032a10: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
+00032a20: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
+00032a30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00032a40: 7572 6c20 3d20 222f 6170 692f 726f 7574  url = "/api/rout
+00032a50: 696e 672f 7631 2f6f 7370 662f 6461 7461  ing/v1/ospf/data
+00032a60: 6261 7365 220a 0a20 2020 2020 2020 2070  base"..        p
+00032a70: 6172 616d 7320 3d20 7b0a 2020 2020 2020  arams = {.      
+00032a80: 2020 2020 2020 2764 6576 6963 6527 3a20        'device': 
+00032a90: 6465 7669 6365 2c0a 2020 2020 2020 2020  device,.        
+00032aa0: 2020 2020 276d 6172 6b65 7227 3a20 6d61      'marker': ma
+00032ab0: 726b 6572 2c0a 2020 2020 2020 2020 2020  rker,.          
+00032ac0: 2020 276c 696d 6974 273a 206c 696d 6974    'limit': limit
+00032ad0: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00032ae0: 2020 2020 7265 7475 726e 2061 7761 6974      return await
+00032af0: 2073 656c 662e 6765 7428 7572 6c2c 2070   self.get(url, p
+00032b00: 6172 616d 733d 7061 7261 6d73 290a 0a20  arams=params).. 
+00032b10: 2020 2061 7379 6e63 2064 6566 2067 6574     async def get
+00032b20: 5f6f 7665 726c 6179 5f63 6f6e 6e65 6374  _overlay_connect
+00032b30: 696f 6e28 0a20 2020 2020 2020 2073 656c  ion(.        sel
+00032b40: 662c 0a20 2020 2020 2020 2064 6576 6963  f,.        devic
+00032b50: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+00032b60: 6d61 726b 6572 3a20 7374 7220 3d20 4e6f  marker: str = No
+00032b70: 6e65 2c0a 2020 2020 2020 2020 6c69 6d69  ne,.        limi
+00032b80: 743a 2069 6e74 203d 2031 3030 2c0a 2020  t: int = 100,.  
+00032b90: 2020 2920 2d3e 2052 6573 706f 6e73 653a    ) -> Response:
+00032ba0: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+00032bb0: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+00032bc0: 7420 6f76 6572 6c61 7920 636f 6e74 726f  t overlay contro
+00032bd0: 6c20 636f 6e6e 6563 7469 6f6e 2e0a 0a20  l connection... 
+00032be0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00032bf0: 2020 2020 2020 2020 2064 6576 6963 6520           device 
+00032c00: 2873 7472 293a 2044 6576 6963 6520 7365  (str): Device se
+00032c10: 7269 616c 206e 756d 6265 720a 2020 2020  rial number.    
+00032c20: 2020 2020 2020 2020 6d61 726b 6572 2028          marker (
+00032c30: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+00032c40: 4f70 6171 7565 2068 616e 646c 6520 746f  Opaque handle to
+00032c50: 2066 6574 6368 206e 6578 7420 7061 6765   fetch next page
+00032c60: 0a20 2020 2020 2020 2020 2020 206c 696d  .            lim
+00032c70: 6974 2028 696e 742c 206f 7074 696f 6e61  it (int, optiona
+00032c80: 6c29 3a20 7061 6765 2073 697a 6520 4465  l): page size De
+00032c90: 6661 756c 7473 2074 6f20 3130 302e 0a0a  faults to 100...
+00032ca0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00032cb0: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
+00032cc0: 706f 6e73 653a 2043 656e 7472 616c 4150  ponse: CentralAP
+00032cd0: 4920 5265 7370 6f6e 7365 206f 626a 6563  I Response objec
+00032ce0: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
+00032cf0: 2020 2020 2020 7572 6c20 3d20 222f 6170        url = "/ap
+00032d00: 692f 726f 7574 696e 672f 7631 2f6f 7665  i/routing/v1/ove
+00032d10: 726c 6179 2f63 6f6e 6e65 6374 696f 6e22  rlay/connection"
+00032d20: 0a0a 2020 2020 2020 2020 7061 7261 6d73  ..        params
+00032d30: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00032d40: 2027 6465 7669 6365 273a 2064 6576 6963   'device': devic
+00032d50: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
+00032d60: 6d61 726b 6572 273a 206d 6172 6b65 722c  marker': marker,
+00032d70: 0a20 2020 2020 2020 2020 2020 2027 6c69  .            'li
+00032d80: 6d69 7427 3a20 6c69 6d69 740a 2020 2020  mit': limit.    
+00032d90: 2020 2020 7d0a 0a20 2020 2020 2020 2072      }..        r
+00032da0: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+00032db0: 2e67 6574 2875 726c 2c20 7061 7261 6d73  .get(url, params
+00032dc0: 3d70 6172 616d 7329 0a0a 2020 2020 6173  =params)..    as
+00032dd0: 796e 6320 6465 6620 7265 7365 745f 6f76  ync def reset_ov
+00032de0: 6572 6c61 795f 636f 6e6e 6563 7469 6f6e  erlay_connection
+00032df0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00032e00: 2020 2020 2020 2020 6465 7669 6365 3a20          device: 
+00032e10: 7374 722c 0a20 2020 2029 202d 3e20 5265  str,.    ) -> Re
+00032e20: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+00032e30: 2222 2252 6573 6574 206f 7665 726c 6179  """Reset overlay
+00032e40: 2063 6f6e 7472 6f6c 2063 6f6e 6e65 6374   control connect
+00032e50: 696f 6e2e 0a0a 2020 2020 2020 2020 4172  ion...        Ar
+00032e60: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00032e70: 6465 7669 6365 2028 7374 7229 3a20 4465  device (str): De
+00032e80: 7669 6365 2073 6572 6961 6c20 6e75 6d62  vice serial numb
+00032e90: 6572 0a0a 2020 2020 2020 2020 5265 7475  er..        Retu
+00032ea0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00032eb0: 2052 6573 706f 6e73 653a 2043 656e 7472   Response: Centr
+00032ec0: 616c 4150 4920 5265 7370 6f6e 7365 206f  alAPI Response o
+00032ed0: 626a 6563 740a 2020 2020 2020 2020 2222  bject.        ""
+00032ee0: 220a 2020 2020 2020 2020 7572 6c20 3d20  ".        url = 
+00032ef0: 222f 6170 692f 726f 7574 696e 672f 7631  "/api/routing/v1
+00032f00: 2f6f 7665 726c 6179 2f63 6f6e 6e65 6374  /overlay/connect
+00032f10: 696f 6e2f 7265 7365 7422 0a0a 2020 2020  ion/reset"..    
+00032f20: 2020 2020 7061 7261 6d73 203d 207b 0a20      params = {. 
+00032f30: 2020 2020 2020 2020 2020 2027 6465 7669             'devi
+00032f40: 6365 273a 2064 6576 6963 650a 2020 2020  ce': device.    
+00032f50: 2020 2020 7d0a 0a20 2020 2020 2020 2072      }..        r
+00032f60: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+00032f70: 2e70 7574 2875 726c 2c20 7061 7261 6d73  .put(url, params
+00032f80: 3d70 6172 616d 7329 0a0a 2020 2020 6173  =params)..    as
+00032f90: 796e 6320 6465 6620 6765 745f 6f76 6572  ync def get_over
+00032fa0: 6c61 795f 726f 7574 6573 5f6c 6561 726e  lay_routes_learn
+00032fb0: 6564 280a 2020 2020 2020 2020 7365 6c66  ed(.        self
+00032fc0: 2c0a 2020 2020 2020 2020 6465 7669 6365  ,.        device
+00032fd0: 3a20 7374 722c 0a20 2020 2020 2020 202a  : str,.        *
+00032fe0: 2c0a 2020 2020 2020 2020 6265 7374 3a20  ,.        best: 
+00032ff0: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+00033000: 2020 2020 2020 6d61 726b 6572 3a20 7374        marker: st
+00033010: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00033020: 2020 6c69 6d69 743a 2069 6e74 203d 2031    limit: int = 1
+00033030: 3030 2c0a 2020 2020 2920 2d3e 2052 6573  00,.    ) -> Res
+00033040: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
+00033050: 2222 4c69 7374 206f 6620 6c65 6172 6e65  ""List of learne
+00033060: 6420 726f 7574 6573 2066 726f 6d20 6f76  d routes from ov
+00033070: 6572 6c61 792e 0a0a 2020 2020 2020 2020  erlay...        
+00033080: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00033090: 2020 6465 7669 6365 2028 7374 7229 3a20    device (str): 
+000330a0: 4465 7669 6365 2073 6572 6961 6c20 6e75  Device serial nu
+000330b0: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
+000330c0: 2062 6573 7420 2862 6f6f 6c29 3a20 5265   best (bool): Re
+000330d0: 7475 726e 206f 6e6c 7920 6265 7374 202f  turn only best /
+000330e0: 2070 7265 6665 7272 6564 2072 6f75 7465   preferred route
+000330f0: 730a 2020 2020 2020 2020 2020 2020 6d61  s.            ma
+00033100: 726b 6572 2028 7374 722c 206f 7074 696f  rker (str, optio
+00033110: 6e61 6c29 3a20 4f70 6171 7565 2068 616e  nal): Opaque han
+00033120: 646c 6520 746f 2066 6574 6368 206e 6578  dle to fetch nex
+00033130: 7420 7061 6765 0a20 2020 2020 2020 2020  t page.         
+00033140: 2020 206c 696d 6974 2028 696e 742c 206f     limit (int, o
+00033150: 7074 696f 6e61 6c29 3a20 7061 6765 2073  ptional): page s
+00033160: 697a 6520 4465 6661 756c 7473 2074 6f20  ize Defaults to 
+00033170: 3130 302e 0a0a 2020 2020 2020 2020 5265  100...        Re
+00033180: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00033190: 2020 2052 6573 706f 6e73 653a 2043 656e     Response: Cen
+000331a0: 7472 616c 4150 4920 5265 7370 6f6e 7365  tralAPI Response
+000331b0: 206f 626a 6563 740a 2020 2020 2020 2020   object.        
+000331c0: 2222 220a 2020 2020 2020 2020 7572 6c20  """.        url 
+000331d0: 3d20 222f 6170 692f 726f 7574 696e 672f  = "/api/routing/
+000331e0: 7631 2f6f 7665 726c 6179 2f72 6f75 7465  v1/overlay/route
+000331f0: 2f6c 6561 726e 6564 220a 2020 2020 2020  /learned".      
+00033200: 2020 6966 2062 6573 743a 0a20 2020 2020    if best:.     
+00033210: 2020 2020 2020 2075 726c 203d 2066 277b         url = f'{
+00033220: 7572 6c7d 2f62 6573 7427 0a0a 2020 2020  url}/best'..    
+00033230: 2020 2020 7061 7261 6d73 203d 207b 0a20      params = {. 
+00033240: 2020 2020 2020 2020 2020 2027 6465 7669             'devi
+00033250: 6365 273a 2064 6576 6963 652c 0a20 2020  ce': device,.   
+00033260: 2020 2020 2020 2020 2027 6d61 726b 6572           'marker
+00033270: 273a 206d 6172 6b65 722c 0a20 2020 2020  ': marker,.     
+00033280: 2020 2020 2020 2027 6c69 6d69 7427 3a20         'limit': 
+00033290: 6c69 6d69 740a 2020 2020 2020 2020 7d0a  limit.        }.
+000332a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000332b0: 6177 6169 7420 7365 6c66 2e67 6574 2875  await self.get(u
+000332c0: 726c 2c20 7061 7261 6d73 3d70 6172 616d  rl, params=param
+000332d0: 7329 0a0a 2020 2020 6173 796e 6320 6465  s)..    async de
+000332e0: 6620 6765 745f 6f76 6572 6c61 795f 726f  f get_overlay_ro
+000332f0: 7574 6573 5f61 6476 6572 7469 7365 6428  utes_advertised(
+00033300: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00033310: 2020 2020 2020 2064 6576 6963 653a 2073         device: s
+00033320: 7472 2c0a 2020 2020 2020 2020 6d61 726b  tr,.        mark
+00033330: 6572 3a20 7374 7220 3d20 4e6f 6e65 2c0a  er: str = None,.
+00033340: 2020 2020 2020 2020 6c69 6d69 743a 2069          limit: i
+00033350: 6e74 203d 2031 3030 2c0a 2020 2020 2920  nt = 100,.    ) 
+00033360: 2d3e 2052 6573 706f 6e73 653a 0a20 2020  -> Response:.   
+00033370: 2020 2020 2022 2222 4c69 7374 206f 6620       """List of 
+00033380: 6164 7665 7274 6973 6564 2072 6f75 7465  advertised route
+00033390: 7320 746f 206f 7665 726c 6179 2e0a 0a20  s to overlay... 
+000333a0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+000333b0: 2020 2020 2020 2020 2064 6576 6963 6520           device 
+000333c0: 2873 7472 293a 2044 6576 6963 6520 7365  (str): Device se
+000333d0: 7269 616c 206e 756d 6265 720a 2020 2020  rial number.    
+000333e0: 2020 2020 2020 2020 6d61 726b 6572 2028          marker (
+000333f0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+00033400: 4f70 6171 7565 2068 616e 646c 6520 746f  Opaque handle to
+00033410: 2066 6574 6368 206e 6578 7420 7061 6765   fetch next page
+00033420: 0a20 2020 2020 2020 2020 2020 206c 696d  .            lim
+00033430: 6974 2028 696e 742c 206f 7074 696f 6e61  it (int, optiona
+00033440: 6c29 3a20 7061 6765 2073 697a 6520 4465  l): page size De
+00033450: 6661 756c 7473 2074 6f20 3130 302e 0a0a  faults to 100...
+00033460: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00033470: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
+00033480: 706f 6e73 653a 2043 656e 7472 616c 4150  ponse: CentralAP
+00033490: 4920 5265 7370 6f6e 7365 206f 626a 6563  I Response objec
+000334a0: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
+000334b0: 2020 2020 2020 7572 6c20 3d20 222f 6170        url = "/ap
+000334c0: 692f 726f 7574 696e 672f 7631 2f6f 7665  i/routing/v1/ove
+000334d0: 726c 6179 2f72 6f75 7465 2f61 6476 6572  rlay/route/adver
+000334e0: 7469 7365 6422 0a0a 2020 2020 2020 2020  tised"..        
+000334f0: 7061 7261 6d73 203d 207b 0a20 2020 2020  params = {.     
+00033500: 2020 2020 2020 2027 6465 7669 6365 273a         'device':
+00033510: 2064 6576 6963 652c 0a20 2020 2020 2020   device,.       
+00033520: 2020 2020 2027 6d61 726b 6572 273a 206d       'marker': m
+00033530: 6172 6b65 722c 0a20 2020 2020 2020 2020  arker,.         
+00033540: 2020 2027 6c69 6d69 7427 3a20 6c69 6d69     'limit': limi
+00033550: 740a 2020 2020 2020 2020 7d0a 0a20 2020  t.        }..   
+00033560: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+00033570: 7420 7365 6c66 2e67 6574 2875 726c 2c20  t self.get(url, 
+00033580: 7061 7261 6d73 3d70 6172 616d 7329 0a0a  params=params)..
+00033590: 2020 2020 6173 796e 6320 6465 6620 6765      async def ge
+000335a0: 745f 6f76 6572 6c61 795f 696e 7465 7266  t_overlay_interf
+000335b0: 6163 6573 280a 2020 2020 2020 2020 7365  aces(.        se
+000335c0: 6c66 2c0a 2020 2020 2020 2020 6465 7669  lf,.        devi
+000335d0: 6365 3a20 7374 722c 0a20 2020 2020 2020  ce: str,.       
+000335e0: 206d 6172 6b65 723a 2073 7472 203d 204e   marker: str = N
+000335f0: 6f6e 652c 0a20 2020 2020 2020 206c 696d  one,.        lim
+00033600: 6974 3a20 696e 7420 3d20 3130 302c 0a20  it: int = 100,. 
+00033610: 2020 2029 202d 3e20 5265 7370 6f6e 7365     ) -> Response
+00033620: 3a0a 2020 2020 2020 2020 2222 224c 6973  :.        """Lis
+00033630: 7420 6f66 206f 7665 726c 6179 2069 6e74  t of overlay int
+00033640: 6572 6661 6365 7320 2874 756e 6e65 6c73  erfaces (tunnels
+00033650: 292e 0a0a 2020 2020 2020 2020 4172 6773  )...        Args
+00033660: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
+00033670: 7669 6365 2028 7374 7229 3a20 4465 7669  vice (str): Devi
+00033680: 6365 2073 6572 6961 6c20 6e75 6d62 6572  ce serial number
+00033690: 0a20 2020 2020 2020 2020 2020 206d 6172  .            mar
+000336a0: 6b65 7220 2873 7472 2c20 6f70 7469 6f6e  ker (str, option
+000336b0: 616c 293a 204f 7061 7175 6520 6861 6e64  al): Opaque hand
+000336c0: 6c65 2074 6f20 6665 7463 6820 6e65 7874  le to fetch next
+000336d0: 2070 6167 650a 2020 2020 2020 2020 2020   page.          
+000336e0: 2020 6c69 6d69 7420 2869 6e74 2c20 6f70    limit (int, op
+000336f0: 7469 6f6e 616c 293a 2070 6167 6520 7369  tional): page si
+00033700: 7a65 2044 6566 6175 6c74 7320 746f 2031  ze Defaults to 1
+00033710: 3030 2e0a 0a20 2020 2020 2020 2052 6574  00...        Ret
+00033720: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00033730: 2020 5265 7370 6f6e 7365 3a20 4365 6e74    Response: Cent
+00033740: 7261 6c41 5049 2052 6573 706f 6e73 6520  ralAPI Response 
+00033750: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
+00033760: 2222 0a20 2020 2020 2020 2075 726c 203d  "".        url =
+00033770: 2022 2f61 7069 2f72 6f75 7469 6e67 2f76   "/api/routing/v
+00033780: 312f 6f76 6572 6c61 792f 696e 7465 7266  1/overlay/interf
+00033790: 6163 6522 0a0a 2020 2020 2020 2020 7061  ace"..        pa
+000337a0: 7261 6d73 203d 207b 0a20 2020 2020 2020  rams = {.       
+000337b0: 2020 2020 2027 6465 7669 6365 273a 2064       'device': d
+000337c0: 6576 6963 652c 0a20 2020 2020 2020 2020  evice,.         
+000337d0: 2020 2027 6d61 726b 6572 273a 206d 6172     'marker': mar
+000337e0: 6b65 722c 0a20 2020 2020 2020 2020 2020  ker,.           
+000337f0: 2027 6c69 6d69 7427 3a20 6c69 6d69 740a   'limit': limit.
+00033800: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00033810: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+00033820: 7365 6c66 2e67 6574 2875 726c 2c20 7061  self.get(url, pa
+00033830: 7261 6d73 3d70 6172 616d 7329 0a0a 2020  rams=params)..  
+00033840: 2020 6173 796e 6320 6465 6620 6765 745f    async def get_
+00033850: 6465 6e79 6c69 7374 5f63 6c69 656e 7473  denylist_clients
+00033860: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00033870: 2020 2020 2020 2020 7365 7269 616c 3a20          serial: 
+00033880: 7374 722c 0a20 2020 2029 202d 3e20 5265  str,.    ) -> Re
+00033890: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+000338a0: 2222 2247 6574 2061 6c6c 2064 656e 796c  """Get all denyl
+000338b0: 6973 7420 636c 6965 6e74 206d 6163 2061  ist client mac a
+000338c0: 6464 7265 7373 2069 6e20 6465 7669 6365  ddress in device
+000338d0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+000338e0: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
+000338f0: 6961 6c20 2873 7472 293a 2044 6576 6963  ial (str): Devic
+00033900: 6520 6964 206f 6620 7669 7274 7561 6c20  e id of virtual 
+00033910: 636f 6e74 726f 6c6c 6572 2028 414f 5338  controller (AOS8
+00033920: 2049 4150 2920 6f72 2073 6572 6961 6c20   IAP) or serial 
+00033930: 6f66 2041 4f53 3130 2061 702e 0a20 2020  of AOS10 ap..   
+00033940: 2020 2020 2020 2020 2020 2020 2045 7861               Exa
+00033950: 6d70 6c65 3a31 3462 3337 3433 6330 3166  mple:14b3743c01f
+00033960: 3830 3830 6266 6130 3763 6130 3533 6566  8080bfa07ca053ef
+00033970: 3165 3839 3564 6639 6330 3638 3066 6535  1e895df9c0680fe5
+00033980: 6131 3762 6664 350a 0a20 2020 2020 2020  a17bfd5..       
+00033990: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+000339a0: 2020 2020 2020 5265 7370 6f6e 7365 3a20        Response: 
+000339b0: 4365 6e74 7261 6c41 5049 2052 6573 706f  CentralAPI Respo
+000339c0: 6e73 6520 6f62 6a65 6374 0a20 2020 2020  nse object.     
+000339d0: 2020 2022 2222 0a20 2020 2020 2020 2075     """.        u
+000339e0: 726c 203d 2066 222f 636f 6e66 6967 7572  rl = f"/configur
+000339f0: 6174 696f 6e2f 7631 2f73 7761 726d 2f7b  ation/v1/swarm/{
+00033a00: 7365 7269 616c 7d2f 626c 6163 6b6c 6973  serial}/blacklis
+00033a10: 7469 6e67 220a 0a20 2020 2020 2020 2072  ting"..        r
+00033a20: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+00033a30: 2e67 6574 2875 726c 290a 0a0a 2020 2020  .get(url)...    
+00033a40: 6173 796e 6320 6465 6620 6765 745f 6175  async def get_au
+00033a50: 746f 5f73 7562 7363 7269 6265 280a 2020  to_subscribe(.  
+00033a60: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00033a70: 2920 2d3e 2052 6573 706f 6e73 653a 0a20  ) -> Response:. 
+00033a80: 2020 2020 2020 2022 2222 4765 7420 7468         """Get th
+00033a90: 6520 7365 7276 6963 6573 2077 6869 6368  e services which
+00033aa0: 2068 6176 6520 6175 746f 2073 7562 7363   have auto subsc
+00033ab0: 7269 6265 2065 6e61 626c 6564 2e0a 0a20  ribe enabled... 
+00033ac0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00033ad0: 2020 2020 2020 2020 2020 2020 5265 7370              Resp
+00033ae0: 6f6e 7365 3a20 4365 6e74 7261 6c41 5049  onse: CentralAPI
+00033af0: 2052 6573 706f 6e73 6520 6f62 6a65 6374   Response object
+00033b00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00033b10: 2020 2020 2075 726c 203d 2022 2f70 6c61       url = "/pla
+00033b20: 7466 6f72 6d2f 6c69 6365 6e73 696e 672f  tform/licensing/
+00033b30: 7631 2f63 7573 746f 6d65 722f 7365 7474  v1/customer/sett
+00033b40: 696e 6773 2f61 7574 6f6c 6963 656e 7365  ings/autolicense
+00033b50: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+00033b60: 6e20 6177 6169 7420 7365 6c66 2e67 6574  n await self.get
+00033b70: 2875 726c 290a 0a20 2020 2061 7379 6e63  (url)..    async
+00033b80: 2064 6566 2065 6e61 626c 655f 6175 746f   def enable_auto
+00033b90: 5f73 7562 7363 7269 6265 280a 2020 2020  _subscribe(.    
+00033ba0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00033bb0: 2020 7365 7276 6963 6573 3a20 4c69 7374    services: List
+00033bc0: 5b73 7472 5d20 7c20 7374 722c 0a20 2020  [str] | str,.   
+00033bd0: 2029 202d 3e20 5265 7370 6f6e 7365 3a0a   ) -> Response:.
+00033be0: 2020 2020 2020 2020 2222 2253 7461 6e64          """Stand
+00033bf0: 616c 6f6e 6520 4375 7374 6f6d 6572 2041  alone Customer A
+00033c00: 5049 3a20 4173 7369 676e 206c 6963 656e  PI: Assign licen
+00033c10: 7365 7320 746f 2061 6c6c 2064 6576 6963  ses to all devic
+00033c20: 6573 2061 6e64 2065 6e61 626c 6520 6175  es and enable au
+00033c30: 746f 2073 7562 7363 7269 6265 2066 6f72  to subscribe for
+00033c40: 0a20 2020 2020 2020 2067 6976 656e 2073  .        given s
+00033c50: 6572 7669 6365 732e 0a0a 2020 2020 2020  ervices...      
+00033c60: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00033c70: 2020 2020 7365 7276 6963 6573 2028 4c69      services (Li
+00033c80: 7374 5b73 7472 5d29 3a20 6c69 7374 206f  st[str]): list o
+00033c90: 6620 7365 7276 6963 6573 2065 2e67 2e20  f services e.g. 
+00033ca0: 5b27 7061 272c 2027 7563 6327 2c20 666f  ['pa', 'ucc', fo
+00033cb0: 756e 6461 7469 6f6e 5f61 702c 0a20 2020  undation_ap,.   
+00033cc0: 2020 2020 2020 2020 2020 2020 2061 6476               adv
+00033cd0: 616e 6365 645f 7377 6974 6368 5f36 3230  anced_switch_620
+00033ce0: 302c 2066 6f75 6e64 6174 696f 6e5f 3730  0, foundation_70
+00033cf0: 5858 2065 7463 202e 2e2e 5d2e 2043 6865  XX etc ...]. Che
+00033d00: 636b 0a20 2020 2020 2020 2020 2020 2020  ck.             
+00033d10: 2020 202f 706c 6174 666f 726d 2f6c 6963     /platform/lic
+00033d20: 656e 7369 6e67 2f76 312f 7365 7276 6963  ensing/v1/servic
+00033d30: 6573 2f63 6f6e 6669 6720 4150 4920 7265  es/config API re
+00033d40: 7370 6f6e 7365 2074 6f20 6b6e 6f77 2074  sponse to know t
+00033d50: 6865 206c 6973 7420 6f66 2073 7570 706f  he list of suppo
+00033d60: 7274 6564 0a20 2020 2020 2020 2020 2020  rted.           
+00033d70: 2020 2020 2073 6572 7669 6365 732e 0a0a       services...
+00033d80: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00033d90: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
+00033da0: 706f 6e73 653a 2043 656e 7472 616c 4150  ponse: CentralAP
+00033db0: 4920 5265 7370 6f6e 7365 206f 626a 6563  I Response objec
+00033dc0: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
+00033dd0: 2020 2020 2020 7572 6c20 3d20 222f 706c        url = "/pl
+00033de0: 6174 666f 726d 2f6c 6963 656e 7369 6e67  atform/licensing
+00033df0: 2f76 312f 6375 7374 6f6d 6572 2f73 6574  /v1/customer/set
+00033e00: 7469 6e67 732f 6175 746f 6c69 6365 6e73  tings/autolicens
+00033e10: 6522 0a0a 2020 2020 2020 2020 6966 2069  e"..        if i
+00033e20: 7369 6e73 7461 6e63 6528 7365 7276 6963  sinstance(servic
+00033e30: 6573 2c20 7374 7229 3a0a 2020 2020 2020  es, str):.      
+00033e40: 2020 2020 2020 7365 7276 6963 6573 203d        services =
+00033e50: 205b 7365 7276 6963 6573 5d0a 0a20 2020   [services]..   
+00033e60: 2020 2020 206a 736f 6e5f 6461 7461 203d       json_data =
+00033e70: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
+00033e80: 7365 7276 6963 6573 273a 2073 6572 7669  services': servi
+00033e90: 6365 730a 2020 2020 2020 2020 7d0a 0a20  ces.        }.. 
+00033ea0: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+00033eb0: 6169 7420 7365 6c66 2e70 6f73 7428 7572  ait self.post(ur
+00033ec0: 6c2c 206a 736f 6e5f 6461 7461 3d6a 736f  l, json_data=jso
+00033ed0: 6e5f 6461 7461 290a 0a20 2020 2061 7379  n_data)..    asy
+00033ee0: 6e63 2064 6566 2064 6973 6162 6c65 5f61  nc def disable_a
+00033ef0: 7574 6f5f 7375 6273 6372 6962 6528 0a20  uto_subscribe(. 
+00033f00: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00033f10: 2020 2020 2073 6572 7669 6365 733a 204c       services: L
+00033f20: 6973 745b 7374 725d 207c 2073 7472 2c0a  ist[str] | str,.
+00033f30: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
+00033f40: 653a 0a20 2020 2020 2020 2022 2222 5374  e:.        """St
+00033f50: 616e 6461 6c6f 6e65 2043 7573 746f 6d65  andalone Custome
+00033f60: 7220 4150 493a 2044 6973 6162 6c65 2061  r API: Disable a
+00033f70: 7574 6f20 6c69 6365 6e73 696e 6720 666f  uto licensing fo
+00033f80: 7220 6769 7665 6e20 7365 7276 6963 6573  r given services
+00033f90: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00033fa0: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
+00033fb0: 7669 6365 7320 284c 6973 745b 7374 725d  vices (List[str]
+00033fc0: 293a 206c 6973 7420 6f66 2073 6572 7669  ): list of servi
+00033fd0: 6365 7320 652e 672e 205b 2770 6127 2c20  ces e.g. ['pa', 
+00033fe0: 2775 6363 272c 2066 6f75 6e64 6174 696f  'ucc', foundatio
+00033ff0: 6e5f 6170 2c0a 2020 2020 2020 2020 2020  n_ap,.          
+00034000: 2020 2020 2020 6164 7661 6e63 6564 5f73        advanced_s
+00034010: 7769 7463 685f 3632 3030 2c20 666f 756e  witch_6200, foun
+00034020: 6461 7469 6f6e 5f37 3058 5820 6574 6320  dation_70XX etc 
+00034030: 2e2e 2e5d 2e20 4368 6563 6b0a 2020 2020  ...]. Check.    
+00034040: 2020 2020 2020 2020 2020 2020 2f70 6c61              /pla
+00034050: 7466 6f72 6d2f 6c69 6365 6e73 696e 672f  tform/licensing/
+00034060: 7631 2f73 6572 7669 6365 732f 636f 6e66  v1/services/conf
+00034070: 6967 2041 5049 2072 6573 706f 6e73 6520  ig API response 
+00034080: 746f 206b 6e6f 7720 7468 6520 6c69 7374  to know the list
+00034090: 206f 6620 7375 7070 6f72 7465 640a 2020   of supported.  
+000340a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000340b0: 7276 6963 6573 2e0a 0a20 2020 2020 2020  rvices...       
+000340c0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+000340d0: 2020 2020 2020 5265 7370 6f6e 7365 3a20        Response: 
+000340e0: 4365 6e74 7261 6c41 5049 2052 6573 706f  CentralAPI Respo
+000340f0: 6e73 6520 6f62 6a65 6374 0a20 2020 2020  nse object.     
+00034100: 2020 2022 2222 0a20 2020 2020 2020 2075     """.        u
+00034110: 726c 203d 2022 2f70 6c61 7466 6f72 6d2f  rl = "/platform/
+00034120: 6c69 6365 6e73 696e 672f 7631 2f63 7573  licensing/v1/cus
+00034130: 746f 6d65 722f 7365 7474 696e 6773 2f61  tomer/settings/a
+00034140: 7574 6f6c 6963 656e 7365 220a 0a20 2020  utolicense"..   
+00034150: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00034160: 6365 2873 6572 7669 6365 732c 2073 7472  ce(services, str
+00034170: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00034180: 6572 7669 6365 7320 3d20 5b73 6572 7669  ervices = [servi
+00034190: 6365 735d 0a0a 2020 2020 2020 2020 6a73  ces]..        js
+000341a0: 6f6e 5f64 6174 6120 3d20 7b0a 2020 2020  on_data = {.    
+000341b0: 2020 2020 2020 2020 2773 6572 7669 6365          'service
+000341c0: 7327 3a20 7365 7276 6963 6573 0a20 2020  s': services.   
+000341d0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+000341e0: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+000341f0: 662e 6465 6c65 7465 2875 726c 2c20 6a73  f.delete(url, js
+00034200: 6f6e 5f64 6174 613d 6a73 6f6e 5f64 6174  on_data=json_dat
+00034210: 6129 0a0a 2020 2020 2320 2f2f 202d 2d20  a)..    # // -- 
+00034220: 4e6f 7420 7573 6564 2062 7920 636f 6d6d  Not used by comm
+00034230: 616e 6473 2079 6574 2e20 2075 6e64 6f63  ands yet.  undoc
+00034240: 756d 656e 7465 6420 6b6d 7320 6170 6920  umented kms api 
+00034250: 2d2d 202f 2f0a 2020 2020 6173 796e 6320  -- //.    async 
+00034260: 6465 6620 6b6d 735f 6765 745f 7379 6e63  def kms_get_sync
+00034270: 6564 5f61 7073 2873 656c 662c 206d 6163  ed_aps(self, mac
+00034280: 3a20 7374 7229 202d 3e20 5265 7370 6f6e  : str) -> Respon
+00034290: 7365 3a0a 2020 2020 2020 2020 7572 6c20  se:.        url 
+000342a0: 3d20 6622 2f6b 6579 6d67 6d74 2f76 312f  = f"/keymgmt/v1/
+000342b0: 7379 6e63 6564 6170 6c69 7374 2f7b 6d61  syncedaplist/{ma
+000342c0: 637d 220a 2020 2020 2020 2020 7265 7475  c}".        retu
+000342d0: 726e 2061 7761 6974 2073 656c 662e 6765  rn await self.ge
+000342e0: 7428 7572 6c29 0a0a 2020 2020 6173 796e  t(url)..    asyn
+000342f0: 6320 6465 6620 6b6d 735f 6765 745f 636c  c def kms_get_cl
+00034300: 6965 6e74 5f72 6563 6f72 6428 7365 6c66  ient_record(self
+00034310: 2c20 6d61 633a 2073 7472 2920 2d3e 2052  , mac: str) -> R
+00034320: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
+00034330: 2075 726c 203d 2066 222f 6b65 796d 676d   url = f"/keymgm
+00034340: 742f 7631 2f6b 6579 6361 6368 652f 7b6d  t/v1/keycache/{m
+00034350: 6163 7d22 0a20 2020 2020 2020 2072 6574  ac}".        ret
+00034360: 7572 6e20 6177 6169 7420 7365 6c66 2e67  urn await self.g
+00034370: 6574 2875 726c 290a 0a20 2020 2061 7379  et(url)..    asy
+00034380: 6e63 2064 6566 206b 6d73 5f67 6574 5f68  nc def kms_get_h
+00034390: 6173 6828 7365 6c66 2920 2d3e 2052 6573  ash(self) -> Res
+000343a0: 706f 6e73 653a 0a20 2020 2020 2020 2075  ponse:.        u
+000343b0: 726c 203d 2022 2f6b 6579 6d67 6d74 2f76  rl = "/keymgmt/v
+000343c0: 312f 6b65 7968 6173 6822 0a20 2020 2020  1/keyhash".     
+000343d0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+000343e0: 7365 6c66 2e67 6574 2875 726c 290a 0a20  self.get(url).. 
+000343f0: 2020 2061 7379 6e63 2064 6566 206b 6d73     async def kms
+00034400: 5f67 6574 5f61 705f 7374 6174 6528 7365  _get_ap_state(se
+00034410: 6c66 2c20 7365 7269 616c 3a20 7374 7229  lf, serial: str)
+00034420: 202d 3e20 5265 7370 6f6e 7365 3a0a 2020   -> Response:.  
+00034430: 2020 2020 2020 7572 6c20 3d20 6622 2f6b        url = f"/k
+00034440: 6579 6d67 6d74 2f76 312f 5374 6174 732f  eymgmt/v1/Stats/
+00034450: 6170 2f7b 7365 7269 616c 7d22 0a20 2020  ap/{serial}".   
+00034460: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+00034470: 7420 7365 6c66 2e67 6574 2875 726c 290a  t self.get(url).
+00034480: 0a20 2020 2023 2042 6164 2065 6e64 706f  .    # Bad endpo
+00034490: 696e 7420 5552 4c20 3430 340a 2020 2020  int URL 404.    
+000344a0: 6173 796e 6320 6465 6620 6b6d 735f 6765  async def kms_ge
+000344b0: 745f 6865 616c 7468 2873 656c 6629 202d  t_health(self) -
+000344c0: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
+000344d0: 2020 2020 7572 6c20 3d20 222f 6b65 796d      url = "/keym
+000344e0: 676d 742f 7631 2f68 6561 6c74 6822 0a20  gmt/v1/health". 
+000344f0: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+00034500: 6169 7420 7365 6c66 2e67 6574 2875 726c  ait self.get(url
+00034510: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+00034520: 2063 6c6f 7564 6175 7468 5f67 6574 5f72   cloudauth_get_r
+00034530: 6567 6973 7465 7265 645f 6d61 6373 280a  egistered_macs(.
+00034540: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00034550: 2020 2020 2020 7365 6172 6368 3a20 7374        search: st
+00034560: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00034570: 2020 736f 7274 3a20 7374 7220 3d20 4e6f    sort: str = No
+00034580: 6e65 2c0a 2020 2020 2020 2020 6669 6c65  ne,.        file
+00034590: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
+000345a0: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
+000345b0: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
+000345c0: 4665 7463 6820 616c 6c20 4d61 6320 5265  Fetch all Mac Re
+000345d0: 6769 7374 7261 7469 6f6e 7320 6173 2061  gistrations as a
+000345e0: 2043 5356 2066 696c 652e 0a0a 2020 2020   CSV file...    
+000345f0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00034600: 2020 2020 2020 7365 6172 6368 2028 7374        search (st
+00034610: 722c 206f 7074 696f 6e61 6c29 3a20 4669  r, optional): Fi
+00034620: 6c74 6572 2074 6865 204d 6163 2052 6567  lter the Mac Reg
+00034630: 6973 7472 6174 696f 6e73 2062 7920 4d61  istrations by Ma
+00034640: 6320 4164 6472 6573 7320 616e 6420 436c  c Address and Cl
+00034650: 6965 6e74 204e 616d 652e 0a20 2020 2020  ient Name..     
+00034660: 2020 2020 2020 2020 2020 2044 6f65 7320             Does 
+00034670: 6120 2763 6f6e 7461 696e 7327 206d 6174  a 'contains' mat
+00034680: 6368 2e0a 2020 2020 2020 2020 2020 2020  ch..            
+00034690: 736f 7274 2028 7374 722c 206f 7074 696f  sort (str, optio
+000346a0: 6e61 6c29 3a20 536f 7274 206f 7264 6572  nal): Sort order
+000346b0: 2020 5661 6c69 6420 5661 6c75 6573 3a20    Valid Values: 
+000346c0: 2b6e 616d 652c 202d 6e61 6d65 2c20 2b64  +name, -name, +d
+000346d0: 6973 706c 6179 5f6e 616d 652c 0a20 2020  isplay_name,.   
+000346e0: 2020 2020 2020 2020 2020 2020 202d 6469               -di
+000346f0: 7370 6c61 795f 6e61 6d65 0a20 2020 2020  splay_name.     
+00034700: 2020 2020 2020 2066 696c 656e 616d 6520         filename 
+00034710: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+00034720: 2053 7567 6765 7374 2061 2066 696c 6520   Suggest a file 
+00034730: 6e61 6d65 2066 6f72 2074 6865 2064 6f77  name for the dow
+00034740: 6e6c 6f61 6469 6e67 2066 696c 6520 7669  nloading file vi
+00034750: 6120 636f 6e74 656e 740a 2020 2020 2020  a content.      
+00034760: 2020 2020 2020 2020 2020 6469 7370 6f73            dispos
+00034770: 6974 696f 6e20 6865 6164 6572 2e0a 0a20  ition header... 
+00034780: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00034790: 2020 2020 2020 2020 2020 2020 5265 7370              Resp
+000347a0: 6f6e 7365 3a20 4365 6e74 7261 6c41 5049  onse: CentralAPI
+000347b0: 2052 6573 706f 6e73 6520 6f62 6a65 6374   Response object
+000347c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000347d0: 2020 2020 2075 726c 203d 2022 2f63 6c6f       url = "/clo
+000347e0: 7564 6175 7468 2f61 7069 2f76 332f 6275  udauth/api/v3/bu
+000347f0: 6c6b 2f6d 6163 220a 0a20 2020 2020 2020  lk/mac"..       
+00034800: 2070 6172 616d 7320 3d20 7b0a 2020 2020   params = {.    
+00034810: 2020 2020 2020 2020 2773 6561 7263 6827          'search'
+00034820: 3a20 7365 6172 6368 2c0a 2020 2020 2020  : search,.      
+00034830: 2020 2020 2020 2773 6f72 7427 3a20 736f        'sort': so
+00034840: 7274 2c0a 2020 2020 2020 2020 2020 2020  rt,.            
+00034850: 2766 696c 656e 616d 6527 3a20 6669 6c65  'filename': file
+00034860: 6e61 6d65 0a20 2020 2020 2020 207d 0a0a  name.        }..
+00034870: 2020 2020 2020 2020 7265 7370 203d 2061          resp = a
+00034880: 7761 6974 2073 656c 662e 6765 7428 7572  wait self.get(ur
+00034890: 6c2c 2070 6172 616d 733d 7061 7261 6d73  l, params=params
+000348a0: 290a 0a20 2020 2020 2020 2069 6620 7265  )..        if re
+000348b0: 7370 3a0a 2020 2020 2020 2020 2020 2020  sp:.            
+000348c0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+000348d0: 2020 2020 2064 7320 3d20 7461 626c 6962       ds = tablib
+000348e0: 2e44 6174 6173 6574 2829 2e6c 6f61 6428  .Dataset().load(
+000348f0: 7265 7370 2e6f 7574 7075 7429 0a20 2020  resp.output).   
+00034900: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00034910: 702e 6f75 7470 7574 203d 2079 616d 6c2e  p.output = yaml.
+00034920: 6c6f 6164 2864 732e 6a73 6f6e 2c20 4c6f  load(ds.json, Lo
+00034930: 6164 6572 3d79 616d 6c2e 5361 6665 4c6f  ader=yaml.SafeLo
+00034940: 6164 6572 290a 2020 2020 2020 2020 2020  ader).          
+00034950: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00034960: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+00034970: 2020 2020 2020 2020 206c 6f67 2e65 7272           log.err
+00034980: 6f72 2866 2263 6c6f 7564 6175 7468 5f67  or(f"cloudauth_g
+00034990: 6574 5f72 6567 6973 7465 7265 645f 6d61  et_registered_ma
+000349a0: 6373 2063 6175 6768 7420 7b65 2e5f 5f63  cs caught {e.__c
+000349b0: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f7d  lass__.__name__}
+000349c0: 2074 7279 696e 6720 746f 2063 6f6e 7665   trying to conve
+000349d0: 7274 2063 7376 2072 6574 7572 6e20 6672  rt csv return fr
+000349e0: 6f6d 2041 5049 2074 6f20 6469 6374 2e22  om API to dict."
+000349f0: 2c20 6361 7074 696f 6e3d 5472 7565 290a  , caption=True).
+00034a00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00034a10: 7265 7370 0a0a 2020 2020 6173 796e 6320  resp..    async 
+00034a20: 6465 6620 636c 6f75 6461 7574 685f 7570  def cloudauth_up
+00034a30: 6c6f 6164 5f66 6978 6d65 280a 2020 2020  load_fixme(.    
+00034a40: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00034a50: 2020 7570 6c6f 6164 5f74 7970 653a 2043    upload_type: C
+00034a60: 6c6f 7564 4175 7468 5570 6c6f 6164 5479  loudAuthUploadTy
+00034a70: 7065 2c0a 2020 2020 2020 2020 6669 6c65  pe,.        file
+00034a80: 3a20 556e 696f 6e5b 5061 7468 2c20 7374  : Union[Path, st
+00034a90: 725d 2c0a 2020 2020 2020 2020 7373 6964  r],.        ssid
+00034aa0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00034ab0: 2020 2920 2d3e 2052 6573 706f 6e73 653a    ) -> Response:
+00034ac0: 0a20 2020 2020 2020 2022 2222 5570 6c6f  .        """Uplo
+00034ad0: 6164 2066 696c 652e 0a0a 2020 2020 2020  ad file...      
+00034ae0: 2020 5468 6973 2064 6f65 736e 2774 2077    This doesn't w
+00034af0: 6f72 6b20 7374 696c 6c20 736f 7274 696e  ork still sortin
+00034b00: 6720 7468 6520 666f 726d 6174 206f 6620  g the format of 
+00034b10: 466f 726d 4461 7461 0a0a 2020 2020 2020  FormData..      
+00034b20: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00034b30: 2020 2020 7570 6c6f 6164 5f74 7970 6520      upload_type 
+00034b40: 2843 6c6f 7564 4175 7468 5570 6c6f 6164  (CloudAuthUpload
+00034b50: 5479 7065 293a 2054 7970 6520 6f66 2066  Type): Type of f
+00034b60: 696c 6520 7570 6c6f 6164 2020 5661 6c69  ile upload  Vali
+00034b70: 6420 5661 6c75 6573 3a20 6d70 736b 2c20  d Values: mpsk, 
+00034b80: 6d61 630a 2020 2020 2020 2020 2020 2020  mac.            
+00034b90: 6669 6c65 2028 556e 696f 6e5b 5061 7468  file (Union[Path
+00034ba0: 2c20 7374 725d 293a 2054 6865 2063 7376  , str]): The csv
+00034bb0: 2066 696c 6520 746f 2075 706c 6f61 640a   file to upload.
+00034bc0: 2020 2020 2020 2020 2020 2020 7373 6964              ssid
+00034bd0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
+00034be0: 3a20 4d50 534b 206e 6574 776f 726b 2053  : MPSK network S
+00034bf0: 5349 442c 2072 6571 7569 7265 6420 6966  SID, required if
+00034c00: 207b 7570 6c6f 6164 5f74 7970 657d 203d   {upload_type} =
+00034c10: 2027 6d70 736b 270a 0a20 2020 2020 2020   'mpsk'..       
+00034c20: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00034c30: 2020 2020 2020 5265 7370 6f6e 7365 3a20        Response: 
+00034c40: 4365 6e74 7261 6c41 5049 2052 6573 706f  CentralAPI Respo
+00034c50: 6e73 6520 6f62 6a65 6374 0a20 2020 2020  nse object.     
+00034c60: 2020 2022 2222 0a20 2020 2020 2020 2075     """.        u
+00034c70: 726c 203d 2066 222f 636c 6f75 6461 7574  rl = f"/cloudaut
+00034c80: 682f 6170 692f 7633 2f62 756c 6b2f 7b75  h/api/v3/bulk/{u
+00034c90: 706c 6f61 645f 7479 7065 7d22 0a20 2020  pload_type}".   
+00034ca0: 2020 2020 2066 696c 6520 3d20 6669 6c65       file = file
+00034cb0: 2069 6620 6973 696e 7374 616e 6365 2866   if isinstance(f
+00034cc0: 696c 652c 2050 6174 6829 2065 6c73 6520  ile, Path) else 
+00034cd0: 5061 7468 2873 7472 2866 696c 6529 290a  Path(str(file)).
+00034ce0: 2020 2020 2020 2020 2320 6461 7461 203d          # data =
+00034cf0: 206d 756c 7469 7061 7274 6966 7928 6669   multipartify(fi
+00034d00: 6c65 2e72 6561 645f 6279 7465 7328 2929  le.read_bytes())
+00034d10: 0a20 2020 2020 2020 2023 2064 6174 6120  .        # data 
+00034d20: 3d20 6169 6f68 7474 702e 466f 726d 4461  = aiohttp.FormDa
+00034d30: 7461 2866 696c 652e 6f70 656e 2829 290a  ta(file.open()).
+00034d40: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
+00034d50: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00034d60: 2773 7369 6427 3a20 7373 6964 0a20 2020  'ssid': ssid.   
+00034d70: 2020 2020 207d 0a20 2020 2020 2020 2066       }.        f
+00034d80: 696c 6573 203d 207b 2022 6669 6c65 223a  iles = { "file":
+00034d90: 2028 6669 6c65 2e6e 616d 652c 2066 696c   (file.name, fil
+00034da0: 652e 6f70 656e 2822 7262 2229 2c20 2274  e.open("rb"), "t
+00034db0: 6578 742f 6373 7622 2920 7d0a 2020 2020  ext/csv") }.    
+00034dc0: 2020 2020 666f 726d 5f64 6174 6120 3d20      form_data = 
+00034dd0: 6169 6f68 7474 702e 466f 726d 4461 7461  aiohttp.FormData
+00034de0: 2866 696c 6573 290a 2020 2020 2020 2020  (files).        
+00034df0: 2320 6669 6c65 7320 3d20 7b66 277b 7570  # files = {f'{up
+00034e00: 6c6f 6164 5f74 7970 657d 5f69 6d70 6f72  load_type}_impor
+00034e10: 7427 3a20 2866 277b 7570 6c6f 6164 5f74  t': (f'{upload_t
+00034e20: 7970 657d 5f69 6d70 6f72 742e 6373 7627  ype}_import.csv'
+00034e30: 2c20 6669 6c65 2e72 6561 645f 6279 7465  , file.read_byte
+00034e40: 7328 2929 7d0a 2020 2020 2020 2020 6865  s())}.        he
+00034e50: 6164 6572 7320 3d20 7b0a 2020 2020 2020  aders = {.      
+00034e60: 2020 2020 2020 2243 6f6e 7465 6e74 2d54        "Content-T
+00034e70: 7970 6522 3a20 226d 756c 7469 7061 7274  ype": "multipart
+00034e80: 2f66 6f72 6d2d 6461 7461 222c 0a20 2020  /form-data",.   
+00034e90: 2020 2020 2020 2020 2027 4163 6365 7074           'Accept
+00034ea0: 273a 2027 6170 706c 6963 6174 696f 6e2f  ': 'application/
+00034eb0: 6a73 6f6e 270a 2020 2020 2020 2020 7d0a  json'.        }.
+00034ec0: 2020 2020 2020 2020 6865 6164 6572 7320          headers 
+00034ed0: 3d20 7b2a 2a68 6561 6465 7273 2c20 2a2a  = {**headers, **
+00034ee0: 6469 6374 2861 696f 6874 7470 2e46 6f72  dict(aiohttp.For
+00034ef0: 6d44 6174 6128 6669 6c65 7329 2e5f 7772  mData(files)._wr
+00034f00: 6974 6572 2e5f 6865 6164 6572 7329 7d0a  iter._headers)}.
+00034f10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00034f20: 6177 6169 7420 7365 6c66 2e70 6f73 7428  await self.post(
+00034f30: 7572 6c2c 2068 6561 6465 7273 3d68 6561  url, headers=hea
+00034f40: 6465 7273 2c20 7061 7261 6d73 3d70 6172  ders, params=par
+00034f50: 616d 732c 2070 6179 6c6f 6164 3d66 6f72  ams, payload=for
+00034f60: 6d5f 6461 7461 290a 0a20 2020 2061 7379  m_data)..    asy
+00034f70: 6e63 2064 6566 2063 6c6f 7564 6175 7468  nc def cloudauth
+00034f80: 5f75 706c 6f61 6428 0a20 2020 2020 2020  _upload(.       
+00034f90: 2073 656c 662c 0a20 2020 2020 2020 2075   self,.        u
+00034fa0: 706c 6f61 645f 7479 7065 3a20 436c 6f75  pload_type: Clou
+00034fb0: 6441 7574 6855 706c 6f61 6454 7970 652c  dAuthUploadType,
+00034fc0: 0a20 2020 2020 2020 2066 696c 653a 2055  .        file: U
+00034fd0: 6e69 6f6e 5b50 6174 682c 2073 7472 5d2c  nion[Path, str],
+00034fe0: 0a20 2020 2020 2020 2073 7369 643a 2073  .        ssid: s
+00034ff0: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
+00035000: 202d 3e20 5265 7370 6f6e 7365 3a0a 0a20   -> Response:.. 
+00035010: 2020 2020 2020 2022 2222 5570 6c6f 6164         """Upload
+00035020: 2066 696c 652e 0a0a 2020 2020 2020 2020   file...        
+00035030: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00035040: 2020 7570 6c6f 6164 5f74 7970 6520 2843    upload_type (C
+00035050: 6c6f 7564 4175 7468 5570 6c6f 6164 5479  loudAuthUploadTy
+00035060: 7065 293a 2054 7970 6520 6f66 2066 696c  pe): Type of fil
+00035070: 6520 7570 6c6f 6164 2020 5661 6c69 6420  e upload  Valid 
+00035080: 5661 6c75 6573 3a20 6d70 736b 2c20 6d61  Values: mpsk, ma
+00035090: 630a 2020 2020 2020 2020 2020 2020 6669  c.            fi
+000350a0: 6c65 2028 556e 696f 6e5b 5061 7468 2c20  le (Union[Path, 
+000350b0: 7374 725d 293a 2054 6865 2063 7376 2066  str]): The csv f
+000350c0: 696c 6520 746f 2075 706c 6f61 640a 2020  ile to upload.  
+000350d0: 2020 2020 2020 2020 2020 7373 6964 2028            ssid (
+000350e0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+000350f0: 4d50 534b 206e 6574 776f 726b 2053 5349  MPSK network SSI
+00035100: 442c 2072 6571 7569 7265 6420 6966 207b  D, required if {
+00035110: 7570 6c6f 6164 5f74 7970 657d 203d 2027  upload_type} = '
+00035120: 6d70 736b 270a 0a20 2020 2020 2020 2052  mpsk'..        R
+00035130: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00035140: 2020 2020 5265 7370 6f6e 7365 3a20 4365      Response: Ce
+00035150: 6e74 7261 6c41 5049 2052 6573 706f 6e73  ntralAPI Respons
+00035160: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
+00035170: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
+00035180: 203d 2066 222f 636c 6f75 6461 7574 682f   = f"/cloudauth/
+00035190: 6170 692f 7633 2f62 756c 6b2f 7b75 706c  api/v3/bulk/{upl
+000351a0: 6f61 645f 7479 7065 7d22 0a20 2020 2020  oad_type}".     
+000351b0: 2020 2066 696c 6520 3d20 6669 6c65 2069     file = file i
+000351c0: 6620 6973 696e 7374 616e 6365 2866 696c  f isinstance(fil
+000351d0: 652c 2050 6174 6829 2065 6c73 6520 5061  e, Path) else Pa
+000351e0: 7468 2873 7472 2866 696c 6529 290a 2020  th(str(file)).  
+000351f0: 2020 2020 2020 7061 7261 6d73 203d 207b        params = {
+00035200: 0a20 2020 2020 2020 2020 2020 2027 7373  .            'ss
+00035210: 6964 273a 2073 7369 640a 2020 2020 2020  id': ssid.      
+00035220: 2020 7d0a 0a20 2020 2020 2020 2023 2048    }..        # H
+00035230: 4143 4b20 6e65 6564 2074 6f20 6d61 6b65  ACK need to make
+00035240: 2074 6865 2061 626f 7665 2061 7379 6e63   the above async
+00035250: 2066 756e 6374 696f 6e20 776f 726b 0a20   function work. 
+00035260: 2020 2020 2020 2069 6d70 6f72 7420 7265         import re
+00035270: 7175 6573 7473 0a20 2020 2020 2020 2068  quests.        h
+00035280: 6561 6465 7273 203d 207b 0a20 2020 2020  eaders = {.     
+00035290: 2020 2020 2020 2022 4175 7468 6f72 697a         "Authoriz
+000352a0: 6174 696f 6e22 3a20 6622 4265 6172 6572  ation": f"Bearer
+000352b0: 207b 7365 6c66 2e61 7574 682e 6365 6e74   {self.auth.cent
+000352c0: 7261 6c5f 696e 666f 5b27 746f 6b65 6e27  ral_info['token'
+000352d0: 5d5b 2761 6363 6573 735f 746f 6b65 6e27  ]['access_token'
+000352e0: 5d7d 222c 0a20 2020 2020 2020 2020 2020  ]}",.           
+000352f0: 2027 4163 6365 7074 273a 2027 6170 706c   'Accept': 'appl
+00035300: 6963 6174 696f 6e2f 6a73 6f6e 270a 2020  ication/json'.  
+00035310: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00035320: 2066 696c 6573 203d 207b 2022 6669 6c65   files = { "file
+00035330: 223a 2028 6669 6c65 2e6e 616d 652c 2066  ": (file.name, f
+00035340: 696c 652e 6f70 656e 2822 7262 2229 2c20  ile.open("rb"), 
+00035350: 2274 6578 742f 6373 7622 2920 7d0a 2020  "text/csv") }.  
+00035360: 2020 2020 2020 7572 6c3d 6622 7b73 656c        url=f"{sel
+00035370: 662e 6175 7468 2e63 656e 7472 616c 5f69  f.auth.central_i
+00035380: 6e66 6f5b 2762 6173 655f 7572 6c27 5d7d  nfo['base_url']}
+00035390: 7b75 726c 7d22 0a0a 2020 2020 2020 2020  {url}"..        
+000353a0: 666f 7220 5f20 696e 2072 616e 6765 2832  for _ in range(2
+000353b0: 293a 0a20 2020 2020 2020 2020 2020 205f  ):.            _
+000353c0: 7265 7370 203d 2072 6571 7565 7374 732e  resp = requests.
+000353d0: 7265 7175 6573 7428 2250 4f53 5422 2c20  request("POST", 
+000353e0: 7572 6c3d 7572 6c2c 2070 6172 616d 733d  url=url, params=
+000353f0: 7061 7261 6d73 2c20 6669 6c65 733d 6669  params, files=fi
+00035400: 6c65 732c 2068 6561 6465 7273 3d68 6561  les, headers=hea
+00035410: 6465 7273 290a 2020 2020 2020 2020 2020  ders).          
+00035420: 2020 6f75 7470 7574 203d 2066 225b 7b5f    output = f"[{_
+00035430: 7265 7370 2e72 6561 736f 6e7d 5d22 202b  resp.reason}]" +
+00035440: 2022 2022 202b 205f 7265 7370 2e74 6578   " " + _resp.tex
+00035450: 742e 6c73 7472 6970 2827 5b5c 6e20 2227  t.lstrip('[\n "'
+00035460: 292e 7273 7472 6970 2827 225c 6e5d 2729  ).rstrip('"\n]')
+00035470: 0a20 2020 2020 2020 2020 2020 2023 204d  .            # M
+00035480: 616b 6520 7265 7175 6573 7473 2052 6573  ake requests Res
+00035490: 706f 6e73 6520 6c6f 6f6b 206c 696b 6520  ponse look like 
+000354a0: 6169 6f68 7474 702e 436c 6965 6e74 5265  aiohttp.ClientRe
+000354b0: 7370 6f6e 7365 0a20 2020 2020 2020 2020  sponse.         
+000354c0: 2020 205f 7265 7370 2e73 7461 7475 732c     _resp.status,
+000354d0: 205f 7265 7370 2e6d 6574 686f 642c 205f   _resp.method, _
+000354e0: 7265 7370 2e75 726c 203d 205f 7265 7370  resp.url = _resp
+000354f0: 2e73 7461 7475 735f 636f 6465 2c20 2250  .status_code, "P
+00035500: 4f53 5422 2c20 5552 4c28 5f72 6573 702e  OST", URL(_resp.
+00035510: 7572 6c29 0a20 2020 2020 2020 2020 2020  url).           
+00035520: 2072 6573 7020 3d20 5265 7370 6f6e 7365   resp = Response
+00035530: 285f 7265 7370 2c20 6f75 7470 7574 3d6f  (_resp, output=o
+00035540: 7574 7075 742c 2065 7272 6f72 3d4e 6f6e  utput, error=Non
+00035550: 6520 6966 205f 7265 7370 2e6f 6b20 656c  e if _resp.ok el
+00035560: 7365 205f 7265 7370 2e72 6561 736f 6e2c  se _resp.reason,
+00035570: 2075 726c 3d55 524c 2875 726c 292c 2065   url=URL(url), e
+00035580: 6c61 7073 6564 3d72 6f75 6e64 285f 7265  lapsed=round(_re
+00035590: 7370 2e65 6c61 7073 6564 2e74 6f74 616c  sp.elapsed.total
+000355a0: 5f73 6563 6f6e 6473 2829 2c20 3229 2c20  _seconds(), 2), 
+000355b0: 7374 6174 7573 5f63 6f64 653d 5f72 6573  status_code=_res
+000355c0: 702e 7374 6174 7573 5f63 6f64 652c 2072  p.status_code, r
+000355d0: 6c5f 7374 723d 222d 2229 0a20 2020 2020  l_str="-").     
+000355e0: 2020 2020 2020 2069 6620 2269 6e76 616c         if "inval
+000355f0: 6964 5f74 6f6b 656e 2220 696e 2072 6573  id_token" in res
+00035600: 702e 6f75 7470 7574 3a0a 2020 2020 2020  p.output:.      
+00035610: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00035620: 6566 7265 7368 5f74 6f6b 656e 2829 0a20  efresh_token(). 
+00035630: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00035640: 6561 6465 7273 5b22 4175 7468 6f72 697a  eaders["Authoriz
+00035650: 6174 696f 6e22 5d20 3d20 6622 4265 6172  ation"] = f"Bear
+00035660: 6572 207b 7365 6c66 2e61 7574 682e 6365  er {self.auth.ce
+00035670: 6e74 7261 6c5f 696e 666f 5b27 746f 6b65  ntral_info['toke
+00035680: 6e27 5d5b 2761 6363 6573 735f 746f 6b65  n']['access_toke
+00035690: 6e27 5d7d 220a 2020 2020 2020 2020 2020  n']}".          
+000356a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000356b0: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
+000356c0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000356d0: 700a 0a20 2020 2061 7379 6e63 2064 6566  p..    async def
+000356e0: 2063 6c6f 7564 6175 7468 5f75 706c 6f61   cloudauth_uploa
+000356f0: 645f 7374 6174 7573 280a 2020 2020 2020  d_status(.      
+00035700: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00035710: 7570 6c6f 6164 5f74 7970 653a 2043 6c6f  upload_type: Clo
+00035720: 7564 4175 7468 5570 6c6f 6164 5479 7065  udAuthUploadType
+00035730: 2c0a 2020 2020 2020 2020 7373 6964 3a20  ,.        ssid: 
+00035740: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00035750: 2920 2d3e 2052 6573 706f 6e73 653a 0a20  ) -> Response:. 
+00035760: 2020 2020 2020 2022 2222 5265 6164 2075         """Read u
+00035770: 706c 6f61 6420 7374 6174 7573 206f 6620  pload status of 
+00035780: 6c61 7374 2066 696c 6520 7570 6c6f 6164  last file upload
+00035790: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+000357a0: 0a20 2020 2020 2020 2020 2020 2075 706c  .            upl
+000357b0: 6f61 645f 7479 7065 2028 436c 6f75 6441  oad_type (CloudA
+000357c0: 7574 6855 706c 6f61 6454 7970 6529 3a20  uthUploadType): 
+000357d0: 5479 7065 206f 6620 6669 6c65 2075 706c  Type of file upl
+000357e0: 6f61 6420 2056 616c 6964 2056 616c 7565  oad  Valid Value
+000357f0: 733a 206d 7073 6b2c 206d 6163 0a20 2020  s: mpsk, mac.   
+00035800: 2020 2020 2020 2020 2073 7369 6420 2873           ssid (s
+00035810: 7472 2c20 6f70 7469 6f6e 616c 293a 204d  tr, optional): M
+00035820: 5053 4b20 6e65 7477 6f72 6b20 5353 4944  PSK network SSID
+00035830: 2c20 7265 7175 6972 6564 2069 6620 7b75  , required if {u
+00035840: 706c 6f61 645f 7479 7065 7d20 3d20 276d  pload_type} = 'm
+00035850: 7073 6b27 0a0a 2020 2020 2020 2020 5265  psk'..        Re
+00035860: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00035870: 2020 2052 6573 706f 6e73 653a 2043 656e     Response: Cen
+00035880: 7472 616c 4150 4920 5265 7370 6f6e 7365  tralAPI Response
+00035890: 206f 626a 6563 740a 2020 2020 2020 2020   object.        
+000358a0: 2222 220a 2020 2020 2020 2020 7572 6c20  """.        url 
+000358b0: 3d20 6622 2f63 6c6f 7564 6175 7468 2f61  = f"/cloudauth/a
+000358c0: 7069 2f76 332f 6275 6c6b 2f7b 7570 6c6f  pi/v3/bulk/{uplo
+000358d0: 6164 5f74 7970 657d 2f73 7461 7475 7322  ad_type}/status"
+000358e0: 0a0a 2020 2020 2020 2020 7061 7261 6d73  ..        params
+000358f0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00035900: 2027 7373 6964 273a 2073 7369 640a 2020   'ssid': ssid.  
+00035910: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00035920: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+00035930: 6c66 2e67 6574 2875 726c 2c20 7061 7261  lf.get(url, para
+00035940: 6d73 3d70 6172 616d 7329 0a0a 2020 2020  ms=params)..    
+00035950: 6173 796e 6320 6465 6620 636c 6f75 6461  async def clouda
+00035960: 7574 685f 6765 745f 6d70 736b 5f6e 6574  uth_get_mpsk_net
+00035970: 776f 726b 7328 0a20 2020 2020 2020 2073  works(.        s
+00035980: 656c 662c 0a20 2020 2029 202d 3e20 5265  elf,.    ) -> Re
+00035990: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+000359a0: 2222 2252 6561 6420 616c 6c20 636f 6e66  """Read all conf
+000359b0: 6967 7572 6564 204d 5053 4b20 6e65 7477  igured MPSK netw
+000359c0: 6f72 6b73 2e0a 0a20 2020 2020 2020 2052  orks...        R
+000359d0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+000359e0: 2020 2020 5265 7370 6f6e 7365 3a20 4365      Response: Ce
+000359f0: 6e74 7261 6c41 5049 2052 6573 706f 6e73  ntralAPI Respons
+00035a00: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
+00035a10: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
+00035a20: 203d 2022 2f63 6c6f 7564 4175 7468 2f61   = "/cloudAuth/a
+00035a30: 7069 2f76 322f 6d70 736b 220a 0a20 2020  pi/v2/mpsk"..   
+00035a40: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+00035a50: 7420 7365 6c66 2e67 6574 2875 726c 290a  t self.get(url).
+00035a60: 0a20 2020 2061 7379 6e63 2064 6566 2063  .    async def c
+00035a70: 6c6f 7564 6175 7468 5f67 6574 5f6e 616d  loudauth_get_nam
+00035a80: 6564 6d70 736b 280a 2020 2020 2020 2020  edmpsk(.        
+00035a90: 7365 6c66 2c0a 2020 2020 2020 2020 6d70  self,.        mp
+00035aa0: 736b 5f69 643a 2073 7472 2c0a 2020 2020  sk_id: str,.    
+00035ab0: 2020 2020 6e61 6d65 3a20 7374 7220 3d20      name: str = 
+00035ac0: 4e6f 6e65 2c0a 2020 2020 2020 2020 726f  None,.        ro
+00035ad0: 6c65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  le: str = None,.
+00035ae0: 2020 2020 2020 2020 7374 6174 7573 3a20          status: 
+00035af0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00035b00: 2020 2020 6375 7273 6f72 3a20 7374 7220      cursor: str 
+00035b10: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00035b20: 736f 7274 3a20 7374 7220 3d20 4e6f 6e65  sort: str = None
+00035b30: 2c0a 2020 2020 2020 2020 6c69 6d69 743a  ,.        limit:
+00035b40: 2069 6e74 203d 2031 3030 2c0a 2020 2020   int = 100,.    
+00035b50: 2920 2d3e 2052 6573 706f 6e73 653a 0a20  ) -> Response:. 
+00035b60: 2020 2020 2020 2022 2222 5265 6164 2061         """Read a
+00035b70: 6c6c 206e 616d 6564 204d 5053 4b2e 0a0a  ll named MPSK...
+00035b80: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00035b90: 2020 2020 2020 2020 2020 6d70 736b 5f69            mpsk_i
+00035ba0: 6420 2873 7472 293a 2054 6865 204d 5053  d (str): The MPS
+00035bb0: 4b20 636f 6e66 6967 7572 6174 696f 6e20  K configuration 
+00035bc0: 4944 0a20 2020 2020 2020 2020 2020 206e  ID.            n
+00035bd0: 616d 6520 2873 7472 2c20 6f70 7469 6f6e  ame (str, option
+00035be0: 616c 293a 2046 696c 7465 7220 6279 206e  al): Filter by n
+00035bf0: 616d 6520 6f66 2074 6865 206e 616d 6564  ame of the named
+00035c00: 204d 5053 4b2e 2044 6f65 7320 6120 2763   MPSK. Does a 'c
+00035c10: 6f6e 7461 696e 7327 206d 6174 6368 2e0a  ontains' match..
+00035c20: 2020 2020 2020 2020 2020 2020 726f 6c65              role
+00035c30: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
+00035c40: 3a20 4669 6c74 6572 2062 7920 726f 6c65  : Filter by role
+00035c50: 206f 6620 7468 6520 6e61 6d65 6420 4d50   of the named MP
+00035c60: 534b 2e20 446f 6573 2061 6e20 2765 7175  SK. Does an 'equ
+00035c70: 616c 7327 206d 6174 6368 2e0a 2020 2020  als' match..    
+00035c80: 2020 2020 2020 2020 7374 6174 7573 2028          status (
+00035c90: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+00035ca0: 4669 6c74 6572 2062 7920 7374 6174 7573  Filter by status
+00035cb0: 206f 6620 7468 6520 6e61 6d65 6420 4d50   of the named MP
+00035cc0: 534b 2e20 446f 6573 2061 6e20 2765 7175  SK. Does an 'equ
+00035cd0: 616c 7327 206d 6174 6368 2e0a 2020 2020  als' match..    
+00035ce0: 2020 2020 2020 2020 2020 2020 5661 6c69              Vali
+00035cf0: 6420 5661 6c75 6573 3a20 656e 6162 6c65  d Values: enable
+00035d00: 642c 2064 6973 6162 6c65 640a 2020 2020  d, disabled.    
+00035d10: 2020 2020 2020 2020 6375 7273 6f72 2028          cursor (
+00035d20: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+00035d30: 466f 7220 6375 7273 6f72 2062 6173 6564  For cursor based
+00035d40: 2070 6167 696e 6174 696f 6e2e 0a20 2020   pagination..   
+00035d50: 2020 2020 2020 2020 2073 6f72 7420 2873           sort (s
+00035d60: 7472 2c20 6f70 7469 6f6e 616c 293a 2053  tr, optional): S
+00035d70: 6f72 7420 6f72 6465 7220 2056 616c 6964  ort order  Valid
+00035d80: 2056 616c 7565 733a 202b 6e61 6d65 2c20   Values: +name, 
+00035d90: 2d6e 616d 652c 202b 726f 6c65 2c20 2d72  -name, +role, -r
+00035da0: 6f6c 652c 202b 7374 6174 7573 2c0a 2020  ole, +status,.  
+00035db0: 2020 2020 2020 2020 2020 2020 2020 2d73                -s
+00035dc0: 7461 7475 730a 2020 2020 2020 2020 2020  tatus.          
+00035dd0: 2020 6c69 6d69 7420 2869 6e74 2c20 6f70    limit (int, op
+00035de0: 7469 6f6e 616c 293a 204e 756d 6265 7220  tional): Number 
+00035df0: 6f66 2069 7465 6d73 2074 6f20 6265 2066  of items to be f
+00035e00: 6574 6368 6564 2044 6566 6175 6c74 7320  etched Defaults 
+00035e10: 746f 2031 3030 2e0a 0a20 2020 2020 2020  to 100...       
+00035e20: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00035e30: 2020 2020 2020 5265 7370 6f6e 7365 3a20        Response: 
+00035e40: 4365 6e74 7261 6c41 5049 2052 6573 706f  CentralAPI Respo
+00035e50: 6e73 6520 6f62 6a65 6374 0a20 2020 2020  nse object.     
+00035e60: 2020 2022 2222 0a20 2020 2020 2020 2075     """.        u
+00035e70: 726c 203d 2066 222f 636c 6f75 6441 7574  rl = f"/cloudAut
+00035e80: 682f 6170 692f 7632 2f6d 7073 6b2f 7b6d  h/api/v2/mpsk/{m
+00035e90: 7073 6b5f 6964 7d2f 6e61 6d65 644d 5053  psk_id}/namedMPS
+00035ea0: 4b22 0a0a 2020 2020 2020 2020 7061 7261  K"..        para
+00035eb0: 6d73 203d 207b 0a20 2020 2020 2020 2020  ms = {.         
+00035ec0: 2020 2027 6e61 6d65 273a 206e 616d 652c     'name': name,
+00035ed0: 0a20 2020 2020 2020 2020 2020 2027 726f  .            'ro
+00035ee0: 6c65 273a 2072 6f6c 652c 0a20 2020 2020  le': role,.     
+00035ef0: 2020 2020 2020 2027 7374 6174 7573 273a         'status':
+00035f00: 2073 7461 7475 732c 0a20 2020 2020 2020   status,.       
+00035f10: 2020 2020 2027 6375 7273 6f72 273a 2063       'cursor': c
+00035f20: 7572 736f 722c 0a20 2020 2020 2020 2020  ursor,.         
+00035f30: 2020 2027 736f 7274 273a 2073 6f72 742c     'sort': sort,
+00035f40: 0a20 2020 2020 2020 2020 2020 2027 6c69  .            'li
+00035f50: 6d69 7427 3a20 6c69 6d69 740a 2020 2020  mit': limit.    
+00035f60: 2020 2020 7d0a 0a20 2020 2020 2020 2072      }..        r
+00035f70: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+00035f80: 2e67 6574 2875 726c 2c20 7061 7261 6d73  .get(url, params
+00035f90: 3d70 6172 616d 7329 0a0a 2020 2020 6173  =params)..    as
+00035fa0: 796e 6320 6465 6620 636c 6f75 6461 7574  ync def cloudaut
+00035fb0: 685f 646f 776e 6c6f 6164 5f6d 7073 6b5f  h_download_mpsk_
+00035fc0: 6373 7628 0a20 2020 2020 2020 2073 656c  csv(.        sel
+00035fd0: 662c 0a20 2020 2020 2020 2073 7369 643a  f,.        ssid:
+00035fe0: 2073 7472 2c0a 2020 2020 2020 2020 6669   str,.        fi
+00035ff0: 6c65 6e61 6d65 3a20 7374 7220 3d20 4e6f  lename: str = No
+00036000: 6e65 2c0a 2020 2020 2020 2020 6e61 6d65  ne,.        name
+00036010: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00036020: 2020 2020 2020 726f 6c65 3a20 7374 7220        role: str 
+00036030: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00036040: 7374 6174 7573 3a20 7374 7220 3d20 4e6f  status: str = No
+00036050: 6e65 2c0a 2020 2020 2020 2020 736f 7274  ne,.        sort
+00036060: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00036070: 2020 2920 2d3e 2052 6573 706f 6e73 653a    ) -> Response:
+00036080: 0a20 2020 2020 2020 2022 2222 4665 7463  .        """Fetc
+00036090: 6820 616c 6c20 4e61 6d65 6420 4d50 534b  h all Named MPSK
+000360a0: 2061 7320 6120 4353 5620 6669 6c65 2e0a   as a CSV file..
+000360b0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+000360c0: 2020 2020 2020 2020 2020 2073 7369 6420             ssid 
+000360d0: 2873 7472 293a 2043 6f6e 6669 6775 7265  (str): Configure
+000360e0: 6420 4d50 534b 2053 5349 4420 666f 7220  d MPSK SSID for 
+000360f0: 7768 6963 6820 4e61 6d65 6420 4d50 534b  which Named MPSK
+00036100: 7320 6172 6520 746f 2062 6520 646f 776e  s are to be down
+00036110: 6c6f 6164 6564 2e0a 2020 2020 2020 2020  loaded..        
+00036120: 2020 2020 6669 6c65 6e61 6d65 2028 7374      filename (st
+00036130: 722c 206f 7074 696f 6e61 6c29 3a20 5375  r, optional): Su
+00036140: 6767 6573 7420 6120 6669 6c65 206e 616d  ggest a file nam
+00036150: 6520 666f 7220 7468 6520 646f 776e 6c6f  e for the downlo
+00036160: 6164 696e 6720 6669 6c65 2076 6961 2063  ading file via c
+00036170: 6f6e 7465 6e74 0a20 2020 2020 2020 2020  ontent.         
+00036180: 2020 2020 2020 2064 6973 706f 7369 7469         dispositi
+00036190: 6f6e 2068 6561 6465 722e 0a20 2020 2020  on header..     
+000361a0: 2020 2020 2020 206e 616d 6520 2873 7472         name (str
+000361b0: 2c20 6f70 7469 6f6e 616c 293a 2046 696c  , optional): Fil
+000361c0: 7465 7220 6279 206e 616d 6520 6f66 2074  ter by name of t
+000361d0: 6865 206e 616d 6564 204d 5053 4b2e 2044  he named MPSK. D
+000361e0: 6f65 7320 6120 2763 6f6e 7461 696e 7327  oes a 'contains'
+000361f0: 206d 6174 6368 2e0a 2020 2020 2020 2020   match..        
+00036200: 2020 2020 726f 6c65 2028 7374 722c 206f      role (str, o
+00036210: 7074 696f 6e61 6c29 3a20 4669 6c74 6572  ptional): Filter
+00036220: 2062 7920 726f 6c65 206f 6620 7468 6520   by role of the 
+00036230: 6e61 6d65 6420 4d50 534b 2e20 446f 6573  named MPSK. Does
+00036240: 2061 6e20 2765 7175 616c 7327 206d 6174   an 'equals' mat
+00036250: 6368 2e0a 2020 2020 2020 2020 2020 2020  ch..            
+00036260: 7374 6174 7573 2028 7374 722c 206f 7074  status (str, opt
+00036270: 696f 6e61 6c29 3a20 4669 6c74 6572 2062  ional): Filter b
+00036280: 7920 7374 6174 7573 206f 6620 7468 6520  y status of the 
+00036290: 6e61 6d65 6420 4d50 534b 2e20 446f 6573  named MPSK. Does
+000362a0: 2061 6e20 2765 7175 616c 7327 206d 6174   an 'equals' mat
+000362b0: 6368 2e0a 2020 2020 2020 2020 2020 2020  ch..            
+000362c0: 2020 2020 5661 6c69 6420 5661 6c75 6573      Valid Values
+000362d0: 3a20 656e 6162 6c65 642c 2064 6973 6162  : enabled, disab
+000362e0: 6c65 640a 2020 2020 2020 2020 2020 2020  led.            
+000362f0: 736f 7274 2028 7374 722c 206f 7074 696f  sort (str, optio
+00036300: 6e61 6c29 3a20 536f 7274 206f 7264 6572  nal): Sort order
+00036310: 2020 5661 6c69 6420 5661 6c75 6573 3a20    Valid Values: 
+00036320: 2b6e 616d 652c 202d 6e61 6d65 2c20 2b72  +name, -name, +r
+00036330: 6f6c 652c 202d 726f 6c65 2c20 2b73 7461  ole, -role, +sta
+00036340: 7475 732c 0a20 2020 2020 2020 2020 2020  tus,.           
+00036350: 2020 2020 202d 7374 6174 7573 0a0a 2020       -status..  
+00036360: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00036370: 2020 2020 2020 2020 2020 2052 6573 706f             Respo
+00036380: 6e73 653a 2043 656e 7472 616c 4150 4920  nse: CentralAPI 
+00036390: 5265 7370 6f6e 7365 206f 626a 6563 740a  Response object.
+000363a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000363b0: 2020 2020 7572 6c20 3d20 222f 636c 6f75      url = "/clou
+000363c0: 6441 7574 682f 6170 692f 7632 2f64 6f77  dAuth/api/v2/dow
+000363d0: 6e6c 6f61 642f 6d70 736b 220a 0a20 2020  nload/mpsk"..   
+000363e0: 2020 2020 2070 6172 616d 7320 3d20 7b0a       params = {.
+000363f0: 2020 2020 2020 2020 2020 2020 2773 7369              'ssi
+00036400: 6427 3a20 7373 6964 2c0a 2020 2020 2020  d': ssid,.      
+00036410: 2020 2020 2020 2766 696c 656e 616d 6527        'filename'
+00036420: 3a20 6669 6c65 6e61 6d65 2c0a 2020 2020  : filename,.    
+00036430: 2020 2020 2020 2020 276e 616d 6527 3a20          'name': 
+00036440: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00036450: 2020 2772 6f6c 6527 3a20 726f 6c65 2c0a    'role': role,.
+00036460: 2020 2020 2020 2020 2020 2020 2773 7461              'sta
+00036470: 7475 7327 3a20 7374 6174 7573 2c0a 2020  tus': status,.  
+00036480: 2020 2020 2020 2020 2020 2773 6f72 7427            'sort'
+00036490: 3a20 736f 7274 0a20 2020 2020 2020 207d  : sort.        }
+000364a0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000364b0: 2061 7761 6974 2073 656c 662e 6765 7428   await self.get(
+000364c0: 7572 6c2c 2070 6172 616d 733d 7061 7261  url, params=para
+000364d0: 6d73 290a 0a20 2020 2061 7379 6e63 2064  ms)..    async d
+000364e0: 6566 2067 6574 5f75 7365 725f 6163 636f  ef get_user_acco
+000364f0: 756e 7473 280a 2020 2020 2020 2020 7365  unts(.        se
+00036500: 6c66 2c0a 2020 2020 2020 2020 6170 705f  lf,.        app_
+00036510: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
+00036520: 2c0a 2020 2020 2020 2020 7479 7065 3a20  ,.        type: 
+00036530: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00036540: 2020 2020 7374 6174 7573 3a20 7374 7220      status: str 
+00036550: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00036560: 6f72 6465 725f 6279 3a20 7374 7220 3d20  order_by: str = 
+00036570: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f66  None,.        of
+00036580: 6673 6574 3a20 696e 7420 3d20 302c 0a20  fset: int = 0,. 
+00036590: 2020 2020 2020 206c 696d 6974 3a20 696e         limit: in
+000365a0: 7420 3d20 3130 302c 0a20 2020 2029 202d  t = 100,.    ) -
+000365b0: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
+000365c0: 2020 2020 2222 224c 6973 7420 7573 6572      """List user
+000365d0: 2061 6363 6f75 6e74 732e 0a0a 2020 2020   accounts...    
+000365e0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+000365f0: 2020 2020 2020 6170 705f 6e61 6d65 2028        app_name (
+00036600: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+00036610: 4170 706e 616d 6520 6e6d 7320 746f 2066  Appname nms to f
+00036620: 696c 7465 7220 4172 7562 6120 4365 6e74  ilter Aruba Cent
+00036630: 7261 6c20 7573 6572 732c 2061 6e64 2061  ral users, and a
+00036640: 6363 6f75 6e74 5f73 6574 7469 6e67 0a20  ccount_setting. 
+00036650: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00036660: 6f20 6669 6c74 6572 2048 5045 2047 7265  o filter HPE Gre
+00036670: 656e 4c61 6b65 2045 6467 6520 746f 2043  enLake Edge to C
+00036680: 6c6f 7564 2050 6c61 7466 6f72 6d20 2843  loud Platform (C
+00036690: 4353 2920 6170 706c 6963 6174 696f 6e20  CS) application 
+000366a0: 7573 6572 7320 2056 616c 6964 0a20 2020  users  Valid.   
+000366b0: 2020 2020 2020 2020 2020 2020 2056 616c               Val
+000366c0: 7565 733a 206e 6d73 2c20 6163 636f 756e  ues: nms, accoun
+000366d0: 745f 7365 7474 696e 670a 2020 2020 2020  t_setting.      
+000366e0: 2020 2020 2020 7479 7065 2028 7374 722c        type (str,
+000366f0: 206f 7074 696f 6e61 6c29 3a20 4669 6c74   optional): Filt
+00036700: 6572 2062 6173 6564 206f 6e20 7379 7374  er based on syst
+00036710: 656d 206f 7220 6665 6465 7261 7465 6420  em or federated 
+00036720: 7573 6572 2020 5661 6c69 6420 5661 6c75  user  Valid Valu
+00036730: 6573 3a20 7379 7374 656d 2c0a 2020 2020  es: system,.    
+00036740: 2020 2020 2020 2020 2020 2020 6665 6465              fede
+00036750: 7261 7465 640a 2020 2020 2020 2020 2020  rated.          
+00036760: 2020 7374 6174 7573 2028 7374 722c 206f    status (str, o
+00036770: 7074 696f 6e61 6c29 3a20 4669 6c74 6572  ptional): Filter
+00036780: 2075 7365 7220 6261 7365 6420 6f6e 2073   user based on s
+00036790: 7461 7475 7320 2869 6e70 726f 6772 6573  tatus (inprogres
+000367a0: 732c 2066 6169 6c65 6429 2020 5661 6c69  s, failed)  Vali
+000367b0: 6420 5661 6c75 6573 3a0a 2020 2020 2020  d Values:.      
+000367c0: 2020 2020 2020 2020 2020 696e 7072 6f67            inprog
+000367d0: 7265 7373 2c20 6661 696c 6564 0a20 2020  ress, failed.   
+000367e0: 2020 2020 2020 2020 206f 7264 6572 5f62           order_b
+000367f0: 7920 2873 7472 2c20 6f70 7469 6f6e 616c  y (str, optional
+00036800: 293a 2053 6f72 7420 6f72 6465 7269 6e67  ): Sort ordering
+00036810: 2028 6173 6365 6e64 696e 6720 6f72 2064   (ascending or d
+00036820: 6573 6365 6e64 696e 6729 2e20 2b75 7365  escending). +use
+00036830: 726e 616d 6520 7369 676e 6966 6965 730a  rname signifies.
+00036840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00036850: 6173 6365 6e64 696e 6720 6f72 6465 7220  ascending order 
+00036860: 6f66 2075 7365 726e 616d 652e 2020 5661  of username.  Va
+00036870: 6c69 6420 5661 6c75 6573 3a20 2b75 7365  lid Values: +use
+00036880: 726e 616d 652c 202d 7573 6572 6e61 6d65  rname, -username
+00036890: 0a20 2020 2020 2020 2020 2020 206f 6666  .            off
+000368a0: 7365 7420 2869 6e74 2c20 6f70 7469 6f6e  set (int, option
+000368b0: 616c 293a 205a 6572 6f20 6261 7365 6420  al): Zero based 
+000368c0: 6f66 6673 6574 2074 6f20 7374 6172 7420  offset to start 
+000368d0: 6672 6f6d 2044 6566 6175 6c74 7320 746f  from Defaults to
+000368e0: 2030 2e0a 2020 2020 2020 2020 2020 2020   0..            
+000368f0: 6c69 6d69 7420 2869 6e74 2c20 6f70 7469  limit (int, opti
+00036900: 6f6e 616c 293a 204d 6178 696d 756d 206e  onal): Maximum n
+00036910: 756d 6265 7220 6f66 2069 7465 6d73 2074  umber of items t
+00036920: 6f20 7265 7475 726e 2044 6566 6175 6c74  o return Default
+00036930: 7320 746f 2031 3030 2e0a 0a20 2020 2020  s to 100...     
+00036940: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00036950: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
+00036960: 3a20 4365 6e74 7261 6c41 5049 2052 6573  : CentralAPI Res
+00036970: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
+00036980: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00036990: 2075 726c 203d 2022 2f70 6c61 7466 6f72   url = "/platfor
+000369a0: 6d2f 7262 6163 2f76 312f 7573 6572 7322  m/rbac/v1/users"
+000369b0: 0a0a 2020 2020 2020 2020 7061 7261 6d73  ..        params
+000369c0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+000369d0: 2027 6170 705f 6e61 6d65 273a 2061 7070   'app_name': app
+000369e0: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
+000369f0: 2020 2027 7479 7065 273a 2074 7970 652c     'type': type,
+00036a00: 0a20 2020 2020 2020 2020 2020 2027 7374  .            'st
+00036a10: 6174 7573 273a 2073 7461 7475 732c 0a20  atus': status,. 
+00036a20: 2020 2020 2020 2020 2020 2027 6f72 6465             'orde
+00036a30: 725f 6279 273a 206f 7264 6572 5f62 792c  r_by': order_by,
+00036a40: 0a20 2020 2020 2020 2020 2020 2027 6f66  .            'of
+00036a50: 6673 6574 273a 206f 6666 7365 742c 0a20  fset': offset,. 
+00036a60: 2020 2020 2020 2020 2020 2027 6c69 6d69             'limi
+00036a70: 7427 3a20 6c69 6d69 740a 2020 2020 2020  t': limit.      
+00036a80: 2020 7d0a 0a20 2020 2020 2020 2023 2054    }..        # T
+00036a90: 4f44 4f20 7468 6973 206e 6565 6473 2061  ODO this needs a
+00036aa0: 2066 6169 7220 616d 6f75 6e74 206f 6620   fair amount of 
+00036ab0: 6d61 7373 6167 696e 6720 746f 2074 7572  massaging to tur
+00036ac0: 6e20 696e 746f 2061 2063 6f6d 6d61 6e64  n into a command
+00036ad0: 2c20 6974 2773 206e 6573 7465 6420 6469  , it's nested di
+00036ae0: 6374 730a 2020 2020 2020 2020 2320 6578  cts.        # ex
+00036af0: 616d 706c 6520 7265 7370 6f6e 7365 2069  ample response i
+00036b00: 6e20 7072 6976 6174 6520 7673 636f 6465  n private vscode
+00036b10: 2064 6972 2e0a 2020 2020 2020 2020 7265   dir..        re
+00036b20: 7370 203d 2061 7761 6974 2073 656c 662e  sp = await self.
+00036b30: 6765 7428 7572 6c2c 2070 6172 616d 733d  get(url, params=
+00036b40: 7061 7261 6d73 290a 2020 2020 2020 2020  params).        
+00036b50: 7265 7475 726e 2072 6573 700a 0a69 6620  return resp..if 
+00036b60: 5f5f 6e61 6d65 5f5f 203d 3d20 225f 5f6d  __name__ == "__m
+00036b70: 6169 6e5f 5f22 3a0a 2020 2020 7061 7373  ain__":.    pass
+00036b80: 0a                                       .
```

### Comparing `centralcli-5.0.0/centralcli/cleaner.py` & `centralcli-5.1.0/centralcli/cleaner.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     if pkg_dir.name == "centralcli":
         sys.path.insert(0, str(pkg_dir.parent))
         from centralcli import constants, log, utils
     else:
         print(pkg_dir.parts)
         raise e
 
-from centralcli.constants import DevTypes, StatusOptions
+from centralcli.constants import DevTypes, StatusOptions, LLDPCapabilityTypes
 from centralcli.objects import DateTime
 from centralcli.models import CloudAuthUploadResponse
 
 
 def epoch_convert(func):
     @functools.wraps(func)
     def wrapper(epoch):
@@ -229,14 +229,19 @@
     "firmware_version": lambda v: v if not v or len(set(v.split("-"))) == len(v.split("-")) else "-".join(v.split("-")[1:]),
     "learn_time": _log_timestamp,
     "last_state_change": _log_timestamp,
     "graceful_restart_timer": _duration_words,
     "disable_ssid": lambda v: '✅' if not v else '❌', # field is changed to "enabled" check: \u2705 x: \u274c
     "poe_detection_status": lambda i: constants.PoEDetectionStatus(i).name,
     "reserved_power_in_watts": lambda v: round(v, 2),
+    "speed": lambda v: "1000BaseT FD" if v == "1000BaseTFD - Four-pair Category 5 UTP, full duplex mode" else v,
+    "ec": lambda v: v if not isinstance(v, list) else ", ".join([LLDPCapabilityTypes(ec).name.replace("_", " ") for ec in v]),
+    "sc": lambda v: v if not isinstance(v, list) else ", ".join([LLDPCapabilityTypes(ec).name.replace("_", " ") for ec in v]),
+    "chassis_id_type": lambda v: None,
+    "chassis_id_type_str": lambda v: None,
     # "enabled": lambda v: not v, # field is changed to "enabled"
     # "allowed_vlan": lambda v: str(sorted(v)).replace(" ", "").strip("[]")
 }
 
 _short_key = {
     "interface_port": "interface",
     "firmware_version": "version",
@@ -308,14 +313,17 @@
     "poe_detection_status": "status",
     "power_drawn_in_watts": "draw",
     "pse_allocated_power": "allocated",
     "reserved_power_in_watts": "reserved",
     "power_class": "class",
     "cluster_group_name": "group",
     "cluster_redundancy_type": "redundancy type",
+    "ec": "enabled capabilities",
+    "sc": "system capabilities",
+    "ec_str": "enabled capabilities"
 }
 
 
 def strip_outer_keys(data: dict) -> Union[list, dict]:
     """strip unnecessary wrapping key from API response payload
 
     Args:
@@ -1014,19 +1022,20 @@
 def get_lldp_neighbor(data: List[Dict[str, str]]) -> Dict[str: Dict[str, str]]:
     data = utils.listify(data)
     strip_keys = ["cid"]
     _short_val = {
         "1000BaseTFD - Four-pair Category 5 UTP, full duplex mode": "1000BaseT FD"
     }
     # grab the key details from switch lldp return, make data look closer to lldp return from AP
+
     if data and "dn" in data[0].keys():
         data = [{**dict(d if "dn" not in d else d["dn"]), "vlan_id": ",".join(d.get("vlan_id", [])), "lldp_poe": d.get("lldp_poe_enabled")} for d in data]
         data = sort_interfaces(data, interface_key="port")
     # simplify some of the values and strip the bond0 entry from AP
-    data = [{k: _short_val.get(d[k], d[k]) for k in d if d.get("localPort", "") != "bond0" and k not in strip_keys} for d in data]
+    data = [dict(short_value(k, d[k]) for k in d if d.get("localPort", "") != "bond0" and k not in strip_keys) for d in data]
 
     return strip_no_value(data)
 
 
 def get_vlans(data: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
     short_keys = {
         # site
@@ -1406,14 +1415,20 @@
     data = [
         dict(short_value(k, d.get(k, "")) for k in field_order) for d in data
     ]
     data = strip_no_value(data)
 
     return data
 
+
+def get_portal_profile(data: List[Dict[str, Any]]) -> Dict[str, Any]:
+    # _display_output will listify the dict prior to sending it in as most outputs are List[dict]
+    data = utils.unlistify(data)
+    return {k: v for k, v in data.items() if k != "logo"}
+
 def get_ospf_neighbor(data: Union[List[dict], dict],) -> Union[List[dict], dict]:
     data = utils.listify(data)
 
     # send all key/value pairs through formatters and return
     # swapping "address" for ip here as address is also used for site address
     data = [
         dict(short_value(k if k != "address" else "ip", v) for k, v in inner.items()) for inner in data
```

### Comparing `centralcli-5.0.0/centralcli/cli.py` & `centralcli-5.1.0/centralcli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 try:
     import psutil
     hook_enabled = True
 except (ImportError, ModuleNotFoundError):
     hook_enabled = False
 
 err_console = Console(stderr=True)
+clean_console = Console(emoji=False)
 
 # Detect if called from pypi installed package or via cloned github repo (development)
 try:
     from centralcli import (Response, cleaner, cli, cliadd, cliassign,
                             clibatch, clicaas, cliclone, clidel, clikick, cliset,
                             clirefresh, clirename, clishow, clitest, clitshoot,
                             cliunassign, cliupdate, cliupgrade, cliexport,
@@ -129,15 +130,14 @@
                                 envvar="ARUBACLI_ACCOUNT",
                                 help="The Aruba Central Account to use (must be defined in the config)",
                                 autocompletion=cli.cache.account_completion),
 ) -> None:
     """Move device(s) to a defined group and/or site.
     """
     central = cli.central
-    console = Console()
 
     # For the benefit of the help text
     # kw1_val = site
     # kw2_val = group
     # TODO reverted as breaks completion logic would need to modif dev_kwarg_completion
     group, site, = None, None
     device = device or ()
@@ -160,16 +160,15 @@
         print(f"Warning [cyan italic]--reset-group[/] flag ignored as destination group {group} was provided")
 
     site = site or _site
     if site:
         _site = cli.cache.get_site_identifier(site)
 
     if not group and not site:
-        print("Missing Required Argument, group and/or site is required.")
-        raise typer.Exit(1)
+        cli.exit("Missing Required Argument, group and/or site is required.")
 
     # TODO improve logic.  if they are moving to a group we can use inventory as backup
     # BUT if they are moving to a site it has to be connected to central first.  So would need to be in cache
     dev = [cli.cache.get_dev_identifier(d, include_inventory=True) for d in device]
     if any([d is None for d in dev]):
         # cache lookup failed... will happen if device has not connected yet
         inv = cli.central.request(cli.central.get_device_inventory)
@@ -192,15 +191,15 @@
         else:
             devs_by_type[d.generic_type] += [d]
         dev_all_names += [f"[reset][cyan]{d.name}[/]|[cyan]{d.serial}[/]"]
         dev_all_serials += [d.serial]
 
         if site and d.get("site"):
             if d.site == _site.name:  # device is already in desired site
-                console.print(f"[dark_orange]:warning:[/] {d.rich_help_text} is already in Site: {_site.summary_text}")
+                clean_console.print(f"\u26a0  {d.rich_help_text} is already in Site: {_site.summary_text}")  # \u26a0 is :warning: we need emoji off
                 if not group:  # remove serial from devs_by_type if already in desired site, and site move is the only operation
                     _ = devs_by_type[d.generic_type].pop(len(devs_by_type[d.generic_type]) - 1)
                     if not devs_by_type[d.generic_type]:  # if type list is empty remove the type
                         del devs_by_type[d.generic_type]
                 continue
 
             if f"{d.site}~|~{d.generic_type}" not in devs_by_site:
@@ -209,27 +208,28 @@
                 devs_by_site[f"{d.site}~|~{d.generic_type}"] += [d]
 
     if len(dev_all_names) > 2:
         _msg_devs = ", ".join(dev_all_names)
     else:
         _msg_devs = " & ".join(dev_all_names)
 
+    # Build confirmation message
     confirm_msg = f"[bright_green]Move[/] {_msg_devs}\n"
     if group:
         _group = CentralObject("group", {"name": "unprovisioned"}) if group.lower() == "unprovisioned" else cli.cache.get_group_identifier(group)
         confirm_msg += f"  To Group: [cyan]{_group.name}[/]\n"
         if cx_retain_config:
             confirm_msg += "  [italic]Config for CX switches will be preserved during move.[/]\n"
     if site:
         # _site = cli.cache.get_site_identifier(site)
         confirm_msg += f"  To Site: [cyan]{_site.name}[/]\n"
         if devs_by_site:
             confirm_msg += "\n  [italic bright_red]Devices will be removed from current sites.[/]\n"
 
-    print(confirm_msg)
+    clean_console.print(confirm_msg)
     confirmed = True if yes or typer.confirm("\nProceed?", abort=True) else False
     # TODO currently will ask to confirm even if it will result in no calls (dev already in site) Need to build reqs list
     #      Then ask for confirmation if there are reqs to perform...  Need to refactor/simplify
 
     # TODO can probably be cleaner.  list of site_rm_reqs, list of group/site mv reqs do requests at end
     # If devices are associated with a site currently remove them from that site first
     # FIXME moving 3 devices from one site to another no longer works correctly (disassociated 2 then 1, (2 calls) then added 1)
@@ -488,15 +488,15 @@
         func = cli.central.send_command_to_device
         arg = dev.serial
         if swarm:
             print(f":warning:  Ignoring -s|--swarm option, as it only applies to APs not {dev.type}\n")
     else:  # AP all others will error in get_dev_identifier
         func = cli.central.send_command_to_swarm
         arg = dev.swack_id
-        if dev.version.startswith("10."):  # TODO add aos8 vs aos10 flag to dev cache
+        if dev.version.startswith("10."):
             cli.exit("This command is only valid for [cyan]AOS8[/] IAP clusters not [cyan]AOS10[/] APs")
         elif not swarm:
             cli.exit("This command is only valid for the entire swarm in AOS8, not individual APs.  Use [green]-s[/]|[cyan]--swarm[/] to default the entire IAP cluster")
         else:
             conf_msg = f'the [cyan]swarm {dev.name}[/] belongs to'
 
     console = Console(emoji=False)
@@ -888,14 +888,15 @@
     final_config = utils.generate_template(template, var_file=var_file)
     cli.display_results(data=final_config.splitlines(), outfile=outfile)
 
 
 
 
 def all_commands_callback(ctx: typer.Context, update_cache: bool):
+    # --raw and --debug-limit are honored and stripped out in init
     if ctx.resilient_parsing:
         config.is_completion = True
     if not ctx.resilient_parsing:
         version, account, debug, debugv, default, update_cache = None, None, None, None, None, None
         for idx, arg in enumerate(sys.argv[1:]):
             if idx == 0 and arg in ["-v", "-V", "--version"]:
                 version = True
@@ -922,16 +923,14 @@
             cli.version_callback(ctx)
             raise typer.Exit(0)
         if default:
             if "--account " in str(sys.argv) and account not in ["central_info", "default"]:
                 err_console.print(f":warning:  Both [cyan]-d[/] and [cyan]--account[/] flag used.  Honoring [cyan]-d[/], ignoring account [cyan]{account}[/]")
                 account = config.default_account
             cli.account_name_callback(ctx, account=config.default_account, default=True)
-            # default = cli.default_callback(ctx, True)
-        # elif account:
         else:
             cli.account_name_callback(ctx, account=account)
 
         if debug:
             cli.debug_callback(ctx, debug=debug)
         if debugv:
             log.DEBUG = config.debug = log.verbose = config.debugv = debugv
```

### Comparing `centralcli-5.0.0/centralcli/cliadd.py` & `centralcli-5.1.0/centralcli/cliadd.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/cliassign.py` & `centralcli-5.1.0/centralcli/cliassign.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clibatch.py` & `centralcli-5.1.0/centralcli/clibatch.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clicaas.py` & `centralcli-5.1.0/centralcli/clicaas.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/cliclone.py` & `centralcli-5.1.0/centralcli/cliclone.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,27 +26,24 @@
 
 
 @app.command(short_help="Clone a group")
 def group(
     clone_group: str = typer.Argument(..., metavar="[NAME OF GROUP TO CLONE]", autocompletion=cli.cache.group_completion),
     new_group: str = typer.Argument(..., metavar="[NAME OF GROUP TO CREATE]"),
     aos10: bool = typer.Option(None, "--aos10", help="Upgrade new cloned group to AOS10"),
-    yes: bool = typer.Option(False, "-Y", help="Bypass confirmation prompts - Assume Yes"),
-    yes_: bool = typer.Option(False, "-y", hidden=True),
+    yes: bool = typer.Option(False, "-Y", "-y", help="Bypass confirmation prompts - Assume Yes"),
     debug: bool = typer.Option(False, "--debug", envvar="ARUBACLI_DEBUG", help="Enable Additional Debug Logging",
                                callback=cli.debug_callback),
-    default: bool = typer.Option(False, "-d", is_flag=True, help="Use default central account", show_default=False,
-                                 callback=cli.default_callback),
-    account: str = typer.Option("central_info",
-                                envvar="ARUBACLI_ACCOUNT",
-                                help="The Aruba Central Account to use (must be defined in the config)",
-                                callback=cli.account_name_callback),
+    default: bool = typer.Option(False, "-d", is_flag=True, help="Use default central account", show_default=False,),
+    account: str = typer.Option(
+        "central_info",
+        envvar="ARUBACLI_ACCOUNT",
+        help="The Aruba Central Account to use (must be defined in the config)",
+    ),
 ) -> None:
-    yes = yes_ if yes_ else yes
-
     print(f"Clone group: {color(clone_group)} to new group {color(new_group)}")
     if aos10:
         print(f"    Upgrade cloned group to AOS10: {color(True)}")
         print(
             "\n    [dark_orange]WARNING[/dark_orange]: [italic]Upgrade doesn't always work despite "
             f"returning {color('success')},\n    Group is cloned if {color('success')} is returned "
             "but upgrade to AOS10 may not occur.\n    API method appears to have some caveats."
```

### Comparing `centralcli-5.0.0/centralcli/clicommon.py` & `centralcli-5.1.0/centralcli/clicommon.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from centralcli.central import CentralApi
 from centralcli.objects import DateTime, Encoder
 
 
 tty = utils.tty
 CASE_SENSITIVE_TOKENS = ["R", "U"]
-TableFormat = Literal["json", "yaml", "csv", "rich", "simple", "tabulate", "raw", "action"]
+TableFormat = Literal["json", "yaml", "csv", "rich", "simple", "tabulate", "raw", "action", "clean"]
 MsgType = Literal["initial", "previous", "forgot", "will_forget", "previous_will_forget"]
 console = Console(emoji=False)
 err_console = Console(emoji=False, stderr=True)
 
 
 class CLICommon:
     def __init__(self, account: str = "default", cache: Cache = None, central: CentralApi = None, raw_out: bool = False):
@@ -325,21 +325,24 @@
                     "Used simple string conversion"
 
             print("[italic green]Done")
             if out_msg:
                 log.warning(out_msg, show=True)
 
     @staticmethod
-    def exit(msg: str, code: int = 1) -> None:
-        """Print error text and exit.
+    def exit(msg: str = None, code: int = 1) -> None:
+        """Print msg text and exit.
+
+        Prepends warning emoji to msg if code indicates an error.
         """
         if code != 0:
-            msg = f":warning:  {msg}"
+            msg = f":warning:  {msg}" if msg else msg
 
-        print(msg)
+        if msg:
+            print(msg)
         raise typer.Exit(code=code)
 
     def _display_results(
         self,
         data: Union[List[dict], List[str], dict, None] = None,
         tablefmt: str = "rich",
         title: str = None,
@@ -513,15 +516,15 @@
                     "GET": "bright_green",
                     "DELETE": "red",
                     "PATCH": "dark_orange3",
                     "PUT": "dark_orange3",
                     "POST": "dark_orange3"
                 }
                 fg = "bright_green" if r else "red"
-                conditions = [len(resp) > 1, tablefmt in ["action", "raw"], r.ok and not r.output]
+                conditions = [len(resp) > 1, tablefmt in ["action", "raw", "clean"], r.ok and not r.output]
                 if any(conditions):
                     _url = r.url if not hasattr(r.url, "path") else r.url.path
                     m_color = m_colors.get(r.method, "reset")
                     print(
                         f"Request {idx + 1} [[{m_color}]{r.method}[reset]: "
                         f"[cyan]{_url}[/cyan]]\n [fg]Response[reset]:"
                     )
@@ -532,29 +535,37 @@
                 # Nothing returned in response payload
                 if not r.output:
                     print(f"  Status Code: [{fg}]{r.status}[/]")
                     print("  :warning: Empty Response.  This may be normal.")
                 elif not cleaner and r.url and r.url.path == "/caasapi/v1/exec/cmd":
                     cleaner = clean.parse_caas_response
 
-                if not r or tablefmt in ["action", "raw"]:
+                if not r or tablefmt in ["action", "raw", "clean"]:
 
                     # raw output (unformatted response from Aruba Central API GW)
-                    if tablefmt == "raw":
+                    if tablefmt in ["raw", "clean"]:
                         status_code = f"[{fg}]status code: {r.status}[/{fg}]"
                         print(r.url)
                         print(status_code)
                         if not r.ok:
                             print(r.error)
-                        print("[bold cyan]Unformatted response from Aruba Central API GW[/bold cyan]")
-                        plain_console = Console(color_system=None, emoji=False)
-                        plain_console.print(r.raw)
+
+                        if tablefmt == "clean":
+                            typer.echo_via_pager(r.output) if pager else typer.echo(r.output)
+                        else:
+                            print("[bold cyan]Unformatted response from Aruba Central API GW[/bold cyan]")
+                            plain_console = Console(color_system=None, emoji=False)
+                            if pager:
+                                with plain_console.pager:
+                                    plain_console.print(r.raw)
+                            else:
+                                plain_console.print(r.raw)
 
                         if outfile:
-                            self.write_file(outfile, r.raw)
+                            self.write_file(outfile, r.raw if tablefmt != "clean" else r.output)
 
                     # prints the Response objects __str__ method which includes status_code
                     # and formatted contents of any payload. example below
                     # status code: 201
                     # Success
                     else:
                         console.print(f"[{fg}]{r}[/]")
```

### Comparing `centralcli-5.0.0/centralcli/clidel.py` & `centralcli-5.1.0/centralcli/clidel.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clidelfirmware.py` & `centralcli-5.1.0/centralcli/clidelfirmware.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/cliexport.py` & `centralcli-5.1.0/centralcli/cliexport.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clikick.py` & `centralcli-5.1.0/centralcli/clikick.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clirefresh.py` & `centralcli-5.1.0/centralcli/clirefresh.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clirename.py` & `centralcli-5.1.0/centralcli/clirename.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/cliset.py` & `centralcli-5.1.0/centralcli/cliset.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clisetfirmware.py` & `centralcli-5.1.0/centralcli/clisetfirmware.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clishow.py` & `centralcli-5.1.0/centralcli/clishow.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from __future__ import annotations
 import typer
 import time
 import pendulum
 import asyncio
 import sys
 import json
-from typing import List, Iterable, Literal
+import os
+from typing import List, Iterable, Literal, Dict
 from pathlib import Path
 from rich import print
 from rich.console import Console
 from copy import deepcopy
 
 try:
     import psutil
@@ -50,55 +51,100 @@
 app.add_typer(clishowaudit.app, name="audit")
 app.add_typer(clishowcloudauth.app, name="cloud-auth")
 app.add_typer(clishowmpsk.app, name="mpsk")
 
 tty = utils.tty
 iden_meta = IdenMetaVars()
 
+class Counts:
+    def __init__(self, total: int, up: int, not_checked_in: int, down: int = None ):
+        self.total = total
+        self.up = up
+        self.inventory = not_checked_in
+        self.down = down or total - not_checked_in - up
+
 def _build_caption(resp: Response, *, inventory: bool = False, dev_type: GenericDevTypes = None, status: Literal["Up", "Down"] = None) -> str:
+    inventory_only = False  # toggled while building cnt_str if no devices have status (meaning called from show inventory)
     def get_switch_counts(data) -> dict:
         dev_types = set([t.get("switch_type", "ERR") for t in data])
         # return {LIB_DEV_TYPE.get(_type, _type): [t for t in data if t.get("switch_type", "ERR") == _type] for _type in dev_types}
         return {
             LIB_DEV_TYPE.get(_type, _type): {
                 "total": len(list(filter(lambda x: x["switch_type"] == _type, data))),
                 "up": len(list(filter(lambda x: x["switch_type"] == _type and x["status"] == "Up", data)))
             }
             for _type in dev_types
         }
 
+    def get_counts(data: List[Dict], dev_type: Literal["cx", "sw", "ap", "gw"]) -> Counts:
+        _match_type = [d for d in data if d["type"] == dev_type]
+        _tot = len(_match_type)
+        _up = len([d for d in _match_type if d.get("status") and d["status"] == "Up"])
+        _inv = len([d for d in _match_type if not d.get("status")])
+        return Counts(_tot, _up, _inv)
+
+
     if not dev_type:
-        counts_by_type = {**{k: {"total": resp.raw[k][0]["total"], "up": len(list(filter(lambda x: x["status"], resp.raw[k][0][k])))} for k in resp.raw.keys() if k != "switches"}, **get_switch_counts(resp.raw["switches"][0]["switches"])}
-        status_by_type = {LIB_DEV_TYPE.get(_type, _type): {"total": counts_by_type[_type]["total"], "up": counts_by_type[_type]["up"], "down": counts_by_type[_type]["total"] - counts_by_type[_type]["up"]} for _type in counts_by_type}
+        if inventory:  # cencli show inventory -v or cencli show all --inv
+            status_by_type = {}
+            _types = set(d["type"] for d in resp.output)
+            for t in _types:
+                counts = get_counts(resp.output, t)
+                status_by_type[t] = {"total": counts.total, "up": counts.up, "down": counts.down, "inventory_only": counts.inventory}
+
+        else:  # show all [--inv], or show ivnentory -v
+            counts_by_type = {**{k: {"total": resp.raw[k][0]["total"], "up": len(list(filter(lambda x: x["status"], resp.raw[k][0][k])))} for k in resp.raw.keys() if k != "switches"}, **get_switch_counts(resp.raw["switches"][0]["switches"])}
+            status_by_type = {LIB_DEV_TYPE.get(_type, _type): {"total": counts_by_type[_type]["total"], "up": counts_by_type[_type]["up"], "down": counts_by_type[_type]["total"] - counts_by_type[_type]["up"]} for _type in counts_by_type}
     elif dev_type == "switch":
         counts_by_type = get_switch_counts(resp.raw["switches"])
         status_by_type = {LIB_DEV_TYPE.get(_type, _type): {"total": counts_by_type[_type]["total"], "up": counts_by_type[_type]["up"], "down": counts_by_type[_type]["total"] - counts_by_type[_type]["up"]} for _type in counts_by_type}
     else:
         _tot = len(resp)
         _up = len(list(filter(lambda a: a["status"] == "Up", resp.output)))
         _down = _tot - _up
         status_by_type = {dev_type: {"total": _tot, "up": _up, "down": _down}}
 
+    # Put together counts caption string
     if status:
         _cnt_str = ", ".join([f'[{"bright_green" if status.lower() == "up" else "red"}]{t}[/]: [cyan]{status_by_type[t]["total"]}[/]' for t in status_by_type])
+    elif inventory:
+        def _get_inv_msg(data: Dict, dev_type: DevTypes) -> str:
+            inv_str = '' if not data["inventory_only"] else f" Not checked in: [cyan]{data['inventory_only']}[/]"
+            up_down_str = '' if data["up"] + data["down"] == 0 else f'([bright_green]{data["up"]}[/]:[red]{data["down"]}[/])'
+            return f'[{"bright_green" if not data["down"] else "red"}]{dev_type}[/]: [cyan]{data["total"]}[/] {up_down_str}{inv_str if up_down_str else ""}'
+
+        _cnt_str = f"Total in inventory: [cyan]{len(resp.output)}[/], "
+        _cnt_str = _cnt_str + ", ".join(
+            [f'{_get_inv_msg(status_by_type[t], t)}' for t in status_by_type]
+        )
+        if "(" not in _cnt_str:
+            inventory_only = True
     else:
         _cnt_str = ", ".join([f'[{"bright_green" if not status_by_type[t]["down"] else "red"}]{t}[/]: [cyan]{status_by_type[t]["total"]}[/] ([bright_green]{status_by_type[t]["up"]}[/]:[red]{status_by_type[t]["down"]}[/])' for t in status_by_type])
 
     if status is None or status.lower() != "down":
         try:
             clients = sum([t.get("client_count", 0) for t in resp.output if t.get("client_count") != "-"])
-            _cnt_str = f"{_cnt_str}, [bright_green]clients[/]: [cyan]{clients}[/]"
+            if clients:
+                _cnt_str = f"{_cnt_str}, [bright_green]clients[/]: [cyan]{clients}[/]"
         except Exception as e:
             log.exception(f"Exception occured in _build_caption\n{e}")
 
-    caption = "  [cyan]Show all[/cyan] displays fields common to all device types. "
-    caption = f"[reset]{'Counts' if not status else f'{status} Devices'}: {_cnt_str}\n{caption}To see all columns for a given device use [cyan]show <DEVICE TYPE>[/cyan]" if not dev_type else f"[reset]Counts: {_cnt_str}"
+    if not inventory_only:
+        caption = "  [cyan]cencli show all[/cyan]|[cyan]cencli show inventory -v[/cyan] displays fields common to all device types. "
+        caption = f"[reset]{'Counts' if not status else f'{status} Devices'}: {_cnt_str}\n{caption}"
+        if not dev_type:
+            caption = f"{caption} To see all columns for a given device use [cyan]cencli show <DEVICE TYPE>[/cyan]"
+        else:
+            caption = f"[reset]Counts: {_cnt_str}"
+    else:
+        caption = f"[reset]Counts: {_cnt_str}"
 
-    if inventory:
-        caption = f"{caption}\n  [italic green3]verbose listing, devices lacking name/ip are in the inventory, but have not connected to central.[/]"
+    if inventory and not inventory_only:
+        caption = f"{caption}\n  [italic green3]Devices lacking name/ip are in the inventory, but have not connected to central.[/]"
     return caption
 
 def show_devices(
     devices: str | Iterable[str] = None, dev_type: Literal["all", "ap", "gw", "cx", "sw", "switch"] = None, include_inventory: bool = False, verbosity: int = 0, outfile: Path = None,
     update_cache: bool = False, group: str = None, site: str = None, label: str = None, status: str = None, state: str = None, pub_ip: str = None,
     do_clients: bool = True, do_stats: bool = False, do_ssids: bool = False, sort_by: str = None, reverse: bool = False, pager: bool = False, do_json: bool = False, do_csv: bool = False,
     do_yaml: bool = False, do_table: bool = False
@@ -221,14 +267,30 @@
         sort_by=sort_by,
         reverse=reverse,
         output_by_key=output_key,
         cleaner=cleaner.get_devices,
         verbosity=verbosity,
     )
 
+def download_logo(resp: Response, path: Path, portal: CentralObject) -> None:
+    if not resp.output.get("logo"):
+        cli.exit(f"Unable to download logo image.  A logo has not been applied to the {resp.output['name']} portal")
+
+    import base64
+    file = path / resp.output["logo_name"] if path.is_dir() else path
+    if not os.access(file.parent, os.W_OK):
+        cli.exit(f"{file.parent} is not writable")
+
+    img_data = base64.b64decode(resp.output["logo"].split(",")[1])
+    if file.write_bytes(img_data):
+        cli.exit(f"Logo saved to {file}", code=0)
+    else:
+        cli.exit(
+            f"Check {file}, write operation indicated no bytes were written.  Use [cyan]cencli show portals {portal.name} --raw[/] to see raw response including logo data."
+        )
 
 @app.command("all")
 def all_(
     group: str = typer.Option(None, help="Filter by Group", autocompletion=cli.cache.group_completion, show_default=False,),
     site: str = typer.Option(None, help="Filter by Site", autocompletion=cli.cache.site_completion, show_default=False,),
     label: str = typer.Option(None, help="Filter by Label", autocompletion=cli.cache.label_completion,show_default=False,),
     status: StatusOptions = typer.Option(None, metavar="[up|down]", hidden=True, help="Filter by device status"),
@@ -681,29 +743,30 @@
     elif dev_type == "ap":
         title = "APs in Inventory"
     elif dev_type == "vgw":
         title = "Virtual Gateways in Inventory"
     else:
         title = "Inventory"
 
+    if verbose:
+        show_devices(
+            dev_type='all', outfile=outfile, include_inventory=verbose, do_clients=True, sort_by=sort_by, reverse=reverse,
+            pager=pager, do_json=do_json, do_csv=do_csv, do_yaml=do_yaml, do_table=do_table
+        )
+        cli.exit("", code=0)
+
     resp = cli.central.request(cli.cache.update_inv_db, dev_type=lib_to_api("inventory", dev_type), sub=sub)
-    if verbose:  # TODO just pass this to all_() so output is consistent
-        cache_devices = cli.cache.devices
-        for idx, dev in enumerate(resp.output):
-            from_cache = [d for d in cache_devices if d["serial"] == dev["serial"]]
-            if from_cache:
-                resp.output[idx] = {**dev, **from_cache[0]}
 
     cli.display_results(
         resp,
         tablefmt=tablefmt,
         title=title,
         sort_by=sort_by,
         reverse=reverse,
-        caption=None if not verbose else _build_caption(resp, inventory=True),
+        caption=_build_caption(resp, inventory=True),
         pager=pager,
         outfile=outfile,
         cleaner=None,  # Cleaner is applied in cache update
     )
 
 
 # TODO --sort option for date fields sorts converted value, needs to be sorted by epoch before conversion
@@ -1495,19 +1558,20 @@
         help="The Aruba Central Account to use (must be defined in the config)",
         autocompletion=cli.cache.account_completion,
     ),
 ) -> None:
     """Show AP lldp neighbor
 
     Valid on APs and CX switches
-    Command will run on AOS-SW, but neighbor table will only show neighbors that are CX switches or APs
+
+    Use [cyan]cencli show aps -n --site <SITE>[/] to see lldp neighbors for all APs in a site.
+    NOTE: AOS-SW will return LLDP neighbors, but only it reports neighbors for connected Aruba devices managed in Central
     """
     central = cli.central
 
-    # TODO need get_dev_identier to accept cx
     devs: List[CentralObject] = [cli.cache.get_dev_identifier(_dev, dev_type=("ap", "switch"), conductor_only=True,) for _dev in device if not _dev.lower().startswith("neighbor")]
     batch_reqs = [BatchRequest(central.get_ap_lldp_neighbor, (dev.serial,)) for dev in devs if dev.type == "ap"]
     batch_reqs += [BatchRequest(central.get_cx_switch_neighbors, (dev.serial,)) for dev in devs if dev.generic_type == "switch" and not dev.swack_id]
     unique_stack_ids = set([dev.swack_id for dev in devs if dev.generic_type == "switch" and dev.swack_id])
     batch_reqs += [BatchRequest(central.get_cx_switch_stack_neighbors, (swack_id,)) for swack_id in unique_stack_ids]
     batch_resp = central.batch_request(batch_reqs)
     # if all([res.ok for res in batch_resp]):
@@ -1520,14 +1584,15 @@
         title = f"{dev.name} LLDP Neighbor information"
         if tablefmt not in ["table", "rich"]:
             console.print(f'[green]{"-" * 5}[/] [cyan bold]{title}[/] [green]{"-" * 5}[/]')
         cli.display_results(
             r,
             tablefmt=tablefmt,
             title=title,
+            caption = "  :warning:  [italic dark_olive_green2]AOS-SW only reflects LLDP neighbors that are managed by Aruba Central[/]" if dev.type == "sw" else None,
             pager=pager,
             outfile=outfile,
             output_by_key=["port", "localPort"],
             cleaner=cleaner.get_lldp_neighbor,
         )
 
 @app.command(short_help="Show certificates/details")
@@ -1633,30 +1698,21 @@
         tablefmt = None
 
     cli.display_results(resp, tablefmt=tablefmt, pager=pager, outfile=outfile)
 
 
 # TODO --status does not work
 # https://web.yammer.com/main/org/hpe.com/threads/eyJfdHlwZSI6IlRocmVhZCIsImlkIjoiMTQyNzU1MDg5MTQ0MjE3NiJ9
-@app.command(
-    "config",
-    short_help="Show Central Group/Device or cencli Config",
-    help=(
-        "Show Effective Group/Device Config (UI Group) or cencli config."
-        "    Examples: 'cencli show config GROUPNAME --gw', "
-        "'cencli show config DEVICENAME', "
-        "'cencli show config cencli'"
-    ),
-)
+@app.command("config")
 def config_(
     group_dev: str = typer.Argument(
         ...,
         metavar=f"{iden_meta.group_dev_cencli}",
         autocompletion=cli.cache.group_dev_ap_gw_completion,
-        help = "Device Identifier for (AP or GW), Group Name along with --ap or --gw option, or 'cencli' to see cencli configuration details.",
+        help = "Device Identifier, Group Name along with --ap or --gw option, or 'cencli' to see cencli configuration details.",
         show_default=False,
     ),
     device: str = typer.Argument(
         None,
         autocompletion=cli.cache.dev_ap_gw_completion,
         hidden=True,
         show_default=False,
@@ -1683,19 +1739,31 @@
     account: str = typer.Option(
         "central_info",
         envvar="ARUBACLI_ACCOUNT",
         help="The Aruba Central Account to use (must be defined in the config)",
         autocompletion=cli.cache.account_completion,
     ),
 ) -> None:
+    """Show Effective Group/Device Config (UI Group) or cencli config.
+
+    Group level configs are available for APs or GWs.
+    Device level configs are available for all device types, however
+    AP and GW, show what Aruba Central has configured at the group or device level.
+    Switches fetch the running config from the device.  [italic]Same as [cyan]cencli show run[/cyan][/italic].
+
+    Examples:
+    \t[cyan]cencli show config GROUPNAME --gw[/]\tCentral's Group level config for a GW
+    \t[cyan]cencli show config DEVICENAME[/]\t\tCentral's device level config if device is AP or GW, or running config from device if switch
+    \t[cyan]cencli show config cencli[/]\t\tcencli configuration information (from config.yaml)
+    """
     if group_dev == "cencli":  # Hidden show cencli config
         return _get_cencli_config()
 
     group_dev: CentralObject = cli.cache.get_identifier(group_dev, ["group", "dev"], device_type=["ap", "gw"])
-    if all:
+    if all:  # TODO move this either to cliexport or clibatch (cencli batch export configs)
         if not any([do_gw, do_ap]):
             print(":warning:  Invalid combination [cyan]--all[/] requires [cyan]--ap[/] or [cyan]--gw[/] flag.")
             raise typer.Exit(1)
         elif not group_dev.is_group:
             print(":warning:  Invalid combination [cyan]--all[/] requires first argument to be a group")
             raise typer.Exit(1)
         else:  # TODO make this a sep func  Allow site as first arg
@@ -1739,49 +1807,51 @@
             raise typer.Exit(0)
 
     if group_dev.is_group:
         group = group_dev
         if device:
             device = cli.cache.get_dev_identifier(device)
         elif not do_ap and not do_gw:
-            print(":warning:  Invalid Input, --gw or --ap option must be supplied for group level config.")
-            raise typer.Exit(1)
+            cli.exit("Invalid Input, --gw or --ap option must be supplied for group level config.")
     else:  # group_dev is a device iden
         group = cli.cache.get_group_identifier(group_dev.group)
         if device is not None:
-            print(":warning:  Invalid input enter \[[cyan]Group[/]] \[[cyan]device iden[/]] or \[[cyan]device iden[/]]")
-            raise typer.Exit(1)
+            cli.exit("Invalid input enter \[[cyan]Group[/]] \[[cyan]device iden[/]] or \[[cyan]device iden[/]]")
         else:
             device = group_dev
 
     _data_key = None
     if do_gw or (device and device.generic_type == "gw"):
         if device and device.generic_type != "gw":
-            print(f":warning:  Invalid input: --gw option conflicts with {device.name} which is an {device.generic_type}")
-            raise typer.Exit(1)
+            cli.exit(f"Invalid input: --gw option conflicts with {device.name} which is an {device.generic_type}")
         caasapi = caas.CaasAPI(central=cli.central)
         if not status:
             func = caasapi.show_config
             _data_key = "config"
         else:
             func = caasapi.get_config_status
     elif do_ap or (device and device.generic_type == "ap"):
         if device:
             if device.generic_type == "ap":
                 func = cli.central.get_per_ap_config
                 args = [device.serial]
             else:
-                print(f":warning:  Invalid input: --ap option conflicts with {device.name} which is a {device.generic_type}")
-                raise typer.Exit(1)
+                cli.exit(f"Invalid input: --ap option conflicts with {device.name} which is a {device.generic_type}")
         else:
             func = cli.central.get_ap_config
             args = [group.name]
+    elif device and device.type == "cx":
+        clitshoot.send_cmds_by_id(device, commands=[6002], pager=pager, outfile=outfile)
+        cli.exit(code=0)
+    elif device and device.type == "sw":
+        clitshoot.send_cmds_by_id(device, commands=[1022], pager=pager, outfile=outfile)
+        cli.exit(code=0)
     else:
-        print(f"This command is currently only supported for gw and ap, not {device.generic_type}")
-        raise typer.Exit(1)
+        log.error("Command Logic Failure, Please report this on GitHub.  Failed to determine appropriate function for provided arguments/options", show=True)
+        cli.exit()
 
     # Build arguments cli.central method associated with each device type supported.
     if device:
         if device.generic_type == "ap" or status:
             args = [device.serial]
         else:
             args = [group.name, device.mac]
@@ -2937,33 +3007,77 @@
     ),
 ) -> None:
     """Show archived devices"""
     resp = cli.central.request(cli.central.get_archived_devices)
     cli.display_results(resp, tablefmt="yaml")
 
 
-# TODO cahce portal/name ids
+# TODO sort_by / reverse tablefmt options add verbosity 1 to cleaner
 @app.command()
 def portals(
+    portal: List[str] = typer.Argument(
+        None,
+        metavar="[name|id]",
+        help="show details for a specific portal profile [grey42]\[default: show summary for all portals][/]",
+        autocompletion=cli.cache.portal_completion,
+        show_default=False,),
+    logo: bool = typer.Option(
+        False,
+        "-L", "--logo",
+        metavar="PATH",
+        help=f"Download logo for specified portal to specified path. [cyan]Portal argument is requrired[/] [grey42]\[default: {Path.cwd()}/<original_logo_filename>[/]]",
+        show_default = False,
+        writable=True,
+    ),
+    sort_by: str = typer.Option(None, "--sort", help="Field to sort by", show_default=False,),
+    reverse: bool = typer.Option(False, "-r", is_flag=True, help="Sort in descending order"),
+    do_json: bool = typer.Option(False, "--json", is_flag=True, help="Output in JSON", hidden=False),
+    do_yaml: bool = typer.Option(False, "--yaml", is_flag=True, help="Output in YAML", hidden=True),
+    do_csv: bool = typer.Option(False, "--csv", is_flag=True, help="Output in CSV"),
+    do_table: bool = typer.Option(False, "--table", help="Output in table format",),
+    outfile: Path = typer.Option(None, "--out", help="Output to file (and terminal)", writable=True, show_default=False,),
+    pager: bool = typer.Option(False, "--pager", help="Enable Paged Output"),
     default: bool = typer.Option(
         False, "-d", is_flag=True, help="Use default central account", show_default=False,
     ),
     debug: bool = typer.Option(
         False, "--debug", envvar="ARUBACLI_DEBUG", help="Enable Additional Debug Logging",
     ),
     account: str = typer.Option(
         "central_info",
         envvar="ARUBACLI_ACCOUNT",
         help="The Aruba Central Account to use (must be defined in the config)",
         autocompletion=cli.cache.account_completion,
     ),
 ) -> None:
-    """Show Configured Guest Portals"""
-    resp = cli.central.request(cli.central.get_portals)
-    cli.display_results(resp, cleaner=cleaner.get_portals, fold_cols=["url"],)
+    """Show Configured Guest Portals, details for a specific portal, or download logo for a specified portal"""
+    path = Path.cwd()
+    if portal and len(portal) > 2:
+        cli.exit("Too many Arguments")
+    elif len(portal) > 1:
+        if not logo:
+            cli.exit("Too many Arguments")
+        path = Path(portal[-1])
+        if not path.is_dir() and not path.parent.is_dir():
+            cli.exit(f"[cyan]{path.parent}[/] directory not found, provide full path with filename, or an existing directory to use original filename")
+
+    portal = portal[0] if portal else portal
+
+    if portal is None:
+        resp: Response = cli.central.request(cli.cache.update_portal_db)
+        _cleaner = cleaner.get_portals
+    else:
+        p: CentralObject = cli.cache.get_name_id_identifier("portal", portal)
+        resp: Response = cli.central.request(cli.central.get_portal_profile, p.id)
+        _cleaner = cleaner.get_portal_profile
+        if logo and resp.ok:
+            download_logo(resp, path, p)  # this will exit CLI after writing to file
+
+    tablefmt = cli.get_format(do_json=do_json, do_yaml=do_yaml, do_csv=do_csv, do_table=do_table, default="yaml" if portal else "rich")
+    cli.display_results(resp, tablefmt=tablefmt, title="Portals", pager=pager, outfile=outfile, sort_by=sort_by, reverse=reverse, cleaner=_cleaner, fold_cols=["url"],)
 
 
 # TODO add sort_by completion
 @app.command()
 def guests(
     portal_id: str = typer.Argument(..., ),
     sort_by: str = typer.Option(None, "--sort", help="Field to sort by"),
```

### Comparing `centralcli-5.0.0/centralcli/clishowaudit.py` & `centralcli-5.1.0/centralcli/clishowaudit.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clishowbranch.py` & `centralcli-5.1.0/centralcli/clishowbranch.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clishowcloudauth.py` & `centralcli-5.1.0/centralcli/clishowcloudauth.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clishowfirmware.py` & `centralcli-5.1.0/centralcli/clishowfirmware.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clishowmpsk.py` & `centralcli-5.1.0/centralcli/clishowmpsk.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clishowospf.py` & `centralcli-5.1.0/centralcli/clishowospf.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clishowoverlay.py` & `centralcli-5.1.0/centralcli/clishowoverlay.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clishowtshoot.py` & `centralcli-5.1.0/centralcli/clishowtshoot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import typer
 import sys
 from pathlib import Path
 from rich import print
-from rich.console import Console
 
 
 # Detect if called from pypi installed package or via cloned github repo (development)
 try:
     from centralcli import cleaner, cli
 except (ImportError, ModuleNotFoundError) as e:
     pkg_dir = Path(__file__).absolute().parent
@@ -30,30 +29,31 @@
 
 
 @app.command(short_help="Show Troubleshooting output")
 def results(
     device: str = typer.Argument(
         ...,
         metavar=iden_meta.dev,
-        help="Aruba Central Device",
+        help="Aruba Central Device or the session id of a previously run troubleshooting session",
         autocompletion=cli.cache.dev_completion,
         show_default=False,
     ),
     session_id: str = typer.Argument(
         None,
         help="The troubleshooting session id.",
         show_default=False,
     ),
-    verbose2: bool = typer.Option(
+    clean: bool = typer.Option(
         False,
-        "-vv",
-        help="Show raw response (no formatting but still honors --yaml, --csv ... if provided)",
+        "--clean",
+        help="Clean response, don't send through any formatters.  [grey42 italic]Useful for excessively long output[/]",
         show_default=False,
     ),
     pager: bool = typer.Option(False, "--pager", help="Enable Paged Output",),
+    outfile: Path = typer.Option(None, "--out", help="Output to file (and terminal)", writable=True, show_default=False,),
     default: bool = typer.Option(
         False, "-d",
         is_flag=True,
         help="Use default central account",
         show_default=False,
     ),
     debug: bool = typer.Option(
@@ -67,42 +67,44 @@
         "central_info",
         envvar="ARUBACLI_ACCOUNT",
         help="The Aruba Central Account to use (must be defined in the config)",
         autocompletion=cli.cache.account_completion,
     ),
 ) -> None:
     """
-    [cyan]Show Troubleshooting results from an existing session.[/]
+    [cyan]Show Troubleshooting results from a previously run troubleshooting session.[/]
 
     Use [cyan]cencli tshoot...[/] to start a troubleshooting session.
 
     """
     central = cli.central
-    con = Console(emoji=False)
     dev = cli.cache.get_dev_identifier(device)
 
     # Fetch session ID if not provided
     if not session_id:
         resp = central.request(central.get_ts_session_id, dev.serial)
         if resp.ok and "session_id" in resp.output:
             session_id = resp.output["session_id"]
         else:
             print(f"No session id provided, unable to find active session id for {dev.name}")
-            cli.display_results(resp)
-            raise typer.Exit(1)
+            cli.display_results(resp, exit_on_fail=True)
 
     title = f"Troubleshooting output for {dev.name} session {session_id}"
+
     resp = central.request(central.get_ts_output, dev.serial, session_id=session_id)
     if not resp or resp.output.get("status", "") != "COMPLETED":
         cli.display_results(resp, title=title, tablefmt="rich",)
-    elif verbose2:
-        cli.display_results(resp)
     else:
-        con.print(resp)
-        con.print(f"\n   {resp.rl}")
+        if "output" in resp.output:
+            _output = resp.output["output"]
+            del resp.output["output"]
+            cli.display_results(resp, tablefmt="action")
+            resp.output = _output
+
+        cli.display_results(resp, pager=pager, outfile=outfile, tablefmt="simple" if not clean else "clean")
 
 
 @app.command(short_help="Show available troubleshooting commands")
 def commands(
     device_type: TSDevTypes = typer.Argument(..., metavar=iden_meta.dev_types_w_mas, show_default=False,),
     sort_by: SortTsCmdOptions = typer.Option("id", "--sort",),
     reverse: bool = typer.Option(False, "-r", help="Reverse output order", show_default=False,),
```

### Comparing `centralcli-5.0.0/centralcli/clishowwids.py` & `centralcli-5.1.0/centralcli/clishowwids.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clitest.py` & `centralcli-5.1.0/centralcli/clitest.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/clitshoot.py` & `centralcli-5.1.0/centralcli/clitshoot.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,23 +51,25 @@
 
     complete = False
     while not complete:
         for x in range(3):
             _delay = 15 if device.type == "cx" else 10
             for _ in track(range(_delay), description="[green]Allowing time for commands to complete[/]..."):
                 sleep(1)
-            # with console.status("Waiting for Troubleshooting Response..."):
-            #     sleep(10)
+
             ts_resp = cli.central.request(cli.central.get_ts_output, device.serial, resp.session_id)
 
             if ts_resp.output.get("status", "") == "COMPLETED":
                 lines = "\n".join([line for line in ts_resp.output["output"].splitlines() if line != " "])
                 ts_resp.raw = ts_resp.output["output"]
                 ts_resp.output = lines
-                cli.display_results(ts_resp, pager=pager, outfile=outfile)
+                show_tech_ap = [115, 369, 465]
+                tablefmt = "clean" if sorted(commands) != show_tech_ap else "raw"
+
+                cli.display_results(ts_resp, pager=pager, outfile=outfile, tablefmt=tablefmt)
                 complete = True
                 break
             else:
                 print(f'{ts_resp.output.get("message", " . ").split(".")[0]}. [cyan]Waiting...[/]')
 
 
         if not complete:
```

### Comparing `centralcli-5.0.0/centralcli/cliunassign.py` & `centralcli-5.1.0/centralcli/cliunassign.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/cliupdate.py` & `centralcli-5.1.0/centralcli/cliupdate.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from rich.console import Console
 from jinja2 import FileSystemLoader, Environment
 import yaml
 import asyncio
 
 # Detect if called from pypi installed package or via cloned github repo (development)
 try:
-    from centralcli import utils, cli, caas, cleaner, config
+    from centralcli import utils, cli, caas, cleaner
 except (ImportError, ModuleNotFoundError) as e:
     pkg_dir = Path(__file__).absolute().parent
     if pkg_dir.name == "centralcli":
         sys.path.insert(0, str(pkg_dir.parent))
-        from centralcli import utils, cli, caas, cleaner, config
+        from centralcli import utils, cli, caas, cleaner
     else:
         print(pkg_dir.parts)
         raise e
 
 from centralcli.constants import IdenMetaVars, DevTypes, GatewayRole, state_abbrev_to_pretty
 from centralcli import CentralObject
 from centralcli.strings import LongHelp
```

### Comparing `centralcli-5.0.0/centralcli/cliupgrade.py` & `centralcli-5.1.0/centralcli/cliupgrade.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     default: bool = typer.Option(False, "-d", is_flag=True, help="Use default central account", show_default=False,),
     account: str = typer.Option("central_info",
                                 envvar="ARUBACLI_ACCOUNT",
                                 help="The Aruba Central Account to use (must be defined in the config)",),
 ) -> None:
     """Upgrade firmware on a device
     """
-    dev = cli.cache.get_dev_identifier(device, swack=True)
+    dev = cli.cache.get_dev_identifier(device, conductor_only=True)
     if dev.generic_type == "ap":
         reboot = True
     at = None if not at else int(round(at.timestamp()))
 
     ver_msg = "Recommended version" if not version else version
     ver_msg = f'Upgrade [cyan]{dev.name}[/] to [green3]{ver_msg}[/]'
     ver_msg = f"{ver_msg} and reboot" if reboot else f"{ver_msg} ('-R' not specified, [italic bright_red]device will not be rebooted[/])"
```

### Comparing `centralcli-5.0.0/centralcli/config.py` & `centralcli-5.1.0/centralcli/config.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/constants.py` & `centralcli-5.1.0/centralcli/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,21 +43,38 @@
 
 class SendConfigDevIdens(str, Enum):
     ap = "ap"
     gw = "gw"
     # sw = "sw"  # hopefully some day
     # cx = "cx"
 
-
 class PoEDetectionStatus(Enum):
     NA = 0
     Undefined = 1  # TODO figure out what this status is
     Searching = 2
     Delivering = 3
 
+# Here are all the types for the below Enum
+# 3: Bridge (Switch)
+# DOCSIS Cable Device
+# Other
+# Repeater
+# 5 but think 5: Router
+# Station
+# Telephone
+# 4: WLAN Access Point
+class LLDPCapabilityTypes(Enum):
+    unknown0 = 0
+    unknown1 = 1
+    unknown2 = 2
+    Bridge = 3  # 3 and 5 are assumption need to verify
+    Wlan_Access_Point = 4
+    Router = 5
+    unknown6 = 6
+    unknown7 = 7
 
 # Not used currently # TODO reference in cleaner
 class SwitchRoles(Enum):
     ERR = 0
     StandAlone = 1
     StackConductor = 2
     StackSecondary = 3
@@ -278,14 +295,15 @@
     licenses = "licenses"
     logs = "logs"
     events = "events"
     hook_config = "hook_config"
     hook_data = "hook_data"
     hook_active = "hook_active"
     mpsk = "mpsk"
+    portals = "portals"
 
 
 class KickArgs(str, Enum):
     all = "all"
     mac = "mac"
     wlan = "wlan"
```

### Comparing `centralcli-5.0.0/centralcli/logger.py` & `centralcli-5.1.0/centralcli/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
         """
         if not self._caption:
             return
         else:
             return "\n".join([f'  {msg}' for msg in self._caption])
 
     def log_print(self, msgs, log: bool = False, show: bool = False, caption: bool = False, level: str = 'info', *args, **kwargs):
-        # TODO can prob remove log_msgs, used by another project I re-used this object from (ConsolePi)
         msgs = [msgs] if not isinstance(msgs, list) else msgs
         _msgs = []
         _logged = []
         for i in msgs:
             i = str(i)
             if not self.DEBUG and [i for d in to_debug if d in i]:
                 continue
@@ -116,15 +115,15 @@
                 if i and i not in self.log_msgs:
                     _msgs.append(i)
 
         if show is not False and True in [show, self.show]:
             self.log_msgs += _msgs
             for m in self.log_msgs:
                 if console.is_terminal or environ.get("PYTEST_CURRENT_TEST"):
-                    emoji_console.print(f"{':warning:  ' if not level=='info' else ''}{m}")
+                    emoji_console.print(f"{':warning:  ' if level not in ['info', 'debug'] else ''}{m}")
             self.log_msgs = []
 
         if caption:
             self._caption = [*self._caption, *msgs]
 
     @property
     def level_name(self):
```

### Comparing `centralcli-5.0.0/centralcli/models.py` & `centralcli-5.1.0/centralcli/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,7 +607,24 @@
 class CacheMpskNetwork(BaseModel):
     id: str
     name: str = Field(alias="ssid")
 
 
 class CacheMpskNetworks(BaseModel):
     items: List[CacheMpskNetwork]
+
+
+class CachePortal(BaseModel):
+    name: str
+    id: str
+    url: str = Field(alias="capture_url")
+    auth_type: str
+    is_aruba_cert: bool
+    is_default: bool
+    is_editable: bool
+    is_shared: bool
+    register_accept_email: bool
+    register_accept_phone: bool
+
+
+class CachePortals(BaseModel):
+    portals: List[CachePortal]
```

### Comparing `centralcli-5.0.0/centralcli/objects.py` & `centralcli-5.1.0/centralcli/objects.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/render.py` & `centralcli-5.1.0/centralcli/render.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 from centralcli import constants
 from centralcli.config import Config
 from centralcli.objects import Encoder
 
 tty = utils.tty
 CASE_SENSITIVE_TOKENS = ["R", "U"]
-TableFormat = Literal["json", "yaml", "csv", "rich", "simple", "tabulate", "raw", "action"]
+TableFormat = Literal["json", "yaml", "csv", "rich", "tabulate", "simple"]  #, "raw", "action"]
 REDACT = ["mac", "serial", "neighborMac", "neighborSerial", "neighborPortMac", "longitude", "latitude"]
 RICH_FULL_COLS = ['mac', 'serial', 'ip', 'public ip', 'version', 'radio', 'id']
 RICH_FOLD_COLS = ["description"]
 console = Console(emoji=False)
 
 
 CUST_KEYS = ["customer_id", "customer_name", "cid", "cust_id"]
@@ -123,15 +123,20 @@
             _out += [
                 f"  {' ':{pad}}{line}" if isborder(line) or idx < data_start else f"{i}.{' ' * ipad}{line}"
             ]
         return "".join(_out)
 
     @property
     def file(self):
-        return "" if not self._file else typer.unstyle(self._file)
+        if not self._file:
+            return self.tty  # this should not happen
+        try:
+            return typer.unstyle(self._file)
+        except TypeError:
+            return self._file
 
 
 def do_pretty(key: str, value: str) -> str:
     """Apply coloring to tty output
 
     Applies color to certain columns/values prior to formatting
     """
@@ -313,15 +318,15 @@
 
         return raw_data, table_data
 
     return outdata, outdata
 
 def output(
     outdata: Union[List[str], Dict[str, Any]],
-    tablefmt: str = "rich",
+    tablefmt: TableFormat = "rich",  # "action" and "raw" are not sent through formatter, handled in clicommon.display_output
     title: str = None,
     caption: str = None,
     account: str = None,
     config: Config = None,
     output_by_key: str | List[str] = "name",
     set_width_cols: dict = None,
     full_cols: Union[List[str], str] = [],
@@ -331,16 +336,16 @@
     raw_data = outdata
     _lexer = table_data = None
 
     if config and config.sanitize and raw_data and all(isinstance(x, dict) for x in raw_data):
         outdata = [{k: d[k] if k not in REDACT else "--redacted--" for k in d} for d in raw_data]
 
     # -- // List[str, ...] \\ --  Bypass all formatters, (config file output, etc...)
-    if outdata and all(isinstance(x, str) for x in outdata):
-        tablefmt = "strings"
+    if tablefmt != "simple" and outdata and all(isinstance(x, str) for x in outdata):
+        tablefmt = "simple"
 
     # -- convert List[dict] --> Dict[dev_name: dict] for yaml/json outputs unless output_dict_by_key is specified, then use the provided key(s) rather than name
     if tablefmt in ['json', 'yaml', 'yml']:
         outdata = utils.listify(outdata)
         if output_by_key and outdata and isinstance(outdata[0], dict):
             if len(output_by_key) == 1 and "+" in output_by_key[0]:
                 found_keys = [k for k in output_by_key[0].split("+") if k in outdata[0]]
```

### Comparing `centralcli-5.0.0/centralcli/response.py` & `centralcli-5.1.0/centralcli/response.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/static/favicon.ico` & `centralcli-5.1.0/centralcli/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/strings.py` & `centralcli-5.1.0/centralcli/strings.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/utils.py` & `centralcli-5.1.0/centralcli/utils.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/vscodeargs.py` & `centralcli-5.1.0/centralcli/vscodeargs.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/wh2snow.py` & `centralcli-5.1.0/centralcli/wh2snow.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/centralcli/wh_proxy.py` & `centralcli-5.1.0/centralcli/wh_proxy.py`

 * *Files identical despite different names*

### Comparing `centralcli-5.0.0/pyproject.toml` & `centralcli-5.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "centralcli"
-version = "5.0.0"
+version = "5.1.0"
 description = "A CLI for interacting with Aruba Central (Cloud Management Platform).  Facilitates bulk imports, exports, reporting.  A handy tool if you have devices managed by Aruba Central."
 license = "MIT"
 authors = ["Wade Wells (Pack3tL0ss) <wade@consolepi.org>"]
 maintainers = ["Wade Wells (Pack3tL0ss) <wade@consolepi.org>"]
 readme = "README.md"
 repository = "https://github.com/Pack3tL0ss/central-api-cli"
 documentation = "https://central-api-cli.readthedocs.org"
```

### Comparing `centralcli-5.0.0/PKG-INFO` & `centralcli-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: centralcli
-Version: 5.0.0
+Version: 5.1.0
 Summary: A CLI for interacting with Aruba Central (Cloud Management Platform).  Facilitates bulk imports, exports, reporting.  A handy tool if you have devices managed by Aruba Central.
 Home-page: https://github.com/Pack3tL0ss/central-api-cli
 License: MIT
 Keywords: cli,Aruba,Aruba Networks,Aruba Central,HPE,API,RESTFUL,REST
 Author: Wade Wells (Pack3tL0ss)
 Author-email: wade@consolepi.org
 Maintainer: Wade Wells (Pack3tL0ss)
```

