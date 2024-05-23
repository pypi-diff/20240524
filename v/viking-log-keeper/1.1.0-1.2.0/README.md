# Comparing `tmp/viking_log_keeper-1.1.0.tar.gz` & `tmp/viking_log_keeper-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viking_log_keeper-1.1.0.tar", max compression
+gzip compressed data, was "viking_log_keeper-1.2.0.tar", max compression
```

## Comparing `viking_log_keeper-1.1.0.tar` & `viking_log_keeper-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     3000 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/README.md
--rw-r--r--   0        0        0     1309 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/dashboard/__init__.py
--rw-r--r--   0        0        0     7922 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/dashboard/auth.py
--rw-r--r--   0        0        0     7124 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/dashboard/main.py
--rw-r--r--   0        0        0     7385 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/dashboard/plots.py
--rw-r--r--   0        0        0     1290 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/dashboard/utils.py
--rw-r--r--   0        0        0        0 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/log_keeper/__init__.py
--rw-r--r--   0        0        0     5441 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/log_keeper/get_config.py
--rw-r--r--   0        0        0     5000 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/log_keeper/ingest.py
--rw-r--r--   0        0        0     2739 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/log_keeper/main.py
--rw-r--r--   0        0        0     3805 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/log_keeper/output.py
--rw-r--r--   0        0        0     3040 2024-05-18 08:24:21.619343 viking_log_keeper-1.1.0/src/log_keeper/utils.py
--rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 viking_log_keeper-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3000 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/README.md
+-rw-r--r--   0        0        0     1326 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/dashboard/__init__.py
+-rw-r--r--   0        0        0     7922 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/dashboard/auth.py
+-rw-r--r--   0        0        0     7124 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/dashboard/main.py
+-rw-r--r--   0        0        0     7385 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/dashboard/plots.py
+-rw-r--r--   0        0        0     1290 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/dashboard/utils.py
+-rw-r--r--   0        0        0        0 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/log_keeper/__init__.py
+-rw-r--r--   0        0        0     5441 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/log_keeper/get_config.py
+-rw-r--r--   0        0        0     5113 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/log_keeper/ingest.py
+-rw-r--r--   0        0        0     2870 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/log_keeper/main.py
+-rw-r--r--   0        0        0     3654 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/log_keeper/output.py
+-rw-r--r--   0        0        0     3040 2024-05-23 12:23:00.036087 viking_log_keeper-1.2.0/src/log_keeper/utils.py
+-rw-r--r--   0        0        0     4237 1970-01-01 00:00:00.000000 viking_log_keeper-1.2.0/PKG-INFO
```

### Comparing `viking_log_keeper-1.1.0/README.md` & `viking_log_keeper-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.1.0/pyproject.toml` & `viking_log_keeper-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "viking-log-keeper"
-version = "1.1.0"
+version = "1.2.0"
 description = "661 VGS - Function to collate 2965D log sheets into a master log, database, and dashboard."
 authors = ["Michael Jennings <mjennings061@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -22,14 +22,15 @@
 logging = "^0.4.9.6"
 matplotlib = "^3.8.0"
 openpyxl = "^3.1.2"
 python = ">=3.10,<4.0"
 pandas = "^2.2.0"
 pymongo = {extras = ["srv"], version = "^4.6.1"}
 streamlit = "^1.32.0"
+tqdm = "^4.66.0"
 xlsxwriter = "^3.2.0"
 
 [tool.poetry.urls]
 homepage = "https://github.com/mjennings061/viking-log-keeper"
 repository = "https://github.com/mjennings061/viking-log-keeper.git"
 
 [tool.poetry.scripts]
```

### Comparing `viking_log_keeper-1.1.0/src/dashboard/auth.py` & `viking_log_keeper-1.2.0/src/dashboard/auth.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.1.0/src/dashboard/main.py` & `viking_log_keeper-1.2.0/src/dashboard/main.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.1.0/src/dashboard/plots.py` & `viking_log_keeper-1.2.0/src/dashboard/plots.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.1.0/src/dashboard/utils.py` & `viking_log_keeper-1.2.0/src/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.1.0/src/log_keeper/get_config.py` & `viking_log_keeper-1.2.0/src/log_keeper/get_config.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.1.0/src/log_keeper/ingest.py` & `viking_log_keeper-1.2.0/src/log_keeper/ingest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 """ingest.py
 
 This file handles log sheet extraction and sanitisation.
 """
 
-import sys
+# Get packages.
 import logging
+from typing import Union
+from pathlib import Path
 import pandas as pd
+from tqdm import tqdm
 
+# Set up logging.
+logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 def ingest_log_sheet(file_path: str) -> pd.DataFrame:
     """
     Extract data from an excel log sheet.
     Output a pandas dataframe.
@@ -96,15 +101,15 @@
 
     # Rename 2ndPilot to SecondPilot.
     log_sheet_df.rename(columns={"2ndPilot": "SecondPilot"}, inplace=True)
 
     return log_sheet_df
 
 
-def collate_log_sheets(dir_path):
+def collate_log_sheets(dir_path: Union[str, Path]) -> pd.DataFrame:
     """
     Collate all log sheets into a single dataframe
     using the path to the log sheet directory.
 
     Args:
         dir_path (str): The path to the log sheet directory.
 
@@ -112,51 +117,52 @@
         pandas.DataFrame: The collated dataframe containing data
             from all log sheets.
 
     Raises:
         FileNotFoundError: If no log sheets are found in the
             specified directory.
     """
+    # Convert to Path object.
+    dir_path = Path(dir_path)
+
     # Get the directory contents.
     FILE_NAME = "2965D_*.xlsx"
     dir_contents = dir_path.glob(f"{FILE_NAME}")
     log_sheet_files = [x for x in dir_contents if x.is_file()]
 
     # Check if list is empty.
     if not log_sheet_files:
         raise FileNotFoundError(f"No log sheets found in \n{dir_path}")
 
     # Log the number of log sheets found.
-    n_files = len(log_sheet_files)
-    logger.info("Found %d log sheets.", n_files)
+    logger.info("Found %d log sheets.", len(log_sheet_files))
 
     # Extract data from each log sheet.
-    log_sheet_df = pd.DataFrame()
-    for i_file, file_path in enumerate(log_sheet_files, start=1):
+    log_sheet_list = []
+    for file_path in tqdm(log_sheet_files,
+                          desc="Processing log sheets",
+                          unit="file"):
         # Get the log sheet data.
-        sys.stdout.write(f"\rProcessing file {i_file}/{n_files}")
-        sys.stdout.flush()
         try:
-            this_sheet_df = ingest_log_sheet(file_path)
             # TODO: Write a function to also ingest the launches
             # and hours CF for F724 if given.
-            if i_file == 1:
-                # Create a new dataframe based on the first file ingest.
-                log_sheet_df = this_sheet_df
-            else:
-                # Append to the master dataframe.
-                log_sheet_df = pd.concat(
-                    [log_sheet_df, this_sheet_df],
-                    ignore_index=True
-                )
+            this_sheet_df = ingest_log_sheet(file_path)
+            log_sheet_list.append(this_sheet_df)
         except Exception:   # pylint: disable=broad-except
             if file_path.name != "2965D_YYMMDD_ZEXXX.xlsx":
-                logger.warning("\n\nLog sheet invalid: %s\n\n",
-                               file_path.name,
-                               exc_info=True)
+                warning_msg = f"Log sheet invalid: {file_path.name}"
+                tqdm.write(warning_msg)
 
-    sys.stdout.write("\nDone processing files.\n")
-    sys.stdout.flush()
+    # Concatenate the log sheets.
+    log_sheet_df = pd.concat(log_sheet_list, ignore_index=True)
+    logger.info("Done importing log sheets.")
 
     # Sanitise the log sheets.
     collated_df = sanitise_log_sheets(log_sheet_df)
     return collated_df
+
+
+if __name__ == "__main__":
+    # Test the collate function.
+    test_dir_path = "C:\\Users\\Michael.Jennings\\Downloads\\Logs"
+    test_collated_df = collate_log_sheets(test_dir_path)
+    logger.info(test_collated_df.head())
```

### Comparing `viking_log_keeper-1.1.0/src/log_keeper/main.py` & `viking_log_keeper-1.2.0/src/log_keeper/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,18 @@
     # Master log file path.
     master_log_filepath = Path(
         log_sheets_dir,
         "Master Log.xlsx"
     )
 
     # Save the launches to excel.
-    launches_to_excel(launches_df, master_log_filepath)
+    try:
+        launches_to_excel(launches_df, master_log_filepath)
+    except Exception:  # pylint: disable=broad-except
+        logger.warning("Could not save Master Log excel file.")
 
     # Save the master log to MongoDB Atlas.
     try:
         launches_to_db(launches_df, db_config)
     except Exception as e:  # pylint: disable=broad-except
         # Filter a ConnectionError.
         if isinstance(e, ConnectionError):
```

### Comparing `viking_log_keeper-1.1.0/src/log_keeper/output.py` & `viking_log_keeper-1.2.0/src/log_keeper/output.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 This file handles outputting the master log to excel and MongoDB Atlas.
 """
 
 import logging
 from pathlib import Path
 import pandas as pd
 from datetime import datetime
-from pymongo.mongo_client import MongoClient
-from pymongo.server_api import ServerApi
 
+# Set up logging.
+logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 def launches_to_excel(launches_df, output_file_path):
     """Save the master log dataframe to an excel table."""
 
     # Sheet the table should be inserted into.
@@ -21,15 +21,17 @@
 
     # Create the excel file and table.
     try:
         writer = pd.ExcelWriter(output_file_path, engine='xlsxwriter')
     except Exception:
         # Writing to MASTER_LOG didn't work. We will need to create a temp
         # file to copy and paste.
-        logger.error("Could not write to MASTER_LOG.xlsx. ", exc_info=True)
+        logger.warning(
+            "Could not write to MASTER_LOG.xlsx. Saving to temp file."
+        )
         # Get new path using todays date.
         date = datetime.today().strftime('%y%m%d')
         output_file_path = output_file_path.with_suffix('')
         output_file_path = Path(str(output_file_path) + '-' + date + '.xlsx')
         logger.info("Writing to %s", output_file_path.name)
         writer = pd.ExcelWriter(output_file_path, engine='xlsxwriter')
 
@@ -74,19 +76,15 @@
     # Print success message.
     logger.info("Saved to %s", output_file_path.name)
 
 
 def launches_to_db(launches_df, db_config):
     """Save the master log dataframe to a MongoDB."""
     # Get environment variables.
-    db_hostname = db_config.db_hostname
-    db_username = db_config.db_username
-    db_password = db_config.db_password
     db_collection_name = db_config.db_collection_name
-    db_name = db_config.db_name
 
     # Format dataframe to be saved.
     master_dict = launches_df.to_dict('records')
     client = db_config.connect_to_db()
     db = client[db_config.db_name]
 
     # Get all collections in the DB.
```

### Comparing `viking_log_keeper-1.1.0/src/log_keeper/utils.py` & `viking_log_keeper-1.2.0/src/log_keeper/utils.py`

 * *Files identical despite different names*

### Comparing `viking_log_keeper-1.1.0/PKG-INFO` & `viking_log_keeper-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viking-log-keeper
-Version: 1.1.0
+Version: 1.2.0
 Summary: 661 VGS - Function to collate 2965D log sheets into a master log, database, and dashboard.
 License: MIT
 Author: Michael Jennings
 Author-email: mjennings061@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,15 @@
 Requires-Dist: keyring (>=24.3.0,<25.0.0)
 Requires-Dist: logging (>=0.4.9.6,<0.5.0.0)
 Requires-Dist: matplotlib (>=3.8.0,<4.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pymongo[srv] (>=4.6.1,<5.0.0)
 Requires-Dist: streamlit (>=1.32.0,<2.0.0)
+Requires-Dist: tqdm (>=4.66.0,<5.0.0)
 Requires-Dist: xlsxwriter (>=3.2.0,<4.0.0)
 Project-URL: homepage, https://github.com/mjennings061/viking-log-keeper
 Project-URL: repository, https://github.com/mjennings061/viking-log-keeper.git
 Description-Content-Type: text/markdown
 
 # Log Keeper
 661 VGS - All-in-one log keeper for the Viking fleet. Records launches from 2965D log sheets, uploads to MongoDB Atlas, and provides a web interface for viewing statistics.
```

