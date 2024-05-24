# Comparing `tmp/celery-debug-0.1.2.tar.gz` & `tmp/celery-debug-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery-debug-0.1.2.tar", last modified: Sat May 18 00:01:26 2024, max compression
+gzip compressed data, was "celery-debug-0.1.3.tar", last modified: Fri May 24 14:42:39 2024, max compression
```

## Comparing `celery-debug-0.1.2.tar` & `celery-debug-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-18 00:01:26.526633 celery-debug-0.1.2/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-17 12:58:21.000000 celery-debug-0.1.2/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      156 2024-05-17 23:15:59.000000 celery-debug-0.1.2/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     1680 2024-05-18 00:01:26.526506 celery-debug-0.1.2/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1083 2024-05-17 23:55:32.000000 celery-debug-0.1.2/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-18 00:01:26.525576 celery-debug-0.1.2/celery_debug/
--rw-r--r--   0 test       (501) staff       (20)        0 2024-05-17 23:38:36.000000 celery-debug-0.1.2/celery_debug/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      249 2024-05-17 23:40:08.000000 celery-debug-0.1.2/celery_debug/app.py
--rw-r--r--   0 test       (501) staff       (20)      198 2024-05-17 23:40:18.000000 celery-debug-0.1.2/celery_debug/tasks.py
--rw-r--r--   0 test       (501) staff       (20)     1483 2024-05-17 23:33:44.000000 celery-debug-0.1.2/celery_debug/utils.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-18 00:01:26.526310 celery-debug-0.1.2/celery_debug.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     1680 2024-05-18 00:01:26.000000 celery-debug-0.1.2/celery_debug.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      358 2024-05-18 00:01:26.000000 celery-debug-0.1.2/celery_debug.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-18 00:01:26.000000 celery-debug-0.1.2/celery_debug.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-18 00:01:26.000000 celery-debug-0.1.2/celery_debug.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)        7 2024-05-18 00:01:26.000000 celery-debug-0.1.2/celery_debug.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       13 2024-05-18 00:01:26.000000 celery-debug-0.1.2/celery_debug.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)        7 2024-05-17 12:58:30.000000 celery-debug-0.1.2/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-05-18 00:01:26.526678 celery-debug-0.1.2/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1186 2024-05-17 23:55:40.000000 celery-debug-0.1.2/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-24 14:42:39.108244 celery-debug-0.1.3/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-17 12:58:21.000000 celery-debug-0.1.3/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      156 2024-05-17 23:15:59.000000 celery-debug-0.1.3/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     2067 2024-05-24 14:42:39.108121 celery-debug-0.1.3/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1470 2024-05-24 14:42:15.000000 celery-debug-0.1.3/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-24 14:42:39.107170 celery-debug-0.1.3/celery_debug/
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-05-17 23:38:36.000000 celery-debug-0.1.3/celery_debug/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      249 2024-05-17 23:40:08.000000 celery-debug-0.1.3/celery_debug/app.py
+-rw-r--r--   0 test       (501) staff       (20)      762 2024-05-24 14:36:34.000000 celery-debug-0.1.3/celery_debug/tasks.py
+-rw-r--r--   0 test       (501) staff       (20)     1643 2024-05-24 14:31:47.000000 celery-debug-0.1.3/celery_debug/utils.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-24 14:42:39.107955 celery-debug-0.1.3/celery_debug.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     2067 2024-05-24 14:42:39.000000 celery-debug-0.1.3/celery_debug.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      358 2024-05-24 14:42:39.000000 celery-debug-0.1.3/celery_debug.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-24 14:42:39.000000 celery-debug-0.1.3/celery_debug.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-24 14:42:39.000000 celery-debug-0.1.3/celery_debug.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)        7 2024-05-24 14:42:39.000000 celery-debug-0.1.3/celery_debug.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       13 2024-05-24 14:42:39.000000 celery-debug-0.1.3/celery_debug.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)        7 2024-05-17 12:58:30.000000 celery-debug-0.1.3/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-24 14:42:39.108287 celery-debug-0.1.3/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1186 2024-05-24 14:32:11.000000 celery-debug-0.1.3/setup.py
```

### Comparing `celery-debug-0.1.2/LICENSE` & `celery-debug-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `celery-debug-0.1.2/PKG-INFO` & `celery-debug-0.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-debug
-Version: 0.1.2
+Version: 0.1.3
 Summary: celery debug tasks.
 Home-page: UNKNOWN
 Author: Chen YuBo
 Maintainer: Chen YuBo
 License: MIT
 Keywords: celery debug tasks
 Platform: UNKNOWN
@@ -33,24 +33,31 @@
 - debug.echo
 
 ## 启动
 
 1. 在工作目录下创建`celeryconfig.py`，添加以下内容
 
     ```python
+    # concurrency
     worker_concurrency = 10
     worker_pool = "threads"
+    # broker_url and result_backend
     broker_url = "redis://redis/0"
     result_backend = "redis://redis/1"
+    # internal configs
     accept_content = ["application/json"]
     task_serializer = "json"
     result_accept_content = ["application/json"]
     result_serializer = "json"
     timezone = "Asia/Shanghai"
     broker_connection_retry_on_startup = True
+    task_track_started = True
+    task_acks_late = True
+    task_acks_on_failure_or_timeout = True
+    task_reject_on_worker_lost = True
     # 额外新增的配置项
     # 配置后所有任务都使用不同的队列
     use_different_queue = True
     ```
 
 2. 使用以下命令启动celery worker
 
@@ -68,8 +75,15 @@
 
 - 提供配置项，快速让所有任务都使用不同的队列。
 
 ### v0.1.2
 
 - use_different_queue方法做成工具函数。让用户自主控制，避免一引入就强制设置。
 
+### v0.1.3
+
+- `use_different_queue`自动绑定`celery`消息队列。
+- 添加`deubg.sleep`任务。
+- 添加`debug.raise_error`任务。
+- 添加`debug.retry_n`任务。
+
```

### Comparing `celery-debug-0.1.2/celery_debug/utils.py` & `celery-debug-0.1.3/celery_debug/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from kombu import Queue
 from kombu import Exchange
 
 
 def use_different_queue(app):
     """设置每个任务都使用不同的队列。"""
     logging.info("let CELERY use a different queue for each task...")
+
     # 处理没有task_routes预设置的情况
     if app.conf.task_routes is None:
         app.conf.task_routes = {}
     # 处理task_routes预设置为tuple的情况
     if isinstance(app.conf.task_routes, tuple):
         app.conf.task_routes = list(app.conf.task_routes)
         # 处理task_routes预设置为tuple但没有添加有效
@@ -36,7 +37,12 @@
                 app.conf.task_routes[0][0].append(
                     (task_name, {"queue": task_name}),
                 )
 
         app.conf.task_queues.append(
             Queue(task_name, Exchange(task_name, type="direct"), routing_key=task_name),
         )
+
+    # 绑定celery默认消息队列
+    app.conf.task_queues.append(
+        Queue("celery", Exchange("celery", type="direct"), routing_key="celery"),
+    )
```

### Comparing `celery-debug-0.1.2/celery_debug.egg-info/PKG-INFO` & `celery-debug-0.1.3/celery_debug.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-debug
-Version: 0.1.2
+Version: 0.1.3
 Summary: celery debug tasks.
 Home-page: UNKNOWN
 Author: Chen YuBo
 Maintainer: Chen YuBo
 License: MIT
 Keywords: celery debug tasks
 Platform: UNKNOWN
@@ -33,24 +33,31 @@
 - debug.echo
 
 ## 启动
 
 1. 在工作目录下创建`celeryconfig.py`，添加以下内容
 
     ```python
+    # concurrency
     worker_concurrency = 10
     worker_pool = "threads"
+    # broker_url and result_backend
     broker_url = "redis://redis/0"
     result_backend = "redis://redis/1"
+    # internal configs
     accept_content = ["application/json"]
     task_serializer = "json"
     result_accept_content = ["application/json"]
     result_serializer = "json"
     timezone = "Asia/Shanghai"
     broker_connection_retry_on_startup = True
+    task_track_started = True
+    task_acks_late = True
+    task_acks_on_failure_or_timeout = True
+    task_reject_on_worker_lost = True
     # 额外新增的配置项
     # 配置后所有任务都使用不同的队列
     use_different_queue = True
     ```
 
 2. 使用以下命令启动celery worker
 
@@ -68,8 +75,15 @@
 
 - 提供配置项，快速让所有任务都使用不同的队列。
 
 ### v0.1.2
 
 - use_different_queue方法做成工具函数。让用户自主控制，避免一引入就强制设置。
 
+### v0.1.3
+
+- `use_different_queue`自动绑定`celery`消息队列。
+- 添加`deubg.sleep`任务。
+- 添加`debug.raise_error`任务。
+- 添加`debug.retry_n`任务。
+
```

### Comparing `celery-debug-0.1.2/setup.py` & `celery-debug-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="celery-debug",
-    version="0.1.2",
+    version="0.1.3",
     description="celery debug tasks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Chen YuBo",
     maintainer="Chen YuBo",
     license="MIT",
     classifiers=[
```

