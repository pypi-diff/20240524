# Comparing `tmp/bstk_notitia-0.4.0.tar.gz` & `tmp/bstk_notitia-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstk_notitia-0.4.0.tar", max compression
+gzip compressed data, was "bstk_notitia-0.5.0.tar", max compression
```

## Comparing `bstk_notitia-0.4.0.tar` & `bstk_notitia-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1705 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/README.md
--rw-r--r--   0        0        0     1080 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/__init__.py
--rw-r--r--   0        0        0      903 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/error.py
--rw-r--r--   0        0        0     1430 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/lib/abc/driver.py
--rw-r--r--   0        0        0     1086 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/lib/abc/informant.py
--rw-r--r--   0        0        0     5381 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/lib/abc/investigator.py
--rw-r--r--   0        0        0     2037 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/lib/abc/observer.py
--rw-r--r--   0        0        0     1309 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/lib/abc/reporter.py
--rw-r--r--   0        0        0     9185 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/loader.py
--rw-r--r--   0        0        0     8904 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/driver/mongodb.py
--rw-r--r--   0        0        0      565 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/driver/null.py
--rw-r--r--   0        0        0     2463 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/driver/passthrough.py
--rw-r--r--   0        0        0      745 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/informant/internal/datetime.py
--rw-r--r--   0        0        0      400 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/informant/internal/http.py
--rw-r--r--   0        0        0     1466 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/investigator/internal/clock.py
--rw-r--r--   0        0        0     1895 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/investigator/internal/mongo_record_processor.py
--rw-r--r--   0        0        0     3313 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/investigator/internal/notitia_casereporter.py
--rw-r--r--   0        0        0     1648 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/mongo_changestream.py
--rw-r--r--   0        0        0     3532 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/mongo_collectionstream.py
--rw-r--r--   0        0        0     1434 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/mongo_record.py
--rw-r--r--   0        0        0     1460 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/tick.py
--rw-r--r--   0        0        0      697 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/reporter/internal/echo.py
--rw-r--r--   0        0        0     3018 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/reporter/internal/mongo_record.py
--rw-r--r--   0        0        0     4025 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/modules/reporter/internal/notitia_case.py
--rw-r--r--   0        0        0    10357 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/notitia.py
--rw-r--r--   0        0        0    15705 2024-05-16 01:17:50.404759 bstk_notitia-0.4.0/bstk_notitia/roster.py
--rw-r--r--   0        0        0      815 2024-05-16 01:18:06.456922 bstk_notitia-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2307 1970-01-01 00:00:00.000000 bstk_notitia-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1705 2024-05-24 09:31:23.536636 bstk_notitia-0.5.0/README.md
+-rw-r--r--   0        0        0     1080 2024-05-24 09:31:23.536636 bstk_notitia-0.5.0/bstk_notitia/__init__.py
+-rw-r--r--   0        0        0      903 2024-05-24 09:31:23.536636 bstk_notitia-0.5.0/bstk_notitia/error.py
+-rw-r--r--   0        0        0     1430 2024-05-24 09:31:23.536636 bstk_notitia-0.5.0/bstk_notitia/lib/abc/driver.py
+-rw-r--r--   0        0        0     1086 2024-05-24 09:31:23.536636 bstk_notitia-0.5.0/bstk_notitia/lib/abc/informant.py
+-rw-r--r--   0        0        0     5702 2024-05-24 09:31:23.536636 bstk_notitia-0.5.0/bstk_notitia/lib/abc/investigator.py
+-rw-r--r--   0        0        0     2037 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/lib/abc/observer.py
+-rw-r--r--   0        0        0     1309 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/lib/abc/reporter.py
+-rw-r--r--   0        0        0     9185 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/loader.py
+-rw-r--r--   0        0        0     8904 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/driver/mongodb.py
+-rw-r--r--   0        0        0      565 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/driver/null.py
+-rw-r--r--   0        0        0     2463 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/driver/passthrough.py
+-rw-r--r--   0        0        0      745 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/informant/internal/datetime.py
+-rw-r--r--   0        0        0      400 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/informant/internal/http.py
+-rw-r--r--   0        0        0     1466 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/investigator/internal/clock.py
+-rw-r--r--   0        0        0     1895 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/investigator/internal/mongo_record_processor.py
+-rw-r--r--   0        0        0     3313 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/investigator/internal/notitia_casereporter.py
+-rw-r--r--   0        0        0     2451 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/mongo_changestream.py
+-rw-r--r--   0        0        0     4011 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/mongo_collectionstream.py
+-rw-r--r--   0        0        0     1434 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/mongo_record.py
+-rw-r--r--   0        0        0     1460 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/tick.py
+-rw-r--r--   0        0        0      697 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/reporter/internal/echo.py
+-rw-r--r--   0        0        0     3528 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/reporter/internal/mongo_record.py
+-rw-r--r--   0        0        0     4025 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/reporter/internal/notitia_case.py
+-rw-r--r--   0        0        0    10372 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/notitia.py
+-rw-r--r--   0        0        0    15705 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/roster.py
+-rw-r--r--   0        0        0      815 2024-05-24 09:31:38.024966 bstk_notitia-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2307 1970-01-01 00:00:00.000000 bstk_notitia-0.5.0/PKG-INFO
```

### Comparing `bstk_notitia-0.4.0/README.md` & `bstk_notitia-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/__init__.py` & `bstk_notitia-0.5.0/bstk_notitia/__init__.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/error.py` & `bstk_notitia-0.5.0/bstk_notitia/error.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/lib/abc/driver.py` & `bstk_notitia-0.5.0/bstk_notitia/lib/abc/driver.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/lib/abc/informant.py` & `bstk_notitia-0.5.0/bstk_notitia/lib/abc/informant.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/lib/abc/investigator.py` & `bstk_notitia-0.5.0/bstk_notitia/lib/abc/investigator.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,14 +126,27 @@
         )
         if _stat:
             document["state"] = new_state
 
         await self._log(_log, _stat)
         return _stat
 
+    async def close(
+        self,
+        document: typing.Dict,
+        reporter: ReporterABC,
+        updates: typing.Optional[typing.Dict],
+    ):
+        return await self.record(
+            document=document,
+            reporter=reporter,
+            updates=updates,
+            new_state="complete",
+        )
+
     async def record(
         self,
         document: typing.Dict,
         reporter: ReporterABC,
         updates: typing.Dict,
         new_state: typing.Optional[str] = None,
     ):
```

### Comparing `bstk_notitia-0.4.0/bstk_notitia/lib/abc/observer.py` & `bstk_notitia-0.5.0/bstk_notitia/lib/abc/observer.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/lib/abc/reporter.py` & `bstk_notitia-0.5.0/bstk_notitia/lib/abc/reporter.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/loader.py` & `bstk_notitia-0.5.0/bstk_notitia/loader.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/modules/driver/mongodb.py` & `bstk_notitia-0.5.0/bstk_notitia/modules/driver/mongodb.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/modules/driver/null.py` & `bstk_notitia-0.5.0/bstk_notitia/modules/driver/null.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/modules/driver/passthrough.py` & `bstk_notitia-0.5.0/bstk_notitia/modules/driver/passthrough.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/modules/informant/internal/datetime.py` & `bstk_notitia-0.5.0/bstk_notitia/modules/informant/internal/datetime.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/modules/investigator/internal/clock.py` & `bstk_notitia-0.5.0/bstk_notitia/modules/investigator/internal/clock.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/modules/investigator/internal/mongo_record_processor.py` & `bstk_notitia-0.5.0/bstk_notitia/modules/investigator/internal/mongo_record_processor.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/modules/investigator/internal/notitia_casereporter.py` & `bstk_notitia-0.5.0/bstk_notitia/modules/investigator/internal/notitia_casereporter.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/mongo_collectionstream.py` & `bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/mongo_collectionstream.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,19 @@
     },
 }
 
 # Where the mongo record observer does a "find all", and the mongo change stream observer "watches" for
 # changes, the notitia collection stream observer wraps both up into a consolidated "find & watch" observer,
 # whereby it will establish a change stream starting "now", find all pre-existing items matching the lookup,
 # yield until empty, then move on to results from the change stream.
+#
+# When using this observer from an investigator, ensure you carefully consider the implications on the shift runner.
+# A quiet collection that does not receive updates very often can cause the entire shift to run into overtime.
+# Split your investigators into long lived pools until we get to py3.12
+# ( https://docs.python.org/3.12/library/asyncio-task.html#waiting-primitives )
 
 
 @dataclass
 class NotitiaModule(ObserverABC):
     name = "Internal Mongo Collection Observer"
     key = "internal/mongo_collectionstream"
 
@@ -76,24 +81,28 @@
             prematch_hits.append(doc["_id"])
             yield doc
 
         _stream_params = {
             "collection": _collection,
             "pipeline": [_lookup],
             "resume_token": None,
-            "full_document": "whenAvailable",
+            "full_document": "updateLookup",
         }
         change_stream = self.driver["mongodb"].change_stream(
             **_stream_params,
             start_at_operation_time=_cursor_start_time,
         )
 
         async for token, change in self.driver["mongodb"].watch(
             changestream=change_stream, **_stream_params
         ):
+            if not change:
+                # Something's gone wrong, stop.
+                break
+
             _stream_params["resume_token"] = token
             _t = change.get("operationType")
             if _t not in self.operations:
                 # We should never see this, so if we do - it's a sign things have gone poorly
                 break
 
             doc = await self.glance(change)
```

### Comparing `bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/mongo_record.py` & `bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/mongo_record.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/modules/observer/internal/tick.py` & `bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/tick.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/modules/reporter/internal/echo.py` & `bstk_notitia-0.5.0/bstk_notitia/modules/reporter/internal/echo.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/modules/reporter/internal/mongo_record.py` & `bstk_notitia-0.5.0/bstk_notitia/modules/reporter/internal/mongo_record.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+from dataclasses import dataclass, field
 from types import NoneType
 import typing
 from bstk_notitia.lib.abc.reporter import ReporterABC
 
 if typing.TYPE_CHECKING:
     from modules.driver.mongodb import NotitiaModule as MongoDBDriver, DriverABC
     from pymongo.results import (
@@ -17,18 +18,21 @@
     "driver": {
         "type": "mongodb",
         "required": True,
     },
 }
 
 
+@dataclass
 class NotitiaModule(ReporterABC):
     name = "Internal MongoDB Record Reporter"
     key = "internal/mongodb_record"
 
+    collection: typing.Optional[typing.AnyStr] = field(kw_only=True, default=None)
+
     if typing.TYPE_CHECKING:
         driver: typing.Dict[str, typing.Union[MongoDBDriver, DriverABC]]
 
     async def receive(
         self,
         action: str,
         data: typing.Union[typing.List[typing.Dict], typing.Dict],
@@ -36,33 +40,44 @@
         constraints: typing.Optional[typing.Dict[str, typing.Any]] = None,
     ):
         brief = None
         if action == "update":
             if not record or not record.get("_id"):
                 return False
 
-            stream = self.driver["mongodb"].get_collection().update_one
+            stream = self.driver["mongodb"].get_collection(self.collection).update_one
             if not constraints:
                 constraints = {"_id": record["_id"]}
             else:
                 constraints["_id"] = record["_id"]
 
             if not self._has_update_operators(data):
                 data = {"$set": data}
 
             stream_params = {"filter": constraints, "update": data}
 
         if action == "insert":
             if isinstance(data, list):
-                stream = self.driver["mongodb"].get_collection().insert_many
+                stream = (
+                    self.driver["mongodb"].get_collection(self.collection).insert_many
+                )
                 stream_params = {"documents": data}
             else:
-                stream = self.driver["mongodb"].get_collection().insert_one
+                stream = (
+                    self.driver["mongodb"].get_collection(self.collection).insert_one
+                )
                 stream_params = {"document": data}
 
+        if action == "apply":
+            if not constraints:
+                return False
+
+            stream = self.driver["mongodb"].get_collection(self.collection).update_many
+            stream_params = {"filter": constraints, "update": data}
+
         if not stream:
             return False
 
         brief = stream(**stream_params)
 
         if not brief:
             return False
```

### Comparing `bstk_notitia-0.4.0/bstk_notitia/modules/reporter/internal/notitia_case.py` & `bstk_notitia-0.5.0/bstk_notitia/modules/reporter/internal/notitia_case.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/bstk_notitia/notitia.py` & `bstk_notitia-0.5.0/bstk_notitia/notitia.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,15 @@
 
     def _load_resolve_module(
         self, _mod: ModuleType, init_params: typing.Optional[typing.Dict]
     ):
         try:
             return _mod.NotitiaModule(**init_params, department=self.department)
         except TypeError as ex:
-            raise NotitiaBootstrapError from ex
+            raise NotitiaBootstrapError(_mod.__file__) from ex
 
     def _add_to_roster(
         self, investigator: InvestigatorABC, startup_params: typing.Dict
     ):
         if not self._roster:
             self._roster = Roster()
```

### Comparing `bstk_notitia-0.4.0/bstk_notitia/roster.py` & `bstk_notitia-0.5.0/bstk_notitia/roster.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.4.0/pyproject.toml` & `bstk_notitia-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bstk_notitia"
-version = "0.4.0"
+version = "0.5.0"
 description = "notitia core runtime & modules"
 authors = ["colin <colin@broadstack.com.au>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = { extras = ["cli"], version = "^1.0.0" }
```

### Comparing `bstk_notitia-0.4.0/PKG-INFO` & `bstk_notitia-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstk_notitia
-Version: 0.4.0
+Version: 0.5.0
 Summary: notitia core runtime & modules
 Author: colin
 Author-email: colin@broadstack.com.au
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

