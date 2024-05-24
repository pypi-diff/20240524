# Comparing `tmp/tinyticker-0.7.0.tar.gz` & `tmp/tinyticker-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.7.0.tar", max compression
+gzip compressed data, was "tinyticker-0.7.1.tar", max compression
```

## Comparing `tinyticker-0.7.0.tar` & `tinyticker-0.7.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1068 2024-05-24 00:37:02.507527 tinyticker-0.7.0/LICENSE
--rw-r--r--   0        0        0     3955 2024-05-24 00:37:02.507527 tinyticker-0.7.0/README.md
--rw-r--r--   0        0        0      917 2024-05-24 00:37:02.507527 tinyticker-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      465 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/__init__.py
--rw-r--r--   0        0        0     5967 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/__main__.py
--rw-r--r--   0        0        0     2496 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/config.py
--rw-r--r--   0        0        0     9000 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/paths.py
--rw-r--r--   0        0        0     5483 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/sequence.py
--rw-r--r--   0        0        0     1112 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/tickers/__init__.py
--rw-r--r--   0        0        0     3618 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/tickers/_base.py
--rw-r--r--   0        0        0     4620 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/tickers/crypto.py
--rw-r--r--   0        0        0     2915 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/tickers/stock.py
--rw-r--r--   0        0        0     2391 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0    21091 2024-05-24 00:37:02.511527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in7.py
--rw-r--r--   0        0        0    19697 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in7_V2.py
--rw-r--r--   0        0        0     1551 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2895 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     8457 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/app.py
--rw-r--r--   0        0        0     3656 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/command.py
--rw-r--r--   0        0        0      506 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/startup.py
--rw-r--r--   0        0        0   274777 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    14743 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     1904 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     2449 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     2970 2024-05-24 00:37:02.515527 tinyticker-0.7.0/tinyticker/web/templates/startup.html
--rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 tinyticker-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-24 02:31:01.199461 tinyticker-0.7.1/LICENSE
+-rw-r--r--   0        0        0     3955 2024-05-24 02:31:01.199461 tinyticker-0.7.1/README.md
+-rw-r--r--   0        0        0      917 2024-05-24 02:31:01.199461 tinyticker-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      465 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/__init__.py
+-rw-r--r--   0        0        0     5967 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/__main__.py
+-rw-r--r--   0        0        0     2496 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/config.py
+-rw-r--r--   0        0        0     9000 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/paths.py
+-rw-r--r--   0        0        0     5483 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/sequence.py
+-rw-r--r--   0        0        0     1112 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/tickers/__init__.py
+-rw-r--r--   0        0        0     3618 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/tickers/_base.py
+-rw-r--r--   0        0        0     4620 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/tickers/crypto.py
+-rw-r--r--   0        0        0     2915 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/tickers/stock.py
+-rw-r--r--   0        0        0     2391 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-24 02:31:01.203461 tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0    21091 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in7.py
+-rw-r--r--   0        0        0    19697 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in7_V2.py
+-rw-r--r--   0        0        0     1551 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2895 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     8457 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/web/app.py
+-rw-r--r--   0        0        0     3656 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/web/command.py
+-rw-r--r--   0        0        0      503 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/web/startup.py
+-rw-r--r--   0        0        0   274777 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    14743 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     1904 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-24 02:31:01.207460 tinyticker-0.7.1/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-24 02:31:01.211460 tinyticker-0.7.1/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     2449 2024-05-24 02:31:01.211460 tinyticker-0.7.1/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     2970 2024-05-24 02:31:01.211460 tinyticker-0.7.1/tinyticker/web/templates/startup.html
+-rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 tinyticker-0.7.1/PKG-INFO
```

### Comparing `tinyticker-0.7.0/LICENSE` & `tinyticker-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/README.md` & `tinyticker-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/pyproject.toml` & `tinyticker-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.7.0"
+version = "0.7.1"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.7.0/tinyticker/__main__.py` & `tinyticker-0.7.1/tinyticker/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/config.py` & `tinyticker-0.7.1/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/display.py` & `tinyticker-0.7.1/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/sequence.py` & `tinyticker-0.7.1/tinyticker/sequence.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/tickers/__init__.py` & `tinyticker-0.7.1/tinyticker/tickers/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/tickers/_base.py` & `tinyticker-0.7.1/tinyticker/tickers/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/tickers/crypto.py` & `tinyticker-0.7.1/tinyticker/tickers/crypto.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/tickers/stock.py` & `tinyticker-0.7.1/tinyticker/tickers/stock.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/utils.py` & `tinyticker-0.7.1/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.7.1/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/waveshare_lib/device.py` & `tinyticker-0.7.1/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in7.py` & `tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in7.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/waveshare_lib/epd2in7_V2.py` & `tinyticker-0.7.1/tinyticker/waveshare_lib/epd2in7_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/waveshare_lib/models.py` & `tinyticker-0.7.1/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/web/__main__.py` & `tinyticker-0.7.1/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/web/app.py` & `tinyticker-0.7.1/tinyticker/web/app.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/web/command.py` & `tinyticker-0.7.1/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.7.1/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.7.1/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.7.1/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.7.1/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/web/templates/index.html` & `tinyticker-0.7.1/tinyticker/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/web/templates/js/index.js` & `tinyticker-0.7.1/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.7.1/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.7.1/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/web/templates/logfiles.html` & `tinyticker-0.7.1/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/tinyticker/web/templates/startup.html` & `tinyticker-0.7.1/tinyticker/web/templates/startup.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.0/PKG-INFO` & `tinyticker-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.7.0
+Version: 0.7.1
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.7.0 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.7.1 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

