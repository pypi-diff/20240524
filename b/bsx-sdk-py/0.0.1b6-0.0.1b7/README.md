# Comparing `tmp/bsx_sdk_py-0.0.1b6.tar.gz` & `tmp/bsx_sdk_py-0.0.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsx_sdk_py-0.0.1b6.tar", max compression
+gzip compressed data, was "bsx_sdk_py-0.0.1b7.tar", max compression
```

## Comparing `bsx_sdk_py-0.0.1b6.tar` & `bsx_sdk_py-0.0.1b7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2170 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/README.md
--rw-r--r--   0        0        0       89 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/account/__init__.py
--rw-r--r--   0        0        0     1797 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/account/client.py
--rw-r--r--   0        0        0      176 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/account/types.py
--rw-r--r--   0        0        0        0 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/auth/__init__.py
--rw-r--r--   0        0        0     2453 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/auth/client.py
--rw-r--r--   0        0        0      214 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/auth/types.py
--rw-r--r--   0        0        0     3254 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/base.py
--rw-r--r--   0        0        0        0 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/market/__init__.py
--rw-r--r--   0        0        0     4250 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/market/client.py
--rw-r--r--   0        0        0      224 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/client/rest/market/types.py
--rw-r--r--   0        0        0       24 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/__init__.py
--rw-r--r--   0        0        0      481 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/acc_info.py
--rw-r--r--   0        0        0     1167 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/exception.py
--rw-r--r--   0        0        0     1882 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/lock.py
--rw-r--r--   0        0        0        0 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/types/__init__.py
--rw-r--r--   0        0        0     6955 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/types/account.py
--rw-r--r--   0        0        0     1470 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/types/auth.py
--rw-r--r--   0        0        0      234 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/types/base.py
--rw-r--r--   0        0        0     8455 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/common/types/market.py
--rw-r--r--   0        0        0       62 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/helper/__init__.py
--rw-r--r--   0        0        0     1292 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/helper/acc_storage.py
--rw-r--r--   0        0        0     1871 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/helper/api_key_base_manager.py
--rw-r--r--   0        0        0     1563 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/helper/base.py
--rw-r--r--   0        0        0     1417 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/helper/secret_base_manager.py
--rw-r--r--   0        0        0     8789 2024-04-29 06:31:42.024713 bsx_sdk_py-0.0.1b6/bsx_py/instance.py
--rw-r--r--   0        0        0      556 2024-04-29 06:31:42.044713 bsx_sdk_py-0.0.1b6/pyproject.toml
--rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 bsx_sdk_py-0.0.1b6/PKG-INFO
+-rw-r--r--   0        0        0     2485 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/README.md
+-rw-r--r--   0        0        0       89 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/client/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/client/rest/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/client/rest/account/__init__.py
+-rw-r--r--   0        0        0     1797 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/client/rest/account/client.py
+-rw-r--r--   0        0        0      176 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/client/rest/account/types.py
+-rw-r--r--   0        0        0        0 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/client/rest/auth/__init__.py
+-rw-r--r--   0        0        0     2453 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/client/rest/auth/client.py
+-rw-r--r--   0        0        0      214 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/client/rest/auth/types.py
+-rw-r--r--   0        0        0     3254 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/client/rest/base.py
+-rw-r--r--   0        0        0        0 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/client/rest/market/__init__.py
+-rw-r--r--   0        0        0     4250 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/client/rest/market/client.py
+-rw-r--r--   0        0        0      224 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/client/rest/market/types.py
+-rw-r--r--   0        0        0       24 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/common/__init__.py
+-rw-r--r--   0        0        0      481 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/common/acc_info.py
+-rw-r--r--   0        0        0     1167 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/common/exception.py
+-rw-r--r--   0        0        0     1882 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/common/lock.py
+-rw-r--r--   0        0        0        0 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/common/types/__init__.py
+-rw-r--r--   0        0        0     6955 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/common/types/account.py
+-rw-r--r--   0        0        0     1470 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/common/types/auth.py
+-rw-r--r--   0        0        0      234 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/common/types/base.py
+-rw-r--r--   0        0        0     8455 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/common/types/market.py
+-rw-r--r--   0        0        0       62 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/helper/__init__.py
+-rw-r--r--   0        0        0     1292 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/helper/acc_storage.py
+-rw-r--r--   0        0        0     1871 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/helper/api_key_base_manager.py
+-rw-r--r--   0        0        0     1563 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/helper/base.py
+-rw-r--r--   0        0        0     1417 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/helper/secret_base_manager.py
+-rw-r--r--   0        0        0     8789 2024-05-24 07:09:32.683210 bsx_sdk_py-0.0.1b7/bsx_py/instance.py
+-rw-r--r--   0        0        0      556 2024-05-24 07:09:32.707210 bsx_sdk_py-0.0.1b7/pyproject.toml
+-rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 bsx_sdk_py-0.0.1b7/PKG-INFO
```

### Comparing `bsx_sdk_py-0.0.1b6/README.md` & `bsx_sdk_py-0.0.1b7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,40 +19,40 @@
 ## Basic usage
 
 ### Create a wallet and a signer from private keys
 
 ```python
 from eth_account import Account
 
-wallet_private_key = "xxx"
-signer_private_key = "yyy"
+wallet_private_key = "0x0000000000000000000000000000000000000000000000000000000000000000"
+signer_private_key = "0x1111111111111111111111111111111111111111111111111111111111111111"
 wallet = Account.from_key(wallet_private_key)
 signer = Account.from_key(signer_private_key)
 ```
 
 ### Create the BSXInstance using the main wallet's private key:
 
 ```python
 from eth_account import Account
 from bsx_py import BSXInstance, Environment
 
-wallet_private_key = "xxx"
-signer_private_key = "yyy"
+wallet_private_key = "0x0000000000000000000000000000000000000000000000000000000000000000"
+signer_private_key = "0x1111111111111111111111111111111111111111111111111111111111111111"
 wallet = Account.from_key(wallet_private_key)
 signer = Account.from_key(signer_private_key)
 bsx_instance = BSXInstance(env=Environment.TESTNET, wallet=wallet, signer=signer)
 ```
 
 ### Create the BSXInstance using an active API key:
 
 ```python
 from eth_account import Account
 from bsx_py import BSXInstance, Environment
 
-signer_private_key = "yyy"
+signer_private_key = "0x1111111111111111111111111111111111111111111111111111111111111111"
 signer = Account.from_key(signer_private_key)
 bsx_instance = BSXInstance.from_api_key(api_key="xxx", api_secret="zzz", signer=signer, env=Environment.TESTNET)
 ```
 
 ### Perform basic operations:
 
 ```python
```

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/client/rest/account/client.py` & `bsx_sdk_py-0.0.1b7/bsx_py/client/rest/account/client.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/client/rest/auth/client.py` & `bsx_sdk_py-0.0.1b7/bsx_py/client/rest/auth/client.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/client/rest/base.py` & `bsx_sdk_py-0.0.1b7/bsx_py/client/rest/base.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/client/rest/market/client.py` & `bsx_sdk_py-0.0.1b7/bsx_py/client/rest/market/client.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/common/exception.py` & `bsx_sdk_py-0.0.1b7/bsx_py/common/exception.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/common/lock.py` & `bsx_sdk_py-0.0.1b7/bsx_py/common/lock.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/common/types/account.py` & `bsx_sdk_py-0.0.1b7/bsx_py/common/types/account.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/common/types/auth.py` & `bsx_sdk_py-0.0.1b7/bsx_py/common/types/auth.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/common/types/market.py` & `bsx_sdk_py-0.0.1b7/bsx_py/common/types/market.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/helper/acc_storage.py` & `bsx_sdk_py-0.0.1b7/bsx_py/helper/acc_storage.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/helper/api_key_base_manager.py` & `bsx_sdk_py-0.0.1b7/bsx_py/helper/api_key_base_manager.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/helper/base.py` & `bsx_sdk_py-0.0.1b7/bsx_py/helper/base.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/helper/secret_base_manager.py` & `bsx_sdk_py-0.0.1b7/bsx_py/helper/secret_base_manager.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/bsx_py/instance.py` & `bsx_sdk_py-0.0.1b7/bsx_py/instance.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b6/pyproject.toml` & `bsx_sdk_py-0.0.1b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bsx-sdk-py"
-version = "0.0.1beta6"
+version = "0.0.1beta7"
 description = ""
 authors = ["bsx-engineering <dev@bsx.exchange>"]
 readme = "README.md"
 packages = [
     { include = "bsx_py" }
 ]
```

### Comparing `bsx_sdk_py-0.0.1b6/PKG-INFO` & `bsx_sdk_py-0.0.1b7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsx-sdk-py
-Version: 0.0.1b6
+Version: 0.0.1b7
 Summary: 
 Author: bsx-engineering
 Author-email: dev@bsx.exchange
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -38,40 +38,40 @@
 ## Basic usage
 
 ### Create a wallet and a signer from private keys
 
 ```python
 from eth_account import Account
 
-wallet_private_key = "xxx"
-signer_private_key = "yyy"
+wallet_private_key = "0x0000000000000000000000000000000000000000000000000000000000000000"
+signer_private_key = "0x1111111111111111111111111111111111111111111111111111111111111111"
 wallet = Account.from_key(wallet_private_key)
 signer = Account.from_key(signer_private_key)
 ```
 
 ### Create the BSXInstance using the main wallet's private key:
 
 ```python
 from eth_account import Account
 from bsx_py import BSXInstance, Environment
 
-wallet_private_key = "xxx"
-signer_private_key = "yyy"
+wallet_private_key = "0x0000000000000000000000000000000000000000000000000000000000000000"
+signer_private_key = "0x1111111111111111111111111111111111111111111111111111111111111111"
 wallet = Account.from_key(wallet_private_key)
 signer = Account.from_key(signer_private_key)
 bsx_instance = BSXInstance(env=Environment.TESTNET, wallet=wallet, signer=signer)
 ```
 
 ### Create the BSXInstance using an active API key:
 
 ```python
 from eth_account import Account
 from bsx_py import BSXInstance, Environment
 
-signer_private_key = "yyy"
+signer_private_key = "0x1111111111111111111111111111111111111111111111111111111111111111"
 signer = Account.from_key(signer_private_key)
 bsx_instance = BSXInstance.from_api_key(api_key="xxx", api_secret="zzz", signer=signer, env=Environment.TESTNET)
 ```
 
 ### Perform basic operations:
 
 ```python
```

