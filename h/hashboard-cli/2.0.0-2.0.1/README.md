# Comparing `tmp/hashboard_cli-2.0.0.tar.gz` & `tmp/hashboard_cli-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashboard_cli-2.0.0.tar", last modified: Tue May  7 17:05:21 2024, max compression
+gzip compressed data, was "hashboard_cli-2.0.1.tar", last modified: Fri May 24 15:44:15 2024, max compression
```

## Comparing `hashboard_cli-2.0.0.tar` & `hashboard_cli-2.0.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-07 17:05:21.875799 hashboard_cli-2.0.0/
--rw-r--r--   0 anixon     (501) staff       (20)    11357 2022-12-17 00:47:55.000000 hashboard_cli-2.0.0/LICENSE
--rw-r--r--   0 anixon     (501) staff       (20)      924 2024-05-07 17:05:21.875698 hashboard_cli-2.0.0/PKG-INFO
--rw-r--r--   0 anixon     (501) staff       (20)      141 2023-09-29 18:00:46.000000 hashboard_cli-2.0.0/README.md
--rw-r--r--   0 anixon     (501) staff       (20)      104 2023-08-30 15:47:31.000000 hashboard_cli-2.0.0/pyproject.toml
--rw-r--r--   0 anixon     (501) staff       (20)      878 2024-05-07 17:05:21.876123 hashboard_cli-2.0.0/setup.cfg
--rw-r--r--   0 anixon     (501) staff       (20)       38 2022-12-17 00:47:55.000000 hashboard_cli-2.0.0/setup.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-07 17:05:21.866871 hashboard_cli-2.0.0/src/
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-07 17:05:21.869324 hashboard_cli-2.0.0/src/hashboard/
--rw-r--r--   0 anixon     (501) staff       (20)       18 2024-05-07 17:04:42.000000 hashboard_cli-2.0.0/src/hashboard/__init__.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-07 17:05:21.869535 hashboard_cli-2.0.0/src/hashboard/api/
--rw-r--r--   0 anixon     (501) staff       (20)    15394 2024-04-30 14:54:57.000000 hashboard_cli-2.0.0/src/hashboard/api/__init__.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-07 17:05:21.870350 hashboard_cli-2.0.0/src/hashboard/api/access_keys/
--rw-r--r--   0 anixon     (501) staff       (20)        0 2023-09-19 18:12:31.000000 hashboard_cli-2.0.0/src/hashboard/api/access_keys/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)     4227 2023-09-19 18:12:31.000000 hashboard_cli-2.0.0/src/hashboard/api/access_keys/browser_auth.py
--rw-r--r--   0 anixon     (501) staff       (20)     4409 2024-03-18 20:02:56.000000 hashboard_cli-2.0.0/src/hashboard/api/access_keys/existing_user.py
--rw-r--r--   0 anixon     (501) staff       (20)     2143 2024-03-18 20:02:56.000000 hashboard_cli-2.0.0/src/hashboard/api/access_keys/utils.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-07 17:05:21.871145 hashboard_cli-2.0.0/src/hashboard/api/analytics/
--rw-r--r--   0 anixon     (501) staff       (20)      900 2023-09-29 18:00:46.000000 hashboard_cli-2.0.0/src/hashboard/api/analytics/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)     4003 2023-09-29 18:00:46.000000 hashboard_cli-2.0.0/src/hashboard/api/analytics/cli_with_tracking.py
--rw-r--r--   0 anixon     (501) staff       (20)       20 2024-04-16 20:21:42.000000 hashboard_cli-2.0.0/src/hashboard/api/analytics/events.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-07 17:05:21.871804 hashboard_cli-2.0.0/src/hashboard/api/datasource/
--rw-r--r--   0 anixon     (501) staff       (20)        0 2024-04-22 20:51:24.000000 hashboard_cli-2.0.0/src/hashboard/api/datasource/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)     9994 2024-04-26 20:17:46.000000 hashboard_cli-2.0.0/src/hashboard/api/datasource/datasource_cli.py
--rw-r--r--   0 anixon     (501) staff       (20)    10025 2024-04-26 20:17:46.000000 hashboard_cli-2.0.0/src/hashboard/api/datasource/utils.py
--rw-r--r--   0 anixon     (501) staff       (20)    40037 2024-05-07 15:44:47.000000 hashboard_cli-2.0.0/src/hashboard/cli.py
--rw-r--r--   0 anixon     (501) staff       (20)      346 2023-09-19 18:12:31.000000 hashboard_cli-2.0.0/src/hashboard/constants.py
--rw-r--r--   0 anixon     (501) staff       (20)     1744 2023-09-19 18:12:31.000000 hashboard_cli-2.0.0/src/hashboard/credentials.py
--rw-r--r--   0 anixon     (501) staff       (20)     3973 2024-05-06 20:46:07.000000 hashboard_cli-2.0.0/src/hashboard/filesystem.py
--rw-r--r--   0 anixon     (501) staff       (20)      597 2023-09-29 18:00:46.000000 hashboard_cli-2.0.0/src/hashboard/session.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-07 17:05:21.873293 hashboard_cli-2.0.0/src/hashboard/utils/
--rw-r--r--   0 anixon     (501) staff       (20)        0 2023-09-19 18:12:31.000000 hashboard_cli-2.0.0/src/hashboard/utils/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)      665 2023-09-19 18:12:31.000000 hashboard_cli-2.0.0/src/hashboard/utils/cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     1977 2024-04-16 20:21:42.000000 hashboard_cli-2.0.0/src/hashboard/utils/config.py
--rw-r--r--   0 anixon     (501) staff       (20)      230 2023-09-19 18:12:31.000000 hashboard_cli-2.0.0/src/hashboard/utils/env.py
--rw-r--r--   0 anixon     (501) staff       (20)     2922 2023-11-06 18:51:09.000000 hashboard_cli-2.0.0/src/hashboard/utils/grn.py
--rw-r--r--   0 anixon     (501) staff       (20)      941 2023-09-19 18:12:31.000000 hashboard_cli-2.0.0/src/hashboard/utils/input_validation.py
--rw-r--r--   0 anixon     (501) staff       (20)     1468 2023-09-19 18:12:31.000000 hashboard_cli-2.0.0/src/hashboard/utils/resource.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-07 17:05:21.875178 hashboard_cli-2.0.0/src/hashboard_cli.egg-info/
--rw-r--r--   0 anixon     (501) staff       (20)      924 2024-05-07 17:05:21.000000 hashboard_cli-2.0.0/src/hashboard_cli.egg-info/PKG-INFO
--rw-r--r--   0 anixon     (501) staff       (20)     1224 2024-05-07 17:05:21.000000 hashboard_cli-2.0.0/src/hashboard_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anixon     (501) staff       (20)        1 2024-05-07 17:05:21.000000 hashboard_cli-2.0.0/src/hashboard_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anixon     (501) staff       (20)       42 2024-05-07 17:05:21.000000 hashboard_cli-2.0.0/src/hashboard_cli.egg-info/entry_points.txt
--rw-r--r--   0 anixon     (501) staff       (20)      138 2024-05-07 17:05:21.000000 hashboard_cli-2.0.0/src/hashboard_cli.egg-info/requires.txt
--rw-r--r--   0 anixon     (501) staff       (20)       10 2024-05-07 17:05:21.000000 hashboard_cli-2.0.0/src/hashboard_cli.egg-info/top_level.txt
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2024-05-07 17:05:21.874827 hashboard_cli-2.0.0/tests/
--rw-r--r--   0 anixon     (501) staff       (20)      310 2023-09-19 18:12:31.000000 hashboard_cli-2.0.0/tests/test_cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     1534 2023-09-19 18:12:31.000000 hashboard_cli-2.0.0/tests/test_credentials.py
--rw-r--r--   0 anixon     (501) staff       (20)     4245 2024-05-06 20:46:07.000000 hashboard_cli-2.0.0/tests/test_filesystem.py
--rw-r--r--   0 anixon     (501) staff       (20)      668 2023-09-19 18:12:31.000000 hashboard_cli-2.0.0/tests/test_hashboard_api.py
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-05-24 15:44:15.280272 hashboard_cli-2.0.1/
+-rw-r--r--   0 dse        (501) staff       (20)    11357 2021-08-09 13:38:38.000000 hashboard_cli-2.0.1/LICENSE
+-rw-r--r--   0 dse        (501) staff       (20)      924 2024-05-24 15:44:15.280207 hashboard_cli-2.0.1/PKG-INFO
+-rw-r--r--   0 dse        (501) staff       (20)      141 2023-12-27 16:23:17.000000 hashboard_cli-2.0.1/README.md
+-rw-r--r--   0 dse        (501) staff       (20)      104 2023-08-24 19:56:44.000000 hashboard_cli-2.0.1/pyproject.toml
+-rw-r--r--   0 dse        (501) staff       (20)      878 2024-05-24 15:44:15.280852 hashboard_cli-2.0.1/setup.cfg
+-rw-r--r--   0 dse        (501) staff       (20)       38 2021-09-03 21:01:45.000000 hashboard_cli-2.0.1/setup.py
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-05-24 15:44:15.267099 hashboard_cli-2.0.1/src/
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-05-24 15:44:15.271611 hashboard_cli-2.0.1/src/hashboard/
+-rw-r--r--   0 dse        (501) staff       (20)       18 2024-05-24 15:39:36.000000 hashboard_cli-2.0.1/src/hashboard/__init__.py
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-05-24 15:44:15.271930 hashboard_cli-2.0.1/src/hashboard/api/
+-rw-r--r--   0 dse        (501) staff       (20)    15394 2024-05-24 14:07:12.000000 hashboard_cli-2.0.1/src/hashboard/api/__init__.py
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-05-24 15:44:15.273925 hashboard_cli-2.0.1/src/hashboard/api/access_keys/
+-rw-r--r--   0 dse        (501) staff       (20)        0 2023-09-07 12:15:00.000000 hashboard_cli-2.0.1/src/hashboard/api/access_keys/__init__.py
+-rw-r--r--   0 dse        (501) staff       (20)     4227 2023-09-14 16:54:13.000000 hashboard_cli-2.0.1/src/hashboard/api/access_keys/browser_auth.py
+-rw-r--r--   0 dse        (501) staff       (20)     4409 2024-01-26 20:40:40.000000 hashboard_cli-2.0.1/src/hashboard/api/access_keys/existing_user.py
+-rw-r--r--   0 dse        (501) staff       (20)     2143 2024-01-26 20:40:40.000000 hashboard_cli-2.0.1/src/hashboard/api/access_keys/utils.py
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-05-24 15:44:15.275117 hashboard_cli-2.0.1/src/hashboard/api/analytics/
+-rw-r--r--   0 dse        (501) staff       (20)      900 2023-12-27 16:23:17.000000 hashboard_cli-2.0.1/src/hashboard/api/analytics/__init__.py
+-rw-r--r--   0 dse        (501) staff       (20)     4003 2023-12-27 16:23:17.000000 hashboard_cli-2.0.1/src/hashboard/api/analytics/cli_with_tracking.py
+-rw-r--r--   0 dse        (501) staff       (20)       20 2024-05-24 14:07:12.000000 hashboard_cli-2.0.1/src/hashboard/api/analytics/events.py
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-05-24 15:44:15.275780 hashboard_cli-2.0.1/src/hashboard/api/datasource/
+-rw-r--r--   0 dse        (501) staff       (20)        0 2024-05-24 14:07:12.000000 hashboard_cli-2.0.1/src/hashboard/api/datasource/__init__.py
+-rw-r--r--   0 dse        (501) staff       (20)     9994 2024-05-24 14:07:12.000000 hashboard_cli-2.0.1/src/hashboard/api/datasource/datasource_cli.py
+-rw-r--r--   0 dse        (501) staff       (20)    10025 2024-05-24 14:07:12.000000 hashboard_cli-2.0.1/src/hashboard/api/datasource/utils.py
+-rw-r--r--   0 dse        (501) staff       (20)    40114 2024-05-24 15:39:36.000000 hashboard_cli-2.0.1/src/hashboard/cli.py
+-rw-r--r--   0 dse        (501) staff       (20)      346 2023-09-14 16:54:13.000000 hashboard_cli-2.0.1/src/hashboard/constants.py
+-rw-r--r--   0 dse        (501) staff       (20)     1744 2023-09-14 16:54:13.000000 hashboard_cli-2.0.1/src/hashboard/credentials.py
+-rw-r--r--   0 dse        (501) staff       (20)     3973 2024-05-24 14:07:12.000000 hashboard_cli-2.0.1/src/hashboard/filesystem.py
+-rw-r--r--   0 dse        (501) staff       (20)      597 2023-12-27 16:23:17.000000 hashboard_cli-2.0.1/src/hashboard/session.py
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-05-24 15:44:15.277549 hashboard_cli-2.0.1/src/hashboard/utils/
+-rw-r--r--   0 dse        (501) staff       (20)        0 2023-09-07 12:15:00.000000 hashboard_cli-2.0.1/src/hashboard/utils/__init__.py
+-rw-r--r--   0 dse        (501) staff       (20)      665 2023-09-07 12:15:00.000000 hashboard_cli-2.0.1/src/hashboard/utils/cli.py
+-rw-r--r--   0 dse        (501) staff       (20)     1977 2024-05-24 14:07:12.000000 hashboard_cli-2.0.1/src/hashboard/utils/config.py
+-rw-r--r--   0 dse        (501) staff       (20)      230 2023-09-07 12:15:00.000000 hashboard_cli-2.0.1/src/hashboard/utils/env.py
+-rw-r--r--   0 dse        (501) staff       (20)     2922 2023-12-27 16:23:17.000000 hashboard_cli-2.0.1/src/hashboard/utils/grn.py
+-rw-r--r--   0 dse        (501) staff       (20)      941 2023-09-07 12:15:00.000000 hashboard_cli-2.0.1/src/hashboard/utils/input_validation.py
+-rw-r--r--   0 dse        (501) staff       (20)     1468 2023-09-07 12:15:00.000000 hashboard_cli-2.0.1/src/hashboard/utils/resource.py
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-05-24 15:44:15.279700 hashboard_cli-2.0.1/src/hashboard_cli.egg-info/
+-rw-r--r--   0 dse        (501) staff       (20)      924 2024-05-24 15:44:15.000000 hashboard_cli-2.0.1/src/hashboard_cli.egg-info/PKG-INFO
+-rw-r--r--   0 dse        (501) staff       (20)     1224 2024-05-24 15:44:15.000000 hashboard_cli-2.0.1/src/hashboard_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 dse        (501) staff       (20)        1 2024-05-24 15:44:15.000000 hashboard_cli-2.0.1/src/hashboard_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 dse        (501) staff       (20)       42 2024-05-24 15:44:15.000000 hashboard_cli-2.0.1/src/hashboard_cli.egg-info/entry_points.txt
+-rw-r--r--   0 dse        (501) staff       (20)      138 2024-05-24 15:44:15.000000 hashboard_cli-2.0.1/src/hashboard_cli.egg-info/requires.txt
+-rw-r--r--   0 dse        (501) staff       (20)       10 2024-05-24 15:44:15.000000 hashboard_cli-2.0.1/src/hashboard_cli.egg-info/top_level.txt
+drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-05-24 15:44:15.279249 hashboard_cli-2.0.1/tests/
+-rw-r--r--   0 dse        (501) staff       (20)      310 2023-09-07 12:15:00.000000 hashboard_cli-2.0.1/tests/test_cli.py
+-rw-r--r--   0 dse        (501) staff       (20)     1534 2023-09-14 16:54:13.000000 hashboard_cli-2.0.1/tests/test_credentials.py
+-rw-r--r--   0 dse        (501) staff       (20)     4245 2024-05-24 14:07:12.000000 hashboard_cli-2.0.1/tests/test_filesystem.py
+-rw-r--r--   0 dse        (501) staff       (20)      668 2023-09-07 12:15:00.000000 hashboard_cli-2.0.1/tests/test_hashboard_api.py
```

### Comparing `hashboard_cli-2.0.0/LICENSE` & `hashboard_cli-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/PKG-INFO` & `hashboard_cli-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashboard-cli
-Version: 2.0.0
+Version: 2.0.1
 Summary: Command-line tools for interacting with Hashboard
 Home-page: https://hashboard.com/
 Author: Dan Eisenberg
 Author-email: dan@hashboard.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashboard_cli-2.0.0/setup.cfg` & `hashboard_cli-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/api/__init__.py` & `hashboard_cli-2.0.1/src/hashboard/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/api/access_keys/browser_auth.py` & `hashboard_cli-2.0.1/src/hashboard/api/access_keys/browser_auth.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/api/access_keys/existing_user.py` & `hashboard_cli-2.0.1/src/hashboard/api/access_keys/existing_user.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/api/access_keys/utils.py` & `hashboard_cli-2.0.1/src/hashboard/api/access_keys/utils.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/api/analytics/__init__.py` & `hashboard_cli-2.0.1/src/hashboard/api/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/api/analytics/cli_with_tracking.py` & `hashboard_cli-2.0.1/src/hashboard/api/analytics/cli_with_tracking.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/api/datasource/datasource_cli.py` & `hashboard_cli-2.0.1/src/hashboard/api/datasource/datasource_cli.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/api/datasource/utils.py` & `hashboard_cli-2.0.1/src/hashboard/api/datasource/utils.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/cli.py` & `hashboard_cli-2.0.1/src/hashboard/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,20 @@
     build_id = build_results["data"]["createAsyncBuild"]
     build_results = _poll_for_build_status(build_id)
 
     _echo_async_build_results(build_results)
 
 
 # TODO: Update to follow a build -> apply pattern
-@cli.command("deploy", cls=CommandWithTracking)
+@cli.command("deploy",
+    cls=CommandWithTracking,
+    context_settings=dict(
+        ignore_unknown_options=True,
+    ),
+)
 @allow_dangerous_empty_build_option
 @git_revision_option
 @git_path_option
 @dbt_manifest_option
 @run_dbt_parse_option
 @local_path_argument
 @dbt_parse_flags_argument
```

### Comparing `hashboard_cli-2.0.0/src/hashboard/credentials.py` & `hashboard_cli-2.0.1/src/hashboard/credentials.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/filesystem.py` & `hashboard_cli-2.0.1/src/hashboard/filesystem.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/session.py` & `hashboard_cli-2.0.1/src/hashboard/session.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/utils/cli.py` & `hashboard_cli-2.0.1/src/hashboard/utils/cli.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/utils/config.py` & `hashboard_cli-2.0.1/src/hashboard/utils/config.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/utils/grn.py` & `hashboard_cli-2.0.1/src/hashboard/utils/grn.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/utils/input_validation.py` & `hashboard_cli-2.0.1/src/hashboard/utils/input_validation.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard/utils/resource.py` & `hashboard_cli-2.0.1/src/hashboard/utils/resource.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/src/hashboard_cli.egg-info/PKG-INFO` & `hashboard_cli-2.0.1/src/hashboard_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashboard-cli
-Version: 2.0.0
+Version: 2.0.1
 Summary: Command-line tools for interacting with Hashboard
 Home-page: https://hashboard.com/
 Author: Dan Eisenberg
 Author-email: dan@hashboard.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hashboard_cli-2.0.0/src/hashboard_cli.egg-info/SOURCES.txt` & `hashboard_cli-2.0.1/src/hashboard_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/tests/test_credentials.py` & `hashboard_cli-2.0.1/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/tests/test_filesystem.py` & `hashboard_cli-2.0.1/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `hashboard_cli-2.0.0/tests/test_hashboard_api.py` & `hashboard_cli-2.0.1/tests/test_hashboard_api.py`

 * *Files identical despite different names*

