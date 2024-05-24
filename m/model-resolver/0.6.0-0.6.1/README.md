# Comparing `tmp/model_resolver-0.6.0.tar.gz` & `tmp/model_resolver-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_resolver-0.6.0.tar", max compression
+gzip compressed data, was "model_resolver-0.6.1.tar", max compression
```

## Comparing `model_resolver-0.6.0.tar` & `model_resolver-0.6.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2024-05-24 16:43:26.249903 model_resolver-0.6.0/LICENSE
--rw-r--r--   0        0        0     1752 2024-05-24 16:43:26.249903 model_resolver-0.6.0/README.md
--rw-r--r--   0        0        0       36 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/__init__.py
--rw-r--r--   0        0        0       59 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/__main__.py
--rw-r--r--   0        0        0     1924 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/cli.py
--rw-r--r--   0        0        0     1474 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/my_glutinit.py
--rw-r--r--   0        0        0    14476 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/plugin.py
--rw-r--r--   0        0        0    19793 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/render.py
--rw-r--r--   0        0        0     1248 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/utils.py
--rw-r--r--   0        0        0      748 2024-05-24 16:43:44.053776 model_resolver-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-24 19:34:26.531158 model_resolver-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1752 2024-05-24 19:34:26.531158 model_resolver-0.6.1/README.md
+-rw-r--r--   0        0        0       36 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/__main__.py
+-rw-r--r--   0        0        0     1924 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/cli.py
+-rw-r--r--   0        0        0     1474 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/my_glutinit.py
+-rw-r--r--   0        0        0    14762 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/plugin.py
+-rw-r--r--   0        0        0    19793 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/render.py
+-rw-r--r--   0        0        0     1248 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/utils.py
+-rw-r--r--   0        0        0      748 2024-05-24 19:34:43.443154 model_resolver-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.6.1/PKG-INFO
```

### Comparing `model_resolver-0.6.0/LICENSE` & `model_resolver-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.0/README.md` & `model_resolver-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.0/model_resolver/cli.py` & `model_resolver-0.6.1/model_resolver/cli.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.0/model_resolver/my_glutinit.py` & `model_resolver-0.6.1/model_resolver/my_glutinit.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.0/model_resolver/plugin.py` & `model_resolver-0.6.1/model_resolver/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     logger.info(f"Resolving models...")
     models = {}
     for model in set(ctx.assets.models.keys()):
         if filter is not None and len(filter) > 0:
             if not model in filter:
                 continue
-        resolved_model = resolve_model(ctx.assets.models[model], vanilla.assets.models)
+        resolved_model = resolve_model(ctx.assets.models[model], vanilla.assets.models, ctx.assets.models)
         resolved_model = bake_model(
             resolved_model, ctx, vanilla, model, generated_textures
         )
         if not "textures" in resolved_model.data:
             continue
         if model in cache.json["models"] and use_cache:
             img = handle_cache(cache, model, resolved_model, ctx, vanilla)
@@ -234,26 +234,31 @@
         merged["overrides"] = child.data["overrides"]
     if "gui_light" in child.data:
         merged["gui_light"] = child.data["gui_light"]
 
     return Model(merged)
 
 
-def resolve_model(model: Model, vanilla_models: dict[str, Model]) -> Model:
+def resolve_model(model: Model, vanilla_models: dict[str, Model], ctx_models: dict[str, Model]) -> Model:
     # Do something with the model
     if "parent" in model.data:
         resolved_key = resolve_key(model.data["parent"])
         if resolved_key in [
             "minecraft:builtin/generated",
             "minecraft:builtin/entity",
         ]:
             return model
-        parent_model = vanilla_models[resolved_key]
+        if resolved_key in vanilla_models:
+            parent_model = vanilla_models[resolved_key]
+        elif resolved_key in ctx_models:
+            parent_model = ctx_models[resolved_key]
+        else:
+            raise ValueError(f"Parent model {resolved_key} not found")
         parent_model = deepcopy(parent_model)
-        parent_model_resolved = resolve_model(parent_model, vanilla_models)
+        parent_model_resolved = resolve_model(parent_model, vanilla_models, ctx_models)
 
         return merge_model(model, parent_model_resolved)
     else:
         return model
 
 
 def bake_model(
```

### Comparing `model_resolver-0.6.0/model_resolver/render.py` & `model_resolver-0.6.1/model_resolver/render.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.0/model_resolver/utils.py` & `model_resolver-0.6.1/model_resolver/utils.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.0/pyproject.toml` & `model_resolver-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "model-resolver"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 authors = ["edayot <pro.e.dayot@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `model_resolver-0.6.0/PKG-INFO` & `model_resolver-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-resolver
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 License: MIT
 Author: edayot
 Author-email: pro.e.dayot@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

