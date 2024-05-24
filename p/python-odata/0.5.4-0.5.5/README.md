# Comparing `tmp/python_odata-0.5.4.tar.gz` & `tmp/python_odata-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_odata-0.5.4.tar", max compression
+gzip compressed data, was "python_odata-0.5.5.tar", max compression
```

## Comparing `python_odata-0.5.4.tar` & `python_odata-0.5.5.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1100 2023-02-17 07:38:59.292617 python_odata-0.5.4/LICENSE
--rw-r--r--   0        0        0      117 2023-03-06 10:15:16.241206 python_odata-0.5.4/odata/__init__.py
--rw-r--r--   0        0        0    12990 2023-03-02 13:02:58.675225 python_odata-0.5.4/odata/action.py
--rw-r--r--   0        0        0     2788 2023-03-02 13:02:58.669220 python_odata-0.5.4/odata/complextype.py
--rw-r--r--   0        0        0     6585 2023-03-15 11:52:45.722584 python_odata-0.5.4/odata/connection.py
--rw-r--r--   0        0        0     4784 2023-03-06 10:16:54.505663 python_odata-0.5.4/odata/context.py
--rw-r--r--   0        0        0     4894 2023-03-06 10:16:50.818100 python_odata-0.5.4/odata/entity.py
--rw-r--r--   0        0        0      630 2023-03-02 13:02:58.685304 python_odata-0.5.4/odata/enumtype.py
--rw-r--r--   0        0        0     1354 2023-02-17 07:38:59.302617 python_odata-0.5.4/odata/exceptions.py
--rw-r--r--   0        0        0    22036 2023-03-06 10:16:50.820621 python_odata-0.5.4/odata/metadata.py
--rw-r--r--   0        0        0     5850 2023-03-14 08:47:41.324066 python_odata-0.5.4/odata/navproperty.py
--rw-r--r--   0        0        0    11651 2023-03-20 10:30:20.345259 python_odata-0.5.4/odata/property.py
--rw-r--r--   0        0        0    11993 2023-03-21 10:16:55.036384 python_odata-0.5.4/odata/query.py
--rw-r--r--   0        0        0      754 2023-03-06 10:16:50.822620 python_odata-0.5.4/odata/reflect-templates/entity.mako
--rw-r--r--   0        0        0     1165 2023-03-06 10:16:50.823620 python_odata-0.5.4/odata/reflect-templates/main.mako
--rw-r--r--   0        0        0      581 2023-03-06 10:16:50.824620 python_odata-0.5.4/odata/reflect-templates/nav_property.mako
--rw-r--r--   0        0        0      544 2023-03-06 10:16:50.824620 python_odata-0.5.4/odata/reflect-templates/property.mako
--rw-r--r--   0        0        0        0 2023-03-06 10:16:50.824620 python_odata-0.5.4/odata/reflect-templates/typevar.mako
--rw-r--r--   0        0        0     5107 2023-03-06 15:51:01.171127 python_odata-0.5.4/odata/reflector.py
--rw-r--r--   0        0        0     8031 2023-03-06 17:53:20.398812 python_odata-0.5.4/odata/service.py
--rw-r--r--   0        0        0     9309 2023-03-06 10:16:47.116904 python_odata-0.5.4/odata/state.py
--rw-r--r--   0        0        0     1461 2023-03-06 10:16:54.506372 python_odata-0.5.4/odata/utils.py
--rw-r--r--   0        0        0      893 2023-03-21 10:16:59.281062 python_odata-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1412 2023-03-06 10:24:04.148395 python_odata-0.5.4/README.md
--rw-r--r--   0        0        0     2188 1970-01-01 00:00:00.000000 python_odata-0.5.4/setup.py
--rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 python_odata-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-02-17 07:38:59.292617 python_odata-0.5.5/LICENSE
+-rw-r--r--   0        0        0      117 2023-03-06 10:15:16.241206 python_odata-0.5.5/odata/__init__.py
+-rw-r--r--   0        0        0    12990 2023-03-02 13:02:58.675225 python_odata-0.5.5/odata/action.py
+-rw-r--r--   0        0        0     2788 2023-03-02 13:02:58.669220 python_odata-0.5.5/odata/complextype.py
+-rw-r--r--   0        0        0     6708 2024-05-24 10:10:40.952549 python_odata-0.5.5/odata/connection.py
+-rw-r--r--   0        0        0     4784 2023-03-06 10:16:54.505663 python_odata-0.5.5/odata/context.py
+-rw-r--r--   0        0        0     4894 2023-03-06 10:16:50.818100 python_odata-0.5.5/odata/entity.py
+-rw-r--r--   0        0        0      630 2023-03-02 13:02:58.685304 python_odata-0.5.5/odata/enumtype.py
+-rw-r--r--   0        0        0     1354 2023-02-17 07:38:59.302617 python_odata-0.5.5/odata/exceptions.py
+-rw-r--r--   0        0        0    22036 2023-03-06 10:16:50.820621 python_odata-0.5.5/odata/metadata.py
+-rw-r--r--   0        0        0     5850 2023-03-14 08:47:41.324066 python_odata-0.5.5/odata/navproperty.py
+-rw-r--r--   0        0        0    11651 2023-03-20 10:30:20.345259 python_odata-0.5.5/odata/property.py
+-rw-r--r--   0        0        0    11993 2023-03-21 10:16:55.036384 python_odata-0.5.5/odata/query.py
+-rw-r--r--   0        0        0      754 2023-03-06 10:16:50.822620 python_odata-0.5.5/odata/reflect-templates/entity.mako
+-rw-r--r--   0        0        0     1165 2023-03-06 10:16:50.823620 python_odata-0.5.5/odata/reflect-templates/main.mako
+-rw-r--r--   0        0        0      581 2023-03-06 10:16:50.824620 python_odata-0.5.5/odata/reflect-templates/nav_property.mako
+-rw-r--r--   0        0        0      544 2023-03-06 10:16:50.824620 python_odata-0.5.5/odata/reflect-templates/property.mako
+-rw-r--r--   0        0        0        0 2023-03-06 10:16:50.824620 python_odata-0.5.5/odata/reflect-templates/typevar.mako
+-rw-r--r--   0        0        0     5107 2023-03-06 15:51:01.171127 python_odata-0.5.5/odata/reflector.py
+-rw-r--r--   0        0        0     8031 2023-03-06 17:53:20.398812 python_odata-0.5.5/odata/service.py
+-rw-r--r--   0        0        0     9309 2023-03-06 10:16:47.116904 python_odata-0.5.5/odata/state.py
+-rw-r--r--   0        0        0     1461 2023-03-06 10:16:54.506372 python_odata-0.5.5/odata/utils.py
+-rw-r--r--   0        0        0      893 2024-05-24 10:11:14.630349 python_odata-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1412 2023-03-06 10:24:04.148395 python_odata-0.5.5/README.md
+-rw-r--r--   0        0        0     2156 1970-01-01 00:00:00.000000 python_odata-0.5.5/PKG-INFO
```

### Comparing `python_odata-0.5.4/LICENSE` & `python_odata-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/action.py` & `python_odata-0.5.5/odata/action.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/complextype.py` & `python_odata-0.5.5/odata/complextype.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/connection.py` & `python_odata-0.5.5/odata/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,26 +83,28 @@
                     code = odata_error.get('code', None) or code
                     message = odata_error.get('message', None) or message
                     if 'innererror' in odata_error:
                         ie = odata_error['innererror']
                         detailed_message = ie.get('message', None) or detailed_message
             elif "application/problem+json" in response_ct:
                 errordata = response.json()
-                if "exception"in errordata:
+                if "exception" in errordata:
                     odata_exception = errordata.get("exception")
                     code = errordata.get("type", None) or code
                     code = errordata.get("errorId", None) or code
                     detailed_message = errordata.get("detail", None) or detailed_message
                     message = odata_exception.get("message", None) or message
 
                     inner = ["innerexception", "innerException"]
                     for candidate in inner:
                         if candidate in odata_exception:
                             ie = odata_exception[candidate]
                             detailed_message = ie.get("message", None) or detailed_message
+                else:
+                    detailed_message = response.headers.get('WWW-Authenticate', detailed_message)
             else:
                 detailed_message = response.text
 
             msg = ' | '.join([str(status_code), str(code), str(message), str(detailed_message)])
             err = ODataError(msg)
             err.status_code = status_code
             err.code = code
```

### Comparing `python_odata-0.5.4/odata/context.py` & `python_odata-0.5.5/odata/context.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/entity.py` & `python_odata-0.5.5/odata/entity.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/enumtype.py` & `python_odata-0.5.5/odata/enumtype.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/exceptions.py` & `python_odata-0.5.5/odata/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/metadata.py` & `python_odata-0.5.5/odata/metadata.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/navproperty.py` & `python_odata-0.5.5/odata/navproperty.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/property.py` & `python_odata-0.5.5/odata/property.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/query.py` & `python_odata-0.5.5/odata/query.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/reflect-templates/entity.mako` & `python_odata-0.5.5/odata/reflect-templates/entity.mako`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/reflect-templates/main.mako` & `python_odata-0.5.5/odata/reflect-templates/main.mako`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/reflect-templates/nav_property.mako` & `python_odata-0.5.5/odata/reflect-templates/nav_property.mako`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/reflect-templates/property.mako` & `python_odata-0.5.5/odata/reflect-templates/property.mako`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/reflector.py` & `python_odata-0.5.5/odata/reflector.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/service.py` & `python_odata-0.5.5/odata/service.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/state.py` & `python_odata-0.5.5/odata/state.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/odata/utils.py` & `python_odata-0.5.5/odata/utils.py`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/pyproject.toml` & `python_odata-0.5.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-odata"
-version = "0.5.4"
+version = "0.5.5"
 description = "A simple library for read/write access to OData services."
 license="MIT"
 authors = ["Tuomas Mursu <tuomas.mursu@kapsi.fi>", "Cristian Libotean <eblis102@gmail.com>"]
 readme = "README.md"
 packages = [
 	{ include = "odata/*.py" },
 ]
```

### Comparing `python_odata-0.5.4/README.md` & `python_odata-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `python_odata-0.5.4/PKG-INFO` & `python_odata-0.5.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: python-odata
-Version: 0.5.4
+Version: 0.5.5
 Summary: A simple library for read/write access to OData services.
 License: MIT
 Author: Tuomas Mursu
 Author-email: tuomas.mursu@kapsi.fi
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: mako (>=1.2.4)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: requests (>=2.28.2)
 Requires-Dist: rich (>=13.3.1)
 Description-Content-Type: text/markdown
 
 # python-odata
```

