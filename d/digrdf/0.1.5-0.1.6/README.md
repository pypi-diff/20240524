# Comparing `tmp/digrdf-0.1.5.tar.gz` & `tmp/digrdf-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digrdf-0.1.5.tar", max compression
+gzip compressed data, was "digrdf-0.1.6.tar", max compression
```

## Comparing `digrdf-0.1.5.tar` & `digrdf-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1143 2024-05-03 05:56:07.796450 digrdf-0.1.5/README.md
--rw-r--r--   0        0        0       35 2024-05-03 02:30:07.231145 digrdf-0.1.5/digrdf/__init__.py
--rw-r--r--   0        0        0     5567 2024-05-17 06:40:47.789395 digrdf-0.1.5/digrdf/__main__.py
--rw-r--r--   0        0        0      101 2024-05-03 05:49:19.197611 digrdf-0.1.5/digrdf/instance_query.sparql
--rw-r--r--   0        0        0      703 2024-05-15 11:51:48.620609 digrdf-0.1.5/digrdf/prefixes.py
--rw-r--r--   0        0        0      289 2024-05-03 05:49:20.734434 digrdf-0.1.5/digrdf/schema_query.sparql
--rw-r--r--   0        0        0      409 2024-05-17 06:55:02.911094 digrdf-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 digrdf-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1139 2024-05-23 14:15:58.616664 digrdf-0.1.6/README.md
+-rw-r--r--   0        0        0       32 2024-05-23 11:53:28.672509 digrdf-0.1.6/digrdf/__init__.py
+-rw-r--r--   0        0        0     9250 2024-05-23 14:13:48.314127 digrdf-0.1.6/digrdf/__main__.py
+-rw-r--r--   0        0        0      187 2024-05-23 13:59:39.819260 digrdf-0.1.6/digrdf/instance_query.sparql
+-rw-r--r--   0        0        0      703 2024-05-15 11:51:48.620609 digrdf-0.1.6/digrdf/prefixes.py
+-rw-r--r--   0        0        0      316 2024-05-23 11:01:26.761882 digrdf-0.1.6/digrdf/schema_query.sparql
+-rw-r--r--   0        0        0      409 2024-05-23 14:16:54.995870 digrdf-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 digrdf-0.1.6/PKG-INFO
```

### Comparing `digrdf-0.1.5/README.md` & `digrdf-0.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -17,36 +17,36 @@
 ```
 
 ## Usage
 
 from the command line
 
 ```bash
-python -m digrdf -i myfiles/
+python -m digrdf -s myfiles/
 ```
 
 This will create a file called diagram.html in the working directory and open it for viewing.
 
 You can query any sparql endpoint as well.
 
 ```bash
-python -m digrdf -i "http://myserver.com/sparql"
+python -m digrdf -s "http://myserver.com/sparql"
 ```
 
 This will generate a schema diagram for all triples at that endpoint.
 
 > **warning** The query is intensive and may crash / timeout if the triple store has a lot of triples (like 1.0GB plus)
 
 You can also generate an instance level diagram for a particular iri
 
 ```bash
-python -m rdflib -i "http://myserver.com/sparql" -s "http://myserver.com/objects/1234"
+python -m rdflib -s "http://myserver.com/sparql" -i "http://myserver.com/objects/1234"
 ```
 
-where `-s` or `--subject` is a valid iri for an object in the triple store
+where `-i` or `--iri` is a valid iri for an object in the triple store
 
 
 To see all the cmdline options run
 
 ```bash
 python -m digrdf -h
 ```
```

### Comparing `digrdf-0.1.5/digrdf/prefixes.py` & `digrdf-0.1.6/digrdf/prefixes.py`

 * *Files identical despite different names*

### Comparing `digrdf-0.1.5/PKG-INFO` & `digrdf-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digrdf
-Version: 0.1.5
+Version: 0.1.6
 Summary: RDF Schema Diagram creation tool
 Author: Lawson Lewis
 Author-email: lawson@kurrawong.ai
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -31,36 +31,36 @@
 ```
 
 ## Usage
 
 from the command line
 
 ```bash
-python -m digrdf -i myfiles/
+python -m digrdf -s myfiles/
 ```
 
 This will create a file called diagram.html in the working directory and open it for viewing.
 
 You can query any sparql endpoint as well.
 
 ```bash
-python -m digrdf -i "http://myserver.com/sparql"
+python -m digrdf -s "http://myserver.com/sparql"
 ```
 
 This will generate a schema diagram for all triples at that endpoint.
 
 > **warning** The query is intensive and may crash / timeout if the triple store has a lot of triples (like 1.0GB plus)
 
 You can also generate an instance level diagram for a particular iri
 
 ```bash
-python -m rdflib -i "http://myserver.com/sparql" -s "http://myserver.com/objects/1234"
+python -m rdflib -s "http://myserver.com/sparql" -i "http://myserver.com/objects/1234"
 ```
 
-where `-s` or `--subject` is a valid iri for an object in the triple store
+where `-i` or `--iri` is a valid iri for an object in the triple store
 
 
 To see all the cmdline options run
 
 ```bash
 python -m digrdf -h
 ```
```

