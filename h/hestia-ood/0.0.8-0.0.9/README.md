# Comparing `tmp/hestia_ood-0.0.8.tar.gz` & `tmp/hestia_ood-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hestia_ood-0.0.8.tar", last modified: Fri May  3 10:29:16 2024, max compression
+gzip compressed data, was "hestia_ood-0.0.9.tar", last modified: Fri May 17 10:56:51 2024, max compression
```

## Comparing `hestia_ood-0.0.8.tar` & `hestia_ood-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:29:16.037675 hestia_ood-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-03 10:29:16.037675 hestia_ood-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:29:16.033675 hestia_ood-0.0.8/hestia/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    15677 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/dataset_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    25658 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    37111 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:29:16.033675 hestia_ood-0.0.8/hestia/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/utils/file_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/utils/graph_part_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/utils/label_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:29:16.037675 hestia_ood-0.0.8/hestia_ood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-03 10:29:16.000000 hestia_ood-0.0.8/hestia_ood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 10:29:16.000000 hestia_ood-0.0.8/hestia_ood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:29:16.000000 hestia_ood-0.0.8/hestia_ood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:29:15.000000 hestia_ood-0.0.8/hestia_ood.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 10:29:16.000000 hestia_ood-0.0.8/hestia_ood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 10:29:16.000000 hestia_ood-0.0.8/hestia_ood.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:29:16.037675 hestia_ood-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:56:50.998258 hestia_ood-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-17 10:56:50.998258 hestia_ood-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:56:50.994258 hestia_ood-0.0.9/hestia/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/hestia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/hestia/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16056 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/hestia/dataset_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25658 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/hestia/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/hestia/reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37111 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/hestia/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:56:50.998258 hestia_ood-0.0.9/hestia/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/hestia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/hestia/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/hestia/utils/file_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/hestia/utils/graph_part_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/hestia/utils/label_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:56:50.998258 hestia_ood-0.0.9/hestia_ood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-17 10:56:50.000000 hestia_ood-0.0.9/hestia_ood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-17 10:56:50.000000 hestia_ood-0.0.9/hestia_ood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:56:50.000000 hestia_ood-0.0.9/hestia_ood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:56:50.000000 hestia_ood-0.0.9/hestia_ood.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 10:56:50.000000 hestia_ood-0.0.9/hestia_ood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 10:56:50.000000 hestia_ood-0.0.9/hestia_ood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:56:50.998258 hestia_ood-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-17 10:56:47.000000 hestia_ood-0.0.9/setup.py
```

### Comparing `hestia_ood-0.0.8/LICENSE` & `hestia_ood-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hestia_ood-0.0.8/PKG-INFO` & `hestia_ood-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-ood
-Version: 0.0.8
+Version: 0.0.9
 Summary: Suite of tools for analysing the independence between training and evaluation biosequence datasets and to generate new generalisation-evaluating hold-out partitions
 Home-page: https://github.com/IBM/Hestia-OOD
 Author: Raul Fernandez-Diaz
 Author-email: raul.fernandezdiaz@ucdconnect.ie
 License: MIT
 Keywords: hestia
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hestia-ood Version: 0.0.8 Summary: Suite of tools
+Metadata-Version: 2.1 Name: hestia-ood Version: 0.0.9 Summary: Suite of tools
 for analysing the independence between training and evaluation biosequence
 datasets and to generate new generalisation-evaluating hold-out partitions
 Home-page: https://github.com/IBM/Hestia-OOD Author: Raul Fernandez-Diaz
 Author-email: raul.fernandezdiaz@ucdconnect.ie License: MIT Keywords: hestia
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
```

### Comparing `hestia_ood-0.0.8/README.md` & `hestia_ood-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hestia_ood-0.0.8/hestia/clustering.py` & `hestia_ood-0.0.9/hestia/clustering.py`

 * *Files identical despite different names*

### Comparing `hestia_ood-0.0.8/hestia/dataset_generator.py` & `hestia_ood-0.0.9/hestia/dataset_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             datasets will be generated.
         :type data: pd.DataFrame
         """
         self.data = data
         self.sim_df = None
         self.partitions = None
         print('Initialising Hestia Dataset Generator')
-        print(f'Number of items in data: {len(self.data)}')
+        print(f'Number of items in data: {len(self.data):,}')
 
     def from_precalculated(self, data_path: str):
         """Load partition indexes if they have already being calculated.
 
         :param data_path: Path to saved partition indexes.
         :type data_path: str
         """
@@ -256,18 +256,19 @@
         :param random_state: Seed for pseudo-random number
         generator algorithm, defaults to 42
         :type random_state: int, optional
         :param similarity_args: See similarity arguments entry, defaults to SimilarityArguments()
         :type similarity_args: SimilarityArguments, optional
         :raises ValueError: Partitioning algorithm not supported.
         """
-        print('Calculating partitions...')
         self.partitions = {}
         if self.sim_df is None:
             self.calculate_similarity(similarity_args)
+        print('Calculating partitions...')
+
         if partition_algorithm == 'ccpart':
             partition_algorithm = ccpart
         elif partition_algorithm == 'graph_part':
             partition_algorithm = graph_part
         else:
             raise ValueError(
                 f'Partition algorithm: {partition_algorithm} is not ' +
@@ -307,23 +308,31 @@
 
     def generate_datasets(self, dataset_type: str, threshold: float) -> dict:
         ds = {}
 
         if dataset_type == 'huggingface' or dataset_type == 'hf':
             try:
                 import datasets
+                import pyarrow as pa
             except ImportError:
                 raise ImportError(
                     f"This dataset_type: {dataset_type} requires `datasets` " +
                     "to be installed. Install using: `pip install datasets`"
                     )
             for key, value in self.partitions[threshold].items():
-                ds[key] = datasets.Dataset.from_pandas(
-                    self.data.iloc[value].reset_index()
-                )
+                try:
+                    ds[key] = datasets.Dataset.from_pandas(
+                        self.data.iloc[value].reset_index()
+                    )
+                except pa.ArrowInvalid:
+                    ds[key] = datasets.Dataset.from_dict({
+                        column: [row[column] for idx, row in
+                                 self.data.iloc[value].iterrows()]
+                        for column in self.data.columns
+                    })
             return ds
         elif dataset_type == 'pytorch' or dataset_type == 'torch':
             try:
                 from hestia.utils.dataset_utils import Dataset_from_pandas
             except ModuleNotFoundError:
                 raise ImportError(
                     f"This dataset_type: {dataset_type} requires `torch` " +
```

### Comparing `hestia_ood-0.0.8/hestia/partition.py` & `hestia_ood-0.0.9/hestia/partition.py`

 * *Files identical despite different names*

### Comparing `hestia_ood-0.0.8/hestia/reduction.py` & `hestia_ood-0.0.9/hestia/reduction.py`

 * *Files identical despite different names*

### Comparing `hestia_ood-0.0.8/hestia/similarity.py` & `hestia_ood-0.0.9/hestia/similarity.py`

 * *Files identical despite different names*

### Comparing `hestia_ood-0.0.8/hestia/utils/file_format.py` & `hestia_ood-0.0.9/hestia/utils/file_format.py`

 * *Files identical despite different names*

### Comparing `hestia_ood-0.0.8/hestia/utils/graph_part_utils.py` & `hestia_ood-0.0.9/hestia/utils/graph_part_utils.py`

 * *Files identical despite different names*

### Comparing `hestia_ood-0.0.8/hestia/utils/label_balance.py` & `hestia_ood-0.0.9/hestia/utils/label_balance.py`

 * *Files identical despite different names*

### Comparing `hestia_ood-0.0.8/hestia_ood.egg-info/PKG-INFO` & `hestia_ood-0.0.9/hestia_ood.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-ood
-Version: 0.0.8
+Version: 0.0.9
 Summary: Suite of tools for analysing the independence between training and evaluation biosequence datasets and to generate new generalisation-evaluating hold-out partitions
 Home-page: https://github.com/IBM/Hestia-OOD
 Author: Raul Fernandez-Diaz
 Author-email: raul.fernandezdiaz@ucdconnect.ie
 License: MIT
 Keywords: hestia
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hestia-ood Version: 0.0.8 Summary: Suite of tools
+Metadata-Version: 2.1 Name: hestia-ood Version: 0.0.9 Summary: Suite of tools
 for analysing the independence between training and evaluation biosequence
 datasets and to generate new generalisation-evaluating hold-out partitions
 Home-page: https://github.com/IBM/Hestia-OOD Author: Raul Fernandez-Diaz
 Author-email: raul.fernandezdiaz@ucdconnect.ie License: MIT Keywords: hestia
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
```

### Comparing `hestia_ood-0.0.8/setup.py` & `hestia_ood-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     keywords='hestia',
     name='hestia-ood',
     packages=find_packages(),
     long_description_content_type="text/markdown",
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/IBM/Hestia-OOD',
-    version='0.0.8',
+    version='0.0.9',
     zip_safe=False,
 )
```

