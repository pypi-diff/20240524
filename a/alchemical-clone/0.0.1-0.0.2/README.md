# Comparing `tmp/alchemical_clone-0.0.1.tar.gz` & `tmp/alchemical_clone-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemical_clone-0.0.1.tar", last modified: Tue May 21 15:03:28 2024, max compression
+gzip compressed data, was "alchemical_clone-0.0.2.tar", last modified: Fri May 24 13:10:02 2024, max compression
```

## Comparing `alchemical_clone-0.0.1.tar` & `alchemical_clone-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 francisco  (1000) francisco  (1000)        0 2024-05-21 15:03:28.931380 alchemical_clone-0.0.1/
--rw-r--r--   0 francisco  (1000) francisco  (1000)     1062 2024-05-21 14:53:12.000000 alchemical_clone-0.0.1/LICENSE
--rw-r--r--   0 francisco  (1000) francisco  (1000)     8388 2024-05-21 15:03:28.931380 alchemical_clone-0.0.1/PKG-INFO
--rw-r--r--   0 francisco  (1000) francisco  (1000)     7683 2024-05-21 14:45:20.000000 alchemical_clone-0.0.1/README.md
-drwxr-xr-x   0 francisco  (1000) francisco  (1000)        0 2024-05-21 15:03:28.921380 alchemical_clone-0.0.1/alchemical_clone/
--rw-r--r--   0 francisco  (1000) francisco  (1000)      447 2024-05-18 13:23:07.000000 alchemical_clone-0.0.1/alchemical_clone/__init__.py
--rw-r--r--   0 francisco  (1000) francisco  (1000)     2904 2024-05-17 15:02:47.000000 alchemical_clone-0.0.1/alchemical_clone/alchemical_column.py
--rw-r--r--   0 francisco  (1000) francisco  (1000)     4372 2024-05-21 13:59:19.000000 alchemical_clone-0.0.1/alchemical_clone/alchemical_constraint.py
--rw-r--r--   0 francisco  (1000) francisco  (1000)     1280 2024-05-17 13:34:37.000000 alchemical_clone-0.0.1/alchemical_clone/alchemical_index.py
--rw-r--r--   0 francisco  (1000) francisco  (1000)     4206 2024-05-21 09:48:52.000000 alchemical_clone-0.0.1/alchemical_clone/alchemical_lab.py
--rw-r--r--   0 francisco  (1000) francisco  (1000)     6532 2024-05-21 14:05:15.000000 alchemical_clone-0.0.1/alchemical_clone/alchemical_table.py
--rw-r--r--   0 francisco  (1000) francisco  (1000)      167 2024-05-21 09:23:51.000000 alchemical_clone-0.0.1/alchemical_clone/generated_code.py
-drwxr-xr-x   0 francisco  (1000) francisco  (1000)        0 2024-05-21 15:03:28.931380 alchemical_clone-0.0.1/alchemical_clone/plugins/
--rw-r--r--   0 francisco  (1000) francisco  (1000)      130 2024-05-21 13:40:29.000000 alchemical_clone-0.0.1/alchemical_clone/plugins/__init__.py
--rw-r--r--   0 francisco  (1000) francisco  (1000)     2052 2024-05-21 11:32:49.000000 alchemical_clone-0.0.1/alchemical_clone/plugins/many_to_many.py
--rw-r--r--   0 francisco  (1000) francisco  (1000)     1836 2024-05-21 13:55:12.000000 alchemical_clone-0.0.1/alchemical_clone/plugins/one_to_many.py
-drwxr-xr-x   0 francisco  (1000) francisco  (1000)        0 2024-05-21 15:03:28.931380 alchemical_clone-0.0.1/alchemical_clone/utils/
--rw-r--r--   0 francisco  (1000) francisco  (1000)      139 2024-05-17 12:59:43.000000 alchemical_clone-0.0.1/alchemical_clone/utils/__init__.py
--rw-r--r--   0 francisco  (1000) francisco  (1000)     1159 2024-05-17 11:53:37.000000 alchemical_clone-0.0.1/alchemical_clone/utils/utils.py
-drwxr-xr-x   0 francisco  (1000) francisco  (1000)        0 2024-05-21 15:03:28.931380 alchemical_clone-0.0.1/alchemical_clone.egg-info/
--rw-r--r--   0 francisco  (1000) francisco  (1000)     8388 2024-05-21 15:03:28.000000 alchemical_clone-0.0.1/alchemical_clone.egg-info/PKG-INFO
--rw-r--r--   0 francisco  (1000) francisco  (1000)      686 2024-05-21 15:03:28.000000 alchemical_clone-0.0.1/alchemical_clone.egg-info/SOURCES.txt
--rw-r--r--   0 francisco  (1000) francisco  (1000)        1 2024-05-21 15:03:28.000000 alchemical_clone-0.0.1/alchemical_clone.egg-info/dependency_links.txt
--rw-r--r--   0 francisco  (1000) francisco  (1000)       19 2024-05-21 15:03:28.000000 alchemical_clone-0.0.1/alchemical_clone.egg-info/requires.txt
--rw-r--r--   0 francisco  (1000) francisco  (1000)       17 2024-05-21 15:03:28.000000 alchemical_clone-0.0.1/alchemical_clone.egg-info/top_level.txt
--rw-r--r--   0 francisco  (1000) francisco  (1000)      739 2024-05-21 15:03:12.000000 alchemical_clone-0.0.1/pyproject.toml
--rw-r--r--   0 francisco  (1000) francisco  (1000)       21 2024-05-21 09:33:40.000000 alchemical_clone-0.0.1/requirements.txt
--rw-r--r--   0 francisco  (1000) francisco  (1000)       38 2024-05-21 15:03:28.931380 alchemical_clone-0.0.1/setup.cfg
+drwxr-xr-x   0 francisco  (1000) francisco  (1000)        0 2024-05-24 13:10:02.965868 alchemical_clone-0.0.2/
+-rw-r--r--   0 francisco  (1000) francisco  (1000)     1062 2024-05-21 14:53:12.000000 alchemical_clone-0.0.2/LICENSE
+-rw-r--r--   0 francisco  (1000) francisco  (1000)     8388 2024-05-24 13:10:02.965868 alchemical_clone-0.0.2/PKG-INFO
+-rw-r--r--   0 francisco  (1000) francisco  (1000)     7683 2024-05-21 14:45:20.000000 alchemical_clone-0.0.2/README.md
+drwxr-xr-x   0 francisco  (1000) francisco  (1000)        0 2024-05-24 13:10:02.955868 alchemical_clone-0.0.2/alchemical_clone/
+-rw-r--r--   0 francisco  (1000) francisco  (1000)      447 2024-05-18 13:23:07.000000 alchemical_clone-0.0.2/alchemical_clone/__init__.py
+-rw-r--r--   0 francisco  (1000) francisco  (1000)     3002 2024-05-24 13:06:30.000000 alchemical_clone-0.0.2/alchemical_clone/alchemical_column.py
+-rw-r--r--   0 francisco  (1000) francisco  (1000)     4372 2024-05-21 13:59:19.000000 alchemical_clone-0.0.2/alchemical_clone/alchemical_constraint.py
+-rw-r--r--   0 francisco  (1000) francisco  (1000)     1280 2024-05-17 13:34:37.000000 alchemical_clone-0.0.2/alchemical_clone/alchemical_index.py
+-rw-r--r--   0 francisco  (1000) francisco  (1000)     4206 2024-05-21 09:48:52.000000 alchemical_clone-0.0.2/alchemical_clone/alchemical_lab.py
+-rw-r--r--   0 francisco  (1000) francisco  (1000)     6794 2024-05-24 13:06:44.000000 alchemical_clone-0.0.2/alchemical_clone/alchemical_table.py
+-rw-r--r--   0 francisco  (1000) francisco  (1000)      167 2024-05-21 09:23:51.000000 alchemical_clone-0.0.2/alchemical_clone/generated_code.py
+drwxr-xr-x   0 francisco  (1000) francisco  (1000)        0 2024-05-24 13:10:02.955868 alchemical_clone-0.0.2/alchemical_clone/plugins/
+-rw-r--r--   0 francisco  (1000) francisco  (1000)      130 2024-05-21 13:40:29.000000 alchemical_clone-0.0.2/alchemical_clone/plugins/__init__.py
+-rw-r--r--   0 francisco  (1000) francisco  (1000)     2124 2024-05-24 13:08:36.000000 alchemical_clone-0.0.2/alchemical_clone/plugins/many_to_many.py
+-rw-r--r--   0 francisco  (1000) francisco  (1000)     1912 2024-05-24 13:07:49.000000 alchemical_clone-0.0.2/alchemical_clone/plugins/one_to_many.py
+drwxr-xr-x   0 francisco  (1000) francisco  (1000)        0 2024-05-24 13:10:02.955868 alchemical_clone-0.0.2/alchemical_clone/utils/
+-rw-r--r--   0 francisco  (1000) francisco  (1000)      139 2024-05-17 12:59:43.000000 alchemical_clone-0.0.2/alchemical_clone/utils/__init__.py
+-rw-r--r--   0 francisco  (1000) francisco  (1000)     1159 2024-05-17 11:53:37.000000 alchemical_clone-0.0.2/alchemical_clone/utils/utils.py
+drwxr-xr-x   0 francisco  (1000) francisco  (1000)        0 2024-05-24 13:10:02.955868 alchemical_clone-0.0.2/alchemical_clone.egg-info/
+-rw-r--r--   0 francisco  (1000) francisco  (1000)     8388 2024-05-24 13:10:02.000000 alchemical_clone-0.0.2/alchemical_clone.egg-info/PKG-INFO
+-rw-r--r--   0 francisco  (1000) francisco  (1000)      686 2024-05-24 13:10:02.000000 alchemical_clone-0.0.2/alchemical_clone.egg-info/SOURCES.txt
+-rw-r--r--   0 francisco  (1000) francisco  (1000)        1 2024-05-24 13:10:02.000000 alchemical_clone-0.0.2/alchemical_clone.egg-info/dependency_links.txt
+-rw-r--r--   0 francisco  (1000) francisco  (1000)       19 2024-05-24 13:10:02.000000 alchemical_clone-0.0.2/alchemical_clone.egg-info/requires.txt
+-rw-r--r--   0 francisco  (1000) francisco  (1000)       17 2024-05-24 13:10:02.000000 alchemical_clone-0.0.2/alchemical_clone.egg-info/top_level.txt
+-rw-r--r--   0 francisco  (1000) francisco  (1000)      739 2024-05-24 13:09:32.000000 alchemical_clone-0.0.2/pyproject.toml
+-rw-r--r--   0 francisco  (1000) francisco  (1000)       21 2024-05-21 09:33:40.000000 alchemical_clone-0.0.2/requirements.txt
+-rw-r--r--   0 francisco  (1000) francisco  (1000)       38 2024-05-24 13:10:02.965868 alchemical_clone-0.0.2/setup.cfg
```

### Comparing `alchemical_clone-0.0.1/LICENSE` & `alchemical_clone-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemical_clone-0.0.1/PKG-INFO` & `alchemical_clone-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemical_clone
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for generating SQLAlchemy ORM code from an existing database
 Author-email: Francisco Rodrigues <francisco.rodrigues@gmail.com>
 Project-URL: Homepage, https://github.com/ArmindoFlores/alchemical-clone
 Project-URL: Issues, https://github.com/ArmindoFlores/alchemical-clone/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `alchemical_clone-0.0.1/README.md` & `alchemical_clone-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alchemical_clone-0.0.1/alchemical_clone/alchemical_column.py` & `alchemical_clone-0.0.2/alchemical_clone/alchemical_column.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.server_default = repr(self._column.server_default.arg.text) if self._column.server_default is not None else None
         self.server_onupdate = repr(self._column.server_onupdate.arg.text) if self._column.server_onupdate is not None else None
 
     def codegen(self, try_set_primary_key: bool = False) -> str:
         """Generate SQLAlchemy ORM code for this column."""
 
         if try_set_primary_key:
-            if self._column.nullable is False:
+            if self.valid_primary_key:
                 self.implicit_primary_key = True
 
         optional_attributes = {
             "primary_key": self.implicit_primary_key if self.implicit_primary_key else None,
             "comment": self.comment,
             "server_default": self.server_default,
             "server_onupdate": self.server_onupdate,
@@ -61,14 +61,18 @@
             if value is not None:
                 code += f", {attr}={value}"
         code += ")"
 
         return code
     
     @property
+    def valid_primary_key(self) -> bool:
+        return self._column.nullable is False
+    
+    @property
     def target_name(self) -> str:
         name = ""
         if self._table.schema is not None:
             name += f"{self._table.schema}."
         name += f"{self._table.name}.{self.name}"
         return name
```

### Comparing `alchemical_clone-0.0.1/alchemical_clone/alchemical_constraint.py` & `alchemical_clone-0.0.2/alchemical_clone/alchemical_constraint.py`

 * *Files identical despite different names*

### Comparing `alchemical_clone-0.0.1/alchemical_clone/alchemical_index.py` & `alchemical_clone-0.0.2/alchemical_clone/alchemical_index.py`

 * *Files identical despite different names*

### Comparing `alchemical_clone-0.0.1/alchemical_clone/alchemical_lab.py` & `alchemical_clone-0.0.2/alchemical_clone/alchemical_lab.py`

 * *Files identical despite different names*

### Comparing `alchemical_clone-0.0.1/alchemical_clone/alchemical_table.py` & `alchemical_clone-0.0.2/alchemical_clone/alchemical_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,14 +79,22 @@
                 orm_imports.add("relationship")
                 break
         return { 
             "sqlalchemy": base_types.union(column_types.union(constraint_types)), 
             "sqlalchemy.orm": orm_imports 
         }
 
+    def will_generate(self) -> bool:
+        """Check if this table will generate any code."""
+        
+        for column in self.columns:
+            if column.implicit_primary_key or column.valid_primary_key:
+                return True
+        return False
+
     def codegen(self) -> typing.Dict[CodeLocation, str]:
         """Generate SQLAlchemy ORM code for this table."""
 
         class_code = ""
         after_class_code = ""
 
         class_code =  f"class {self.class_name}(Base):\n"
```

### Comparing `alchemical_clone-0.0.1/alchemical_clone/plugins/many_to_many.py` & `alchemical_clone-0.0.2/alchemical_clone/plugins/many_to_many.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,17 @@
         foreign_key_constraints = tuple(filter(lambda c: c.type == "ForeignKeyConstraint", table.constraints))
         if len(foreign_key_constraints) == 2:
             referred_table1, referred_table2 = foreign_key_constraints[0].referred_table, foreign_key_constraints[1].referred_table
 
             if referred_table1 == table or referred_table2 == table:
                 continue
 
+            if not table.will_generate():
+                    continue
+
             plugin_imports = [
                 PluginImport("sqlalchemy.orm", {"relationship"}),
                 PluginImport(f".{table.name}", {table.class_name})
             ]
 
             t1_mtm_name = f"{referred_table2.name}_through_{table.name}"
             t2_mtm_name = f"{referred_table1.name}_through_{table.name}"
```

### Comparing `alchemical_clone-0.0.1/alchemical_clone/plugins/one_to_many.py` & `alchemical_clone-0.0.2/alchemical_clone/plugins/one_to_many.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 
         for constraint in valid_constraints:
             if len(constraint.referenced_columns) == 1 and len(constraint.columns) == 1:
                 referred_table = constraint.referred_table
                 if referred_table == table:
                     continue
 
+                if not table.will_generate():
+                    continue
+
                 plugin_imports = [
                     PluginImport("sqlalchemy.orm", {"relationship"}),
                     PluginImport(f".{table.name}", {table.class_name})
                 ]
 
                 relationship_name = f"{referred_table.name}_to_{table.name}"
```

### Comparing `alchemical_clone-0.0.1/alchemical_clone/utils/utils.py` & `alchemical_clone-0.0.2/alchemical_clone/utils/utils.py`

 * *Files identical despite different names*

### Comparing `alchemical_clone-0.0.1/alchemical_clone.egg-info/PKG-INFO` & `alchemical_clone-0.0.2/alchemical_clone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemical_clone
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for generating SQLAlchemy ORM code from an existing database
 Author-email: Francisco Rodrigues <francisco.rodrigues@gmail.com>
 Project-URL: Homepage, https://github.com/ArmindoFlores/alchemical-clone
 Project-URL: Issues, https://github.com/ArmindoFlores/alchemical-clone/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `alchemical_clone-0.0.1/alchemical_clone.egg-info/SOURCES.txt` & `alchemical_clone-0.0.2/alchemical_clone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alchemical_clone-0.0.1/pyproject.toml` & `alchemical_clone-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "alchemical_clone"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Francisco Rodrigues", email="francisco.rodrigues@gmail.com" },
 ]
 description = "A Python package for generating SQLAlchemy ORM code from an existing database"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

