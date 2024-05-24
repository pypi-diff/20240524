# Comparing `tmp/arrow_odbc-6.0.0.tar.gz` & `tmp/arrow_odbc-7.0.0.tar.gz`

## Comparing `arrow_odbc-6.0.0.tar` & `arrow_odbc-7.0.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 arrow_odbc-6.0.0/Cargo.toml
--rw-r--r--   0      501       20      136 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/.gitattributes
--rw-r--r--   0      501       20      213 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/.github/dependabot.yml
--rw-r--r--   0      501       20     1762 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/.github/workflows/test.yml
--rw-r--r--   0      501       20     2648 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/.github/workflows/wheel.yml
--rw-r--r--   0      501       20      286 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/.gitignore
--rw-r--r--   0      501       20      841 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/.readthedocs.yaml
--rw-r--r--   0      501       20    11859 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/Changelog.md
--rw-r--r--   0      501       20     1954 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/Contributing.md
--rw-r--r--   0      501       20     1069 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/LICENSE
--rw-r--r--   0      501       20     7988 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/README.md
--rw-r--r--   0      501       20       14 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/cbindgen.toml
--rw-r--r--   0      501       20      623 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/conftest.py
--rw-r--r--   0      501       20      638 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/Makefile
--rw-r--r--   0      501       20      804 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/make.bat
--rw-r--r--   0      501       20       16 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/requirements.txt
--rw-r--r--   0      501       20      155 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/source/arrow_odbc.rst
--rw-r--r--   0      501       20     1965 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/source/conf.py
--rw-r--r--   0      501       20      458 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/source/index.rst
--rw-r--r--   0      501       20       67 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/source/modules.rst
--rw-r--r--   0      501       20      348 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/docker-compose.yml
--rw-r--r--   0      501       20      564 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/manylinux/Dockerfile
--rw-r--r--   0      501       20      121 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/manylinux/Readme.md
--rw-r--r--   0      501       20      148 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/manylinux/WHEEL
--rw-r--r--   0      501       20     1256 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/manylinux/build_wheel.sh
--rw-r--r--   0      501       20      446 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/__init__.py
--rw-r--r--   0      501       20     1946 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/connect.py
--rw-r--r--   0      501       20      672 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/error.py
--rw-r--r--   0      501       20      788 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/log.py
--rw-r--r--   0      501       20      578 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/pool.py
--rw-r--r--   0      501       20    25180 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/reader.py
--rw-r--r--   0      501       20     9625 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/writer.py
--rw-r--r--   0      501       20     2322 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/error.rs
--rw-r--r--   0      501       20     3434 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/lib.rs
--rw-r--r--   0      501       20      655 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/logging.rs
--rw-r--r--   0      501       20     1239 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/parameter.rs
--rw-r--r--   0      501       20      421 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/pool.rs
--rw-r--r--   0      501       20     8757 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/reader/arrow_odbc_reader.rs
--rw-r--r--   0      501       20    12865 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/reader.rs
--rw-r--r--   0      501       20     3545 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/writer.rs
--rw-r--r--   0      501       20   274432 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/temp_db.duckdb
--rw-r--r--   0      501       20        0 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/tests/__init__.py
--rw-r--r--   0      501       20     4115 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/tests/iris.csv
--rw-r--r--   0      501       20     2413 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/tests/iris.parquet
--rw-r--r--   0      501       20    29032 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/tests/test_arrow_odbc.py
--rw-r--r--   0      501       20    43744 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/Cargo.lock
--rw-r--r--   0      501       20      825 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/pyproject.toml
--rw-r--r--   0        0        0     8600 1970-01-01 00:00:00.000000 arrow_odbc-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 arrow_odbc-7.0.0/Cargo.toml
+-rw-r--r--   0      501       20      136 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/.gitattributes
+-rw-r--r--   0      501       20      213 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/.github/dependabot.yml
+-rw-r--r--   0      501       20     1762 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/.github/workflows/test.yml
+-rw-r--r--   0      501       20     2648 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/.github/workflows/wheel.yml
+-rw-r--r--   0      501       20      286 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/.gitignore
+-rw-r--r--   0      501       20      841 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/.readthedocs.yaml
+-rw-r--r--   0      501       20    12072 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/Changelog.md
+-rw-r--r--   0      501       20     1954 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/Contributing.md
+-rw-r--r--   0      501       20     1069 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/LICENSE
+-rw-r--r--   0      501       20     8040 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/README.md
+-rw-r--r--   0      501       20       14 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/cbindgen.toml
+-rw-r--r--   0      501       20      623 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/conftest.py
+-rw-r--r--   0      501       20      638 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/Makefile
+-rw-r--r--   0      501       20      804 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/make.bat
+-rw-r--r--   0      501       20       16 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/requirements.txt
+-rw-r--r--   0      501       20      155 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/source/arrow_odbc.rst
+-rw-r--r--   0      501       20     1965 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/source/conf.py
+-rw-r--r--   0      501       20      458 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/source/index.rst
+-rw-r--r--   0      501       20       67 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/source/modules.rst
+-rw-r--r--   0      501       20      348 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/docker-compose.yml
+-rw-r--r--   0      501       20      564 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/manylinux/Dockerfile
+-rw-r--r--   0      501       20      121 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/manylinux/Readme.md
+-rw-r--r--   0      501       20      148 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/manylinux/WHEEL
+-rw-r--r--   0      501       20     1256 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/manylinux/build_wheel.sh
+-rw-r--r--   0      501       20      446 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/__init__.py
+-rw-r--r--   0      501       20     1885 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/connect.py
+-rw-r--r--   0      501       20      672 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/error.py
+-rw-r--r--   0      501       20      788 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/log.py
+-rw-r--r--   0      501       20      578 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/pool.py
+-rw-r--r--   0      501       20    25240 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/reader.py
+-rw-r--r--   0      501       20     9625 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/writer.py
+-rw-r--r--   0      501       20     2322 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/error.rs
+-rw-r--r--   0      501       20     3434 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/lib.rs
+-rw-r--r--   0      501       20      655 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/logging.rs
+-rw-r--r--   0      501       20     1239 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/parameter.rs
+-rw-r--r--   0      501       20      421 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/pool.rs
+-rw-r--r--   0      501       20     8757 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/reader/arrow_odbc_reader.rs
+-rw-r--r--   0      501       20    12865 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/reader.rs
+-rw-r--r--   0      501       20     3545 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/writer.rs
+-rw-r--r--   0      501       20   274432 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/temp_db.duckdb
+-rw-r--r--   0      501       20        0 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/tests/__init__.py
+-rw-r--r--   0      501       20     4115 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/tests/iris.csv
+-rw-r--r--   0      501       20     2413 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/tests/iris.parquet
+-rw-r--r--   0      501       20    29032 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/tests/test_arrow_odbc.py
+-rw-r--r--   0      501       20    42700 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/Cargo.lock
+-rw-r--r--   0      501       20      825 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8652 1970-01-01 00:00:00.000000 arrow_odbc-7.0.0/PKG-INFO
```

### Comparing `arrow_odbc-6.0.0/Cargo.toml` & `arrow_odbc-7.0.0/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 [lib]
 # Name needs to be identical to python package name
 name = "arrow_odbc"
 crate-type = ["cdylib"]
 
 [dependencies]
-arrow-odbc = "9.0.0"
+arrow-odbc = "11.0.0"
 # arrow would be included indirectly using arrow-odbc, but we need to explicitly specify the ffi
 # feature.
 arrow = { version = "51.0.0", default-features = false, features = ["ffi"] }
 stderrlog = "0.6.0"
 log = "0.4.21"
 
 [profile.release]
```

### Comparing `arrow_odbc-6.0.0/.github/workflows/test.yml` & `arrow_odbc-7.0.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/.github/workflows/wheel.yml` & `arrow_odbc-7.0.0/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/.readthedocs.yaml` & `arrow_odbc-7.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/Changelog.md` & `arrow_odbc-7.0.0/Changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # Changelog
 
+## 7.0.0
+
+- unsigned TinyInt is now mapped to `UInt8`.
+
 ## 6.0.0
 
 - Support for passing desired packet size to the ODBC driver. This may help with packet loss on fragile connections if the ODBC driver supports it.
+- `insert_into_table` will now wrap column names in double quotes then creating the statement, if the column name is not a valid identifier in transact SQL.
 
 ## 5.0.0
 
 - Fix: Database connection have not been cleaned up in case the parameters caused a type error.
 - Changend `BatchReader.to_pyarrow_record_batch_reader` into `BatchReader.into_pyarrow_record_batch_reader`. The new method fully passes ownership and leaves self empty.
 
 ## 4.2.0
```

### Comparing `arrow_odbc-6.0.0/Contributing.md` & `arrow_odbc-7.0.0/Contributing.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/LICENSE` & `arrow_odbc-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/README.md` & `arrow_odbc-7.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,16 @@
 | Date                     | Date32               |
 | LongVarbinary            | Binary               |
 | Timestamp(p = 0)         | TimestampSecond      |
 | Timestamp(p: 1..3)       | TimestampMilliSecond |
 | Timestamp(p: 4..6)       | TimestampMicroSecond |
 | Timestamp(p >= 7 )       | TimestampNanoSecond  |
 | BigInt                   | Int64                |
-| TinyInt                  | Int8                 |
+| TinyInt Signed           | Int8                 |
+| TinyInt Unsigned         | UInt8                |
 | Bit                      | Boolean              |
 | Varbinary                | Binary               |
 | Binary                   | FixedSizedBinary     |
 | All others               | Utf8                 |
 
 ## Matching of Arrow to ODBC types then inserting
```

### Comparing `arrow_odbc-6.0.0/conftest.py` & `arrow_odbc-7.0.0/conftest.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/doc/Makefile` & `arrow_odbc-7.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/doc/make.bat` & `arrow_odbc-7.0.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/doc/source/conf.py` & `arrow_odbc-7.0.0/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "arrow-odbc"
 copyright = "2021, Markus Klein"
 author = "Markus Klein"
 
 # The full version, including alpha/beta/rc tags
-release = "6.0.0"
+release = "7.0.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `arrow_odbc-6.0.0/manylinux/Dockerfile` & `arrow_odbc-7.0.0/manylinux/Dockerfile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/manylinux/build_wheel.sh` & `arrow_odbc-7.0.0/manylinux/build_wheel.sh`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/python/arrow_odbc/connect.py` & `arrow_odbc-7.0.0/python/arrow_odbc/connect.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from typing import Any, Optional, Tuple
 from cffi.api import FFI  # type: ignore
 
-from pyarrow.cffi import ffi as arrow_ffi  # type: ignore
-
 from .arrow_odbc import ffi, lib  # type: ignore
 from arrow_odbc.error import raise_on_error
 
 
 def to_bytes_and_len(value: Optional[str]) -> Tuple[bytes, int]:
     if value is None:
         value_bytes = FFI.NULL
```

### Comparing `arrow_odbc-6.0.0/python/arrow_odbc/error.py` & `arrow_odbc-7.0.0/python/arrow_odbc/error.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/python/arrow_odbc/log.py` & `arrow_odbc-7.0.0/python/arrow_odbc/log.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/python/arrow_odbc/pool.py` & `arrow_odbc-7.0.0/python/arrow_odbc/pool.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/python/arrow_odbc/reader.py` & `arrow_odbc-7.0.0/python/arrow_odbc/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,17 +312,18 @@
 
         ``arrow-odbc``s BatchReader interface offers some functionality specific to ODBC
         datasources. E.g. the ability to move to the next result set of a stored procedure. You may
         not need this extra functionality and would rather like to integrate the ``BatchReader``
         with other libraries like e.g. DuckDB. In order to do this you can use this method to
         convert the ``arrow-odbc`` BatchReader into a ``pyarrow`` ``RecordBatchReader``.
         """
-        # Move self to tmp
+        # New empty tmp reader
         reader = _BatchReaderRaii()
         tmp = BatchReader(reader)
+        # Swap self and tmp
         tmp.reader, self.reader = self.reader, tmp.reader
         tmp.schema, self.schema = self.schema, tmp.schema
         return pyarrow.RecordBatchReader.from_batches(tmp.schema, tmp)
 
     def fetch_concurrently(self):
         """
         Allocate another transit buffer and use it to fetch row set groups (aka. batches) from the
@@ -358,21 +359,22 @@
             for batch in reader:
                 # Process arrow batches
                 df = batch.to_pandas()
                 # ...
         """
         try:
             self.reader.into_concurrent()
-        except:
+        except Exception:
             # Making a reader concurrent will not change its schema, yet if there is an error the
             # reader is destroyed and its schema is empty.
             # self.schema == self.reader.schema()
             # should always be true and so asigning it never would make the code incorrect. Yet we
             # only need to do so if it actually changes.
             self.schema = self.reader.schema()
+            raise
 
 
 def read_arrow_batches_from_odbc(
     query: str,
     connection_string: str,
     batch_size: int = 65535,
     user: Optional[str] = None,
```

### Comparing `arrow_odbc-6.0.0/python/arrow_odbc/writer.py` & `arrow_odbc-7.0.0/python/arrow_odbc/writer.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/src/error.rs` & `arrow_odbc-7.0.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/src/lib.rs` & `arrow_odbc-7.0.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/src/logging.rs` & `arrow_odbc-7.0.0/src/logging.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/src/parameter.rs` & `arrow_odbc-7.0.0/src/parameter.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/src/reader/arrow_odbc_reader.rs` & `arrow_odbc-7.0.0/src/reader/arrow_odbc_reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/src/reader.rs` & `arrow_odbc-7.0.0/src/reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/src/writer.rs` & `arrow_odbc-7.0.0/src/writer.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/temp_db.duckdb` & `arrow_odbc-7.0.0/temp_db.duckdb`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/tests/iris.csv` & `arrow_odbc-7.0.0/tests/iris.csv`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/tests/iris.parquet` & `arrow_odbc-7.0.0/tests/iris.parquet`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/tests/test_arrow_odbc.py` & `arrow_odbc-7.0.0/tests/test_arrow_odbc.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-6.0.0/Cargo.lock` & `arrow_odbc-7.0.0/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android-activity"
-version = "0.5.2"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee91c0c2905bae44f84bfa4e044536541df26b7703fd0888deeb9060fcc44289"
+checksum = "ef6978589202a00cd7e118380c448a08b6ed394c3a8df3a430d0898e3a42d046"
 dependencies = [
  "android-properties",
  "bitflags 2.5.0",
  "cc",
  "cesu8",
  "jni",
  "jni-sys",
@@ -157,17 +157,17 @@
  "arrow-schema",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-odbc"
-version = "9.0.0"
+version = "11.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44c0f42b7fff9cdd6fcc1ba5a955b5e233ef645d5fe4b636b372e9bb4d36214a"
+checksum = "9436a94fd8cf677d725199d3ab40b5dec080377cd2a76ff72a3ffc28eee06135"
 dependencies = [
  "arrow",
  "chrono",
  "log",
  "odbc-api",
  "thiserror",
 ]
@@ -265,52 +265,42 @@
 name = "atomic-waker"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1505bd5d3d116872e7271a6d4e16d81d0c8570876c8de68093a09ac269d8aac0"
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "base64"
-version = "0.22.0"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
-name = "block-sys"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae85a0696e7ea3b835a453750bf002770776609115e6d25c6d2ff28a8200f7e7"
-dependencies = [
- "objc-sys",
-]
-
-[[package]]
 name = "block2"
-version = "0.3.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15b55663a85f33501257357e6421bb33e769d5c9ffb5ba0921c975a123e35e68"
+checksum = "2c132eebf10f5cad5289222520a4a058514204aed6d791f1cf4fe8088b82d15f"
 dependencies = [
- "block-sys",
  "objc2",
 ]
 
 [[package]]
 name = "bumpalo"
 version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -334,20 +324,21 @@
  "rustix",
  "slab",
  "thiserror",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.94"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cesu8"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d43a04d8753f35258c91f8ec639f792891f748a1edbd759cf1dcea3382ad83c"
@@ -356,17 +347,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cfg_aliases"
-version = "0.1.1"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
+checksum = "613afe47fcd5fac7ccf1db93babcb082c5994d996f20b8b159f2ad1658eb5724"
 
 [[package]]
 name = "chrono"
 version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
@@ -386,17 +377,17 @@
 dependencies = [
  "bytes",
  "memchr",
 ]
 
 [[package]]
 name = "concurrent-queue"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d16048cd947b08fa32c24458a22f5dc5e835264f689f4f5653210c69fd107363"
+checksum = "4ca0197aee26d1ae37445ee532fefce43251d24cc7c166799f4d46817f1d3973"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "const-random"
 version = "0.1.18"
@@ -455,17 +446,17 @@
  "bitflags 1.3.2",
  "core-foundation",
  "libc",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
@@ -487,24 +478,30 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "330c60081dcc4c72131f8eb70510f1ac07223e5d4163db481a04a0befcffa412"
 dependencies = [
  "libloading",
 ]
 
 [[package]]
+name = "dpi"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f25c0e292a7ca6d6498557ff1df68f32c99850012b6ea401cf8daf771f22ff53"
+
+[[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "foreign-types"
@@ -531,17 +528,17 @@
 name = "foreign-types-shared"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa9a19cbb55df58761df49b23516a86d432839add4af60fc256da840f66ed35b"
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -553,17 +550,17 @@
  "cfg-if",
  "crunchy",
  "num-traits",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "hermit-abi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
@@ -587,25 +584,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
-name = "icrate"
-version = "0.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99d3aaff8a54577104bafdf686ff18565c3b6903ca5782a2026ef06e2c7aa319"
-dependencies = [
- "block2",
- "dispatch",
- "objc2",
-]
-
-[[package]]
 name = "indexmap"
 version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
@@ -642,17 +628,17 @@
 name = "jni-sys"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8eaf4bc02d17cbdd7ff4c7438cafcdf7fb9a4613313ad11b4f8fefe7d3fa0130"
 
 [[package]]
 name = "jobserver"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "685a7d121ee3f65ae4fddd72b25a04bb36b6af81bc0828f7d5434c0fe60fa3a2"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -724,17 +710,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
@@ -752,22 +738,22 @@
 name = "libredox"
 version = "0.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3af92c55d7d839293953fcd0fda5ecfe93297cfde6ffbdec13b41d99c0ba6607"
 dependencies = [
  "bitflags 2.5.0",
  "libc",
- "redox_syscall 0.4.1",
+ "redox_syscall",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.13"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
+checksum = "78b3ae25bc7c8c38cec158d1f2757ee79e9b3740fbc7ccf0e59e4b08d793fa89"
 
 [[package]]
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
@@ -775,17 +761,17 @@
 name = "memchr"
 version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "ndk"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2076a31b7010b17a38c01907c45b945e8f11495ee4dd588309718901b1f7a5b7"
+checksum = "c3f42e7bbe13d351b6bead8286a43aac9534b82bd3cc43e47037f012ebfd62d4"
 dependencies = [
  "bitflags 2.5.0",
  "jni-sys",
  "log",
  "ndk-sys",
  "num_enum",
  "raw-window-handle",
@@ -796,51 +782,50 @@
 name = "ndk-context"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "27b02d87554356db9e9a873add8782d4ea6e3e58ea071a9adb9a2e8ddb884a8b"
 
 [[package]]
 name = "ndk-sys"
-version = "0.5.0+25.2.9519653"
+version = "0.6.0+11769913"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c196769dd60fd4f363e11d948139556a344e79d451aeb2fa2fd040738ef7691"
+checksum = "ee6cda3051665f1fb8d9e08fc35c96d5a244fb1be711a03b71118828afc9a873"
 dependencies = [
  "jni-sys",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.2"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3135b08af27d103b0a51f2ae0f8632117b7b185ccf931445affa8df530576a41"
+checksum = "35bd024e8b2ff75562e5f34e7f4905839deb4b22955ef5e73d2fea1b9813cb23"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
 ]
 
 [[package]]
 name = "num-bigint"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
+checksum = "c165a9ab64cf766f73521c0dd2cfdff64f488b8f0b3e621face3462d3db536d7"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.46"
@@ -848,40 +833,39 @@
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-iter"
-version = "0.1.44"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d869c01cc0c455284163fd0092f1f93835385ccab5a98a0dcc497b2f8bf055a9"
+checksum = "1429034a0490724d0075ebb2bc9e875d6503c3cf69e235a8941aa757d83ef5bf"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-rational"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+checksum = "f83d14da390562dca69fc84082e73e548e1ad308d24accdedd2720017cb37824"
 dependencies = [
- "autocfg",
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_enum"
@@ -902,39 +886,117 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "objc-sys"
-version = "0.3.3"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da284c198fb9b7b0603f8635185e85fbd5b64ee154b1ed406d489077de2d6d60"
+checksum = "cdb91bdd390c7ce1a8607f35f3ca7151b65afc0ff5ff3b34fa350f7d7c7e4310"
 
 [[package]]
 name = "objc2"
-version = "0.4.1"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "559c5a40fdd30eb5e344fbceacf7595a81e242529fb4e21cf5f43fb4f11ff98d"
+checksum = "46a785d4eeff09c14c487497c162e92766fbb3e4059a71840cecc03d9a50b804"
 dependencies = [
  "objc-sys",
  "objc2-encode",
 ]
 
 [[package]]
+name = "objc2-app-kit"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e4e89ad9e3d7d297152b17d39ed92cd50ca8063a89a9fa569046d41568891eff"
+dependencies = [
+ "bitflags 2.5.0",
+ "block2",
+ "libc",
+ "objc2",
+ "objc2-core-data",
+ "objc2-core-image",
+ "objc2-foundation",
+ "objc2-quartz-core",
+]
+
+[[package]]
+name = "objc2-core-data"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "617fbf49e071c178c0b24c080767db52958f716d9eabdf0890523aeae54773ef"
+dependencies = [
+ "bitflags 2.5.0",
+ "block2",
+ "objc2",
+ "objc2-foundation",
+]
+
+[[package]]
+name = "objc2-core-image"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "55260963a527c99f1819c4f8e3b47fe04f9650694ef348ffd2227e8196d34c80"
+dependencies = [
+ "block2",
+ "objc2",
+ "objc2-foundation",
+ "objc2-metal",
+]
+
+[[package]]
 name = "objc2-encode"
-version = "3.0.0"
+version = "4.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d079845b37af429bfe5dfa76e6d087d788031045b25cfc6fd898486fd9847666"
+checksum = "7891e71393cd1f227313c9379a26a584ff3d7e6e7159e988851f0934c993f0f8"
+
+[[package]]
+name = "objc2-foundation"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ee638a5da3799329310ad4cfa62fbf045d5f56e3ef5ba4149e7452dcf89d5a8"
+dependencies = [
+ "bitflags 2.5.0",
+ "block2",
+ "dispatch",
+ "libc",
+ "objc2",
+]
+
+[[package]]
+name = "objc2-metal"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dd0cba1276f6023976a406a14ffa85e1fdd19df6b0f737b063b95f6c8c7aadd6"
+dependencies = [
+ "bitflags 2.5.0",
+ "block2",
+ "objc2",
+ "objc2-foundation",
+]
+
+[[package]]
+name = "objc2-quartz-core"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e42bee7bff906b14b167da2bac5efe6b6a07e6f7c0a21a7308d40c960242dc7a"
+dependencies = [
+ "bitflags 2.5.0",
+ "block2",
+ "objc2",
+ "objc2-foundation",
+ "objc2-metal",
+]
 
 [[package]]
 name = "odbc-api"
-version = "7.0.0"
+version = "7.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e53cd49196dfbaeea079afac5305cd38bf16c7d3e595764dc045f386cbde8d6"
+checksum = "5f11608c88bac7ee4594473d68e47997641b7493d34432cc1b3d21e15efb491f"
 dependencies = [
  "atoi",
  "log",
  "odbc-sys",
  "thiserror",
  "widestring",
  "winit",
@@ -958,24 +1020,44 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "52f0d54bde9774d3a51dcf281a5def240c71996bc6ca05d2c847ec8b2b216166"
 dependencies = [
  "libredox",
 ]
 
 [[package]]
+name = "pin-project"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
+dependencies = [
+ "pin-project-internal",
+]
+
+[[package]]
+name = "pin-project-internal"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "polling"
-version = "3.6.0"
+version = "3.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0c976a60b2d7e99d6f229e414670a9b85d13ac305cc6d1e9c134de58c5aaaf6"
+checksum = "645493cf344456ef24219d02a768cf1fb92ddf8c92161679ae3d91b91a637be3"
 dependencies = [
  "cfg-if",
  "concurrent-queue",
  "hermit-abi",
  "pin-project-lite",
  "rustix",
  "tracing",
@@ -989,17 +1071,17 @@
 checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
 dependencies = [
  "toml_edit",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
@@ -1007,26 +1089,17 @@
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "raw-window-handle"
-version = "0.6.0"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42a9830a0e1b9fb145ebb365b8bc4ccd75f290f98c0247deafbbe2c75cefb544"
-
-[[package]]
-name = "redox_syscall"
-version = "0.3.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
-dependencies = [
- "bitflags 1.3.2",
-]
+checksum = "20675572f6f24e9e76ef639bc5552774ed45f1c30e2951e1e99c59888861c539"
 
 [[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
@@ -1060,54 +1133,54 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.198"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
+checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.198"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
+checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1117,17 +1190,17 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smol_str"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6845563ada680337a52d43bb0b29f396f2d911616f6573012645b9e3d048a49"
+checksum = "dd538fb6910ac1099850255cf94a94df6551fbdd602454387d0adb2d1ca6dead"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
@@ -1145,17 +1218,17 @@
  "log",
  "termcolor",
  "thread_local",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.60"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1165,26 +1238,26 @@
 checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1204,17 +1277,17 @@
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
 dependencies = [
  "crunchy",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.5"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
+checksum = "4badfd56924ae69bcc9039335b2e017639ce3f9b001c393c1b2d1ef846ce2cbf"
 
 [[package]]
 name = "toml_edit"
 version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a8534fd7f78b5405e860340ad6575217ce99f38d4d5c8f2442cb5ecb50090e1"
 dependencies = [
@@ -1347,60 +1420,38 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "web-time"
-version = "0.2.4"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa30049b1c872b72c89866d458eae9f20380ab280ffd1b1e18df2d3e2d98cfe0"
+checksum = "5a6580f308b1fad9207618087a65c04e7a10bc77e02c8e84e9b00dd4b12fa0bb"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "widestring"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7219d36b6eac893fa81e84ebe06485e7dcbb616177469b142df14f1f4deb1311"
 
 [[package]]
-name = "winapi"
-version = "0.3.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
-dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
-]
-
-[[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
-
-[[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
-
-[[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
  "windows-targets 0.52.5",
 ]
@@ -1412,23 +1463,14 @@
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.48.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
-dependencies = [
- "windows-targets 0.48.5",
-]
-
-[[package]]
-name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
  "windows-targets 0.52.5",
 ]
 
@@ -1445,29 +1487,14 @@
  "windows_x86_64_gnu 0.42.2",
  "windows_x86_64_gnullvm 0.42.2",
  "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
-dependencies = [
- "windows_aarch64_gnullvm 0.48.5",
- "windows_aarch64_msvc 0.48.5",
- "windows_i686_gnu 0.48.5",
- "windows_i686_msvc 0.48.5",
- "windows_x86_64_gnu 0.48.5",
- "windows_x86_64_gnullvm 0.48.5",
- "windows_x86_64_msvc 0.48.5",
-]
-
-[[package]]
-name = "windows-targets"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm 0.52.5",
  "windows_aarch64_msvc 0.52.5",
  "windows_i686_gnu 0.52.5",
@@ -1482,56 +1509,38 @@
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
 
 [[package]]
 name = "windows_i686_gnullvm"
 version = "0.52.5"
@@ -1542,111 +1551,89 @@
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winit"
-version = "0.29.15"
+version = "0.30.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d59ad965a635657faf09c8f062badd885748428933dad8e8bdd64064d92e5ca"
+checksum = "ea9e6d5d66cbf702e0dd820302144f51b69a95acdc495dd98ca280ff206562b1"
 dependencies = [
  "android-activity",
  "atomic-waker",
  "bitflags 2.5.0",
  "calloop",
  "cfg_aliases",
+ "concurrent-queue",
  "core-foundation",
  "core-graphics",
  "cursor-icon",
- "icrate",
+ "dpi",
  "js-sys",
  "libc",
- "log",
  "ndk",
- "ndk-sys",
  "objc2",
- "once_cell",
+ "objc2-app-kit",
+ "objc2-foundation",
  "orbclient",
+ "pin-project",
  "raw-window-handle",
- "redox_syscall 0.3.5",
+ "redox_syscall",
  "rustix",
  "smol_str",
+ "tracing",
  "unicode-segmentation",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "web-time",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
  "xkbcommon-dl",
 ]
 
 [[package]]
 name = "winnow"
 version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1672,24 +1659,24 @@
 name = "xkeysym"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "054a8e68b76250b253f671d1268cb7f1ae089ec35e195b2efb2a4e9a836d0621"
 
 [[package]]
 name = "zerocopy"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
```

### Comparing `arrow_odbc-6.0.0/pyproject.toml` & `arrow_odbc-7.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "maturin"
 
 [project]
 name = "arrow-odbc"
 authors = [{name = "Markus Klein"}]
 description="Read the data of an ODBC data source as sequence of Apache Arrow record batches."
 readme = "README.md"
-version = "6.0.0"
+version = "7.0.0"
 dependencies = ["cffi", "pyarrow >= 8.0.0"]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = ["pytest < 8.0.0", "pyodbc", "duckdb"]
```

### Comparing `arrow_odbc-6.0.0/PKG-INFO` & `arrow_odbc-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arrow-odbc
-Version: 6.0.0
+Version: 7.0.0
 Requires-Dist: cffi
 Requires-Dist: pyarrow >=8.0.0
 Requires-Dist: pytest <8.0.0 ; extra == 'test'
 Requires-Dist: pyodbc ; extra == 'test'
 Requires-Dist: duckdb ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
@@ -155,15 +155,16 @@
 | Date                     | Date32               |
 | LongVarbinary            | Binary               |
 | Timestamp(p = 0)         | TimestampSecond      |
 | Timestamp(p: 1..3)       | TimestampMilliSecond |
 | Timestamp(p: 4..6)       | TimestampMicroSecond |
 | Timestamp(p >= 7 )       | TimestampNanoSecond  |
 | BigInt                   | Int64                |
-| TinyInt                  | Int8                 |
+| TinyInt Signed           | Int8                 |
+| TinyInt Unsigned         | UInt8                |
 | Bit                      | Boolean              |
 | Varbinary                | Binary               |
 | Binary                   | FixedSizedBinary     |
 | All others               | Utf8                 |
 
 ## Matching of Arrow to ODBC types then inserting
```

