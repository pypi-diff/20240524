# Comparing `tmp/traderpy-1.0.6.tar.gz` & `tmp/traderpy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traderpy-1.0.6.tar", last modified: Sun Dec 10 15:42:47 2023, max compression
+gzip compressed data, was "traderpy-1.0.7.tar", last modified: Fri May 24 11:44:05 2024, max compression
```

## Comparing `traderpy-1.0.6.tar` & `traderpy-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rakshithcrm   (501) staff       (20)        0 2023-12-10 15:42:47.549656 traderpy-1.0.6/
--rw-r--r--   0 rakshithcrm   (501) staff       (20)     1069 2023-09-07 05:18:16.000000 traderpy-1.0.6/LICENSE
--rw-r--r--   0 rakshithcrm   (501) staff       (20)     1218 2023-12-10 15:42:47.549444 traderpy-1.0.6/PKG-INFO
--rw-r--r--   0 rakshithcrm   (501) staff       (20)      899 2023-12-06 11:06:19.000000 traderpy-1.0.6/README.md
--rw-r--r--   0 rakshithcrm   (501) staff       (20)       38 2023-12-10 15:42:47.549699 traderpy-1.0.6/setup.cfg
--rw-r--r--   0 rakshithcrm   (501) staff       (20)      469 2023-12-10 15:42:21.000000 traderpy-1.0.6/setup.py
-drwxr-xr-x   0 rakshithcrm   (501) staff       (20)        0 2023-12-10 15:42:47.546839 traderpy-1.0.6/tests/
--rw-r--r--   0 rakshithcrm   (501) staff       (20)     1984 2023-12-10 15:41:28.000000 traderpy-1.0.6/tests/testing.py
-drwxr-xr-x   0 rakshithcrm   (501) staff       (20)        0 2023-12-10 15:42:47.548393 traderpy-1.0.6/trader/
--rw-r--r--   0 rakshithcrm   (501) staff       (20)      197 2023-12-06 11:14:23.000000 traderpy-1.0.6/trader/__init__.py
--rw-r--r--   0 rakshithcrm   (501) staff       (20)     2231 2023-12-06 12:21:59.000000 traderpy-1.0.6/trader/display.py
--rw-r--r--   0 rakshithcrm   (501) staff       (20)     2898 2023-12-10 15:38:45.000000 traderpy-1.0.6/trader/ma.py
--rw-r--r--   0 rakshithcrm   (501) staff       (20)     1950 2023-11-29 09:30:38.000000 traderpy-1.0.6/trader/plotter.py
--rw-r--r--   0 rakshithcrm   (501) staff       (20)     3482 2023-12-10 15:38:14.000000 traderpy-1.0.6/trader/processor.py
--rw-r--r--   0 rakshithcrm   (501) staff       (20)      470 2023-11-29 10:18:18.000000 traderpy-1.0.6/trader/queable.py
--rw-r--r--   0 rakshithcrm   (501) staff       (20)     2962 2023-12-10 15:39:10.000000 traderpy-1.0.6/trader/rsi.py
--rw-r--r--   0 rakshithcrm   (501) staff       (20)     5006 2023-12-10 15:39:29.000000 traderpy-1.0.6/trader/rsl.py
--rw-r--r--   0 rakshithcrm   (501) staff       (20)     2073 2023-12-10 09:04:20.000000 traderpy-1.0.6/trader/stock.py
--rw-r--r--   0 rakshithcrm   (501) staff       (20)     2086 2023-12-10 15:40:02.000000 traderpy-1.0.6/trader/trend.py
--rw-r--r--   0 rakshithcrm   (501) staff       (20)     1176 2023-12-10 07:07:08.000000 traderpy-1.0.6/trader/utils.py
-drwxr-xr-x   0 rakshithcrm   (501) staff       (20)        0 2023-12-10 15:42:47.549209 traderpy-1.0.6/traderpy.egg-info/
--rw-r--r--   0 rakshithcrm   (501) staff       (20)     1218 2023-12-10 15:42:47.000000 traderpy-1.0.6/traderpy.egg-info/PKG-INFO
--rw-r--r--   0 rakshithcrm   (501) staff       (20)      384 2023-12-10 15:42:47.000000 traderpy-1.0.6/traderpy.egg-info/SOURCES.txt
--rw-r--r--   0 rakshithcrm   (501) staff       (20)        1 2023-12-10 15:42:47.000000 traderpy-1.0.6/traderpy.egg-info/dependency_links.txt
--rw-r--r--   0 rakshithcrm   (501) staff       (20)       69 2023-12-10 15:42:47.000000 traderpy-1.0.6/traderpy.egg-info/requires.txt
--rw-r--r--   0 rakshithcrm   (501) staff       (20)        7 2023-12-10 15:42:47.000000 traderpy-1.0.6/traderpy.egg-info/top_level.txt
+drwxr-xr-x   0 rakshithcrm   (501) staff       (20)        0 2024-05-24 11:44:05.099082 traderpy-1.0.7/
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)     1069 2023-09-07 05:18:16.000000 traderpy-1.0.7/LICENSE
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)     1218 2024-05-24 11:44:05.098735 traderpy-1.0.7/PKG-INFO
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)      899 2023-12-06 11:06:19.000000 traderpy-1.0.7/README.md
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)       38 2024-05-24 11:44:05.099284 traderpy-1.0.7/setup.cfg
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)      469 2023-12-10 16:00:25.000000 traderpy-1.0.7/setup.py
+drwxr-xr-x   0 rakshithcrm   (501) staff       (20)        0 2024-05-24 11:44:05.090582 traderpy-1.0.7/tests/
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)     1984 2023-12-10 16:35:33.000000 traderpy-1.0.7/tests/testing.py
+drwxr-xr-x   0 rakshithcrm   (501) staff       (20)        0 2024-05-24 11:44:05.096034 traderpy-1.0.7/trader/
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)      197 2023-12-06 11:14:23.000000 traderpy-1.0.7/trader/__init__.py
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)     2231 2023-12-06 12:21:59.000000 traderpy-1.0.7/trader/display.py
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)     2898 2023-12-10 15:38:45.000000 traderpy-1.0.7/trader/ma.py
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)     1950 2024-05-24 08:18:04.000000 traderpy-1.0.7/trader/plotter.py
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)     3508 2023-12-10 16:36:41.000000 traderpy-1.0.7/trader/processor.py
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)      470 2023-11-29 10:18:18.000000 traderpy-1.0.7/trader/queable.py
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)     2856 2023-12-10 17:34:50.000000 traderpy-1.0.7/trader/rsi.py
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)     5006 2023-12-10 15:39:29.000000 traderpy-1.0.7/trader/rsl.py
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)     2073 2023-12-10 09:04:20.000000 traderpy-1.0.7/trader/stock.py
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)     2086 2023-12-10 15:40:02.000000 traderpy-1.0.7/trader/trend.py
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)     1177 2023-12-10 19:35:21.000000 traderpy-1.0.7/trader/utils.py
+drwxr-xr-x   0 rakshithcrm   (501) staff       (20)        0 2024-05-24 11:44:05.098264 traderpy-1.0.7/traderpy.egg-info/
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)     1218 2024-05-24 11:44:05.000000 traderpy-1.0.7/traderpy.egg-info/PKG-INFO
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)      384 2024-05-24 11:44:05.000000 traderpy-1.0.7/traderpy.egg-info/SOURCES.txt
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)        1 2024-05-24 11:44:05.000000 traderpy-1.0.7/traderpy.egg-info/dependency_links.txt
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)       69 2024-05-24 11:44:05.000000 traderpy-1.0.7/traderpy.egg-info/requires.txt
+-rw-r--r--   0 rakshithcrm   (501) staff       (20)        7 2024-05-24 11:44:05.000000 traderpy-1.0.7/traderpy.egg-info/top_level.txt
```

### Comparing `traderpy-1.0.6/LICENSE` & `traderpy-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `traderpy-1.0.6/PKG-INFO` & `traderpy-1.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traderpy
-Version: 1.0.6
+Version: 1.0.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: yfinance
 Requires-Dist: pandas
 Requires-Dist: pygame
 Requires-Dist: plotly
 Requires-Dist: tqdm
```

### Comparing `traderpy-1.0.6/README.md` & `traderpy-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `traderpy-1.0.6/tests/testing.py` & `traderpy-1.0.7/tests/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 
 
 def process_ticker(ticker):
     print("-" * 150)
 
     stock = Stock(ticker)
     print("Processing stock ticker", ticker, "number of datapoints", len(stock.get_data()))
-    # processor = Processor.default_processor(stock=stock)
-    processor = Processor.load_processor(stock=stock, dir=MODEL_DIR)
+    processor = Processor.default_processor(stock=stock)
+    # processor = Processor.load_processor(stock=stock, dir=MODEL_DIR)
     processor.process()
     results = processor.result()
     trade_quality = processor.quality()
     print(processor.description())
     processor.save(dir=MODEL_DIR)
     print("TRADE QUALITIES")
     for key, value in trade_quality.items():
```

### Comparing `traderpy-1.0.6/trader/display.py` & `traderpy-1.0.7/trader/display.py`

 * *Files identical despite different names*

### Comparing `traderpy-1.0.6/trader/ma.py` & `traderpy-1.0.7/trader/ma.py`

 * *Files identical despite different names*

### Comparing `traderpy-1.0.6/trader/plotter.py` & `traderpy-1.0.7/trader/plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import plotly.io as pio
 
 from .stock import Stock
 from .utils import DAYS
 
 
 class Plotter:
-    def __init__(self, layout, row_heights=[], focus=DAYS["3mo"]):
+    def __init__(self, layout, row_heights=[], focus=DAYS["6mo"]):
         self.fig = sp.make_subplots(
             rows=layout[0], cols=layout[1], row_heights=row_heights, shared_xaxes=True
         )
         self.fig.update_layout(xaxis_rangeslider_visible=False)
         self.focus = focus
 
     def addLine(self, index, values, row, col, name):
```

### Comparing `traderpy-1.0.6/trader/processor.py` & `traderpy-1.0.7/trader/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
     def add(self, queable_obj: Queable):
         self.queue.append(queable_obj)
 
     def process(self):
         for obj in tqdm(self.queue):
             obj.process()
+            obj.quality()
 
     def result(self):
         results = []
         for obj in self.queue:
             results.append(obj.result())
         return results
```

### Comparing `traderpy-1.0.6/trader/rsi.py` & `traderpy-1.0.7/trader/rsi.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,13 +77,11 @@
         avg_gains = np.mean(net_gains)
         avg_losses = abs(np.mean(net_losses))
         rs = avg_gains / avg_losses
         rsi_value = 100 - (100 / (1 + rs))
         return rsi_value
 
     def quality(self):
-        current_price = self.stock.get_data()["Close"][-1]
-        if are_numbers_close(self.rsi_values[-1], current_price):
+        self.trade_quality = False
+        if self.rsi_values[-1] > 70:
             self.trade_quality = True
-        else:
-            self.trade_quality = False
         return self.trade_quality
```

### Comparing `traderpy-1.0.6/trader/rsl.py` & `traderpy-1.0.7/trader/rsl.py`

 * *Files identical despite different names*

### Comparing `traderpy-1.0.6/trader/stock.py` & `traderpy-1.0.7/trader/stock.py`

 * *Files identical despite different names*

### Comparing `traderpy-1.0.6/trader/trend.py` & `traderpy-1.0.7/trader/trend.py`

 * *Files identical despite different names*

### Comparing `traderpy-1.0.6/trader/utils.py` & `traderpy-1.0.7/trader/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def are_numbers_close(number1, number2):
     absolute_difference = abs(number1 - number2)
     average = (number1 + number2) / 2
 
     relative_difference = absolute_difference / average
 
     # Define a threshold for closeness (e.g., 0.1 for 10%)
-    threshold = 0.03  # Adjust this threshold as needed
+    threshold = 0.015  # Adjust this threshold as needed
 
     if relative_difference < threshold:
         return True
     else:
         return False
```

### Comparing `traderpy-1.0.6/traderpy.egg-info/PKG-INFO` & `traderpy-1.0.7/traderpy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traderpy
-Version: 1.0.6
+Version: 1.0.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: yfinance
 Requires-Dist: pandas
 Requires-Dist: pygame
 Requires-Dist: plotly
 Requires-Dist: tqdm
```

