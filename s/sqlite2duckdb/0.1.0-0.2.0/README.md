# Comparing `tmp/sqlite2duckdb-0.1.0-py2.py3-none-any.whl.zip` & `tmp/sqlite2duckdb-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 2940 bytes, number of entries: 6
--rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 sqlite2duckdb/__init__.py
--rw-r--r--  2.0 unx     1657 b- defN 20-Feb-02 00:00 sqlite2duckdb/__main__.py
-?rw-r--r--  2.0 unx      565 b- defN 20-Feb-02 00:00 sqlite2duckdb-0.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 sqlite2duckdb-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1069 b- defN 20-Feb-02 00:00 sqlite2duckdb-0.1.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      488 b- defN 20-Feb-02 00:00 sqlite2duckdb-0.1.0.dist-info/RECORD
-6 files, 3884 bytes uncompressed, 2052 bytes compressed:  47.2%
+Zip file size: 4293 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      144 b- defN 20-Feb-02 00:00 sqlite2duckdb/__init__.py
+-rw-r--r--  2.0 unx      965 b- defN 20-Feb-02 00:00 sqlite2duckdb/__main__.py
+-rw-r--r--  2.0 unx     1230 b- defN 20-Feb-02 00:00 sqlite2duckdb/sqlite_to_duckdb.py
+?rw-r--r--  2.0 unx     1797 b- defN 20-Feb-02 00:00 sqlite2duckdb-0.2.0.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 sqlite2duckdb-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx       66 b- defN 20-Feb-02 00:00 sqlite2duckdb-0.2.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1069 b- defN 20-Feb-02 00:00 sqlite2duckdb-0.2.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      681 b- defN 20-Feb-02 00:00 sqlite2duckdb-0.2.0.dist-info/RECORD
+8 files, 6057 bytes uncompressed, 3095 bytes compressed:  48.9%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
 Filename: sqlite2duckdb/__init__.py
 Comment: 
 
 Filename: sqlite2duckdb/__main__.py
 Comment: 
 
-Filename: sqlite2duckdb-0.1.0.dist-info/METADATA
+Filename: sqlite2duckdb/sqlite_to_duckdb.py
 Comment: 
 
-Filename: sqlite2duckdb-0.1.0.dist-info/WHEEL
+Filename: sqlite2duckdb-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: sqlite2duckdb-0.1.0.dist-info/licenses/LICENSE
+Filename: sqlite2duckdb-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite2duckdb-0.1.0.dist-info/RECORD
+Filename: sqlite2duckdb-0.2.0.dist-info/entry_points.txt
+Comment: 
+
+Filename: sqlite2duckdb-0.2.0.dist-info/licenses/LICENSE
+Comment: 
+
+Filename: sqlite2duckdb-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite2duckdb/__init__.py

```diff
@@ -0,0 +1,9 @@
+00000000: 696d 706f 7274 2069 6d70 6f72 746c 6962  import importlib
+00000010: 2e6d 6574 6164 6174 610a 6672 6f6d 2073  .metadata.from s
+00000020: 716c 6974 6532 6475 636b 6462 2e73 716c  qlite2duckdb.sql
+00000030: 6974 655f 746f 5f64 7563 6b64 6220 696d  ite_to_duckdb im
+00000040: 706f 7274 2073 716c 6974 655f 746f 5f64  port sqlite_to_d
+00000050: 7563 6b64 620a 5f5f 5645 5253 494f 4e5f  uckdb.__VERSION_
+00000060: 5f20 3d20 696d 706f 7274 6c69 622e 6d65  _ = importlib.me
+00000070: 7461 6461 7461 2e76 6572 7369 6f6e 2827  tadata.version('
+00000080: 7371 6c69 7465 3264 7563 6b64 6227 290a  sqlite2duckdb').
```

## sqlite2duckdb/__main__.py

```diff
@@ -1,60 +1,28 @@
 import duckdb 
 import argparse 
 import os
+from sqlite2duckdb import sqlite_to_duckdb, __VERSION__
 
-def sqlite2duckdb(sqlite_db:str, duck_db:str):
-
-    print(f"Create {duck_db} databases")
-
-    # Remove database if exists
-    if os.path.exists(duck_db):
-        raise Exception(f"Database {duck_db} already exists")
-
-    # Create databases 
-    conn = duckdb.connect(duck_db)
-    db_name = conn.sql("SELECT database_name FROM duckdb_databases").fetchone()[0]
-
-    ## Install sqlite
-    conn.sql(f"""
-    INSTALL sqlite;
-    LOAD sqlite;
-    ATTACH '{sqlite_db}' as __other;
-    """)
-
-    ## Get sqlite Names 
-    conn.sql("USE __other")
-    tables = [i[0] for i  in conn.sql("SHOW tables").fetchall()]
-    print(f"{len(tables)} tables found(s)")
-    conn.sql(f"USE {db_name}")
-
-    # Create tables     
-    for table in tables:
-        print(f"Create duckdb table {table}")
-        conn.sql(f"CREATE TABLE {table} AS select * FROM __other.{table}")
-
-    conn.sql(f"DETACH __other")
-    conn.close()
-    print("Done!")
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description='Convert Sqlite database to Duckdb database')
+def main_cli():
+    
+    parser = argparse.ArgumentParser(description='Convert Sqlite database to Duckdb database', usage="sqlite2duckdb <sqlite_path> <duckdb_path>")
 
     parser.add_argument('sqlite_path', type=str, help='sqlite file path')
     parser.add_argument('duckdb_path', type=str, help='duckdb file path')
-
+    parser.add_argument("-v", "--version", action="version", version=f"sqlite2duckdb {__VERSION__}")
 
     # Analyser les arguments
     args = parser.parse_args()
 
     if os.path.exists(args.duckdb_path):
         delete_input = input(f"{args.duckdb_path} already exists. do you want to delete this file ? (yes/no): ").strip().lower()
         if delete_input in ("yes", "y"):
             os.remove(args.duckdb_path)
         else:
             exit(1)
+    sqlite_to_duckdb(args.sqlite_path, args.duckdb_path)
 
-        
 
-        
-    sqlite2duckdb(args.sqlite_path, args.duckdb_path)
+if __name__ == "__main__":
+
+    main_cli()
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `sqlite2duckdb-0.1.0.dist-info/licenses/LICENSE` & `sqlite2duckdb-0.2.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

