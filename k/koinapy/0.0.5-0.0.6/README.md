# Comparing `tmp/koinapy-0.0.5.tar.gz` & `tmp/koinapy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koinapy-0.0.5.tar", max compression
+gzip compressed data, was "koinapy-0.0.6.tar", max compression
```

## Comparing `koinapy-0.0.5.tar` & `koinapy-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       37 2024-05-13 17:21:36.425215 koinapy-0.0.5/README.md
--rw-r--r--   0        0        0       24 2024-05-13 17:21:36.425215 koinapy-0.0.5/koinapy/__init__.py
--rw-r--r--   0        0        0      930 2024-05-13 17:21:36.425215 koinapy-0.0.5/koinapy/__main__.py
--rw-r--r--   0        0        0    28615 2024-05-13 17:21:36.425215 koinapy-0.0.5/koinapy/grpc.py
--rw-r--r--   0        0        0      783 2024-05-13 17:21:36.425215 koinapy-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 koinapy-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-24 07:55:58.570239 koinapy-0.0.6/README.md
+-rw-r--r--   0        0        0       24 2024-05-24 07:55:58.570239 koinapy-0.0.6/koinapy/__init__.py
+-rw-r--r--   0        0        0      930 2024-05-24 07:55:58.570239 koinapy-0.0.6/koinapy/__main__.py
+-rw-r--r--   0        0        0    29369 2024-05-24 07:55:58.570239 koinapy-0.0.6/koinapy/grpc.py
+-rw-r--r--   0        0        0      783 2024-05-24 07:55:58.570239 koinapy-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 koinapy-0.0.6/PKG-INFO
```

### Comparing `koinapy-0.0.5/koinapy/__main__.py` & `koinapy-0.0.6/koinapy/__main__.py`

 * *Files identical despite different names*

### Comparing `koinapy-0.0.5/koinapy/grpc.py` & `koinapy-0.0.6/koinapy/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         :param data: A dictionary containing input data for inference. Keys are input names, and values are numpy arrays.
 
         :return: A dictionary containing the model's predictions. Keys are output names, and values are numpy arrays representing
             the model's output.
         """
         predictions: Dict[str, np.ndarray] = {}
         for data_batch in tqdm(
-            self.__slice_dict(data, self.batchsize), desc="Getting predictions"
+            self.__slice_dict(data, self.batchsize), desc=f"{self.model_name}:"
         ):
             pred_batch = self.__predict_batch(data_batch)
             if predictions:
                 predictions = self.__merge_array_dict(predictions, pred_batch)
             else:
                 predictions = pred_batch  # Only first iteration to initialize dict keys
         return predictions
@@ -464,17 +464,19 @@
                 outputs=batch_outputs,
                 client_timeout=timeout,
             )
             yield
 
     def predict(
         self,
-        data: Union[Dict[str, np.ndarray], pd.DataFrame],
+        inputs: Union[Dict[str, np.ndarray], pd.DataFrame],
         mode="semi_async",
         debug=False,
+        df_output=True,
+        min_intensity=1e-4,
     ) -> Dict[str, np.ndarray]:
         """
         Perform inference on the given data using the Koina model.
 
         This method allows you to perform inference on the provided input data using the configured Koina model. You can
         choose to perform inference asynchronously (in parallel) or sequentially, depending on the value of the '_async'
         parameter. If asynchronous inference is selected, the method will return when all inference tasks are complete.
@@ -497,28 +499,49 @@
                 "precursor_charges": np.array([2 for _ in range(size)]),
                 "collision_energies": np.array([20 for _ in range(size)]),
                 "fragmentation_types": np.array(["HCD" for _ in range(size)]),
                 "instrument_types": np.array(["QE" for _ in range(size)])
             }
             predictions = model.predict(input_data)
         """
-        if isinstance(data, pd.DataFrame):
-            data = {
-                input_field: data[input_field].to_numpy().reshape(-1, 1)
+        if isinstance(inputs, pd.DataFrame):
+            dict_inputs = {
+                input_field: inputs[input_field].to_numpy().reshape(-1, 1)
                 for input_field in self.model_inputs.keys()
             }
+        else:
+            dict_inputs = inputs
+
         if mode == "semi_async":
-            return self.__predict_semi_async(data, debug=debug)
+            predictions = self.__predict_semi_async(dict_inputs, debug=debug)
         elif mode == "async":
-            return self.__predict_async(data, debug=debug)
+            predictions = self.__predict_async(dict_inputs, debug=debug)
         elif mode == "sync":
-            return self.__predict_sequential(data)
+            predictions = self.__predict_sequential(dict_inputs)
         else:
             raise ValueError(f"mode must be one of 'semi_async', 'async' or 'sync'")
 
+        if df_output and isinstance(inputs, pd.DataFrame):
+            return self.__construct_df(inputs, predictions, min_intensity=min_intensity)
+        else:
+            return predictions
+
+    def __construct_df(self, inputs, predictions, min_intensity=1e-4):
+        output_shape_dim1 = list(predictions.values())[0].shape[1]
+
+        tmp = inputs.apply(lambda x: np.repeat(x, output_shape_dim1))
+
+        for k, v in predictions.items():
+            tmp[k] = v.flatten()
+
+        if "intensities" in predictions:
+            tmp = tmp[tmp["intensities"] > min_intensity]
+
+        return tmp
+
     def __predict_semi_async(self, data, debug=False, disable_progress_bar=False):
         results = []
         data_subsets = list(self.__slice_dict(data, self.batchsize * 10))
         pbar = tqdm(
             total=ceil(next(iter(data.values())).shape[0] / self.batchsize),
             desc=f"{self.model_name}:",
             disable=disable_progress_bar,
```

### Comparing `koinapy-0.0.5/pyproject.toml` & `koinapy-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "koinapy"
-version = "0.0.5"
+version = "0.0.6"
 description = "Python client to communicate with Koina."
 authors = ["Ludwig Lautenbacher <Ludwig.Lautenbacher@tum.de>"]
 license = "Apache 2.0"
 homepage = "https://koina.wilhelmlab.org/"
 repository = "https://github.com/wilhelm-lab/koina"
 documentation = "https://koina.wilhelmlab.org/docs"
 readme = "README.md"
```

### Comparing `koinapy-0.0.5/PKG-INFO` & `koinapy-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koinapy
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python client to communicate with Koina.
 Home-page: https://koina.wilhelmlab.org/
 License: Apache 2.0
 Author: Ludwig Lautenbacher
 Author-email: Ludwig.Lautenbacher@tum.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
```

