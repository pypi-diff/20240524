# Comparing `tmp/sunpy-sphinx-theme-2.0.8rc2.tar.gz` & `tmp/sunpy-sphinx-theme-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunpy-sphinx-theme-2.0.8rc2.tar", last modified: Sat Apr  6 20:02:53 2024, max compression
+gzip compressed data, was "sunpy-sphinx-theme-2.0.9.tar", last modified: Fri Apr 12 15:07:53 2024, max compression
```

## Comparing `sunpy-sphinx-theme-2.0.8rc2.tar` & `sunpy-sphinx-theme-2.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.689839 sunpy-sphinx-theme-2.0.8rc2/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/.rtd-environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/.stylelintrc.json
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-06 20:02:53.689839 sunpy-sphinx-theme-2.0.8rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-06 20:02:53.689839 sunpy-sphinx-theme-2.0.8rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.681840 sunpy-sphinx-theme-2.0.8rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.681840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.681840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.685840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.685840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/built-with.html
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/footer-links.html
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/navbar-logo.html
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_center.html
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_start.html
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/sst-sidebar-nav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.685840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/sections/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/sections/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.685840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.685840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/favicon-32.ico
--rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/numfocus-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   187674 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy-bg.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    15708 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon_128x128.png
--rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/sunpy_style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.685840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-06 20:02:53.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-06 20:02:53.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:02:53.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-06 20:02:53.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-06 20:02:53.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 20:02:53.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:07:53.949781 sunpy-sphinx-theme-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/.rtd-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/.stylelintrc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-12 15:07:53.949781 sunpy-sphinx-theme-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-12 15:07:53.949781 sunpy-sphinx-theme-2.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:07:53.941781 sunpy-sphinx-theme-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:07:53.945781 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:07:53.941781 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:07:53.945781 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:07:53.945781 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/components/built-with.html
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/components/footer-links.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/components/navbar-logo.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_center.html
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_start.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/components/sst-sidebar-nav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:07:53.945781 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/sections/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:07:53.949781 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:07:53.949781 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/img/favicon-32.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/img/numfocus-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   187674 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy-bg.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    15708 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon_128x128.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/sunpy_style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-12 15:07:40.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:07:53.949781 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-12 15:07:53.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-12 15:07:53.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:07:53.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 15:07:53.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 15:07:53.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 15:07:53.000000 sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme.egg-info/top_level.txt
```

### Comparing `sunpy-sphinx-theme-2.0.8rc2/LICENSE.md` & `sunpy-sphinx-theme-2.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/PKG-INFO` & `sunpy-sphinx-theme-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpy-sphinx-theme
-Version: 2.0.8rc2
+Version: 2.0.9
 Summary: The sphinx theme for the SunPy website and documentation.
 Author: The SunPy Developers
 License: BSD 2-Clause License
         
         Copyright (c) 2018-2023, The SunPy Developers
         All rights reserved.
```

### Comparing `sunpy-sphinx-theme-2.0.8rc2/README.md` & `sunpy-sphinx-theme-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/pyproject.toml` & `sunpy-sphinx-theme-2.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/__init__.py` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 
 
 def default_navbar():
     return [
         (
             "About",
             [
-                ("Our Mission", "about/index.html", 2),
-                ("SunPy Project", "about/project.html", 2),
-                ("Presentations", "about/presentations.html", 2),
-                ("Community Roles", "about/roles.html", 2),
-                ("Meetings", "about/meetings.html", 2),
-                ("Code of Conduct", "coc.html", 2),
+                ("Our Mission", "about/", 2),
+                ("SunPy Project", "about/project/", 2),
+                ("Presentations", "about/presentations/", 2),
+                ("Community Roles", "about/roles/", 2),
+                ("Meetings", "about/meetings/", 2),
+                ("Code of Conduct", "coc/", 2),
             ],
         ),
         (
             "Documentation",
             [
                 ("sunpy", "https://docs.sunpy.org/", 3),
                 ("ndcube", "https://docs.sunpy.org/projects/ndcube/", 3),
@@ -48,18 +48,18 @@
                 ("sunraster", "https://docs.sunpy.org/projects/sunraster/", 3),
                 ("sunpy-soar", "https://docs.sunpy.org/projects/soar/", 3),
                 ("roentgen", "https://roentgen.readthedocs.io/", 3),
                 ("demcmc", "https://demcmc.readthedocs.io/en/latest/", 3),
                 ("dkist", "https://docs.dkist.nso.edu/projects/python-tools", 3),
             ],
         ),
-        ("Affiliated Packages", "affiliated.html", 2),
-        ("Get Help", "help.html", 2),
-        ("Contribute", "contribute.html", 2),
-        ("Blog", "blog.html", 2),
+        ("Affiliated Packages", "affiliated/", 2),
+        ("Get Help", "help/", 2),
+        ("Contribute", "contribute/", 2),
+        ("Blog", "blog/", 2),
     ]
 
 
 def update_config(app):
     """
     Update config with new default values and handle deprecated keys.
     """
```

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/conf.py` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/conf.py`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/built-with.html` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/components/built-with.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/navbar-logo.html` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/components/navbar-logo.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_center.html` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_center.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_start.html` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_start.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/sst-sidebar-nav.html` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/components/sst-sidebar-nav.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/favicon-32.ico` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/img/favicon-32.ico`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/numfocus-logo.svg` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/img/numfocus-logo.svg`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy-bg.jpg` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy-bg.jpg`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon.svg` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon.svg`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon_128x128.png` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon_128x128.png`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/sunpy_style.css` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/static/sunpy_style.css`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/theme.conf` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme/theme/sunpy/theme.conf`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/PKG-INFO` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpy-sphinx-theme
-Version: 2.0.8rc2
+Version: 2.0.9
 Summary: The sphinx theme for the SunPy website and documentation.
 Author: The SunPy Developers
 License: BSD 2-Clause License
         
         Copyright (c) 2018-2023, The SunPy Developers
         All rights reserved.
```

### Comparing `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/SOURCES.txt` & `sunpy-sphinx-theme-2.0.9/src/sunpy_sphinx_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

