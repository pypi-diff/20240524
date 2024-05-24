# Comparing `tmp/tum_esm_utils-2.0.2.tar.gz` & `tmp/tum_esm_utils-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_utils-2.0.2.tar", last modified: Sun Apr 14 18:12:41 2024, max compression
+gzip compressed data, was "tum_esm_utils-2.1.0.tar", last modified: Fri May 24 00:21:50 2024, max compression
```

## Comparing `tum_esm_utils-2.0.2.tar` & `tum_esm_utils-2.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    34888 2024-04-14 14:19:39.952724 tum_esm_utils-2.0.2/LICENSE
--rw-r--r--   0        0        0     1754 2024-04-14 16:07:45.718345 tum_esm_utils-2.0.2/README.md
--rw-r--r--   0        0        0     2211 2024-04-14 18:12:41.849801 tum_esm_utils-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      556 2024-04-14 14:19:39.955953 tum_esm_utils-2.0.2/tum_esm_utils/__init__.py
--rw-r--r--   0        0        0     2421 2024-04-14 14:19:39.956240 tum_esm_utils-2.0.2/tum_esm_utils/code.py
--rw-r--r--   0        0        0     3397 2024-04-14 15:59:57.269809 tum_esm_utils-2.0.2/tum_esm_utils/datastructures.py
--rw-r--r--   0        0        0     1437 2024-04-14 15:41:47.672621 tum_esm_utils-2.0.2/tum_esm_utils/decorators.py
--rw-r--r--   0        0        0     7328 2024-04-14 16:01:30.940351 tum_esm_utils-2.0.2/tum_esm_utils/em27.py
--rw-r--r--   0        0        0     5234 2024-04-14 16:02:35.509373 tum_esm_utils-2.0.2/tum_esm_utils/files.py
--rw-r--r--   0        0        0       64 2023-08-02 15:33:55.496271 tum_esm_utils-2.0.2/tum_esm_utils/ifg_parser/.gitignore
--rw-r--r--   0        0        0     2462 2023-08-02 15:33:55.496337 tum_esm_utils-2.0.2/tum_esm_utils/ifg_parser/glob_OPUSparms.F90
--rw-r--r--   0        0        0     2459 2023-08-02 15:33:55.496400 tum_esm_utils-2.0.2/tum_esm_utils/ifg_parser/glob_prepro4.F90
--rw-r--r--   0        0        0    28408 2023-08-02 15:33:55.496530 tum_esm_utils-2.0.2/tum_esm_utils/ifg_parser/ifg_parser.F90
--rw-r--r--   0        0        0      758 2023-08-02 15:33:55.496606 tum_esm_utils-2.0.2/tum_esm_utils/ifg_parser/ifg_parser.template.inp
--rw-r--r--   0        0        0   983040 2023-08-02 15:33:55.499240 tum_esm_utils-2.0.2/tum_esm_utils/ifg_parser/refspec.dat
--rw-r--r--   0        0        0   983040 2023-08-02 15:33:55.501952 tum_esm_utils-2.0.2/tum_esm_utils/ifg_parser/refspec2.dat
--rw-r--r--   0        0        0      381 2024-04-14 16:02:47.777922 tum_esm_utils-2.0.2/tum_esm_utils/mathematics.py
--rw-r--r--   0        0        0     4533 2024-04-14 16:03:35.124703 tum_esm_utils-2.0.2/tum_esm_utils/plotting.py
--rw-r--r--   0        0        0     3428 2024-04-14 15:46:07.935669 tum_esm_utils-2.0.2/tum_esm_utils/processes.py
--rw-r--r--   0        0        0        0 2023-08-02 15:33:55.502312 tum_esm_utils-2.0.2/tum_esm_utils/py.typed
--rw-r--r--   0        0        0     3779 2024-04-14 16:07:15.811102 tum_esm_utils-2.0.2/tum_esm_utils/shell.py
--rw-r--r--   0        0        0     1922 2024-04-14 16:04:30.167681 tum_esm_utils-2.0.2/tum_esm_utils/system.py
--rw-r--r--   0        0        0     2537 2024-04-14 16:05:45.880077 tum_esm_utils-2.0.2/tum_esm_utils/text.py
--rw-r--r--   0        0        0     5119 2024-04-14 16:06:55.042381 tum_esm_utils-2.0.2/tum_esm_utils/timing.py
--rw-r--r--   0        0        0     2171 2024-04-14 14:19:39.958359 tum_esm_utils-2.0.2/tum_esm_utils/validators.py
--rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 tum_esm_utils-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34888 2024-04-14 14:19:39.952724 tum_esm_utils-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1754 2024-04-14 16:07:45.718345 tum_esm_utils-2.1.0/README.md
+-rw-r--r--   0        0        0     2256 2024-05-24 00:21:50.821074 tum_esm_utils-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      711 2024-05-24 00:17:29.610338 tum_esm_utils-2.1.0/tum_esm_utils/__init__.py
+-rw-r--r--   0        0        0     2421 2024-04-14 14:19:39.956240 tum_esm_utils-2.1.0/tum_esm_utils/code.py
+-rw-r--r--   0        0        0     3397 2024-04-14 15:59:57.269809 tum_esm_utils-2.1.0/tum_esm_utils/datastructures.py
+-rw-r--r--   0        0        0     1437 2024-04-14 15:41:47.672621 tum_esm_utils-2.1.0/tum_esm_utils/decorators.py
+-rw-r--r--   0        0        0     8505 2024-05-24 00:17:29.610702 tum_esm_utils-2.1.0/tum_esm_utils/em27.py
+-rw-r--r--   0        0        0     5234 2024-04-14 16:02:35.509373 tum_esm_utils-2.1.0/tum_esm_utils/files.py
+-rw-r--r--   0        0        0      381 2024-04-14 16:02:47.777922 tum_esm_utils-2.1.0/tum_esm_utils/mathematics.py
+-rw-r--r--   0        0        0       87 2024-05-24 00:17:29.610879 tum_esm_utils-2.1.0/tum_esm_utils/opus_file_validator/.gitignore
+-rw-r--r--   0        0        0     2587 2024-05-24 00:17:29.611045 tum_esm_utils-2.1.0/tum_esm_utils/opus_file_validator/glob_OPUSparms6.F90
+-rw-r--r--   0        0        0     2738 2024-05-24 00:17:29.611216 tum_esm_utils-2.1.0/tum_esm_utils/opus_file_validator/glob_prepro6.F90
+-rw-r--r--   0        0        0    31718 2024-05-24 00:17:29.611421 tum_esm_utils-2.1.0/tum_esm_utils/opus_file_validator/opus_file_validator.F90
+-rw-r--r--   0        0        0     1219 2024-05-24 00:17:29.611603 tum_esm_utils-2.1.0/tum_esm_utils/opus_file_validator/opus_file_validator.template.inp
+-rw-r--r--   0        0        0   983040 2024-05-24 00:17:29.613788 tum_esm_utils-2.1.0/tum_esm_utils/opus_file_validator/refspec.dat
+-rw-r--r--   0        0        0   983040 2024-05-24 00:17:29.616042 tum_esm_utils-2.1.0/tum_esm_utils/opus_file_validator/refspec2.dat
+-rw-r--r--   0        0        0     4533 2024-04-14 16:03:35.124703 tum_esm_utils-2.1.0/tum_esm_utils/plotting.py
+-rw-r--r--   0        0        0     3428 2024-04-14 15:46:07.935669 tum_esm_utils-2.1.0/tum_esm_utils/processes.py
+-rw-r--r--   0        0        0        0 2023-08-02 15:33:55.502312 tum_esm_utils-2.1.0/tum_esm_utils/py.typed
+-rw-r--r--   0        0        0     3779 2024-04-14 16:07:15.811102 tum_esm_utils-2.1.0/tum_esm_utils/shell.py
+-rw-r--r--   0        0        0     1922 2024-04-14 16:04:30.167681 tum_esm_utils-2.1.0/tum_esm_utils/system.py
+-rw-r--r--   0        0        0     2537 2024-04-14 16:05:45.880077 tum_esm_utils-2.1.0/tum_esm_utils/text.py
+-rw-r--r--   0        0        0     5119 2024-04-14 16:06:55.042381 tum_esm_utils-2.1.0/tum_esm_utils/timing.py
+-rw-r--r--   0        0        0     2171 2024-04-14 14:19:39.958359 tum_esm_utils-2.1.0/tum_esm_utils/validators.py
+-rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 tum_esm_utils-2.1.0/PKG-INFO
```

### Comparing `tum_esm_utils-2.0.2/LICENSE` & `tum_esm_utils-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/README.md` & `tum_esm_utils-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/pyproject.toml` & `tum_esm_utils-2.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tum_esm_utils"
-version = "2.0.2"
+version = "2.1.0"
 description = "Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich"
 authors = [
     { name = "Moritz Makowski", email = "moritz.makowski@tum.de" },
 ]
 dependencies = [
     "filelock>=3.13.4",
     "requests>=2.31.0",
@@ -92,12 +92,12 @@
 
 [tool.pdm.build]
 includes = [
     "tum_esm_utils",
 ]
 excludes = [
     "tests",
-    "tum_esm_utils/ifg_parser/*.mod",
-    "tum_esm_utils/ifg_parser/*.lock",
-    "tum_esm_utils/ifg_parser/*.txt",
-    "tum_esm_utils/ifg_parser/ifg_parser",
+    "tum_esm_utils/opus_file_validator/*.mod",
+    "tum_esm_utils/opus_file_validator/*.lock",
+    "tum_esm_utils/opus_file_validator/*.txt",
+    "tum_esm_utils/opus_file_validator/opus_file_validator",
 ]
```

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/__init__.py` & `tum_esm_utils-2.1.0/tum_esm_utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,21 @@
     shell,
     system,
     text,
     timing,
     validators,
 )
 
+# ignore import errors from the following submodules
+# because they requires extras to be installed
+
+# requires extra "polars"
 try:
     from . import em27
 except ImportError:
     pass
 
+# requires extra "plotting"
 try:
     from . import plotting
 except ImportError:
     pass
```

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/code.py` & `tum_esm_utils-2.1.0/tum_esm_utils/code.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/datastructures.py` & `tum_esm_utils-2.1.0/tum_esm_utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/decorators.py` & `tum_esm_utils-2.1.0/tum_esm_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/em27.py` & `tum_esm_utils-2.1.0/tum_esm_utils/em27.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 """Functions for interacting with EM27 interferograms.
 
-Implements: `detect_corrupt_ifgs`, `load_proffast2_result`
+Implements: `detect_corrupt_opus_files`, `load_proffast2_result`.
 
 This requires you to install this utils library with the optional `polars` dependency:
 
 ```bash
 pip install "tum_esm_utils[polars]"
 # or
 pdm add "tum_esm_utils[polars]"
 ```"""
 
 from __future__ import annotations
 from typing import Any, Literal
-import time
 import os
-import re
 import subprocess
+from typing_extensions import deprecated
 import filelock
 import tum_esm_utils
 import polars as pl
 
 _PARSER_DIR = os.path.join(
-    os.path.dirname(os.path.abspath(__file__)), "ifg_parser"
+    os.path.dirname(os.path.abspath(__file__)), "opus_file_validator"
 )
 
 
 def _compile_fortran_code(
     silent: bool = True,
     fortran_compiler: Literal["gfortran", "gfortran-9"] = "gfortran",
     force_recompile: bool = False,
 ) -> None:
     if force_recompile or (
-        not os.path.isfile(os.path.join(_PARSER_DIR, "ifg_parser"))
+        not os.path.isfile(os.path.join(_PARSER_DIR, "opus_file_validator"))
     ):
         if not silent:
             print("compiling fortran code")
 
-        command = f"{fortran_compiler} -nocpp -O3 -o ./ifg_parser glob_prepro4.F90 glob_OPUSparms.F90 ifg_parser.F90"
+        command = (
+            f"{fortran_compiler} -nocpp -O3 -o ./opus_file_validator " +
+            f"glob_prepro6.F90 glob_OPUSparms6.F90 opus_file_validator.F90"
+        )
         p = subprocess.run(
             command,
             shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             cwd=_PARSER_DIR,
             env=os.environ.copy(),
@@ -50,29 +52,22 @@
             stderr = p.stderr.decode("utf-8", errors="replace").strip()
             raise Exception(
                 f"command '{command}' failed with exit code {p.returncode}, " +
                 f"stderr: {stderr}, stout:{stdout}",
             )
 
 
-def _write_input_file(random_id: str, ifgs: list[str]) -> None:
-    with open(f"{_PARSER_DIR}/ifg_parser.template.inp", "r") as f:
-        template_content = f.read()
-    with open(f"{_PARSER_DIR}/ifg_parser.inp.{random_id}", "w") as f:
-        f.write(template_content.replace("%IFG_LIST%", "\n".join(ifgs)))
-
-
-def detect_corrupt_ifgs(
+def detect_corrupt_opus_files(
     ifg_directory: str,
     silent: bool = True,
     fortran_compiler: Literal["gfortran", "gfortran-9"] = "gfortran",
     force_recompile: bool = False,
 ) -> dict[str, list[str]]:
     """Returns dict[filename, list[error_messages]] for all
-    corrupt interferograms in the given directory.
+    corrupt opus files in the given directory.
 
     It will compile the fortran code using a given compiler
     to perform this task. The fortran code is derived from
     the preprocess source code of Proffast 2
     (https://www.imk-asf.kit.edu/english/3225.php). We use
     it because the retrieval using Proffast 2 will fail if
     there are corrupt interferograms in the input.
@@ -83,99 +78,139 @@
         fortran_compiler:  The fortran compiler to use.
         force_recompile:   If set to True, the fortran code will be recompiled.
 
     Returns:
         A dictionary containing corrupt filenames as keys and a list of error
         messages as values."""
 
-    # compiling fortran code
+    # compiling the fortran code in a semaphore
     with filelock.FileLock(
-        os.path.join(_PARSER_DIR, "ifg_parser.compile.lock"),
+        os.path.join(_PARSER_DIR, "opus_file_validator.lock"),
         timeout=30,
     ):
-        # these sleeps are sadly necessary to eliminate race conditions between
-        # two parallel processes. I don't knwo why, but now it works. Don't spend
-        # more hours here.
-        time.sleep(1)
         _compile_fortran_code(
             silent=silent,
             fortran_compiler=fortran_compiler,
             force_recompile=force_recompile
         )
-        time.sleep(1)
 
-    # generate input file
-    ifgs = [f"{ifg_directory}/{x}" for x in os.listdir(ifg_directory)]
-    ifgs = list(sorted(list(filter(os.path.isfile, ifgs))))
+    # list directory files
+    filepaths = list(
+        sorted([
+            fp for fp in
+            [f"{ifg_directory}/{x}" for x in os.listdir(ifg_directory)]
+            if os.path.isfile(fp)
+        ])
+    )
+
+    # write input file for parser in a semaphore
+    with filelock.FileLock(f"{_PARSER_DIR}/opus_file_validator.lock"):
+        random_id = tum_esm_utils.text.get_random_string(
+            10,
+            forbidden=[
+                f.replace("opus_file_validator.inp.", "")
+                for f in os.listdir(_PARSER_DIR)
+                if f.startswith("opus_file_validator.inp.")
+            ],
+        )
+        input_file_path = f"{_PARSER_DIR}/opus_file_validator.inp.{random_id}"
 
-    # run the parser
-    results: dict[str, list[str]] = {}
-    stdout: str = ""
-    while True:
-        with filelock.FileLock(f"{_PARSER_DIR}/ifg_parser.inp.lock"):
-            random_id = tum_esm_utils.text.get_random_string(
-                10,
-                forbidden=[
-                    f.replace("ifg_parser.inp.", "")
-                    for f in os.listdir(_PARSER_DIR)
-                    if f.startswith("ifg_parser.inp.")
-                ],
+        with open(f"{_PARSER_DIR}/opus_file_validator.template.inp", "r") as f:
+            template_content = f.read()
+        with open(input_file_path, "w") as f:
+            f.write(
+                template_content.replace("%IFG_LIST%", "\n".join(filepaths))
             )
-            _write_input_file(random_id, ifgs)
-        process = subprocess.run(
-            ["./ifg_parser", f"ifg_parser.inp.{random_id}"],
-            cwd=_PARSER_DIR,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
+
+    # run the parser
+    process = subprocess.run(
+        ["./opus_file_validator", input_file_path],
+        cwd=_PARSER_DIR,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+    )
+    os.remove(input_file_path)
+    stdout = process.stdout.decode()
+    stderr = process.stderr.decode()
+
+    if not process.returncode == 0:
+        raise RuntimeError(
+            f"Opus File Parser failed with exit code {process.returncode}, " +
+            f"stderr: {stderr}, stdout: {stdout}",
         )
-        os.remove(f"{_PARSER_DIR}/ifg_parser.inp.{random_id}")
-        stdout = process.stdout.decode()
-        stderr = process.stderr.decode()
-        if process.returncode == 0:
-            break
-        else:
-            # find the filename that caused the error
-            failing_filenames = list(
-                filter(lambda f: f in ifgs, stderr.split("'"))
-            )
-            assert (
-                "At line 837 of file ifg_parser.F90" in stderr
-            ), f"Unknown error behavior: {stderr}"
-            assert len(
-                failing_filenames
-            ) == 1, "invalid filename not found in stderr"
-            failing_filepath = failing_filenames[0]
-
-            # remove the error-causing file from the ifg list and try again
-            ifgs.remove(failing_filepath)
-            failing_filename = failing_filepath.split("/")[-1]
-            results[failing_filename] = ["file not processable"]
-            if not silent:
-                print(f'error with file "{failing_filename}", running again')
 
+    # locate the block of verification results
+    if ((stdout.count("--- Start verifying file integrities ---") != 1) or
+        (stdout.count("--- Done verifying file integrities ---") != 1)):
+        raise Exception("This is a bug in the `tum_esm_utils` library")
+    verification_block = stdout.split(
+        "--- Start verifying file integrities ---"
+    )[1].split("--- Done verifying file integrities ---")[0].strip("\t\n ")
+
+    # parse the verification results
+    results: dict[str, list[str]] = {}
+    checked_files: set[str] = set(filepaths)
+    if "\n\n" in verification_block:
+        file_verification_blocks = verification_block.split("\n\n")
+        for block in file_verification_blocks:
+            lines = block.split("\n")
+            is_corrupt = len(lines) > 2
+            filepath = lines[0].split('"')[1]
+            if is_corrupt:
+                results[os.path.basename(filepath)] = lines[1 :-1]
+            checked_files.remove(filepath)
+
+    # every file not mentioned in the verification results failed during reading it
+    for filepath in checked_files:
+        results[os.path.basename(filepath)] = [
+            "File not even readible by the parser"
+        ]
+
+    # save the raw output for debugging purposes
     with open(os.path.join(_PARSER_DIR, "output.txt"), "w") as f:
         f.write(stdout)
 
-    file_parsing_block = stdout.split("Done!")[-1]
-    file_parsing_lines = file_parsing_block.split("Read OPUS parms:")[1 :]
+    return results
 
-    # get results from output stream
-    for line in file_parsing_lines:
-        filename = line[12 :].split("\n")[0].split("/")[-1].replace(")", "")
-        parser_output = line[12 :].replace("\n", " ")
-        parser_messages = re.findall(
-            'charfilter "[^"]+" is missing', parser_output
-        )
-        if len(parser_messages) > 0:
-            results[filename] = [
-                ("charfilter '" + x.split('"')[1] + "' is missing")
-                for x in parser_messages
-            ]
 
-    return results
+@deprecated(
+    "This will be removed in the next breaking release. Please use " +
+    "the identical function `detect_corrupt_opus_files` instead."
+)
+def detect_corrupt_ifgs(
+    ifg_directory: str,
+    silent: bool = True,
+    fortran_compiler: Literal["gfortran", "gfortran-9"] = "gfortran",
+    force_recompile: bool = False,
+) -> dict[str, list[str]]:
+    """Returns dict[filename, list[error_messages]] for all
+    corrupt opus files in the given directory.
+
+    It will compile the fortran code using a given compiler
+    to perform this task. The fortran code is derived from
+    the preprocess source code of Proffast 2
+    (https://www.imk-asf.kit.edu/english/3225.php). We use
+    it because the retrieval using Proffast 2 will fail if
+    there are corrupt interferograms in the input.
+    
+    Args:
+        ifg_directory:     The directory containing the interferograms.
+        silent:            If set to False, print additional information.
+        fortran_compiler:  The fortran compiler to use.
+        force_recompile:   If set to True, the fortran code will be recompiled.
+
+    Returns:
+        A dictionary containing corrupt filenames as keys and a list of error
+        messages as values."""
+    return detect_corrupt_opus_files(
+        ifg_directory=ifg_directory,
+        silent=silent,
+        fortran_compiler=fortran_compiler,
+        force_recompile=force_recompile,
+    )
 
 
 def load_proffast2_result(path: str) -> pl.DataFrame:
     """Loads the output of Proffast 2 into a polars DataFrame.
 
     Args:
         path: The path to the Proffast 2 output file.
```

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/files.py` & `tum_esm_utils-2.1.0/tum_esm_utils/files.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/ifg_parser/glob_OPUSparms.F90` & `tum_esm_utils-2.1.0/tum_esm_utils/opus_file_validator/glob_OPUSparms6.F90`

 * *Files 18% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 ! MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ! GNU General Public License for more details.
 !
 ! You should have received a copy of the GNU General Public License
 ! along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
-module glob_OPUSparms
+module glob_OPUSparms6
 
-use glob_prepro4,only : maxmeas,maxOPUSchar
+use glob_prepro6,only : maxmeas,maxOPUSchar
 
 implicit none
 
 !    ' RES - resolution
 !    ' HFW - high folding limit(should be sligtly less than 15798)
 !    ' LWN - laser wavenumber (should be near 15798)
 !    ' DAT - date
@@ -29,15 +29,16 @@
 !    ' NSS - number of scans (should be even and equal to GFW + GBW)
 !    ' GFW - number good fwd scans
 !    ' GBW - number of good backward scans
 !    ' AQM - acquisition mode (should be DD)
 !    ' HPF - high pass filter
 !    ' LPF - low pass filter
 !    ' TSC - scanner T
-!    ' SSM - sample spacing multiplicator (should be 2)  
+!    ' SSM - sample spacing multiplicator (should be 2)
+!    ' DUR - total duration of sample recording (sec)  
 
 type OPUS_parameters
     sequence
     character(len=maxOPUSchar) :: DAT ! date
     character(len=maxOPUSchar) :: TIM ! time
     character(len=maxOPUSchar) :: VEL ! scanner velocity ENUM!!
     character(len=maxOPUSchar) :: AQM ! acquisition mode (should be DD)
@@ -47,13 +48,14 @@
     integer :: GFW                    ! number good fwd scans
     integer :: GBW                    ! number of good backward scans
     integer :: SSM                    ! sample spacing multiplicator (should be 2)
     real(8) :: RES                    ! resolution
     real(8) :: HFL                    ! high folding limit(should be sligtly less than 15798)
     real(8) :: LWN                    ! laser wavenumber (should be near 15798)
     real(8) :: TSC                    ! scanner T
+    real(8) :: DUR                    ! total scan duration in sec
 end type
 
 type (OPUS_parameters) :: OPUS_parms(maxmeas)
 
-end module glob_OPUSparms
+end module glob_OPUSparms6
```

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/ifg_parser/glob_prepro4.F90` & `tum_esm_utils-2.1.0/tum_esm_utils/opus_file_validator/glob_prepro6.F90`

 * *Files 15% similar despite different names*

```diff
@@ -9,47 +9,46 @@
 ! but WITHOUT ANY WARRANTY; without even the implied warranty of
 ! MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ! GNU General Public License for more details.
 !
 ! You should have received a copy of the GNU General Public License
 ! along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-module glob_prepro4
+module glob_prepro6
 
 implicit none
 
-character(len=1),parameter::pathstr="/"         ! Windows or Linux
+character(len=1),parameter :: pathstr = "\"         ! Windows or Linux
 integer,parameter :: maxblock = 40
 integer,parameter :: maxblength = 50000
 integer,parameter :: nzf = 32 ! oversampling of sinc kernel on fft grid
 integer,parameter :: nconv = 400 ! conv range (-nconv...+nconv) for resampling on fft grid
 integer,parameter :: maxmeas = 100000
 integer,parameter :: maxOPUSchar = 64
 integer,parameter :: nsmooth = 400 ! iterations for DC correction of IFG
-integer,parameter :: lengthcharmeas = 300   ! supported name length of measured file (path + name)
+integer,parameter :: lengthcharmeas = 400 ! supported name length of measured file (path + name)
 integer,parameter :: minfilesize = 100000 ! if smaller, assume OPUS file is truncated
+integer,parameter :: nphaspts = 3000 ! number of pts required on short side of SS ifg
+integer,parameter :: nphasrim = 665 ! narrows window for analytical phase calculation
+integer,parameter :: nphas = 14 ! polynomial order for analytical phase fit
+integer,parameter :: maxT = 29 ! number of spectra for T-dependent transmission model (0 ... 56 C, in 2 deg steps)
 
 real(8),parameter :: pi = 3.141592653589793d0
 real(8),parameter :: gradtorad = pi / 180.0d0
 real(8),parameter :: radtograd = 180.0d0 / pi
 real(8),parameter :: nuelas = 15798.0d0
-real(8),parameter :: semiFOV = 2.36e-3 !0.5 * 0.6 mm / 127 mm
-
-real(8),parameter :: phasa1max = 1.0d-3!1.0d-4
-real(8),parameter :: phasa2max = 1.0d-7!1.0d-9
-real(8),parameter :: phasa3max = 1.0d-11!1.0d-13
+real(8),parameter :: semiFOVref = 2.36e-3 !0.5 * 0.6 mm / 127 mm (EM27/SUN value)
 
 real(8),parameter :: nuersstart = 4500.0d0
 real(8),parameter :: nuersstop = 14000.0d0
 real(8),parameter :: nuersstart2 = 3800.0d0
 real(8),parameter :: nuersstop2 = 5200.0d0
 
-logical :: obsfixdec,checkoutdec,quietrundec
+logical :: obsfixdec,checkoutdec,quietrundec,dualchandec,chanswapdec,anaphasdec
 character(len=300) :: infotext,diagoutpath,binoutpath
 character(len=30) :: obslocation
-integer :: mpowFFT,ifgradius,maxifg,maxspc,maxspcrs
-integer :: nmeas,nsinc,TCCONkind !nsinc: width of sinc kernel on oversampled fft grid -nsinc...+nsinc
-real(8) :: OPDmax
-real :: ILSapo,ILSapo2,ILSphas,ILSphas2,DCmin,DCvar,obsfixlatdeg,obsfixlondeg &
-  ,obsfixaltkm,toffseth_UT
+integer :: mpowFFT,ifgradius,maxifg,maxspc,maxspcrs,bandselect
+integer :: nmeas,nsinc !nsinc: width of sinc kernel on oversampled fft grid -nsinc...+nsinc
+real(8) :: OPDmax,semiFOV
+real :: obsfixlatdeg,obsfixlondeg,obsfixaltkm,ILSapo,ILSapo2,ILSphas,ILSphas2,DCmin,DCvar,toffseth_UT
 
-end module glob_prepro4
+end module glob_prepro6
```

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/ifg_parser/ifg_parser.F90` & `tum_esm_utils-2.1.0/tum_esm_utils/opus_file_validator/opus_file_validator.F90`

 * *Files 16% similar despite different names*

```diff
@@ -9,297 +9,260 @@
 ! but WITHOUT ANY WARRANTY; without even the implied warranty of
 ! MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ! GNU General Public License for more details.
 !
 ! You should have received a copy of the GNU General Public License
 ! along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-
 !====================================================================
 !
 ! This program is for the preprocessing of COCCON measurements.
 ! It performs quality checks, DC-correction, FFT and phase correction,
 ! and a resampling of the spectrum to a minimally sampled grid.
 !
 ! This code has been created by Frank Hase (frank.hase@kit.edu) and
 ! Darko Dubravica (darko.dubravica@kit.edu), both affiliated with KIT
 ! in the framework of ESA's COCCON-PROCEEDS project.
 !
 !====================================================================
 
-program ifg_parser
+program opus_file_validator
 
-use glob_prepro4
+use glob_prepro6
 
 implicit none
 
-logical :: dateidadec
-integer :: imeas,itest,iunit,iscan,narg,next_free_unit
-character(len=300) :: inputdatei,logdatei,logdatei_test
-character(len=10) :: idchar
-character(len=7) :: imeaschar
-character(len=4) :: argchar
+logical :: dateidadec,reftrmdec
+integer :: imeas
+character(len=300) :: inputdatei
 
 character(len=lengthcharmeas),dimension(:),allocatable :: measfile
-logical,dimension(:),allocatable :: dualifg
+integer(8),dimension(:),allocatable :: errflag,errflag_CO 
 integer,dimension(:),allocatable :: nptrfirstdir,nofblock,nifg &
-  ,errflag,errflag_CO,icbfwd,icbbwd,icbfwd2,icbbwd2
+  ,icbfwd,icbbwd,icbfwd2,icbbwd2
 integer,dimension(:,:),allocatable :: blocktype,blocklength,blockptr
 
 real(8),dimension(:),allocatable :: JDdate
 real,dimension(:),allocatable :: UTh,durationsec,astrelev,azimuth
 
 character(len=6),dimension(:),allocatable :: YYMMDDlocal,HHMMSSlocal,YYMMDDUT
 
-real,dimension(:),allocatable :: refspec,refspec2,sinc
+real,dimension(:,:),allocatable :: reftrmT
+real,dimension(:),allocatable :: refspec,refspec2,refphas,reftrm,sinc
 real,dimension(:),allocatable :: cbfwd,cbbwd,cbfwd2,cbbwd2
+real,dimension(:),allocatable :: obslatdeg,obslondeg,obsaltkm
 
-! arrays for processing loop
-real,dimension(:),allocatable :: ifgfwd,ifgbwd,ifgfwd2,ifgbwd2
-real,dimension(:),allocatable :: specfwd,specbwd,specfwd2,specbwd2
-real,dimension(:),allocatable :: specfwdrs,specbwdrs,specfwd2rs,specbwd2rs
-real,dimension(:),allocatable :: specmeanrs,specmean2rs
-complex,dimension(:),allocatable :: cspecfwd,cspecbwd,cspecfwd2,cspecbwd2
+logical :: file_is_intact
 
 !====================================================================
 !  read command argument
-!  check presence of optional tccon.inp File
 !  read input file
 !====================================================================
 call get_command_argument(1,inputdatei)
-
-inquire (file = 'tccon.inp',exist = dateidadec)
-if (dateidadec) then
-    print *,'Optional TCCON input file detected...'
-    iunit = next_free_unit()
-    open (iunit,file = 'tccon.inp',status = 'old',action = 'read')
-    call gonext(iunit,.false.)
-    read (iunit,*) TCCONkind
-    print *,'TCCONkind:',TCCONkind
-    close (iunit)
-else
-   print *,'No optional TCCON input file detected...'
-   TCCONkind = 0
-end if
-
 print *,'Reading input file...'
 call read_input(trim(inputdatei))
 print *,'Done!'
 print *,'Number of raw measurements to be processed:',nmeas
 
 if (nmeas .gt. maxmeas) then
     print *,'nmeas maxmeas: ',nmeas,maxmeas
-    call warnout ('Too many files for processing!',0)
+    call warnout ('Too many files for processing!')
 end if
 
 !====================================================================
-!  set ifg, spectral points and OPDmax according to choice of mpowFFT
+!  set ifg, spectral points and OPDmax according to input choice of mpowFFT
 !====================================================================
 select case (mpowFFT)
     case (17)
-        OPDmax = 1.8d0
-        ifgradius = 56873
-        maxspcrs = 56874            
-    case (18)
-        OPDmax = 3.0d0
+        OPDmax = 1.8d0 ! equivalent to Bruker Res 0.5 cm-1
+        ifgradius = 56873            
+    case (19)
+        OPDmax = 4.5d0
+        ifgradius = 142182
+    case (20)
+        OPDmax = 16.2d0
+        ifgradius = 511857
+    case (181)
+        mpowFFT = 18
+        OPDmax = 2.5d0 ! equivalent to Bruker Res 0.36 cm-1
+        ifgradius = 78990
+    case (182)
+        mpowFFT = 18
+        OPDmax = 3.0d0 ! equivalent to Bruker Res 0.3 cm-1
         ifgradius = 94788
-        maxspcrs = 94789
     case default
-        call warnout("Invalid choice of mpowFFT (allowed: 17 or 18)!",0)
+        call warnout("Invalid choice of mpowFFT (allowed: 17, 181/182, 19, 20)!")
 end select
+maxspcrs = ifgradius + 1
 maxifg = 2**mpowFFT
 maxspc = maxifg / 2 
 
 !====================================================================
 !  allocation of general arrays, init sinc, read reference spectrum (for nue cal check)
 !====================================================================
-allocate (dualifg(nmeas))
-allocate (measfile(nmeas),nptrfirstdir(nmeas),nofblock(nmeas) &
-  ,nifg(nmeas),errflag(nmeas),errflag_CO(nmeas))
+allocate (errflag(nmeas),errflag_CO(nmeas))
+allocate (measfile(nmeas),nptrfirstdir(nmeas),nofblock(nmeas),nifg(nmeas))
 allocate (icbfwd(nmeas),icbbwd(nmeas),icbfwd2(nmeas),icbbwd2(nmeas))
 allocate (cbfwd(nmeas),cbbwd(nmeas),cbfwd2(nmeas),cbbwd2(nmeas))
+allocate (obslatdeg(maxmeas),obslondeg(maxmeas),obsaltkm(maxmeas))
 allocate (blocktype(maxblock,nmeas),blocklength(maxblock,nmeas),blockptr(maxblock,nmeas))
 allocate (YYMMDDlocal(nmeas),HHMMSSlocal(nmeas),YYMMDDUT(nmeas))
 allocate (JDdate(nmeas),UTh(nmeas),durationsec(nmeas),astrelev(nmeas),azimuth(nmeas))
 nsinc = nzf * nconv
 allocate (sinc(-nsinc:nsinc))
-allocate (refspec(maxspc),refspec2(maxspc))
+allocate (refspec(maxspc),refspec2(maxspc),refphas(maxspc),reftrm(maxspc))
 
 call prepare_sinc(sinc)
 
 if (checkoutdec) then 
     call tofile_spec(trim(diagoutpath)//pathstr//'sinc.dat',2*nsinc+1,sinc(-nsinc:nsinc))
 end if
 
 call read_refspec('refspec.dat',maxspc,refspec)
 call read_refspec('refspec2.dat',maxspc,refspec2)
 
+inquire (file = 'refphase.inp',exist = dateidadec)
+if (dateidadec) then
+    print *,'Optional phase reference file detected...'
+    call read_refspec('refphase.inp',maxspc,refphas)
+else
+    refphas = 0.0
+end if
+
+inquire (file = 'reftrm.inp',exist = dateidadec)
+if (dateidadec) then
+    print *,'Optional trm reference file detected...'
+    allocate (reftrmT(maxT,maxspc))
+    reftrmdec = .true.
+    call read_reftrmT('reftrm.inp',maxT,maxspc,reftrmT)
+else
+    reftrmdec = .false.
+end if
+
 !====================================================================
 !  read file names
 !====================================================================
 print *,'Reading file names'
-call read_meas_files(trim(inputdatei),nmeas,measfile)
+call read_meas_files(trim(inputdatei),nmeas,measfile,obslatdeg,obslondeg,obsaltkm)
 print *,'Done!'
 
 !====================================================================
 !  read all OPUS file headers, ephemerid calculation
 !====================================================================
 errflag(1:nmeas) = 0
 errflag_CO(1:nmeas) = 0
 
+print *
+print '(A)', '--- Start verifying file integrities ---'
+print *
+
 do imeas = 1,nmeas
-    
-    print *, 'Read OPUS parms:', imeas, ' (', trim(measfile(imeas)), ')'
+    file_is_intact = .true.
+    print '(A)', 'Parsing file "' // trim(measfile(imeas)) // '"'
 
     ! read OPUS parms
-    call read_opus_hdr(measfile(imeas),nptrfirstdir(imeas),nofblock(imeas))
-    call read_opus_dir(measfile(imeas),nptrfirstdir(imeas),nofblock(imeas) &
-      ,blocktype(1:maxblock,imeas),blocklength(1:maxblock,imeas) &
-      ,blockptr(1:maxblock,imeas),dualifg(imeas),nifg(imeas))
-    call read_opus_parms(imeas,measfile(imeas),nofblock(imeas) &
-      ,blocktype(1:maxblock,imeas),blocklength(1:maxblock,imeas),blockptr(1:maxblock,imeas))
+    call read_opus_hdr( &
+        measfile(imeas), &
+        nptrfirstdir(imeas), &
+        nofblock(imeas), &
+        file_is_intact &
+    )
+    call read_opus_dir( &
+        measfile(imeas), &
+        nptrfirstdir(imeas), &
+        nofblock(imeas), &
+        blocktype(1:maxblock,imeas), &
+        blocklength(1:maxblock,imeas), &
+        blockptr(1:maxblock,imeas), &
+        nifg(imeas), &
+        file_is_intact &
+    )
+    call read_opus_parms( &
+        imeas, &
+        measfile(imeas), &
+        nofblock(imeas), &
+        blocktype(1:maxblock,imeas), &
+        blocklength(1:maxblock,imeas), &
+        blockptr(1:maxblock,imeas), &
+        file_is_intact &
+    )
 
     ! check formal consistency of file with COCCON / preprocessor demands
-    call checkOPUSparms(measfile(imeas),imeas)
+    call checkOPUSparms( &
+        imeas, &
+        file_is_intact &
+    )
+
+    if (file_is_intact) then
+        print '(A)', 'File is intact'
+    else
+        print '(A)', 'File is corrupted'
+    end if
+
+    print *
 
 end do
 
+print '(A)', '--- Done verifying file integrities ---'
+
 !====================================================================
 !  Deallocation of general arrays
 !====================================================================
-deallocate (refspec,refspec2)
+if (reftrmdec) deallocate (reftrmT)
+deallocate (refspec,refspec2,refphas,reftrm)
 deallocate (sinc)
 
 deallocate (JDdate,UTh,durationsec,astrelev,azimuth)
 deallocate (YYMMDDlocal,HHMMSSlocal,YYMMDDUT)
+deallocate (obslatdeg,obslondeg,obsaltkm)
 deallocate (cbfwd,cbbwd,cbfwd2,cbbwd2)
 deallocate (blocktype,blocklength,blockptr)
 deallocate (measfile,nptrfirstdir,nofblock,nifg)
-deallocate (errflag,errflag_CO,icbfwd,icbbwd,icbfwd2,icbbwd2)
-deallocate (dualifg)
+deallocate (icbfwd,icbbwd,icbfwd2,icbbwd2)
+deallocate (errflag,errflag_CO)
 
-end program ifg_parser
+end program opus_file_validator
 
 
 
 
 
 
 
 
 
 !====================================================================
 !  checkOPUSparms
 !====================================================================
-subroutine checkOPUSparms(measfile,imeas)
+subroutine checkOPUSparms(imeas,file_is_intact)
 
-use glob_prepro4, only : OPDmax
-use glob_OPUSparms
+use glob_prepro6, only : OPDmax
+use glob_OPUSparms6
 
 implicit none
 
-character(len=*),intent(in) :: measfile
 integer,intent(in) :: imeas
+logical,intent(inout) :: file_is_intact
 
-if (OPUS_parms(imeas)%RES .lt. 0.8999999d0 / OPDmax) then
-    print *,measfile
+if (OPUS_parms(imeas)%RES .gt. 0.90001d0 / OPDmax) then
     print *,'OPUS RES:',OPUS_parms(imeas)%RES
     print *,'Requested RES:',0.9d0 / OPDmax
-    call warnout ('RES too small!',0)
+    call warnout ('RES too small!')
+    file_is_intact = .false.
 end if
 
 if (modulo(OPUS_parms(imeas)%NSS,2) .gt. 0) then
-    print *,measfile
-    call warnout ('Uneven number of scans!',0)    
+    call warnout ('Uneven number of scans!') 
+    file_is_intact = .false.   
 end if
 
-if (scan(OPUS_parms(imeas)%AQM,"DD") .lt. 1) then
-    print *,measfile
-    call warnout ('IFG not double-sided!',0)
-end if
 
 end subroutine checkOPUSparms
 
 
-
-
-
-!====================================================================
-!  FFT
-!====================================================================
-subroutine FFT(ifg,spec)
-
-use glob_prepro4,only : mpowFFT,maxifg,maxspc,pi
-
-implicit none
-
-real,dimension(maxifg),intent(in) :: ifg
-complex,dimension(maxspc),intent(out) :: spec
-
-integer :: i,j,k,l,n1,n2
-real(8) :: angle,argument,xdum,ydum,c,s
-real(8),dimension(:),allocatable :: x,y
-
-allocate(x(maxifg),y(maxifg))
-
-do i = 1,maxifg
-    x(i) = real(ifg(i),8)
-end do
-y = 0.0d0
-
-n2 = maxifg
-do k = 1,mpowFFT
-    n1 = n2
-    n2 = n2 / 2
-    angle = 0.0d0
-    argument = 2.0d0 * pi / real(n1,8)
-    do j = 0,n2 - 1
-        c = cos(angle)
-        s = sin(angle)
-        do i = j,maxifg - 1,n1
-            l = i + n2
-            xdum = x(i+1) - x(l+1)
-            x(i+1) = x(i+1) + x(l+1)
-            ydum = y(i+1) - y(l+1)
-            y(i+1) = y(i+1) + y(l+1)
-            x(l+1) = xdum * c - ydum * s
-            y(l+1) = ydum * c + xdum * s
-        end do ! i loop
-        angle = real(j + 1,8) * argument
-    end do !j loop
-end do !k loop
-
-j = 0
-do i = 0,maxifg - 2
-    if (i .lt. j) then
-        xdum = x(j+1)
-        x(j+1) = x(i+1)
-        x(i+1) = xdum
-        ydum = y(j+1)
-        y(j+1) = y(i+1)
-        y(i+1) = ydum
-    end if
-    k = maxifg / 2
-    do while (k .lt. j + 1)
-        j = j - k
-        k = k / 2
-    end do
-    j = j + k
-end do ! i loop
-
-do i = 1,maxspc
-    spec(i) = cmplx(x(i),y(i))
-end do
-
-deallocate (x,y)
-
-end subroutine FFT
-
-
-
 !====================================================================
 !  gonext: Einlesen bis zum naechsten $ Zeichen
 !====================================================================
 subroutine gonext(ifile,bindec)
 
 implicit none
 
@@ -316,47 +279,14 @@
         read(ifile,'(A1)') nextchar
     end if
 end do
 
 end subroutine gonext
 
 
-
-!====================================================================
-!  mysinc
-!====================================================================
-real function mysinc(x)
-
-implicit none
-
-real,parameter :: spi = 3.141592654
-real,parameter :: spihalb = 1.570796327
-
-real,intent(in) :: x
-real :: xabs,xabsmod,xabsqu,xabsmodqu
-
-
-xabs = abs(x) + 1.0e-8
-xabsqu = xabs * xabs
-!xabsmod = mod(xabs,spi)
-
-mysinc = sin(xabs) / (xabs + 5.0e-8 * xabsqu * xabsqu)
-
-!if (xabsmod .ge. spihalb) xabsmod = spi - xabsmod
-!
-!xabsmodqu = xabsmod * xabsmod
-!xabsqu = xabs * xabs
-!mysinc = (xabsmod &
-!  * (1.0 + xabsmodqu * (-0.1666595 + xabsmodqu &
-!  * (0.008315 - xabsmodqu * 0.0001855)))) / (xabs + 2.0e-7 * xabsqu * xabsqu)
-
-end function mysinc
-
-
-
 !====================================================================
 !  next_free_unit
 !====================================================================
 integer function next_free_unit()
 
 implicit none
 
@@ -365,54 +295,53 @@
 
 iu_free = 9
 is_open = .true.
 
 do while (is_open .and. iu_free < 100)
     iu_free = iu_free+1
     inquire (unit=iu_free, opened=is_open, iostat=istatus)
-    if (istatus .ne. 0) call warnout ('Error in inquiry!',0)
+    if (istatus .ne. 0) call warnout ('Error in inquiry!')
 enddo
 
-if (iu_free >= 100) call warnout ('No free unit < 100 found!',0)
+if (iu_free >= 100) call warnout ('No free unit < 100 found!')
 
 next_free_unit = iu_free
 
 end function next_free_unit
 
 
 
 !====================================================================
 !  OPUS_eval_char
 !====================================================================
 subroutine OPUS_eval_char(blocklength,binchar,charfilter,charwert)
 
-use glob_prepro4,only : maxOPUSchar
+use glob_prepro6,only : maxOPUSchar
 
 implicit none
 
 integer,intent(in) :: blocklength
 character(len=blocklength),intent(in) :: binchar
 character(len=3),intent(in) :: charfilter
 character(len=maxOPUSchar),intent(out) :: charwert
 
 integer(2) :: ityp,ireserved
 integer :: ipos
 
 ipos = index(binchar,charfilter//achar(0))
 if (ipos .eq. 0) then
-    print *, 'charfilter "', charfilter, '" is missing'
-    !call warnout('charfilter not found!',0)
+    print '(A)', 'Charfilter "', charfilter, '" is missing'
 end if
 
 read(binchar(ipos+4:ipos+5),FMT='(A2)') ityp
 
 read(binchar(ipos+6:ipos+7),FMT='(A2)') ireserved
     
 if (ityp .ne. 2 .and. ityp .ne. 3) then
-    call warnout('Inconsistent parameter kind in OPUS file!',0)
+    call warnout('Inconsistent parameter kind in OPUS file!')
 end if
 
 charwert = '                                                  '
 read(binchar(ipos+8:ipos+8+2*ireserved-1),FMT='(A)') charwert(1:2*ireserved)
 
 end subroutine OPUS_eval_char
 
@@ -431,24 +360,23 @@
 integer,intent(out) :: iwert
 
 integer(2) :: ityp,ireserved
 integer :: ipos
 
 ipos = index(binchar,charfilter//achar(0))
 if (ipos .eq. 0) then
-    print *, 'charfilter "', charfilter, '" is missing'
-    !call warnout('charfilter not found!',0)
+    print '(A)', 'Charfilter "', charfilter, '" is missing'
 end if
 
 read(binchar(ipos+4:ipos+5),FMT='(A2)') ityp
 
 read(binchar(ipos+6:ipos+7),FMT='(A2)') ireserved
     
 if (ityp .ne. 0 .or. ireserved .ne. 2) then
-    call warnout('Inconsistent parameter kind in OPUS file!',0)
+    call warnout('Inconsistent parameter kind in OPUS file!')
 end if
 
 read(binchar(ipos+8:ipos+8+2*ireserved-1),FMT='(A4)') iwert
 
 end subroutine OPUS_eval_int
 
 
@@ -465,39 +393,37 @@
 real(8),intent(out) :: dblewert
 
 integer(2) :: ityp,ireserved
 integer :: ipos
 
 ipos = index(binchar,charfilter//achar(0))
 if (ipos .eq. 0) then
-    print *, 'charfilter "', charfilter, '" is missing'
-    !call warnout('charfilter not found!',0)
+    print '(A)', 'Charfilter "', charfilter, '" is missing'
 end if
 
 read(binchar(ipos+4:ipos+5),FMT='(A2)') ityp
 
 read(binchar(ipos+6:ipos+7),FMT='(A2)') ireserved
     
 if (ityp .ne. 1 .or. ireserved .ne. 4) then
-    call warnout('Inconsistent parameter kind in OPUS file!',0)
+    call warnout('Inconsistent parameter kind in OPUS file!')
 end if
 
 read(binchar(ipos+8:ipos+8+2*ireserved-1),FMT='(A8)') dblewert
 
 end subroutine OPUS_eval_dble
 
 
 
-
 !====================================================================
 !  prepare_sinc
 !====================================================================
 subroutine prepare_sinc(sinc)
 
-use glob_prepro4, only : nconv,nzf,nsinc,pi
+use glob_prepro6, only : nconv,nzf,nsinc,pi
 
 implicit none
 
 real,dimension(-nsinc:nsinc),intent(out) :: sinc
 
 integer :: i
 real(8) :: x,xapo,apowert
@@ -516,46 +442,46 @@
     sinc(-i) = sinc(i)
 end do
 
 end subroutine prepare_sinc
 
 
 
-
 !====================================================================
-!  read_input: Einlesen der Eingabedatei
+!  read_input
 !====================================================================
 subroutine read_input(inpdatei)
 
-use glob_prepro4
+use glob_prepro6
 
 implicit none
 
 character(len=*),intent(in) :: inpdatei
 
-character(len=300) :: zeile
+character(len = lengthcharmeas) :: zeile,dateiname
 logical :: marke,decfileda,decsize
-integer :: iunit,iowert,imeas,next_free_unit,nfilebytes
+integer :: iunit,iowert,imeas,next_free_unit,nfilebytes,iscan
 
 iunit = next_free_unit()
 open (iunit,file = trim(inpdatei),status = 'old',iostat = iowert)
 if (iowert .ne. 0) then
     print *,trim(inpdatei)
-    call warnout('Cannot open input file!',0)
+    call warnout('Cannot open input file!')
 end if
 
 call gonext(iunit,.false.)
 read(iunit,*) checkoutdec
 read(iunit,*) mpowFFT
 read(iunit,*) DCmin
 read(iunit,*) DCvar
 
 call gonext(iunit,.false.)
 read(iunit,*) ILSapo,ILSphas
 read(iunit,*) ILSapo2,ILSphas2
+read(iunit,*) semiFOV
 
 call gonext(iunit,.false.)
 read(iunit,*) obsfixdec
 read(iunit,*) obslocation
 read(iunit,*) toffseth_UT
 if (obsfixdec) then
     read(iunit,*) obsfixlatdeg,obsfixlondeg,obsfixaltkm
@@ -563,33 +489,47 @@
     continue
 end if
 
 call gonext(iunit,.false.)
 read(iunit,'(L)') quietrundec
 read(iunit,'(A)') diagoutpath
 read(iunit,'(A)') binoutpath
+read(iunit,'(L)') dualchandec
+read(iunit,'(L)') chanswapdec
+read(iunit,'(L)') anaphasdec
+read(iunit,'(I2)') bandselect
+
 if (diagoutpath .eq. 'standard') diagoutpath = 'diagnosis'
+if (chanswapdec .and. .not. dualchandec) call warnout('chanswap requires dualchandec')
+if (bandselect .eq. 1 .and. .not. dualchandec) call warnout('bandselect = 1 requires dualchandec')
 
 call gonext(iunit,.false.)
 read(iunit,'(A)') infotext
 
 call gonext(iunit,.false.)
 ! determine number of raw measurements to treat
 marke = .false.
 imeas = 0
 do while (.not. marke)
+    zeile = ''
     read(iunit,'(A)') zeile
     if (zeile(1:3) .eq. '***') then
         marke = .true.
     else        
-        ! test file existence and size here
-        inquire(file = zeile,exist = decfileda,size = nfilebytes)
+        ! test OPSUS file existence and size here
+        if (obsfixdec) then
+            dateiname = trim(zeile)
+        else
+            iscan = scan(zeile,',')
+            dateiname = zeile(1:iscan - 1)
+        end if
+        inquire(file = trim(dateiname),exist = decfileda,size = nfilebytes)
         if (.not. decfileda) then
-            print *,zeile
-            call warnout('spectrum file does not exist!',0)
+            print *,dateiname
+            call warnout('spectrum file does not exist!')
         end if
         if (nfilebytes .lt. minfilesize) then
             decsize = .false.
         else
             decsize = .true.
         end if
         if (decsize) imeas = imeas + 1
@@ -600,63 +540,81 @@
 nmeas = imeas
 
 end subroutine read_input
 
 
 
 !====================================================================
-!  read names of all files to be processed
+! read_meas_files
 !====================================================================
-subroutine read_meas_files(inpdatei,nmeas,measfile)
+subroutine read_meas_files(inpdatei,nmeas,measfile,obslatdeg,obslondeg,obsaltkm)
 
-use glob_prepro4, only : lengthcharmeas,minfilesize
+use glob_prepro6, only : obsfixdec,obsfixlatdeg,obsfixlondeg,obsfixaltkm,lengthcharmeas,minfilesize
 
 implicit none
 
 character(len=*),intent(in) :: inpdatei
 integer,intent(in) :: nmeas
 character(len=lengthcharmeas),dimension(nmeas),intent(out) :: measfile
+real,dimension(nmeas),intent(out) :: obslatdeg,obslondeg,obsaltkm
 
 logical :: marke,decfileda,decsize
-character(len=lengthcharmeas) :: zeile
-integer :: i,imeas,imeasall,iunit,iowert,next_free_unit,nfilebytes
+character(len=lengthcharmeas) :: zeile,dateiname
+integer :: i,imeas,iunit,iowert,next_free_unit,nfilebytes,iscan
+real :: latdeg,londeg,altkm
 
 iunit = next_free_unit()
 
 open (iunit,file = trim(inpdatei),status = 'old',iostat = iowert)
 if (iowert .ne. 0) then
     print *,trim(inpdatei)
-    call warnout('Cannot open input file!',0)
+    call warnout('Cannot open input file!')
 end if
 
 do i = 1,6
     call gonext(iunit,.false.)
 end do
 
 marke = .false.
 imeas = 0
 do while (.not. marke)
+    zeile = ''
     read(iunit,'(A)') zeile
+    if (zeile(1:3) .ne. '***') then
+        if (obsfixdec) then
+            dateiname = trim(zeile)
+            latdeg = obsfixlatdeg
+            londeg = obsfixlondeg
+            altkm = obsfixaltkm
+        else
+            iscan = scan(zeile,',')
+            dateiname = zeile(1:iscan - 1)
+            read(zeile(iscan+1:len(trim(zeile))),*) latdeg,londeg,altkm
+        end if
+    end if
     if (zeile(1:3) .eq. '***') then
         marke = .true.
     else        
         ! test file size here
-        inquire(file = zeile,exist = decfileda,size = nfilebytes)
+        inquire(file = trim(dateiname),exist = decfileda,size = nfilebytes)
         if (.not. decfileda) then
-            print *,zeile
-            call warnout('spectrum file does not exist!',0)
+            print *,dateiname
+            call warnout('spectrum file does not exist!')
         end if
         if (nfilebytes .lt. minfilesize) then
             decsize = .false.
         else
             decsize = .true.
         end if
         if (decsize) then
             imeas = imeas + 1
-            measfile(imeas) = trim(zeile)
+            obslatdeg(imeas) = latdeg
+            obslondeg(imeas) = londeg
+            obsaltkm(imeas) = altkm
+            measfile(imeas) = trim(dateiname)
             print *,trim(measfile(imeas))
         end if
     end if
 end do
 
 close (iunit)
 
@@ -664,29 +622,29 @@
 
 
 
 !====================================================================
 !  read_opus_dir
 !====================================================================
 subroutine read_opus_dir(measfile,nptrfirstdir,nofblock,blocktype &
-  ,blocklength,blockptr,dualifg,nifg)
+  ,blocklength,blockptr,nifg,file_is_intact)
 
-use glob_prepro4,only : maxblock,maxblength,maxifg
+use glob_prepro6,only : maxblock,maxblength,maxifg,dualchandec,ifgradius,nphaspts
 
 implicit none
 
 character(len=*),intent(in) :: measfile
 integer,intent(in) :: nptrfirstdir,nofblock
 integer,dimension(maxblock),intent(out) :: blocktype,blocklength,blockptr
-logical,intent(out) :: dualifg
 integer,intent(out) :: nifg
+logical,intent(inout) :: file_is_intact
 
 character(len=1) :: charbyte
-integer :: i,nifga,nifgb,iwert,magic,iunit,iowert,next_free_unit
-real(8) :: progver
+logical :: dualifg
+integer :: i,nifga,nifgb,iwert,iunit,iowert,next_free_unit
 
 iunit = next_free_unit()
 
 open (iunit,file = trim(measfile),form='unformatted',access ='stream',status = 'old',action = 'read',iostat = iowert)
 
 do i = 1,nptrfirstdir
     read(iunit) charbyte
@@ -712,72 +670,80 @@
     ! dual channel?
     if (blocktype(i) .eq. 34823) then
         dualifg = .true.
         nifgb = blocklength(i)
     end if
 end do
 
+if (dualifg .neqv. dualchandec) then
+    call warnout ('Inconsistent dualifg!') 
+    file_is_intact = .false.   
+end if
+
 if (nifga .eq. 0) then
-    print *,measfile
-    call warnout('Zero IFG block size!',0)
+    call warnout('Zero IFG block size!')
+    file_is_intact = .false.
 end if
 
-if (dualifg .and. nifga .ne. nifgb) then
-    print *,measfile
-    call warnout('Differing sizes of dual channel IFGs!',0)
+if (dualchandec .and. nifga .ne. nifgb) then
+    call warnout('Differing sizes of dual channel IFGs!')
+    file_is_intact = .false.
 else
     if (mod(nifga,8) .ne. 0) then
         print*, measfile
-        call warnout('Unexpected IFG size!',0)
+        call warnout('Unexpected IFG size!')
+        file_is_intact = .false.
     end if
     nifg = nifga / 8
 end if
 
-if (mod(nifg,2) .ne. 0) then
-    print *,measfile
-    call warnout('nifg not even!',0)
+if (nifg .gt. maxifg) then
+    call warnout('Note: nifg > maxifg')
+    file_is_intact = .false.
 end if
 
-if (nifg .gt. maxifg) then
-    print *,measfile
-    call warnout('IFG size too big!',0)
+if (nifg .lt. ifgradius + nphaspts + 1) then
+    call warnout('IFG size too small!')
+    file_is_intact = .false.
 end if
 
 end subroutine read_opus_dir
 
 
 
 !====================================================================
 !  read_opus_hdr
 !====================================================================
-subroutine read_opus_hdr(measfile,nptrfirstdir,nofblock)
+subroutine read_opus_hdr(measfile,nptrfirstdir,nofblock,file_is_intact)
 
-use glob_prepro4, only : maxblock
+use glob_prepro6, only : maxblock
 
 implicit none
 
 character(len=*),intent(in) :: measfile
 integer,intent(out) :: nptrfirstdir,nofblock
+logical,intent(inout) :: file_is_intact
 
-character(len=1) :: charbyte
-integer :: i,ntest,magic,iunit,iowert,next_free_unit
+integer :: ntest,magic,iunit,iowert,next_free_unit
 real(8) :: progver
 
 iunit = next_free_unit()
 
 open (iunit,file = trim(measfile),form='unformatted',access ='stream',status = 'old',action = 'read',iostat = iowert)
 if (iowert .ne. 0) then
     print *,trim(measfile)
-    call warnout('Cannot open measurement file!',0)
+    call warnout('Cannot open measurement file!')
+    file_is_intact = .false.
 end if
 
 read(iunit) magic
 if (magic .ne. -16905718) then
     print *,'measurement file:',trim(measfile)
-    call warnout('Not an OPUS file!',0)
+    call warnout('Not an OPUS file!')
+    file_is_intact = .false.
 end if
 
 read(iunit) progver
 !print *,progver
 
 read(iunit) nptrfirstdir
 !print *,nptrfirstdir
@@ -785,84 +751,90 @@
 read(iunit) ntest ! Angabe maxblock
 !print *,ntest
 
 read(iunit) nofblock
 !print *,nofblock
 if (nofblock .gt. maxblock) then
     print *,'measurement file:',trim(measfile)
-    call warnout('nofblock too big!',0)
+    call warnout('nofblock too big!')
+    file_is_intact = .false.
 end if
 
 close (iunit)
 
 end subroutine read_opus_hdr
 
 
 
 !====================================================================
-!  read OPUS parameters
-!              
+! read_opus_parms           
 !====================================================================
-subroutine read_opus_parms(imeas,measfile,nofblock,blocktype,blocklength,blockptr)
+subroutine read_opus_parms(imeas,measfile,nofblock,blocktype,blocklength,blockptr,file_is_intact)
 
-use glob_prepro4,only : maxblock,maxblength
-use glob_OPUSparms
+use glob_prepro6,only : maxblock,maxblength
+use glob_OPUSparms6
 
 implicit none
 
 character(len=*),intent(in) :: measfile
 integer,intent(in) :: imeas,nofblock
 integer,dimension(maxblock),intent(in) :: blocktype,blocklength,blockptr
+logical,intent(inout) :: file_is_intact
 
 integer :: i,iunit,iowert,next_free_unit
 character(len=maxblength) :: binchar
 
 ! read variables from blocktype 32: HFL,LWN,GFW,GBW,TSC,SSM
 do i = 1,nofblock
    if (blocktype(i) .eq. 32) exit
 end do
 
 iunit = next_free_unit()
 
 open (iunit,file = trim(measfile),form='unformatted',access ='stream',status = 'old',action = 'read',iostat = iowert)
 if (iowert .ne. 0) then
     print *,trim(measfile)
-    call warnout('Cannot open measurement file!',0)
+    call warnout('Cannot open measurement file!')
+    file_is_intact = .false.
 end if
 
 if (blocklength(i) .gt. maxblength) then
     print *,trim(measfile)
-    call warnout('Max blocklength exceeded!',0)
+    call warnout('Max blocklength exceeded!')
+    file_is_intact = .false.
 end if
 
 read(unit = iunit,pos = blockptr(i) + 1) binchar(1:blocklength(i))
 close (iunit)
 
 call OPUS_eval_int(blocklength(i),binchar,'GFW',OPUS_parms(imeas)%GFW)
 call OPUS_eval_int(blocklength(i),binchar,'GBW',OPUS_parms(imeas)%GBW)
 call OPUS_eval_dble(blocklength(i),binchar,'HFL',OPUS_parms(imeas)%HFL)
 call OPUS_eval_dble(blocklength(i),binchar,'LWN',OPUS_parms(imeas)%LWN)
 call OPUS_eval_dble(blocklength(i),binchar,'TSC',OPUS_parms(imeas)%TSC)
+call OPUS_eval_dble(blocklength(i),binchar,'DUR',OPUS_parms(imeas)%DUR)
 
 ! read variables from blocktype 48: NSS,AQM
 do i = 1,nofblock
    if (blocktype(i) .eq. 48) exit
 end do
 
 iunit = next_free_unit()
 
 open (iunit,file = trim(measfile),form='unformatted',access ='stream',status = 'old',action = 'read',iostat = iowert)
 if (iowert .ne. 0) then
     print *,trim(measfile)
-    call warnout('Cannot open measurement file!',0)
+    call warnout('Cannot open measurement file!')
+    file_is_intact = .false.
 end if
 
 if (blocklength(i) .gt. maxblength) then
     print *,trim(measfile)
-    call warnout('Max blocklength exceeded!',0)
+    call warnout('Max blocklength exceeded!')
+    file_is_intact = .false.
 end if
 
 read(unit = iunit,pos = blockptr(i) + 1) binchar(1:blocklength(i))
 close (iunit)
 
 !call OPUS_eval_char(blocklength,binchar,'VEL',OPUS_parms(imeas)%VEL)
 !print*,OPUS_parms(imeas)%VEL
@@ -877,20 +849,22 @@
 end do
 
 iunit = next_free_unit()
 
 open (iunit,file = trim(measfile),form='unformatted',access ='stream',status = 'old',action = 'read',iostat = iowert)
 if (iowert .ne. 0) then
     print *,trim(measfile)
-    call warnout('Cannot open measurement file!',0)
+    call warnout('Cannot open measurement file!')
+    file_is_intact = .false.
 end if
 
 if (blocklength(i) .gt. maxblength) then
     print *,trim(measfile)
-    call warnout('Max blocklength exceeded!',0)
+    call warnout('Max blocklength exceeded!')
+    file_is_intact = .false.
 end if
 
 read(unit = iunit,pos = blockptr(i) + 1) binchar(1:blocklength(i))
 close (iunit)
 
 call OPUS_eval_char(blocklength(i),binchar,'VEL',OPUS_parms(imeas)%VEL)
 call OPUS_eval_char(blocklength(i),binchar,'HPF',OPUS_parms(imeas)%HPF)
@@ -903,20 +877,22 @@
 end do
 
 iunit = next_free_unit()
 
 open (iunit,file = trim(measfile),form='unformatted',access ='stream',status = 'old',action = 'read',iostat = iowert)
 if (iowert .ne. 0) then
     print *,trim(measfile)
-    call warnout('Cannot open measurement file!',0)
+    call warnout('Cannot open measurement file!')
+    file_is_intact = .false.
 end if
 
 if (blocklength(i) .gt. maxblength) then
     print *,trim(measfile)
-    call warnout('Max blocklength exceeded!',0)
+    call warnout('Max blocklength exceeded!')
+    file_is_intact = .false.
 end if
 
 read(unit = iunit,pos = blockptr(i) + 1) binchar(1:blocklength(i))
 close (iunit)
 
 call OPUS_eval_char(blocklength(i),binchar,'DAT',OPUS_parms(imeas)%DAT)
 call OPUS_eval_char(blocklength(i),binchar,'TIM',OPUS_parms(imeas)%TIM)
@@ -932,47 +908,140 @@
 
 implicit none
 
 character(len=*),intent(in) :: refspecfile
 integer,intent(in) :: maxspc
 real,dimension(maxspc),intent(out) :: refspec
 
-integer :: i,icount,iunit,iowert,next_free_unit
+integer :: i,icount,ixpos,iunit,iowert,next_free_unit
 real :: wert
+real(8) :: a0,a1,a2,a3,a4,xpos,rest,gridratio
+real,dimension(:),allocatable :: wrkspec
 
 iunit = next_free_unit()
 ! check availability of file, number of file entries
 open (iunit,file = trim(refspecfile),status = 'old',iostat = iowert)
 if (iowert .ne. 0) then
     print *,trim(refspecfile)
-    call warnout('Cannot open refspec file!',0)
+    call warnout('Cannot open refspec file!')
 end if
 
 icount = 0
 do
     read(iunit,*,end = 102) wert
     icount = icount + 1
 end do
 102 continue
 close (iunit)
 
-if (icount .ne. maxspc) then
+if (icount .lt. maxspc) then
     print *,'maxspc:',maxspc
     print *,'icount:',icount
-    call warnout('Incompatible # of entries in refspec!',0)
+    call warnout('Incompatible # of entries in refspec!')
 end if
 
 iunit = next_free_unit()
 open (iunit,file = trim(refspecfile),status = 'old',iostat = iowert)
-do i = 1,icount
-    read(iunit,*) refspec(i)
+if (icount .gt. maxspc) then
+    allocate (wrkspec(icount))    
+    do i = 1,icount
+        read(iunit,*) wrkspec(i)
+    end do
+    close (iunit)
+    ! interpolation on output grid
+    gridratio = real(icount - 1,8) / real(maxspc - 1,8)
+    refspec(1) = wrkspec(1)
+    xpos = 1.0d0 + gridratio
+    ixpos = nint(xpos)
+    rest = xpos - real(ixpos,8)
+    a0 = wrkspec(ixpos)
+    a1 = 0.5d0 * (wrkspec(ixpos + 1) - wrkspec(ixpos - 1))
+    a2 = 0.125d0 * (wrkspec(ixpos-1) - 2.0d0 * wrkspec(ixpos) + wrkspec(ixpos+1))
+    refspec(2) = a0 + rest * (a1 + rest * a2)
+    do i = 3,maxspc - 2
+        xpos = 1.0d0 + gridratio * real(i - 1,8)
+        ixpos = nint(xpos)
+        rest = xpos - real(ixpos,8)
+        a0 = wrkspec(ixpos)
+        a1 = wrkspec(ixpos - 2) / 12.0d0 - 2.0d0 * wrkspec(ixpos - 1) &
+          / 3.0d0 + 2.0d0 * wrkspec(ixpos + 1) / 3.0d0 - wrkspec(ixpos + 2) / 12.0d0
+        a2 = - wrkspec(ixpos - 2) / 24.0d0 + 2.0d0 * wrkspec(ixpos - 1) / 3.0d0 - 5.0d0 * wrkspec(ixpos) / 4.0d0 &
+          + 2.0d0 * wrkspec(ixpos + 1) / 3.0d0 - wrkspec(ixpos + 2) / 24.0d0
+        a3 = - wrkspec(ixpos - 2) / 12.0d0 + wrkspec(ixpos - 1) / 6.0d0 - wrkspec(ixpos + 1) / 6.0d0 &
+          + wrkspec(ixpos + 2) / 12.0d0
+        a4 = wrkspec(ixpos - 2) / 24.0d0 - wrkspec(ixpos - 1) / 6.0d0 + 0.25d0 * wrkspec(ixpos) - wrkspec(ixpos + 1) &
+          / 6.0d0 + wrkspec(ixpos + 2) / 24.0d0
+        refspec(i) = a0 + rest * (a1 + rest * (a2 + rest * (a3 + rest * a4)))
+    end do
+    xpos = 1.0d0 + gridratio * real(maxspc - 2,8)
+    ixpos = nint(xpos)
+    rest = xpos - real(ixpos,8)
+    a0 = wrkspec(ixpos)
+    a1 = 0.5d0 * (wrkspec(ixpos + 1) - wrkspec(ixpos - 1))
+    a2 = 0.125d0 * (wrkspec(ixpos-1) - 2.0d0 * wrkspec(ixpos) + wrkspec(ixpos+1))
+    refspec(maxspc - 1) = a0 + rest * (a1 + rest * a2)
+    refspec(maxspc) = wrkspec(icount)
+    deallocate (wrkspec)
+else
+    do i = 1,icount
+        read(iunit,*) refspec(i)
+    end do
+    close (iunit)
+end if
+
+end subroutine read_refspec
+
+
+
+!====================================================================
+!  read_reftrmT
+!====================================================================
+subroutine read_reftrmT(refspecfile,maxT,maxspc,reftrmT)
+
+implicit none
+
+character(len=*),intent(in) :: refspecfile
+integer,intent(in) :: maxT,maxspc
+real,dimension(maxT,maxspc),intent(out) :: reftrmT
+
+character(len=376) :: zeile
+integer :: i,j,icount,iunit,iowert,next_free_unit
+
+iunit = next_free_unit()
+! check availability of file, number of file entries
+open (iunit,file = trim(refspecfile),status = 'old',iostat = iowert)
+
+if (iowert .ne. 0) then
+    print *,trim(refspecfile)
+    call warnout('Cannot open refspec file!')
+end if
+
+icount = 0
+do
+    read(iunit,'(A376)',end = 102) zeile
+    icount = icount + 1
 end do
+102 continue
 close (iunit)
 
-end subroutine read_refspec
+if (icount .ne. maxspc) then
+    print *,'maxspc:',maxspc
+    print *,'icount:',icount
+    call warnout('Incompatible # of entries in reftrmT!')
+end if
+
+iunit = next_free_unit()
+open (iunit,file = trim(refspecfile),status = 'old',iostat = iowert)  
+do i = 1,maxspc
+    read(iunit,'(A376)') zeile
+    read (zeile,'(E12.5,28(1X,E12.5))') (reftrmT(j,i),j = 1,maxT)
+end do
+close (iunit)
+
+end subroutine read_reftrmT
 
 
 
 !====================================================================
 !  tofile_spec
 !====================================================================
 subroutine tofile_spec(ausdatei,nspec,spec)
@@ -995,26 +1064,22 @@
 
 close (iunit)
 
 end subroutine tofile_spec
 
 
 
+
 !====================================================================
 !� Warnung rausschreiben und Programm evtl. beenden
 !====================================================================
-subroutine warnout(text,predec)
+subroutine warnout(text)
 
 use ISO_FORTRAN_ENV, only : ERROR_UNIT
-use glob_prepro4, only : quietrundec
 
 implicit none
 
 character(len=*),intent(in) :: text
-integer,intent(in) :: predec
-character(len=1) :: chardum
-integer :: intdec
 
-print *,'Warning:'
-print *, trim(text)
+print '(A)', trim(text)
 
 end subroutine warnout
```

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/ifg_parser/refspec.dat` & `tum_esm_utils-2.1.0/tum_esm_utils/opus_file_validator/refspec.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/ifg_parser/refspec2.dat` & `tum_esm_utils-2.1.0/tum_esm_utils/opus_file_validator/refspec2.dat`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/plotting.py` & `tum_esm_utils-2.1.0/tum_esm_utils/plotting.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/processes.py` & `tum_esm_utils-2.1.0/tum_esm_utils/processes.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/shell.py` & `tum_esm_utils-2.1.0/tum_esm_utils/shell.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/system.py` & `tum_esm_utils-2.1.0/tum_esm_utils/system.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/text.py` & `tum_esm_utils-2.1.0/tum_esm_utils/text.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/timing.py` & `tum_esm_utils-2.1.0/tum_esm_utils/timing.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/tum_esm_utils/validators.py` & `tum_esm_utils-2.1.0/tum_esm_utils/validators.py`

 * *Files identical despite different names*

### Comparing `tum_esm_utils-2.0.2/PKG-INFO` & `tum_esm_utils-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tum_esm_utils
-Version: 2.0.2
+Version: 2.1.0
 Summary: Python utilities by the Professorship of Environmental Sensing and Modeling at the Technical University of Munich
 Keywords: tum,utils,utilities,environmental,sensing,modeling,python,library,utilities,pydoc-markdown
 Author-Email: Moritz Makowski <moritz.makowski@tum.de>
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

