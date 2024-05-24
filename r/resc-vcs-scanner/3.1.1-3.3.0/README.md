# Comparing `tmp/resc_vcs_scanner-3.1.1.tar.gz` & `tmp/resc_vcs_scanner-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_vcs_scanner-3.1.1.tar", last modified: Wed May 22 10:08:21 2024, max compression
+gzip compressed data, was "resc_vcs_scanner-3.3.0.tar", last modified: Fri May 24 16:05:25 2024, max compression
```

## Comparing `resc_vcs_scanner-3.1.1.tar` & `resc_vcs_scanner-3.3.0.tar`

### file list

```diff
@@ -1,42 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.985753 resc_vcs_scanner-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-22 10:08:21.985753 resc_vcs_scanner-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-22 10:08:21.985753 resc_vcs_scanner-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.977753 resc_vcs_scanner-3.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.985753 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 10:08:21.000000 resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.981753 resc_vcs_scanner-3.1.1/src/vcs_scanner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.981753 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/env_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/finding_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/finding_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/ignore_list_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/resc_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.985753 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/celery_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/git_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/secret_scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:08:21.985753 resc_vcs_scanner-3.1.1/src/vcs_scanner/static/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-22 10:08:17.000000 resc_vcs_scanner-3.1.1/src/vcs_scanner/static/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:25.096680 resc_vcs_scanner-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-24 16:05:25.096680 resc_vcs_scanner-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-24 16:05:25.096680 resc_vcs_scanner-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:25.088680 resc_vcs_scanner-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:25.096680 resc_vcs_scanner-3.3.0/src/resc_vcs_scanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-24 16:05:25.000000 resc_vcs_scanner-3.3.0/src/resc_vcs_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-24 16:05:25.000000 resc_vcs_scanner-3.3.0/src/resc_vcs_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:05:25.000000 resc_vcs_scanner-3.3.0/src/resc_vcs_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-24 16:05:25.000000 resc_vcs_scanner-3.3.0/src/resc_vcs_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:05:25.000000 resc_vcs_scanner-3.3.0/src/resc_vcs_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-24 16:05:25.000000 resc_vcs_scanner-3.3.0/src/resc_vcs_scanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 16:05:25.000000 resc_vcs_scanner-3.3.0/src/resc_vcs_scanner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:25.092680 resc_vcs_scanner-3.3.0/src/vcs_scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:25.092680 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/env_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/finding_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/finding_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/gitleaks_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:25.092680 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/providers/ignore_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/providers/rule_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/providers/rule_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/providers/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:25.096680 resc_vcs_scanner-3.3.0/src/vcs_scanner/output_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/output_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/output_modules/output_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/output_modules/rws_api_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/output_modules/stdout_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/resc_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:25.096680 resc_vcs_scanner-3.3.0/src/vcs_scanner/secret_scanners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/secret_scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/secret_scanners/celery_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/secret_scanners/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/secret_scanners/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/secret_scanners/git_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/secret_scanners/secret_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:05:25.096680 resc_vcs_scanner-3.3.0/src/vcs_scanner/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-24 16:05:18.000000 resc_vcs_scanner-3.3.0/src/vcs_scanner/static/logging.ini
```

### Comparing `resc_vcs_scanner-3.1.1/LICENSE.md` & `resc_vcs_scanner-3.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.1/PKG-INFO` & `resc_vcs_scanner-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scanner
-Version: 3.1.1
+Version: 3.3.0
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: celery==5.3.1
 Requires-Dist: amqp==5.1.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: typing==3.7.4.3
 Requires-Dist: pydantic==1.10.15
 Requires-Dist: GitPython==3.1.41
-Requires-Dist: resc-backend>=3.1.1
+Requires-Dist: resc-backend>=3.2.2
 Requires-Dist: tenacity==8.2.2
 Requires-Dist: prettytable==3.8.0
 Requires-Dist: termcolor==2.3.0
 Requires-Dist: tomlkit==0.12.1
 
 # Repository Scanner Version Control System Scanner (RESC-VCS-SCANNER)
 [![Python][python-shield]][python-url]
```

### Comparing `resc_vcs_scanner-3.1.1/README.md` & `resc_vcs_scanner-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.1/setup.cfg` & `resc_vcs_scanner-3.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_vcs_scanner
 description = Repository Scanner - Version Control System - Scanner
-version = 3.1.1
+version = 3.3.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE.md
```

### Comparing `resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/PKG-INFO` & `resc_vcs_scanner-3.3.0/src/resc_vcs_scanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scanner
-Version: 3.1.1
+Version: 3.3.0
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: celery==5.3.1
 Requires-Dist: amqp==5.1.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: typing==3.7.4.3
 Requires-Dist: pydantic==1.10.15
 Requires-Dist: GitPython==3.1.41
-Requires-Dist: resc-backend>=3.1.1
+Requires-Dist: resc-backend>=3.2.2
 Requires-Dist: tenacity==8.2.2
 Requires-Dist: prettytable==3.8.0
 Requires-Dist: termcolor==2.3.0
 Requires-Dist: tomlkit==0.12.1
 
 # Repository Scanner Version Control System Scanner (RESC-VCS-SCANNER)
 [![Python][python-shield]][python-url]
```

### Comparing `resc_vcs_scanner-3.1.1/src/resc_vcs_scanner.egg-info/SOURCES.txt` & `resc_vcs_scanner-3.3.0/src/resc_vcs_scanner.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,24 @@
 src/vcs_scanner/resc_worker.py
 src/vcs_scanner/helpers/__init__.py
 src/vcs_scanner/helpers/cli.py
 src/vcs_scanner/helpers/env_default.py
 src/vcs_scanner/helpers/environment_wrapper.py
 src/vcs_scanner/helpers/finding_action.py
 src/vcs_scanner/helpers/finding_filter.py
-src/vcs_scanner/helpers/ignore_list_provider.py
+src/vcs_scanner/helpers/gitleaks_types.py
+src/vcs_scanner/helpers/providers/__init__.py
+src/vcs_scanner/helpers/providers/ignore_list.py
+src/vcs_scanner/helpers/providers/rule_comment.py
+src/vcs_scanner/helpers/providers/rule_file.py
+src/vcs_scanner/helpers/providers/rule_tag.py
+src/vcs_scanner/output_modules/__init__.py
+src/vcs_scanner/output_modules/output_module.py
+src/vcs_scanner/output_modules/rws_api_writer.py
+src/vcs_scanner/output_modules/stdout_writer.py
 src/vcs_scanner/secret_scanners/__init__.py
 src/vcs_scanner/secret_scanners/celery_worker.py
 src/vcs_scanner/secret_scanners/cli.py
 src/vcs_scanner/secret_scanners/configuration.py
 src/vcs_scanner/secret_scanners/git_operation.py
 src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
 src/vcs_scanner/secret_scanners/secret_scanner.py
```

### Comparing `resc_vcs_scanner-3.1.1/src/vcs_scanner/common.py` & `resc_vcs_scanner-3.3.0/src/vcs_scanner/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,9 +94,9 @@
         vcs_instance.name: vcs_instance for vcs_instance in vcs_instances_list
     }
     return vcs_instances_map
 
 
 def get_rule_pack_version_from_file(file_content: str) -> str | None:
     toml_rule_dictionary = tomlkit.loads(file_content)
-    rule_pack_version = toml_rule_dictionary["version"] if "version" in toml_rule_dictionary else None
+    rule_pack_version = toml_rule_dictionary.get("version", None)
     return rule_pack_version
```

### Comparing `resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/cli.py` & `resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/env_default.py` & `resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/env_default.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/environment_wrapper.py` & `resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.1/src/vcs_scanner/helpers/ignore_list_provider.py` & `resc_vcs_scanner-3.3.0/src/vcs_scanner/helpers/providers/ignore_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 # Third Party
 
 logger = logging.getLogger(__name__)
 
 
 class IgnoredListProvider:  # pylint: disable=R0902
-    def __init__(self, ignore_findings_path: str):
-        self.ignore_findings_path: str = ignore_findings_path
+    def __init__(self, ignore_findings_path: str | None):
+        self.ignore_findings_path: str | None = ignore_findings_path
         self.today: datetime = datetime.now(UTC)
 
     def get_ignore_list(self) -> dict[str, True]:
         """
         Get the dictionary of ignored findings according to the file
         The output will contain a dictionary with the path|rule|line as key and True as value.
         We use a dictionary for random access instead of list.
```

### Comparing `resc_vcs_scanner-3.1.1/src/vcs_scanner/input_parser.py` & `resc_vcs_scanner-3.3.0/src/vcs_scanner/input_parser.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.1/src/vcs_scanner/model.py` & `resc_vcs_scanner-3.3.0/src/vcs_scanner/model.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/celery_worker.py` & `resc_vcs_scanner-3.3.0/src/vcs_scanner/secret_scanners/celery_worker.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 # Standard Library
 import json
 import os
 
 # Third Party
 from celery import Celery
 from celery.utils.log import get_task_logger
-from resc_backend.constants import TEMP_RULE_FILE
+from resc_backend.constants import TEMP_RULE_FILE, TEMP_RULE_DIR_FILE, TEMP_RULE_REPO_FILE
 from resc_backend.resc_web_service.schema.repository import Repository
 
 # First Party
 from vcs_scanner.common import initialise_logs, load_vcs_instances
 from vcs_scanner.constants import LOG_FILE_PATH
 from vcs_scanner.helpers.environment_wrapper import validate_environment
 from vcs_scanner.model import RepositoryRuntime
 from vcs_scanner.output_modules.rws_api_writer import RESTAPIWriter
+from vcs_scanner.helpers.providers.rule_tag import RuleTagProvider
+from vcs_scanner.helpers.providers.rule_file import RuleFileProvider
 from vcs_scanner.secret_scanners.configuration import (
     GITLEAKS_PATH,
     RABBITMQ_DEFAULT_VHOST,
     RABBITMQ_PASSWORD,
     RABBITMQ_QUEUE,
     RABBITMQ_SERVICE_HOST,
     RABBITMQ_USERNAME,
@@ -88,30 +90,38 @@
         )
         # Split the include_tags by comma if supplied
         include_tags = env_variables[RESC_INCLUDE_TAGS].split(",") if env_variables[RESC_INCLUDE_TAGS] else None
 
         # Split the ignore_tags by comma if supplied
         ignore_tags = env_variables[RESC_IGNORE_TAGS].split(",") if env_variables[RESC_IGNORE_TAGS] else None
 
+        rule_tag_provider = RuleTagProvider()
+        rule_tag_provider.load(TEMP_RULE_FILE)
+
+        rest_api_writer = RESTAPIWriter(
+            rws_url=rws_url, include_tags=include_tags, ignore_tags=ignore_tags, rule_tag_provider=rule_tag_provider
+        )
+
+        gitleaks_rules_provider = RuleFileProvider(TEMP_RULE_FILE)
+        gitleaks_rules_provider.init(
+            destination_rule_as_repo=TEMP_RULE_REPO_FILE,
+            destination_rule_as_dir=TEMP_RULE_DIR_FILE,
+        )
+
         secret_scanner = SecretScanner(
             gitleaks_binary_path=env_variables[GITLEAKS_PATH],
-            gitleaks_rules_path=TEMP_RULE_FILE,
+            gitleaks_rules_provider=gitleaks_rules_provider,
             rule_pack_version=active_rule_pack_version,
-            output_plugin=RESTAPIWriter(
-                rws_url=rws_url,
-                toml_rule_file_path=TEMP_RULE_FILE,
-                include_tags=include_tags,
-                ignore_tags=ignore_tags,
-            ),
+            output_plugin=rest_api_writer,
             repository=repository,
             username=vcs_instance.username,
             personal_access_token=vcs_instance.token,
             force_base_scan=os.getenv("FORCE_BASE_SCAN", "false").lower() in "true",
             latest_commit=repository_runtime.latest_commit,
         )
 
-        secret_scanner.run_repository_scan()
+        secret_scanner.run_scan(as_dir=True, as_repo=True)
     except KeyError:
         logger.error(
             f"No configuration found for vcs instance {repository_runtime.vcs_instance_name}, "
             f"unable to scan {repository_runtime.project_key}/{repository_runtime.repository_name}"
         )
```

### Comparing `resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/cli.py` & `resc_vcs_scanner-3.3.0/src/vcs_scanner/secret_scanners/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     CLI_VCS_LOCAL_SCAN,
     LOG_FILE_PATH_CLI,
 )
 from vcs_scanner.helpers.cli import create_cli_argparser
 from vcs_scanner.model import RepositoryRuntime
 from vcs_scanner.output_modules.rws_api_writer import RESTAPIWriter
 from vcs_scanner.output_modules.stdout_writer import STDOUTWriter
+from vcs_scanner.secret_scanners.git_operation import read_repo_from_local
 from vcs_scanner.secret_scanners.secret_scanner import SecretScanner
+from vcs_scanner.helpers.providers.rule_file import RuleFileProvider
 
 logger_config = initialise_logs(LOG_FILE_PATH_CLI)
 logger = logging.getLogger(__name__)
 
 FAKE_COMMIT = "hash"
 FAKE_URL = "http://fake-host.none"
 
@@ -105,22 +107,30 @@
 
     if args.command == "dir":
         logger.info(f"Scanning directory {args.dir.absolute()}")
         scan_directory(args)
     elif args.command == "repo":
         if args.repository_location == "local":
             logger.info(f"Scanning repository local {args.dir.absolute()}")
-            args.repo_url = FAKE_URL
+            args.repo_url = fetch_url_from_dot_git_config(args.dir.absolute())
             args.username = None
             args.password = None
         elif args.repository_location == "remote":
             logger.info(f"Scanning repository remote {args.repo_url}")
         scan_repository(args)
 
 
+def fetch_url_from_dot_git_config(path: str):
+    if not os.path.exists(path / ".git/config"):
+        return FAKE_URL
+
+    return read_repo_from_local(path)
+
+
+# TODO refactor and merge scan_directory / scan_repository to avoid code duplication.
 def scan_directory(args: Namespace):
     """
         Start the process of scanning a non-git directory
     :param args:
         Namespace object containing the CLI arguments
     """
     repository = RepositoryRuntime(
@@ -128,40 +138,37 @@
         repository_name="local",
         repository_id="local",
         project_key="local",
         vcs_instance_name="vcs_instance_name",
         latest_commit=FAKE_COMMIT,
     )
 
-    output_plugin = STDOUTWriter(
-        toml_rule_file_path=args.gitleaks_rules_path,
-        exit_code_warn=args.exit_code_warn,
-        exit_code_block=args.exit_code_block,
-        include_tags=args.include_tags,
-        ignore_tags=args.ignore_tags,
-        working_dir=args.dir,
-        ignore_findings_path=args.ignored_blocker_path,
-    )
-    with open(args.gitleaks_rules_path, encoding="utf-8") as rule_pack:
-        rule_pack_version = get_rule_pack_version_from_file(rule_pack.read())
+    output_plugin = STDOUTWriter.make(args)
+    rule_pack_version = _get_rule_pack_version(args)
+
     if not rule_pack_version:
         rule_pack_version = "0.0.0"
 
+    gitleaks_rules_provider = RuleFileProvider(args.gitleaks_rules_path, init=True)
+
     secret_scanner = SecretScanner(
         gitleaks_binary_path=args.gitleaks_path,
-        gitleaks_rules_path=args.gitleaks_rules_path,
+        gitleaks_rules_provider=gitleaks_rules_provider,
         rule_pack_version=rule_pack_version,
         output_plugin=output_plugin,
         repository=repository.convert_to_repository(vcs_instance_id=1),
         username="",
         personal_access_token="",
         local_path=f"{args.dir.absolute()}",
+        # we force a base scan because it does not matter
+        # in this use case: we are not sending data to RESC.
+        force_base_scan=True,
     )
 
-    secret_scanner.run_directory_scan()
+    secret_scanner.run_scan(as_dir=True)
 
 
 def scan_repository(args: Namespace):
     """
         Start the process of scanning a git repository (remote or local)
     :param args:
         Namespace object containing the CLI arguments
@@ -175,51 +182,40 @@
         repository_id=args.repo_name,
         project_key=args.repo_name,
         vcs_instance_name=vcs_name,
         latest_commit=FAKE_COMMIT,
     )
 
     if args.rws_url:
-        output_plugin = RESTAPIWriter(
-            rws_url=args.rws_url,
-            toml_rule_file_path=args.gitleaks_rules_path,
-            include_tags=args.include_tags,
-            ignore_tags=args.ignore_tags,
-        )
+        output_plugin = RESTAPIWriter.make(args)
         rule_pack_version = output_plugin.download_rule_pack()
 
     else:
-        output_plugin = STDOUTWriter(
-            toml_rule_file_path=args.gitleaks_rules_path,
-            exit_code_warn=args.exit_code_warn,
-            exit_code_block=args.exit_code_block,
-            include_tags=args.include_tags,
-            ignore_tags=args.ignore_tags,
-            working_dir=args.dir,
-            ignore_findings_path=args.ignored_blocker_path,
-        )
-        with open(args.gitleaks_rules_path, encoding="utf-8") as rule_pack:
-            rule_pack_version = get_rule_pack_version_from_file(rule_pack.read())
+        output_plugin = STDOUTWriter.make(args)
+        rule_pack_version = _get_rule_pack_version(args)
+
     if not rule_pack_version:
         rule_pack_version = "0.0.0"
 
+    gitleaks_rules_provider = RuleFileProvider(args.gitleaks_rules_path, init=True)
+
     secret_scanner = SecretScanner(
         gitleaks_binary_path=args.gitleaks_path,
-        gitleaks_rules_path=args.gitleaks_rules_path,
+        gitleaks_rules_provider=gitleaks_rules_provider,
         rule_pack_version=rule_pack_version,
         output_plugin=output_plugin,
         repository=repository.convert_to_repository(vcs_instance_id=1),
         username=args.username,
         personal_access_token=args.password,
         local_path=f"{args.dir.absolute()}",
         force_base_scan=args.force_base_scan,
         latest_commit="unknown",
     )
 
-    secret_scanner.run_repository_scan()
+    secret_scanner.run_scan(as_repo=True)
 
 
 def guess_vcs_provider(repo_url: str) -> VCSProviders:
     """
         Guess the vcs provider based on the url given, defaulted to bitbucket
     :param repo_url:
         Full url of the repository
@@ -248,7 +244,12 @@
     vcs_name = CLI_VCS_LOCAL_SCAN
     if repo_url and repo_url is not FAKE_URL:
         if vcs_type == VCSProviders.AZURE_DEVOPS:
             vcs_name = CLI_VCS_AZURE
         elif vcs_type == VCSProviders.BITBUCKET:
             vcs_name = CLI_VCS_BITBUCKET
     return vcs_name
+
+
+def _get_rule_pack_version(args: Namespace) -> str | None:
+    with open(args.gitleaks_rules_path, encoding="utf-8") as rule_pack:
+        return get_rule_pack_version_from_file(rule_pack.read())
```

### Comparing `resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/configuration.py` & `resc_vcs_scanner-3.3.0/src/vcs_scanner/secret_scanners/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py` & `resc_vcs_scanner-3.3.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             command.append("--no-git")
 
         # Incremental scan command
         if self.scan_from:
             command.append(f"--log-opts={self.scan_from}..")
         return command
 
-    def start_scan(self) -> list[FindingBase] | None:
+    def start_scan(self) -> list[FindingBase]:
         """
         :return: Output.
             If Successful, a list of FindingCreate objects is returned.
             Otherwise, a None object is returned
         """
         try:
             result = subprocess.run(
@@ -68,24 +68,24 @@
             if exitcode == NO_LEAKS_FOUND_EXIT_CODE:
                 return []
             if exitcode == LEAKS_FOUND_EXIT_CODE:
                 return self._parse_output(self.report_filepath)
 
             error_output = result.stderr.decode("utf-8")
             logger.error(f"GitLeaks exited with an unexpected code: {exitcode}. Output: {error_output}")
-            return None
+            return []
 
         except subprocess.CalledProcessError as called_process_error:
             logger.error(
                 f"Error encountered while running the gitleaks process: {called_process_error.stdout.decode('utf-8')}"
             )
-            return None
+            return []
         except FileNotFoundError as error:
             logger.error(f"Unable to locate a file: {error}")
-            return None
+            return []
 
     @staticmethod
     def _calculate_permanent_leak_url(leak_url: str, repository: str, commit_id: str) -> str:
         """
             The Leak URL given by bitbucket is not correct.
             Construct a proper one that links to the exact change in the commit
         :param leak_url: The url of the leak (Bitbucket format)
@@ -104,46 +104,50 @@
         new_url = new_url.replace("/blob/", "/commits/")
         new_url = new_url.replace(f"/{repository}/", f"/repos/{repository[:-4]}/")  # remove .git at the end
         new_url = new_url.replace(f"/{commit_id}/", f"/{commit_id}#")
 
         return new_url
 
     @staticmethod
-    def _is_valid_timestamp(timestamp: str) -> datetime | None:
+    def _get_valid_timestamp(timestamp: str) -> datetime:
+        if timestamp == "":
+            logger.debug("Date is empty, using now(UTC) instead.")
+            return datetime.now(UTC)
+
         try:
-            converted_timestamp: datetime | None = datetime.strptime(timestamp, "%Y-%m-%dT%H:%M:%S%z")
+            converted_timestamp: datetime | None = datetime.fromisoformat(timestamp)
         except ValueError:
-            converted_timestamp = None
+            logger.debug(f"{timestamp} has an unexpected date format. Expected ISO 8601")
+            converted_timestamp = datetime.now(UTC)
+
         return converted_timestamp
 
     @classmethod
     def _parse_output(cls, file_path: str) -> list[FindingBase]:
         """
         Parse the gitleaks findings from the temp file and return a list of Finding objects
         :param file_path: the tempfile containing the gitleaks findings
         :return: list of Finding objects
         """
         findings = []
         with open(file_path, encoding="utf-8") as report_file:
             results = json.load(report_file)
 
         for result in results:
-            commit_timestamp = cls._is_valid_timestamp(result["Date"])
-            if not commit_timestamp:
-                logger.debug(f"{result['Date']} has an unexpected date format. Expected ISO 8601")
-                commit_timestamp = datetime.now(UTC)
+            commit_timestamp = cls._get_valid_timestamp(result["Date"])
             finding = FindingBase(
                 file_path=result["File"],
                 line_number=result["StartLine"],
                 column_start=result["StartColumn"],
                 column_end=result["EndColumn"],
                 email=result["Email"],
                 author=result["Author"],
                 commit_id=result["Commit"],
                 commit_message=result["Message"],
                 commit_timestamp=commit_timestamp,
                 rule_name=result["RuleID"],
             )
+            logger.debug(finding)
 
             findings.append(finding)
 
         return findings
```

### Comparing `resc_vcs_scanner-3.1.1/src/vcs_scanner/secret_scanners/secret_scanner.py` & `resc_vcs_scanner-3.3.0/src/vcs_scanner/secret_scanners/secret_scanner.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,232 +2,309 @@
 # Standard Library
 import logging
 import os
 import shutil
 import time
 import uuid
 from datetime import datetime, UTC
+from collections.abc import Callable
 
 # Third Party
 from resc_backend.resc_web_service.schema.finding import FindingBase
 from resc_backend.resc_web_service.schema.repository import Repository
+from resc_backend.resc_web_service.schema.repository import RepositoryBase
 from resc_backend.resc_web_service.schema.scan import Scan
+from resc_backend.resc_web_service.schema.scan import ScanRead
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 
 # First Party
 from vcs_scanner.output_modules.output_module import OutputModule
 from vcs_scanner.resc_worker import RESCWorker
 from vcs_scanner.secret_scanners.git_operation import clone_repository
 from vcs_scanner.secret_scanners.gitleaks_wrapper import GitLeaksWrapper
+from vcs_scanner.helpers.providers.rule_file import RuleFileProvider
 
 # This is an arbitrary number to distinguish between no issues, an error and
 # the situation in which leaks are found. Note that this number cannot be bigger than 255 (OS limitation)
 LEAKS_FOUND_EXIT_CODE = 42
 NO_LEAKS_FOUND_EXIT_CODE = 0
 
 logger = logging.getLogger(__name__)
 
 
 class SecretScanner(RESCWorker):  # pylint: disable=R0902
     def __init__(
         self,
         gitleaks_binary_path: str,
-        gitleaks_rules_path: str,
+        gitleaks_rules_provider: RuleFileProvider,
         rule_pack_version: str,
         output_plugin: OutputModule,
         repository: Repository,
         username: str,
         personal_access_token: str,
         scan_tmp_directory: str = ".",
-        local_path: str = None,
+        local_path: str | None = None,
         force_base_scan: bool = False,
-        latest_commit: str = None,
+        latest_commit: str | None = None,
     ):
-        self.gitleaks_rules_path: str = gitleaks_rules_path
+        self.rule_provider: RuleFileProvider | None = None
+        self.gitleaks_rules_provider: RuleFileProvider = gitleaks_rules_provider
         self.gitleaks_binary_path: str = gitleaks_binary_path
         self.rule_pack_version: str = rule_pack_version
         self._output_module: OutputModule = output_plugin
         self._scan_tmp_directory: str = scan_tmp_directory
         self.repository: Repository = repository
         self.username: str = username
         self.personal_access_token: str = personal_access_token
         self.local_path = local_path
         self.force_base_scan = force_base_scan
         self.latest_commit = latest_commit
+        self.head_commit: None | str = None
+
+        self._as_dir: bool = False
+        self._as_repo: bool = False
+        self._created_repository: None | RepositoryBase = None
+        self._last_scanned_commit: None | str = None
+        self._scan_type_to_run: None | ScanType = None
+        self._scan_timestamp_start: None | datetime = None
+        self._created_scan: None | ScanRead = None
+        self._repo_clone_path: None | str = None
+        self._findings_from_repo: list[FindingBase] = []
+        self._findings_from_dir: list[FindingBase] = []
+        self._findings: list[FindingBase] = []
+
         if self.local_path:
             self.repo_display_name = self.local_path.replace(".", "_").replace("/", "_")
         else:
             self.repo_display_name = self.repository.repository_url
 
-    def clone_repo(self) -> str:
-        repo_clone_path = f"{self._scan_tmp_directory}/{self.repository.repository_name}"
-        clone_repository(
-            self.repository.repository_url,
-            repo_clone_path,
-            username=self.username,
-            personal_access_token=self.personal_access_token,
-        )
-        return repo_clone_path
+    def run_scan(self, as_dir: bool = False, as_repo: bool = False) -> None:
+        """
+        Run the scan steps by steps.
+
+        Args:
+            as_dir (bool, optional): whether we scan as directory. Defaults to False.
+            as_repo (bool, optional): whether we scan as repository. Defaults to False.
+        """
+        self._as_dir = as_dir
+        self._as_repo = as_repo
+
+        pipes: list[Callable[[], bool]] = [
+            self._is_valid,
+            self._is_scan_needed_from_latest_commit,
+            self._create_repository,
+            self._fetch_last_scanned_commit,
+            self._is_scan_needed,
+            self._start_timer,
+            self._create_scan,
+            self._clone_repo,
+            self._run_repo_scan,
+            self._run_dir_scan,
+            self._merge_findings,
+            self._write_findings,
+            self._cleaning_up,
+        ]
+
+        for pipe in pipes:
+            # If the pipe does not succeed we exit immediately.
+            if not pipe():
+                return
+
+    def _is_valid(self) -> bool:
+        if not self._as_dir and not self._as_repo:
+            logger.error("no scan type selected")
+            return False
+        return True
 
-    def run_repository_scan(self) -> None:
-        if not self.latest_commit:
+    def _is_scan_needed_from_latest_commit(self) -> bool:
+        if self._as_repo and not self.latest_commit:
             # There is no latest commit for this repository, assuming that its empty
             logger.info(
                 f"Skipping scanning of {self.repository.project_key}/{self.repository.repository_name} "
                 f"there are no commits"
             )
-            return
+            return False
         logger.info(
             f"Started task for scanning {self.repository.repository_name} using "
             f"rule pack version: {self.rule_pack_version}"
         )
+        return True
 
+    def _create_repository(self) -> bool:
         # Insert in to repository table
-        created_repository = self._output_module.write_repository(self.repository)
-        if not created_repository:
+        self._created_repository = self._output_module.write_repository(self.repository)
+        if not self._created_repository:
             logger.error(
                 f"Error processing "
                 f"{self.repository.repository_name}."
-                f" Error details: unable to create repository: {created_repository}"
+                f" Error details: unable to create repository: {self._created_repository}"
             )
-            return
+            return False
 
         logger.info(f"Scanning repository {self.repository.project_key}/{self.repository.repository_name}")
+        return True
 
+    def _fetch_last_scanned_commit(self) -> True:
         # Get last scanned commit for the repository
-        last_scan_for_repository = self._output_module.get_last_scan_for_repository(repository=created_repository)
-        last_scanned_commit = last_scan_for_repository.last_scanned_commit if last_scan_for_repository else None
-        scan_type_to_run = self.determine_scan_type(
-            latest_commit=self.latest_commit,
+        last_scan_for_repository = self._output_module.get_last_scan_for_repository(repository=self._created_repository)
+        self._last_scanned_commit = last_scan_for_repository.last_scanned_commit if last_scan_for_repository else None
+        self._scan_type_to_run = self._determine_scan_type(
             last_scan_for_repository=last_scan_for_repository,
         )
+        return True
 
-        if scan_type_to_run:
-            # Insert in to scan table
-            scan_timestamp_start = datetime.now(UTC)
-            created_scan = self._output_module.write_scan(
-                scan_type_to_run,
-                self.latest_commit,
-                scan_timestamp_start.isoformat(),
-                created_repository,
-                rule_pack=self.rule_pack_version,
-            )
-            if not created_scan:
-                logger.error(
-                    f"Error processing {self.repository.project_key}/{self.repository.repository_name} "
-                    f"Error details: unable to create scan object"
-                )
-                return
-
-            # Clone and run scan upon the repository
-            if not self.local_path:
-                repo_clone_path: str = self.clone_repo()
-            else:
-                repo_clone_path = self.local_path
+    def _determine_scan_type(self, last_scan_for_repository: Scan) -> ScanType | None:
+        # Force base scan, or has no previous scan
+        if self.force_base_scan or last_scan_for_repository is None:
+            return ScanType.BASE
+        # Has previous scan
+        if last_scan_for_repository:
+            # Rule-pack is different from previous scan
+            if last_scan_for_repository.rule_pack != self.rule_pack_version:
+                return ScanType.BASE
+            # Last commit is different from previous scan
+            if self.latest_commit and self.latest_commit != last_scan_for_repository.last_scanned_commit:
+                return ScanType.INCREMENTAL
+        # Skip scanning, no conditions match
+        return None
 
-            findings = self.scan_repo(scan_type_to_run, last_scanned_commit, repo_clone_path)
-            scan_timestamp_end = datetime.now(UTC)
+    def _is_scan_needed(self) -> bool:
+        if self._scan_type_to_run is None:
             logger.info(
-                f"Running {scan_type_to_run} scan on repository "
-                f"{self.repository.project_key}/{self.repository.repository_name}"
-                f" took {scan_timestamp_end - scan_timestamp_start} ms."
+                "Skipped scanning on repository: "
+                f"{self.repository.project_key}/{self.repository.repository_name} no new commits found."
             )
+            return False
+        return True
 
-            if findings:
-                logger.info(f"Scan completed: {len(findings)} findings were found.")
-                self._output_module.write_findings(
-                    repository_id=created_repository.id_,
-                    scan_id=created_scan.id_,
-                    scan_findings=findings,
-                )
-            else:
-                logger.info(
-                    "No findings registered in " f"{self.repository.project_key}/{self.repository.repository_name}"
-                )
-        else:
-            logger.info(
-                f"Skipped {scan_type_to_run} scanning on repository: "
-                f"{self.repository.project_key}/{self.repository.repository_name} no new commits found."
+    def _start_timer(self) -> True:
+        self._scan_timestamp_start = datetime.now(UTC)
+        return True
+
+    def _create_scan(self) -> bool:
+        self._created_scan = self._output_module.write_scan(
+            self._scan_type_to_run,
+            self.latest_commit,
+            self._scan_timestamp_start.isoformat(),
+            self._created_repository,
+            rule_pack=self.rule_pack_version,
+        )
+        if not self._created_scan:
+            logger.error(
+                f"Error processing {self.repository.project_key}/{self.repository.repository_name} "
+                f"Error details: unable to create scan object"
             )
+            return False
+        return True
 
-    def run_directory_scan(self) -> None:
-        """
-        Scan the given non-git directory, set in the self.local_path variable
-        """
-        logger.info(f"Started task for scanning {self.local_path} using rule pack version: {self.rule_pack_version}")
+    def _clone_repo(self) -> True:
+        # Clone and run scan upon the repository
+        if not self.local_path:
+            self._repo_clone_path = f"{self._scan_tmp_directory}/{self.repository.repository_name}"
+            self.head_commit = clone_repository(
+                repository_url=self.repository.repository_url,
+                repo_clone_path=self._repo_clone_path,
+                username=self.username,
+                personal_access_token=self.personal_access_token,
+            )
+        else:
+            self._repo_clone_path = self.local_path
+        return True
+
+    def _run_repo_scan(self) -> True:
+        if not self._as_repo:
+            return True
+
+        if self.gitleaks_rules_provider.scan_as_repo_rule_file_path is None:
+            return True
 
+        logger.info(
+            f"Started task for scanning {self._repo_clone_path} using rule pack version: {self.rule_pack_version}"
+        )
         scan_timestamp_start = datetime.now(UTC)
-        findings = self.scan_directory(self.local_path)
+        self._findings_from_repo = self._scan_repo(self._scan_type_to_run, self._last_scanned_commit)
         scan_timestamp_end = datetime.now(UTC)
-        logger.info(f"Running local scan on {self.local_path} took {scan_timestamp_end - scan_timestamp_start} ms.")
-
-        if findings:
-            logger.info(f"Scan completed: {len(findings)} findings were found.")
-            self._output_module.write_findings(repository_id=0, scan_id=0, scan_findings=findings)
-        else:
-            logger.info(f"No findings registered in {self.local_path}.")
+        logger.info(
+            f"Running {self._scan_type_to_run} scan on repository "
+            f"{self.repository.project_key}/{self.repository.repository_name}"
+            f" took {scan_timestamp_end - scan_timestamp_start} ms."
+        )
+        return True
 
-    def scan_repo(
-        self, scan_type_to_run: str, last_scanned_commit: str, repo_clone_path: str
-    ) -> list[FindingBase] | None:
+    def _scan_repo(self, scan_type_to_run: str, last_scanned_commit: str) -> list[FindingBase]:
         """
             Clone and scan the given repository
-        :param repo_clone_path:
-            Directory path where the repository has already been cloned
         :param scan_type_to_run:
             Type of scan to run (Base or Incremental)
         :param last_scanned_commit:
             Last scanned commit of the repository to scan
         :return: Success, output.
             If Success is False, the output will contain an error message.
             Otherwise, the output will contain a list of findings or an empty list if no issue was found
         """
 
         logger.debug(f"Started scanning {self.repo_display_name}")
         if not self.local_path:
-            report_filepath = f"{self._scan_tmp_directory}/{repo_clone_path}_{str(uuid.uuid4().hex)}.json"
+            report_filepath = f"{self._scan_tmp_directory}/{self._repo_clone_path}_{str(uuid.uuid4().hex)}.json"
         else:
             report_filepath = f"{self.local_path}/{self.repo_display_name}_{str(uuid.uuid4().hex)}.json"
         try:
             if scan_type_to_run == ScanType.BASE:
                 scan_from = None
             elif scan_type_to_run == ScanType.INCREMENTAL and last_scanned_commit:
                 scan_from = last_scanned_commit
             else:
                 scan_from = None
 
             gitleaks_command = GitLeaksWrapper(
                 scan_from=scan_from,
                 gitleaks_path=self.gitleaks_binary_path,
-                repository_path=repo_clone_path,
-                rules_filepath=self.gitleaks_rules_path,
+                repository_path=self._repo_clone_path,
+                rules_filepath=self.gitleaks_rules_provider.scan_as_repo_rule_file_path,
                 report_filepath=report_filepath,
             )
 
             before_scan = time.time()
-            findings: list[FindingBase] | None = gitleaks_command.start_scan()
+            findings: list[FindingBase] = gitleaks_command.start_scan()
             after_scan = time.time()
             scan_duration = int(after_scan - before_scan)
-            logger.info(f"scan of repository {repo_clone_path} took {scan_duration} seconds")
+            logger.info(f"scan of repository {self._repo_clone_path} took {scan_duration} seconds")
             return findings
         except BaseException as error:
             logger.error(
                 f"An exception occurred while scanning repository {self.repository.repository_url} " f"error: {error}"
             )
+            return []
         finally:
             # Make sure the tempfile and repo cloned path removed
             logger.debug(f"Cleaning up the temporary report: {report_filepath}")
             if os.path.exists(report_filepath):
                 os.remove(report_filepath)
-            if repo_clone_path and not self.local_path and os.path.exists(repo_clone_path):
-                logger.debug(f"Cleaning up the repository cloned directory: {repo_clone_path}")
-                shutil.rmtree(repo_clone_path)
-        return None
 
-    def scan_directory(self, directory_path: str) -> list[FindingBase] | None:
+    def _run_dir_scan(self):
+        if not self._as_dir:
+            return True
+
+        if self.gitleaks_rules_provider.scan_as_dir_rule_file_path is None:
+            return True
+
+        logger.info(
+            f"Started task for scanning {self._repo_clone_path} using rule pack version: {self.rule_pack_version}"
+        )
+
+        scan_timestamp_start = datetime.now(UTC)
+        self._findings_from_dir = self._scan_directory(self._repo_clone_path)
+        scan_timestamp_end = datetime.now(UTC)
+        logger.info(
+            f"Running directory scan on {self._repo_clone_path}"
+            f" took {scan_timestamp_end - scan_timestamp_start} ms."
+        )
+        return True
+
+    def _scan_directory(self, directory_path: str) -> list[FindingBase] | None:
         """
             Scan the given directory
         :param directory_path:
             Directory path to be scanned
         :return: Optional[List[FindingBase]].
             The output will contain a list of findings or an empty list if no finding was found
         """
@@ -237,42 +314,62 @@
         else:
             report_filepath = f"{self.local_path}/{self.repo_display_name}_{str(uuid.uuid4().hex)}.json"
         try:
             gitleaks_command = GitLeaksWrapper(
                 scan_from=None,
                 gitleaks_path=self.gitleaks_binary_path,
                 repository_path=directory_path,
-                rules_filepath=self.gitleaks_rules_path,
+                rules_filepath=self.gitleaks_rules_provider.scan_as_dir_rule_file_path,
                 report_filepath=report_filepath,
                 git_scan=False,
             )
 
             before_scan = time.time()
-            findings: list[FindingBase] | None = gitleaks_command.start_scan()
+            findings: list[FindingBase] = gitleaks_command.start_scan()
             after_scan = time.time()
             scan_duration = int(after_scan - before_scan)
             logger.info(f"scan of repository {directory_path} took {scan_duration} seconds")
             return findings
         except BaseException as error:
             logger.error(f"An exception occurred while scanning directory {directory_path} error: {error}")
         finally:
             # Make sure the tempfile is removed
             logger.debug(f"Cleaning up the temporary report: {report_filepath}")
             if os.path.exists(report_filepath):
                 os.remove(report_filepath)
         return None
 
-    # Decide which type of scan to run
-    def determine_scan_type(self, last_scan_for_repository: Scan, latest_commit: str = None):
-        # Force base scan, or has no previous scan
-        if self.force_base_scan or last_scan_for_repository is None:
-            return ScanType.BASE
-        # Has previous scan
-        if last_scan_for_repository:
-            # Rule-pack is different from previous scan
-            if last_scan_for_repository.rule_pack != self.rule_pack_version:
-                return ScanType.BASE
-            # Last commit is different from previous scan
-            if latest_commit and latest_commit != last_scan_for_repository.last_scanned_commit:
-                return ScanType.INCREMENTAL
-        # Skip scanning, no conditions match
-        return None
+    def _merge_findings(self) -> bool:
+        if len(self._findings_from_dir) == 0 and len(self._findings_from_repo) == 0:
+            path = (
+                self.local_path
+                if self.local_path
+                else self.repository.project_key + "/" + self.repository.repository_name
+            )
+            logger.info(f"No findings registered in {path}.")
+            return False
+
+        self._findings = self._findings_from_repo + self._findings_from_dir
+        self._findings = list(map(self._populate_if_empty, self._findings))
+        return True
+
+    def _populate_if_empty(self, finding: FindingBase) -> FindingBase:
+        finding.commit_id = finding.commit_id or self.head_commit or "unknown"
+        finding.author = finding.author or "vcs-scanner"
+        return finding
+
+    def _write_findings(self) -> True:
+        logger.info(f"Scan completed: {len(self._findings)} findings were found.")
+        self._output_module.write_findings(
+            repository_id=getattr(self._created_repository, "id_", 0),
+            scan_id=getattr(self._created_scan, "id_", 0),
+            scan_findings=self._findings,
+            repository_name=self.repository.repository_name,
+        )
+        return True
+
+    def _cleaning_up(self) -> True:
+        # Make sure the tempfile and repo cloned path removed
+        if self._repo_clone_path and not self.local_path and os.path.exists(self._repo_clone_path):
+            logger.debug(f"Cleaning up the repository cloned directory: {self._repo_clone_path}")
+            shutil.rmtree(self._repo_clone_path)
+        return True
```

### Comparing `resc_vcs_scanner-3.1.1/src/vcs_scanner/static/logging.ini` & `resc_vcs_scanner-3.3.0/src/vcs_scanner/static/logging.ini`

 * *Files identical despite different names*

