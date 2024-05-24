# Comparing `tmp/tamqp-0.0.8.tar.gz` & `tmp/tamqp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamqp-0.0.8.tar", last modified: Mon Jan 29 18:26:47 2024, max compression
+gzip compressed data, was "tamqp-0.0.9.tar", last modified: Fri May 24 17:49:59 2024, max compression
```

## Comparing `tamqp-0.0.8.tar` & `tamqp-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-01-29 18:26:47.051080 tamqp-0.0.8/
--rw-r--r--   0 tyeou      (501) staff       (20)      448 2024-01-29 18:26:47.050894 tamqp-0.0.8/PKG-INFO
--rw-r--r--   0 tyeou      (501) staff       (20)       38 2024-01-29 18:26:47.051124 tamqp-0.0.8/setup.cfg
--rw-r--r--   0 tyeou      (501) staff       (20)      584 2024-01-29 18:26:07.000000 tamqp-0.0.8/setup.py
-drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-01-29 18:26:47.045938 tamqp-0.0.8/tamqp/
--rw-r--r--   0 tyeou      (501) staff       (20)      225 2024-01-29 18:26:12.000000 tamqp-0.0.8/tamqp/__init__.py
-drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-01-29 18:26:47.046730 tamqp-0.0.8/tamqp/consumers/
--rw-r--r--   0 tyeou      (501) staff       (20)        0 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/consumers/__init__.py
--rw-r--r--   0 tyeou      (501) staff       (20)     1760 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/consumers/job_consumer.py
-drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-01-29 18:26:47.047769 tamqp-0.0.8/tamqp/consumers/models/
--rw-r--r--   0 tyeou      (501) staff       (20)        0 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/consumers/models/__init__.py
--rw-r--r--   0 tyeou      (501) staff       (20)     1290 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/consumers/models/communication_model.py
--rw-r--r--   0 tyeou      (501) staff       (20)      151 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/consumers/models/communication_object.py
--rw-r--r--   0 tyeou      (501) staff       (20)      317 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/consumers/models/test_model.py
--rw-r--r--   0 tyeou      (501) staff       (20)      339 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/consumers/models/test_publish_model.py
-drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-01-29 18:26:47.048508 tamqp-0.0.8/tamqp/exceptions/
--rw-r--r--   0 tyeou      (501) staff       (20)        0 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/exceptions/__init__.py
--rw-r--r--   0 tyeou      (501) staff       (20)      122 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/exceptions/channel_creation_exception.py
--rw-r--r--   0 tyeou      (501) staff       (20)      124 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/exceptions/connection_refused_exception.py
--rw-r--r--   0 tyeou      (501) staff       (20)      121 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/exceptions/enrolling_queue_exception.py
--rw-r--r--   0 tyeou      (501) staff       (20)      121 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/exceptions/publish_message_exception.py
--rw-r--r--   0 tyeou      (501) staff       (20)      119 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/exceptions/queue_declare_exception.py
-drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-01-29 18:26:47.049143 tamqp-0.0.8/tamqp/models/
--rw-r--r--   0 tyeou      (501) staff       (20)        0 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/models/__init__.py
--rw-r--r--   0 tyeou      (501) staff       (20)     1527 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/models/amqp_init.py
--rw-r--r--   0 tyeou      (501) staff       (20)      348 2024-01-15 18:10:23.000000 tamqp-0.0.8/tamqp/models/communication_wrapper.py
--rw-r--r--   0 tyeou      (501) staff       (20)     1522 2024-01-15 18:10:24.000000 tamqp-0.0.8/tamqp/models/rabbit_library.py
--rw-r--r--   0 tyeou      (501) staff       (20)      338 2024-01-15 18:10:24.000000 tamqp-0.0.8/tamqp/models/retry_queue.py
-drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-01-29 18:26:47.050449 tamqp-0.0.8/tamqp/services/
--rw-r--r--   0 tyeou      (501) staff       (20)        0 2024-01-15 18:10:24.000000 tamqp-0.0.8/tamqp/services/__init__.py
--rw-r--r--   0 tyeou      (501) staff       (20)     1752 2024-01-15 19:42:32.000000 tamqp-0.0.8/tamqp/services/amqp.py
--rw-r--r--   0 tyeou      (501) staff       (20)    12339 2024-01-16 16:54:17.000000 tamqp-0.0.8/tamqp/services/amqp_provider.py
--rw-r--r--   0 tyeou      (501) staff       (20)      829 2024-01-15 18:10:24.000000 tamqp-0.0.8/tamqp/services/amqp_provider_config.py
--rw-r--r--   0 tyeou      (501) staff       (20)      985 2024-01-29 18:25:42.000000 tamqp-0.0.8/tamqp/services/amqp_utils.py
--rw-r--r--   0 tyeou      (501) staff       (20)     1044 2024-01-15 18:10:24.000000 tamqp-0.0.8/tamqp/services/encoded_provider.py
-drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-01-29 18:26:47.050704 tamqp-0.0.8/tamqp/utils/
--rw-r--r--   0 tyeou      (501) staff       (20)        0 2024-01-15 18:10:24.000000 tamqp-0.0.8/tamqp/utils/__init__.py
--rw-r--r--   0 tyeou      (501) staff       (20)      586 2024-01-15 18:10:24.000000 tamqp-0.0.8/tamqp/utils/string_decoder.py
-drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-01-29 18:26:47.046514 tamqp-0.0.8/tamqp.egg-info/
--rw-r--r--   0 tyeou      (501) staff       (20)      448 2024-01-29 18:26:47.000000 tamqp-0.0.8/tamqp.egg-info/PKG-INFO
--rw-r--r--   0 tyeou      (501) staff       (20)     1088 2024-01-29 18:26:47.000000 tamqp-0.0.8/tamqp.egg-info/SOURCES.txt
--rw-r--r--   0 tyeou      (501) staff       (20)        1 2024-01-29 18:26:47.000000 tamqp-0.0.8/tamqp.egg-info/dependency_links.txt
--rw-r--r--   0 tyeou      (501) staff       (20)       12 2024-01-29 18:26:47.000000 tamqp-0.0.8/tamqp.egg-info/requires.txt
--rw-r--r--   0 tyeou      (501) staff       (20)        6 2024-01-29 18:26:47.000000 tamqp-0.0.8/tamqp.egg-info/top_level.txt
+drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-05-24 17:49:59.891867 tamqp-0.0.9/
+-rw-r--r--   0 tyeou      (501) staff       (20)      448 2024-05-24 17:49:59.891648 tamqp-0.0.9/PKG-INFO
+-rw-r--r--   0 tyeou      (501) staff       (20)       38 2024-05-24 17:49:59.891950 tamqp-0.0.9/setup.cfg
+-rw-r--r--   0 tyeou      (501) staff       (20)      584 2024-05-23 17:12:08.000000 tamqp-0.0.9/setup.py
+drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-05-24 17:49:59.862566 tamqp-0.0.9/tamqp/
+-rw-r--r--   0 tyeou      (501) staff       (20)      225 2024-05-23 17:11:22.000000 tamqp-0.0.9/tamqp/__init__.py
+drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-05-24 17:49:59.866406 tamqp-0.0.9/tamqp/consumers/
+-rw-r--r--   0 tyeou      (501) staff       (20)        0 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/consumers/__init__.py
+-rw-r--r--   0 tyeou      (501) staff       (20)     1760 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/consumers/job_consumer.py
+drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-05-24 17:49:59.875236 tamqp-0.0.9/tamqp/consumers/models/
+-rw-r--r--   0 tyeou      (501) staff       (20)        0 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/consumers/models/__init__.py
+-rw-r--r--   0 tyeou      (501) staff       (20)     1290 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/consumers/models/communication_model.py
+-rw-r--r--   0 tyeou      (501) staff       (20)      151 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/consumers/models/communication_object.py
+-rw-r--r--   0 tyeou      (501) staff       (20)      317 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/consumers/models/test_model.py
+-rw-r--r--   0 tyeou      (501) staff       (20)      339 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/consumers/models/test_publish_model.py
+drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-05-24 17:49:59.878784 tamqp-0.0.9/tamqp/exceptions/
+-rw-r--r--   0 tyeou      (501) staff       (20)        0 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/exceptions/__init__.py
+-rw-r--r--   0 tyeou      (501) staff       (20)      122 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/exceptions/channel_creation_exception.py
+-rw-r--r--   0 tyeou      (501) staff       (20)      124 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/exceptions/connection_refused_exception.py
+-rw-r--r--   0 tyeou      (501) staff       (20)      121 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/exceptions/enrolling_queue_exception.py
+-rw-r--r--   0 tyeou      (501) staff       (20)      121 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/exceptions/publish_message_exception.py
+-rw-r--r--   0 tyeou      (501) staff       (20)      119 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/exceptions/queue_declare_exception.py
+drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-05-24 17:49:59.883096 tamqp-0.0.9/tamqp/models/
+-rw-r--r--   0 tyeou      (501) staff       (20)        0 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/models/__init__.py
+-rw-r--r--   0 tyeou      (501) staff       (20)     1527 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/models/amqp_init.py
+-rw-r--r--   0 tyeou      (501) staff       (20)      348 2024-01-15 18:10:23.000000 tamqp-0.0.9/tamqp/models/communication_wrapper.py
+-rw-r--r--   0 tyeou      (501) staff       (20)     1631 2024-05-23 16:29:40.000000 tamqp-0.0.9/tamqp/models/rabbit_library.py
+-rw-r--r--   0 tyeou      (501) staff       (20)      338 2024-01-15 18:10:24.000000 tamqp-0.0.9/tamqp/models/retry_queue.py
+drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-05-24 17:49:59.890231 tamqp-0.0.9/tamqp/services/
+-rw-r--r--   0 tyeou      (501) staff       (20)        0 2024-01-15 18:10:24.000000 tamqp-0.0.9/tamqp/services/__init__.py
+-rw-r--r--   0 tyeou      (501) staff       (20)     1752 2024-01-15 19:42:32.000000 tamqp-0.0.9/tamqp/services/amqp.py
+-rw-r--r--   0 tyeou      (501) staff       (20)    12339 2024-01-16 16:54:17.000000 tamqp-0.0.9/tamqp/services/amqp_provider.py
+-rw-r--r--   0 tyeou      (501) staff       (20)      829 2024-01-15 18:10:24.000000 tamqp-0.0.9/tamqp/services/amqp_provider_config.py
+-rw-r--r--   0 tyeou      (501) staff       (20)      985 2024-01-29 18:25:42.000000 tamqp-0.0.9/tamqp/services/amqp_utils.py
+-rw-r--r--   0 tyeou      (501) staff       (20)     1044 2024-01-15 18:10:24.000000 tamqp-0.0.9/tamqp/services/encoded_provider.py
+drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-05-24 17:49:59.891149 tamqp-0.0.9/tamqp/utils/
+-rw-r--r--   0 tyeou      (501) staff       (20)        0 2024-01-15 18:10:24.000000 tamqp-0.0.9/tamqp/utils/__init__.py
+-rw-r--r--   0 tyeou      (501) staff       (20)      586 2024-01-15 18:10:24.000000 tamqp-0.0.9/tamqp/utils/string_decoder.py
+drwxr-xr-x   0 tyeou      (501) staff       (20)        0 2024-05-24 17:49:59.863666 tamqp-0.0.9/tamqp.egg-info/
+-rw-r--r--   0 tyeou      (501) staff       (20)      448 2024-05-24 17:49:59.000000 tamqp-0.0.9/tamqp.egg-info/PKG-INFO
+-rw-r--r--   0 tyeou      (501) staff       (20)     1088 2024-05-24 17:49:59.000000 tamqp-0.0.9/tamqp.egg-info/SOURCES.txt
+-rw-r--r--   0 tyeou      (501) staff       (20)        1 2024-05-24 17:49:59.000000 tamqp-0.0.9/tamqp.egg-info/dependency_links.txt
+-rw-r--r--   0 tyeou      (501) staff       (20)       12 2024-05-24 17:49:59.000000 tamqp-0.0.9/tamqp.egg-info/requires.txt
+-rw-r--r--   0 tyeou      (501) staff       (20)        6 2024-05-24 17:49:59.000000 tamqp-0.0.9/tamqp.egg-info/top_level.txt
```

### Comparing `tamqp-0.0.8/setup.py` & `tamqp-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tamqp',
-    version='0.0.8',
+    version='0.0.9',
     description='Adaptable Python library to interact with cloud RabbitMQ providers',
     url='https://s-g@bitbucket.org/yployalty/tamqp',
     author='Saurabh Gupta',
     author_email='sgupta@taekus.com',
     license='GNU General Public License v3.0',
     packages=find_packages(),
     install_requires=['pika==1.3.2', ],
```

### Comparing `tamqp-0.0.8/tamqp/consumers/job_consumer.py` & `tamqp-0.0.9/tamqp/consumers/job_consumer.py`

 * *Files identical despite different names*

### Comparing `tamqp-0.0.8/tamqp/consumers/models/communication_model.py` & `tamqp-0.0.9/tamqp/consumers/models/communication_model.py`

 * *Files identical despite different names*

### Comparing `tamqp-0.0.8/tamqp/models/amqp_init.py` & `tamqp-0.0.9/tamqp/models/amqp_init.py`

 * *Files identical despite different names*

### Comparing `tamqp-0.0.8/tamqp/models/rabbit_library.py` & `tamqp-0.0.9/tamqp/models/rabbit_library.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 class ExchangeType(Enum):
     TOPIC = "topic"
     HEADERS = "headers"
     FANOUT = "fanout"
     DIRECT = "direct"
+    DELAY = "x-delayed-message" # https://www.rabbitmq.com/blog/2015/04/16/scheduling-messages-with-rabbitmq
 
     def exchange_type_to_string(self) -> str:
         return self.value
 
 
 class Exchange:
     def __init__(
```

### Comparing `tamqp-0.0.8/tamqp/services/amqp.py` & `tamqp-0.0.9/tamqp/services/amqp.py`

 * *Files identical despite different names*

### Comparing `tamqp-0.0.8/tamqp/services/amqp_provider.py` & `tamqp-0.0.9/tamqp/services/amqp_provider.py`

 * *Files identical despite different names*

### Comparing `tamqp-0.0.8/tamqp/services/amqp_provider_config.py` & `tamqp-0.0.9/tamqp/services/amqp_provider_config.py`

 * *Files identical despite different names*

### Comparing `tamqp-0.0.8/tamqp/services/amqp_utils.py` & `tamqp-0.0.9/tamqp/services/amqp_utils.py`

 * *Files identical despite different names*

### Comparing `tamqp-0.0.8/tamqp/services/encoded_provider.py` & `tamqp-0.0.9/tamqp/services/encoded_provider.py`

 * *Files identical despite different names*

### Comparing `tamqp-0.0.8/tamqp/utils/string_decoder.py` & `tamqp-0.0.9/tamqp/utils/string_decoder.py`

 * *Files identical despite different names*

### Comparing `tamqp-0.0.8/tamqp.egg-info/SOURCES.txt` & `tamqp-0.0.9/tamqp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

