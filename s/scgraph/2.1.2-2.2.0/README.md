# Comparing `tmp/scgraph-2.1.2.tar.gz` & `tmp/scgraph-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scgraph-2.1.2.tar", last modified: Thu May  2 19:49:24 2024, max compression
+gzip compressed data, was "scgraph-2.2.0.tar", last modified: Fri May 24 19:32:02 2024, max compression
```

## Comparing `scgraph-2.1.2.tar` & `scgraph-2.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:49:24.867123 scgraph-2.1.2/
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-2.1.2/LICENSE
--rw-r--r--   0 conmak    (1000) conmak    (1000)     9354 2024-05-02 19:49:24.867123 scgraph-2.1.2/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     8732 2024-04-25 13:26:43.000000 scgraph-2.1.2/README.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      858 2024-05-02 19:46:47.000000 scgraph-2.1.2/pyproject.toml
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:49:24.863123 scgraph-2.1.2/scgraph/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-04-25 13:24:49.000000 scgraph-2.1.2/scgraph/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    40504 2024-05-02 18:40:40.000000 scgraph-2.1.2/scgraph/core.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:49:24.867123 scgraph-2.1.2/scgraph/geographs/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2024-04-25 13:24:49.000000 scgraph-2.1.2/scgraph/geographs/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   733914 2024-04-25 13:24:49.000000 scgraph-2.1.2/scgraph/geographs/marnet.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   557967 2024-04-25 13:24:49.000000 scgraph-2.1.2/scgraph/geographs/north_america_rail.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   583015 2024-04-25 13:24:49.000000 scgraph-2.1.2/scgraph/geographs/oak_ridge_maritime.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   867927 2024-04-25 13:24:49.000000 scgraph-2.1.2/scgraph/geographs/us_freeway.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     4430 2024-05-02 17:52:07.000000 scgraph-2.1.2/scgraph/utils.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-02 19:49:24.867123 scgraph-2.1.2/scgraph.egg-info/
--rw-r--r--   0 conmak    (1000) conmak    (1000)     9354 2024-05-02 19:49:24.000000 scgraph-2.1.2/scgraph.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      389 2024-05-02 19:49:24.000000 scgraph-2.1.2/scgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-05-02 19:49:24.000000 scgraph-2.1.2/scgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2024-05-02 19:49:24.000000 scgraph-2.1.2/scgraph.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      138 2024-05-02 19:49:24.867123 scgraph-2.1.2/setup.cfg
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-24 19:32:02.690542 scgraph-2.2.0/
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-2.2.0/LICENSE
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     9519 2024-05-24 19:32:02.690542 scgraph-2.2.0/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     8897 2024-05-24 19:28:33.000000 scgraph-2.2.0/README.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      858 2024-05-24 19:25:58.000000 scgraph-2.2.0/pyproject.toml
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-24 19:32:02.686542 scgraph-2.2.0/scgraph/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-04-25 13:24:49.000000 scgraph-2.2.0/scgraph/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    49292 2024-05-24 19:19:42.000000 scgraph-2.2.0/scgraph/core.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-24 19:32:02.690542 scgraph-2.2.0/scgraph/geographs/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2024-05-24 19:19:53.000000 scgraph-2.2.0/scgraph/geographs/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   733914 2024-04-25 13:24:49.000000 scgraph-2.2.0/scgraph/geographs/marnet.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   557967 2024-04-25 13:24:49.000000 scgraph-2.2.0/scgraph/geographs/north_america_rail.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   583015 2024-04-25 13:24:49.000000 scgraph-2.2.0/scgraph/geographs/oak_ridge_maritime.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   867927 2024-04-25 13:24:49.000000 scgraph-2.2.0/scgraph/geographs/us_freeway.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     4430 2024-05-24 18:45:57.000000 scgraph-2.2.0/scgraph/utils.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-24 19:32:02.690542 scgraph-2.2.0/scgraph.egg-info/
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     9519 2024-05-24 19:32:02.000000 scgraph-2.2.0/scgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      389 2024-05-24 19:32:02.000000 scgraph-2.2.0/scgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-05-24 19:32:02.000000 scgraph-2.2.0/scgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2024-05-24 19:32:02.000000 scgraph-2.2.0/scgraph.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      138 2024-05-24 19:32:02.690542 scgraph-2.2.0/setup.cfg
```

### Comparing `scgraph-2.1.2/LICENSE` & `scgraph-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scgraph-2.1.2/PKG-INFO` & `scgraph-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 2.1.2
+Version: 2.2.0
 Summary: Determine an approximate route between two points on earth.
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/connor-makowski/scgraph
 Project-URL: Bug Tracker, https://github.com/connor-makowski/scgraph/issues
 Project-URL: Documentation, https://connor-makowski.github.io/scgraph/core.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -161,14 +161,16 @@
     origin_node={"latitude": 7.87,"longitude": 80.77}, 
     destination_node={"latitude": 5.15,"longitude": 46.20}
 )
 # Write the output to a geojson file
 get_line_path(output, filename='output.geojson')
 ```
 
+Modify an existing geograph: See the notebook [here](https://colab.research.google.com/github/connor-makowski/scgraph/blob/main/example_making_modifications.ipynb)
+
 
 You can specify your own custom graphs for direct access to the solving algorithms. This requires the use of the low level `Graph` class
 
 ```py
 from scgraph import Graph
 
 # Define a graph
```

### Comparing `scgraph-2.1.2/README.md` & `scgraph-2.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,16 @@
     origin_node={"latitude": 7.87,"longitude": 80.77}, 
     destination_node={"latitude": 5.15,"longitude": 46.20}
 )
 # Write the output to a geojson file
 get_line_path(output, filename='output.geojson')
 ```
 
+Modify an existing geograph: See the notebook [here](https://colab.research.google.com/github/connor-makowski/scgraph/blob/main/example_making_modifications.ipynb)
+
 
 You can specify your own custom graphs for direct access to the solving algorithms. This requires the use of the low level `Graph` class
 
 ```py
 from scgraph import Graph
 
 # Define a graph
```

### Comparing `scgraph-2.1.2/pyproject.toml` & `scgraph-2.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scgraph"
-version = "2.1.2"
+version = "2.2.0"
 description = "Determine an approximate route between two points on earth."
 authors = [
     {name="Connor Makowski", email="conmak@mit.edu"}
 ]
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `scgraph-2.1.2/scgraph/core.py` & `scgraph-2.2.0/scgraph/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -311,17 +311,14 @@
             - Type: list of dictionaries
             - What: A list of dictionaries where the indicies are origin node ids and the values are dictionaries of destination node indices and distances
             - Note: All nodes must be included as origins in the graph regardless of if they have any connected destinations
         - `nodes`
             - Type: list of lists
             - What: A list of lists where the values are coordinates (latitude then longitude)
             - Note: The length of the nodes list must be the same as that of the graph list
-
-        Optional Arguments:
-
         """
         self.graph = graph
         self.nodes = nodes
 
     def validate_graph(
         self, check_symmetry: bool = True, check_connected: bool = True
     ) -> None:
@@ -873,38 +870,249 @@
 
         - `filename`
             - Type: str
             - What: The filename to save the geojson file as
 
         """
         features = []
-        for origin_idx, destinations in self.graph.items():
+        for origin_idx, destinations in enumerate(self.graph):
             for destination_idx, distance in destinations.items():
                 # Create an undirected graph for geojson purposes
                 if origin_idx > destination_idx:
                     continue
-                origin = self.nodes.get(origin_idx)
-                destination = self.nodes.get(destination_idx)
+                origin = self.nodes[origin_idx]
+                destination = self.nodes[destination_idx]
                 features.append(
                     {
                         "type": "Feature",
                         "properties": {
                             "origin_idx": origin_idx,
                             "destination_idx": destination_idx,
                             "distance": distance,
                         },
                         "geometry": {
                             "type": "LineString",
                             "coordinates": [
-                                [origin["longitude"], origin["latitude"]],
+                                [origin[1], origin[0]],
                                 [
-                                    destination["longitude"],
-                                    destination["latitude"],
+                                    destination[1],
+                                    destination[0],
                                 ],
                             ],
                         },
                     }
                 )
 
         out_dict = {"type": "FeatureCollection", "features": features}
         with open(filename, "w") as f:
             json.dump(out_dict, f)
+
+    def save_as_geograph(self, name: str) -> None:
+        """
+        Function:
+
+        - Save the current geograph as an importable python file
+
+        Required Arguments:
+
+        - `name`
+            - Type: str
+            - What: The name of the geograph and file
+            - EG: 'custom'
+                - Stored as: 'custom.py'
+                    - In your current directory
+                - Import as: 'from .custom import custom_geograph'
+        """
+        self.validate_nodes()
+        self.validate_graph(
+            check_symmetry=True, check_connected=False
+        )
+        out_string = f"""from scgraph.core import GeoGraph\ngraph={str(self.graph)}\nnodes={str(self.nodes)}\n{name}_geograph = GeoGraph(graph=graph, nodes=nodes)"""
+        with open(name+".py", "w") as f:
+            f.write(out_string)
+    
+    def mod_remove_arc(self, origin_idx: int, destination_idx: int, undirected: bool = True) -> None:
+        """
+        Function:
+
+        - Remove an arc from the graph
+
+        Required Arguments:
+
+        - `origin_idx`
+            - Type: int
+            - What: The index of the origin node
+        - `destination_idx`
+            - Type: int
+            - What: The index of the destination node
+
+        Optional Arguments:
+
+        - `undirected`
+            - Type: bool
+            - What: Whether to remove the arc in both directions
+            - Default: True
+        """
+        assert origin_idx < len(self.graph), "Origin node does not exist"
+        assert destination_idx < len(self.graph), "Destination node does not exist"
+        assert destination_idx in self.graph[origin_idx], "Arc does not exist"
+        del self.graph[origin_idx][destination_idx]
+        if undirected:
+            if origin_idx in self.graph[destination_idx]:
+                del self.graph[destination_idx][origin_idx]
+
+    def mod_add_node(self, latitude: [float, int], longitude: [float, int]) -> int:
+        """
+        Function:
+
+        - Add a node to the graph
+
+        Required Arguments:
+
+        - `latitude`
+            - Type: int | float
+            - What: The latitude of the node
+        - `longitude`
+            - Type: int | float
+            - What: The longitude of the node
+
+        Returns:
+
+        - The index of the new node
+        """
+        self.nodes.append([latitude, longitude])
+        self.graph.append({})
+        return len(self.graph) - 1
+    
+    def mod_add_arc(self, origin_idx: int, destination_idx: int, distance: [int, float]=0, use_haversine_distance=True, undirected: bool = True) -> None:
+        """
+        Function:
+
+        - Add an arc to the graph
+
+        Required Arguments:
+
+        - `origin_idx`
+            - Type: int
+            - What: The index of the origin node
+        - `destination_idx`
+            - Type: int
+            - What: The index of the destination node
+
+        Optional Arguments:
+
+        - `distance`
+            - Type: int | float
+            - What: The distance between the origin and destination nodes in terms of the graph distance (normally km)
+            - Default: 0
+        - `use_haversine_distance`
+            - Type: bool
+            - What: Whether to calculate the haversine distance (km) between the nodes when calculating the distance
+            - Default: True
+            - Note: If true, overrides the `distance` argument
+        - `undirected`
+            - Type: bool
+            - What: Whether to add the arc in both directions
+            - Default: True
+        """
+        assert origin_idx < len(self.graph), "Origin node does not exist"
+        assert destination_idx < len(self.graph), "Destination node does not exist"
+        if use_haversine_distance:
+            distance = haversine(self.nodes[origin_idx], self.nodes[destination_idx])
+        self.graph[origin_idx][destination_idx] = distance
+        if undirected:
+            self.graph[destination_idx][origin_idx] = distance
+
+def load_geojson_as_geograph(geojson_filename: str) -> GeoGraph:
+    """
+    Function:
+
+    - Create a CustomGeoGraph object loaded from a geojson file
+
+    Required Arguments:
+
+    - `geojson_filename`
+        - Type: str
+        - What: The filename of the geojson file to load
+        - Note: All arcs read in will be undirected
+        - Note: This geojson file must be formatted in a specific way
+            - The geojson file must be a FeatureCollection
+            - Each feature must be a LineString with two coordinate pairs
+                - The first coordinate pair must be the origin node
+                - The second coordinate pair must be the destination node
+                - The properties of the feature must include the distance between the origin and destination nodes
+                - The properties of the feature must include the origin and destination node idxs
+                - Origin and destination node idxs must be integers between 0 and n-1 where n is the number of nodes in the graph
+            - EG:
+            ```
+            {
+                "type": "FeatureCollection",
+                "features": [
+                    {
+                        "type": "Feature",
+                        "properties": {
+                            "origin_idx": 0,
+                            "destination_idx": 1,
+                            "distance": 10
+                        },
+                        "geometry": {
+                            "type": "LineString",
+                            "coordinates": [
+                                [121.47, 31.23],
+                                [121.48, 31.24]
+                            ]
+                        }
+                    }
+                ]
+            }
+            ```
+    """
+    with open (geojson_filename, "r") as f:
+        geojson_features = json.load(f).get("features", [])
+    
+    nodes_dict = {}
+    graph_dict = {}
+    for feature in geojson_features:
+        properties = feature.get("properties", {})
+        origin_idx = properties.get("origin_idx")
+        destination_idx = properties.get("destination_idx")
+        distance = properties.get("distance")
+        geometry = feature.get("geometry", {})
+        coordinates = geometry.get("coordinates", [])
+
+        # Validations
+        assert feature.get("type") == "Feature", "All features must be of type 'Feature'"
+        assert geometry.get("type") == "LineString", "All geometries must be of type 'LineString'"
+        assert len(coordinates) == 2, "All LineStrings must have exactly 2 coordinates"
+        assert isinstance(origin_idx, int), "All features must have an 'origin_idx' property that is an integer"
+        assert isinstance(destination_idx, int), "All features must have a 'destination_idx' property that is an integer"
+        assert isinstance(distance, (int, float)), "All features must have a 'distance' property that is a number"
+        assert origin_idx >= 0, "All origin_idxs must be greater than or equal to 0"
+        assert destination_idx >= 0, "All destination_idxs must be greater than or equal to 0"
+        assert distance >= 0, "All distances must be greater than or equal to 0"
+        origin = coordinates[0]
+        destination = coordinates[1]
+        assert isinstance(origin, list), "All coordinates must be lists"
+        assert isinstance(destination, list), "All coordinates must be lists"
+        assert len(origin) == 2, "All coordinates must have a length of 2"
+        assert len(destination) == 2, "All coordinates must have a length of 2"
+        assert all([isinstance(i, (int, float)) for i in origin]), "All coordinates must be numeric"
+        assert all([isinstance(i, (int, float)) for i in destination]), "All coordinates must be numeric"
+        # assert all([origin[0] >= -90, origin[0] <= 90, origin[1] >= -180, origin[1] <= 180]), "All coordinates must be valid latitudes and longitudes"
+        # assert all([destination[0] >= -90, destination[0] <= 90, destination[1] >= -180, destination[1] <= 180]), "All coordinates must be valid latitudes and longitudes"
+        
+        # Update the data
+        nodes_dict[origin_idx] = origin
+        nodes_dict[destination_idx] = destination
+        graph_dict[origin_idx] = {**graph_dict.get(origin_idx, {}), destination_idx: distance}
+        graph_dict[destination_idx] = {**graph_dict.get(destination_idx, {}), origin_idx: distance}
+    assert len(nodes_dict) == len(graph_dict), "All nodes must be included as origins in the graph dictionary"
+    nodes = [[i[1][1],i[1][0]] for i in sorted(nodes_dict.items(), key=lambda x: x[0])]
+    ordered_graph_tuple = sorted(graph_dict.items(), key=lambda x: x[0])
+    graph_map = {i[0]: idx for idx, i in enumerate(ordered_graph_tuple)}
+    graph = [
+        {graph_map[k]: v for k, v in i[1].items()} for i in ordered_graph_tuple
+    ]
+    return GeoGraph(
+        graph=graph,
+        nodes=nodes
+    )
```

### Comparing `scgraph-2.1.2/scgraph/geographs/marnet.py` & `scgraph-2.2.0/scgraph/geographs/marnet.py`

 * *Files identical despite different names*

### Comparing `scgraph-2.1.2/scgraph/geographs/north_america_rail.py` & `scgraph-2.2.0/scgraph/geographs/north_america_rail.py`

 * *Files identical despite different names*

### Comparing `scgraph-2.1.2/scgraph/geographs/oak_ridge_maritime.py` & `scgraph-2.2.0/scgraph/geographs/oak_ridge_maritime.py`

 * *Files identical despite different names*

### Comparing `scgraph-2.1.2/scgraph/geographs/us_freeway.py` & `scgraph-2.2.0/scgraph/geographs/us_freeway.py`

 * *Files identical despite different names*

### Comparing `scgraph-2.1.2/scgraph/utils.py` & `scgraph-2.2.0/scgraph/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
     - Calculate the great circle distance in kilometers between two points on the earth (specified in decimal degrees)
 
     Required Arguments:
 
     - `origin`:
         - Type: list of two floats | ints
-        - What: The origin point as a list of "longitude" and "latitude"
+        - What: The origin point as a list of "latitude" and "longitude"
     - `destination`:
         - Type: list of two floats | ints
-        - What: The destination point as a list of "longitude" and "latitude"
+        - What: The destination point as a list of "latitude" and "longitude"
 
     Optional Arguments:
 
     - `units`:
         - Type: str
         - What: units to return the distance in? (one of "km", "m", "mi", or "ft")
         - Default: "km"
```

### Comparing `scgraph-2.1.2/scgraph.egg-info/PKG-INFO` & `scgraph-2.2.0/scgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 2.1.2
+Version: 2.2.0
 Summary: Determine an approximate route between two points on earth.
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/connor-makowski/scgraph
 Project-URL: Bug Tracker, https://github.com/connor-makowski/scgraph/issues
 Project-URL: Documentation, https://connor-makowski.github.io/scgraph/core.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -161,14 +161,16 @@
     origin_node={"latitude": 7.87,"longitude": 80.77}, 
     destination_node={"latitude": 5.15,"longitude": 46.20}
 )
 # Write the output to a geojson file
 get_line_path(output, filename='output.geojson')
 ```
 
+Modify an existing geograph: See the notebook [here](https://colab.research.google.com/github/connor-makowski/scgraph/blob/main/example_making_modifications.ipynb)
+
 
 You can specify your own custom graphs for direct access to the solving algorithms. This requires the use of the low level `Graph` class
 
 ```py
 from scgraph import Graph
 
 # Define a graph
```

