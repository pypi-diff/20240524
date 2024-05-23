# Comparing `tmp/pyvalkey-0.0.4.tar.gz` & `tmp/pyvalkey-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvalkey-0.0.4.tar", max compression
+gzip compressed data, was "pyvalkey-0.0.5.tar", max compression
```

## Comparing `pyvalkey-0.0.4.tar` & `pyvalkey-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0     1090 2023-03-21 22:51:27.852685 pyvalkey-0.0.4/LICENSE
--rw-r--r--   0        0        0      772 2024-04-12 14:49:51.174521 pyvalkey-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      213 2024-04-12 14:28:25.850391 pyvalkey-0.0.4/pyvalkey/__init__.py
--rw-r--r--   0        0        0      202 2024-04-12 14:28:27.961359 pyvalkey-0.0.4/pyvalkey/__main__.py
--rw-r--r--   0        0        0        2 2023-10-17 22:24:37.362186 pyvalkey-0.0.4/pyvalkey/commands/__init__.py
--rw-r--r--   0        0        0     1835 2024-04-12 14:33:22.670789 pyvalkey-0.0.4/pyvalkey/commands/acls.py
--rw-r--r--   0        0        0     2799 2024-04-12 14:38:12.134395 pyvalkey-0.0.4/pyvalkey/commands/admins.py
--rw-r--r--   0        0        0     6494 2024-04-12 14:35:23.351330 pyvalkey-0.0.4/pyvalkey/commands/bits.py
--rw-r--r--   0        0        0     4630 2024-04-12 14:33:22.514540 pyvalkey-0.0.4/pyvalkey/commands/clients.py
--rw-r--r--   0        0        0     1131 2024-04-12 14:33:22.514540 pyvalkey-0.0.4/pyvalkey/commands/configs.py
--rw-r--r--   0        0        0      908 2024-04-12 14:28:26.282659 pyvalkey-0.0.4/pyvalkey/commands/context.py
--rw-r--r--   0        0        0      458 2024-04-12 14:28:26.034214 pyvalkey-0.0.4/pyvalkey/commands/core.py
--rw-r--r--   0        0        0     2282 2024-04-12 14:28:25.901023 pyvalkey-0.0.4/pyvalkey/commands/creators.py
--rw-r--r--   0        0        0     2722 2024-04-12 14:33:22.655164 pyvalkey-0.0.4/pyvalkey/commands/databases.py
--rw-r--r--   0        0        0      196 2024-04-12 14:33:22.530164 pyvalkey-0.0.4/pyvalkey/commands/dependencies.py
--rw-r--r--   0        0        0      245 2024-04-12 14:33:22.592663 pyvalkey-0.0.4/pyvalkey/commands/geo_commands.py
--rw-r--r--   0        0        0     5170 2024-04-12 14:33:22.545791 pyvalkey-0.0.4/pyvalkey/commands/hash_maps.py
--rw-r--r--   0        0        0      462 2024-04-12 14:33:22.389540 pyvalkey-0.0.4/pyvalkey/commands/informations.py
--rw-r--r--   0        0        0      974 2024-04-12 14:33:22.483305 pyvalkey-0.0.4/pyvalkey/commands/keyspace_commands.py
--rw-r--r--   0        0        0     4043 2024-04-12 14:34:29.222473 pyvalkey-0.0.4/pyvalkey/commands/lists.py
--rw-r--r--   0        0        0     1482 2024-04-12 14:37:55.239227 pyvalkey-0.0.4/pyvalkey/commands/parameters.py
--rw-r--r--   0        0        0    11688 2024-04-12 14:38:32.048611 pyvalkey-0.0.4/pyvalkey/commands/parsers.py
--rw-r--r--   0        0        0     1853 2024-04-12 14:33:22.608287 pyvalkey-0.0.4/pyvalkey/commands/router.py
--rw-r--r--   0        0        0     2004 2024-04-12 14:33:22.420795 pyvalkey-0.0.4/pyvalkey/commands/servers.py
--rw-r--r--   0        0        0     5501 2024-04-12 14:33:22.530164 pyvalkey-0.0.4/pyvalkey/commands/sets.py
--rw-r--r--   0        0        0    10170 2024-04-12 14:33:22.405180 pyvalkey-0.0.4/pyvalkey/commands/sorted_sets.py
--rw-r--r--   0        0        0      505 2023-10-17 22:24:37.393445 pyvalkey-0.0.4/pyvalkey/commands/utils.py
--rw-r--r--   0        0        0        2 2023-12-20 07:40:07.427425 pyvalkey-0.0.4/pyvalkey/consts.py
--rw-r--r--   0        0        0        0 2023-12-20 07:40:07.428423 pyvalkey-0.0.4/pyvalkey/database_objects/__init__.py
--rw-r--r--   0        0        0     3958 2023-12-20 20:21:51.646922 pyvalkey-0.0.4/pyvalkey/database_objects/acl.py
--rw-r--r--   0        0        0     2261 2024-04-12 14:28:26.167372 pyvalkey-0.0.4/pyvalkey/database_objects/clients.py
--rw-r--r--   0        0        0     2750 2024-04-12 14:28:25.795715 pyvalkey-0.0.4/pyvalkey/database_objects/configurations.py
--rw-r--r--   0        0        0     7763 2024-04-12 14:31:14.166461 pyvalkey-0.0.4/pyvalkey/database_objects/databases.py
--rw-r--r--   0        0        0      448 2024-04-12 14:31:14.010212 pyvalkey-0.0.4/pyvalkey/database_objects/errors.py
--rw-r--r--   0        0        0      897 2024-04-12 14:31:13.947717 pyvalkey-0.0.4/pyvalkey/database_objects/information.py
--rw-r--r--   0        0        0      379 2023-12-20 07:40:07.434423 pyvalkey-0.0.4/pyvalkey/database_objects/utils.py
--rw-r--r--   0        0        0     3116 2023-10-17 22:24:37.393445 pyvalkey-0.0.4/pyvalkey/resp.py
--rw-r--r--   0        0        0     4963 2024-04-12 14:34:29.191220 pyvalkey-0.0.4/pyvalkey/server.py
--rw-r--r--   0        0        0     1689 2024-04-12 14:34:29.191220 pyvalkey-0.0.4/README.md
--rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 pyvalkey-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-03-21 22:51:27.852685 pyvalkey-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1099 2024-05-23 22:21:41.611439 pyvalkey-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      213 2024-04-12 14:28:25.850391 pyvalkey-0.0.5/pyvalkey/__init__.py
+-rw-r--r--   0        0        0      258 2024-05-23 18:31:15.898590 pyvalkey-0.0.5/pyvalkey/__main__.py
+-rw-r--r--   0        0        0        2 2023-10-17 22:24:37.362186 pyvalkey-0.0.5/pyvalkey/commands/__init__.py
+-rw-r--r--   0        0        0     1944 2024-05-23 21:59:09.227458 pyvalkey-0.0.5/pyvalkey/commands/acls.py
+-rw-r--r--   0        0        0     5639 2024-05-23 22:01:36.689990 pyvalkey-0.0.5/pyvalkey/commands/admins.py
+-rw-r--r--   0        0        0     6724 2024-05-23 21:59:05.658102 pyvalkey-0.0.5/pyvalkey/commands/bits.py
+-rw-r--r--   0        0        0     4805 2024-05-23 18:56:15.811774 pyvalkey-0.0.5/pyvalkey/commands/clients.py
+-rw-r--r--   0        0        0     1168 2024-05-23 22:01:36.687991 pyvalkey-0.0.5/pyvalkey/commands/configs.py
+-rw-r--r--   0        0        0      931 2024-05-23 18:59:59.013324 pyvalkey-0.0.5/pyvalkey/commands/context.py
+-rw-r--r--   0        0        0      523 2024-05-23 22:03:18.129998 pyvalkey-0.0.5/pyvalkey/commands/core.py
+-rw-r--r--   0        0        0     2324 2024-05-23 22:03:41.694605 pyvalkey-0.0.5/pyvalkey/commands/creators.py
+-rw-r--r--   0        0        0     2884 2024-05-23 21:59:05.118773 pyvalkey-0.0.5/pyvalkey/commands/databases.py
+-rw-r--r--   0        0        0      243 2024-05-23 19:19:52.713705 pyvalkey-0.0.5/pyvalkey/commands/dependencies.py
+-rw-r--r--   0        0        0      295 2024-05-23 19:01:21.278124 pyvalkey-0.0.5/pyvalkey/commands/geo_commands.py
+-rw-r--r--   0        0        0     5357 2024-05-23 22:04:10.963991 pyvalkey-0.0.5/pyvalkey/commands/hash_maps.py
+-rw-r--r--   0        0        0      512 2024-05-23 19:02:05.026204 pyvalkey-0.0.5/pyvalkey/commands/informations.py
+-rw-r--r--   0        0        0     1889 2024-05-23 19:08:12.500956 pyvalkey-0.0.5/pyvalkey/commands/keyspace_commands.py
+-rw-r--r--   0        0        0     4197 2024-05-23 21:59:08.428558 pyvalkey-0.0.5/pyvalkey/commands/lists.py
+-rw-r--r--   0        0        0     1833 2024-05-23 21:58:41.252411 pyvalkey-0.0.5/pyvalkey/commands/parameters.py
+-rw-r--r--   0        0        0    13027 2024-05-23 22:04:18.362901 pyvalkey-0.0.5/pyvalkey/commands/parsers.py
+-rw-r--r--   0        0        0     2423 2024-05-23 22:04:35.627720 pyvalkey-0.0.5/pyvalkey/commands/router.py
+-rw-r--r--   0        0        0     2236 2024-05-23 19:55:28.447126 pyvalkey-0.0.5/pyvalkey/commands/servers.py
+-rw-r--r--   0        0        0     5755 2024-05-23 22:04:45.755859 pyvalkey-0.0.5/pyvalkey/commands/sets.py
+-rw-r--r--   0        0        0    10308 2024-05-23 21:59:09.166365 pyvalkey-0.0.5/pyvalkey/commands/sorted_sets.py
+-rw-r--r--   0        0        0      522 2024-05-23 19:33:31.700381 pyvalkey-0.0.5/pyvalkey/commands/utils.py
+-rw-r--r--   0        0        0        0 2023-12-20 07:40:07.428423 pyvalkey-0.0.5/pyvalkey/database_objects/__init__.py
+-rw-r--r--   0        0        0     6900 2024-05-23 22:04:59.582199 pyvalkey-0.0.5/pyvalkey/database_objects/acl.py
+-rw-r--r--   0        0        0     2545 2024-05-23 21:58:41.252411 pyvalkey-0.0.5/pyvalkey/database_objects/clients.py
+-rw-r--r--   0        0        0     2819 2024-05-23 21:58:41.268036 pyvalkey-0.0.5/pyvalkey/database_objects/configurations.py
+-rw-r--r--   0        0        0     8166 2024-05-23 21:59:10.130623 pyvalkey-0.0.5/pyvalkey/database_objects/databases.py
+-rw-r--r--   0        0        0      796 2024-05-23 20:39:54.179087 pyvalkey-0.0.5/pyvalkey/database_objects/errors.py
+-rw-r--r--   0        0        0      905 2024-05-23 19:43:02.272364 pyvalkey-0.0.5/pyvalkey/database_objects/information.py
+-rw-r--r--   0        0        0      432 2024-05-23 21:58:06.374815 pyvalkey-0.0.5/pyvalkey/database_objects/utils.py
+-rw-r--r--   0        0        0     3541 2024-05-23 22:05:16.325055 pyvalkey-0.0.5/pyvalkey/resp.py
+-rw-r--r--   0        0        0     6010 2024-05-23 19:55:44.253862 pyvalkey-0.0.5/pyvalkey/server.py
+-rw-r--r--   0        0        0     1694 2024-05-16 19:49:53.547971 pyvalkey-0.0.5/README.md
+-rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 pyvalkey-0.0.5/PKG-INFO
```

### Comparing `pyvalkey-0.0.4/LICENSE` & `pyvalkey-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/acls.py` & `pyvalkey-0.0.5/pyvalkey/commands/acls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 from os import urandom
 
 from pyvalkey.commands.core import Command
 from pyvalkey.commands.dependencies import server_command_dependency
 from pyvalkey.commands.parameters import positional_parameter
 from pyvalkey.commands.router import ServerCommandsRouter
 from pyvalkey.database_objects.acl import ACL
+from pyvalkey.resp import ValueType
 
 
 @ServerCommandsRouter.command(b"help", [b"slow", b"connection"], b"acl")
 class AclHelp(Command):
-    def execute(self):
+    def execute(self) -> ValueType:
         return ["genpass"]
 
 
 @ServerCommandsRouter.command(b"genpass", [b"slow"], b"acl")
 class AclGeneratePassword(Command):
     length: int = positional_parameter(default=64)
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return urandom(self.length)
 
 
 @ServerCommandsRouter.command(b"cat", [b"slow"], b"acl")
 class AclCategory(Command):
     category: bytes | None = positional_parameter(default=None)
 
-    def execute(self):
+    def execute(self) -> ValueType:
         if self.category is not None:
             return ACL.get_category_commands(self.category)
         return ACL.get_categories()
 
 
 @ServerCommandsRouter.command(b"deluser", [b"admin", b"slow", b"dangerous"], b"acl")
 class AclDeleteUser(Command):
     acl: ACL = server_command_dependency()
+
     user_names: list[bytes] = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         user_deleted = 0
         for user_name in self.user_names:
             if user_name == b"default":
                 pass
             user_deleted += 1 if self.acl.pop(user_name, None) is not None else 0
         return user_deleted
 
 
 @ServerCommandsRouter.command(b"getuser", [b"admin", b"slow", b"dangerous"], b"acl")
 class AclGetUser(Command):
     acl: ACL = server_command_dependency()
     user_name: bytes = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         if self.user_name not in self.acl:
-            return
+            return None
         return self.acl[self.user_name].info
```

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/bits.py` & `pyvalkey-0.0.5/pyvalkey/commands/bits.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,38 +3,39 @@
 from functools import reduce
 from typing import Any, ClassVar
 
 from pyvalkey.commands.databases import DatabaseCommand
 from pyvalkey.commands.parameters import positional_parameter
 from pyvalkey.commands.router import ServerCommandsRouter
 from pyvalkey.database_objects.databases import Database
-from pyvalkey.database_objects.errors import ServerException
+from pyvalkey.database_objects.errors import ServerError
+from pyvalkey.resp import ValueType
 
 
 @ServerCommandsRouter.command(b"getbit", [b"read", b"bitmap", b"fast"])
 class GetBit(DatabaseCommand):
     key: bytes = positional_parameter()
     offset: int = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         s = self.database.get_or_create_string(self.key)
 
         bytes_offset = self.offset // 8
         byte_offset = self.offset - (bytes_offset * 8)
 
         return (s.bytes_value[bytes_offset] >> byte_offset) & 1
 
 
 @ServerCommandsRouter.command(b"setbit", [b"write", b"bitmap", b"slow"])
 class SetBit(DatabaseCommand):
     key: bytes = positional_parameter()
     offset: int = positional_parameter()
     value: bool = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         s = self.database.get_or_create_string(self.key)
 
         offset = int(self.offset)
         bytes_offset = offset // 8
         byte_offset = offset - (bytes_offset * 8)
 
         if len(s.bytes_value) <= bytes_offset:
@@ -66,15 +67,15 @@
         BitOperationMode.XOR: operator.xor,
     }
 
     operation: BitOperationMode = positional_parameter()
     destination_key: bytes = positional_parameter()
     source_keys: list[bytes] = positional_parameter()
 
-    def handle(self):
+    def handle(self) -> int:
         if self.operation in self.OPERATION_TO_OPERATOR:
             result = reduce(
                 self.OPERATION_TO_OPERATOR[self.operation],
                 (self.database.get_string(source_key).int_value for source_key in self.source_keys),
             )
             s = self.database.get_or_create_string(self.destination_key)
             s.update_with_int_value(result)
@@ -90,15 +91,15 @@
 
 @ServerCommandsRouter.command(b"bitcount", [b"read", b"bitmap", b"slow"])
 class BitCount(DatabaseCommand):
     key: bytes = positional_parameter()
     count_range: tuple[int, int] | None = positional_parameter(default=None)
     bit_mode: bool = positional_parameter(default=False, values_mapping={b"BYTE": False, b"BIT": True})
 
-    def handle_byte_mode(self, key: bytes, start: int, end: int):
+    def handle_byte_mode(self, key: bytes, start: int, end: int) -> int:
         s = self.database.get_string(key)
 
         length = len(s.bytes_value)
         server_start = start
         server_stop = end
 
         if server_start >= 0:
@@ -109,82 +110,83 @@
         if server_stop >= 0:
             stop = min(length, server_stop)
         else:
             stop = max(length + int(server_stop), 0)
 
         return sum(map(int.bit_count, s.bytes_value[start : stop + 1]))
 
-    def handle_bit_mode(self, key: bytes, start: int, end: int):
+    def handle_bit_mode(self, key: bytes, start: int, end: int) -> int:
         s = self.database.get_string(key)
         value: int = s.int_value
 
         length = value.bit_length()
 
         if start < 0:
             start = length + start
 
         if end < 0:
             end = length + (end + 1)
 
         bit_count = ((value & ((2**end) - 1)) >> start).bit_count()
         return bit_count
 
-    def execute(self):
+    def execute(self) -> ValueType:
         if not self.count_range:
             s = self.database.get_string(self.key)
             return sum(map(int.bit_count, s.bytes_value))
 
         start, end = self.count_range
 
         if self.bit_mode:
-            self.handle_bit_mode(self.key, start, end)
+            return self.handle_bit_mode(self.key, start, end)
+        return self.handle_byte_mode(self.key, start, end)
 
 
-def apply_increment(database: Database, key: bytes, increment: int | float = 1):
+def apply_increment(database: Database, key: bytes, increment: int | float = 1) -> bytes:
     s = database.get_or_create_string(key)
     if s.numeric_value is None:
-        raise ServerException(b"ERR value is not an integer or out of range")
+        raise ServerError(b"ERR value is not an integer or out of range")
     s.update_with_numeric_value(s.numeric_value + increment)
     return s.bytes_value
 
 
 @ServerCommandsRouter.command(b"incr", [b"write", b"string", b"fast"])
 class Increment(DatabaseCommand):
     key: bytes = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return apply_increment(self.database, self.key)
 
 
 @ServerCommandsRouter.command(b"incrby", [b"write", b"string", b"fast"])
 class IncrementBy(DatabaseCommand):
     key: bytes = positional_parameter()
     increment: int = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return apply_increment(self.database, self.key, self.increment)
 
 
 @ServerCommandsRouter.command(b"incrbyfloat", [b"write", b"string", b"fast"])
 class IncrementByFloat(DatabaseCommand):
     key: bytes = positional_parameter()
     increment: float = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return apply_increment(self.database, self.key, self.increment)
 
 
 @ServerCommandsRouter.command(b"decr", [b"write", b"string", b"fast"])
 class Decrement(DatabaseCommand):
     key: bytes = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return apply_increment(self.database, self.key, -1)
 
 
 @ServerCommandsRouter.command(b"decrby", [b"write", b"string", b"fast"])
 class DecrementBy(DatabaseCommand):
     key: bytes = positional_parameter()
     decrement: float = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return apply_increment(self.database, self.key, self.decrement * -1)
```

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/clients.py` & `pyvalkey-0.0.5/pyvalkey/commands/clients.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,76 +2,76 @@
 from dataclasses import dataclass
 from enum import Enum
 
 from pyvalkey.commands.context import ClientContext
 from pyvalkey.commands.core import Command
 from pyvalkey.commands.dependencies import server_command_dependency
 from pyvalkey.commands.parameters import (
-    server_keyword_parameter,
     positional_parameter,
+    server_keyword_parameter,
 )
 from pyvalkey.commands.router import ServerCommandsRouter
-from pyvalkey.resp import RESP_OK, RespError
+from pyvalkey.resp import RESP_OK, RespError, ValueType
 
 
 @dataclass
 class ClientCommand(Command):
     client_context: ClientContext = server_command_dependency()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         raise NotImplementedError()
 
 
 @ServerCommandsRouter.command(b"select", [b"connection", b"fast"])
 class SelectDatabase(ClientCommand):
     index: int = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         self.client_context.current_database = self.index
         return RESP_OK
 
 
 @ServerCommandsRouter.command(b"list", [b"admin", b"slow", b"dangerous", b"connection"], b"client")
 class ClientList(ClientCommand):
     client_type: bytes | None = server_keyword_parameter(flag=b"TYPE", default=None)
 
-    def execute(self):
+    def execute(self) -> ValueType:
         if self.client_type:
             return self.client_context.server_context.clients.filter_(client_type=self.client_type).info
         return self.client_context.server_context.clients.info
 
 
 @ServerCommandsRouter.command(b"id", [b"slow", b"connection"], b"client")
 class ClientId(ClientCommand):
-    def execute(self):
+    def execute(self) -> ValueType:
         return self.client_context.current_client.client_id
 
 
 @ServerCommandsRouter.command(b"setname", [b"slow", b"connection"], b"client")
 class ClientSetName(ClientCommand):
     name: bytes = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         self.client_context.current_client.name = self.name
         return RESP_OK
 
 
 @ServerCommandsRouter.command(b"getname", [b"slow", b"connection"], b"client")
 class ClientGetName(ClientCommand):
-    def execute(self):
+    def execute(self) -> ValueType:
         return self.client_context.current_client.name or None
 
 
 @ServerCommandsRouter.command(b"kill", [b"admin", b"slow", b"dangerous", b"connection"], b"client")
 class ClientKill(ClientCommand):
     old_format_address: bytes | None = positional_parameter(default=None)
     client_id: int = server_keyword_parameter(flag=b"ID", default=None)
     address: bytes = server_keyword_parameter(flag=b"ADDR", default=None)
 
-    def execute(self):
+    def execute(self) -> ValueType:
         if self.old_format_address:
             clients = self.client_context.server_context.clients.filter_(address=self.old_format_address).values()
             if not clients:
                 return RespError(b"ERR No such client")
             (client,) = clients
             client.is_killed = True
             return RESP_OK
@@ -84,48 +84,49 @@
         return len(clients)
 
 
 @ServerCommandsRouter.command(b"pause", [b"admin", b"slow", b"dangerous", b"connection"], b"client")
 class ClientPause(ClientCommand):
     timeout_seconds: int = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         self.client_context.server_context.pause_timeout = time.time() + self.timeout_seconds
         self.client_context.server_context.is_paused = True
         return RESP_OK
 
 
 @ServerCommandsRouter.command(b"unpause", [b"admin", b"slow", b"dangerous", b"connection"], b"client")
 class ClientUnpause(ClientCommand):
     timeout_seconds: int = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         self.client_context.server_context.is_paused = False
         return RESP_OK
 
 
 class ReplyMode(Enum):
     ON = b"ON"
     OFF = b"OFF"
     SKIP = b"SKIP"
 
 
 @ServerCommandsRouter.command(b"reply", [b"slow", b"connection"], b"client")
 class ClientReply(ClientCommand):
     mode: ReplyMode = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         if self.mode == ReplyMode.ON:
             return RESP_OK
+        return None
 
 
 @ServerCommandsRouter.command(b"setinfo", [b"slow", b"connection"], b"client")
 class ClientSetInformation(ClientCommand):
     library_name: bytes | None = server_keyword_parameter(flag=b"LIB-NAME", default=None)
     library_version: bytes | None = server_keyword_parameter(flag=b"LIB-VER", default=None)
 
-    def execute(self):
+    def execute(self) -> ValueType:
         if self.library_name:
             self.client_context.current_client.library_name = self.library_name
         if self.library_version:
             self.client_context.current_client.library_version = self.library_version
         return RESP_OK
```

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/configs.py` & `pyvalkey-0.0.5/pyvalkey/commands/configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from pyvalkey.commands.core import Command
 from pyvalkey.commands.dependencies import server_command_dependency
 from pyvalkey.commands.parameters import positional_parameter
 from pyvalkey.commands.router import ServerCommandsRouter
 from pyvalkey.database_objects.configurations import Configurations
-from pyvalkey.resp import RESP_OK
+from pyvalkey.resp import RESP_OK, ValueType
 
 
 @ServerCommandsRouter.command(b"get", [b"admin", b"slow", b"dangerous"], b"config")
 class ConfigGet(Command):
     configurations: Configurations = server_command_dependency()
     parameters: list[bytes] = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         names = self.configurations.get_names(*self.parameters)
         return self.configurations.info(names)
 
 
 @ServerCommandsRouter.command(b"set", [b"admin", b"slow", b"dangerous"], b"config")
 class ConfigSet(Command):
     configurations: Configurations = server_command_dependency()
     parameters_values: list[tuple[bytes, bytes]] = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         for name, value in self.parameters_values:
             self.configurations.set_values(name, value)
         return RESP_OK
```

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/context.py` & `pyvalkey-0.0.5/pyvalkey/commands/context.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import defaultdict
 from dataclasses import dataclass
 
-from pyvalkey.database_objects.acl import ACL
+from pyvalkey.database_objects.acl import ACL, ACLUser
 from pyvalkey.database_objects.clients import Client, ClientList
 from pyvalkey.database_objects.configurations import Configurations
 from pyvalkey.database_objects.databases import Database
 from pyvalkey.database_objects.information import Information
 
 
 @dataclass
@@ -22,12 +22,12 @@
 
 @dataclass
 class ClientContext:
     server_context: ServerContext
     current_client: Client
 
     current_database: int = 0
-    current_user: bytes | None = None
+    current_user: ACLUser | None = None
 
     @property
-    def database(self):
+    def database(self) -> Database:
         return self.server_context.databases[self.current_database]
```

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/creators.py` & `pyvalkey-0.0.5/pyvalkey/commands/creators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from collections.abc import Callable
 from dataclasses import Field, dataclass, fields
 from enum import Enum, auto
-from typing import Callable
+from typing import Self
 
 from pyvalkey.commands.context import ClientContext, ServerContext
 from pyvalkey.commands.core import Command
 from pyvalkey.database_objects.acl import ACL
 from pyvalkey.database_objects.configurations import Configurations
 from pyvalkey.database_objects.databases import Database
 from pyvalkey.database_objects.information import Information
@@ -16,15 +17,15 @@
 
 @dataclass
 class CommandCreator:
     command_cls: type[Command]
     command_creator: Callable[..., Command]
     dependencies: list[Field]
 
-    def __call__(self, parameters: list[bytes], client_context: ClientContext):
+    def __call__(self, parameters: list[bytes], client_context: ClientContext) -> Command:
         command_kwargs = self.command_cls.parse(parameters)
 
         for command_dependency in self.dependencies:
             if command_dependency.type == Database:
                 command_kwargs[command_dependency.name] = client_context.database
             elif command_dependency.type == ACL:
                 command_kwargs[command_dependency.name] = client_context.server_context.acl
@@ -38,17 +39,17 @@
                 command_kwargs[command_dependency.name] = client_context.server_context.configurations
             else:
                 raise TypeError()
 
         return self.command_creator(**command_kwargs)
 
     @classmethod
-    def create(cls, command_cls: type[Command]):
+    def create(cls, command_cls: type[Command]) -> Self:
         command_dependencies = []
 
         for command_dependency in fields(command_cls):
             if not command_dependency.metadata.get(DependencyMetadata.DEPENDENCY):
                 continue
 
             command_dependencies.append(command_dependency)
 
-        return CommandCreator(command_cls, command_cls, command_dependencies)
+        return cls(command_cls, command_cls, command_dependencies)
```

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/databases.py` & `pyvalkey-0.0.5/pyvalkey/commands/databases.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,88 +2,88 @@
 from dataclasses import dataclass
 
 from pyvalkey.commands.core import Command
 from pyvalkey.commands.dependencies import server_command_dependency
 from pyvalkey.commands.parameters import positional_parameter
 from pyvalkey.commands.router import ServerCommandsRouter
 from pyvalkey.database_objects.databases import Database
-from pyvalkey.resp import RESP_OK
+from pyvalkey.resp import RESP_OK, ValueType
 
 
 @dataclass
 class DatabaseCommand(Command):
     database: Database = server_command_dependency()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         raise NotImplementedError()
 
 
 @ServerCommandsRouter.command(b"echo", [b"fast", b"connection"])
 class Echo(Command):
     message: bytes = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return self.message
 
 
 @ServerCommandsRouter.command(b"ping", [b"fast", b"connection"])
 class Ping(Command):
-    message: bytes = positional_parameter(default=None)
+    message: bytes | None = positional_parameter(default=None)
 
-    def execute(self):
+    def execute(self) -> ValueType:
         if self.message:
             return self.message
         return b"PONG"
 
 
 @ServerCommandsRouter.command(b"get", [b"read", b"string", b"fast"])
 class Get(DatabaseCommand):
-    key: bytes = positional_parameter()
+    key: bytes = positional_parameter(key_mode=b"R")
 
-    def execute(self):
+    def execute(self) -> ValueType:
         if s := self.database.get_string_or_none(self.key):
             return s.bytes_value
         return None
 
 
 @ServerCommandsRouter.command(b"set", [b"write", b"string", b"slow"])
 class Set(DatabaseCommand):
-    key: bytes = positional_parameter()
+    key: bytes = positional_parameter(key_mode=b"RW")
     value: bytes = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         s = self.database.get_or_create_string(self.key)
         s.update_with_bytes_value(self.value)
         return RESP_OK
 
 
 @ServerCommandsRouter.command(b"del", [b"keyspace", b"write", b"slow"])
 class Delete(DatabaseCommand):
     keys: list[bytes] = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return len([1 for _ in filter(None, [self.database.pop(key, None) for key in self.keys])])
 
 
 @ServerCommandsRouter.command(b"keys", [b"keyspace", b"read", b"slow", b"dangerous"])
 class Keys(DatabaseCommand):
     pattern: bytes = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return list(fnmatch.filter(self.database.keys(), self.pattern))
 
 
 @ServerCommandsRouter.command(b"dbsize", [b"keyspace", b"read", b"fast"])
 class DatabaseSize(DatabaseCommand):
-    def execute(self):
+    def execute(self) -> ValueType:
         return len(self.database.keys())
 
 
 @ServerCommandsRouter.command(b"append", [b"write", b"string", b"fast"])
 class Append(DatabaseCommand):
     key: bytes = positional_parameter()
     value: bytes = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         s = self.database.get_or_create_string(self.key)
         s.update_with_bytes_value(s.bytes_value + self.value)
         return len(s)
```

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/hash_maps.py` & `pyvalkey-0.0.5/pyvalkey/commands/sets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,157 @@
+import functools
+from collections.abc import Callable
+
 from pyvalkey.commands.databases import DatabaseCommand
 from pyvalkey.commands.parameters import positional_parameter
 from pyvalkey.commands.router import ServerCommandsRouter
 from pyvalkey.database_objects.databases import Database
-from pyvalkey.database_objects.errors import ServerInvalidIntegerError
-from pyvalkey.resp import RESP_OK
+from pyvalkey.resp import ValueType
 
 
-def apply_hash_map_increase_by(database: Database, key: bytes, field: bytes, increment: int | float):
-    hash_get = database.get_or_create_hash_table(key)
+@ServerCommandsRouter.command(b"smove", [b"write", b"set", b"fast"])
+class SetMove(DatabaseCommand):
+    source: bytes = positional_parameter()
+    destination: bytes = positional_parameter()
+    member: bytes = positional_parameter()
 
-    if field not in hash_get:
-        hash_get[field] = 0
-    if not isinstance(hash_get[field], (int, float)):
-        raise ServerInvalidIntegerError
-    hash_get[field] += increment
-    return hash_get[field]
+    def execute(self) -> ValueType:
+        source_set = self.database.get_set(self.source)
+        destination_set = self.database.get_or_create_set(self.destination)
+        if self.member not in source_set:
+            return False
+        source_set.remove(self.member)
+        destination_set.add(self.member)
+        return True
 
 
-@ServerCommandsRouter.command(b"hincrby", [b"write", b"hash", b"fast"])
-class HashMapIncreaseBy(DatabaseCommand):
+@ServerCommandsRouter.command(b"smismember", [b"read", b"set", b"slow"])
+class SetAreMembers(DatabaseCommand):
     key: bytes = positional_parameter()
-    field: bytes = positional_parameter()
-    value: int = positional_parameter()
+    members: set[bytes] = positional_parameter()
 
-    def execute(self):
-        return apply_hash_map_increase_by(self.database, self.key, self.field, self.value)
+    def execute(self) -> ValueType:
+        a_set = self.database.get_set(self.key)
+        return list(map(lambda m: m in a_set, self.members))
 
 
-@ServerCommandsRouter.command(b"hincrbyfloat", [b"write", b"hash", b"fast"])
-class HashMapIncreaseByFloat(DatabaseCommand):
+@ServerCommandsRouter.command(b"sismember", [b"read", b"set", b"fast"])
+class SetIsMember(DatabaseCommand):
     key: bytes = positional_parameter()
-    field: bytes = positional_parameter()
-    value: float = positional_parameter()
+    member: bytes = positional_parameter()
 
-    def execute(self):
-        return apply_hash_map_increase_by(self.database, self.key, self.field, self.value)
+    def execute(self) -> ValueType:
+        return self.member in self.database.get_set(self.key)
 
 
-@ServerCommandsRouter.command(b"hexists", [b"read", b"hash", b"fast"])
-class HashMapExists(DatabaseCommand):
+@ServerCommandsRouter.command(b"smembers", [b"read", b"set", b"fast"])
+class SetMembers(DatabaseCommand):
     key: bytes = positional_parameter()
-    field: bytes = positional_parameter()
 
-    def execute(self):
-        return self.field in self.database.get_hash_table(self.key)
+    def execute(self) -> ValueType:
+        return list(self.database.get_set(self.key))
 
 
-@ServerCommandsRouter.command(b"hget", [b"read", b"hash", b"fast"])
-class HashMapGet(DatabaseCommand):
+@ServerCommandsRouter.command(b"scard", [b"read", b"set", b"fast"])
+class SetCardinality(DatabaseCommand):
     key: bytes = positional_parameter()
-    field: bytes = positional_parameter()
 
-    def execute(self):
-        return self.database.get_hash_table(self.key).get(self.field)
+    def execute(self) -> ValueType:
+        return len(self.database.get_set(self.key))
 
 
-@ServerCommandsRouter.command(b"hmget", [b"read", b"hash", b"fast"])
-class HashMapGetMultiple(DatabaseCommand):
+@ServerCommandsRouter.command(b"sadd", [b"write", b"set", b"fast"])
+class SetAdd(DatabaseCommand):
     key: bytes = positional_parameter()
-    fields: list[bytes] = positional_parameter()
+    members: set[bytes] = positional_parameter()
 
-    def execute(self):
-        hash_map = self.database.get_hash_table(self.key)
-        return [hash_map.get(f, None) for f in self.fields]
+    def execute(self) -> ValueType:
+        a_set = self.database.get_or_create_set(self.key)
+        length_before = len(a_set)
+        for member in self.members:
+            a_set.add(member)
+        return len(a_set) - length_before
 
 
-@ServerCommandsRouter.command(b"hgetall", [b"read", b"hash", b"slow"])
-class HashMapGetAll(DatabaseCommand):
+@ServerCommandsRouter.command(b"spop", [b"write", b"set", b"fast"])
+class SetPop(DatabaseCommand):
     key: bytes = positional_parameter()
+    count: int = positional_parameter(default=None)
 
-    def execute(self):
-        hash_set = self.database.get_hash_table(self.key)
-
-        response = []
-        for k, v in hash_set.items():
-            response.extend([k, v])
-        return response
+    def execute(self) -> ValueType:
+        a_set = self.database.get_set(self.key).pop()
+        if self.count is None:
+            return a_set.pop() if a_set else None
+        return [a_set.pop() for _ in range(min(len(a_set), self.count))]
 
 
-@ServerCommandsRouter.command(b"hkeys", [b"read", b"hash", b"slow"])
-class HashMapKeys(DatabaseCommand):
+@ServerCommandsRouter.command(b"srem", [b"write", b"set", b"fast"])
+class SetRemove(DatabaseCommand):
     key: bytes = positional_parameter()
+    members: set[bytes] = positional_parameter()
 
-    def execute(self):
-        return list(self.database.get_hash_table(self.key).keys())
+    def execute(self) -> ValueType:
+        a_set = self.database.get_set(self.key)
+        self.database[self.key] = a_set - self.members
+        return len(a_set.intersection(self.members))
 
 
-@ServerCommandsRouter.command(b"hlen", [b"read", b"hash", b"fast"])
-class HashMapLength(DatabaseCommand):
-    key: bytes = positional_parameter()
+def apply_set_operation(database: Database, operation: Callable[[set, set], set], keys: list[bytes]) -> list:
+    return list(functools.reduce(operation, map(database.get_set, keys)))  # type: ignore[arg-type]
 
-    def execute(self):
-        return len(self.database.get_hash_table(self.key))
 
+@ServerCommandsRouter.command(b"sunion", [b"read", b"set", b"slow"])
+class SetUnion(DatabaseCommand):
+    keys: list[bytes] = positional_parameter()
 
-@ServerCommandsRouter.command(b"hvals", [b"read", b"hash", b"slow"])
-class HashMapValues(DatabaseCommand):
-    key: bytes = positional_parameter()
+    def execute(self) -> ValueType:
+        return apply_set_operation(self.database, set.union, self.keys)
 
-    def execute(self):
-        return list(self.database.get_hash_table(self.key).values())
 
+@ServerCommandsRouter.command(b"sinter", [b"read", b"set", b"slow"])
+class SetIntersection(DatabaseCommand):
+    keys: list[bytes] = positional_parameter()
 
-@ServerCommandsRouter.command(b"hstrlen", [b"read", b"hash", b"fast"])
-class HashMapStringLength(DatabaseCommand):
-    key: bytes = positional_parameter()
-    field: bytes = positional_parameter()
+    def execute(self) -> ValueType:
+        return apply_set_operation(self.database, set.intersection, self.keys)
 
-    def execute(self):
-        return len(self.database.get_hash_table(self.key).get(self.field, b""))
 
+@ServerCommandsRouter.command(b"sdiff", [b"read", b"set", b"slow"])
+class SetDifference(DatabaseCommand):
+    keys: list[bytes] = positional_parameter()
 
-@ServerCommandsRouter.command(b"hdel", [b"write", b"hash", b"fast"])
-class HashMapDelete(DatabaseCommand):
-    key: bytes = positional_parameter()
-    fields: list[bytes] = positional_parameter()
+    def execute(self) -> ValueType:
+        return apply_set_operation(self.database, set.difference, self.keys)
 
-    def execute(self):
-        hash_map = self.database.get_hash_table(self.key)
 
-        return sum([1 if hash_map.pop(f, None) is not None else 0 for f in self.fields])
+def apply_set_store_operation(
+    database: Database, operation: Callable[[set, set], set], keys: list[bytes], destination: bytes
+) -> int:
+    database[destination] = functools.reduce(operation, map(database.get_set, keys))
+    return len(database[destination])
 
 
-@ServerCommandsRouter.command(b"hset", [b"write", b"hash", b"fast"])
-class HashMapSet(DatabaseCommand):
-    key: bytes = positional_parameter()
-    fields_values: list[tuple[bytes, bytes]] = positional_parameter()
+@ServerCommandsRouter.command(b"sunionstore", [b"write", b"set", b"slow"])
+class SetUnionStore(DatabaseCommand):
+    destination: bytes = positional_parameter()
+    keys: list[bytes] = positional_parameter()
 
-    def execute(self):
-        hash_map = self.database.get_or_create_hash_table(self.key)
+    def execute(self) -> ValueType:
+        return apply_set_store_operation(self.database, set.union, self.keys, self.destination)
 
-        added_fields = 0
-        for field, value in self.fields_values:
-            if field not in hash_map:
-                added_fields += 1
-            hash_map[field] = value
-        return added_fields
 
+@ServerCommandsRouter.command(b"sinterstore", [b"write", b"set", b"slow"])
+class SetIntersectionStore(DatabaseCommand):
+    destination: bytes = positional_parameter()
+    keys: list[bytes] = positional_parameter()
+
+    def execute(self) -> ValueType:
+        return apply_set_store_operation(self.database, set.intersection, self.keys, self.destination)
 
-@ServerCommandsRouter.command(b"hmset", [b"write", b"hash", b"fast"])
-class HashMapSetMultiple(DatabaseCommand):
-    key: bytes = positional_parameter()
-    fields_values: list[tuple[bytes, bytes]] = positional_parameter()
 
-    def execute(self):
-        hash_map = self.database.get_or_create_hash_table(self.key)
+@ServerCommandsRouter.command(b"sdiffstore", [b"write", b"set", b"slow"])
+class SetDifferenceStore(DatabaseCommand):
+    destination: bytes = positional_parameter()
+    keys: list[bytes] = positional_parameter()
 
-        for field, value in self.fields_values:
-            hash_map[field] = value
-        return RESP_OK
+    def execute(self) -> ValueType:
+        return apply_set_store_operation(self.database, set.difference, self.keys, self.destination)
```

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/lists.py` & `pyvalkey-0.0.5/pyvalkey/commands/lists.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from enum import Enum
 
 from pyvalkey.commands.databases import DatabaseCommand
 from pyvalkey.commands.parameters import positional_parameter
 from pyvalkey.commands.router import ServerCommandsRouter
 from pyvalkey.commands.utils import parse_range_parameters
+from pyvalkey.resp import ValueType
 
 
 @ServerCommandsRouter.command(b"llen", [b"read", b"list", b"fast"])
 class ListLength(DatabaseCommand):
     key: bytes = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return len(self.database.get_list(self.key))
 
 
 @ServerCommandsRouter.command(b"lindex", [b"read", b"list", b"slow"])
 class ListIndex(DatabaseCommand):
     key: bytes = positional_parameter()
     index: int = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         server_list = self.database.get_list(self.key)
 
         try:
             return server_list[self.index]
         except IndexError:
             return None
 
 
 @ServerCommandsRouter.command(b"lrange", [b"read", b"list", b"slow"])
 class ListRange(DatabaseCommand):
     key: bytes = positional_parameter()
     start: int = positional_parameter()
     stop: int = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return self.database.get_list(self.key)[parse_range_parameters(self.start, self.stop)]
 
 
 class DirectionMode(Enum):
     BEFORE = b"before"
     AFTER = b"after"
 
@@ -46,59 +47,59 @@
 @ServerCommandsRouter.command(b"linsert", [b"write", b"list", b"slow"])
 class ListInsert(DatabaseCommand):
     key: bytes = positional_parameter()
     direction: DirectionMode = positional_parameter()
     pivot: bytes = positional_parameter()
     element: bytes = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         a_list = self.database.get_or_create_list(self.key)
 
         if not a_list:
             return 0
         try:
             index = a_list.index(self.pivot)
         except ValueError:
             return -1
         a_list.insert(index + 0 if self.direction == DirectionMode.BEFORE else 1, self.element)
         return len(a_list)
 
 
 @ServerCommandsRouter.command(b"lpush", [b"write", b"list", b"fast"])
 class ListPush(DatabaseCommand):
-    key: bytes = positional_parameter()
+    key: bytes = positional_parameter(key_mode=b"W")
     values: list[bytes] = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         a_list = self.database.get_or_create_list(self.key)
 
         for v in self.values:
             a_list.insert(0, v)
         return len(a_list)
 
 
 @ServerCommandsRouter.command(b"rpush", [b"write", b"list", b"fast"])
 class ListPushAtTail(DatabaseCommand):
     key: bytes = positional_parameter()
     values: list[bytes] = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         a_list = self.database.get_or_create_list(self.key)
 
         for v in self.values:
             a_list.append(v)
         return len(a_list)
 
 
 @ServerCommandsRouter.command(b"lpop", [b"write", b"list", b"fast"])
 class ListPop(DatabaseCommand):
     key: bytes = positional_parameter()
     count: int = positional_parameter(default=None)
 
-    def execute(self):
+    def execute(self) -> ValueType:
         a_list = self.database.get_or_create_list(self.key)
 
         if not a_list:
             return None
         if self.count:
             return [a_list.pop(0) for _ in range(min(len(a_list), self.count))]
         return a_list.pop(0)
@@ -106,15 +107,15 @@
 
 @ServerCommandsRouter.command(b"lrem", [b"write", b"list", b"slow"])
 class ListRemove(DatabaseCommand):
     key: bytes = positional_parameter()
     count: int = positional_parameter()
     element: bytes = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         a_list = self.database.get_or_create_list(self.key)
 
         if not a_list:
             return 0
         count = int(self.count)
         to_delete = abs(count)
         if count < 0:
```

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/parameters.py` & `pyvalkey-0.0.5/pyvalkey/commands/parameters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,52 @@
+from __future__ import annotations
+
 from dataclasses import MISSING, field
 from enum import Enum, auto
 from typing import Any
 
 
 class ParameterMetadata(Enum):
     SERVER_PARAMETER = auto()
     VALUES_MAPPING = auto()
     FLAG = auto()
+    KEY_MODE = auto()
 
 
 def server_parameter(
     values_mapping: dict[bytes, Any] | None = None,
-    default=MISSING,
+    default: Any = MISSING,  # noqa: ANN401
     flag: bytes | dict[bytes, Any] | None = None,
-):
+    key_mode: bytes | None = None,
+) -> Any:  # noqa: ANN401
     metadata: dict[ParameterMetadata, Any] = {ParameterMetadata.SERVER_PARAMETER: True}
     if values_mapping:
         metadata[ParameterMetadata.VALUES_MAPPING] = values_mapping
     if flag:
         if isinstance(flag, dict):
             metadata[ParameterMetadata.FLAG] = {key.upper(): value for key, value in flag.items()}
             default = None
         else:
             metadata[ParameterMetadata.FLAG] = flag.upper()
             metadata[ParameterMetadata.VALUES_MAPPING] = {
                 flag.upper(): True,
             }
             default = False
+    if key_mode is not None:
+        metadata[ParameterMetadata.KEY_MODE] = key_mode
     return field(default=default, metadata=metadata, kw_only=bool(flag))
 
 
 def positional_parameter(
     values_mapping: dict[bytes, Any] | None = None,
-    default=MISSING,
-):
-    return server_parameter(
-        values_mapping=values_mapping,
-        default=default,
-    )
+    default: Any = MISSING,  # noqa: ANN401
+    key_mode: bytes | None = None,
+) -> Any:  # noqa: ANN401
+    return server_parameter(values_mapping=values_mapping, default=default, key_mode=key_mode)
 
 
 def server_keyword_parameter(
     values_mapping: dict[bytes, Any] | None = None,
-    default=MISSING,
+    default: Any = MISSING,  # noqa: ANN401
     flag: bytes | dict[bytes, Any] | None = None,
-):
+) -> Any:  # noqa: ANN401
     return server_parameter(values_mapping=values_mapping, default=default, flag=flag)
```

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/parsers.py` & `pyvalkey-0.0.5/pyvalkey/commands/parsers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,110 +1,126 @@
+from __future__ import annotations
+
+from collections.abc import Callable
 from dataclasses import MISSING, Field, dataclass, field, fields, is_dataclass
 from enum import Enum
 from types import UnionType
-from typing import Any, Union, get_args, get_origin
-
-from typing_extensions import Self
+from typing import TYPE_CHECKING, Any, ClassVar, Self, Union, get_args, get_origin, overload
 
 from pyvalkey.commands.creators import CommandCreator
 from pyvalkey.commands.parameters import ParameterMetadata
 from pyvalkey.database_objects.errors import (
-    ServerException,
+    ServerError,
     ServerSyntaxError,
-    ServerWrongNumberOfArguments,
+    ServerWrongNumberOfArgumentsError,
 )
 
+if TYPE_CHECKING:
+    from pyvalkey.commands.core import Command
+
 
 class ParameterParser:
     @classmethod
     def next_parameter(cls, parameters: list[bytes]) -> bytes:
         try:
             return parameters.pop(0)
         except IndexError:
-            raise ServerWrongNumberOfArguments()
+            raise ServerWrongNumberOfArgumentsError()
 
-    def parse(self, parameters: list[bytes]) -> Any:
+    def parse(self, parameters: list[bytes]) -> Any:  # noqa: ANN401
         return self.next_parameter(parameters)
 
     @classmethod
-    def _extract_optional_type(cls, parameter_type):
+    def _extract_optional_type(cls, parameter_type: Any) -> Any:  # noqa: ANN401
         if get_origin(parameter_type) == Union or get_origin(parameter_type) == UnionType:
-            items = get_args(parameter_type)
-            items = set([arg for arg in items if arg is not type(None)])
+            args = get_args(parameter_type)
+            items = set([arg for arg in args if arg is not type(None)])
             if len(items) > 1:
                 raise TypeError(items)
             parameter_type = items.pop()
         return parameter_type
 
     @classmethod
-    def create(cls, parameter_field: Field):
+    def create(cls, parameter_field: Field) -> ParameterParser:
         parameter_type = cls._extract_optional_type(parameter_field.type)
 
         if isinstance(parameter_type, type) and issubclass(parameter_type, Enum):
             return EnumParameterParser(parameter_type)
 
         if is_dataclass(parameter_type):
             return ObjectParser.create(parameter_type)
 
         match parameter_type():
             case bytes():
+                if parameter_field.metadata.get(ParameterMetadata.KEY_MODE, False):
+                    return KeyParameterParser()
                 return ParameterParser()
             case bool():
                 return BoolParameterParser(
                     parameter_field.metadata.get(
                         ParameterMetadata.VALUES_MAPPING, BoolParameterParser.DEFAULT_VALUES_MAPPING
                     )
                 )
             case int():
                 return IntParameterParser()
             case float():
                 return FloatParameterParser()
             case list():
-                return ListParameterParser.create(get_args(parameter_type)[0])
+                return ListParameterParser.create_from_list_type(get_args(parameter_type)[0])
             case set():
                 return SetParameterParser.create(get_args(parameter_type)[0])
             case tuple():
-                return TupleParameterParser.create(get_args(parameter_type))
+                return TupleParameterParser.create_from_tuple_types(get_args(parameter_type))
             case default:
                 raise TypeError(default)
 
 
+class KeyParameterParser(ParameterParser):
+    def parse(self, parameters: list[bytes]) -> Any:  # noqa: ANN401
+        return self.next_parameter(parameters)
+
+
 class ParametersGroup(ParameterParser):
-    def parse(self, parameters: list[bytes]) -> dict[str, Any]:
+    def parse(self, parameters: list[bytes]) -> Any:  # noqa: ANN401
         raise NotImplementedError()
 
 
 @dataclass
 class NamedParameterParser(ParameterParser):
     name: str
     parameter_parser: ParameterParser
 
-    def parse(self, parameters: list[bytes]) -> Any:
-        return self.parameter_parser.parse(parameters)
+    def parse(self, parameters: list[bytes]) -> dict[str, Any]:
+        return {self.name: self.parameter_parser.parse(parameters)}
+
+
+@dataclass
+class OptionalNamedParameterParser(NamedParameterParser):
+    pass
 
 
 @dataclass
 class ListParameterParser(ParameterParser):
     parameter_parser: ParameterParser
 
     def parse(self, parameters: list[bytes]) -> list:
         list_parameter = []
         while parameters:
             list_parameter.append(self.parameter_parser.parse(parameters))
         return list_parameter
 
     @classmethod
-    def create(cls, list_type) -> "ListParameterParser":
+    def create_from_list_type(cls, list_type: Any) -> Self:  # noqa: ANN401
         match list_type():
             case bytes():
-                return ListParameterParser(ParameterParser())
+                return cls(ParameterParser())
             case int():
-                return ListParameterParser(IntParameterParser())
+                return cls(IntParameterParser())
             case tuple():
-                return ListParameterParser(TupleParameterParser.create(get_args(list_type)))
+                return cls(TupleParameterParser.create_from_tuple_types(get_args(list_type)))
             case default:
                 raise TypeError(default)
 
 
 @dataclass
 class SetParameterParser(ParameterParser):
     parameter_parser: ParameterParser
@@ -112,20 +128,20 @@
     def parse(self, parameters: list[bytes]) -> set:
         set_value = set()
         while parameters:
             set_value.add(self.parameter_parser.parse(parameters))
         return set_value
 
     @classmethod
-    def create(cls, set_type) -> "SetParameterParser":
+    def create(cls, set_type: Any) -> Self:  # noqa: ANN401
         match set_type():
             case bytes():
-                return SetParameterParser(ParameterParser())
+                return cls(ParameterParser())
             case int():
-                return SetParameterParser(IntParameterParser())
+                return cls(IntParameterParser())
             case default:
                 raise TypeError(default)
 
 
 @dataclass
 class TupleParameterParser(ParameterParser):
     parameter_parser_tuple: tuple[ParameterParser, ...]
@@ -133,15 +149,15 @@
     def parse(self, parameters: list[bytes]) -> tuple:
         tuple_parameter = []
         for parameter_parser in self.parameter_parser_tuple:
             tuple_parameter.append(parameter_parser.parse(parameters))
         return tuple(tuple_parameter)
 
     @classmethod
-    def create(cls, tuple_types) -> Self:
+    def create_from_tuple_types(cls, tuple_types: tuple[Any, ...]) -> Self:
         parameter_parser_tuple = []
         for arg in tuple_types:
             match arg():
                 case bytes():
                     parameter_parser_tuple.append(ParameterParser())
                 case int():
                     parameter_parser_tuple.append(IntParameterParser())
@@ -151,23 +167,23 @@
 
 
 class IntParameterParser(ParameterParser):
     def parse(self, parameters: list[bytes]) -> int:
         try:
             return int(self.next_parameter(parameters))
         except ValueError:
-            raise ServerException(b"ERR value is not an integer or out of range")
+            raise ServerError(b"ERR value is not an integer or out of range")
 
 
 class FloatParameterParser(ParameterParser):
     def parse(self, parameters: list[bytes]) -> float:
         try:
             return float(self.next_parameter(parameters))
         except ValueError:
-            raise ServerException(b"ERR value is not a valid float")
+            raise ServerError(b"ERR value is not a valid float")
 
 
 @dataclass
 class EnumParameterParser(ParameterParser):
     enum_cls: type[Enum]
 
     def parse(self, parameters: list[bytes]) -> Enum:
@@ -176,127 +192,129 @@
             return self.enum_cls(enum_value)
         except ValueError as e:
             raise ServerSyntaxError(enum_value) from e
 
 
 @dataclass
 class BoolParameterParser(ParameterParser):
-    DEFAULT_VALUES_MAPPING = {b"1": True, b"0": False}
+    DEFAULT_VALUES_MAPPING: ClassVar = {b"1": True, b"0": False}
 
     values_mapping: dict[bytes, bool] = field(default_factory=lambda: BoolParameterParser.DEFAULT_VALUES_MAPPING)
 
     def parse(self, parameters: list[bytes]) -> bool:
         bytes_value = self.next_parameter(parameters).upper()
         if bytes_value not in self.values_mapping:
             raise ServerSyntaxError(bytes_value)
         return self.values_mapping[bytes_value]
 
 
 @dataclass
-class KeywordParameter(ParameterParser):
-    def parse(self, parameters: list[bytes]) -> dict[str, Any]:
-        raise NotImplementedError()
-
-
-@dataclass
-class OptionalParametersGroup(ParametersGroup):
+class OptionalKeywordParametersGroup(ParametersGroup):
     parameters_parsers_map: dict[bytes, NamedParameterParser]
 
     def parse(self, parameters: list[bytes]) -> dict[str, Any]:
         parsed_kw_parameters: dict[str, Any] = {}
 
         while parameters:
             top_parameter = parameters[0].upper()
             if top_parameter not in self.parameters_parsers_map:
                 return parsed_kw_parameters
             parameter = self.parameters_parsers_map[top_parameter]
 
             if parameter.name in parsed_kw_parameters:
                 raise ServerSyntaxError()
-            parsed_kw_parameters[parameter.name] = parameter.parse(parameters)
+            parsed_kw_parameters.update(parameter.parse(parameters))
 
         return parsed_kw_parameters
 
 
 @dataclass
 class ObjectParametersParser(ParametersGroup):
     parameters_parsers: list[ParameterParser]
 
-    def parse(self, parameters: list[bytes]) -> Any:
+    @classmethod
+    def _is_optional(cls, parameter_parser: ParameterParser) -> bool:
+        return isinstance(parameter_parser, OptionalKeywordParametersGroup | OptionalNamedParameterParser)
+
+    def parse(self, parameters: list[bytes]) -> Any:  # noqa: ANN401
         parsed_parameters: dict[str, Any] = {}
 
+        non_optional_parameters = sum(1 for p in self.parameters_parsers if not self._is_optional(p))
+
         for index, parameter_parser in enumerate(self.parameters_parsers):
-            if len(parameters) <= (len(self.parameters_parsers) - index - 1):
+            if self._is_optional(parameter_parser) and len(parameters) <= (non_optional_parameters - index):
                 continue
 
-            if isinstance(parameter_parser, NamedParameterParser):
-                parsed_parameters[parameter_parser.name] = parameter_parser.parse(parameters)
-            else:
-                parsed_parameters.update(parameter_parser.parse(parameters))
+            parsed_parameters.update(parameter_parser.parse(parameters))
 
         return parsed_parameters
 
-    def __call__(self, parameters: list[bytes]):
+    def __call__(self, parameters: list[bytes]) -> Any:  # noqa: ANN401
         return self.parse(list(parameters))
 
     @classmethod
-    def create(cls, object_cls) -> Self:
+    def create(cls, object_cls: Any) -> Self:  # noqa: ANN401
         parameter_fields = {
             parameter_field.name: parameter_field
             for parameter_field in fields(object_cls)
             if parameter_field.metadata.get(ParameterMetadata.SERVER_PARAMETER)
         }
         parameter_fields_by_order = list(parameter_fields.keys())
         if hasattr(object_cls, "__original_order__"):
             parameter_fields_by_order = list(getattr(object_cls, "__original_order__"))
 
         parameters_parsers: list[ParameterParser] = []
 
-        flagged_fields = {}
+        optional_keyword_parameters = {}
         for parameter_field_name in parameter_fields_by_order:
             parameter_field = parameter_fields[parameter_field_name]
             flag = parameter_field.metadata.get(ParameterMetadata.FLAG)
             if flag:
                 named_parameter_parser = NamedParameterParser(
                     parameter_field_name, ParameterParser.create(parameter_field)
                 )
                 if isinstance(flag, dict):
                     for flag_key in flag.keys():
-                        flagged_fields[flag_key] = named_parameter_parser
+                        optional_keyword_parameters[flag_key] = named_parameter_parser
                 else:
-                    flagged_fields[flag] = named_parameter_parser
+                    optional_keyword_parameters[flag] = named_parameter_parser
             else:
-                if flagged_fields:
-                    parameters_parsers.append(OptionalParametersGroup(flagged_fields))
-                    flagged_fields = {}
-
-                parameters_parsers.append(
-                    NamedParameterParser(parameter_field.name, ParameterParser.create(parameter_field))
-                )
+                if optional_keyword_parameters:
+                    parameters_parsers.append(OptionalKeywordParametersGroup(optional_keyword_parameters))
+                    optional_keyword_parameters = {}
+
+                if parameter_field.default != MISSING:
+                    parameters_parsers.append(
+                        OptionalNamedParameterParser(parameter_field.name, ParameterParser.create(parameter_field))
+                    )
+                else:
+                    parameters_parsers.append(
+                        NamedParameterParser(parameter_field.name, ParameterParser.create(parameter_field))
+                    )
 
-        if flagged_fields:
-            parameters_parsers.append(OptionalParametersGroup(flagged_fields))
+        if optional_keyword_parameters:
+            parameters_parsers.append(OptionalKeywordParametersGroup(optional_keyword_parameters))
 
         return cls(parameters_parsers)
 
 
 @dataclass
 class ObjectParser(ParametersGroup):
     object_cls: Any
     object_parameters_parser: ObjectParametersParser
 
-    def parse(self, parameters: list[bytes]) -> Any:
+    def parse(self, parameters: list[bytes]) -> Any:  # noqa: ANN401
         return self.object_cls(self.object_parameters_parser.parse(parameters))
 
     @classmethod
-    def create(cls, object_cls) -> "ObjectParser":
-        return ObjectParser(object_cls, ObjectParametersParser.create(object_cls))
+    def create(cls, object_cls: Any) -> Self:  # noqa: ANN401
+        return cls(object_cls, ObjectParametersParser.create(object_cls))
 
 
-def _server_command_wrapper(command_cls):
+def _server_command_wrapper(command_cls: type[Command]) -> type[Command]:
     original_order = []
 
     annotations = getattr(command_cls, "__annotations__", {})
 
     for name in list(command_cls.__dict__.keys()):
         value = getattr(command_cls, name)
 
@@ -324,11 +342,19 @@
     setattr(command_cls, "__original_order__", original_order)
     setattr(command_cls, "parse", ObjectParametersParser.create(command_cls))
     setattr(command_cls, "create", CommandCreator.create(command_cls))
 
     return command_cls
 
 
-def server_command(command_cls=None):
-    if command_cls is None:
+@overload
+def server_command(command_cls: Callable[[type[Command]], type[Command]], /) -> type[Command]: ...
+
+
+@overload
+def server_command(*args: type[Command]) -> type[Command]: ...
+
+
+def server_command(*args: Any) -> Any:
+    if len(args) == 0:
         return _server_command_wrapper
-    return _server_command_wrapper(command_cls)
+    return _server_command_wrapper(args[0])
```

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/router.py` & `pyvalkey-0.0.5/pyvalkey/commands/router.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,69 @@
-from dataclasses import dataclass
-from typing import ClassVar
+from __future__ import annotations
 
-from black.trans import defaultdict
+from collections import defaultdict
+from collections.abc import Callable
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Any, ClassVar
 
-from pyvalkey.commands.context import ClientContext
-from pyvalkey.commands.core import Command
 from pyvalkey.commands.parsers import server_command
 from pyvalkey.database_objects.acl import ACL
 from pyvalkey.database_objects.errors import RouterKeyError
 
+if TYPE_CHECKING:
+    from pyvalkey.commands.context import ClientContext
+    from pyvalkey.commands.core import Command
+
 
 @dataclass
 class ServerCommandsRouter:
-    ROUTES: ClassVar[dict[bytes, Command | dict[bytes, Command]]] = defaultdict(dict)
+    ROUTES: ClassVar[defaultdict[bytes, Any]] = defaultdict(dict)
 
-    def internal_route(self, parameters: list[bytes], routes: dict[bytes, Command | dict[bytes, Command]]) -> Command:
+    def internal_route(
+        self,
+        parameters: list[bytes],
+        routes: dict[bytes, type[Command]] | dict[bytes, type[Command] | dict[bytes, type[Command]]],
+    ) -> type[Command]:
         command = parameters.pop(0).lower()
 
         if command not in routes:
             raise RouterKeyError()
 
         routed_command = routes[command]
 
         if isinstance(routed_command, dict):
             return self.internal_route(parameters, routed_command)
 
         return routed_command
 
-    def route(self, parameters: list[bytes], client_context: ClientContext):
-        routed_command: Command = self.internal_route(parameters, self.ROUTES)
+    def route(self, parameters: list[bytes], client_context: ClientContext) -> Command:
+        routed_command: type[Command] = self.internal_route(parameters, self.ROUTES)
 
         return routed_command.create(parameters, client_context)
 
     @classmethod
-    def command(cls, command: bytes, acl_categories: list[bytes], parent_command: bytes = None):
-        def _command_wrapper(command_cls: Command):
+    def command(
+        cls, command: bytes, acl_categories: list[bytes], parent_command: bytes | None = None
+    ) -> Callable[[type[Command]], type[Command]]:
+        def _command_wrapper(command_cls: type[Command]) -> type[Command]:
             command_cls = server_command(command_cls)
 
             if not acl_categories:
                 raise TypeError("command must have at least one acl_categories")
 
+            command_name = parent_command + b"|" + command if parent_command else command
+
+            ACL.COMMAND_CATEGORIES[command_name] = set(acl_categories)
             for acl_category in acl_categories:
                 ACL.CATEGORIES[acl_category].add(command)
 
-            routes = cls.ROUTES
+            ACL.COMMANDS_NAMES[command_cls] = command_name
+
             if parent_command is not None:
-                routes = routes[parent_command]
-            routes[command] = command_cls
+                sub_route = cls.ROUTES[parent_command]
+                sub_route[command] = command_cls
+            else:
+                cls.ROUTES[command] = command_cls
 
             return command_cls
 
         return _command_wrapper
```

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/servers.py` & `pyvalkey-0.0.5/pyvalkey/commands/servers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 from dataclasses import dataclass
 from hashlib import sha256
 
-from pyvalkey.commands.context import ServerContext
+from pyvalkey.commands.context import ClientContext, ServerContext
 from pyvalkey.commands.core import Command
 from pyvalkey.commands.dependencies import server_command_dependency
 from pyvalkey.commands.parameters import positional_parameter
 from pyvalkey.commands.router import ServerCommandsRouter
 from pyvalkey.database_objects.acl import ACL
 from pyvalkey.database_objects.configurations import Configurations
-from pyvalkey.database_objects.errors import ServerException
-from pyvalkey.resp import RESP_OK, RespError
+from pyvalkey.database_objects.errors import ServerError
+from pyvalkey.resp import RESP_OK, RespError, ValueType
 
 
 @dataclass
 class ServerCommand(Command):
     server_context: ServerContext
 
-    def execute(self):
+    def execute(self) -> ValueType:
         raise NotImplementedError()
 
 
 @ServerCommandsRouter.command(b"auth", [b"fast", b"connection"])
 class Authorize(Command):
     acl: ACL = server_command_dependency()
     configurations: Configurations = server_command_dependency()
+    client_context: ClientContext = server_command_dependency()
 
     username: bytes | None = positional_parameter(default=None)
     password: bytes = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         password_hash = sha256(self.password).hexdigest().encode()
         if self.username is not None:
             if self.username not in self.acl:
-                raise ServerException(b"WRONGPASS invalid username-password pair or user is disabled.")
+                raise ServerError(b"WRONGPASS invalid username-password pair or user is disabled.")
             if self.username == b"default" and password_hash == self.configurations.requirepass:
                 return RESP_OK
-            if password_hash not in self.acl[self.username].passwords:
+            acl_user = self.acl[self.username]
+            if not acl_user.is_no_password_user and password_hash not in acl_user.passwords:
                 return RespError(b"WRONGPASS invalid username-password pair or user is disabled.")
+            self.client_context.current_user = acl_user
             return RESP_OK
 
         if self.configurations.requirepass and password_hash == self.configurations.requirepass:
             return RESP_OK
-        raise ServerException(
+        raise ServerError(
             b"ERR AUTH "
             b"<password> called without any password configured for the default user. "
             b"Are you sure your configuration is correct?"
         )
```

### Comparing `pyvalkey-0.0.4/pyvalkey/commands/sorted_sets.py` & `pyvalkey-0.0.5/pyvalkey/commands/sorted_sets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,48 @@
-import math
 from enum import Enum
 
 from pyvalkey.commands.databases import DatabaseCommand
 from pyvalkey.commands.parameters import (
-    server_keyword_parameter,
     positional_parameter,
+    server_keyword_parameter,
 )
 from pyvalkey.commands.router import ServerCommandsRouter
 from pyvalkey.commands.utils import parse_range_parameters
 from pyvalkey.database_objects.databases import (
-    MAX_STRING,
+    MAX_BYTES,
     Database,
     RangeLimit,
-    MaxString,
     ServerSortedSet,
 )
+from pyvalkey.resp import ValueType
 
 
-def parse_score_parameter(score: bytes) -> tuple[bytes | MaxString | float, bool]:
-    result_score: bytes | MaxString | float
+def parse_score_parameter(score: bytes) -> tuple[bytes, bool]:
+    result_score: bytes
     min_inclusive = True
     if score == b"-":
         result_score = b""
     elif score == b"+":
-        result_score = MAX_STRING
+        result_score = MAX_BYTES
     elif score == b"-inf":
-        result_score = -math.inf
+        result_score = score
     elif score == b"+inf":
-        result_score = -math.inf
+        result_score = score
     elif b"(" in score:
         result_score = score[1:]
         min_inclusive = False
     elif b"[" in score:
         result_score = score[1:]
     else:
         result_score = score
 
     return result_score, min_inclusive
 
 
-def parse_ordered_range_parameters(min_score: bytes, max_score: bytes):
+def parse_ordered_range_parameters(min_score: bytes, max_score: bytes) -> tuple[bytes, bool, bytes, bool]:
     return parse_score_parameter(min_score) + parse_score_parameter(max_score)
 
 
 class RangeMode(Enum):
     BY_INDEX = None
     BY_SCORE = b"BYSCORE"
     BY_LEX = b"BYLEX"
@@ -55,15 +54,15 @@
     start: bytes,
     stop: bytes,
     with_scores: bool = False,
     range_mode: RangeMode = RangeMode.BY_INDEX,
     is_reversed: bool = False,
     limit: RangeLimit | None = None,
     destination: bytes | None = None,
-):
+) -> int | list:
     z = database.get_sorted_set(key)
 
     if range_mode == RangeMode.BY_SCORE:
         min_score, min_inclusive, max_score, max_inclusive = parse_ordered_range_parameters(start, stop)
         result_iterator = z.range_by_score(
             float(min_score),
             float(max_score),
@@ -117,15 +116,15 @@
     score_update: ScoreUpdateMode = server_keyword_parameter(
         default=ScoreUpdateMode.ALL, flag={b"LT": ScoreUpdateMode.LESS_THAN, b"GT": ScoreUpdateMode.GREATER_THAN}
     )
     return_changed_elements: bool = server_keyword_parameter(flag=b"CH")
     increment_mode: bool = server_keyword_parameter(flag=b"INCR")
     scores_members: list[tuple[int, bytes]] = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         z = self.database.get_or_create_sorted_set(self.key)
         length_before = len(z)
         for score, member in self.scores_members:
             z.add(score, member)
         return len(z) - length_before
 
 
@@ -137,15 +136,15 @@
     range_mode: RangeMode = server_keyword_parameter(
         default=RangeMode.BY_INDEX, flag={b"BYSCORE": RangeMode.BY_SCORE, b"BYLEX": RangeMode.BY_LEX}
     )
     rev: bool = server_keyword_parameter(flag=b"REV")
     limit: RangeLimit | None = server_keyword_parameter(default=None, flag=b"LIMIT")
     with_scores: bool = server_keyword_parameter(flag=b"WITHSCORES")
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return sorted_set_range(
             self.database,
             self.key,
             self.start,
             self.stop,
             self.with_scores,
             self.range_mode,
@@ -163,15 +162,15 @@
     range_mode: RangeMode = server_keyword_parameter(
         default=RangeMode.BY_INDEX, flag={b"BYSCORE": RangeMode.BY_SCORE, b"BYLEX": RangeMode.BY_LEX}
     )
     rev: bool = server_keyword_parameter(flag=b"REV")
     limit: RangeLimit | None = server_keyword_parameter(default=None, flag=b"LIMIT")
     with_scores: bool = server_keyword_parameter(flag=b"WITHSCORES")
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return sorted_set_range(
             self.database,
             self.key,
             self.start,
             self.stop,
             self.with_scores,
             self.range_mode,
@@ -184,15 +183,15 @@
 @ServerCommandsRouter.command(b"zrevrange", [b"read", b"sortedset", b"slow"])
 class SortedSetReversedRange(DatabaseCommand):
     key: bytes = positional_parameter()
     start: bytes = positional_parameter()
     stop: bytes = positional_parameter()
     with_scores: bool = server_keyword_parameter(flag=b"WITHSCORES")
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return sorted_set_range(
             database=self.database,
             key=self.key,
             start=self.start,
             stop=self.stop,
             with_scores=self.with_scores,
         )
@@ -202,15 +201,15 @@
 class SortedSetRangeByScore(DatabaseCommand):
     key: bytes = positional_parameter()
     min: bytes = positional_parameter()
     max: bytes = positional_parameter()
     with_scores: bool = server_keyword_parameter(flag=b"WITHSCORES")
     limit: RangeLimit | None = server_keyword_parameter(default=None, flag=b"LIMIT")
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return sorted_set_range(
             database=self.database,
             key=self.key,
             start=self.min,
             stop=self.max,
             with_scores=self.with_scores,
             limit=self.limit,
@@ -222,15 +221,15 @@
 class SortedSetReversedRangeByScore(DatabaseCommand):
     key: bytes = positional_parameter()
     max: bytes = positional_parameter()
     min: bytes = positional_parameter()
     with_scores: bool = server_keyword_parameter(flag=b"WITHSCORES")
     limit: RangeLimit | None = server_keyword_parameter(default=None, flag=b"LIMIT")
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return sorted_set_range(
             database=self.database,
             key=self.key,
             start=self.min,
             stop=self.max,
             with_scores=self.with_scores,
             limit=self.limit,
@@ -242,15 +241,15 @@
 @ServerCommandsRouter.command(b"zrangebylex", [b"read", b"sortedset", b"slow"])
 class SortedSetRangeByLexical(DatabaseCommand):
     key: bytes = positional_parameter()
     min: bytes = positional_parameter()
     max: bytes = positional_parameter()
     limit: RangeLimit | None = server_keyword_parameter(default=None, flag=b"LIMIT")
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return sorted_set_range(
             database=self.database,
             key=self.key,
             start=self.min,
             stop=self.max,
             limit=self.limit,
             range_mode=RangeMode.BY_LEX,
@@ -260,15 +259,15 @@
 @ServerCommandsRouter.command(b"zrevrangebylex", [b"read", b"sortedset", b"slow"])
 class SortedSetReversedRangeByLexical(DatabaseCommand):
     key: bytes = positional_parameter()
     max: bytes = positional_parameter()
     min: bytes = positional_parameter()
     limit: RangeLimit | None = server_keyword_parameter(default=None, flag=b"LIMIT")
 
-    def execute(self):
+    def execute(self) -> ValueType:
         return sorted_set_range(
             database=self.database,
             key=self.key,
             start=self.min,
             stop=self.max,
             limit=self.limit,
             is_reversed=True,
@@ -278,15 +277,15 @@
 
 @ServerCommandsRouter.command(b"zcount", [b"read", b"sortedset", b"fast"])
 class SortedSetCount(DatabaseCommand):
     key: bytes = positional_parameter()
     min: bytes = positional_parameter()
     max: bytes = positional_parameter()
 
-    def execute(self):
+    def execute(self) -> ValueType:
         min_score, min_inclusive, max_score, max_inclusive = parse_ordered_range_parameters(self.min, self.max)
 
         z = self.database.get_or_create_sorted_set(self.key)
 
         return sum(
             1
             for _ in z.range_by_score(
@@ -295,9 +294,9 @@
         )
 
 
 @ServerCommandsRouter.command(b"zcard", [b"read", b"sortedset", b"fast"])
 class SortedSetCardinality(DatabaseCommand):
     key: bytes = positional_parameter()
 
-    def handle(self):
+    def execute(self) -> ValueType:
         return len(self.database.get_or_create_sorted_set(self.key).members)
```

### Comparing `pyvalkey-0.0.4/pyvalkey/database_objects/clients.py` & `pyvalkey-0.0.5/pyvalkey/database_objects/clients.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import itertools
+from collections.abc import Iterable
 from dataclasses import dataclass
+from typing import Self
 
 from pyvalkey.database_objects.utils import to_bytes
 
 
 @dataclass
 class Client:
     client_id: int
@@ -25,26 +27,34 @@
         return self.host + b":" + str(self.port).encode()
 
     @property
     def flags(self) -> bytes:
         return b"".join([b"N" if self.is_normal else b"", b"S" if self.is_replica else b""])
 
     @property
-    def info(self):
-        items = {b"id": self.client_id, b"addr": self.address, b"flags": self.flags, b"name": self.name}.items()
-        return b" ".join([k + b"=" + to_bytes(v) for k, v in items])
+    def info(self) -> bytes:
+        items: dict[bytes, bytes | int] = {
+            b"id": self.client_id,
+            b"addr": self.address,
+            b"flags": self.flags,
+            b"name": self.name,
+        }
+        return b" ".join([k + b"=" + to_bytes(v) for k, v in items.items()])
 
 
 class ClientList(dict[int, Client]):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(
+        self, *seq: dict[int, Client] | Iterable[tuple[int, Client]] | None, **kwargs: dict[int, Client]
+    ) -> None:
+        super().__init__(*seq, **kwargs)
+
         self.client_ids = itertools.count(0)
 
-    def all(self):
-        return ClientList({id_: c for id_, c in self.items() if not c.is_killed})
+    def all(self) -> Self:
+        return self.__class__({id_: c for id_, c in self.items() if not c.is_killed})
 
     def filter_(
         self, client_id: int | None = None, address: bytes | None = None, client_type: bytes | None = None
     ) -> "ClientList":
         filtered = ClientList()
         for c in self.all().values():
             if client_id is not None and c.client_id != client_id:
@@ -59,15 +69,15 @@
             filtered[c.client_id] = c
         return filtered
 
     @property
     def info(self) -> bytes:
         return b"\r".join([c.info for c in self.all().values()])
 
-    def create_client(self, host: bytes, port: int):
+    def create_client(self, host: bytes, port: int) -> Client:
         current_client_id = next(self.client_ids)
         self[current_client_id] = Client(
             client_id=current_client_id,
             host=host,
             port=port,
         )
         return self[current_client_id]
```

### Comparing `pyvalkey-0.0.4/pyvalkey/database_objects/configurations.py` & `pyvalkey-0.0.5/pyvalkey/database_objects/configurations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import fnmatch
 from dataclasses import Field, dataclass, field, fields
 from hashlib import sha256
-from typing import Literal
+from typing import Any, Literal
 
 from pyvalkey.database_objects.utils import to_bytes
 
 
 def configuration(
     default: int | bytes, type_: Literal["string", "password", "integer"] = "string", number_of_values: int = 1
-):
+) -> Any:  # noqa:ANN401
     return field(
         default=default,
         metadata={
             "type": type_,
             "number_of_values": number_of_values,
         },
     )
@@ -44,15 +44,15 @@
     def get_type(cls, name: bytes) -> str:
         try:
             a_field: Field = cls.__dataclass_fields__[name.decode().replace("-", "_")]
             return a_field.metadata["type"]
         except KeyError:
             return ""
 
-    def set_values(self, name: bytes, *values: bytes):
+    def set_values(self, name: bytes, *values: bytes) -> None:
         field_type = self.get_type(name)
 
         if field_type == "password":
             (value,) = values
             setattr(self, name.decode(), sha256(value).hexdigest().encode())
         elif field_type == "integer":
             (value,) = values
@@ -63,13 +63,13 @@
 
     def get_names(self, *patterns: bytes) -> set[bytes]:
         names: set[bytes] = set([])
         for pattern in patterns:
             names.update(set(fnmatch.filter((f.name.replace("_", "-").encode() for f in fields(self)), pattern)))
         return names
 
-    def info(self, names):
+    def info(self, names: set[bytes]) -> dict[bytes, bytes]:
         return {
             f.name.replace("_", "-").encode(): to_bytes(getattr(self, f.name))
             for f in fields(self)
             if f.name.replace("_", "-").encode() in names
         }
```

### Comparing `pyvalkey-0.0.4/pyvalkey/database_objects/databases.py` & `pyvalkey-0.0.5/pyvalkey/database_objects/databases.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 import functools
 import itertools
+from collections.abc import Iterable
 from dataclasses import dataclass
-from typing import Any, Iterable
+from typing import Any
 
 from sortedcontainers import SortedDict, SortedSet
 
 from pyvalkey.commands.parameters import positional_parameter
-from pyvalkey.database_objects.errors import ServerWrongType
+from pyvalkey.database_objects.errors import ServerWrongTypeError
 from pyvalkey.database_objects.utils import flatten
 
 
 @functools.total_ordering
-class MaxString:
-    def __eq__(self, other):
-        if isinstance(other, (bytes, str)):
+class MaxBytes(bytes):
+    def less(self, other: Any) -> bool:  # noqa: ANN401
+        if isinstance(other, bytes):
             return False
         raise NotImplementedError()
 
-    def __ge__(self, other):
-        if isinstance(other, (bytes, str)):
+    def more(self, other: Any) -> bool:  # noqa: ANN401
+        if isinstance(other, bytes):
             return True
         raise NotImplementedError()
 
+    __eq__ = less
+    __le__ = less
+    __lt__ = less
+    __ge__ = more
+    __gt__ = more
 
-MAX_STRING = MaxString()
+
+MAX_BYTES = MaxBytes()
 
 
 @dataclass
 class ServerString:
     bytes_value: bytes = b""
     int_value: int = 0
     numeric_value: float | None = 0
@@ -44,59 +51,59 @@
     def int_to_bytes(cls, value: int) -> bytes:
         return value.to_bytes(length=(8 + (value + (value < 0)).bit_length()) // 8, byteorder="big", signed=True)
 
     @classmethod
     def int_from_bytes(cls, value: bytes) -> int:
         return int.from_bytes(value, byteorder="big", signed=True)
 
-    def update_with_numeric_value(self, value: int | float):
+    def update_with_numeric_value(self, value: int | float) -> None:
         self.numeric_value = value
         self.bytes_value = f"{value:g}".encode()
         self.int_value = self.int_from_bytes(self.bytes_value)
 
-    def update_with_int_value(self, value: int):
+    def update_with_int_value(self, value: int) -> None:
         self.int_value = value
         self.bytes_value = self.int_to_bytes(value)
         self.numeric_value = int(self.bytes_value) if self.bytes_value.isdigit() else None
 
-    def update_with_bytes_value(self, value: bytes):
+    def update_with_bytes_value(self, value: bytes) -> None:
         self.int_value = self.int_from_bytes(value)
         self.bytes_value = value
         self.numeric_value = float(value) if self.is_float(value) else None
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.bytes_value)
 
 
 @dataclass(eq=True)
 class RangeLimit:
     offset: int = positional_parameter()
     count: int = positional_parameter()
 
 
 class ServerSortedSet:
-    def __init__(self, members_and_scores: Iterable[tuple[bytes, float]] | None = None):
+    def __init__(self, members_and_scores: Iterable[tuple[bytes, float]] | None = None) -> None:
         members_and_scores = members_and_scores or []
         self.members = SortedSet({(score, member) for member, score in members_and_scores})
         self.members_scores = SortedDict({member: score for member, score in members_and_scores})
 
-    def update(self, *scored_members: tuple[float, bytes]):
+    def update(self, *scored_members: tuple[float, bytes]) -> None:
         for score, member in scored_members:
             self.add(score, member)
 
-    def update_with_iterator(self, iterator):
+    def update_with_iterator(self, iterator: Iterable[bytes | float]) -> None:
         member = None
         for item in iterator:
             if member is None:
                 member = item
             else:
                 self.add(item, member)
                 member = None
 
-    def add(self, score: float, member: bytes):
+    def add(self, score: float, member: bytes) -> None:
         if member in self.members_scores:
             old_score = self.members_scores[member]
             self.members.remove((old_score, member))
         self.members_scores[member] = score
         self.members.add((score, member))
 
     def range_by_score(
@@ -104,22 +111,22 @@
         min_score: float,
         max_score: float,
         min_inclusive: bool,
         max_inclusive: bool,
         with_scores: bool = False,
         is_reversed: bool = False,
         limit: RangeLimit | None = None,
-    ):
+    ) -> Iterable[bytes | float]:
         if not is_reversed:
-            minimum = (min_score, (b"" if min_inclusive else MAX_STRING))
-            maximum = (max_score, (MAX_STRING if max_inclusive else b""))
+            minimum = (min_score, (b"" if min_inclusive else MAX_BYTES))
+            maximum = (max_score, (MAX_BYTES if max_inclusive else b""))
         else:
             min_inclusive, max_inclusive = max_inclusive, min_inclusive
-            minimum = (max_score, (b"" if max_inclusive else MAX_STRING))
-            maximum = (min_score, (MAX_STRING if min_inclusive else b""))
+            minimum = (max_score, (b"" if max_inclusive else MAX_BYTES))
+            maximum = (min_score, (MAX_BYTES if min_inclusive else b""))
 
         iterator = self.members.irange(minimum, maximum, (min_inclusive, max_inclusive), reverse=is_reversed)
 
         if limit:
             offset = limit.offset
             count = limit.count + limit.offset
         else:
@@ -134,103 +141,99 @@
 
     def range_by_lexical(
         self,
         min_lex: bytes,
         max_lex: bytes,
         min_inclusive: bool,
         max_inclusive: bool,
-        with_scores=False,
-        is_reversed=False,
-        limit=None,
-    ):
+        with_scores: bool = False,
+        is_reversed: bool = False,
+        limit: RangeLimit | None = None,
+    ) -> Iterable[bytes | float]:
         if not is_reversed:
             minimum, maximum = min_lex, max_lex
         else:
             minimum, maximum = max_lex, min_lex
             min_inclusive, max_inclusive = max_inclusive, min_inclusive
 
         iterator = self.members_scores.irange(minimum, maximum, (min_inclusive, max_inclusive), reverse=is_reversed)
 
         if limit:
-            offset = limit["offset"]
-            count = limit["count"] + limit["offset"]
+            offset = limit.offset
+            count = limit.count + limit.offset
         else:
             offset = None
             count = None
         for member in itertools.islice(iterator, offset, count):
             if with_scores:
                 yield member
                 yield self.members_scores[member]
             else:
                 yield member
 
-    def range(self, range_slice, with_scores=False, limit=None):
+    def range(self, range_slice: slice, with_scores: bool = False) -> list[bytes | float]:
         result = self.members[range_slice]
 
-        if limit:
-            offset = limit["offset"]
-            count = limit["count"] + limit["offset"]
-        else:
-            offset = None
-            count = None
+        offset = None
+        count = None
         if with_scores:
             return list(itertools.islice(flatten(result, reverse_sub_lists=True), offset, count))
         return list(itertools.islice((member for score, member in result), offset, count))
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.members)
 
 
 class Database(dict[bytes, Any]):
-    def get_by_type(self, key, type_):
+    def get_by_type(self, key: bytes, type_: type) -> Any:  # noqa: ANN401
         value = type_()
         if key in self:
             value = self[key]
         if not isinstance(value, type_):
-            raise ServerWrongType()
+            raise ServerWrongTypeError()
         return value
 
-    def get_or_create_by_type(self, key, type_):
+    def get_or_create_by_type(self, key: bytes, type_: type) -> Any:  # noqa: ANN401
         if key not in self:
             self[key] = type_()
         value = self[key]
         if not isinstance(value, type_):
-            raise ServerWrongType()
+            raise ServerWrongTypeError()
         return value
 
-    def get_string(self, key) -> ServerString:
+    def get_string(self, key: bytes) -> ServerString:
         return self.get_by_type(key, ServerString)
 
-    def get_string_or_none(self, key) -> ServerString | None:
+    def get_string_or_none(self, key: bytes) -> ServerString | None:
         if key not in self:
             return None
         s = self[key]
         if not isinstance(s, ServerString):
-            raise ServerWrongType()
+            raise ServerWrongTypeError()
         return s
 
-    def get_or_create_string(self, key) -> ServerString:
+    def get_or_create_string(self, key: bytes) -> ServerString:
         return self.get_or_create_by_type(key, ServerString)
 
-    def get_hash_table(self, key) -> dict:
+    def get_hash_table(self, key: bytes) -> dict:
         return self.get_by_type(key, dict)
 
-    def get_or_create_hash_table(self, key) -> dict:
+    def get_or_create_hash_table(self, key: bytes) -> dict:
         return self.get_or_create_by_type(key, dict)
 
-    def get_list(self, key) -> list:
+    def get_list(self, key: bytes) -> list:
         return self.get_by_type(key, list)
 
-    def get_or_create_list(self, key) -> list:
+    def get_or_create_list(self, key: bytes) -> list:
         return self.get_or_create_by_type(key, list)
 
-    def get_sorted_set(self, key) -> ServerSortedSet:
+    def get_sorted_set(self, key: bytes) -> ServerSortedSet:
         return self.get_by_type(key, ServerSortedSet)
 
-    def get_or_create_sorted_set(self, key) -> ServerSortedSet:
+    def get_or_create_sorted_set(self, key: bytes) -> ServerSortedSet:
         return self.get_or_create_by_type(key, ServerSortedSet)
 
-    def get_set(self, key) -> set:
+    def get_set(self, key: bytes) -> set:
         return self.get_by_type(key, set)
 
-    def get_or_create_set(self, key) -> set:
+    def get_or_create_set(self, key: bytes) -> set:
         return self.get_or_create_by_type(key, set)
```

### Comparing `pyvalkey-0.0.4/pyvalkey/database_objects/information.py` & `pyvalkey-0.0.5/pyvalkey/database_objects/information.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 class Information:
     server_version: bytes = b"7.0.0"
     arch_bits: bytes = b"64"
     cluster_enabled: bool = False
     enterprise: bool = False
     total_commands_processed: int = 0
 
-    def all(self):
+    def all(self) -> bytes:
         return b"\r\n".join(
             [
                 b"# Server",
-                b"valkey_version:" + self.server_version,
+                b"redis_version:" + self.server_version,
                 b"arch_bits:" + self.arch_bits,
                 b"",
                 b"# Cluster",
                 b"cluster_enabled:" + (b"1" if self.cluster_enabled else b"0"),
                 b"",
                 b"# Stats",
                 b"total_commands_processed:" + to_bytes(self.total_commands_processed),
```

### Comparing `pyvalkey-0.0.4/pyvalkey/resp.py` & `pyvalkey-0.0.5/pyvalkey/resp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,105 +1,113 @@
 from dataclasses import dataclass
-from typing import Any, AnyStr, BinaryIO
+from typing import AnyStr, BinaryIO
 
 
 class RespSimpleString(bytes):
     pass
 
 
 RESP_OK = RespSimpleString(b"OK")
 
 
 class RespError(bytes):
     pass
 
 
+ValueType = bool | int | float | RespSimpleString | RespError | str | bytes | list | set | dict | None
+LoadedType = list | bytes | int | None
+
+
 @dataclass
 class RespLoader:
     reader: BinaryIO
 
-    def load_array(self, length: int):
-        array = [None] * length
+    def load_array(self, length: int) -> list[LoadedType]:
+        array: list[LoadedType] = [None] * length
         for i in range(length):
             array[i] = self.load()
         return array
 
-    def load(self):
-        line = self.reader.readline().strip()
+    def load(self) -> LoadedType:
+        line = self.reader.readline().strip(b"\r\n")
         match line[0:1], line[1:]:
             case b"*", length:
                 return self.load_array(int(length))
             case b"$", length:
-                bulk_string = self.reader.read(int(length) + 2).strip()
+                bulk_string = self.reader.read(int(length) + 2).strip(b"\r\n")
                 if len(bulk_string) != int(length):
                     raise ValueError()
                 return bulk_string
             case b":", value:
                 return int(value)
             case b"+", value:
                 return RespSimpleString(value)
             case b"-", value:
                 return RespError(value)
             case _:
                 return None
 
+    def load_dynamic_array(self) -> list:
+        line = self.reader.readline().strip(b"\r\n")
+        return self.load_array(int(line[1:]))
+
 
-def load(stream: BinaryIO):
-    return RespLoader(stream).load()
+def load(stream: BinaryIO) -> list:
+    return RespLoader(stream).load_dynamic_array()
 
 
 @dataclass
 class RespDumper:
     writer: BinaryIO
 
-    def dump_bulk_string(self, value: AnyStr):
+    def dump_bulk_string(self, value: AnyStr) -> None:
         if isinstance(value, str):
             bytes_value = value.encode()
         else:
             bytes_value = value
         self.writer.write(b"$" + str(len(bytes_value)).encode() + b"\r\n" + bytes_value + b"\r\n")
 
-    def dump_string(self, value: AnyStr):
+    def dump_string(self, value: AnyStr) -> None:
         if isinstance(value, str):
             bytes_value = value.encode()
         else:
             bytes_value = value
         self.writer.write(b"+" + bytes_value + b"\r\n")
 
-    def dump_array(self, value: list):
+    def dump_array(self, value: list) -> None:
         self.writer.write(f"*{len(value)}\r\n".encode())
         for item in value:
             self.dump(item)
 
-    def dump(self, value):
+    def dump(self, value: ValueType) -> None:
         if isinstance(value, bool):
             if value:
                 self.dump(1)
             else:
                 self.dump(0)
         elif isinstance(value, int):
             self.writer.write(f":{value}\r\n".encode())
         elif isinstance(value, float):
             self.dump_bulk_string(f"{value:g}")
         elif isinstance(value, RespSimpleString):
             self.dump_string(value)
         elif isinstance(value, RespError):
             self.writer.write(f"-{value.decode()}\r\n".encode())
-        elif isinstance(value, (str, bytes)):
+        elif isinstance(value, str | bytes):
             if isinstance(value, str):
                 value = value.encode()
             self.dump_bulk_string(value)
         elif isinstance(value, list):
             self.dump_array(value)
         elif isinstance(value, set):
             self.dump_array(list(value))
         elif isinstance(value, dict):
             result = []
             for k, v in value.items():
                 result += [k, v]
             self.dump_array(result)
         elif value is None:
-            self.writer.write("$-1\r\n".encode())
+            self.writer.write(b"$-1\r\n")
 
 
-def dump(value: Any, stream: BinaryIO):
+def dump(value: ValueType, stream: BinaryIO) -> None:
     RespDumper(stream).dump(value)
```

### Comparing `pyvalkey-0.0.4/pyvalkey/server.py` & `pyvalkey-0.0.5/pyvalkey/server.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 import itertools
 import logging
+import select
 import time
 from collections import defaultdict
 from io import BytesIO
 from socket import socket
 from socketserver import StreamRequestHandler, ThreadingTCPServer
 
 from pyvalkey.commands.context import ClientContext, ServerContext
 from pyvalkey.commands.router import ServerCommandsRouter
 from pyvalkey.database_objects.acl import ACL
 from pyvalkey.database_objects.clients import Client, ClientList
 from pyvalkey.database_objects.configurations import Configurations
 from pyvalkey.database_objects.databases import Database
 from pyvalkey.database_objects.errors import (
-    ServerException,
+    CommandPermissionError,
+    RouterKeyError,
+    ServerError,
     ServerInvalidIntegerError,
     ServerSyntaxError,
-    ServerWrongType,
-    RouterKeyError,
+    ServerWrongTypeError,
 )
 from pyvalkey.database_objects.information import Information
-from pyvalkey.resp import RESP_OK, RespError, dump, load
+from pyvalkey.resp import RESP_OK, RespError, ValueType, dump, load
 
 logger = logging.getLogger(__name__)
 
 
 class ServerConnectionHandler(StreamRequestHandler):
-    def __init__(self, request, client_address, server: "ValkeyServer"):
+    def __init__(self, request: socket, client_address: tuple[str, int], server: "ValkeyServer") -> None:
         super().__init__(request, client_address, server)
         self.server: ValkeyServer = server
-        self.request: socket
 
         self.current_database = self.databases[0]
         self.current_client: Client
 
     @property
-    def configurations(self):
+    def configurations(self) -> Configurations:
         return self.server.configurations
 
     @property
-    def databases(self):
+    def databases(self) -> defaultdict[int, Database]:
         return self.server.databases
 
     @property
-    def clients(self):
+    def clients(self) -> ClientList:
         return self.server.clients
 
     @property
-    def acl(self):
+    def acl(self) -> ACL:
         return self.server.acl
 
     def setup(self) -> None:
         super().setup()
 
         self.current_client = self.clients.create_client(
             host=self.client_address[0].encode(),
@@ -69,74 +70,96 @@
         self.client_context = ClientContext(
             self.server_context,
             current_client=self.current_client,
         )
 
         self.router = ServerCommandsRouter()
 
-    def dump(self, value):
+    def dump(self, value: ValueType) -> None:
         dumped = BytesIO()
         dump(value, dumped)
         print(self.current_client.client_id, "result", dumped.getvalue())
 
         if self.current_client.reply_mode == "skip":
             self.current_client.reply_mode = "on"
             return
 
         if self.current_client.reply_mode == "off":
             return
 
         dump(value, self.wfile)
 
-    def handle(self):
+    def handle(self) -> None:
         while not self.current_client.is_killed:
+            ready = select.select([self.connection], [], [], 1)
+            if not ready:
+                continue
             command = load(self.rfile)
 
             if command is None:
                 break
             if command[0] == b"QUIT":
                 self.dump(RESP_OK)
                 break
 
             self.server.information.total_commands_processed += 1
 
             print(self.current_client.client_id, command)
 
             try:
-                self.dump(self.router.route(list(command), self.client_context).execute())
+                routed_command = self.router.route(list(command), self.client_context)
+
+                if self.client_context.current_user:
+                    self.client_context.current_user.check_permissions(routed_command)
+
+                self.dump(routed_command.execute())
                 if self.server_context.pause_timeout:
                     while self.server_context.is_paused and time.time() < self.server_context.pause_timeout:
                         time.sleep(0.1)
                     self.server_context.pause_timeout = 0
             except RouterKeyError:
-                return RespError(
-                    f"ERR unknown command '{command[0]}', "
-                    f"with args beginning with: {command[1] if len(command) > 1 else ''}".encode()
+                self.dump(
+                    RespError(
+                        f"ERR unknown command '{command[0]}', "
+                        f"with args beginning with: {command[1] if len(command) > 1 else ''}".encode()
+                    )
                 )
-            except ServerWrongType:
+            except ServerWrongTypeError:
                 self.dump(RespError(b"WRONGTYPE Operation against a key holding the wrong kind of value"))
             except ServerSyntaxError:
                 self.dump(RespError(b"ERR syntax error"))
             except ServerInvalidIntegerError:
                 self.dump(RespError(b"ERR hash value is not an integer"))
-            except ServerException as e:
+            except CommandPermissionError as e:
+                if not self.client_context.current_user:
+                    raise e
+                self.dump(
+                    RespError(
+                        b"NOPERM User "
+                        + self.client_context.current_user.name
+                        + b" has no permissions to run the '"
+                        + e.command_name
+                        + b"' command"
+                    )
+                )
+            except ServerError as e:
                 self.dump(RespError(e.message))
             except Exception as e:
                 self.dump(RespError(b"ERR internal"))
                 raise e
 
         print(self.current_client.client_id, "exited")
 
     def finish(self) -> None:
         del self.clients[self.current_client.client_id]
         super().finish()
 
 
 class ValkeyServer(ThreadingTCPServer):
-    def __init__(self, server_address, bind_and_activate=True):
+    def __init__(self, server_address: tuple[str, int], bind_and_activate: bool = True) -> None:
         super().__init__(server_address, ServerConnectionHandler, bind_and_activate)
         self.databases: defaultdict[int, Database] = defaultdict(Database, {0: Database()})
         self.acl: ACL = ACL.create()
         self.client_ids = itertools.count(0)
         self.clients: ClientList = ClientList()
         self.configurations: Configurations = Configurations()
         self.information: Information = Information()
```

### Comparing `pyvalkey-0.0.4/README.md` & `pyvalkey-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# r3dis: Python implemented Valkey server
+# pyvalkey: Python implemented Valkey server
 
 [![PyPI version](https://img.shields.io/pypi/v/r3dis.svg)](https://pypi.python.org/pypi/r3dis/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/r3dis.svg)](https://pypi.python.org/pypi/r3dis/)
 [![GitHub](https://img.shields.io/github/license/netanelrevah/r3dis)](https://pypi.python.org/pypi/r3dis/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/r3dis)](https://pypi.python.org/pypi/r3dis/)
 
 Tired of DevOps telling you not deploy Valkey on your system?
@@ -66,8 +66,8 @@
 * KEYS
 * APPEND
 
 in the future:
 * more commands
 * support for multiple client using asyncio loop instead of thread per client
 
-you are invited to help :)
+you are invited to help :)
```

### Comparing `pyvalkey-0.0.4/PKG-INFO` & `pyvalkey-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: pyvalkey
-Version: 0.0.4
+Version: 0.0.5
 Summary: pyvalkey: Python implemented Valkey server
 License: MIT
 Author: Netanel Revah
 Author-email: netanelrevah@outlook.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.12,<0.13)
 Requires-Dist: typing-extensions (>=4.8.0,<5.0.0)
 Description-Content-Type: text/markdown
 
-# r3dis: Python implemented Valkey server
+# pyvalkey: Python implemented Valkey server
 
 [![PyPI version](https://img.shields.io/pypi/v/r3dis.svg)](https://pypi.python.org/pypi/r3dis/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/r3dis.svg)](https://pypi.python.org/pypi/r3dis/)
 [![GitHub](https://img.shields.io/github/license/netanelrevah/r3dis)](https://pypi.python.org/pypi/r3dis/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/r3dis)](https://pypi.python.org/pypi/r3dis/)
 
 Tired of DevOps telling you not deploy Valkey on your system?
@@ -85,7 +84,8 @@
 * APPEND
 
 in the future:
 * more commands
 * support for multiple client using asyncio loop instead of thread per client
 
 you are invited to help :)
+
```

