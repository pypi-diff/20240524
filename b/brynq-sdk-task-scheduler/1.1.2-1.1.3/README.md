# Comparing `tmp/brynq_sdk_task_scheduler-1.1.2.tar.gz` & `tmp/brynq_sdk_task_scheduler-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brynq_sdk_task_scheduler-1.1.2.tar", last modified: Thu Apr 25 10:38:23 2024, max compression
+gzip compressed data, was "dist/brynq_sdk_task_scheduler-1.1.3.tar", last modified: Fri May 24 07:29:42 2024, max compression
```

## Comparing `brynq_sdk_task_scheduler-1.1.2.tar` & `brynq_sdk_task_scheduler-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:38:23.000000 brynq_sdk_task_scheduler-1.1.2/
--rw-r--r--   0 root         (0) root         (0)      327 2024-04-25 10:38:23.000000 brynq_sdk_task_scheduler-1.1.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:38:23.000000 brynq_sdk_task_scheduler-1.1.2/brynq_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:38:23.000000 brynq_sdk_task_scheduler-1.1.2/brynq_sdk/task_scheduler/
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-25 10:38:04.000000 brynq_sdk_task_scheduler-1.1.2/brynq_sdk/task_scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    43069 2024-04-25 10:38:04.000000 brynq_sdk_task_scheduler-1.1.2/brynq_sdk/task_scheduler/task_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 10:38:23.000000 brynq_sdk_task_scheduler-1.1.2/brynq_sdk_task_scheduler.egg-info/
--rw-r--r--   0 root         (0) root         (0)      327 2024-04-25 10:38:23.000000 brynq_sdk_task_scheduler-1.1.2/brynq_sdk_task_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-25 10:38:23.000000 brynq_sdk_task_scheduler-1.1.2/brynq_sdk_task_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 10:38:23.000000 brynq_sdk_task_scheduler-1.1.2/brynq_sdk_task_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 10:38:23.000000 brynq_sdk_task_scheduler-1.1.2/brynq_sdk_task_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      104 2024-04-25 10:38:23.000000 brynq_sdk_task_scheduler-1.1.2/brynq_sdk_task_scheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-25 10:38:23.000000 brynq_sdk_task_scheduler-1.1.2/brynq_sdk_task_scheduler.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 10:38:23.000000 brynq_sdk_task_scheduler-1.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-25 10:38:04.000000 brynq_sdk_task_scheduler-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:29:42.000000 brynq_sdk_task_scheduler-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-24 07:29:42.000000 brynq_sdk_task_scheduler-1.1.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:29:42.000000 brynq_sdk_task_scheduler-1.1.3/brynq_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:29:42.000000 brynq_sdk_task_scheduler-1.1.3/brynq_sdk/task_scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-05-24 07:29:19.000000 brynq_sdk_task_scheduler-1.1.3/brynq_sdk/task_scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    43061 2024-05-24 07:29:19.000000 brynq_sdk_task_scheduler-1.1.3/brynq_sdk/task_scheduler/task_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:29:42.000000 brynq_sdk_task_scheduler-1.1.3/brynq_sdk_task_scheduler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-24 07:29:42.000000 brynq_sdk_task_scheduler-1.1.3/brynq_sdk_task_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-24 07:29:42.000000 brynq_sdk_task_scheduler-1.1.3/brynq_sdk_task_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 07:29:42.000000 brynq_sdk_task_scheduler-1.1.3/brynq_sdk_task_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 07:29:42.000000 brynq_sdk_task_scheduler-1.1.3/brynq_sdk_task_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-24 07:29:42.000000 brynq_sdk_task_scheduler-1.1.3/brynq_sdk_task_scheduler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-24 07:29:42.000000 brynq_sdk_task_scheduler-1.1.3/brynq_sdk_task_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 07:29:42.000000 brynq_sdk_task_scheduler-1.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-24 07:29:19.000000 brynq_sdk_task_scheduler-1.1.3/setup.py
```

### Comparing `brynq_sdk_task_scheduler-1.1.2/brynq_sdk/task_scheduler/task_scheduler.py` & `brynq_sdk_task_scheduler-1.1.3/brynq_sdk/task_scheduler/task_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
         elif data is not None and full_extract is False:
             extra_payload['full_load'] = False
 
         # Preparing the primary payload with log details
         payload = {
             'reload_id': self.run_id,
             'task_id': self.task_id,
-            'customer_id': os.getenv('BRYNQ_CUSTOMER_NAME').lower().replace(' ', '_'),
+            'customer_id': os.getenv('BRYNQ_SUBDOMAIN').lower().replace(' ', '_'),
             'started_at': datetime.datetime.now().isoformat(),
             'loglevel': loglevel,
             'message': message
         }
         payload.update(extra_payload)
 
         # Sending the payload to ElasticSearch
@@ -386,15 +386,15 @@
         :return: nothing
         """
 
         # Preparing the primary payload with error details for upload to elastic
         payload = {
             'reload_id': self.run_id,
             'task_id': self.task_id,
-            'customer_id': os.getenv('BRYNQ_CUSTOMER_NAME').lower().replace(' ', '_'),
+            'customer_id': os.getenv('BRYNQ_SUBDOMAIN').lower().replace(' ', '_'),
             'started_at': datetime.datetime.now().isoformat(),
             'loglevel': 'CRITICAL',
             'message': str(e),
             'traceback': traceback.format_exc()
         }
 
         # Sending the payload to ElasticSearch
```

### Comparing `brynq_sdk_task_scheduler-1.1.2/setup.py` & `brynq_sdk_task_scheduler-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 
 setup(
     name='brynq_sdk_task_scheduler',
-    version='1.1.2',
+    version='1.1.3',
     description='Code to execute tasks in BrynQ.com with the task scheduler',
     long_description='Code to execute tasks in the BrynQ.com platform with the task scheduler',
     author='BrynQ',
     author_email='support@brynq.com',
     packages=["brynq_sdk.task_scheduler"],
     license='BrynQ License',
     install_requires=[
         'brynq-sdk-brynq>=1',
         'brynq-sdk-functions>=1',
         'brynq-sdk-mysql>=1',
         'brynq-sdk-mandrill>=1',
-        'brynq-sdk-elastic>=1'
+        'brynq-sdk-elastic>=2'
     ],
     zip_safe=False,
 )
```

