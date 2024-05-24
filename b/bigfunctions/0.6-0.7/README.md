# Comparing `tmp/bigfunctions-0.6.tar.gz` & `tmp/bigfunctions-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigfunctions-0.6.tar", last modified: Mon May 13 14:59:48 2024, max compression
+gzip compressed data, was "bigfunctions-0.7.tar", last modified: Fri May 24 10:16:50 2024, max compression
```

## Comparing `bigfunctions-0.6.tar` & `bigfunctions-0.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.478641 bigfunctions-0.6/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2023-11-08 21:20:23.000000 bigfunctions-0.6/LICENSE
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9821 2024-05-13 14:59:48.477641 bigfunctions-0.6/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9097 2024-02-22 22:16:20.000000 bigfunctions-0.6/README.md
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.466640 bigfunctions-0.6/bigfun/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2023-11-08 21:20:23.000000 bigfunctions-0.6/bigfun/__init__.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     8507 2024-05-10 19:42:48.000000 bigfunctions-0.6/bigfun/bigfunctions.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9663 2024-05-10 19:32:19.000000 bigfunctions-0.6/bigfun/cli.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      844 2023-12-01 17:33:50.000000 bigfunctions-0.6/bigfun/load_table.py
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.470641 bigfunctions-0.6/bigfun/templates/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1086 2023-11-08 21:20:23.000000 bigfunctions-0.6/bigfun/templates/Dockerfile
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    11722 2024-05-10 19:28:43.000000 bigfunctions-0.6/bigfun/templates/bigfunction.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     3784 2024-01-19 20:34:23.000000 bigfunctions-0.6/bigfun/templates/bookmarklet.js
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1618 2024-05-10 09:49:39.000000 bigfunctions-0.6/bigfun/templates/categories.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4164 2024-01-24 23:20:01.000000 bigfunctions-0.6/bigfun/templates/data.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      554 2024-02-23 19:54:09.000000 bigfunctions-0.6/bigfun/templates/function_js.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7724 2024-02-23 21:48:51.000000 bigfunctions-0.6/bigfun/templates/function_py.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      403 2024-05-13 13:22:43.000000 bigfunctions-0.6/bigfun/templates/function_py.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      212 2024-02-23 21:42:39.000000 bigfunctions-0.6/bigfun/templates/function_py_test.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      410 2024-02-23 19:54:09.000000 bigfunctions-0.6/bigfun/templates/function_sql.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      251 2024-02-23 22:59:01.000000 bigfunctions-0.6/bigfun/templates/function_sql_test.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      702 2024-02-23 19:54:09.000000 bigfunctions-0.6/bigfun/templates/procedure.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      717 2024-02-23 22:23:06.000000 bigfunctions-0.6/bigfun/templates/procedure_test.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      345 2024-02-23 19:54:09.000000 bigfunctions-0.6/bigfun/templates/table_function.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    13269 2024-05-10 19:41:56.000000 bigfunctions-0.6/bigfun/utils.py
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.471641 bigfunctions-0.6/bigfun/website/
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.475641 bigfunctions-0.6/bigfun/website/assets/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1714 2023-11-29 13:48:58.000000 bigfunctions-0.6/bigfun/website/assets/GitHub-Mark-32px.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)  1353755 2024-01-19 20:34:23.000000 bigfunctions-0.6/bigfun/website/assets/bookmarklet_usage.gif
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    23806 2023-11-29 13:48:58.000000 bigfunctions-0.6/bigfun/website/assets/logo.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    73519 2023-11-29 13:48:58.000000 bigfunctions-0.6/bigfun/website/assets/logo_and_name.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    49771 2023-11-29 13:48:58.000000 bigfunctions-0.6/bigfun/website/assets/logo_and_name_wo_supercharge.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1712 2024-05-10 18:53:52.000000 bigfunctions-0.6/bigfun/website/mkdocs.yml
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.475641 bigfunctions-0.6/bigfun/website/theme_overrides/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6185 2024-05-10 12:11:21.000000 bigfunctions-0.6/bigfun/website/theme_overrides/main.html
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.477641 bigfunctions-0.6/bigfunctions.egg-info/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9821 2024-05-13 14:59:48.000000 bigfunctions-0.6/bigfunctions.egg-info/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1076 2024-05-13 14:59:48.000000 bigfunctions-0.6/bigfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-05-13 14:59:48.000000 bigfunctions-0.6/bigfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       42 2024-05-13 14:59:48.000000 bigfunctions-0.6/bigfunctions.egg-info/entry_points.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      130 2024-05-13 14:59:48.000000 bigfunctions-0.6/bigfunctions.egg-info/requires.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        7 2024-05-13 14:59:48.000000 bigfunctions-0.6/bigfunctions.egg-info/top_level.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-05-13 14:59:48.478641 bigfunctions-0.6/setup.cfg
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1111 2024-05-13 14:59:05.000000 bigfunctions-0.6/setup.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-24 10:16:50.206531 bigfunctions-0.7/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2023-11-08 21:20:23.000000 bigfunctions-0.7/LICENSE
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9821 2024-05-24 10:16:50.206531 bigfunctions-0.7/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9097 2024-02-22 22:16:20.000000 bigfunctions-0.7/README.md
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-24 10:16:49.775488 bigfunctions-0.7/bigfun/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2023-11-08 21:20:23.000000 bigfunctions-0.7/bigfun/__init__.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     8515 2024-05-15 15:59:44.000000 bigfunctions-0.7/bigfun/bigfunctions.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9663 2024-05-10 19:32:19.000000 bigfunctions-0.7/bigfun/cli.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      844 2023-12-01 17:33:50.000000 bigfunctions-0.7/bigfun/load_table.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-24 10:16:50.016512 bigfunctions-0.7/bigfun/templates/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      971 2024-05-16 21:53:41.000000 bigfunctions-0.7/bigfun/templates/Dockerfile
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    11722 2024-05-10 19:28:43.000000 bigfunctions-0.7/bigfun/templates/bigfunction.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     3784 2024-01-19 20:34:23.000000 bigfunctions-0.7/bigfun/templates/bookmarklet.js
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1618 2024-05-10 09:49:39.000000 bigfunctions-0.7/bigfun/templates/categories.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4164 2024-01-24 23:20:01.000000 bigfunctions-0.7/bigfun/templates/data.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      554 2024-05-15 15:53:39.000000 bigfunctions-0.7/bigfun/templates/function_js.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7753 2024-05-24 10:14:26.000000 bigfunctions-0.7/bigfun/templates/function_py.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      403 2024-05-13 13:22:43.000000 bigfunctions-0.7/bigfun/templates/function_py.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      212 2024-02-23 21:42:39.000000 bigfunctions-0.7/bigfun/templates/function_py_test.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      410 2024-02-23 19:54:09.000000 bigfunctions-0.7/bigfun/templates/function_sql.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      251 2024-02-23 22:59:01.000000 bigfunctions-0.7/bigfun/templates/function_sql_test.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      702 2024-02-23 19:54:09.000000 bigfunctions-0.7/bigfun/templates/procedure.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      717 2024-02-23 22:23:06.000000 bigfunctions-0.7/bigfun/templates/procedure_test.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      345 2024-02-23 19:54:09.000000 bigfunctions-0.7/bigfun/templates/table_function.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    13269 2024-05-10 19:41:56.000000 bigfunctions-0.7/bigfun/utils.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-24 10:16:50.017513 bigfunctions-0.7/bigfun/website/
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-24 10:16:50.171528 bigfunctions-0.7/bigfun/website/assets/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1714 2023-11-29 13:48:58.000000 bigfunctions-0.7/bigfun/website/assets/GitHub-Mark-32px.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)  1353755 2024-01-19 20:34:23.000000 bigfunctions-0.7/bigfun/website/assets/bookmarklet_usage.gif
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    23806 2023-11-29 13:48:58.000000 bigfunctions-0.7/bigfun/website/assets/logo.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    73519 2023-11-29 13:48:58.000000 bigfunctions-0.7/bigfun/website/assets/logo_and_name.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    49771 2023-11-29 13:48:58.000000 bigfunctions-0.7/bigfun/website/assets/logo_and_name_wo_supercharge.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1712 2024-05-15 16:01:22.000000 bigfunctions-0.7/bigfun/website/mkdocs.yml
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-24 10:16:50.191530 bigfunctions-0.7/bigfun/website/theme_overrides/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6185 2024-05-10 12:11:21.000000 bigfunctions-0.7/bigfun/website/theme_overrides/main.html
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-24 10:16:50.205531 bigfunctions-0.7/bigfunctions.egg-info/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9821 2024-05-24 10:16:49.000000 bigfunctions-0.7/bigfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1076 2024-05-24 10:16:49.000000 bigfunctions-0.7/bigfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-05-24 10:16:49.000000 bigfunctions-0.7/bigfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       42 2024-05-24 10:16:49.000000 bigfunctions-0.7/bigfunctions.egg-info/entry_points.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      130 2024-05-24 10:16:49.000000 bigfunctions-0.7/bigfunctions.egg-info/requires.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        7 2024-05-24 10:16:49.000000 bigfunctions-0.7/bigfunctions.egg-info/top_level.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-05-24 10:16:50.206531 bigfunctions-0.7/setup.cfg
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1111 2024-05-24 10:16:06.000000 bigfunctions-0.7/setup.py
```

### Comparing `bigfunctions-0.6/LICENSE` & `bigfunctions-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/PKG-INFO` & `bigfunctions-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bigfunctions
-Version: 0.6
+Version: 0.7
 Summary: Supercharge BigQuery with BigFunctions
-Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.6.tar.gz
+Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.7.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: bigfunctions Version: 0.6 Summary: Supercharge
+Metadata-Version: 2.1 Name: bigfunctions Version: 0.7 Summary: Supercharge
 BigQuery with BigFunctions Download-URL: https://github.com/unytics/
-bigfunctions/archive/refs/tags/v0.6.tar.gz Author: Unytics Author-email:
+bigfunctions/archive/refs/tags/v0.7.tar.gz Author: Unytics Author-email:
 paul.marcombes@unytics.io Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: google-cloud-bigquery Requires-
 Dist: google-cloud-bigquery_connection Requires-Dist: google-cloud-storage
 Requires-Dist: pyyaml Requires-Dist: jinja2 Requires-Dist: mkdocs-material
 Requires-Dist: click Requires-Dist: click-help-colors
```

### Comparing `bigfunctions-0.6/README.md` & `bigfunctions-0.7/README.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/bigfunctions.py` & `bigfunctions-0.7/bigfun/bigfunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 BIGFUNCTION_DOC_TEMPLATE = jinja2.Template(open(BIGFUNCTION_DOC_TEMPLATE_FILENAME, encoding='utf-8').read())
 
 
 
 
 
 def list_bigfunctions():
-    return [f.replace('.yaml', '') for f in os.listdir(BIGFUNCTIONS_FOLDER) if f.endswith('.yaml')]
+    return sorted([f.replace('.yaml', '') for f in os.listdir(BIGFUNCTIONS_FOLDER) if f.endswith('.yaml')])
 
 
 
 class BigFunction:
 
     def __init__(self, name, project=None, dataset=None, **config_override):
         self.name = name
```

### Comparing `bigfunctions-0.6/bigfun/cli.py` & `bigfunctions-0.7/bigfun/cli.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/load_table.py` & `bigfunctions-0.7/bigfun/load_table.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/templates/Dockerfile` & `bigfunctions-0.7/bigfun/templates/Dockerfile`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM {% if dockerfile is defined and dockerfile.base_image is defined %}{{ dockerfile.base_image }}{% else %}python:3.10-slim{% endif %}
+FROM python:3.11-slim
 
 EXPOSE 8080
 
 # Allow statements and log messages to immediately appear in the Knative logs
 ENV PYTHONUNBUFFERED True
 ENV PORT=8080
```

### Comparing `bigfunctions-0.6/bigfun/templates/bigfunction.md` & `bigfunctions-0.7/bigfun/templates/bigfunction.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/templates/bookmarklet.js` & `bigfunctions-0.7/bigfun/templates/bookmarklet.js`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/templates/categories.md` & `bigfunctions-0.7/bigfun/templates/categories.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/templates/data.md` & `bigfunctions-0.7/bigfun/templates/data.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/templates/function_js.sql` & `bigfunctions-0.7/bigfun/templates/function_js.sql`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/templates/function_py.py` & `bigfunctions-0.7/bigfun/templates/function_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 error_reporter = google.cloud.error_reporting.Client()
 app = Flask(__name__)
 
 
 CACHE = {}
 CURRENT_LOCATION = '{{ cloud_run_location }}'
 
-QUOTAS = {{ quotas }}
+QUOTAS = {{ quotas if quotas is defined else {} }}
 
 
 _, PROJECT = google.auth.default()
 
 
 def get_current_service_account():
     if 'current_service_account' not in CACHE:
```

### Comparing `bigfunctions-0.6/bigfun/templates/procedure.sql` & `bigfunctions-0.7/bigfun/templates/procedure.sql`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/templates/procedure_test.sql` & `bigfunctions-0.7/bigfun/templates/procedure_test.sql`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/utils.py` & `bigfunctions-0.7/bigfun/utils.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/website/assets/GitHub-Mark-32px.png` & `bigfunctions-0.7/bigfun/website/assets/GitHub-Mark-32px.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/website/assets/bookmarklet_usage.gif` & `bigfunctions-0.7/bigfun/website/assets/bookmarklet_usage.gif`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/website/assets/logo.png` & `bigfunctions-0.7/bigfun/website/assets/logo.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/website/assets/logo_and_name.png` & `bigfunctions-0.7/bigfun/website/assets/logo_and_name.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/website/assets/logo_and_name_wo_supercharge.png` & `bigfunctions-0.7/bigfun/website/assets/logo_and_name_wo_supercharge.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfun/website/mkdocs.yml` & `bigfunctions-0.7/bigfun/website/mkdocs.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -37,22 +37,20 @@
 nav:
   - Get Started!: README.md
   - Explore BigFunctions: bigfunctions/README.md
 validation:
   nav:
     omitted_files: ignore
 bigfunctions_categories:
-  - name: "explore"
-    emoticon: "👀"
   - name: "AI"
     emoticon: "🧠"
-  - name: "get_data"
-    emoticon: "🛢"
   - name: "notify"
     emoticon: "💬"
+  - name: "get_data"
+    emoticon: "🛢"
   - name: "export"
     emoticon: "🚀"
   - name: "transform_numeric"
     emoticon: "1️⃣"
   - name: "transform_string"
     emoticon: "✨"
   - name: "transform_geo_data"
@@ -65,9 +63,11 @@
     emoticon: "<span style=\"color: var(--md-primary-fg-color);\">[...]</span>"
   - name: "machine_learning"
     emoticon: "🧠"
   - name: "graph"
     emoticon: "🌐"
   - name: "convert_data_format"
     emoticon: "🔨"
+  - name: "explore"
+    emoticon: "👀"
   - name: "utils"
     emoticon: "🔨"
```

### Comparing `bigfunctions-0.6/bigfun/website/theme_overrides/main.html` & `bigfunctions-0.7/bigfun/website/theme_overrides/main.html`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/bigfunctions.egg-info/PKG-INFO` & `bigfunctions-0.7/bigfunctions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bigfunctions
-Version: 0.6
+Version: 0.7
 Summary: Supercharge BigQuery with BigFunctions
-Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.6.tar.gz
+Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.7.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: bigfunctions Version: 0.6 Summary: Supercharge
+Metadata-Version: 2.1 Name: bigfunctions Version: 0.7 Summary: Supercharge
 BigQuery with BigFunctions Download-URL: https://github.com/unytics/
-bigfunctions/archive/refs/tags/v0.6.tar.gz Author: Unytics Author-email:
+bigfunctions/archive/refs/tags/v0.7.tar.gz Author: Unytics Author-email:
 paul.marcombes@unytics.io Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: google-cloud-bigquery Requires-
 Dist: google-cloud-bigquery_connection Requires-Dist: google-cloud-storage
 Requires-Dist: pyyaml Requires-Dist: jinja2 Requires-Dist: mkdocs-material
 Requires-Dist: click Requires-Dist: click-help-colors
```

### Comparing `bigfunctions-0.6/bigfunctions.egg-info/SOURCES.txt` & `bigfunctions-0.7/bigfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.6/setup.py` & `bigfunctions-0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = '0.6'
+VERSION = '0.7'
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
```

