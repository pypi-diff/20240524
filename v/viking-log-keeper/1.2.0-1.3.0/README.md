# Comparing `tmp/viking_log_keeper-1.2.0.tar.gz` & `tmp/viking-log-keeper-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viking_log_keeper-1.2.0.tar", max compression
+gzip compressed data, was "viking-log-keeper-1.3.0.tar", last modified: Thu May 23 22:21:34 2024, max compression
```

## Comparing `viking_log_keeper-1.2.0.tar` & `viking-log-keeper-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,27 @@
--rw-r--r--   0        0        0     1075 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/LICENSE
--rw-r--r--   0        0        0     3000 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/README.md
--rw-r--r--   0        0        0     1326 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/dashboard/__init__.py
--rw-r--r--   0        0        0     7922 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/dashboard/auth.py
--rw-r--r--   0        0        0     7124 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/dashboard/main.py
--rw-r--r--   0        0        0     7385 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/dashboard/plots.py
--rw-r--r--   0        0        0     1290 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/dashboard/utils.py
--rw-r--r--   0        0        0        0 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/log_keeper/__init__.py
--rw-r--r--   0        0        0     5441 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/log_keeper/get_config.py
--rw-r--r--   0        0        0     5113 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/log_keeper/ingest.py
--rw-r--r--   0        0        0     2870 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/log_keeper/main.py
--rw-r--r--   0        0        0     3654 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/log_keeper/output.py
--rw-r--r--   0        0        0     3040 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/log_keeper/utils.py
--rw-r--r--   0        0        0     4237 1970-01-01 00:00:00.000000 viking_log_keeper-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:34.247119 viking-log-keeper-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-23 22:21:34.247119 viking-log-keeper-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:21:34.247119 viking-log-keeper-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:34.243119 viking-log-keeper-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:34.243119 viking-log-keeper-1.3.0/src/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/dashboard/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/dashboard/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/dashboard/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/dashboard/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:34.247119 viking-log-keeper-1.3.0/src/log_keeper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/log_keeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/log_keeper/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/log_keeper/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/log_keeper/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/log_keeper/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-23 22:21:21.000000 viking-log-keeper-1.3.0/src/log_keeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:21:34.247119 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-23 22:21:34.000000 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-23 22:21:34.000000 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:21:34.000000 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-23 22:21:34.000000 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-23 22:21:34.000000 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 22:21:34.000000 viking-log-keeper-1.3.0/src/viking_log_keeper.egg-info/top_level.txt
```

### Comparing `viking_log_keeper-1.2.0/LICENSE` & `viking-log-keeper-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.2.0/README.md` & `viking-log-keeper-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.2.0/src/dashboard/auth.py` & `viking-log-keeper-1.3.0/src/dashboard/auth.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.2.0/src/dashboard/main.py` & `viking-log-keeper-1.3.0/src/dashboard/main.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.2.0/src/dashboard/plots.py` & `viking-log-keeper-1.3.0/src/dashboard/plots.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.2.0/src/dashboard/utils.py` & `viking-log-keeper-1.3.0/src/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.2.0/src/log_keeper/get_config.py` & `viking-log-keeper-1.3.0/src/log_keeper/get_config.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.2.0/src/log_keeper/ingest.py` & `viking-log-keeper-1.3.0/src/log_keeper/ingest.py`

 * *Files 24% similar despite different names*

```diff
@@ -45,17 +45,51 @@
             'Aircraft': 'string',
             'Date': 'datetime64[ns]',
             'P1': 'bool',
             'P2': 'bool'
         }
     )
 
+    # Validate the log sheet. Raise an error if invalid.
+    validate_log_sheet(raw_df)
     return raw_df
 
 
+def validate_log_sheet(log_sheet_df: pd.DataFrame):
+    """
+    Validate the log sheet dataframe.
+
+    Parameters:
+    - log_sheet_df (pandas.DataFrame): The log sheet dataframe to be validated.
+    """
+    # Constants.
+    MAX_FLIGHT_TIME = 240   # [Minutes].
+
+    # Check if the dataframe is empty.
+    if log_sheet_df.empty:
+        raise ValueError("Log sheet is empty.")
+
+    # Check for NaT (not a time).
+    columns_to_check = ['Date', 'TakeOffTime', 'LandingTime']
+    if log_sheet_df[columns_to_check].isna().any().any():
+        raise ValueError("Date or time columns contain NaT values.")
+
+    # Check if the LandingTime is before the TakeOffTime.
+    if (log_sheet_df['LandingTime'] < log_sheet_df['TakeOffTime']).any():
+        raise ValueError("LandingTime is before TakeOffTime.")
+
+    # Check for wild values in the FlightTime column.
+    if log_sheet_df['FlightTime'].max() > MAX_FLIGHT_TIME:
+        raise ValueError("FlightTime column contains huge value.")
+
+    # Check there is an aircraft. Excel defaults to 0 if empty.
+    if (log_sheet_df['Aircraft'] == '0').any():
+        raise ValueError("Aircraft column has no aircraft.")
+
+
 def sanitise_log_sheets(log_sheet_df):
     """
     Filter and replace data in the master log dataframe.
 
     Parameters:
     log_sheet_df (pandas.DataFrame): The master log dataframe to
         be filtered and modified.
@@ -159,10 +193,10 @@
     # Sanitise the log sheets.
     collated_df = sanitise_log_sheets(log_sheet_df)
     return collated_df
 
 
 if __name__ == "__main__":
     # Test the collate function.
-    test_dir_path = "C:\\Users\\Michael.Jennings\\Downloads\\Logs"
+    test_dir_path = "C:\\Users\\mjenn\\Downloads\\Logs"
     test_collated_df = collate_log_sheets(test_dir_path)
     logger.info(test_collated_df.head())
```

### Comparing `viking_log_keeper-1.2.0/src/log_keeper/main.py` & `viking-log-keeper-1.3.0/src/log_keeper/main.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.2.0/src/log_keeper/output.py` & `viking-log-keeper-1.3.0/src/log_keeper/output.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.2.0/src/log_keeper/utils.py` & `viking-log-keeper-1.3.0/src/log_keeper/utils.py`

 * *Files identical despite different names*

