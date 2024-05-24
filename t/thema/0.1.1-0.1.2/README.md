# Comparing `tmp/thema-0.1.1.tar.gz` & `tmp/thema-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thema-0.1.1.tar", max compression
+gzip compressed data, was "thema-0.1.2.tar", max compression
```

## Comparing `thema-0.1.1.tar` & `thema-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    13690 2024-05-15 22:54:34.714820 thema-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     3862 2024-05-23 06:39:05.671417 thema-0.1.1/README.md
--rw-r--r--   0        0        0      857 2024-05-23 06:41:43.325832 thema-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       67 2024-05-20 21:04:36.092285 thema-0.1.1/thema/__init__.py
--rw-r--r--   0        0        0     5513 2024-05-20 21:04:36.093771 thema-0.1.1/thema/config.py
--rw-r--r--   0        0        0     9151 2024-05-20 21:04:36.094484 thema-0.1.1/thema/core.py
--rw-r--r--   0        0        0      185 2024-05-20 21:04:36.094663 thema-0.1.1/thema/multiverse/__init__.py
--rw-r--r--   0        0        0     9864 2024-05-20 21:04:36.095872 thema-0.1.1/thema/multiverse/system/inner/inner_utils.py
--rw-r--r--   0        0        0     7190 2024-05-20 21:04:36.096553 thema-0.1.1/thema/multiverse/system/inner/moon.py
--rw-r--r--   0        0        0    21301 2024-05-20 21:04:36.097282 thema-0.1.1/thema/multiverse/system/inner/planet.py
--rw-r--r--   0        0        0     2749 2024-05-20 21:04:36.097892 thema-0.1.1/thema/multiverse/system/outer/comet.py
--rw-r--r--   0        0        0    13750 2024-05-20 21:04:36.098622 thema-0.1.1/thema/multiverse/system/outer/oort.py
--rw-r--r--   0        0        0     2323 2024-05-20 21:04:36.099577 thema-0.1.1/thema/multiverse/system/outer/projectiles/pcaProj.py
--rw-r--r--   0        0        0     2463 2024-05-20 21:04:36.100216 thema-0.1.1/thema/multiverse/system/outer/projectiles/tsneProj.py
--rw-r--r--   0        0        0     2811 2024-05-20 21:04:36.100763 thema-0.1.1/thema/multiverse/system/outer/projectiles/umapProj.py
--rw-r--r--   0        0        0    17189 2024-05-20 21:04:36.102031 thema-0.1.1/thema/multiverse/universe/galaxy.py
--rw-r--r--   0        0        0     3216 2024-05-20 21:04:36.103184 thema-0.1.1/thema/multiverse/universe/geodesics.py
--rw-r--r--   0        0        0     2283 2024-05-20 21:04:36.103934 thema-0.1.1/thema/multiverse/universe/star.py
--rw-r--r--   0        0        0     6526 2024-05-20 21:04:36.104883 thema-0.1.1/thema/multiverse/universe/starGraph.py
--rw-r--r--   0        0        0      169 2024-05-20 21:04:36.105938 thema-0.1.1/thema/multiverse/universe/starSelectors.py
--rw-r--r--   0        0        0    11388 2024-05-20 21:04:36.106873 thema-0.1.1/thema/multiverse/universe/stars/jmapStar.py
--rw-r--r--   0        0        0      166 2024-05-20 21:04:36.107111 thema-0.1.1/thema/probe/__init__.py
--rw-r--r--   0        0        0     9678 2024-05-20 21:04:36.108167 thema-0.1.1/thema/probe/data_utils.py
--rw-r--r--   0        0        0    22921 2024-05-20 21:04:36.109063 thema-0.1.1/thema/probe/observatories/jmapObservatory.py
--rw-r--r--   0        0        0     4932 2024-05-20 21:04:36.110248 thema-0.1.1/thema/probe/observatory.py
--rw-r--r--   0        0        0    22100 2024-05-20 21:04:36.111781 thema-0.1.1/thema/probe/telescope.py
--rw-r--r--   0        0        0     7151 2024-05-20 21:04:36.112304 thema-0.1.1/thema/probe/visual_utils.py
--rw-r--r--   0        0        0     5923 2024-05-20 21:04:36.112933 thema-0.1.1/thema/utils.py
--rw-r--r--   0        0        0     5040 1970-01-01 00:00:00.000000 thema-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    13690 2024-05-15 22:54:34.714820 thema-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     3862 2024-05-23 06:39:05.671417 thema-0.1.2/README.md
+-rw-r--r--   0        0        0      857 2024-05-24 18:19:01.552461 thema-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       67 2024-05-20 21:04:36.092285 thema-0.1.2/thema/__init__.py
+-rw-r--r--   0        0        0     5513 2024-05-20 21:04:36.093771 thema-0.1.2/thema/config.py
+-rw-r--r--   0        0        0     9151 2024-05-20 21:04:36.094484 thema-0.1.2/thema/core.py
+-rw-r--r--   0        0        0      185 2024-05-20 21:04:36.094663 thema-0.1.2/thema/multiverse/__init__.py
+-rw-r--r--   0        0        0     9878 2024-05-24 18:14:59.185287 thema-0.1.2/thema/multiverse/system/inner/inner_utils.py
+-rw-r--r--   0        0        0     7415 2024-05-24 18:14:59.186410 thema-0.1.2/thema/multiverse/system/inner/moon.py
+-rw-r--r--   0        0        0    21454 2024-05-24 18:14:59.187516 thema-0.1.2/thema/multiverse/system/inner/planet.py
+-rw-r--r--   0        0        0     2749 2024-05-20 21:04:36.097892 thema-0.1.2/thema/multiverse/system/outer/comet.py
+-rw-r--r--   0        0        0    13750 2024-05-20 21:04:36.098622 thema-0.1.2/thema/multiverse/system/outer/oort.py
+-rw-r--r--   0        0        0     2323 2024-05-20 21:04:36.099577 thema-0.1.2/thema/multiverse/system/outer/projectiles/pcaProj.py
+-rw-r--r--   0        0        0     2463 2024-05-20 21:04:36.100216 thema-0.1.2/thema/multiverse/system/outer/projectiles/tsneProj.py
+-rw-r--r--   0        0        0     2811 2024-05-20 21:04:36.100763 thema-0.1.2/thema/multiverse/system/outer/projectiles/umapProj.py
+-rw-r--r--   0        0        0    17189 2024-05-20 21:04:36.102031 thema-0.1.2/thema/multiverse/universe/galaxy.py
+-rw-r--r--   0        0        0     3216 2024-05-20 21:04:36.103184 thema-0.1.2/thema/multiverse/universe/geodesics.py
+-rw-r--r--   0        0        0     2283 2024-05-20 21:04:36.103934 thema-0.1.2/thema/multiverse/universe/star.py
+-rw-r--r--   0        0        0     6526 2024-05-20 21:04:36.104883 thema-0.1.2/thema/multiverse/universe/starGraph.py
+-rw-r--r--   0        0        0      169 2024-05-20 21:04:36.105938 thema-0.1.2/thema/multiverse/universe/starSelectors.py
+-rw-r--r--   0        0        0    11388 2024-05-20 21:04:36.106873 thema-0.1.2/thema/multiverse/universe/stars/jmapStar.py
+-rw-r--r--   0        0        0      166 2024-05-20 21:04:36.107111 thema-0.1.2/thema/probe/__init__.py
+-rw-r--r--   0        0        0     9678 2024-05-20 21:04:36.108167 thema-0.1.2/thema/probe/data_utils.py
+-rw-r--r--   0        0        0    22921 2024-05-20 21:04:36.109063 thema-0.1.2/thema/probe/observatories/jmapObservatory.py
+-rw-r--r--   0        0        0     4932 2024-05-20 21:04:36.110248 thema-0.1.2/thema/probe/observatory.py
+-rw-r--r--   0        0        0    22100 2024-05-20 21:04:36.111781 thema-0.1.2/thema/probe/telescope.py
+-rw-r--r--   0        0        0     7151 2024-05-20 21:04:36.112304 thema-0.1.2/thema/probe/visual_utils.py
+-rw-r--r--   0        0        0     5923 2024-05-20 21:04:36.112933 thema-0.1.2/thema/utils.py
+-rw-r--r--   0        0        0     5040 1970-01-01 00:00:00.000000 thema-0.1.2/PKG-INFO
```

### Comparing `thema-0.1.1/LICENSE.md` & `thema-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/README.md` & `thema-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/pyproject.toml` & `thema-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thema"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = [
     "jeremy.wayland <jeremy.don.wayland@gmail.com>",
     "stuart.wayland <swayland@ucsc.edu>",
     "sid.gathrid <sgathrid@yahoo.com>",
 ]
 readme = "README.md"
```

### Comparing `thema-0.1.1/thema/config.py` & `thema-0.1.2/thema/config.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/core.py` & `thema-0.1.2/thema/core.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/multiverse/system/inner/inner_utils.py` & `thema-0.1.2/thema/multiverse/system/inner/inner_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,17 @@
     2    2.0
     3    3.0
     4    3.0
     5    2.0
     dtype: float64
     """
     column = column.copy()
-    mode_value = column.mode().iloc[0]  # Get the first mode if multiple modes exist
+    mode_value = column.mode().iloc[
+        0
+    ]  # Get the first mode if multiple modes exist
     column.fillna(mode_value, inplace=True)
     return column
 
 
 def median(column, seed):
     """
     Fill in missing data in a column based on its median value.
```

### Comparing `thema-0.1.1/thema/multiverse/system/inner/moon.py` & `thema-0.1.2/thema/multiverse/system/inner/moon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # File: multiverse/system/inner/moon.py
 # Last Update: 05/15/24
 # Updated By: JW
 
 import pickle
+import warnings
 
 import category_encoders as ce
 import pandas as pd
 from sklearn.preprocessing import StandardScaler
 
 from ....core import Core
 from . import inner_utils
 
 
 class Moon(Core):
     """
-    Modify, Omit, Oscillate and Normalize.
+    The Moon: Modify, Omit, Oscillate and Normalize.
     ----------
 
     The Moon data class resides cosmically near to the original raw dataset.
     This class handles a multitude of individual preprocessing steps helpful
     for smooth computation and analysis farther downstream the analysis pipeline.
 
     The intended use of this class is simplify the cleaning process and
@@ -128,36 +129,43 @@
         numeric, and complete representation of the original raw data set.
 
         Examples
         ----------
         >>> moon = Moon()
         >>> moon.fit()
         """
-        # Cleaning procedure
-        if not self.dropColumns == [] and all(
-            column in self.data.columns for column in self.dropColumns
-        ):
-            self.imputeData = self.data.drop(columns=self.dropColumns)
-        else:
-            self.imputeData = self.data
-
-        self.imputeData = inner_utils.add_imputed_flags(self.data, self.imputeColumns)
 
+        self.imputeData = inner_utils.add_imputed_flags(
+            self.data, self.imputeColumns
+        )
         for index, column in enumerate(self.imputeColumns):
             impute_function = getattr(inner_utils, self.imputeMethods[index])
-            self.imputeData[column] = impute_function(self.data[column], self.seed)
+            self.imputeData[column] = impute_function(
+                self.data[column], self.seed
+            )
+
+        self.dropColumns = [
+            col for col in self.dropColumns if col in self.data.columns
+        ]
+        # Drop Columns
+        if not self.dropColumns == []:
+            self.imputeData = self.data.drop(columns=self.dropColumns)
 
-        # Drops unaccounted columns
-        self.imputeData.dropna(axis=1, inplace=True)
+        # Drop Rows with Nans
+        self.imputeData.dropna(axis=0, inplace=True)
 
         if type(self.encoding) == str:
             self.encoding = [
                 self.encoding
                 for _ in range(
-                    len(self.imputeData.select_dtypes(include=["object"]).columns)
+                    len(
+                        self.imputeData.select_dtypes(
+                            include=["object"]
+                        ).columns
+                    )
                 )
             ]
 
         # Encoding
         assert len(self.encoding) == len(
             self.imputeData.select_dtypes(include=["object"]).columns
         ), f"length of encoding: {len(self.encoding)}, length of cat variables: {len(self.imputeData.select_dtypes(include=['object']).columns)}"
@@ -176,16 +184,20 @@
             elif encoding == "integer":
                 if self.imputeData[column].dtype == object:
                     vals = self.imputeData[column].values
                     self.imputeData[column] = inner_utils.integer_encoder(vals)
 
             elif encoding == "hash":
                 if self.imputeData[column].dtype == object:
-                    hashing_encoder = ce.HashingEncoder(cols=[column], n_components=10)
-                    self.imputeData = hashing_encoder.fit_transform(self.imputeData)
+                    hashing_encoder = ce.HashingEncoder(
+                        cols=[column], n_components=10
+                    )
+                    self.imputeData = hashing_encoder.fit_transform(
+                        self.imputeData
+                    )
 
             else:
                 pass
 
         # Scaling
         assert self.scaler in ["standard"], "Invalid Scaler"
         if self.scaler == "standard":
```

### Comparing `thema-0.1.1/thema/multiverse/system/inner/planet.py` & `thema-0.1.2/thema/multiverse/system/inner/planet.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,34 +312,40 @@
             self.dropColumns = dropColumns
 
         if imputeColumns is None or imputeColumns == "None":
             self.imputeColumns = []
 
         elif imputeColumns == "all":
 
-            self.imputeColumns = self.data.columns[self.data.isna().any()].tolist()
+            self.imputeColumns = self.data.columns[
+                self.data.isna().any()
+            ].tolist()
 
         elif type(imputeColumns) == ListConfig or type(imputeColumns) == list:
             self.imputeColumns = imputeColumns
             for c in imputeColumns:
                 if c not in self.data.columns:
                     print("Invalid impute column. Defaulting to 'None'")
                     self.imputeColumns = []
         else:
             self.imputeColumns = []
 
         if imputeMethods is None or imputeMethods == "None":
-            self.imputeMethods = ["drop" for _ in range(len(self.imputeColumns))]
+            self.imputeMethods = [
+                "drop" for _ in range(len(self.imputeColumns))
+            ]
 
         elif type(imputeMethods) == str:
             if not imputeMethods in supported_imputeMethods:
                 print("Invalid impute methods. Defaulting to 'drop'")
                 imputeMethods = "drop"
                 self.numSamples = 1
-            self.imputeMethods = [imputeMethods for _ in range(len(self.imputeColumns))]
+            self.imputeMethods = [
+                imputeMethods for _ in range(len(self.imputeColumns))
+            ]
         else:
             assert len(imputeMethods) == len(
                 self.imputeColumns
             ), f"Lengh of imputeMethods: {len(imputeMethods)} must match length of imputeColumns: {len(self.imputeColumns)}"
             for index, method in enumerate(imputeMethods):
                 if not method in supported_imputeMethods:
                     print("Invalid impute methods. Defaulting to 'drop'")
@@ -517,32 +523,37 @@
         --------
         >>> planet = Planet()
         >>> planet._instantiate_moon(1)
         """
 
         if self.seeds is None:
             self.seeds = dict()
-        self.seeds[id] = np.random.randint(0, 1000)
+            self.seeds[id] = np.random.randint(0, 1000)
 
         my_moon = Moon(
             data=self.get_data_path(),
             dropColumns=self.dropColumns,
             encoding=self.encoding,
             scaler=self.scaler,
             imputeColumns=self.imputeColumns,
             imputeMethods=self.imputeMethods,
             seed=self.seeds[id],
             id=id,
         )
         my_moon.fit()
 
-        filename_without_extension, extension = os.path.splitext(self.get_data_path())
+        filename_without_extension, extension = os.path.splitext(
+            self.get_data_path()
+        )
         data_name = filename_without_extension.split("/")[-1]
         file_name = clean_data_filename(
-            data_name=data_name, id=id, scaler=self.scaler, encoding=self.encoding
+            data_name=data_name,
+            id=id,
+            scaler=self.scaler,
+            encoding=self.encoding,
         )
         output_filepath = os.path.join(self.outDir, file_name)
 
         my_moon.save(file_path=output_filepath)
 
     def getParams(self) -> dict:
         """
```

### Comparing `thema-0.1.1/thema/multiverse/system/outer/comet.py` & `thema-0.1.2/thema/multiverse/system/outer/comet.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/multiverse/system/outer/oort.py` & `thema-0.1.2/thema/multiverse/system/outer/oort.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/multiverse/system/outer/projectiles/pcaProj.py` & `thema-0.1.2/thema/multiverse/system/outer/projectiles/pcaProj.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/multiverse/system/outer/projectiles/tsneProj.py` & `thema-0.1.2/thema/multiverse/system/outer/projectiles/tsneProj.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/multiverse/system/outer/projectiles/umapProj.py` & `thema-0.1.2/thema/multiverse/system/outer/projectiles/umapProj.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/multiverse/universe/galaxy.py` & `thema-0.1.2/thema/multiverse/universe/galaxy.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/multiverse/universe/geodesics.py` & `thema-0.1.2/thema/multiverse/universe/geodesics.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/multiverse/universe/star.py` & `thema-0.1.2/thema/multiverse/universe/star.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/multiverse/universe/starGraph.py` & `thema-0.1.2/thema/multiverse/universe/starGraph.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/multiverse/universe/stars/jmapStar.py` & `thema-0.1.2/thema/multiverse/universe/stars/jmapStar.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/probe/data_utils.py` & `thema-0.1.2/thema/probe/data_utils.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/probe/observatories/jmapObservatory.py` & `thema-0.1.2/thema/probe/observatories/jmapObservatory.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/probe/observatory.py` & `thema-0.1.2/thema/probe/observatory.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/probe/telescope.py` & `thema-0.1.2/thema/probe/telescope.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/probe/visual_utils.py` & `thema-0.1.2/thema/probe/visual_utils.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/thema/utils.py` & `thema-0.1.2/thema/utils.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.1/PKG-INFO` & `thema-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thema
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: jeremy.wayland
 Author-email: jeremy.don.wayland@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

