# Comparing `tmp/g3t-etl-0.0.1rc8.tar.gz` & `tmp/g3t-etl-0.0.1rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3t-etl-0.0.1rc8.tar", last modified: Thu Feb 29 06:25:29 2024, max compression
+gzip compressed data, was "g3t-etl-0.0.1rc9.tar", last modified: Thu Mar 28 22:16:17 2024, max compression
```

## Comparing `g3t-etl-0.0.1rc8.tar` & `g3t-etl-0.0.1rc9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-02-29 06:25:29.081909 g3t-etl-0.0.1rc8/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2670 2024-02-29 06:25:29.081543 g3t-etl-0.0.1rc8/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1825 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-02-29 06:25:29.053830 g3t-etl-0.0.1rc8/g3t_etl/
--rw-r--r--   0 walsbr   (320923486) 1971611142     8830 2024-02-21 21:45:41.000000 g3t-etl-0.0.1rc8/g3t_etl/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5296 2024-02-26 17:31:00.000000 g3t-etl-0.0.1rc8/g3t_etl/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    11325 2024-02-21 00:28:15.000000 g3t-etl-0.0.1rc8/g3t_etl/factory.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      628 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/g3t_etl/loader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3233 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/g3t_etl/submission_dictionary.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1180 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/g3t_etl/test_aced_etl.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-02-29 06:25:29.064664 g3t-etl-0.0.1rc8/g3t_etl/util/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-22 16:13:13.000000 g3t-etl-0.0.1rc8/g3t_etl/util/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     8656 2024-02-29 06:25:05.000000 g3t-etl-0.0.1rc8/g3t_etl/util/local_fhir_db.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-02-29 06:25:29.081047 g3t-etl-0.0.1rc8/g3t_etl.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2670 2024-02-29 06:25:28.000000 g3t-etl-0.0.1rc8/g3t_etl.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142      797 2024-02-29 06:25:29.000000 g3t-etl-0.0.1rc8/g3t_etl.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-02-29 06:25:28.000000 g3t-etl-0.0.1rc8/g3t_etl.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       44 2024-02-29 06:25:28.000000 g3t-etl-0.0.1rc8/g3t_etl.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       83 2024-02-29 06:25:28.000000 g3t-etl-0.0.1rc8/g3t_etl.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       33 2024-02-29 06:25:28.000000 g3t-etl-0.0.1rc8/g3t_etl.egg-info/top_level.txt
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-02-29 06:25:29.069423 g3t-etl-0.0.1rc8/sample_transformer/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/sample_transformer/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    19593 2024-02-28 02:46:27.000000 g3t-etl-0.0.1rc8/sample_transformer/submission.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     6803 2024-02-21 00:39:15.000000 g3t-etl-0.0.1rc8/sample_transformer/transformer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-02-29 06:25:29.081956 g3t-etl-0.0.1rc8/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5575 2024-02-29 06:25:16.000000 g3t-etl-0.0.1rc8/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-02-29 06:25:29.044609 g3t-etl-0.0.1rc8/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-02-29 06:25:29.073920 g3t-etl-0.0.1rc8/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      668 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1117 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/tests/integration/test_extract.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1311 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/tests/integration/test_transform.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-02-29 06:25:29.080640 g3t-etl-0.0.1rc8/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      343 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/tests/unit/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      596 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     6289 2024-02-29 06:01:49.000000 g3t-etl-0.0.1rc8/tests/unit/test_local_db.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      833 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc8/tests/unit/test_spreadsheet_json_schema.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-03-28 22:16:17.578636 g3t-etl-0.0.1rc9/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2670 2024-03-28 22:16:17.578161 g3t-etl-0.0.1rc9/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1825 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/README.md
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-03-28 22:16:17.526370 g3t-etl-0.0.1rc9/g3t_etl/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     8828 2024-03-28 15:39:40.000000 g3t-etl-0.0.1rc9/g3t_etl/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5507 2024-03-28 14:57:31.000000 g3t-etl-0.0.1rc9/g3t_etl/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    21004 2024-03-28 21:49:39.000000 g3t-etl-0.0.1rc9/g3t_etl/factory.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      628 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/g3t_etl/loader.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3233 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/g3t_etl/submission_dictionary.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1180 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/g3t_etl/test_aced_etl.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-03-28 22:16:17.548266 g3t-etl-0.0.1rc9/g3t_etl/util/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 16:13:13.000000 g3t-etl-0.0.1rc9/g3t_etl/util/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    11023 2024-03-01 16:29:17.000000 g3t-etl-0.0.1rc9/g3t_etl/util/local_fhir_db.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-03-28 22:16:17.577508 g3t-etl-0.0.1rc9/g3t_etl.egg-info/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2670 2024-03-28 22:16:17.000000 g3t-etl-0.0.1rc9/g3t_etl.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      797 2024-03-28 22:16:17.000000 g3t-etl-0.0.1rc9/g3t_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        1 2024-03-28 22:16:17.000000 g3t-etl-0.0.1rc9/g3t_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       44 2024-03-28 22:16:17.000000 g3t-etl-0.0.1rc9/g3t_etl.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       83 2024-03-28 22:16:17.000000 g3t-etl-0.0.1rc9/g3t_etl.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       33 2024-03-28 22:16:17.000000 g3t-etl-0.0.1rc9/g3t_etl.egg-info/top_level.txt
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-03-28 22:16:17.549877 g3t-etl-0.0.1rc9/sample_transformer/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/sample_transformer/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    19593 2024-02-28 02:46:27.000000 g3t-etl-0.0.1rc9/sample_transformer/submission.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     6803 2024-02-21 00:39:15.000000 g3t-etl-0.0.1rc9/sample_transformer/transformer.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       38 2024-03-28 22:16:17.578695 g3t-etl-0.0.1rc9/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5575 2024-03-28 22:16:08.000000 g3t-etl-0.0.1rc9/setup.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-03-28 22:16:17.508767 g3t-etl-0.0.1rc9/tests/
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-03-28 22:16:17.551708 g3t-etl-0.0.1rc9/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      668 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1117 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/tests/integration/test_extract.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1311 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/tests/integration/test_transform.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-03-28 22:16:17.576857 g3t-etl-0.0.1rc9/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      343 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/tests/unit/conftest.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      596 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      565 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     7450 2024-03-01 06:27:25.000000 g3t-etl-0.0.1rc9/tests/unit/test_local_db.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      833 2024-02-20 18:10:17.000000 g3t-etl-0.0.1rc9/tests/unit/test_spreadsheet_json_schema.py
```

### Comparing `g3t-etl-0.0.1rc8/PKG-INFO` & `g3t-etl-0.0.1rc9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3t-etl
-Version: 0.0.1rc8
+Version: 0.0.1rc9
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/g3t_etl.git
 Author: Ellrott Lab
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `g3t-etl-0.0.1rc8/README.md` & `g3t-etl-0.0.1rc9/README.md`

 * *Files identical despite different names*

### Comparing `g3t-etl-0.0.1rc8/g3t_etl/__init__.py` & `g3t-etl-0.0.1rc9/g3t_etl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,16 +106,14 @@
         if resource:
             _.reference = Reference(reference=f"{resource.resource_type}/{resource.id}")
         if concept:
             _.concept = concept
         assert _ and (_.reference or _.concept), f"Could not create CodeableReference from {resource} and {concept}"
         return _
 
-
-
     def populate_codeable_concept(self, code: str, display: str, system: str = None, text: str = None) -> CodeableConcept:
         """Populate a FHIR CodeableConcept."""
         if not text:
             text = display
         if not system or 'http' not in system:
             system = self.system
         return CodeableConcept(**{
```

### Comparing `g3t-etl-0.0.1rc8/g3t_etl/cli.py` & `g3t-etl-0.0.1rc9/g3t_etl/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,27 +57,32 @@
     Use this command to track changes to the data dictionary.
     INPUT_PATH: where to read master spreadsheet default: provided by plugin
     OUTPUT_PATH: where to write per subject csvs default: templates/submission.schema.json
     """
     try:
         if not input_path:
             input_path = factory.default_dictionary_path
+
         input_path = Path(input_path)
         assert input_path.exists(), f"Spreadsheet not found at {input_path},"\
                                     " please see README in docs/ for instructions."
         schema = spreadsheet_json_schema(input_path)
         output_path = Path(output_path)
         output_path.parent.mkdir(parents=True, exist_ok=True)
         with open(output_path, 'w') as fp:
             fp.write(orjson.dumps(schema, option=orjson.OPT_INDENT_2).decode())
 
         click.secho(f"Transformed {input_path} into jsonschema file in {output_path}",
                     fg='green', file=sys.stderr)
+        transformer_path = '<your_transformer>'
+        if len(factory.transformers) > 0:
+            transformer_path = factory.transformers[0].__module__.split('.')[0]
+
         cmd = f"datamodel-codegen  --input {output_path} --input-file-type jsonschema  "\
-              "--output sample_transformer/submission.py --field-extra-keys json_schema_extra"
+              f"--output {transformer_path}/submission.py --field-extra-keys json_schema_extra"
         click.secho("Use this command to generate pydantic model from schema (change paths depending on your environment):", fg='green', file=sys.stderr)
         print(cmd)
     except Exception as e:
         click.secho(f"Error parsing {input_path} into {output_path}: {e}", fg='red')
         if verbose:
             raise e
 
@@ -124,7 +129,11 @@
     \b
     INPUT_PATH: where to read FHIR  default: META/
     OUTPUT_PATH: where to write db.
     """
     db = LocalFHIRDatabase(db_name=pathlib.Path(output_path))
     db.load_ndjson_from_dir(input_path)
     click.secho(f"Exported {input_path} into {output_path}", fg='green', file=sys.stderr)
+
+
+if __name__ == '__main__':
+    cli()
```

### Comparing `g3t-etl-0.0.1rc8/g3t_etl/loader.py` & `g3t-etl-0.0.1rc9/g3t_etl/loader.py`

 * *Files identical despite different names*

### Comparing `g3t-etl-0.0.1rc8/g3t_etl/submission_dictionary.py` & `g3t-etl-0.0.1rc9/g3t_etl/submission_dictionary.py`

 * *Files identical despite different names*

### Comparing `g3t-etl-0.0.1rc8/g3t_etl/test_aced_etl.py` & `g3t-etl-0.0.1rc9/g3t_etl/test_aced_etl.py`

 * *Files identical despite different names*

### Comparing `g3t-etl-0.0.1rc8/g3t_etl/util/local_fhir_db.py` & `g3t-etl-0.0.1rc9/g3t_etl/util/local_fhir_db.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,121 @@
 import pathlib
 import sqlite3
 import json
-from typing import Generator
+from typing import Generator, Any
 
 import inflection
 import ndjson
 
 
+def is_related_observation(resource, related_resource):
+    """Check if the related resource is an observation linked to the resource."""
+    observation_links = [_['reference'] for _ in related_resource['focus']]
+    observation_links.extend([related_resource['subject']['reference']])
+    resource_type = resource['resourceType']
+    if f"{resource_type}/{resource['id']}" not in observation_links:
+        return False
+    return True
+
+
+def observation_value(related_resource) -> tuple[str, Any]:
+    """Return the code  and value of the observation."""
+    # TODO - pick first coding, h2 allow user to specify preferred coding
+    code = related_resource['code']['coding'][0]['code']
+    if 'valueQuantity' in related_resource:
+        value = related_resource['valueQuantity']['value']
+    elif 'valueCodeableConcept' in related_resource:
+        value = related_resource['valueCodeableConcept']['text']
+    elif 'valueInteger' in related_resource:
+        value = related_resource['valueInteger']
+    elif 'valueString' in related_resource:
+        value = related_resource['valueString']
+    else:
+        value = None
+    assert value is not None, f"no value for {related_resource['id']}"
+    return code, value
+
+
+def only_scalars(resource: dict) -> dict:
+    """Return only the scalar values from the resource."""
+    resource_type = resource['resourceType']
+    resource_type = inflection.underscore(resource_type)
+    skip = ['id', 'resource_type', 'resourceType']
+    _ = {f"{resource_type}_{k}": v for k, v in resource.items() if not isinstance(v, (dict, list)) and k not in skip}
+    if 'identifier' in resource:
+        if isinstance(resource['identifier'], list):
+            identifier = resource['identifier'][0]
+        else:
+            identifier = resource['identifier']
+        if isinstance(identifier, dict):
+            _['identifier'] = identifier['value']
+        else:
+            _['identifier'] = identifier
+    return _
+
+
+def simplify_patient(patient: dict) -> dict[str, Any]:
+    return only_scalars(patient)
+
+
+def simplify_condition(condition: dict) -> dict[str, Any]:
+    _ = only_scalars(condition)
+    _['condition_code'] = condition['code']['text']
+    if 'onsetAge' in condition:
+        _['condition_onsetAge'] = condition['onsetAge']['value']
+    return _
+
+
+def simplify_procedure(procedure) -> dict[str, Any]:
+    _ = only_scalars(procedure)
+    _.update({
+        'procedure_code': procedure['code']['coding'][0]['display'],
+        # 'procedure_reason': procedure['reason'][0]['reference']['reference'],
+        'procedure_occurrenceAge': procedure['occurrenceAge']['value']
+    })
+    return _
+
+
+def simplify_related_resource(resource, related_resource, skipped=['ResearchSubject']) -> dict[str, Any]:
+    """Simplify the related resource, returns a dict to apply to resource.
+
+    resource: is the fhir object that is being simplified, not modified in this call
+    related_resource: is the fhir object that is related to resource
+    returns a dict of the simplified related resource
+    """
+    simplified = {}
+    skipped.append(resource['resourceType'])
+
+    if related_resource['resourceType'] == 'Patient':
+        simplified.update(simplify_patient(related_resource))
+
+    elif related_resource['resourceType'] == 'Procedure':
+        simplified.update(simplify_procedure(related_resource))
+
+    elif related_resource['resourceType'] == 'Condition':
+        if f"Condition/{related_resource['id']}" == resource.get('reason', None):
+            simplified.update(simplify_condition(related_resource))
+        if related_resource['subject']['reference'] == f"{resource['resourceType']}/{resource['id']}":
+            simplified.update(simplify_condition(related_resource))
+
+    elif related_resource['resourceType'] == 'Observation':
+        if is_related_observation(resource, related_resource):
+            code, value = observation_value(related_resource)
+            simplified[code] = value
+
+    # skip these
+    elif related_resource['resourceType'] not in skipped:
+        # un-anticipated resource type
+        assert False, f"Unexpected resource type {related_resource['resourceType']}"
+
+    return simplified
+
+
 class LocalFHIRDatabase:
+    """Local FHIR Database.  This is a simple wrapper around sqlite3 to store FHIR resources.  It is used to store FHIR data"""
     def __init__(self, db_name):  # , db_name=pathlib.Path('.g3t') / 'local.db'):
         self.db_name = db_name
         self.connection = None
         self.cursor = None
         self.table_created = {}  # Flag to track if the table has been created
 
     def connect(self) -> sqlite3.Cursor:
@@ -134,80 +238,45 @@
     def patient(self, patient_id) -> dict:
         """Return the patient resource."""
         cursor = self.connection.cursor()
         cursor.execute("SELECT * FROM resources WHERE json_extract(resource, '$.id') = ?", (patient_id,))
         key, resource_type, resource = cursor.fetchone()
         return json.loads(resource)
 
-    def flattened_procedure(self) -> Generator[dict, None, None]:
-        """Return all the procedures with everything resolved"""
+    def flatten(self, resource_type: str) -> Generator[dict, None, None]:
+        """Return all resources of type resource_type, flattened with relationships resolved"""
         loaded_db = self
-        connection = sqlite3.connect(loaded_db.db_name)
-        cursor = connection.cursor()
-        cursor.execute("SELECT * FROM resources where resource_type = ?", ("Procedure",))
+        cursor = self.connection.cursor()
+        cursor.execute("SELECT key, resource_type, resource FROM resources where resource_type = ?", (resource_type,))
 
         for _ in cursor.fetchall():
-            key, resource_type, procedure = _
-            procedure = json.loads(procedure)
+            key, resource_type, resource = _
+            resource = json.loads(resource)
+
             # simplify the identifier
-            procedure['identifier'] = procedure['identifier'][0]['value']
-            # simplify the code
-            procedure['code'] = procedure['code']['coding'][0]['display']
-            # simplify the reason
-            procedure['reason'] = procedure['reason'][0]['reference']['reference']
-            # simplify the occurrenceAge
-            procedure['occurrenceAge'] = procedure['occurrenceAge']['value']
+            resource['identifier'] = resource['identifier'][0]['value']
+
+            if resource_type == 'Procedure':
+                for k, v in simplify_procedure(resource).items():
+                    resource[k] = v
+
             # simplify the subject
-            subject = procedure['subject']['reference']
-            procedure['subject'] = subject
+            subject = None
+            if 'subject' in resource:
+                subject = resource['subject']['reference']
+                resource['subject'] = subject
+
+            if resource_type == 'Patient':
+                subject = f"Patient/{resource['id']}"
+
+            if subject and subject.startswith('Patient/'):
 
-            if subject.startswith('Patient/'):
                 _, patient_id = subject.split('/')
                 resources = [_ for _ in loaded_db.patient_everything(patient_id)]
                 resources.append(loaded_db.patient(patient_id))
-                for resource in resources:
 
-                    if resource['resourceType'] == 'Patient':
-                        procedure['patient'] = resource['identifier'][0]['value']
-                        continue
-
-                    if resource['resourceType'] == 'Condition' and f"Condition/{resource['id']}" == procedure['reason']:
-                        procedure['reason'] = resource['code']['text']
-                        continue
-
-                    if resource['resourceType'] == 'Observation':
-                        # must be focus
-                        if f"Procedure/{procedure['id']}" not in [_['reference'] for _ in resource['focus']]:
-                            continue
-
-                        # TODO - pick first coding, h2 allow user to specify preferred coding
-                        code = resource['code']['coding'][0]['code']
-
-                        if 'valueQuantity' in resource:
-                            value = resource['valueQuantity']['value']
-                        elif 'valueCodeableConcept' in resource:
-                            value = resource['valueCodeableConcept']['text']
-                        elif 'valueInteger' in resource:
-                            value = resource['valueInteger']
-                        elif 'valueString' in resource:
-                            value = resource['valueString']
-                        else:
-                            value = None
-
-                        assert value is not None, f"no value for {resource['id']}"
-                        procedure[code] = value
-
-                        continue
-
-                    # skip these
-                    if resource['resourceType'] in ['Specimen', 'Procedure', 'ResearchSubject']:
-                        continue
-
-                    # default, add entire resource as an item of the list
-                    resource_type = inflection.underscore(resource['resourceType'])
-                    if resource_type not in procedure:
-                        procedure[resource_type] = []
-                    procedure[resource_type].append(resource)
+                for related_resource in resources:
 
-            yield procedure
+                    for k, v in simplify_related_resource(resource, related_resource).items():
+                        resource[k] = v
 
-        connection.close()
+            yield resource
```

### Comparing `g3t-etl-0.0.1rc8/g3t_etl.egg-info/PKG-INFO` & `g3t-etl-0.0.1rc9/g3t_etl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3t-etl
-Version: 0.0.1rc8
+Version: 0.0.1rc9
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/g3t_etl.git
 Author: Ellrott Lab
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `g3t-etl-0.0.1rc8/g3t_etl.egg-info/SOURCES.txt` & `g3t-etl-0.0.1rc9/g3t_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g3t-etl-0.0.1rc8/sample_transformer/submission.py` & `g3t-etl-0.0.1rc9/sample_transformer/submission.py`

 * *Files identical despite different names*

### Comparing `g3t-etl-0.0.1rc8/sample_transformer/transformer.py` & `g3t-etl-0.0.1rc9/sample_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `g3t-etl-0.0.1rc8/setup.py` & `g3t-etl-0.0.1rc9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='g3t-etl',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.1rc8',  # Required
+    version='0.0.1rc9',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `g3t-etl-0.0.1rc8/tests/integration/conftest.py` & `g3t-etl-0.0.1rc9/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `g3t-etl-0.0.1rc8/tests/integration/test_extract.py` & `g3t-etl-0.0.1rc9/tests/integration/test_extract.py`

 * *Files identical despite different names*

### Comparing `g3t-etl-0.0.1rc8/tests/integration/test_transform.py` & `g3t-etl-0.0.1rc9/tests/integration/test_transform.py`

 * *Files identical despite different names*

### Comparing `g3t-etl-0.0.1rc8/tests/unit/test_cli.py` & `g3t-etl-0.0.1rc9/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `g3t-etl-0.0.1rc8/tests/unit/test_coding_conventions.py` & `g3t-etl-0.0.1rc9/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `g3t-etl-0.0.1rc8/tests/unit/test_local_db.py` & `g3t-etl-0.0.1rc9/tests/unit/test_local_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -140,14 +140,19 @@
 
 @pytest.fixture
 def patient_expected_resource_count():
     return 185
 
 
 @pytest.fixture
+def patient_count():
+    return 30
+
+
+@pytest.fixture
 def procedure_expected_resource_count():
     return 160
 
 
 def test_load_from_dir(loaded_db, expected_count):
     """Check if the data from the NDJSON files has been inserted into the database"""
     connection = sqlite3.connect(loaded_db.db_name)
@@ -174,20 +179,40 @@
 
     assert patient_id == patient['id'], f"Expected {patient_id}, got {patient['id']}"
 
 
 def test_procedure_everything(loaded_db, procedure_expected_resource_count):
     """Normalize, patient, condition and observation connected to procedure."""
 
-    c = loaded_db.bulk_insert_data(loaded_db.flattened_procedure(), table_name="procedure_everything")
+    c = loaded_db.bulk_insert_data(loaded_db.flatten(resource_type="Procedure"), table_name="procedure_everything")
     assert c == procedure_expected_resource_count, f"Expected {procedure_expected_resource_count}, got {c}"
     loaded_db.disconnect()
     assert loaded_db.count() > 0, "No data loaded from NDJSON file."
     assert loaded_db.count(table_name="procedure_everything") > 0, "No data loaded into procedure_everything."
     (resource, ) = loaded_db.connection.cursor().execute("SELECT resource FROM procedure_everything").fetchone()
     assert resource is not None, "No data loaded into procedure_everything."
     resource = json.loads(resource)
     assert 'id' in resource, "No id in resource"
     assert 'code' in resource, "No code in resource"
     assert 'gleason' in resource.keys(), "No gleason in resource"
     assert 'reason' in resource.keys(), "No reason in resource"
     assert isinstance(resource['reason'], str), "reason is not a string"
+
+
+def test_patient_everything(loaded_db, patient_count):
+    """Normalize, patient, etc connected to procedure."""
+
+    c = loaded_db.bulk_insert_data(loaded_db.flatten(resource_type="Patient"), table_name="patient_everything")
+    assert c == patient_count, f"Expected {patient_count}, got {c}"
+    loaded_db.disconnect()
+    assert loaded_db.count() > 0, "No data loaded from NDJSON file."
+    assert loaded_db.count(table_name="patient_everything") > 0, "No data loaded into patient_everything."
+    (resource, ) = loaded_db.connection.cursor().execute("SELECT resource FROM patient_everything").fetchone()
+    assert resource is not None, "No data loaded into procedure_everything."
+    resource = json.loads(resource)
+    assert 'id' in resource, "No id in resource"
+    # assert 'code' in resource, "No code in resource"
+    # assert 'gleason' in resource.keys(), "No gleason in resource"
+    # assert 'reason' in resource.keys(), "No reason in resource"
+    # assert isinstance(resource['reason'], str), "reason is not a string"
+    print(json.dumps(resource, indent=2))
+    assert False
```

### Comparing `g3t-etl-0.0.1rc8/tests/unit/test_spreadsheet_json_schema.py` & `g3t-etl-0.0.1rc9/tests/unit/test_spreadsheet_json_schema.py`

 * *Files identical despite different names*

