# Comparing `tmp/oso_cloud-1.4.1-py3-none-any.whl.zip` & `tmp/oso_cloud-1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 11872 bytes, number of entries: 14
--rw-r--r--  2.0 unx      310 b- defN 24-May-02 18:23 oso_cloud/__init__.py
--rw-r--r--  2.0 unx    14524 b- defN 24-May-02 18:23 oso_cloud/api.py
--rw-r--r--  2.0 unx     3586 b- defN 24-May-02 18:23 oso_cloud/helpers.py
--rw-r--r--  2.0 unx     7708 b- defN 24-May-02 18:23 oso_cloud/oso.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 18:23 oso_cloud/py.typed
--rw-r--r--  2.0 unx     2122 b- defN 24-May-02 18:23 oso_cloud/types.py
--rw-r--r--  2.0 unx       22 b- defN 24-May-02 18:23 oso_cloud/version.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 18:23 oso_cloud/experimental/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 18:23 oso_cloud/experimental/client_gen/__init__.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-02 18:23 oso_cloud/experimental/client_gen/__main__.py
--rw-r--r--  2.0 unx     3464 b- defN 24-May-02 18:23 oso_cloud-1.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-02 18:23 oso_cloud-1.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-May-02 18:23 oso_cloud-1.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1118 b- defN 24-May-02 18:23 oso_cloud-1.4.1.dist-info/RECORD
-14 files, 39668 bytes uncompressed, 10008 bytes compressed:  74.8%
+Zip file size: 11975 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      310 b- defN 24-May-24 20:37 oso_cloud/__init__.py
+-rw-r--r--  2.0 unx    14866 b- defN 24-May-24 20:37 oso_cloud/api.py
+-rw-r--r--  2.0 unx     3976 b- defN 24-May-24 20:37 oso_cloud/helpers.py
+-rw-r--r--  2.0 unx     8265 b- defN 24-May-24 20:37 oso_cloud/oso.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 20:37 oso_cloud/py.typed
+-rw-r--r--  2.0 unx     2144 b- defN 24-May-24 20:37 oso_cloud/types.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-24 20:37 oso_cloud/version.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 20:37 oso_cloud/experimental/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 20:37 oso_cloud/experimental/client_gen/__init__.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-24 20:37 oso_cloud/experimental/client_gen/__main__.py
+-rw-r--r--  2.0 unx     3464 b- defN 24-May-24 20:38 oso_cloud-1.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 20:38 oso_cloud-1.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-24 20:38 oso_cloud-1.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1118 b- defN 24-May-24 20:38 oso_cloud-1.5.0.dist-info/RECORD
+14 files, 40979 bytes uncompressed, 10111 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: oso_cloud/experimental/client_gen/__init__.py
 Comment: 
 
 Filename: oso_cloud/experimental/client_gen/__main__.py
 Comment: 
 
-Filename: oso_cloud-1.4.1.dist-info/METADATA
+Filename: oso_cloud-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: oso_cloud-1.4.1.dist-info/WHEEL
+Filename: oso_cloud-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: oso_cloud-1.4.1.dist-info/top_level.txt
+Filename: oso_cloud-1.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: oso_cloud-1.4.1.dist-info/RECORD
+Filename: oso_cloud-1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oso_cloud/api.py

```diff
@@ -463,14 +463,24 @@
             "column": column,
             "data_bindings": self.data_bindings,
         }
         result = self._do_post("/list_query", params=params, json=json)
         response = self._handle_result(result)
         return LocalQueryResult(**response)
 
+    def post_actions_query(self, query):
+        params = None
+        json = {
+            "query": asdict(query),
+            "data_bindings": self.data_bindings,
+        }
+        result = self._do_post("/actions_query", params=params, json=json)
+        response = self._handle_result(result)
+        return LocalQueryResult(**response)
+
     def clear_data(self):
         params = None
         json = None
         result = self._do_post("/clear_data", params=params, json=json)
         response = self._handle_result(result, True)
         return ApiResult(**response)
```

## oso_cloud/helpers.py

```diff
@@ -15,14 +15,18 @@
     if isinstance(instance, str):
         if instance == "":
             raise TypeError(
                 "Oso: Instance cannot be an empty string. "
                 + "For wildcards, use the empty dict ({}) or None."
             )
         return api.VariableValue("String", instance)
+    if isinstance(instance, bool):
+        return api.VariableValue("Boolean", str(instance).lower())
+    if isinstance(instance, int):
+        return api.VariableValue("Integer", str(instance))
     if "id" not in instance or instance["id"] is None:
         if "type" not in instance or instance["type"] is None:
             return api.VariableValue(None, None)
         return api.VariableValue(instance["type"], None)
 
     if "type" not in instance or instance["type"] is None:
         raise TypeError(f"Oso: Instances with an ID must also have a type: {instance}")
@@ -32,14 +36,18 @@
 def to_api_value(instance: types.Value) -> api.ConcreteValue:
     if instance is None:
         raise TypeError("Oso: Expected a concrete value with type and ID. Got None.")
     if isinstance(instance, str):
         if instance == "":
             raise TypeError("Oso: Value cannot be an empty string. ")
         return api.ConcreteValue("String", instance)
+    if isinstance(instance, bool):
+        return api.ConcreteValue("Boolean", str(instance).lower())
+    if isinstance(instance, int):
+        return api.ConcreteValue("Integer", str(instance))
     if "id" not in instance or instance["id"] is None:
         raise TypeError("Oso: Expected a concrete value, but ID was None")
 
     if "type" not in instance or instance["type"] is None:
         raise TypeError("Oso: Expected a concrete value, but type was None")
     return api.ConcreteValue(instance["type"], convert_to_str(instance["id"]))
```

## oso_cloud/oso.py

```diff
@@ -249,7 +249,22 @@
             actor_typed_id.id,
             action,
             resource_type,
             [],
         )
         result = self.api.post_list_query(data, column)
         return result.sql
+
+    def actions_local(self, actor, resource) -> str:
+        """Fetches a query that can be run against your database to determine the actions
+        an actor can perform on a resource."""
+        actor_typed_id = to_api_value(actor)
+        resource_typed_id = to_api_value(resource)
+        data = api.ActionsQuery(
+            actor_typed_id.type,
+            actor_typed_id.id,
+            resource_typed_id.type,
+            resource_typed_id.id,
+            [],
+        )
+        result = self.api.post_actions_query(data)
+        return result.sql
```

## oso_cloud/types.py

```diff
@@ -7,28 +7,28 @@
 
 
 # This lets values be a subtype of variable values
 class ValueDict(VariableValueDict, total=True):
     pass
 
 
-Value = Union[str, ValueDict]
+Value = Union[str, int, bool, ValueDict]
 """
 APIs expecting concrete values accept either a string or a dict with type and ID fields.
 
 ### Example
 
 ```python
 user: Value = {"type": "User", "id": "1"}
 role: Value = "admin
 ```
 """
 
 
-VariableValue = Union[None, str, VariableValueDict]
+VariableValue = Union[None, str, int, bool, VariableValueDict]
 """
 Variable values allow for wildcards -- expressed by ommitting ID and/or type arguments
 
 ### Example
 
 ```python
 any_user: VariableValue = {"type": "User"}
```

## oso_cloud/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.4.1"
+__version__ = "1.5.0"
```

## Comparing `oso_cloud-1.4.1.dist-info/METADATA` & `oso_cloud-1.5.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oso-cloud
-Version: 1.4.1
+Version: 1.5.0
 Summary: Oso Cloud Python client
 Home-page: https://www.osohq.com
 Author: Oso Security
 Author-email: support@osohq.com
 License: Apache-2.0
 Project-URL: Documentation, https://www.osohq.com/docs
 Keywords: authorization,rbac,oso,oso cloud,authorization as a service,microservice authorization
```

## Comparing `oso_cloud-1.4.1.dist-info/RECORD` & `oso_cloud-1.5.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 oso_cloud/__init__.py,sha256=0LriETIbMx6BvXRCs32SfOb-dFx00-EIGBvMM7TBg3I,310
-oso_cloud/api.py,sha256=VkrmEZhi9Iejt3D6sKAWAfyKxvqiW6ysCE5z9hlVYK0,14524
-oso_cloud/helpers.py,sha256=bw7-aYpa8u1JKQY03q4LH4EvGXB-QpC2Hx-a7YHFnlw,3586
-oso_cloud/oso.py,sha256=bPygNygKILa4HlhVWODwlpwKz1LRLy4noa0F_ynaffs,7708
+oso_cloud/api.py,sha256=Tl64eE1lK9k18Xkw6vwtZwW80OIGkKPigR51n2rSyVI,14866
+oso_cloud/helpers.py,sha256=uvDIStenqJNNQeTaFQ1NkPRZGWOi-4vB-haavXeZlGM,3976
+oso_cloud/oso.py,sha256=QL2ibZDdGuNyRdAvHQlTobG60SpNe1YSLEHsiFKM6mQ,8265
 oso_cloud/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-oso_cloud/types.py,sha256=1AvezZCg4Tw-ERVYOtTWS97Q5lZ1JGMqLHs95pm_mYk,2122
-oso_cloud/version.py,sha256=BqOI5y46o1G1RWC9bF1DPL-YM68lGYPmZt1pn6FZFZs,22
+oso_cloud/types.py,sha256=D7SiVI41EsXC4dMgM72YUczDuANO4Jd1Q3HSJzYrdIY,2144
+oso_cloud/version.py,sha256=X9pTeGHIYZtDOmfb9pnn2DEqWZMAyaPlqdFwEhsuSvk,22
 oso_cloud/experimental/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oso_cloud/experimental/client_gen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oso_cloud/experimental/client_gen/__main__.py,sha256=vUInc2TOz6QgiWASksm8RY7z76FqssXmzwErRcxd4qI,6712
-oso_cloud-1.4.1.dist-info/METADATA,sha256=u5BED8F2f_IKRg8BOki2AnezlHtDqqV8PMPhAdDYPy4,3464
-oso_cloud-1.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-oso_cloud-1.4.1.dist-info/top_level.txt,sha256=pzOq04dOQpqHFKR4eDR1MMZ23BacelJsh7LKlSdFnmw,10
-oso_cloud-1.4.1.dist-info/RECORD,,
+oso_cloud-1.5.0.dist-info/METADATA,sha256=WpJFhwn8D8xhPwP4DLqI35Ue_2p060JHvdov3eRx1SQ,3464
+oso_cloud-1.5.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+oso_cloud-1.5.0.dist-info/top_level.txt,sha256=pzOq04dOQpqHFKR4eDR1MMZ23BacelJsh7LKlSdFnmw,10
+oso_cloud-1.5.0.dist-info/RECORD,,
```

