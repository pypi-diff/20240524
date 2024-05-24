# Comparing `tmp/asynctradier-0.0.1b9.tar.gz` & `tmp/asynctradier-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynctradier-0.0.1b9.tar", max compression
+gzip compressed data, was "asynctradier-1.0.0.tar", max compression
```

## Comparing `asynctradier-0.0.1b9.tar` & `asynctradier-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,32 @@
--rw-r--r--   0        0        0     1067 2024-01-13 15:29:07.774062 asynctradier-0.0.1b9/LICENSE
--rw-r--r--   0        0        0     2002 2024-01-13 15:29:07.774062 asynctradier-0.0.1b9/README.md
--rw-r--r--   0        0        0       29 2024-01-13 15:29:48.458988 asynctradier-0.0.1b9/asynctradier/__init__.py
--rw-r--r--   0        0        0     3161 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/common/__init__.py
--rw-r--r--   0        0        0      538 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/common/expiration.py
--rw-r--r--   0        0        0     2105 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/common/option_contract.py
--rw-r--r--   0        0        0     3851 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/common/order.py
--rw-r--r--   0        0        0      818 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/common/position.py
--rw-r--r--   0        0        0     6322 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/common/quote.py
--rw-r--r--   0        0        0     1940 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/exceptions/__init__.py
--rw-r--r--   0        0        0    21472 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/tradier.py
--rw-r--r--   0        0        0        0 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/utils/__init__.py
--rw-r--r--   0        0        0     1785 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/utils/common.py
--rw-r--r--   0        0        0     3871 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/utils/webutils.py
--rw-r--r--   0        0        0      868 2024-01-13 15:29:48.458988 asynctradier-0.0.1b9/pyproject.toml
--rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 asynctradier-0.0.1b9/setup.py
--rw-r--r--   0        0        0     2587 1970-01-01 00:00:00.000000 asynctradier-0.0.1b9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-24 08:38:43.534130 asynctradier-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2439 2024-05-24 08:38:43.534130 asynctradier-1.0.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-24 08:39:22.130245 asynctradier-1.0.0/asynctradier/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/clients/__init__.py
+-rw-r--r--   0        0        0    10868 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/clients/account_clients.py
+-rw-r--r--   0        0        0    16514 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/clients/marketdata_client.py
+-rw-r--r--   0        0        0     5004 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/clients/streaming_client.py
+-rw-r--r--   0        0        0    18022 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/clients/trading_client.py
+-rw-r--r--   0        0        0     4399 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/clients/watchlist_client.py
+-rw-r--r--   0        0        0     6157 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/__init__.py
+-rw-r--r--   0        0        0     9084 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/account_balance.py
+-rw-r--r--   0        0        0     1779 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/calendar.py
+-rw-r--r--   0        0        0      875 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/clock.py
+-rw-r--r--   0        0        0     2199 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/event.py
+-rw-r--r--   0        0        0      538 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/expiration.py
+-rw-r--r--   0        0        0     2289 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/gain_loss.py
+-rw-r--r--   0        0        0     9519 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/market_data.py
+-rw-r--r--   0        0        0     2104 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/option_contract.py
+-rw-r--r--   0        0        0     3852 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/order.py
+-rw-r--r--   0        0        0      818 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/position.py
+-rw-r--r--   0        0        0     6560 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/quote.py
+-rw-r--r--   0        0        0     1577 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/security.py
+-rw-r--r--   0        0        0     2200 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/user_profile.py
+-rw-r--r--   0        0        0     1049 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/common/watchlist.py
+-rw-r--r--   0        0        0     2520 2024-05-24 08:38:43.534130 asynctradier-1.0.0/asynctradier/exceptions/__init__.py
+-rw-r--r--   0        0        0     1163 2024-05-24 08:38:43.538130 asynctradier-1.0.0/asynctradier/tradier.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:38:43.538130 asynctradier-1.0.0/asynctradier/utils/__init__.py
+-rw-r--r--   0        0        0     2158 2024-05-24 08:38:43.538130 asynctradier-1.0.0/asynctradier/utils/common.py
+-rw-r--r--   0        0        0     3871 2024-05-24 08:38:43.538130 asynctradier-1.0.0/asynctradier/utils/webutils.py
+-rw-r--r--   0        0        0      885 2024-05-24 08:39:22.130245 asynctradier-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 asynctradier-1.0.0/setup.py
+-rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 asynctradier-1.0.0/PKG-INFO
```

### Comparing `asynctradier-0.0.1b9/LICENSE` & `asynctradier-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asynctradier-0.0.1b9/asynctradier/common/expiration.py` & `asynctradier-1.0.0/asynctradier/common/expiration.py`

 * *Files identical despite different names*

### Comparing `asynctradier-0.0.1b9/asynctradier/common/option_contract.py` & `asynctradier-1.0.0/asynctradier/common/option_contract.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 This module defines the OptionContract class, which represents an option contract in a trading system.
 """
 
-
 from asynctradier.common import OptionType, OrderSide
 from asynctradier.exceptions import InvalidExiprationDate, InvalidOptionType
 from asynctradier.utils.common import build_option_symbol, is_valid_expiration_date
 
 
 class OptionContract:
     """
```

### Comparing `asynctradier-0.0.1b9/asynctradier/common/order.py` & `asynctradier-1.0.0/asynctradier/common/order.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This module defines the Order class, which represents an order in a trading system.
 """
+
 from asynctradier.common import Duration, OrderClass, OrderSide, OrderStatus, OrderType
 
 
 class Order:
     """
     Represent an Order object.
```

### Comparing `asynctradier-0.0.1b9/asynctradier/common/position.py` & `asynctradier-1.0.0/asynctradier/common/position.py`

 * *Files identical despite different names*

### Comparing `asynctradier-0.0.1b9/asynctradier/common/quote.py` & `asynctradier-1.0.0/asynctradier/common/quote.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,16 @@
         expiration_date (str, optional): The expiration date for options.
         expiration_type (str, optional): The expiration type for options.
         option_type (OptionType, optional): The type of the option.
         root_symbols (str): Comma-delimited list of option root symbols for an underlier.
         root_symbol (str, optional): The root symbol for an underlier.
         greeks (Greeks, optional): The Greeks values for options.
         note (str, optional): The note for the quote.
+        date (str, optional): The date of the quote.
+        vwap (float, optional): The volume-weighted average price of the financial instrument.
     """
 
     def __init__(self, **kwargs):
         self.symbol = kwargs.get("symbol")
         self.description = kwargs.get("description")
         self.exch = kwargs.get("exch")
         self.type = QuoteType(kwargs.get("type")) if kwargs.get("type") else None
@@ -122,7 +124,9 @@
         )  # Comma-delimited list of option root symbols for an underlier
         self.root_symbol = kwargs.get(
             "root_symbol", None
         )  # Root symbol for an underlier
 
         self.greeks = Greeks(**kwargs.get("greeks")) if kwargs.get("greeks") else None
         self.note = kwargs.get("note", None)
+        self.date = kwargs.get("date", None)
+        self.vwap = kwargs.get("vwap", None)
```

### Comparing `asynctradier-0.0.1b9/asynctradier/exceptions/__init__.py` & `asynctradier-1.0.0/asynctradier/exceptions/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,7 +73,33 @@
     Attributes:
         code (int): The HTTP status code of the bad request.
         msg (str): The error message.
     """
 
     def __init__(self, code: int, msg: str) -> None:
         super().__init__(f"Request failed: {code}, msg: {msg}")
+
+
+class APINotAvailable(Exception):
+    """
+    Exception raised when the API is not available.
+
+    Attributes:
+        msg (str): The error message.
+    """
+
+    def __init__(self, msg: str) -> None:
+        super().__init__(f"API is not available. {msg}")
+
+
+class InvalidDateFormat(Exception):
+    """
+    Exception raised when the date format is not valid.
+
+    Attributes:
+        date (str): The invalid date.
+    """
+
+    def __init__(self, date: str) -> None:
+        super().__init__(
+            f"Date format {date} is not valid. Valid values is: YYYY-MM-DD"
+        )
```

### Comparing `asynctradier-0.0.1b9/asynctradier/tradier.py` & `asynctradier-1.0.0/asynctradier/clients/marketdata_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,450 +1,38 @@
-import json
-from typing import AsyncIterator, List, Optional
+from typing import List, Optional
 
-import websockets
-
-from asynctradier.common import Duration, OptionType, OrderClass, OrderSide, OrderType
+from asynctradier.common import OptionType
+from asynctradier.common.calendar import Calendar
+from asynctradier.common.clock import Clock
 from asynctradier.common.expiration import Expiration
-from asynctradier.common.option_contract import OptionContract
-from asynctradier.common.order import Order
-from asynctradier.common.position import Position
 from asynctradier.common.quote import Quote
-from asynctradier.exceptions import (
-    InvalidExiprationDate,
-    InvalidOptionType,
-    InvalidParameter,
-    InvalidStrikeType,
-    MissingRequiredParameter,
-)
-from asynctradier.utils.common import build_option_symbol, is_valid_expiration_date
-
-from .utils.webutils import WebUtil
+from asynctradier.common.security import Security
+from asynctradier.exceptions import InvalidExiprationDate, InvalidParameter
+from asynctradier.utils.common import is_valid_datetime, is_valid_expiration_date
+from asynctradier.utils.webutils import WebUtil
 
 
-class TradierClient:
+class MarketDataClient:
     """
-    A client for interacting with the Tradier API.
+    A client for accessing market data.
 
     Args:
-        account_id (str): The account ID.
-        token (str): The API token.
+        session (WebUtil): The session object used for making HTTP requests.
+        account_id (str): The account ID associated with the client.
+        token (str): The authentication token for accessing the market data.
         sandbox (bool, optional): Whether to use the sandbox environment. Defaults to False.
     """
 
-    def __init__(self, account_id: str, token: str, sandbox: bool = False) -> None:
+    def __init__(
+        self, session: WebUtil, account_id: str, token: str, sandbox: bool = False
+    ) -> None:
+        self.session = session
         self.account_id = account_id
         self.token = token
-        base_url = (
-            "https://api.tradier.com" if not sandbox else "https://sandbox.tradier.com"
-        )
-        self.session = WebUtil(base_url, token)
-
-    async def get_positions(self) -> List[Position]:
-        """
-        Get the positions for the account.
-
-        Returns:
-            List[Position]: A list of Position objects.
-        """
-        url = f"/v1/accounts/{self.account_id}/positions"
-        response = await self.session.get(url)
-        if response["positions"] == "null":
-            positions = []
-        else:
-            positions = response["positions"]["position"]
-        if not isinstance(positions, list):
-            positions = [positions]
-        results: List[Position] = []
-        for position in positions:
-            results.append(
-                Position(
-                    **position,
-                )
-            )
-        return results
-
-    async def get_order(self, order_id: str) -> Order:
-        """
-        Get an order by its ID.
-
-        Args:
-            order_id (str): The ID of the order.
-
-        Returns:
-            Order: The Order object.
-        """
-        url = f"/v1/accounts/{self.account_id}/orders/{order_id}"
-        params = {"includeTags": "true"}
-        response = await self.session.get(url, params=params)
-        order = response["order"]
-        return Order(
-            **order,
-        )
-
-    async def buy_option(
-        self,
-        symbol: str,
-        expiration_date: str,
-        strike: float | int,
-        option_type: OptionType,
-        quantity: int,
-        order_type: OrderType = OrderType.market,
-        order_duration: Duration = Duration.day,
-        tag: Optional[str] = None,
-        price: Optional[float] = None,
-        stop: Optional[float] = None,
-    ) -> Order:
-        """
-        Place a buy option order.
-
-        Args:
-            symbol (str): The symbol of the option.
-            expiration_date (str): The expiration date of the option (YYYY-MM-DD).
-            strike (float | int): The strike price of the option.
-            option_type (OptionType): The type of the option (call or put).
-            quantity (int): The quantity of the option contracts to buy.
-            order_type (OrderType, optional): The type of the order. Defaults to OrderType.market.
-            order_duration (Duration, optional): The duration of the order. Defaults to Duration.day.
-            tag (str, optional): An optional tag for the order. Defaults to None.
-            price (float, optional): The price at which to place the order. Required for limit orders. Defaults to None.
-            stop (float, optional): The stop price for the order. Required for stop orders. Defaults to None.
-
-        Returns:
-            Order: The Order object.
-        """
-        return await self._option_operation(
-            OrderSide.buy_to_open,
-            symbol,
-            expiration_date,
-            strike,
-            option_type,
-            quantity,
-            order_type,
-            order_duration,
-            tag,
-            price,
-            stop,
-        )
-
-    async def sell_option(
-        self,
-        symbol: str,
-        expiration_date: str,
-        strike: float | int,
-        option_type: OptionType,
-        quantity: int,
-        order_type: OrderType = OrderType.market,
-        order_duration: Duration = Duration.day,
-        tag: Optional[str] = None,
-        price: Optional[float] = None,
-        stop: Optional[float] = None,
-    ) -> Order:
-        """
-        Place a sell option order.
-
-        Args:
-            symbol (str): The symbol of the option.
-            expiration_date (str): The expiration date of the option (YYYY-MM-DD).
-            strike (float | int): The strike price of the option.
-            option_type (OptionType): The type of the option (call or put).
-            quantity (int): The quantity of the option contracts to sell.
-            order_type (OrderType, optional): The type of the order. Defaults to OrderType.market.
-            order_duration (Duration, optional): The duration of the order. Defaults to Duration.day.
-            tag (str, optional): An optional tag for the order. Defaults to None.
-            price (float, optional): The price at which to place the order. Required for limit orders. Defaults to None.
-            stop (float, optional): The stop price for the order. Required for stop orders. Defaults to None.
-
-        Returns:
-            Order: The Order object.
-        """
-        return await self._option_operation(
-            OrderSide.sell_to_close,
-            symbol,
-            expiration_date,
-            strike,
-            option_type,
-            quantity,
-            order_type,
-            order_duration,
-            tag,
-            price,
-            stop,
-        )
-
-    async def _option_operation(
-        self,
-        side: OrderSide,
-        symbol: str,
-        expiration_date: str,
-        strike: float | int,
-        option_type: OptionType,
-        quantity: int,
-        order_type: OrderType = OrderType.market,
-        order_duration: Duration = Duration.day,
-        tag: Optional[str] = None,
-        price: Optional[float] = None,
-        stop: Optional[float] = None,
-    ) -> Order:
-        """
-        Perform an option operation.
-
-        Args:
-            side (OrderSide): The side of the option order.
-            symbol (str): The symbol of the option.
-            expiration_date (str): The expiration date of the option (YYYY-MM-DD).
-            strike (float | int): The strike price of the option.
-            option_type (OptionType): The type of the option (call or put).
-            quantity (int): The quantity of the option contracts.
-            order_type (OrderType, optional): The type of the order. Defaults to OrderType.market.
-            order_duration (Duration, optional): The duration of the order. Defaults to Duration.day.
-            tag (str, optional): An optional tag for the order. Defaults to None.
-            price (float, optional): The price at which to place the order. Required for limit orders. Defaults to None.
-            stop (float, optional): The stop price for the order. Required for stop orders. Defaults to None.
-
-        Returns:
-            Order: The Order object.
-        """
-        if not is_valid_expiration_date(expiration_date):
-            raise InvalidExiprationDate(expiration_date)
-
-        if not isinstance(option_type, OptionType):
-            raise InvalidOptionType(option_type)
-
-        if not isinstance(strike, float) and not isinstance(strike, int):
-            raise InvalidStrikeType(strike)
-
-        if order_type == OrderType.limit and price is None:
-            raise MissingRequiredParameter("Price must be specified for limit orders")
-
-        if order_type == OrderType.stop and stop is None:
-            raise MissingRequiredParameter("Stop must be specified for stop orders")
-
-        url = f"/v1/accounts/{self.account_id}/orders"
-        params = {
-            "class": OrderClass.option.value,
-            "symbol": symbol,
-            "option_symbol": build_option_symbol(
-                symbol, expiration_date, strike, option_type.value
-            ),
-            "side": side.value,
-            "quantity": str(quantity),
-            "type": order_type.value,
-            "duration": order_duration.value,
-            "price": price if price is not None else "",
-            "stop": stop if stop is not None else "",
-            "tag": tag,
-        }
-        response = await self.session.post(url, data=params)
-        order = response["order"]
-        return Order(
-            **order,
-        )
-
-    async def cancel_order(self, order_id: str | int) -> Order:
-        """
-        Cancel an order by its ID.
-
-        Args:
-            order_id (str | int): The ID of the order.
-
-        Returns:
-            Order: The Order object.
-        """
-        url = f"/v1/accounts/{self.account_id}/orders/{order_id}"
-        response = await self.session.delete(url)
-        order = response["order"]
-        return Order(
-            **order,
-        )
-
-    async def get_orders(self, page: int = 1) -> List[Order]:
-        """
-        Get a list of orders for the account.
-
-        Parameters:
-            page (int, optional): The page number of the orders to retrieve. Defaults to 1.
-
-        Returns:
-            List[Order]: A list of Order objects.
-        """
-        res = []
-        page = 1
-        while True:
-            orders = await self._get_orders(page)
-            res += orders
-            page += 1
-            if len(orders) <= 0:
-                break
-        return res
-
-    async def _get_orders(self, page: int) -> List[Order]:
-        """
-        Get a list of orders for the account.
-
-        Args:
-            page (int): The page number of the orders to retrieve.
-
-        Returns:
-            List[Order]: A list of Order objects.
-        """
-        url = f"/v1/accounts/{self.account_id}/orders"
-        params = {
-            "page": page,
-            "includeTags": "true",
-        }
-        response = await self.session.get(url, params=params)
-        if response["orders"] == "null":
-            orders = []
-        else:
-            orders = response["orders"]["order"]
-
-        if not isinstance(orders, list):
-            orders = [orders]
-        results: List[Order] = []
-        for order in orders:
-            results.append(
-                Order(
-                    **order,
-                )
-            )
-        return results
-
-    async def modify_order(
-        self,
-        order_id: str | int,
-        order_type: Optional[OrderType] = None,
-        order_duration: Optional[Duration] = None,
-        price: Optional[float] = None,
-        stop: Optional[float] = None,
-    ) -> Order:
-        """
-        Modify an order by its ID.
-
-        Args:
-            order_id (str | int): The ID of the order.
-            order_type (OrderType, optional): The new type of the order. Defaults to None.
-            order_duration (Duration, optional): The new duration of the order. Defaults to None.
-            price (float, optional): The new price for the order. Defaults to None.
-            stop (float, optional): The new stop price for the order. Defaults to None.
-
-        Returns:
-            Order: The Order object.
-        """
-        url = f"/v1/accounts/{self.account_id}/orders/{order_id}"
-        param = {}
-        if order_type is not None:
-            param["type"] = order_type.value
-        if order_duration is not None:
-            param["duration"] = order_duration.value
-        if price is not None:
-            param["price"] = price
-        if stop is not None:
-            param["stop"] = stop
-
-        if len(param) == 0:
-            raise InvalidParameter("No parameters to modify")
-        response = await self.session.put(url, data=param)
-        order = response["order"]
-        return Order(
-            **order,
-        )
-
-    async def _get_streaming_account_session(self) -> str:
-        """
-        Get the streaming account session.
-
-        Returns:
-            str: The streaming account session.
-        """
-        url = "/v1/accounts/events/session"
-        response = await self.session.post(url)
-        return response
-
-    async def stream_order(self, with_detail: bool = True) -> AsyncIterator[Order]:
-        """
-        Stream order events.
-
-        Args:
-            with_detail (bool, optional): Whether to include order details. Defaults to True.
-        """
-        streaming_session = await self._get_streaming_account_session()
-        uri = streaming_session["stream"]["url"]
-        session_id = streaming_session["stream"]["sessionid"]
-
-        async with websockets.connect(uri) as websocket:
-            payload = {
-                "events": ["order"],
-                "sessionid": session_id,
-                "excludeAccounts": [],
-            }
-            payload = json.dumps(payload)
-
-            await websocket.send(payload)
-
-            while True:
-                response = json.loads(await websocket.recv())
-                if response["event"] == "heartbeat":
-                    continue
-                if response["event"] == "order":
-                    if with_detail:
-                        order_id = response["id"]
-                        yield await self.get_order(order_id)
-                    else:
-                        yield response
-
-    async def multileg(
-        self,
-        symbol: str,
-        order_type: OrderType,
-        duration: Duration,
-        legs: List[OptionContract],
-        price: Optional[float] = None,
-    ) -> Order:
-        """
-        Executes a multileg order.
-
-        Args:
-            symbol (str): The symbol of the order.
-            order_type (OrderType): The type of the order.
-            duration (Duration): The duration of the order.
-            legs (List[OptionContract]): The list of option contracts for the multileg order.
-            price (Optional[float]): The price of the order (required for spread orders).
-
-        Returns:
-            Order: The executed order.
-
-        Raises:
-            MissingRequiredParameter: If price is not specified for spread orders.
-        """
-
-        url = f"/v1/accounts/{self.account_id}/orders"
-        body = {}
-        if order_type == OrderType.debit or order_type == OrderType.credit:
-            if price is None:
-                raise MissingRequiredParameter(
-                    "Price must be specified for spread orders"
-                )
-            body["price"] = price
-
-        body["class"] = OrderClass.multileg.value
-        body["symbol"] = symbol
-        body["type"] = order_type.value
-        body["duration"] = duration.value
-
-        for i, leg in enumerate(legs):
-            body[f"option_symbol[{i}]"] = leg.option_symbol
-            body[f"quantity[{i}]"] = str(leg.quantity)
-            body[f"side[{i}]"] = leg.order_side.value
-
-        response = await self.session.post(url, data=body)
-        order = response["order"]
-        return Order(
-            **order,
-        )
+        self.sandbox = sandbox
 
     async def get_quotes(self, symbols: List[str], greeks: bool = False) -> List[Quote]:
         """
         Get quotes for a list of symbols.
 
         Args:
             symbols (List[str]): A list of symbols.
@@ -490,14 +78,15 @@
         """
         Get option chains for a symbol.
 
         Args:
             symbol (str): The symbol.
             expiration_date (str): The expiration date (YYYY-MM-DD).
             greeks (bool, optional): Whether to include greeks in the response. Defaults to False.
+            option_type (OptionType, optional): Filter by option type. Defaults to None.
         """
         if not is_valid_expiration_date(expiration_date):
             raise InvalidExiprationDate(expiration_date)
 
         url = "/v1/markets/options/chains"
         params = {
             "symbol": symbol,
@@ -623,7 +212,275 @@
         """
         url = "/v1/markets/options/lookup"
         params = {"underlying": symbol}
         response = await self.session.get(url, params=params)
         if response.get("symbols") is None:
             return []
         return response.get("symbols")[0].get("options", [])
+
+    async def get_calendar(self, year: str, month: str) -> List[Calendar]:
+        """
+        Retrieves the calendar for a specific year and month.
+
+        Args:
+            year (str): The year in the format YYYY.
+            month (str): The month in the format MM.
+
+        Returns:
+            List[Calendar]: A list of Calendar objects representing the calendar for the specified year and month.
+        """
+
+        if len(year) != 4:
+            raise InvalidParameter("year must be in the format YYYY")
+        if len(month) != 2:
+            raise InvalidParameter("month must be in the format MM")
+
+        if int(month) < 1 or int(month) > 12:
+            raise InvalidParameter("month must be between 1 and 12")
+
+        url = "/v1/markets/calendar"
+        params = {"year": year, "month": month}
+
+        response = await self.session.get(url, params=params)
+
+        if response.get("calendar") is None:
+            return []
+        details = response["calendar"]["days"]["day"]
+
+        results: List[Calendar] = []
+
+        for detail in details:
+            results.append(
+                Calendar(
+                    **detail,
+                )
+            )
+
+        return results
+
+    async def get_historical_quotes(
+        self, symbol: str, interval: str, start: str, end: str
+    ) -> List[Quote]:
+        """
+        Get historical quotes for a symbol.
+
+        Args:
+            symbol (str): The symbol.
+            interval (str): The interval for the historical quotes.
+            start (str): The start date (YYYY-MM-DD).
+            end (str): The end date (YYYY-MM-DD).
+        """
+        if interval not in ["daily", "weekly", "monthly"]:
+            raise InvalidParameter("interval must be one of daily, weekly, or monthly")
+
+        if not is_valid_expiration_date(start):
+            raise InvalidParameter(
+                f"start date {start} is not valid. Valid values is: YYYY-MM-DD"
+            )
+
+        if not is_valid_expiration_date(end):
+            raise InvalidParameter(
+                f"end date {end} is not valid. Valid values is: YYYY-MM-DD"
+            )
+        url = "/v1/markets/history"
+        params = {
+            "symbol": symbol,
+            "interval": interval,
+            "start": start,
+            "end": end,
+        }
+        response = await self.session.get(url, params=params)
+
+        results = []
+        quotes = response.get("history", {}).get("day", [])
+        if not isinstance(quotes, list):
+            quotes = [quotes]
+        for quote in quotes:
+            results.append(
+                Quote(
+                    **quote,
+                )
+            )
+        return results
+
+    async def get_time_and_sales(
+        self,
+        symbol: str,
+        interval: str = "tick",
+        start: Optional[str] = None,
+        end: Optional[str] = None,
+        session_filter: str = "all",
+    ) -> List[Quote]:
+        """
+        Retrieves time and sales data for a given symbol within a specified interval.
+
+        Args:
+            symbol (str): The symbol for which to retrieve time and sales data.
+            interval (str, optional): The interval of the time and sales data. Defaults to "tick".
+            start (str, optional): The start date and time for the data retrieval. Format: "YYYY-MM-DD HH:MM". Defaults to None.
+            end (str, optional): The end date and time for the data retrieval. Format: "YYYY-MM-DD HH:MM". Defaults to None.
+            session_filter (str, optional): The session filter for the data retrieval. Must be one of "all" or "open". Defaults to "all".
+
+        Returns:
+            List[Quote]: A list of Quote objects representing the time and sales data.
+
+        Raises:
+            InvalidParameter: If the provided interval, session_filter, start date, or end date is invalid.
+        """
+
+        if interval not in ["tick", "1min", "5min", "15min", "30min", "hour"]:
+            raise InvalidParameter(
+                "interval must be one of tick, 1min, 5min, 15min, 30min, or hour"
+            )
+
+        if session_filter not in ["all", "open"]:
+            raise InvalidParameter("session_filter must be one of all or open")
+
+        if start and not is_valid_datetime(start):
+            raise InvalidParameter(
+                f"start date {start} is not valid. Valid values is: YYYY-MM-DD HH:MM"
+            )
+
+        if end and not is_valid_datetime(end):
+            raise InvalidParameter(
+                f"end date {end} is not valid. Valid values is: YYYY-MM-DD HH:MM"
+            )
+
+        url = "/v1/markets/timesales"
+
+        params = {
+            "symbol": symbol,
+            "interval": interval,
+            "start": start,
+            "end": end,
+            "session_filter": session_filter,
+        }
+
+        response = await self.session.get(url, params=params)
+
+        results = []
+        quotes = response.get("series", {}).get("data", [])
+
+        if not isinstance(quotes, list):
+            quotes = [quotes]
+
+        for quote in quotes:
+            results.append(
+                Quote(
+                    **quote,
+                )
+            )
+
+        return results
+
+    async def get_etb_securities(self) -> List[Security]:
+        """
+        Retrieves a list of ETB (Exchange Traded Bond) securities.
+
+        Returns:
+            List[str]: A list of ETB securities.
+        """
+        url = "/v1/markets/etb"
+        response = await self.session.get(url)
+
+        if response.get("securities") is None:
+            return []
+
+        etbs = response.get("securities", {}).get("security", [])
+        results = []
+        if not isinstance(etbs, list):
+            etbs = [etbs]
+
+        for etb in etbs:
+            results.append(
+                Security(
+                    **etb,
+                )
+            )
+        return results
+
+    async def search_companies(
+        self, query: str, indexes: bool = False
+    ) -> List[Security]:
+        """
+        Search for companies based on the given query.
+
+        Args:
+            query (str): The search query.
+            indexes (bool, optional): Whether to include indexes in the search results. Defaults to False.
+
+        Returns:
+            List[Security]: A list of Security objects representing the search results.
+        """
+        url = "/v1/markets/search"
+        params = {"q": query, "indexes": str(indexes).lower()}
+        response = await self.session.get(url, params=params)
+        if response.get("securities") is None:
+            return []
+        results = []
+
+        securities = response.get("securities", {}).get("security", [])
+        if not isinstance(securities, list):
+            securities = [securities]
+
+        for security in securities:
+            results.append(
+                Security(
+                    **security,
+                )
+            )
+
+        return results
+
+    async def lookup_symbol(
+        self, query: str, exchanges: Optional[str] = None, types: Optional[str] = None
+    ) -> List[Security]:
+        """
+        Search for companies based on the given query.
+
+        Args:
+            query (str): The search query.
+            exchanges (str, optional): The exchanges to search. Must be one of "Q" or "N". Defaults to None.
+            types (str, optional): The types of securities to search. Must be one of "stock", "option", "etf", or "index". Defaults to None.
+        Returns:
+            List[Security]: A list of Security objects representing the search results.
+        """
+        if exchanges and exchanges not in ["Q", "N"]:
+            raise InvalidParameter("exchanges must be one of Q or N")
+        if types and types not in ["stock", "option", "etf", "index"]:
+            raise InvalidParameter("types must be one of stock, option, etf, index")
+        url = "/v1/markets/lookup"
+        params = {"q": query}
+        if exchanges:
+            params["exchanges"] = exchanges
+        if types:
+            params["types"] = types
+        response = await self.session.get(url, params=params)
+        if response.get("securities") is None:
+            return []
+        results = []
+
+        securities = response.get("securities", {}).get("security", [])
+        if not isinstance(securities, list):
+            securities = [securities]
+
+        for security in securities:
+            results.append(
+                Security(
+                    **security,
+                )
+            )
+
+        return results
+
+    async def get_clock(self, delay: bool = False) -> Clock:
+        """
+        Retrieves the current market clock.
+
+        Returns:
+            Clock: A Clock object representing the current market clock.
+        """
+        if delay and not self.sandbox:
+            raise InvalidParameter("delay is only available in the sandbox environment")
+        url = "/v1/markets/clock"
+        response = await self.session.get(url, params={"delay": str(delay).lower()})
+        return Clock(**response.get("clock", {}))
```

### Comparing `asynctradier-0.0.1b9/asynctradier/utils/webutils.py` & `asynctradier-1.0.0/asynctradier/utils/webutils.py`

 * *Files identical despite different names*

### Comparing `asynctradier-0.0.1b9/pyproject.toml` & `asynctradier-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 authors = ["Jiakuan Li <jiakuan.li.cs@gmail.com>"]
 description = "Async api wrapper for [Tradier](https://documentation.tradier.com/)."
 name = "asynctradier"
 packages = [{include = "asynctradier"}]
 readme = "README.md"
-version = "0.0.1-beta.9"
+version = "1.0.0"
 
 [tool.poetry.dependencies]
-aiohttp = "^3.9.1"
+aiohttp = "^3.9.5"
 python = "^3.9"
 strenum = "^0.4.15"
 websockets = "^12.0"
 
 [tool.poetry.group.dev.dependencies]
+aioresponses = "^0.7.6"
+m2r2 = "^0.3.3.post2"
 pre-commit = "^3.6.0"
 pytest = "^7.4.3"
 pytest-asyncio = "^0.23.2"
 pytest-cov = "^4.1.0"
 pytest-mock = "^3.12.0"
 sphinx = "^7.2.6"
-sphinx-rtd-theme = "^2.0.0"
 sphinx-autobuild = "^2021.3.14"
+sphinx-rtd-theme = "^2.0.0"
 sphinxcontrib-apidoc = "^0.4.0"
-m2r2 = "^0.3.3.post2"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
 vcs = "git"
 
 [build-system]
```

