# Comparing `tmp/myscale-telemetry-0.1.2.tar.gz` & `tmp/myscale-telemetry-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myscale-telemetry-0.1.2.tar", last modified: Fri May 24 07:00:53 2024, max compression
+gzip compressed data, was "myscale-telemetry-0.1.3.tar", last modified: Fri May 24 07:10:25 2024, max compression
```

## Comparing `myscale-telemetry-0.1.2.tar` & `myscale-telemetry-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 07:00:53.384720 myscale-telemetry-0.1.2/
--rw-r--r--   0 xuj        (501) staff       (20)     1064 2024-05-21 03:32:44.000000 myscale-telemetry-0.1.2/LICENSE
--rw-r--r--   0 xuj        (501) staff       (20)     6424 2024-05-24 07:00:53.384595 myscale-telemetry-0.1.2/PKG-INFO
--rw-r--r--   0 xuj        (501) staff       (20)     5967 2024-05-24 07:00:29.000000 myscale-telemetry-0.1.2/README.md
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 07:00:53.383566 myscale-telemetry-0.1.2/myscale_telemetry/
--rw-r--r--   0 xuj        (501) staff       (20)        0 2024-05-21 05:08:28.000000 myscale-telemetry-0.1.2/myscale_telemetry/__init__.py
--rw-r--r--   0 xuj        (501) staff       (20)     5569 2024-05-21 05:09:24.000000 myscale-telemetry-0.1.2/myscale_telemetry/consumer.py
--rw-r--r--   0 xuj        (501) staff       (20)    21572 2024-05-24 04:42:34.000000 myscale-telemetry-0.1.2/myscale_telemetry/handler.py
--rw-r--r--   0 xuj        (501) staff       (20)     3671 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.2/myscale_telemetry/span_data.py
--rw-r--r--   0 xuj        (501) staff       (20)     6557 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.2/myscale_telemetry/task_manager.py
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 07:00:53.384357 myscale-telemetry-0.1.2/myscale_telemetry.egg-info/
--rw-r--r--   0 xuj        (501) staff       (20)     6424 2024-05-24 07:00:53.000000 myscale-telemetry-0.1.2/myscale_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 xuj        (501) staff       (20)      384 2024-05-24 07:00:53.000000 myscale-telemetry-0.1.2/myscale_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 xuj        (501) staff       (20)        1 2024-05-24 07:00:53.000000 myscale-telemetry-0.1.2/myscale_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 xuj        (501) staff       (20)       85 2024-05-24 07:00:53.000000 myscale-telemetry-0.1.2/myscale_telemetry.egg-info/requires.txt
--rw-r--r--   0 xuj        (501) staff       (20)       18 2024-05-24 07:00:53.000000 myscale-telemetry-0.1.2/myscale_telemetry.egg-info/top_level.txt
--rw-r--r--   0 xuj        (501) staff       (20)       38 2024-05-24 07:00:53.384767 myscale-telemetry-0.1.2/setup.cfg
--rw-r--r--   0 xuj        (501) staff       (20)      893 2024-05-24 07:00:50.000000 myscale-telemetry-0.1.2/setup.py
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 07:10:25.712673 myscale-telemetry-0.1.3/
+-rw-r--r--   0 xuj        (501) staff       (20)     1064 2024-05-21 03:32:44.000000 myscale-telemetry-0.1.3/LICENSE
+-rw-r--r--   0 xuj        (501) staff       (20)     6636 2024-05-24 07:10:25.712542 myscale-telemetry-0.1.3/PKG-INFO
+-rw-r--r--   0 xuj        (501) staff       (20)     6179 2024-05-24 07:09:19.000000 myscale-telemetry-0.1.3/README.md
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 07:10:25.711570 myscale-telemetry-0.1.3/myscale_telemetry/
+-rw-r--r--   0 xuj        (501) staff       (20)        0 2024-05-21 05:08:28.000000 myscale-telemetry-0.1.3/myscale_telemetry/__init__.py
+-rw-r--r--   0 xuj        (501) staff       (20)     5569 2024-05-21 05:09:24.000000 myscale-telemetry-0.1.3/myscale_telemetry/consumer.py
+-rw-r--r--   0 xuj        (501) staff       (20)    21572 2024-05-24 04:42:34.000000 myscale-telemetry-0.1.3/myscale_telemetry/handler.py
+-rw-r--r--   0 xuj        (501) staff       (20)     3671 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.3/myscale_telemetry/span_data.py
+-rw-r--r--   0 xuj        (501) staff       (20)     6557 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.3/myscale_telemetry/task_manager.py
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 07:10:25.712320 myscale-telemetry-0.1.3/myscale_telemetry.egg-info/
+-rw-r--r--   0 xuj        (501) staff       (20)     6636 2024-05-24 07:10:25.000000 myscale-telemetry-0.1.3/myscale_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 xuj        (501) staff       (20)      384 2024-05-24 07:10:25.000000 myscale-telemetry-0.1.3/myscale_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 xuj        (501) staff       (20)        1 2024-05-24 07:10:25.000000 myscale-telemetry-0.1.3/myscale_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       85 2024-05-24 07:10:25.000000 myscale-telemetry-0.1.3/myscale_telemetry.egg-info/requires.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       18 2024-05-24 07:10:25.000000 myscale-telemetry-0.1.3/myscale_telemetry.egg-info/top_level.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       38 2024-05-24 07:10:25.712716 myscale-telemetry-0.1.3/setup.cfg
+-rw-r--r--   0 xuj        (501) staff       (20)      893 2024-05-24 07:02:35.000000 myscale-telemetry-0.1.3/setup.py
```

### Comparing `myscale-telemetry-0.1.2/LICENSE` & `myscale-telemetry-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.2/PKG-INFO` & `myscale-telemetry-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: myscale-telemetry
-Version: 0.1.2
-Summary: Open-source observability for your LLM application.
-Home-page: https://github.com/myscale/myscale-telemetry
-Author: Xu Jing
-Author-email: xuj@myscale.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MyScale Telemetry
 
 The MyScale Telemetry is a powerful tool designed to enhance the observability of LLM applications by capturing trace data from LangChain-based applications and storing it in [MyScaleDB](https://github.com/myscale/MyScaleDB) or ClickHouse. This enables developers to diagnose issues, optimize performance, and gain deeper insights into their applications' behavior.
 
 ## Installation
 
 Install the MyScale Telemetry package using pip:
@@ -117,23 +103,23 @@
 ### Set up the Trace Dashboard
 
 Once you have Grafana, installed the ClickHouse data source plugin, and have a MyScale cluster with trace data collected through MyScale Telemetry, follow these steps to set up the MyScale Trace Dashboard in Grafana:
 
 1. **Add a new ClickHouse Data Source in Grafana:**
 
    In the Grafana Data Source settings, add a new ClickHouse Data Source. Enter the Server Address, Server Port, Username, and Password to match those of your MyScale Cloud/MyScaleDB.
-   ![data_source](./assets/add_data_source.png)
-   ![config_data_source](./assets/config_data_source.png)
+   ![data_source](https://github.com/myscale/myscale-telemetry/blob/main/assets/add_data_source.png)
+   ![config_data_source](https://github.com/myscale/myscale-telemetry/blob/main/assets/config_data_source.png)
 
 2. **Import the MyScale Trace Dashboard:**
 
    Once the ClickHouse Data Source is added, you can import the [MyScale Trace Dashboard](https://github.com/myscale/myscale-telemetry/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
 
-   ![import_dashboard](./assets/import_dashboard.png)
+   ![import_dashboard](https://github.com/myscale/myscale-telemetry/blob/main/assets/import_dashboard.png)
 
 3. **Configure the Dashboard:**
 
    After importing, select the MyScale Cluster (ClickHouse Data Source Name), the database name, table name, and TraceID of the trace you want to analyze. The dashboard will then display the Traces Table and the Trace Details Panel of the selected trace.
 
-   ![trace_dashboard_overview](./assets/dashboard.png)
+   ![trace_dashboard_overview](https://github.com/myscale/myscale-telemetry/blob/main/assets/dashboard.png)
 
 The MyScale Trace Dashboard provides comprehensive insights into the runtime behavior of your LLM applications, similar to LangSmith. It displays critical information that helps in debugging, optimizing, and understanding the performance of your applications.
```

### Comparing `myscale-telemetry-0.1.2/README.md` & `myscale-telemetry-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: myscale-telemetry
+Version: 0.1.3
+Summary: Open-source observability for your LLM application.
+Home-page: https://github.com/myscale/myscale-telemetry
+Author: Xu Jing
+Author-email: xuj@myscale.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MyScale Telemetry
 
 The MyScale Telemetry is a powerful tool designed to enhance the observability of LLM applications by capturing trace data from LangChain-based applications and storing it in [MyScaleDB](https://github.com/myscale/MyScaleDB) or ClickHouse. This enables developers to diagnose issues, optimize performance, and gain deeper insights into their applications' behavior.
 
 ## Installation
 
 Install the MyScale Telemetry package using pip:
@@ -103,23 +117,23 @@
 ### Set up the Trace Dashboard
 
 Once you have Grafana, installed the ClickHouse data source plugin, and have a MyScale cluster with trace data collected through MyScale Telemetry, follow these steps to set up the MyScale Trace Dashboard in Grafana:
 
 1. **Add a new ClickHouse Data Source in Grafana:**
 
    In the Grafana Data Source settings, add a new ClickHouse Data Source. Enter the Server Address, Server Port, Username, and Password to match those of your MyScale Cloud/MyScaleDB.
-   ![data_source](./assets/add_data_source.png)
-   ![config_data_source](./assets/config_data_source.png)
+   ![data_source](https://github.com/myscale/myscale-telemetry/blob/main/assets/add_data_source.png)
+   ![config_data_source](https://github.com/myscale/myscale-telemetry/blob/main/assets/config_data_source.png)
 
 2. **Import the MyScale Trace Dashboard:**
 
    Once the ClickHouse Data Source is added, you can import the [MyScale Trace Dashboard](https://github.com/myscale/myscale-telemetry/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
 
-   ![import_dashboard](./assets/import_dashboard.png)
+   ![import_dashboard](https://github.com/myscale/myscale-telemetry/blob/main/assets/import_dashboard.png)
 
 3. **Configure the Dashboard:**
 
    After importing, select the MyScale Cluster (ClickHouse Data Source Name), the database name, table name, and TraceID of the trace you want to analyze. The dashboard will then display the Traces Table and the Trace Details Panel of the selected trace.
 
-   ![trace_dashboard_overview](./assets/dashboard.png)
+   ![trace_dashboard_overview](https://github.com/myscale/myscale-telemetry/blob/main/assets/dashboard.png)
 
 The MyScale Trace Dashboard provides comprehensive insights into the runtime behavior of your LLM applications, similar to LangSmith. It displays critical information that helps in debugging, optimizing, and understanding the performance of your applications.
```

### Comparing `myscale-telemetry-0.1.2/myscale_telemetry/consumer.py` & `myscale-telemetry-0.1.3/myscale_telemetry/consumer.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.2/myscale_telemetry/handler.py` & `myscale-telemetry-0.1.3/myscale_telemetry/handler.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.2/myscale_telemetry/span_data.py` & `myscale-telemetry-0.1.3/myscale_telemetry/span_data.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.2/myscale_telemetry/task_manager.py` & `myscale-telemetry-0.1.3/myscale_telemetry/task_manager.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.2/myscale_telemetry.egg-info/PKG-INFO` & `myscale-telemetry-0.1.3/myscale_telemetry.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myscale-telemetry
-Version: 0.1.2
+Version: 0.1.3
 Summary: Open-source observability for your LLM application.
 Home-page: https://github.com/myscale/myscale-telemetry
 Author: Xu Jing
 Author-email: xuj@myscale.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -117,23 +117,23 @@
 ### Set up the Trace Dashboard
 
 Once you have Grafana, installed the ClickHouse data source plugin, and have a MyScale cluster with trace data collected through MyScale Telemetry, follow these steps to set up the MyScale Trace Dashboard in Grafana:
 
 1. **Add a new ClickHouse Data Source in Grafana:**
 
    In the Grafana Data Source settings, add a new ClickHouse Data Source. Enter the Server Address, Server Port, Username, and Password to match those of your MyScale Cloud/MyScaleDB.
-   ![data_source](./assets/add_data_source.png)
-   ![config_data_source](./assets/config_data_source.png)
+   ![data_source](https://github.com/myscale/myscale-telemetry/blob/main/assets/add_data_source.png)
+   ![config_data_source](https://github.com/myscale/myscale-telemetry/blob/main/assets/config_data_source.png)
 
 2. **Import the MyScale Trace Dashboard:**
 
    Once the ClickHouse Data Source is added, you can import the [MyScale Trace Dashboard](https://github.com/myscale/myscale-telemetry/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
 
-   ![import_dashboard](./assets/import_dashboard.png)
+   ![import_dashboard](https://github.com/myscale/myscale-telemetry/blob/main/assets/import_dashboard.png)
 
 3. **Configure the Dashboard:**
 
    After importing, select the MyScale Cluster (ClickHouse Data Source Name), the database name, table name, and TraceID of the trace you want to analyze. The dashboard will then display the Traces Table and the Trace Details Panel of the selected trace.
 
-   ![trace_dashboard_overview](./assets/dashboard.png)
+   ![trace_dashboard_overview](https://github.com/myscale/myscale-telemetry/blob/main/assets/dashboard.png)
 
 The MyScale Trace Dashboard provides comprehensive insights into the runtime behavior of your LLM applications, similar to LangSmith. It displays critical information that helps in debugging, optimizing, and understanding the performance of your applications.
```

### Comparing `myscale-telemetry-0.1.2/setup.py` & `myscale-telemetry-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="myscale-telemetry",
-    version="0.1.2",
+    version="0.1.3",
     description="Open-source observability for your LLM application.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Xu Jing",
     author_email="xuj@myscale.com",
     url="https://github.com/myscale/myscale-telemetry",
     packages=find_packages(),
```

