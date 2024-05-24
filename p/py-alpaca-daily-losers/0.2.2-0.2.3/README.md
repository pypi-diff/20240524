# Comparing `tmp/py_alpaca_daily_losers-0.2.2.tar.gz` & `tmp/py_alpaca_daily_losers-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_daily_losers-0.2.2.tar", max compression
+gzip compressed data, was "py_alpaca_daily_losers-0.2.3.tar", max compression
```

## Comparing `py_alpaca_daily_losers-0.2.2.tar` & `py_alpaca_daily_losers-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1066 2024-05-19 01:55:07.733136 py_alpaca_daily_losers-0.2.2/LICENSE
--rw-r--r--   0        0        0    13887 2024-05-19 01:55:07.733136 py_alpaca_daily_losers-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-05-19 01:55:07.733136 py_alpaca_daily_losers-0.2.2/py_alpaca_daily_losers/__init__.py
--rw-r--r--   0        0        0    19580 2024-05-20 23:09:02.439340 py_alpaca_daily_losers-0.2.2/py_alpaca_daily_losers/daily_losers.py
--rw-r--r--   0        0        0        0 2024-05-19 01:55:07.733136 py_alpaca_daily_losers-0.2.2/py_alpaca_daily_losers/src/__init__.py
--rw-r--r--   0        0        0     1407 2024-05-19 19:01:05.570313 py_alpaca_daily_losers-0.2.2/py_alpaca_daily_losers/src/article_extractor.py
--rw-r--r--   0        0        0      481 2024-05-19 15:45:30.783151 py_alpaca_daily_losers-0.2.2/py_alpaca_daily_losers/src/global_fuctions.py
--rw-r--r--   0        0        0      936 2024-05-19 19:01:28.900310 py_alpaca_daily_losers-0.2.2/py_alpaca_daily_losers/src/marketaux.py
--rw-r--r--   0        0        0     2183 2024-05-19 15:58:13.033135 py_alpaca_daily_losers-0.2.2/py_alpaca_daily_losers/src/openai.py
--rw-r--r--   0        0        0     1941 2024-05-19 15:58:22.013134 py_alpaca_daily_losers-0.2.2/py_alpaca_daily_losers/src/slack.py
--rw-r--r--   0        0        0      692 2024-05-21 00:35:27.258586 py_alpaca_daily_losers-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    14549 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-19 01:55:07.733136 py_alpaca_daily_losers-0.2.3/LICENSE
+-rw-r--r--   0        0        0    13887 2024-05-19 01:55:07.733136 py_alpaca_daily_losers-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 01:55:07.733136 py_alpaca_daily_losers-0.2.3/py_alpaca_daily_losers/__init__.py
+-rw-r--r--   0        0        0    19822 2024-05-23 21:26:22.026759 py_alpaca_daily_losers-0.2.3/py_alpaca_daily_losers/daily_losers.py
+-rw-r--r--   0        0        0        0 2024-05-19 01:55:07.733136 py_alpaca_daily_losers-0.2.3/py_alpaca_daily_losers/src/__init__.py
+-rw-r--r--   0        0        0     1407 2024-05-19 19:01:05.570313 py_alpaca_daily_losers-0.2.3/py_alpaca_daily_losers/src/article_extractor.py
+-rw-r--r--   0        0        0      481 2024-05-19 15:45:30.783151 py_alpaca_daily_losers-0.2.3/py_alpaca_daily_losers/src/global_fuctions.py
+-rw-r--r--   0        0        0      936 2024-05-19 19:01:28.900310 py_alpaca_daily_losers-0.2.3/py_alpaca_daily_losers/src/marketaux.py
+-rw-r--r--   0        0        0     2183 2024-05-19 15:58:13.033135 py_alpaca_daily_losers-0.2.3/py_alpaca_daily_losers/src/openai.py
+-rw-r--r--   0        0        0     1941 2024-05-19 15:58:22.013134 py_alpaca_daily_losers-0.2.3/py_alpaca_daily_losers/src/slack.py
+-rw-r--r--   0        0        0      692 2024-05-23 21:26:51.936757 py_alpaca_daily_losers-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    14549 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-0.2.3/PKG-INFO
```

### Comparing `py_alpaca_daily_losers-0.2.2/LICENSE` & `py_alpaca_daily_losers-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.2/README.md` & `py_alpaca_daily_losers-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.2/py_alpaca_daily_losers/daily_losers.py` & `py_alpaca_daily_losers-0.2.3/py_alpaca_daily_losers/daily_losers.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,17 +69,15 @@
             # Try to sell the stock
             try:
                 # Get the quantity of the stock to sell
                 qty = current_positions[current_positions["symbol"] == symbol][
                     "qty"
                 ].values[0]
                 if self.alpaca.market.clock().is_open:
-                    self.alpaca.order.market(
-                        symbol=symbol, qty=qty, side="sell"
-                    )
+                    self.alpaca.position.close(symbol=symbol, percentage=100)
             # If there is an error, print or send a slack message
             except Exception as e:
                 send_message(f"Error selling {symbol}: {e}")
                 continue
             # If the order was successful, append the sold position to the sold_positions list
             else:
                 sold_positions.append({"symbol": symbol, "qty": qty})
@@ -128,18 +126,29 @@
                 axis=1
             )
         ) | (
             (
                 assets_history[["bbhi14", "bbhi30", "bbhi50", "bbhi200"]] == 1
             ).any(axis=1)
         )
+
         # Get the filtered positions based on the sell criteria
         sell_filtered_df = assets_history[sell_criteria]
+        sell_list = sell_filtered_df["symbol"].tolist()
+
+        percentage_change_list = current_positions[
+            current_positions["profit_pct"] > 0.1
+        ]["symbol"].tolist()
+
+        for symbol in percentage_change_list:
+            if symbol not in sell_list:
+                sell_list.append(symbol)
+
         # Get the symbol list from the filtered positions
-        return sell_filtered_df["symbol"].tolist()
+        return sell_list
 
     ########################################################
     # Define the liquidate_positions_for_capital function
     ########################################################
     def liquidate_positions_for_capital(self):
         """
         Liquidate the positions to make cash 10% of the portfolio
```

### Comparing `py_alpaca_daily_losers-0.2.2/py_alpaca_daily_losers/src/article_extractor.py` & `py_alpaca_daily_losers-0.2.3/py_alpaca_daily_losers/src/article_extractor.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.2/py_alpaca_daily_losers/src/marketaux.py` & `py_alpaca_daily_losers-0.2.3/py_alpaca_daily_losers/src/marketaux.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.2/py_alpaca_daily_losers/src/openai.py` & `py_alpaca_daily_losers-0.2.3/py_alpaca_daily_losers/src/openai.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.2/py_alpaca_daily_losers/src/slack.py` & `py_alpaca_daily_losers-0.2.3/py_alpaca_daily_losers/src/slack.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_daily_losers-0.2.2/pyproject.toml` & `py_alpaca_daily_losers-0.2.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-daily-losers"
-version = "0.2.2"
+version = "0.2.3"
 description = "Daily Losers strategy, uses py-alpaca-api for Alpaca Markets integration."
 authors = ["TexasCoding <jeff10278@me.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 python-dotenv = "^1.0.1"
```

### Comparing `py_alpaca_daily_losers-0.2.2/PKG-INFO` & `py_alpaca_daily_losers-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-daily-losers
-Version: 0.2.2
+Version: 0.2.3
 Summary: Daily Losers strategy, uses py-alpaca-api for Alpaca Markets integration.
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openai (>=1.30.1,<2.0.0)
```

