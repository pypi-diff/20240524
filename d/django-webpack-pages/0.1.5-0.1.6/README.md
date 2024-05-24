# Comparing `tmp/django_webpack_pages-0.1.5.tar.gz` & `tmp/django_webpack_pages-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_webpack_pages-0.1.5.tar", max compression
+gzip compressed data, was "django_webpack_pages-0.1.6.tar", max compression
```

## Comparing `django_webpack_pages-0.1.5.tar` & `django_webpack_pages-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2335 2022-05-15 17:18:34.832700 django_webpack_pages-0.1.5/README.md
--rw-r--r--   0        0        0     1111 2024-03-26 08:18:25.844662 django_webpack_pages-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-14 09:23:50.202822 django_webpack_pages-0.1.5/webpack_pages/__init__.py
--rw-r--r--   0        0        0      804 2024-03-26 06:12:44.036383 django_webpack_pages-0.1.5/webpack_pages/jinja2ext.py
--rw-r--r--   0        0        0     2829 2024-03-26 06:12:44.036383 django_webpack_pages-0.1.5/webpack_pages/pageassetfinder.py
--rw-r--r--   0        0        0     5012 2024-03-26 08:16:44.813003 django_webpack_pages-0.1.5/webpack_pages/templatetags.py
--rw-r--r--   0        0        0      210 2022-05-14 10:38:52.903315 django_webpack_pages-0.1.5/webpack_pages/utils.py
--rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 django_webpack_pages-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2335 2022-05-15 17:18:34.832700 django_webpack_pages-0.1.6/README.md
+-rw-r--r--   0        0        0     1111 2024-05-24 17:28:00.830779 django_webpack_pages-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-05-14 09:23:50.202822 django_webpack_pages-0.1.6/webpack_pages/__init__.py
+-rw-r--r--   0        0        0      804 2024-03-26 06:12:44.036383 django_webpack_pages-0.1.6/webpack_pages/jinja2ext.py
+-rw-r--r--   0        0        0     2829 2024-03-26 06:12:44.036383 django_webpack_pages-0.1.6/webpack_pages/pageassetfinder.py
+-rw-r--r--   0        0        0     5121 2024-05-24 17:27:13.378698 django_webpack_pages-0.1.6/webpack_pages/templatetags.py
+-rw-r--r--   0        0        0      578 2024-05-24 17:26:36.510638 django_webpack_pages-0.1.6/webpack_pages/utils.py
+-rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 django_webpack_pages-0.1.6/PKG-INFO
```

### Comparing `django_webpack_pages-0.1.5/README.md` & `django_webpack_pages-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `django_webpack_pages-0.1.5/pyproject.toml` & `django_webpack_pages-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "django-webpack-pages"
-version = "0.1.5"
+version = "0.1.6"
 description = "Use webpack with your multi-page, multi-lingual django webapp"
 authors = ["MrP01 <peter@waldert.at>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/MrP01/django-webpack-pages"
 keywords = ["django", "webpack", "assets"]
 packages = [{ include = "webpack_pages" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-django-webpack-loader = "^3.0.1"
-Django = "^5.0.3"
-Jinja2 = "^3.1.3"
+django-webpack-loader = "^3.1.0"
+Django = "^5.0.6"
+Jinja2 = "^3.1.4"
 
 [tool.poetry.group.dev.dependencies]
-pylint = "^3.1.0"
+pylint = "^3.2.2"
 
 [tool.nitpick]
 style = [
   "github://MrP01/lint-me-now/nitpick-base-style.toml",
   "github://MrP01/lint-me-now/nitpick-python-style.toml",
 ]
```

### Comparing `django_webpack_pages-0.1.5/webpack_pages/jinja2ext.py` & `django_webpack_pages-0.1.6/webpack_pages/jinja2ext.py`

 * *Files identical despite different names*

### Comparing `django_webpack_pages-0.1.5/webpack_pages/pageassetfinder.py` & `django_webpack_pages-0.1.6/webpack_pages/pageassetfinder.py`

 * *Files identical despite different names*

### Comparing `django_webpack_pages-0.1.5/webpack_pages/templatetags.py` & `django_webpack_pages-0.1.6/webpack_pages/templatetags.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from django.conf import settings
 from django.contrib.staticfiles import finders
 from django.utils import translation
 from django.utils.safestring import mark_safe
 from webpack_loader.utils import get_files
 
 from .pageassetfinder import PageAssetFinder
-from .utils import is_first_visit
+from .utils import is_first_visit, conditional_decorator
 
 register = template.Library()
 
 
 def get_unique_files(entrypoints, extension, config):
     """For multiple entrypoints (or bundles), scans through their files and deduplicates them."""
     if settings.WEBPACK_PAGES["STRATEGY"] == "ACCRUE":
@@ -73,22 +73,22 @@
 @register.simple_tag(takes_context=True)
 def render_js(context, config="DEFAULT"):
     """Similar to render_css, but for JavaScript."""
     files = get_unique_files(getattr(context, "webpack_entrypoints", []), "js", config)
     return mark_safe("".join(f"<script src='{file['url']}'></script>" for file in files))
 
 
-@functools.lru_cache()
+@conditional_decorator(functools.lru_cache(), not settings.DEBUG)
 def inline_static_file(path):
     """Plain static file inlining utility, with caching"""
     with open(finders.find(path), encoding="utf-8") as f:  # type: ignore
         return mark_safe(f.read())
 
 
-@functools.lru_cache()
+@conditional_decorator(functools.lru_cache(), not settings.DEBUG)
 def inline_entrypoint(entrypoint, extension, config="DEFAULT"):
     """Inlines all files of an entrypoint directly (i.e. returns a string)"""
     inlined = ""
     base = settings.WEBPACK_PAGES["STATICFILE_BUNDLES_BASE"].format(locale=translation.get_language())
     for file in get_unique_files((entrypoint,), extension, config=config):
         with open(finders.find(base + file["name"]), encoding="utf-8") as f:  # type: ignore
             inlined += f.read()
```

### Comparing `django_webpack_pages-0.1.5/PKG-INFO` & `django_webpack_pages-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: django-webpack-pages
-Version: 0.1.5
+Version: 0.1.6
 Summary: Use webpack with your multi-page, multi-lingual django webapp
 Home-page: https://github.com/MrP01/django-webpack-pages
 License: MIT
 Keywords: django,webpack,assets
 Author: MrP01
 Author-email: peter@waldert.at
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: Django (>=5.0.3,<6.0.0)
-Requires-Dist: Jinja2 (>=3.1.3,<4.0.0)
-Requires-Dist: django-webpack-loader (>=3.0.1,<4.0.0)
+Requires-Dist: Django (>=5.0.6,<6.0.0)
+Requires-Dist: Jinja2 (>=3.1.4,<4.0.0)
+Requires-Dist: django-webpack-loader (>=3.1.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # django-webpack-pages
 
 [![PyPI version](https://badge.fury.io/py/django-webpack-pages.svg)](https://pypi.org/project/django-webpack-pages/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: django-webpack-pages Version: 0.1.5 Summary: Use
+Metadata-Version: 2.1 Name: django-webpack-pages Version: 0.1.6 Summary: Use
 webpack with your multi-page, multi-lingual django webapp Home-page: https://
 github.com/MrP01/django-webpack-pages License: MIT Keywords:
 django,webpack,assets Author: MrP01 Author-email: peter@waldert.at Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: Django
-(>=5.0.3,<6.0.0) Requires-Dist: Jinja2 (>=3.1.3,<4.0.0) Requires-Dist: django-
-webpack-loader (>=3.0.1,<4.0.0) Description-Content-Type: text/markdown #
+(>=5.0.6,<6.0.0) Requires-Dist: Jinja2 (>=3.1.4,<4.0.0) Requires-Dist: django-
+webpack-loader (>=3.1.0,<4.0.0) Description-Content-Type: text/markdown #
 django-webpack-pages [![PyPI version](https://badge.fury.io/py/django-webpack-
 pages.svg)](https://pypi.org/project/django-webpack-pages/) [![Code style:
 black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/psf/black) Use webpack with your multi-page, multi-lingual django
 webapp. This project is based on [django-webpack-loader](https://pypi.org/
 project/django-webpack-loader/) which handles the connection to webpack.
 Consider using [webpack-critical-pages](https://www.npmjs.com/package/webpack-
```

