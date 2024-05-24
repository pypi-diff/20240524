# Comparing `tmp/coltrane-0.34.0.tar.gz` & `tmp/coltrane-0.35.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coltrane-0.34.0.tar", max compression
+gzip compressed data, was "coltrane-0.35.0.tar", max compression
```

## Comparing `coltrane-0.34.0.tar` & `coltrane-0.35.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1066 2022-01-05 04:16:46.952062 coltrane-0.34.0/LICENSE
--rw-r--r--   0        0        0     4820 2024-05-13 22:55:14.205664 coltrane-0.34.0/README.md
--rw-r--r--   0        0        0    14047 2024-05-13 22:55:14.205913 coltrane-0.34.0/coltrane/__init__.py
--rw-r--r--   0        0        0        0 2022-01-08 22:33:55.376070 coltrane-0.34.0/coltrane/config/__init__.py
--rw-r--r--   0        0        0     1404 2023-11-21 02:29:05.205562 coltrane-0.34.0/coltrane/config/cache.py
--rw-r--r--   0        0        0     2918 2024-05-13 22:55:14.206087 coltrane-0.34.0/coltrane/config/paths.py
--rw-r--r--   0        0        0     1022 2024-05-13 22:55:14.206208 coltrane-0.34.0/coltrane/config/redirects.py
--rw-r--r--   0        0        0     2955 2024-05-13 22:55:14.206370 coltrane-0.34.0/coltrane/config/settings.py
--rw-r--r--   0        0        0     4474 2024-03-01 13:05:09.414741 coltrane-0.34.0/coltrane/console.py
--rw-r--r--   0        0        0       87 2024-05-13 22:55:14.206504 coltrane-0.34.0/coltrane/context_processors.py
--rw-r--r--   0        0        0     1404 2024-01-07 19:55:42.426694 coltrane-0.34.0/coltrane/default-files/Dockerfile
--rw-r--r--   0        0        0       79 2024-01-08 00:16:44.092955 coltrane-0.34.0/coltrane/default-files/README.md
--rw-r--r--   0        0        0      245 2024-01-08 00:16:57.676856 coltrane-0.34.0/coltrane/default-files/app.py
--rw-r--r--   0        0        0       68 2024-01-07 15:38:37.525852 coltrane-0.34.0/coltrane/default-files/env
--rw-r--r--   0        0        0       10 2024-01-07 15:34:34.518859 coltrane-0.34.0/coltrane/default-files/gitignore
--rw-r--r--   0        0        0      165 2024-01-07 15:33:37.336569 coltrane-0.34.0/coltrane/default-files/gunicorn.conf.py
--rw-r--r--   0        0        0       37 2024-01-07 15:35:30.796182 coltrane-0.34.0/coltrane/default-files/watchmanconfig
--rw-r--r--   0        0        0     1281 2024-03-01 12:30:51.465959 coltrane-0.34.0/coltrane/feeds.py
--rw-r--r--   0        0        0        0 2022-01-01 20:39:42.219557 coltrane-0.34.0/coltrane/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 02:02:14.248102 coltrane-0.34.0/coltrane/management/commands/__init__.py
--rw-r--r--   0        0        0    12040 2024-05-13 22:55:14.206800 coltrane-0.34.0/coltrane/management/commands/build.py
--rw-r--r--   0        0        0     7688 2023-11-21 02:29:05.207699 coltrane-0.34.0/coltrane/manifest.py
--rw-r--r--   0        0        0      693 2023-12-03 02:20:31.935691 coltrane-0.34.0/coltrane/middleware.py
--rw-r--r--   0        0        0      958 2024-05-13 22:55:14.206919 coltrane-0.34.0/coltrane/module_finder.py
--rw-r--r--   0        0        0    14059 2024-05-13 22:55:14.207147 coltrane-0.34.0/coltrane/renderer.py
--rw-r--r--   0        0        0     4292 2024-03-01 12:30:51.466354 coltrane-0.34.0/coltrane/retriever.py
--rw-r--r--   0        0        0      342 2022-03-12 21:23:42.389804 coltrane-0.34.0/coltrane/sitemaps.py
--rw-r--r--   0        0        0      408 2022-02-26 20:13:57.756348 coltrane-0.34.0/coltrane/templates/coltrane/base.html
--rw-r--r--   0        0        0       92 2022-01-02 18:58:48.459102 coltrane-0.34.0/coltrane/templates/coltrane/content.html
--rw-r--r--   0        0        0        0 2022-02-18 02:46:45.605179 coltrane-0.34.0/coltrane/templatetags/__init__.py
--rw-r--r--   0        0        0     6625 2023-11-25 04:16:44.358354 coltrane-0.34.0/coltrane/templatetags/coltrane_tags.py
--rw-r--r--   0        0        0     1539 2024-05-13 22:55:14.207307 coltrane-0.34.0/coltrane/urls.py
--rw-r--r--   0        0        0     1740 2024-04-30 11:50:51.820465 coltrane-0.34.0/coltrane/utils.py
--rw-r--r--   0        0        0     7526 2023-11-26 03:27:35.595687 coltrane-0.34.0/coltrane/views.py
--rw-r--r--   0        0        0     5360 2024-05-13 22:55:14.210389 coltrane-0.34.0/pyproject.toml
--rw-r--r--   0        0        0     6799 1970-01-01 00:00:00.000000 coltrane-0.34.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-01-05 04:16:46.952062 coltrane-0.35.0/LICENSE
+-rw-r--r--   0        0        0     4722 2024-05-24 12:04:19.636824 coltrane-0.35.0/README.md
+-rw-r--r--   0        0        0    14466 2024-05-23 23:43:03.471452 coltrane-0.35.0/coltrane/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-08 22:33:55.376070 coltrane-0.35.0/coltrane/config/__init__.py
+-rw-r--r--   0        0        0     1404 2023-11-21 02:29:05.205562 coltrane-0.35.0/coltrane/config/cache.py
+-rw-r--r--   0        0        0     2918 2024-05-13 22:55:14.206087 coltrane-0.35.0/coltrane/config/paths.py
+-rw-r--r--   0        0        0     1022 2024-05-13 22:55:14.206208 coltrane-0.35.0/coltrane/config/redirects.py
+-rw-r--r--   0        0        0     2955 2024-05-13 22:55:14.206370 coltrane-0.35.0/coltrane/config/settings.py
+-rw-r--r--   0        0        0     5177 2024-05-24 00:21:57.806314 coltrane-0.35.0/coltrane/console.py
+-rw-r--r--   0        0        0       87 2024-05-13 22:55:14.206504 coltrane-0.35.0/coltrane/context_processors.py
+-rw-r--r--   0        0        0     1346 2024-05-24 00:21:18.987673 coltrane-0.35.0/coltrane/default-files/Dockerfile
+-rw-r--r--   0        0        0       79 2024-01-08 00:16:44.092955 coltrane-0.35.0/coltrane/default-files/README.md
+-rw-r--r--   0        0        0      245 2024-01-08 00:16:57.676856 coltrane-0.35.0/coltrane/default-files/app.py
+-rw-r--r--   0        0        0       68 2024-01-07 15:38:37.525852 coltrane-0.35.0/coltrane/default-files/env
+-rw-r--r--   0        0        0       10 2024-01-07 15:34:34.518859 coltrane-0.35.0/coltrane/default-files/gitignore
+-rw-r--r--   0        0        0      165 2024-01-07 15:33:37.336569 coltrane-0.35.0/coltrane/default-files/gunicorn.conf.py
+-rw-r--r--   0        0        0      153 2024-05-24 12:13:06.821936 coltrane-0.35.0/coltrane/default-files/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-01-07 15:35:30.796182 coltrane-0.35.0/coltrane/default-files/watchmanconfig
+-rw-r--r--   0        0        0     1281 2024-03-01 12:30:51.465959 coltrane-0.35.0/coltrane/feeds.py
+-rw-r--r--   0        0        0        0 2022-01-01 20:39:42.219557 coltrane-0.35.0/coltrane/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 02:02:14.248102 coltrane-0.35.0/coltrane/management/commands/__init__.py
+-rw-r--r--   0        0        0    12032 2024-05-14 10:49:50.074140 coltrane-0.35.0/coltrane/management/commands/build.py
+-rw-r--r--   0        0        0     7688 2023-11-21 02:29:05.207699 coltrane-0.35.0/coltrane/manifest.py
+-rw-r--r--   0        0        0      693 2023-12-03 02:20:31.935691 coltrane-0.35.0/coltrane/middleware.py
+-rw-r--r--   0        0        0      958 2024-05-13 22:55:14.206919 coltrane-0.35.0/coltrane/module_finder.py
+-rw-r--r--   0        0        0    14059 2024-05-13 22:55:14.207147 coltrane-0.35.0/coltrane/renderer.py
+-rw-r--r--   0        0        0     4292 2024-03-01 12:30:51.466354 coltrane-0.35.0/coltrane/retriever.py
+-rw-r--r--   0        0        0      342 2022-03-12 21:23:42.389804 coltrane-0.35.0/coltrane/sitemaps.py
+-rw-r--r--   0        0        0      408 2022-02-26 20:13:57.756348 coltrane-0.35.0/coltrane/templates/coltrane/base.html
+-rw-r--r--   0        0        0       92 2022-01-02 18:58:48.459102 coltrane-0.35.0/coltrane/templates/coltrane/content.html
+-rw-r--r--   0        0        0        0 2022-02-18 02:46:45.605179 coltrane-0.35.0/coltrane/templatetags/__init__.py
+-rw-r--r--   0        0        0     6625 2023-11-25 04:16:44.358354 coltrane-0.35.0/coltrane/templatetags/coltrane_tags.py
+-rw-r--r--   0        0        0     1539 2024-05-13 22:55:14.207307 coltrane-0.35.0/coltrane/urls.py
+-rw-r--r--   0        0        0     1740 2024-04-30 11:50:51.820465 coltrane-0.35.0/coltrane/utils.py
+-rw-r--r--   0        0        0     7526 2023-11-26 03:27:35.595687 coltrane-0.35.0/coltrane/views.py
+-rw-r--r--   0        0        0     5559 2024-05-24 00:16:57.340009 coltrane-0.35.0/pyproject.toml
+-rw-r--r--   0        0        0     6753 1970-01-01 00:00:00.000000 coltrane-0.35.0/PKG-INFO
```

### Comparing `coltrane-0.34.0/LICENSE` & `coltrane-0.35.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/README.md` & `coltrane-0.35.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -23,46 +23,46 @@
 - Local development server which includes [live re-rendering of markdown and data](https://twitter.com/adamghill/status/1487522925393715205) via https://github.com/adamchainz/django-browser-reload
 - Site-wide redirects
 - Deployment best practices with `whitenoise` and `gunicorn` already configured
 - Leverage the power of built-in `Django` templates, template tags, and filters inside `markdown` files
 - Any custom template tags and filters are enabled automatically for use in `markdown` or HTML templates
 - Include any third-party [`Django` app](https://djangopackages.org) for additional functionality
 - Optional command to generate static HTML files
-- Able to be integrated into a regular `Django` project as a standard third-party `Django` app
+- Can be integrated into a regular `Django` project as a standard third-party `Django` app to render markdown content
 
 ## ⚡ Quick start
 
 1. `mkdir new-site && cd new-site` to create a new folder
-1. `poetry init --no-interaction --dependency 'coltrane:<1' && poetry install` to create a new virtual environment and install the `coltrane` package
-1. Optional: `brew install watchman` on MacOS for less resource-intensive local development server
-1. `poetry run coltrane create` to create the folder structure for a new site
-1. `poetry run coltrane play` to start local development server
+1. `python3 -m venv .venv && source .venv/bin/activate && pip install coltrane` to install the `coltrane` package
+1. `coltrane create` to create the folder structure for a new site
+1. `coltrane play` to start local development server
 1. Go to http://localhost:8000 to see the original markdown rendered into HTML
 1. Update `content/index.md`
-1. Go to http://localhost:8000 to see the updated markdown rendered into HTML
-1. Optional: run `poetry run coltrane record` to build static HTML files
+1. Refresh http://localhost:8000 to see the updated markdown rendered into HTML
+1. Optional: run `coltrane record` to build static HTML files
 
 ### Generated `coltrane` file structure
 
 ```bash
 .
-├── .env
 ├── .gitignore
-├── .watchmanconfig
-├── __init__.py
-├── app.py
-├── content
-│   └── index.md
-├── data
 ├── Dockerfile
-├── gunicorn.conf.py
-├── templates
-├── poetry.lock
-└── pyproject.toml
-└── redirects.json
+├── README.md
+├── pyproject.toml
+└── site
+    ├── .env
+    ├── .watchmanconfig
+    ├── __init__.py
+    ├── app.py
+    ├── content
+    │   └── index.md
+    ├── data
+    ├── gunicorn.conf.py
+    ├── static
+    └── templates
 ```
 
 ## 📝 Content
 
 Add `markdown` files or sub-directories to the `content` directory and rendered HTML will be accessible via auto-generated routes.
 
 - `/` would render the `markdown` in `content/index.md`
```

#### html2text {}

```diff
@@ -15,43 +15,41 @@
 twitter.com/adamghill/status/1487522925393715205) via https://github.com/
 adamchainz/django-browser-reload - Site-wide redirects - Deployment best
 practices with `whitenoise` and `gunicorn` already configured - Leverage the
 power of built-in `Django` templates, template tags, and filters inside
 `markdown` files - Any custom template tags and filters are enabled
 automatically for use in `markdown` or HTML templates - Include any third-party
 [`Django` app](https://djangopackages.org) for additional functionality -
-Optional command to generate static HTML files - Able to be integrated into a
-regular `Django` project as a standard third-party `Django` app ## â¡ Quick
-start 1. `mkdir new-site && cd new-site` to create a new folder 1. `poetry init
---no-interaction --dependency 'coltrane:<1' && poetry install` to create a new
-virtual environment and install the `coltrane` package 1. Optional: `brew
-install watchman` on MacOS for less resource-intensive local development server
-1. `poetry run coltrane create` to create the folder structure for a new site
-1. `poetry run coltrane play` to start local development server 1. Go to http:/
-/localhost:8000 to see the original markdown rendered into HTML 1. Update
-`content/index.md` 1. Go to http://localhost:8000 to see the updated markdown
-rendered into HTML 1. Optional: run `poetry run coltrane record` to build
-static HTML files ### Generated `coltrane` file structure ```bash . âââ
-.env âââ .gitignore âââ .watchmanconfig âââ __init__.py
-âââ app.py âââ content âÂ Â  âââ index.md âââ data
-âââ Dockerfile âââ gunicorn.conf.py âââ templates âââ
-poetry.lock âââ pyproject.toml âââ redirects.json ``` ## ð
-Content Add `markdown` files or sub-directories to the `content` directory and
-rendered HTML will be accessible via auto-generated routes. - `/` would render
-the `markdown` in `content/index.md` - `/about/` would render the `markdown` in
-`content/about.md` - `/articles/this-is-the-first-article/` would render the
-content from `/content/articles/this-is-the-first-article.md` - `/not-there/
-` will 404 HTML will also be served automatically if a `markdown` file can not
-be found. - `/app/` would render the HTML from `/templates/app.html` or `/
-templates/app/index.html` - `/app/some-user` would render the HTML from `/
-templates/app/*.html` ## Deployment Example `Dockerfile` and `gunicorn.conf.py`
-files are created when an app is created, and optional dependencies can be
-installed for efficient `static` serving with `whitenoise`. # ð
-Documentation Read all of the documentation at https://coltrane.readthedocs.io.
-## Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
-allcontributors.org/docs/en/emoji-key)):
+Optional command to generate static HTML files - Can be integrated into a
+regular `Django` project as a standard third-party `Django` app to render
+markdown content ## â¡ Quick start 1. `mkdir new-site && cd new-site` to
+create a new folder 1. `python3 -m venv .venv && source .venv/bin/activate &&
+pip install coltrane` to install the `coltrane` package 1. `coltrane create` to
+create the folder structure for a new site 1. `coltrane play` to start local
+development server 1. Go to http://localhost:8000 to see the original markdown
+rendered into HTML 1. Update `content/index.md` 1. Refresh http://localhost:
+8000 to see the updated markdown rendered into HTML 1. Optional: run `coltrane
+record` to build static HTML files ### Generated `coltrane` file structure
+```bash . âââ .gitignore âââ Dockerfile âââ README.md
+âââ pyproject.toml âââ site âââ .env âââ
+.watchmanconfig âââ __init__.py âââ app.py âââ content
+âÂ Â  âââ index.md âââ data âââ gunicorn.conf.py âââ
+static âââ templates ``` ## ð Content Add `markdown` files or sub-
+directories to the `content` directory and rendered HTML will be accessible via
+auto-generated routes. - `/` would render the `markdown` in `content/index.md`
+- `/about/` would render the `markdown` in `content/about.md` - `/articles/
+this-is-the-first-article/` would render the content from `/content/articles/
+this-is-the-first-article.md` - `/not-there/` will 404 HTML will also be served
+automatically if a `markdown` file can not be found. - `/app/` would render the
+HTML from `/templates/app.html` or `/templates/app/index.html` - `/app/some-
+user` would render the HTML from `/templates/app/*.html` ## Deployment Example
+`Dockerfile` and `gunicorn.conf.py` files are created when an app is created,
+and optional dependencies can be installed for efficient `static` serving with
+`whitenoise`. # ð Documentation Read all of the documentation at https://
+coltrane.readthedocs.io. ## Contributors â¨ Thanks goes to these wonderful
+people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 _[_T_o_b_i_ _D_E_G_N_O_N_]
  _TT_oo_bb_ii_ _DD_EE_GG_NN_OO_NN
  _â__ _ï_¸_ _ð___»
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `coltrane-0.34.0/coltrane/__init__.py` & `coltrane-0.35.0/coltrane/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 from django import setup as django_setup
 from django.conf import settings
 from django.core.handlers.wsgi import WSGIHandler
 from django.template.library import InvalidTemplateLibrary, import_library
-from dotenv import load_dotenv
+from dotenv.main import DotEnv
 
 from coltrane.config.settings import (
     DEFAULT_COLTRANE_SETTINGS,
 )
 from coltrane.module_finder import (
     is_django_compressor_installed,
     is_django_unicorn_installed,
@@ -64,15 +64,18 @@
 
 def _get_base_dir(base_dir: Optional[Path]) -> Path:
     """
     Gets the base directory.
     """
 
     if base_dir is None:
-        base_dir = Path(".")
+        base_dir = Path("site")
+
+        if not base_dir.exists():
+            base_dir = Path(".")
     elif isinstance(base_dir, str):
         base_dir = Path(base_dir)
 
     return base_dir
 
 
 def _get_template_tag_module_name(base_dir: Path, file: Path) -> str:
@@ -397,22 +400,31 @@
     """
     Configures the settings in Django.
     """
 
     settings.configure(**django_settings)
 
 
+def _load_environment_variables(base_dir: Path, django_settings: Dict[str, Any]) -> None:
+    dot_env = DotEnv(base_dir / ".env")
+    dot_env.set_as_environment_variables()
+
+    if "ENV" not in django_settings:
+        django_settings["ENV"] = {}
+
+    django_settings["ENV"].update(dot_env.dict())
+
+
 def initialize(**django_settings) -> WSGIHandler:
     """
     Initializes the Django static site.
     """
 
     base_dir = _get_base_dir(django_settings.get("BASE_DIR"))
-
-    load_dotenv(base_dir / ".env")
+    _load_environment_variables(base_dir=base_dir, django_settings=django_settings)
 
     django_settings = _merge_settings(base_dir, django_settings)
     _configure_settings(django_settings)
 
     django_setup()
 
     return WSGIHandler()
```

### Comparing `coltrane-0.34.0/coltrane/config/cache.py` & `coltrane-0.35.0/coltrane/config/cache.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/coltrane/config/paths.py` & `coltrane-0.35.0/coltrane/config/paths.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/coltrane/config/redirects.py` & `coltrane-0.35.0/coltrane/config/redirects.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/coltrane/config/settings.py` & `coltrane-0.35.0/coltrane/config/settings.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/coltrane/console.py` & `coltrane-0.35.0/coltrane/console.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,24 +10,31 @@
 
 import rich_click as click
 from click_aliases import ClickAliasedGroup
 from django.core.management.utils import get_random_secret_key
 from rich_click.rich_command import RichCommand
 
 FILES_PATH = Path(__file__).parent / "default-files"
+APP_DIR = "site"
 
 
 def _run_management_command(command_name, *args):
     current_directory = getcwd()
     file_path = Path(current_directory) / "app.py"
 
+    if not file_path.exists():
+        file_path = Path(current_directory) / APP_DIR / "app.py"
+
+    if not file_path.exists():
+        raise Exception("app.py could not be found.")
+
     run_process([file_path, command_name, *list(args)])  # noqa: S603, PLW1510
 
 
-def _copy_file(file_name) -> None:
+def _copy_file(file_name, in_app_dir=False) -> None:
     default_file_name = file_name
 
     if file_name.startswith("."):
         default_file_name = file_name[1:]
 
     with (FILES_PATH / default_file_name).open() as f:
         file_text = f.read()
@@ -38,15 +45,20 @@
 
         if "__app_name__" in file_text:
             current_directory = getcwd().split("/")
             app_name = current_directory[len(current_directory) - 1 :][0]
 
             file_text = file_text.replace("__app_name__", app_name)
 
-        Path(file_name).write_text(file_text)
+        path = Path(file_name)
+
+        if in_app_dir:
+            path = APP_DIR / path
+
+        path.write_text(file_text)
 
 
 class AliasedCommands(ClickAliasedGroup, RichCommand):
     pass
 
 
 @click.group(cls=AliasedCommands, help="Runs commands for coltrane.")
@@ -56,66 +68,73 @@
 
 
 @cli.command(help="Create a new coltrane site. Alias: init.", aliases=["init"])
 @click.option("--force/--no-force", default=False, help="Force creating a new site")
 def create(force):
     app_file = Path("app.py")
 
+    if not app_file.exists():
+        app_file = APP_DIR / Path("app.py")
+
     if app_file.exists() and not force:
         click.secho("Skip project creation because app.py already exists.", fg="red")
     else:
         click.secho("Start creating files...\n", fg="yellow")
-        Path("__init__.py").touch()
+        Path(APP_DIR).mkdir(exist_ok=True)
+        (APP_DIR / Path("__init__.py")).touch()
 
-        click.secho("- Create app.py")
-        _copy_file("app.py")
+        click.secho("- Create .gitignore")
+        _copy_file(".gitignore")
 
-        click.secho("- Set app.py as executable")
-        app_file.chmod(app_file.stat().st_mode | S_IEXEC)
+        click.secho("- Create Dockerfile")
+        _copy_file("Dockerfile")
+
+        click.secho("- Create pyproject.toml")
+        _copy_file("pyproject.toml")
 
-        click.secho("- Create .env")
-        _copy_file(".env")
+        click.secho("- Create README.md")
+        _copy_file("README.md")
+
+        click.secho(f"- Create {APP_DIR}/.env")
+        _copy_file(".env", in_app_dir=True)
 
         # Add randomly generated secret key
-        with Path(".env").open("a") as f:
+        with (APP_DIR / Path(".env")).open("a") as f:
             f.write(f"SECRET_KEY={get_random_secret_key()}")
 
-        click.secho("- Create .watchmanconfig")
-        _copy_file(".watchmanconfig")
+        click.secho(f"- Create {APP_DIR}/.watchmanconfig")
+        _copy_file(".watchmanconfig", in_app_dir=True)
 
-        click.secho("- Create .gitignore")
-        _copy_file(".gitignore")
+        click.secho(f"- Create {APP_DIR}/app.py")
+        _copy_file("app.py", in_app_dir=True)
 
-        click.secho("- Create README.md")
-        _copy_file("README.md")
-
-        click.secho("- Create gunicorn.conf.py")
-        _copy_file("gunicorn.conf.py")
+        click.secho(f"- Set {APP_DIR}/app.py as executable")
+        app_file.chmod(app_file.stat().st_mode | S_IEXEC)
 
-        click.secho("- Create Dockerfile")
-        _copy_file("Dockerfile")
+        click.secho(f"- Create {APP_DIR}/gunicorn.conf.py")
+        _copy_file("gunicorn.conf.py", in_app_dir=True)
 
-        click.secho("- Create content directory")
-        Path("content").mkdir(exist_ok=True)
-        (Path("content") / "index.md").write_text("# index.md")
+        click.secho("- Create site/content directory")
+        (APP_DIR / Path("content")).mkdir(exist_ok=True)
+        (APP_DIR / Path("content") / "index.md").write_text("# index.md")
 
-        click.secho("- Create data directory")
-        Path("data").mkdir(exist_ok=True)
+        click.secho("- Create site/data directory")
+        (APP_DIR / Path("data")).mkdir(exist_ok=True)
 
-        click.secho("- Create static directory")
-        Path("static").mkdir(exist_ok=True)
+        click.secho("- Create site/static directory")
+        (APP_DIR / Path("static")).mkdir(exist_ok=True)
 
-        click.secho("- Create templates directory")
-        Path("templates").mkdir(exist_ok=True)
+        click.secho("- Create site/templates directory")
+        (APP_DIR / Path("templates")).mkdir(exist_ok=True)
 
     click.secho()
     click.secho("For local development: ", nl=False, fg="green")
-    click.secho("poetry run coltrane play")
+    click.secho("coltrane play")
     click.secho("Build static HTML: ", nl=False, fg="green")
-    click.secho("poetry run coltrane record")
+    click.secho("coltrane record")
 
 
 @cli.command(help="Start a local development server. Alias: serve.", aliases=["serve"])
 @click.option("--port", default=8000, help="Port to serve localhost from")
 def play(port):
     _run_management_command("runserver", f"0:{port}")
```

### Comparing `coltrane-0.34.0/coltrane/feeds.py` & `coltrane-0.35.0/coltrane/feeds.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/coltrane/management/commands/build.py` & `coltrane-0.35.0/coltrane/management/commands/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import sys
 import time
-from concurrent.futures import Future, ThreadPoolExecutor
+from concurrent.futures import ThreadPoolExecutor
 from contextlib import redirect_stdout
 from io import StringIO
 from multiprocessing import cpu_count
 from pathlib import Path
 from shutil import copy2
 from types import SimpleNamespace
 from typing import Dict, List, Optional
```

### Comparing `coltrane-0.34.0/coltrane/manifest.py` & `coltrane-0.35.0/coltrane/manifest.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/coltrane/middleware.py` & `coltrane-0.35.0/coltrane/middleware.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/coltrane/module_finder.py` & `coltrane-0.35.0/coltrane/module_finder.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/coltrane/renderer.py` & `coltrane-0.35.0/coltrane/renderer.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/coltrane/retriever.py` & `coltrane-0.35.0/coltrane/retriever.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/coltrane/templatetags/coltrane_tags.py` & `coltrane-0.35.0/coltrane/templatetags/coltrane_tags.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/coltrane/urls.py` & `coltrane-0.35.0/coltrane/urls.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/coltrane/utils.py` & `coltrane-0.35.0/coltrane/utils.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/coltrane/views.py` & `coltrane-0.35.0/coltrane/views.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.34.0/pyproject.toml` & `coltrane-0.35.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "coltrane"
 authors = [{name = "Adam Hill", email = "adam@adamghill.com"}]
 dynamic = ["version", "description"]
 
 [tool.poetry]
 name = "coltrane"
-version = "0.34.0"
+version = "0.35.0"
 description = "A minimal app framework for content sites 🎵"
 authors = ["adamghill <adam@adamghill.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["django", "python", "static", "markdown"]
 packages = [{ include = "coltrane" }]
 repository = "https://github.com/adamghill/coltrane/"
@@ -55,20 +55,21 @@
 linkify-it-py = { version = "*", optional = true }
 myst-parser = { version = "*", optional = true }
 furo = { version = "*", optional = true }
 sphinx-copybutton = { version = "*", optional = true }
 sphinx-autobuild = { version = "*", optional = true }
 toml = { version = "*", optional = true }
 attrs = { version = "*", optional = true }
+sphinx-inline-tabs = { version = "*", optional = true }
 
 [tool.poetry.extras]
 deploy = ["gunicorn", "whitenoise"]
 json5 = ["pyjson5"]
 compressor = ["django-compressor"]
-docs = ["Sphinx", "linkify-it-py", "myst-parser", "furo", "sphinx-copybutton", "sphinx-autobuild", "toml", "attrs"]
+docs = ["Sphinx", "linkify-it-py", "myst-parser", "furo", "sphinx-copybutton", "sphinx-autobuild", "toml", "attrs", "sphinx-inline-tabs"]
 
 [tool.poetry.group.development.dependencies]
 poethepoet = "*"
 ruff = "*"
 coverage = {extras = ["toml"], version = "*"}
 pytest-cov = "*"
 pytest = "*"
@@ -178,14 +179,18 @@
 script = "django.core.management.utils:get_random_secret_key()"
 print_result = true
 
 [tool.poe.tasks.r]
 cmd = "example_standalone/app.py runserver 0:8045"
 help = "Start dev server for example_standalone"
 
+[tool.poe.tasks.ri]
+cmd = "example_standalone/app.py runserver 0:8046"
+help = "Start dev server for example_integrated"
+
 [tool.poe.tasks.record]
 cmd = "coltrane record"
 cwd = "example_standalone"
 help = "Build example_standalone"
 
 [tool.poe.tasks.g]
 cmd = "gunicorn -b localhost:8045 example_standalone.app:wsgi"
```

### Comparing `coltrane-0.34.0/PKG-INFO` & `coltrane-0.35.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coltrane
-Version: 0.34.0
+Version: 0.35.0
 Summary: A minimal app framework for content sites 🎵
 Home-page: https://github.com/adamghill/coltrane/
 License: MIT
 Keywords: django,python,static,markdown
 Author: adamghill
 Author-email: adam@adamghill.com
 Requires-Python: >=3.8,<4.0
@@ -39,14 +39,15 @@
 Requires-Dist: pyjson5 ; extra == "json5"
 Requires-Dist: python-dotenv (>0.17)
 Requires-Dist: python-frontmatter (>=1,<2)
 Requires-Dist: pywatchman
 Requires-Dist: rich-click (>=1,<2)
 Requires-Dist: sphinx-autobuild ; extra == "docs"
 Requires-Dist: sphinx-copybutton ; extra == "docs"
+Requires-Dist: sphinx-inline-tabs ; extra == "docs"
 Requires-Dist: toml ; extra == "docs"
 Requires-Dist: whitenoise ; extra == "deploy"
 Project-URL: Documentation, https://coltrane.readthedocs.io/
 Project-URL: Funding, https://github.com/sponsors/adamghill
 Project-URL: Repository, https://github.com/adamghill/coltrane/
 Description-Content-Type: text/markdown
 
@@ -75,46 +76,46 @@
 - Local development server which includes [live re-rendering of markdown and data](https://twitter.com/adamghill/status/1487522925393715205) via https://github.com/adamchainz/django-browser-reload
 - Site-wide redirects
 - Deployment best practices with `whitenoise` and `gunicorn` already configured
 - Leverage the power of built-in `Django` templates, template tags, and filters inside `markdown` files
 - Any custom template tags and filters are enabled automatically for use in `markdown` or HTML templates
 - Include any third-party [`Django` app](https://djangopackages.org) for additional functionality
 - Optional command to generate static HTML files
-- Able to be integrated into a regular `Django` project as a standard third-party `Django` app
+- Can be integrated into a regular `Django` project as a standard third-party `Django` app to render markdown content
 
 ## ⚡ Quick start
 
 1. `mkdir new-site && cd new-site` to create a new folder
-1. `poetry init --no-interaction --dependency 'coltrane:<1' && poetry install` to create a new virtual environment and install the `coltrane` package
-1. Optional: `brew install watchman` on MacOS for less resource-intensive local development server
-1. `poetry run coltrane create` to create the folder structure for a new site
-1. `poetry run coltrane play` to start local development server
+1. `python3 -m venv .venv && source .venv/bin/activate && pip install coltrane` to install the `coltrane` package
+1. `coltrane create` to create the folder structure for a new site
+1. `coltrane play` to start local development server
 1. Go to http://localhost:8000 to see the original markdown rendered into HTML
 1. Update `content/index.md`
-1. Go to http://localhost:8000 to see the updated markdown rendered into HTML
-1. Optional: run `poetry run coltrane record` to build static HTML files
+1. Refresh http://localhost:8000 to see the updated markdown rendered into HTML
+1. Optional: run `coltrane record` to build static HTML files
 
 ### Generated `coltrane` file structure
 
 ```bash
 .
-├── .env
 ├── .gitignore
-├── .watchmanconfig
-├── __init__.py
-├── app.py
-├── content
-│   └── index.md
-├── data
 ├── Dockerfile
-├── gunicorn.conf.py
-├── templates
-├── poetry.lock
-└── pyproject.toml
-└── redirects.json
+├── README.md
+├── pyproject.toml
+└── site
+    ├── .env
+    ├── .watchmanconfig
+    ├── __init__.py
+    ├── app.py
+    ├── content
+    │   └── index.md
+    ├── data
+    ├── gunicorn.conf.py
+    ├── static
+    └── templates
 ```
 
 ## 📝 Content
 
 Add `markdown` files or sub-directories to the `content` directory and rendered HTML will be accessible via auto-generated routes.
 
 - `/` would render the `markdown` in `content/index.md`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coltrane Version: 0.34.0 Summary: A minimal app
+Metadata-Version: 2.1 Name: coltrane Version: 0.35.0 Summary: A minimal app
 framework for content sites ðµ Home-page: https://github.com/adamghill/
 coltrane/ License: MIT Keywords: django,python,static,markdown Author:
 adamghill Author-email: adam@adamghill.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -16,19 +16,19 @@
 == "deploy" Requires-Dist: halo (>=0,<1) Requires-Dist: linkify-it-py ; extra
 == "docs" Requires-Dist: minestrone (>=0.6.2) Requires-Dist: mistune (>=3,<4)
 Requires-Dist: msgspec (>=0,<1) Requires-Dist: myst-parser ; extra == "docs"
 Requires-Dist: pygments (>=2.7.3) Requires-Dist: pyjson5 ; extra == "json5"
 Requires-Dist: python-dotenv (>0.17) Requires-Dist: python-frontmatter (>=1,<2)
 Requires-Dist: pywatchman Requires-Dist: rich-click (>=1,<2) Requires-Dist:
 sphinx-autobuild ; extra == "docs" Requires-Dist: sphinx-copybutton ; extra ==
-"docs" Requires-Dist: toml ; extra == "docs" Requires-Dist: whitenoise ; extra
-== "deploy" Project-URL: Documentation, https://coltrane.readthedocs.io/
-Project-URL: Funding, https://github.com/sponsors/adamghill Project-URL:
-Repository, https://github.com/adamghill/coltrane/ Description-Content-Type:
-text/markdown
+"docs" Requires-Dist: sphinx-inline-tabs ; extra == "docs" Requires-Dist: toml
+; extra == "docs" Requires-Dist: whitenoise ; extra == "deploy" Project-URL:
+Documentation, https://coltrane.readthedocs.io/ Project-URL: Funding, https://
+github.com/sponsors/adamghill Project-URL: Repository, https://github.com/
+adamghill/coltrane/ Description-Content-Type: text/markdown
                             _**_**_**_**_**_**_ _cc_oo_ll_tt_rr_aa_nn_ee_ _**_**_**_**_**_**
                 A minimal app framework for content sites ðµ
 ![PyPI](https://img.shields.io/pypi/v/coltrane?color=blue&style=flat-square) !
 [PyPI - Downloads](https://img.shields.io/pypi/dm/
 coltrane?color=blue&style=flat-square) ![GitHub Sponsors](https://
 img.shields.io/github/sponsors/adamghill?color=blue&style=flat-square) ![All
 Contributors](https://img.shields.io/badge/all_contributors-1-
@@ -42,43 +42,41 @@
 twitter.com/adamghill/status/1487522925393715205) via https://github.com/
 adamchainz/django-browser-reload - Site-wide redirects - Deployment best
 practices with `whitenoise` and `gunicorn` already configured - Leverage the
 power of built-in `Django` templates, template tags, and filters inside
 `markdown` files - Any custom template tags and filters are enabled
 automatically for use in `markdown` or HTML templates - Include any third-party
 [`Django` app](https://djangopackages.org) for additional functionality -
-Optional command to generate static HTML files - Able to be integrated into a
-regular `Django` project as a standard third-party `Django` app ## â¡ Quick
-start 1. `mkdir new-site && cd new-site` to create a new folder 1. `poetry init
---no-interaction --dependency 'coltrane:<1' && poetry install` to create a new
-virtual environment and install the `coltrane` package 1. Optional: `brew
-install watchman` on MacOS for less resource-intensive local development server
-1. `poetry run coltrane create` to create the folder structure for a new site
-1. `poetry run coltrane play` to start local development server 1. Go to http:/
-/localhost:8000 to see the original markdown rendered into HTML 1. Update
-`content/index.md` 1. Go to http://localhost:8000 to see the updated markdown
-rendered into HTML 1. Optional: run `poetry run coltrane record` to build
-static HTML files ### Generated `coltrane` file structure ```bash . âââ
-.env âââ .gitignore âââ .watchmanconfig âââ __init__.py
-âââ app.py âââ content âÂ Â  âââ index.md âââ data
-âââ Dockerfile âââ gunicorn.conf.py âââ templates âââ
-poetry.lock âââ pyproject.toml âââ redirects.json ``` ## ð
-Content Add `markdown` files or sub-directories to the `content` directory and
-rendered HTML will be accessible via auto-generated routes. - `/` would render
-the `markdown` in `content/index.md` - `/about/` would render the `markdown` in
-`content/about.md` - `/articles/this-is-the-first-article/` would render the
-content from `/content/articles/this-is-the-first-article.md` - `/not-there/
-` will 404 HTML will also be served automatically if a `markdown` file can not
-be found. - `/app/` would render the HTML from `/templates/app.html` or `/
-templates/app/index.html` - `/app/some-user` would render the HTML from `/
-templates/app/*.html` ## Deployment Example `Dockerfile` and `gunicorn.conf.py`
-files are created when an app is created, and optional dependencies can be
-installed for efficient `static` serving with `whitenoise`. # ð
-Documentation Read all of the documentation at https://coltrane.readthedocs.io.
-## Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
-allcontributors.org/docs/en/emoji-key)):
+Optional command to generate static HTML files - Can be integrated into a
+regular `Django` project as a standard third-party `Django` app to render
+markdown content ## â¡ Quick start 1. `mkdir new-site && cd new-site` to
+create a new folder 1. `python3 -m venv .venv && source .venv/bin/activate &&
+pip install coltrane` to install the `coltrane` package 1. `coltrane create` to
+create the folder structure for a new site 1. `coltrane play` to start local
+development server 1. Go to http://localhost:8000 to see the original markdown
+rendered into HTML 1. Update `content/index.md` 1. Refresh http://localhost:
+8000 to see the updated markdown rendered into HTML 1. Optional: run `coltrane
+record` to build static HTML files ### Generated `coltrane` file structure
+```bash . âââ .gitignore âââ Dockerfile âââ README.md
+âââ pyproject.toml âââ site âââ .env âââ
+.watchmanconfig âââ __init__.py âââ app.py âââ content
+âÂ Â  âââ index.md âââ data âââ gunicorn.conf.py âââ
+static âââ templates ``` ## ð Content Add `markdown` files or sub-
+directories to the `content` directory and rendered HTML will be accessible via
+auto-generated routes. - `/` would render the `markdown` in `content/index.md`
+- `/about/` would render the `markdown` in `content/about.md` - `/articles/
+this-is-the-first-article/` would render the content from `/content/articles/
+this-is-the-first-article.md` - `/not-there/` will 404 HTML will also be served
+automatically if a `markdown` file can not be found. - `/app/` would render the
+HTML from `/templates/app.html` or `/templates/app/index.html` - `/app/some-
+user` would render the HTML from `/templates/app/*.html` ## Deployment Example
+`Dockerfile` and `gunicorn.conf.py` files are created when an app is created,
+and optional dependencies can be installed for efficient `static` serving with
+`whitenoise`. # ð Documentation Read all of the documentation at https://
+coltrane.readthedocs.io. ## Contributors â¨ Thanks goes to these wonderful
+people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 _[_T_o_b_i_ _D_E_G_N_O_N_]
  _TT_oo_bb_ii_ _DD_EE_GG_NN_OO_NN
  _â__ _ï_¸_ _ð___»
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

