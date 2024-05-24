# Comparing `tmp/credsmash-3.0.1.tar.gz` & `tmp/credsmash-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credsmash-3.0.1.tar", last modified: Wed May 22 21:42:09 2024, max compression
+gzip compressed data, was "credsmash-3.0.2.tar", last modified: Fri May 24 07:42:10 2024, max compression
```

## Comparing `credsmash-3.0.1.tar` & `credsmash-3.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-22 21:42:09.432509 credsmash-3.0.1/
--rw-r--r--   0 nathan    (1000) nathan    (1000)    11358 2018-05-16 01:54:08.000000 credsmash-3.0.1/LICENSE
--rw-r--r--   0 nathan    (1000) nathan    (1000)    16977 2024-05-22 21:42:09.432509 credsmash-3.0.1/PKG-INFO
--rw-r--r--   0 nathan    (1000) nathan    (1000)    15657 2018-05-16 01:54:08.000000 credsmash-3.0.1/README.md
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-22 21:42:09.428509 credsmash-3.0.1/credsmash/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        6 2024-05-22 21:41:49.000000 credsmash-3.0.1/credsmash/VERSION
--rwxrwxr-x   0 nathan    (1000) nathan    (1000)      734 2024-05-22 02:32:09.000000 credsmash-3.0.1/credsmash/__init__.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-22 21:42:09.428509 credsmash-3.0.1/credsmash/api/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      238 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/api/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      592 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/api/delete.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      491 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/api/get.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      158 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/api/list.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      776 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/api/prune.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1183 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/api/put.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    12966 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/cli.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      708 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/cli_dynamodb.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-22 21:42:09.432509 credsmash-3.0.1/credsmash/crypto/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1569 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/crypto/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5211 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/crypto/aes_ctr.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1982 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/crypto/aes_gcm.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5692 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/dynamodb_storage_service.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2114 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/kms_key_service.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     8699 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/templates.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     7088 2024-05-22 21:41:44.000000 credsmash-3.0.1/credsmash/util.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-22 21:42:09.432509 credsmash-3.0.1/credsmash.egg-info/
--rw-r--r--   0 nathan    (1000) nathan    (1000)    16977 2024-05-22 21:42:09.000000 credsmash-3.0.1/credsmash.egg-info/PKG-INFO
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      670 2024-05-22 21:42:09.000000 credsmash-3.0.1/credsmash.egg-info/SOURCES.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        1 2024-05-22 21:42:09.000000 credsmash-3.0.1/credsmash.egg-info/dependency_links.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      301 2024-05-22 21:42:09.000000 credsmash-3.0.1/credsmash.egg-info/entry_points.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      159 2024-05-22 21:42:09.000000 credsmash-3.0.1/credsmash.egg-info/requires.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       10 2024-05-22 21:42:09.000000 credsmash-3.0.1/credsmash.egg-info/top_level.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      171 2024-05-22 21:42:09.432509 credsmash-3.0.1/setup.cfg
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2300 2024-05-22 21:34:21.000000 credsmash-3.0.1/setup.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-22 21:42:09.432509 credsmash-3.0.1/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1941 2019-03-13 05:47:16.000000 credsmash-3.0.1/tests/test_crypto.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-24 07:42:10.656672 credsmash-3.0.2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)    11358 2018-05-16 01:54:08.000000 credsmash-3.0.2/LICENSE
+-rw-r--r--   0 nathan    (1000) nathan    (1000)    16977 2024-05-24 07:42:10.656672 credsmash-3.0.2/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)    15657 2018-05-16 01:54:08.000000 credsmash-3.0.2/README.md
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-24 07:42:10.652672 credsmash-3.0.2/credsmash/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        6 2024-05-24 07:40:53.000000 credsmash-3.0.2/credsmash/VERSION
+-rwxrwxr-x   0 nathan    (1000) nathan    (1000)      734 2024-05-22 02:32:09.000000 credsmash-3.0.2/credsmash/__init__.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-24 07:42:10.656672 credsmash-3.0.2/credsmash/api/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      238 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/api/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      592 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/api/delete.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      491 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/api/get.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      158 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/api/list.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      776 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/api/prune.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1183 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/api/put.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    12966 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/cli.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      708 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/cli_dynamodb.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-24 07:42:10.656672 credsmash-3.0.2/credsmash/crypto/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1569 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/crypto/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5211 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/crypto/aes_ctr.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1982 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/crypto/aes_gcm.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5692 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/dynamodb_storage_service.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2114 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/kms_key_service.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     8699 2024-05-22 21:41:44.000000 credsmash-3.0.2/credsmash/templates.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     7098 2024-05-24 07:38:35.000000 credsmash-3.0.2/credsmash/util.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-24 07:42:10.656672 credsmash-3.0.2/credsmash.egg-info/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)    16977 2024-05-24 07:42:10.000000 credsmash-3.0.2/credsmash.egg-info/PKG-INFO
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      670 2024-05-24 07:42:10.000000 credsmash-3.0.2/credsmash.egg-info/SOURCES.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        1 2024-05-24 07:42:10.000000 credsmash-3.0.2/credsmash.egg-info/dependency_links.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      301 2024-05-24 07:42:10.000000 credsmash-3.0.2/credsmash.egg-info/entry_points.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      159 2024-05-24 07:42:10.000000 credsmash-3.0.2/credsmash.egg-info/requires.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       10 2024-05-24 07:42:10.000000 credsmash-3.0.2/credsmash.egg-info/top_level.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      171 2024-05-24 07:42:10.656672 credsmash-3.0.2/setup.cfg
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2300 2024-05-22 21:34:21.000000 credsmash-3.0.2/setup.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-24 07:42:10.656672 credsmash-3.0.2/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1941 2019-03-13 05:47:16.000000 credsmash-3.0.2/tests/test_crypto.py
```

### Comparing `credsmash-3.0.1/LICENSE` & `credsmash-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/PKG-INFO` & `credsmash-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsmash
-Version: 3.0.1
+Version: 3.0.2
 Summary: A utility for managing secrets in the cloud using AWS KMS and DynamoDB
 Home-page: https://github.com/3stack-software/credsmash
 Maintainer: Nathan Muir
 Maintainer-email: ndmuir@gmail.com
 License: Apache2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `credsmash-3.0.1/README.md` & `credsmash-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/credsmash/__init__.py` & `credsmash-3.0.2/credsmash/__init__.py`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/credsmash/api/delete.py` & `credsmash-3.0.2/credsmash/api/delete.py`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/credsmash/api/prune.py` & `credsmash-3.0.2/credsmash/api/prune.py`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/credsmash/api/put.py` & `credsmash-3.0.2/credsmash/api/put.py`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/credsmash/cli.py` & `credsmash-3.0.2/credsmash/cli.py`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/credsmash/cli_dynamodb.py` & `credsmash-3.0.2/credsmash/cli_dynamodb.py`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/credsmash/crypto/__init__.py` & `credsmash-3.0.2/credsmash/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/credsmash/crypto/aes_ctr.py` & `credsmash-3.0.2/credsmash/crypto/aes_ctr.py`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/credsmash/crypto/aes_gcm.py` & `credsmash-3.0.2/credsmash/crypto/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/credsmash/dynamodb_storage_service.py` & `credsmash-3.0.2/credsmash/dynamodb_storage_service.py`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/credsmash/kms_key_service.py` & `credsmash-3.0.2/credsmash/kms_key_service.py`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/credsmash/templates.py` & `credsmash-3.0.2/credsmash/templates.py`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/credsmash/util.py` & `credsmash-3.0.2/credsmash/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,30 +115,30 @@
             for entry in csvreader
         }
     if format == 'json':
         secrets = json.load(source)
     elif format == 'yaml':
         if not HAS_YAML:
             raise RuntimeError('YAML Module not loaded. Please install with `pip install credsmash[yaml]`')
-        secrets = yaml.load(source)
+        secrets = yaml.safe_load(source)
     else:
         raise RuntimeError('Unsupported format: %s' % format)
     if not isinstance(secrets, dict):
         raise RuntimeError('Unsupported type: %s', type(secrets))
     return secrets
 
 
 def parse_manifest(source, format):
     # type: (...) -> List[dict]
     if format == 'json':
         return json.load(source)
     if format == 'yaml':
         if not HAS_YAML:
             raise RuntimeError('YAML Module not loaded. Please install with `pip install credsmash[yaml]`')
-        return yaml.load(source)
+        return yaml.safe_load(source)
     raise RuntimeError('Unsupported format: %s' % format)
 
 
 def parse_config(fp):
     config = {}
     cp = configparser.RawConfigParser()
     if hasattr(cp, 'read_file'):
```

### Comparing `credsmash-3.0.1/credsmash.egg-info/PKG-INFO` & `credsmash-3.0.2/credsmash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsmash
-Version: 3.0.1
+Version: 3.0.2
 Summary: A utility for managing secrets in the cloud using AWS KMS and DynamoDB
 Home-page: https://github.com/3stack-software/credsmash
 Maintainer: Nathan Muir
 Maintainer-email: ndmuir@gmail.com
 License: Apache2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `credsmash-3.0.1/credsmash.egg-info/SOURCES.txt` & `credsmash-3.0.2/credsmash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/setup.py` & `credsmash-3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `credsmash-3.0.1/tests/test_crypto.py` & `credsmash-3.0.2/tests/test_crypto.py`

 * *Files identical despite different names*

