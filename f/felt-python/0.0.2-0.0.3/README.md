# Comparing `tmp/felt_python-0.0.2.tar.gz` & `tmp/felt_python-0.0.3.tar.gz`

## Comparing `felt_python-0.0.2.tar` & `felt_python-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 felt_python-0.0.2/testing_elements.ipynb
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 felt_python-0.0.2/testing_layers.ipynb
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 felt_python-0.0.2/felt_python/__init__.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 felt_python-0.0.2/felt_python/api.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 felt_python-0.0.2/felt_python/elements.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 felt_python-0.0.2/felt_python/exceptions.py
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 felt_python-0.0.2/felt_python/layers.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 felt_python-0.0.2/felt_python/maps.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 felt_python-0.0.2/tests/fixtures/null-island-points-sample.geojson
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 felt_python-0.0.2/tests/fixtures/null-island-points.geojson
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 felt_python-0.0.2/tests/fixtures/null-island-polygons-wkt.csv
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 felt_python-0.0.2/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 felt_python-0.0.2/LICENSE
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 felt_python-0.0.2/README.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 felt_python-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 felt_python-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 felt_python-0.0.3/testing_elements.ipynb
+-rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 felt_python-0.0.3/testing_layers.ipynb
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 felt_python-0.0.3/felt_python/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 felt_python-0.0.3/felt_python/api.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 felt_python-0.0.3/felt_python/elements.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 felt_python-0.0.3/felt_python/exceptions.py
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 felt_python-0.0.3/felt_python/layers.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 felt_python-0.0.3/felt_python/maps.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 felt_python-0.0.3/tests/fixtures/null-island-points-sample.geojson
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 felt_python-0.0.3/tests/fixtures/null-island-points.geojson
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 felt_python-0.0.3/tests/fixtures/null-island-polygons-wkt.csv
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 felt_python-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 felt_python-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 felt_python-0.0.3/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 felt_python-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 felt_python-0.0.3/PKG-INFO
```

### Comparing `felt_python-0.0.2/testing_elements.ipynb` & `felt_python-0.0.3/testing_elements.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998015873015873%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(7, \'resp["url"]\')], delete: [7]}}}'}*

```diff
@@ -46,15 +46,15 @@
                 "resp = create_map(\n",
                 "    title=\"A felt-py map for testing elements\",\n",
                 "    lat=40,\n",
                 "    lon=-3,\n",
                 "    public_access=\"private\",\n",
                 ")\n",
                 "map_id = resp[\"id\"]\n",
-                "resp[\"attributes\"][\"url\"]"
+                "resp[\"url\"]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Create elements\n",
```

### Comparing `felt_python-0.0.2/testing_layers.ipynb` & `felt_python-0.0.3/testing_layers.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964151916248956%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'import time\\n')]}}, 7: {'source': {insert: [(1, "*

 * *            '\'layer_id = layer_resp["layer_id"]\')], delete: [1]}}, 9: {\'source\': [\'while '*

 * *            'get_layer_details(map_id, layer_id)["progress"] < 100:\\n\', \'    print("Waiting for '*

 * *            'layer to finish processing...")\\n\', \'    time.sleep(5)\']}, 13: {\'source\': '*

 * *            '{insert: [(2, \'url_layer_id = url_upload["layer_id"]\')], delete: [2]}}, 15: '*

 * *            "{'source': {insert:  […]*

```diff
@@ -12,14 +12,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "fc85a763-cd96-4eab-85d1-d82adfe0eea1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
+                "import time\n",
                 "\n",
                 "from felt_python import (\n",
                 "    create_map,\n",
                 "    delete_map,\n",
                 "    get_map_details,\n",
                 "    list_layers,\n",
                 "    upload_file,\n",
@@ -93,15 +94,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "bd6045fa-a226-4072-8e4a-924470638347",
             "metadata": {},
             "outputs": [],
             "source": [
                 "layer_resp = upload_file(map_id, \"tests/fixtures/null-island-points-sample.geojson\", \"The Points Layer\")\n",
-                "layer_id = layer_resp[\"attributes\"][\"first_layer_id\"]"
+                "layer_id = layer_resp[\"layer_id\"]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "62dd0688",
             "metadata": {},
             "source": [
@@ -111,15 +112,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "39488500",
             "metadata": {},
             "outputs": [],
             "source": [
-                "get_layer_details(map_id, layer_id)"
+                "while get_layer_details(map_id, layer_id)[\"progress\"] < 100:\n",
+                "    print(\"Waiting for layer to finish processing...\")\n",
+                "    time.sleep(5)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "050e2bc0-30e4-4f4b-83cf-9e22f91df1e8",
             "metadata": {},
             "source": [
@@ -153,15 +156,15 @@
             "execution_count": null,
             "id": "07d46bab-6721-451e-8f63-83017f2cf974",
             "metadata": {},
             "outputs": [],
             "source": [
                 "live_earthquakes_url = \"https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_hour.geojson\"\n",
                 "url_upload = upload_url(map_id, live_earthquakes_url, \"Live Earthquakes\")\n",
-                "url_layer_id = url_upload[\"attributes\"][\"first_layer_id\"]"
+                "url_layer_id = url_upload[\"layer_id\"]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "feaa457c-9695-4451-a783-45bb476e1574",
             "metadata": {},
             "source": [
@@ -173,14 +176,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a7021996-4d4a-4276-89e0-88e8d501bfe0",
             "metadata": {},
             "outputs": [],
             "source": [
+                "while get_layer_details(map_id, url_layer_id)[\"progress\"] < 100:\n",
+                "    print(\"Waiting for layer to finish processing...\")\n",
+                "    time.sleep(5)\n",
                 "refresh_url_layer(map_id, url_layer_id)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "adc9d25b-a64c-4c7d-8463-20d13dcad10a",
             "metadata": {},
@@ -199,15 +205,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6519d2bb-6223-490b-9eee-7e0d54052092",
             "metadata": {},
             "outputs": [],
             "source": [
-                "current_style = get_layer_details(map_id, layer_id)[\"attributes\"][\"style\"]\n",
+                "current_style = get_layer_details(map_id, layer_id)[\"style\"]\n",
                 "current_style"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c37f77cc-fcba-4906-a76c-23ad51abd618",
             "metadata": {},
@@ -311,13 +317,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.13"
+            "version": "3.11.6"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `felt_python-0.0.2/felt_python/__init__.py` & `felt_python-0.0.3/felt_python/__init__.py`

 * *Files identical despite different names*

### Comparing `felt_python-0.0.2/felt_python/maps.py` & `felt_python-0.0.3/felt_python/maps.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 """Maps"""
 
-import requests
+import json
 
-from .api import make_request, MAPS_TEMPLATE
+from urllib.parse import urljoin
+
+from .api import make_request, BASE_URL
+
+
+MAPS_ENDPOINT = urljoin(BASE_URL, "maps/")
+MAP_TEMPLATE = urljoin(MAPS_ENDPOINT, "{map_id}/")
 
 
 def create_map(api_token: str | None = None, **json_args):
     """Create a new Felt map"""
     response = make_request(
-        url=MAPS_TEMPLATE.expand(),
-        method=requests.post,
+        url=MAPS_ENDPOINT,
+        method="POST",
         json=json_args,
         api_token=api_token,
     )
-    return response.json()["data"]
+    return json.load(response)
 
 
 def delete_map(map_id: str, api_token: str | None = None):
     """Delete a map"""
     make_request(
-        url=MAPS_TEMPLATE.expand(map_id=map_id),
-        method=requests.delete,
+        url=MAP_TEMPLATE.format(map_id=map_id),
+        method="DELETE",
         api_token=api_token,
     )
 
 
 def get_map_details(map_id: str, api_token: str | None = None):
     """Get details of a map"""
     response = make_request(
-        url=MAPS_TEMPLATE.expand(map_id=map_id),
-        method=requests.get,
+        url=MAP_TEMPLATE.format(map_id=map_id),
+        method="GET",
         api_token=api_token,
     )
-    return response.json()["data"]
+    return json.load(response)
 
 
 def update_map(map_id: str, new_title: str, api_token: str | None = None):
     """Update a map's details (title only for now)"""
     response = make_request(
-        url=MAPS_TEMPLATE.expand(map_id=map_id),
-        method=requests.patch,
+        url=MAP_TEMPLATE.format(map_id=map_id),
+        method="PATCH",
         json={"title": new_title},
         api_token=api_token,
     )
-    return response.json()["data"]
+    return json.load(response)
```

### Comparing `felt_python-0.0.2/tests/fixtures/null-island-points-sample.geojson` & `felt_python-0.0.3/tests/fixtures/null-island-points-sample.geojson`

 * *Files identical despite different names*

### Comparing `felt_python-0.0.2/tests/fixtures/null-island-points.geojson` & `felt_python-0.0.3/tests/fixtures/null-island-points.geojson`

 * *Files identical despite different names*

### Comparing `felt_python-0.0.2/tests/fixtures/null-island-polygons-wkt.csv` & `felt_python-0.0.3/tests/fixtures/null-island-polygons-wkt.csv`

 * *Files identical despite different names*

### Comparing `felt_python-0.0.2/.gitignore` & `felt_python-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `felt_python-0.0.2/LICENSE` & `felt_python-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `felt_python-0.0.2/README.md` & `felt_python-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 This client is especially useful at simplifying certain operations like uploading and
 refreshing files and (Geo)DataFrames or updating layer styles and element properties.
 
 ## Installation
 
 ```bash
-pip install felt-python==0.0.1
+pip install felt-python
 ```
 
 ## Usage
 
 ### Authentication
 
 To authenticate with the Felt API, you need to provide your API token. You can either 
@@ -41,21 +41,20 @@
 ```
 
 ### Uploading a file
 
 ```python
 from felt_python import upload_file, list_layers
 
-upload_file(
+upload = upload_file(
     map_id=map_id,
     file_path="path/to/file.csv",
     layer_name="My new layer",
 )
-layer_groups = list_layers(map_id)
-layer_id = layer_groups[0]["relationships"]["datasets"]["data"][0]["id"]
+layer_id = upload["layer_id"]
 ```
 
 ### Uploading a Pandas DataFrame
 ```python
 import pandas as pd
 from felt_python import upload_dataframe
```

### Comparing `felt_python-0.0.2/PKG-INFO` & `felt_python-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.3
 Name: felt-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: The official Felt API client library
 Project-URL: Homepage, https://github.com/felt/felt-python
 Project-URL: Issues, https://github.com/felt/felt-python/issues
 Project-URL: Documentation, https://felt-1.gitbook.io/developer-docs
 Author-email: Álvaro Arredondo <alvaro@felt.com>, Chris Loer <chris@felt.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
-Requires-Dist: requests
-Requires-Dist: uritemplate
 Description-Content-Type: text/markdown
 
 (WIP) The official Python client for the Felt API
 ===========================================
 
 **felt-python** is a Python client for the Felt API. It provides convenient wrappers for
 common operations like creating, deleting and updating maps and data layers.
 
 This client is especially useful at simplifying certain operations like uploading and
 refreshing files and (Geo)DataFrames or updating layer styles and element properties.
 
 ## Installation
 
 ```bash
-pip install felt-python==0.0.1
+pip install felt-python
 ```
 
 ## Usage
 
 ### Authentication
 
 To authenticate with the Felt API, you need to provide your API token. You can either 
@@ -58,21 +56,20 @@
 ```
 
 ### Uploading a file
 
 ```python
 from felt_python import upload_file, list_layers
 
-upload_file(
+upload = upload_file(
     map_id=map_id,
     file_path="path/to/file.csv",
     layer_name="My new layer",
 )
-layer_groups = list_layers(map_id)
-layer_id = layer_groups[0]["relationships"]["datasets"]["data"][0]["id"]
+layer_id = upload["layer_id"]
 ```
 
 ### Uploading a Pandas DataFrame
 ```python
 import pandas as pd
 from felt_python import upload_dataframe
```

