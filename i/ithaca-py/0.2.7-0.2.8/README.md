# Comparing `tmp/ithaca_py-0.2.7.tar.gz` & `tmp/ithaca_py-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ithaca_py-0.2.7.tar", max compression
+gzip compressed data, was "ithaca_py-0.2.8.tar", max compression
```

## Comparing `ithaca_py-0.2.7.tar` & `ithaca_py-0.2.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      983 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/README.md
--rw-r--r--   0        0        0     5147 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/__init__.py
--rw-r--r--   0        0        0     3870 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/analytics.py
--rw-r--r--   0        0        0    10809 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/auth.py
--rw-r--r--   0        0        0     5589 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/calculation.py
--rw-r--r--   0        0        0     3668 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/client.py
--rw-r--r--   0        0        0     1846 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/constants.py
--rw-r--r--   0        0        0    12592 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/fundlock.py
--rw-r--r--   0        0        0      603 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/market.py
--rw-r--r--   0        0        0     7370 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/orders.py
--rw-r--r--   0        0        0     1373 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/protocol.py
--rw-r--r--   0        0        0     2406 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/socket.py
--rw-r--r--   0        0        0      929 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      983 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/README.md
+-rw-r--r--   0        0        0     5147 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/__init__.py
+-rw-r--r--   0        0        0     3870 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/analytics.py
+-rw-r--r--   0        0        0    10809 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/auth.py
+-rw-r--r--   0        0        0     5589 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/calculation.py
+-rw-r--r--   0        0        0     3668 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/client.py
+-rw-r--r--   0        0        0     1846 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/constants.py
+-rw-r--r--   0        0        0    12592 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/fundlock.py
+-rw-r--r--   0        0        0      603 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/market.py
+-rw-r--r--   0        0        0     7370 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/orders.py
+-rw-r--r--   0        0        0     1513 2024-05-24 04:27:54.188907 ithaca_py-0.2.8/ithaca/protocol.py
+-rw-r--r--   0        0        0     2406 2024-05-24 04:27:54.192906 ithaca_py-0.2.8/ithaca/socket.py
+-rw-r--r--   0        0        0      929 2024-05-24 04:27:54.192906 ithaca_py-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.8/PKG-INFO
```

### Comparing `ithaca_py-0.2.7/README.md` & `ithaca_py-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.7/ithaca/__init__.py` & `ithaca_py-0.2.8/ithaca/__init__.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.7/ithaca/analytics.py` & `ithaca_py-0.2.8/ithaca/analytics.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.7/ithaca/auth.py` & `ithaca_py-0.2.8/ithaca/auth.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.7/ithaca/calculation.py` & `ithaca_py-0.2.8/ithaca/calculation.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.7/ithaca/client.py` & `ithaca_py-0.2.8/ithaca/client.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.7/ithaca/constants.py` & `ithaca_py-0.2.8/ithaca/constants.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.7/ithaca/fundlock.py` & `ithaca_py-0.2.8/ithaca/fundlock.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.7/ithaca/market.py` & `ithaca_py-0.2.8/ithaca/market.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.7/ithaca/orders.py` & `ithaca_py-0.2.8/ithaca/orders.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.7/ithaca/protocol.py` & `ithaca_py-0.2.8/ithaca/protocol.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,7 +41,11 @@
         body = {"ids": ids}
         return self.parent.post("/clientapi/contractListByIds", json=body)
 
     def historical_contracts(self, expiry):
         """Get historical contracts."""
         body = {"expiry": expiry}
         return self.parent.post("/clientapi/historicalContracts", json=body)
+    
+    def orderbook(self):
+        """Get orderbbok if flagged as MARKET_MAKER"""
+        return self.parent.post('/clientapi/orderbook')
```

### Comparing `ithaca_py-0.2.7/ithaca/socket.py` & `ithaca_py-0.2.8/ithaca/socket.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.7/pyproject.toml` & `ithaca_py-0.2.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ithaca_py"
-version = "0.2.7"
+version = "0.2.8"
 description = "Ithaca Protocol SDK"
 authors = ["nhaga <nhaga5@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ithaca"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ithaca_py-0.2.7/PKG-INFO` & `ithaca_py-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ithaca_py
-Version: 0.2.7
+Version: 0.2.8
 Summary: Ithaca Protocol SDK
 Author: nhaga
 Author-email: nhaga5@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

