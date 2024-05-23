# Comparing `tmp/miska-0.0.4.tar.gz` & `tmp/miska-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miska-0.0.4.tar", last modified: Wed May 22 15:29:45 2024, max compression
+gzip compressed data, was "miska-0.0.5.tar", last modified: Thu May 23 23:14:34 2024, max compression
```

## Comparing `miska-0.0.4.tar` & `miska-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.819277 miska-0.0.4/
--rw-r--r--   0 cell      (1000) cell      (1000)     1289 2024-03-09 16:24:22.000000 miska-0.0.4/LICENSE
--rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-22 15:29:45.818277 miska-0.0.4/PKG-INFO
--rw-r--r--   0 cell      (1000) cell      (1000)      578 2024-03-09 16:24:22.000000 miska-0.0.4/README.rst
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.813278 miska-0.0.4/miska/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.4/miska/__init__.py
--rw-r--r--   0 cell      (1000) cell      (1000)     1215 2024-05-22 15:28:25.000000 miska-0.0.4/miska/dataclasses.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.815277 miska-0.0.4/miska/http/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.4/miska/http/__init__.py
--rw-r--r--   0 cell      (1000) cell      (1000)     1395 2024-03-09 16:24:22.000000 miska-0.0.4/miska/http/rs.py
--rw-r--r--   0 cell      (1000) cell      (1000)      222 2024-03-09 16:24:22.000000 miska-0.0.4/miska/mixins.py
--rw-r--r--   0 cell      (1000) cell      (1000)     1828 2024-05-22 15:28:18.000000 miska-0.0.4/miska/registries.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.816277 miska-0.0.4/miska/types/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.4/miska/types/__init__.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.816277 miska-0.0.4/miska/types/network/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.4/miska/types/network/__init__.py
--rw-r--r--   0 cell      (1000) cell      (1000)     3206 2024-03-09 16:24:22.000000 miska-0.0.4/miska/types/network/bgp.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.817278 miska-0.0.4/miska.egg-info/
--rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-22 15:29:45.000000 miska-0.0.4/miska.egg-info/PKG-INFO
--rw-r--r--   0 cell      (1000) cell      (1000)      400 2024-05-22 15:29:45.000000 miska-0.0.4/miska.egg-info/SOURCES.txt
--rw-r--r--   0 cell      (1000) cell      (1000)        1 2024-05-22 15:29:45.000000 miska-0.0.4/miska.egg-info/dependency_links.txt
--rw-r--r--   0 cell      (1000) cell      (1000)       36 2024-05-22 15:29:45.000000 miska-0.0.4/miska.egg-info/requires.txt
--rw-r--r--   0 cell      (1000) cell      (1000)        6 2024-05-22 15:29:45.000000 miska-0.0.4/miska.egg-info/top_level.txt
--rw-r--r--   0 cell      (1000) cell      (1000)      843 2024-05-22 15:28:25.000000 miska-0.0.4/pyproject.toml
--rw-r--r--   0 cell      (1000) cell      (1000)       38 2024-05-22 15:29:45.819277 miska-0.0.4/setup.cfg
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-22 15:29:45.817278 miska-0.0.4/tests/
--rw-r--r--   0 cell      (1000) cell      (1000)      275 2024-05-21 08:54:48.000000 miska-0.0.4/tests/test_registries.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-23 23:14:34.393249 miska-0.0.5/
+-rw-r--r--   0 cell      (1000) cell      (1000)     1289 2024-03-09 16:24:22.000000 miska-0.0.5/LICENSE
+-rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-23 23:14:34.393249 miska-0.0.5/PKG-INFO
+-rw-r--r--   0 cell      (1000) cell      (1000)      578 2024-03-09 16:24:22.000000 miska-0.0.5/README.rst
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-23 23:14:34.390249 miska-0.0.5/miska/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.5/miska/__init__.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     2987 2024-05-23 23:04:10.000000 miska-0.0.5/miska/dataclasses.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-23 23:14:34.391249 miska-0.0.5/miska/http/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.5/miska/http/__init__.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     1395 2024-03-09 16:24:22.000000 miska-0.0.5/miska/http/rs.py
+-rw-r--r--   0 cell      (1000) cell      (1000)      222 2024-03-09 16:24:22.000000 miska-0.0.5/miska/mixins.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     1828 2024-05-22 15:28:18.000000 miska-0.0.5/miska/registries.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-23 23:14:34.391249 miska-0.0.5/miska/types/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.5/miska/types/__init__.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-23 23:14:34.392249 miska-0.0.5/miska/types/network/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.5/miska/types/network/__init__.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     3206 2024-03-09 16:24:22.000000 miska-0.0.5/miska/types/network/bgp.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-23 23:14:34.392249 miska-0.0.5/miska.egg-info/
+-rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-23 23:14:34.000000 miska-0.0.5/miska.egg-info/PKG-INFO
+-rw-r--r--   0 cell      (1000) cell      (1000)      400 2024-05-23 23:14:34.000000 miska-0.0.5/miska.egg-info/SOURCES.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)        1 2024-05-23 23:14:34.000000 miska-0.0.5/miska.egg-info/dependency_links.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)       36 2024-05-23 23:14:34.000000 miska-0.0.5/miska.egg-info/requires.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)        6 2024-05-23 23:14:34.000000 miska-0.0.5/miska.egg-info/top_level.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)      843 2024-05-23 23:04:10.000000 miska-0.0.5/pyproject.toml
+-rw-r--r--   0 cell      (1000) cell      (1000)       38 2024-05-23 23:14:34.393249 miska-0.0.5/setup.cfg
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-23 23:14:34.392249 miska-0.0.5/tests/
+-rw-r--r--   0 cell      (1000) cell      (1000)      275 2024-05-21 08:54:48.000000 miska-0.0.5/tests/test_registries.py
```

### Comparing `miska-0.0.4/LICENSE` & `miska-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `miska-0.0.4/PKG-INFO` & `miska-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miska
-Version: 0.0.4
+Version: 0.0.5
 Summary: An exceptional library
 Author-email: Dima Burmistrov <pyctrl.dev@gmail.com>
 License: Copyright (c) 2023-2024 Dmitry Burmistrov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `miska-0.0.4/README.rst` & `miska-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `miska-0.0.4/miska/dataclasses.py` & `miska-0.0.5/miska/dataclasses.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,43 +2,103 @@
 
 
 _K_PRIVATE = "private"
 _K_METADATA = "metadata"
 _BASE_MODEL_INIT_FLAG = "_BASE_MODEL_INIT_FLAG"
 
 
+public_field = dataclasses.field
+
+
 def private_field(**kwargs) -> dataclasses.Field:
     kwargs.setdefault(_K_METADATA, {})[_K_PRIVATE] = True
     return dataclasses.field(**kwargs)
 
 
 class BaseModel:
 
+    """Base class for dataclass magic
+
+    - supports private fields that can't be modified
+
+    from dataclasses import *
+    from miska.dataclasses import *
+
+    @dataclass
+    class MyDataClass(BaseModel):
+        public_field: str = public_field()
+        private_field: str = private_field()
+
+    d = MyDataClass("a", "b")
+    print(d)  # MyDataClass(public_field='a', private_field='b')
+
+    d.public_field = "A"
+    print(d)  # MyDataClass(public_field='A', private_field='b')
+
+    d.private_field = "B"
+    # AttributeError: Forbidden to modify private attribute: private_field
+    """
+
+    __allow_attribute_deletion__ = False
+
     __PRIVATES = {}
 
     as_tuple = dataclasses.astuple
     as_dict =  dataclasses.asdict
 
     def __post_init__(self):
+        self._validate()
         self._mark_init_finished()
 
-    def _mark_init_finished(self):
+    def _mark_init_finished(self) -> None:
         setattr(self, _BASE_MODEL_INIT_FLAG, False)
 
     def _setattr(self, key, value):
         return super().__setattr__(key, value)
 
-    def __setattr__(self, key, value):
-        if getattr(self, _BASE_MODEL_INIT_FLAG, True):
-            return super().__setattr__(key, value)
+    def _validate(self) -> None:
+        pass
+
+    def __discover_privates(self):
+        privates = set()
+        for field in dataclasses.fields(self):
+            flag = field.metadata.get(_K_PRIVATE, False)
+            if flag:
+                privates.add(field.name)
+        return privates
 
+    def __get_privates(self):
         privates = self.__PRIVATES.get(self.__class__)
         if privates is None:
-            privates = {field.name: field.metadata.get(_K_PRIVATE, False)
-                        for field in dataclasses.fields(self)}
+            privates = self.__discover_privates()
             self.__PRIVATES[self.__class__] = privates
+        return privates
+
+    def __setattr__(self, key: str, value):
+        # allow to initialize instance during dataclass magic
+        if getattr(self, _BASE_MODEL_INIT_FLAG, True):
+            return super().__setattr__(key, value)
+        # allow managing regular private attributes
+        elif key.startswith("_") and hasattr(self, key):
+            return super().__setattr__(key, value)
+
+        privates = self.__get_privates()
+
+        # magic for inner modification like `self._private_field = 42`
+        #   (it converts name into field that marked as private)
+        if key.startswith("_"):
+            _key = key[1:]
+            if _key in privates:
+                return super().__setattr__(_key, value)
 
-        if privates[key]:
+        # magic for restricting private field modifications
+        if key in privates:
             msg = f"Forbidden to modify private attribute: {key}"
             raise AttributeError(msg)
 
         return super().__setattr__(key, value)
+
+    def __delattr__(self, item):
+        if self.__allow_attribute_deletion__:
+            return super().__delattr__(item)
+
+        raise AttributeError("Attributes can't be deleted")
```

### Comparing `miska-0.0.4/miska/http/rs.py` & `miska-0.0.5/miska/http/rs.py`

 * *Files identical despite different names*

### Comparing `miska-0.0.4/miska/registries.py` & `miska-0.0.5/miska/registries.py`

 * *Files identical despite different names*

### Comparing `miska-0.0.4/miska/types/network/bgp.py` & `miska-0.0.5/miska/types/network/bgp.py`

 * *Files identical despite different names*

### Comparing `miska-0.0.4/miska.egg-info/PKG-INFO` & `miska-0.0.5/miska.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miska
-Version: 0.0.4
+Version: 0.0.5
 Summary: An exceptional library
 Author-email: Dima Burmistrov <pyctrl.dev@gmail.com>
 License: Copyright (c) 2023-2024 Dmitry Burmistrov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `miska-0.0.4/pyproject.toml` & `miska-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "miska"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Dima Burmistrov", email="pyctrl.dev@gmail.com" },
 ]
 description = "An exceptional library"
 readme = "README.rst"
 license = {file = "LICENSE"}
```

