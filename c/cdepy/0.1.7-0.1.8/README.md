# Comparing `tmp/cdepy-0.1.7.tar.gz` & `tmp/cdepy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdepy-0.1.7.tar", last modified: Tue Feb 13 18:52:17 2024, max compression
+gzip compressed data, was "cdepy-0.1.8.tar", last modified: Thu May 23 02:46:50 2024, max compression
```

## Comparing `cdepy-0.1.7.tar` & `cdepy-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 pauldefusco   (502) staff       (20)        0 2024-02-13 18:52:17.209790 cdepy-0.1.7/
--rw-r--r--   0 pauldefusco   (502) staff       (20)     1070 2024-02-13 18:32:02.000000 cdepy-0.1.7/LICENSE
--rw-r--r--   0 pauldefusco   (502) staff       (20)       34 2023-10-11 18:06:12.000000 cdepy-0.1.7/MANIFEST.in
--rw-r--r--   0 pauldefusco   (502) staff       (20)     4152 2024-02-13 18:52:17.209622 cdepy-0.1.7/PKG-INFO
--rw-r--r--   0 pauldefusco   (502) staff       (20)     3592 2024-02-13 18:30:28.000000 cdepy-0.1.7/README.md
-drwxr-xr-x   0 pauldefusco   (502) staff       (20)        0 2024-02-13 18:52:17.208576 cdepy-0.1.7/cdepy/
--rw-r--r--   0 pauldefusco   (502) staff       (20)        0 2023-10-11 17:22:42.000000 cdepy-0.1.7/cdepy/__init__.py
--rw-r--r--   0 pauldefusco   (502) staff       (20)     1173 2024-02-13 17:13:33.000000 cdepy-0.1.7/cdepy/cdeconnection.py
--rw-r--r--   0 pauldefusco   (502) staff       (20)     5232 2024-02-13 17:13:32.000000 cdepy-0.1.7/cdepy/cdejob.py
--rw-r--r--   0 pauldefusco   (502) staff       (20)    15142 2024-02-13 17:13:31.000000 cdepy-0.1.7/cdepy/cdemanager.py
--rw-r--r--   0 pauldefusco   (502) staff       (20)     1663 2024-02-13 17:13:29.000000 cdepy-0.1.7/cdepy/cderesource.py
--rw-r--r--   0 pauldefusco   (502) staff       (20)     2116 2024-02-13 18:48:17.000000 cdepy-0.1.7/cdepy/utils.py
-drwxr-xr-x   0 pauldefusco   (502) staff       (20)        0 2024-02-13 18:52:17.209369 cdepy-0.1.7/cdepy.egg-info/
--rw-r--r--   0 pauldefusco   (502) staff       (20)     4152 2024-02-13 18:52:16.000000 cdepy-0.1.7/cdepy.egg-info/PKG-INFO
--rw-r--r--   0 pauldefusco   (502) staff       (20)      295 2024-02-13 18:52:17.000000 cdepy-0.1.7/cdepy.egg-info/SOURCES.txt
--rw-r--r--   0 pauldefusco   (502) staff       (20)        1 2024-02-13 18:52:16.000000 cdepy-0.1.7/cdepy.egg-info/dependency_links.txt
--rw-r--r--   0 pauldefusco   (502) staff       (20)       60 2024-02-13 18:52:17.000000 cdepy-0.1.7/cdepy.egg-info/requires.txt
--rw-r--r--   0 pauldefusco   (502) staff       (20)        6 2024-02-13 18:52:17.000000 cdepy-0.1.7/cdepy.egg-info/top_level.txt
--rw-r--r--   0 pauldefusco   (502) staff       (20)       38 2024-02-13 18:52:17.209842 cdepy-0.1.7/setup.cfg
--rw-r--r--   0 pauldefusco   (502) staff       (20)      951 2024-02-13 18:49:37.000000 cdepy-0.1.7/setup.py
+drwxr-xr-x   0 pauldefusco   (502) staff       (20)        0 2024-05-23 02:46:50.908887 cdepy-0.1.8/
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     1070 2024-02-13 18:32:02.000000 cdepy-0.1.8/LICENSE
+-rw-r--r--   0 pauldefusco   (502) staff       (20)       34 2023-10-11 18:06:12.000000 cdepy-0.1.8/MANIFEST.in
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     6565 2024-05-23 02:46:50.908706 cdepy-0.1.8/PKG-INFO
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     6005 2024-05-23 02:46:06.000000 cdepy-0.1.8/README.md
+drwxr-xr-x   0 pauldefusco   (502) staff       (20)        0 2024-05-23 02:46:50.907290 cdepy-0.1.8/cdepy/
+-rw-r--r--   0 pauldefusco   (502) staff       (20)        0 2023-10-11 17:22:42.000000 cdepy-0.1.8/cdepy/__init__.py
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     6014 2024-05-23 02:35:46.000000 cdepy-0.1.8/cdepy/cdeairflowpython.py
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     1173 2024-02-13 17:13:33.000000 cdepy-0.1.8/cdepy/cdeconnection.py
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     5232 2024-02-13 17:13:32.000000 cdepy-0.1.8/cdepy/cdejob.py
+-rw-r--r--   0 pauldefusco   (502) staff       (20)    15142 2024-02-13 17:13:31.000000 cdepy-0.1.8/cdepy/cdemanager.py
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     1663 2024-02-13 17:13:29.000000 cdepy-0.1.8/cdepy/cderesource.py
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     2116 2024-02-13 18:48:17.000000 cdepy-0.1.8/cdepy/utils.py
+drwxr-xr-x   0 pauldefusco   (502) staff       (20)        0 2024-05-23 02:46:50.908441 cdepy-0.1.8/cdepy.egg-info/
+-rw-r--r--   0 pauldefusco   (502) staff       (20)     6565 2024-05-23 02:46:50.000000 cdepy-0.1.8/cdepy.egg-info/PKG-INFO
+-rw-r--r--   0 pauldefusco   (502) staff       (20)      321 2024-05-23 02:46:50.000000 cdepy-0.1.8/cdepy.egg-info/SOURCES.txt
+-rw-r--r--   0 pauldefusco   (502) staff       (20)        1 2024-05-23 02:46:50.000000 cdepy-0.1.8/cdepy.egg-info/dependency_links.txt
+-rw-r--r--   0 pauldefusco   (502) staff       (20)       60 2024-05-23 02:46:50.000000 cdepy-0.1.8/cdepy.egg-info/requires.txt
+-rw-r--r--   0 pauldefusco   (502) staff       (20)        6 2024-05-23 02:46:50.000000 cdepy-0.1.8/cdepy.egg-info/top_level.txt
+-rw-r--r--   0 pauldefusco   (502) staff       (20)       38 2024-05-23 02:46:50.908947 cdepy-0.1.8/setup.cfg
+-rw-r--r--   0 pauldefusco   (502) staff       (20)      951 2024-05-23 02:36:09.000000 cdepy-0.1.8/setup.py
```

### Comparing `cdepy-0.1.7/LICENSE` & `cdepy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cdepy-0.1.7/PKG-INFO` & `cdepy-0.1.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: cdepy
-Version: 0.1.7
-Summary: A Python Package for interacting with Cloudera Data Engineering Clusters
-Home-page: https://github.com/pdefusco/cdepy
-Author: Paul de Fusco
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cdepy Package
 
 cdepy is a package for interacting with ***Cludera Data Engineering Virtual Clusters***.
 
 You can find out more about Cloudera Data Engineering in the [Cloudera Documentation](https://docs.cloudera.com/data-engineering/cloud/index.html).
 
 ## Usage
@@ -33,14 +16,16 @@
 
 - CDE Resources: create resources of type Files and Python-Environment
 - CDE Jobs: create jobs of type Airflow and Spark
 - Job Observability: monitor job status
 
 ## Examples
 
+### BASICS
+
 ```
 from cdepy import cdeconnection
 from cdepy import cdejob
 from cdepy import cdemanager
 from cdepy import cderesource
 ```
 
@@ -172,8 +157,104 @@
 
 ```
 CDE_RESOURCE_NAME = "myFilesCdeResource"
 
 myCdeClusterManager.deleteResource(CDE_RESOURCE_NAME)
 ```
 
+### CDE AIRFLOW PYTHON ENVIRONMENTS
+
+NB: There is only one Airflow Python Environment per CDE Virtual Cluster.
+
+```
+from cdepy import cdeconnection
+from cdepy import cdeairflowpython
+import os
+import json
+```
+
+#### Connect via CdeConnection Object
+
+```
+JOBS_API_URL = "<myJobsAPIurl>"
+WORKLOAD_USER = "<myusername>"
+WORKLOAD_PASSWORD = "<mypwd>"
+
+myCdeConnection = cdeconnection.CdeConnection(JOBS_API_URL, WORKLOAD_USER, WORKLOAD_PASSWORD)
+
+myCdeConnection.setToken()
+```
+
+#### Use CdeAirflowPythonEnv object to manage Airflow Python Environments
+
+```
+myAirflowPythonEnvManager = cdeairflowpython.CdeAirflowPythonEnv(myCdeConnection)
+```
+
+#### Create a Maintenance Session in order to perform any Airflow Python Environments related actions
+
+```
+myAirflowPythonEnvManager.createMaintenanceSession()
+```
 
+#### First Create a pip repository
+
+```
+myAirflowPythonEnvManager.createPipRepository()
+```
+
+#### Check on Status of Maintenance Session
+
+```
+myAirflowPythonEnvManager.checkAirflowPythonEnvStatus()
+###### STATUS SHOULD BE {"status":"pip-repos-defined"}
+```
+
+#### Load requirements.txt file
+
+```
+pathToRequirementsTxt = "/examples/requirements.txt"
+myAirflowPythonEnvManager.buildAirflowPythonEnv(pathToRequirementsTxt)
+###### requirements.txt file must be customized
+
+myAirflowPythonEnvManager.checkAirflowPythonEnvStatus()
+###### RESPONSE STATUS SHOULD BE {"status":"building"}
+###### AFTER 2 MINUTES REPEAT THE REQUEST. RESPONSE STATUS SHOULD EVENTUALLY BE {"status":"built"}
+```
+
+#### Validate status of Python environment
+
+```
+myAirflowPythonEnvManager.getAirflowPythonEnvironmentDetails()
+```
+
+#### Explore Maintenace Session logs
+
+```
+myAirflowPythonEnvManager.viewMaintenanceSessionLogs()
+```
+
+#### Activate the Python environment
+
+```
+myAirflowPythonEnvManager.activateAirflowPythonEnv()
+```
+
+#### Check on Python environment build status
+
+```
+myAirflowPythonEnvManager.checkAirflowPythonEnvStatus()
+###### AT FIRST RESPONSE STATUS SHOULD BE {"status":"activating"}
+###### AFTER A COUPLE OF MINUTES THE MAINTENANCE SESSION WILL AUTOMATICALLY END. THIS MEANS THE AIRFLOW PYTHON ENV HAS ACTIVATED.
+```
+
+#### Optional: Create a new session and then delete the Python environment
+
+```
+myAirflowPythonEnvManager.deleteAirflowPythonEnv()
+```
+
+#### Optional: End the Maintenance Session once you have deleted the Python environment
+
+```
+myAirflowPythonEnvManager.deleteMaintenanceSession()
+```
```

### Comparing `cdepy-0.1.7/cdepy/cdeconnection.py` & `cdepy-0.1.8/cdepy/cdeconnection.py`

 * *Files identical despite different names*

### Comparing `cdepy-0.1.7/cdepy/cdejob.py` & `cdepy-0.1.8/cdepy/cdejob.py`

 * *Files identical despite different names*

### Comparing `cdepy-0.1.7/cdepy/cdemanager.py` & `cdepy-0.1.8/cdepy/cdemanager.py`

 * *Files identical despite different names*

### Comparing `cdepy-0.1.7/cdepy/cderesource.py` & `cdepy-0.1.8/cdepy/cderesource.py`

 * *Files identical despite different names*

### Comparing `cdepy-0.1.7/cdepy/utils.py` & `cdepy-0.1.8/cdepy/utils.py`

 * *Files identical despite different names*

### Comparing `cdepy-0.1.7/setup.py` & `cdepy-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup(
     author="Paul de Fusco",
     description="A Python Package for interacting with Cloudera Data Engineering Clusters",
     long_description=read_file("README.md"),
     long_description_content_type="text/markdown",
     name="cdepy",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(include=["cdepy", "cdepy.*"]),
     install_requires=["pyparsing==3.0.9", "requests-toolbelt==1.0.0", "xmltodict==0.13.0"],
     python_requires=">=2.7",
     license="MIT",
     url = "https://github.com/pdefusco/cdepy",
     classifiers=[
         'Development Status :: 4 - Beta',
```

