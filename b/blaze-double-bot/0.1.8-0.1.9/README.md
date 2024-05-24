# Comparing `tmp/blaze_double_bot-0.1.8.tar.gz` & `tmp/blaze_double_bot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaze_double_bot-0.1.8.tar", last modified: Thu May 23 23:11:56 2024, max compression
+gzip compressed data, was "blaze_double_bot-0.1.9.tar", last modified: Thu May 23 23:38:12 2024, max compression
```

## Comparing `blaze_double_bot-0.1.8.tar` & `blaze_double_bot-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 23:11:56.467838 blaze_double_bot-0.1.8/
--rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     3146 2024-05-23 23:11:56.463825 blaze_double_bot-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2657 2024-05-23 12:04:16.000000 blaze_double_bot-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 23:11:56.407737 blaze_double_bot-0.1.8/blaze_double_bot/
--rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.1.8/blaze_double_bot/__init__.py
--rw-rw-rw-   0        0        0     9625 2024-05-23 23:02:20.000000 blaze_double_bot-0.1.8/blaze_double_bot/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:11:56.463825 blaze_double_bot-0.1.8/blaze_double_bot.egg-info/
--rw-rw-rw-   0        0        0     3146 2024-05-23 23:11:56.000000 blaze_double_bot-0.1.8/blaze_double_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-23 23:11:56.000000 blaze_double_bot-0.1.8/blaze_double_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 23:11:56.000000 blaze_double_bot-0.1.8/blaze_double_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 23:11:56.000000 blaze_double_bot-0.1.8/blaze_double_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-23 23:11:56.000000 blaze_double_bot-0.1.8/blaze_double_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 23:11:56.467838 blaze_double_bot-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-05-23 22:49:39.000000 blaze_double_bot-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:38:12.217370 blaze_double_bot-0.1.9/
+-rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     3146 2024-05-23 23:38:12.217370 blaze_double_bot-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2657 2024-05-23 12:04:16.000000 blaze_double_bot-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 23:38:12.163082 blaze_double_bot-0.1.9/blaze_double_bot/
+-rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.1.9/blaze_double_bot/__init__.py
+-rw-rw-rw-   0        0        0     9974 2024-05-23 23:36:12.000000 blaze_double_bot-0.1.9/blaze_double_bot/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:38:12.215056 blaze_double_bot-0.1.9/blaze_double_bot.egg-info/
+-rw-rw-rw-   0        0        0     3146 2024-05-23 23:38:11.000000 blaze_double_bot-0.1.9/blaze_double_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-23 23:38:12.000000 blaze_double_bot-0.1.9/blaze_double_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 23:38:11.000000 blaze_double_bot-0.1.9/blaze_double_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 23:38:11.000000 blaze_double_bot-0.1.9/blaze_double_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-23 23:38:11.000000 blaze_double_bot-0.1.9/blaze_double_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 23:38:12.217370 blaze_double_bot-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-23 23:37:40.000000 blaze_double_bot-0.1.9/setup.py
```

### Comparing `blaze_double_bot-0.1.8/LICENSE` & `blaze_double_bot-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.1.8/PKG-INFO` & `blaze_double_bot-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.1.8
+Version: 0.1.9
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blaze_double_bot-0.1.8/README.md` & `blaze_double_bot-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.1.8/blaze_double_bot/bot.py` & `blaze_double_bot-0.1.9/blaze_double_bot/bot.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import argparse
 import undetected_chromedriver as uc
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
 from selenium.webdriver.chrome.options import Options
 from time import sleep
+from datetime import datetime
 import requests
 
 class BlazeDoubleBot:
     def __init__(self, config):
         self.username = config['username']
         self.password = config['password']
         self.bet_amount = config['bet_amount']
@@ -106,15 +107,15 @@
                 actions = ActionChains(self.driver)
                 sleep(1)
                 actions.click(b).perform()
                 break
 
     def print_bet(self, color):
         print(f'''
-
+{datetime.now().strftime("%m/%d/%Y %H:%M")}
 Bet on {"Red" if color == "red" else "Black"}
 Completed
 Waiting for result ...
 
 ''')
 
     def print_bet_result(self, history, color):
@@ -139,14 +140,15 @@
         return max_size
 
     def print_initialization_text(self):
         print(f'''
 {50 * "*"}
 
 ***  Blaze Double Bet Bot Started   ***
+{datetime.now().strftime("%m/%d/%Y %H:%M")}
 
 Initial Balance: $ {round(self.initial_balance, 2)}
 
 Stop Loss: $ {round(self.stop_loss, 2)}
 
 Stop Win: $ {round(self.stop_win, 2)}
 
@@ -162,14 +164,16 @@
 
 ***  Blaze Double Bet Bot Finished   ***
 
 Initial Balance: $ {round(self.initial_balance, 2)}
 
 Final Balance: $ {round(self.current_balance, 2)}
 
+{datetime.now().strftime("%m/%d/%Y %H:%M")}
+
 {50 * "*"}
 
 ''')
 
     def wait_for_next_round(self):
         while True:
             try:
@@ -190,14 +194,15 @@
             strategy_size = self.get_strategy_size()
             while True:
                 if self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
                     if self.wait_for_next_round():
                         history = self.get_history_api(strategy_size)
                         color = self.strategy(history)
                         if color:
+                            
                             print(history)
                             print()
                             self.choose_color(color)
                             self.place_bet(self.bet_amount)
                             self.print_bet(color)
                             self.wait_for_next_round()
                             sleep(1)
@@ -219,19 +224,21 @@
                                     sleep(1)
                                     history = self.get_history_api(strategy_size)
                             self.print_bet_result(history, color)
                             print(history)
                             sleep(8)
                             self.current_balance = self.get_balance()
                             print('Balance: $ ',self.current_balance)
+                            print(datetime.now().strftime("%m/%d/%Y %H:%M"))
                             if self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
                                 print('Waiting 150 seconds(5 rounds) to restart analysis ...')
                                 sleep(150)
                                 print(50*'*')
                                 print('Analyzes restarted!\n')
+                                print(datetime.now().strftime("%m/%d/%Y %H:%M"))
                             
                 else:
                     self.print_final_text()
                     self.close_driver()
                     break
```

### Comparing `blaze_double_bot-0.1.8/blaze_double_bot.egg-info/PKG-INFO` & `blaze_double_bot-0.1.9/blaze_double_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.1.8
+Version: 0.1.9
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

