# Comparing `tmp/myscale-telemetry-0.1.1.tar.gz` & `tmp/myscale-telemetry-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myscale-telemetry-0.1.1.tar", last modified: Fri May 24 06:59:37 2024, max compression
+gzip compressed data, was "myscale-telemetry-0.1.2.tar", last modified: Fri May 24 07:00:53 2024, max compression
```

## Comparing `myscale-telemetry-0.1.1.tar` & `myscale-telemetry-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 06:59:37.702933 myscale-telemetry-0.1.1/
--rw-r--r--   0 xuj        (501) staff       (20)     1064 2024-05-21 03:32:44.000000 myscale-telemetry-0.1.1/LICENSE
--rw-r--r--   0 xuj        (501) staff       (20)     6351 2024-05-24 06:59:37.702807 myscale-telemetry-0.1.1/PKG-INFO
--rw-r--r--   0 xuj        (501) staff       (20)     5894 2024-05-24 05:19:23.000000 myscale-telemetry-0.1.1/README.md
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 06:59:37.701800 myscale-telemetry-0.1.1/myscale_telemetry/
--rw-r--r--   0 xuj        (501) staff       (20)        0 2024-05-21 05:08:28.000000 myscale-telemetry-0.1.1/myscale_telemetry/__init__.py
--rw-r--r--   0 xuj        (501) staff       (20)     5569 2024-05-21 05:09:24.000000 myscale-telemetry-0.1.1/myscale_telemetry/consumer.py
--rw-r--r--   0 xuj        (501) staff       (20)    21572 2024-05-24 04:42:34.000000 myscale-telemetry-0.1.1/myscale_telemetry/handler.py
--rw-r--r--   0 xuj        (501) staff       (20)     3671 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.1/myscale_telemetry/span_data.py
--rw-r--r--   0 xuj        (501) staff       (20)     6557 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.1/myscale_telemetry/task_manager.py
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 06:59:37.702581 myscale-telemetry-0.1.1/myscale_telemetry.egg-info/
--rw-r--r--   0 xuj        (501) staff       (20)     6351 2024-05-24 06:59:37.000000 myscale-telemetry-0.1.1/myscale_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 xuj        (501) staff       (20)      384 2024-05-24 06:59:37.000000 myscale-telemetry-0.1.1/myscale_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 xuj        (501) staff       (20)        1 2024-05-24 06:59:37.000000 myscale-telemetry-0.1.1/myscale_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 xuj        (501) staff       (20)       85 2024-05-24 06:59:37.000000 myscale-telemetry-0.1.1/myscale_telemetry.egg-info/requires.txt
--rw-r--r--   0 xuj        (501) staff       (20)       18 2024-05-24 06:59:37.000000 myscale-telemetry-0.1.1/myscale_telemetry.egg-info/top_level.txt
--rw-r--r--   0 xuj        (501) staff       (20)       38 2024-05-24 06:59:37.702979 myscale-telemetry-0.1.1/setup.cfg
--rw-r--r--   0 xuj        (501) staff       (20)      893 2024-05-24 06:59:36.000000 myscale-telemetry-0.1.1/setup.py
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 07:00:53.384720 myscale-telemetry-0.1.2/
+-rw-r--r--   0 xuj        (501) staff       (20)     1064 2024-05-21 03:32:44.000000 myscale-telemetry-0.1.2/LICENSE
+-rw-r--r--   0 xuj        (501) staff       (20)     6424 2024-05-24 07:00:53.384595 myscale-telemetry-0.1.2/PKG-INFO
+-rw-r--r--   0 xuj        (501) staff       (20)     5967 2024-05-24 07:00:29.000000 myscale-telemetry-0.1.2/README.md
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 07:00:53.383566 myscale-telemetry-0.1.2/myscale_telemetry/
+-rw-r--r--   0 xuj        (501) staff       (20)        0 2024-05-21 05:08:28.000000 myscale-telemetry-0.1.2/myscale_telemetry/__init__.py
+-rw-r--r--   0 xuj        (501) staff       (20)     5569 2024-05-21 05:09:24.000000 myscale-telemetry-0.1.2/myscale_telemetry/consumer.py
+-rw-r--r--   0 xuj        (501) staff       (20)    21572 2024-05-24 04:42:34.000000 myscale-telemetry-0.1.2/myscale_telemetry/handler.py
+-rw-r--r--   0 xuj        (501) staff       (20)     3671 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.2/myscale_telemetry/span_data.py
+-rw-r--r--   0 xuj        (501) staff       (20)     6557 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.2/myscale_telemetry/task_manager.py
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 07:00:53.384357 myscale-telemetry-0.1.2/myscale_telemetry.egg-info/
+-rw-r--r--   0 xuj        (501) staff       (20)     6424 2024-05-24 07:00:53.000000 myscale-telemetry-0.1.2/myscale_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 xuj        (501) staff       (20)      384 2024-05-24 07:00:53.000000 myscale-telemetry-0.1.2/myscale_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 xuj        (501) staff       (20)        1 2024-05-24 07:00:53.000000 myscale-telemetry-0.1.2/myscale_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       85 2024-05-24 07:00:53.000000 myscale-telemetry-0.1.2/myscale_telemetry.egg-info/requires.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       18 2024-05-24 07:00:53.000000 myscale-telemetry-0.1.2/myscale_telemetry.egg-info/top_level.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       38 2024-05-24 07:00:53.384767 myscale-telemetry-0.1.2/setup.cfg
+-rw-r--r--   0 xuj        (501) staff       (20)      893 2024-05-24 07:00:50.000000 myscale-telemetry-0.1.2/setup.py
```

### Comparing `myscale-telemetry-0.1.1/LICENSE` & `myscale-telemetry-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.1/PKG-INFO` & `myscale-telemetry-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: myscale-telemetry
-Version: 0.1.1
+Version: 0.1.2
 Summary: Open-source observability for your LLM application.
 Home-page: https://github.com/myscale/myscale-telemetry
 Author: Xu Jing
 Author-email: xuj@myscale.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# MyScale Callback
+# MyScale Telemetry
 
-The MyScale Telemetry is a powerful tool designed to enhance the observability of LLM applications by capturing trace data from LangChain-based applications and storing it in the [MyScale database](https://myscale.com/). This enables developers to diagnose issues, optimize performance, and gain deeper insights into their applications' behavior.
+The MyScale Telemetry is a powerful tool designed to enhance the observability of LLM applications by capturing trace data from LangChain-based applications and storing it in [MyScaleDB](https://github.com/myscale/MyScaleDB) or ClickHouse. This enables developers to diagnose issues, optimize performance, and gain deeper insights into their applications' behavior.
 
 ## Installation
 
 Install the MyScale Telemetry package using pip:
 
 ```bash
 pip install myscale-telemetry
@@ -49,15 +49,15 @@
 retriever = vectorstore.as_retriever()
 model = ChatOpenAI()
 template = """Answer the question based only on the following context:
 {context}
 
 Question: {question}
 
-"""
+"""python
 prompt = ChatPromptTemplate.from_template(template)
 
 chain = (
     {
     "context": itemgetter("question") | retriever,
     "question": itemgetter("question"),
     }
@@ -71,63 +71,66 @@
     callbacks=[
         MyScaleCallbackHandler()
     ]
 ))
 ```
 
 In the default scenario, the callback handler generates a `trace_id` for a single Agent call. However, if you wish to integrate the Trace of the LLM call process with a higher-level caller, you can configure the `RunnableConfig` to pass in metadata with `trace_id` as the key during the call, as in the following example:
-```
+
+```python
 # trace_id obtained from the upper layer, such as request_id of http request
 trace_id = "http-request-id-xxx"
 chain.invoke({"question": "where did harrison work"}, config=RunnableConfig(
         callbacks=[
             MyScaleCallbackHandler()
         ],
         metadata={"trace_id": trace_id}
     ))
 ```
 
 ## Custom Parameters
 
 When invoking `MyScaleCallbackHandler()`, you can specify several parameters to customize its behavior. If not specified, the default values will be used.
 
-* `myscale_host`: MyScale database host (can also be set via `MYSCALE_HOST` environment variable)             
-* `myscale_port`: MyScale database port (can also be set via `MYSCALE_PORT` environment variable)             
-* `myscale_username`: MyScale database username (can also be set via `MYSCALE_USERNAME` environment variable) 
-* `myscale_password`: MyScale database password (can also be set via `MYSCALE_PASSWORD` environment variable) 
+* `myscale_host`: MyScale database host (can also be set via `MYSCALE_HOST` environment variable)
+* `myscale_port`: MyScale database port (can also be set via `MYSCALE_PORT` environment variable)
+* `myscale_username`: MyScale database username (can also be set via `MYSCALE_USERNAME` environment variable)
+* `myscale_password`: MyScale database password (can also be set via `MYSCALE_PASSWORD` environment variable)
 * `threads`: Number of upload threads (default: 1)
 * `max_retries`: Maximum number of upload retries (default: 10)
 * `max_batch_size`: Maximum upload batch size (default: 1000)
 * `max_task_queue_size`: Maximum upload task queue size (default: 10000)
 * `upload_interval`: Upload interval in seconds (default: 0.5)
 * `database_name`: Name of the trace database (default: "otel")
 * `table_name`: Name of the trace table (default: "otel_traces")
 
 ## Observability
 
 To display trace data collected through the MyScale Telemetry from the LLM Application runtime easily and clearly, we also provide a [Grafana Trace Dashboard](https://github.com/myscale/myscale-telemetry/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
 The dashboard allows users to monitor the status of the LLM Application which is similar to LangSmith, making it easier to debug and improve its performance.
 
 ### Requirements
+
 * [Grafana](https://grafana.com/grafana)
-* [Grafana-clickhouse-datasource Plugin](https://grafana.com/grafana/plugins/grafana-clickhouse-datasource/)
-* [A MyScale Cluster with stored Trace Data](https://myscale.com/)
+* [Official ClickHouse data source for Grafana](https://grafana.com/grafana/plugins/grafana-clickhouse-datasource/)
+* A compatible database instance. MyScale Telemetry supports [MyScaleDB](https://github.com/myscale/MyScaleDB), [MyScale Cloud](https://myscale.com/), and ClickHouse.
 
 ### Set up the Trace Dashboard
-Once you have Grafana, installed the ClickHouse datasource plugin, and have a MyScale cluster with trace data collected through MyScale Telemetry, follow these steps to set up the MyScale Trace Dashboard in Grafana:
+
+Once you have Grafana, installed the ClickHouse data source plugin, and have a MyScale cluster with trace data collected through MyScale Telemetry, follow these steps to set up the MyScale Trace Dashboard in Grafana:
 
 1. **Add a new ClickHouse Data Source in Grafana:**
 
-   In the Grafana Data Source settings, add a new ClickHouse Data Source. The Server Address, Server Port, Username, and Password should correspond to the Host, Port, Username, and Password of the MyScale Cloud/MyScaleDB used.
+   In the Grafana Data Source settings, add a new ClickHouse Data Source. Enter the Server Address, Server Port, Username, and Password to match those of your MyScale Cloud/MyScaleDB.
    ![data_source](./assets/add_data_source.png)
    ![config_data_source](./assets/config_data_source.png)
 
 2. **Import the MyScale Trace Dashboard:**
 
-   Once the ClickHouse Data Source is added, you can import the [MyScale Trace Dashboard](https://github.com/myscale/myscale_callback/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
+   Once the ClickHouse Data Source is added, you can import the [MyScale Trace Dashboard](https://github.com/myscale/myscale-telemetry/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
 
    ![import_dashboard](./assets/import_dashboard.png)
 
 3. **Configure the Dashboard:**
 
    After importing, select the MyScale Cluster (ClickHouse Data Source Name), the database name, table name, and TraceID of the trace you want to analyze. The dashboard will then display the Traces Table and the Trace Details Panel of the selected trace.
```

### Comparing `myscale-telemetry-0.1.1/README.md` & `myscale-telemetry-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# MyScale Callback
+# MyScale Telemetry
 
-The MyScale Telemetry is a powerful tool designed to enhance the observability of LLM applications by capturing trace data from LangChain-based applications and storing it in the [MyScale database](https://myscale.com/). This enables developers to diagnose issues, optimize performance, and gain deeper insights into their applications' behavior.
+The MyScale Telemetry is a powerful tool designed to enhance the observability of LLM applications by capturing trace data from LangChain-based applications and storing it in [MyScaleDB](https://github.com/myscale/MyScaleDB) or ClickHouse. This enables developers to diagnose issues, optimize performance, and gain deeper insights into their applications' behavior.
 
 ## Installation
 
 Install the MyScale Telemetry package using pip:
 
 ```bash
 pip install myscale-telemetry
@@ -35,15 +35,15 @@
 retriever = vectorstore.as_retriever()
 model = ChatOpenAI()
 template = """Answer the question based only on the following context:
 {context}
 
 Question: {question}
 
-"""
+"""python
 prompt = ChatPromptTemplate.from_template(template)
 
 chain = (
     {
     "context": itemgetter("question") | retriever,
     "question": itemgetter("question"),
     }
@@ -57,63 +57,66 @@
     callbacks=[
         MyScaleCallbackHandler()
     ]
 ))
 ```
 
 In the default scenario, the callback handler generates a `trace_id` for a single Agent call. However, if you wish to integrate the Trace of the LLM call process with a higher-level caller, you can configure the `RunnableConfig` to pass in metadata with `trace_id` as the key during the call, as in the following example:
-```
+
+```python
 # trace_id obtained from the upper layer, such as request_id of http request
 trace_id = "http-request-id-xxx"
 chain.invoke({"question": "where did harrison work"}, config=RunnableConfig(
         callbacks=[
             MyScaleCallbackHandler()
         ],
         metadata={"trace_id": trace_id}
     ))
 ```
 
 ## Custom Parameters
 
 When invoking `MyScaleCallbackHandler()`, you can specify several parameters to customize its behavior. If not specified, the default values will be used.
 
-* `myscale_host`: MyScale database host (can also be set via `MYSCALE_HOST` environment variable)             
-* `myscale_port`: MyScale database port (can also be set via `MYSCALE_PORT` environment variable)             
-* `myscale_username`: MyScale database username (can also be set via `MYSCALE_USERNAME` environment variable) 
-* `myscale_password`: MyScale database password (can also be set via `MYSCALE_PASSWORD` environment variable) 
+* `myscale_host`: MyScale database host (can also be set via `MYSCALE_HOST` environment variable)
+* `myscale_port`: MyScale database port (can also be set via `MYSCALE_PORT` environment variable)
+* `myscale_username`: MyScale database username (can also be set via `MYSCALE_USERNAME` environment variable)
+* `myscale_password`: MyScale database password (can also be set via `MYSCALE_PASSWORD` environment variable)
 * `threads`: Number of upload threads (default: 1)
 * `max_retries`: Maximum number of upload retries (default: 10)
 * `max_batch_size`: Maximum upload batch size (default: 1000)
 * `max_task_queue_size`: Maximum upload task queue size (default: 10000)
 * `upload_interval`: Upload interval in seconds (default: 0.5)
 * `database_name`: Name of the trace database (default: "otel")
 * `table_name`: Name of the trace table (default: "otel_traces")
 
 ## Observability
 
 To display trace data collected through the MyScale Telemetry from the LLM Application runtime easily and clearly, we also provide a [Grafana Trace Dashboard](https://github.com/myscale/myscale-telemetry/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
 The dashboard allows users to monitor the status of the LLM Application which is similar to LangSmith, making it easier to debug and improve its performance.
 
 ### Requirements
+
 * [Grafana](https://grafana.com/grafana)
-* [Grafana-clickhouse-datasource Plugin](https://grafana.com/grafana/plugins/grafana-clickhouse-datasource/)
-* [A MyScale Cluster with stored Trace Data](https://myscale.com/)
+* [Official ClickHouse data source for Grafana](https://grafana.com/grafana/plugins/grafana-clickhouse-datasource/)
+* A compatible database instance. MyScale Telemetry supports [MyScaleDB](https://github.com/myscale/MyScaleDB), [MyScale Cloud](https://myscale.com/), and ClickHouse.
 
 ### Set up the Trace Dashboard
-Once you have Grafana, installed the ClickHouse datasource plugin, and have a MyScale cluster with trace data collected through MyScale Telemetry, follow these steps to set up the MyScale Trace Dashboard in Grafana:
+
+Once you have Grafana, installed the ClickHouse data source plugin, and have a MyScale cluster with trace data collected through MyScale Telemetry, follow these steps to set up the MyScale Trace Dashboard in Grafana:
 
 1. **Add a new ClickHouse Data Source in Grafana:**
 
-   In the Grafana Data Source settings, add a new ClickHouse Data Source. The Server Address, Server Port, Username, and Password should correspond to the Host, Port, Username, and Password of the MyScale Cloud/MyScaleDB used.
+   In the Grafana Data Source settings, add a new ClickHouse Data Source. Enter the Server Address, Server Port, Username, and Password to match those of your MyScale Cloud/MyScaleDB.
    ![data_source](./assets/add_data_source.png)
    ![config_data_source](./assets/config_data_source.png)
 
 2. **Import the MyScale Trace Dashboard:**
 
-   Once the ClickHouse Data Source is added, you can import the [MyScale Trace Dashboard](https://github.com/myscale/myscale_callback/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
+   Once the ClickHouse Data Source is added, you can import the [MyScale Trace Dashboard](https://github.com/myscale/myscale-telemetry/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
 
    ![import_dashboard](./assets/import_dashboard.png)
 
 3. **Configure the Dashboard:**
 
    After importing, select the MyScale Cluster (ClickHouse Data Source Name), the database name, table name, and TraceID of the trace you want to analyze. The dashboard will then display the Traces Table and the Trace Details Panel of the selected trace.
```

### Comparing `myscale-telemetry-0.1.1/myscale_telemetry/consumer.py` & `myscale-telemetry-0.1.2/myscale_telemetry/consumer.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.1/myscale_telemetry/handler.py` & `myscale-telemetry-0.1.2/myscale_telemetry/handler.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.1/myscale_telemetry/span_data.py` & `myscale-telemetry-0.1.2/myscale_telemetry/span_data.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.1/myscale_telemetry/task_manager.py` & `myscale-telemetry-0.1.2/myscale_telemetry/task_manager.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.1/myscale_telemetry.egg-info/PKG-INFO` & `myscale-telemetry-0.1.2/myscale_telemetry.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: myscale-telemetry
-Version: 0.1.1
+Version: 0.1.2
 Summary: Open-source observability for your LLM application.
 Home-page: https://github.com/myscale/myscale-telemetry
 Author: Xu Jing
 Author-email: xuj@myscale.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# MyScale Callback
+# MyScale Telemetry
 
-The MyScale Telemetry is a powerful tool designed to enhance the observability of LLM applications by capturing trace data from LangChain-based applications and storing it in the [MyScale database](https://myscale.com/). This enables developers to diagnose issues, optimize performance, and gain deeper insights into their applications' behavior.
+The MyScale Telemetry is a powerful tool designed to enhance the observability of LLM applications by capturing trace data from LangChain-based applications and storing it in [MyScaleDB](https://github.com/myscale/MyScaleDB) or ClickHouse. This enables developers to diagnose issues, optimize performance, and gain deeper insights into their applications' behavior.
 
 ## Installation
 
 Install the MyScale Telemetry package using pip:
 
 ```bash
 pip install myscale-telemetry
@@ -49,15 +49,15 @@
 retriever = vectorstore.as_retriever()
 model = ChatOpenAI()
 template = """Answer the question based only on the following context:
 {context}
 
 Question: {question}
 
-"""
+"""python
 prompt = ChatPromptTemplate.from_template(template)
 
 chain = (
     {
     "context": itemgetter("question") | retriever,
     "question": itemgetter("question"),
     }
@@ -71,63 +71,66 @@
     callbacks=[
         MyScaleCallbackHandler()
     ]
 ))
 ```
 
 In the default scenario, the callback handler generates a `trace_id` for a single Agent call. However, if you wish to integrate the Trace of the LLM call process with a higher-level caller, you can configure the `RunnableConfig` to pass in metadata with `trace_id` as the key during the call, as in the following example:
-```
+
+```python
 # trace_id obtained from the upper layer, such as request_id of http request
 trace_id = "http-request-id-xxx"
 chain.invoke({"question": "where did harrison work"}, config=RunnableConfig(
         callbacks=[
             MyScaleCallbackHandler()
         ],
         metadata={"trace_id": trace_id}
     ))
 ```
 
 ## Custom Parameters
 
 When invoking `MyScaleCallbackHandler()`, you can specify several parameters to customize its behavior. If not specified, the default values will be used.
 
-* `myscale_host`: MyScale database host (can also be set via `MYSCALE_HOST` environment variable)             
-* `myscale_port`: MyScale database port (can also be set via `MYSCALE_PORT` environment variable)             
-* `myscale_username`: MyScale database username (can also be set via `MYSCALE_USERNAME` environment variable) 
-* `myscale_password`: MyScale database password (can also be set via `MYSCALE_PASSWORD` environment variable) 
+* `myscale_host`: MyScale database host (can also be set via `MYSCALE_HOST` environment variable)
+* `myscale_port`: MyScale database port (can also be set via `MYSCALE_PORT` environment variable)
+* `myscale_username`: MyScale database username (can also be set via `MYSCALE_USERNAME` environment variable)
+* `myscale_password`: MyScale database password (can also be set via `MYSCALE_PASSWORD` environment variable)
 * `threads`: Number of upload threads (default: 1)
 * `max_retries`: Maximum number of upload retries (default: 10)
 * `max_batch_size`: Maximum upload batch size (default: 1000)
 * `max_task_queue_size`: Maximum upload task queue size (default: 10000)
 * `upload_interval`: Upload interval in seconds (default: 0.5)
 * `database_name`: Name of the trace database (default: "otel")
 * `table_name`: Name of the trace table (default: "otel_traces")
 
 ## Observability
 
 To display trace data collected through the MyScale Telemetry from the LLM Application runtime easily and clearly, we also provide a [Grafana Trace Dashboard](https://github.com/myscale/myscale-telemetry/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
 The dashboard allows users to monitor the status of the LLM Application which is similar to LangSmith, making it easier to debug and improve its performance.
 
 ### Requirements
+
 * [Grafana](https://grafana.com/grafana)
-* [Grafana-clickhouse-datasource Plugin](https://grafana.com/grafana/plugins/grafana-clickhouse-datasource/)
-* [A MyScale Cluster with stored Trace Data](https://myscale.com/)
+* [Official ClickHouse data source for Grafana](https://grafana.com/grafana/plugins/grafana-clickhouse-datasource/)
+* A compatible database instance. MyScale Telemetry supports [MyScaleDB](https://github.com/myscale/MyScaleDB), [MyScale Cloud](https://myscale.com/), and ClickHouse.
 
 ### Set up the Trace Dashboard
-Once you have Grafana, installed the ClickHouse datasource plugin, and have a MyScale cluster with trace data collected through MyScale Telemetry, follow these steps to set up the MyScale Trace Dashboard in Grafana:
+
+Once you have Grafana, installed the ClickHouse data source plugin, and have a MyScale cluster with trace data collected through MyScale Telemetry, follow these steps to set up the MyScale Trace Dashboard in Grafana:
 
 1. **Add a new ClickHouse Data Source in Grafana:**
 
-   In the Grafana Data Source settings, add a new ClickHouse Data Source. The Server Address, Server Port, Username, and Password should correspond to the Host, Port, Username, and Password of the MyScale Cloud/MyScaleDB used.
+   In the Grafana Data Source settings, add a new ClickHouse Data Source. Enter the Server Address, Server Port, Username, and Password to match those of your MyScale Cloud/MyScaleDB.
    ![data_source](./assets/add_data_source.png)
    ![config_data_source](./assets/config_data_source.png)
 
 2. **Import the MyScale Trace Dashboard:**
 
-   Once the ClickHouse Data Source is added, you can import the [MyScale Trace Dashboard](https://github.com/myscale/myscale_callback/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
+   Once the ClickHouse Data Source is added, you can import the [MyScale Trace Dashboard](https://github.com/myscale/myscale-telemetry/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
 
    ![import_dashboard](./assets/import_dashboard.png)
 
 3. **Configure the Dashboard:**
 
    After importing, select the MyScale Cluster (ClickHouse Data Source Name), the database name, table name, and TraceID of the trace you want to analyze. The dashboard will then display the Traces Table and the Trace Details Panel of the selected trace.
```

### Comparing `myscale-telemetry-0.1.1/setup.py` & `myscale-telemetry-0.1.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="myscale-telemetry",
-    version="0.1.1",
+    version="0.1.2",
     description="Open-source observability for your LLM application.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Xu Jing",
     author_email="xuj@myscale.com",
     url="https://github.com/myscale/myscale-telemetry",
     packages=find_packages(),
```

