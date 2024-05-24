# Comparing `tmp/utilix-0.8.3.tar.gz` & `tmp/utilix-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilix-0.8.3.tar", last modified: Mon Apr 22 19:10:26 2024, max compression
+gzip compressed data, was "utilix-0.8.4.tar", last modified: Fri May 24 19:59:02 2024, max compression
```

## Comparing `utilix-0.8.3.tar` & `utilix-0.8.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:26.531867 utilix-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)    17292 2024-04-22 19:10:26.531867 utilix-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-22 19:10:24.000000 utilix-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:10:26.531867 utilix-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-22 19:10:24.000000 utilix-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:26.527867 utilix-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:24.000000 utilix-0.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-22 19:10:24.000000 utilix-0.8.3/tests/test_batchq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-22 19:10:24.000000 utilix-0.8.3/tests/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-22 19:10:24.000000 utilix-0.8.3/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-22 19:10:24.000000 utilix-0.8.3/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-04-22 19:10:24.000000 utilix-0.8.3/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-22 19:10:24.000000 utilix-0.8.3/tests/test_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:26.527867 utilix-0.8.3/utilix/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-22 19:10:24.000000 utilix-0.8.3/utilix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20057 2024-04-22 19:10:24.000000 utilix-0.8.3/utilix/batchq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-22 19:10:24.000000 utilix-0.8.3/utilix/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-22 19:10:24.000000 utilix-0.8.3/utilix/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    23294 2024-04-22 19:10:24.000000 utilix-0.8.3/utilix/mongo_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-04-22 19:10:24.000000 utilix-0.8.3/utilix/rundb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:26.531867 utilix-0.8.3/utilix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17292 2024-04-22 19:10:26.000000 utilix-0.8.3/utilix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-22 19:10:26.000000 utilix-0.8.3/utilix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:10:26.000000 utilix-0.8.3/utilix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-22 19:10:26.000000 utilix-0.8.3/utilix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 19:10:26.000000 utilix-0.8.3/utilix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:59:02.096509 utilix-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    17292 2024-05-24 19:59:02.096509 utilix-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-05-24 19:58:59.000000 utilix-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 19:59:02.096509 utilix-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-24 19:58:59.000000 utilix-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:59:02.092509 utilix-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:58:59.000000 utilix-0.8.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-05-24 19:58:59.000000 utilix-0.8.4/tests/test_batchq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-24 19:58:59.000000 utilix-0.8.4/tests/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-24 19:58:59.000000 utilix-0.8.4/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-24 19:58:59.000000 utilix-0.8.4/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-24 19:58:59.000000 utilix-0.8.4/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-24 19:58:59.000000 utilix-0.8.4/tests/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:59:02.092509 utilix-0.8.4/utilix/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-24 19:58:59.000000 utilix-0.8.4/utilix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20110 2024-05-24 19:58:59.000000 utilix-0.8.4/utilix/batchq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-24 19:58:59.000000 utilix-0.8.4/utilix/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-24 19:58:59.000000 utilix-0.8.4/utilix/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23294 2024-05-24 19:58:59.000000 utilix-0.8.4/utilix/mongo_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-05-24 19:58:59.000000 utilix-0.8.4/utilix/rundb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:59:02.096509 utilix-0.8.4/utilix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17292 2024-05-24 19:59:01.000000 utilix-0.8.4/utilix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-24 19:59:02.000000 utilix-0.8.4/utilix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:59:01.000000 utilix-0.8.4/utilix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-24 19:59:01.000000 utilix-0.8.4/utilix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 19:59:01.000000 utilix-0.8.4/utilix.egg-info/top_level.txt
```

### Comparing `utilix-0.8.3/PKG-INFO` & `utilix-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilix
-Version: 0.8.3
+Version: 0.8.4
 Summary: User-friendly interface to various utilities for XENON users
 Home-page: https://github.com/XENONnT/utilix
 License: UNKNOWN
 Description: # utilix
         [![PyPI version shields.io](https://img.shields.io/pypi/v/utilix.svg)](https://pypi.python.org/pypi/utilix/)
         
         ``utilix`` is a utility package for XENON software, mainly relating to analysis. It currently has two main features: (1) a general XENON configuration framework and (2) easy access to the runsDB by wrapping python calls to a RESTful API. Eventually, we would like to include easy functions for interacting with the Midway and OSG batch queues.
```

### Comparing `utilix-0.8.3/README.md` & `utilix-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `utilix-0.8.3/setup.py` & `utilix-0.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     readme = file.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setup(
     name="utilix",
-    version="0.8.3",
+    version="0.8.4",
     url='https://github.com/XENONnT/utilix',
     description="User-friendly interface to various utilities for XENON users",
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=requires,
     python_requires=">=3.6",
     long_description=readme + '\n\n' + history,
```

### Comparing `utilix-0.8.3/tests/test_batchq.py` & `utilix-0.8.4/tests/test_batchq.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,26 +63,30 @@
         JobSubmission(
             jobstring="Hello World", qos="xenon1t", hours=10, container="invalid.ext"
         )
     assert "Container must end with .simg" in str(exc_info.value)
 
 
 def test_valid_container(valid_job_submission: JobSubmission):
-    """Test case to check if a valid container value is accepted."""
-    assert valid_job_submission.container == "xenonnt-development.simg"
+    """Test case to check if a valid path for the container is found."""
+    assert "xenonnt-development.simg" in valid_job_submission.container
 
 
 def test_container_exists(valid_job_submission: JobSubmission, tmp_path: str):
-    """Test case to check if the appropriate validation error is raised when the specified container does not exist."""
-    with patch.dict("utilix.batchq.SINGULARITY_DIR", {"xenon1t": str(tmp_path)}):
+    """
+    Test case to check if the appropriate validation error is raised when the specified container does not exist.
+    """
+    invalid_container = "nonexistent-container.simg"
+    with patch.object(batchq, "SINGULARITY_DIR", "/lgrandi/xenonnt/singularity-images"):
         with pytest.raises(FileNotFoundError) as exc_info:
-            JobSubmission(**valid_job_submission.dict())
-        assert "Singularity image xenonnt-development.simg does not exist" in str(
-            exc_info.value
-        )
+            JobSubmission(
+                **valid_job_submission.dict(exclude={"container"}),
+                container=invalid_container,
+            )
+        assert f"Container {invalid_container} does not exist" in str(exc_info.value)
 
 
 def test_bypass_validation_qos(valid_job_submission: JobSubmission):
     """
     Test case to check if the validation for the qos field is skipped when it is included in the bypass_validation list.
     """
     job_submission_data = valid_job_submission.dict().copy()
@@ -148,9 +152,7 @@
     for field_name in job_submission_fields:
         if field_name not in submit_job_params:
             missing_params.append(field_name)
 
     assert (
         len(missing_params) == 0
     ), f"Missing parameters in submit_job: {', '.join(missing_params)}"
-
-
```

### Comparing `utilix-0.8.3/tests/test_get.py` & `utilix-0.8.4/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `utilix-0.8.3/tests/test_query.py` & `utilix-0.8.4/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `utilix-0.8.3/tests/test_update.py` & `utilix-0.8.4/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `utilix-0.8.3/tests/test_url.py` & `utilix-0.8.4/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `utilix-0.8.3/utilix/batchq.py` & `utilix-0.8.4/utilix/batchq.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 if USER is None:
     raise ValueError("USER environment variable is not set")
 
 SCRATCH_DIR: str = os.environ.get("SCRATCH", ".")
 # SCRATCH_DIR must have write permission
 if not os.access(SCRATCH_DIR, os.W_OK):
     raise ValueError(
-        f"SCRATCH_DIR {SCRATCH_DIR} does not have write permission."
+        f"SCRATCH_DIR {SCRATCH_DIR} does not have write permission. "
         "You may need to set SCRATCH_DIR manually in your .bashrc or .bash_profile."
     )
 
 PARTITIONS: List[str] = [
     "dali",
     "lgrandi",
     "xenon1t",
@@ -38,23 +38,17 @@
     "lgrandi": os.path.join(SCRATCH_DIR, "tmp"),
     "xenon1t": os.path.join(SCRATCH_DIR, "tmp"),
     "broadwl": os.path.join(SCRATCH_DIR, "tmp"),
     "kicp": os.path.join(SCRATCH_DIR, "tmp"),
     "caslake": os.path.join(SCRATCH_DIR, "tmp"),
     "build": os.path.join(SCRATCH_DIR, "tmp"),
 }
-SINGULARITY_DIR: Dict[str, str] = {
-    "dali": "/dali/lgrandi/xenonnt/singularity-images",
-    "lgrandi": "/project2/lgrandi/xenonnt/singularity-images",
-    "xenon1t": "/project2/lgrandi/xenonnt/singularity-images",
-    "broadwl": "/project2/lgrandi/xenonnt/singularity-images",
-    "kicp": "/project2/lgrandi/xenonnt/singularity-images",
-    "caslake": "/project2/lgrandi/xenonnt/singularity-images",
-    "build": "/project2/lgrandi/xenonnt/singularity-images",
-}
+
+SINGULARITY_DIR: str = "lgrandi/xenonnt/singularity-images"
+
 DEFAULT_BIND: List[str] = [
     "/project2/lgrandi/xenonnt/dali:/dali",
     "/project2",
     "/project",
     f"/scratch/midway2/{USER}",
     f"/scratch/midway3/{USER}",
 ]
@@ -64,15 +58,14 @@
     "/dali/lgrandi/grid_proxy/xenon_service_proxy:/project2/lgrandi/grid_proxy/xenon_service_proxy",
 ]
 
 class QOSNotFoundError(Exception):
     """
     Provided qos is not found in the qos list
     """
-    
 class FormatError(Exception):
     """
     Format of file is not correct
     """
 
 def _make_executable(path: str) -> None:
     """
@@ -178,15 +171,14 @@
             field (str): The name of the field to check.
             values (Dict[str, Any]): The values dictionary containing the bypass_validation list.
 
         Returns:
             bool: True if the field should be validated, False otherwise.
         """
         return field in values.get("bypass_validation", [])
-    
     # validate the bypass_validation so that it can be reached in values
     @validator("bypass_validation", pre=True, each_item=True)
     def check_bypass_validation(cls, v: list) -> list:
         return v
 
     @validator("bind", pre=True, each_item=True)
     def check_bind(cls, v: str, values: Dict[Any, Any]) -> str:
@@ -302,35 +294,40 @@
 
     @validator("container")
     def check_container_format(cls, v: str, values: Dict[Any, Any]) -> str:
         """
         Check if the container ends with .simg and if it exists.
 
         Args:
-            v (str): The container to check.
+            v (str): Full path of the container or the name of the container file.
             values (Dict[Any, Any]): The values of the model.
 
         Raises:
             ValueError: Container not ending with .simg
             FileNotFoundError: Container does not exist.
 
         Returns:
             str: The container to use.
         """
-        if cls._skip_validation("container", values):
+        if cls._skip_validation("container", values) or os.path.exists(v):
             return v
         if not v.endswith(".simg"):
             raise FormatError("Container must end with .simg")
-        # Check if the container exists
+        # Search for the container when the full path is not provided
         partition: str = values.get("partition", "xenon1t")
-        if not os.path.exists(os.path.join(SINGULARITY_DIR[partition], v)):
-            raise FileNotFoundError(
-                f"Singularity image {v} does not exist in {SINGULARITY_DIR[partition]}"
-            )
-        return v
+        if partition == "dali":
+            root_dir = ["/dali"]
+        else:
+            root_dir = ["/project2", "/project"]
+        for root in root_dir:
+            image_path = os.path.join(root, SINGULARITY_DIR, v)
+            print("searched in", image_path)
+            if os.path.exists(image_path):
+                return image_path
+        raise FileNotFoundError(f"Container {v} does not exist")
 
     @validator("sbatch_file")
     def check_sbatch_file(
         cls, v: Optional[str], values: Dict[Any, Any]
     ) -> Optional[str]:
         """
         Check if the sbatch_file is None.
@@ -366,27 +363,25 @@
                 suffix=".sh", dir=TMPDIR[self.partition]
             )
             _make_executable(exec_file)
             os.write(file_discriptor, bytes("#!/bin/bash\n" + self.jobstring, "utf-8"))
         bind_string = " ".join(
             [f"--bind {b}" for b in self.bind]  # pylint: disable=not-an-iterable
         )
-        image = os.path.join(SINGULARITY_DIR[self.partition], self.container)
-        if not os.path.exists(image):
-            raise FileNotFoundError(f"Singularity image {image} does not exist")
         # Warn user if CUTAX_LOCATION is unset due to INSTALL_CUTAX
         if os.environ.get("INSTALL_CUTAX") == "1":
             logger.warning(
                 "INSTALL_CUTAX is set to 1, ignoring CUTAX_LOCATION and unsetting it for the job."
             )
         new_job_string = (
+            f"echo running on $SLURMD_NODENAME\n"
             f"unset X509_CERT_DIR\n"
             f'if [ "$INSTALL_CUTAX" == "1" ]; then unset CUTAX_LOCATION; fi\n'
             f"module load singularity\n"
-            f"singularity exec {bind_string} {image} {exec_file}\n"
+            f"singularity exec {bind_string} {self.container} {exec_file}\n"
             f"exit_code=$?\n"
             f"rm {exec_file}\n"
             f"if [ $exit_code -ne 0 ]; then\n"
             f"    echo Python script failed with exit code $exit_code\n"
             f"    exit $exit_code\n"
             f"fi\n"
         )
@@ -558,7 +553,20 @@
 
     Returns:
         int: Number of jobs in the queue.
     """
     output: str = subprocess.check_output(["squeue", "-u", str(USER)]).decode("utf-8")
     lines = output.split("\n")
     return len([job for job in lines if string in job])
+
+
+def used_nodes() -> list[str]:
+    """
+    Get the list of nodes that are currently being used.
+
+    Returns:
+        List[str]: List of nodes that are currently being used.
+    """
+    output = subprocess.check_output(["squeue", "-o", "%R", "-u", str(USER)]).decode(
+        "utf-8"
+    )
+    return list(set(output.split("\n")[1:-1]))
```

### Comparing `utilix-0.8.3/utilix/config.py` & `utilix-0.8.4/utilix/config.py`

 * *Files identical despite different names*

### Comparing `utilix-0.8.3/utilix/io.py` & `utilix-0.8.4/utilix/io.py`

 * *Files identical despite different names*

### Comparing `utilix-0.8.3/utilix/mongo_files.py` & `utilix-0.8.4/utilix/mongo_files.py`

 * *Files identical despite different names*

### Comparing `utilix-0.8.3/utilix/rundb.py` & `utilix-0.8.4/utilix/rundb.py`

 * *Files identical despite different names*

### Comparing `utilix-0.8.3/utilix.egg-info/PKG-INFO` & `utilix-0.8.4/utilix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilix
-Version: 0.8.3
+Version: 0.8.4
 Summary: User-friendly interface to various utilities for XENON users
 Home-page: https://github.com/XENONnT/utilix
 License: UNKNOWN
 Description: # utilix
         [![PyPI version shields.io](https://img.shields.io/pypi/v/utilix.svg)](https://pypi.python.org/pypi/utilix/)
         
         ``utilix`` is a utility package for XENON software, mainly relating to analysis. It currently has two main features: (1) a general XENON configuration framework and (2) easy access to the runsDB by wrapping python calls to a RESTful API. Eventually, we would like to include easy functions for interacting with the Midway and OSG batch queues.
```

