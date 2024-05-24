# Comparing `tmp/pulse_eco-2.3.0.tar.gz` & `tmp/pulse_eco-2.3.1.tar.gz`

## Comparing `pulse_eco-2.3.0.tar` & `pulse_eco-2.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/_version.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/constants.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/enums.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/py.typed
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/utils.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/api/__init__.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/api/base.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/api/data_types.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/api/http_clients.py
--rw-r--r--   0        0        0    15846 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/api/pulse_eco_api.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/client/__init__.py
--rw-r--r--   0        0        0     8690 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/client/client.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/client/enums.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pulseeco/client/models.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/LICENSE
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/README.md
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/hatch.toml
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 pulse_eco-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/_version.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/constants.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/enums.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/py.typed
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/utils.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/api/__init__.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/api/base.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/api/data_types.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/api/http_clients.py
+-rw-r--r--   0        0        0    15846 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/api/pulse_eco_api.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/client/__init__.py
+-rw-r--r--   0        0        0     8690 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/client/client.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/client/enums.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pulseeco/client/models.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/LICENSE
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/README.md
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/hatch.toml
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 pulse_eco-2.3.1/PKG-INFO
```

### Comparing `pulse_eco-2.3.0/pulseeco/__init__.py` & `pulse_eco-2.3.1/pulseeco/__init__.py`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/pulseeco/constants.py` & `pulse_eco-2.3.1/pulseeco/constants.py`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/pulseeco/utils.py` & `pulse_eco-2.3.1/pulseeco/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,9 +31,10 @@
     if isinstance(to, str):
         to = datetime.fromisoformat(to)
     current = fr
     prev = current
     while current + td < to:
         current += td
         yield prev, current
-        prev = current + timedelta(seconds=1)
-    yield prev, to
+        prev = current = current + timedelta(seconds=1)
+    if prev < to:
+        yield prev, to
```

### Comparing `pulse_eco-2.3.0/pulseeco/api/base.py` & `pulse_eco-2.3.1/pulseeco/api/base.py`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/pulseeco/api/data_types.py` & `pulse_eco-2.3.1/pulseeco/api/data_types.py`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/pulseeco/api/http_clients.py` & `pulse_eco-2.3.1/pulseeco/api/http_clients.py`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/pulseeco/api/pulse_eco_api.py` & `pulse_eco-2.3.1/pulseeco/api/pulse_eco_api.py`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/pulseeco/client/client.py` & `pulse_eco-2.3.1/pulseeco/client/client.py`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/pulseeco/client/enums.py` & `pulse_eco-2.3.1/pulseeco/client/enums.py`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/pulseeco/client/models.py` & `pulse_eco-2.3.1/pulseeco/client/models.py`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/.gitignore` & `pulse_eco-2.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/LICENSE` & `pulse_eco-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/README.md` & `pulse_eco-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/hatch.toml` & `pulse_eco-2.3.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/pyproject.toml` & `pulse_eco-2.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulse_eco-2.3.0/PKG-INFO` & `pulse_eco-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulse-eco
-Version: 2.3.0
+Version: 2.3.1
 Summary: pulse.eco API wrapper
 Project-URL: Bug Tracker, https://github.com/martinkozle/pulse-eco/issues
 Project-URL: Homepage, https://github.com/martinkozle/pulse-eco
 Author-email: martinkozle <martinkozle@yahoo.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: air,air pollution,air quality index,api,aqi,eco,pollution,pulse,pulse.eco,python,quality,wrapper
```

