# Comparing `tmp/cdbt-0.2.3.tar.gz` & `tmp/cdbt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdbt-0.2.3.tar", last modified: Tue May 21 04:49:55 2024, max compression
+gzip compressed data, was "cdbt-0.2.4.tar", last modified: Fri May 24 02:48:40 2024, max compression
```

## Comparing `cdbt-0.2.3.tar` & `cdbt-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-21 04:49:55.508609 cdbt-0.2.3/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      466 2024-05-21 04:49:55.508044 cdbt-0.2.3/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-17 13:41:23.000000 cdbt-0.2.3/README.md
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-21 04:49:55.500752 cdbt-0.2.3/cdbt/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.2.3/cdbt/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     6134 2024-05-21 02:30:10.000000 cdbt-0.2.3/cdbt/build_dbt_docs_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     7330 2024-05-17 13:41:23.000000 cdbt-0.2.3/cdbt/build_unit_test_data_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     6256 2024-05-21 03:23:30.000000 cdbt-0.2.3/cdbt/cmdline.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    19056 2024-05-21 04:19:11.000000 cdbt-0.2.3/cdbt/main.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    17490 2024-05-17 13:41:23.000000 cdbt-0.2.3/cdbt/prompts.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-21 04:49:55.507698 cdbt-0.2.3/cdbt.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      466 2024-05-21 04:49:55.000000 cdbt-0.2.3/cdbt.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      327 2024-05-21 04:49:55.000000 cdbt-0.2.3/cdbt.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-21 04:49:55.000000 cdbt-0.2.3/cdbt.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-21 04:49:55.000000 cdbt-0.2.3/cdbt.egg-info/entry_points.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       51 2024-05-21 04:49:55.000000 cdbt-0.2.3/cdbt.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-21 04:49:55.000000 cdbt-0.2.3/cdbt.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-21 04:49:55.508667 cdbt-0.2.3/setup.cfg
--rwxr-xr-x   0 craiglathrop   (501) staff       (20)      710 2024-05-21 04:49:44.000000 cdbt-0.2.3/setup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-21 04:49:55.507234 cdbt-0.2.3/tests/
--rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.2.3/tests/test_main.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:48:40.731193 cdbt-0.2.4/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 02:48:40.730385 cdbt-0.2.4/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-17 13:41:23.000000 cdbt-0.2.4/README.md
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:48:40.716118 cdbt-0.2.4/cdbt/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.2.4/cdbt/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4634 2024-05-24 02:44:30.000000 cdbt-0.2.4/cdbt/ai_core.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4591 2024-05-24 02:45:14.000000 cdbt-0.2.4/cdbt/build_dbt_docs_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4070 2024-05-24 02:39:54.000000 cdbt-0.2.4/cdbt/build_unit_test_data_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     6704 2024-05-23 17:30:10.000000 cdbt-0.2.4/cdbt/cmdline.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    19551 2024-05-24 02:39:54.000000 cdbt-0.2.4/cdbt/main.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    17569 2024-05-24 02:39:54.000000 cdbt-0.2.4/cdbt/prompts.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:48:40.729723 cdbt-0.2.4/cdbt.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 02:48:40.000000 cdbt-0.2.4/cdbt.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      343 2024-05-24 02:48:40.000000 cdbt-0.2.4/cdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-24 02:48:40.000000 cdbt-0.2.4/cdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-24 02:48:40.000000 cdbt-0.2.4/cdbt.egg-info/entry_points.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       72 2024-05-24 02:48:40.000000 cdbt-0.2.4/cdbt.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-24 02:48:40.000000 cdbt-0.2.4/cdbt.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-24 02:48:40.731327 cdbt-0.2.4/setup.cfg
+-rwxr-xr-x   0 craiglathrop   (501) staff       (20)      753 2024-05-24 02:48:37.000000 cdbt-0.2.4/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:48:40.728887 cdbt-0.2.4/tests/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.2.4/tests/test_main.py
```

### Comparing `cdbt-0.2.3/README.md` & `cdbt-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.3/cdbt/cmdline.py` & `cdbt-0.2.4/cdbt/cmdline.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,7 +140,16 @@
 @cdbt.command()
 @click.option('--select', '-s', type=str, help='Name of the model to build unit test data for.')
 @click.pass_context
 def build_unit(ctx, select):
     """Build unit test mock and expect data for a model."""
     build_unit_test_data = BuildUnitTestDataAI()
     build_unit_test_data.main(select)
+
+@cdbt.command()
+@click.option('--select', '-s', type=str, help='Name of the model to start a lightdash preview for. If not provided, all models will be previewed.')
+@click.option('--name', '-n', type=str, required=True, help='Name of the lightdash preview. Required.')
+@click.pass_context
+def lightdash(ctx, select, name):
+    """Start a lightdash preview for a model."""
+    preview_name = name
+    cdbt_class.lightdash(ctx, select, preview_name)
```

### Comparing `cdbt-0.2.3/cdbt/main.py` & `cdbt-0.2.4/cdbt/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -198,14 +198,28 @@
             '--threads', str(threads),
         ]
         if full_refresh:
             args.append('--full-refresh')
 
         self.execute_dbt_command_stream('build', args)
 
+    def lightdash(self, ctx, select, preview_name):
+        args = ['lightdash', 'start-preview', '--name', preview_name]
+        if select:
+            args = args + ['--select', select]
+
+        try:
+            subprocess.run(args, check=True)
+        except subprocess.CalledProcessError as e:
+            print(f'Failure while running command: {" ".join(e.cmd)}')
+            print(e.stderr)
+            print(e.stdout)
+            sys.exit(e.returncode)
+
+
     def execute_state_based_build(self, ctx: Context, artifact_dir: str, manifest_artifact_path: str,
                                   manifest_path: str, full_refresh: bool, threads: int, roll_back_manifest_flag: bool):
         if roll_back_manifest_flag and not self.test_mode:
             print(f'Making a backup of the current manifest.json at {manifest_path} to {manifest_artifact_path}')
             # Move the manifest from ./target to ./_artifacts. This becomes the prior state. Only used for local state
             # build. Not used for pdbuild (production build).
             shutil.move(manifest_path, manifest_artifact_path)
@@ -369,46 +383,47 @@
 
         dbt_command = ['dbt', command] + args
         print(f'Running command: {" ".join(dbt_command)}')
         if self.test_mode:
             self.dbt_test_mode_command_check_value = dbt_command
             return True
         else:
-            process = subprocess.Popen(
-                dbt_command,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-                text=True  # Ensure outputs are in text mode rather than bytes
-            )
-
-            # Real-time output streaming
-            while True:
-                output = process.stdout.readline()
-                if output == '' and process.poll() is not None:
-                    break
-                if output:
-                    print(output.rstrip())  # Print each line of the output
-                    self.dbt_execute_command_output += output.rstrip() + '\n'
-
-            # Capture and print any remaining output after the loop
-            stdout, stderr = process.communicate()
-            if stdout:
-                print(stdout.strip())
-
-            # Check exit code
-            if process.returncode != 0:
-                print(f"Command resulted in an error: {stderr}")
-                raise subprocess.CalledProcessError(returncode=process.returncode, cmd=dbt_command, output=stderr)
+            stderr, stdout = self.subprocess_stream(dbt_command)
 
             # Check for errors using a regex method if necessary
             if self.contains_errors(stdout + stderr):
                 return False
 
             return True
 
+    def subprocess_stream(self, args):
+        process = subprocess.Popen(
+            args,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            text=True  # Ensure outputs are in text mode rather than bytes
+        )
+        # Real-time output streaming
+        while True:
+            output = process.stdout.readline()
+            if output == '' and process.poll() is not None:
+                break
+            if output:
+                print(output.rstrip())  # Print each line of the output
+                self.dbt_execute_command_output += output.rstrip() + '\n'
+        # Capture and print any remaining output after the loop
+        stdout, stderr = process.communicate()
+        if stdout:
+            print(stdout.strip())
+        # Check exit code
+        if process.returncode != 0:
+            print(f"Command resulted in an error: {stderr}")
+            raise subprocess.CalledProcessError(returncode=process.returncode, cmd=args, output=stderr)
+        return stderr, stdout
+
     @staticmethod
     def extract_sql_code(log: str) -> str:
         """
         Extract the SQL code from the given log string.
 
         Parameters:
         log (str): The log string containing the header info and SQL code.
@@ -433,14 +448,16 @@
     @staticmethod
     def contains_errors(text):
         pattern = r"([2-9]|\d{2,})\s+errors?"
         error_flag = bool(re.search(pattern, text))
         return error_flag
 
 
+
+
 class DbtError(Exception):
     def __init__(self, message):
         self.message = 'DBT build failed with errors.'
 
     def __str__(self):
         return self.message
 
@@ -455,19 +472,18 @@
             'parents_children': False,
             'build_parent_count': None
         }
 
 
 if __name__ == '__main__':
     cdbt = ColdBoreCapitalDBT()
+    mock_ctx = MockCtx(Command('Duck'))
+    mock_ctx.obj['build_children'] = True
     # cdbt.build(full_refresh=False, select=None, fail_fast=False)
     # cdbt.trun(full_refresh=False, select=None, fail_fast=False)
     # cdbt.run(full_refresh=False, select=None, fail_fast=False)
     # cdbt.test(select=None, fail_fast=False)
     # cdbt.compile()
     # cdbt.sbuild(ctx=None, full_refresh=False)
     # cdbt.pbuild(ctx=MockCtx(Command('Duck')), full_refresh=False)
-
-    mock_ctx = MockCtx(Command('Duck'))
-    mock_ctx.obj['build_children'] = True
-    cdbt.gbuild(ctx=mock_ctx, full_refresh=False, threads=8)
+    # cdbt.gbuild(ctx=mock_ctx, full_refresh=False, threads=8)
     sys.exit(0)
```

### Comparing `cdbt-0.2.3/cdbt/prompts.py` & `cdbt-0.2.4/cdbt/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,16 @@
               type: average
               label: "Medical Appointment Count - Avg"
               description: "Average count of medical appointments."
               round: 0
               compact: thousands
               group_label: "Count"
 ```
-        
+
+This is a CSV data sample from the model:        
         """
 
     @property
     def dbt_docs_lte_l2_prompt(self):
         return """
         You will help build DBT documentation YML files for a given SQL query. Sometimes you will be asked to generate a description from scratch, other times you will be asked to fill in missing columns that exist in the model, but not in the documentation.
 
@@ -277,15 +278,15 @@
 
       - name: medical_revenue
         description: "Total revenue from medical services."
 
       - name: medical_appointment_count
         description: "Count of medical appointments."
 ```
-        
+This is a CSV data sample from the model:    
         """
 
     @property
     def build_unit_test_prompt(self):
 
         return """
 You will help build mockup input and expected output data for DBT unit tests using the EqualExperts/dbt_unit_testing package. The input and expect data will be in a CSV type format using | as a seperator between fields.
```

### Comparing `cdbt-0.2.3/setup.py` & `cdbt-0.2.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cdbt',
-    version='0.2.3',
+    version='0.2.4',
     description='A CLI tool to manage dbt builds with state handling and manifest management',
     author='Craig Lathrop',
     author_email='development@coldborecapital.com',
     packages=find_packages(),
     install_requires=[
         'click',
         'pyperclip',
-        'snowflake-connector-python[pandas]'
+        'snowflake-connector-python[pandas]',
+        'python-dotenv',
+        'openai'
     ],
     entry_points={
         'console_scripts': [
             'cdbt=cdbt.cmdline:cdbt',
         ],
     },
     classifiers=[
```

### Comparing `cdbt-0.2.3/tests/test_main.py` & `cdbt-0.2.4/tests/test_main.py`

 * *Files identical despite different names*

