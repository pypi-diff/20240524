# Comparing `tmp/lumibot-3.4.2.tar.gz` & `tmp/lumibot-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumibot-3.4.2.tar", last modified: Thu May 23 06:19:04 2024, max compression
+gzip compressed data, was "lumibot-3.4.3.tar", last modified: Fri May 24 17:43:57 2024, max compression
```

## Comparing `lumibot-3.4.2.tar` & `lumibot-3.4.3.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.752124 lumibot-3.4.2/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.4.2/LICENSE
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-23 06:19:04.752058 lumibot-3.4.2/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.4.2/README.md
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.721798 lumibot-3.4.2/lumibot/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.725275 lumibot-3.4.2/lumibot/backtesting/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/backtesting/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/backtesting/alpaca_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/backtesting/alpha_vantage_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    31699 2024-05-10 17:14:24.000000 lumibot-3.4.2/lumibot/backtesting/backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/backtesting/ccxt_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/backtesting/pandas_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    14652 2024-05-23 04:53:36.000000 lumibot-3.4.2/lumibot/backtesting/polygon_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/backtesting/yahoo_backtesting.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.727911 lumibot-3.4.2/lumibot/brokers/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/brokers/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/brokers/alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    44089 2024-05-23 04:53:24.000000 lumibot-3.4.2/lumibot/brokers/broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-04-16 22:57:26.000000 lumibot-3.4.2/lumibot/brokers/ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/brokers/interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    27085 2024-05-08 03:43:54.000000 lumibot-3.4.2/lumibot/brokers/tradier.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.732237 lumibot-3.4.2/lumibot/data_sources/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/data_sources/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/data_sources/alpaca_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/data_sources/alpha_vantage_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/data_sources/ccxt_backtesting_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/data_sources/ccxt_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    19315 2024-05-23 04:53:24.000000 lumibot-3.4.2/lumibot/data_sources/data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.4.2/lumibot/data_sources/data_source_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/data_sources/exceptions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/data_sources/interactive_brokers_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15521 2024-05-10 17:41:22.000000 lumibot-3.4.2/lumibot/data_sources/pandas_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11734 2024-05-23 04:53:24.000000 lumibot-3.4.2/lumibot/data_sources/tradier_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7022 2024-04-10 20:12:46.000000 lumibot-3.4.2/lumibot/data_sources/yahoo_data.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.735486 lumibot-3.4.2/lumibot/entities/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/entities/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9605 2024-05-10 17:15:05.000000 lumibot-3.4.2/lumibot/entities/asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/entities/bar.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/entities/bars.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21849 2024-05-08 03:43:54.000000 lumibot-3.4.2/lumibot/entities/data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/entities/dataline.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    28373 2024-05-08 05:17:06.000000 lumibot-3.4.2/lumibot/entities/order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/entities/position.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/entities/trading_fee.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.738184 lumibot-3.4.2/lumibot/example_strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/example_strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/example_strategies/ccxt_backtesting_example.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-04-16 22:57:26.000000 lumibot-3.4.2/lumibot/example_strategies/crypto_important_functions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2613 2024-04-10 20:12:46.000000 lumibot-3.4.2/lumibot/example_strategies/options_hold_to_expiry.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/example_strategies/simple_start_single_file.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/example_strategies/stock_bracket.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/example_strategies/stock_buy_and_hold.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/example_strategies/stock_diversified_leverage.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/example_strategies/stock_limit_and_trailing_stops.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/example_strategies/stock_momentum.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/example_strategies/stock_oco.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/example_strategies/strangle.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.740546 lumibot-3.4.2/lumibot/strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    53746 2024-05-23 04:53:36.000000 lumibot-3.4.2/lumibot/strategies/_strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)   153357 2024-05-23 06:14:17.000000 lumibot-3.4.2/lumibot/strategies/strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    39943 2024-05-08 03:43:54.000000 lumibot-3.4.2/lumibot/strategies/strategy_executor.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.744968 lumibot-3.4.2/lumibot/tools/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/tools/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/tools/black_scholes.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.4.2/lumibot/tools/ccxt_data_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/tools/debugers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/tools/decorators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/tools/helpers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    26283 2024-05-08 03:43:54.000000 lumibot-3.4.2/lumibot/tools/indicators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/tools/lumibot_time.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/tools/pandas.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21338 2024-05-23 04:53:36.000000 lumibot-3.4.2/lumibot/tools/polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/tools/types.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15762 2024-05-08 03:43:54.000000 lumibot-3.4.2/lumibot/tools/yahoo_helper.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.745516 lumibot-3.4.2/lumibot/traders/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/traders/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7997 2024-05-10 16:59:36.000000 lumibot-3.4.2/lumibot/traders/trader.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.746180 lumibot-3.4.2/lumibot/trading_builtins/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/trading_builtins/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/trading_builtins/custom_stream.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.4.2/lumibot/trading_builtins/safe_list.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.751750 lumibot-3.4.2/lumibot.egg-info/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-23 06:19:04.000000 lumibot-3.4.2/lumibot.egg-info/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3260 2024-05-23 06:19:04.000000 lumibot-3.4.2/lumibot.egg-info/SOURCES.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-05-23 06:19:04.000000 lumibot-3.4.2/lumibot.egg-info/dependency_links.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-05-23 06:19:04.000000 lumibot-3.4.2/lumibot.egg-info/requires.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-05-23 06:19:04.000000 lumibot-3.4.2/lumibot.egg-info/top_level.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.4.2/pyproject.toml
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-05-23 06:19:04.752416 lumibot-3.4.2/setup.cfg
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1809 2024-05-23 06:16:26.000000 lumibot-3.4.2/setup.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.749464 lumibot-3.4.2/tests/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.4.2/tests/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-23 06:19:04.751481 lumibot-3.4.2/tests/backtest/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.4.2/tests/backtest/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      553 2024-05-08 03:43:54.000000 lumibot-3.4.2/tests/backtest/fixtures.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11668 2024-05-23 04:53:36.000000 lumibot-3.4.2/tests/backtest/test_example_strategies.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.4.2/tests/backtest/test_main_pandas_daily.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    17827 2024-05-23 04:53:36.000000 lumibot-3.4.2/tests/backtest/test_polygon.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.4.2/tests/backtest/test_strategy_executor.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1928 2024-05-08 03:43:54.000000 lumibot-3.4.2/tests/backtest/test_yahoo.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.4.2/tests/test_alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.4.2/tests/test_alpaca_old.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.4.2/tests/test_asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.4.2/tests/test_backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.4.2/tests/test_ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.4.2/tests/test_ccxt_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1571 2024-05-23 04:53:24.000000 lumibot-3.4.2/tests/test_data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.4.2/tests/test_interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4177 2024-04-10 20:12:46.000000 lumibot-3.4.2/tests/test_order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21487 2024-05-23 04:53:36.000000 lumibot-3.4.2/tests/test_polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.4.2/tests/test_strategy_methods.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21225 2024-05-23 04:53:24.000000 lumibot-3.4.2/tests/test_tradier.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.4.2/tests/test_tradingfee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.423857 lumibot-3.4.3/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.4.3/LICENSE
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-24 17:43:57.423782 lumibot-3.4.3/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.4.3/README.md
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.397703 lumibot-3.4.3/lumibot/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.400475 lumibot-3.4.3/lumibot/backtesting/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/backtesting/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/backtesting/alpaca_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/backtesting/alpha_vantage_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    31699 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/backtesting/backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/backtesting/ccxt_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/backtesting/pandas_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    14652 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/backtesting/polygon_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/backtesting/yahoo_backtesting.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.402704 lumibot-3.4.3/lumibot/brokers/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/brokers/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/brokers/alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    44490 2024-05-24 16:33:35.000000 lumibot-3.4.3/lumibot/brokers/broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-04-16 22:57:26.000000 lumibot-3.4.3/lumibot/brokers/ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/brokers/interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    29851 2024-05-24 16:33:35.000000 lumibot-3.4.3/lumibot/brokers/tradier.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.406234 lumibot-3.4.3/lumibot/data_sources/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/alpaca_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/alpha_vantage_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/ccxt_backtesting_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/ccxt_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    19315 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/data_sources/data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.4.3/lumibot/data_sources/data_source_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/exceptions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/interactive_brokers_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15521 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/data_sources/pandas_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11734 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/data_sources/tradier_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7022 2024-04-10 20:12:46.000000 lumibot-3.4.3/lumibot/data_sources/yahoo_data.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.408550 lumibot-3.4.3/lumibot/entities/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/entities/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9605 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/entities/asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/entities/bar.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/entities/bars.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21849 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/entities/data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/entities/dataline.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    28502 2024-05-24 16:33:35.000000 lumibot-3.4.3/lumibot/entities/order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/entities/position.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/entities/trading_fee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.411294 lumibot-3.4.3/lumibot/example_strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/ccxt_backtesting_example.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-04-16 22:57:26.000000 lumibot-3.4.3/lumibot/example_strategies/crypto_important_functions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2613 2024-04-10 20:12:46.000000 lumibot-3.4.3/lumibot/example_strategies/options_hold_to_expiry.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/simple_start_single_file.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/stock_bracket.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/stock_buy_and_hold.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/stock_diversified_leverage.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/stock_limit_and_trailing_stops.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/stock_momentum.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/stock_oco.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/strangle.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.413462 lumibot-3.4.3/lumibot/strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    53746 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/strategies/_strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)   153357 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/strategies/strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    39943 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/strategies/strategy_executor.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.417320 lumibot-3.4.3/lumibot/tools/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/black_scholes.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.4.3/lumibot/tools/ccxt_data_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/debugers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/decorators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/helpers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    26283 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/tools/indicators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/lumibot_time.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/pandas.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21338 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/tools/polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/types.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15762 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/tools/yahoo_helper.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.417749 lumibot-3.4.3/lumibot/traders/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/traders/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7997 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/traders/trader.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.418426 lumibot-3.4.3/lumibot/trading_builtins/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/trading_builtins/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/trading_builtins/custom_stream.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/trading_builtins/safe_list.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.423444 lumibot-3.4.3/lumibot.egg-info/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-24 17:43:57.000000 lumibot-3.4.3/lumibot.egg-info/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3260 2024-05-24 17:43:57.000000 lumibot-3.4.3/lumibot.egg-info/SOURCES.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-05-24 17:43:57.000000 lumibot-3.4.3/lumibot.egg-info/dependency_links.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-05-24 17:43:57.000000 lumibot-3.4.3/lumibot.egg-info/requires.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-05-24 17:43:57.000000 lumibot-3.4.3/lumibot.egg-info/top_level.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.4.3/pyproject.toml
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-05-24 17:43:57.424163 lumibot-3.4.3/setup.cfg
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1809 2024-05-24 16:33:35.000000 lumibot-3.4.3/setup.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.421351 lumibot-3.4.3/tests/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.423129 lumibot-3.4.3/tests/backtest/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/backtest/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      553 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/backtest/fixtures.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11668 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/backtest/test_example_strategies.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/backtest/test_main_pandas_daily.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    17827 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/backtest/test_polygon.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/backtest/test_strategy_executor.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1928 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/backtest/test_yahoo.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_alpaca_old.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_ccxt_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1571 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/test_data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4177 2024-04-10 20:12:46.000000 lumibot-3.4.3/tests/test_order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21487 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/test_polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_strategy_methods.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21225 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/test_tradier.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_tradingfee.py
```

### Comparing `lumibot-3.4.2/LICENSE` & `lumibot-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/PKG-INFO` & `lumibot-3.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.4.2
+Version: 3.4.3
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lumibot-3.4.2/README.md` & `lumibot-3.4.3/README.md`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/__init__.py` & `lumibot-3.4.3/lumibot/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/backtesting/backtesting_broker.py` & `lumibot-3.4.3/lumibot/backtesting/backtesting_broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/backtesting/polygon_backtesting.py` & `lumibot-3.4.3/lumibot/backtesting/polygon_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/brokers/alpaca.py` & `lumibot-3.4.3/lumibot/brokers/alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/brokers/broker.py` & `lumibot-3.4.3/lumibot/brokers/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -838,15 +838,22 @@
 
     def _parse_broker_orders(self, broker_orders, strategy_name, strategy_object=None):
         """parse a list of broker orders into a
         list of order objects"""
         result = []
         if broker_orders is not None:
             for broker_order in broker_orders:
-                result.append(self._parse_broker_order(broker_order, strategy_name, strategy_object=strategy_object))
+                # Check if it is a multileg order
+                if "leg" in broker_order and isinstance(broker_order["leg"], list):
+                    for leg in broker_order["leg"]:
+                        order = self._parse_broker_order(leg, strategy_name, strategy_object=strategy_object)
+                        result.append(order)
+                else:
+                    order = self._parse_broker_order(broker_order, strategy_name, strategy_object=strategy_object)
+                    result.append(order)
         else:
             self.logger.warning("No orders found in broker._parse_broker_orders: the broker_orders object is None")
 
         return result
 
     def _pull_order(self, identifier, strategy_name):
         """pull and parse a broker order by id"""
```

### Comparing `lumibot-3.4.2/lumibot/brokers/ccxt.py` & `lumibot-3.4.3/lumibot/brokers/ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/brokers/interactive_brokers.py` & `lumibot-3.4.3/lumibot/brokers/interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/brokers/tradier.py` & `lumibot-3.4.3/lumibot/brokers/tradier.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,25 +103,27 @@
 
         if not order.identifier:
             raise ValueError("Order identifier is not set, unable to cancel order. Did you remember to submit it?")
 
         # Cancel the order
         self.tradier.orders.cancel(order.identifier)
 
-    def submit_orders(self, orders, is_multileg=False, order_type="market", duration="day", price=None, tag=None):
+    def submit_orders(self, orders, is_multileg=False, order_type="market", duration="day", price=None):
         """
         Submit multiple orders to the broker. This function will submit the orders in the order they are provided.
         If any order fails to submit, the function will stop submitting orders and return the last successful order.
         """
         # Check if the orders are empty
-        if not orders:
+        if not orders or len(orders) == 0:
             return
         
         # Check if it is a multi-leg order
         if is_multileg:
+            tag = orders[0].tag if orders[0].tag else orders[0].strategy
+
             # Submit the multi-leg order
             return self._submit_multileg_order(orders, order_type, duration, price, tag)
 
         # Submit each order
         for order in orders:
             self.submit_order(order)
 
@@ -322,14 +324,55 @@
         # Loop through each position and check if it matches the asset
         for position in all_positions:
             if position.asset == asset:
                 # We found the position, return it
                 return position
 
         return None
+    
+    def _parse_broker_order_dict(self, response: dict, strategy_name: str, strategy_object=None):
+        """
+        Parse a broker order representation to a Lumi order object or objects. Once the Lumi order has been created,
+        it will be dispatched to our "stream" queue for processing until a time when Live Streaming can be implemented.
+
+        Parameters
+        ----------
+        response: dict
+            The output from TradierAPI call returned by pull_broker_order()
+        strategy_name: str
+            The name of the strategy that placed the order
+        strategy_object: Strategy
+            The strategy object that placed the order
+
+        Returns
+        -------
+        list[Order]
+            The Lumibot order objects created from the response
+        """
+
+        # Check if the order is a multileg order
+        if "leg" in response and isinstance(response["leg"], list):
+            # Create the orders list
+            orders = []
+
+            # Loop through each leg in the response
+            for leg in response["leg"]:
+                # Create the order object
+                order = self._parse_broker_order(leg, strategy_name, strategy_object)
+
+                # TODO: Get the average fill price and quantity
+
+                # Add the order to the list
+                orders.append(order)
+
+            return orders
+        
+        # Create the order object
+        order = self._parse_broker_order(response, strategy_name, strategy_object)
+        return [order]
 
     def _parse_broker_order(self, response: dict, strategy_name: str, strategy_object=None):
         """
         Parse a broker order representation to a Lumi order object. Once the Lumi order has been created, it will
         be dispatched to our "stream" queue for processing until a time when Live Streaming can be implemented.
 
         Tradier API Documentation:
@@ -362,14 +405,15 @@
             quantity=response["quantity"],
             type=response["type"],
             time_in_force=response["duration"],
             limit_price=response["price"] if "price" in response and response["price"] else None,
             stop_price=response["stop_price"] if "stop_price" in response and response["stop_price"] else None,
             tag=response["tag"] if "tag" in response and response["tag"] else None,
             date_created=response["create_date"],
+            avg_fill_price=response["avg_fill_price"] if "avg_fill_price" in response else None,
         )
         order.status = response["status"]
         order.avg_fill_price = response.get("avg_fill_price", order.avg_fill_price)
         order.update_raw(response)  # This marks order as 'transmitted'
         return order
 
     def _pull_broker_order(self, identifier):
@@ -464,88 +508,111 @@
         # Get current orders from Tradier and dispatch them to the stream for processing. Need to see all
         # lumi orders (not just active "tracked" ones) to catch any orders that might have changed final
         # status in Tradier.
         # df_orders = self.tradier.orders.get_orders()
         raw_orders = self._pull_broker_all_orders()
         stored_orders = {x.identifier: x for x in self.get_all_orders()}
         for order_row in raw_orders:
-            order = self._parse_broker_order(order_row, strategy_name=order_row.get("tag"))
+            orders = self._parse_broker_order_dict(order_row, strategy_name=order_row.get("tag"))
 
-            # First time seeing this order, something weird has happened, dispatch it as a new order
-            if order.identifier not in stored_orders:
-                # If it is the brokers first iteration then fully process the order because it is likely
-                # that the order was filled/canceled/etc before the strategy started.
-                if self._first_iteration:
-                    if order.status == Order.OrderStatus.FILLED:
-                        self._process_new_order(order)
-                        self._process_filled_order(order, order.avg_fill_price, order.quantity)
-                    elif order.status == Order.OrderStatus.CANCELED:
-                        self._process_new_order(order)
-                        self._process_canceled_order(order)
-                    elif order.status == Order.OrderStatus.PARTIALLY_FILLED:
-                        self._process_new_order(order)
-                        self._process_partially_filled_order(order, order.avg_fill_price, order.quantity)
-                    elif order.status == Order.OrderStatus.NEW:
+            for order in orders:
+                # First time seeing this order, something weird has happened
+                if order.identifier not in stored_orders:
+                    # If it is the brokers first iteration then fully process the order because it is likely
+                    # that the order was filled/canceled/etc before the strategy started.
+                    if self._first_iteration:
+                        if order.status == Order.OrderStatus.FILLED:
+                            self._process_new_order(order)
+                            self._process_filled_order(order, order.avg_fill_price, order.quantity)
+                        elif order.status == Order.OrderStatus.CANCELED:
+                            self._process_new_order(order)
+                            self._process_canceled_order(order)
+                        elif order.status == Order.OrderStatus.PARTIALLY_FILLED:
+                            self._process_new_order(order)
+                            self._process_partially_filled_order(order, order.avg_fill_price, order.quantity)
+                        elif order.status == Order.OrderStatus.NEW:
+                            self._process_new_order(order)
+                    else:
+                        # Add to order in lumibot.
                         self._process_new_order(order)
                 else:
-                    # Add to order in lumibot.
-                    self._process_new_order(order)
-            else:
-                stored_order = stored_orders[order.identifier]
-                stored_order.quantity = order.quantity  # Update the quantity in case it has changed
+                    stored_order = stored_orders[order.identifier]
+                    stored_order.quantity = order.quantity  # Update the quantity in case it has changed
 
-                # Status has changed since last time we saw it, dispatch the new status.
-                #  - Polling methods are unable to track partial fills
-                #     - Partial fills often happen quickly and it is highly likely that polling will miss some of them
-                #     - Additionally, Lumi Order objects don't have a way to track quantity status changes and
-                #        adjusting the average sell price can be tricky
-                #     - Only dispatch filled orders if they are completely filled.
-                if not order.equivalent_status(stored_order):
-                    match order.status.lower():
-                        case "submitted" | "open":
-                            self.stream.dispatch(self.NEW_ORDER, order=stored_order)
-                        case "partial_filled":
-                            # Not handled for polling, only dispatch completely filled orders
-                            pass
-                        case "fill":
-                            fill_price = order_row["avg_fill_price"]
-                            fill_qty = order_row["exec_quantity"] if "exec_quantity" in order_row else order.quantity
-                            self.stream.dispatch(
-                                self.FILLED_ORDER, order=stored_order, price=fill_price, filled_quantity=fill_qty
-                            )
-                        case "canceled":
-                            self.stream.dispatch(self.CANCELED_ORDER, order=stored_order)
-                        case "error":
-                            default_msg = f"{self.name} encountered an error with order {order.identifier} | {order}"
-                            msg = order_row["reason_description"] if "reason_description" in order_row else default_msg
-                            self.stream.dispatch(self.ERROR_ORDER, order=stored_order, error_msg=msg)
-                        case "cash_settled":
-                            # Don't know how to detect this case in Tradier.
-                            # Reference: https://documentation.tradier.com/brokerage-api/reference/response/orders
-                            # Theory:
-                            #  - Tradier will auto settle and create a new fill order for cash settled orders. Needs
-                            #    testing to confirm.
-                            pass
-                else:
-                    # Status hasn't changed, but make sure we use the broker's status.
-                    # I.e. 'submitted' becomes 'open'
-                    stored_order.status = order.status
+                    # Status has changed since last time we saw it, dispatch the new status.
+                    #  - Polling methods are unable to track partial fills
+                    #     - Partial fills often happen quickly and it is highly likely that polling will miss some of them
+                    #     - Additionally, Lumi Order objects don't have a way to track quantity status changes and
+                    #        adjusting the average sell price can be tricky
+                    #     - Only dispatch filled orders if they are completely filled.
+                    if not order.equivalent_status(stored_order):
+                        match order.status.lower():
+                            case "submitted" | "open":
+                                self.stream.dispatch(self.NEW_ORDER, order=stored_order)
+                            case "partial_filled":
+                                # Not handled for polling, only dispatch completely filled orders
+                                pass
+                            case "fill":
+                                # Check if the order has an avg_fill_price, if not use the order_row price
+                                if order.avg_fill_price is None:
+                                    fill_price = order_row["avg_fill_price"] 
+                                else:
+                                    fill_price = order.avg_fill_price
+
+                                # Check if the order has a quantity, if not 
+                                if order.quantity is None:
+                                    fill_qty = order_row["exec_quantity"]
+                                else:
+                                    fill_qty = order.quantity
+
+                                self.stream.dispatch(
+                                    self.FILLED_ORDER, order=stored_order, price=fill_price, filled_quantity=fill_qty
+                                )
+                            case "canceled":
+                                self.stream.dispatch(self.CANCELED_ORDER, order=stored_order)
+                            case "error":
+                                default_msg = f"{self.name} encountered an error with order {order.identifier} | {order}"
+                                msg = order_row["reason_description"] if "reason_description" in order_row else default_msg
+                                self.stream.dispatch(self.ERROR_ORDER, order=stored_order, error_msg=msg)
+                            case "cash_settled":
+                                # Don't know how to detect this case in Tradier.
+                                # Reference: https://documentation.tradier.com/brokerage-api/reference/response/orders
+                                # Theory:
+                                #  - Tradier will auto settle and create a new fill order for cash settled orders. Needs
+                                #    testing to confirm.
+                                pass
+                    else:
+                        # Status hasn't changed, but make sure we use the broker's status.
+                        # I.e. 'submitted' becomes 'open'
+                        stored_order.status = order.status
 
         # See if there are any tracked (aka active) orders that are no longer in the broker's list,
         # dispatch them as cancelled
         tracked_orders = {x.identifier: x for x in self.get_tracked_orders()}
-        broker_ids = [o["id"] for o in raw_orders]
+        broker_ids = self._get_broker_id_from_raw_orders(raw_orders)
         for order_id, order in tracked_orders.items():
             if order_id not in broker_ids:
                 logging.info(
                     f"Poll Update: {self.name} no longer has order {order}, but Lumibot does. " 
                     f"Dispatching as cancelled."
                 )
                 self.stream.dispatch(self.CANCELED_ORDER, order=order)
 
+    def _get_broker_id_from_raw_orders(self, raw_orders):
+        ids = []
+        for o in raw_orders:
+            if "id" in o:
+                ids.append(o["id"])
+            if "leg" in o:
+                for leg in o["leg"]:
+                    if "id" in leg:
+                        ids.append(leg["id"])
+
+        return ids
+
     def _get_stream_object(self):
         """get the broker stream connection"""
         stream = PollingStream(self.polling_interval)
         return stream
 
     def _register_stream_events(self):
         """Register the function on_trade_event
```

### Comparing `lumibot-3.4.2/lumibot/data_sources/alpaca_data.py` & `lumibot-3.4.3/lumibot/data_sources/alpaca_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/data_sources/alpha_vantage_data.py` & `lumibot-3.4.3/lumibot/data_sources/alpha_vantage_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/data_sources/ccxt_backtesting_data.py` & `lumibot-3.4.3/lumibot/data_sources/ccxt_backtesting_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/data_sources/ccxt_data.py` & `lumibot-3.4.3/lumibot/data_sources/ccxt_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/data_sources/data_source.py` & `lumibot-3.4.3/lumibot/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/data_sources/data_source_backtesting.py` & `lumibot-3.4.3/lumibot/data_sources/data_source_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/data_sources/exceptions.py` & `lumibot-3.4.3/lumibot/data_sources/exceptions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/data_sources/interactive_brokers_data.py` & `lumibot-3.4.3/lumibot/data_sources/interactive_brokers_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/data_sources/pandas_data.py` & `lumibot-3.4.3/lumibot/data_sources/pandas_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/data_sources/tradier_data.py` & `lumibot-3.4.3/lumibot/data_sources/tradier_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/data_sources/yahoo_data.py` & `lumibot-3.4.3/lumibot/data_sources/yahoo_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/entities/asset.py` & `lumibot-3.4.3/lumibot/entities/asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/entities/bar.py` & `lumibot-3.4.3/lumibot/entities/bar.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/entities/bars.py` & `lumibot-3.4.3/lumibot/entities/bars.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/entities/data.py` & `lumibot-3.4.3/lumibot/entities/data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/entities/order.py` & `lumibot-3.4.3/lumibot/entities/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         quote=None,
         pair=None,
         date_created=None,
         type=None,
         trade_cost: float = None,
         custom_params={},
         identifier=None,
+        avg_fill_price=None,
         tag="",
     ):
         """Order class for managing individual orders.
 
         Order class for creating order objects that will track details
         of each order through the lifecycle of the order from creation
         through cancel, fill or closed for other reasons.
@@ -181,14 +182,16 @@
         type : str
             The type of order. Possible values are: `market`, `limit`, `stop`, `stop_limit`, `trail`, `trail_limit`, `bracket`, `bracket_limit`, `bracket_stop`, `bracket_stop_limit`.
         trade_cost : float
             The cost of this order in the quote currency.
         custom_params : dict
             A dictionary of custom parameters that can be used to pass additional information to the broker. This is useful for passing custom parameters to the broker that are not supported by Lumibot.
             Eg. `custom_params={"leverage": 3}` for Kraken margin trading.
+        avg_fill_price: float
+            The average price that the order was fileld at.
         tag: str
             A tag that can be used to identify the order. This is useful for tracking orders in the broker. Not all
             brokers support this feature and lumibot will simply ignore it for those that don't.
         Examples
         --------
         >>> from lumibot.entities import Asset
         >>> from lumibot.entities import Order
@@ -278,15 +281,15 @@
         self.dependent_order = None
         self.dependent_order_filled = False
         self.type = type
         self.trade_cost = trade_cost
         self.custom_params = custom_params
         self._trail_stop_price = None
         self.tag = tag
-        self.avg_fill_price = 0.0  # The weighted average filled price for this order. Calculated if not given by broker
+        self.avg_fill_price = avg_fill_price # The weighted average filled price for this order. Calculated if not given by broker
         self.broker_create_date = None  # The datetime the order was created by the broker
         self.broker_update_date = None  # The datetime the order was last updated by the broker
 
         # Options:
         self.exchange = exchange
 
         # Cryptocurrency market.
```

### Comparing `lumibot-3.4.2/lumibot/entities/position.py` & `lumibot-3.4.3/lumibot/entities/position.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/entities/trading_fee.py` & `lumibot-3.4.3/lumibot/entities/trading_fee.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/example_strategies/ccxt_backtesting_example.py` & `lumibot-3.4.3/lumibot/example_strategies/ccxt_backtesting_example.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/example_strategies/crypto_important_functions.py` & `lumibot-3.4.3/lumibot/example_strategies/crypto_important_functions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/example_strategies/options_hold_to_expiry.py` & `lumibot-3.4.3/lumibot/example_strategies/options_hold_to_expiry.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/example_strategies/simple_start_single_file.py` & `lumibot-3.4.3/lumibot/example_strategies/simple_start_single_file.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/example_strategies/stock_bracket.py` & `lumibot-3.4.3/lumibot/example_strategies/stock_bracket.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/example_strategies/stock_buy_and_hold.py` & `lumibot-3.4.3/lumibot/example_strategies/stock_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/example_strategies/stock_diversified_leverage.py` & `lumibot-3.4.3/lumibot/example_strategies/stock_diversified_leverage.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/example_strategies/stock_limit_and_trailing_stops.py` & `lumibot-3.4.3/lumibot/example_strategies/stock_limit_and_trailing_stops.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/example_strategies/stock_momentum.py` & `lumibot-3.4.3/lumibot/example_strategies/stock_momentum.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/example_strategies/stock_oco.py` & `lumibot-3.4.3/lumibot/example_strategies/stock_oco.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/example_strategies/strangle.py` & `lumibot-3.4.3/lumibot/example_strategies/strangle.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/strategies/_strategy.py` & `lumibot-3.4.3/lumibot/strategies/_strategy.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/strategies/strategy.py` & `lumibot-3.4.3/lumibot/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/strategies/strategy_executor.py` & `lumibot-3.4.3/lumibot/strategies/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/tools/__init__.py` & `lumibot-3.4.3/lumibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/tools/black_scholes.py` & `lumibot-3.4.3/lumibot/tools/black_scholes.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/tools/ccxt_data_store.py` & `lumibot-3.4.3/lumibot/tools/ccxt_data_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/tools/decorators.py` & `lumibot-3.4.3/lumibot/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/tools/helpers.py` & `lumibot-3.4.3/lumibot/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/tools/indicators.py` & `lumibot-3.4.3/lumibot/tools/indicators.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/tools/lumibot_time.py` & `lumibot-3.4.3/lumibot/tools/lumibot_time.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/tools/pandas.py` & `lumibot-3.4.3/lumibot/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/tools/polygon_helper.py` & `lumibot-3.4.3/lumibot/tools/polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/tools/types.py` & `lumibot-3.4.3/lumibot/tools/types.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/tools/yahoo_helper.py` & `lumibot-3.4.3/lumibot/tools/yahoo_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/traders/trader.py` & `lumibot-3.4.3/lumibot/traders/trader.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/trading_builtins/custom_stream.py` & `lumibot-3.4.3/lumibot/trading_builtins/custom_stream.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot/trading_builtins/safe_list.py` & `lumibot-3.4.3/lumibot/trading_builtins/safe_list.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot.egg-info/PKG-INFO` & `lumibot-3.4.3/lumibot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.4.2
+Version: 3.4.3
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lumibot-3.4.2/lumibot.egg-info/SOURCES.txt` & `lumibot-3.4.3/lumibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/lumibot.egg-info/requires.txt` & `lumibot-3.4.3/lumibot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/pyproject.toml` & `lumibot-3.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/setup.cfg` & `lumibot-3.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/setup.py` & `lumibot-3.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lumibot",
-    version="3.4.2",
+    version="3.4.3",
     author="Robert Grzesik",
     author_email="rob@lumiwealth.com",
     description="Backtesting and Trading Library, Made by Lumiwealth",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Lumiwealth/lumibot",
     packages=setuptools.find_packages(),
```

### Comparing `lumibot-3.4.2/tests/backtest/fixtures.py` & `lumibot-3.4.3/tests/backtest/fixtures.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/backtest/test_example_strategies.py` & `lumibot-3.4.3/tests/backtest/test_example_strategies.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/backtest/test_main_pandas_daily.py` & `lumibot-3.4.3/tests/backtest/test_main_pandas_daily.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/backtest/test_polygon.py` & `lumibot-3.4.3/tests/backtest/test_polygon.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/backtest/test_strategy_executor.py` & `lumibot-3.4.3/tests/backtest/test_strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/backtest/test_yahoo.py` & `lumibot-3.4.3/tests/backtest/test_yahoo.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/test_alpaca.py` & `lumibot-3.4.3/tests/test_alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/test_alpaca_old.py` & `lumibot-3.4.3/tests/test_alpaca_old.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/test_asset.py` & `lumibot-3.4.3/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/test_backtesting_broker.py` & `lumibot-3.4.3/tests/test_backtesting_broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/test_ccxt.py` & `lumibot-3.4.3/tests/test_ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/test_ccxt_store.py` & `lumibot-3.4.3/tests/test_ccxt_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/test_data_source.py` & `lumibot-3.4.3/tests/test_data_source.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/test_interactive_brokers.py` & `lumibot-3.4.3/tests/test_interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/test_order.py` & `lumibot-3.4.3/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/test_polygon_helper.py` & `lumibot-3.4.3/tests/test_polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/test_strategy_methods.py` & `lumibot-3.4.3/tests/test_strategy_methods.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.2/tests/test_tradier.py` & `lumibot-3.4.3/tests/test_tradier.py`

 * *Files identical despite different names*

