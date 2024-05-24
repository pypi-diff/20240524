# Comparing `tmp/sqlfluff_common_conventions-0.3.0.tar.gz` & `tmp/sqlfluff_common_conventions-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlfluff_common_conventions-0.3.0.tar", last modified: Wed May  8 08:33:31 2024, max compression
+gzip compressed data, was "sqlfluff_common_conventions-0.3.1.tar", last modified: Fri May 24 09:24:41 2024, max compression
```

## Comparing `sqlfluff_common_conventions-0.3.0.tar` & `sqlfluff_common_conventions-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-05-08 08:33:31.349658 sqlfluff_common_conventions-0.3.0/
--rw-r--r--   0 valerie.tan   (502) staff       (20)     1067 2024-04-08 03:18:16.000000 sqlfluff_common_conventions-0.3.0/LICENSE
--rw-r--r--   0 valerie.tan   (502) staff       (20)       65 2024-04-11 09:37:24.000000 sqlfluff_common_conventions-0.3.0/MANIFEST.in
--rw-r--r--   0 valerie.tan   (502) staff       (20)     3150 2024-05-08 08:33:31.349240 sqlfluff_common_conventions-0.3.0/PKG-INFO
--rw-r--r--   0 valerie.tan   (502) staff       (20)      618 2024-05-08 08:31:04.000000 sqlfluff_common_conventions-0.3.0/README.md
--rw-r--r--   0 valerie.tan   (502) staff       (20)     1539 2024-05-08 08:33:02.000000 sqlfluff_common_conventions-0.3.0/pyproject.toml
--rw-r--r--   0 valerie.tan   (502) staff       (20)       38 2024-05-08 08:33:31.349873 sqlfluff_common_conventions-0.3.0/setup.cfg
-drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-05-08 08:33:31.334250 sqlfluff_common_conventions-0.3.0/src/
-drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-05-08 08:33:31.344847 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/
--rw-r--r--   0 valerie.tan   (502) staff       (20)     4134 2024-05-02 09:19:06.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC01.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)     2699 2024-05-02 09:19:06.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC02.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)     2461 2024-05-02 09:19:06.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC03.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)     6311 2024-05-08 02:20:21.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC04.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)     6476 2024-05-08 02:11:13.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC05.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)     2634 2024-05-08 02:51:17.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC06.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)     2613 2024-05-08 02:34:03.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/__init__.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)      470 2024-05-08 02:23:29.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/plugin_default_config.cfg
-drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-05-08 08:33:31.348740 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/
--rw-r--r--   0 valerie.tan   (502) staff       (20)     3150 2024-05-08 08:33:31.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/PKG-INFO
--rw-r--r--   0 valerie.tan   (502) staff       (20)      718 2024-05-08 08:33:31.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/SOURCES.txt
--rw-r--r--   0 valerie.tan   (502) staff       (20)        1 2024-05-08 08:33:31.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/dependency_links.txt
--rw-r--r--   0 valerie.tan   (502) staff       (20)       69 2024-05-08 08:33:31.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/entry_points.txt
--rw-r--r--   0 valerie.tan   (502) staff       (20)       16 2024-05-08 08:33:31.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/requires.txt
--rw-r--r--   0 valerie.tan   (502) staff       (20)       28 2024-05-08 08:33:31.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/top_level.txt
+drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-05-24 09:24:41.018519 sqlfluff_common_conventions-0.3.1/
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     1067 2024-04-08 03:18:16.000000 sqlfluff_common_conventions-0.3.1/LICENSE
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       65 2024-04-11 09:37:24.000000 sqlfluff_common_conventions-0.3.1/MANIFEST.in
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     3150 2024-05-24 09:24:41.018094 sqlfluff_common_conventions-0.3.1/PKG-INFO
+-rw-r--r--   0 valerie.tan   (502) staff       (20)      618 2024-05-09 07:54:12.000000 sqlfluff_common_conventions-0.3.1/README.md
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     1539 2024-05-24 09:24:29.000000 sqlfluff_common_conventions-0.3.1/pyproject.toml
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       38 2024-05-24 09:24:41.018577 sqlfluff_common_conventions-0.3.1/setup.cfg
+drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-05-24 09:24:41.009004 sqlfluff_common_conventions-0.3.1/src/
+drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-05-24 09:24:41.014270 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     4134 2024-05-09 07:54:12.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/CC01.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     2699 2024-05-09 07:54:12.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/CC02.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     2461 2024-05-09 07:54:12.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/CC03.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     6447 2024-05-24 09:23:16.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/CC04.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     6476 2024-05-09 07:54:12.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/CC05.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     2634 2024-05-09 08:46:27.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/CC06.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     2613 2024-05-09 07:54:12.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/__init__.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)      470 2024-05-09 07:54:12.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/plugin_default_config.cfg
+drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-05-24 09:24:41.017592 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions.egg-info/
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     3150 2024-05-24 09:24:41.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions.egg-info/PKG-INFO
+-rw-r--r--   0 valerie.tan   (502) staff       (20)      718 2024-05-24 09:24:41.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions.egg-info/SOURCES.txt
+-rw-r--r--   0 valerie.tan   (502) staff       (20)        1 2024-05-24 09:24:41.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions.egg-info/dependency_links.txt
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       69 2024-05-24 09:24:41.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions.egg-info/entry_points.txt
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       16 2024-05-24 09:24:41.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions.egg-info/requires.txt
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       28 2024-05-24 09:24:41.000000 sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions.egg-info/top_level.txt
```

### Comparing `sqlfluff_common_conventions-0.3.0/LICENSE` & `sqlfluff_common_conventions-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlfluff_common_conventions-0.3.0/PKG-INFO` & `sqlfluff_common_conventions-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff_common_conventions
-Version: 0.3.0
+Version: 0.3.1
 Summary: A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL and Databricks SQL.
 Author-email: Valerie Tan <valerietanhx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Valerie Tan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sqlfluff_common_conventions-0.3.0/README.md` & `sqlfluff_common_conventions-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlfluff_common_conventions-0.3.0/pyproject.toml` & `sqlfluff_common_conventions-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqlfluff_common_conventions"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Valerie Tan", email="valerietanhx@gmail.com" },
 ]
 description = "A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL and Databricks SQL."
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["sqlfluff", "sql", "linter", "formatter", "bigquery", "databricks"]
```

### Comparing `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC01.py` & `sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/CC01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC02.py` & `sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/CC02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC03.py` & `sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/CC03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC04.py` & `sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/CC04.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,18 +93,21 @@
         )
 
         is_table = context.parent_stack[-1].is_type("table_reference") or (
             context.parent_stack[-2].is_type("from_expression_element")
             and context.parent_stack[-1].is_type("alias_expression")
         )
 
+        allowed_strings_columns_set.update(allowed_strings_all_set)
+        allowed_strings_tables_set.update(allowed_strings_all_set)
+
         for allowed_strings_set, condition in (
-            (allowed_strings_all_set, identifier),
             (allowed_strings_columns_set, is_column),
             (allowed_strings_tables_set, is_table),
+            (allowed_strings_all_set, identifier),
         ):
             if allowed_strings_set and condition:
                 allowed_strings_set_regex = "|".join(allowed_strings_set)
                 if self.allow_whitespace:
                     allowed_strings_set_regex += "|\\s"
 
                 match = re.findall(
```

### Comparing `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC05.py` & `sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/CC05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC06.py` & `sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/CC06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/__init__.py` & `sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/PKG-INFO` & `sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff_common_conventions
-Version: 0.3.0
+Version: 0.3.1
 Summary: A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL and Databricks SQL.
 Author-email: Valerie Tan <valerietanhx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Valerie Tan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/SOURCES.txt` & `sqlfluff_common_conventions-0.3.1/src/sqlfluff_common_conventions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

