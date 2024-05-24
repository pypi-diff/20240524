# Comparing `tmp/mostlyai-0.3.6.tar.gz` & `tmp/mostlyai-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mostlyai-0.3.6.tar", max compression
+gzip compressed data, was "mostlyai-0.3.7.tar", max compression
```

## Comparing `mostlyai-0.3.6.tar` & `mostlyai-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-12-22 12:47:38.462094 mostlyai-0.3.6/LICENSE
--rw-r--r--   0        0        0     2438 2024-05-21 10:29:45.117002 mostlyai-0.3.6/README.md
--rw-r--r--   0        0        0       58 2024-05-15 08:25:32.630029 mostlyai-0.3.6/mostlyai/__init__.py
--rw-r--r--   0        0        0    14463 2024-05-21 10:29:45.117812 mostlyai-0.3.6/mostlyai/api.py
--rw-r--r--   0        0        0     9150 2024-04-19 16:58:34.132208 mostlyai-0.3.6/mostlyai/base.py
--rw-r--r--   0        0        0     3103 2024-05-13 15:27:45.794003 mostlyai-0.3.6/mostlyai/connectors.py
--rw-r--r--   0        0        0      574 2024-04-19 16:58:25.136734 mostlyai-0.3.6/mostlyai/exceptions.py
--rw-r--r--   0        0        0     4232 2024-05-21 10:29:45.118404 mostlyai-0.3.6/mostlyai/generators.py
--rw-r--r--   0        0        0    44710 2024-05-21 10:29:45.119013 mostlyai-0.3.6/mostlyai/model.py
--rw-r--r--   0        0        0     1694 2024-04-22 07:20:07.509641 mostlyai-0.3.6/mostlyai/shares.py
--rw-r--r--   0        0        0     6701 2024-05-21 10:29:45.119700 mostlyai-0.3.6/mostlyai/synthetic_datasets.py
--rw-r--r--   0        0        0     9491 2024-05-21 10:29:45.120294 mostlyai-0.3.6/mostlyai/utils.py
--rw-r--r--   0        0        0     1269 2024-05-21 10:55:44.122851 mostlyai-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 mostlyai-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-22 12:47:38.462094 mostlyai-0.3.7/LICENSE
+-rw-r--r--   0        0        0     2438 2024-05-21 10:29:45.117002 mostlyai-0.3.7/README.md
+-rw-r--r--   0        0        0      138 2024-05-24 05:24:06.051330 mostlyai-0.3.7/mostlyai/__init__.py
+-rw-r--r--   0        0        0    14726 2024-05-24 05:18:18.943839 mostlyai-0.3.7/mostlyai/api.py
+-rw-r--r--   0        0        0     9150 2024-04-19 16:58:34.132208 mostlyai-0.3.7/mostlyai/base.py
+-rw-r--r--   0        0        0     3103 2024-05-13 15:27:45.794003 mostlyai-0.3.7/mostlyai/connectors.py
+-rw-r--r--   0        0        0      574 2024-04-19 16:58:25.136734 mostlyai-0.3.7/mostlyai/exceptions.py
+-rw-r--r--   0        0        0     4232 2024-05-21 10:29:45.118404 mostlyai-0.3.7/mostlyai/generators.py
+-rw-r--r--   0        0        0    44710 2024-05-21 10:29:45.119013 mostlyai-0.3.7/mostlyai/model.py
+-rw-r--r--   0        0        0     1694 2024-04-22 07:20:07.509641 mostlyai-0.3.7/mostlyai/shares.py
+-rw-r--r--   0        0        0     6701 2024-05-21 10:29:45.119700 mostlyai-0.3.7/mostlyai/synthetic_datasets.py
+-rw-r--r--   0        0        0     9849 2024-05-24 05:18:18.945055 mostlyai-0.3.7/mostlyai/utils.py
+-rw-r--r--   0        0        0     1461 2024-05-24 05:24:06.001718 mostlyai-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 mostlyai-0.3.7/PKG-INFO
```

### Comparing `mostlyai-0.3.6/LICENSE` & `mostlyai-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.6/README.md` & `mostlyai-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.6/mostlyai/api.py` & `mostlyai-0.3.7/mostlyai/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,15 +260,22 @@
         :param seed: Optional. Either a single pandas DataFrame data, or a path to a CSV or PARQUET file, or a dictionary of those. Used for seeding the subject table(s).
         :param name: Optional. The name of the synthetic dataset.
         :param start: If true, then generation is started right away. Default: true.
         :param wait: If true, then the function only returns once generation has finished. Default: true.
         :param progress_bar: If true, then the progress bar will be displayed, in case of wait=True
         :return: The created synthetic dataset.
         """
-        config = _harmonize_sd_config(generator, size, seed, config, name)
+        config = _harmonize_sd_config(
+            generator,
+            get_generator=self.generators.get,
+            size=size,
+            seed=seed,
+            config=config,
+            name=name,
+        )
         sd = self.synthetic_datasets.create(config)
         rich.print(
             f"Created synthetic dataset "
             f"[link={self.base_url}/d/synthetic-datasets/{sd.id} blue underline]{sd.id}[/] "
             f"with generator "
             f"[link={self.base_url}/d/generators/{sd.generator.id} blue underline]{sd.generator.id}[/]"
         )
@@ -298,15 +305,21 @@
 
         :param generator: The generator instance or its UUID, that is to be used for generating synthetic data.
         :param config: The configuration parameters of the synthetic dataset to be created. See SyntheticDataset.config for the structure of the parameters.
         :param size: Optional. Either a single integer, or a dictionary of integers. Used for specifying the sample_size of the subject table(s).
         :param seed: Optional. Either a single pandas DataFrame data, or a path to a CSV or PARQUET file, or list of samples, or a dictionary of those. Used for seeding the subject table(s).
         :return: The created synthetic probe.
         """
-        config = _harmonize_sd_config(generator, size, seed, config)
+        config = _harmonize_sd_config(
+            generator,
+            get_generator=self.generators.get,
+            size=size,
+            seed=seed,
+            config=config,
+        )
         dfs = self.synthetic_probes.create(config)
         if return_type == "auto" and len(dfs) == 1:
             return list(dfs.values())[0]
         else:
             return dfs
 
     # SHARES
```

### Comparing `mostlyai-0.3.6/mostlyai/base.py` & `mostlyai-0.3.7/mostlyai/base.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.6/mostlyai/connectors.py` & `mostlyai-0.3.7/mostlyai/connectors.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.6/mostlyai/exceptions.py` & `mostlyai-0.3.7/mostlyai/exceptions.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.6/mostlyai/generators.py` & `mostlyai-0.3.7/mostlyai/generators.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.6/mostlyai/model.py` & `mostlyai-0.3.7/mostlyai/model.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.6/mostlyai/shares.py` & `mostlyai-0.3.7/mostlyai/shares.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.6/mostlyai/synthetic_datasets.py` & `mostlyai-0.3.7/mostlyai/synthetic_datasets.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.6/mostlyai/utils.py` & `mostlyai-0.3.7/mostlyai/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,39 +156,52 @@
 
 
 Seed = Union[pd.DataFrame, str, Path, list[dict[str, Any]]]
 
 
 def _harmonize_sd_config(
     generator: Union[Generator, str, None] = None,
+    get_generator: Union[Callable[[str], Generator], None] = None,
     size: Union[int, dict[str, int], None] = None,
     seed: Union[Seed, dict[str, Seed], None] = None,
     config: Union[dict, None] = None,
     name: Optional[str] = None,
 ) -> dict:
     config = config or {}
-    subject_tables = _get_subject_table_names(generator)
+    size = size if size is not None else {}
+    seed = seed if seed is not None else {}
 
-    # insert generatorId into config
     if isinstance(generator, Generator):
-        config["generatorId"] = str(generator.id)
+        generator_id = str(generator.id)
     elif generator is not None:
-        config["generatorId"] = str(generator)
+        generator_id = str(generator)
     elif "generatorId" not in config:
         raise ValueError(
             "Either a generator or a configuration with a generatorId must be provided."
         )
 
+    if (
+        not isinstance(size, dict)
+        or not isinstance(seed, dict)
+        or "tables" not in config
+    ):
+        if not isinstance(generator, Generator):
+            generator = get_generator(generator_id)
+        subject_tables = _get_subject_table_names(generator)
+    else:
+        subject_tables = []
+
+    # insert generatorId into config
+    config["generatorId"] = generator_id
+
     # normalize size
-    size = size if size is not None else {}
     if not isinstance(size, dict):
         size = {table: size for table in subject_tables}
 
     # normalize seed
-    seed = seed if seed is not None else {}
     if not isinstance(seed, dict):
         seed = {table: seed for table in subject_tables}
 
     # insert name into config
     if name is not None:
         config |= {"name": name}
```

### Comparing `mostlyai-0.3.6/pyproject.toml` & `mostlyai-0.3.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mostlyai"
-version = "0.3.6"
+version = "0.3.7"
 description = "The official Python client for the MOSTLY AI platform."
 homepage = "https://app.mostly.ai/"
 authors = ["MOSTLY AI <office@mostly.ai>"]
 license = "Proprietary"
 readme = "README.md"
 packages = [
     { include = "mostlyai" }
@@ -27,14 +27,15 @@
 ruff = "0.4.4"
 respx = "^0.20.2"
 twine = "^5.0.0"
 commitizen = "^3.18.0"
 mkdocs = "^1.5.3"
 mkdocstrings = "^0.24.1"
 mkdocs-material = "^9.5.13"
+poetry-bumpversion = "^0.3.2"
 
 [tool.mypy]
 python_version = "3.9"
 follow_imports = "silent"
 ignore_missing_imports = true
 warn_unused_to_dicts = true
 warn_redundant_casts = true
@@ -47,10 +48,15 @@
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
 version_provider = "poetry"
 update_changelog_on_bump = true
 major_version_zero = true
 
+[[tool.poetry_bumpversion.replacements]]
+files = ["mostlyai/__init__.py"]
+search = '__version__ = "{current_version}"'
+replace = '__version__ = "{new_version}"'
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mostlyai-0.3.6/PKG-INFO` & `mostlyai-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mostlyai
-Version: 0.3.6
+Version: 0.3.7
 Summary: The official Python client for the MOSTLY AI platform.
 Home-page: https://app.mostly.ai/
 License: Proprietary
 Author: MOSTLY AI
 Author-email: office@mostly.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

