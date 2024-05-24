# Comparing `tmp/arrow_odbc-7.0.0.tar.gz` & `tmp/arrow_odbc-7.0.1.tar.gz`

## Comparing `arrow_odbc-7.0.0.tar` & `arrow_odbc-7.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 arrow_odbc-7.0.0/Cargo.toml
--rw-r--r--   0      501       20      136 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/.gitattributes
--rw-r--r--   0      501       20      213 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/.github/dependabot.yml
--rw-r--r--   0      501       20     1762 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/.github/workflows/test.yml
--rw-r--r--   0      501       20     2648 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/.github/workflows/wheel.yml
--rw-r--r--   0      501       20      286 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/.gitignore
--rw-r--r--   0      501       20      841 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/.readthedocs.yaml
--rw-r--r--   0      501       20    12072 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/Changelog.md
--rw-r--r--   0      501       20     1954 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/Contributing.md
--rw-r--r--   0      501       20     1069 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/LICENSE
--rw-r--r--   0      501       20     8040 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/README.md
--rw-r--r--   0      501       20       14 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/cbindgen.toml
--rw-r--r--   0      501       20      623 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/conftest.py
--rw-r--r--   0      501       20      638 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/Makefile
--rw-r--r--   0      501       20      804 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/make.bat
--rw-r--r--   0      501       20       16 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/requirements.txt
--rw-r--r--   0      501       20      155 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/source/arrow_odbc.rst
--rw-r--r--   0      501       20     1965 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/source/conf.py
--rw-r--r--   0      501       20      458 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/source/index.rst
--rw-r--r--   0      501       20       67 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/doc/source/modules.rst
--rw-r--r--   0      501       20      348 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/docker-compose.yml
--rw-r--r--   0      501       20      564 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/manylinux/Dockerfile
--rw-r--r--   0      501       20      121 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/manylinux/Readme.md
--rw-r--r--   0      501       20      148 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/manylinux/WHEEL
--rw-r--r--   0      501       20     1256 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/manylinux/build_wheel.sh
--rw-r--r--   0      501       20      446 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/__init__.py
--rw-r--r--   0      501       20     1885 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/connect.py
--rw-r--r--   0      501       20      672 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/error.py
--rw-r--r--   0      501       20      788 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/log.py
--rw-r--r--   0      501       20      578 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/pool.py
--rw-r--r--   0      501       20    25240 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/reader.py
--rw-r--r--   0      501       20     9625 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/python/arrow_odbc/writer.py
--rw-r--r--   0      501       20     2322 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/error.rs
--rw-r--r--   0      501       20     3434 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/lib.rs
--rw-r--r--   0      501       20      655 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/logging.rs
--rw-r--r--   0      501       20     1239 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/parameter.rs
--rw-r--r--   0      501       20      421 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/pool.rs
--rw-r--r--   0      501       20     8757 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/reader/arrow_odbc_reader.rs
--rw-r--r--   0      501       20    12865 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/reader.rs
--rw-r--r--   0      501       20     3545 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/src/writer.rs
--rw-r--r--   0      501       20   274432 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/temp_db.duckdb
--rw-r--r--   0      501       20        0 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/tests/__init__.py
--rw-r--r--   0      501       20     4115 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/tests/iris.csv
--rw-r--r--   0      501       20     2413 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/tests/iris.parquet
--rw-r--r--   0      501       20    29032 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/tests/test_arrow_odbc.py
--rw-r--r--   0      501       20    42700 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/Cargo.lock
--rw-r--r--   0      501       20      825 2024-05-24 19:02:15.000000 arrow_odbc-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     8652 1970-01-01 00:00:00.000000 arrow_odbc-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 arrow_odbc-7.0.1/Cargo.toml
+-rw-r--r--   0      501       20      136 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/.gitattributes
+-rw-r--r--   0      501       20      213 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/.github/dependabot.yml
+-rw-r--r--   0      501       20     1762 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/.github/workflows/test.yml
+-rw-r--r--   0      501       20     2654 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/.github/workflows/wheel.yml
+-rw-r--r--   0      501       20      286 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/.gitignore
+-rw-r--r--   0      501       20      841 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/.readthedocs.yaml
+-rw-r--r--   0      501       20    12114 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/Changelog.md
+-rw-r--r--   0      501       20     1954 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/Contributing.md
+-rw-r--r--   0      501       20     1069 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/LICENSE
+-rw-r--r--   0      501       20     8040 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/README.md
+-rw-r--r--   0      501       20       14 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/cbindgen.toml
+-rw-r--r--   0      501       20      623 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/conftest.py
+-rw-r--r--   0      501       20      638 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/Makefile
+-rw-r--r--   0      501       20      804 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/make.bat
+-rw-r--r--   0      501       20       16 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/requirements.txt
+-rw-r--r--   0      501       20      155 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/source/arrow_odbc.rst
+-rw-r--r--   0      501       20     1965 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/source/conf.py
+-rw-r--r--   0      501       20      458 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/source/index.rst
+-rw-r--r--   0      501       20       67 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/doc/source/modules.rst
+-rw-r--r--   0      501       20      348 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/docker-compose.yml
+-rw-r--r--   0      501       20      564 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/manylinux/Dockerfile
+-rw-r--r--   0      501       20      121 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/manylinux/Readme.md
+-rw-r--r--   0      501       20      148 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/manylinux/WHEEL
+-rw-r--r--   0      501       20     1256 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/manylinux/build_wheel.sh
+-rw-r--r--   0      501       20      446 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/__init__.py
+-rw-r--r--   0      501       20     1885 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/connect.py
+-rw-r--r--   0      501       20      672 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/error.py
+-rw-r--r--   0      501       20      788 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/log.py
+-rw-r--r--   0      501       20      578 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/pool.py
+-rw-r--r--   0      501       20    25240 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/reader.py
+-rw-r--r--   0      501       20     9625 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/python/arrow_odbc/writer.py
+-rw-r--r--   0      501       20     2322 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/error.rs
+-rw-r--r--   0      501       20     3434 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/lib.rs
+-rw-r--r--   0      501       20      655 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/logging.rs
+-rw-r--r--   0      501       20     1239 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/parameter.rs
+-rw-r--r--   0      501       20      421 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/pool.rs
+-rw-r--r--   0      501       20     8757 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/reader/arrow_odbc_reader.rs
+-rw-r--r--   0      501       20    12865 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/reader.rs
+-rw-r--r--   0      501       20     3545 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/src/writer.rs
+-rw-r--r--   0      501       20   274432 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/temp_db.duckdb
+-rw-r--r--   0      501       20        0 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/tests/__init__.py
+-rw-r--r--   0      501       20     4115 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/tests/iris.csv
+-rw-r--r--   0      501       20     2413 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/tests/iris.parquet
+-rw-r--r--   0      501       20    29032 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/tests/test_arrow_odbc.py
+-rw-r--r--   0      501       20    42700 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/Cargo.lock
+-rw-r--r--   0      501       20      825 2024-05-24 19:13:27.000000 arrow_odbc-7.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8652 1970-01-01 00:00:00.000000 arrow_odbc-7.0.1/PKG-INFO
```

### Comparing `arrow_odbc-7.0.0/Cargo.toml` & `arrow_odbc-7.0.1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/.github/workflows/test.yml` & `arrow_odbc-7.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/.github/workflows/wheel.yml` & `arrow_odbc-7.0.1/.github/workflows/wheel.yml`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
       run: |
         python -m pip install --upgrade pip
         python -m pip install build
         python -m build
         pip install twine
         twine upload --skip-existing -u __token__ -p "${{ secrets.PYPI_API_TOKEN }}" dist/*
 
-  os-x-wheel:
+  osx_13_x86:
 
-    runs-on: macos-latest
+    runs-on: macos_x86_wheel
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: '3.x'
@@ -61,15 +61,15 @@
       run: |
         docker build -t cargodock ./manylinux
         docker run --rm -v ${PWD}:/io cargodock bash /io/manylinux/build_wheel.sh
         pip install twine
         twine upload --skip-existing -u __token__ -p "${{ secrets.PYPI_API_TOKEN }}" dist/*
 
 
-  macos-wheel:
+  macos-wheel-m1:
 
     runs-on: flyci-macos-14-m1
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
```

### Comparing `arrow_odbc-7.0.0/.readthedocs.yaml` & `arrow_odbc-7.0.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/Changelog.md` & `arrow_odbc-7.0.1/Changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 7.0.1
+
+- Build wheel for MacOS 13 x86
+
 ## 7.0.0
 
 - unsigned TinyInt is now mapped to `UInt8`.
 
 ## 6.0.0
 
 - Support for passing desired packet size to the ODBC driver. This may help with packet loss on fragile connections if the ODBC driver supports it.
```

### Comparing `arrow_odbc-7.0.0/Contributing.md` & `arrow_odbc-7.0.1/Contributing.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/LICENSE` & `arrow_odbc-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/README.md` & `arrow_odbc-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/conftest.py` & `arrow_odbc-7.0.1/conftest.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/doc/Makefile` & `arrow_odbc-7.0.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/doc/make.bat` & `arrow_odbc-7.0.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/doc/source/conf.py` & `arrow_odbc-7.0.1/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "arrow-odbc"
 copyright = "2021, Markus Klein"
 author = "Markus Klein"
 
 # The full version, including alpha/beta/rc tags
-release = "7.0.0"
+release = "7.0.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `arrow_odbc-7.0.0/manylinux/Dockerfile` & `arrow_odbc-7.0.1/manylinux/Dockerfile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/manylinux/build_wheel.sh` & `arrow_odbc-7.0.1/manylinux/build_wheel.sh`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/python/arrow_odbc/connect.py` & `arrow_odbc-7.0.1/python/arrow_odbc/connect.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/python/arrow_odbc/error.py` & `arrow_odbc-7.0.1/python/arrow_odbc/error.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/python/arrow_odbc/log.py` & `arrow_odbc-7.0.1/python/arrow_odbc/log.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/python/arrow_odbc/pool.py` & `arrow_odbc-7.0.1/python/arrow_odbc/pool.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/python/arrow_odbc/reader.py` & `arrow_odbc-7.0.1/python/arrow_odbc/reader.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/python/arrow_odbc/writer.py` & `arrow_odbc-7.0.1/python/arrow_odbc/writer.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/src/error.rs` & `arrow_odbc-7.0.1/src/error.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/src/lib.rs` & `arrow_odbc-7.0.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/src/logging.rs` & `arrow_odbc-7.0.1/src/logging.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/src/parameter.rs` & `arrow_odbc-7.0.1/src/parameter.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/src/reader/arrow_odbc_reader.rs` & `arrow_odbc-7.0.1/src/reader/arrow_odbc_reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/src/reader.rs` & `arrow_odbc-7.0.1/src/reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/src/writer.rs` & `arrow_odbc-7.0.1/src/writer.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/temp_db.duckdb` & `arrow_odbc-7.0.1/temp_db.duckdb`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/tests/iris.csv` & `arrow_odbc-7.0.1/tests/iris.csv`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/tests/iris.parquet` & `arrow_odbc-7.0.1/tests/iris.parquet`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/tests/test_arrow_odbc.py` & `arrow_odbc-7.0.1/tests/test_arrow_odbc.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/Cargo.lock` & `arrow_odbc-7.0.1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `arrow_odbc-7.0.0/pyproject.toml` & `arrow_odbc-7.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "maturin"
 
 [project]
 name = "arrow-odbc"
 authors = [{name = "Markus Klein"}]
 description="Read the data of an ODBC data source as sequence of Apache Arrow record batches."
 readme = "README.md"
-version = "7.0.0"
+version = "7.0.1"
 dependencies = ["cffi", "pyarrow >= 8.0.0"]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = ["pytest < 8.0.0", "pyodbc", "duckdb"]
```

### Comparing `arrow_odbc-7.0.0/PKG-INFO` & `arrow_odbc-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arrow-odbc
-Version: 7.0.0
+Version: 7.0.1
 Requires-Dist: cffi
 Requires-Dist: pyarrow >=8.0.0
 Requires-Dist: pytest <8.0.0 ; extra == 'test'
 Requires-Dist: pyodbc ; extra == 'test'
 Requires-Dist: duckdb ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
```

