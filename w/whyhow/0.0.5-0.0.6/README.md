# Comparing `tmp/whyhow-0.0.5.tar.gz` & `tmp/whyhow-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyhow-0.0.5.tar", last modified: Tue May  7 04:21:22 2024, max compression
+gzip compressed data, was "whyhow-0.0.6.tar", last modified: Fri May 24 04:58:46 2024, max compression
```

## Comparing `whyhow-0.0.5.tar` & `whyhow-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.673420 whyhow-0.0.5/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     7907 2024-05-07 04:21:22.673212 whyhow-0.0.5/PKG-INFO
--rw-r--r--   0 tomsmoker   (501) staff       (20)     6778 2024-05-07 03:43:17.000000 whyhow-0.0.5/README.md
--rw-r--r--   0 tomsmoker   (501) staff       (20)     2061 2024-05-07 03:43:17.000000 whyhow-0.0.5/pyproject.toml
--rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-05-07 04:21:22.673464 whyhow-0.0.5/setup.cfg
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.666854 whyhow-0.0.5/src/
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.668275 whyhow-0.0.5/src/whyhow/
--rw-r--r--   0 tomsmoker   (501) staff       (20)      125 2024-05-07 03:43:27.000000 whyhow-0.0.5/src/whyhow/__init__.py
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.669967 whyhow-0.0.5/src/whyhow/apis/
--rw-r--r--   0 tomsmoker   (501) staff       (20)       49 2024-03-30 23:23:35.000000 whyhow-0.0.5/src/whyhow/apis/__init__.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      501 2024-04-04 06:55:34.000000 whyhow-0.0.5/src/whyhow/apis/base.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     5024 2024-05-07 03:43:17.000000 whyhow-0.0.5/src/whyhow/apis/graph.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     6707 2024-04-21 01:37:48.000000 whyhow-0.0.5/src/whyhow/client.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      166 2024-03-30 23:23:35.000000 whyhow-0.0.5/src/whyhow/exceptions.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)        0 2024-03-30 23:23:35.000000 whyhow-0.0.5/src/whyhow/py.typed
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.671265 whyhow-0.0.5/src/whyhow/schemas/
--rw-r--r--   0 tomsmoker   (501) staff       (20)      189 2024-03-30 23:23:35.000000 whyhow-0.0.5/src/whyhow/schemas/__init__.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      624 2024-03-30 23:23:35.000000 whyhow-0.0.5/src/whyhow/schemas/base.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     5002 2024-05-07 03:43:17.000000 whyhow-0.0.5/src/whyhow/schemas/common.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     2110 2024-05-07 03:43:17.000000 whyhow-0.0.5/src/whyhow/schemas/graph.py
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.672135 whyhow-0.0.5/src/whyhow.egg-info/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     7907 2024-05-07 04:21:22.000000 whyhow-0.0.5/src/whyhow.egg-info/PKG-INFO
--rw-r--r--   0 tomsmoker   (501) staff       (20)      548 2024-05-07 04:21:22.000000 whyhow-0.0.5/src/whyhow.egg-info/SOURCES.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-05-07 04:21:22.000000 whyhow-0.0.5/src/whyhow.egg-info/dependency_links.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-31 17:56:30.000000 whyhow-0.0.5/src/whyhow.egg-info/not-zip-safe
--rw-r--r--   0 tomsmoker   (501) staff       (20)      218 2024-05-07 04:21:22.000000 whyhow-0.0.5/src/whyhow.egg-info/requires.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        7 2024-05-07 04:21:22.000000 whyhow-0.0.5/src/whyhow.egg-info/top_level.txt
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-07 04:21:22.671803 whyhow-0.0.5/tests/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     1431 2024-05-07 03:43:17.000000 whyhow-0.0.5/tests/test_client.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)       48 2024-03-30 23:23:35.000000 whyhow-0.0.5/tests/test_dummy.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.662514 whyhow-0.0.6/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     8677 2024-05-24 04:58:46.662273 whyhow-0.0.6/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     7548 2024-05-24 04:57:29.000000 whyhow-0.0.6/README.md
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     2061 2024-05-07 03:43:17.000000 whyhow-0.0.6/pyproject.toml
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-05-24 04:58:46.662553 whyhow-0.0.6/setup.cfg
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.656150 whyhow-0.0.6/src/
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.657557 whyhow-0.0.6/src/whyhow/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      125 2024-05-24 04:57:51.000000 whyhow-0.0.6/src/whyhow/__init__.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.659309 whyhow-0.0.6/src/whyhow/apis/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       49 2024-03-30 23:23:35.000000 whyhow-0.0.6/src/whyhow/apis/__init__.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      501 2024-04-04 06:55:34.000000 whyhow-0.0.6/src/whyhow/apis/base.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     9876 2024-05-24 02:12:35.000000 whyhow-0.0.6/src/whyhow/apis/graph.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     6707 2024-04-21 01:37:48.000000 whyhow-0.0.6/src/whyhow/client.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      166 2024-03-30 23:23:35.000000 whyhow-0.0.6/src/whyhow/exceptions.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        0 2024-03-30 23:23:35.000000 whyhow-0.0.6/src/whyhow/py.typed
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.660312 whyhow-0.0.6/src/whyhow/schemas/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      189 2024-03-30 23:23:35.000000 whyhow-0.0.6/src/whyhow/schemas/__init__.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      624 2024-03-30 23:23:35.000000 whyhow-0.0.6/src/whyhow/schemas/base.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     5089 2024-05-24 02:12:35.000000 whyhow-0.0.6/src/whyhow/schemas/common.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     2569 2024-05-24 02:12:35.000000 whyhow-0.0.6/src/whyhow/schemas/graph.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.661165 whyhow-0.0.6/src/whyhow.egg-info/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     8677 2024-05-24 04:58:46.000000 whyhow-0.0.6/src/whyhow.egg-info/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      548 2024-05-24 04:58:46.000000 whyhow-0.0.6/src/whyhow.egg-info/SOURCES.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-05-24 04:58:46.000000 whyhow-0.0.6/src/whyhow.egg-info/dependency_links.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-31 17:56:30.000000 whyhow-0.0.6/src/whyhow.egg-info/not-zip-safe
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      218 2024-05-24 04:58:46.000000 whyhow-0.0.6/src/whyhow.egg-info/requires.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        7 2024-05-24 04:58:46.000000 whyhow-0.0.6/src/whyhow.egg-info/top_level.txt
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.660760 whyhow-0.0.6/tests/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     1431 2024-05-07 03:43:17.000000 whyhow-0.0.6/tests/test_client.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       48 2024-03-30 23:23:35.000000 whyhow-0.0.6/tests/test_dummy.py
```

### Comparing `whyhow-0.0.5/PKG-INFO` & `whyhow-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyhow
-Version: 0.0.5
+Version: 0.0.6
 Summary: Whyhow automated KG SDK
 Author-email: Tom Smoker <tom@whyhow.ai>, Chris Rec <chris@whyhow.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/whyhow-ai/whyhow
 Keywords: SDK,KG
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -110,27 +110,32 @@
 print(documents_response)
 # Adding your documents
 
 ```
 
 ## Create a graph
 
-You can create a graph in two different ways. First, you can create a graph using a user-defined schema, giving you complete control over the types of entities and relationships that are extracted and used to build the graph. Or, you can create a graph using a set of seed questions. In this case, WhyHow will automatically extract entities and relationships that are most applicable to the things you want to know, and construct a graph from these concepts.
+You can create a graph in three different ways. First, you can create a graph using a user-defined schema, giving you complete control over the types of entities and relationships that are extracted and used to build the graph. You can also create a graph using a set of seed questions. In this case, WhyHow will automatically extract entities and relationships that are most applicable to the things you want to know, and construct a graph from these concepts. Or, you can fully deterministically create a graph from structured context in the form of a CSV.
 
 Create graph with **schema** if...
 
 1. Your graph must adhere to a consistent structure.
 2. You are very familiar with the structure of your raw documents.
 3. You need comprehensive extraction of concepts across the entire document.
 
 Create graph with **seed questions** if...
 
 1. You are unsure as to which relationships and patterns you'd like to build into your graph.
 2. You want to build your graph with only the most semantically similar raw data.
 
+Create graph with **csv** if...
+
+1. You alrady know the structure of your data.
+2. You already have data stored in a table format.
+
 ### Create a graph with schema
 
 Tell the WhyHow SDK exactly which entities, relationships, and patterns you'd like to extract and build into your graph by defining them in a JSON-based schema.
 
 ```shell
 
 #schema.json
@@ -198,24 +203,44 @@
 
 create_graph_response = client.graph.create_graph(namespace, questions)
 print(create_graph_response)
 # Creating your graph
 
 ```
 
-## Query a graph
+### Create a graph with a csv
 
-Query your graph using natural language. Using your natural language query, we automatically construct a Cypher query to run against the graph stored in your Neo4j instance.
+Provide a CSV and a schema (or automatically generate one using the `generate_schema` method) to create a graph. WhyHow will automatically extract entities and relationships from your CSV headers and data.
 
 ```shell
 
-query = "What does Harry wear?"
+namespace = "specialists"
+documents = ["../examples/assets/specialists.csv"]
+schema_file = "../examples/assets/specialists.json"
+
+# Automatically generate a schema
+schema = client.graph.generate_schema(documents=documents)
+
+# Create a graph from a CSV and the schema you bring/build
+csv_graph = client.graph.create_graph_from_csv(
+    namespace=namespace, schema_file=schema_file
+)
+
+# Query the graph created from csv using specific entities and relations
+query = "Who speaks English and live in Houston?"
+entities = ["English","Houston"]
+relations = ["SPEAKS","LIVE_IN"]
 
-query_response = client.graph.query_graph(namespace, query)
-print(query_response)
-# {answer: "Harry wears a cloak, glasses, robe, and Dudley's old clothes.", cypher_query: "MATCH (:Entity {name: "Harry"})-[:WEARS]->(clothing:Entity)\nRETURN clothing;"}
+specific_query_response = client.graph.query_graph_specific(
+    namespace=namespace,
+    query=query,
+    entities=entities,
+    relations=relations,
+    include_triples=False,
+    include_chunks=False,
+)
 
 ```
 
 ### Support
 
 WhyHow.AI is building tools to help developers bring more determinism and control to their RAG pipelines using graph structures. If you're thinking about, in the process of, or have already incorporated knowledge graphs in RAG, we’d love to chat at team@whyhow.ai, or follow our newsletter at [WhyHow.AI](https://www.whyhow.ai/). Join our discussions about rules, determinism and knowledge graphs in RAG on our [Discord](https://discord.com/invite/9bWqrsxgHr).
```

### Comparing `whyhow-0.0.5/README.md` & `whyhow-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -78,27 +78,32 @@
 print(documents_response)
 # Adding your documents
 
 ```
 
 ## Create a graph
 
-You can create a graph in two different ways. First, you can create a graph using a user-defined schema, giving you complete control over the types of entities and relationships that are extracted and used to build the graph. Or, you can create a graph using a set of seed questions. In this case, WhyHow will automatically extract entities and relationships that are most applicable to the things you want to know, and construct a graph from these concepts.
+You can create a graph in three different ways. First, you can create a graph using a user-defined schema, giving you complete control over the types of entities and relationships that are extracted and used to build the graph. You can also create a graph using a set of seed questions. In this case, WhyHow will automatically extract entities and relationships that are most applicable to the things you want to know, and construct a graph from these concepts. Or, you can fully deterministically create a graph from structured context in the form of a CSV.
 
 Create graph with **schema** if...
 
 1. Your graph must adhere to a consistent structure.
 2. You are very familiar with the structure of your raw documents.
 3. You need comprehensive extraction of concepts across the entire document.
 
 Create graph with **seed questions** if...
 
 1. You are unsure as to which relationships and patterns you'd like to build into your graph.
 2. You want to build your graph with only the most semantically similar raw data.
 
+Create graph with **csv** if...
+
+1. You alrady know the structure of your data.
+2. You already have data stored in a table format.
+
 ### Create a graph with schema
 
 Tell the WhyHow SDK exactly which entities, relationships, and patterns you'd like to extract and build into your graph by defining them in a JSON-based schema.
 
 ```shell
 
 #schema.json
@@ -166,24 +171,44 @@
 
 create_graph_response = client.graph.create_graph(namespace, questions)
 print(create_graph_response)
 # Creating your graph
 
 ```
 
-## Query a graph
+### Create a graph with a csv
 
-Query your graph using natural language. Using your natural language query, we automatically construct a Cypher query to run against the graph stored in your Neo4j instance.
+Provide a CSV and a schema (or automatically generate one using the `generate_schema` method) to create a graph. WhyHow will automatically extract entities and relationships from your CSV headers and data.
 
 ```shell
 
-query = "What does Harry wear?"
-
-query_response = client.graph.query_graph(namespace, query)
-print(query_response)
-# {answer: "Harry wears a cloak, glasses, robe, and Dudley's old clothes.", cypher_query: "MATCH (:Entity {name: "Harry"})-[:WEARS]->(clothing:Entity)\nRETURN clothing;"}
+namespace = "specialists"
+documents = ["../examples/assets/specialists.csv"]
+schema_file = "../examples/assets/specialists.json"
+
+# Automatically generate a schema
+schema = client.graph.generate_schema(documents=documents)
+
+# Create a graph from a CSV and the schema you bring/build
+csv_graph = client.graph.create_graph_from_csv(
+    namespace=namespace, schema_file=schema_file
+)
+
+# Query the graph created from csv using specific entities and relations
+query = "Who speaks English and live in Houston?"
+entities = ["English","Houston"]
+relations = ["SPEAKS","LIVE_IN"]
+
+specific_query_response = client.graph.query_graph_specific(
+    namespace=namespace,
+    query=query,
+    entities=entities,
+    relations=relations,
+    include_triples=False,
+    include_chunks=False,
+)
 
 ```
 
 ### Support
 
 WhyHow.AI is building tools to help developers bring more determinism and control to their RAG pipelines using graph structures. If you're thinking about, in the process of, or have already incorporated knowledge graphs in RAG, we’d love to chat at team@whyhow.ai, or follow our newsletter at [WhyHow.AI](https://www.whyhow.ai/). Join our discussions about rules, determinism and knowledge graphs in RAG on our [Discord](https://discord.com/invite/9bWqrsxgHr).
```

### Comparing `whyhow-0.0.5/pyproject.toml` & `whyhow-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.5/src/whyhow/client.py` & `whyhow-0.0.6/src/whyhow/client.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.5/src/whyhow/schemas/base.py` & `whyhow-0.0.6/src/whyhow/schemas/base.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.5/src/whyhow/schemas/common.py` & `whyhow-0.0.6/src/whyhow/schemas/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,14 +138,16 @@
 
 
 # GRAPH SCHEMA
 class SchemaEntity(BaseModel):
     """Schema Entity model."""
 
     name: str
+    property_columns: Optional[List[str]] = None
+    set_type_as: Optional[str] = None
     description: str
 
 
 class SchemaRelation(BaseModel):
     """Schema Relation model."""
 
     name: str
```

### Comparing `whyhow-0.0.5/src/whyhow/schemas/graph.py` & `whyhow-0.0.6/src/whyhow/schemas/graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,7 +83,25 @@
 class QueryGraphReturn(BaseReturn):
     """Schema for the return value of the query graph endpoint."""
 
     namespace: str
     answer: str
     triples: list[QueryGraphTripleResponse] = []
     chunks: list[QueryGraphChunkResponse] = []
+
+
+class SpecificQueryGraphRequest(BaseRequest):
+    """Schema for the request body of the specific query graph endpoint."""
+
+    query: str
+    entities: list[str] = []
+    relations: list[str] = []
+    include_triples: bool = False
+    include_chunks: bool = False
+
+
+class SpecificQueryGraphResponse(BaseResponse):
+    """Schema for the response body of the query graph endpoint."""
+
+    namespace: str
+    answer: str
+    triples: list[dict[str, str]] = []
```

### Comparing `whyhow-0.0.5/src/whyhow.egg-info/PKG-INFO` & `whyhow-0.0.6/src/whyhow.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyhow
-Version: 0.0.5
+Version: 0.0.6
 Summary: Whyhow automated KG SDK
 Author-email: Tom Smoker <tom@whyhow.ai>, Chris Rec <chris@whyhow.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/whyhow-ai/whyhow
 Keywords: SDK,KG
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -110,27 +110,32 @@
 print(documents_response)
 # Adding your documents
 
 ```
 
 ## Create a graph
 
-You can create a graph in two different ways. First, you can create a graph using a user-defined schema, giving you complete control over the types of entities and relationships that are extracted and used to build the graph. Or, you can create a graph using a set of seed questions. In this case, WhyHow will automatically extract entities and relationships that are most applicable to the things you want to know, and construct a graph from these concepts.
+You can create a graph in three different ways. First, you can create a graph using a user-defined schema, giving you complete control over the types of entities and relationships that are extracted and used to build the graph. You can also create a graph using a set of seed questions. In this case, WhyHow will automatically extract entities and relationships that are most applicable to the things you want to know, and construct a graph from these concepts. Or, you can fully deterministically create a graph from structured context in the form of a CSV.
 
 Create graph with **schema** if...
 
 1. Your graph must adhere to a consistent structure.
 2. You are very familiar with the structure of your raw documents.
 3. You need comprehensive extraction of concepts across the entire document.
 
 Create graph with **seed questions** if...
 
 1. You are unsure as to which relationships and patterns you'd like to build into your graph.
 2. You want to build your graph with only the most semantically similar raw data.
 
+Create graph with **csv** if...
+
+1. You alrady know the structure of your data.
+2. You already have data stored in a table format.
+
 ### Create a graph with schema
 
 Tell the WhyHow SDK exactly which entities, relationships, and patterns you'd like to extract and build into your graph by defining them in a JSON-based schema.
 
 ```shell
 
 #schema.json
@@ -198,24 +203,44 @@
 
 create_graph_response = client.graph.create_graph(namespace, questions)
 print(create_graph_response)
 # Creating your graph
 
 ```
 
-## Query a graph
+### Create a graph with a csv
 
-Query your graph using natural language. Using your natural language query, we automatically construct a Cypher query to run against the graph stored in your Neo4j instance.
+Provide a CSV and a schema (or automatically generate one using the `generate_schema` method) to create a graph. WhyHow will automatically extract entities and relationships from your CSV headers and data.
 
 ```shell
 
-query = "What does Harry wear?"
+namespace = "specialists"
+documents = ["../examples/assets/specialists.csv"]
+schema_file = "../examples/assets/specialists.json"
+
+# Automatically generate a schema
+schema = client.graph.generate_schema(documents=documents)
+
+# Create a graph from a CSV and the schema you bring/build
+csv_graph = client.graph.create_graph_from_csv(
+    namespace=namespace, schema_file=schema_file
+)
+
+# Query the graph created from csv using specific entities and relations
+query = "Who speaks English and live in Houston?"
+entities = ["English","Houston"]
+relations = ["SPEAKS","LIVE_IN"]
 
-query_response = client.graph.query_graph(namespace, query)
-print(query_response)
-# {answer: "Harry wears a cloak, glasses, robe, and Dudley's old clothes.", cypher_query: "MATCH (:Entity {name: "Harry"})-[:WEARS]->(clothing:Entity)\nRETURN clothing;"}
+specific_query_response = client.graph.query_graph_specific(
+    namespace=namespace,
+    query=query,
+    entities=entities,
+    relations=relations,
+    include_triples=False,
+    include_chunks=False,
+)
 
 ```
 
 ### Support
 
 WhyHow.AI is building tools to help developers bring more determinism and control to their RAG pipelines using graph structures. If you're thinking about, in the process of, or have already incorporated knowledge graphs in RAG, we’d love to chat at team@whyhow.ai, or follow our newsletter at [WhyHow.AI](https://www.whyhow.ai/). Join our discussions about rules, determinism and knowledge graphs in RAG on our [Discord](https://discord.com/invite/9bWqrsxgHr).
```

### Comparing `whyhow-0.0.5/src/whyhow.egg-info/SOURCES.txt` & `whyhow-0.0.6/src/whyhow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.5/tests/test_client.py` & `whyhow-0.0.6/tests/test_client.py`

 * *Files identical despite different names*

