# Comparing `tmp/falcon-helpers-0.9.5.tar.gz` & `tmp/falcon-helpers-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/falcon-helpers-0.9.5.tar", last modified: Fri Mar  2 06:02:25 2018, max compression
+gzip compressed data, was "dist/falcon-helpers-0.9.6.tar", last modified: Fri Mar  2 06:06:46 2018, max compression
```

## Comparing `falcon-helpers-0.9.5.tar` & `falcon-helpers-0.9.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/
--rw-r--r--   0 nzac       (501) staff       (20)       49 2018-02-14 02:37:37.000000 falcon-helpers-0.9.5/.gitignore
--rw-r--r--   0 nzac       (501) staff       (20)     2958 2018-03-02 05:59:38.000000 falcon-helpers-0.9.5/CHANGELOG.rst
-drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/falcon_helpers/
--rw-r--r--   0 nzac       (501) staff       (20)      215 2017-12-16 00:05:06.000000 falcon-helpers-0.9.5/falcon_helpers/__init__.py
-drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/falcon_helpers/contrib/
--rw-r--r--   0 nzac       (501) staff       (20)       41 2018-02-24 01:21:53.000000 falcon-helpers-0.9.5/falcon_helpers/contrib/__init__.py
--rw-r--r--   0 nzac       (501) staff       (20)     4546 2018-03-02 04:13:46.000000 falcon-helpers-0.9.5/falcon_helpers/contrib/auth.py
--rw-r--r--   0 nzac       (501) staff       (20)     4499 2018-03-01 00:25:50.000000 falcon-helpers-0.9.5/falcon_helpers/contrib/storage.py
-drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/falcon_helpers/middlewares/
--rw-r--r--   0 nzac       (501) staff       (20)      407 2018-02-23 22:47:04.000000 falcon-helpers-0.9.5/falcon_helpers/middlewares/__init__.py
--rw-r--r--   0 nzac       (501) staff       (20)     1646 2018-02-14 02:42:57.000000 falcon-helpers-0.9.5/falcon_helpers/middlewares/auth_required.py
--rw-r--r--   0 nzac       (501) staff       (20)     2785 2017-11-30 02:48:22.000000 falcon-helpers-0.9.5/falcon_helpers/middlewares/jinja2.py
--rw-r--r--   0 nzac       (501) staff       (20)     1333 2018-02-16 03:09:45.000000 falcon-helpers-0.9.5/falcon_helpers/middlewares/load_user.py
--rw-r--r--   0 nzac       (501) staff       (20)     1706 2018-02-24 21:09:29.000000 falcon-helpers-0.9.5/falcon_helpers/middlewares/marshmallow.py
--rw-r--r--   0 nzac       (501) staff       (20)      119 2018-02-23 22:47:04.000000 falcon-helpers-0.9.5/falcon_helpers/middlewares/multipart.py
--rw-r--r--   0 nzac       (501) staff       (20)     2946 2018-02-16 03:08:33.000000 falcon-helpers-0.9.5/falcon_helpers/middlewares/parsejwt.py
--rw-r--r--   0 nzac       (501) staff       (20)      656 2018-02-16 03:52:13.000000 falcon-helpers-0.9.5/falcon_helpers/middlewares/sqla.py
--rw-r--r--   0 nzac       (501) staff       (20)     2469 2017-11-15 03:13:52.000000 falcon-helpers-0.9.5/falcon_helpers/middlewares/statics.py
-drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/falcon_helpers/resources/
--rw-r--r--   0 nzac       (501) staff       (20)       93 2017-11-15 03:13:52.000000 falcon-helpers-0.9.5/falcon_helpers/resources/__init__.py
--rw-r--r--   0 nzac       (501) staff       (20)     3190 2017-12-16 00:32:03.000000 falcon-helpers-0.9.5/falcon_helpers/resources/auth0.py
--rw-r--r--   0 nzac       (501) staff       (20)     4053 2018-03-02 03:50:15.000000 falcon-helpers-0.9.5/falcon_helpers/resources/crud.py
--rw-r--r--   0 nzac       (501) staff       (20)      502 2017-11-30 02:44:26.000000 falcon-helpers-0.9.5/falcon_helpers/resources/redirect.py
-drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/falcon_helpers/sqla/
--rw-r--r--   0 nzac       (501) staff       (20)       98 2017-11-30 03:24:46.000000 falcon-helpers-0.9.5/falcon_helpers/sqla/__init__.py
--rw-r--r--   0 nzac       (501) staff       (20)     1510 2017-12-16 00:05:06.000000 falcon-helpers-0.9.5/falcon_helpers/sqla/columns.py
--rw-r--r--   0 nzac       (501) staff       (20)      143 2017-11-15 03:13:52.000000 falcon-helpers-0.9.5/falcon_helpers/sqla/core.py
--rw-r--r--   0 nzac       (501) staff       (20)      112 2018-02-16 03:53:01.000000 falcon-helpers-0.9.5/falcon_helpers/sqla/db.py
--rw-r--r--   0 nzac       (501) staff       (20)     2533 2018-02-28 02:47:47.000000 falcon-helpers-0.9.5/falcon_helpers/sqla/orm.py
--rw-r--r--   0 nzac       (501) staff       (20)      193 2017-11-15 03:13:52.000000 falcon-helpers-0.9.5/falcon_helpers/sqla/postgres.py
--rw-r--r--   0 nzac       (501) staff       (20)     1258 2017-12-16 00:05:06.000000 falcon-helpers-0.9.5/falcon_helpers/sqla/utils.py
--rw-r--r--   0 nzac       (501) staff       (20)      271 2018-02-16 05:26:22.000000 falcon-helpers-0.9.5/falcon_helpers/utils.py
-drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/falcon_helpers.egg-info/
--rw-r--r--   0 nzac       (501) staff       (20)        1 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/falcon_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 nzac       (501) staff       (20)     5217 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/falcon_helpers.egg-info/PKG-INFO
--rw-r--r--   0 nzac       (501) staff       (20)       72 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/falcon_helpers.egg-info/requires.txt
--rw-r--r--   0 nzac       (501) staff       (20)     1135 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/falcon_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 nzac       (501) staff       (20)       15 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/falcon_helpers.egg-info/top_level.txt
--rw-r--r--   0 nzac       (501) staff       (20)        1 2017-11-15 03:50:24.000000 falcon-helpers-0.9.5/falcon_helpers.egg-info/zip-safe
--rw-r--r--   0 nzac       (501) staff       (20)     1536 2017-11-15 03:13:52.000000 falcon-helpers-0.9.5/LICENSE
--rw-r--r--   0 nzac       (501) staff       (20)     5217 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/PKG-INFO
--rw-r--r--   0 nzac       (501) staff       (20)      416 2017-11-15 03:13:52.000000 falcon-helpers-0.9.5/README.rst
--rw-r--r--   0 nzac       (501) staff       (20)      130 2018-03-02 06:02:25.000000 falcon-helpers-0.9.5/setup.cfg
--rw-r--r--   0 nzac       (501) staff       (20)     1291 2018-02-24 21:33:54.000000 falcon-helpers-0.9.5/setup.py
+drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/
+-rw-r--r--   0 nzac       (501) staff       (20)       49 2018-02-14 02:37:37.000000 falcon-helpers-0.9.6/.gitignore
+-rw-r--r--   0 nzac       (501) staff       (20)     3020 2018-03-02 06:06:38.000000 falcon-helpers-0.9.6/CHANGELOG.rst
+drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/falcon_helpers/
+-rw-r--r--   0 nzac       (501) staff       (20)      215 2017-12-16 00:05:06.000000 falcon-helpers-0.9.6/falcon_helpers/__init__.py
+drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/falcon_helpers/contrib/
+-rw-r--r--   0 nzac       (501) staff       (20)       41 2018-02-24 01:21:53.000000 falcon-helpers-0.9.6/falcon_helpers/contrib/__init__.py
+-rw-r--r--   0 nzac       (501) staff       (20)     4546 2018-03-02 04:13:46.000000 falcon-helpers-0.9.6/falcon_helpers/contrib/auth.py
+-rw-r--r--   0 nzac       (501) staff       (20)     4499 2018-03-01 00:25:50.000000 falcon-helpers-0.9.6/falcon_helpers/contrib/storage.py
+drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/falcon_helpers/middlewares/
+-rw-r--r--   0 nzac       (501) staff       (20)      407 2018-02-23 22:47:04.000000 falcon-helpers-0.9.6/falcon_helpers/middlewares/__init__.py
+-rw-r--r--   0 nzac       (501) staff       (20)     1646 2018-02-14 02:42:57.000000 falcon-helpers-0.9.6/falcon_helpers/middlewares/auth_required.py
+-rw-r--r--   0 nzac       (501) staff       (20)     2785 2017-11-30 02:48:22.000000 falcon-helpers-0.9.6/falcon_helpers/middlewares/jinja2.py
+-rw-r--r--   0 nzac       (501) staff       (20)     1333 2018-02-16 03:09:45.000000 falcon-helpers-0.9.6/falcon_helpers/middlewares/load_user.py
+-rw-r--r--   0 nzac       (501) staff       (20)     1706 2018-02-24 21:09:29.000000 falcon-helpers-0.9.6/falcon_helpers/middlewares/marshmallow.py
+-rw-r--r--   0 nzac       (501) staff       (20)      119 2018-02-23 22:47:04.000000 falcon-helpers-0.9.6/falcon_helpers/middlewares/multipart.py
+-rw-r--r--   0 nzac       (501) staff       (20)     2946 2018-02-16 03:08:33.000000 falcon-helpers-0.9.6/falcon_helpers/middlewares/parsejwt.py
+-rw-r--r--   0 nzac       (501) staff       (20)      656 2018-02-16 03:52:13.000000 falcon-helpers-0.9.6/falcon_helpers/middlewares/sqla.py
+-rw-r--r--   0 nzac       (501) staff       (20)     2469 2017-11-15 03:13:52.000000 falcon-helpers-0.9.6/falcon_helpers/middlewares/statics.py
+drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/falcon_helpers/resources/
+-rw-r--r--   0 nzac       (501) staff       (20)       93 2017-11-15 03:13:52.000000 falcon-helpers-0.9.6/falcon_helpers/resources/__init__.py
+-rw-r--r--   0 nzac       (501) staff       (20)     3190 2017-12-16 00:32:03.000000 falcon-helpers-0.9.6/falcon_helpers/resources/auth0.py
+-rw-r--r--   0 nzac       (501) staff       (20)     4058 2018-03-02 06:04:45.000000 falcon-helpers-0.9.6/falcon_helpers/resources/crud.py
+-rw-r--r--   0 nzac       (501) staff       (20)      502 2017-11-30 02:44:26.000000 falcon-helpers-0.9.6/falcon_helpers/resources/redirect.py
+drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/falcon_helpers/sqla/
+-rw-r--r--   0 nzac       (501) staff       (20)       98 2017-11-30 03:24:46.000000 falcon-helpers-0.9.6/falcon_helpers/sqla/__init__.py
+-rw-r--r--   0 nzac       (501) staff       (20)     1510 2017-12-16 00:05:06.000000 falcon-helpers-0.9.6/falcon_helpers/sqla/columns.py
+-rw-r--r--   0 nzac       (501) staff       (20)      143 2017-11-15 03:13:52.000000 falcon-helpers-0.9.6/falcon_helpers/sqla/core.py
+-rw-r--r--   0 nzac       (501) staff       (20)      112 2018-02-16 03:53:01.000000 falcon-helpers-0.9.6/falcon_helpers/sqla/db.py
+-rw-r--r--   0 nzac       (501) staff       (20)     2533 2018-02-28 02:47:47.000000 falcon-helpers-0.9.6/falcon_helpers/sqla/orm.py
+-rw-r--r--   0 nzac       (501) staff       (20)      193 2017-11-15 03:13:52.000000 falcon-helpers-0.9.6/falcon_helpers/sqla/postgres.py
+-rw-r--r--   0 nzac       (501) staff       (20)     1258 2017-12-16 00:05:06.000000 falcon-helpers-0.9.6/falcon_helpers/sqla/utils.py
+-rw-r--r--   0 nzac       (501) staff       (20)      271 2018-02-16 05:26:22.000000 falcon-helpers-0.9.6/falcon_helpers/utils.py
+drwxr-xr-x   0 nzac       (501) staff       (20)        0 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/falcon_helpers.egg-info/
+-rw-r--r--   0 nzac       (501) staff       (20)        1 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/falcon_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 nzac       (501) staff       (20)     5319 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/falcon_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 nzac       (501) staff       (20)       72 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/falcon_helpers.egg-info/requires.txt
+-rw-r--r--   0 nzac       (501) staff       (20)     1135 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/falcon_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 nzac       (501) staff       (20)       15 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/falcon_helpers.egg-info/top_level.txt
+-rw-r--r--   0 nzac       (501) staff       (20)        1 2017-11-15 03:50:24.000000 falcon-helpers-0.9.6/falcon_helpers.egg-info/zip-safe
+-rw-r--r--   0 nzac       (501) staff       (20)     1536 2017-11-15 03:13:52.000000 falcon-helpers-0.9.6/LICENSE
+-rw-r--r--   0 nzac       (501) staff       (20)     5319 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/PKG-INFO
+-rw-r--r--   0 nzac       (501) staff       (20)      416 2017-11-15 03:13:52.000000 falcon-helpers-0.9.6/README.rst
+-rw-r--r--   0 nzac       (501) staff       (20)      130 2018-03-02 06:06:46.000000 falcon-helpers-0.9.6/setup.cfg
+-rw-r--r--   0 nzac       (501) staff       (20)     1291 2018-02-24 21:33:54.000000 falcon-helpers-0.9.6/setup.py
```

### Comparing `falcon-helpers-0.9.5/CHANGELOG.rst` & `falcon-helpers-0.9.6/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+0.9.6 - 2018-03-02
+##################
+
+* [BUG] Forgot a self
+
 0.9.5 - 2018-03-01
 ##################
 
 * [NEW] get_object was implemented for CrudBase
 * [FEAT] has_permission now supports an enum type
 * [NEW] kwargs is now used on CrudBase
```

### Comparing `falcon-helpers-0.9.5/falcon_helpers/contrib/auth.py` & `falcon-helpers-0.9.6/falcon_helpers/contrib/auth.py`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/falcon_helpers/contrib/storage.py` & `falcon-helpers-0.9.6/falcon_helpers/contrib/storage.py`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/falcon_helpers/middlewares/auth_required.py` & `falcon-helpers-0.9.6/falcon_helpers/middlewares/auth_required.py`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/falcon_helpers/middlewares/jinja2.py` & `falcon-helpers-0.9.6/falcon_helpers/middlewares/jinja2.py`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/falcon_helpers/middlewares/load_user.py` & `falcon-helpers-0.9.6/falcon_helpers/middlewares/load_user.py`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/falcon_helpers/middlewares/marshmallow.py` & `falcon-helpers-0.9.6/falcon_helpers/middlewares/marshmallow.py`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/falcon_helpers/middlewares/parsejwt.py` & `falcon-helpers-0.9.6/falcon_helpers/middlewares/parsejwt.py`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/falcon_helpers/middlewares/sqla.py` & `falcon-helpers-0.9.6/falcon_helpers/middlewares/sqla.py`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/falcon_helpers/middlewares/statics.py` & `falcon-helpers-0.9.6/falcon_helpers/middlewares/statics.py`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/falcon_helpers/resources/auth0.py` & `falcon-helpers-0.9.6/falcon_helpers/resources/auth0.py`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/falcon_helpers/resources/crud.py` & `falcon-helpers-0.9.6/falcon_helpers/resources/crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     """
     db_cls = None
     schema = None
     default_param_name = 'obj_id'
 
     def get_object(self, req, **kwargs):
         try:
-            obj_id = kwargs[default_param_name]
+            obj_id = kwargs[self.default_param_name]
             return self.session.query(self.db_cls).get(obj_id)
         except KeyError:
             raise falcon.HTTPInternalServerError("Misconfigured route")
 
     def on_get(self, req, resp, **kwargs):
         result = self.get_object(req, **kwargs)
```

### Comparing `falcon-helpers-0.9.5/falcon_helpers/sqla/columns.py` & `falcon-helpers-0.9.6/falcon_helpers/sqla/columns.py`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/falcon_helpers/sqla/orm.py` & `falcon-helpers-0.9.6/falcon_helpers/sqla/orm.py`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/falcon_helpers/sqla/utils.py` & `falcon-helpers-0.9.6/falcon_helpers/sqla/utils.py`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/falcon_helpers.egg-info/PKG-INFO` & `falcon-helpers-0.9.6/falcon_helpers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: falcon-helpers
-Version: 0.9.5
+Version: 0.9.6
 Summary: A few helpful tools to make working with the falcon framework a real joy!
 Home-page: https://gitlab.com/skosh/falcon-helpers
 Author: Nick Zaccardi
 Author-email: nicholas.zaccardi@gmail.com
 License: BSD
 Description: .. default-role:: code
         .. role:: python(code)
@@ -33,14 +33,19 @@
           api = falcon.API(
             middlewares=[
               falcon_helpers.middlewares.StaticsMiddleware()
             ]
           )
         
         
+        0.9.6 - 2018-03-02
+        ##################
+        
+        * [BUG] Forgot a self
+        
         0.9.5 - 2018-03-01
         ##################
         
         * [NEW] get_object was implemented for CrudBase
         * [FEAT] has_permission now supports an enum type
         * [NEW] kwargs is now used on CrudBase
```

### Comparing `falcon-helpers-0.9.5/falcon_helpers.egg-info/SOURCES.txt` & `falcon-helpers-0.9.6/falcon_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/LICENSE` & `falcon-helpers-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon-helpers-0.9.5/PKG-INFO` & `falcon-helpers-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: falcon-helpers
-Version: 0.9.5
+Version: 0.9.6
 Summary: A few helpful tools to make working with the falcon framework a real joy!
 Home-page: https://gitlab.com/skosh/falcon-helpers
 Author: Nick Zaccardi
 Author-email: nicholas.zaccardi@gmail.com
 License: BSD
 Description: .. default-role:: code
         .. role:: python(code)
@@ -33,14 +33,19 @@
           api = falcon.API(
             middlewares=[
               falcon_helpers.middlewares.StaticsMiddleware()
             ]
           )
         
         
+        0.9.6 - 2018-03-02
+        ##################
+        
+        * [BUG] Forgot a self
+        
         0.9.5 - 2018-03-01
         ##################
         
         * [NEW] get_object was implemented for CrudBase
         * [FEAT] has_permission now supports an enum type
         * [NEW] kwargs is now used on CrudBase
```

### Comparing `falcon-helpers-0.9.5/setup.py` & `falcon-helpers-0.9.6/setup.py`

 * *Files identical despite different names*

