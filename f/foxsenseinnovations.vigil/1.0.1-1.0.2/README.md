# Comparing `tmp/foxsenseinnovations.vigil-1.0.1.tar.gz` & `tmp/foxsenseinnovations_vigil-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxsenseinnovations.vigil-1.0.1.tar", last modified: Wed Apr 17 12:51:36 2024, max compression
+gzip compressed data, was "foxsenseinnovations_vigil-1.0.2.tar", last modified: Fri May 24 06:18:41 2024, max compression
```

## Comparing `foxsenseinnovations.vigil-1.0.1.tar` & `foxsenseinnovations_vigil-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.233585 foxsenseinnovations.vigil-1.0.1/
--rw-rw-rw-   0        0        0       17 2024-04-02 09:29:10.000000 foxsenseinnovations.vigil-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7587 2024-04-17 12:51:36.228801 foxsenseinnovations.vigil-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7020 2024-04-17 10:21:49.000000 foxsenseinnovations.vigil-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 12:51:35.690280 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/
--rw-rw-rw-   0        0        0       33 2024-02-09 02:43:40.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.045090 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/
--rw-rw-rw-   0        0        0      444 2024-02-09 02:43:13.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/__init__.py
--rw-rw-rw-   0        0        0     4758 2024-04-02 06:15:26.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/api_manager_django.py
--rw-rw-rw-   0        0        0      879 2024-03-25 05:56:46.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/api_service.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.146817 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/constants/
--rw-rw-rw-   0        0        0       78 2024-02-09 02:31:28.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/constants/__init__.py
--rw-rw-rw-   0        0        0      749 2024-03-26 05:17:52.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/constants/route_constants.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.155794 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/enums/
--rw-rw-rw-   0        0        0       71 2024-02-09 02:31:47.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/enums/__init__.py
--rw-rw-rw-   0        0        0      444 2024-03-26 05:17:14.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/enums/http_method_enum.py
--rw-rw-rw-   0        0        0     2494 2024-04-02 06:18:21.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/error_manager.py
--rw-rw-rw-   0        0        0     4153 2024-04-02 06:19:10.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/job_manager.py
--rw-rw-rw-   0        0        0      983 2024-03-25 06:10:12.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.181724 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/
--rw-rw-rw-   0        0        0      313 2024-02-09 02:32:15.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/__init__.py
--rw-rw-rw-   0        0        0     6580 2024-03-26 05:11:06.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/api_monitoring_types.py
--rw-rw-rw-   0        0        0      664 2024-03-26 05:12:12.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/exception_log_types.py
--rw-rw-rw-   0        0        0     2459 2024-03-26 05:14:39.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/job_monitoring_types.py
--rw-rw-rw-   0        0        0      607 2024-03-26 05:16:10.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/vigil_options_types.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.210646 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_utils/
--rw-rw-rw-   0        0        0      133 2024-04-02 09:28:13.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_utils/__init__.py
--rw-rw-rw-   0        0        0     6893 2024-04-02 06:19:53.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_utils/api_monitoring_utils_django.py
--rw-rw-rw-   0        0        0     2167 2024-04-02 05:01:06.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_utils/common_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:51:36.223613 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/
--rw-rw-rw-   0        0        0     7587 2024-04-17 12:51:34.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1220 2024-04-17 12:51:35.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 12:51:35.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-17 12:51:35.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-17 12:51:35.000000 foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 12:51:36.234583 foxsenseinnovations.vigil-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      670 2024-04-17 12:49:40.000000 foxsenseinnovations.vigil-1.0.1/setup.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.447714 foxsenseinnovations_vigil-1.0.2/
+-rw-r--r--   0 haripriya   (502) staff       (20)       17 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/MANIFEST.in
+-rw-r--r--   0 haripriya   (502) staff       (20)     7500 2024-05-24 06:18:41.447513 foxsenseinnovations_vigil-1.0.2/PKG-INFO
+-rw-r--r--   0 haripriya   (502) staff       (20)     7125 2024-05-24 05:42:17.000000 foxsenseinnovations_vigil-1.0.2/README.md
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.442413 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/
+-rw-r--r--   0 haripriya   (502) staff       (20)       33 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/__init__.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.444513 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/
+-rw-r--r--   0 haripriya   (502) staff       (20)      803 2024-05-24 05:25:16.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/__init__.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     4758 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/api_manager_django.py
+-rw-r--r--   0 haripriya   (502) staff       (20)      879 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/api_service.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.444973 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/constants/
+-rw-r--r--   0 haripriya   (502) staff       (20)       78 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/constants/__init__.py
+-rw-r--r--   0 haripriya   (502) staff       (20)      749 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/constants/route_constants.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.445650 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/enums/
+-rw-r--r--   0 haripriya   (502) staff       (20)       71 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/enums/__init__.py
+-rw-r--r--   0 haripriya   (502) staff       (20)      444 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/enums/http_method_enum.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     2878 2024-05-24 05:42:44.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/error_manager.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     4153 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/job_manager.py
+-rw-r--r--   0 haripriya   (502) staff       (20)      983 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.446464 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/
+-rw-r--r--   0 haripriya   (502) staff       (20)      313 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/__init__.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     6580 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/api_monitoring_types.py
+-rw-r--r--   0 haripriya   (502) staff       (20)      664 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/exception_log_types.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     2459 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/job_monitoring_types.py
+-rw-r--r--   0 haripriya   (502) staff       (20)      607 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/vigil_options_types.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.447090 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_utils/
+-rw-r--r--   0 haripriya   (502) staff       (20)      133 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_utils/__init__.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     6893 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_utils/api_monitoring_utils_django.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     2167 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_utils/common_utils.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.447286 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/
+-rw-r--r--   0 haripriya   (502) staff       (20)     7500 2024-05-24 06:18:41.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/PKG-INFO
+-rw-r--r--   0 haripriya   (502) staff       (20)     1220 2024-05-24 06:18:41.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/SOURCES.txt
+-rw-r--r--   0 haripriya   (502) staff       (20)        1 2024-05-24 06:18:41.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/dependency_links.txt
+-rw-r--r--   0 haripriya   (502) staff       (20)       36 2024-05-24 06:18:41.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/requires.txt
+-rw-r--r--   0 haripriya   (502) staff       (20)       20 2024-05-24 06:18:41.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/top_level.txt
+-rw-r--r--   0 haripriya   (502) staff       (20)       38 2024-05-24 06:18:41.447753 foxsenseinnovations_vigil-1.0.2/setup.cfg
+-rw-r--r--   0 haripriya   (502) staff       (20)      670 2024-05-24 05:58:30.000000 foxsenseinnovations_vigil-1.0.2/setup.py
```

### Comparing `foxsenseinnovations.vigil-1.0.1/PKG-INFO` & `foxsenseinnovations_vigil-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,192 +1,194 @@
-Metadata-Version: 2.1
-Name: foxsenseinnovations.vigil
-Version: 1.0.1
-Summary: Official SDK for Vigil - A comprehensive solution for all your monitoring requirements, including exceptions, jobs, APIs, and website availability
-License: ISC
-Description-Content-Type: text/markdown
-Requires-Dist: setuptools
-Requires-Dist: requests
-Requires-Dist: werkzeug
-Requires-Dist: django
-
-# Vigil - SDK
-
-## Overview
-
-Welcome to the official SDK for Vigil - A comprehensive solution for all your monitoring requirements. The foxsenseinnovations.vigil PyPi package provides developers with a powerful and easy-to-use toolkit for integrating Vigil into their applications. Monitor exceptions, jobs, APIs, and website availability seamlessly with this SDK.
-
-## Features
-
-- Exception Monitoring: Keep track of exceptions in your application, receive detailed reports, and gain insights into potential issues.
-- Job Monitoring: Monitor the status and performance of background jobs, ensuring that critical tasks are executed successfully.
-- API Monitoring: Track the health and performance of your APIs, ensuring optimal functionality and responsiveness.
-- Website Availability: Check the availability and responsiveness of your websites to ensure a seamless user experience.
-
-## Installation
-
-To get started with 'foxsenseinnovations.vigil' SDK, follow these steps:
-
-### Install the pypi Package:
-
-```
-pip install foxsenseinnovations.vigil
-```
-
-### Initialize Vigil:
-
-Initialize Vigil with the provided VigilOptions. This step involves setting up the necessary configurations for your Vigil instance. Define API_KEY (mandatory) , INSTANCE_URL (optional) and CLIENT_VERSION (optional) in settings.py file. Declare the below statements in main application views.py file.
-
-```
-# import Vigil to initialize the API KEY
-from foxsenseinnovations.vigil import Vigil
-from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
-
-# Access the API_KEY from settings.py file
-api_key = django_settings.API_KEY
-
-# Define the VigilOptions instance with the desired values
-options = VigilOptions(api_key=api_key)
-
-# Initialize the Vigil class with the provided options
-Vigil.initialize(options)
-```
-
-If optional parameters are also included in the settings.py file, then the initialization of Vigil would be as follows:
-
-```
-# import Vigil to initialize the API KEY
-from foxsenseinnovations.vigil import Vigil
-from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
-
-# Access the INSTANCE_URL, CLIENT_VERSION from settings.py file
-instance_url = django_settings.INSTANCE_URL
-cient_version = django_settings.CLIENT_VERSION
-
-# Define the VigilOptions instance with the desired values
-options = VigilOptions(api_key=api_key, version=cient_version, instance_url=instance_url)
-
-# Initialize the Vigil class with the provided options
-Vigil.initialize(options)
-```
-
-## API Monitoring
-
-Declare the below statements in settings.py file
-
-```
-from foxsenseinnovations.vigil.vigil_types.api_monitoring_types import ApiMonitoringOptions, ExcludeOptions
-
-# In MIDDLEWARE of settings.py file add the below line
-'foxsenseinnovations.vigil.api_manager_django.ApiMonitoringMiddleware'
-```
-
-### Options
-
-Options are not mandatory
-
-| Options | Mandatory |     Default      |                          Values                          |
-| ------- | :-------: | :--------------: | :------------------------------------------------------: |
-| exclude |   FALSE   | ExcludeOptions() | ExcludeOptions(GET: [], POST: [], PATCH: [], DELETE: []) |
-
-#### Exclude
-
-- The exclude option allows you to specify certain API paths to be excluded from monitoring for each HTTP method. This means that requests to these excluded paths will not be tracked or analyzed by Vigil.
-- It's particularly useful when there are specific endpoints that you don't want to include in your monitoring activities, perhaps because they are known to be non-critical or for internal use only.
-- For each HTTP method (GET, POST, PATCH, DELETE), you can define a list of API paths to be excluded. By default, if no exclusions are provided, all API paths are monitored.
-
-```
-from foxsenseinnovations.vigil.vigil_types.api_monitoring_types import ApiMonitoringOptions, ExcludeOptions
-
-# In MIDDLEWARE list of settings.py file add the below line
-'foxsenseinnovations.vigil.api_manager_django.ApiMonitoringMiddleware'
-
-# After MIDDLEWARE list add the below lines
-exclude_options = ApiMonitoringOptions(exclude=ExcludeOptions(GET=['/'],POST=['/health']))
-
-# '/' GET method and '/health' POST method APIs are not monitored
-API_MONITORING_OPTIONS = exclude_options
-```
-
-## Job Monitoring
-
-To ensure monitoring of jobs within the application, integrate the following code snippet wherever jobs are defined and executed:
-
-```
-# import JobManager to monitor the Jobs in the application
-from foxsenseinnovations.vigil.job_manager import JobManager
-from foxsenseinnovations.vigil.vigil_types.job_monitoring_types import JobDetail
-
-# Job function
-def job_func():
-    try:
-        // log that the job triggered with a start message
-        start_job_detail = {'job_id': "<job-id>", 'message': "<job-start-message>"}
-        JobManager.capture_job_start(JobDetail(**start_job_detail))
-        ...
-        ...
-        // log that the job has completed its execution with a success message
-        stop_job_detail = {'job_id': "<job-id>", 'message': "<job-end-message>"}
-        JobManager.capture_job_end(JobDetail(**stop_job_detail))
-    except Exception as error:
-        fail_job_detail = {'job_id'="<job-id>", message=f"<job-failure-message>: {str(error)}"}
-        JobManager.capture_job_failure(JobDetail(**fail_job_detail))
-```
-
-Incorporating this code into job functions enables monitoring of job execution, capturing start, success, and failure events.
-
-## Error Monitoring
-
-To ensure monitoring of errors within the application, integrate the following code snippet wherever errors are captured:
-
-```
-# import ErrorManager to capture any exceptions/errors that occur in the application
-from foxsenseinnovations.vigil.error_manager import ErrorManager
-
-def function():
-    try:
-        ...
-        ...
-    except Exception as error:
-        // capture the exception from the error object
-        ErrorManager.capture_exception(error)
-```
-
-### Options
-
-Options are not mandatory
-
-| Options | Mandatory | Default |      Values      |
-| ------- | :-------: | :-----: | :--------------: |
-| tags    |   FALSE   |   []    | Array of strings |
-| context |   FALSE   |   {}    |    An object     |
-
-#### Tags and Context
-
-- Gives extra information about the exception that occurred
-
-```
-# import ErrorManager to capture any exceptions/errors that occur in the application
-from foxsenseinnovations.vigil.error_manager import ErrorManager
-
-def function():
-    try:
-        ...
-        ...
-    except Exception as error:
-        options = {
-            tags: ['tag1','tag2'],
-            context: {
-                <key1>: <value1>,
-                <key2>: <value2>
-            }
-        }
-        // capture the exception from the error object
-        // and pass extra information about the exception in options
-        ErrorManager.capture_exception(error, options)
-```
-
-## Support
-
-In case of any issues, questions or assistance needed, please feel free to reach out to our support team (support@vigilnow.freshdesk.com).
-
-Happy Monitoring with Vigil!
+Metadata-Version: 2.1
+Name: foxsenseinnovations.vigil
+Version: 1.0.2
+Summary: Official SDK for Vigil - A comprehensive solution for all your monitoring requirements, including exceptions, jobs, APIs, and website availability
+License: ISC
+Description-Content-Type: text/markdown
+Requires-Dist: setuptools
+Requires-Dist: requests
+Requires-Dist: werkzeug
+Requires-Dist: django
+
+# Vigil - SDK
+
+## Overview
+
+Welcome to the official SDK for Vigil - A comprehensive solution for all your monitoring requirements. The foxsenseinnovations.vigil PyPi package provides developers with a powerful and easy-to-use toolkit for integrating Vigil into their applications. Monitor exceptions, jobs, APIs, and website availability seamlessly with this SDK.
+
+## Features
+
+- Exception Monitoring: Keep track of exceptions in your application, receive detailed reports, and gain insights into potential issues.
+- Job Monitoring: Monitor the status and performance of background jobs, ensuring that critical tasks are executed successfully.
+- API Monitoring: Track the health and performance of your APIs, ensuring optimal functionality and responsiveness.
+- Website Availability: Check the availability and responsiveness of your websites to ensure a seamless user experience.
+
+## Installation
+
+To get started with 'foxsenseinnovations.vigil' SDK, follow these steps:
+
+### Install the pypi Package:
+
+```
+pip install foxsenseinnovations.vigil
+```
+
+### Initialize Vigil:
+
+Initialize Vigil with the provided VigilOptions. This step involves setting up the necessary configurations for your Vigil instance. Define API_KEY (mandatory) , INSTANCE_URL (optional) and CLIENT_VERSION (optional) in settings.py file. Declare the below statements in main application manage.py file.
+
+```
+# import Vigil to initialize the API KEY
+from foxsenseinnovations.vigil import Vigil
+from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
+from django.conf import settings as django_settings
+
+# Access the API_KEY from settings.py file
+api_key = django_settings.API_KEY
+
+# Define the VigilOptions instance with the desired values
+options = VigilOptions(api_key=api_key)
+
+# Initialize the Vigil class with the provided options
+Vigil.initialize(options)
+```
+
+If optional parameters are also included in the settings.py file, then the initialization of Vigil would be as follows:
+
+```
+# import Vigil to initialize the API KEY
+from foxsenseinnovations.vigil import Vigil
+from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
+from django.conf import settings as django_settings
+
+# Access the INSTANCE_URL, CLIENT_VERSION from settings.py file
+instance_url = django_settings.INSTANCE_URL
+cient_version = django_settings.CLIENT_VERSION
+
+# Define the VigilOptions instance with the desired values
+options = VigilOptions(api_key=api_key, version=cient_version, instance_url=instance_url)
+
+# Initialize the Vigil class with the provided options
+Vigil.initialize(options)
+```
+
+## API Monitoring
+
+Declare the below statements in settings.py file
+
+```
+from foxsenseinnovations.vigil.vigil_types.api_monitoring_types import ApiMonitoringOptions, ExcludeOptions
+
+# In MIDDLEWARE of settings.py file add the below line
+'foxsenseinnovations.vigil.api_manager_django.ApiMonitoringMiddleware'
+```
+
+### Options
+
+Options are not mandatory
+
+| Options | Mandatory |     Default      |                          Values                          |
+| ------- | :-------: | :--------------: | :------------------------------------------------------: |
+| exclude |   FALSE   | ExcludeOptions() | ExcludeOptions(GET: [], POST: [], PATCH: [], DELETE: []) |
+
+#### Exclude
+
+- The exclude option allows you to specify certain API paths to be excluded from monitoring for each HTTP method. This means that requests to these excluded paths will not be tracked or analyzed by Vigil.
+- It's particularly useful when there are specific endpoints that you don't want to include in your monitoring activities, perhaps because they are known to be non-critical or for internal use only.
+- For each HTTP method (GET, POST, PATCH, DELETE), you can define a list of API paths to be excluded. By default, if no exclusions are provided, all API paths are monitored.
+
+```
+from foxsenseinnovations.vigil.vigil_types.api_monitoring_types import ApiMonitoringOptions, ExcludeOptions
+
+# In MIDDLEWARE list of settings.py file add the below line
+'foxsenseinnovations.vigil.api_manager_django.ApiMonitoringMiddleware'
+
+# After MIDDLEWARE list add the below lines
+exclude_options = ApiMonitoringOptions(exclude=ExcludeOptions(GET=['/'],POST=['/health']))
+
+# '/' GET method and '/health' POST method APIs are not monitored
+API_MONITORING_OPTIONS = exclude_options
+```
+
+## Job Monitoring
+
+To ensure monitoring of jobs within the application, integrate the following code snippet wherever jobs are defined and executed:
+
+```
+# import JobManager to monitor the Jobs in the application
+from foxsenseinnovations.vigil.job_manager import JobManager
+from foxsenseinnovations.vigil.vigil_types.job_monitoring_types import JobDetail
+
+# Job function
+def job_func():
+    try:
+        // log that the job triggered with a start message
+        start_job_detail = {'job_id': "<job-id>", 'message': "<job-start-message>"}
+        JobManager.capture_job_start(JobDetail(**start_job_detail))
+        ...
+        ...
+        // log that the job has completed its execution with a success message
+        stop_job_detail = {'job_id': "<job-id>", 'message': "<job-end-message>"}
+        JobManager.capture_job_end(JobDetail(**stop_job_detail))
+    except Exception as error:
+        fail_job_detail = {'job_id'="<job-id>", message=f"<job-failure-message>: {str(error)}"}
+        JobManager.capture_job_failure(JobDetail(**fail_job_detail))
+```
+
+Incorporating this code into job functions enables monitoring of job execution, capturing start, success, and failure events.
+
+## Error Monitoring
+
+To ensure monitoring of errors within the application, integrate the following code snippet wherever errors are captured:
+
+```
+# import ErrorManager to capture any exceptions/errors that occur in the application
+from foxsenseinnovations.vigil.error_manager import ErrorManager
+
+def function():
+    try:
+        ...
+        ...
+    except Exception as error:
+        // capture the exception from the error object
+        ErrorManager.capture_exception(error)
+```
+
+### Options
+
+Options are not mandatory
+
+| Options | Mandatory | Default |      Values      |
+| ------- | :-------: | :-----: | :--------------: |
+| tags    |   FALSE   |   []    | Array of strings |
+| context |   FALSE   |   {}    |    An object     |
+
+#### Tags and Context
+
+- Gives extra information about the exception that occurred
+
+```
+# import ErrorManager to capture any exceptions/errors that occur in the application
+from foxsenseinnovations.vigil.error_manager import ErrorManager
+
+def function():
+    try:
+        ...
+        ...
+    except Exception as error:
+        options = {
+            tags: ['tag1','tag2'],
+            context: {
+                <key1>: <value1>,
+                <key2>: <value2>
+            }
+        }
+        // capture the exception from the error object
+        // and pass extra information about the exception in options
+        ErrorManager.capture_exception(error, options)
+```
+
+## Support
+
+In case of any issues, questions or assistance needed, please feel free to reach out to our support team (support@vigilnow.freshdesk.com).
+
+Happy Monitoring with Vigil!
```

### Comparing `foxsenseinnovations.vigil-1.0.1/README.md` & `foxsenseinnovations_vigil-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,21 @@
 
 ```
 pip install foxsenseinnovations.vigil
 ```
 
 ### Initialize Vigil:
 
-Initialize Vigil with the provided VigilOptions. This step involves setting up the necessary configurations for your Vigil instance. Define API_KEY (mandatory) , INSTANCE_URL (optional) and CLIENT_VERSION (optional) in settings.py file. Declare the below statements in main application views.py file.
+Initialize Vigil with the provided VigilOptions. This step involves setting up the necessary configurations for your Vigil instance. Define API_KEY (mandatory) , INSTANCE_URL (optional) and CLIENT_VERSION (optional) in settings.py file. Declare the below statements in main application manage.py file.
 
 ```
 # import Vigil to initialize the API KEY
 from foxsenseinnovations.vigil import Vigil
 from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
+from django.conf import settings as django_settings
 
 # Access the API_KEY from settings.py file
 api_key = django_settings.API_KEY
 
 # Define the VigilOptions instance with the desired values
 options = VigilOptions(api_key=api_key)
 
@@ -42,14 +43,15 @@
 
 If optional parameters are also included in the settings.py file, then the initialization of Vigil would be as follows:
 
 ```
 # import Vigil to initialize the API KEY
 from foxsenseinnovations.vigil import Vigil
 from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
+from django.conf import settings as django_settings
 
 # Access the INSTANCE_URL, CLIENT_VERSION from settings.py file
 instance_url = django_settings.INSTANCE_URL
 cient_version = django_settings.CLIENT_VERSION
 
 # Define the VigilOptions instance with the desired values
 options = VigilOptions(api_key=api_key, version=cient_version, instance_url=instance_url)
```

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/api_manager_django.py` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/api_manager_django.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/api_service.py` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/api_service.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/constants/route_constants.py` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/constants/route_constants.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/error_manager.py` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/error_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,46 +14,47 @@
     Attributes:
         None
     """
     def capture_exception(
         self,
         exception: Any,
         extra_attributes: Optional[ExceptionExtraAttributes] = None,
+        isUnhandled: Optional[bool] = False
     ) -> None:
         """
         Captures an exception and sends data to Vigil for monitoring.
         Args:
             exception (Any): The exception object.
             extra_attributes (Optional[ExceptionExtraAttributes]): Extra attributes related to the exception
             (default None).
         Returns:
             None
         """
         frames = traceback.extract_tb(exception.__traceback__)
         frames_info = [
             {
-                'beforeParse': traceback.format_exc(),
+                'beforeParse': repr(frame),
                 'fileName': frame.filename,
                 'functionName': frame.name,
                 'functionShortName': frame.name,
                 'fileFullPath': frame.filename,
                 'lineNo': frame.lineno
             }
             for frame in frames
         ]
         error_data = {
-            "clientVersion": extra_attributes.get('client_version', Vigil.version),
+            "clientVersion": extra_attributes.get('client_version') if extra_attributes and extra_attributes.get('client_version') is not None else Vigil.version,
             "error": {
                 "name": exception.__class__.__name__,
                 "message": str(exception),
-                "stack": traceback.format_exc(),
+                "stack": traceback.format_exc() if isUnhandled is False else ''.join(traceback.format_exception(exception.__class__.__name__, exception, exception.__traceback__)),
                 "stackFrames": frames_info
             },
-            "tags": extra_attributes.get('tags', None),
-            "context": extra_attributes.get('context', None),
+            "tags": extra_attributes.get('tags') if extra_attributes and extra_attributes.get('tags') is not None else None,
+            "context": extra_attributes.get('context') if extra_attributes and extra_attributes.get('context') is not None else None,
             "reportedAt": datetime.now(timezone.utc).isoformat(),
         }
 
         response = ApiService.make_api_call(
             Vigil.instance_url,
             RouteConstants.ERROR_MONITORING,
             error_data,
```

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/job_manager.py` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/job_manager.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil.py` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/api_monitoring_types.py` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/api_monitoring_types.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/exception_log_types.py` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/exception_log_types.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/job_monitoring_types.py` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/job_monitoring_types.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_types/vigil_options_types.py` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/vigil_options_types.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_utils/api_monitoring_utils_django.py` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_utils/api_monitoring_utils_django.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations/vigil/vigil_utils/common_utils.py` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/PKG-INFO` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,192 +1,194 @@
-Metadata-Version: 2.1
-Name: foxsenseinnovations.vigil
-Version: 1.0.1
-Summary: Official SDK for Vigil - A comprehensive solution for all your monitoring requirements, including exceptions, jobs, APIs, and website availability
-License: ISC
-Description-Content-Type: text/markdown
-Requires-Dist: setuptools
-Requires-Dist: requests
-Requires-Dist: werkzeug
-Requires-Dist: django
-
-# Vigil - SDK
-
-## Overview
-
-Welcome to the official SDK for Vigil - A comprehensive solution for all your monitoring requirements. The foxsenseinnovations.vigil PyPi package provides developers with a powerful and easy-to-use toolkit for integrating Vigil into their applications. Monitor exceptions, jobs, APIs, and website availability seamlessly with this SDK.
-
-## Features
-
-- Exception Monitoring: Keep track of exceptions in your application, receive detailed reports, and gain insights into potential issues.
-- Job Monitoring: Monitor the status and performance of background jobs, ensuring that critical tasks are executed successfully.
-- API Monitoring: Track the health and performance of your APIs, ensuring optimal functionality and responsiveness.
-- Website Availability: Check the availability and responsiveness of your websites to ensure a seamless user experience.
-
-## Installation
-
-To get started with 'foxsenseinnovations.vigil' SDK, follow these steps:
-
-### Install the pypi Package:
-
-```
-pip install foxsenseinnovations.vigil
-```
-
-### Initialize Vigil:
-
-Initialize Vigil with the provided VigilOptions. This step involves setting up the necessary configurations for your Vigil instance. Define API_KEY (mandatory) , INSTANCE_URL (optional) and CLIENT_VERSION (optional) in settings.py file. Declare the below statements in main application views.py file.
-
-```
-# import Vigil to initialize the API KEY
-from foxsenseinnovations.vigil import Vigil
-from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
-
-# Access the API_KEY from settings.py file
-api_key = django_settings.API_KEY
-
-# Define the VigilOptions instance with the desired values
-options = VigilOptions(api_key=api_key)
-
-# Initialize the Vigil class with the provided options
-Vigil.initialize(options)
-```
-
-If optional parameters are also included in the settings.py file, then the initialization of Vigil would be as follows:
-
-```
-# import Vigil to initialize the API KEY
-from foxsenseinnovations.vigil import Vigil
-from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
-
-# Access the INSTANCE_URL, CLIENT_VERSION from settings.py file
-instance_url = django_settings.INSTANCE_URL
-cient_version = django_settings.CLIENT_VERSION
-
-# Define the VigilOptions instance with the desired values
-options = VigilOptions(api_key=api_key, version=cient_version, instance_url=instance_url)
-
-# Initialize the Vigil class with the provided options
-Vigil.initialize(options)
-```
-
-## API Monitoring
-
-Declare the below statements in settings.py file
-
-```
-from foxsenseinnovations.vigil.vigil_types.api_monitoring_types import ApiMonitoringOptions, ExcludeOptions
-
-# In MIDDLEWARE of settings.py file add the below line
-'foxsenseinnovations.vigil.api_manager_django.ApiMonitoringMiddleware'
-```
-
-### Options
-
-Options are not mandatory
-
-| Options | Mandatory |     Default      |                          Values                          |
-| ------- | :-------: | :--------------: | :------------------------------------------------------: |
-| exclude |   FALSE   | ExcludeOptions() | ExcludeOptions(GET: [], POST: [], PATCH: [], DELETE: []) |
-
-#### Exclude
-
-- The exclude option allows you to specify certain API paths to be excluded from monitoring for each HTTP method. This means that requests to these excluded paths will not be tracked or analyzed by Vigil.
-- It's particularly useful when there are specific endpoints that you don't want to include in your monitoring activities, perhaps because they are known to be non-critical or for internal use only.
-- For each HTTP method (GET, POST, PATCH, DELETE), you can define a list of API paths to be excluded. By default, if no exclusions are provided, all API paths are monitored.
-
-```
-from foxsenseinnovations.vigil.vigil_types.api_monitoring_types import ApiMonitoringOptions, ExcludeOptions
-
-# In MIDDLEWARE list of settings.py file add the below line
-'foxsenseinnovations.vigil.api_manager_django.ApiMonitoringMiddleware'
-
-# After MIDDLEWARE list add the below lines
-exclude_options = ApiMonitoringOptions(exclude=ExcludeOptions(GET=['/'],POST=['/health']))
-
-# '/' GET method and '/health' POST method APIs are not monitored
-API_MONITORING_OPTIONS = exclude_options
-```
-
-## Job Monitoring
-
-To ensure monitoring of jobs within the application, integrate the following code snippet wherever jobs are defined and executed:
-
-```
-# import JobManager to monitor the Jobs in the application
-from foxsenseinnovations.vigil.job_manager import JobManager
-from foxsenseinnovations.vigil.vigil_types.job_monitoring_types import JobDetail
-
-# Job function
-def job_func():
-    try:
-        // log that the job triggered with a start message
-        start_job_detail = {'job_id': "<job-id>", 'message': "<job-start-message>"}
-        JobManager.capture_job_start(JobDetail(**start_job_detail))
-        ...
-        ...
-        // log that the job has completed its execution with a success message
-        stop_job_detail = {'job_id': "<job-id>", 'message': "<job-end-message>"}
-        JobManager.capture_job_end(JobDetail(**stop_job_detail))
-    except Exception as error:
-        fail_job_detail = {'job_id'="<job-id>", message=f"<job-failure-message>: {str(error)}"}
-        JobManager.capture_job_failure(JobDetail(**fail_job_detail))
-```
-
-Incorporating this code into job functions enables monitoring of job execution, capturing start, success, and failure events.
-
-## Error Monitoring
-
-To ensure monitoring of errors within the application, integrate the following code snippet wherever errors are captured:
-
-```
-# import ErrorManager to capture any exceptions/errors that occur in the application
-from foxsenseinnovations.vigil.error_manager import ErrorManager
-
-def function():
-    try:
-        ...
-        ...
-    except Exception as error:
-        // capture the exception from the error object
-        ErrorManager.capture_exception(error)
-```
-
-### Options
-
-Options are not mandatory
-
-| Options | Mandatory | Default |      Values      |
-| ------- | :-------: | :-----: | :--------------: |
-| tags    |   FALSE   |   []    | Array of strings |
-| context |   FALSE   |   {}    |    An object     |
-
-#### Tags and Context
-
-- Gives extra information about the exception that occurred
-
-```
-# import ErrorManager to capture any exceptions/errors that occur in the application
-from foxsenseinnovations.vigil.error_manager import ErrorManager
-
-def function():
-    try:
-        ...
-        ...
-    except Exception as error:
-        options = {
-            tags: ['tag1','tag2'],
-            context: {
-                <key1>: <value1>,
-                <key2>: <value2>
-            }
-        }
-        // capture the exception from the error object
-        // and pass extra information about the exception in options
-        ErrorManager.capture_exception(error, options)
-```
-
-## Support
-
-In case of any issues, questions or assistance needed, please feel free to reach out to our support team (support@vigilnow.freshdesk.com).
-
-Happy Monitoring with Vigil!
+Metadata-Version: 2.1
+Name: foxsenseinnovations.vigil
+Version: 1.0.2
+Summary: Official SDK for Vigil - A comprehensive solution for all your monitoring requirements, including exceptions, jobs, APIs, and website availability
+License: ISC
+Description-Content-Type: text/markdown
+Requires-Dist: setuptools
+Requires-Dist: requests
+Requires-Dist: werkzeug
+Requires-Dist: django
+
+# Vigil - SDK
+
+## Overview
+
+Welcome to the official SDK for Vigil - A comprehensive solution for all your monitoring requirements. The foxsenseinnovations.vigil PyPi package provides developers with a powerful and easy-to-use toolkit for integrating Vigil into their applications. Monitor exceptions, jobs, APIs, and website availability seamlessly with this SDK.
+
+## Features
+
+- Exception Monitoring: Keep track of exceptions in your application, receive detailed reports, and gain insights into potential issues.
+- Job Monitoring: Monitor the status and performance of background jobs, ensuring that critical tasks are executed successfully.
+- API Monitoring: Track the health and performance of your APIs, ensuring optimal functionality and responsiveness.
+- Website Availability: Check the availability and responsiveness of your websites to ensure a seamless user experience.
+
+## Installation
+
+To get started with 'foxsenseinnovations.vigil' SDK, follow these steps:
+
+### Install the pypi Package:
+
+```
+pip install foxsenseinnovations.vigil
+```
+
+### Initialize Vigil:
+
+Initialize Vigil with the provided VigilOptions. This step involves setting up the necessary configurations for your Vigil instance. Define API_KEY (mandatory) , INSTANCE_URL (optional) and CLIENT_VERSION (optional) in settings.py file. Declare the below statements in main application manage.py file.
+
+```
+# import Vigil to initialize the API KEY
+from foxsenseinnovations.vigil import Vigil
+from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
+from django.conf import settings as django_settings
+
+# Access the API_KEY from settings.py file
+api_key = django_settings.API_KEY
+
+# Define the VigilOptions instance with the desired values
+options = VigilOptions(api_key=api_key)
+
+# Initialize the Vigil class with the provided options
+Vigil.initialize(options)
+```
+
+If optional parameters are also included in the settings.py file, then the initialization of Vigil would be as follows:
+
+```
+# import Vigil to initialize the API KEY
+from foxsenseinnovations.vigil import Vigil
+from foxsenseinnovations.vigil.vigil_types.vigil_options_types import VigilOptions
+from django.conf import settings as django_settings
+
+# Access the INSTANCE_URL, CLIENT_VERSION from settings.py file
+instance_url = django_settings.INSTANCE_URL
+cient_version = django_settings.CLIENT_VERSION
+
+# Define the VigilOptions instance with the desired values
+options = VigilOptions(api_key=api_key, version=cient_version, instance_url=instance_url)
+
+# Initialize the Vigil class with the provided options
+Vigil.initialize(options)
+```
+
+## API Monitoring
+
+Declare the below statements in settings.py file
+
+```
+from foxsenseinnovations.vigil.vigil_types.api_monitoring_types import ApiMonitoringOptions, ExcludeOptions
+
+# In MIDDLEWARE of settings.py file add the below line
+'foxsenseinnovations.vigil.api_manager_django.ApiMonitoringMiddleware'
+```
+
+### Options
+
+Options are not mandatory
+
+| Options | Mandatory |     Default      |                          Values                          |
+| ------- | :-------: | :--------------: | :------------------------------------------------------: |
+| exclude |   FALSE   | ExcludeOptions() | ExcludeOptions(GET: [], POST: [], PATCH: [], DELETE: []) |
+
+#### Exclude
+
+- The exclude option allows you to specify certain API paths to be excluded from monitoring for each HTTP method. This means that requests to these excluded paths will not be tracked or analyzed by Vigil.
+- It's particularly useful when there are specific endpoints that you don't want to include in your monitoring activities, perhaps because they are known to be non-critical or for internal use only.
+- For each HTTP method (GET, POST, PATCH, DELETE), you can define a list of API paths to be excluded. By default, if no exclusions are provided, all API paths are monitored.
+
+```
+from foxsenseinnovations.vigil.vigil_types.api_monitoring_types import ApiMonitoringOptions, ExcludeOptions
+
+# In MIDDLEWARE list of settings.py file add the below line
+'foxsenseinnovations.vigil.api_manager_django.ApiMonitoringMiddleware'
+
+# After MIDDLEWARE list add the below lines
+exclude_options = ApiMonitoringOptions(exclude=ExcludeOptions(GET=['/'],POST=['/health']))
+
+# '/' GET method and '/health' POST method APIs are not monitored
+API_MONITORING_OPTIONS = exclude_options
+```
+
+## Job Monitoring
+
+To ensure monitoring of jobs within the application, integrate the following code snippet wherever jobs are defined and executed:
+
+```
+# import JobManager to monitor the Jobs in the application
+from foxsenseinnovations.vigil.job_manager import JobManager
+from foxsenseinnovations.vigil.vigil_types.job_monitoring_types import JobDetail
+
+# Job function
+def job_func():
+    try:
+        // log that the job triggered with a start message
+        start_job_detail = {'job_id': "<job-id>", 'message': "<job-start-message>"}
+        JobManager.capture_job_start(JobDetail(**start_job_detail))
+        ...
+        ...
+        // log that the job has completed its execution with a success message
+        stop_job_detail = {'job_id': "<job-id>", 'message': "<job-end-message>"}
+        JobManager.capture_job_end(JobDetail(**stop_job_detail))
+    except Exception as error:
+        fail_job_detail = {'job_id'="<job-id>", message=f"<job-failure-message>: {str(error)}"}
+        JobManager.capture_job_failure(JobDetail(**fail_job_detail))
+```
+
+Incorporating this code into job functions enables monitoring of job execution, capturing start, success, and failure events.
+
+## Error Monitoring
+
+To ensure monitoring of errors within the application, integrate the following code snippet wherever errors are captured:
+
+```
+# import ErrorManager to capture any exceptions/errors that occur in the application
+from foxsenseinnovations.vigil.error_manager import ErrorManager
+
+def function():
+    try:
+        ...
+        ...
+    except Exception as error:
+        // capture the exception from the error object
+        ErrorManager.capture_exception(error)
+```
+
+### Options
+
+Options are not mandatory
+
+| Options | Mandatory | Default |      Values      |
+| ------- | :-------: | :-----: | :--------------: |
+| tags    |   FALSE   |   []    | Array of strings |
+| context |   FALSE   |   {}    |    An object     |
+
+#### Tags and Context
+
+- Gives extra information about the exception that occurred
+
+```
+# import ErrorManager to capture any exceptions/errors that occur in the application
+from foxsenseinnovations.vigil.error_manager import ErrorManager
+
+def function():
+    try:
+        ...
+        ...
+    except Exception as error:
+        options = {
+            tags: ['tag1','tag2'],
+            context: {
+                <key1>: <value1>,
+                <key2>: <value2>
+            }
+        }
+        // capture the exception from the error object
+        // and pass extra information about the exception in options
+        ErrorManager.capture_exception(error, options)
+```
+
+## Support
+
+In case of any issues, questions or assistance needed, please feel free to reach out to our support team (support@vigilnow.freshdesk.com).
+
+Happy Monitoring with Vigil!
```

### Comparing `foxsenseinnovations.vigil-1.0.1/foxsenseinnovations.vigil.egg-info/SOURCES.txt` & `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations.vigil-1.0.1/setup.py` & `foxsenseinnovations_vigil-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='foxsenseinnovations.vigil',
-    version='1.0.1',
+    version='1.0.2',
     description='Official SDK for Vigil - A comprehensive solution for all your monitoring requirements, including exceptions, jobs, APIs, and website availability',
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     packages=find_packages(exclude=['foxsenseinnovations.vigil.flask']),
     install_requires=[
         'setuptools',
```

