# Comparing `tmp/zopyx_fastapi_auth-0.2.1.tar.gz` & `tmp/zopyx_fastapi_auth-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zopyx_fastapi_auth-0.2.1.tar", last modified: Thu May 23 10:39:30 2024, max compression
+gzip compressed data, was "zopyx_fastapi_auth-0.2.2.tar", last modified: Fri May 24 04:51:31 2024, max compression
```

## Comparing `zopyx_fastapi_auth-0.2.1.tar` & `zopyx_fastapi_auth-0.2.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:39:30.848186 zopyx_fastapi_auth-0.2.1/
--rw-------   0 ajung     (1000) ajung     (1000)       27 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/MANIFEST.in
--rw-r--r--   0 ajung     (1000) ajung     (1000)     5195 2024-05-23 10:39:30.848186 zopyx_fastapi_auth-0.2.1/PKG-INFO
--rw-------   0 ajung     (1000) ajung     (1000)     4183 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/README.md
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:39:30.840186 zopyx_fastapi_auth-0.2.1/fastapi_auth/
--rw-------   0 ajung     (1000) ajung     (1000)       14 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/fastapi_auth/__init__.py
--rw-------   0 ajung     (1000) ajung     (1000)      336 2024-05-23 09:47:35.000000 zopyx_fastapi_auth-0.2.1/fastapi_auth/auth_config.py
--rw-------   0 ajung     (1000) ajung     (1000)     2856 2024-05-23 09:44:02.000000 zopyx_fastapi_auth-0.2.1/fastapi_auth/auth_routes.py
--rw-------   0 ajung     (1000) ajung     (1000)     3008 2024-05-23 09:24:56.000000 zopyx_fastapi_auth-0.2.1/fastapi_auth/demo_app.py
--rw-------   0 ajung     (1000) ajung     (1000)     2465 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/fastapi_auth/dependencies.py
--rw-------   0 ajung     (1000) ajung     (1000)      290 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/fastapi_auth/jinja2_templates.py
--rw-------   0 ajung     (1000) ajung     (1000)      106 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/fastapi_auth/logger.py
--rw-------   0 ajung     (1000) ajung     (1000)      294 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/fastapi_auth/permissions.py
--rw-------   0 ajung     (1000) ajung     (1000)     1716 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/fastapi_auth/roles.py
--rw-------   0 ajung     (1000) ajung     (1000)     2163 2024-05-23 09:54:30.000000 zopyx_fastapi_auth-0.2.1/fastapi_auth/user_cmd.py
--rw-------   0 ajung     (1000) ajung     (1000)     2778 2024-05-23 09:57:10.000000 zopyx_fastapi_auth-0.2.1/fastapi_auth/user_management_sqlobject.py
--rw-------   0 ajung     (1000) ajung     (1000)     1242 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/fastapi_auth/users.py
--rw-------   0 ajung     (1000) ajung     (1000)     1123 2024-05-23 10:39:24.000000 zopyx_fastapi_auth-0.2.1/pyproject.toml
--rw-------   0 ajung     (1000) ajung     (1000)       38 2024-05-23 10:39:30.848186 zopyx_fastapi_auth-0.2.1/setup.cfg
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:39:30.840186 zopyx_fastapi_auth-0.2.1/static/
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:39:30.840186 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:39:30.844186 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/
--rw-------   0 ajung     (1000) ajung     (1000)    70329 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css
--rw-------   0 ajung     (1000) ajung     (1000)   203221 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    51795 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   115986 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    70403 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css
--rw-------   0 ajung     (1000) ajung     (1000)   203225 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    51870 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   116063 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    12065 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css
--rw-------   0 ajung     (1000) ajung     (1000)   129371 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    10126 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css
--rw-------   0 ajung     (1000) ajung     (1000)    51369 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    12058 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css
--rw-------   0 ajung     (1000) ajung     (1000)   129386 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    10198 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css
--rw-------   0 ajung     (1000) ajung     (1000)    63943 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   107823 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css
--rw-------   0 ajung     (1000) ajung     (1000)   267535 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    85352 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   180381 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   107691 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css
--rw-------   0 ajung     (1000) ajung     (1000)   267476 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    85281 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   180217 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   281046 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.css
--rw-------   0 ajung     (1000) ajung     (1000)   679755 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   232803 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   589892 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   280259 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css
--rw-------   0 ajung     (1000) ajung     (1000)   679615 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   232911 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   589087 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:39:30.848186 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/
--rw-------   0 ajung     (1000) ajung     (1000)   207819 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js
--rw-------   0 ajung     (1000) ajung     (1000)   444579 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map
--rw-------   0 ajung     (1000) ajung     (1000)    80721 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js
--rw-------   0 ajung     (1000) ajung     (1000)   332090 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map
--rw-------   0 ajung     (1000) ajung     (1000)   135829 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js
--rw-------   0 ajung     (1000) ajung     (1000)   305438 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map
--rw-------   0 ajung     (1000) ajung     (1000)    73935 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js
--rw-------   0 ajung     (1000) ajung     (1000)   222455 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map
--rw-------   0 ajung     (1000) ajung     (1000)   145401 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.js
--rw-------   0 ajung     (1000) ajung     (1000)   306606 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.js.map
--rw-------   0 ajung     (1000) ajung     (1000)    60635 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js
--rw-------   0 ajung     (1000) ajung     (1000)   220561 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:39:30.848186 zopyx_fastapi_auth-0.2.1/zopyx_fastapi_auth.egg-info/
--rw-r--r--   0 ajung     (1000) ajung     (1000)     5195 2024-05-23 10:39:30.000000 zopyx_fastapi_auth-0.2.1/zopyx_fastapi_auth.egg-info/PKG-INFO
--rw-------   0 ajung     (1000) ajung     (1000)     3080 2024-05-23 10:39:30.000000 zopyx_fastapi_auth-0.2.1/zopyx_fastapi_auth.egg-info/SOURCES.txt
--rw-------   0 ajung     (1000) ajung     (1000)        1 2024-05-23 10:39:30.000000 zopyx_fastapi_auth-0.2.1/zopyx_fastapi_auth.egg-info/dependency_links.txt
--rw-------   0 ajung     (1000) ajung     (1000)       71 2024-05-23 10:39:30.000000 zopyx_fastapi_auth-0.2.1/zopyx_fastapi_auth.egg-info/entry_points.txt
--rw-------   0 ajung     (1000) ajung     (1000)      173 2024-05-23 10:39:30.000000 zopyx_fastapi_auth-0.2.1/zopyx_fastapi_auth.egg-info/requires.txt
--rw-------   0 ajung     (1000) ajung     (1000)       13 2024-05-23 10:39:30.000000 zopyx_fastapi_auth-0.2.1/zopyx_fastapi_auth.egg-info/top_level.txt
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:51:31.890025 zopyx_fastapi_auth-0.2.2/
+-rw-------   0 ajung     (1000) ajung     (1000)       27 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/MANIFEST.in
+-rw-r--r--   0 ajung     (1000) ajung     (1000)     6842 2024-05-24 04:51:31.890025 zopyx_fastapi_auth-0.2.2/PKG-INFO
+-rw-------   0 ajung     (1000) ajung     (1000)     5788 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/README.md
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:51:31.882024 zopyx_fastapi_auth-0.2.2/fastapi_auth/
+-rw-------   0 ajung     (1000) ajung     (1000)       14 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/fastapi_auth/__init__.py
+-rw-------   0 ajung     (1000) ajung     (1000)      347 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/fastapi_auth/auth_config.py
+-rw-------   0 ajung     (1000) ajung     (1000)     2122 2024-05-24 04:50:07.000000 zopyx_fastapi_auth-0.2.2/fastapi_auth/auth_routes.py
+-rw-------   0 ajung     (1000) ajung     (1000)     3008 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/fastapi_auth/demo_app.py
+-rw-------   0 ajung     (1000) ajung     (1000)     2465 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/fastapi_auth/dependencies.py
+-rw-------   0 ajung     (1000) ajung     (1000)      290 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/fastapi_auth/jinja2_templates.py
+-rw-------   0 ajung     (1000) ajung     (1000)      106 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/fastapi_auth/logger.py
+-rw-------   0 ajung     (1000) ajung     (1000)      294 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/fastapi_auth/permissions.py
+-rw-------   0 ajung     (1000) ajung     (1000)     1716 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/fastapi_auth/roles.py
+-rw-------   0 ajung     (1000) ajung     (1000)     1899 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/fastapi_auth/user_cmd.py
+-rw-------   0 ajung     (1000) ajung     (1000)     4422 2024-05-24 04:51:00.000000 zopyx_fastapi_auth-0.2.2/fastapi_auth/user_management_sqlobject.py
+-rw-------   0 ajung     (1000) ajung     (1000)     1356 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/fastapi_auth/users.py
+-rw-------   0 ajung     (1000) ajung     (1000)     1141 2024-05-24 04:51:17.000000 zopyx_fastapi_auth-0.2.2/pyproject.toml
+-rw-------   0 ajung     (1000) ajung     (1000)       38 2024-05-24 04:51:31.890025 zopyx_fastapi_auth-0.2.2/setup.cfg
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:51:31.882024 zopyx_fastapi_auth-0.2.2/static/
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:51:31.882024 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:51:31.890025 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/
+-rw-------   0 ajung     (1000) ajung     (1000)    70329 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css
+-rw-------   0 ajung     (1000) ajung     (1000)   203221 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    51795 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   115986 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    70403 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css
+-rw-------   0 ajung     (1000) ajung     (1000)   203225 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    51870 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   116063 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    12065 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css
+-rw-------   0 ajung     (1000) ajung     (1000)   129371 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    10126 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)    51369 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    12058 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css
+-rw-------   0 ajung     (1000) ajung     (1000)   129386 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    10198 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)    63943 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   107823 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css
+-rw-------   0 ajung     (1000) ajung     (1000)   267535 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    85352 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   180381 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   107691 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css
+-rw-------   0 ajung     (1000) ajung     (1000)   267476 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    85281 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   180217 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   281046 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.css
+-rw-------   0 ajung     (1000) ajung     (1000)   679755 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   232803 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   589892 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   280259 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css
+-rw-------   0 ajung     (1000) ajung     (1000)   679615 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   232911 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   589087 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:51:31.890025 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/
+-rw-------   0 ajung     (1000) ajung     (1000)   207819 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js
+-rw-------   0 ajung     (1000) ajung     (1000)   444579 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)    80721 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js
+-rw-------   0 ajung     (1000) ajung     (1000)   332090 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)   135829 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js
+-rw-------   0 ajung     (1000) ajung     (1000)   305438 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)    73935 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js
+-rw-------   0 ajung     (1000) ajung     (1000)   222455 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)   145401 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.js
+-rw-------   0 ajung     (1000) ajung     (1000)   306606 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)    60635 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.min.js
+-rw-------   0 ajung     (1000) ajung     (1000)   220561 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 04:51:31.890025 zopyx_fastapi_auth-0.2.2/zopyx_fastapi_auth.egg-info/
+-rw-r--r--   0 ajung     (1000) ajung     (1000)     6842 2024-05-24 04:51:31.000000 zopyx_fastapi_auth-0.2.2/zopyx_fastapi_auth.egg-info/PKG-INFO
+-rw-------   0 ajung     (1000) ajung     (1000)     3080 2024-05-24 04:51:31.000000 zopyx_fastapi_auth-0.2.2/zopyx_fastapi_auth.egg-info/SOURCES.txt
+-rw-------   0 ajung     (1000) ajung     (1000)        1 2024-05-24 04:51:31.000000 zopyx_fastapi_auth-0.2.2/zopyx_fastapi_auth.egg-info/dependency_links.txt
+-rw-------   0 ajung     (1000) ajung     (1000)       71 2024-05-24 04:51:31.000000 zopyx_fastapi_auth-0.2.2/zopyx_fastapi_auth.egg-info/entry_points.txt
+-rw-------   0 ajung     (1000) ajung     (1000)      184 2024-05-24 04:51:31.000000 zopyx_fastapi_auth-0.2.2/zopyx_fastapi_auth.egg-info/requires.txt
+-rw-------   0 ajung     (1000) ajung     (1000)       13 2024-05-24 04:51:31.000000 zopyx_fastapi_auth-0.2.2/zopyx_fastapi_auth.egg-info/top_level.txt
```

### Comparing `zopyx_fastapi_auth-0.2.1/PKG-INFO` & `zopyx_fastapi_auth-0.2.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,18 @@
-Metadata-Version: 2.1
-Name: zopyx-fastapi-auth
-Version: 0.2.1
-Summary: FastAPI authentication and authorization
-Author-email: Andreas Jung <info@zopyx.com>
-Project-URL: homepage, https://github.com/zopyx/fastapi-auth
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-Requires-Dist: fastapi
-Requires-Dist: pydantic
-Requires-Dist: pydantic-settings
-Requires-Dist: uvicorn
-Requires-Dist: markdown
-Requires-Dist: starlette-session
-Requires-Dist: loguru
-Requires-Dist: bcrypt
-Requires-Dist: jinja2
-Requires-Dist: sqlmodel
-Requires-Dist: rich
-Requires-Dist: python-multipart
-Requires-Dist: typer
-Requires-Dist: typeguard
-Provides-Extra: dev
-Requires-Dist: tox; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: build; extra == "dev"
-
-# fastapi-auth
+# zopyx-fastapi-auth
 
 An opionated authentication and authorization system for FastAPI.
 
 ## Features
 
-- a SQLite-based user database (to be rewritten using SQLObject for broader database support)
+- a RDBMS-based user database (support for almost all databases through sqlmodel)
 - a commandline utility for adding, deleting users
 - roles and permissions
 - FastAPI endpoint protection based on permission or roles
+- fully tested, full test coverage, full mypy compliance, parameter checks at runtime
 
 
 ## Status
 
 - experimental
 
 ## Example usage
@@ -151,18 +120,19 @@
 
 # add static files (for demo login form)
 app.mount("/static", StaticFiles(directory="static"), name="static")
 ```
 
 ## User management
 
-For now, `fastapi-auth` stores user accounts inside a Sqlite database. There is
+For now, `fastapi-auth` stores user accounts inside a SQL database. There is
 the `fastapi-auth-user-admin` utility for managing user accounts through the
 commandline.  There is no support (and there will be no support) for managing
-user accounts through a web admin interface.
+user accounts through a web admin interface. The database connection can be configured
+using the `AUTH_DB_URI` environment variable.
 
 ### adding user
 
 ```
 fastapi-auth-user-admin add <username> <password> "Role1,Role2..."
 ```
 
@@ -180,20 +150,83 @@
 
 ### set password users
 
 ```
 fastapi-auth-user-admin set-password <username> <new-password> 
 ```
 
+## Environment variables
+
+### AUTH_DEFAULT_KEY
+
+`AUTH_DEFAULT_KEY` is used as encryption key for the user's session information.
+It is strongly recommended to set this value rather than depending on the
+default key as used in the code.
+
+### AUTH_DB_URI
+
+`AUTH_DB_URI` must be set to a SQL database. `zopyx-fastapi-auth` uses `sqlmodel` under the hood which uses `SQLAlchemy`and all supported databases (see https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls). 
+
+Example for using a SQLite database `users.db` inside the current working directory:
+
+```
+export AUTH_DB_URI=sqlite:///users.db
+```
+
 ## Internals
 
 The implementation is based on top of the `starlette-session`
 (https://pypi.org/project/starlette-session/) middleware. The user information
 is stored through a  signed cookie-based HTTP session. Session information is
 readable but not modifiable. The encryption key can be configured through an environment
 variable.
 
+## Getting started with the include mini demo application
+
+### Installation
+
+Checkout the codebase and install it using pip or uv:
+
+```
+python3.12 -m venv .venv
+source .venv/bin/activate
+pip3 install -e .
+```
+
+or
+```
+uv venv -p python3.12
+source .venv/bin/activate
+uv pip install -e .
+```
+
+### Create a demo user
+
+```
+fastapi-auth-user-admin add admin admin Administrator
+```
+This will create a user `admin` with password `admin`.
+
+### Running the demo service
+
+```
+uvicorn fastapi_auth.demo_app:app
+```
+
+### Login into the demo application
+
+Visit http://localhost:8000/auth/login and login as `admin`/`admin`.
+
+![Login into application](/images/login.png)
+
+### After successfull login
+
+![Login into application](/images/logged-in.png)
+
+## To do
+- a simple pluggable authentication system for integration of several user sources
+
 
 ## Author
 
 Andreas Jung <info@zopyx.com>
```

### Comparing `zopyx_fastapi_auth-0.2.1/fastapi_auth/auth_routes.py` & `zopyx_fastapi_auth-0.2.2/fastapi_auth/auth_routes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from typing import Optional
 
 from fastapi import Depends, Form, Request, APIRouter
 from fastapi.responses import HTMLResponse, RedirectResponse
 from starlette import status
-from datetime import timedelta
 
 from .dependencies import get_user
 from .logger import LOG
 from .users import User, ANONYMOUS_USER
-from .user_management_sqlobject import UserManagement
+from .user_management_sqlobject import get_user_from_fastapi_request, authenticate_user_for_fastapi
 from .jinja2_templates import templates
-from .roles import ROLES_REGISTRY
-from datetime import datetime, timezone
 
 from starlette.middleware.sessions import SessionMiddleware
 
 from .auth_config import AUTH_SETTINGS
 
 LIFE_TIME = 3600 * 24
 
@@ -56,43 +53,25 @@
 
 
 @router.post("/login")
 async def login_post(
     request: Request,
     username: str = Form(...),
     password: str = Form(...),
-    user: User = Depends(get_user),
 ):
-    um = UserManagement(AUTH_SETTINGS.db_uri)
-    user_data = um.get_user(username, password)
+    user = await get_user_from_fastapi_request(request)
 
-    if user_data is not None:
-        roles = user_data["roles"]
-        roles = [ROLES_REGISTRY.get_role(r) for r in roles if ROLES_REGISTRY.has_role(r)]
-
-        now = datetime.now(timezone.utc)
-        expires = now + timedelta(seconds=LIFE_TIME)
-        user = User(
-            name=user_data["username"],
-            description=user_data["username"],
-            is_anonymous=False,
-            roles=roles,
-            properties=dict(
-                source="internal",
-                logged_in=now.isoformat(),
-                expires=expires.isoformat(),
-            ),
-        )
-        request.session["user"] = user.model_dump()
-        message = f"Welcome {user_data['username']}. You are now logged in."
-        LOG.info(f"User {user_data['username']} logged in")
+    if user:
+        authenticate_user_for_fastapi(user=user, request=request)
+        message = f"Welcome {user.name}. You are now logged in."
+        LOG.info(f"User {user.name} logged in")
         return RedirectResponse(f"/?message={message}", status_code=status.HTTP_302_FOUND)
 
     else:
-        message = f"You {username} could not be logged in. Please try again."
+        message = "You could not be logged in. Please try again."
         LOG.error(message)
         return templates.TemplateResponse(
             request,
             "login.html",
             {
                 "user": ANONYMOUS_USER,
                 "error_message": message,
```

### Comparing `zopyx_fastapi_auth-0.2.1/fastapi_auth/demo_app.py` & `zopyx_fastapi_auth-0.2.2/fastapi_auth/demo_app.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/fastapi_auth/dependencies.py` & `zopyx_fastapi_auth-0.2.2/fastapi_auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/fastapi_auth/roles.py` & `zopyx_fastapi_auth-0.2.2/fastapi_auth/roles.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/fastapi_auth/user_cmd.py` & `zopyx_fastapi_auth-0.2.2/fastapi_auth/user_cmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,24 +65,7 @@
     table = Table(show_header=True, header_style="bold magenta")
     table.add_column("Name")
     table.add_column("Role")
     table.add_column("Created")
     for user in users:
         table.add_row(user.username, user.roles, user.created.isoformat())
     console.print(table)
-
-
-@app.command()
-def delete_db() -> None:
-    """Delete the database."""
-    um = get_user_management()
-    um.delete_db()
-    LOG.debug("Deleted the database.")
-
-
-def main() -> None:
-    """Run the application."""
-    app()
-
-
-if __name__ == "__main__":
-    app()
```

### Comparing `zopyx_fastapi_auth-0.2.1/fastapi_auth/users.py` & `zopyx_fastapi_auth-0.2.2/fastapi_auth/users.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,18 +6,23 @@
 
 from typeguard import typechecked
 
 
 class User(BaseModel):
     """Users"""
 
+    # Name of user
     name: str = Field(..., description="Name of the user")
+    # Description of user
     description: str = Field(..., description="Description of the user")
+    # Is user anonymous
     is_anonymous: bool = True
+    # Roles of user
     roles: list[Role] = []
+    # Properties of user
     properties: dict = {}
 
     def __str__(self) -> str:
         """Return a string representation of the user."""
         self_str = super().__str__()
         return f"{self.__class__.__name__}({self_str})"
```

### Comparing `zopyx_fastapi_auth-0.2.1/pyproject.toml` & `zopyx_fastapi_auth-0.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "zopyx-fastapi-auth"
 description = "FastAPI authentication and authorization"
-version = "0.2.1"
+version = "0.2.2"
 readme = "README.md"
 authors = [
     { name = "Andreas Jung", email = "info@zopyx.com" }
 ]
 classifiers = [
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
@@ -33,14 +33,15 @@
 [project.optional-dependencies]
 dev = [
     "tox",
     "pytest",
     "ruff",
     "twine", 
     "build",
+    "pytest-cov",
 ]
 
 [project.urls]
 homepage = "https://github.com/zopyx/fastapi-auth"
 
 [tool.setuptools]
 packages = ["fastapi_auth"]
```

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.js` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.js.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map` & `zopyx_fastapi_auth-0.2.2/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.1/zopyx_fastapi_auth.egg-info/PKG-INFO` & `zopyx_fastapi_auth-0.2.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zopyx-fastapi-auth
-Version: 0.2.1
+Version: 0.2.2
 Summary: FastAPI authentication and authorization
 Author-email: Andreas Jung <info@zopyx.com>
 Project-URL: homepage, https://github.com/zopyx/fastapi-auth
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -25,25 +25,27 @@
 Requires-Dist: typeguard
 Provides-Extra: dev
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: build; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 
-# fastapi-auth
+# zopyx-fastapi-auth
 
 An opionated authentication and authorization system for FastAPI.
 
 ## Features
 
-- a SQLite-based user database (to be rewritten using SQLObject for broader database support)
+- a RDBMS-based user database (support for almost all databases through sqlmodel)
 - a commandline utility for adding, deleting users
 - roles and permissions
 - FastAPI endpoint protection based on permission or roles
+- fully tested, full test coverage, full mypy compliance, parameter checks at runtime
 
 
 ## Status
 
 - experimental
 
 ## Example usage
@@ -151,18 +153,19 @@
 
 # add static files (for demo login form)
 app.mount("/static", StaticFiles(directory="static"), name="static")
 ```
 
 ## User management
 
-For now, `fastapi-auth` stores user accounts inside a Sqlite database. There is
+For now, `fastapi-auth` stores user accounts inside a SQL database. There is
 the `fastapi-auth-user-admin` utility for managing user accounts through the
 commandline.  There is no support (and there will be no support) for managing
-user accounts through a web admin interface.
+user accounts through a web admin interface. The database connection can be configured
+using the `AUTH_DB_URI` environment variable.
 
 ### adding user
 
 ```
 fastapi-auth-user-admin add <username> <password> "Role1,Role2..."
 ```
 
@@ -180,20 +183,83 @@
 
 ### set password users
 
 ```
 fastapi-auth-user-admin set-password <username> <new-password> 
 ```
 
+## Environment variables
+
+### AUTH_DEFAULT_KEY
+
+`AUTH_DEFAULT_KEY` is used as encryption key for the user's session information.
+It is strongly recommended to set this value rather than depending on the
+default key as used in the code.
+
+### AUTH_DB_URI
+
+`AUTH_DB_URI` must be set to a SQL database. `zopyx-fastapi-auth` uses `sqlmodel` under the hood which uses `SQLAlchemy`and all supported databases (see https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls). 
+
+Example for using a SQLite database `users.db` inside the current working directory:
+
+```
+export AUTH_DB_URI=sqlite:///users.db
+```
+
 ## Internals
 
 The implementation is based on top of the `starlette-session`
 (https://pypi.org/project/starlette-session/) middleware. The user information
 is stored through a  signed cookie-based HTTP session. Session information is
 readable but not modifiable. The encryption key can be configured through an environment
 variable.
 
+## Getting started with the include mini demo application
+
+### Installation
+
+Checkout the codebase and install it using pip or uv:
+
+```
+python3.12 -m venv .venv
+source .venv/bin/activate
+pip3 install -e .
+```
+
+or
+```
+uv venv -p python3.12
+source .venv/bin/activate
+uv pip install -e .
+```
+
+### Create a demo user
+
+```
+fastapi-auth-user-admin add admin admin Administrator
+```
+This will create a user `admin` with password `admin`.
+
+### Running the demo service
+
+```
+uvicorn fastapi_auth.demo_app:app
+```
+
+### Login into the demo application
+
+Visit http://localhost:8000/auth/login and login as `admin`/`admin`.
+
+![Login into application](/images/login.png)
+
+### After successfull login
+
+![Login into application](/images/logged-in.png)
+
+## To do
+- a simple pluggable authentication system for integration of several user sources
+
 
 ## Author
 
 Andreas Jung <info@zopyx.com>
```

### Comparing `zopyx_fastapi_auth-0.2.1/zopyx_fastapi_auth.egg-info/SOURCES.txt` & `zopyx_fastapi_auth-0.2.2/zopyx_fastapi_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

