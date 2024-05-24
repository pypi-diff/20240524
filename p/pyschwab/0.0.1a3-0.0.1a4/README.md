# Comparing `tmp/pyschwab-0.0.1a3.tar.gz` & `tmp/pyschwab-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyschwab-0.0.1a3.tar", max compression
+gzip compressed data, was "pyschwab-0.0.1a4.tar", max compression
```

## Comparing `pyschwab-0.0.1a3.tar` & `pyschwab-0.0.1a4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1066 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/LICENSE
--rw-r--r--   0        0        0     3878 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/README.md
--rw-r--r--   0        0        0     1033 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/pyschwab/__init__.py
--rw-r--r--   0        0        0     5685 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/pyschwab/auth.py
--rw-r--r--   0        0        0     1049 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/pyschwab/exceptions.py
--rw-r--r--   0        0        0      372 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/pyschwab/log.py
--rw-r--r--   0        0        0     5741 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/pyschwab/market.py
--rw-r--r--   0        0        0    13261 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/pyschwab/market_models.py
--rw-r--r--   0        0        0     7640 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/pyschwab/trading.py
--rw-r--r--   0        0        0    17480 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/pyschwab/trading_models.py
--rw-r--r--   0        0        0     6052 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/pyschwab/types.py
--rw-r--r--   0        0        0     1013 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/pyschwab/user_input.py
--rw-r--r--   0        0        0     6161 2024-05-22 12:37:16.020563 pyschwab-0.0.1a3/pyschwab/utils.py
--rw-r--r--   0        0        0     4930 1970-01-01 00:00:00.000000 pyschwab-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-24 18:04:34.866068 pyschwab-0.0.1a4/LICENSE
+-rw-r--r--   0        0        0     3628 2024-05-24 18:04:34.866068 pyschwab-0.0.1a4/README.md
+-rw-r--r--   0        0        0     1033 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/__init__.py
+-rw-r--r--   0        0        0     5685 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/auth.py
+-rw-r--r--   0        0        0     1049 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/exceptions.py
+-rw-r--r--   0        0        0      372 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/log.py
+-rw-r--r--   0        0        0     5736 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/market.py
+-rw-r--r--   0        0        0    13261 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/market_models.py
+-rw-r--r--   0        0        0    10612 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/trading.py
+-rw-r--r--   0        0        0    19645 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/trading_models.py
+-rw-r--r--   0        0        0     9711 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/types.py
+-rw-r--r--   0        0        0     1013 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/user_input.py
+-rw-r--r--   0        0        0     7131 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/utils.py
+-rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 pyschwab-0.0.1a4/PKG-INFO
```

### Comparing `pyschwab-0.0.1a3/LICENSE` & `pyschwab-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a3/README.md` & `pyschwab-0.0.1a4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -48,34 +48,29 @@
 access_token = authorizer.get_access_token()
 print(access_token)
 
 # Example usage of trading APIs
 trading_api = TradingApi(access_token, app_config['trading'])
 
 account_num = 0 # CHANGE this to your actual account number
-trading_data = trading_api.fetch_trading_data(account_num)
+trading_api.set_current_account_number(account_num)
+trading_data = trading_api.fetch_trading_data()
 # List positions
 for position in trading_data.positions:
     print("position:", position)
 
 # List transactions 
-for transaction in trading_api.get_transactions(account_num):
+for transaction in trading_api.get_transactions():
     print("transaction:", transaction)
 
 # Place order
-order_dict = {
-    "orderType": "LIMIT", "session": "NORMAL", "duration": "DAY", "orderStrategyType": "SINGLE", "price": '100.00',
-    "orderLegCollection": [
-        {"instruction": "BUY", "quantity": 1, "instrument": {"symbol": "TSLA", "assetType": "EQUITY"}}
-    ]
-    }
-trading_api.place_order(order_dict, account_num)
+trading_api.buy_equity("TSLA", quantity=1, price=100)
 
 # List orders
-for order in trading_api.get_orders(account_num):
+for order in trading_api.get_orders():
     print("order:", order)
 
 # Example usage of market APIs
 market_api = MarketApi(access_token, app_config['market'])
 
 # Get quotes
 symbols = ['TSLA', 'NVDA']
```

### Comparing `pyschwab-0.0.1a3/pyproject.toml` & `pyschwab-0.0.1a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyschwab"
-version = "0.0.1a3"
+version = "0.0.1a4"
 description = "A Python library for the Schwab trading API"
 authors = ["Hui Zheng <xyz.dll@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hzheng/pyschwab"
 documentation = "https://pyschwab.readthedocs.io"
 keywords = ["finance", "trading", "schwab", "api", "python"]
```

### Comparing `pyschwab-0.0.1a3/pyschwab/auth.py` & `pyschwab-0.0.1a4/pyschwab/auth.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a3/pyschwab/exceptions.py` & `pyschwab-0.0.1a4/pyschwab/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a3/pyschwab/market.py` & `pyschwab-0.0.1a4/pyschwab/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .types import MarketType, MoverSort, OptionStrategy, PeriodFrequency, SecuritySearch
 from .utils import format_list, format_params, request, time_to_int, time_to_str
 
 
 """
 Schwab Market API
 
-Reference: https://beta-developer.schwab.com/products/trader-api--individual/details/specifications/Market%20Data%20Production
+Reference: https://developer.schwab.com/products/trader-api--individual/details/specifications/Market%20Data%20Production
 """
 class MarketApi:
     base_market_url: str
 
     def __init__(self, access_token: str, market_config: Dict[str, Any]):
         load_dotenv()
         self.base_market_url = market_config['base_market_url']
```

### Comparing `pyschwab-0.0.1a3/pyschwab/market_models.py` & `pyschwab-0.0.1a4/pyschwab/market_models.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a3/pyschwab/trading.py` & `pyschwab-0.0.1a4/pyschwab/trading.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,143 +1,190 @@
 from datetime import datetime, timedelta
 from typing import Any, Dict, List
 
 from dotenv import load_dotenv
 
-from .utils import format_params, request, time_to_str, to_json_str
-from .trading_models import Order, SecuritiesAccount, TradingData, Transaction, UserPreference
-from .types import OrderStatus, TransactionType
+from .utils import format_params, remove_none_values, request, time_to_str, to_json_str
+from .trading_models import Instrument, Order, OrderLeg, SecuritiesAccount, TradingData, Transaction, UserPreference
+from .types import AssetType, ExecutionType, MarketSession, OrderDuration, OrderInstruction, OrderStatus, OrderStrategyType, OrderType, TransactionType
 
 
 """
 Schwab Trading API
 
-Reference: https://beta-developer.schwab.com/products/trader-api--individual/details/specifications/Retail%20Trader%20API%20Production
+Reference: https://developer.schwab.com/products/trader-api--individual/details/specifications/Retail%20Trader%20API%20Production
 """
 class TradingApi:
     base_trader_url: str
 
     def __init__(self, access_token: str, trading_config: Dict[str, Any]):
         load_dotenv()
         self.base_trader_url = trading_config['base_trader_url']
         self.auth = {'Authorization': f'Bearer {access_token}'}
         self.auth2 = {**self.auth, 'Content-Type': 'application/json'}
         response = request(f'{self.base_trader_url}/accounts/accountNumbers', headers=self.auth).json()
         self.accounts_hash = {account.get('accountNumber'): account.get('hashValue') for account in response}
         self.accounts: Dict[str, SecuritiesAccount] = {}
+        self.current_account_num = None
  
     def get_accounts_hash(self) -> Dict[str, str]:
         return self.accounts_hash
  
-    def get_account_hash(self, account_number: str) -> str:
-        return self.accounts_hash.get(account_number, None)
+    def set_current_account_number(self, account_number: str) -> None:
+        self.current_account_num = account_number
+
+    def get_current_account_number(self) -> str:
+        return self.current_account_num
+
+    def get_account_hash(self, account_number: str=None) -> str:
+        return self.accounts_hash.get(account_number or self.current_account_num, None)
  
     def get_accounts(self) -> Dict[str, SecuritiesAccount]:
         return self.accounts
  
-    def get_account(self, account_number: str) -> SecuritiesAccount:
-        return self.accounts.get(account_number, None)
+    def get_account(self, account_number: str=None) -> SecuritiesAccount:
+        return self.accounts.get(account_number or self.current_account_num, None)
+
+    def _get_account_hash(self, account_num: int | str=None) -> str:
+        account_num = account_num or self.current_account_num
+        if not account_num:
+            raise ValueError("Account number not set")
 
-    def _get_account_hash(self, account_num: int | str) -> str:
         account_hash = self.accounts_hash.get(str(account_num), None)
         if account_hash is None:
             raise ValueError(f"Account number {account_num} not found.")
         return account_hash
-    
+ 
     def get_user_preference(self):
         response = request(f'{self.base_trader_url}/userPreference', headers=self.auth).json()
         return UserPreference.from_dict(response)
 
-    def fetch_trading_data(self, account_num: str, include_pos: bool=True) -> TradingData:
-        account_hash = self._get_account_hash(account_num)
+    def fetch_trading_data(self, include_pos: bool=True) -> TradingData:
+        account_hash = self._get_account_hash()
         params = {'fields': ['positions'] if include_pos else []}
         resp = request(f'{self.base_trader_url}/accounts/{account_hash}', headers=self.auth, params=params).json()
         trading_data = TradingData.from_dict(resp)
         account = trading_data.account
         self.accounts[account.account_number] = account
         return trading_data
 
-
     def fetch_all_trading_data(self, include_pos: bool=True) -> Dict[str, TradingData]:
         params = {'fields': ['positions'] if include_pos else []}
         trading_data_map = {}
         for resp in request(f'{self.base_trader_url}/accounts/', headers=self.auth, params=params).json():
             trading_data = TradingData.from_dict(resp)
             account = trading_data.account
             account_num = account.account_number
             trading_data_map[account_num] = trading_data
             self.accounts[account_num] = account
         return trading_data_map
 
-    def get_all_orders(self, start_time: datetime=None, end_time: datetime=None, status: OrderStatus=None, max_results: int=100) -> List[Order]:
+    def get_all_orders(self, start_time: datetime=None, end_time: datetime=None, status: OrderStatus=None, max_results: int=None) -> List[Order]:
         now = datetime.now()
-        start = time_to_str(start_time or now - timedelta(days=30))
-        end = time_to_str(end_time or now)
+        start = time_to_str(start_time or now - timedelta(days=60))
+        end = time_to_str(end_time or now + timedelta(days=1))
         params = {'maxResults': max_results, 'fromEnteredTime': start, 'toEnteredTime': end, 'status': status}
         orders = request(f'{self.base_trader_url}/orders', headers=self.auth, params=format_params(params)).json()
         return [Order.from_dict(order) for order in orders]
 
-    def get_orders(self, account_num: str, start_time: datetime=None, end_time: datetime=None, status: OrderStatus=None, max_results: int=100) -> List[Order]:
-        account_hash = self._get_account_hash(account_num)
+    def get_orders(self, start_time: datetime=None, end_time: datetime=None, status: OrderStatus=None, max_results: int=None) -> List[Order]:
+        account_hash = self._get_account_hash()
         now = datetime.now()
-        start = time_to_str(start_time or now - timedelta(days=30))
-        end = time_to_str(end_time or now)
+        start = time_to_str(start_time or now - timedelta(days=60))
+        end = time_to_str(end_time or now + timedelta(days=1))
         params = {'maxResults': max_results, 'fromEnteredTime': start, 'toEnteredTime': end, 'status': status}
         orders = request(f'{self.base_trader_url}/accounts/{account_hash}/orders', headers=self.auth, params=format_params(params)).json()
         return [Order.from_dict(order) for order in orders]
 
-    def get_order(self, account_num: int | str, order_id: str) -> Order:
+    @staticmethod
+    def is_active_order(order: Order) -> bool:
+        if order.status.is_inactive():
+            return False
+
+        activities = order.order_activity_collection
+        if activities:
+            if activities[0].execution_type == ExecutionType.CANCELED:
+                return False
+        return order.cancel_time is None
+
+    def get_working_orders(self, start_time: datetime=None, end_time: datetime=None) -> List[Order]:
+        return self.get_orders(start_time, end_time, status=OrderStatus.WORKING)
+
+    def get_order(self, order_id: str, account_num: int | str=None) -> Order:
         account_hash = self._get_account_hash(account_num)
         order = request(f'{self.base_trader_url}/accounts/{account_hash}/orders/{order_id}', headers=self.auth).json()
         return Order.from_dict(order)
 
-    def place_order(self, order: Dict[str, Any] | Order, account_num: int | str) -> None:
-        account_hash = self._get_account_hash(account_num)
+    def place_order(self, order: Dict[str, Any] | Order) -> None:
+        account_hash = self._get_account_hash()
         order_dict = self._convert_order(order)
         request(f'{self.base_trader_url}/accounts/{account_hash}/orders', method='POST', headers=self.auth, json=order_dict)
+ 
+    def place_complex_order(self, price: float, leg_collection: List[OrderLeg],
+                    strategy_type: OrderStrategyType=OrderStrategyType.SINGLE, order_type: OrderType=OrderType.LIMIT,
+                    duration: OrderDuration=OrderDuration.DAY, session: MarketSession=MarketSession.NORMAL) -> None:
+        order = Order(price=price, order_leg_collection=leg_collection, order_strategy_type=strategy_type,
+                      order_type=order_type, duration=duration, session=session)
+        self.place_order(order)
+
+    def place_single_order(self, symbol: str, quantity: int, price: float, instruction: OrderInstruction, 
+            asset_type: AssetType=AssetType.EQUITY, order_type: OrderType=OrderType.LIMIT,
+            duration: OrderDuration=OrderDuration.DAY, session: MarketSession=MarketSession.NORMAL) -> None:
+        instrument = Instrument(symbol=symbol, asset_type=asset_type)
+        leg_collection = [OrderLeg(instruction=instruction, quantity=quantity, instrument=instrument)]
+        self.place_complex_order(price=price, leg_collection=leg_collection, strategy_type=OrderStrategyType.SINGLE,
+                                 order_type=order_type, duration=duration, session=session)
+ 
+    def buy_equity(self, symbol: str, quantity: int, price: float, order_type: OrderType=OrderType.LIMIT,
+                   duration: OrderDuration=OrderDuration.DAY, session: MarketSession=MarketSession.NORMAL) -> None:
+        self.place_single_order(symbol=symbol, quantity=quantity, price=price, instruction=OrderInstruction.BUY,
+                                order_type=order_type, duration=duration, session=session)
+ 
+    def sell_equity(self, symbol: str, price: float, quantity: int, order_type: OrderType=OrderType.LIMIT,
+                   duration: OrderDuration=OrderDuration.DAY, session: MarketSession=MarketSession.NORMAL) -> None:
+        self.place_single_order(symbol=symbol, quantity=quantity, price=price, instruction=OrderInstruction.SELL,
+                                order_type=order_type, duration=duration, session=session)
 
-    def cancel_order(self, order_id: int | str, account_num: int | str) -> None:
-        account_hash = self._get_account_hash(account_num)
+    def cancel_order(self, order_id: int | str) -> None:
+        account_hash = self._get_account_hash()
         request(f'{self.base_trader_url}/accounts/{account_hash}/orders/{order_id}', method='DELETE', headers=self.auth)
 
     def replace_order(self, order: Dict[str, Any] | Order) -> None:
         order_dict = self._convert_order(order)
         order_id = order_dict.get('orderId', None)
         if not order_id:
             raise ValueError("Order ID not found in order data.")
-        account_num = order_dict.get('accountNumber', None)
-        if not account_num:
-            raise ValueError("Account number not found in order data.")
 
-        account_hash = self._get_account_hash(account_num)
+        account_hash = self._get_account_hash()
         order_json = to_json_str(order_dict)
         request(f'{self.base_trader_url}/accounts/{account_hash}/orders/{order_id}', method='PUT', headers=self.auth2, data=order_json)
 
-    def preview_order(self, order: Dict[str, Any] | Order, account_num: int | str) -> Dict[str, Any]:
+    def preview_order(self, order: Dict[str, Any] | Order) -> Dict[str, Any]:
         """Coming Soon as per official document"""
-        account_hash = self._get_account_hash(account_num)
+        account_hash = self._get_account_hash()
         order_dict = self._convert_order(order)
         order_json = to_json_str(order_dict)
         return request(f'{self.base_trader_url}/accounts/{account_hash}/previewOrder', method='POST', headers=self.auth2, data=order_json).json()
 
     def _convert_order(self, order: Dict[str, Any] | Order) -> Dict[str, Any]:
+        order_dict = None
         if isinstance(order, Dict):
-            return order
-
-        if isinstance(order, Order):
-            return order.to_dict(clean_keys=True)
- 
-        raise ValueError("Order must be a dictionary or Order object.")
+            order_dict = order
+        elif isinstance(order, Order):
+            order_dict = order.to_dict(clean_keys=True)
+        else:
+            raise ValueError("Order must be a dictionary or Order object.")
+        return remove_none_values(order_dict)
 
-    def get_transactions(self, account_num: str, start_time: datetime=None, end_time: datetime=None, symbol: str=None, types: TransactionType=TransactionType.TRADE) -> List[Transaction]:
-        account_hash = self._get_account_hash(account_num)
+    def get_transactions(self, start_time: datetime=None, end_time: datetime=None, symbol: str=None, types: TransactionType=TransactionType.TRADE) -> List[Transaction]:
+        account_hash = self._get_account_hash()
         now = datetime.now()
         start = time_to_str(start_time or now - timedelta(days=30))
         end = time_to_str(end_time or now)
         params = {'startDate': start, 'endDate': end, 'symbol': symbol, 'types': types}
         transactions = request(f'{self.base_trader_url}/accounts/{account_hash}/transactions', headers=self.auth, params=format_params(params)).json()
         return [Transaction.from_dict(transaction) for transaction in transactions]
 
-    def get_transaction(self, account_num: int | str, transaction_id: str) -> Transaction:
-        account_hash = self._get_account_hash(account_num)
+    def get_transaction(self, transaction_id: str) -> Transaction:
+        account_hash = self._get_account_hash()
         transaction = request(f'{self.base_trader_url}/accounts/{account_hash}/transactions/{transaction_id}', headers=self.auth).json()
         return Transaction.from_dict(transaction)
```

### Comparing `pyschwab-0.0.1a3/pyschwab/trading_models.py` & `pyschwab-0.0.1a4/pyschwab/trading_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
+from .types import ActivityType, AssetType, ComplexOrderStrategyType, ExecutionType, MarketSession, OptionActionType, \
+    OptionAssetType, OrderDuration, OrderInstruction, OrderStatus, OrderStrategyType, OrderType, \
+    PositionEffect, QuantityType, RequestedDestination
 from .utils import camel_to_snake, dataclass_to_dict, to_time
 
 
 @dataclass
 class SecuritiesAccount:
     """
     Represents a security account with various properties related to trading.
@@ -32,26 +35,27 @@
         """
         converted_data = {camel_to_snake(key): value for key, value in data.items()}
         return cls(**converted_data)
 
 
 @dataclass
 class Deliverable:
-    asset_type: str
+    asset_type: OptionAssetType
     status: str
     symbol: str
     instrument_id: int
     closing_price: float
     type: str
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> 'Deliverable':
         if data is None:
             return None
         converted_data = {camel_to_snake(key): value for key, value in data.items()}
+        converted_data['asset_type'] = OptionAssetType.from_str(converted_data['asset_type'])
         return cls(**converted_data)
 
 
 @dataclass
 class OptionDeliverable:
     deliverable_units: float
     deliverable: Deliverable
@@ -70,33 +74,33 @@
 
 @dataclass
 class Instrument:
     """
     Represents the financial instrument in a trading position.
     
     Attributes:
-        asset_type (str): The type of the asset, e.g., 'EQUITY'.
+        asset_type (AssetType): The type of the asset, e.g., AssetType.EQUITY.
         symbol (str): The trading symbol for the instrument.
         cusip (str): The CUSIP identifier for the instrument.
         net_change (float): The net change in the instrument's value since the last close.
         instrument_id (int): The id of the instrument
     """
-    asset_type: str
     symbol: str
+    asset_type: AssetType = AssetType.EQUITY
     cusip: str = None
-    net_change: float = 0.0
-    instrument_id: int = 0
+    net_change: float = None
+    instrument_id: int = None
     description: str = None
-    closing_price: float = 0.0
+    closing_price: float = None
     status: str = None
     type: str = None
     expiration_date: datetime = None
     option_deliverables: List[Deliverable] = None
-    option_premium_multiplier: float = 0.0
-    put_call: str = None
+    option_premium_multiplier: float = None
+    put_call: OptionActionType = None
     strike_price: float = None
     underlying_symbol: str = None
     underlying_cusip: str = None
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> 'Instrument':
         """
@@ -105,14 +109,16 @@
         converted_data = {camel_to_snake(key): value for key, value in data.items()}
         expiration_time = converted_data.get('expiration_date', None)
         if expiration_time:
             converted_data['expiration_date'] = datetime.fromisoformat(expiration_time)
         deliverables = converted_data.get('option_deliverables', None)
         if deliverables:
             converted_data['option_deliverables'] = [OptionDeliverable.from_dict(deliverable) for deliverable in converted_data['option_deliverables']]
+        converted_data['asset_type'] = AssetType.from_str(converted_data['asset_type'])
+        converted_data['put_call'] = OptionActionType.from_str(converted_data.get('put_call', None))
         return cls(**converted_data)
 
 
 @dataclass
 class Position:
     """
     Represents a trading position.
@@ -282,102 +288,115 @@
         converted_data = {camel_to_snake(key): value for key, value in data.items()}
         converted_data['time'] = datetime.fromisoformat(converted_data['time'])
         return cls(**converted_data)
 
 
 @dataclass
 class OrderActivity:
-    activity_type: str
-    execution_type: str
+    activity_type: ActivityType
+    execution_type: ExecutionType
     quantity: int
     order_remaining_quantity: int
     execution_legs: List[ExecutionLeg]
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> 'OrderActivity':
         converted_data = {camel_to_snake(key): value for key, value in data.items()}
+        converted_data['activity_type'] = ActivityType.from_str(converted_data.get('activity_type', None))
+        converted_data['execution_type'] = ExecutionType.from_str(converted_data.get('execution_type', None))
         converted_data['execution_legs'] = [ExecutionLeg.from_dict(leg) for leg in converted_data['execution_legs']]
         return cls(**converted_data)
 
 
 @dataclass
 class OrderLeg:
     instrument: Instrument
-    instruction: str
+    instruction: OrderInstruction
     quantity: int
-    position_effect: str = 'OPENING'
-    order_leg_type: str = 'EQUITY'
-    leg_id: int = 0
-    quantity_type: str = None
+    position_effect: PositionEffect = None
+    order_leg_type: AssetType = None
+    quantity_type: QuantityType = None
+    leg_id: int = None
     div_cap_gains: str = None
     to_symbol: str = None
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> 'OrderLeg':
         converted_data = {camel_to_snake(key): value for key, value in data.items()}
         converted_data['instrument'] = Instrument.from_dict(converted_data['instrument'])
+        converted_data['instruction'] = OrderInstruction.from_str(converted_data['instruction'])
+        converted_data['position_effect'] = PositionEffect.from_str(converted_data.get('position_effect', None))
+        converted_data['order_leg_type'] = AssetType.from_str(converted_data.get('order_leg_type', None))
+        converted_data['quantity_type'] = QuantityType.from_str(converted_data.get('quantity_type', None))
         return cls(**converted_data)
 
 
 @dataclass
 class Order:
-    order_type: str
-    session: str
     price: float
-    duration: str
-    entered_time: datetime
-    close_time: datetime
-    release_time: datetime
-    order_id: int = 0
-    account_number: int = 0
-    status: str = 'AWAITING_PARENT_ORDER'
-    quantity: int = 0
-    filled_quantity: int = 0
-    remaining_quantity: int = 0
-    complex_order_strategy_type: str = "NONE"
-    requested_destination: str = "AUTO"
+    entered_time: datetime = None
+    close_time: datetime = None
+    release_time: datetime = None
+    order_type: OrderType = OrderType.LIMIT
+    duration: OrderDuration = OrderDuration.DAY
+    session: MarketSession = MarketSession.NORMAL
+    order_strategy_type: OrderStrategyType = OrderStrategyType.SINGLE
+    order_id: int = None
+    account_number: int = None
+    status: OrderStatus = None
+    quantity: int = None
+    filled_quantity: int = None
+    remaining_quantity: int = None
+    complex_order_strategy_type: ComplexOrderStrategyType = None
+    requested_destination: RequestedDestination = None
     destination_link_name: str = None
     order_leg_collection: List[OrderLeg] = None
     order_activity_collection: List[OrderActivity] = None
-    stop_price: float = 0.0
+    stop_price: float = None
     stop_price_link_basis: str = None
     stop_price_link_type: str = None
     stop_price_offset: float = None
     stop_type: str = None
     price_link_basis: str = None
     price_link_type: str = None
     tax_lot_method: str = None
-    activation_price: float = 0.0
+    activation_price: float = None
     special_instruction: str = None
-    order_strategy_type: str = None
-    cancelable: bool = False
-    editable: bool = False
+    cancelable: bool = None
+    editable: bool = None
     cancel_time: datetime = None
     tag: str = None
     status_description: str = None
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> 'Order':
         converted_data = {camel_to_snake(key): value for key, value in data.items()}
         for key in ['cancel_time', 'release_time', 'entered_time', 'close_time']:
             converted_data[key] = to_time(converted_data.get(key, None))
         converted_data['order_leg_collection'] = [OrderLeg.from_dict(leg) for leg in converted_data.get('order_leg_collection', [])]
         converted_data['order_activity_collection'] = [OrderActivity.from_dict(activity) for activity in converted_data.get('order_activity_collection', [])]
+        converted_data['order_type'] = OrderType.from_str(converted_data['order_type'])
+        converted_data['duration'] = OrderDuration.from_str(converted_data['duration'])
+        converted_data['session'] = MarketSession.from_str(converted_data['session'])
+        converted_data['order_strategy_type'] = OrderStrategyType.from_str(converted_data['order_strategy_type'])
+        converted_data['status'] = OrderStatus.from_str(converted_data.get('status', None))
+        converted_data['complex_order_strategy_type'] = ComplexOrderStrategyType.from_str(converted_data.get('complex_order_strategy_type', None))
         return cls(**converted_data)
 
     def to_dict(self, clean_keys: bool=False) -> Dict[str, Any]:
         order_dict = dataclass_to_dict(self)
         if clean_keys:
             for key in ['enteredTime', 'closeTime', 'releaseTime', 'cancelTime', # time
                         'remainingQuantity', 'filledQuantity', 'quantity', # quanity
                         'priceLinkBasis', 'priceLinkType', 'activationPrice', # price
                         'stopPriceLinkBasis', 'stopPrice', 'stopPriceOffset', 'stopType', # stop
                         'destinationLinkName', 'requestedDestination', # destination
                         'status', 'statusDescription', # status
                         'tag', # tag
+                        'orderActivityCollection',
                         ]:
                 del order_dict[key]
         return order_dict
 
 
 @dataclass
 class TransferItem:
```

### Comparing `pyschwab-0.0.1a3/pyschwab/user_input.py` & `pyschwab-0.0.1a4/pyschwab/user_input.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a3/pyschwab/utils.py` & `pyschwab-0.0.1a4/pyschwab/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 def dataclass_to_dict(instance):
     """
     Convert a dataclass instance to a dictionary with camelCase keys.
     Handles nested dataclass instances as well.
     """
     if instance is None:
         return instance
+    if isinstance(instance, Enum):
+        return instance.value
     if isinstance(instance, list):
         return [dataclass_to_dict(item) for item in instance]
     if not hasattr(instance, '__dataclass_fields__'):
         return instance
 
     result = {}
     for field_name in instance.__dataclass_fields__.keys():
@@ -163,14 +165,42 @@
 
 def format_list(lst: str | List) -> str:
     if lst is None or isinstance(lst, str):
         return lst
 
     return ",".join(lst)
 
+def remove_none_values(data: Dict[str, Any]) -> Dict[str, Any]:
+    """
+    Recursively remove all keys with None values from the dictionary.
+
+    Args:
+    data (dict): The dictionary to clean.
+
+    Returns:
+    dict: The cleaned dictionary with no None values.
+    """
+    if not isinstance(data, dict):
+        return data
+
+    clean_dict = {}
+    for key, value in data.items():
+        if isinstance(value, dict):
+            nested_clean_dict = remove_none_values(value)
+            if nested_clean_dict:  # only add non-empty nested dictionaries
+                clean_dict[key] = nested_clean_dict
+        elif isinstance(value, list):
+            clean_list = [remove_none_values(item) for item in value]
+            if clean_list:  # only add non-empty lists
+                clean_dict[key] = clean_list
+        elif value is not None:
+            clean_dict[key] = value
+
+    return clean_dict
+
 
 def to_json_str(obj):
     def json_encode(obj):
         """Custom JSON serializer for objects not serializable by default json code."""
         if isinstance(obj, datetime) or isinstance(obj, date):
             return obj.isoformat()
```

### Comparing `pyschwab-0.0.1a3/PKG-INFO` & `pyschwab-0.0.1a4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyschwab
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A Python library for the Schwab trading API
 Home-page: https://github.com/hzheng/pyschwab
 License: MIT
 Keywords: finance,trading,schwab,api,python
 Author: Hui Zheng
 Author-email: xyz.dll@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -75,34 +75,29 @@
 access_token = authorizer.get_access_token()
 print(access_token)
 
 # Example usage of trading APIs
 trading_api = TradingApi(access_token, app_config['trading'])
 
 account_num = 0 # CHANGE this to your actual account number
-trading_data = trading_api.fetch_trading_data(account_num)
+trading_api.set_current_account_number(account_num)
+trading_data = trading_api.fetch_trading_data()
 # List positions
 for position in trading_data.positions:
     print("position:", position)
 
 # List transactions 
-for transaction in trading_api.get_transactions(account_num):
+for transaction in trading_api.get_transactions():
     print("transaction:", transaction)
 
 # Place order
-order_dict = {
-    "orderType": "LIMIT", "session": "NORMAL", "duration": "DAY", "orderStrategyType": "SINGLE", "price": '100.00',
-    "orderLegCollection": [
-        {"instruction": "BUY", "quantity": 1, "instrument": {"symbol": "TSLA", "assetType": "EQUITY"}}
-    ]
-    }
-trading_api.place_order(order_dict, account_num)
+trading_api.buy_equity("TSLA", quantity=1, price=100)
 
 # List orders
-for order in trading_api.get_orders(account_num):
+for order in trading_api.get_orders():
     print("order:", order)
 
 # Example usage of market APIs
 market_api = MarketApi(access_token, app_config['market'])
 
 # Get quotes
 symbols = ['TSLA', 'NVDA']
```

