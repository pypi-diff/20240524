# Comparing `tmp/brynq_sdk_elastic-1.0.0.tar.gz` & `tmp/brynq_sdk_elastic-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brynq_sdk_elastic-1.0.0.tar", last modified: Thu Apr 25 10:04:28 2024, max compression
+gzip compressed data, was "dist/brynq_sdk_elastic-2.0.0.tar", last modified: Fri May 24 07:28:42 2024, max compression
```

## Comparing `brynq_sdk_elastic-1.0.0.tar` & `brynq_sdk_elastic-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:04:28.000000 brynq_sdk_elastic-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      243 2024-04-25 10:04:28.000000 brynq_sdk_elastic-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:04:28.000000 brynq_sdk_elastic-1.0.0/brynq_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:04:28.000000 brynq_sdk_elastic-1.0.0/brynq_sdk/elastic/
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-04-25 10:04:11.000000 brynq_sdk_elastic-1.0.0/brynq_sdk/elastic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16202 2024-04-25 10:04:11.000000 brynq_sdk_elastic-1.0.0/brynq_sdk/elastic/elastic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:04:28.000000 brynq_sdk_elastic-1.0.0/brynq_sdk_elastic.egg-info/
--rw-r--r--   0 root         (0) root         (0)      243 2024-04-25 10:04:28.000000 brynq_sdk_elastic-1.0.0/brynq_sdk_elastic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      311 2024-04-25 10:04:28.000000 brynq_sdk_elastic-1.0.0/brynq_sdk_elastic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 10:04:28.000000 brynq_sdk_elastic-1.0.0/brynq_sdk_elastic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 10:04:28.000000 brynq_sdk_elastic-1.0.0/brynq_sdk_elastic.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       32 2024-04-25 10:04:28.000000 brynq_sdk_elastic-1.0.0/brynq_sdk_elastic.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-25 10:04:28.000000 brynq_sdk_elastic-1.0.0/brynq_sdk_elastic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 10:04:28.000000 brynq_sdk_elastic-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-04-25 10:04:11.000000 brynq_sdk_elastic-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:28:42.000000 brynq_sdk_elastic-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      243 2024-05-24 07:28:42.000000 brynq_sdk_elastic-2.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:28:42.000000 brynq_sdk_elastic-2.0.0/brynq_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:28:42.000000 brynq_sdk_elastic-2.0.0/brynq_sdk/elastic/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-05-24 07:28:24.000000 brynq_sdk_elastic-2.0.0/brynq_sdk/elastic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17059 2024-05-24 07:28:24.000000 brynq_sdk_elastic-2.0.0/brynq_sdk/elastic/elastic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:28:42.000000 brynq_sdk_elastic-2.0.0/brynq_sdk_elastic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      243 2024-05-24 07:28:42.000000 brynq_sdk_elastic-2.0.0/brynq_sdk_elastic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      311 2024-05-24 07:28:42.000000 brynq_sdk_elastic-2.0.0/brynq_sdk_elastic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 07:28:42.000000 brynq_sdk_elastic-2.0.0/brynq_sdk_elastic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 07:28:42.000000 brynq_sdk_elastic-2.0.0/brynq_sdk_elastic.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-24 07:28:42.000000 brynq_sdk_elastic-2.0.0/brynq_sdk_elastic.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-24 07:28:42.000000 brynq_sdk_elastic-2.0.0/brynq_sdk_elastic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 07:28:42.000000 brynq_sdk_elastic-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-24 07:28:24.000000 brynq_sdk_elastic-2.0.0/setup.py
```

### Comparing `brynq_sdk_elastic-1.0.0/brynq_sdk/elastic/elastic.py` & `brynq_sdk_elastic-2.0.0/brynq_sdk/elastic/elastic.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 import requests
 import json
 import datetime
 import string
 import random
 import pandas as pd
 import os
@@ -11,25 +12,42 @@
     def __init__(self, api_key: str = None, customer_name: str = None, space_name: str = None):
         """
         A package to create indexes, users, roles, getting data, etc.
         :param api_key: The api key to connect to elasticsearch if not provided in the .env file
         """
         try:
             self.verify = False
-            if os.getenv('BRYNQ_ENVIRONMENT') == 'prod':
-                self.elasticsearch_host = f'https://{os.getenv("ELASTIC_HOST_LIVE", "localhost")}:{os.getenv("ELASTIC_PORT_LIVE", "9200")}'
-                self.kibana_host = f'http://{os.getenv("ELASTIC_HOST_LIVE", "localhost")}:{os.getenv("KIBANA_PORT_LIVE", "5601")}'
-                self.elastic_token = os.getenv('ELASTIC_API_KEY_LIVE', api_key)
-            else:
-                self.elasticsearch_host = f'https://{os.getenv("ELASTIC_HOST_STAGING", "localhost")}:{os.getenv("ELASTIC_PORT_STAGING", "9200")}'
-                self.kibana_host = f'http://{os.getenv("ELASTIC_HOST_STAGING", "localhost")}:{os.getenv("KIBANA_PORT_STAGING", "5601")}'
-                self.elastic_token = os.getenv('ELASTIC_API_KEY_STAGING', api_key)
+            elasticsearch_host = os.getenv("ELASTIC_HOST", "localhost")
+            elasticsearch_port = os.getenv("ELASTIC_PORT", "9200")
+            kibana_port = os.getenv("KIBANA_PORT", "5601")
+            elastic_token = os.getenv('ELASTIC_API_KEY', None)
 
-            self.client_user = os.getenv('BRYNQ_CUSTOMER_NAME', 'default').lower().replace(' ', '_') if customer_name is None else customer_name.lower().replace(' ', '_')
+            # Build the host URLs
+            self.elasticsearch_host = f'https://{elasticsearch_host}:{elasticsearch_port}'
+            self.kibana_host = f'http://{elasticsearch_host}:{kibana_port}'
+            self.elastic_token = elastic_token if elastic_token is not None else api_key
             self.space_name = os.getenv('ELASTIC_SPACE', 'default') if space_name is None else space_name
+            self.client_user = os.getenv('BRYNQ_SUBDOMAIN', 'default').lower().replace(' ', '_') if customer_name is None else customer_name.lower().replace(' ', '_')
+
+            # Check for missing environment variables and show warnings
+            if elasticsearch_host == "localhost":
+                warnings.warn("Environment variable ELASTIC_HOST is not set. Using default: localhost")
+            if elasticsearch_port == "9200":
+                warnings.warn("Environment variable ELASTIC_PORT is not set. Using default: 9200")
+            if kibana_port == "5601":
+                warnings.warn("Environment variable KIBANA_PORT is not set. Using default: 5601")
+            if elastic_token is None:
+                raise KeyError("Environment variable ELASTIC_API_KEY is not set and no api_key is provided. Please specify either one and try again")
+            if self.space_name == 'default':
+                warnings.warn("Environment variable ELASTIC_SPACE is not set. Using 'default'")
+            if self.client_user == 'default':
+                warnings.warn("Environment variable BRYNQ_SUBDOMAIN is not set and customer_name is not specified. Using 'default'")
+
+            print(f"Elasticsearch running on: {elasticsearch_host}")
+
             self.timestamp = int(datetime.datetime.now().timestamp())
             self.elastic_headers = {
                 'Content-Type': 'application/json',
                 'Authorization': f'ApiKey {self.elastic_token}'
             }
             self.kibana_headers = {
                 'Content-Type': 'application/json',
```

