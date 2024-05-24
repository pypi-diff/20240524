# Comparing `tmp/better_web3-3.2.1.tar.gz` & `tmp/better_web3-4.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-3.2.1.tar", max compression
+gzip compressed data, was "better_web3-4.0.0b2.tar", max compression
```

## Comparing `better_web3-3.2.1.tar` & `better_web3-4.0.0b2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      319 2023-08-21 17:16:57.189000 better_web3-3.2.1/better_web3/__init__.py
--rw-r--r--   0        0        0    10519 2023-08-11 17:57:06.795000 better_web3-3.2.1/better_web3/batch_call.py
--rw-r--r--   0        0        0    14897 2024-01-19 22:14:32.391614 better_web3-3.2.1/better_web3/chain.py
--rw-r--r--   0        0        0      251 2023-07-07 12:10:35.727000 better_web3-3.2.1/better_web3/contract/__init__.py
--rw-r--r--   0        0        0      525 2023-12-16 17:27:00.084000 better_web3-3.2.1/better_web3/contract/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      406 2024-01-10 21:45:55.898445 better_web3-3.2.1/better_web3/contract/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      687 2023-12-16 17:27:30.383000 better_web3-3.2.1/better_web3/contract/__pycache__/_abi.cpython-311.pyc
--rw-r--r--   0        0        0      568 2024-01-10 21:46:32.919665 better_web3-3.2.1/better_web3/contract/__pycache__/_abi.cpython-312.pyc
--rw-r--r--   0        0        0      351 2023-12-16 17:27:40.401000 better_web3-3.2.1/better_web3/contract/__pycache__/_paths.cpython-311.pyc
--rw-r--r--   0        0        0      305 2024-01-10 21:46:32.928171 better_web3-3.2.1/better_web3/contract/__pycache__/_paths.cpython-312.pyc
--rw-r--r--   0        0        0     2957 2023-12-16 17:27:01.875000 better_web3-3.2.1/better_web3/contract/__pycache__/contract.cpython-311.pyc
--rw-r--r--   0        0        0     3214 2024-01-10 21:45:55.899489 better_web3-3.2.1/better_web3/contract/__pycache__/contract.cpython-312.pyc
--rw-r--r--   0        0        0     1949 2023-12-16 17:27:33.403000 better_web3-3.2.1/better_web3/contract/__pycache__/disperse.cpython-311.pyc
--rw-r--r--   0        0        0     1612 2024-01-10 21:46:32.931171 better_web3-3.2.1/better_web3/contract/__pycache__/disperse.cpython-312.pyc
--rw-r--r--   0        0        0     3886 2023-12-16 17:27:35.432000 better_web3-3.2.1/better_web3/contract/__pycache__/erc20.cpython-311.pyc
--rw-r--r--   0        0        0     3263 2024-01-10 21:46:32.932171 better_web3-3.2.1/better_web3/contract/__pycache__/erc20.cpython-312.pyc
--rw-r--r--   0        0        0     5434 2023-12-16 17:27:37.100000 better_web3-3.2.1/better_web3/contract/__pycache__/erc721.cpython-311.pyc
--rw-r--r--   0        0        0     4409 2024-01-10 21:46:32.933172 better_web3-3.2.1/better_web3/contract/__pycache__/erc721.cpython-312.pyc
--rw-r--r--   0        0        0     9841 2023-12-16 17:27:28.421000 better_web3-3.2.1/better_web3/contract/__pycache__/multicall.cpython-311.pyc
--rw-r--r--   0        0        0     7989 2024-01-10 21:46:32.919665 better_web3-3.2.1/better_web3/contract/__pycache__/multicall.cpython-312.pyc
--rw-r--r--   0        0        0      352 2023-07-07 12:07:06.130000 better_web3-3.2.1/better_web3/contract/_abi.py
--rw-r--r--   0        0        0       99 2023-06-05 07:41:10.829000 better_web3-3.2.1/better_web3/contract/_paths.py
--rw-r--r--   0        0        0     1193 2023-06-23 09:34:50.869000 better_web3-3.2.1/better_web3/contract/abi/disperse.json
--rw-r--r--   0        0        0     6301 2023-06-05 07:31:23.813000 better_web3-3.2.1/better_web3/contract/abi/erc1155.json
--rw-r--r--   0        0        0     5904 2023-06-05 07:28:46.510000 better_web3-3.2.1/better_web3/contract/abi/erc20.json
--rw-r--r--   0        0        0     6755 2023-06-05 07:31:36.520000 better_web3-3.2.1/better_web3/contract/abi/erc721.json
--rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-3.2.1/better_web3/contract/abi/multicall_v3.json
--rw-r--r--   0        0        0     1462 2024-01-10 21:33:15.426463 better_web3-3.2.1/better_web3/contract/contract.py
--rw-r--r--   0        0        0      990 2023-08-11 17:25:57.219000 better_web3-3.2.1/better_web3/contract/disperse.py
--rw-r--r--   0        0        0     1804 2023-08-11 16:44:34.770000 better_web3-3.2.1/better_web3/contract/erc20.py
--rw-r--r--   0        0        0     2903 2023-08-11 16:44:38.452000 better_web3-3.2.1/better_web3/contract/erc721.py
--rw-r--r--   0        0        0     6290 2023-08-11 17:25:56.334000 better_web3-3.2.1/better_web3/contract/multicall.py
--rw-r--r--   0        0        0      598 2023-08-18 20:36:57.122000 better_web3-3.2.1/better_web3/provider.py
--rw-r--r--   0        0        0      730 2023-08-21 17:39:28.900000 better_web3-3.2.1/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      917 2023-12-16 17:27:32.282000 better_web3-3.2.1/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      698 2024-01-10 21:46:32.920666 better_web3-3.2.1/better_web3/utils/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4358 2023-12-16 17:27:34.414000 better_web3-3.2.1/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0     3533 2024-01-10 21:46:32.922666 better_web3-3.2.1/better_web3/utils/__pycache__/eth.cpython-312.pyc
--rw-r--r--   0        0        0     3719 2023-12-16 17:27:36.000000 better_web3-3.2.1/better_web3/utils/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     2780 2024-01-10 21:46:32.923666 better_web3-3.2.1/better_web3/utils/__pycache__/file.cpython-312.pyc
--rw-r--r--   0        0        0      837 2023-12-16 17:27:37.593000 better_web3-3.2.1/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0      707 2024-01-10 21:46:32.927171 better_web3-3.2.1/better_web3/utils/__pycache__/other.cpython-312.pyc
--rw-r--r--   0        0        0     2244 2023-08-21 17:39:28.911000 better_web3-3.2.1/better_web3/utils/eth.py
--rw-r--r--   0        0        0     1120 2023-08-21 17:35:17.049000 better_web3-3.2.1/better_web3/utils/file.py
--rw-r--r--   0        0        0      406 2023-08-21 17:39:27.911000 better_web3-3.2.1/better_web3/utils/other.py
--rw-r--r--   0        0        0     3243 2024-01-10 22:01:14.385974 better_web3-3.2.1/better_web3/wallet.py
--rw-r--r--   0        0        0      498 2024-02-24 16:28:36.627673 better_web3-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     1028 2024-02-24 16:28:32.888076 better_web3-3.2.1/README.md
--rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 better_web3-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0      577 2024-04-02 09:30:25.140486 better_web3-4.0.0b2/better_web3/__init__.py
+-rw-r--r--   0        0        0    10519 2023-08-11 17:57:06.795000 better_web3-4.0.0b2/better_web3/batch_call.py
+-rw-r--r--   0        0        0    14763 2024-04-02 12:00:11.715704 better_web3-4.0.0b2/better_web3/chain.py
+-rw-r--r--   0        0        0      191 2024-04-02 09:22:28.122802 better_web3-4.0.0b2/better_web3/chains/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-02 09:06:03.839102 better_web3-4.0.0b2/better_web3/chains/chains.py
+-rw-r--r--   0        0        0      759 2024-04-02 08:52:35.875360 better_web3-4.0.0b2/better_web3/chains/models.py
+-rw-r--r--   0        0        0     1581 2024-04-02 04:32:21.450710 better_web3-4.0.0b2/better_web3/contract.py
+-rw-r--r--   0        0        0      243 2024-04-02 09:22:28.128804 better_web3-4.0.0b2/better_web3/contracts/__init__.py
+-rw-r--r--   0        0        0      525 2023-12-16 17:27:00.084000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      406 2024-01-10 21:45:55.898445 better_web3-4.0.0b2/better_web3/contracts/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      687 2023-12-16 17:27:30.383000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/_abi.cpython-311.pyc
+-rw-r--r--   0        0        0      568 2024-01-10 21:46:32.919665 better_web3-4.0.0b2/better_web3/contracts/__pycache__/_abi.cpython-312.pyc
+-rw-r--r--   0        0        0      351 2023-12-16 17:27:40.401000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/_paths.cpython-311.pyc
+-rw-r--r--   0        0        0      305 2024-01-10 21:46:32.928171 better_web3-4.0.0b2/better_web3/contracts/__pycache__/_paths.cpython-312.pyc
+-rw-r--r--   0        0        0     1949 2023-12-16 17:27:33.403000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/disperse.cpython-311.pyc
+-rw-r--r--   0        0        0     1612 2024-01-10 21:46:32.931171 better_web3-4.0.0b2/better_web3/contracts/__pycache__/disperse.cpython-312.pyc
+-rw-r--r--   0        0        0     3886 2023-12-16 17:27:35.432000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/erc20.cpython-311.pyc
+-rw-r--r--   0        0        0     3263 2024-01-10 21:46:32.932171 better_web3-4.0.0b2/better_web3/contracts/__pycache__/erc20.cpython-312.pyc
+-rw-r--r--   0        0        0     5434 2023-12-16 17:27:37.100000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/erc721.cpython-311.pyc
+-rw-r--r--   0        0        0     4409 2024-01-10 21:46:32.933172 better_web3-4.0.0b2/better_web3/contracts/__pycache__/erc721.cpython-312.pyc
+-rw-r--r--   0        0        0     9841 2023-12-16 17:27:28.421000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/multicall.cpython-311.pyc
+-rw-r--r--   0        0        0     7989 2024-01-10 21:46:32.919665 better_web3-4.0.0b2/better_web3/contracts/__pycache__/multicall.cpython-312.pyc
+-rw-r--r--   0        0        0      352 2023-07-07 12:07:06.130000 better_web3-4.0.0b2/better_web3/contracts/_abi.py
+-rw-r--r--   0        0        0       99 2023-06-05 07:41:10.829000 better_web3-4.0.0b2/better_web3/contracts/_paths.py
+-rw-r--r--   0        0        0     1193 2023-06-23 09:34:50.869000 better_web3-4.0.0b2/better_web3/contracts/abi/disperse.json
+-rw-r--r--   0        0        0     6301 2023-06-05 07:31:23.813000 better_web3-4.0.0b2/better_web3/contracts/abi/erc1155.json
+-rw-r--r--   0        0        0     5904 2023-06-05 07:28:46.510000 better_web3-4.0.0b2/better_web3/contracts/abi/erc20.json
+-rw-r--r--   0        0        0     6755 2023-06-05 07:31:36.520000 better_web3-4.0.0b2/better_web3/contracts/abi/erc721.json
+-rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-4.0.0b2/better_web3/contracts/abi/multicall_v3.json
+-rw-r--r--   0        0        0      655 2024-04-02 04:32:21.461710 better_web3-4.0.0b2/better_web3/contracts/disperse.py
+-rw-r--r--   0        0        0     1545 2024-04-02 04:32:21.446709 better_web3-4.0.0b2/better_web3/contracts/erc20.py
+-rw-r--r--   0        0        0     2644 2024-04-02 04:32:21.458714 better_web3-4.0.0b2/better_web3/contracts/erc721.py
+-rw-r--r--   0        0        0     5777 2024-04-02 06:36:40.841552 better_web3-4.0.0b2/better_web3/contracts/multicall.py
+-rw-r--r--   0        0        0      255 2024-04-02 08:49:51.858266 better_web3-4.0.0b2/better_web3/models.py
+-rw-r--r--   0        0        0      554 2024-04-02 09:30:25.133484 better_web3-4.0.0b2/better_web3/utils/__init__.py
+-rw-r--r--   0        0        0      917 2023-12-16 17:27:32.282000 better_web3-4.0.0b2/better_web3/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      698 2024-01-10 21:46:32.920666 better_web3-4.0.0b2/better_web3/utils/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4358 2023-12-16 17:27:34.414000 better_web3-4.0.0b2/better_web3/utils/__pycache__/eth.cpython-311.pyc
+-rw-r--r--   0        0        0     3533 2024-01-10 21:46:32.922666 better_web3-4.0.0b2/better_web3/utils/__pycache__/eth.cpython-312.pyc
+-rw-r--r--   0        0        0     3719 2023-12-16 17:27:36.000000 better_web3-4.0.0b2/better_web3/utils/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     2780 2024-01-10 21:46:32.923666 better_web3-4.0.0b2/better_web3/utils/__pycache__/file.cpython-312.pyc
+-rw-r--r--   0        0        0      837 2023-12-16 17:27:37.593000 better_web3-4.0.0b2/better_web3/utils/__pycache__/other.cpython-311.pyc
+-rw-r--r--   0        0        0      707 2024-01-10 21:46:32.927171 better_web3-4.0.0b2/better_web3/utils/__pycache__/other.cpython-312.pyc
+-rw-r--r--   0        0        0     3143 2024-04-02 09:30:25.131514 better_web3-4.0.0b2/better_web3/utils/eth.py
+-rw-r--r--   0        0        0      360 2024-04-01 16:25:26.575693 better_web3-4.0.0b2/better_web3/utils/file.py
+-rw-r--r--   0        0        0      406 2024-04-02 04:04:59.695626 better_web3-4.0.0b2/better_web3/utils/other.py
+-rw-r--r--   0        0        0      563 2024-05-24 05:30:30.290708 better_web3-4.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b2/README.md
+-rw-r--r--   0        0        0     1483 1970-01-01 00:00:00.000000 better_web3-4.0.0b2/PKG-INFO
```

### Comparing `better_web3-3.2.1/better_web3/batch_call.py` & `better_web3-4.0.0b2/better_web3/batch_call.py`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/chain.py` & `better_web3-4.0.0b2/better_web3/chain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,116 +1,170 @@
 import asyncio
-from dataclasses import dataclass
 
+from better_proxy import Proxy
 from eth_account.signers.local import LocalAccount
 from eth_typing import BlockNumber, ChecksumAddress, HexStr, Address, Hash32
 from eth_utils import to_wei
 from hexbytes import HexBytes
-from web3 import AsyncWeb3
+from web3 import AsyncWeb3, AsyncHTTPProvider
 from web3.contract.async_contract import AsyncContractFunction
-from web3.middleware import async_geth_poa_middleware, async_simple_cache_middleware
+from web3.middleware import ExtraDataToPOAMiddleware
 from web3.types import (
     BlockData,
     BlockIdentifier,
     Nonce,
     TxData,
     TxParams,
     TxReceipt,
     Wei,
 )
 
-from .provider import CustomAsyncHTTPProvider
 from .batch_call import BatchCallManager
-from .contract import Contract, Multicall, Disperse, ERC20, ERC721
-from .utils import link_by_tx_hash
-
-
-@dataclass
-class NativeToken:
-    symbol: str = "ETH"
-    decimals: int = 18
+from .contract import Contract
+from .contracts import Multicall, Disperse, ERC20, ERC721
+from .utils import tx_url, tx_hash_info, tx_receipt_info
+from .models import Explorer, NativeCurrency
 
 
 class Chain:
     def __init__(
             self,
             rpc: str,
             *,
-            name: str = "EVM Chain",
-            is_testnet: bool = False,
-            use_eip1559: bool = True,
-            # Proxy
-            proxy: str = None,
-            # Native token
-            symbol: str = "ETH",
-            decimals: int = 18,
-            # Explorer
-            explorer_url: str = None,
+            explorers: list[Explorer] = None,
+            name: str = None,
+            short_name: str = None,
+            title: str = None,
+            info_url: str = None,
+            native_currency: NativeCurrency = None,
             # Connection settings
             provider_timeout: int = 15,
-            # Middlewares
-            use_poa_middleware: bool = True,
-            use_cache_middleware: bool = True,
-            # Multicall
+            proxy: str | Proxy = None,
+            # Contracts
             multicall_v3_contract_address: ChecksumAddress | str = None,
-            # Disperse
             disperse_contract_address: ChecksumAddress | str = None,
             # Batch request
             batch_request_size: int = 10,
             batch_request_delay: int = 1,
             # Tx params
+            fee_unit: str = "gwei",
             # legacy pricing
             gas_price: Wei | int = None,
             # dynamic fee pricing
             max_fee_per_gas: Wei | int = None,
             max_priority_fee_per_gas: Wei | int = None,
+            # Features
+            eip1559: bool = False,
+            # Middleware
+            use_poa_middleware: bool = True,
     ):
-        self._rpc = rpc
-        self.name = name
-        self.is_testnet = is_testnet
-        self.token = NativeToken(symbol=symbol, decimals=decimals)
-        self.explorer_url = explorer_url
-        self.use_eip1559 = use_eip1559
+        self.explorers = explorers
 
-        self.w3_provider = CustomAsyncHTTPProvider(self._rpc, proxy=proxy, request_kwargs={"timeout": provider_timeout})
-        self.w3 = AsyncWeb3(provider=self.w3_provider)
+        self.name = name
+        self.short_name = short_name
+        self.title = title
+        self.info_url = info_url
+        self.native_currency = native_currency or NativeCurrency()
+
+        self.eip1559 = eip1559
+
+        http_provider = AsyncHTTPProvider(
+            rpc,
+            request_kwargs={"timeout": provider_timeout},
+        )
+        http_provider.cache_allowed_requests = True
+        self.w3 = AsyncWeb3(provider=http_provider)
 
         if use_poa_middleware:
-            self.w3.middleware_onion.inject(async_geth_poa_middleware, layer=0)
-
-        if use_cache_middleware:
-            self.w3.middleware_onion.add(async_simple_cache_middleware)
+            self.w3.middleware_onion.inject(ExtraDataToPOAMiddleware, layer=0)
 
         self.multicall = Multicall(chain=self, address=multicall_v3_contract_address)
         self.disperse = Disperse(chain=self, address=disperse_contract_address)
 
         self.batch_request = BatchCallManager(
             self, batch_request_size, batch_request_delay)
 
-        self.default_gas_price = gas_price
-        self.default_max_fee_per_gas = max_fee_per_gas
-        self.default_max_priority_fee_per_gas = max_priority_fee_per_gas
+        self.default_gas_price = to_wei(gas_price, fee_unit) if gas_price else None
+        self.default_max_fee_per_gas = to_wei(max_fee_per_gas, fee_unit) if gas_price else None
+        self.default_max_priority_fee_per_gas = to_wei(max_priority_fee_per_gas, fee_unit) if gas_price else None
+
+        self._proxy = None
+        self.proxy = proxy
 
     def __str__(self):
         return f"{self.name}"
 
     def __repr__(self):
         return f"{self.__class__.__name__}(rpc={self.rpc}, name={self.name})"
 
     @property
+    def provider(self) -> AsyncHTTPProvider:
+        return self.w3.provider
+
+    @provider.setter
+    def provider(self, provider: AsyncHTTPProvider):
+        self.w3.provider = provider
+
+    @property
     def rpc(self):
-        return self._rpc
+        return self.provider.endpoint_uri
+
+    @property
+    def proxy(self) -> Proxy | None:
+        return self._proxy
+
+    @proxy.setter
+    def proxy(self, proxy: str | Proxy | None):
+        if proxy is None:
+            self._proxy = None
+            if "proxies" in self.provider._request_kwargs:
+                del self.provider._request_kwargs["proxies"]
+            return
+
+        if isinstance(proxy, str):
+            self._proxy = Proxy.from_str(proxy)
+
+        self.provider._request_kwargs["proxies"] = {"http": self._proxy.as_url, "https": self._proxy.as_url}
+
+    ################################################################################
+    # Tx info shortcuts
+    ################################################################################
+
+    def tx_url(
+            self,
+            tx_hash: HexBytes | HexStr | str,
+            explorer_name: str = None,
+    ):
+        if not self.explorers:
+            raise ValueError("No explorers")
+
+        target_explorer = None
 
-    def get_link_by_tx_hash(self, tx_hash: HexBytes | HexStr | str):
-        if self.explorer_url is None:
-            raise ValueError("Set explorer_url before using this method")
+        if explorer_name:
+            for explorer in self.explorers:
+                if explorer.name == explorer_name:
+                    target_explorer = explorer
+                    break
+
+            if not target_explorer:
+                raise ValueError("No explorer with this name")
+
+        else:
+            target_explorer = self.explorers[0]
 
         if isinstance(tx_hash, HexBytes):
             tx_hash = tx_hash.hex()
-        return link_by_tx_hash(self.explorer_url, tx_hash)
+
+        return tx_url(target_explorer.url, tx_hash)
+
+    def tx_hash_info(self, address: str, tx_hash: HexStr | str, value: Wei | int = None) -> str:
+        return tx_hash_info(self, address, tx_hash, value)
+
+    def tx_receipt_info(self, address: str, tx_receipt: TxReceipt, value: Wei | int = None) -> str:
+        return tx_receipt_info(self, address, tx_receipt, value)
 
     ################################################################################
     # Contract creation shortcuts
     ################################################################################
 
     def contract(self, address, abi) -> Contract:
         return Contract(self, address, abi)
@@ -160,39 +214,39 @@
     async def get_tx_receipt(self, tx_hash: Hash32 | HexBytes | HexStr) -> TxReceipt:
         return await self.w3.eth.get_transaction_receipt(tx_hash)
 
     async def wait_for_tx_receipt(
             self,
             tx_hash: Hash32 | HexBytes | HexStr,
             timeout: float = 120,
-            poll_latency: float = 0.1
+            poll_latency: float = 0.1,
     ) -> TxReceipt:
         """
         raises: TimeExhausted:
                  Raised when a method has not retrieved the desired result within a specified timeout.
                  TransactionNotFound:
                  Raised when a tx hash used to look up a tx in a jsonrpc call cannot be found.
         """
         tx_receipt = await self.w3.eth.wait_for_transaction_receipt(tx_hash, timeout, poll_latency)
 
-        # Add extra sleep to let tx propogate correctly
+        # Add extra sleep to let tx propagate correctly
         await asyncio.sleep(1)
         return tx_receipt
 
     async def get_block(
             self,
             block_identifier: BlockIdentifier,
-            full_transactions: bool = False
+            full_transactions: bool = False,
     ) -> BlockData:
         return await self.w3.eth.get_block(block_identifier, full_transactions=full_transactions)
 
     async def check_tx_with_confirmations(
             self,
             tx_hash: Hash32 | HexBytes | HexStr,
-            confirmations: int
+            confirmations: int,
     ) -> bool:
         tx_receipt = await self.get_tx_receipt(tx_hash)
 
         if not tx_receipt or tx_receipt["blockNumber"] is None:
             # If `tx_receipt` exists but `blockNumber` is `None`,
             # the transaction is still pending (only for Parity).
             return False
@@ -274,31 +328,29 @@
         elif address_from is not None:
             tx_params["nonce"] = await self.get_nonce(address_from)
 
         return tx_params
 
     async def _build_tx_fee_params(
             self,
-            # legacy pricing
             gas_price: Wei | int = None,
-            # dynamic fee pricing
             max_fee_per_gas: Wei | int = None,
             max_priority_fee_per_gas: Wei | int = None,
             *,
             tx_params: TxParams = None,
     ) -> TxParams:
         if tx_params is None:
             tx_params = dict()
         tx_params = tx_params.copy()
 
         max_fee_per_gas = max_fee_per_gas or self.default_max_fee_per_gas
         max_priority_fee_per_gas = max_priority_fee_per_gas or self.default_max_priority_fee_per_gas
 
         if (self.is_eip1559_supported and
-                ((gas_price is None and self.use_eip1559)
+                ((gas_price is None and self.eip1559)
                  or max_fee_per_gas is not None
                  or max_priority_fee_per_gas is not None)):
             tx_params["maxFeePerGas"] = max_fee_per_gas or await self.request_gas_price()
             tx_params["maxPriorityFeePerGas"] = max_priority_fee_per_gas or await self.request_max_priority_fee()
         else:
             tx_params["gasPrice"] = gas_price or await self.request_gas_price()
 
@@ -308,17 +360,15 @@
             self,
             contract_function: AsyncContractFunction,
             gas: int = None,
             address_from: Address | ChecksumAddress | str = None,
             address_to: Address | ChecksumAddress | str = None,
             nonce: Nonce | int = None,
             value: Wei | int = None,
-            # legacy pricing
             gas_price: Wei | int = None,
-            # dynamic fee pricing
             max_fee_per_gas: Wei | int = None,
             max_priority_fee_per_gas: Wei | int = None,
     ) -> TxParams:
         gas_price = gas_price or self.default_gas_price
         tx_params = await self._build_tx_base_params(gas, address_from, address_to, nonce, value)
         gas = await contract_function.estimate_gas(tx_params)
         tx_params = await self._build_tx_base_params(gas, tx_params=tx_params)
@@ -331,50 +381,11 @@
         tx_hash = await self._send_raw_tx(signed_tx.rawTransaction)
         return HexStr(tx_hash.hex())
 
     async def execute_fn(
             self,
             account: LocalAccount,
             fn: AsyncContractFunction,
-            *,
-            gas: int = None,
-            nonce: Nonce | int = None,
-            value: Wei | int = None,
-            # legacy pricing
-            gas_price: Wei | int = None,
-            # dynamic fee pricing
-            max_fee_per_gas: Wei | int = None,
-            max_priority_fee_per_gas: Wei | int = None,
-    ) -> HexStr:
-        tx = await self.build_tx(
-            fn,
-            address_from=account.address,
-            gas=gas,
-            nonce=nonce,
-            value=value,
-            gas_price=gas_price,
-            max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas,
-        )
-        tx_hash = await self.sign_and_send_tx(account, tx)
-        return tx_hash
-
-
-def load_chains(chains_data: dict, ensure_chain_id=False, **chain_kwargs) -> dict[int: Chain]:
-    chains: dict[int: Chain] = {}
-    minimal_balances: dict[int: Wei] = {}
-    for net_mode, id_to_chain_data in chains_data.items():
-        is_testnet = True if net_mode == "testnet" else False
-        for chain_id, chain_data in id_to_chain_data.items():
-            chain_id = int(chain_id)
-            if "minimal_balance" in chain_data:
-                minimal_balances[chain_id] = to_wei(chain_data.pop("minimal_balance"), "ether")
-            if "gas_price" in chain_data:
-                chain_data["gas_price"] = to_wei(chain_data["gas_price"], "gwei")
-            if "max_fee_per_gas" in chain_data:
-                chain_data["max_fee_per_gas"] = to_wei(chain_data["max_fee_per_gas"], "gwei")
-            if "max_priority_fee_per_gas" in chain_data:
-                chain_data["max_priority_fee_per_gas"] = to_wei(chain_data["max_priority_fee_per_gas"], "gwei")
-            chain = Chain(**chain_data, is_testnet=is_testnet, **chain_kwargs)
-            if ensure_chain_id and chain.chain_id == chain_id or not ensure_chain_id:
-                chains[chain_id] = chain
-    return chains, minimal_balances
+            **kwargs,
+    ) -> HexStr | TxReceipt:
+        tx = await self.build_tx(fn, address_from=account.address, **kwargs)
+        return await self.sign_and_send_tx(account, tx)
```

### Comparing `better_web3-3.2.1/better_web3/contract/__pycache__/__init__.cpython-311.pyc` & `better_web3-4.0.0b2/better_web3/contracts/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/__pycache__/_abi.cpython-311.pyc` & `better_web3-4.0.0b2/better_web3/contracts/__pycache__/_abi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/__pycache__/_abi.cpython-312.pyc` & `better_web3-4.0.0b2/better_web3/contracts/__pycache__/_abi.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/__pycache__/disperse.cpython-311.pyc` & `better_web3-4.0.0b2/better_web3/contracts/__pycache__/disperse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/__pycache__/disperse.cpython-312.pyc` & `better_web3-4.0.0b2/better_web3/contracts/__pycache__/disperse.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/__pycache__/erc20.cpython-311.pyc` & `better_web3-4.0.0b2/better_web3/contracts/__pycache__/erc20.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/__pycache__/erc20.cpython-312.pyc` & `better_web3-4.0.0b2/better_web3/contracts/__pycache__/erc20.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/__pycache__/erc721.cpython-311.pyc` & `better_web3-4.0.0b2/better_web3/contracts/__pycache__/erc721.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/__pycache__/erc721.cpython-312.pyc` & `better_web3-4.0.0b2/better_web3/contracts/__pycache__/erc721.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/__pycache__/multicall.cpython-311.pyc` & `better_web3-4.0.0b2/better_web3/contracts/__pycache__/multicall.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/__pycache__/multicall.cpython-312.pyc` & `better_web3-4.0.0b2/better_web3/contracts/__pycache__/multicall.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/abi/disperse.json` & `better_web3-4.0.0b2/better_web3/contracts/abi/disperse.json`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/abi/erc1155.json` & `better_web3-4.0.0b2/better_web3/contracts/abi/erc1155.json`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/abi/erc20.json` & `better_web3-4.0.0b2/better_web3/contracts/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/abi/erc721.json` & `better_web3-4.0.0b2/better_web3/contracts/abi/erc721.json`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/abi/multicall_v3.json` & `better_web3-4.0.0b2/better_web3/contracts/abi/multicall_v3.json`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/contract/contract.py` & `better_web3-4.0.0b2/better_web3/contract.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from typing import TYPE_CHECKING
 
-from eth_typing import ChecksumAddress
-from eth_utils import to_checksum_address
+from eth_typing import Address, ChecksumAddress
+from web3.types import ENS, ABI
 from web3 import Web3
 from web3.contract.async_contract import (
     AsyncContract,
     AsyncContractFunctions,
     AsyncContractEvents,
 )
-from web3.types import ABI
 
 if TYPE_CHECKING:
-    from ..chain import Chain
+    from .chain import Chain
 
 
 class Contract:
-    def __init__(self, chain: "Chain", address: ChecksumAddress | str, abi):
-        if isinstance(address, str):
-            address = to_checksum_address(address)
+    DEFAULT_ABI = None
+    DEFAULT_ADDRESS = None
+
+    def __init__(
+            self,
+            chain: "Chain",
+            address: Address | ChecksumAddress | ENS = None,
+            abi: ABI | str = None,
+    ):
         self._chain = chain
+        abi = abi or self.DEFAULT_ABI
+        address = address or self.DEFAULT_ADDRESS
         self._contract: AsyncContract = self._chain.w3.eth.contract(address, abi=abi)
 
     def __str__(self):
         return self.address
 
     def __repr__(self):
         return f"{self.__class__.__name__}(address={self.address}, chain.name={self.chain.name})"
```

### Comparing `better_web3-3.2.1/better_web3/contract/disperse.py` & `better_web3-4.0.0b2/better_web3/contracts/disperse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,18 @@
 from eth_typing import ChecksumAddress
 from web3.contract.async_contract import AsyncContractFunction
 from web3.types import Wei
 
 from ._abi import DISPERSE_ABI
-from .contract import Contract
-
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from ..chain import Chain
-
-
-DISPERSE_CONTRACT_ADDRESS = "0xD152f549545093347A162Dce210e7293f1452150"
+from ..contract import Contract
 
 
 class Disperse(Contract):
-    def __init__(
-        self,
-        chain: "Chain",
-        address: ChecksumAddress | str = None,
-        abi=None,
-    ):
-        address = address or DISPERSE_CONTRACT_ADDRESS
-        abi = abi or DISPERSE_ABI
-        super().__init__(chain, address, abi)
+    DEFAULT_ABI = DISPERSE_ABI
+    DEFAULT_ADDRESS = "0xD152f549545093347A162Dce210e7293f1452150"
 
     def disperse_ether(
             self,
             recipients: list[ChecksumAddress | str],
             values: list[Wei | int],
     ) -> AsyncContractFunction:
         """
```

### Comparing `better_web3-3.2.1/better_web3/contract/erc20.py` & `better_web3-4.0.0b2/better_web3/contracts/erc20.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 from functools import cached_property
-from typing import TYPE_CHECKING, Iterable
+from typing import Iterable
 
 from eth_typing import ChecksumAddress, BlockIdentifier
 from web3.types import Wei
 
 from ._abi import ERC20_ABI
-from .contract import Contract
-
-if TYPE_CHECKING:
-    from ..chain import Chain
+from ..contract import Contract
 
 
 class ERC20(Contract):
-    def __init__(
-            self,
-            chain: "Chain",
-            address: ChecksumAddress | str,
-            abi=None,
-    ):
-        abi = abi or ERC20_ABI
-        super().__init__(chain, address, abi)
+    DEFAULT_ABI = ERC20_ABI
 
     @cached_property
     async def name(self) -> str:
         return await self.functions.name().call()
 
     @cached_property
     async def symbol(self) -> str:
```

### Comparing `better_web3-3.2.1/better_web3/contract/erc721.py` & `better_web3-4.0.0b2/better_web3/contracts/erc721.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 from functools import cached_property
-from typing import TYPE_CHECKING, Iterable
+from typing import Iterable
 
 from eth_typing import ChecksumAddress, BlockIdentifier
 from eth_utils import to_checksum_address
 
 from ._abi import ERC721_ABI
-from .contract import Contract
-
-if TYPE_CHECKING:
-    from ..chain import Chain
+from ..contract import Contract
 
 
 class ERC721(Contract):
-    def __init__(
-            self,
-            chain: "Chain",
-            address: ChecksumAddress | str,
-            abi=None,
-    ):
-        abi = abi or ERC721_ABI
-        super().__init__(chain, address, abi)
+    DEFAULT_ABI = ERC721_ABI
 
     @cached_property
     def name(self) -> str:
         return self.functions.name().call()
 
     @cached_property
     def symbol(self) -> str:
```

### Comparing `better_web3-3.2.1/better_web3/contract/multicall.py` & `better_web3-4.0.0b2/better_web3/contracts/multicall.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-"""More about MulticallV3: https://github.com/mds1/multicall
 """
+More about MulticallV3: https://github.com/mds1/multicall
+"""
+
 from dataclasses import dataclass
 from typing import Any, Sequence
 
 import eth_abi
 from eth_abi.exceptions import DecodingError
 from eth_typing import BlockIdentifier, BlockNumber, ChecksumAddress
 from hexbytes import HexBytes
 from web3._utils.abi import map_abi_data
 from web3._utils.normalizers import BASE_RETURN_NORMALIZERS
-from web3.contract.async_contract import AsyncContract, AsyncContractFunction
+from web3.contract.async_contract import AsyncContractFunction
 from web3.exceptions import ContractLogicError
 
 from ._abi import MULTICALL_V3_ABI
-from .contract import Contract
-
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from ..chain import Chain
-
-
-MULTICALL_V3_CONTRACT_ADDRESS = "0xcA11bde05977b3631167028862bE2a173976CA11"
+from ..contract import Contract
 
 
 @dataclass
 class MulticallResult:
     success: bool
     return_data: bytes | None
 
@@ -36,23 +31,16 @@
 
 
 class MulticallFailed(Exception):
     pass
 
 
 class Multicall(Contract):
-    def __init__(
-        self,
-        chain: "Chain",
-        address: ChecksumAddress | str = None,
-        abi=None,
-    ):
-        address = address or MULTICALL_V3_CONTRACT_ADDRESS
-        abi = abi or MULTICALL_V3_ABI
-        super().__init__(chain, address, abi)
+    DEFAULT_ABI = MULTICALL_V3_ABI
+    DEFAULT_ADDRESS = "0xcA11bde05977b3631167028862bE2a173976CA11"
 
     @staticmethod
     def _build_payload(
         contract_functions: Sequence[AsyncContractFunction],
     ) -> tuple[list[tuple[ChecksumAddress, bytes]], list[list[Any]]]:
         targets_with_data = []
         output_types = []
@@ -67,36 +55,31 @@
                 [output["type"] for output in contract_function.abi["outputs"]]
             )
 
         return targets_with_data, output_types
 
     @staticmethod
     def _decode_data(output_type: Sequence[str], data: bytes) -> Any | None:
-        """
+        if not data:
+            return
 
-        :param output_type:
-        :param data:
-        :return:
-        :raises: DecodingError
-        """
-        if data:
-            try:
-                decoded_values = eth_abi.decode(output_type, data)
-                normalized_data = map_abi_data(
-                    BASE_RETURN_NORMALIZERS, output_type, decoded_values
-                )
-                if len(normalized_data) == 1:
-                    return normalized_data[0]
-                else:
-                    return normalized_data
-            except DecodingError:
-                print(
-                    "Cannot decode %s using output-type %s", data, output_type
-                )
-                return data
+        try:
+            decoded_values = eth_abi.decode(output_type, data)
+            normalized_data = map_abi_data(
+                BASE_RETURN_NORMALIZERS, output_type, decoded_values
+            )
+            if len(normalized_data) == 1:
+                return normalized_data[0]
+            else:
+                return normalized_data
+        except DecodingError:
+            print(
+                "Cannot decode %s using output-type %s", data, output_type
+            )
+            return data
 
     async def _aggregate(
         self,
         targets_with_data: Sequence[tuple[ChecksumAddress, bytes]],
         block_identifier: BlockIdentifier = "latest",
     ) -> tuple[BlockNumber, list[Any | None]]:
         """
```

### Comparing `better_web3-3.2.1/better_web3/utils/__pycache__/__init__.cpython-311.pyc` & `better_web3-4.0.0b2/better_web3/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/utils/__pycache__/__init__.cpython-312.pyc` & `better_web3-4.0.0b2/better_web3/utils/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/utils/__pycache__/eth.cpython-311.pyc` & `better_web3-4.0.0b2/better_web3/utils/__pycache__/eth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/utils/__pycache__/eth.cpython-312.pyc` & `better_web3-4.0.0b2/better_web3/utils/__pycache__/eth.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/utils/__pycache__/file.cpython-311.pyc` & `better_web3-4.0.0b2/better_web3/utils/__pycache__/file.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/utils/__pycache__/file.cpython-312.pyc` & `better_web3-4.0.0b2/better_web3/utils/__pycache__/file.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/utils/__pycache__/other.cpython-311.pyc` & `better_web3-4.0.0b2/better_web3/utils/__pycache__/other.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/better_web3/utils/__pycache__/other.cpython-312.pyc` & `better_web3-4.0.0b2/better_web3/utils/__pycache__/other.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-3.2.1/README.md` & `better_web3-4.0.0b2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,13 +5,9 @@
 [![PyPI downloads per month](https://img.shields.io/pypi/dm/better-web3.svg)](https://pypi.python.org/pypi/better-web3)
 
 ```bash
 pip install better-web3
 ```
 
 More libraries of the family:
+- [tweepy-self](https://github.com/alenkimov/tweepy-self)
 - [better-proxy](https://github.com/alenkimov/better_proxy)
-- [better-automation](https://github.com/alenkimov/better_automation)
-
-## Credits
-- [safe-global](https://github.com/safe-global) / [Safe-eth-py (previosly known as Gnosis-py)](https://github.com/safe-global/safe-eth-py)
-- [Whynot63](https://github.com/Whynot63) / [web3-premium](https://github.com/Whynot63/web3-premium)
```

