# Comparing `tmp/sqladaptor-0.1.1.tar.gz` & `tmp/sqladaptor-0.2.tar.gz`

## Comparing `sqladaptor-0.1.1.tar` & `sqladaptor-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.python-version
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/.gitignore
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/ruff.xml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/sqladaptor.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/workspace.xml
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/example/db.sqlite
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/example/quick_run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/src/sqladaptor/__init__.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/src/sqladaptor/sqlite.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/test/test_sqlite_adaptor.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/.gitignore
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 sqladaptor-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sqladaptor-0.2/.python-version
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 sqladaptor-0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sqladaptor-0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sqladaptor-0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 sqladaptor-0.2/.idea/ruff.xml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 sqladaptor-0.2/.idea/sqladaptor.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sqladaptor-0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    10077 2020-02-02 00:00:00.000000 sqladaptor-0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 sqladaptor-0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sqladaptor-0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 sqladaptor-0.2/example/db.sqlite
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 sqladaptor-0.2/example/quick_run.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 sqladaptor-0.2/src/sqladaptor/__init__.py
+-rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 sqladaptor-0.2/src/sqladaptor/sqlite.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 sqladaptor-0.2/test/test_sqlite_adaptor.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqladaptor-0.2/.gitignore
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 sqladaptor-0.2/README.md
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 sqladaptor-0.2/pyproject.toml
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 sqladaptor-0.2/PKG-INFO
```

### Comparing `sqladaptor-0.1.1/.idea/sqladaptor.iml` & `sqladaptor-0.2/.idea/sqladaptor.iml`

 * *Files identical despite different names*

### Comparing `sqladaptor-0.1.1/.idea/inspectionProfiles/Project_Default.xml` & `sqladaptor-0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `sqladaptor-0.1.1/test/test_sqlite_adaptor.py` & `sqladaptor-0.2/test/test_sqlite_adaptor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,50 @@
+from copy import deepcopy
+
 import pandas
 import pytest
 from path import Path
 from pydash import py_
 
-from sqladaptor.sqlite import SqliteAdaptor
+from sqladaptor.sqlite import SqliteAdaptor, var_name_regex
+
+schema = {
+    "type": "object",
+    "properties": {
+        "row_id": {"type": "integer"},
+        "description": {"type": "string"},
+        "amount": {"type": "number"},
+        "category": {"type": "string"},
+    },
+    "required": ["row_id"],
+}
 
 
 @pytest.fixture(scope="function")
 def test_db():
     db_fname = Path(__file__).parent / "test.sqlite3"
     db_fname.remove_p()
 
     db = SqliteAdaptor(db_fname)
-    db.execute("""
-        CREATE TABLE IF NOT EXISTS test_table (
-            row_id INTEGER PRIMARY KEY, 
-            description text, 
-            amount FLOAT,
-            category text
-        );
-    """)
+    db.create_table("test_table", schema)
     db.commit()
 
     yield db
 
     db.close()
     db_fname.remove_p()
 
 
+def test_get_schema(test_db):
+    this_schema = deepcopy(schema)
+    del this_schema["required"]
+    return_schmea = test_db.get_table_schema("test_table")
+    assert return_schmea == this_schema
+
+
 def test_insert_row(test_db):
     entry = dict(description="haha", amount=2)
     test_db.insert("test_table", entry)
     saved_entries = test_db.get_df("test_table").to_dict(orient="records")
     assert py_.find(saved_entries, entry)
 
 
@@ -71,16 +84,38 @@
     entry = dict(description="haha", amount=2)
     test_db.insert("test_table", entry)
     row = test_db.get_one_row("test_table")
     for val in entry.values():
         assert val in row
 
 
-def test_get_list_of_dict(test_db):
+def test_get_dicts(test_db):
     entries = [
         dict(description="haha", amount=2),
         dict(description="dodo", amount=3),
     ]
     test_db.set_from_df("test_table", pandas.DataFrame(entries))
-    return_entries = test_db.get_dict_list("test_table")
+    return_entries = test_db.get_dicts("test_table")
     for entry in return_entries:
         assert py_.find(return_entries, entry)
+
+
+def test_get_one_dict(test_db):
+    entries = [
+        dict(description="haha", amount=2),
+        dict(description="dodo", amount=3),
+    ]
+    test_db.set_from_df("test_table", pandas.DataFrame(entries))
+    return_entry = test_db.get_one_dict("test_table")
+    is_found = False
+    for entry in entries:
+        if entry.items() < return_entry.items():
+            is_found = True
+    assert is_found
+
+
+def test_var_names():
+    assert var_name_regex.fullmatch("__ha__")
+    assert not var_name_regex.fullmatch("1__ha__")
+    assert not var_name_regex.fullmatch("__ ha__")
+    assert not var_name_regex.fullmatch("var#")
+    assert not var_name_regex.fullmatch("v;ar")
```

### Comparing `sqladaptor-0.1.1/README.md` & `sqladaptor-0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 updating/inserting data to disk is more efficient. 
 
 SqlAdaptor allows an easy transition to such a database.
 This includes methods to search using dicts, and
 to return rows as dicts for web-servers. 
 
 This is possible
-because there is an equivalence between lists of JSON dicts, Pandas DataFrames
-and SQl tables - they are all tabular arrangements of columnar data.
+because there is an equivalence between JSON dict lists, Pandas DataFrames
+and SQL tables - they are all tabular arrangements of columnar data.
 
 ## Installation
 
 ```bash
 pip install sqladaptor
 ```
 
@@ -32,21 +32,24 @@
     {"description": "this", "value": 1},
     {"description": "that", "value": 2}
 ]
 
 db = SqliteAdaptor('db.sqlite')
 db.set_from_df('data1', pandas.DataFrame(entries))
 
-entries = db.get_dict_list('data1')
-# [{'description': 'this', 'value': 1}, {'description': 'that', 'value': 2}]
+entries = db.get_dicts('data1')
+# [
+#   {'description': 'this', 'value': 1}, 
+#   {'description': 'that', 'value': 2}
+# ]
 
-entries = db.get_dict_list('data1', {"description": "this"})
+return_entries = db.get_dicts('data1', {"description": "this"})
 # [{'description': 'this', 'value': 1}]
 
 df = db.get_df("data1", {"value": 2})
 #   description  value
 # 0        that      2
 
 db.update("data1", {"value": 2}, {"description": "altered"})
-entries = db.get_dict_list('data1', {"value": 2})
-[{'description': 'altered', 'value': 2}]
-```
+return_entries2 = db.get_dicts('data1', {"value": 2})
+# [{'description': 'altered', 'value': 2}]
+```
```

### Comparing `sqladaptor-0.1.1/pyproject.toml` & `sqladaptor-0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [project]
 name = "sqladaptor"
-version = "0.1.1"
+version = "0.2"
 description = "Starting adaptor for JSON/Pandas to SQL db"
 authors = [
     { name = "Bosco Ho", email = "apposite@gmail.com" }
 ]
 dependencies = [
     "path>=16.14.0",
     "pydash>=8.0.1",
     "pandas>=2.2.2",
     "pytest>=8.2.1",
     "rich>=13.7.1",
+    "fastjsonschema>=2.19.1",
+    "ruff>=0.4.5",
+    "ruff-lsp>=0.0.53",
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `sqladaptor-0.1.1/PKG-INFO` & `sqladaptor-0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.3
 Name: sqladaptor
-Version: 0.1.1
+Version: 0.2
 Summary: Starting adaptor for JSON/Pandas to SQL db
 Author-email: Bosco Ho <apposite@gmail.com>
 Requires-Python: >=3.8
+Requires-Dist: fastjsonschema>=2.19.1
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: path>=16.14.0
 Requires-Dist: pydash>=8.0.1
 Requires-Dist: pytest>=8.2.1
 Requires-Dist: rich>=13.7.1
+Requires-Dist: ruff-lsp>=0.0.53
+Requires-Dist: ruff>=0.4.5
 Description-Content-Type: text/markdown
 
 # sqladaptor
 
 Transferring data, stored as JSON or Pandas, into an SQL database and back again.
 
 ## Why?
@@ -22,16 +25,16 @@
 updating/inserting data to disk is more efficient. 
 
 SqlAdaptor allows an easy transition to such a database.
 This includes methods to search using dicts, and
 to return rows as dicts for web-servers. 
 
 This is possible
-because there is an equivalence between lists of JSON dicts, Pandas DataFrames
-and SQl tables - they are all tabular arrangements of columnar data.
+because there is an equivalence between JSON dict lists, Pandas DataFrames
+and SQL tables - they are all tabular arrangements of columnar data.
 
 ## Installation
 
 ```bash
 pip install sqladaptor
 ```
 
@@ -45,21 +48,24 @@
     {"description": "this", "value": 1},
     {"description": "that", "value": 2}
 ]
 
 db = SqliteAdaptor('db.sqlite')
 db.set_from_df('data1', pandas.DataFrame(entries))
 
-entries = db.get_dict_list('data1')
-# [{'description': 'this', 'value': 1}, {'description': 'that', 'value': 2}]
+entries = db.get_dicts('data1')
+# [
+#   {'description': 'this', 'value': 1}, 
+#   {'description': 'that', 'value': 2}
+# ]
 
-entries = db.get_dict_list('data1', {"description": "this"})
+return_entries = db.get_dicts('data1', {"description": "this"})
 # [{'description': 'this', 'value': 1}]
 
 df = db.get_df("data1", {"value": 2})
 #   description  value
 # 0        that      2
 
 db.update("data1", {"value": 2}, {"description": "altered"})
-entries = db.get_dict_list('data1', {"value": 2})
-[{'description': 'altered', 'value': 2}]
-```
+return_entries2 = db.get_dicts('data1', {"value": 2})
+# [{'description': 'altered', 'value': 2}]
+```
```

