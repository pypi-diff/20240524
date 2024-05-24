# Comparing `tmp/tinyticker-0.6.4.tar.gz` & `tmp/tinyticker-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.6.4.tar", max compression
+gzip compressed data, was "tinyticker-0.6.5.tar", max compression
```

## Comparing `tinyticker-0.6.4.tar` & `tinyticker-0.6.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1068 2024-05-22 22:44:39.118936 tinyticker-0.6.4/LICENSE
--rw-r--r--   0        0        0     3787 2024-05-22 22:44:39.118936 tinyticker-0.6.4/README.md
--rw-r--r--   0        0        0      917 2024-05-22 22:44:39.118936 tinyticker-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      465 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/__init__.py
--rw-r--r--   0        0        0     6582 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/__main__.py
--rw-r--r--   0        0        0     2496 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/config.py
--rw-r--r--   0        0        0     9000 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/paths.py
--rw-r--r--   0        0        0     4653 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/sequence.py
--rw-r--r--   0        0        0     1112 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/tickers/__init__.py
--rw-r--r--   0        0        0     3618 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/tickers/_base.py
--rw-r--r--   0        0        0     4620 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/tickers/crypto.py
--rw-r--r--   0        0        0     2915 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/tickers/stock.py
--rw-r--r--   0        0        0     2391 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0    21091 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in7.py
--rw-r--r--   0        0        0    19697 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in7_V2.py
--rw-r--r--   0        0        0     1551 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2583 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6750 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/web/app.py
--rw-r--r--   0        0        0     3393 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    15682 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     1904 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     2349 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 tinyticker-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-23 18:27:45.641275 tinyticker-0.6.5/LICENSE
+-rw-r--r--   0        0        0     3986 2024-05-23 18:27:45.641275 tinyticker-0.6.5/README.md
+-rw-r--r--   0        0        0      917 2024-05-23 18:27:45.641275 tinyticker-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      465 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/__init__.py
+-rw-r--r--   0        0        0     5967 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/__main__.py
+-rw-r--r--   0        0        0     2496 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/config.py
+-rw-r--r--   0        0        0     9000 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/paths.py
+-rw-r--r--   0        0        0     5483 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/sequence.py
+-rw-r--r--   0        0        0     1112 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/tickers/__init__.py
+-rw-r--r--   0        0        0     3618 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/tickers/_base.py
+-rw-r--r--   0        0        0     4620 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/tickers/crypto.py
+-rw-r--r--   0        0        0     2915 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/tickers/stock.py
+-rw-r--r--   0        0        0     2391 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0    21091 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in7.py
+-rw-r--r--   0        0        0    19697 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in7_V2.py
+-rw-r--r--   0        0        0     1551 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2583 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6750 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/web/app.py
+-rw-r--r--   0        0        0     3656 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/web/command.py
+-rw-r--r--   0        0        0   274777 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    15682 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     1904 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     2349 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 tinyticker-0.6.5/PKG-INFO
```

### Comparing `tinyticker-0.6.4/LICENSE` & `tinyticker-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/README.md` & `tinyticker-0.6.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
   <img  src="https://i.imgur.com/J4k3PCM.png" height=400>
   <img src="https://i.imgur.com/QWP7bpH.png" height=400>
 </div>
 <p align="center">
   <a href="https://pypi.org/project/tinyticker/"><img src="https://img.shields.io/pypi/v/tinyticker"></a>
   <a href="./LICENSE.md"><img src="https://img.shields.io/badge/license-MIT-blue.svg"></a>
   <a href="https://github.com/loiccoyle/tinyticker/actions/workflows/ci.yml"><img src="https://github.com/loiccoyle/tinyticker/actions/workflows/ci.yml/badge.svg"></a>
+  <a href="https://discord.com/channels/1239232827237597184/1239232827841839297"><img alt="Discord" src="https://img.shields.io/discord/1239232827237597184?logo=discord&logoSize=auto&label=%20"></a>
 </p>
 <hr/>
 
 `tinyticker` uses a Raspberry Pi zero W and a small ePaper display to periodically display a stock or crypto chart.
 
 A `flask` web interface is created to set the ticker options and control the Raspberry Pi.
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
                       ************ ?ð??? ttiinnyyttiicckkeerr ?ð??? ************
       [https://i.imgur.com/J4k3PCM.png][https://i.imgur.com/QWP7bpH.png]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_t_i_n_y_t_i_c_k_e_r_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
     _l_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_o_i_c_c_o_y_l_e_/_t_i_n_y_t_i_c_k_e_r_/_a_c_t_i_o_n_s_/
-                          _w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_]
+                     _w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_D_i_s_c_o_r_d_]
 ===============================================================================
 `tinyticker` uses a Raspberry Pi zero W and a small ePaper display to
 periodically display a stock or crypto chart. A `flask` web interface is
 created to set the ticker options and control the Raspberry Pi. `tinyticker`
 uses the [`cryptocompare`](https://github.com/lagerfeuer/cryptocompare) API to
 query the crypto price information, you'll need to get yourself a free [API
 key](https://min-api.cryptocompare.com/pricing). As well as the [`yfinance`]
```

### Comparing `tinyticker-0.6.4/pyproject.toml` & `tinyticker-0.6.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.6.4"
+version = "0.6.5"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.6.4/tinyticker/__main__.py` & `tinyticker-0.6.5/tinyticker/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import argparse
+import asyncio
 import atexit
-import multiprocessing
 import os
 import signal
 import sys
 from pathlib import Path
-from time import sleep
 from typing import List
 
 from watchdog.events import FileModifiedEvent, FileSystemEventHandler
 from watchdog.observers import Observer
 
 from . import __version__, logger
 from .config import load_config_safe
@@ -49,28 +48,14 @@
         help="Show the version and exit.",
         action="version",
         version="%(prog)s {version}".format(version=__version__),
     )
     return parser.parse_args(args)
 
 
-def start_ticker_process(config_file: Path) -> multiprocessing.Process:
-    """Create and start the ticker process.
-
-    Args:
-        config_file: config file path.
-
-    Returns:
-        The ticker process.
-    """
-    tick_process = multiprocessing.Process(target=start_ticker, args=(config_file,))
-    tick_process.start()
-    return tick_process
-
-
 def show_ticker(ticker: TickerBase, resp: TickerResponse, display: Display):
     delta_range_start = resp.historical.iloc[0]["Open"]
     delta_range = 100 * (resp.current_price - delta_range_start) / delta_range_start
 
     top_string = f"{ticker.config.symbol}: $ {resp.current_price:.2f}"
     if ticker.config.avg_buy_price is not None:
         # calculate the delta from the average buy price
@@ -95,52 +80,58 @@
         xlim=xlim,
         type=ticker.config.plot_type,
         mav=ticker.config.mav,
         volume=ticker.config.volume,
     )
 
 
-def start_ticker(config_file: Path) -> None:
+async def start_ticker(config_file: Path) -> None:
     """Start ticking.
 
     Args:
         config_file: config file path.
     """
     logger.info("Starting ticker process")
 
-    def skip_current(*_):
-        logger.info("Skip current ticker.")
-        if sequence is not None:
-            sequence._skip_current = True
+    def next_ticker(*_):
+        logger.info("Next ticker.")
+        if sequence is not None and sequence.current_index is not None:
+            sequence.go_to_index((sequence.current_index + 1) % len(sequence.tickers))
+
+    def prev_ticker(*_):
+        logger.info("Previous ticker.")
+        if sequence is not None and sequence.current_index is not None:
+            sequence.go_to_index((sequence.current_index - 1) % len(sequence.tickers))
 
-    signal.signal(signal.SIGUSR1, skip_current)
+    signal.signal(signal.SIGUSR1, next_ticker)
+    signal.signal(signal.SIGUSR2, prev_ticker)
 
     # Read config values
     tt_config = load_config_safe(config_file)
 
     display = Display.from_tinyticker_config(tt_config)
     sequence = Sequence.from_tinyticker_config(tt_config)
     logger.debug(sequence)
 
     try:
-        for ticker, resp in sequence.start():
-            logger.debug("API len(historical): %s", len(resp.historical))
-            logger.debug("API current_price: %s", resp.current_price)
+        async for ticker, resp in sequence.start():
+            logger.debug("Ticker response len(historical): %s", len(resp.historical))
+            logger.debug("Ticker response current_price: %s", resp.current_price)
             show_ticker(ticker, resp, display)
     except Exception as exc:
         logger.error(exc, stack_info=True)
         display.text(
             f"Whoops something broke:\n{exc}",
             show=True,
             weight="bold",
             fontsize="small",
         )
 
 
-def main():
+async def run():
     args = parse_args(sys.argv[1:])
     config_file: Path = args.config
 
     if args.verbose > 0:
         set_verbosity(logger, args.verbose)
     logger.info("Tinyticker version: %s", __version__)
 
@@ -154,65 +145,51 @@
     logger.info("PID: %s", pid)
     if not PID_FILE.parent.is_dir():
         PID_FILE.parent.mkdir(parents=True, exist_ok=True)
     PID_FILE.write_text(str(pid))
 
     logger.debug("Args: %s", args)
 
-    def refresh(*_) -> None:
-        """Kill the ticker process, it gets restarted in the main thread."""
-        logger.info("Refreshing ticker process.")
-        if not tick_process._closed and tick_process.is_alive():  # type: ignore
-            tick_process.kill()
-            tick_process.join()
-            tick_process.close()
-
     class ConfigModifiedHandler(FileSystemEventHandler):
         def on_modified(self, event):
-            logger.info(f"{event.src_path} was changed, refreshing ticker thread.")
-            refresh()
+            logger.info(f"{event.src_path} was changed, cancelling ticker task.")
+            if tick_task and not tick_task.done():
+                tick_task.cancel()
 
     observer = Observer()
     config_modified_handler = ConfigModifiedHandler()
     observer.schedule(
         config_modified_handler, config_file, event_filter=[FileModifiedEvent]
     )
     observer.start()
 
-    signal.signal(signal.SIGUSR2, refresh)
-
     def cleanup():
         """Remove the PID file on exit."""
         logger.info("Exiting.")
         if PID_FILE.is_file():
             PID_FILE.unlink()
         observer.stop()
         observer.join()
-        tick_process.kill()
-        tick_process.join()
 
     atexit.register(cleanup)
 
-    def skip_ticker(*_):
-        """Skip the current ticker."""
-        logger.info("Sending signal to skip the current ticker.")
-        # forward the signal to the ticker process
-        if (
-            tick_process is not None
-            and tick_process.is_alive()
-            and tick_process.pid is not None
-        ):
-            os.kill(tick_process.pid, signal.SIGUSR1)
-
-    signal.signal(signal.SIGUSR1, skip_ticker)
-
     # start ticking, we pass the config file so that is can be reloaded on refresh
-    tick_process = start_ticker_process(config_file)
+    tick_task = None
     while True:
-        if tick_process._closed or not tick_process.is_alive():  # type: ignore
-            tick_process = start_ticker_process(config_file)
-        else:
-            sleep(1)
+        if not tick_task or tick_task.done():
+            try:
+                tick_task = asyncio.create_task(start_ticker(config_file))
+                await tick_task
+            except asyncio.CancelledError:
+                logger.info("Task cancelled.")
+
+
+def main():
+    try:
+        asyncio.run(run())
+    except KeyboardInterrupt:
+        logger.info("Exiting.")
+        sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tinyticker-0.6.4/tinyticker/config.py` & `tinyticker-0.6.5/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/display.py` & `tinyticker-0.6.5/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/sequence.py` & `tinyticker-0.6.5/tinyticker/sequence.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import asyncio
 import logging
 import time
-from typing import Iterator, List, Tuple
+from typing import AsyncGenerator, List, Optional, Tuple
 
 import pandas as pd
 
 from . import utils
 from .config import TinytickerConfig
-from .tickers._base import TickerBase, TickerResponse
 from .tickers import Ticker
+from .tickers._base import TickerBase, TickerResponse
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Sequence:
     @classmethod
     def from_tinyticker_config(cls, tt_config: TinytickerConfig) -> "Sequence":
@@ -52,32 +53,56 @@
                 ticker. This typically happens when the stock market closes.
         """
         if len(tickers) == 0:
             raise ValueError("No tickers provided.")
         self.tickers = tickers
         self.skip_empty = skip_empty
         self.skip_outdated = skip_outdated
-        self._skip_current = False
 
-    def start(self) -> Iterator[Tuple[TickerBase, TickerResponse]]:
+        self.current_index: Optional[int] = None
+        self._skip_ticker = False
+        self._got_to_index: Optional[int] = None
+
+    def go_to_index(self, index: int) -> None:
+        """Skip to a specific ticker.
+        Args:
+            index: index of the ticker to skip to.
+        """
+        if index < 0 or index >= len(self.tickers):
+            LOGGER.error(f"Invalid index {index}.")
+            return
+        self._skip_ticker = True
+        self._go_to_index = index
+
+    async def start(
+        self,
+    ) -> AsyncGenerator[Tuple[TickerBase, TickerResponse], None]:
         """Start iterating through the tickers.
 
         Returns:
             The `Ticker` instance and its response.
         """
         # if all tickers are skipped, we want to sleep for the smallest wait time
         all_skipped_cooldown = min(ticker.wait_time for ticker in self.tickers)
 
         all_skipped = False
         while True:
             if all_skipped:
                 LOGGER.info(f"All tickers skipped, sleeping {all_skipped_cooldown}s.")
                 time.sleep(all_skipped_cooldown)
             all_skipped = True
-            for ticker in self.tickers:
+            for i, ticker in enumerate(self.tickers):
+                if self._skip_ticker:
+                    if self._go_to_index == i % len(self.tickers):
+                        self._skip_ticker = False
+                    else:
+                        LOGGER.debug(f"Skipping {ticker}.")
+                        continue
+                self.current_index = i % len(self.tickers)
+
                 try:
                     response = ticker.single_tick()
                 except Exception as e:
                     LOGGER.error(f"{ticker} failed with {e}")
                     continue
                 if self.skip_empty and (
                     response.historical is None or response.historical.empty
@@ -100,20 +125,19 @@
                         LOGGER.debug(f"{ticker} response outdated, skipping.")
                         continue
                 all_skipped = False
                 yield (ticker, response)
 
                 LOGGER.info(f"Sleeping {ticker.wait_time}s.")
                 # we want to sleep for the ticker's wait time and check every second if we
-                # should skip the next ticker.
+                # should skip this ticker.
                 for _ in range(ticker.wait_time):
-                    if self._skip_current:
-                        LOGGER.info(f"Skipping {ticker}.")
-                        self._skip_current = False
+                    if self._skip_ticker:
+                        LOGGER.info(f"Stop waiting, skipping {ticker}.")
                         break
-                    time.sleep(1)
+                    await asyncio.sleep(1)
 
     def __str__(self):
         return (
             f"Sequence(skip_outdated={self.skip_outdated}, skip_empty={self.skip_empty}): \n"
             + "\n".join([ticker.__str__() for ticker in self.tickers])
         )
```

### Comparing `tinyticker-0.6.4/tinyticker/tickers/__init__.py` & `tinyticker-0.6.5/tinyticker/tickers/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/tickers/_base.py` & `tinyticker-0.6.5/tinyticker/tickers/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/tickers/crypto.py` & `tinyticker-0.6.5/tinyticker/tickers/crypto.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/tickers/stock.py` & `tinyticker-0.6.5/tinyticker/tickers/stock.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/utils.py` & `tinyticker-0.6.5/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.6.5/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/waveshare_lib/device.py` & `tinyticker-0.6.5/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in7.py` & `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in7.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in7_V2.py` & `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in7_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/waveshare_lib/models.py` & `tinyticker-0.6.5/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/web/__main__.py` & `tinyticker-0.6.5/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/web/app.py` & `tinyticker-0.6.5/tinyticker/web/app.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/web/command.py` & `tinyticker-0.6.5/tinyticker/web/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,38 +53,48 @@
     """Restart the tinyticker and tinyticker-web systemd services."""
     LOGGER.info("Restarting services.")
     try_command("systemctl --user restart tinyticker")
     try_command("systemctl --user restart tinyticker-web")
 
 
 @register
-def skip_current() -> None:
-    """Skip over the current ticker and display the next on."""
+def next_ticker() -> None:
+    """Skip the current ticker and display the next one."""
     if PID_FILE.is_file():
-        LOGGER.info("Sending SIGUSR2 to tinyticker.")
+        LOGGER.info("Sending SIGUSR1 to tinyticker.")
         with open(PID_FILE, "r") as pid_file:
             pid = int(pid_file.readline())
         os.kill(pid, signal.SIGUSR1)
     else:
         LOGGER.info("tinyticker is not runnning.")
 
 
 @register
-def refresh() -> None:
-    """Refresh tinyticker's ticker process."""
+def previous_ticker() -> None:
+    """Skip the current ticker and display the previous one."""
     if PID_FILE.is_file():
         LOGGER.info("Sending SIGUSR2 to tinyticker.")
         with open(PID_FILE, "r") as pid_file:
             pid = int(pid_file.readline())
         os.kill(pid, signal.SIGUSR2)
     else:
         LOGGER.info("tinyticker is not runnning.")
 
 
 @register
+def refresh() -> None:
+    """Refresh tinyticker's ticker process."""
+    if PID_FILE.is_file():
+        LOGGER.info("Touching config file.")
+        CONFIG_FILE.touch()
+    else:
+        LOGGER.info("tinyticker is not runnning.")
+
+
+@register
 def reboot() -> None:
     """Reboot the  RPi, requires sudo."""
     LOGGER.info("Rebooting.")
     try_command("sudo reboot")
 
 
 @register
```

### Comparing `tinyticker-0.6.4/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.6.5/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.6.5/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.6.5/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.6.5/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/web/templates/index.html` & `tinyticker-0.6.5/tinyticker/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/web/templates/js/index.js` & `tinyticker-0.6.5/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.6.5/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.6.5/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/tinyticker/web/templates/logfiles.html` & `tinyticker-0.6.5/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.4/PKG-INFO` & `tinyticker-0.6.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.6.4
+Version: 0.6.5
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
@@ -36,14 +36,15 @@
   <img  src="https://i.imgur.com/J4k3PCM.png" height=400>
   <img src="https://i.imgur.com/QWP7bpH.png" height=400>
 </div>
 <p align="center">
   <a href="https://pypi.org/project/tinyticker/"><img src="https://img.shields.io/pypi/v/tinyticker"></a>
   <a href="./LICENSE.md"><img src="https://img.shields.io/badge/license-MIT-blue.svg"></a>
   <a href="https://github.com/loiccoyle/tinyticker/actions/workflows/ci.yml"><img src="https://github.com/loiccoyle/tinyticker/actions/workflows/ci.yml/badge.svg"></a>
+  <a href="https://discord.com/channels/1239232827237597184/1239232827841839297"><img alt="Discord" src="https://img.shields.io/discord/1239232827237597184?logo=discord&logoSize=auto&label=%20"></a>
 </p>
 <hr/>
 
 `tinyticker` uses a Raspberry Pi zero W and a small ePaper display to periodically display a stock or crypto chart.
 
 A `flask` web interface is created to set the ticker options and control the Raspberry Pi.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.6.4 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.6.5 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -16,15 +16,15 @@
 (>=4.0.0,<5.0.0) Requires-Dist: yfinance (>=0.2.0,<0.3.0) Project-URL:
 Repository, https://github.com/loiccoyle/tinyticker Description-Content-Type:
 text/markdown
                       ************ ?ð??? ttiinnyyttiicckkeerr ?ð??? ************
       [https://i.imgur.com/J4k3PCM.png][https://i.imgur.com/QWP7bpH.png]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_t_i_n_y_t_i_c_k_e_r_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
     _l_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_o_i_c_c_o_y_l_e_/_t_i_n_y_t_i_c_k_e_r_/_a_c_t_i_o_n_s_/
-                          _w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_]
+                     _w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_D_i_s_c_o_r_d_]
 ===============================================================================
 `tinyticker` uses a Raspberry Pi zero W and a small ePaper display to
 periodically display a stock or crypto chart. A `flask` web interface is
 created to set the ticker options and control the Raspberry Pi. `tinyticker`
 uses the [`cryptocompare`](https://github.com/lagerfeuer/cryptocompare) API to
 query the crypto price information, you'll need to get yourself a free [API
 key](https://min-api.cryptocompare.com/pricing). As well as the [`yfinance`]
```

