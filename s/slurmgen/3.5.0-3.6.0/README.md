# Comparing `tmp/slurmgen-3.5.0.tar.gz` & `tmp/slurmgen-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurmgen-3.5.0.tar", last modified: Wed May 22 22:39:13 2024, max compression
+gzip compressed data, was "slurmgen-3.6.0.tar", last modified: Fri May 24 15:01:36 2024, max compression
```

## Comparing `slurmgen-3.5.0.tar` & `slurmgen-3.6.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-22 22:39:13.526689 slurmgen-3.5.0/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      278 2023-11-27 16:21:41.000000 slurmgen-3.5.0/.gitignore
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1303 2023-11-27 14:39:14.000000 slurmgen-3.5.0/LICENSE.txt
--rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-22 22:39:13.526689 slurmgen-3.5.0/PKG-INFO
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     2093 2024-03-30 02:44:17.000000 slurmgen-3.5.0/README.md
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-22 22:39:13.526689 slurmgen-3.5.0/example/
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-22 22:39:13.526689 slurmgen-3.5.0/example/data_output/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-05-22 22:37:06.000000 slurmgen-3.5.0/example/data_output/goodbye.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       55 2024-05-22 22:37:06.000000 slurmgen-3.5.0/example/data_output/hello.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      756 2024-05-22 21:53:10.000000 slurmgen-3.5.0/example/job_def.json
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-05-22 21:27:31.000000 slurmgen-3.5.0/example/job_tmpl.json
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1027 2023-11-27 20:00:16.000000 slurmgen-3.5.0/example/run_slurm.py
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-22 22:39:13.526689 slurmgen-3.5.0/example/slurm_output/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      756 2024-05-22 22:37:20.000000 slurmgen-3.5.0/example/slurm_output/test.log
--rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     1271 2024-05-22 22:37:20.000000 slurmgen-3.5.0/example/slurm_output/test.sh
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1566 2024-05-03 05:50:27.000000 slurmgen-3.5.0/pyproject.toml
--rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     1719 2023-11-27 16:21:41.000000 slurmgen-3.5.0/run_release.sh
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       38 2024-05-22 22:39:13.526689 slurmgen-3.5.0/setup.cfg
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-22 22:39:13.526689 slurmgen-3.5.0/slurmgen/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      176 2024-05-03 05:52:06.000000 slurmgen-3.5.0/slurmgen/__init__.py
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      265 2024-05-22 21:17:32.000000 slurmgen-3.5.0/slurmgen/error.py
--rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     8106 2024-05-22 21:53:34.000000 slurmgen-3.5.0/slurmgen/gen.py
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     2836 2024-05-22 21:17:59.000000 slurmgen-3.5.0/slurmgen/run.py
--rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     7880 2024-05-22 21:42:13.000000 slurmgen-3.5.0/slurmgen/script.py
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        5 2024-05-22 22:39:13.000000 slurmgen-3.5.0/slurmgen/version.txt
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-22 22:39:13.526689 slurmgen-3.5.0/slurmgen.egg-info/
--rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-22 22:39:13.000000 slurmgen-3.5.0/slurmgen.egg-info/PKG-INFO
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      521 2024-05-22 22:39:13.000000 slurmgen-3.5.0/slurmgen.egg-info/SOURCES.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        1 2024-05-22 22:39:13.000000 slurmgen-3.5.0/slurmgen.egg-info/dependency_links.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       45 2024-05-22 22:39:13.000000 slurmgen-3.5.0/slurmgen.egg-info/entry_points.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        9 2024-05-22 22:39:13.000000 slurmgen-3.5.0/slurmgen.egg-info/top_level.txt
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-24 15:01:36.063351 slurmgen-3.6.0/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      278 2023-11-27 16:21:41.000000 slurmgen-3.6.0/.gitignore
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1303 2023-11-27 14:39:14.000000 slurmgen-3.6.0/LICENSE.txt
+-rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-24 15:01:36.063351 slurmgen-3.6.0/PKG-INFO
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     2093 2024-03-30 02:44:17.000000 slurmgen-3.6.0/README.md
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-24 15:01:36.059351 slurmgen-3.6.0/example/
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-24 15:01:36.059351 slurmgen-3.6.0/example/data_output/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-05-24 14:52:38.000000 slurmgen-3.6.0/example/data_output/goodbye.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       55 2024-05-24 14:52:38.000000 slurmgen-3.6.0/example/data_output/hello.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      756 2024-05-22 21:53:10.000000 slurmgen-3.6.0/example/job_def.json
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-05-22 21:27:31.000000 slurmgen-3.6.0/example/job_tmpl.json
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1063 2024-05-24 14:52:38.000000 slurmgen-3.6.0/example/run_slurm.py
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-24 15:01:36.059351 slurmgen-3.6.0/example/slurm_output/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      782 2024-05-24 14:52:38.000000 slurmgen-3.6.0/example/slurm_output/test.log
+-rwxrw-r--   0 tguillod  (1000) tguillod  (1000)     1271 2024-05-24 14:52:38.000000 slurmgen-3.6.0/example/slurm_output/test.sh
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1566 2024-05-03 05:50:27.000000 slurmgen-3.6.0/pyproject.toml
+-rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     1719 2023-11-27 16:21:41.000000 slurmgen-3.6.0/run_release.sh
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       38 2024-05-24 15:01:36.063351 slurmgen-3.6.0/setup.cfg
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-24 15:01:36.063351 slurmgen-3.6.0/slurmgen/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      176 2024-05-24 14:43:56.000000 slurmgen-3.6.0/slurmgen/__init__.py
+-rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     7930 2024-05-24 14:52:38.000000 slurmgen-3.6.0/slurmgen/gen.py
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     3249 2024-05-24 14:52:38.000000 slurmgen-3.6.0/slurmgen/run.py
+-rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     7461 2024-05-24 14:52:38.000000 slurmgen-3.6.0/slurmgen/script.py
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        5 2024-05-24 15:01:35.000000 slurmgen-3.6.0/slurmgen/version.txt
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-24 15:01:36.063351 slurmgen-3.6.0/slurmgen.egg-info/
+-rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-24 15:01:36.000000 slurmgen-3.6.0/slurmgen.egg-info/PKG-INFO
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      503 2024-05-24 15:01:36.000000 slurmgen-3.6.0/slurmgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        1 2024-05-24 15:01:36.000000 slurmgen-3.6.0/slurmgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       45 2024-05-24 15:01:36.000000 slurmgen-3.6.0/slurmgen.egg-info/entry_points.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        9 2024-05-24 15:01:36.000000 slurmgen-3.6.0/slurmgen.egg-info/top_level.txt
```

### Comparing `slurmgen-3.5.0/LICENSE.txt` & `slurmgen-3.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slurmgen-3.5.0/PKG-INFO` & `slurmgen-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmgen
-Version: 3.5.0
+Version: 3.6.0
 Summary: SlurmGen - Simple Slurm Manager
 Author-email: Thomas Guillod <guillod@otvam.ch>
 Maintainer-email: Thomas Guillod <guillod@otvam.ch>
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/otvam/slurmgen
 Project-URL: Repository, https://github.com/otvam/slurmgen
 Project-URL: Releases, https://github.com/otvam/slurmgen/releases
```

### Comparing `slurmgen-3.5.0/README.md` & `slurmgen-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `slurmgen-3.5.0/example/job_def.json` & `slurmgen-3.6.0/example/job_def.json`

 * *Files identical despite different names*

### Comparing `slurmgen-3.5.0/example/run_slurm.py` & `slurmgen-3.6.0/example/run_slurm.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 
 if __name__ == "__main__":
     # parse arguments
     if len(sys.argv) == 3:
         FILENAME = sys.argv[1]
         ARGUMENT = sys.argv[2]
     else:
-        print("error: invalid arguments")
+        print("invalid arguments")
         sys.exit(1)
 
     # print the variable content
     print("enter script")
+    print("enter script", file=sys.stderr)
     print("    ARGUMENT = %s" % ARGUMENT)
     print("    VARWORLD = %s" % VARWORLD)
     print("exit script")
 
     # create file with the variable content
     with open(os.path.join("data_output", FILENAME + ".txt"), "w") as fid:
         fid.write("ARGUMENT = %s\n" % ARGUMENT)
```

### Comparing `slurmgen-3.5.0/example/slurm_output/test.log` & `slurmgen-3.6.0/example/slurm_output/test.log`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-================================== test - 05/22/24 21:55:45
+================================== test - 05/24/24 14:52:38
 ==================== PARAM
 JOB TAG      : test
 LOG FILE     : slurm_output/test.log
 SCRIPT FILE  : slurm_output/test.sh
 ==================== TIME
-DATE GEN     : 05/22/24 21:55:45
-DATE RUN     : 05/22/24 21:55:45
+DATE GEN     : 05/24/24 14:52:38
+DATE RUN     : 05/24/24 14:52:38
 ==================== SLURM
 JOB ID       : NOT SLURM
 JOB NAME     : NOT SLURM
 JOB NODE     : NOT SLURM
 ==================== ENV VAR
 ==================== RUN: version
 Python 3.10.12
 ==================== RUN: hello
 enter script
+enter script
     ARGUMENT = hello world!
     VARWORLD = Welcome to everyone
 exit script
 ==================== RUN: goodbye
 enter script
+enter script
     ARGUMENT = goodbye world!
     VARWORLD = Welcome to everyone
 exit script
-================================== test - 05/22/24 21:55:45
+================================== test - 05/24/24 14:52:38
```

### Comparing `slurmgen-3.5.0/example/slurm_output/test.sh` & `slurmgen-3.6.0/example/slurm_output/test.sh`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 echo "==================== PARAM"
 echo "JOB TAG      : test"
 echo "LOG FILE     : slurm_output/test.log"
 echo "SCRIPT FILE  : slurm_output/test.sh"
 
 echo "==================== TIME"
-echo "DATE GEN     : 05/22/24 21:55:45"
+echo "DATE GEN     : 05/24/24 14:52:38"
 echo "DATE RUN     : `date -u +"%D %H:%M:%S"`"
 
 echo "==================== SLURM"
 echo "JOB ID       : $SLURM_JOB_ID"
 echo "JOB NAME     : $SLURM_JOB_NAME"
 echo "JOB NODE     : $SLURM_JOB_NODELIST"
```

### Comparing `slurmgen-3.5.0/pyproject.toml` & `slurmgen-3.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slurmgen-3.5.0/run_release.sh` & `slurmgen-3.6.0/run_release.sh`

 * *Files identical despite different names*

### Comparing `slurmgen-3.5.0/slurmgen/gen.py` & `slurmgen-3.6.0/slurmgen/gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 __author__ = "Thomas Guillod"
 __copyright__ = "Thomas Guillod - Dartmouth College"
 __license__ = "BSD License"
 
 import os.path
 import shutil
 import datetime
-from slurmgen.error import SlurmGenError
+
+
+class GenError(Exception):
+    """
+    Exception during the script generation.
+    """
+
+    pass
 
 
 def _write_title(fid, tag):
     """
     Write simulation header.
 
     Parameters
@@ -46,19 +53,19 @@
         Path of the log file created by during the Slurm job.
     pragmas : dict
         Dictionary with the pragmas controlling the Slurm job.
     """
 
     # check pragmas
     if "job-name" in pragmas:
-        raise SlurmGenError("error: job name is already set by the script")
+        raise GenError("job name is already set by the script")
     if "output" in pragmas:
-        raise SlurmGenError("error: job log is already set by the script")
+        raise GenError("job log is already set by the script")
     if "error" in pragmas:
-        raise SlurmGenError("error: job log is already set by the script")
+        raise GenError("job log is already set by the script")
 
     fid.write('#!/bin/bash\n')
     fid.write('\n')
     fid.write('# ############### define Slurm commands\n')
     fid.write('#SBATCH --job-name="%s"\n' % tag)
     fid.write('#SBATCH --output="%s"\n' % filename_log)
     for tag, val in pragmas.items():
@@ -231,50 +238,46 @@
 
     # get filenames
     filename_script = os.path.join(folder_output, tag + ".sh")
     filename_log = os.path.join(folder_output, tag + ".log")
 
     # remove previous files (if selected)
     if overwrite:
-        print("info: remove existing files")
         try:
             os.remove(filename_script)
         except FileNotFoundError:
             pass
         try:
             os.remove(filename_log)
         except FileNotFoundError:
             pass
         try:
             os.makedirs(folder_output)
         except FileExistsError:
             pass
 
     # check that the output files are not existing
-    print("info: check files")
     if os.path.isfile(filename_script):
-        raise SlurmGenError("error: Slurm file already exists")
+        raise GenError("Slurm file already exists")
     if os.path.isfile(filename_log):
-        raise SlurmGenError("error: log file already exists")
+        raise GenError("log file already exists")
     if not os.path.isdir(folder_output):
-        raise SlurmGenError("error: output folder does not exist")
+        raise GenError("output folder does not exist")
 
     # remove folders
-    print("info: remove folders")
     for folder in folder_delete:
         try:
             shutil.rmtree(folder)
         except FileNotFoundError:
             pass
 
-    print("info: create folders")
+    # create folders
     for folder in folder_create:
         try:
             os.makedirs(folder)
         except FileExistsError:
             pass
 
     # create the script
-    print("info: generate Slurm file")
     _generate_file(tag, filename_script, filename_log, pragmas, envs, commands)
 
     return filename_script, filename_log
```

### Comparing `slurmgen-3.5.0/slurmgen/run.py` & `slurmgen-3.6.0/slurmgen/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,26 @@
 Module for running a Slurm script.
 """
 
 __author__ = "Thomas Guillod"
 __copyright__ = "Thomas Guillod - Dartmouth College"
 __license__ = "BSD License"
 
+import sys
 import stat
 import os.path
 import subprocess
-from slurmgen.error import SlurmGenError
+
+
+class RunError(Exception):
+    """
+    Exception during data loading and parsing.
+    """
+
+    pass
 
 
 def _run_cmd_raw(command, env):
     """
     Run a Slurm script.
 
     Parameters
@@ -22,26 +30,30 @@
         Command to be executed.
     env : dict
         Dictionary with the environment variables.
     """
 
     # run the command
     try:
-        process = subprocess.run(
+        # start process
+        process = subprocess.Popen(
             command,
             env=env,
+            stderr=subprocess.DEVNULL,
+            stdout=subprocess.DEVNULL,
         )
+
+        # wait return
+        process.wait()
     except OSError as ex:
-        raise SlurmGenError("error: command error: %s" % str(ex))
+        raise RunError("command error: %s" % str(ex))
 
     # check return code
-    if process.returncode == 0:
-        print("info: valid return code")
-    else:
-        raise SlurmGenError("error: invalid return code")
+    if process.returncode != 0:
+        raise RunError("invalid return code")
 
 
 def _run_cmd_log(command, filename_log, env):
     """
     Run a Slurm script.
 
     Parameters
@@ -52,29 +64,39 @@
         Path of the log file created by during the Slurm job.
     env : dict
         Dictionary with the environment variables.
     """
 
     # run the command
     try:
+        # start process
+        process = subprocess.Popen(
+            command,
+            env=env,
+            stderr=subprocess.STDOUT,
+            stdout=subprocess.PIPE,
+            text=True,
+            bufsize=1,
+        )
+
+        # display data
         with open(filename_log, "w") as fid:
-            process = subprocess.run(
-                command,
-                env=env,
-                stderr=fid,
-                stdout=fid,
-            )
+            for line in process.stdout:
+                print(line.rstrip(), file=sys.stdout)
+                fid.write(line)
+                fid.flush()
+
+        # wait return
+        process.wait()
     except OSError as ex:
-        raise SlurmGenError("error: command error: %s" % str(ex))
+        raise RunError("command error: %s" % str(ex))
 
     # check return code
-    if process.returncode == 0:
-        print("info: valid return code")
-    else:
-        raise SlurmGenError("error: invalid return code")
+    if process.returncode != 0:
+        raise RunError("invalid return code")
 
 
 def run_data(filename_script, filename_log, local, cluster):
     """
     Run a Slurm script.
 
     Parameters
@@ -89,31 +111,31 @@
         Run (or not) the job on the cluster.
     """
 
     # make the script executable
     st = os.stat(filename_script)
     os.chmod(filename_script, st.st_mode | stat.S_IEXEC)
 
+    # check for incompatible flag
+    if local and cluster:
+        raise RunError("invalid flag: local and cluster")
+
     # submit Slurm job
     if cluster:
-        print("info: run Slurm job")
-
         # find env
         env = os.environ.copy()
 
         # find command
         command = ["sbatch", filename_script]
 
         # run
         _run_cmd_raw(command, env)
 
     # run locally
     if local:
-        print("info: run Shell job")
-
         # find env
         env = os.environ.copy()
         env["SLURM_JOB_ID"] = "NOT SLURM"
         env["SLURM_JOB_NAME"] = "NOT SLURM"
         env["SLURM_JOB_NODELIST"] = "NOT SLURM"
 
         # find command
```

### Comparing `slurmgen-3.5.0/slurmgen/script.py` & `slurmgen-3.6.0/slurmgen/script.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,15 +14,22 @@
 import sys
 import json
 import string
 import argparse
 import traceback
 from slurmgen import gen
 from slurmgen import run
-from slurmgen.error import SlurmGenError
+
+
+class ScriptError(Exception):
+    """
+    Exception during the script execution.
+    """
+
+    pass
 
 
 def _get_parser():
     """
     Create a command line parser with a description.
 
     Returns
@@ -107,25 +114,25 @@
     # load the template from a file
     if tmpl_file is not None:
         # load the template file
         try:
             with open(tmpl_file, "r") as fid:
                 data_raw = fid.read()
         except OSError as ex:
-            raise SlurmGenError("error: template file not found: %s" % str(ex))
+            raise ScriptError("template file not found: %s" % str(ex))
 
         # parse the template data
         try:
             tmpl_tmp = json.loads(data_raw)
         except json.JSONDecodeError as ex:
-            raise SlurmGenError("error: template file is invalid: %s" % str(ex))
+            raise ScriptError("template file is invalid: %s" % str(ex))
 
         # check type
         if type(tmpl_tmp) is not dict:
-            raise SlurmGenError("error: template file should contain a dict")
+            raise ScriptError("template file should contain a dict")
 
         # merge the template data
         tmpl_data = {**tmpl_data, **tmpl_tmp}
 
     # load the template file
     if tmpl_str is not None:
         tmpl_tmp = {}
@@ -134,17 +141,17 @@
 
         # merge the template data
         tmpl_data = {**tmpl_data, **tmpl_tmp}
 
     # check template
     for tag, val in tmpl_data.items():
         if type(tag) != str:
-            raise SlurmGenError("error: template substitution should be strings")
+            raise ScriptError("template substitution should be strings")
         if type(val) != str:
-            raise SlurmGenError("error: template substitution should be strings")
+            raise ScriptError("template substitution should be strings")
 
     return tmpl_data
 
 
 def _get_def(def_file, tmpl_data):
     """
     Load the job definition file and run the template.
@@ -163,34 +170,28 @@
     """
 
     # load the JSON data
     try:
         with open(def_file, "r") as fid:
             data_raw = fid.read()
     except OSError as ex:
-        raise SlurmGenError("error: definition file not found: %s" % str(ex))
-
-    # show template content
-    if tmpl_data:
-        print("info: template content")
-        for tag, val in tmpl_data.items():
-            print("info: var: \"%s\" => \"%s\"" % (tag, val))
+        raise ScriptError("definition file not found: %s" % str(ex))
 
     # apply the template
     try:
         obj = string.Template(data_raw)
         def_data = obj.substitute(tmpl_data)
     except (ValueError, KeyError) as ex:
-        raise SlurmGenError("error: template parsing error: %s" % str(ex))
+        raise ScriptError("template parsing error: %s" % str(ex))
 
     # load the JSON data
     try:
         def_data = json.loads(def_data)
     except json.JSONDecodeError as ex:
-        raise SlurmGenError("error: definition file is invalid: %s" % str(ex))
+        raise ScriptError("definition file is invalid: %s" % str(ex))
 
     return def_data
 
 
 def run_args(def_file, tmpl_file=None, tmpl_str=None, local=False, cluster=False, directory=None):
     """
     Run the script with arguments.
@@ -271,23 +272,18 @@
             args.def_file,
             tmpl_file=args.tmpl_file,
             tmpl_str=args.tmpl_str,
             local=args.local,
             cluster=args.cluster,
             directory=args.directory,
         )
-    except SlurmGenError as ex:
-        print("error: ============== SlurmGen ==============", file=sys.stderr)
-        print(str(ex), file=sys.stderr)
-        print("error: ============== SlurmGen ==============", file=sys.stderr)
-        sys.exit(1)
     except Exception as ex:
-        print("error: ============== Unknown ==============", file=sys.stderr)
-        traceback.print_exception(ex, limit=0, chain=False)
-        print("error: ============== Unknown ==============", file=sys.stderr)
+        print("================================== invalid termination", file=sys.stderr)
+        traceback.print_exception(ex, limit=0, chain=False, file=sys.stderr)
+        print("================================== invalid termination", file=sys.stderr)
         sys.exit(1)
 
     # return
     sys.exit(0)
 
 
 if __name__ == "__main__":
```

### Comparing `slurmgen-3.5.0/slurmgen.egg-info/PKG-INFO` & `slurmgen-3.6.0/slurmgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmgen
-Version: 3.5.0
+Version: 3.6.0
 Summary: SlurmGen - Simple Slurm Manager
 Author-email: Thomas Guillod <guillod@otvam.ch>
 Maintainer-email: Thomas Guillod <guillod@otvam.ch>
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/otvam/slurmgen
 Project-URL: Repository, https://github.com/otvam/slurmgen
 Project-URL: Releases, https://github.com/otvam/slurmgen/releases
```

