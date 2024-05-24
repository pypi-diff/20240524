# Comparing `tmp/airbyte_source_intercom-0.6.5.tar.gz` & `tmp/airbyte_source_intercom-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_intercom-0.6.5.tar", max compression
+gzip compressed data, was "airbyte_source_intercom-0.6.6.tar", max compression
```

## Comparing `airbyte_source_intercom-0.6.5.tar` & `airbyte_source_intercom-0.6.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4547 2024-05-10 09:07:02.694307 airbyte_source_intercom-0.6.5/README.md
--rw-r--r--   0        0        0      763 2024-05-10 09:11:43.464599 airbyte_source_intercom-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      128 2024-05-10 09:07:02.694307 airbyte_source_intercom-0.6.5/source_intercom/__init__.py
--rw-r--r--   0        0        0    19417 2024-05-10 09:07:02.694307 airbyte_source_intercom-0.6.5/source_intercom/components.py
--rw-r--r--   0        0        0    78469 2024-05-10 09:07:02.694307 airbyte_source_intercom-0.6.5/source_intercom/manifest.yaml
--rw-r--r--   0        0        0      236 2024-05-10 09:07:02.694307 airbyte_source_intercom-0.6.5/source_intercom/run.py
--rw-r--r--   0        0        0      477 2024-05-10 09:07:02.694307 airbyte_source_intercom-0.6.5/source_intercom/source.py
--rw-r--r--   0        0        0     2431 2024-05-10 09:07:02.694307 airbyte_source_intercom-0.6.5/source_intercom/spec.json
--rw-r--r--   0        0        0     5262 1970-01-01 00:00:00.000000 airbyte_source_intercom-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     4547 2024-05-24 08:51:40.605024 airbyte_source_intercom-0.6.6/README.md
+-rw-r--r--   0        0        0      763 2024-05-24 08:58:24.261637 airbyte_source_intercom-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-05-24 08:51:40.609024 airbyte_source_intercom-0.6.6/source_intercom/__init__.py
+-rw-r--r--   0        0        0    19417 2024-05-24 08:51:40.609024 airbyte_source_intercom-0.6.6/source_intercom/components.py
+-rw-r--r--   0        0        0    78514 2024-05-24 08:51:40.609024 airbyte_source_intercom-0.6.6/source_intercom/manifest.yaml
+-rw-r--r--   0        0        0      236 2024-05-24 08:51:40.609024 airbyte_source_intercom-0.6.6/source_intercom/run.py
+-rw-r--r--   0        0        0      477 2024-05-24 08:51:40.609024 airbyte_source_intercom-0.6.6/source_intercom/source.py
+-rw-r--r--   0        0        0     2853 2024-05-24 08:51:40.609024 airbyte_source_intercom-0.6.6/source_intercom/spec.json
+-rw-r--r--   0        0        0     5262 1970-01-01 00:00:00.000000 airbyte_source_intercom-0.6.6/PKG-INFO
```

### Comparing `airbyte_source_intercom-0.6.5/README.md` & `airbyte_source_intercom-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_intercom-0.6.5/pyproject.toml` & `airbyte_source_intercom-0.6.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.6.5"
+version = "0.6.6"
 name = "airbyte-source-intercom"
 description = "Source implementation for Intercom Yaml."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_intercom-0.6.5/source_intercom/components.py` & `airbyte_source_intercom-0.6.6/source_intercom/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_intercom-0.6.5/source_intercom/manifest.yaml` & `airbyte_source_intercom-0.6.6/source_intercom/manifest.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2304,15 +2304,15 @@
     incremental_sync:
       type: DatetimeBasedCursor
       cursor_field: created_at
       cursor_datetime_formats:
         - "%s"
       datetime_format: "%s"
       cursor_granularity: "PT1S"
-      step: "P30D"
+      step: "P{{ config.get('activity_logs_time_step', 30) }}D"
       start_datetime:
         datetime: "{{ config['start_date'] }}"
         datetime_format: "%Y-%m-%dT%H:%M:%SZ"
       end_time_option:
         field_name: "created_at_before"
         inject_into: "request_parameter"
       start_time_option:
```

### Comparing `airbyte_source_intercom-0.6.5/source_intercom/spec.json` & `airbyte_source_intercom-0.6.6/source_intercom/spec.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963888888888889%*

 * *Differences: {"'connectionSpecification'": "{'properties': {'access_token': {'order': 0}, 'client_id': "*

 * *                              "{'order': 1}, 'client_secret': {'order': 2}, "*

 * *                              "'activity_logs_time_step': OrderedDict([('type', 'integer'), "*

 * *                              "('default', 30), ('minimum', 1), ('maximum', 91), ('title', "*

 * *                              "'Activity logs stream slice step size (in days)'), ('description', "*

 * *                              "'Set lower value in case […]*

```diff
@@ -46,26 +46,43 @@
     "connectionSpecification": {
         "$schema": "http://json-schema.org/draft-07/schema#",
         "additionalProperties": true,
         "properties": {
             "access_token": {
                 "airbyte_secret": true,
                 "description": "Access token for making authenticated requests. See the <a href=\"https://developers.intercom.com/building-apps/docs/authentication-types#how-to-get-your-access-token\">Intercom docs</a> for more information.",
+                "order": 0,
                 "title": "Access token",
                 "type": "string"
             },
+            "activity_logs_time_step": {
+                "default": 30,
+                "description": "Set lower value in case of failing long running sync of Activity Logs stream.",
+                "examples": [
+                    30,
+                    10,
+                    5
+                ],
+                "maximum": 91,
+                "minimum": 1,
+                "order": 3,
+                "title": "Activity logs stream slice step size (in days)",
+                "type": "integer"
+            },
             "client_id": {
                 "airbyte_secret": true,
                 "description": "Client Id for your Intercom application.",
+                "order": 1,
                 "title": "Client Id",
                 "type": "string"
             },
             "client_secret": {
                 "airbyte_secret": true,
                 "description": "Client Secret for your Intercom application.",
+                "order": 2,
                 "title": "Client Secret",
                 "type": "string"
             },
             "start_date": {
                 "description": "UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated.",
                 "examples": [
                     "2020-11-16T00:00:00Z"
```

### Comparing `airbyte_source_intercom-0.6.5/PKG-INFO` & `airbyte_source_intercom-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-intercom
-Version: 0.6.5
+Version: 0.6.6
 Summary: Source implementation for Intercom Yaml.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

