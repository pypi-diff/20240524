# Comparing `tmp/dwd_global_radiation-1.0.0rc6.tar.gz` & `tmp/dwd_global_radiation-1.0.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwd_global_radiation-1.0.0rc6.tar", last modified: Wed May 22 14:32:56 2024, max compression
+gzip compressed data, was "dwd_global_radiation-1.0.0rc7.tar", last modified: Fri May 24 08:37:21 2024, max compression
```

## Comparing `dwd_global_radiation-1.0.0rc6.tar` & `dwd_global_radiation-1.0.0rc7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-22 14:32:56.435814 dwd_global_radiation-1.0.0rc6/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1065 2024-05-05 09:59:58.000000 dwd_global_radiation-1.0.0rc6/LICENSE
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-22 14:32:56.435814 dwd_global_radiation-1.0.0rc6/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21423 2024-05-21 10:47:19.000000 dwd_global_radiation-1.0.0rc6/README.md
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-22 14:32:56.431814 dwd_global_radiation-1.0.0rc6/dwd_global_radiation/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       45 2024-05-07 07:51:24.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation/__init__.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    24231 2024-05-22 14:22:24.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation/global_radiation.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    18137 2024-05-15 21:06:36.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation/utils.py
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-22 14:32:56.435814 dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-22 14:32:56.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      349 2024-05-22 14:32:56.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/SOURCES.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)        1 2024-05-22 14:32:56.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/dependency_links.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      128 2024-05-22 14:32:56.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/requires.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       21 2024-05-22 14:32:56.000000 dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/top_level.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       38 2024-05-22 14:32:56.435814 dwd_global_radiation-1.0.0rc6/setup.cfg
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1656 2024-05-22 14:23:30.000000 dwd_global_radiation-1.0.0rc6/setup.py
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-24 08:37:21.601738 dwd_global_radiation-1.0.0rc7/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1065 2024-05-05 09:59:58.000000 dwd_global_radiation-1.0.0rc7/LICENSE
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-24 08:37:21.601738 dwd_global_radiation-1.0.0rc7/PKG-INFO
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21423 2024-05-21 10:47:19.000000 dwd_global_radiation-1.0.0rc7/README.md
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-24 08:37:21.601738 dwd_global_radiation-1.0.0rc7/dwd_global_radiation/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       45 2024-05-07 07:51:24.000000 dwd_global_radiation-1.0.0rc7/dwd_global_radiation/__init__.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    27286 2024-05-24 08:01:52.000000 dwd_global_radiation-1.0.0rc7/dwd_global_radiation/global_radiation.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    18137 2024-05-15 21:06:36.000000 dwd_global_radiation-1.0.0rc7/dwd_global_radiation/utils.py
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-24 08:37:21.601738 dwd_global_radiation-1.0.0rc7/dwd_global_radiation.egg-info/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-24 08:37:21.000000 dwd_global_radiation-1.0.0rc7/dwd_global_radiation.egg-info/PKG-INFO
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)      349 2024-05-24 08:37:21.000000 dwd_global_radiation-1.0.0rc7/dwd_global_radiation.egg-info/SOURCES.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)        1 2024-05-24 08:37:21.000000 dwd_global_radiation-1.0.0rc7/dwd_global_radiation.egg-info/dependency_links.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)      128 2024-05-24 08:37:21.000000 dwd_global_radiation-1.0.0rc7/dwd_global_radiation.egg-info/requires.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       21 2024-05-24 08:37:21.000000 dwd_global_radiation-1.0.0rc7/dwd_global_radiation.egg-info/top_level.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       38 2024-05-24 08:37:21.601738 dwd_global_radiation-1.0.0rc7/setup.cfg
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1656 2024-05-24 08:00:50.000000 dwd_global_radiation-1.0.0rc7/setup.py
```

### Comparing `dwd_global_radiation-1.0.0rc6/LICENSE` & `dwd_global_radiation-1.0.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.0.0rc6/PKG-INFO` & `dwd_global_radiation-1.0.0rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.0.0rc6
+Version: 1.0.0rc7
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dwd_global_radiation-1.0.0rc6/README.md` & `dwd_global_radiation-1.0.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.0.0rc6/dwd_global_radiation/global_radiation.py` & `dwd_global_radiation-1.0.0rc7/dwd_global_radiation/global_radiation.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,42 +50,69 @@
             f"latitude={self.latitude}",
             f"longitude={self.longitude}",
             f"measurements={measurement_count} {'item' if measurement_count == 1 else 'items'}",
             f"forecasts={forecast_count} {'item' if forecast_count == 1 else 'items'})"
         ]
         return ", ".join(parts)
 
+    def to_dict(self):
+        """Convert Location to a dictionary."""
+        return {
+            "latitude": float(self.latitude),  # Explicit conversion to float
+            "longitude": float(self.longitude), # Explicit conversion to float
+            "name": self.name,
+            "measurements": [measurement.to_dict() for measurement in self.measurements],
+            "forecasts": [forecast.to_dict() for forecast in self.forecasts]
+        }
+
 @dataclass
 class MeasurementEntry:
     """Class for storing DWD global radiation measurement data."""
     timestamp: float  # assuming timestamp is a Unix time float
     sis: float        # Solar Irradiance in W/m^2
 
+    def to_dict(self):
+        """Convert MeasurementEntry to a dictionary."""
+        return {
+            "timestamp": float(self.timestamp),  # Explicit conversion to float
+            "sis": float(self.sis)               # Explicit conversion to float
+        }
+
 
 @dataclass
 class Measurement:
     """Class for hosting various quarterly hour global radiation measurement
     data from DWD servers"""
     grid_latitude: float
     grid_longitude: float
     distance: float
     nearest_index: int
-    measurement_values: list = field(default_factory=list)
+    measurement_values: list[MeasurementEntry] = field(default_factory=list)
 
     def __repr__(self):
         measurement_values_count=len(self.measurement_values)
         # Round latitude and longitude to two decimal places
         lat = round(self.grid_latitude, 2) if self.grid_latitude is not None else None
         lon = round(self.grid_longitude, 2) if self.grid_longitude is not None else None
         return (f"Measurement(grid_latitude={lat}, "
                 f"grid_longitude={lon}, "
                 f"distance={self.distance}, "
                 f"nearest_index={self.nearest_index}, "
                 f"measurement_values=Count: {measurement_values_count})")
 
+    def to_dict(self):
+        """Convert Measurement to a dictionary."""
+        return {
+            "grid_latitude": float(self.grid_latitude),  # Explicit conversion to float
+            "grid_longitude": float(self.grid_longitude), # Explicit conversion to float
+            "distance": float(self.distance),            # Explicit conversion to float
+            "nearest_index": int(self.nearest_index),    # Explicit conversion to int
+            "measurement_values": [entry.to_dict() for entry in self.measurement_values]
+        }
+
     def add_measurement_value(self, timestamp, sis):
         """Method for adding retrieved measurement values as SIS"""
         self.measurement_values.append(MeasurementEntry(timestamp, sis))
 
     def get_measurement_values(self):
         """Method to retrieve all measurement values"""
         return self.measurement_values
@@ -114,14 +141,25 @@
         return (
             f"Forecast(issuance_time={self.issuance_time}, "
             f"grid_latitude={lat}, grid_longitude={lon}, "
             f"distance={self.distance}, entries={entries_count}, "
             f"metadata=status '{metadata_status}')"
         )
 
+    def to_dict(self):
+        """Convert Forecast to a dictionary."""
+        return {
+            "issuance_time": float(self.issuance_time),  # Explicit conversion to float
+            "grid_latitude": float(self.grid_latitude),  # Explicit conversion to float
+            "grid_longitude": float(self.grid_longitude), # Explicit conversion to float
+            "distance": float(self.distance),            # Explicit conversion to float
+            "entries": [entry.to_dict() for entry in self.entries],
+            "metadata": self.metadata
+        }
+
     def set_metadata(self, standard_name=None, long_name=None, units=None):
         """Function for writing global radiation metadata of the DWD data file"""
         self.metadata["standard_name"] = standard_name
         self.metadata["long_name"] = long_name
         self.metadata["units"] = units
 
     def set_distance(self, latitude=None, longitude=None):
@@ -142,14 +180,21 @@
 @dataclass
 class ForecastEntry:
     """Class for storing DWD global radiation forecast data"""
 
     timestamp: str
     sis: float
 
+    def to_dict(self):
+        """Convert ForecastEntry to a dictionary."""
+        return {
+            "timestamp": float(self.timestamp),  # Explicit conversion to float
+            "sis": float(self.sis)               # Explicit conversion to float
+        }
+
 @dataclass
 class IndentConfig:
     """Handles indentation settings for pretty-printing data outputs."""
     indent: str = "     "
     sub_indent: str = "        "
 
 @dataclass
@@ -175,14 +220,26 @@
 
     locations: list = field(default_factory=list)
     last_measurement_fetch_date: datetime = None
     last_forecast_fetch_date: datetime = None
     measurement_health_state: str = 'green'
     forecast_health_state: str = 'green'
 
+    def to_dict(self):
+        """Convert GlobalRadiation to a dictionary."""
+        return {
+            "locations": [location.to_dict() for location in self.locations],
+            "last_measurement_fetch_date": self.last_measurement_fetch_date.isoformat(
+                ) if self.last_measurement_fetch_date else None,
+            "last_forecast_fetch_date": self.last_forecast_fetch_date.isoformat(
+                ) if self.last_forecast_fetch_date else None,
+            "measurement_health_state": self.measurement_health_state,
+            "forecast_health_state": self.forecast_health_state
+        }
+
     def get_location_by_name(self, name):
         """Returns a location by its name, if exists."""
         for location in self.locations:
             if location.name == name:
                 return location
         return None  # or raise an exception if a location is not found
 
@@ -378,48 +435,54 @@
         ndlats = all_grid_global_rad_data.variables["lat"][:].filled()
         ndlons = all_grid_global_rad_data.variables["lon"][:].filled()
         long_grid, lat_grid = np.meshgrid(ndlons, ndlats)
         coordinates = np.dstack((lat_grid, long_grid)).reshape(-1, 2)
         return all_grid_global_rad_data, coordinates
 
     def _get_nearest_grid_point(self, latitude, longitude, grid_data):
-        all_grid_global_rad_data, _ = grid_data
+        def calculate_candidate_points(lat, lon, lat_res=0.05, lon_res=0.05):
+            lat_min = np.floor(lat / lat_res) * lat_res
+            lon_min = np.floor(lon / lon_res) * lon_res
+            return [
+                (lat_min, lon_min),
+                (lat_min, lon_min + lon_res),
+                (lat_min + lat_res, lon_min),
+                (lat_min + lat_res, lon_min + lon_res)
+            ]
 
-        # Calculate approximate indices based on the grid resolution of 0.05
-        lat_res = 0.05
-        lon_res = 0.05
-
-        lat_min = np.floor(latitude / lat_res) * lat_res
-        lon_min = np.floor(longitude / lon_res) * lon_res
-
-        # Four closest grid points to check
-        candidate_points = [
-            (lat_min, lon_min),
-            (lat_min, lon_min + lon_res),
-            (lat_min + lat_res, lon_min),
-            (lat_min + lat_res, lon_min + lon_res)
-        ]
+        def find_nearest_point(lat, lon, candidate_points):
+            distances = [
+                utils.haversine(lat, lon, c_lat, c_lon)
+                for c_lat, c_lon in candidate_points
+            ]
+            nearest_idx = np.argmin(distances)
+            return round(distances[nearest_idx], 3), candidate_points[nearest_idx]
 
-        # Compute distances for the four candidate points
-        distances = [
-            utils.haversine(latitude, longitude, lat, lon)
-            for lat, lon in candidate_points
-        ]
+        def get_grid_indices(grid_lat, grid_lon, grid_data):
+            lat_var = grid_data.variables["lat"][:]
+            lon_var = grid_data.variables["lon"][:]
+            lat_idx = np.argmin(np.abs(lat_var - grid_lat))
+            lon_idx = np.argmin(np.abs(lon_var - grid_lon))
+            return lat_idx, lon_idx
 
-        nearest_index = np.argmin(distances)
-        nearest_distance = round(distances[nearest_index], 3)
-        grid_latitude, grid_longitude = candidate_points[nearest_index]
-
-        # Find the nearest index in the grid data
-        lat_var = all_grid_global_rad_data.variables["lat"][:]
-        lon_var = all_grid_global_rad_data.variables["lon"][:]
-        lat_index = np.argmin(np.abs(lat_var - grid_latitude))
-        lon_index = np.argmin(np.abs(lon_var - grid_longitude))
+        all_grid_global_rad_data, _ = grid_data
+        candidate_points = calculate_candidate_points(latitude, longitude)
+        nearest_distance, (
+            grid_latitude, grid_longitude) = find_nearest_point(
+                latitude, longitude, candidate_points)
+        lat_index, lon_index = get_grid_indices(
+            grid_latitude, grid_longitude, all_grid_global_rad_data)
+
+        return (
+            lat_index * len(all_grid_global_rad_data.variables["lon"][:]) + lon_index,
+            nearest_distance,
+            round(grid_latitude, 2),
+            round(grid_longitude, 2)
+        )
 
-        return (lat_index * len(lon_var) + lon_index), nearest_distance, round(grid_latitude, 2), round(grid_longitude, 2)
 
     def _get_measurement_value_from_loaded_data(
         self, all_grid_global_rad_data, nearest_index
     ):
         lat_index = nearest_index // all_grid_global_rad_data.variables["lat"].shape[0]
         lon_index = nearest_index % all_grid_global_rad_data.variables["lat"].shape[0]
         measurement_value = all_grid_global_rad_data.variables["SIS"][:][
```

### Comparing `dwd_global_radiation-1.0.0rc6/dwd_global_radiation/utils.py` & `dwd_global_radiation-1.0.0rc7/dwd_global_radiation/utils.py`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.0.0rc6/dwd_global_radiation.egg-info/PKG-INFO` & `dwd_global_radiation-1.0.0rc7/dwd_global_radiation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.0.0rc6
+Version: 1.0.0rc7
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dwd_global_radiation-1.0.0rc6/setup.py` & `dwd_global_radiation-1.0.0rc7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='dwd_global_radiation',
-    version='1.0.0rc6',
+    version='1.0.0rc7',
     packages=find_packages(),
     description='Access and analyze DWD global radiation data and forecasts',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/aschmere/dwd_global_radiation',
     author='Arno Schmerer',
     license='MIT',
```

