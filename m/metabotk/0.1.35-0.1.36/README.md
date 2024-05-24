# Comparing `tmp/metabotk-0.1.35.tar.gz` & `tmp/metabotk-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabotk-0.1.35.tar", max compression
+gzip compressed data, was "metabotk-0.1.36.tar", max compression
```

## Comparing `metabotk-0.1.35.tar` & `metabotk-0.1.36.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2184 2024-05-23 10:36:38.955800 metabotk-0.1.35/README.md
--rw-r--r--   0        0        0      531 2024-05-23 10:28:10.899057 metabotk-0.1.35/metabotk/__init__.py
--rw-r--r--   0        0        0       23 2024-05-23 10:38:44.289244 metabotk-0.1.35/metabotk/_version.py
--rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.35/metabotk/cli.py
--rw-r--r--   0        0        0    26255 2024-05-23 10:33:39.163099 metabotk-0.1.35/metabotk/dataset_manager.py
--rw-r--r--   0        0        0     2388 2024-05-21 18:11:30.585916 metabotk-0.1.35/metabotk/dimensionality_reduction.py
--rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.35/metabotk/feature_selection.py
--rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.35/metabotk/imputation.py
--rw-r--r--   0        0        0     6549 2024-05-12 14:39:51.768689 metabotk-0.1.35/metabotk/interface.py
--rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.35/metabotk/missing_handler.py
--rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.35/metabotk/models_handler.py
--rw-r--r--   0        0        0     6051 2024-05-17 13:37:46.018747 metabotk-0.1.35/metabotk/normalization.py
--rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.35/metabotk/outliers_handler.py
--rw-r--r--   0        0        0     5527 2024-05-08 10:50:11.939978 metabotk-0.1.35/metabotk/providers_handler.py
--rw-r--r--   0        0        0     9052 2024-05-23 10:29:17.747712 metabotk-0.1.35/metabotk/statistics_handler.py
--rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.35/metabotk/utils.py
--rw-r--r--   0        0        0     4658 2024-05-10 15:46:25.623360 metabotk-0.1.35/metabotk/visualization_handler.py
--rw-r--r--   0        0        0      735 2024-05-23 10:38:52.105569 metabotk-0.1.35/pyproject.toml
--rw-r--r--   0        0        0     3137 1970-01-01 00:00:00.000000 metabotk-0.1.35/PKG-INFO
+-rw-r--r--   0        0        0     2184 2024-05-23 10:40:32.169618 metabotk-0.1.36/README.md
+-rw-r--r--   0        0        0      531 2024-05-23 10:28:10.899057 metabotk-0.1.36/metabotk/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-24 14:28:38.002332 metabotk-0.1.36/metabotk/_version.py
+-rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.36/metabotk/cli.py
+-rw-r--r--   0        0        0    26255 2024-05-23 10:33:39.163099 metabotk-0.1.36/metabotk/dataset_manager.py
+-rw-r--r--   0        0        0     2388 2024-05-21 18:11:30.585916 metabotk-0.1.36/metabotk/dimensionality_reduction.py
+-rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.36/metabotk/feature_selection.py
+-rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.36/metabotk/imputation.py
+-rw-r--r--   0        0        0     6549 2024-05-12 14:39:51.768689 metabotk-0.1.36/metabotk/interface.py
+-rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.36/metabotk/missing_handler.py
+-rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.36/metabotk/models_handler.py
+-rw-r--r--   0        0        0     9020 2024-05-24 10:56:48.094307 metabotk-0.1.36/metabotk/normalization.py
+-rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.36/metabotk/outliers_handler.py
+-rw-r--r--   0        0        0     5527 2024-05-08 10:50:11.939978 metabotk-0.1.36/metabotk/providers_handler.py
+-rw-r--r--   0        0        0     9052 2024-05-23 10:29:17.747712 metabotk-0.1.36/metabotk/statistics_handler.py
+-rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.36/metabotk/utils.py
+-rw-r--r--   0        0        0     4658 2024-05-10 15:46:25.623360 metabotk-0.1.36/metabotk/visualization_handler.py
+-rw-r--r--   0        0        0      735 2024-05-24 14:28:26.954051 metabotk-0.1.36/pyproject.toml
+-rw-r--r--   0        0        0     3137 1970-01-01 00:00:00.000000 metabotk-0.1.36/PKG-INFO
```

### Comparing `metabotk-0.1.35/README.md` & `metabotk-0.1.36/README.md`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/__init__.py` & `metabotk-0.1.36/metabotk/__init__.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/cli.py` & `metabotk-0.1.36/metabotk/cli.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/dataset_manager.py` & `metabotk-0.1.36/metabotk/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/dimensionality_reduction.py` & `metabotk-0.1.36/metabotk/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/feature_selection.py` & `metabotk-0.1.36/metabotk/feature_selection.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/imputation.py` & `metabotk-0.1.36/metabotk/imputation.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/interface.py` & `metabotk-0.1.36/metabotk/interface.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/missing_handler.py` & `metabotk-0.1.36/metabotk/missing_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/models_handler.py` & `metabotk-0.1.36/metabotk/models_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/normalization.py` & `metabotk-0.1.36/metabotk/normalization.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+import pandas as pd
 import pyserrf as srf
 from skloess import LOESS
 
 
 class NormalizationHandler:
     """
     Class for performing normalization on metabolomics data.
@@ -138,12 +140,108 @@
             other_columns=other_columns,
             n_correlated_metabolites=n_correlated_metabolites,
             random_state=random_state,
             threads=threads,
         )
         return raw_variations, normalized_variations
 
-    def loess_single_metabolite_single_batch(
-        self, metabolite_qc, metabolite_samples, degree, smoothing
+    def loess_single_metabolite(
+        self,
+        metabolite: str,
+        degree: int,
+        smoothing: float,
+        rescale: bool,
+        qc_samples: List[str],
+        injection_order_col: str,
+    ) -> pd.Series:
+        """
+        Perform LOESS normalization on a single metabolite.
+
+        Parameters
+        ----------
+        metabolite : str
+            The name of the metabolite to normalize.
+        degree : int
+            The degree of the LOESS polynomial.
+        smoothing : float
+            The smoothing parameter for LOESS.
+        rescale : bool
+            Whether to rescale the normalized values to the median.
+        qc_samples : List[str]
+            The names of the QC samples.
+        injection_order_col : str
+            The name of the column containing the injection order.
+
+        Returns
+        -------
+        pd.Series
+            The normalized values for the metabolite.
+        """
+        # Extract the metabolite and remove missing values
+        data = self._dataset_manager.extract_metabolites(metabolite)
+
+        # Extract the QC samples
+        qc = data.loc[qc_samples]
+        x_qc = qc[injection_order_col]
+        y_qc = qc[metabolite]
+
+        # Perform LOESS normalization
+        loess = LOESS(degree=degree, smoothing=smoothing)
+        loess.fit(x_qc.values, y_qc.values)
+        pred = loess.predict(data[injection_order_col].values)
+        norm = data[metabolite] - pred
+
+        # Rescale the normalized values if requested
+        if rescale:
+            median = data[metabolite].median()
+            norm = norm + median
+
+        return norm
+
+    def loess(
+        self,
+        degree: int,
+        smoothing: float,
+        rescale: bool,
+        qc_samples: List[str],
+        injection_order_col: str,
+        inplace: bool = True,
     ):
-        est = LOESS(degree=degree, smoothing=smoothing)
-        est.fit()
+        """
+        Perform LOESS normalization on all metabolites in the dataset.
+
+        Parameters
+        ----------
+        degree : int
+            The degree of the LOESS polynomial.
+        smoothing : float
+            The smoothing parameter for LOESS.
+        rescale : bool
+            Whether to rescale the normalized values to the median.
+        qc_samples : List[str]
+            The names of the QC samples.
+        injection_order_col : str
+            The name of the column containing the injection order.
+        inplace : bool, optional
+            Whether to perform the normalization inplace. Default is True.
+
+        Returns
+        -------
+        pd.DataFrame
+            The normalized data.
+        """
+        # Loop over all metabolites in the dataset
+        data = self._dataset_manager.data
+        for metabolite in self._dataset_manager.metabolites:
+            normalized_metabolite = self.loess_single_metabolite(
+                metabolite,
+                degree,
+                smoothing,
+                rescale,
+                qc_samples,
+                injection_order_col,
+            )
+            data[metabolite] = normalized_metabolite
+        if inplace:
+            self._dataset_manager.data = data
+        else:
+            return data
```

### Comparing `metabotk-0.1.35/metabotk/outliers_handler.py` & `metabotk-0.1.36/metabotk/outliers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/providers_handler.py` & `metabotk-0.1.36/metabotk/providers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/statistics_handler.py` & `metabotk-0.1.36/metabotk/statistics_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/utils.py` & `metabotk-0.1.36/metabotk/utils.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/metabotk/visualization_handler.py` & `metabotk-0.1.36/metabotk/visualization_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.35/pyproject.toml` & `metabotk-0.1.36/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metabotk"
-version = "0.1.35"
+version = "0.1.36"
 description = "Python toolkit for working with metabolomics data"
 authors = ["matteobolner <matteo.bolner2@unibo.it>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4"
 requests = "^2.31.0"
```

### Comparing `metabotk-0.1.35/PKG-INFO` & `metabotk-0.1.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabotk
-Version: 0.1.35
+Version: 0.1.36
 Summary: Python toolkit for working with metabolomics data
 Author: matteobolner
 Author-email: matteo.bolner2@unibo.it
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

