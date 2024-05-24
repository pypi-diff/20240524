# Comparing `tmp/tinybird-cli-3.9.1.dev5.tar.gz` & `tmp/tinybird-cli-3.9.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cli-3.9.1.dev5.tar", last modified: Tue Apr 30 07:04:29 2024, max compression
+gzip compressed data, was "tinybird-cli-3.9.1.dev6.tar", last modified: Tue Apr 30 08:59:36 2024, max compression
```

## Comparing `tinybird-cli-3.9.1.dev5.tar` & `tinybird-cli-3.9.1.dev6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:04:29.310853 tinybird-cli-3.9.1.dev5/
--rw-r--r--   0 root         (0) root         (0)    68737 2024-04-30 07:04:29.309853 tinybird-cli-3.9.1.dev5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 07:04:29.310853 tinybird-cli-3.9.1.dev5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:04:29.306853 tinybird-cli-3.9.1.dev5/tinybird/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-30 07:04:28.000000 tinybird-cli-3.9.1.dev5/tinybird/__cli__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:04:29.306853 tinybird-cli-3.9.1.dev5/tinybird/ch_utils/
--rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/ch_utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39699 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/ch_utils/engine.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/check_pypi.py
--rw-rw-rw-   0 root         (0) root         (0)    46735 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/config.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/connectors.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/context.py
--rw-rw-rw-   0 root         (0) root         (0)   212518 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/datafile.py
--rw-rw-rw-   0 root         (0) root         (0)     7060 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)    59638 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/feedback_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4707 2024-04-30 07:04:22.000000 tinybird-cli-3.9.1.dev5/tinybird/git_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    41589 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/sql.py
--rw-rw-rw-   0 root         (0) root         (0)    81435 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/sql_template.py
--rw-rw-rw-   0 root         (0) root         (0)    10196 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/sql_template_fmt.py
--rw-rw-rw-   0 root         (0) root         (0)    11568 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/sql_toolset.py
--rw-rw-rw-   0 root         (0) root         (0)    27763 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/syncasync.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:04:29.308853 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    37863 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/branch.py
--rw-rw-rw-   0 root         (0) root         (0)    14087 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/cicd.py
--rw-rw-rw-   0 root         (0) root         (0)    64868 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    78344 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/common.py
--rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/config.py
--rw-rw-rw-   0 root         (0) root         (0)    31660 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/connection.py
--rw-rw-rw-   0 root         (0) root         (0)    31944 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/datasource.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2964 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/job.py
--rw-rw-rw-   0 root         (0) root         (0)    26155 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/pipe.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/regions.py
--rw-rw-rw-   0 root         (0) root         (0)    10490 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/telemetry.py
--rw-rw-rw-   0 root         (0) root         (0)     4223 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:04:29.308853 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/tinyunit/
--rw-rw-rw-   0 root         (0) root         (0)    11667 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/tinyunit/tinyunit.py
--rw-rw-rw-   0 root         (0) root         (0)     1868 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/token.py
--rw-rw-rw-   0 root         (0) root         (0)    10081 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/workspace.py
--rw-rw-rw-   0 root         (0) root         (0)     8268 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/workspace_members.py
--rw-rw-rw-   0 root         (0) root         (0)    41982 2024-04-30 07:04:23.000000 tinybird-cli-3.9.1.dev5/tinybird/tornado_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:04:29.309853 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    68737 2024-04-30 07:04:29.000000 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1348 2024-04-30 07:04:29.000000 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 07:04:29.000000 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-30 07:04:29.000000 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      732 2024-04-30 07:04:29.000000 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-30 07:04:29.000000 tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 08:59:36.694357 tinybird-cli-3.9.1.dev6/
+-rw-r--r--   0 root         (0) root         (0)    68837 2024-04-30 08:59:36.693358 tinybird-cli-3.9.1.dev6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 08:59:36.694357 tinybird-cli-3.9.1.dev6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 08:59:36.690358 tinybird-cli-3.9.1.dev6/tinybird/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-30 08:59:35.000000 tinybird-cli-3.9.1.dev6/tinybird/__cli__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 08:59:36.690358 tinybird-cli-3.9.1.dev6/tinybird/ch_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/ch_utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39699 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/ch_utils/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/check_pypi.py
+-rw-rw-rw-   0 root         (0) root         (0)    46918 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2003 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/context.py
+-rw-rw-rw-   0 root         (0) root         (0)   212518 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/datafile.py
+-rw-rw-rw-   0 root         (0) root         (0)     7060 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)    59923 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/feedback_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4707 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/git_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    41589 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    81435 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/sql_template.py
+-rw-rw-rw-   0 root         (0) root         (0)    10196 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/sql_template_fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)    11568 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/sql_toolset.py
+-rw-rw-rw-   0 root         (0) root         (0)    27763 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/syncasync.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 08:59:36.692358 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    37863 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/branch.py
+-rw-rw-rw-   0 root         (0) root         (0)    14087 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/cicd.py
+-rw-rw-rw-   0 root         (0) root         (0)    64868 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    78344 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    31660 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31944 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/datasource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/job.py
+-rw-rw-rw-   0 root         (0) root         (0)    26155 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/pipe.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/regions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10490 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/telemetry.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 08:59:36.693358 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/tinyunit/
+-rw-rw-rw-   0 root         (0) root         (0)    11667 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/tinyunit/tinyunit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/token.py
+-rw-rw-rw-   0 root         (0) root         (0)    11064 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/workspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/workspace_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    41982 2024-04-30 08:59:31.000000 tinybird-cli-3.9.1.dev6/tinybird/tornado_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 08:59:36.693358 tinybird-cli-3.9.1.dev6/tinybird_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    68837 2024-04-30 08:59:36.000000 tinybird-cli-3.9.1.dev6/tinybird_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-04-30 08:59:36.000000 tinybird-cli-3.9.1.dev6/tinybird_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 08:59:36.000000 tinybird-cli-3.9.1.dev6/tinybird_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-30 08:59:36.000000 tinybird-cli-3.9.1.dev6/tinybird_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      732 2024-04-30 08:59:36.000000 tinybird-cli-3.9.1.dev6/tinybird_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-30 08:59:36.000000 tinybird-cli-3.9.1.dev6/tinybird_cli.egg-info/top_level.txt
```

### Comparing `tinybird-cli-3.9.1.dev5/PKG-INFO` & `tinybird-cli-3.9.1.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.9.1.dev5
+Version: 3.9.1.dev6
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -14,20 +14,24 @@
 =============
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 ----------
 
+3.9.1.dev6
+************
+
+- `Added` Support for unlink materialized pipes doing `tb workspace clear`
+
 3.9.1.dev5
 ************
 
 - `Added` support for adding multiple tokens when pushing a `.datasource` file
 
-
 3.9.1.dev4
 ************
 
 - `Fixed` s3 iamrole connection creation will not fail when `pbcopy` dependency is not available
 
 3.9.1.dev3
 ************
```

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/ch_utils/constants.py` & `tinybird-cli-3.9.1.dev6/tinybird/ch_utils/constants.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/ch_utils/engine.py` & `tinybird-cli-3.9.1.dev6/tinybird/ch_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/check_pypi.py` & `tinybird-cli-3.9.1.dev6/tinybird/check_pypi.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/client.py` & `tinybird-cli-3.9.1.dev6/tinybird/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -584,14 +584,17 @@
     async def pipe_remove_sink(self, pipe_name_or_id: str, node_id: str):
         return await self._req(f"/v0/pipes/{pipe_name_or_id}/nodes/{node_id}/sink", method="DELETE")
 
     async def pipe_run_sink(self, pipe_name_or_id: str, params: Optional[Dict[str, str]] = None):
         params = {**params} if params else {}
         return await self._req(f"/v0/pipes/{pipe_name_or_id}/sink?{urlencode(params)}", method="POST")
 
+    async def pipe_unlink_materialized(self, pipe_name: str, node_id: str):
+        return await self._req(f"/v0/pipes/{pipe_name}/nodes/{node_id}/materialization", method="DELETE")
+
     async def query(self, sql: str, pipeline: Optional[str] = None):
         params = {}
         if pipeline:
             params = {"pipeline": pipeline}
         params.update({"release_replacements": "true"})
 
         if len(sql) > TinyB.MAX_GET_LENGTH:
```

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/config.py` & `tinybird-cli-3.9.1.dev6/tinybird/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/connectors.py` & `tinybird-cli-3.9.1.dev6/tinybird/connectors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/context.py` & `tinybird-cli-3.9.1.dev6/tinybird/context.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/datafile.py` & `tinybird-cli-3.9.1.dev6/tinybird/datafile.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/datatypes.py` & `tinybird-cli-3.9.1.dev6/tinybird/datatypes.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/feedback_manager.py` & `tinybird-cli-3.9.1.dev6/tinybird/feedback_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -639,14 +639,17 @@
     info_data_pushed = info_message("** Data pushed to {datasource}")
     info_materialized_datasource_created = info_message(
         "** Materialized pipe '{pipe}' created the Data Source '{datasource}'"
     )
     info_materialized_datasource_used = info_message(
         "** Materialized pipe '{pipe}' using the Data Source '{datasource}'"
     )
+    info_materialized_unlinking_pipe = info_message("** Unlinking materialized pipe {pipe}")
+    info_materialized_unlinking_pipe_not_found = info_message("** {pipe} not found")
+    info_materialized_dry_unlinking_pipe = info_message("** [DRY RUN] Unlinking materialized pipe {pipe}")
     info_copy_datasource_created = info_message("** Copy pipe '{pipe}' created the Data Source '{datasource}'")
     info_copy_datasource_used = info_message("** Copy pipe '{pipe}' using the Data Source '{datasource}'")
     info_no_pipes_stats = info_message("** No pipe stats")
     info_starting_export_process = info_message("** \N{Chicken} starting export process from {connector}")
     info_ask_for_datasource_confirmation = info_message("** Please type the Data Source name to be replaced")
     info_datasource_doesnt_match = info_message("** The description or schema of '{datasource}' has changed.")
     info_custom_deployment = info_message(
```

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/git_settings.py` & `tinybird-cli-3.9.1.dev6/tinybird/git_settings.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/sql.py` & `tinybird-cli-3.9.1.dev6/tinybird/sql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/sql_template.py` & `tinybird-cli-3.9.1.dev6/tinybird/sql_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/sql_template_fmt.py` & `tinybird-cli-3.9.1.dev6/tinybird/sql_template_fmt.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/sql_toolset.py` & `tinybird-cli-3.9.1.dev6/tinybird/sql_toolset.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/syncasync.py` & `tinybird-cli-3.9.1.dev6/tinybird/syncasync.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/auth.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/auth.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/branch.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/branch.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/cicd.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/cicd.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/cli.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/common.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/common.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/config.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/connection.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/connection.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/datasource.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/datasource.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/exceptions.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/job.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/job.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/pipe.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/pipe.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/regions.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/regions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/telemetry.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/telemetry.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/test.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/test.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/tinyunit/tinyunit.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/tinyunit/tinyunit.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/token.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/token.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/workspace.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/workspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from typing import Optional
 
 import click
 from click import Context
 
 from tinybird.client import CanNotBeDeletedException, DoesNotExistException, TinyB
+from tinybird.datafile import PipeTypes
 from tinybird.feedback_manager import FeedbackManager
 from tinybird.tb_cli_modules.cli import cli
 from tinybird.tb_cli_modules.common import (
     _get_config,
     _get_workspace_plan_name,
     ask_for_user_token,
     coro,
@@ -133,16 +134,35 @@
                     ]
                 )
             break
 
     echo_safe_humanfriendly_tables_format_smart_table(table, column_names=columns)
 
     if yes or click.confirm(FeedbackManager.warning_confirm_clear_workspace()):
-        pipes = await client.pipes(dependencies=False, node_attrs="name", attrs="name")
+        pipes = await client.pipes(dependencies=False, node_attrs="id,name,materialized", attrs="name,type")
         pipe_names = [pipe["name"] for pipe in pipes]
+
+        for pipe in pipes:
+            if pipe["type"] == PipeTypes.MATERIALIZED:
+                if not dry_run:
+                    node_id = None
+                    for node in pipe["nodes"]:
+                        if "materialized" in node and node["materialized"] is not None:
+                            node_id = node["id"]
+                            break
+
+                    if node_id:
+                        click.echo(FeedbackManager.info_materialized_unlinking_pipe(pipe=pipe["name"]))
+                        try:
+                            await client.pipe_unlink_materialized(pipe["name"], node_id)
+                        except DoesNotExistException:
+                            click.echo(FeedbackManager.info_materialized_unlinking_pipe_not_found(pipe=pipe["name"]))
+                else:
+                    click.echo(FeedbackManager.info_materialized_dry_unlinking_pipe(pipe=pipe["name"]))
+
         for pipe_name in pipe_names:
             if not dry_run:
                 click.echo(FeedbackManager.info_removing_pipe(pipe=pipe_name))
                 try:
                     await client.pipe_delete(pipe_name)
                 except DoesNotExistException:
                     click.echo(FeedbackManager.info_removing_pipe_not_found(pipe=pipe_name))
```

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tb_cli_modules/workspace_members.py` & `tinybird-cli-3.9.1.dev6/tinybird/tb_cli_modules/workspace_members.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird/tornado_template.py` & `tinybird-cli-3.9.1.dev6/tinybird/tornado_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/PKG-INFO` & `tinybird-cli-3.9.1.dev6/tinybird_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.9.1.dev5
+Version: 3.9.1.dev6
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -14,20 +14,24 @@
 =============
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 ----------
 
+3.9.1.dev6
+************
+
+- `Added` Support for unlink materialized pipes doing `tb workspace clear`
+
 3.9.1.dev5
 ************
 
 - `Added` support for adding multiple tokens when pushing a `.datasource` file
 
-
 3.9.1.dev4
 ************
 
 - `Fixed` s3 iamrole connection creation will not fail when `pbcopy` dependency is not available
 
 3.9.1.dev3
 ************
```

### Comparing `tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/SOURCES.txt` & `tinybird-cli-3.9.1.dev6/tinybird_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.9.1.dev5/tinybird_cli.egg-info/requires.txt` & `tinybird-cli-3.9.1.dev6/tinybird_cli.egg-info/requires.txt`

 * *Files identical despite different names*

