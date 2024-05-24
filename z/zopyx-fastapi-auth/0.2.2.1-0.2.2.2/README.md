# Comparing `tmp/zopyx_fastapi_auth-0.2.2.1.tar.gz` & `tmp/zopyx_fastapi_auth-0.2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zopyx_fastapi_auth-0.2.2.1.tar", last modified: Fri May 24 04:56:50 2024, max compression
+gzip compressed data, was "zopyx_fastapi_auth-0.2.2.2.tar", last modified: Fri May 24 05:36:29 2024, max compression
```

## Comparing `zopyx_fastapi_auth-0.2.2.1.tar` & `zopyx_fastapi_auth-0.2.2.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:56:50.493297 zopyx_fastapi_auth-0.2.2.1/
--rw-------   0 ajung     (1000) ajung     (1000)       98 2024-05-24 04:56:20.000000 zopyx_fastapi_auth-0.2.2.1/MANIFEST.in
--rw-r--r--   0 ajung     (1000) ajung     (1000)     6844 2024-05-24 04:56:50.493297 zopyx_fastapi_auth-0.2.2.1/PKG-INFO
--rw-------   0 ajung     (1000) ajung     (1000)     5788 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/README.md
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:56:50.485297 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/
--rw-------   0 ajung     (1000) ajung     (1000)       14 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/__init__.py
--rw-------   0 ajung     (1000) ajung     (1000)      347 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/auth_config.py
--rw-------   0 ajung     (1000) ajung     (1000)     2122 2024-05-24 04:50:07.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/auth_routes.py
--rw-------   0 ajung     (1000) ajung     (1000)     3008 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/demo_app.py
--rw-------   0 ajung     (1000) ajung     (1000)     2465 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/dependencies.py
--rw-------   0 ajung     (1000) ajung     (1000)      290 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/jinja2_templates.py
--rw-------   0 ajung     (1000) ajung     (1000)      106 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/logger.py
--rw-------   0 ajung     (1000) ajung     (1000)      294 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/permissions.py
--rw-------   0 ajung     (1000) ajung     (1000)     1716 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/roles.py
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:56:50.485297 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/templates/
--rw-------   0 ajung     (1000) ajung     (1000)     1408 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/templates/base.html
--rw-------   0 ajung     (1000) ajung     (1000)      564 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/templates/demo.html
--rw-------   0 ajung     (1000) ajung     (1000)      881 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/templates/login.html
--rw-------   0 ajung     (1000) ajung     (1000)     1899 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/user_cmd.py
--rw-------   0 ajung     (1000) ajung     (1000)     4422 2024-05-24 04:51:00.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/user_management_sqlobject.py
--rw-------   0 ajung     (1000) ajung     (1000)     1356 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/fastapi_auth/users.py
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:56:50.485297 zopyx_fastapi_auth-0.2.2.1/images/
--rw-------   0 ajung     (1000) ajung     (1000)   172868 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/images/logged-in.png
--rw-------   0 ajung     (1000) ajung     (1000)    86854 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/images/login.png
--rw-------   0 ajung     (1000) ajung     (1000)     1143 2024-05-24 04:56:35.000000 zopyx_fastapi_auth-0.2.2.1/pyproject.toml
--rw-------   0 ajung     (1000) ajung     (1000)       38 2024-05-24 04:56:50.493297 zopyx_fastapi_auth-0.2.2.1/setup.cfg
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:56:50.481297 zopyx_fastapi_auth-0.2.2.1/static/
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:56:50.481297 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:56:50.489297 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/
--rw-------   0 ajung     (1000) ajung     (1000)    70329 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css
--rw-------   0 ajung     (1000) ajung     (1000)   203221 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    51795 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   115986 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    70403 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css
--rw-------   0 ajung     (1000) ajung     (1000)   203225 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    51870 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   116063 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    12065 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css
--rw-------   0 ajung     (1000) ajung     (1000)   129371 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    10126 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css
--rw-------   0 ajung     (1000) ajung     (1000)    51369 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    12058 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css
--rw-------   0 ajung     (1000) ajung     (1000)   129386 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    10198 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css
--rw-------   0 ajung     (1000) ajung     (1000)    63943 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   107823 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css
--rw-------   0 ajung     (1000) ajung     (1000)   267535 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    85352 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   180381 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   107691 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css
--rw-------   0 ajung     (1000) ajung     (1000)   267476 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    85281 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   180217 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   281046 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.css
--rw-------   0 ajung     (1000) ajung     (1000)   679755 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   232803 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   589892 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   280259 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css
--rw-------   0 ajung     (1000) ajung     (1000)   679615 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   232911 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   589087 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:56:50.489297 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/
--rw-------   0 ajung     (1000) ajung     (1000)   207819 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js
--rw-------   0 ajung     (1000) ajung     (1000)   444579 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map
--rw-------   0 ajung     (1000) ajung     (1000)    80721 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js
--rw-------   0 ajung     (1000) ajung     (1000)   332090 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map
--rw-------   0 ajung     (1000) ajung     (1000)   135829 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js
--rw-------   0 ajung     (1000) ajung     (1000)   305438 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map
--rw-------   0 ajung     (1000) ajung     (1000)    73935 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js
--rw-------   0 ajung     (1000) ajung     (1000)   222455 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map
--rw-------   0 ajung     (1000) ajung     (1000)   145401 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.js
--rw-------   0 ajung     (1000) ajung     (1000)   306606 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.js.map
--rw-------   0 ajung     (1000) ajung     (1000)    60635 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js
--rw-------   0 ajung     (1000) ajung     (1000)   220561 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:56:50.493297 zopyx_fastapi_auth-0.2.2.1/zopyx_fastapi_auth.egg-info/
--rw-r--r--   0 ajung     (1000) ajung     (1000)     6844 2024-05-24 04:56:50.000000 zopyx_fastapi_auth-0.2.2.1/zopyx_fastapi_auth.egg-info/PKG-INFO
--rw-------   0 ajung     (1000) ajung     (1000)     3218 2024-05-24 04:56:50.000000 zopyx_fastapi_auth-0.2.2.1/zopyx_fastapi_auth.egg-info/SOURCES.txt
--rw-------   0 ajung     (1000) ajung     (1000)        1 2024-05-24 04:56:50.000000 zopyx_fastapi_auth-0.2.2.1/zopyx_fastapi_auth.egg-info/dependency_links.txt
--rw-------   0 ajung     (1000) ajung     (1000)       71 2024-05-24 04:56:50.000000 zopyx_fastapi_auth-0.2.2.1/zopyx_fastapi_auth.egg-info/entry_points.txt
--rw-------   0 ajung     (1000) ajung     (1000)      184 2024-05-24 04:56:50.000000 zopyx_fastapi_auth-0.2.2.1/zopyx_fastapi_auth.egg-info/requires.txt
--rw-------   0 ajung     (1000) ajung     (1000)       13 2024-05-24 04:56:50.000000 zopyx_fastapi_auth-0.2.2.1/zopyx_fastapi_auth.egg-info/top_level.txt
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 05:36:29.063672 zopyx_fastapi_auth-0.2.2.2/
+-rw-------   0 ajung     (1000) ajung     (1000)       98 2024-05-24 04:56:20.000000 zopyx_fastapi_auth-0.2.2.2/MANIFEST.in
+-rw-r--r--   0 ajung     (1000) ajung     (1000)     6844 2024-05-24 05:36:29.063672 zopyx_fastapi_auth-0.2.2.2/PKG-INFO
+-rw-------   0 ajung     (1000) ajung     (1000)     5788 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/README.md
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 05:36:29.047672 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/
+-rw-------   0 ajung     (1000) ajung     (1000)       14 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/__init__.py
+-rw-------   0 ajung     (1000) ajung     (1000)      347 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/auth_config.py
+-rw-------   0 ajung     (1000) ajung     (1000)     2122 2024-05-24 04:50:07.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/auth_routes.py
+-rw-------   0 ajung     (1000) ajung     (1000)     3008 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/demo_app.py
+-rw-------   0 ajung     (1000) ajung     (1000)     2465 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/dependencies.py
+-rw-------   0 ajung     (1000) ajung     (1000)      290 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/jinja2_templates.py
+-rw-------   0 ajung     (1000) ajung     (1000)      106 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/logger.py
+-rw-------   0 ajung     (1000) ajung     (1000)      294 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/permissions.py
+-rw-------   0 ajung     (1000) ajung     (1000)     1716 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/roles.py
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 05:36:29.047672 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/templates/
+-rw-------   0 ajung     (1000) ajung     (1000)     1408 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/templates/base.html
+-rw-------   0 ajung     (1000) ajung     (1000)      564 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/templates/demo.html
+-rw-------   0 ajung     (1000) ajung     (1000)      881 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/templates/login.html
+-rw-------   0 ajung     (1000) ajung     (1000)     1899 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/user_cmd.py
+-rw-------   0 ajung     (1000) ajung     (1000)     4422 2024-05-24 04:51:00.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/user_management_sqlobject.py
+-rw-------   0 ajung     (1000) ajung     (1000)     1615 2024-05-24 05:35:02.000000 zopyx_fastapi_auth-0.2.2.2/fastapi_auth/users.py
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 05:36:29.047672 zopyx_fastapi_auth-0.2.2.2/images/
+-rw-------   0 ajung     (1000) ajung     (1000)   172868 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/images/logged-in.png
+-rw-------   0 ajung     (1000) ajung     (1000)    86854 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/images/login.png
+-rw-------   0 ajung     (1000) ajung     (1000)     1143 2024-05-24 05:36:11.000000 zopyx_fastapi_auth-0.2.2.2/pyproject.toml
+-rw-------   0 ajung     (1000) ajung     (1000)       38 2024-05-24 05:36:29.063672 zopyx_fastapi_auth-0.2.2.2/setup.cfg
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 05:36:29.043672 zopyx_fastapi_auth-0.2.2.2/static/
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 05:36:29.043672 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 05:36:29.059672 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/
+-rw-------   0 ajung     (1000) ajung     (1000)    70329 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css
+-rw-------   0 ajung     (1000) ajung     (1000)   203221 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    51795 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   115986 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    70403 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css
+-rw-------   0 ajung     (1000) ajung     (1000)   203225 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    51870 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   116063 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    12065 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css
+-rw-------   0 ajung     (1000) ajung     (1000)   129371 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    10126 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)    51369 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    12058 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css
+-rw-------   0 ajung     (1000) ajung     (1000)   129386 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    10198 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)    63943 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   107823 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css
+-rw-------   0 ajung     (1000) ajung     (1000)   267535 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    85352 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   180381 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   107691 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css
+-rw-------   0 ajung     (1000) ajung     (1000)   267476 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    85281 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   180217 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   281046 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.css
+-rw-------   0 ajung     (1000) ajung     (1000)   679755 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   232803 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   589892 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   280259 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css
+-rw-------   0 ajung     (1000) ajung     (1000)   679615 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   232911 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   589087 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 05:36:29.059672 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/
+-rw-------   0 ajung     (1000) ajung     (1000)   207819 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js
+-rw-------   0 ajung     (1000) ajung     (1000)   444579 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)    80721 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js
+-rw-------   0 ajung     (1000) ajung     (1000)   332090 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)   135829 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js
+-rw-------   0 ajung     (1000) ajung     (1000)   305438 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)    73935 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js
+-rw-------   0 ajung     (1000) ajung     (1000)   222455 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)   145401 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.js
+-rw-------   0 ajung     (1000) ajung     (1000)   306606 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)    60635 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.min.js
+-rw-------   0 ajung     (1000) ajung     (1000)   220561 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 05:36:29.063672 zopyx_fastapi_auth-0.2.2.2/zopyx_fastapi_auth.egg-info/
+-rw-r--r--   0 ajung     (1000) ajung     (1000)     6844 2024-05-24 05:36:29.000000 zopyx_fastapi_auth-0.2.2.2/zopyx_fastapi_auth.egg-info/PKG-INFO
+-rw-------   0 ajung     (1000) ajung     (1000)     3218 2024-05-24 05:36:29.000000 zopyx_fastapi_auth-0.2.2.2/zopyx_fastapi_auth.egg-info/SOURCES.txt
+-rw-------   0 ajung     (1000) ajung     (1000)        1 2024-05-24 05:36:29.000000 zopyx_fastapi_auth-0.2.2.2/zopyx_fastapi_auth.egg-info/dependency_links.txt
+-rw-------   0 ajung     (1000) ajung     (1000)       71 2024-05-24 05:36:29.000000 zopyx_fastapi_auth-0.2.2.2/zopyx_fastapi_auth.egg-info/entry_points.txt
+-rw-------   0 ajung     (1000) ajung     (1000)      184 2024-05-24 05:36:29.000000 zopyx_fastapi_auth-0.2.2.2/zopyx_fastapi_auth.egg-info/requires.txt
+-rw-------   0 ajung     (1000) ajung     (1000)       13 2024-05-24 05:36:29.000000 zopyx_fastapi_auth-0.2.2.2/zopyx_fastapi_auth.egg-info/top_level.txt
```

### Comparing `zopyx_fastapi_auth-0.2.2.1/PKG-INFO` & `zopyx_fastapi_auth-0.2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zopyx-fastapi-auth
-Version: 0.2.2.1
+Version: 0.2.2.2
 Summary: FastAPI authentication and authorization
 Author-email: Andreas Jung <info@zopyx.com>
 Project-URL: homepage, https://github.com/zopyx/fastapi-auth
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `zopyx_fastapi_auth-0.2.2.1/README.md` & `zopyx_fastapi_auth-0.2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/fastapi_auth/auth_routes.py` & `zopyx_fastapi_auth-0.2.2.2/fastapi_auth/auth_routes.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/fastapi_auth/demo_app.py` & `zopyx_fastapi_auth-0.2.2.2/fastapi_auth/demo_app.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/fastapi_auth/dependencies.py` & `zopyx_fastapi_auth-0.2.2.2/fastapi_auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/fastapi_auth/roles.py` & `zopyx_fastapi_auth-0.2.2.2/fastapi_auth/roles.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/fastapi_auth/templates/base.html` & `zopyx_fastapi_auth-0.2.2.2/fastapi_auth/templates/base.html`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/fastapi_auth/templates/demo.html` & `zopyx_fastapi_auth-0.2.2.2/fastapi_auth/templates/demo.html`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/fastapi_auth/templates/login.html` & `zopyx_fastapi_auth-0.2.2.2/fastapi_auth/templates/login.html`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/fastapi_auth/user_cmd.py` & `zopyx_fastapi_auth-0.2.2.2/fastapi_auth/user_cmd.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/fastapi_auth/user_management_sqlobject.py` & `zopyx_fastapi_auth-0.2.2.2/fastapi_auth/user_management_sqlobject.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/fastapi_auth/users.py` & `zopyx_fastapi_auth-0.2.2.2/fastapi_auth/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,22 @@
 
     @typechecked
     def has_role(self, role: Role) -> bool:
         """Check if the user has the required role."""
         return role in self.roles
 
     @typechecked
+    def has_role_by_name(self, role_name: str) -> bool:
+        """Check if the user has the required role (by name)."""
+        for role in self.roles:
+            if role.name == role_name:
+                return True
+        return False
+
+    @typechecked
     def has_permission(self, permission: Permission) -> bool:
         """Check if the user has the required permission."""
         for role in self.roles:
             if permission in role.permissions:
                 return True
         return False
```

### Comparing `zopyx_fastapi_auth-0.2.2.1/images/logged-in.png` & `zopyx_fastapi_auth-0.2.2.2/images/logged-in.png`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/images/login.png` & `zopyx_fastapi_auth-0.2.2.2/images/login.png`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/pyproject.toml` & `zopyx_fastapi_auth-0.2.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "zopyx-fastapi-auth"
 description = "FastAPI authentication and authorization"
-version = "0.2.2.1"
+version = "0.2.2.2"
 readme = "README.md"
 authors = [
     { name = "Andreas Jung", email = "info@zopyx.com" }
 ]
 classifiers = [
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.js` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.js.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map` & `zopyx_fastapi_auth-0.2.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.1/zopyx_fastapi_auth.egg-info/PKG-INFO` & `zopyx_fastapi_auth-0.2.2.2/zopyx_fastapi_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zopyx-fastapi-auth
-Version: 0.2.2.1
+Version: 0.2.2.2
 Summary: FastAPI authentication and authorization
 Author-email: Andreas Jung <info@zopyx.com>
 Project-URL: homepage, https://github.com/zopyx/fastapi-auth
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `zopyx_fastapi_auth-0.2.2.1/zopyx_fastapi_auth.egg-info/SOURCES.txt` & `zopyx_fastapi_auth-0.2.2.2/zopyx_fastapi_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

