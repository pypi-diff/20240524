# Comparing `tmp/hydra-callbacks-0.5.1.tar.gz` & `tmp/hydra_callbacks-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra-callbacks-0.5.1.tar", last modified: Wed Nov 15 10:47:53 2023, max compression
+gzip compressed data, was "hydra_callbacks-0.6.1.tar", last modified: Fri May 24 12:17:54 2024, max compression
```

## Comparing `hydra-callbacks-0.5.1.tar` & `hydra_callbacks-0.6.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:47:53.565699 hydra-callbacks-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:47:53.557699 hydra-callbacks-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:47:53.557699 hydra-callbacks-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/.github/workflows/master-cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/.github/workflows/tags-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/.github/workflows/test-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2023-11-15 10:47:53.561699 hydra-callbacks-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 10:47:53.565699 hydra-callbacks-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:47:53.557699 hydra-callbacks-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:47:53.557699 hydra-callbacks-0.5.1/src/hydra_callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/src/hydra_callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-15 10:47:53.000000 hydra-callbacks-0.5.1/src/hydra_callbacks/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10957 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/src/hydra_callbacks/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/src/hydra_callbacks/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/src/hydra_callbacks/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:47:53.561699 hydra-callbacks-0.5.1/src/hydra_callbacks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2023-11-15 10:47:53.000000 hydra-callbacks-0.5.1/src/hydra_callbacks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-11-15 10:47:53.000000 hydra-callbacks-0.5.1/src/hydra_callbacks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 10:47:53.000000 hydra-callbacks-0.5.1/src/hydra_callbacks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-15 10:47:53.000000 hydra-callbacks-0.5.1/src/hydra_callbacks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-15 10:47:53.000000 hydra-callbacks-0.5.1/src/hydra_callbacks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:47:53.561699 hydra-callbacks-0.5.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:47:53.561699 hydra-callbacks-0.5.1/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/tests/test_app/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/tests/test_app/dummy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/tests/test_app/dummy_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/tests/test_app/full_conf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/tests/test_app/gather_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/tests/test_app/gather_app_conf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/tests/test_app/git_callback.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/tests/test_app/latest_callback.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/tests/test_app/perf_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/tests/test_app/resource_monitor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/tests/test_app/runtime_perf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11647 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-11-15 10:47:04.000000 hydra-callbacks-0.5.1/tests/test_perflogger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:17:54.112318 hydra_callbacks-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:17:54.108318 hydra_callbacks-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:17:54.108318 hydra_callbacks-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/.github/workflows/master-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/.github/workflows/tags-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/.github/workflows/test-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-24 12:17:54.112318 hydra_callbacks-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:17:54.112318 hydra_callbacks-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:17:54.108318 hydra_callbacks-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:17:54.108318 hydra_callbacks-0.6.1/src/hydra_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/src/hydra_callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 12:17:54.000000 hydra_callbacks-0.6.1/src/hydra_callbacks/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/src/hydra_callbacks/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/src/hydra_callbacks/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/src/hydra_callbacks/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:17:54.112318 hydra_callbacks-0.6.1/src/hydra_callbacks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-24 12:17:54.000000 hydra_callbacks-0.6.1/src/hydra_callbacks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-24 12:17:54.000000 hydra_callbacks-0.6.1/src/hydra_callbacks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:17:54.000000 hydra_callbacks-0.6.1/src/hydra_callbacks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-24 12:17:54.000000 hydra_callbacks-0.6.1/src/hydra_callbacks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 12:17:54.000000 hydra_callbacks-0.6.1/src/hydra_callbacks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:17:54.112318 hydra_callbacks-0.6.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:17:54.112318 hydra_callbacks-0.6.1/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_app/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_app/dummy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_app/dummy_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_app/full_conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_app/gather_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_app/gather_app_conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_app/git_callback.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_app/latest_callback.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_app/perf_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_app/register_callback.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_app/resource_monitor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_app/runtime_perf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12864 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-24 12:17:04.000000 hydra_callbacks-0.6.1/tests/test_perflogger.py
```

### Comparing `hydra-callbacks-0.5.1/.github/workflows/master-cd.yml` & `hydra_callbacks-0.6.1/.github/workflows/master-cd.yml`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.5.1/.github/workflows/tags-release.yml` & `hydra_callbacks-0.6.1/.github/workflows/tags-release.yml`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.5.1/.github/workflows/test-ci.yml` & `hydra_callbacks-0.6.1/.github/workflows/test-ci.yml`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.5.1/LICENSE` & `hydra_callbacks-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.5.1/PKG-INFO` & `hydra_callbacks-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-callbacks
-Version: 0.5.1
+Version: 0.6.1
 Summary: A collection of usefull hydra callbacks for hydra configuration
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@cea.fr>
 Project-URL: Homepage, https://github.com/paquiteau/hydra-callbacks
 Project-URL: Bug Reports, https://github.com/paquiteau/hydra-callbacks/issues
 Project-URL: Sources, https://github.com/paquiteau/hydra-callbacks
 Keywords: hydra,configuration,callback
 Classifier: Development Status :: 3 - Alpha
@@ -16,14 +16,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hydra-core
 Requires-Dist: GitPython
 Requires-Dist: pandas
 Requires-Dist: numpy
+Requires-Dist: fastparquet
 Requires-Dist: psutil
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `hydra-callbacks-0.5.1/README.md` & `hydra_callbacks-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.5.1/pyproject.toml` & `hydra_callbacks-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 
 dependencies = [
   "hydra-core",
   "GitPython",
   "pandas",
   "numpy",
+  "fastparquet",
   "psutil",
 ]
 
 [project.optional-dependencies]
 dev = ["black", "isort", "ruff"]
 test = ["pytest", "pytest-cov", "pytest-xdist", "pytest-sugar"]
 
@@ -65,14 +66,15 @@
 where=["src"]
 
 
 [tool.setuptools_scm]
 write_to = "src/hydra_callbacks/_version.py"
 version_scheme = "python-simplified-semver"
 local_scheme="no-local-version"
+fallback_version="v99-dev"
 
 # Formatting using black.
 [tool.black]
 
 [tool.isort]
 profile="black"
```

### Comparing `hydra-callbacks-0.5.1/src/hydra_callbacks/callbacks.py` & `hydra_callbacks-0.6.1/src/hydra_callbacks/callbacks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Callback mechanism for hydra  jobs."""
+
 from __future__ import annotations
 from typing import Callable, Any
 import errno
 import glob
 import json
 import logging
 import os
 from pathlib import Path
 import time
 
 import pandas as pd
 from hydra.core.hydra_config import HydraConfig
-from hydra.core.utils import JobReturn
+from hydra.core.utils import JobReturn, JobStatus
 from hydra.experimental.callback import Callback
 from hydra.types import TaskFunction
 from hydra.utils import to_absolute_path
-from omegaconf import DictConfig, open_dict
+from omegaconf import DictConfig, open_dict, OmegaConf
 import omegaconf
 
 from .monitor import ResourceMonitorService
 
 callback_logger = logging.getLogger("hydra.callbacks")
 
 
@@ -203,15 +204,16 @@
 
     def _on_anyrun_end(self, run_dir: str, base_dir: str) -> None:
         latest_dir_path = os.path.join(base_dir, "latest")
         self._force_symlink(
             to_absolute_path(run_dir),
             to_absolute_path(latest_dir_path),
         )
-        callback_logger.info(f"Latest run is at: {latest_dir_path}")
+        callback_logger.info(f"Latest run is at: {run_dir}")
+        callback_logger.info(f"Latest run is also at: {latest_dir_path}")
 
     def _force_symlink(self, src: str, dest: str) -> None:
         """Create a symlink from src to test, overwriting dest if necessary."""
         try:
             os.symlink(src, dest)
         except OSError as e:
             if e.errno == errno.EEXIST:
@@ -232,14 +234,16 @@
     ----------
     enabled : bool
         if True, will log the total runtime.
     sample_interval : float or int
         The time interval at wat which to sample the process, in seconds.
     monitoring_file : str
         The file to write the monitoring data to.
+    gpu_monit: bool , default False
+        Also monitor gpu data.
     """
 
     _monitor: dict[tuple[str, str], Any]
 
     def __init__(
         self,
         enabled: bool = True,
@@ -295,14 +299,16 @@
         job_full_id = self._get_job_info()
         self._monitor[job_full_id].stop()
         sampled_data = self._monitor[job_full_id].get_values()
 
         del self._monitor[job_full_id]
         if sampled_data:
             df = pd.DataFrame(sampled_data)
+            df["job_name"] = job_full_id[0]
+            df["job_id"] = job_full_id[1]
             df.to_csv(
                 self.monitoring_file,
                 mode="a",
                 header=not os.path.exists(self.monitoring_file),
             )
             max_cpu = sampled_data["cpus"].max()
             max_mem = sampled_data["rss_GiB"].max()
@@ -316,7 +322,71 @@
         hconf = HydraConfig.get()
         name = hconf.job.name
         try:
             id = hconf.job.id
         except omegaconf.errors.MissingMandatoryValue:
             id = "0"
         return name, id
+
+
+class RegisterRunCallback(Callback):
+    """Callback that register the run in a .csv file at the end of the run.
+
+    Single and MultiRun are handled in different files. Note that this append one row
+    per config. Only the config is being registered, not the possible output of the run.
+
+    Parameters
+    ----------
+    enabled : bool
+        if True, will register the run.
+
+    register_file: str
+        name of the file to register the run in.
+    """
+
+    def __init__(
+        self,
+        enabled: bool = True,
+        register_file: str = "register.csv",
+        run_base_dir: str = "outputs",
+        multirun_base_dir: str = "multiruns",
+    ):
+        self.enabled = enabled
+        self.register_file = register_file
+        self.run_base_dir = to_absolute_path(run_base_dir)
+        self.multirun_base_dir = to_absolute_path(multirun_base_dir)
+        if not self.enabled:
+            self.on_job_end = dummy_run
+        else:
+            self.on_job_end = self._on_job_end  # type: ignore
+
+    def _on_job_end(
+        self, config: DictConfig, job_return: JobReturn, **kwargs: None
+    ) -> None:
+        """Execute after every job."""
+        # The hydra part of the conf is not resolvable (frozen)
+        # and we don't want to monitor it (if needed it would still be available in
+        # ``.hydra`` folder)
+        # Hence:
+        conf_ = OmegaConf.to_container(config)
+        conf_.pop("hydra")
+        conf_ = DictConfig(conf_)
+        OmegaConf.resolve(conf_)
+        conf_ = OmegaConf.to_container(conf_)
+        pandas_config = pd.json_normalize(conf_)
+        if config.hydra.mode == "MULTIRUN":
+            pandas_config["run-dir"] = config.hydra.sweep.dir
+            base_dir = self.multirun_base_dir
+        else:
+            pandas_config["run-dir"] = config.hydra.run.dir
+            base_dir = self.run_base_dir
+
+        pandas_config["job_success"] = job_return.status == JobStatus.COMPLETED
+
+        register_file = os.path.join(base_dir, self.register_file)
+        try:
+            df = pd.read_csv(register_file, index_col=None)
+            df = pd.concat([df, pandas_config])
+            df.to_csv(register_file, index=False)
+        except FileNotFoundError:
+            df = pd.DataFrame(pandas_config)
+            df.to_csv(register_file, index=False)
```

### Comparing `hydra-callbacks-0.5.1/src/hydra_callbacks/logger.py` & `hydra_callbacks-0.6.1/src/hydra_callbacks/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Performance tracking tool."""
+
 from time import perf_counter
 from logging import Logger
 import logging
 from typing import Callable
 
 
 class PerfLogger:
@@ -62,25 +63,26 @@
         self.timers["/".join(self.timers_stack)] = elapsed
         self.timers_stack.pop(-1)
         self.logger(formatted)
 
     @classmethod
     def recap(cls, logger: Logger | Callable | None = None) -> str:
         """Return a string summarizing all the registered timers."""
-        cls.timers["Total"] = sum(cls.timers.values())
+        cls.timers["Total"] = sum([t for n, t in cls.timers.items() if n != "Total"])
         ret = ", ".join([f"{name}: {t:.2f}s" for name, t in cls.timers.items()])
         if isinstance(logger, Logger):
             logger.info(ret)
         elif callable(logger):
             logger(ret)
         elif logger is not None:
             raise ValueError("logger must be a Logger or a callable")
         return ret
 
     @classmethod
     def reset(cls) -> None:
         """Reset all the registered timers."""
         cls.timers = {}
 
-    def get_timer(self, name: str) -> float:
+    @classmethod
+    def get_timer(cls, name: str) -> float:
         """Return the elapsed time of a timer."""
-        return self.timers[name]
+        return cls.timers[name]
```

### Comparing `hydra-callbacks-0.5.1/src/hydra_callbacks/monitor.py` & `hydra_callbacks-0.6.1/src/hydra_callbacks/monitor.py`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.5.1/src/hydra_callbacks.egg-info/PKG-INFO` & `hydra_callbacks-0.6.1/src/hydra_callbacks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-callbacks
-Version: 0.5.1
+Version: 0.6.1
 Summary: A collection of usefull hydra callbacks for hydra configuration
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@cea.fr>
 Project-URL: Homepage, https://github.com/paquiteau/hydra-callbacks
 Project-URL: Bug Reports, https://github.com/paquiteau/hydra-callbacks/issues
 Project-URL: Sources, https://github.com/paquiteau/hydra-callbacks
 Keywords: hydra,configuration,callback
 Classifier: Development Status :: 3 - Alpha
@@ -16,14 +16,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hydra-core
 Requires-Dist: GitPython
 Requires-Dist: pandas
 Requires-Dist: numpy
+Requires-Dist: fastparquet
 Requires-Dist: psutil
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `hydra-callbacks-0.5.1/src/hydra_callbacks.egg-info/SOURCES.txt` & `hydra_callbacks-0.6.1/src/hydra_callbacks.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -22,9 +22,10 @@
 tests/test_app/dummy_app.py
 tests/test_app/full_conf.yaml
 tests/test_app/gather_app.py
 tests/test_app/gather_app_conf.yaml
 tests/test_app/git_callback.yaml
 tests/test_app/latest_callback.yaml
 tests/test_app/perf_app.py
+tests/test_app/register_callback.yaml
 tests/test_app/resource_monitor.yaml
 tests/test_app/runtime_perf.yaml
```

### Comparing `hydra-callbacks-0.5.1/tests/test_app/gather_app.py` & `hydra_callbacks-0.6.1/tests/test_app/gather_app.py`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.5.1/tests/test_app/perf_app.py` & `hydra_callbacks-0.6.1/tests/test_app/perf_app.py`

 * *Files identical despite different names*

### Comparing `hydra-callbacks-0.5.1/tests/test_callbacks.py` & `hydra_callbacks-0.6.1/tests/test_callbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Test for callbacks.py module."""
+
 import os
 import shutil
 from pathlib import Path
 from textwrap import dedent
 import contextlib
 import pytest
+from datetime import datetime
 import git
 from hydra.test_utils.test_utils import (
     assert_regex_match,
+    assert_multiline_regex_search,
     _chdir_to_dir_containing,
     run_python_script,
 )
 
 import pandas as pd
 import numpy as np
 
@@ -184,39 +187,44 @@
 @pytest.mark.parametrize("multirun", [True, False])
 def test_latest_callback(tmpdir: Path, multirun: bool) -> None:
     """Test for latest callback."""
 
     cmd = [
         "tests/test_app/dummy_app.py",
         "--config-name=latest_callback",
-        "hydra.run.dir=" + str(tmpdir) + "/${now:%Y-%m-%d}/${now:%H-%M-%S-%f}",
-        "hydra.sweep.dir=" + str(tmpdir) + "/${now:%Y-%m-%d}/${now:%H-%M-%S-%f}",
+        "hydra.run.dir=" + str(tmpdir) + "/${now:%Y-%m-%d}/run_one",
+        "hydra.sweep.dir=" + str(tmpdir) + "/${now:%Y-%m-%d}/run_one",
         "hydra.callbacks.latest_callback.run_base_dir=" + str(tmpdir),
         "hydra.callbacks.latest_callback.multirun_base_dir=" + str(tmpdir),
         "hydra.job.chdir=False",
         "hydra.hydra_logging.formatters.simple.format='[HYDRA] %(message)s'",
         "hydra.job_logging.formatters.simple.format='[JOB] %(message)s'",
     ]
     cmd.insert(2, "--multirun") if multirun else None
     result, _err = run_python_script(cmd)
     assert _err == ""
     assert_regex_match(
         (HYDRA_LAUNCH_LOG if multirun else "")
         + dedent(
-            """\
+            r"""
             [JOB] foo: bar
 
-            [{logger}] Latest run is at: {tmpdir}/latest
+            [{logger}] Latest run is at: {tmpdir}/{now}/run_one
+            [{logger}] Latest run is also at: {tmpdir}/latest
             """.format(
-                tmpdir=tmpdir, logger="HYDRA" if multirun else "JOB"
+                tmpdir=tmpdir,
+                logger="HYDRA" if multirun else "JOB",
+                now=datetime.now().strftime("%Y-%m-%d"),
             )
         ),
         result,
     )
     first_run_dir = (tmpdir / "latest").readlink()
+    cmd[2] = "hydra.run.dir=" + str(tmpdir) + "/${now:%Y-%m-%d}/run_two"
+    cmd[3] = "hydra.sweep.dir=" + str(tmpdir) + "/${now:%Y-%m-%d}/run_two"
     result2, _err2 = run_python_script(cmd)
     next_run_dir = (tmpdir / "latest").readlink()
     assert first_run_dir != next_run_dir
     # Do it again, the symlink should be updated
 
 
 def test_multirun_gatherer(tmpdir: Path) -> None:
@@ -378,7 +386,31 @@
 
     df = pd.read_csv(tmpdir / "resource_monitoring.csv", index_col=0)
     # check that the sampling interval is respected
     assert len(df) >= 3 / 0.3
     np.testing.assert_allclose(df["time"].diff().mean(), sampling_time, rtol=0.05)
     # check that we got some activity on the cpu.
     assert df["cpus"].mean() > 0
+
+
+@pytest.mark.parametrize("multirun", [True, False])
+def test_register_callbacks(tmpdir: Path, multirun: bool) -> None:
+    cmd = [
+        "tests/test_app/dummy_app.py",
+        "--config-name=register_callback",
+        "hydra.run.dir=" + str(tmpdir) + "/${now:%Y-%m-%d_%H-%M-%S}/",
+        "hydra.sweep.dir=" + str(tmpdir) + "/sweep/${now:%Y-%m-%d_%H-%M-%S}/",
+        "++hydra.callbacks.register_callback.run_base_dir=" + str(tmpdir),
+        "++hydra.callbacks.register_callback.multirun_base_dir="
+        + str(tmpdir)
+        + "/sweep",
+        "hydra.job.chdir=false",
+        "hydra.verbose=true",
+        "++timestamp=${now:%Y-%m-%d_%H-%M-%S}",
+    ]
+
+    cmd.insert(2, "--multirun") if multirun else None
+    result, _err = run_python_script(cmd)
+    assert _err == ""
+    cmd.insert(-1, "++foo=barbar")
+    result, _err = run_python_script(cmd)
+    assert _err == ""
```

