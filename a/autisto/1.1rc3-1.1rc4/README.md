# Comparing `tmp/autisto-1.1rc3.tar.gz` & `tmp/autisto-1.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autisto-1.1rc3.tar", last modified: Tue Mar 26 00:18:09 2024, max compression
+gzip compressed data, was "autisto-1.1rc4.tar", last modified: Thu May 23 22:12:00 2024, max compression
```

## Comparing `autisto-1.1rc3.tar` & `autisto-1.1rc4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:18:09.823312 autisto-1.1rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-26 00:18:04.000000 autisto-1.1rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 00:18:04.000000 autisto-1.1rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-26 00:18:09.823312 autisto-1.1rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-26 00:18:04.000000 autisto-1.1rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:18:09.823312 autisto-1.1rc3/autisto/
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-03-26 00:18:04.000000 autisto-1.1rc3/autisto/daemons.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-03-26 00:18:04.000000 autisto-1.1rc3/autisto/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-03-26 00:18:04.000000 autisto-1.1rc3/autisto/finances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-26 00:18:04.000000 autisto-1.1rc3/autisto/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    17985 2024-03-26 00:18:04.000000 autisto-1.1rc3/autisto/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-03-26 00:18:04.000000 autisto-1.1rc3/autisto/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:18:09.823312 autisto-1.1rc3/autisto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-26 00:18:09.000000 autisto-1.1rc3/autisto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-26 00:18:09.000000 autisto-1.1rc3/autisto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 00:18:09.000000 autisto-1.1rc3/autisto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-26 00:18:09.000000 autisto-1.1rc3/autisto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-26 00:18:09.000000 autisto-1.1rc3/autisto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-26 00:18:09.000000 autisto-1.1rc3/autisto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-26 00:18:04.000000 autisto-1.1rc3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 00:18:09.823312 autisto-1.1rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-26 00:18:04.000000 autisto-1.1rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 00:18:09.823312 autisto-1.1rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13007 2024-03-26 00:18:04.000000 autisto-1.1rc3/tests/test_autisto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:12:00.340217 autisto-1.1rc4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 22:11:55.000000 autisto-1.1rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 22:11:55.000000 autisto-1.1rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-23 22:12:00.340217 autisto-1.1rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-23 22:11:55.000000 autisto-1.1rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:12:00.336217 autisto-1.1rc4/autisto/
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-05-23 22:11:55.000000 autisto-1.1rc4/autisto/daemons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-23 22:11:55.000000 autisto-1.1rc4/autisto/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-23 22:11:55.000000 autisto-1.1rc4/autisto/finances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-23 22:11:55.000000 autisto-1.1rc4/autisto/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18561 2024-05-23 22:11:55.000000 autisto-1.1rc4/autisto/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-23 22:11:55.000000 autisto-1.1rc4/autisto/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:12:00.336217 autisto-1.1rc4/autisto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-23 22:12:00.000000 autisto-1.1rc4/autisto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-23 22:12:00.000000 autisto-1.1rc4/autisto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:12:00.000000 autisto-1.1rc4/autisto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 22:12:00.000000 autisto-1.1rc4/autisto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 22:12:00.000000 autisto-1.1rc4/autisto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 22:12:00.000000 autisto-1.1rc4/autisto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 22:11:55.000000 autisto-1.1rc4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:12:00.340217 autisto-1.1rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-23 22:11:55.000000 autisto-1.1rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:12:00.336217 autisto-1.1rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13015 2024-05-23 22:11:55.000000 autisto-1.1rc4/tests/test_autisto.py
```

### Comparing `autisto-1.1rc3/LICENSE` & `autisto-1.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `autisto-1.1rc3/PKG-INFO` & `autisto-1.1rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autisto
-Version: 1.1rc3
+Version: 1.1rc4
 Summary: Basic accounting (?) program integrated with Google Sheets to fulfill my own autistic needs of tracking the shit owned.
 Author: Jan Grzybek
 Author-email: lyre_embassy_0n@icloud.com
 License: MIT
 Project-URL: GitHub, https://github.com/jan-grzybek/autisto
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `autisto-1.1rc3/README.md` & `autisto-1.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `autisto-1.1rc3/autisto/daemons.py` & `autisto-1.1rc4/autisto/daemons.py`

 * *Files identical despite different names*

### Comparing `autisto-1.1rc3/autisto/database.py` & `autisto-1.1rc4/autisto/database.py`

 * *Files identical despite different names*

### Comparing `autisto-1.1rc3/autisto/finances.py` & `autisto-1.1rc4/autisto/finances.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 import csv
 import urllib.error
 import urllib.request
 from datetime import datetime
 from dateutil.relativedelta import relativedelta
 
-URL = "https://stat.gov.pl/download/gfx/portalinformacyjny/pl/defaultstronaopisowa/4741/1/1/miesieczne_wskazniki_cen_" \
-      "towarow_i_uslug_konsumpcyjnych_od_1982_roku_3.csv"
-
 
 class FinanceModule:
+    url = ("https://stat.gov.pl/download/gfx/portalinformacyjny/pl/defaultstronaopisowa/4741/1/1/miesieczne_wskazniki_"
+           "cen_towarow_i_uslug_konsumpcyjnych_od_1982_roku_5.csv")
+
     def __init__(self):
         self.error = None
         self._calc_accumulated_inflation(self._extract_month_over_month_inflation(self._load_inflation_data()))
 
     def _load_inflation_data(self):
         try:
-            response = urllib.request.urlopen(URL)
+            response = urllib.request.urlopen(FinanceModule.url)
             return csv.reader([line.decode("windows-1250") for line in response.readlines()], delimiter=";")
         except Exception as e:
             self.error = e
             return []
 
     def _extract_month_over_month_inflation(self, raw_inflation_data):
         month_over_month_inflation_data = {}
         for row in raw_inflation_data:
             if "Poprzedni miesiąc = 100" == row[2]:
                 try:
                     inflation_rate = float(row[5].replace(",", ".")) / 100
                 except ValueError:
                     continue
                 try:
-                      if int(row[3]) in month_over_month_inflation_data.keys():
-                          month_over_month_inflation_data[int(row[3])][int(row[4])] = inflation_rate
-                      else:
-                          month_over_month_inflation_data[int(row[3])] = {int(row[4]): float(row[5].replace(",", ".")) / 100}
+                    if int(row[3]) in month_over_month_inflation_data.keys():
+                        month_over_month_inflation_data[int(row[3])][int(row[4])] = inflation_rate
+                    else:
+                        month_over_month_inflation_data[int(row[3])] = {
+                            int(row[4]): float(row[5].replace(",", ".")) / 100}
                 except Exception as e:
-                      self.error = e
-                      return {}
+                    self.error = e
+                    return {}
 
         two_months_ago = datetime.now() - relativedelta(months=2)
         if self.error is None:
             try:
                 month_over_month_inflation_data[two_months_ago.year][two_months_ago.month]
             except KeyError:
-                self.error = KeyError(f"Error: inflation data for {two_months_ago.strftime('%B')} {two_months_ago.year} " \
-                                      f"is missing in GUS .csv file available at {URL}")
+                self.error = KeyError(
+                    f"Error: inflation data for {two_months_ago.strftime('%B')} {two_months_ago.year} "
+                    f"is missing in GUS .csv file available at {FinanceModule.url}")
         return month_over_month_inflation_data
 
     def _calc_accumulated_inflation(self, month_over_month_inflation_data):
         self._current_time = datetime.now()
         self._accumulated_inflation = {}
         accumulated_inflation = 1.
         for year in reversed(range(1982, self._current_time.year + 1)):
```

### Comparing `autisto-1.1rc3/autisto/server.py` & `autisto-1.1rc4/autisto/server.py`

 * *Files identical despite different names*

### Comparing `autisto-1.1rc3/autisto/spreadsheet.py` & `autisto-1.1rc4/autisto/spreadsheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import gspread
+import urllib.request
 from bson.errors import InvalidId
 from autisto.utils import *
+from autisto.finances import FinanceModule
 from datetime import datetime
 from dateutil.relativedelta import relativedelta
 
 BEGINNING_OF_TIME = datetime(1900, 1, 1)
 
 START_ROW = 1
 START_COL = 1
@@ -45,34 +47,43 @@
         self._start_row = to_1_based(START_ROW)
         self._start_col = START_COL
         self._column_names = CONSOLE_COL_NAMES
         self._orders = []
         self.db = database
 
     def clean_up(self, orders_only=False):
+        url_value = self._sheet.cell(self._start_row, 3).value
+        if url_value is not None:
+            try:
+                urllib.request.urlopen(url_value)
+                FinanceModule.url = url_value
+            except Exception as e:
+                FinanceModule.url = str(e)
         if not orders_only:
-            self._sheet.batch_clear(["A1:A", "A1:Z2", "K1:Z"])
+            self._sheet.batch_clear(["A1:A", "A1:Z3", "K1:Z"])
             self._sheet.format("A1:Z", {"textFormat": {"bold": False}})
-            self._sheet.format(f"B{self._start_row}:Z{self._start_row}", {"textFormat": {"bold": True}})
-            self._sheet.update([self._column_names], f"B{self._start_row}:L{self._start_row}")
+            self._sheet.format(f"B{self._start_row}:Z{self._start_row+1}", {"textFormat": {"bold": True}})
+            self._sheet.update([["URL to .csv file with monthly inflation data (available at GUS website):",
+                                 FinanceModule.url] + [None for _ in range(len(self._column_names)-2)],
+                                self._column_names], f"B{self._start_row}:L{self._start_row+1}")
         for order in self._orders:
             self._sheet.batch_clear([f"B{order.row}:Z{order.row}"])
         self._orders = []
 
     def _get_col_index(self, col_name):
         return self._start_col + self._column_names.index(col_name)
 
     def _get_ready_rows(self):
-        confirmation_tokens = self._sheet.col_values(to_1_based(self._get_col_index("Done? <Y>")))[self._start_row:]
+        confirmation_tokens = self._sheet.col_values(to_1_based(self._get_col_index("Done? <Y>")))[self._start_row+1:]
         ready_rows = []
         for i, token in enumerate(confirmation_tokens):
             if token in ["y", "yes", "Y", "YES"]:
-                ready_rows.append(self._start_row + i)
+                ready_rows.append(self._start_row + i + 1)
             elif token != "":
-                self._sheet.update_cell(self._start_row + i + 1, to_1_based(self._get_col_index("Status")),
+                self._sheet.update_cell(self._start_row + i + 2, to_1_based(self._get_col_index("Status")),
                                         f"Wrong confirmation token: '{confirmation_tokens[i]}' "
                                         f"(should be 'Y' instead)")
         return ready_rows
 
     def _get_id(self, row, value):
         try:
             return self.db.get_id_object(value)
```

### Comparing `autisto-1.1rc3/autisto/utils.py` & `autisto-1.1rc4/autisto/utils.py`

 * *Files identical despite different names*

### Comparing `autisto-1.1rc3/autisto.egg-info/PKG-INFO` & `autisto-1.1rc4/autisto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autisto
-Version: 1.1rc3
+Version: 1.1rc4
 Summary: Basic accounting (?) program integrated with Google Sheets to fulfill my own autistic needs of tracking the shit owned.
 Author: Jan Grzybek
 Author-email: lyre_embassy_0n@icloud.com
 License: MIT
 Project-URL: GitHub, https://github.com/jan-grzybek/autisto
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `autisto-1.1rc3/setup.py` & `autisto-1.1rc4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import setuptools
 
-VERSION = "1.1rc3"
+VERSION = "1.1rc4"
 
 
 def load_readme():
     with open(os.path.join(os.path.dirname(__file__), "README.md")) as f:
         readme = f.read()
     return readme
```

### Comparing `autisto-1.1rc3/tests/test_autisto.py` & `autisto-1.1rc4/tests/test_autisto.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 
 def test_column_titling(spreadsheet):
     print("\nTesting column titling ...")
     sheets_to_titles = {"Console": CONSOLE_COL_NAMES, "Inventory": INVENTORY_COL_NAMES, "Spending": SPENDING_COL_NAMES}
     lock.acquire()
     for sheet, titles in sheets_to_titles.items():
-        start_row = to_1_based(START_ROW) + 1 if sheet == "Inventory" else to_1_based(START_ROW)
+        start_row = to_1_based(START_ROW) + 1 if sheet != "Spending" else to_1_based(START_ROW)
         row_values = spreadsheet.worksheet(sheet).row_values(start_row)[START_COL:]
         for i, col_name in enumerate(titles):
             assert row_values[i] == col_name, f"{row_values[i]} != {col_name}"
     lock.release()
     print("SUCCESS.")
 
 
@@ -105,15 +105,15 @@
             cell_coordinates = cells_to_litter[sheet][i]
             if sheet == "Console":
                 if cell_coordinates.row == 1:
                     assert worksheet.cell(cell_coordinates.row, cell_coordinates.col).value is None
                 elif cell_coordinates.col == 1 or to_1_based(START_COL) + len(
                         CONSOLE_COL_NAMES[:-2]) <= cell_coordinates.col:
                     assert worksheet.cell(cell_coordinates.row, cell_coordinates.col).value is None
-                elif cell_coordinates.row != 2:
+                elif cell_coordinates.row not in [2, 3]:
                     assert worksheet.cell(cell_coordinates.row, cell_coordinates.col).value == litter[i]
             elif sheet == "Inventory":
                 if cell_coordinates.row == 1 or to_1_based(START_ROW) + 2 <= cell_coordinates.row:
                     assert worksheet.cell(cell_coordinates.row, cell_coordinates.col).value is None
                 elif cell_coordinates.col == 1 or \
                         to_1_based(START_COL) + len(INVENTORY_COL_NAMES) <= cell_coordinates.col:
                     assert worksheet.cell(cell_coordinates.row, cell_coordinates.col).value is None
```

