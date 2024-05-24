# Comparing `tmp/hmx-v2-python-1.2.0.tar.gz` & `tmp/hmx-v2-python-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmx-v2-python-1.2.0.tar", last modified: Fri May  3 14:46:09 2024, max compression
+gzip compressed data, was "hmx-v2-python-1.2.1.tar", last modified: Fri May 24 18:33:55 2024, max compression
```

## Comparing `hmx-v2-python-1.2.0.tar` & `hmx-v2-python-1.2.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.988059 hmx-v2-python-1.2.0/
--rw-r--r--   0 adirut     (501) staff       (20)     1064 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/LICENSE
--rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-05-03 14:46:09.988295 hmx-v2-python-1.2.0/PKG-INFO
--rw-r--r--   0 adirut     (501) staff       (20)     3361 2024-04-14 03:17:48.000000 hmx-v2-python-1.2.0/README.md
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.976149 hmx-v2-python-1.2.0/hmx2/
--rw-r--r--   0 adirut     (501) staff       (20)       35 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/__init__.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.980510 hmx-v2-python-1.2.0/hmx2/abis/
--rw-r--r--   0 adirut     (501) staff       (20)     2918 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/abis/AdaptiveFeeCalculator.json
--rw-r--r--   0 adirut     (501) staff       (20)     6094 2023-12-01 07:58:15.000000 hmx-v2-python-1.2.0/hmx2/abis/CIXPriceAdapter.json
--rw-r--r--   0 adirut     (501) staff       (20)     3332 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/abis/CalcPricelens.json
--rw-r--r--   0 adirut     (501) staff       (20)    19788 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/hmx2/abis/Calculator.json
--rw-r--r--   0 adirut     (501) staff       (20)    79643 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/abis/ConfigStorage.json
--rw-r--r--   0 adirut     (501) staff       (20)    23809 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/abis/CrossMarginHandler.json
--rw-r--r--   0 adirut     (501) staff       (20)     3685 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/abis/ERC20.json
--rw-r--r--   0 adirut     (501) staff       (20)    11832 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/abis/GlpManager.json
--rw-r--r--   0 adirut     (501) staff       (20)     5780 2023-12-01 07:58:15.000000 hmx-v2-python-1.2.0/hmx2/abis/GmPriceAdapter.json
--rw-r--r--   0 adirut     (501) staff       (20)    47380 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/abis/LimitTradeHandler.json
--rw-r--r--   0 adirut     (501) staff       (20)     2419 2024-01-15 08:58:17.000000 hmx-v2-python-1.2.0/hmx2/abis/OnchainPricelens.json
--rw-r--r--   0 adirut     (501) staff       (20)     6721 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/abis/OrderbookOracle.json
--rw-r--r--   0 adirut     (501) staff       (20)    26489 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/abis/PerpStorage.json
--rw-r--r--   0 adirut     (501) staff       (20)    27073 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/hmx2/abis/TradeHelper.json
--rw-r--r--   0 adirut     (501) staff       (20)    24329 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/abis/VaultStorage.json
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.981786 hmx-v2-python-1.2.0/hmx2/constants/
--rw-r--r--   0 adirut     (501) staff       (20)      107 2024-04-23 11:48:11.000000 hmx-v2-python-1.2.0/hmx2/constants/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     2146 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/constants/assets.py
--rw-r--r--   0 adirut     (501) staff       (20)      397 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/constants/common.py
--rw-r--r--   0 adirut     (501) staff       (20)     3263 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/constants/contracts.py
--rw-r--r--   0 adirut     (501) staff       (20)       52 2024-04-23 11:48:11.000000 hmx-v2-python-1.2.0/hmx2/constants/intent.py
--rw-r--r--   0 adirut     (501) staff       (20)    14585 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/constants/markets.py
--rw-r--r--   0 adirut     (501) staff       (20)    20697 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/constants/pricefeed.py
--rw-r--r--   0 adirut     (501) staff       (20)    13833 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/constants/tokens.py
--rw-r--r--   0 adirut     (501) staff       (20)      237 2024-04-23 11:48:11.000000 hmx-v2-python-1.2.0/hmx2/enum.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.982230 hmx-v2-python-1.2.0/hmx2/helpers/
--rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/helpers/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)      347 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/helpers/contract_loader.py
--rw-r--r--   0 adirut     (501) staff       (20)      993 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/helpers/mapper.py
--rw-r--r--   0 adirut     (501) staff       (20)      917 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/helpers/util.py
--rw-r--r--   0 adirut     (501) staff       (20)     3002 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/hmx_client.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.982609 hmx-v2-python-1.2.0/hmx2/modules/
--rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/modules/__init__.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.982849 hmx-v2-python-1.2.0/hmx2/modules/calculator/
--rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/modules/calculator/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     8423 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/calculator/calculator.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.983170 hmx-v2-python-1.2.0/hmx2/modules/oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       48 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/__init__.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.983424 hmx-v2-python-1.2.0/hmx2/modules/oracle/calc_pricelens_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       55 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/calc_pricelens_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1209 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/calc_pricelens_oracle/calc_pricelens_oracle.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.983731 hmx-v2-python-1.2.0/hmx2/modules/oracle/cix_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 07:58:15.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/cix_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1315 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/cix_oracle/cix_oracle.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.984234 hmx-v2-python-1.2.0/hmx2/modules/oracle/glp_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/glp_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1428 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/glp_oracle/glp_oracle.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.984532 hmx-v2-python-1.2.0/hmx2/modules/oracle/gm_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       32 2023-12-01 07:58:15.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/gm_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1169 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/gm_oracle/gm_oracle.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.985031 hmx-v2-python-1.2.0/hmx2/modules/oracle/onchain_pricelens_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       59 2024-01-15 08:58:17.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)      788 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py
--rw-r--r--   0 adirut     (501) staff       (20)     3980 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/oracle_middleware.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.985424 hmx-v2-python-1.2.0/hmx2/modules/oracle/pyth_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       36 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/pyth_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1302 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py
--rw-r--r--   0 adirut     (501) staff       (20)    19728 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/private.py
--rw-r--r--   0 adirut     (501) staff       (20)    41224 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/hmx2/modules/public.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.986247 hmx-v2-python-1.2.0/hmx_v2_python.egg-info/
--rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-05-03 14:46:09.000000 hmx-v2-python-1.2.0/hmx_v2_python.egg-info/PKG-INFO
--rw-r--r--   0 adirut     (501) staff       (20)     1995 2024-05-03 14:46:09.000000 hmx-v2-python-1.2.0/hmx_v2_python.egg-info/SOURCES.txt
--rw-r--r--   0 adirut     (501) staff       (20)        1 2024-05-03 14:46:09.000000 hmx-v2-python-1.2.0/hmx_v2_python.egg-info/dependency_links.txt
--rw-r--r--   0 adirut     (501) staff       (20)      161 2024-05-03 14:46:09.000000 hmx-v2-python-1.2.0/hmx_v2_python.egg-info/requires.txt
--rw-r--r--   0 adirut     (501) staff       (20)       11 2024-05-03 14:46:09.000000 hmx-v2-python-1.2.0/hmx_v2_python.egg-info/top_level.txt
--rw-r--r--   0 adirut     (501) staff       (20)       79 2024-05-03 14:46:09.988589 hmx-v2-python-1.2.0/setup.cfg
--rw-r--r--   0 adirut     (501) staff       (20)     1464 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.0/setup.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-03 14:46:09.987894 hmx-v2-python-1.2.0/tests/
--rw-r--r--   0 adirut     (501) staff       (20)       46 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/tests/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     5934 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/tests/constants.py
--rw-r--r--   0 adirut     (501) staff       (20)     3117 2024-03-22 14:32:06.000000 hmx-v2-python-1.2.0/tests/test_create_market_order.py
--rw-r--r--   0 adirut     (501) staff       (20)     5522 2024-04-14 03:17:48.000000 hmx-v2-python-1.2.0/tests/test_deposit_collateral.py
--rw-r--r--   0 adirut     (501) staff       (20)     1307 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.0/tests/test_get_adaptive_fee.py
--rw-r--r--   0 adirut     (501) staff       (20)     1221 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.0/tests/test_init.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.288599 hmx-v2-python-1.2.1/
+-rw-r--r--   0 adirut     (501) staff       (20)     1064 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/LICENSE
+-rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-05-24 18:33:55.288729 hmx-v2-python-1.2.1/PKG-INFO
+-rw-r--r--   0 adirut     (501) staff       (20)     3361 2024-04-14 03:17:48.000000 hmx-v2-python-1.2.1/README.md
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.270151 hmx-v2-python-1.2.1/hmx2/
+-rw-r--r--   0 adirut     (501) staff       (20)       35 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/hmx2/__init__.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.276675 hmx-v2-python-1.2.1/hmx2/abis/
+-rw-r--r--   0 adirut     (501) staff       (20)     2918 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/abis/AdaptiveFeeCalculator.json
+-rw-r--r--   0 adirut     (501) staff       (20)     6094 2023-12-01 07:58:15.000000 hmx-v2-python-1.2.1/hmx2/abis/CIXPriceAdapter.json
+-rw-r--r--   0 adirut     (501) staff       (20)     3332 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/abis/CalcPricelens.json
+-rw-r--r--   0 adirut     (501) staff       (20)    19788 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.1/hmx2/abis/Calculator.json
+-rw-r--r--   0 adirut     (501) staff       (20)    79643 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/abis/ConfigStorage.json
+-rw-r--r--   0 adirut     (501) staff       (20)    23809 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/hmx2/abis/CrossMarginHandler.json
+-rw-r--r--   0 adirut     (501) staff       (20)     3685 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/hmx2/abis/ERC20.json
+-rw-r--r--   0 adirut     (501) staff       (20)    11832 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/hmx2/abis/GlpManager.json
+-rw-r--r--   0 adirut     (501) staff       (20)     5780 2023-12-01 07:58:15.000000 hmx-v2-python-1.2.1/hmx2/abis/GmPriceAdapter.json
+-rw-r--r--   0 adirut     (501) staff       (20)    47380 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/hmx2/abis/LimitTradeHandler.json
+-rw-r--r--   0 adirut     (501) staff       (20)     2419 2024-01-15 08:58:17.000000 hmx-v2-python-1.2.1/hmx2/abis/OnchainPricelens.json
+-rw-r--r--   0 adirut     (501) staff       (20)     6721 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/abis/OrderbookOracle.json
+-rw-r--r--   0 adirut     (501) staff       (20)    26489 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/abis/PerpStorage.json
+-rw-r--r--   0 adirut     (501) staff       (20)    27073 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.1/hmx2/abis/TradeHelper.json
+-rw-r--r--   0 adirut     (501) staff       (20)    24329 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/hmx2/abis/VaultStorage.json
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.279163 hmx-v2-python-1.2.1/hmx2/constants/
+-rw-r--r--   0 adirut     (501) staff       (20)      107 2024-04-23 11:48:11.000000 hmx-v2-python-1.2.1/hmx2/constants/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     2146 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/constants/assets.py
+-rw-r--r--   0 adirut     (501) staff       (20)      397 2024-05-24 18:22:53.000000 hmx-v2-python-1.2.1/hmx2/constants/common.py
+-rw-r--r--   0 adirut     (501) staff       (20)     3263 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/constants/contracts.py
+-rw-r--r--   0 adirut     (501) staff       (20)       52 2024-04-23 11:48:11.000000 hmx-v2-python-1.2.1/hmx2/constants/intent.py
+-rw-r--r--   0 adirut     (501) staff       (20)    14585 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/constants/markets.py
+-rw-r--r--   0 adirut     (501) staff       (20)    20697 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/constants/pricefeed.py
+-rw-r--r--   0 adirut     (501) staff       (20)    13833 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/constants/tokens.py
+-rw-r--r--   0 adirut     (501) staff       (20)      237 2024-04-23 11:48:11.000000 hmx-v2-python-1.2.1/hmx2/enum.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.280142 hmx-v2-python-1.2.1/hmx2/helpers/
+-rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/hmx2/helpers/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)      347 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/hmx2/helpers/contract_loader.py
+-rw-r--r--   0 adirut     (501) staff       (20)      993 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/helpers/mapper.py
+-rw-r--r--   0 adirut     (501) staff       (20)      917 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/helpers/util.py
+-rw-r--r--   0 adirut     (501) staff       (20)     3002 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/hmx_client.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.280883 hmx-v2-python-1.2.1/hmx2/modules/
+-rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/hmx2/modules/__init__.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.281613 hmx-v2-python-1.2.1/hmx2/modules/calculator/
+-rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/hmx2/modules/calculator/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     8423 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/modules/calculator/calculator.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.282273 hmx-v2-python-1.2.1/hmx2/modules/oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       48 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/__init__.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.282831 hmx-v2-python-1.2.1/hmx2/modules/oracle/calc_pricelens_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       55 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/calc_pricelens_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1209 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/calc_pricelens_oracle/calc_pricelens_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.283354 hmx-v2-python-1.2.1/hmx2/modules/oracle/cix_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 07:58:15.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/cix_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1315 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/cix_oracle/cix_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.284119 hmx-v2-python-1.2.1/hmx2/modules/oracle/glp_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/glp_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1428 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/glp_oracle/glp_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.284762 hmx-v2-python-1.2.1/hmx2/modules/oracle/gm_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       32 2023-12-01 07:58:15.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/gm_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1169 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/gm_oracle/gm_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.285409 hmx-v2-python-1.2.1/hmx2/modules/oracle/onchain_pricelens_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       59 2024-01-15 08:58:17.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)      788 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py
+-rw-r--r--   0 adirut     (501) staff       (20)     3980 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/oracle_middleware.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.285945 hmx-v2-python-1.2.1/hmx2/modules/oracle/pyth_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       36 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/pyth_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1302 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.1/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py
+-rw-r--r--   0 adirut     (501) staff       (20)    19866 2024-05-24 18:31:07.000000 hmx-v2-python-1.2.1/hmx2/modules/private.py
+-rw-r--r--   0 adirut     (501) staff       (20)    41224 2024-05-03 14:42:19.000000 hmx-v2-python-1.2.1/hmx2/modules/public.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.286784 hmx-v2-python-1.2.1/hmx_v2_python.egg-info/
+-rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-05-24 18:33:55.000000 hmx-v2-python-1.2.1/hmx_v2_python.egg-info/PKG-INFO
+-rw-r--r--   0 adirut     (501) staff       (20)     1995 2024-05-24 18:33:55.000000 hmx-v2-python-1.2.1/hmx_v2_python.egg-info/SOURCES.txt
+-rw-r--r--   0 adirut     (501) staff       (20)        1 2024-05-24 18:33:55.000000 hmx-v2-python-1.2.1/hmx_v2_python.egg-info/dependency_links.txt
+-rw-r--r--   0 adirut     (501) staff       (20)      161 2024-05-24 18:33:55.000000 hmx-v2-python-1.2.1/hmx_v2_python.egg-info/requires.txt
+-rw-r--r--   0 adirut     (501) staff       (20)       11 2024-05-24 18:33:55.000000 hmx-v2-python-1.2.1/hmx_v2_python.egg-info/top_level.txt
+-rw-r--r--   0 adirut     (501) staff       (20)       79 2024-05-24 18:33:55.289019 hmx-v2-python-1.2.1/setup.cfg
+-rw-r--r--   0 adirut     (501) staff       (20)     1464 2024-05-24 18:31:51.000000 hmx-v2-python-1.2.1/setup.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-05-24 18:33:55.288381 hmx-v2-python-1.2.1/tests/
+-rw-r--r--   0 adirut     (501) staff       (20)       46 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/tests/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     5934 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.1/tests/constants.py
+-rw-r--r--   0 adirut     (501) staff       (20)     3117 2024-03-22 14:32:06.000000 hmx-v2-python-1.2.1/tests/test_create_market_order.py
+-rw-r--r--   0 adirut     (501) staff       (20)     5522 2024-04-14 03:17:48.000000 hmx-v2-python-1.2.1/tests/test_deposit_collateral.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1307 2024-03-18 08:59:51.000000 hmx-v2-python-1.2.1/tests/test_get_adaptive_fee.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1221 2023-12-01 04:47:34.000000 hmx-v2-python-1.2.1/tests/test_init.py
```

### Comparing `hmx-v2-python-1.2.0/LICENSE` & `hmx-v2-python-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/PKG-INFO` & `hmx-v2-python-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmx-v2-python
-Version: 1.2.0
+Version: 1.2.1
 Summary: HMXv2 Python SDK
 Home-page: https://github.com/HMXOrg/v2-sdk-python
 Author: HMXOrg
 Author-email: contact@hmx.org
 License: MIT
 Keywords: hmx exchange perp dex defi ethereum eth arbitrum
 Platform: UNKNOWN
```

### Comparing `hmx-v2-python-1.2.0/README.md` & `hmx-v2-python-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/AdaptiveFeeCalculator.json` & `hmx-v2-python-1.2.1/hmx2/abis/AdaptiveFeeCalculator.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/CIXPriceAdapter.json` & `hmx-v2-python-1.2.1/hmx2/abis/CIXPriceAdapter.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/CalcPricelens.json` & `hmx-v2-python-1.2.1/hmx2/abis/CalcPricelens.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/Calculator.json` & `hmx-v2-python-1.2.1/hmx2/abis/Calculator.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/ConfigStorage.json` & `hmx-v2-python-1.2.1/hmx2/abis/ConfigStorage.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/CrossMarginHandler.json` & `hmx-v2-python-1.2.1/hmx2/abis/CrossMarginHandler.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/ERC20.json` & `hmx-v2-python-1.2.1/hmx2/abis/ERC20.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/GlpManager.json` & `hmx-v2-python-1.2.1/hmx2/abis/GlpManager.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/GmPriceAdapter.json` & `hmx-v2-python-1.2.1/hmx2/abis/GmPriceAdapter.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/LimitTradeHandler.json` & `hmx-v2-python-1.2.1/hmx2/abis/LimitTradeHandler.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/OnchainPricelens.json` & `hmx-v2-python-1.2.1/hmx2/abis/OnchainPricelens.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/OrderbookOracle.json` & `hmx-v2-python-1.2.1/hmx2/abis/OrderbookOracle.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/PerpStorage.json` & `hmx-v2-python-1.2.1/hmx2/abis/PerpStorage.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/TradeHelper.json` & `hmx-v2-python-1.2.1/hmx2/abis/TradeHelper.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/abis/VaultStorage.json` & `hmx-v2-python-1.2.1/hmx2/abis/VaultStorage.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/constants/assets.py` & `hmx-v2-python-1.2.1/hmx2/constants/assets.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/constants/contracts.py` & `hmx-v2-python-1.2.1/hmx2/constants/contracts.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/constants/markets.py` & `hmx-v2-python-1.2.1/hmx2/constants/markets.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/constants/pricefeed.py` & `hmx-v2-python-1.2.1/hmx2/constants/pricefeed.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/constants/tokens.py` & `hmx-v2-python-1.2.1/hmx2/constants/tokens.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/helpers/mapper.py` & `hmx-v2-python-1.2.1/hmx2/helpers/mapper.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/helpers/util.py` & `hmx-v2-python-1.2.1/hmx2/helpers/util.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/hmx_client.py` & `hmx-v2-python-1.2.1/hmx2/hmx_client.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/modules/calculator/calculator.py` & `hmx-v2-python-1.2.1/hmx2/modules/calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/modules/oracle/calc_pricelens_oracle/calc_pricelens_oracle.py` & `hmx-v2-python-1.2.1/hmx2/modules/oracle/calc_pricelens_oracle/calc_pricelens_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/modules/oracle/cix_oracle/cix_oracle.py` & `hmx-v2-python-1.2.1/hmx2/modules/oracle/cix_oracle/cix_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/modules/oracle/glp_oracle/glp_oracle.py` & `hmx-v2-python-1.2.1/hmx2/modules/oracle/glp_oracle/glp_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/modules/oracle/gm_oracle/gm_oracle.py` & `hmx-v2-python-1.2.1/hmx2/modules/oracle/gm_oracle/gm_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py` & `hmx-v2-python-1.2.1/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/modules/oracle/oracle_middleware.py` & `hmx-v2-python-1.2.1/hmx2/modules/oracle/oracle_middleware.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py` & `hmx-v2-python-1.2.1/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx2/modules/private.py` & `hmx-v2-python-1.2.1/hmx2/modules/private.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     return self.cross_margin_handler_instance.functions.depositCollateral(
       sub_account_id,
       token_address,
       amount_wei,
       False
     ).transact({"from": self.eth_signer.address})
 
-  def withdraw_collateral(self, sub_account_id: int, token_address: str, amount: float, wrap: bool = False):
+  def withdraw_collateral(self, sub_account_id: int, token_address: str, amount: float, execution_fee=EXECUTION_FEE, wrap: bool = False):
     '''
     Withdraw ERC20 token as collateral.
 
     :param sub_account_id: required
     :type sub_account_id: int between 0 and 255
 
     :param token_address: required
@@ -138,22 +138,22 @@
       raise Exception("Invalid collateral address")
     check_sub_account_id_param(sub_account_id)
     wrap = wrap if self.token_profile[token_address]['symbol'] == "WETH" else False
 
     amount_wei = int(
       amount * 10 ** self.token_profile[token_address]["decimals"])
 
-    transact_param = {"value": EXECUTION_FEE, "from": self.eth_signer.address,
-                      "gas": 10000000} if self.chain_id == 421614 else {"value": EXECUTION_FEE, "from": self.eth_signer.address}
+    transact_param = {"value": execution_fee, "from": self.eth_signer.address,
+                      "gas": 10000000} if self.chain_id == 421614 else {"value": execution_fee, "from": self.eth_signer.address}
 
     return self.cross_margin_handler_instance.functions.createWithdrawCollateralOrder(
       sub_account_id,
       token_address,
       amount_wei,
-      EXECUTION_FEE,
+      execution_fee,
       wrap
     ).transact(transact_param)
 
   def deposit_eth_collateral(self, sub_account_id: int, amount: float):
     '''
     Deposit ETH as collateral.
 
@@ -172,15 +172,15 @@
     return self.cross_margin_handler_instance.functions.depositCollateral(
       sub_account_id,
       eth_token,
       amount_wei,
       True
     ).transact({"from": self.eth_signer.address, "value": amount_wei})
 
-  def create_market_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, reduce_only: bool, tp_token: str = ADDRESS_ZERO, intent=False):
+  def create_market_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, reduce_only: bool, execution_fee=EXECUTION_FEE, tp_token: str = ADDRESS_ZERO, intent=False):
     '''
     Post a market order
 
     :param sub_account_id: required
     :type sub_account_id: int between 0 and 255
 
     :param market_index: required
@@ -211,33 +211,33 @@
     order = {
       "cmd": Cmd.CREATE,
       "market_index": market_index,
       "size_delta": Web3.to_wei(size, "tether") if buy else -Web3.to_wei(size, "tether"),
       "trigger_price": 0,
       "acceptable_price": MAX_UINT if buy else 0,
       "trigger_above_threshold": True,
-      "execution_fee": EXECUTION_FEE,
+      "execution_fee": execution_fee,
       "reduce_only": reduce_only,
       "tp_token": tp_token
     }
 
     tx = self.__create_order_batch(
-      self.eth_signer.address, sub_account_id, [order]
+      self.eth_signer.address, sub_account_id, execution_fee, [order]
     )
 
     # wait for transaction to be complete
     self.eth_provider.eth.wait_for_transaction_receipt(tx)
 
     events = self.__parse_log(tx, "LogCreateLimitOrder")
     args = {}
     args["tx"] = events[0]["transactionHash"]
     args["order"] = events[0]["args"]
     return args
 
-  def create_trigger_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, trigger_price: float, trigger_above_threshold: bool, reduce_only: bool, tp_token: str = ADDRESS_ZERO, intent: bool = False):
+  def create_trigger_order(self, sub_account_id: int, market_index: int, buy: bool, size: float, trigger_price: float, trigger_above_threshold: bool, reduce_only: bool, execution_fee=EXECUTION_FEE, tp_token: str = ADDRESS_ZERO, intent: bool = False):
     '''
     Post a trigger order
 
     :param sub_account_id: required
     :type sub_account_id: int between 0 and 255
 
     :param market_index: required
@@ -277,21 +277,21 @@
       "trigger_price": Web3.to_wei(trigger_price, "tether"),
       "acceptable_price": Web3.to_wei(
         self.__add_slippage(
           trigger_price) if size > 0 else self.__sub_slippage(trigger_price),
         "tether"
       ),
       "trigger_above_threshold": trigger_above_threshold,
-      "execution_fee": EXECUTION_FEE,
+      "execution_fee": execution_fee,
       "reduce_only": reduce_only,
       "tp_token": tp_token
     }
 
     tx = self.__create_order_batch(
-      self.eth_signer.address, sub_account_id, [order]
+      self.eth_signer.address, sub_account_id, execution_fee, [order]
     )
 
     self.eth_provider.eth.wait_for_transaction_receipt(tx)
 
     events = self.__parse_log(tx, "LogCreateLimitOrder")
     args = {}
     args["tx"] = events[0]["transactionHash"]
@@ -337,15 +337,15 @@
       "acceptable_price": Web3.to_wei(acceptable_price, "tether"),
       "trigger_above_threshold": trigger_above_threshold,
       "reduce_only": reduce_only,
       "tp_token": tp_token
     }
 
     tx = self.__create_order_batch(
-      self.eth_signer.address, sub_account_id, [order]
+      self.eth_signer.address, sub_account_id, 0, [order]
     )
 
     self.eth_provider.eth.wait_for_transaction_receipt(tx)
 
     events = self.__parse_log(tx, "LogUpdateLimitOrder")
     args = {}
     args["tx"] = events[0]["transactionHash"]
@@ -364,15 +364,15 @@
     '''
     order = {
       "cmd": Cmd.CANCEL,
       "order_index": order_index,
     }
 
     tx = self.__create_order_batch(
-      self.eth_signer.address, sub_account_id, [order]
+      self.eth_signer.address, sub_account_id, 0, [order]
     )
 
     self.eth_provider.eth.wait_for_transaction_receipt(tx)
 
     events = self.__parse_log(tx, "LogCancelLimitOrder")
     args = {}
     args["tx"] = events[0]["transactionHash"]
@@ -381,22 +381,22 @@
 
   def __add_slippage(self, value: float):
     return decimal.Decimal(value) * (BPS + 25) / BPS
 
   def __sub_slippage(self, value: float):
     return decimal.Decimal(value) * (BPS - 25) / BPS
 
-  def __create_order_batch(self, account: str, sub_account_id: int, orders):
+  def __create_order_batch(self, account: str, sub_account_id: int, execution_fee, orders):
     (cmds, datas) = self.__prepare_batch_input(orders)
     return self.limit_trade_handler_instance.functions.batch(
       account,
       sub_account_id,
       cmds,
       datas
-    ).transact({"from": self.eth_signer.address, "value": EXECUTION_FEE * cmds.count(Cmd.CREATE)})
+    ).transact({"from": self.eth_signer.address, "value": execution_fee * cmds.count(Cmd.CREATE)})
 
   def __prepare_batch_input(self, orders):
     return ([order["cmd"] for order in orders], [self.__prepare_order_call_data(order) for order in orders])
 
   def __prepare_order_call_data(self, order):
     if order["cmd"] == Cmd.CREATE:
       return self.__prepare_create_order_call_data(
```

### Comparing `hmx-v2-python-1.2.0/hmx2/modules/public.py` & `hmx-v2-python-1.2.1/hmx2/modules/public.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/hmx_v2_python.egg-info/PKG-INFO` & `hmx-v2-python-1.2.1/hmx_v2_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmx-v2-python
-Version: 1.2.0
+Version: 1.2.1
 Summary: HMXv2 Python SDK
 Home-page: https://github.com/HMXOrg/v2-sdk-python
 Author: HMXOrg
 Author-email: contact@hmx.org
 License: MIT
 Keywords: hmx exchange perp dex defi ethereum eth arbitrum
 Platform: UNKNOWN
```

### Comparing `hmx-v2-python-1.2.0/hmx_v2_python.egg-info/SOURCES.txt` & `hmx-v2-python-1.2.1/hmx_v2_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/setup.py` & `hmx-v2-python-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'simple-multicall-v6',
     'responses',
     'python-dotenv>=1.0.0',
 ]
 
 setup(
     name='hmx-v2-python',
-    version='1.2.0',
+    version='1.2.1',
     packages=find_packages(),
     package_data={
       'hmx2': ['abis/*.json'],
     },
     description='HMXv2 Python SDK',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
```

### Comparing `hmx-v2-python-1.2.0/tests/constants.py` & `hmx-v2-python-1.2.1/tests/constants.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/tests/test_create_market_order.py` & `hmx-v2-python-1.2.1/tests/test_create_market_order.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/tests/test_deposit_collateral.py` & `hmx-v2-python-1.2.1/tests/test_deposit_collateral.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/tests/test_get_adaptive_fee.py` & `hmx-v2-python-1.2.1/tests/test_get_adaptive_fee.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.2.0/tests/test_init.py` & `hmx-v2-python-1.2.1/tests/test_init.py`

 * *Files identical despite different names*

