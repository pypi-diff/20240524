# Comparing `tmp/ibind-0.1.1.tar.gz` & `tmp/ibind-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibind-0.1.1.tar", last modified: Sat May 18 04:44:43 2024, max compression
+gzip compressed data, was "ibind-0.1.2.tar", last modified: Fri May 24 15:54:18 2024, max compression
```

## Comparing `ibind-0.1.1.tar` & `ibind-0.1.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.344050 ibind-0.1.1/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    22426 2024-05-18 04:44:43.341050 ibind-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     8341 2024-05-06 13:31:55.000000 ibind-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.166744 ibind-0.1.1/ibind/
--rw-rw-rw-   0        0        0     1062 2024-05-02 11:52:19.000000 ibind-0.1.1/ibind/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.205834 ibind-0.1.1/ibind/base/
--rw-rw-rw-   0        0        0        0 2024-04-04 04:03:06.000000 ibind-0.1.1/ibind/base/__init__.py
--rw-rw-rw-   0        0        0     5286 2024-05-02 07:49:30.000000 ibind-0.1.1/ibind/base/queue_controller.py
--rw-rw-rw-   0        0        0     8555 2024-05-03 06:26:53.000000 ibind-0.1.1/ibind/base/rest_client.py
--rw-rw-rw-   0        0        0    16433 2024-05-03 05:09:05.000000 ibind-0.1.1/ibind/base/subscription_controller.py
--rw-rw-rw-   0        0        0    18799 2024-05-02 07:52:05.000000 ibind-0.1.1/ibind/base/ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.224300 ibind-0.1.1/ibind/client/
--rw-rw-rw-   0        0        0        0 2024-04-03 12:59:53.000000 ibind-0.1.1/ibind/client/__init__.py
--rw-rw-rw-   0        0        0     3653 2024-05-03 03:15:23.000000 ibind-0.1.1/ibind/client/ibkr_client.py
-drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.261037 ibind-0.1.1/ibind/client/ibkr_client_mixins/
--rw-rw-rw-   0        0        0        0 2024-04-04 04:14:49.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/__init__.py
--rw-rw-rw-   0        0        0     3400 2024-05-02 04:33:53.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/accounts_mixin.py
--rw-rw-rw-   0        0        0    16134 2024-05-03 09:06:05.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/contract_mixin.py
--rw-rw-rw-   0        0        0    12514 2024-05-18 03:10:13.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/marketdata_mixin.py
--rw-rw-rw-   0        0        0    10477 2024-05-02 10:28:02.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/order_mixin.py
--rw-rw-rw-   0        0        0     9585 2024-05-02 10:28:35.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/portfolio_mixin.py
--rw-rw-rw-   0        0        0     4220 2024-05-02 10:28:35.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/scanner_mixin.py
--rw-rw-rw-   0        0        0     4611 2024-05-02 10:28:43.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/session_mixin.py
--rw-rw-rw-   0        0        0     2343 2024-05-02 10:30:13.000000 ibind-0.1.1/ibind/client/ibkr_client_mixins/watchlist_mixin.py
--rw-rw-rw-   0        0        0    12413 2024-04-24 12:43:26.000000 ibind-0.1.1/ibind/client/ibkr_definitions.py
--rw-rw-rw-   0        0        0    16278 2024-05-02 06:20:14.000000 ibind-0.1.1/ibind/client/ibkr_utils.py
--rw-rw-rw-   0        0        0    28501 2024-05-03 06:27:53.000000 ibind-0.1.1/ibind/client/ibkr_ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.276085 ibind-0.1.1/ibind/support/
--rw-rw-rw-   0        0        0        0 2024-04-03 13:00:28.000000 ibind-0.1.1/ibind/support/__init__.py
--rw-rw-rw-   0        0        0      227 2024-04-01 07:18:14.000000 ibind-0.1.1/ibind/support/errors.py
--rw-rw-rw-   0        0        0     5612 2024-05-02 10:37:05.000000 ibind-0.1.1/ibind/support/logs.py
--rw-rw-rw-   0        0        0    11297 2024-05-03 05:07:31.000000 ibind-0.1.1/ibind/support/py_utils.py
--rw-rw-rw-   0        0        0     2035 2024-04-25 10:00:26.000000 ibind-0.1.1/ibind/var.py
-drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.338053 ibind-0.1.1/ibind.egg-info/
--rw-rw-rw-   0        0        0    22426 2024-05-18 04:44:43.000000 ibind-0.1.1/ibind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1595 2024-05-18 04:44:43.000000 ibind-0.1.1/ibind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 04:44:43.000000 ibind-0.1.1/ibind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-18 04:44:43.000000 ibind-0.1.1/ibind.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-18 04:44:43.000000 ibind-0.1.1/ibind.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2024-05-18 04:44:15.000000 ibind-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-05-18 04:44:43.346049 ibind-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      225 2024-05-02 11:52:19.000000 ibind-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.283088 ibind-0.1.1/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.1.1/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.287609 ibind-0.1.1/test/integration/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.1.1/test/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.302129 ibind-0.1.1/test/integration/base/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.1.1/test/integration/base/__init__.py
--rw-rw-rw-   0        0        0     3714 2024-04-03 12:45:17.000000 ibind-0.1.1/test/integration/base/test_rest_client_i.py
--rw-rw-rw-   0        0        0    11025 2024-04-24 10:05:09.000000 ibind-0.1.1/test/integration/base/test_websocket_client_i.py
--rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.1.1/test/integration/base/websocketapp_mock.py
-drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.321709 ibind-0.1.1/test/integration/client/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.1.1/test/integration/client/__init__.py
--rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.1.1/test/integration/client/ibkr_responses.py
--rw-rw-rw-   0        0        0    14441 2024-04-25 11:38:46.000000 ibind-0.1.1/test/integration/client/test_ibkr_client_i.py
--rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.1.1/test/integration/client/test_ibkr_utils_i.py
--rw-rw-rw-   0        0        0    19149 2024-05-03 06:23:26.000000 ibind-0.1.1/test/integration/client/test_ibkr_ws_client_i.py
--rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.1.1/test/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.325710 ibind-0.1.1/test/unit/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.1.1/test/unit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 04:44:43.331814 ibind-0.1.1/test/unit/support/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.1.1/test/unit/support/__init__.py
--rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.1.1/test/unit/support/test_py_utils_u.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:18.777765 ibind-0.1.2/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    22426 2024-05-24 15:54:18.775766 ibind-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8341 2024-05-06 13:31:55.000000 ibind-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:18.591465 ibind-0.1.2/ibind/
+-rw-rw-rw-   0        0        0     1062 2024-05-02 11:52:19.000000 ibind-0.1.2/ibind/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:18.634472 ibind-0.1.2/ibind/base/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:03:06.000000 ibind-0.1.2/ibind/base/__init__.py
+-rw-rw-rw-   0        0        0     5286 2024-05-02 07:49:30.000000 ibind-0.1.2/ibind/base/queue_controller.py
+-rw-rw-rw-   0        0        0     8555 2024-05-03 06:26:53.000000 ibind-0.1.2/ibind/base/rest_client.py
+-rw-rw-rw-   0        0        0    16433 2024-05-03 05:09:05.000000 ibind-0.1.2/ibind/base/subscription_controller.py
+-rw-rw-rw-   0        0        0    18799 2024-05-02 07:52:05.000000 ibind-0.1.2/ibind/base/ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:18.659997 ibind-0.1.2/ibind/client/
+-rw-rw-rw-   0        0        0        0 2024-04-03 12:59:53.000000 ibind-0.1.2/ibind/client/__init__.py
+-rw-rw-rw-   0        0        0     3653 2024-05-03 03:15:23.000000 ibind-0.1.2/ibind/client/ibkr_client.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:18.699038 ibind-0.1.2/ibind/client/ibkr_client_mixins/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:14:49.000000 ibind-0.1.2/ibind/client/ibkr_client_mixins/__init__.py
+-rw-rw-rw-   0        0        0     3400 2024-05-02 04:33:53.000000 ibind-0.1.2/ibind/client/ibkr_client_mixins/accounts_mixin.py
+-rw-rw-rw-   0        0        0    16134 2024-05-03 09:06:05.000000 ibind-0.1.2/ibind/client/ibkr_client_mixins/contract_mixin.py
+-rw-rw-rw-   0        0        0    12522 2024-05-24 15:52:00.000000 ibind-0.1.2/ibind/client/ibkr_client_mixins/marketdata_mixin.py
+-rw-rw-rw-   0        0        0    10477 2024-05-02 10:28:02.000000 ibind-0.1.2/ibind/client/ibkr_client_mixins/order_mixin.py
+-rw-rw-rw-   0        0        0     9585 2024-05-02 10:28:35.000000 ibind-0.1.2/ibind/client/ibkr_client_mixins/portfolio_mixin.py
+-rw-rw-rw-   0        0        0     4220 2024-05-02 10:28:35.000000 ibind-0.1.2/ibind/client/ibkr_client_mixins/scanner_mixin.py
+-rw-rw-rw-   0        0        0     4611 2024-05-02 10:28:43.000000 ibind-0.1.2/ibind/client/ibkr_client_mixins/session_mixin.py
+-rw-rw-rw-   0        0        0     2343 2024-05-02 10:30:13.000000 ibind-0.1.2/ibind/client/ibkr_client_mixins/watchlist_mixin.py
+-rw-rw-rw-   0        0        0    12603 2024-05-20 08:55:57.000000 ibind-0.1.2/ibind/client/ibkr_definitions.py
+-rw-rw-rw-   0        0        0    16278 2024-05-02 06:20:14.000000 ibind-0.1.2/ibind/client/ibkr_utils.py
+-rw-rw-rw-   0        0        0    28501 2024-05-03 06:27:53.000000 ibind-0.1.2/ibind/client/ibkr_ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:18.714040 ibind-0.1.2/ibind/support/
+-rw-rw-rw-   0        0        0        0 2024-04-03 13:00:28.000000 ibind-0.1.2/ibind/support/__init__.py
+-rw-rw-rw-   0        0        0      227 2024-04-01 07:18:14.000000 ibind-0.1.2/ibind/support/errors.py
+-rw-rw-rw-   0        0        0     5612 2024-05-02 10:37:05.000000 ibind-0.1.2/ibind/support/logs.py
+-rw-rw-rw-   0        0        0    11297 2024-05-03 05:07:31.000000 ibind-0.1.2/ibind/support/py_utils.py
+-rw-rw-rw-   0        0        0     2035 2024-04-25 10:00:26.000000 ibind-0.1.2/ibind/var.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:18.772738 ibind-0.1.2/ibind.egg-info/
+-rw-rw-rw-   0        0        0    22426 2024-05-24 15:54:18.000000 ibind-0.1.2/ibind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1595 2024-05-24 15:54:18.000000 ibind-0.1.2/ibind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 15:54:18.000000 ibind-0.1.2/ibind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-24 15:54:18.000000 ibind-0.1.2/ibind.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-24 15:54:18.000000 ibind-0.1.2/ibind.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1038 2024-05-24 15:53:58.000000 ibind-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-05-24 15:54:18.779776 ibind-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      225 2024-05-02 11:52:19.000000 ibind-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:18.721042 ibind-0.1.2/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.1.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:18.724056 ibind-0.1.2/test/integration/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.1.2/test/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:18.738163 ibind-0.1.2/test/integration/base/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.1.2/test/integration/base/__init__.py
+-rw-rw-rw-   0        0        0     3714 2024-04-03 12:45:17.000000 ibind-0.1.2/test/integration/base/test_rest_client_i.py
+-rw-rw-rw-   0        0        0    11025 2024-04-24 10:05:09.000000 ibind-0.1.2/test/integration/base/test_websocket_client_i.py
+-rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.1.2/test/integration/base/websocketapp_mock.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:18.757689 ibind-0.1.2/test/integration/client/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.1.2/test/integration/client/__init__.py
+-rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.1.2/test/integration/client/ibkr_responses.py
+-rw-rw-rw-   0        0        0    14441 2024-04-25 11:38:46.000000 ibind-0.1.2/test/integration/client/test_ibkr_client_i.py
+-rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.1.2/test/integration/client/test_ibkr_utils_i.py
+-rw-rw-rw-   0        0        0    19149 2024-05-03 06:23:26.000000 ibind-0.1.2/test/integration/client/test_ibkr_ws_client_i.py
+-rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.1.2/test/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:18.761717 ibind-0.1.2/test/unit/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.1.2/test/unit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:18.767723 ibind-0.1.2/test/unit/support/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.1.2/test/unit/support/__init__.py
+-rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.1.2/test/unit/support/test_py_utils_u.py
```

### Comparing `ibind-0.1.1/LICENSE` & `ibind-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/PKG-INFO` & `ibind-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibind
-Version: 0.1.1
+Version: 0.1.2
 Summary: IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API.
 Author-email: Voy Zan <voy1982@yahoo.co.uk>
 License: Copyright 2020 Voy Zan
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ibind-0.1.1/README.md` & `ibind-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/__init__.py` & `ibind-0.1.2/ibind/__init__.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/base/queue_controller.py` & `ibind-0.1.2/ibind/base/queue_controller.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/base/rest_client.py` & `ibind-0.1.2/ibind/base/rest_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/base/subscription_controller.py` & `ibind-0.1.2/ibind/base/subscription_controller.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/base/ws_client.py` & `ibind-0.1.2/ibind/base/ws_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/client/ibkr_client.py` & `ibind-0.1.2/ibind/client/ibkr_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/client/ibkr_client_mixins/accounts_mixin.py` & `ibind-0.1.2/ibind/client/ibkr_client_mixins/accounts_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/client/ibkr_client_mixins/contract_mixin.py` & `ibind-0.1.2/ibind/client/ibkr_client_mixins/contract_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/client/ibkr_client_mixins/marketdata_mixin.py` & `ibind-0.1.2/ibind/client/ibkr_client_mixins/marketdata_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class MarketdataMixin():
     """
     https://ibkrcampus.com/ibkr-api-page/cpapi-v1/#md
     """
 
-    @ensure_list_arg('conids')
+    @ensure_list_arg('conids', 'fields')
     def live_marketdata_snapshot(self: 'IbkrClient', conids: OneOrMany[str], fields: OneOrMany[str]) -> Result:  # pragma: no cover
         """
         Get Market Data for the given conid(s).
 
         A pre-flight request must be made prior to ever receiving data.
 
         Parameters:
@@ -65,17 +65,17 @@
             start_time: datetime.datetime = None
     ) -> Result:  # pragma: no cover
         """
         Get historical market Data for given conid, length of data is controlled by 'period' and 'bar'.
 
         Parameters:
             conid (str): Contract identifier for the ticker symbol of interest.
+            bar (str): Individual bars of data to be returned. Possible values– 1min, 2min, 3min, 5min, 10min, 15min, 30min, 1h, 2h, 3h, 4h, 8h, 1d, 1w, 1m.
             exchange (str, optional): Returns the exchange you want to receive data from.
             period (str): Overall duration for which data should be returned. Default to 1w. Available time period– {1-30}min, {1-8}h, {1-1000}d, {1-792}w, {1-182}m, {1-15}y.
-            bar (str): Individual bars of data to be returned. Possible values– 1min, 2min, 3min, 5min, 10min, 15min, 30min, 1h, 2h, 3h, 4h, 8h, 1d, 1w, 1m.
             outside_rth (bool, optional): Determine if you want data after regular trading hours.
             start_time (datetime.datetime, optional): Starting date of the request duration.
 
         Note:
             - There's a limit of 5 concurrent requests. Excessive requests will return a 'Too many requests' status 429 response.
         """
         params = params_dict(
@@ -139,34 +139,34 @@
         )
 
         return self.get('hmds/history', params)
 
     def marketdata_history_by_symbol(
             self: 'IbkrClient',
             symbol: Union[str, StockQuery],
+            bar: str,
             exchange: str = None,
             period: str = None,
-            bar: str = None,
             outside_rth: bool = None,
             start_time: datetime.datetime = None,
     ) -> Result:  # pragma: no cover
         """
         Get historical market Data for given symbol, length of data is controlled by 'period' and 'bar'.
 
         Parameters:
             symbol (Union[str, StockQuery]): StockQuery or str symbol for the ticker of interest.
+            bar (str): Individual bars of data to be returned. Possible values– 1min, 2min, 3min, 5min, 10min, 15min, 30min, 1h, 2h, 3h, 4h, 8h, 1d, 1w, 1m.
             exchange (str, optional): Returns the exchange you want to receive data from.
             period (str): Overall duration for which data should be returned. Default to 1w. Available time period– {1-30}min, {1-8}h, {1-1000}d, {1-792}w, {1-182}m, {1-15}y.
-            bar (str): Individual bars of data to be returned. Possible values– 1min, 2min, 3min, 5min, 10min, 15min, 30min, 1h, 2h, 3h, 4h, 8h, 1d, 1w, 1m.
             outside_rth (bool, optional): Determine if you want data after regular trading hours.
             start_time (datetime.datetime, optional): Starting date of the request duration.
 
         """
-        conid = self.stock_conid_by_symbol(symbol).data[symbol]
-        return self.marketdata_history_by_conid(conid, exchange, period, bar, outside_rth, start_time)
+        conid = str(self.stock_conid_by_symbol(symbol).data[symbol])
+        return self.marketdata_history_by_conid(conid, bar, exchange, period, outside_rth, start_time)
 
     @ensure_list_arg('queries')
     def marketdata_history_by_symbols(
             self: 'IbkrClient',
             queries: StockQueries,
             period: str = "1min",
             bar: str = "1min",
```

### Comparing `ibind-0.1.1/ibind/client/ibkr_client_mixins/order_mixin.py` & `ibind-0.1.2/ibind/client/ibkr_client_mixins/order_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/client/ibkr_client_mixins/portfolio_mixin.py` & `ibind-0.1.2/ibind/client/ibkr_client_mixins/portfolio_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/client/ibkr_client_mixins/scanner_mixin.py` & `ibind-0.1.2/ibind/client/ibkr_client_mixins/scanner_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/client/ibkr_client_mixins/session_mixin.py` & `ibind-0.1.2/ibind/client/ibkr_client_mixins/session_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/client/ibkr_client_mixins/watchlist_mixin.py` & `ibind-0.1.2/ibind/client/ibkr_client_mixins/watchlist_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/client/ibkr_definitions.py` & `ibind-0.1.2/ibind/client/ibkr_definitions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,125 +1,125 @@
 """
 This file contains hard coded definitions of what various IBKR market data snapshot fields stand for.
 See: https://ibkrcampus.com/ibkr-api-page/cpapi-v1/#market-data-fields
 """
 
 snapshot_by_key = {
     # Contract
-    'symbol': 55,  # Symbol
-    'conid': 6008,  # Conid - Contract identifier from IBKR's database.
-    'sec_type': 6070,  # SecType - The asset class of the instrument.
-    'underlying_conid': 6457,  # Underlying Conid. Use /trsrv/secdef to get more information about the security
-    'market_data_availability': 6509,  # Market Data Availability. The field may contain three chars. First char defines: R = RealTime, D = Delayed, Z = Frozen, Y = Frozen Delayed, N = Not Subscribed. Second char defines: P = Snapshot, p = Consolidated. Third char defines: B = Book
-    'conid_exchange': 7094,  # Conid + Exchange
+    'symbol': '55',  # Symbol
+    'conid': '6008',  # Conid - Contract identifier from IBKR's database.
+    'sec_type': '6070',  # SecType - The asset class of the instrument.
+    'underlying_conid': '6457',  # Underlying Conid. Use /trsrv/secdef to get more information about the security
+    'market_data_availability': '6509',  # Market Data Availability. The field may contain three chars. First char defines: R = RealTime, D = Delayed, Z = Frozen, Y = Frozen Delayed, N = Not Subscribed. Second char defines: P = Snapshot, p = Consolidated. Third char defines: B = Book
+    'conid_exchange': '7094',  # Conid + Exchange
 
     # Price and Volume
-    'open': 7295,  # Open - Today's opening price.
-    'high': 70,  # High - Current day high price
-    'low': 71,  # Low - Current day low price
-    'close': 7296,  # Close - Today's closing price.
-    'last_price': 31,  # Last Price - The last price at which the contract traded. May contain one of the following prefixes: C - Previous day's closing price. H - Trading has halted.
-    'bid_price': 84,  # Bid Price - The highest-priced bid on the contract.
-    'ask_price': 86,  # Ask Price - The lowest-priced offer on the contract.
-    'bid_size': 88,  # Bid Size - The number of contracts or shares bid for at the bid price. For US stocks, the number displayed is divided by 100.
-    'ask_size': 85,  # Ask Size - The number of contracts or shares offered at the ask price. For US stocks, the number displayed is divided by 100.
-    'prior_close': 7741,  # Prior Close - Yesterday's closing price
-    'mark_price': 7635,  # Mark - The mark price is, the ask price if ask is less than last price, the bid price if bid is more than the last price, otherwise it's equal to last price.
-    'volume': 87,  # Volume - Volume for the day, formatted with 'K' for thousands or 'M' for millions. For higher precision volume refer to field 7762.
-    'volume_long': 7762,  # Volume Long - High precision volume for the day. For formatted volume refer to field 87.
-    'change': 82,  # Change - The difference between the last price and the close on the previous trading day
-    'change_since_open': 7682,  # Change Since Open - The difference between the last price and the open price.
-    'change_percent': 83,  # Change % - The difference between the last price and the close on the previous trading day in percentage.
+    'open': '7295',  # Open - Today's opening price.
+    'high': '70',  # High - Current day high price
+    'low': '71',  # Low - Current day low price
+    'close': '7296',  # Close - Today's closing price.
+    'last_price': '31',  # Last Price - The last price at which the contract traded. May contain one of the following prefixes: C - Previous day's closing price. H - Trading has halted.
+    'bid_price': '84',  # Bid Price - The highest-priced bid on the contract.
+    'ask_price': '86',  # Ask Price - The lowest-priced offer on the contract.
+    'bid_size': '88',  # Bid Size - The number of contracts or shares bid for at the bid price. For US stocks, the number displayed is divided by 100.
+    'ask_size': '85',  # Ask Size - The number of contracts or shares offered at the ask price. For US stocks, the number displayed is divided by 100.
+    'prior_close': '7741',  # Prior Close - Yesterday's closing price
+    'mark_price': '7635',  # Mark - The mark price is, the ask price if ask is less than last price, the bid price if bid is more than the last price, otherwise it's equal to last price.
+    'volume': '87',  # Volume - Volume for the day, formatted with 'K' for thousands or 'M' for millions. For higher precision volume refer to field 7762.
+    'volume_long': '7762',  # Volume Long - High precision volume for the day. For formatted volume refer to field 87.
+    'change': '82',  # Change - The difference between the last price and the close on the previous trading day
+    'change_since_open': '7682',  # Change Since Open - The difference between the last price and the open price.
+    'change_percent': '83',  # Change % - The difference between the last price and the close on the previous trading day in percentage.
 
     # Volatility
-    'implied_vol_hist_vol_percent': 7084,  # Implied Vol./Hist. Vol % - The ratio of the implied volatility over the historical volatility, expressed as a percentage.
-    'hist_vol_close_percent': 7088,  # Hist. Vol. Close % - Shows the historical volatility based on previous close price.
-    'spx_delta': 7696,  # SPX Delta - Beta Weighted Delta is calculated using the formula; Delta x dollar adjusted beta, where adjusted beta is adjusted by the ratio of the close price.
-    'beta': 7718,  # Beta - Beta is against standard index.
+    'implied_vol_hist_vol_percent': '7084',  # Implied Vol./Hist. Vol % - The ratio of the implied volatility over the historical volatility, expressed as a percentage.
+    'hist_vol_close_percent': '7088',  # Hist. Vol. Close % - Shows the historical volatility based on previous close price.
+    'spx_delta': '7696',  # SPX Delta - Beta Weighted Delta is calculated using the formula; Delta x dollar adjusted beta, where adjusted beta is adjusted by the ratio of the close price.
+    'beta': '7718',  # Beta - Beta is against standard index.
 
     # Financial Information
-    'hist_vol_percent': 7087,  # Hist. Vol. % - 30-day real-time historical volatility.
-    'average_volume_90': 7282,  # Average Volume - The average daily trading volume over 90 days.
-    'dividend_amount': 7286,  # Dividend Amount - Displays the amount of the next dividend.
-    'dividend_yield_percent': 7287,  # Dividend Yield % - This value is the total of the expected dividend payments over the next twelve months per share divided by the Current Price and is expressed as a percentage. For derivatives, this displays the total of the expected dividend payments over the expiry date.
-    'ex_date_dividend': 7288,  # Ex-date of the dividend
-    'market_cap': 7289,  # Market Cap
-    'p_e': 7290,  # P/E
-    'eps': 7291,  # EPS
-    '52_week_high': 7293,  # 52 Week High - The highest price for the past 52 weeks.
-    '52_week_low': 7294,  # 52 Week Low - The lowest price for the past 52 weeks.
-    'ema_200': 7674,  # EMA(200) - Exponential moving average (N=200).
-    'ema_100': 7675,  # EMA(100) - Exponential moving average (N=100).
-    'ema_50': 7676,  # EMA(50) - Exponential moving average (N=50).
-    'ema_20': 7677,  # EMA(20) - Exponential moving average (N=20).
-    'price_to_ema_200_percent': 7678,  # Price/EMA(200) - Price to Exponential moving average (N=200) ratio -1, displayed in percents.
-    'price_to_ema_100_percent': 7679,  # Price/EMA(100) - Price to Exponential moving average (N=100) ratio -1, displayed in percents.
-    'price_to_ema_50_percent': 7680,  # Price/EMA(50) - Price to Exponential moving average (N=50) ratio -1, displayed in percents.
-    'price_to_ema_20_percent': 7681,  # Price/EMA(20) - Price to Exponential moving average (N=20) ratio -1, displayed in percents.
+    'hist_vol_percent': '7087',  # Hist. Vol. % - 30-day real-time historical volatility.
+    'average_volume_90': '7282',  # Average Volume - The average daily trading volume over 90 days.
+    'dividend_amount': '7286',  # Dividend Amount - Displays the amount of the next dividend.
+    'dividend_yield_percent': '7287',  # Dividend Yield % - This value is the total of the expected dividend payments over the next twelve months per share divided by the Current Price and is expressed as a percentage. For derivatives, this displays the total of the expected dividend payments over the expiry date.
+    'ex_date_dividend': '7288',  # Ex-date of the dividend
+    'market_cap': '7289',  # Market Cap
+    'p_e': '7290',  # P/E
+    'eps': '7291',  # EPS
+    '52_week_high': '7293',  # 52 Week High - The highest price for the past 52 weeks.
+    '52_week_low': '7294',  # 52 Week Low - The lowest price for the past 52 weeks.
+    'ema_200': '7674',  # EMA(200) - Exponential moving average (N=200).
+    'ema_100': '7675',  # EMA(100) - Exponential moving average (N=100).
+    'ema_50': '7676',  # EMA(50) - Exponential moving average (N=50).
+    'ema_20': '7677',  # EMA(20) - Exponential moving average (N=20).
+    'price_to_ema_200_percent': '7678',  # Price/EMA(200) - Price to Exponential moving average (N=200) ratio -1, displayed in percents.
+    'price_to_ema_100_percent': '7679',  # Price/EMA(100) - Price to Exponential moving average (N=100) ratio -1, displayed in percents.
+    'price_to_ema_50_percent': '7680',  # Price/EMA(50) - Price to Exponential moving average (N=50) ratio -1, displayed in percents.
+    'price_to_ema_20_percent': '7681',  # Price/EMA(20) - Price to Exponential moving average (N=20) ratio -1, displayed in percents.
 
     # Portfolio
-    'market_value': 73,  # Market Value - The current market value of your position in the security. Market Value is calculated with real-time market data (even when not subscribed to market data).
-    'avg_price': 74,  # Avg Price - The average price of the position.
-    'unrealized_pnl': 75,  # Unrealized PnL - Unrealized profit or loss. Unrealized PnL is calculated with real-time market data (even when not subscribed to market data).
-    'formatted_position': 76,  # Formatted position
-    'formatted_unrealized_pnl': 77,  # Formatted Unrealized PnL
-    'daily_pnl': 78,  # Daily PnL - Your profit or loss of the day since prior close. Daily PnL is calculated with real-time market data (even when not subscribed to market data).
-    'realized_pnl': 79,  # Realized PnL - Realized profit or loss. Realized PnL is calculated with real-time market data (even when not subscribed to market data).
-    'unrealized_pnl_percent': 80,  # Unrealized PnL % - Unrealized profit or loss expressed in percentage.
-    'daily_pnl_raw': 7920,  # Daily PnL Raw - Your profit or loss of the day since prior close. Daily PnL is calculated with real-time market data (even when not subscribed to market data).
-    'cost_basis_raw': 7921,  # Cost Basis Raw - Your current position in this security multiplied by the average price and multiplier.
-    'cost_basis': 7292,  # Cost Basis - Your current position in this security multiplied by the average price and multiplier.
+    'market_value': '73',  # Market Value - The current market value of your position in the security. Market Value is calculated with real-time market data (even when not subscribed to market data).
+    'avg_price': '74',  # Avg Price - The average price of the position.
+    'unrealized_pnl': '75',  # Unrealized PnL - Unrealized profit or loss. Unrealized PnL is calculated with real-time market data (even when not subscribed to market data).
+    'formatted_position': '76',  # Formatted position
+    'formatted_unrealized_pnl': '77',  # Formatted Unrealized PnL
+    'daily_pnl': '78',  # Daily PnL - Your profit or loss of the day since prior close. Daily PnL is calculated with real-time market data (even when not subscribed to market data).
+    'realized_pnl': '79',  # Realized PnL - Realized profit or loss. Realized PnL is calculated with real-time market data (even when not subscribed to market data).
+    'unrealized_pnl_percent': '80',  # Unrealized PnL % - Unrealized profit or loss expressed in percentage.
+    'daily_pnl_raw': '7920',  # Daily PnL Raw - Your profit or loss of the day since prior close. Daily PnL is calculated with real-time market data (even when not subscribed to market data).
+    'cost_basis_raw': '7921',  # Cost Basis Raw - Your current position in this security multiplied by the average price and multiplier.
+    'cost_basis': '7292',  # Cost Basis - Your current position in this security multiplied by the average price and multiplier.
 
     # Company and Industry Information
-    'company_name': 7051,  # Company name
-    'exchange': 6004,  # Exchange
-    'listing_exchange': 7221,  # Listing Exchange
-    'industry': 7280,  # Industry - Displays the type of industry under which the underlying company can be categorized.
-    'category': 7281,  # Category - Displays a more detailed level of description within the industry under which the underlying company can be categorized.
-    'ratings': 7706,  # Ratings - Ratings issued for bond contract.
-    'bond_state_code': 7707,  # Bond State Code
-    'bond_type': 7708,  # Bond Type
-    'last_trading_date': 7714,  # Last Trading Date
-    'issue_date': 7715,  # Issue Date
-    'organization_type': 7704,  # Organization Type
-    'debt_class': 7705,  # Debt Class
+    'company_name': '7051',  # Company name
+    'exchange': '6004',  # Exchange
+    'listing_exchange': '7221',  # Listing Exchange
+    'industry': '7280',  # Industry - Displays the type of industry under which the underlying company can be categorized.
+    'category': '7281',  # Category - Displays a more detailed level of description within the industry under which the underlying company can be categorized.
+    'ratings': '7706',  # Ratings - Ratings issued for bond contract.
+    'bond_state_code': '7707',  # Bond State Code
+    'bond_type': '7708',  # Bond Type
+    'last_trading_date': '7714',  # Last Trading Date
+    'issue_date': '7715',  # Issue Date
+    'organization_type': '7704',  # Organization Type
+    'debt_class': '7705',  # Debt Class
 
     # Options and Futures
-    'opt_volume': 7089,  # Opt. Volume - Option Volume
-    'put_call_ratio': 7285,  # Put/Call Ratio
-    'option_open_interest': 7638,  # Option Open Interest
-    'percent_of_mark_value': 7639,  # % of Mark Value - Displays the market value of the contract as a percentage of the total market value of the account. Mark Value is calculated with real-time market data (even when not subscribed to market data).
-    'probability_of_max_return': 7694,  # Probability of Max Return - Customer implied probability of maximum potential gain.
-    'break_even': 7695,  # Break Even - Break even points
-    'probability_of_max_loss': 7702,  # Probability of Max Loss - Customer implied probability of maximum potential loss.
-    'profit_probability': 7703,  # Profit Probability - Customer implied probability of any gain.
-    'last_yield': 7698,  # Last Yield - Implied yield of the bond if it is purchased at the current last price. Last yield is calculated using the Last price on all possible call dates. It is assumed that prepayment occurs if the bond has call or put provisions and the issuer can offer a lower coupon rate based on current market rates. The yield to worst will be the lowest of the yield to maturity or yield to call (if the bond has prepayment provisions). Yield to worse may be the same as yield to maturity but never higher.
-    'bid_yield': 7699,  # Bid Yield - Implied yield of the bond if it is purchased at the current bid price. Bid yield is calculated using the Ask on all possible call dates. It is assumed that prepayment occurs if the bond has call or put provisions and the issuer can offer a lower coupon rate based on current market rates. The yield to worst will be the lowest of the yield to maturity or yield to call (if the bond has prepayment provisions). Yield to worse may be the same as yield to maturity but never higher.
-    'futures_open_interest': 7697,  # Futures Open Interest - Total number of outstanding futures contracts
-    'put_call_interest': 7085,  # Put/Call Interest - Put option open interest/call option open interest for the trading day.
-    'put_call_volume': 7086,  # Put/Call Volume - Put option volume/call option volume for the trading day.
-    'option_implied_vol_percent': 7283,  # Option Implied Vol. % - A prediction of how volatile an underlying will be in the future. At the market volatility estimated for a maturity thirty calendar days forward of the current trading day, and based on option prices from two consecutive expiration months. To query the Implied Vol. % of a specific strike refer to field 7633.
+    'opt_volume': '7089',  # Opt. Volume - Option Volume
+    'put_call_ratio': '7285',  # Put/Call Ratio
+    'option_open_interest': '7638',  # Option Open Interest
+    'percent_of_mark_value': '7639',  # % of Mark Value - Displays the market value of the contract as a percentage of the total market value of the account. Mark Value is calculated with real-time market data (even when not subscribed to market data).
+    'probability_of_max_return': '7694',  # Probability of Max Return - Customer implied probability of maximum potential gain.
+    'break_even': '7695',  # Break Even - Break even points
+    'probability_of_max_loss': '7702',  # Probability of Max Loss - Customer implied probability of maximum potential loss.
+    'profit_probability': '7703',  # Profit Probability - Customer implied probability of any gain.
+    'last_yield': '7698',  # Last Yield - Implied yield of the bond if it is purchased at the current last price. Last yield is calculated using the Last price on all possible call dates. It is assumed that prepayment occurs if the bond has call or put provisions and the issuer can offer a lower coupon rate based on current market rates. The yield to worst will be the lowest of the yield to maturity or yield to call (if the bond has prepayment provisions). Yield to worse may be the same as yield to maturity but never higher.
+    'bid_yield': '7699',  # Bid Yield - Implied yield of the bond if it is purchased at the current bid price. Bid yield is calculated using the Ask on all possible call dates. It is assumed that prepayment occurs if the bond has call or put provisions and the issuer can offer a lower coupon rate based on current market rates. The yield to worst will be the lowest of the yield to maturity or yield to call (if the bond has prepayment provisions). Yield to worse may be the same as yield to maturity but never higher.
+    'futures_open_interest': '7697',  # Futures Open Interest - Total number of outstanding futures contracts
+    'put_call_interest': '7085',  # Put/Call Interest - Put option open interest/call option open interest for the trading day.
+    'put_call_volume': '7086',  # Put/Call Volume - Put option volume/call option volume for the trading day.
+    'option_implied_vol_percent': '7283',  # Option Implied Vol. % - A prediction of how volatile an underlying will be in the future. At the market volatility estimated for a maturity thirty calendar days forward of the current trading day, and based on option prices from two consecutive expiration months. To query the Implied Vol. % of a specific strike refer to field 7633.
 
     # Wall Street Horizon
-    'upcoming_event': 7683,  # Upcoming Event - Shows the next major company event. Requires Wall Street Horizon subscription.
-    'upcoming_event_date': 7684,  # Upcoming Event Date - The date of the next major company event. Requires Wall Street Horizon subscription.
-    'upcoming_analyst_meeting': 7685,  # Upcoming Analyst Meeting - The date and time of the next scheduled analyst meeting. Requires Wall Street Horizon subscription.
-    'upcoming_earnings': 7686,  # Upcoming Earnings - The date and time of the next scheduled earnings/earnings call event. Requires Wall Street Horizon subscription.
-    'upcoming_misc_event': 7687,  # Upcoming Misc Event - The date and time of the next shareholder meeting, presentation, or other event. Requires Wall Street Horizon subscription.
-    'recent_analyst_meeting': 7688,  # Recent Analyst Meeting - The date and time of the most recent analyst meeting. Requires Wall Street Horizon subscription.
-    'recent_earnings': 7689,  # Recent Earnings - The date and time of the most recent earnings/earning call event. Requires Wall Street Horizon subscription.
-    'recent_misc_event': 7690,  # Recent Misc Event - The date and time of the most recent shareholder meeting, presentation, or other event. Requires Wall Street Horizon subscription.
+    'upcoming_event': '7683',  # Upcoming Event - Shows the next major company event. Requires Wall Street Horizon subscription.
+    'upcoming_event_date': '7684',  # Upcoming Event Date - The date of the next major company event. Requires Wall Street Horizon subscription.
+    'upcoming_analyst_meeting': '7685',  # Upcoming Analyst Meeting - The date and time of the next scheduled analyst meeting. Requires Wall Street Horizon subscription.
+    'upcoming_earnings': '7686',  # Upcoming Earnings - The date and time of the next scheduled earnings/earnings call event. Requires Wall Street Horizon subscription.
+    'upcoming_misc_event': '7687',  # Upcoming Misc Event - The date and time of the next shareholder meeting, presentation, or other event. Requires Wall Street Horizon subscription.
+    'recent_analyst_meeting': '7688',  # Recent Analyst Meeting - The date and time of the most recent analyst meeting. Requires Wall Street Horizon subscription.
+    'recent_earnings': '7689',  # Recent Earnings - The date and time of the most recent earnings/earning call event. Requires Wall Street Horizon subscription.
+    'recent_misc_event': '7690',  # Recent Misc Event - The date and time of the most recent shareholder meeting, presentation, or other event. Requires Wall Street Horizon subscription.
 
     # Miscellaneous
-    'shortable': 7644,  # Shortable - Describes the level of difficulty with which the security can be sold short.
-    'service_params': 6508,  # Service Params.
-    'market_data_marker': 6119,  # Marker for market data delivery method (similar to request id)
-    'months': 6072,  # Months
-    'regular_expiry': 6073,  # Regular Expiry
-    'has_trading_permissions': 7768,  # hasTradingPermissions - if the user has trading permissions for the specified contract. Returns 1(true) or 0(false).
+    'shortable': '7644',  # Shortable - Describes the level of difficulty with which the security can be sold short.
+    'service_params': '6508',  # Service Params.
+    'market_data_marker': '6119',  # Marker for market data delivery method (similar to request id)
+    'months': '6072',  # Months
+    'regular_expiry': '6073',  # Regular Expiry
+    'has_trading_permissions': '7768',  # hasTradingPermissions - if the user has trading permissions for the specified contract. Returns 1(true) or 0(false).
     'server_id': 'string',
     'conid_str': 'integer_str',
     '_updated_str': 'integer_str',
 }
 
 snapshot_by_id = {str(value): key for key, value in snapshot_by_key.items()}
```

### Comparing `ibind-0.1.1/ibind/client/ibkr_utils.py` & `ibind-0.1.2/ibind/client/ibkr_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/client/ibkr_ws_client.py` & `ibind-0.1.2/ibind/client/ibkr_ws_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/support/logs.py` & `ibind-0.1.2/ibind/support/logs.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/support/py_utils.py` & `ibind-0.1.2/ibind/support/py_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind/var.py` & `ibind-0.1.2/ibind/var.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/ibind.egg-info/PKG-INFO` & `ibind-0.1.2/ibind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibind
-Version: 0.1.1
+Version: 0.1.2
 Summary: IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API.
 Author-email: Voy Zan <voy1982@yahoo.co.uk>
 License: Copyright 2020 Voy Zan
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ibind-0.1.1/ibind.egg-info/SOURCES.txt` & `ibind-0.1.2/ibind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/pyproject.toml` & `ibind-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ibind"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name="Voy Zan", email="voy1982@yahoo.co.uk" },
 ]
 description = "IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API."
 readme = "README.md"
 requires-python = ">=3.8"
 license={ file = "LICENSE" }
```

### Comparing `ibind-0.1.1/test/integration/base/test_rest_client_i.py` & `ibind-0.1.2/test/integration/base/test_rest_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/test/integration/base/test_websocket_client_i.py` & `ibind-0.1.2/test/integration/base/test_websocket_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/test/integration/base/websocketapp_mock.py` & `ibind-0.1.2/test/integration/base/websocketapp_mock.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/test/integration/client/ibkr_responses.py` & `ibind-0.1.2/test/integration/client/ibkr_responses.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/test/integration/client/test_ibkr_client_i.py` & `ibind-0.1.2/test/integration/client/test_ibkr_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/test/integration/client/test_ibkr_utils_i.py` & `ibind-0.1.2/test/integration/client/test_ibkr_utils_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/test/integration/client/test_ibkr_ws_client_i.py` & `ibind-0.1.2/test/integration/client/test_ibkr_ws_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/test/test_utils.py` & `ibind-0.1.2/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.1.1/test/unit/support/test_py_utils_u.py` & `ibind-0.1.2/test/unit/support/test_py_utils_u.py`

 * *Files identical despite different names*

