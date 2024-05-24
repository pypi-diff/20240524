# Comparing `tmp/viking-log-keeper-1.3.0.tar.gz` & `tmp/viking-log-keeper-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viking-log-keeper-1.3.0.tar", last modified: Thu May 23 22:21:34 2024, max compression
+gzip compressed data, was "viking-log-keeper-1.3.1.tar", last modified: Fri May 24 10:56:08 2024, max compression
```

## Comparing `viking-log-keeper-1.3.0.tar` & `viking-log-keeper-1.3.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:34.247119 viking-log-keeper-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-23 22:21:34.247119 viking-log-keeper-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:21:34.247119 viking-log-keeper-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:34.243119 viking-log-keeper-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:34.243119 viking-log-keeper-1.3.0/src/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/dashboard/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/dashboard/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/dashboard/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/dashboard/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:34.247119 viking-log-keeper-1.3.0/src/log_keeper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/log_keeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/log_keeper/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/log_keeper/ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/log_keeper/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/log_keeper/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/log_keeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:34.247119 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-23 22:21:34.000000 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-23 22:21:34.000000 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:21:34.000000 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-23 22:21:34.000000 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-23 22:21:34.000000 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 22:21:34.000000 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:56:08.291384 viking-log-keeper-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-24 10:56:08.291384 viking-log-keeper-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 10:56:08.291384 viking-log-keeper-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:56:08.287384 viking-log-keeper-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:56:08.287384 viking-log-keeper-1.3.1/src/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/src/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/src/dashboard/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/src/dashboard/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/src/dashboard/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/src/dashboard/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:56:08.287384 viking-log-keeper-1.3.1/src/log_keeper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/src/log_keeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/src/log_keeper/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/src/log_keeper/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/src/log_keeper/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/src/log_keeper/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-24 10:55:59.000000 viking-log-keeper-1.3.1/src/log_keeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:56:08.291384 viking-log-keeper-1.3.1/src/viking_log_keeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-24 10:56:08.000000 viking-log-keeper-1.3.1/src/viking_log_keeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-24 10:56:08.000000 viking-log-keeper-1.3.1/src/viking_log_keeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 10:56:08.000000 viking-log-keeper-1.3.1/src/viking_log_keeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-24 10:56:08.000000 viking-log-keeper-1.3.1/src/viking_log_keeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-24 10:56:08.000000 viking-log-keeper-1.3.1/src/viking_log_keeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 10:56:08.000000 viking-log-keeper-1.3.1/src/viking_log_keeper.egg-info/top_level.txt
```

### Comparing `viking-log-keeper-1.3.0/LICENSE` & `viking-log-keeper-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.0/PKG-INFO` & `viking-log-keeper-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viking-log-keeper
-Version: 1.3.0
+Version: 1.3.1
 Summary: 661 VGS - Function to collate 2965D log sheets into a master log, database, and dashboard.
 Home-page: https://github.com/mjennings061/viking-log-keeper
 Author: Michael Jennings
 Author-email: mjennings061@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `viking-log-keeper-1.3.0/README.md` & `viking-log-keeper-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.0/setup.py` & `viking-log-keeper-1.3.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 from setuptools.command.install import install
 from pathlib import Path
 
 # Configure logging
 logging.basicConfig(level=logging.DEBUG)
 
 
+def parse_requirements(filename):
+    """Parse the requirements file."""
+    req_path = Path(__file__).parent / filename
+    with open(req_path, 'r') as file:
+        return file.read().splitlines()
+
+
 class PostInstallCommand(install):
     """Install the package and run a post-installation script."""
     def run(self):
         """Run the post-installation script."""
         logging.info("Running post-installation script.")
         install.run(self)
         self.post_install()
@@ -50,15 +57,15 @@
         destination = desktop / BAT_FILE_NAME
         shutil.copyfile(source, destination)
         logging.info('%s has been copied to %s', BAT_FILE_NAME, str(desktop))
 
 
 setup(
     name="viking-log-keeper",
-    version="1.3.0",
+    version="1.3.1",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     url="https://github.com/mjennings061/viking-log-keeper",
     license="MIT",
     author="Michael Jennings",
     author_email="mjennings061@gmail.com",
     description="661 VGS - Function to collate 2965D log sheets into a"
@@ -71,26 +78,16 @@
         "Operating System :: OS Independent",
     ],
     cmdclass={
         'install': PostInstallCommand,
     },
     include_package_data=True,
     package_data={'': ['scripts/*.bat']},
-    install_requires=[
-        "extra-streamlit-components>=0.1.70",
-        "inquirer>=3.2.0",
-        "keyring>=24.3.0",
-        "matplotlib>=3.8.0",
-        "openpyxl>=3.1.0",
-        "pandas>=2.2.0",
-        "pymongo[srv]>=4.6.0",
-        "streamlit>=1.32.0",
-        "tqdm>=4.66.0",
-        "xlsxwriter>=3.2.0"
-    ],
+    data_files=[('', ['requirements.txt'])],
+    install_requires=parse_requirements('requirements.txt'),
     entry_points={
         "console_scripts": [
             "update-logs=log_keeper.main:main",
             "update-config=dashboard.auth:update_credentials_wrapper",
             "update-log-sheet-location=log_keeper.get_config:"
             "update_log_sheets_dir_wrapper",
             "viking-dashboard=dashboard.main:display_dashboard"
```

### Comparing `viking-log-keeper-1.3.0/src/dashboard/auth.py` & `viking-log-keeper-1.3.1/src/dashboard/auth.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.0/src/dashboard/main.py` & `viking-log-keeper-1.3.1/src/dashboard/main.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.0/src/dashboard/plots.py` & `viking-log-keeper-1.3.1/src/dashboard/plots.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.0/src/dashboard/utils.py` & `viking-log-keeper-1.3.1/src/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.0/src/log_keeper/get_config.py` & `viking-log-keeper-1.3.1/src/log_keeper/get_config.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.0/src/log_keeper/ingest.py` & `viking-log-keeper-1.3.1/src/log_keeper/ingest.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.0/src/log_keeper/main.py` & `viking-log-keeper-1.3.1/src/log_keeper/main.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.0/src/log_keeper/output.py` & `viking-log-keeper-1.3.1/src/log_keeper/output.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.0/src/log_keeper/utils.py` & `viking-log-keeper-1.3.1/src/log_keeper/utils.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/PKG-INFO` & `viking-log-keeper-1.3.1/src/viking_log_keeper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viking-log-keeper
-Version: 1.3.0
+Version: 1.3.1
 Summary: 661 VGS - Function to collate 2965D log sheets into a master log, database, and dashboard.
 Home-page: https://github.com/mjennings061/viking-log-keeper
 Author: Michael Jennings
 Author-email: mjennings061@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

