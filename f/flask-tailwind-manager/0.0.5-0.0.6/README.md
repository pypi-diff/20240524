# Comparing `tmp/flask_tailwind_manager-0.0.5.tar.gz` & `tmp/flask_tailwind_manager-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_tailwind_manager-0.0.5.tar", last modified: Mon May 20 20:15:34 2024, max compression
+gzip compressed data, was "flask_tailwind_manager-0.0.6.tar", last modified: Fri May 24 04:32:49 2024, max compression
```

## Comparing `flask_tailwind_manager-0.0.5.tar` & `flask_tailwind_manager-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 20:15:34.216354 flask_tailwind_manager-0.0.5/
--rw-r--r--   0 thonder   (1000) thonder   (1000)     3098 2024-04-16 01:38:06.000000 flask_tailwind_manager-0.0.5/.gitignore
--rw-r--r--   0 thonder   (1000) thonder   (1000)     1081 2024-05-19 21:57:00.000000 flask_tailwind_manager-0.0.5/LICENSE
--rw-r--r--   0 thonder   (1000) thonder   (1000)     5099 2024-05-20 20:15:34.216354 flask_tailwind_manager-0.0.5/PKG-INFO
--rw-r--r--   0 thonder   (1000) thonder   (1000)     3295 2024-05-19 22:36:02.000000 flask_tailwind_manager-0.0.5/README.md
--rw-r--r--   0 thonder   (1000) thonder   (1000)      890 2024-05-20 20:15:08.000000 flask_tailwind_manager-0.0.5/pyproject.toml
--rw-r--r--   0 thonder   (1000) thonder   (1000)       26 2024-05-19 21:19:37.000000 flask_tailwind_manager-0.0.5/requirements-dev.txt
--rw-r--r--   0 thonder   (1000) thonder   (1000)        5 2024-05-19 21:19:33.000000 flask_tailwind_manager-0.0.5/requirements.txt
--rw-r--r--   0 thonder   (1000) thonder   (1000)       38 2024-05-20 20:15:34.226354 flask_tailwind_manager-0.0.5/setup.cfg
--rw-r--r--   0 thonder   (1000) thonder   (1000)       54 2024-05-20 19:17:17.000000 flask_tailwind_manager-0.0.5/setup.py
-drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 20:15:34.136355 flask_tailwind_manager-0.0.5/src/
-drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 20:15:34.176355 flask_tailwind_manager-0.0.5/src/flask_tailwind/
--rw-r--r--   0 thonder   (1000) thonder   (1000)       62 2024-05-19 22:11:38.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind/__init__.py
--rw-r--r--   0 thonder   (1000) thonder   (1000)     2365 2024-05-19 22:11:38.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind/cli.py
--rw-r--r--   0 thonder   (1000) thonder   (1000)     1456 2024-05-19 22:11:38.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind/console.py
--rw-r--r--   0 thonder   (1000) thonder   (1000)        0 2024-05-19 22:06:05.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind/py.typed
-drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 20:15:34.196354 flask_tailwind_manager-0.0.5/src/flask_tailwind/starter/
--rw-r--r--   0 thonder   (1000) thonder   (1000)        0 2024-05-19 00:12:17.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind/starter/.gitignore
--rw-r--r--   0 thonder   (1000) thonder   (1000)        0 2024-05-19 02:57:40.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind/starter/package.json
-drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 20:15:34.196354 flask_tailwind_manager-0.0.5/src/flask_tailwind/starter/src/
--rw-r--r--   0 thonder   (1000) thonder   (1000)       58 2024-05-19 00:19:52.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind/starter/src/input.css
--rw-r--r--   0 thonder   (1000) thonder   (1000)        0 2024-05-19 18:03:15.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind/starter/tailwind.config.js
--rw-r--r--   0 thonder   (1000) thonder   (1000)     3686 2024-05-19 22:11:38.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind/tailwind.py
-drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 20:15:34.196354 flask_tailwind_manager-0.0.5/src/flask_tailwind/templates/
--rw-r--r--   0 thonder   (1000) thonder   (1000)       73 2024-05-18 23:09:40.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind/templates/load.jinja
--rw-r--r--   0 thonder   (1000) thonder   (1000)       89 2024-05-19 18:30:33.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind/templates/package.json.jinja
--rw-r--r--   0 thonder   (1000) thonder   (1000)      497 2024-05-19 18:27:46.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind/templates/tailwind.config.js.jinja
-drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-05-20 20:15:34.206354 flask_tailwind_manager-0.0.5/src/flask_tailwind_manager.egg-info/
--rw-r--r--   0 thonder   (1000) thonder   (1000)     5099 2024-05-20 20:15:33.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind_manager.egg-info/PKG-INFO
--rw-r--r--   0 thonder   (1000) thonder   (1000)      792 2024-05-20 20:15:34.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind_manager.egg-info/SOURCES.txt
--rw-r--r--   0 thonder   (1000) thonder   (1000)        1 2024-05-20 20:15:33.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind_manager.egg-info/dependency_links.txt
--rw-r--r--   0 thonder   (1000) thonder   (1000)       16 2024-05-20 20:15:33.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind_manager.egg-info/requires.txt
--rw-r--r--   0 thonder   (1000) thonder   (1000)       15 2024-05-20 20:15:33.000000 flask_tailwind_manager-0.0.5/src/flask_tailwind_manager.egg-info/top_level.txt
+drwxr-xr-x   0 thonder5  (1000) thonder5  (1000)        0 2024-05-24 04:32:49.059302 flask_tailwind_manager-0.0.6/
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)     3098 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/.gitignore
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)     1081 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/LICENSE
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)     5099 2024-05-24 04:32:49.059302 flask_tailwind_manager-0.0.6/PKG-INFO
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)     3295 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/README.md
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)      896 2024-05-24 04:32:43.000000 flask_tailwind_manager-0.0.6/pyproject.toml
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)       38 2024-05-24 03:52:37.000000 flask_tailwind_manager-0.0.6/requirements-dev.txt
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)        5 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/requirements.txt
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)       38 2024-05-24 04:32:49.059302 flask_tailwind_manager-0.0.6/setup.cfg
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)       54 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/setup.py
+drwxr-xr-x   0 thonder5  (1000) thonder5  (1000)        0 2024-05-24 04:32:49.059302 flask_tailwind_manager-0.0.6/src/
+drwxr-xr-x   0 thonder5  (1000) thonder5  (1000)        0 2024-05-24 04:32:49.059302 flask_tailwind_manager-0.0.6/src/flask_tailwind/
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)       62 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind/__init__.py
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)     2601 2024-05-24 04:26:58.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind/cli.py
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)     1456 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind/console.py
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)        0 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind/py.typed
+drwxr-xr-x   0 thonder5  (1000) thonder5  (1000)        0 2024-05-24 04:32:49.059302 flask_tailwind_manager-0.0.6/src/flask_tailwind/starter/
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)        0 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind/starter/.gitignore
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)        0 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind/starter/package.json
+drwxr-xr-x   0 thonder5  (1000) thonder5  (1000)        0 2024-05-24 04:32:49.059302 flask_tailwind_manager-0.0.6/src/flask_tailwind/starter/src/
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)       58 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind/starter/src/input.css
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)        0 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind/starter/tailwind.config.js
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)     3711 2024-05-24 04:25:20.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind/tailwind.py
+drwxr-xr-x   0 thonder5  (1000) thonder5  (1000)        0 2024-05-24 04:32:49.059302 flask_tailwind_manager-0.0.6/src/flask_tailwind/templates/
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)       73 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind/templates/load.jinja
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)       89 2024-05-24 03:50:53.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind/templates/package.json.jinja
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)      706 2024-05-24 04:25:02.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind/templates/tailwind.config.js.jinja
+drwxr-xr-x   0 thonder5  (1000) thonder5  (1000)        0 2024-05-24 04:32:49.059302 flask_tailwind_manager-0.0.6/src/flask_tailwind_manager.egg-info/
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)     5099 2024-05-24 04:32:49.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind_manager.egg-info/PKG-INFO
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)      792 2024-05-24 04:32:49.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)        1 2024-05-24 04:32:49.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)       16 2024-05-24 04:32:49.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind_manager.egg-info/requires.txt
+-rw-r--r--   0 thonder5  (1000) thonder5  (1000)        1 2024-05-24 04:32:49.000000 flask_tailwind_manager-0.0.6/src/flask_tailwind_manager.egg-info/top_level.txt
```

### Comparing `flask_tailwind_manager-0.0.5/.gitignore` & `flask_tailwind_manager-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_tailwind_manager-0.0.5/LICENSE` & `flask_tailwind_manager-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_tailwind_manager-0.0.5/PKG-INFO` & `flask_tailwind_manager-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-tailwind-manager
-Version: 0.0.5
+Version: 0.0.6
 Summary: Easily use tailwind css with Flask projects
 Author-email: Sebastian Salinas <seba.salinas.delrio@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sebastian Salinas Del Rio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `flask_tailwind_manager-0.0.5/README.md` & `flask_tailwind_manager-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `flask_tailwind_manager-0.0.5/pyproject.toml` & `flask_tailwind_manager-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
-include = ["flask_tailwind"]  # alternatively: `exclude = ["additional*"]`
+include = ["starter", "templates"]  # alternatively: `exclude = ["additional*"]`
 namespaces = false
 
 [project]
 name = "flask-tailwind-manager"
-version = "0.0.5"
+version = "0.0.6"
 description = "Easily use tailwind css with Flask projects"
 readme = "README.md"
 authors = [{ name = "Sebastian Salinas", email = "seba.salinas.delrio@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `flask_tailwind_manager-0.0.5/src/flask_tailwind/cli.py` & `flask_tailwind_manager-0.0.6/src/flask_tailwind/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     logging.info(f"🍃 Copying default configuration files into {dest_dir}")
 
     with open(dest_dir / "package.json", "w") as file:
         file.write(tailwind.package_json_str())
 
     with open(dest_dir / "tailwind.config.js", "w") as file:
         file.write(tailwind.tailwind_config_js_str())
+    
+    shutil.move(dest_dir / "tailwind.config.js", ".")
 
     logging.info(f"🍃 Installing dependencies in {tailwind.cwd}")
     console = tailwind.get_console_interface()
     console.npm_run("-D", "install", "tailwindcss")
 
 
 @tailwind.command()
@@ -56,33 +58,35 @@
 def start():
     """Start watching CSS changes for dev."""
     tailwind: "TailwindCSS" = current_app.extensions["tailwind"]
     install_if_needed(tailwind)
     console = tailwind.get_console_interface()
     console.npx_run(
         "tailwindcss",
+        "-c",
+        "../tailwind.config.js",
         "-i",
         "./src/input.css",
         "-o",
         "../" + str(tailwind.get_output_path()),
         "--watch",
     )
 
 
-@tailwind.command()
+@tailwind.command(context_settings=dict(ignore_unknown_options=True, allow_interspersed_args=True))
 @click.argument("args", nargs=-1)
 @with_appcontext
 def npm(args: Tuple[str]) -> None:
     tailwind: "TailwindCSS" = current_app.extensions["tailwind"]
     install_if_needed(tailwind)
     console = tailwind.get_console_interface()
     console.npm_run(*args)
 
 
-@tailwind.command()
+@tailwind.command(context_settings=dict(ignore_unknown_options=True))
 @click.argument("args", nargs=-1)
 @with_appcontext
 def npx(args: Tuple[str]) -> None:
     tailwind: "TailwindCSS" = current_app.extensions["tailwind"]
     install_if_needed(tailwind)
     console = tailwind.get_console_interface()
     console.npx_run(*args)
```

### Comparing `flask_tailwind_manager-0.0.5/src/flask_tailwind/console.py` & `flask_tailwind_manager-0.0.6/src/flask_tailwind/console.py`

 * *Files identical despite different names*

### Comparing `flask_tailwind_manager-0.0.5/src/flask_tailwind/tailwind.py` & `flask_tailwind_manager-0.0.6/src/flask_tailwind/tailwind.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 
     def tailwind_config_js_str(self) -> str:
         app_name = self.app_name or "tailwind-app"
         return render_template(
             "tailwind.config.js.jinja",
             app_name=app_name,
             templates_folder=self.template_folder,
+            cwd=self.cwd
         )
 
     def __tailwind_css_tag(self) -> str:
         return render_template("load.jinja", filename=self.output_css_path)
 
     def __register_app_global(self, app: Flask) -> None:
         app.add_template_global(self.__tailwind_css_tag, "tailwind_css")
```

### Comparing `flask_tailwind_manager-0.0.5/src/flask_tailwind_manager.egg-info/PKG-INFO` & `flask_tailwind_manager-0.0.6/src/flask_tailwind_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-tailwind-manager
-Version: 0.0.5
+Version: 0.0.6
 Summary: Easily use tailwind css with Flask projects
 Author-email: Sebastian Salinas <seba.salinas.delrio@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sebastian Salinas Del Rio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `flask_tailwind_manager-0.0.5/src/flask_tailwind_manager.egg-info/SOURCES.txt` & `flask_tailwind_manager-0.0.6/src/flask_tailwind_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

