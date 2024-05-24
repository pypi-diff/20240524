# Comparing `tmp/model_resolver-0.5.0.tar.gz` & `tmp/model_resolver-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_resolver-0.5.0.tar", max compression
+gzip compressed data, was "model_resolver-0.6.0.tar", max compression
```

## Comparing `model_resolver-0.5.0.tar` & `model_resolver-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2024-05-23 12:22:08.095643 model_resolver-0.5.0/LICENSE
--rw-r--r--   0        0        0     1752 2024-05-23 12:22:08.095643 model_resolver-0.5.0/README.md
--rw-r--r--   0        0        0       36 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/__init__.py
--rw-r--r--   0        0        0       59 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/__main__.py
--rw-r--r--   0        0        0     1951 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/cli.py
--rw-r--r--   0        0        0     1474 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/my_glutinit.py
--rw-r--r--   0        0        0    14567 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/plugin.py
--rw-r--r--   0        0        0    19793 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/render.py
--rw-r--r--   0        0        0     1248 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/utils.py
--rw-r--r--   0        0        0      756 2024-05-23 12:22:25.683667 model_resolver-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-24 16:43:26.249903 model_resolver-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1752 2024-05-24 16:43:26.249903 model_resolver-0.6.0/README.md
+-rw-r--r--   0        0        0       36 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/__main__.py
+-rw-r--r--   0        0        0     1924 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/cli.py
+-rw-r--r--   0        0        0     1474 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/my_glutinit.py
+-rw-r--r--   0        0        0    14476 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/plugin.py
+-rw-r--r--   0        0        0    19793 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/render.py
+-rw-r--r--   0        0        0     1248 2024-05-24 16:43:26.249903 model_resolver-0.6.0/model_resolver/utils.py
+-rw-r--r--   0        0        0      748 2024-05-24 16:43:44.053776 model_resolver-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.6.0/PKG-INFO
```

### Comparing `model_resolver-0.5.0/LICENSE` & `model_resolver-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `model_resolver-0.5.0/README.md` & `model_resolver-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `model_resolver-0.5.0/model_resolver/cli.py` & `model_resolver-0.6.0/model_resolver/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # a simple command
 @app.command()
 def main(
     # fmt: off
     render_size: int = typer.Option(256, help="Size of the rendered image"),
     load_dir: Path = typer.Option(Path.cwd(), help="Directory where the resourcepack is located"),
     output_dir: Path = typer.Option(Path.cwd() / "build", help="Where you want to save the new resourcepack, with new textures corresponding to the model"), 
+    filter: list[str] = typer.Option(None, help="Filter models in directory"),
     use_cache: bool = typer.Option(False, help="Use cache for model rendering)"),
     load_vanilla: bool = typer.Option(False, help="Load vanilla model"),
     resolve_vanilla_atlas: bool = typer.Option(False, help="Resolve vanilla model textures, True if load_vanilla is True"),
-    vanilla_filter: list[str] = typer.Option(None, help="Filter vanilla models to load"),
     minecraft_version: str = typer.Option("latest", help="Minecraft version to use for vanilla models")
     # fmt: on
 ):
     """
     A simple CLI to render models from a resourcepack, can also load vanilla models.
     """
     t_start = perf_counter()
@@ -34,15 +34,15 @@
         meta={
             "model_resolver": {
                 "load_vanilla": load_vanilla,
                 "use_cache": use_cache,
                 "render_size": render_size,
                 "minecraft_version": minecraft_version,
                 "resolve_vanilla_atlas": resolve_vanilla_atlas,
-                "vanilla_filter": vanilla_filter,
+                "filter": filter,
             },
         },
     )
     with run_beet(config=config) as ctx:
         pass
     t_end = perf_counter()
     print(f"[green][bold]✔️[/bold]  Finished in {t_end - t_start:.2f} seconds [/green]")
```

### Comparing `model_resolver-0.5.0/model_resolver/my_glutinit.py` & `model_resolver-0.6.0/model_resolver/my_glutinit.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.5.0/model_resolver/plugin.py` & `model_resolver-0.6.0/model_resolver/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,29 +22,29 @@
     if load_vanilla:
         resolve_vanilla_atlas = True
     use_cache = ctx.meta.get("model_resolver", {}).get("use_cache", False)
     render_size = ctx.meta.get("model_resolver", {}).get("render_size", 1024)
     minecraft_version = ctx.meta.get("model_resolver", {}).get(
         "minecraft_version", "latest"
     )
-    vanilla_filter = ctx.meta.get("model_resolver", {}).get("vanilla_filter", None)
+    filter = ctx.meta.get("model_resolver", {}).get("filter", None)
 
     vanilla = ctx.inject(Vanilla)
     if not minecraft_version == "latest":
         vanilla = vanilla.releases[minecraft_version]
     generated_models = set()
     generated_textures = set()
 
     for atlas in ctx.assets.atlases:
         resolve_atlas(ctx, vanilla, ctx, atlas, generated_textures)
     if resolve_vanilla_atlas:
         for atlas in vanilla.assets.atlases:
             resolve_atlas(ctx, vanilla, vanilla, atlas, generated_textures)
     if load_vanilla:
-        render_vanilla(ctx, vanilla, generated_models, vanilla_filter)
+        render_vanilla(ctx, vanilla, generated_models)
     
 
     cache = ctx.cache.get("model_resolver")
     if not "models" in cache.json:
         cache.json["models"] = {}
         cache.json["render_size"] = render_size
         cache.json["minecraft_version"] = minecraft_version
@@ -56,14 +56,17 @@
         use_cache = False
         cache.json["render_size"] = render_size
         cache.json["minecraft_version"] = minecraft_version
 
     logger.info(f"Resolving models...")
     models = {}
     for model in set(ctx.assets.models.keys()):
+        if filter is not None and len(filter) > 0:
+            if not model in filter:
+                continue
         resolved_model = resolve_model(ctx.assets.models[model], vanilla.assets.models)
         resolved_model = bake_model(
             resolved_model, ctx, vanilla, model, generated_textures
         )
         if not "textures" in resolved_model.data:
             continue
         if model in cache.json["models"] and use_cache:
@@ -104,21 +107,18 @@
 
     # load cached image
     img_path = cache.get_path(f"{model}.png")
     img = Image.open(img_path)
     return img
 
 
-def render_vanilla(ctx: Context, vanilla: Vanilla, models: set[str], vanilla_filter : list[str] | None):
+def render_vanilla(ctx: Context, vanilla: Vanilla, models: set[str]):
     vanilla_models = vanilla.assets.models
 
     for model in vanilla_models.match("minecraft:*"):
-        if vanilla_filter is not None and len(vanilla_filter) > 0:
-            if not model in vanilla_filter:
-                continue
         if "parent" in vanilla_models[model].data:
             if vanilla_models[model].data["parent"] == "builtin/entity":
                 continue
         if model not in ctx.assets.models:
             ctx.assets.models[model] = vanilla_models[model]
             models.add(model)
```

### Comparing `model_resolver-0.5.0/model_resolver/render.py` & `model_resolver-0.6.0/model_resolver/render.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.5.0/model_resolver/utils.py` & `model_resolver-0.6.0/model_resolver/utils.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.5.0/PKG-INFO` & `model_resolver-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-resolver
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 License: MIT
 Author: edayot
 Author-email: pro.e.dayot@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

