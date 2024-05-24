# Comparing `tmp/coinbase-advanced-py-1.4.0.tar.gz` & `tmp/coinbase-advanced-py-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinbase-advanced-py-1.4.0.tar", last modified: Tue May 21 15:25:00 2024, max compression
+gzip compressed data, was "coinbase-advanced-py-1.4.1.tar", last modified: Fri May 24 15:47:24 2024, max compression
```

## Comparing `coinbase-advanced-py-1.4.0.tar` & `coinbase-advanced-py-1.4.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.580436 coinbase-advanced-py-1.4.0/
--rw-r--r--   0 urischwartz   (501) staff       (20)    11343 2023-12-07 15:44:33.000000 coinbase-advanced-py-1.4.0/LICENSE.md
--rw-r--r--   0 urischwartz   (501) staff       (20)    17519 2024-05-21 15:25:00.580057 coinbase-advanced-py-1.4.0/PKG-INFO
--rw-r--r--   0 urischwartz   (501) staff       (20)    16405 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/README.md
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.565272 coinbase-advanced-py-1.4.0/coinbase/
--rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-11-21 15:58:27.000000 coinbase-advanced-py-1.4.0/coinbase/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)       22 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/__version__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2169 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/coinbase/api_base.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      773 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/coinbase/constants.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2350 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.4.0/coinbase/jwt_generator.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.569720 coinbase-advanced-py-1.4.0/coinbase/rest/
--rwxr-xr-x   0 urischwartz   (501) staff       (20)     3572 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1454 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/accounts.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2956 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/convert.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      921 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/fees.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     7002 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/futures.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1672 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/market_data.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    85103 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/orders.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1268 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/payments.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     4364 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/perpetuals.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     4089 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/portfolios.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     3199 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/products.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     5421 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/rest/public.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     7258 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/coinbase/rest/rest_base.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.570735 coinbase-advanced-py-1.4.0/coinbase/websocket/
--rw-r--r--   0 urischwartz   (501) staff       (20)     1013 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/coinbase/websocket/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    15244 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/coinbase/websocket/channels.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    20143 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/coinbase/websocket/websocket_base.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.572008 coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/
--rw-r--r--   0 urischwartz   (501) staff       (20)    17519 2024-05-21 15:25:00.000000 coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/PKG-INFO
--rw-r--r--   0 urischwartz   (501) staff       (20)     1339 2024-05-21 15:25:00.000000 coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/SOURCES.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)        1 2024-05-21 15:25:00.000000 coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/dependency_links.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)      167 2024-05-21 15:25:00.000000 coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/requires.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)       15 2024-05-21 15:25:00.000000 coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/top_level.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)       38 2024-05-21 15:25:00.580513 coinbase-advanced-py-1.4.0/setup.cfg
--rw-r--r--   0 urischwartz   (501) staff       (20)     1642 2024-02-12 19:40:21.000000 coinbase-advanced-py-1.4.0/setup.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.572448 coinbase-advanced-py-1.4.0/tests/
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.577388 coinbase-advanced-py-1.4.0/tests/rest/
--rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-12-18 21:35:16.000000 coinbase-advanced-py-1.4.0/tests/rest/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1531 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/tests/rest/test_accounts.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2924 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/rest/test_convert.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      968 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/rest/test_fees.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     7243 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/tests/rest/test_futures.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1711 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/rest/test_market_data.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    77962 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/tests/rest/test_orders.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1392 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.4.0/tests/rest/test_payments.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     4950 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.0/tests/rest/test_perpetuals.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     4429 2024-01-29 17:15:12.000000 coinbase-advanced-py-1.4.0/tests/rest/test_portfolios.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2701 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/rest/test_products.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     5600 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/tests/rest/test_public.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     7860 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/tests/rest/test_rest_base.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1860 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/tests/test_api_base.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1749 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.4.0/tests/test_jwt_generator.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-21 15:25:00.578821 coinbase-advanced-py-1.4.0/tests/websocket/
--rw-r--r--   0 urischwartz   (501) staff       (20)        0 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/websocket/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2217 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/websocket/mock_ws_server.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     6651 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.0/tests/websocket/test_channels.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    20856 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.0/tests/websocket/test_websocket_base.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-24 15:47:24.527404 coinbase-advanced-py-1.4.1/
+-rw-r--r--   0 urischwartz   (501) staff       (20)    11343 2023-12-07 15:44:33.000000 coinbase-advanced-py-1.4.1/LICENSE.md
+-rw-r--r--   0 urischwartz   (501) staff       (20)    17519 2024-05-24 15:47:24.526601 coinbase-advanced-py-1.4.1/PKG-INFO
+-rw-r--r--   0 urischwartz   (501) staff       (20)    16405 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/README.md
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-24 15:47:24.491533 coinbase-advanced-py-1.4.1/coinbase/
+-rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-11-21 15:58:27.000000 coinbase-advanced-py-1.4.1/coinbase/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)       22 2024-05-24 15:46:51.000000 coinbase-advanced-py-1.4.1/coinbase/__version__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2169 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.1/coinbase/api_base.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      773 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.1/coinbase/constants.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2339 2024-05-24 15:46:51.000000 coinbase-advanced-py-1.4.1/coinbase/jwt_generator.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-24 15:47:24.501493 coinbase-advanced-py-1.4.1/coinbase/rest/
+-rwxr-xr-x   0 urischwartz   (501) staff       (20)     3572 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/coinbase/rest/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1454 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/coinbase/rest/accounts.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2956 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/coinbase/rest/convert.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      921 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/coinbase/rest/fees.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     7002 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/coinbase/rest/futures.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1672 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/coinbase/rest/market_data.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    85103 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/coinbase/rest/orders.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1268 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/coinbase/rest/payments.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4364 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/coinbase/rest/perpetuals.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4089 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/coinbase/rest/portfolios.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     3199 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/coinbase/rest/products.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     5421 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/coinbase/rest/public.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     7258 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.1/coinbase/rest/rest_base.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-24 15:47:24.504007 coinbase-advanced-py-1.4.1/coinbase/websocket/
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1013 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.1/coinbase/websocket/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    15244 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/coinbase/websocket/channels.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    20143 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.1/coinbase/websocket/websocket_base.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-24 15:47:24.506883 coinbase-advanced-py-1.4.1/coinbase_advanced_py.egg-info/
+-rw-r--r--   0 urischwartz   (501) staff       (20)    17519 2024-05-24 15:47:24.000000 coinbase-advanced-py-1.4.1/coinbase_advanced_py.egg-info/PKG-INFO
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1339 2024-05-24 15:47:24.000000 coinbase-advanced-py-1.4.1/coinbase_advanced_py.egg-info/SOURCES.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)        1 2024-05-24 15:47:24.000000 coinbase-advanced-py-1.4.1/coinbase_advanced_py.egg-info/dependency_links.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)      167 2024-05-24 15:47:24.000000 coinbase-advanced-py-1.4.1/coinbase_advanced_py.egg-info/requires.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)       15 2024-05-24 15:47:24.000000 coinbase-advanced-py-1.4.1/coinbase_advanced_py.egg-info/top_level.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)       38 2024-05-24 15:47:24.527526 coinbase-advanced-py-1.4.1/setup.cfg
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1642 2024-02-12 19:40:21.000000 coinbase-advanced-py-1.4.1/setup.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-24 15:47:24.507933 coinbase-advanced-py-1.4.1/tests/
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-24 15:47:24.521839 coinbase-advanced-py-1.4.1/tests/rest/
+-rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-12-18 21:35:16.000000 coinbase-advanced-py-1.4.1/tests/rest/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1531 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.1/tests/rest/test_accounts.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2924 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.1/tests/rest/test_convert.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      968 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.1/tests/rest/test_fees.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     7243 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/tests/rest/test_futures.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1711 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.1/tests/rest/test_market_data.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    77962 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.1/tests/rest/test_orders.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1392 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.4.1/tests/rest/test_payments.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4950 2024-05-21 15:24:22.000000 coinbase-advanced-py-1.4.1/tests/rest/test_perpetuals.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4429 2024-01-29 17:15:12.000000 coinbase-advanced-py-1.4.1/tests/rest/test_portfolios.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2701 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.1/tests/rest/test_products.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     5600 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.1/tests/rest/test_public.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     7860 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.1/tests/rest/test_rest_base.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1860 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.1/tests/test_api_base.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1727 2024-05-24 15:46:51.000000 coinbase-advanced-py-1.4.1/tests/test_jwt_generator.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-24 15:47:24.524592 coinbase-advanced-py-1.4.1/tests/websocket/
+-rw-r--r--   0 urischwartz   (501) staff       (20)        0 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.1/tests/websocket/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2217 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.1/tests/websocket/mock_ws_server.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     6651 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.4.1/tests/websocket/test_channels.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    20856 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.4.1/tests/websocket/test_websocket_base.py
```

### Comparing `coinbase-advanced-py-1.4.0/LICENSE.md` & `coinbase-advanced-py-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/PKG-INFO` & `coinbase-advanced-py-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinbase-advanced-py
-Version: 1.4.0
+Version: 1.4.1
 Summary: Coinbase Advanced API Python SDK
 Home-page: https://github.com/coinbase/coinbase-advanced-py
 Author: Coinbase
 License: Apache 2.0
 Keywords: Coinbase,Advanced Trade,API,Advanced API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `coinbase-advanced-py-1.4.0/README.md` & `coinbase-advanced-py-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/api_base.py` & `coinbase-advanced-py-1.4.1/coinbase/api_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/constants.py` & `coinbase-advanced-py-1.4.1/coinbase/constants.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/jwt_generator.py` & `coinbase-advanced-py-1.4.1/coinbase/jwt_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         raise Exception(
             f"{e}\n"
             "Are you sure you generated your key at https://cloud.coinbase.com/access/api ?"
         )
 
     jwt_data = {
         "sub": key_var,
-        "iss": "coinbase-cloud",
+        "iss": "cdp",
         "nbf": int(time.time()),
         "exp": int(time.time()) + 120,
     }
 
     if uri:
         jwt_data["uri"] = uri
```

### Comparing `coinbase-advanced-py-1.4.0/coinbase/rest/__init__.py` & `coinbase-advanced-py-1.4.1/coinbase/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/rest/accounts.py` & `coinbase-advanced-py-1.4.1/coinbase/rest/accounts.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/rest/convert.py` & `coinbase-advanced-py-1.4.1/coinbase/rest/convert.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/rest/fees.py` & `coinbase-advanced-py-1.4.1/coinbase/rest/fees.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/rest/futures.py` & `coinbase-advanced-py-1.4.1/coinbase/rest/futures.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/rest/market_data.py` & `coinbase-advanced-py-1.4.1/coinbase/rest/market_data.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/rest/orders.py` & `coinbase-advanced-py-1.4.1/coinbase/rest/orders.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/rest/payments.py` & `coinbase-advanced-py-1.4.1/coinbase/rest/payments.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/rest/perpetuals.py` & `coinbase-advanced-py-1.4.1/coinbase/rest/perpetuals.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/rest/portfolios.py` & `coinbase-advanced-py-1.4.1/coinbase/rest/portfolios.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/rest/products.py` & `coinbase-advanced-py-1.4.1/coinbase/rest/products.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/rest/public.py` & `coinbase-advanced-py-1.4.1/coinbase/rest/public.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/rest/rest_base.py` & `coinbase-advanced-py-1.4.1/coinbase/rest/rest_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/websocket/__init__.py` & `coinbase-advanced-py-1.4.1/coinbase/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/websocket/channels.py` & `coinbase-advanced-py-1.4.1/coinbase/websocket/channels.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase/websocket/websocket_base.py` & `coinbase-advanced-py-1.4.1/coinbase/websocket/websocket_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/PKG-INFO` & `coinbase-advanced-py-1.4.1/coinbase_advanced_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinbase-advanced-py
-Version: 1.4.0
+Version: 1.4.1
 Summary: Coinbase Advanced API Python SDK
 Home-page: https://github.com/coinbase/coinbase-advanced-py
 Author: Coinbase
 License: Apache 2.0
 Keywords: Coinbase,Advanced Trade,API,Advanced API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `coinbase-advanced-py-1.4.0/coinbase_advanced_py.egg-info/SOURCES.txt` & `coinbase-advanced-py-1.4.1/coinbase_advanced_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/setup.py` & `coinbase-advanced-py-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/rest/test_accounts.py` & `coinbase-advanced-py-1.4.1/tests/rest/test_accounts.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/rest/test_convert.py` & `coinbase-advanced-py-1.4.1/tests/rest/test_convert.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/rest/test_fees.py` & `coinbase-advanced-py-1.4.1/tests/rest/test_fees.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/rest/test_futures.py` & `coinbase-advanced-py-1.4.1/tests/rest/test_futures.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/rest/test_market_data.py` & `coinbase-advanced-py-1.4.1/tests/rest/test_market_data.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/rest/test_orders.py` & `coinbase-advanced-py-1.4.1/tests/rest/test_orders.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/rest/test_payments.py` & `coinbase-advanced-py-1.4.1/tests/rest/test_payments.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/rest/test_perpetuals.py` & `coinbase-advanced-py-1.4.1/tests/rest/test_perpetuals.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/rest/test_portfolios.py` & `coinbase-advanced-py-1.4.1/tests/rest/test_portfolios.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/rest/test_products.py` & `coinbase-advanced-py-1.4.1/tests/rest/test_products.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/rest/test_public.py` & `coinbase-advanced-py-1.4.1/tests/rest/test_public.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/rest/test_rest_base.py` & `coinbase-advanced-py-1.4.1/tests/rest/test_rest_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/test_api_base.py` & `coinbase-advanced-py-1.4.1/tests/test_api_base.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/test_jwt_generator.py` & `coinbase-advanced-py-1.4.1/tests/test_jwt_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,27 +16,27 @@
         result_jwt = jwt_generator.build_rest_jwt(uri, TEST_API_KEY, TEST_API_SECRET)
 
         decoded_data = jwt.decode(result_jwt, TEST_API_SECRET, algorithms=["ES256"])
         header_bytes = base64.urlsafe_b64decode(str(result_jwt.split(".")[0] + "=="))
         decoded_header = json.loads(header_bytes.decode("utf-8"))
 
         self.assertEqual(decoded_data["sub"], TEST_API_KEY)
-        self.assertEqual(decoded_data["iss"], "coinbase-cloud")
+        self.assertEqual(decoded_data["iss"], "cdp")
         self.assertEqual(decoded_data["uri"], uri)
         self.assertEqual(decoded_header["kid"], TEST_API_KEY)
 
     def test_build_ws_jwt(self):
         result_jwt = jwt_generator.build_ws_jwt(TEST_API_KEY, TEST_API_SECRET)
 
         decoded_data = jwt.decode(result_jwt, TEST_API_SECRET, algorithms=["ES256"])
         header_bytes = base64.urlsafe_b64decode(str(result_jwt.split(".")[0] + "=="))
         decoded_header = json.loads(header_bytes.decode("utf-8"))
 
         self.assertEqual(decoded_data["sub"], TEST_API_KEY)
-        self.assertEqual(decoded_data["iss"], "coinbase-cloud")
+        self.assertEqual(decoded_data["iss"], "cdp")
         self.assertNotIn("uri", decoded_data)
         self.assertEqual(decoded_header["kid"], TEST_API_KEY)
 
     def test_build_rest_jwt_error(self):
         with self.assertRaises(Exception):
             uri = jwt_generator.format_jwt_uri("GET", "/api/v3/brokerage/accounts")
             jwt_generator.build_rest_jwt(uri, TEST_API_KEY, "bad_secret")
```

### Comparing `coinbase-advanced-py-1.4.0/tests/websocket/mock_ws_server.py` & `coinbase-advanced-py-1.4.1/tests/websocket/mock_ws_server.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/websocket/test_channels.py` & `coinbase-advanced-py-1.4.1/tests/websocket/test_channels.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.4.0/tests/websocket/test_websocket_base.py` & `coinbase-advanced-py-1.4.1/tests/websocket/test_websocket_base.py`

 * *Files identical despite different names*

