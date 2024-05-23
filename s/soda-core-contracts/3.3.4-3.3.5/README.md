# Comparing `tmp/soda_core_contracts-3.3.4.tar.gz` & `tmp/soda_core_contracts-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core_contracts-3.3.4.tar", last modified: Tue May  7 23:39:56 2024, max compression
+gzip compressed data, was "soda_core_contracts-3.3.5.tar", last modified: Thu May 23 22:50:25 2024, max compression
```

## Comparing `soda_core_contracts-3.3.4.tar` & `soda_core_contracts-3.3.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:56.259951 soda_core_contracts-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-07 23:39:56.259951 soda_core_contracts-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:39:56.259951 soda_core_contracts-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:56.255951 soda_core_contracts-3.3.4/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:56.255951 soda_core_contracts-3.3.4/soda/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)    34525 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/soda/contracts/check.py
--rw-r--r--   0 runner    (1001) docker     (127)    24749 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/soda/contracts/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)    12454 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/soda/contracts/contract_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:56.259951 soda_core_contracts-3.3.4/soda/contracts/impl/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/soda/contracts/impl/consistent_hash_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/soda/contracts/impl/contract_verification_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/soda/contracts/impl/json_schema_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/soda/contracts/impl/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/soda/contracts/impl/soda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/soda/contracts/impl/variable_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/soda/contracts/impl/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/soda/contracts/impl/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12961 2024-05-07 23:39:42.000000 soda_core_contracts-3.3.4/soda/contracts/soda_data_contract_json_schema_1_0_0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:56.259951 soda_core_contracts-3.3.4/soda_core_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-07 23:39:56.000000 soda_core_contracts-3.3.4/soda_core_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-07 23:39:56.000000 soda_core_contracts-3.3.4/soda_core_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:39:56.000000 soda_core_contracts-3.3.4/soda_core_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 23:39:56.000000 soda_core_contracts-3.3.4/soda_core_contracts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 23:39:56.000000 soda_core_contracts-3.3.4/soda_core_contracts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:25.957929 soda_core_contracts-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-23 22:50:25.957929 soda_core_contracts-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:50:25.957929 soda_core_contracts-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:25.953929 soda_core_contracts-3.3.5/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:25.957929 soda_core_contracts-3.3.5/soda/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)    34525 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/soda/contracts/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24749 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/soda/contracts/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12454 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/soda/contracts/contract_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:25.957929 soda_core_contracts-3.3.5/soda/contracts/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/soda/contracts/impl/consistent_hash_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/soda/contracts/impl/contract_verification_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/soda/contracts/impl/json_schema_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/soda/contracts/impl/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/soda/contracts/impl/soda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/soda/contracts/impl/variable_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/soda/contracts/impl/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/soda/contracts/impl/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12961 2024-05-23 22:50:11.000000 soda_core_contracts-3.3.5/soda/contracts/soda_data_contract_json_schema_1_0_0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:25.957929 soda_core_contracts-3.3.5/soda_core_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-23 22:50:25.000000 soda_core_contracts-3.3.5/soda_core_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-23 22:50:25.000000 soda_core_contracts-3.3.5/soda_core_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:50:25.000000 soda_core_contracts-3.3.5/soda_core_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 22:50:25.000000 soda_core_contracts-3.3.5/soda_core_contracts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 22:50:25.000000 soda_core_contracts-3.3.5/soda_core_contracts.egg-info/top_level.txt
```

### Comparing `soda_core_contracts-3.3.4/soda/contracts/check.py` & `soda_core_contracts-3.3.5/soda/contracts/check.py`

 * *Files identical despite different names*

### Comparing `soda_core_contracts-3.3.4/soda/contracts/contract.py` & `soda_core_contracts-3.3.5/soda/contracts/contract.py`

 * *Files identical despite different names*

### Comparing `soda_core_contracts-3.3.4/soda/contracts/contract_verification.py` & `soda_core_contracts-3.3.5/soda/contracts/contract_verification.py`

 * *Files identical despite different names*

### Comparing `soda_core_contracts-3.3.4/soda/contracts/impl/consistent_hash_builder.py` & `soda_core_contracts-3.3.5/soda/contracts/impl/consistent_hash_builder.py`

 * *Files identical despite different names*

### Comparing `soda_core_contracts-3.3.4/soda/contracts/impl/contract_verification_impl.py` & `soda_core_contracts-3.3.5/soda/contracts/impl/contract_verification_impl.py`

 * *Files identical despite different names*

### Comparing `soda_core_contracts-3.3.4/soda/contracts/impl/json_schema_verifier.py` & `soda_core_contracts-3.3.5/soda/contracts/impl/json_schema_verifier.py`

 * *Files identical despite different names*

### Comparing `soda_core_contracts-3.3.4/soda/contracts/impl/logs.py` & `soda_core_contracts-3.3.5/soda/contracts/impl/logs.py`

 * *Files identical despite different names*

### Comparing `soda_core_contracts-3.3.4/soda/contracts/impl/soda_cloud.py` & `soda_core_contracts-3.3.5/soda/contracts/impl/soda_cloud.py`

 * *Files identical despite different names*

### Comparing `soda_core_contracts-3.3.4/soda/contracts/impl/variable_resolver.py` & `soda_core_contracts-3.3.5/soda/contracts/impl/variable_resolver.py`

 * *Files identical despite different names*

### Comparing `soda_core_contracts-3.3.4/soda/contracts/impl/warehouse.py` & `soda_core_contracts-3.3.5/soda/contracts/impl/warehouse.py`

 * *Files identical despite different names*

### Comparing `soda_core_contracts-3.3.4/soda/contracts/impl/yaml_helper.py` & `soda_core_contracts-3.3.5/soda/contracts/impl/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `soda_core_contracts-3.3.4/soda/contracts/soda_data_contract_json_schema_1_0_0.json` & `soda_core_contracts-3.3.5/soda/contracts/soda_data_contract_json_schema_1_0_0.json`

 * *Files identical despite different names*

### Comparing `soda_core_contracts-3.3.4/soda_core_contracts.egg-info/SOURCES.txt` & `soda_core_contracts-3.3.5/soda_core_contracts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

