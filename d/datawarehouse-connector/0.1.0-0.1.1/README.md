# Comparing `tmp/DATAWAREHOUSE_CONNECTOR-0.1.0.tar.gz` & `tmp/datawarehouse_connector-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DATAWAREHOUSE_CONNECTOR-0.1.0.tar", last modified: Fri May 24 11:40:49 2024, max compression
+gzip compressed data, was "datawarehouse_connector-0.1.1.tar", last modified: Fri May 24 12:43:20 2024, max compression
```

## Comparing `DATAWAREHOUSE_CONNECTOR-0.1.0.tar` & `datawarehouse_connector-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 11:40:49.057280 DATAWAREHOUSE_CONNECTOR-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-05-24 11:40:49.001800 DATAWAREHOUSE_CONNECTOR-0.1.0/DATAWAREHOUSE_CONNECTOR/
--rw-rw-rw-   0        0        0       36 2024-05-24 11:16:12.000000 DATAWAREHOUSE_CONNECTOR-0.1.0/DATAWAREHOUSE_CONNECTOR/__init__.py
--rw-rw-rw-   0        0        0     1964 2024-05-24 11:21:13.000000 DATAWAREHOUSE_CONNECTOR-0.1.0/DATAWAREHOUSE_CONNECTOR/connector.py
--rw-rw-rw-   0        0        0      306 2024-05-24 08:40:26.000000 DATAWAREHOUSE_CONNECTOR-0.1.0/DATAWAREHOUSE_CONNECTOR/constants.py
-drwxrwxrwx   0        0        0        0 2024-05-24 11:40:49.047398 DATAWAREHOUSE_CONNECTOR-0.1.0/DATAWAREHOUSE_CONNECTOR.egg-info/
--rw-rw-rw-   0        0        0      648 2024-05-24 11:40:48.000000 DATAWAREHOUSE_CONNECTOR-0.1.0/DATAWAREHOUSE_CONNECTOR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2024-05-24 11:40:48.000000 DATAWAREHOUSE_CONNECTOR-0.1.0/DATAWAREHOUSE_CONNECTOR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 11:40:48.000000 DATAWAREHOUSE_CONNECTOR-0.1.0/DATAWAREHOUSE_CONNECTOR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2024-05-24 11:40:48.000000 DATAWAREHOUSE_CONNECTOR-0.1.0/DATAWAREHOUSE_CONNECTOR.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-24 11:40:48.000000 DATAWAREHOUSE_CONNECTOR-0.1.0/DATAWAREHOUSE_CONNECTOR.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-05-22 10:02:14.000000 DATAWAREHOUSE_CONNECTOR-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      648 2024-05-24 11:40:49.054060 DATAWAREHOUSE_CONNECTOR-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      125 2024-05-24 11:22:56.000000 DATAWAREHOUSE_CONNECTOR-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 11:40:49.057280 DATAWAREHOUSE_CONNECTOR-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      901 2024-05-24 11:29:52.000000 DATAWAREHOUSE_CONNECTOR-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 12:43:20.120654 datawarehouse_connector-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2024-05-22 10:02:14.000000 datawarehouse_connector-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4116 2024-05-24 12:43:20.119666 datawarehouse_connector-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2729 2024-05-24 12:33:47.000000 datawarehouse_connector-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 12:43:20.076657 datawarehouse_connector-0.1.1/datawarehouse_connector/
+-rw-rw-rw-   0        0        0       36 2024-05-24 11:16:12.000000 datawarehouse_connector-0.1.1/datawarehouse_connector/__init__.py
+-rw-rw-rw-   0        0        0     1964 2024-05-24 11:21:13.000000 datawarehouse_connector-0.1.1/datawarehouse_connector/connector.py
+-rw-rw-rw-   0        0        0      306 2024-05-24 08:40:26.000000 datawarehouse_connector-0.1.1/datawarehouse_connector/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-24 12:43:20.113659 datawarehouse_connector-0.1.1/datawarehouse_connector.egg-info/
+-rw-rw-rw-   0        0        0     4116 2024-05-24 12:43:19.000000 datawarehouse_connector-0.1.1/datawarehouse_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2024-05-24 12:43:19.000000 datawarehouse_connector-0.1.1/datawarehouse_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 12:43:19.000000 datawarehouse_connector-0.1.1/datawarehouse_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2024-05-24 12:43:19.000000 datawarehouse_connector-0.1.1/datawarehouse_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-24 12:43:19.000000 datawarehouse_connector-0.1.1/datawarehouse_connector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 12:43:20.120654 datawarehouse_connector-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      901 2024-05-24 12:39:33.000000 datawarehouse_connector-0.1.1/setup.py
```

### Comparing `DATAWAREHOUSE_CONNECTOR-0.1.0/DATAWAREHOUSE_CONNECTOR/connector.py` & `datawarehouse_connector-0.1.1/datawarehouse_connector/connector.py`

 * *Files identical despite different names*

### Comparing `DATAWAREHOUSE_CONNECTOR-0.1.0/LICENSE` & `datawarehouse_connector-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DATAWAREHOUSE_CONNECTOR-0.1.0/setup.py` & `datawarehouse_connector-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
-    name='DATAWAREHOUSE_CONNECTOR',
-    version='0.1.0',
+    name='datawarehouse_connector',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'psycopg2-binary',
         'redshift-connector',
         'snowflake-connector-python',
         'snowflake-sqlalchemy',
         'SQLAlchemy',
```

