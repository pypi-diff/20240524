# Comparing `tmp/pragma_sdk-1.3.7.tar.gz` & `tmp/pragma_sdk-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pragma_sdk-1.3.7.tar", max compression
+gzip compressed data, was "pragma_sdk-1.3.8.tar", max compression
```

## Comparing `pragma_sdk-1.3.7.tar` & `pragma_sdk-1.3.8.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      943 2024-05-23 19:56:25.774210 pragma_sdk-1.3.7/README.md
--rw-r--r--   0        0        0        0 2024-05-23 19:56:25.774210 pragma_sdk-1.3.7/pragma/__init__.py
--rw-r--r--   0        0        0      195 2024-05-23 19:56:25.774210 pragma_sdk-1.3.7/pragma/core/__init__.py
--rw-r--r--   0        0        0       55 2024-05-23 19:56:25.774210 pragma_sdk-1.3.7/pragma/core/abis/__init__.py
--rw-r--r--   0        0        0     1773 2024-05-23 19:56:25.774210 pragma_sdk-1.3.7/pragma/core/abis/abi.py
--rw-r--r--   0        0        0      375 2024-05-23 19:56:25.774210 pragma_sdk-1.3.7/pragma/core/abis/pragma_Admin.sierra.json
--rw-r--r--   0        0        0     6050 2024-05-23 19:56:25.774210 pragma_sdk-1.3.7/pragma/core/abis/pragma_ERC20.json
--rw-r--r--   0        0        0   140867 2024-05-23 19:56:25.774210 pragma_sdk-1.3.7/pragma/core/abis/pragma_ExampleRandomness.sierra.json
--rw-r--r--   0        0        0    34149 2024-05-23 19:56:25.774210 pragma_sdk-1.3.7/pragma/core/abis/pragma_MockOracle.sierra.json
--rw-r--r--   0        0        0  1705306 2024-05-23 19:56:25.782210 pragma_sdk-1.3.7/pragma/core/abis/pragma_Oracle.sierra.json
--rw-r--r--   0        0        0    42794 2024-05-23 19:56:25.782210 pragma_sdk-1.3.7/pragma/core/abis/pragma_Ownable.sierra.json
--rw-r--r--   0        0        0   275940 2024-05-23 19:56:25.782210 pragma_sdk-1.3.7/pragma/core/abis/pragma_PublisherRegistry.sierra.json
--rw-r--r--   0        0        0   544514 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/abis/pragma_Randomness.sierra.json
--rw-r--r--   0        0        0   323399 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/abis/pragma_SummaryStats.sierra.json
--rw-r--r--   0        0        0      686 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/abis/pragma_Upgradeable.sierra.json
--rw-r--r--   0        0        0   491352 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/abis/pragma_YieldCurve.sierra.json
--rw-r--r--   0        0        0     5669 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/assets.py
--rw-r--r--   0        0        0     6045 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/client.py
--rw-r--r--   0        0        0     1796 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/contract.py
--rw-r--r--   0        0        0    12550 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/entry.py
--rw-r--r--   0        0        0      393 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/logger.py
--rw-r--r--   0        0        0      344 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/mixins/__init__.py
--rw-r--r--   0        0        0     3831 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/mixins/nonce.py
--rw-r--r--   0        0        0     7303 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/mixins/offchain.py
--rw-r--r--   0        0        0    15874 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/mixins/oracle.py
--rw-r--r--   0        0        0     2505 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/mixins/publisher_registry.py
--rw-r--r--   0        0        0    14499 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/mixins/randomness.py
--rw-r--r--   0        0        0      669 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/mixins/transactions.py
--rw-r--r--   0        0        0        0 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/randomness/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/randomness/actions.py
--rw-r--r--   0        0        0    16307 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/randomness/randomness_utils.py
--rw-r--r--   0        0        0     1845 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/randomness/utils.py
--rw-r--r--   0        0        0    11211 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/types.py
--rw-r--r--   0        0        0     2598 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/core/utils.py
--rw-r--r--   0        0        0       59 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/publisher/__init__.py
--rw-r--r--   0        0        0    10500 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/publisher/client.py
--rw-r--r--   0        0        0      652 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/publisher/fetchers/__init__.py
--rw-r--r--   0        0        0     3191 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/publisher/fetchers/ascendex.py
--rw-r--r--   0        0        0     4694 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/publisher/fetchers/binance.py
--rw-r--r--   0        0        0     2330 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/publisher/fetchers/bitstamp.py
--rw-r--r--   0        0        0     4756 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/publisher/fetchers/bybit.py
--rw-r--r--   0        0        0     2832 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/publisher/fetchers/cex.py
--rw-r--r--   0        0        0     2565 2024-05-23 19:56:25.786210 pragma_sdk-1.3.7/pragma/publisher/fetchers/coinbase.py
--rw-r--r--   0        0        0     3243 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/fetchers/coingecko.py
--rw-r--r--   0        0        0     5142 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/fetchers/defillama.py
--rw-r--r--   0        0        0     7690 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/fetchers/gecko.py
--rw-r--r--   0        0        0     2706 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/fetchers/gemini.py
--rw-r--r--   0        0        0     4622 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/fetchers/huobi.py
--rw-r--r--   0        0        0     3219 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/fetchers/index.py
--rw-r--r--   0        0        0     3836 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/fetchers/indexcoop.py
--rw-r--r--   0        0        0     4198 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/fetchers/kucoin.py
--rw-r--r--   0        0        0     3350 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/fetchers/okx.py
--rw-r--r--   0        0        0     6523 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/fetchers/propeller.py
--rw-r--r--   0        0        0     6209 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/fetchers/starknetamm.py
--rw-r--r--   0        0        0     5050 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/fetchers/thegraph.py
--rw-r--r--   0        0        0     2514 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/fetchers/upbit.py
--rw-r--r--   0        0        0      114 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/future_fetchers/__init__.py
--rw-r--r--   0        0        0     4855 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/future_fetchers/binance.py
--rw-r--r--   0        0        0     3161 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/future_fetchers/bybit.py
--rw-r--r--   0        0        0     4511 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/future_fetchers/okx.py
--rw-r--r--   0        0        0     1199 2024-05-23 19:56:25.790210 pragma_sdk-1.3.7/pragma/publisher/types.py
--rw-r--r--   0        0        0     4102 2024-05-23 19:56:25.794210 pragma_sdk-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 pragma_sdk-1.3.7/setup.py
--rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 pragma_sdk-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0      943 2024-05-23 20:45:02.879761 pragma_sdk-1.3.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 20:45:02.879761 pragma_sdk-1.3.8/pragma/__init__.py
+-rw-r--r--   0        0        0      195 2024-05-23 20:45:02.879761 pragma_sdk-1.3.8/pragma/core/__init__.py
+-rw-r--r--   0        0        0       55 2024-05-23 20:45:02.879761 pragma_sdk-1.3.8/pragma/core/abis/__init__.py
+-rw-r--r--   0        0        0     1773 2024-05-23 20:45:02.879761 pragma_sdk-1.3.8/pragma/core/abis/abi.py
+-rw-r--r--   0        0        0      375 2024-05-23 20:45:02.879761 pragma_sdk-1.3.8/pragma/core/abis/pragma_Admin.sierra.json
+-rw-r--r--   0        0        0     6050 2024-05-23 20:45:02.879761 pragma_sdk-1.3.8/pragma/core/abis/pragma_ERC20.json
+-rw-r--r--   0        0        0   140867 2024-05-23 20:45:02.879761 pragma_sdk-1.3.8/pragma/core/abis/pragma_ExampleRandomness.sierra.json
+-rw-r--r--   0        0        0    34149 2024-05-23 20:45:02.879761 pragma_sdk-1.3.8/pragma/core/abis/pragma_MockOracle.sierra.json
+-rw-r--r--   0        0        0  1705306 2024-05-23 20:45:02.887761 pragma_sdk-1.3.8/pragma/core/abis/pragma_Oracle.sierra.json
+-rw-r--r--   0        0        0    42794 2024-05-23 20:45:02.887761 pragma_sdk-1.3.8/pragma/core/abis/pragma_Ownable.sierra.json
+-rw-r--r--   0        0        0   275940 2024-05-23 20:45:02.887761 pragma_sdk-1.3.8/pragma/core/abis/pragma_PublisherRegistry.sierra.json
+-rw-r--r--   0        0        0   544514 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/abis/pragma_Randomness.sierra.json
+-rw-r--r--   0        0        0   323399 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/abis/pragma_SummaryStats.sierra.json
+-rw-r--r--   0        0        0      686 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/abis/pragma_Upgradeable.sierra.json
+-rw-r--r--   0        0        0   491352 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/abis/pragma_YieldCurve.sierra.json
+-rw-r--r--   0        0        0     5669 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/assets.py
+-rw-r--r--   0        0        0     6045 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/client.py
+-rw-r--r--   0        0        0     1796 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/contract.py
+-rw-r--r--   0        0        0    12550 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/entry.py
+-rw-r--r--   0        0        0      393 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/logger.py
+-rw-r--r--   0        0        0      344 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/mixins/__init__.py
+-rw-r--r--   0        0        0     3831 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/mixins/nonce.py
+-rw-r--r--   0        0        0     7303 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/mixins/offchain.py
+-rw-r--r--   0        0        0    15874 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/mixins/oracle.py
+-rw-r--r--   0        0        0     2505 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/mixins/publisher_registry.py
+-rw-r--r--   0        0        0    14505 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/mixins/randomness.py
+-rw-r--r--   0        0        0      669 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/mixins/transactions.py
+-rw-r--r--   0        0        0        0 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/randomness/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/randomness/actions.py
+-rw-r--r--   0        0        0    16307 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/randomness/randomness_utils.py
+-rw-r--r--   0        0        0     1845 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/randomness/utils.py
+-rw-r--r--   0        0        0    11211 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/types.py
+-rw-r--r--   0        0        0     2598 2024-05-23 20:45:02.891761 pragma_sdk-1.3.8/pragma/core/utils.py
+-rw-r--r--   0        0        0       59 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/__init__.py
+-rw-r--r--   0        0        0    10500 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/client.py
+-rw-r--r--   0        0        0      652 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/__init__.py
+-rw-r--r--   0        0        0     3191 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/ascendex.py
+-rw-r--r--   0        0        0     4694 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/binance.py
+-rw-r--r--   0        0        0     2330 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/bitstamp.py
+-rw-r--r--   0        0        0     4756 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/bybit.py
+-rw-r--r--   0        0        0     2832 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/cex.py
+-rw-r--r--   0        0        0     2565 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/coinbase.py
+-rw-r--r--   0        0        0     3243 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/coingecko.py
+-rw-r--r--   0        0        0     5142 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/defillama.py
+-rw-r--r--   0        0        0     7690 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/gecko.py
+-rw-r--r--   0        0        0     2706 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/gemini.py
+-rw-r--r--   0        0        0     4622 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/huobi.py
+-rw-r--r--   0        0        0     3219 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/index.py
+-rw-r--r--   0        0        0     3836 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/indexcoop.py
+-rw-r--r--   0        0        0     4198 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/kucoin.py
+-rw-r--r--   0        0        0     3350 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/okx.py
+-rw-r--r--   0        0        0     6523 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/propeller.py
+-rw-r--r--   0        0        0     6209 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/starknetamm.py
+-rw-r--r--   0        0        0     5050 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/thegraph.py
+-rw-r--r--   0        0        0     2514 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/fetchers/upbit.py
+-rw-r--r--   0        0        0      114 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/future_fetchers/__init__.py
+-rw-r--r--   0        0        0     4855 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/future_fetchers/binance.py
+-rw-r--r--   0        0        0     3161 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/future_fetchers/bybit.py
+-rw-r--r--   0        0        0     4511 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/future_fetchers/okx.py
+-rw-r--r--   0        0        0     1199 2024-05-23 20:45:02.895761 pragma_sdk-1.3.8/pragma/publisher/types.py
+-rw-r--r--   0        0        0     4102 2024-05-23 20:45:02.899761 pragma_sdk-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 pragma_sdk-1.3.8/setup.py
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 pragma_sdk-1.3.8/PKG-INFO
```

### Comparing `pragma_sdk-1.3.7/README.md` & `pragma_sdk-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/abis/abi.py` & `pragma_sdk-1.3.8/pragma/core/abis/abi.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/abis/pragma_ERC20.json` & `pragma_sdk-1.3.8/pragma/core/abis/pragma_ERC20.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/abis/pragma_ExampleRandomness.sierra.json` & `pragma_sdk-1.3.8/pragma/core/abis/pragma_ExampleRandomness.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/abis/pragma_MockOracle.sierra.json` & `pragma_sdk-1.3.8/pragma/core/abis/pragma_MockOracle.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/abis/pragma_Oracle.sierra.json` & `pragma_sdk-1.3.8/pragma/core/abis/pragma_Oracle.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/abis/pragma_Ownable.sierra.json` & `pragma_sdk-1.3.8/pragma/core/abis/pragma_Ownable.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/abis/pragma_PublisherRegistry.sierra.json` & `pragma_sdk-1.3.8/pragma/core/abis/pragma_PublisherRegistry.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/abis/pragma_Randomness.sierra.json` & `pragma_sdk-1.3.8/pragma/core/abis/pragma_Randomness.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/abis/pragma_SummaryStats.sierra.json` & `pragma_sdk-1.3.8/pragma/core/abis/pragma_SummaryStats.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/abis/pragma_Upgradeable.sierra.json` & `pragma_sdk-1.3.8/pragma/core/abis/pragma_Upgradeable.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/abis/pragma_YieldCurve.sierra.json` & `pragma_sdk-1.3.8/pragma/core/abis/pragma_YieldCurve.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/assets.py` & `pragma_sdk-1.3.8/pragma/core/assets.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/client.py` & `pragma_sdk-1.3.8/pragma/core/client.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/contract.py` & `pragma_sdk-1.3.8/pragma/core/contract.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/entry.py` & `pragma_sdk-1.3.8/pragma/core/entry.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/mixins/nonce.py` & `pragma_sdk-1.3.8/pragma/core/mixins/nonce.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/mixins/offchain.py` & `pragma_sdk-1.3.8/pragma/core/mixins/offchain.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/mixins/oracle.py` & `pragma_sdk-1.3.8/pragma/core/mixins/oracle.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/mixins/publisher_registry.py` & `pragma_sdk-1.3.8/pragma/core/mixins/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/mixins/randomness.py` & `pragma_sdk-1.3.8/pragma/core/mixins/randomness.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,15 +390,15 @@
                 block = (
                     await self.full_node_client.get_block(
                         block_number=minimum_block_number
                     )
                     if is_pending
                     else await self.full_node_client.get_block(block_number="pending")
                 )
-                block_hash = block.parent_hash
+                block_hash = block.parent_block_hash
 
                 seed = (
                     event.request_id.to_bytes(8, sys.byteorder)
                     + block_hash.to_bytes(32, sys.byteorder)
                     + event.seed.to_bytes(32, sys.byteorder)
                     + event.caller_address.to_bytes(32, sys.byteorder)
                 )
```

### Comparing `pragma_sdk-1.3.7/pragma/core/mixins/transactions.py` & `pragma_sdk-1.3.8/pragma/core/mixins/transactions.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/randomness/randomness_utils.py` & `pragma_sdk-1.3.8/pragma/core/randomness/randomness_utils.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/randomness/utils.py` & `pragma_sdk-1.3.8/pragma/core/randomness/utils.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/types.py` & `pragma_sdk-1.3.8/pragma/core/types.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/core/utils.py` & `pragma_sdk-1.3.8/pragma/core/utils.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/client.py` & `pragma_sdk-1.3.8/pragma/publisher/client.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/__init__.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/__init__.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/ascendex.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/ascendex.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/binance.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/binance.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/bitstamp.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/bitstamp.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/bybit.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/bybit.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/cex.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/cex.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/coinbase.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/coinbase.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/coingecko.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/coingecko.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/defillama.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/defillama.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/gecko.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/gecko.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/gemini.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/gemini.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/huobi.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/huobi.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/index.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/index.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/indexcoop.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/indexcoop.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/kucoin.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/kucoin.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/okx.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/propeller.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/propeller.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/starknetamm.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/starknetamm.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/thegraph.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/thegraph.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/fetchers/upbit.py` & `pragma_sdk-1.3.8/pragma/publisher/fetchers/upbit.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/future_fetchers/binance.py` & `pragma_sdk-1.3.8/pragma/publisher/future_fetchers/binance.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/future_fetchers/bybit.py` & `pragma_sdk-1.3.8/pragma/publisher/future_fetchers/bybit.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/future_fetchers/okx.py` & `pragma_sdk-1.3.8/pragma/publisher/future_fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pragma/publisher/types.py` & `pragma_sdk-1.3.8/pragma/publisher/types.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.7/pyproject.toml` & `pragma_sdk-1.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pragma-sdk"
-version = "1.3.7"
+version = "1.3.8"
 authors = ["0xevolve <matthias@pragma.build>"]
 description = "Core package for rollup-native Pragma Oracle"
 readme = "README.md"
 homepage = "https://pragma.build"
 repository = "https://github.com/Astraly-Labs/pragma-sdk"
 documentation = "https://docs.pragma.build"
 classifiers = [
```

### Comparing `pragma_sdk-1.3.7/setup.py` & `pragma_sdk-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'python-dotenv>=1.0.0,<2.0.0',
  'requests-mock>=1.11.0,<2.0.0',
  'starknet.py==0.20.0',
  'typer==0.6.1']
 
 setup_kwargs = {
     'name': 'pragma-sdk',
-    'version': '1.3.7',
+    'version': '1.3.8',
     'description': 'Core package for rollup-native Pragma Oracle',
     'long_description': "# Pragma SDK\n\n[![codecov](https://codecov.io/gh/Astraly-Labs/pragma-sdk/graph/badge.svg?token=98pUFYGHIK)](https://codecov.io/gh/Astraly-Labs/pragma-sdk)\n\n[![Checks](https://github.com/Astraly-Labs/pragma-sdk/actions/workflows/checks.yml/badge.svg)](https://github.com/Astraly-Labs/pragma-sdk/actions/workflows/checks.yml)\n\n[![Package](https://img.shields.io/pypi/v/pragma-sdk)](https://pypi.org/project/pragma-sdk/)\n\n---\n\n**Pragma SDK, written in Python.**\n\nOne can leverage this SDK to interact with Pragma on Starknet.\nThis SDK should also be used by Data Providers willing to push data on Pragma contracts.\n\n## About\n\nFor more information, see the [project's repository](https://github.com/Astraly-Labs/Pragma), [documentation overview](https://docs.pragmaoracle.com/) and [documentation on how to publish data](https://docs.pragmaoracle.com/using-pragma/publishing-data).\n\n## Contributing\n\nSee the [CONTRIBUTING](./CONTRIBUTING.md) guide.",
     'author': '0xevolve',
     'author_email': 'matthias@pragma.build',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pragma.build',
```

### Comparing `pragma_sdk-1.3.7/PKG-INFO` & `pragma_sdk-1.3.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pragma-sdk
-Version: 1.3.7
+Version: 1.3.8
 Summary: Core package for rollup-native Pragma Oracle
 Home-page: https://pragma.build
 Author: 0xevolve
 Author-email: matthias@pragma.build
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

