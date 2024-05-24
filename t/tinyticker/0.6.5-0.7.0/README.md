# Comparing `tmp/tinyticker-0.6.5.tar.gz` & `tmp/tinyticker-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.6.5.tar", max compression
+gzip compressed data, was "tinyticker-0.7.0.tar", max compression
```

## Comparing `tinyticker-0.6.5.tar` & `tinyticker-0.7.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0     1068 2024-05-23 18:27:45.641275 tinyticker-0.6.5/LICENSE
--rw-r--r--   0        0        0     3986 2024-05-23 18:27:45.641275 tinyticker-0.6.5/README.md
--rw-r--r--   0        0        0      917 2024-05-23 18:27:45.641275 tinyticker-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      465 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/__init__.py
--rw-r--r--   0        0        0     5967 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/__main__.py
--rw-r--r--   0        0        0     2496 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/config.py
--rw-r--r--   0        0        0     9000 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/paths.py
--rw-r--r--   0        0        0     5483 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/sequence.py
--rw-r--r--   0        0        0     1112 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/tickers/__init__.py
--rw-r--r--   0        0        0     3618 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/tickers/_base.py
--rw-r--r--   0        0        0     4620 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/tickers/crypto.py
--rw-r--r--   0        0        0     2915 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/tickers/stock.py
--rw-r--r--   0        0        0     2391 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0    21091 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in7.py
--rw-r--r--   0        0        0    19697 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in7_V2.py
--rw-r--r--   0        0        0     1551 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2583 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6750 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/web/app.py
--rw-r--r--   0        0        0     3656 2024-05-23 18:27:45.645275 tinyticker-0.6.5/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    15682 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     1904 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     2349 2024-05-23 18:27:45.649275 tinyticker-0.6.5/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 tinyticker-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-24 00:37:02.507527 tinyticker-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3955 2024-05-24 00:37:02.507527 tinyticker-0.7.0/README.md
+-rw-r--r--   0        0        0      917 2024-05-24 00:37:02.507527 tinyticker-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      465 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/__init__.py
+-rw-r--r--   0        0        0     5967 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/__main__.py
+-rw-r--r--   0        0        0     2496 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/config.py
+-rw-r--r--   0        0        0     9000 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/paths.py
+-rw-r--r--   0        0        0     5483 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/sequence.py
+-rw-r--r--   0        0        0     1112 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/tickers/__init__.py
+-rw-r--r--   0        0        0     3618 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/tickers/_base.py
+-rw-r--r--   0        0        0     4620 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/tickers/crypto.py
+-rw-r--r--   0        0        0     2915 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/tickers/stock.py
+-rw-r--r--   0        0        0     2391 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0    21091 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in7.py
+-rw-r--r--   0        0        0    19697 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in7_V2.py
+-rw-r--r--   0        0        0     1551 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2895 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     8457 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/app.py
+-rw-r--r--   0        0        0     3656 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/command.py
+-rw-r--r--   0        0        0      506 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/startup.py
+-rw-r--r--   0        0        0   274777 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    14743 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     1904 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     2449 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     2970 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/startup.html
+-rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 tinyticker-0.7.0/PKG-INFO
```

### Comparing `tinyticker-0.6.5/LICENSE` & `tinyticker-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/README.md` & `tinyticker-0.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   <img  src="https://i.imgur.com/J4k3PCM.png" height=400>
   <img src="https://i.imgur.com/QWP7bpH.png" height=400>
 </div>
 <p align="center">
   <a href="https://pypi.org/project/tinyticker/"><img src="https://img.shields.io/pypi/v/tinyticker"></a>
   <a href="./LICENSE.md"><img src="https://img.shields.io/badge/license-MIT-blue.svg"></a>
   <a href="https://github.com/loiccoyle/tinyticker/actions/workflows/ci.yml"><img src="https://github.com/loiccoyle/tinyticker/actions/workflows/ci.yml/badge.svg"></a>
-  <a href="https://discord.com/channels/1239232827237597184/1239232827841839297"><img alt="Discord" src="https://img.shields.io/discord/1239232827237597184?logo=discord&logoSize=auto&label=%20"></a>
+  <a href="https://discord.com/channels/1239232827237597184/1239232827841839297"><img alt="Discord" src="https://img.shields.io/badge/%20discord-%20?logo=discord"></a>
 </p>
 <hr/>
 
 `tinyticker` uses a Raspberry Pi zero W and a small ePaper display to periodically display a stock or crypto chart.
 
 A `flask` web interface is created to set the ticker options and control the Raspberry Pi.
```

### Comparing `tinyticker-0.6.5/pyproject.toml` & `tinyticker-0.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.6.5"
+version = "0.7.0"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.6.5/tinyticker/__main__.py` & `tinyticker-0.7.0/tinyticker/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/config.py` & `tinyticker-0.7.0/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/display.py` & `tinyticker-0.7.0/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/sequence.py` & `tinyticker-0.7.0/tinyticker/sequence.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/tickers/__init__.py` & `tinyticker-0.7.0/tinyticker/tickers/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/tickers/_base.py` & `tinyticker-0.7.0/tinyticker/tickers/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/tickers/crypto.py` & `tinyticker-0.7.0/tinyticker/tickers/crypto.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/tickers/stock.py` & `tinyticker-0.7.0/tinyticker/tickers/stock.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/utils.py` & `tinyticker-0.7.0/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.7.0/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/waveshare_lib/device.py` & `tinyticker-0.7.0/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in7.py` & `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in7.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/waveshare_lib/epd2in7_V2.py` & `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in7_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/waveshare_lib/models.py` & `tinyticker-0.7.0/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/web/__main__.py` & `tinyticker-0.7.0/tinyticker/web/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ..utils import (
     RawTextArgumentDefaultsHelpFormatter,
     dashboard_qrcode,
     set_verbosity,
 )
 from . import logger
 from .app import create_app
+from .startup import STARTUP_DIR, run_scripts
 
 
 def parse_args(args: List[str]) -> argparse.Namespace:
     """Parse the command line arguments.
 
     Args:
         args: The command line arguments.
@@ -74,14 +75,19 @@
     if args.verbose > 0:
         set_verbosity(logger, args.verbose)
 
     logger.debug("Args: %s", args)
 
     if not args.log_dir.is_dir():
         args.log_dir.mkdir(parents=True)
+    if not STARTUP_DIR.is_dir():
+        STARTUP_DIR.mkdir(parents=True)
+
+    logger.info("Running startup scripts.")
+    processes = run_scripts()
 
     if args.show_qrcode:
         logger.info("Generating qrcode.")
         tt_config = TinytickerConfig.from_file(args.config)
         display = Display.from_tinyticker_config(tt_config)
         qrcode = dashboard_qrcode(
             display.epd.width,
@@ -90,15 +96,21 @@
         )
         logger.info("Displaying qrcode.")
         display.show_image(qrcode)
         del display
         sys.exit()
 
     logger.info("Starting tinyticker-web")
-    app = create_app(config_file=args.config, log_dir=args.log_dir)
-    serve(app, port=args.port)
-    # app.run(host="0.0.0.0", port=args.port, debug=False, threaded=True)
-    logger.info("Stopping tinyticker-web")
+    try:
+        app = create_app(config_file=args.config, log_dir=args.log_dir)
+        serve(app, port=args.port)
+    except Exception as e:
+        logger.error("Error: %s", e)
+        logger.exception(e)
+    finally:
+        for process in processes:
+            process.terminate()
+        logger.info("Stopping tinyticker-web")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tinyticker-0.6.5/tinyticker/web/command.py` & `tinyticker-0.7.0/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.7.0/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.7.0/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.7.0/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.7.0/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/web/templates/index.html` & `tinyticker-0.7.0/tinyticker/web/templates/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,23 @@
     <script src="js/uikit.min.js"></script>
     <script src="js/uikit-icons.min.js"></script>
     <script src="js/index.js"></script>
   </head>
   <body class="uk-background-muted uk-padding-small">
     <div class="uk-flex uk-flex-center uk-flex-middle">
       <div class="uk-width-large">
-        <div class="uk-width-1-1 uk-text-center">
-          <p class="uk-text-large">🚀 TinyTicker Dashboard 🚀</p>
+        <div class="uk-width-1-1 uk-text-center uk-margin">
+          <h3>🚀 TinyTicker Dashboard 🚀</h3>
+          <div class="uk-flex uk-flex-center">
+            <ul class="uk-subnav uk-subnav-divider uk-margin">
+              <li class="uk-active"><a href="#">Home</a></li>
+              <li><a href="/logfiles" target="_self">Log Files</a></li>
+              <li><a href="/startup" target="_self">Startup scripts</a></li>
+            </ul>
+          </div>
         </div>
         <div
           id="updateDiv"
           class="uk-background-default uk-alert uk-padding-small uk-margin-small"
           style="display: none"
         >
           <div class="uk-width-1-1 uk-text-center">
@@ -51,279 +58,279 @@
               uk-tooltip="Update the tinyticker package, will restart once complete."
             >
               Update & Restart
             </button>
           </form>
         </div>
         <div class="uk-width-large">
-          <p class="uk-text-large">Config</p>
           <form action="/set_hostname">
             <label class="uk-form-label" for="hostname">Hostname: </label>
             <input
               class="uk-input uk-width-1-3 uk-width-1-2@m"
               type="text"
               id="hostname"
               name="hostname"
               value="{{ hostname }}"
             />
             <input class="uk-button-small" type="submit" value="Set & Reboot" />
           </form>
           <hr />
-          <form class="uk-form-stacked" action="/config">
-            <div class="uk-grid uk-grid-small">
-              <div class="uk-width-1-1">
-                <label class="uk-form-label" for="epd_model"
-                  >ePaper display model</label
+          <form class="uk-form-stacked uk-width-1-1" action="/config">
+            <div class="uk-flex uk-flex-middle uk-margin-small-bottom">
+              <span
+                uk-icon="icon: tv; ratio: 2"
+                class="uk-padding-small uk-padding-remove-vertical"
+                style="width: 40px;"
+              ></span>
+              <select
+                class="uk-select uk-text-small"
+                id="epd_model"
+                name="epd_model"
+              >
+                {%- for epd_model_option in epd_model_options -%}
+                  {%- if epd_model_option.name == epd_model -%}
+                    <option value="{{ epd_model_option.name }}" selected>
+                      {{ epd_model_option.desc }}
+                    </option>
+                  {%- else -%}
+                    <option value="{{ epd_model_option.name }}">
+                      {{ epd_model_option.desc }}
+                    </option>
+                  {%- endif -%}
+                {%- endfor -%}
+              </select>
+              <label
+                class="uk-form-label uk-flex-none uk-margin-left"
+                for="flip"
+                ><input
+                  class="uk-checkbox uk-margin-small-right"
+                  type="checkbox"
+                  id="flip"
+                  name="flip"
+                  {% if flip | default(False) %}checked{% endif %}
+                />Flip display</label
+              >
+            </div>
+
+            <label class="uk-form-label" for="api_key"
+              ><a
+                uk-tooltip="CryptoCompare API key, use the free plan."
+                href="https://min-api.cryptocompare.com/pricing"
+                >API key</a
+              >
+            </label>
+            <div class="uk-inline uk-width-expand">
+              <a class="uk-form-icon" href="#" uk-icon="icon: lock"></a>
+              <input
+                class="uk-input uk-text-small"
+                type="text"
+                id="api_key"
+                name="api_key"
+                {% if api_key %}value="{{ api_key }}"{% endif %}
+              />
+            </div>
+
+            <div
+              uk-sortable="handle: .ticker-handle"
+              class="container uk-background-secondary uk-flex uk-flex-row uk-flex-middle uk-padding uk-margin uk-flex-left uk-flex-center@m"
+              style="overflow-x: auto; position: relative; box-sizing: border-box; width:100vw; left: calc(-50vw + 50%);"
+            >
+              {%- for ticker in tickers -%}
+                <div
+                  class="ticker uk-card uk-card-default uk-flex-none uk-margin-right uk-padding-small uk-border-rounded"
                 >
-                <div class="uk-flex uk-flex-middle">
-                  <span
-                    uk-icon="icon: tv; ratio: 2"
-                    class="uk-padding-small uk-padding-remove-vertical"
-                    style="width: 40px;"
-                  ></span>
+                  <div style="float: right">
+                    <button
+                      class="ticker-handle"
+                      type="button"
+                      uk-icon="icon: table"
+                    ></button>
+                    <button
+                      class="ticker-close"
+                      type="button"
+                      uk-close
+                      onclick="remove_ticker(this)"
+                    ></button>
+                  </div>
+
+                  <label class="uk-form-label" for="symbol_type"
+                    >Symbol type</label
+                  >
                   <select
-                    class="uk-select uk-text-small"
-                    id="epd_model"
-                    name="epd_model"
+                    class="uk-select"
+                    id="symbol_type"
+                    name="symbol_type"
+                    onchange="hide_prepost(this)"
                   >
-                    {%- for epd_model_option in epd_model_options -%}
-                      {%- if epd_model_option.name == epd_model -%}
-                        <option value="{{ epd_model_option.name }}" selected>
-                          {{ epd_model_option.desc }}
-                        </option>
-                      {%- else -%}
-                        <option value="{{ epd_model_option.name }}">
-                          {{ epd_model_option.desc }}
-                        </option>
-                      {%- endif -%}
+                    {%- for symbol_type_option in symbol_type_options -%}
+                      <option
+                        value="{{ symbol_type_option }}"
+                        {% if symbol_type_option == ticker.symbol_type %}selected{% endif %}
+                      >
+                        {{ symbol_type_option }}
+                      </option>
                     {%- endfor -%}
                   </select>
-                  <label
-                    class="uk-form-label uk-flex-none uk-margin-left"
-                    for="flip"
-                    ><input
-                      class="uk-checkbox uk-margin-small-right"
-                      type="checkbox"
-                      id="flip"
-                      name="flip"
-                      {% if flip | default(False) %}checked{% endif %}
-                    />Flip display</label
-                  >
-                </div>
-                <label class="uk-form-label" for="api_key"
-                  ><a href="https://min-api.cryptocompare.com/pricing"
-                    >CryptoCompare</a
-                  >
-                  API key</label
-                >
-                <div class="uk-inline uk-width-1-1">
-                  <a class="uk-form-icon" href="#" uk-icon="icon: lock"></a>
+
+                  <label class="uk-form-label" for="symbol">Symbol</label>
                   <input
-                    class="uk-input uk-text-small"
+                    class="uk-input"
                     type="text"
-                    id="api_key"
-                    name="api_key"
-                    {% if api_key %}value="{{ api_key }}"{% endif %}
+                    id="symbol"
+                    name="symbol"
+                    value="{{ ticker.symbol }}"
                   />
-                </div>
-                <h4>Tickers</h4>
-                <div
-                  uk-sortable="handle: .ticker-handle"
-                  class="container uk-background-secondary uk-flex uk-flex-row uk-flex-middle uk-padding uk-flex-left uk-flex-center@m"
-                  style="overflow-x: auto; position: relative; box-sizing: border-box; width:100vw; left: calc(-50vw + 50%);"
-                >
-                  {%- for ticker in tickers -%}
-                    <div
-                      class="ticker uk-card uk-card-default uk-flex-none uk-margin-right uk-padding-small uk-border-rounded"
-                    >
-                      <div style="float: right">
-                        <button
-                          class="ticker-handle"
-                          type="button"
-                          uk-icon="icon: table"
-                        ></button>
-                        <button
-                          class="ticker-close"
-                          type="button"
-                          uk-close
-                          onclick="remove_ticker(this)"
-                        ></button>
-                      </div>
-                      <label class="uk-form-label" for="symbol_type"
-                        >Symbol type</label
-                      >
-                      <select
-                        class="uk-select"
-                        id="symbol_type"
-                        name="symbol_type"
-                        onchange="hide_prepost(this)"
-                      >
-                        {%- for symbol_type_option in symbol_type_options -%}
-                          <option
-                            value="{{ symbol_type_option }}"
-                            {% if symbol_type_option == ticker.symbol_type %}selected{% endif %}
-                          >
-                            {{ symbol_type_option }}
-                          </option>
-                        {%- endfor -%}
-                      </select>
-                      <label class="uk-form-label" for="symbol">Symbol</label>
-                      <input
-                        class="uk-input"
-                        type="text"
-                        id="symbol"
-                        name="symbol"
-                        value="{{ ticker.symbol }}"
-                      />
-                      <label class="uk-form-label" for="interval"
-                        >Interval</label
-                      >
-                      <select class="uk-select" id="interval" name="interval">
-                        {%- for interval_option in interval_options -%}
-                          <option
-                            value="{{ interval_option }}"
-                            {% if interval_option == ticker.interval %}selected{% endif %}
-                          >
-                            {{ interval_option }}
-                          </option>
-                        {%- endfor -%}
-                      </select>
-                      <label class="uk-form-label" for="plot_type"
-                        >Plot type</label
+
+                  <label class="uk-form-label" for="interval">Interval</label>
+                  <select class="uk-select" id="interval" name="interval">
+                    {%- for interval_option in interval_options -%}
+                      <option
+                        value="{{ interval_option }}"
+                        {% if interval_option == ticker.interval %}selected{% endif %}
                       >
-                      <select class="uk-select" id="plot_type" name="plot_type">
-                        {%- for plot_type_option in plot_type_options -%}
-                          <option
-                            value="{{ plot_type_option }}"
-                            {% if plot_type_option == ticker.plot_type %}selected{% endif %}
-                          >
-                            {{ plot_type_option }}
-                          </option>
-                        {%- endfor -%}
-                      </select>
-                      <label class="uk-form-label" for="lookback"
-                        >Lookback</label
-                      >
-                      <input
-                        class="uk-input"
-                        inputmode="numeric"
-                        id="lookback"
-                        name="lookback"
-                        min="1"
-                        uk-tooltip="Number of intervals to look back for."
-                        {#- If the look back is None then it has not been set so use the default lookback for the interval #}
-                        {% if ticker.lookback is none %}placeholder="{{ interval_lookbacks[ticker.interval] }}"{% else %}value="{{ ticker.lookback }}"{% endif %}
-                      />
-                      <label class="uk-form-label" for="wait_time"
-                        >Wait time (s)</label
-                      >
-                      <input
-                        class="uk-input"
-                        inputmode="numeric"
-                        id="wait_time"
-                        name="wait_time"
-                        min="1"
-                        uk-tooltip="Time to wait on this ticker."
-                        {#- If the wait_time is None then it has not been set so use the default wait_time for the interval #}
-                        {% if ticker.wait_time is none %}placeholder="{{ interval_wait_times[ticker.interval] }}"{% else %}value="{{ ticker.wait_time }}"{% endif %}
-                      />
-                      <label class="uk-form-label" for="mav"
-                        >Moving average</label
-                      >
-                      <input
-                        class="uk-input"
-                        inputmode="numeric"
-                        id="mav"
-                        name="mav"
-                        min="1"
-                        uk-tooltip="Optional, number of intervals to include in the moving average."
-                        value="{{ ticker.mav if ticker.mav is not none }}"
-                      />
-                      <label class="uk-form-label" for="avg_buy_price"
-                        >Average buy price</label
-                      >
-                      <input
-                        class="uk-input"
-                        inputmode="numeric"
-                        id="avg_buy_price"
-                        name="avg_buy_price"
-                        min="0"
-                        value="{{ ticker.avg_buy_price if ticker.avg_buy_price is not none }}"
-                        uk-tooltip="Optional, used to display percentage change from buy price."
-                      />
-                      <label class="uk-form-label" for="volume">
-                        <input
-                          type="hidden"
-                          name="volume"
-                          value="{{ 1 if ticker.volume | default(false) else 0 }}"
-                        />
-                        <input
-                          class="uk-checkbox"
-                          type="checkbox"
-                          {% if ticker.volume | default(False) %}checked{% endif %}
-                          onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
-                        />
-                        Show trade volume
-                      </label>
-                      <label
-                        class="uk-form-label"
-                        for="volume"
-                        uk-tooltip="Show pre/post market stock data."
+                        {{ interval_option }}
+                      </option>
+                    {%- endfor -%}
+                  </select>
+
+                  <label class="uk-form-label" for="plot_type">Plot type</label>
+                  <select class="uk-select" id="plot_type" name="plot_type">
+                    {%- for plot_type_option in plot_type_options -%}
+                      <option
+                        value="{{ plot_type_option }}"
+                        {% if plot_type_option == ticker.plot_type %}selected{% endif %}
                       >
-                        <input
-                          type="hidden"
-                          name="prepost"
-                          value="{{ 1 if ticker.prepost | default(false) else 0 }}"
-                        />
-                        <input
-                          class="uk-checkbox"
-                          type="checkbox"
-                          {% if ticker.prepost| default(False) %}checked{% endif %}
-                          onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
-                        />
-                        Fetch pre/post market data
-                      </label>
-                    </div>
-                  {%- endfor -%}
-                  <div
-                    class="uk-card uk-card-primary uk-flex-none uk-margin-right uk-padding-small uk-button uk-border-rounded uk-animation-fade"
-                    uk-tooltip="Add a new ticker"
-                    onclick="add_ticker()"
+                        {{ plot_type_option }}
+                      </option>
+                    {%- endfor -%}
+                  </select>
+
+                  <label class="uk-form-label" for="lookback">Lookback</label>
+                  <input
+                    class="uk-input"
+                    inputmode="numeric"
+                    id="lookback"
+                    name="lookback"
+                    min="1"
+                    uk-tooltip="Number of intervals to look back for."
+                    {#- If the look back is None then it has not been set so use the default lookback for the interval #}
+                    {% if ticker.lookback is none %}placeholder="{{ interval_lookbacks[ticker.interval] }}"{% else %}value="{{ ticker.lookback }}"{% endif %}
+                  />
+
+                  <label class="uk-form-label" for="wait_time"
+                    >Wait time (s)</label
                   >
-                    <span uk-icon="plus"></span>
-                  </div>
+                  <input
+                    class="uk-input"
+                    inputmode="numeric"
+                    id="wait_time"
+                    name="wait_time"
+                    min="1"
+                    uk-tooltip="Time to wait on this ticker."
+                    {#- If the wait_time is None then it has not been set so use the default wait_time for the interval #}
+                    {% if ticker.wait_time is none %}placeholder="{{ interval_wait_times[ticker.interval] }}"{% else %}value="{{ ticker.wait_time }}"{% endif %}
+                  />
+
+                  <label class="uk-form-label" for="mav">Moving average</label>
+                  <input
+                    class="uk-input"
+                    inputmode="numeric"
+                    id="mav"
+                    name="mav"
+                    min="1"
+                    uk-tooltip="Optional, number of intervals to include in the moving average."
+                    value="{{ ticker.mav if ticker.mav is not none }}"
+                  />
+
+                  <label class="uk-form-label" for="avg_buy_price"
+                    >Average buy price</label
+                  >
+                  <input
+                    class="uk-input"
+                    inputmode="numeric"
+                    id="avg_buy_price"
+                    name="avg_buy_price"
+                    min="0"
+                    value="{{ ticker.avg_buy_price if ticker.avg_buy_price is not none }}"
+                    uk-tooltip="Optional, used to display percentage change from buy price."
+                  />
+
+                  <label
+                    class="uk-form-label"
+                    for="volume"
+                    uk-tooltip="Add a trade volume plot bellow the graph."
+                  >
+                    <input
+                      type="hidden"
+                      name="volume"
+                      value="{{ 1 if ticker.volume | default(false) else 0 }}"
+                    />
+                    <input
+                      class="uk-checkbox"
+                      type="checkbox"
+                      {% if ticker.volume | default(False) %}checked{% endif %}
+                      onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
+                    />
+                    Show trade volume
+                  </label>
+
+                  <label
+                    class="uk-form-label"
+                    for="volume"
+                    uk-tooltip="Show pre/post market stock data."
+                  >
+                    <input
+                      type="hidden"
+                      name="prepost"
+                      value="{{ 1 if ticker.prepost | default(false) else 0 }}"
+                    />
+                    <input
+                      class="uk-checkbox"
+                      type="checkbox"
+                      {% if ticker.prepost| default(False) %}checked{% endif %}
+                      onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
+                    />
+                    Fetch pre/post market data
+                  </label>
                 </div>
+              {%- endfor -%}
+              <div
+                class="uk-card uk-card-primary uk-flex-none uk-margin-right uk-padding-small uk-button uk-border-rounded uk-animation-fade"
+                uk-tooltip="Add a new ticker"
+                onclick="add_ticker()"
+              >
+                <span uk-icon="plus"></span>
               </div>
-              <div class="uk-width-1-1 uk-margin">
-                <label
-                  class="uk-form-label"
-                  for="skip_outdated"
-                  uk-tooltip="Typically happens when the market is closed."
-                  ><input
-                    class="uk-checkbox uk-margin-small-right"
-                    type="checkbox"
-                    id="skip_outdated"
-                    name="skip_outdated"
-                    {% if sequence.skip_outdated | default(True) %}checked{% endif %}
-                  />Skip tickers with outdated data</label
-                >
-                <button
-                  type="submit"
-                  value="submit"
-                  class="uk-button uk-button-primary uk-width-expand"
-                >
-                  Apply
-                </button>
-              </div>
+            </div>
+            <div class="uk-width-1-1 uk-margin">
+              <label
+                class="uk-form-label"
+                for="skip_outdated"
+                uk-tooltip="Typically happens when the market is closed."
+                ><input
+                  class="uk-checkbox uk-margin-small-right"
+                  type="checkbox"
+                  id="skip_outdated"
+                  name="skip_outdated"
+                  {% if sequence.skip_outdated | default(True) %}checked{% endif %}
+                />Skip tickers with outdated data</label
+              >
+              <button
+                type="submit"
+                value="submit"
+                class="uk-button uk-button-primary uk-width-expand"
+              >
+                Apply
+              </button>
             </div>
           </form>
         </div>
         <div class="uk-width-large uk-margin">
-          <div class="uk-width-1-1">
-            <p class="uk-text-large">Command</p>
+          <div class="uk-width-1-1 uk-text-center">
+            <hr />
             <form class="uk-form-stacked" action="/command">
               {% for command, desc in commands | items %}
                 <button
                   type="submit"
                   name="command"
                   value="{{ command }}"
                   class="uk-button uk-button-primary uk-width-expand uk-margin-small-bottom"
@@ -342,17 +349,15 @@
         >TinyTicker v{{ version }} - <span uk-icon="github"></span
         ><a
           href="https://github.com/loiccoyle/tinyticker"
           title="tinyticker"
           target="_blank"
           >TinyTicker</a
         >
-        - <span uk-icon="file-text"></span
-        ><a href="/logfiles" title="log files" target="_blank">Log files</a> -
-        <span uk-icon="question"></span
+        - <span uk-icon="question"></span
         ><a
           href="https://github.com/loiccoyle/tinyticker/issues/new"
           title="issues"
           target="_blank"
           >Report an issue</a
         >
       </span>
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-🚀 TinyTicker Dashboard 🚀
+******** ?🚀 TTiinnyyTTiicckkeerr DDaasshhbbooaarrdd ?🚀 ********
+    * _H_o_m_e
+    * _L_o_g_ _F_i_l_e_s
+    * _S_t_a_r_t_u_p_ _s_c_r_i_p_t_s
 🥳 Update available 🥳
 Update & Restart
-Config
 Hostname:[{{ hostname }}      ][Set & Reboot]
 ===============================================================================
-ePaper display model
 {%- for epd_model_option in epd_model_options -%} {%- if epd_model_option.name
 == epd_model -%}
 {{ epd_model_option.desc }}
 {%- else -%}
 {{ epd_model_option.desc }}
 {%- endif -%} {%- endfor -%}
 % if flip | default(False) %}checked{% endif %} />Flip display
-_C_r_y_p_t_o_C_o_m_p_a_r_e API key
+_A_P_I_ _k_e_y
 % if api_key %}value="{{ api_key }}"{% endif %} />
-****** TTiicckkeerrss ******
 {%- for ticker in tickers -%}
 {%- for symbol_type_option in symbol_type_options -%}
 % if symbol_type_option == ticker.symbol_type %}selected{% endif %} > {
 { symbol_type_option }}
 {%- endfor -%}
 {%- for interval_option in interval_options -%}
 % if interval_option == ticker.interval %}selected{% endif %} > {
@@ -44,10 +44,10 @@
 /> Show trade volume
 % if ticker.prepost| default(False) %}checked{% endif %}
 onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
 /> Fetch pre/post market data
 {%- endfor -%}
 % if sequence.skip_outdated | default(True) %}checked{% endif %} />Skip tickers
 with outdated data Apply
-Command
+===============================================================================
 {% for command, desc in commands | items %} {{ command.title() }} {% endfor %}
-TinyTicker v{{ version }} - _T_i_n_y_T_i_c_k_e_r - _L_o_g_ _f_i_l_e_s - _R_e_p_o_r_t_ _a_n_ _i_s_s_u_e
+TinyTicker v{{ version }} - _T_i_n_y_T_i_c_k_e_r - _R_e_p_o_r_t_ _a_n_ _i_s_s_u_e
```

### Comparing `tinyticker-0.6.5/tinyticker/web/templates/js/index.js` & `tinyticker-0.7.0/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.7.0/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.7.0/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.5/tinyticker/web/templates/logfiles.html` & `tinyticker-0.7.0/tinyticker/web/templates/logfiles.html`

 * *Files 14% similar despite different names*

```diff
@@ -23,51 +23,56 @@
     />
     <!-- CSS FILES -->
     <link rel="stylesheet" type="text/css" href="css/uikit.min.css" />
     <!-- JS FILES -->
     <script src="js/uikit.min.js"></script>
     <script src="js/uikit-icons.min.js"></script>
     <script>
-      // get the contents of the log file
-      function getLogFileContent(log_file) {
-        return fetch(`/get-log/${log_file}`).then((response) =>
-          response.text(),
-        );
-      }
       // update the content of the log file
       function updateLogFileContent(log_file) {
-        getLogFileContent(log_file).then((content) => {
-          document.getElementById(`content-${log_file}`).textContent = content;
-        });
+        fetch(`/get-log/${log_file}`)
+          .then((response) => response.text())
+          .then((content) => {
+            document.getElementById(`content-${log_file}`).textContent =
+              content;
+          });
       }
       // update the content of all log files every 60s
       function updateAllLogFileContent() {
         {% for log_file in log_files %}
           updateLogFileContent('{{ log_file }}');
         {% endfor %}
         setTimeout(updateAllLogFileContent, 60000);
       }
       // start updating the content of all log files
       updateAllLogFileContent();
     </script>
   </head>
   <body class="uk-background-muted uk-height-1-1 uk-padding-small">
-    <div class="uk-flex uk-flex-center uk-flex-middle">
-      <div class="uk-width-1-1">
-        <div class="uk-text-center">
-          <p class="uk-text-large">🚀 TinyTicker Log Files 🚀</p>
-        </div>
-        <ul uk-accordion="multiple: true">
-        {% for log_file in log_files %}
-          <li>
-            <a class="uk-accordion-title uk-inline" href>
-              {{ log_file }}
-            </a>
-            <a href="/get-log/{{ log_file }}" class="uk-icon-link" uk-icon="download"></a>
-            <pre id="content-{{ log_file }}" class="uk-height-large uk-accordion-content"></pre>
-          </li>
-        {% endfor %}
+    <div class="uk-text-center uk-margin">
+      <h3>🚀 TinyTicker Log Files 🚀</h3>
+      <div class="uk-flex uk-flex-center">
+        <ul class="uk-subnav uk-subnav-divider uk-margin">
+          <li><a href="/" target="_self">Home</a></li>
+          <li class="uk-active"><a href="#">Log Files</a></li>
+          <li><a href="/startup" target="_self">Startup scripts</a></li>
         </ul>
       </div>
     </div>
+    <ul uk-accordion="multiple: true">
+      {% for log_file in log_files %}
+        <li>
+          <a class="uk-accordion-title uk-inline" href> {{ log_file }} </a>
+          <a
+            href="/get-log/{{ log_file }}"
+            class="uk-icon-link"
+            uk-icon="download"
+          ></a>
+          <pre
+            id="content-{{ log_file }}"
+            class="uk-height-large uk-accordion-content"
+          ></pre>
+        </li>
+      {% endfor %}
+    </ul>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,4 +1,7 @@
-🚀 TinyTicker Log Files 🚀
+******** ?🚀 TTiinnyyTTiicckkeerr LLoogg FFiilleess ?🚀 ********
+    * _H_o_m_e
+    * _L_o_g_ _F_i_l_e_s
+    * _S_t_a_r_t_u_p_ _s_c_r_i_p_t_s
     * {% for log_file in log_files %}
     * {{ log_file }}
     * {% endfor %}
```

### Comparing `tinyticker-0.6.5/PKG-INFO` & `tinyticker-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.6.5
+Version: 0.7.0
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
@@ -36,15 +36,15 @@
   <img  src="https://i.imgur.com/J4k3PCM.png" height=400>
   <img src="https://i.imgur.com/QWP7bpH.png" height=400>
 </div>
 <p align="center">
   <a href="https://pypi.org/project/tinyticker/"><img src="https://img.shields.io/pypi/v/tinyticker"></a>
   <a href="./LICENSE.md"><img src="https://img.shields.io/badge/license-MIT-blue.svg"></a>
   <a href="https://github.com/loiccoyle/tinyticker/actions/workflows/ci.yml"><img src="https://github.com/loiccoyle/tinyticker/actions/workflows/ci.yml/badge.svg"></a>
-  <a href="https://discord.com/channels/1239232827237597184/1239232827841839297"><img alt="Discord" src="https://img.shields.io/discord/1239232827237597184?logo=discord&logoSize=auto&label=%20"></a>
+  <a href="https://discord.com/channels/1239232827237597184/1239232827841839297"><img alt="Discord" src="https://img.shields.io/badge/%20discord-%20?logo=discord"></a>
 </p>
 <hr/>
 
 `tinyticker` uses a Raspberry Pi zero W and a small ePaper display to periodically display a stock or crypto chart.
 
 A `flask` web interface is created to set the ticker options and control the Raspberry Pi.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.6.5 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.7.0 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

