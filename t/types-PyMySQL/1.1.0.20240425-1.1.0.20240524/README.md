# Comparing `tmp/types-PyMySQL-1.1.0.20240425.tar.gz` & `tmp/types-PyMySQL-1.1.0.20240524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-PyMySQL-1.1.0.20240425.tar", last modified: Thu Apr 25 02:19:06 2024, max compression
+gzip compressed data, was "types-PyMySQL-1.1.0.20240524.tar", last modified: Fri May 24 02:22:30 2024, max compression
```

## Comparing `types-PyMySQL-1.1.0.20240425.tar` & `types-PyMySQL-1.1.0.20240524.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:06.119223 types-PyMySQL-1.1.0.20240425/
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-25 02:19:05.000000 types-PyMySQL-1.1.0.20240425/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 02:19:05.000000 types-PyMySQL-1.1.0.20240425/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-25 02:19:06.119223 types-PyMySQL-1.1.0.20240425/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:06.119223 types-PyMySQL-1.1.0.20240425/pymysql-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-25 02:19:05.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/charset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/connections.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:06.119223 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/CLIENT.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/COMMAND.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/CR.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/ER.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/FIELD_TYPE.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/FLAG.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/SERVER_STATUS.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/converters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/cursors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/err.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 02:19:05.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/times.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-25 02:18:23.000000 types-PyMySQL-1.1.0.20240425/pymysql-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:19:06.119223 types-PyMySQL-1.1.0.20240425/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-25 02:19:05.000000 types-PyMySQL-1.1.0.20240425/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:06.119223 types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-25 02:19:06.000000 types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-25 02:19:06.000000 types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:19:06.000000 types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 02:19:06.000000 types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:22:30.246662 types-PyMySQL-1.1.0.20240524/
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-24 02:22:28.000000 types-PyMySQL-1.1.0.20240524/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 02:22:28.000000 types-PyMySQL-1.1.0.20240524/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-24 02:22:30.246662 types-PyMySQL-1.1.0.20240524/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:22:30.246662 types-PyMySQL-1.1.0.20240524/pymysql-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-24 02:22:28.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/charset.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/connections.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:22:30.246662 types-PyMySQL-1.1.0.20240524/pymysql-stubs/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/constants/CLIENT.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/constants/COMMAND.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/constants/CR.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/constants/ER.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/constants/FIELD_TYPE.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/constants/FLAG.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/constants/SERVER_STATUS.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/constants/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/converters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/cursors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/err.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 02:22:28.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/times.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 02:22:16.000000 types-PyMySQL-1.1.0.20240524/pymysql-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 02:22:30.246662 types-PyMySQL-1.1.0.20240524/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-24 02:22:28.000000 types-PyMySQL-1.1.0.20240524/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:22:30.246662 types-PyMySQL-1.1.0.20240524/types_PyMySQL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-24 02:22:30.000000 types-PyMySQL-1.1.0.20240524/types_PyMySQL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-24 02:22:30.000000 types-PyMySQL-1.1.0.20240524/types_PyMySQL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:22:30.000000 types-PyMySQL-1.1.0.20240524/types_PyMySQL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-24 02:22:30.000000 types-PyMySQL-1.1.0.20240524/types_PyMySQL.egg-info/top_level.txt
```

### Comparing `types-PyMySQL-1.1.0.20240425/CHANGELOG.md` & `types-PyMySQL-1.1.0.20240524/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.1.0.20240524 (2024-05-24)
+
+Update PyMySQL to 1.1.1 (#12001)
+
+Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
+
 ## 1.1.0.20240425 (2024-04-25)
 
 Bump pyright to v1.1.360 (#11810)
 
 ## 1.1.0.1 (2023-07-20)
 
 Add an upstream_repository field to METADATA.toml (#10487)
```

### Comparing `types-PyMySQL-1.1.0.20240425/PKG-INFO` & `types-PyMySQL-1.1.0.20240524/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyMySQL
-Version: 1.1.0.20240425
+Version: 1.1.0.20240524
 Summary: Typing stubs for PyMySQL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyMySQL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
-with mypy 1.10.0, pyright 1.1.360, and
+This package was generated from typeshed commit `ac6c61ba04c3d3abf476570de04a9afe7447890b` and was tested
+with mypy 1.10.0, pyright 1.1.364, and
 pytype 2024.4.11.
```

### Comparing `types-PyMySQL-1.1.0.20240425/pymysql-stubs/__init__.pyi` & `types-PyMySQL-1.1.0.20240524/pymysql-stubs/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Final
+
 from .connections import Connection as Connection
 from .constants import FIELD_TYPE as FIELD_TYPE
 from .converters import escape_dict as escape_dict, escape_sequence as escape_sequence, escape_string as escape_string
 from .err import (
     DatabaseError as DatabaseError,
     DataError as DataError,
     Error as Error,
@@ -19,14 +21,17 @@
     DateFromTicks as DateFromTicks,
     Time as Time,
     TimeFromTicks as TimeFromTicks,
     Timestamp as Timestamp,
     TimestampFromTicks as TimestampFromTicks,
 )
 
+VERSION: Final[tuple[str | int, ...]]
+VERSION_STRING: Final[str]
+
 threadsafety: int
 apilevel: str
 paramstyle: str
 
 class DBAPISet(frozenset[int]):
     def __ne__(self, other) -> bool: ...
     def __eq__(self, other) -> bool: ...
```

### Comparing `types-PyMySQL-1.1.0.20240425/pymysql-stubs/connections.pyi` & `types-PyMySQL-1.1.0.20240524/pymysql-stubs/connections.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from _typeshed import Incomplete
 from collections.abc import Mapping
 from socket import socket as _socket
+from ssl import _PasswordType
 from typing import Any, AnyStr, Generic, TypeVar, overload
 from typing_extensions import Self
 
 from .charset import charset_by_id as charset_by_id, charset_by_name as charset_by_name
 from .constants import CLIENT as CLIENT, COMMAND as COMMAND, FIELD_TYPE as FIELD_TYPE, SERVER_STATUS as SERVER_STATUS
 from .cursors import Cursor
 from .util import byte2int as byte2int, int2byte as int2byte
@@ -99,14 +100,15 @@
         init_command: Incomplete | None = None,
         connect_timeout: int | None = 10,
         ssl: Mapping[Any, Any] | None = None,
         ssl_ca=None,
         ssl_cert=None,
         ssl_disabled=None,
         ssl_key=None,
+        ssl_key_password: _PasswordType | None = None,
         ssl_verify_cert=None,
         ssl_verify_identity=None,
         read_default_group: Incomplete | None = None,
         compress: Incomplete | None = None,
         named_pipe: Incomplete | None = None,
         autocommit: bool | None = False,
         db: Incomplete | None = None,
```

### Comparing `types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/COMMAND.pyi` & `types-PyMySQL-1.1.0.20240524/pymysql-stubs/constants/COMMAND.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/CR.pyi` & `types-PyMySQL-1.1.0.20240524/pymysql-stubs/constants/CR.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.20240425/pymysql-stubs/constants/ER.pyi` & `types-PyMySQL-1.1.0.20240524/pymysql-stubs/constants/ER.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.20240425/pymysql-stubs/converters.pyi` & `types-PyMySQL-1.1.0.20240524/pymysql-stubs/converters.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import datetime
 import time
 from _typeshed import Unused
 from collections.abc import Callable, Mapping, Sequence
 from decimal import Decimal
-from typing import Any, TypeVar
-from typing_extensions import TypeAlias
+from typing import Any, NoReturn, TypeVar
+from typing_extensions import TypeAlias, deprecated
 
 _EscaperMapping: TypeAlias = Mapping[type[object], Callable[..., str]] | None
 _T = TypeVar("_T")
 
 def escape_item(val: object, charset: object, mapping: _EscaperMapping = None) -> str: ...
-def escape_dict(val: Mapping[str, object], charset: object, mapping: _EscaperMapping = None) -> dict[str, str]: ...
+@deprecated("dict cannot be used as parameter. It didn't produce valid SQL and might cause SQL injection.")
+def escape_dict(val: Mapping[str, object], charset: object, mapping: _EscaperMapping = None) -> NoReturn: ...
 def escape_sequence(val: Sequence[object], charset: object, mapping: _EscaperMapping = None) -> str: ...
 def escape_set(val: set[object], charset: object, mapping: _EscaperMapping = None) -> str: ...
 def escape_bool(value: bool, mapping: _EscaperMapping = None) -> str: ...
 def escape_int(value: int, mapping: _EscaperMapping = None) -> str: ...
 def escape_float(value: float, mapping: _EscaperMapping = None) -> str: ...
 def escape_string(value: str, mapping: _EscaperMapping = None) -> str: ...
 def escape_bytes_prefixed(value: bytes, mapping: _EscaperMapping = None) -> str: ...
```

### Comparing `types-PyMySQL-1.1.0.20240425/pymysql-stubs/cursors.pyi` & `types-PyMySQL-1.1.0.20240524/pymysql-stubs/cursors.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.20240425/pymysql-stubs/err.pyi` & `types-PyMySQL-1.1.0.20240524/pymysql-stubs/err.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.20240425/setup.py` & `types-PyMySQL-1.1.0.20240524/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
-with mypy 1.10.0, pyright 1.1.360, and
+This package was generated from typeshed commit `ac6c61ba04c3d3abf476570de04a9afe7447890b` and was tested
+with mypy 1.10.0, pyright 1.1.364, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="1.1.0.20240425",
+      version="1.1.0.20240524",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyMySQL.md",
```

### Comparing `types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/PKG-INFO` & `types-PyMySQL-1.1.0.20240524/types_PyMySQL.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyMySQL
-Version: 1.1.0.20240425
+Version: 1.1.0.20240524
 Summary: Typing stubs for PyMySQL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyMySQL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
-with mypy 1.10.0, pyright 1.1.360, and
+This package was generated from typeshed commit `ac6c61ba04c3d3abf476570de04a9afe7447890b` and was tested
+with mypy 1.10.0, pyright 1.1.364, and
 pytype 2024.4.11.
```

### Comparing `types-PyMySQL-1.1.0.20240425/types_PyMySQL.egg-info/SOURCES.txt` & `types-PyMySQL-1.1.0.20240524/types_PyMySQL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

