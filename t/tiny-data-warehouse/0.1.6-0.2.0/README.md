# Comparing `tmp/tiny_data_warehouse-0.1.6.tar.gz` & `tmp/tiny_data_warehouse-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_data_warehouse-0.1.6.tar", max compression
+gzip compressed data, was "tiny_data_warehouse-0.2.0.tar", max compression
```

## Comparing `tiny_data_warehouse-0.1.6.tar` & `tiny_data_warehouse-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       55 2024-04-20 14:50:59.621598 tiny_data_warehouse-0.1.6/README.md
--rw-r--r--   0        0        0      546 2024-05-09 11:01:44.089200 tiny_data_warehouse-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       61 2024-04-26 08:58:36.102348 tiny_data_warehouse-0.1.6/tiny_data_warehouse/__init__.py
--rw-r--r--   0        0        0     3831 2024-05-09 11:11:08.330041 tiny_data_warehouse-0.1.6/tiny_data_warehouse/data_warehouse.py
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 tiny_data_warehouse-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-09 11:24:28.526537 tiny_data_warehouse-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0      313 2024-05-09 11:24:09.173912 tiny_data_warehouse-0.2.0/README.md
+-rw-r--r--   0        0        0      607 2024-05-24 05:12:30.274106 tiny_data_warehouse-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-05-19 06:57:03.646927 tiny_data_warehouse-0.2.0/tiny_data_warehouse/__init__.py
+-rw-r--r--   0        0        0     5269 2024-05-24 05:24:57.938126 tiny_data_warehouse-0.2.0/tiny_data_warehouse/data_warehouse.py
+-rw-r--r--   0        0        0      969 1970-01-01 00:00:00.000000 tiny_data_warehouse-0.2.0/PKG-INFO
```

### Comparing `tiny_data_warehouse-0.1.6/pyproject.toml` & `tiny_data_warehouse-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 [tool.poetry]
 name = "tiny-data-warehouse"
-version = "0.1.6"
+version = "0.2.0"
 description = ""
 authors = ["Jean Carlo Machado <jean.machado@getyourguide.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 pandas = "^2.2.1"
 fire = "^0.6.0"
 pypdf2 = "^3.0.1"
+jupyter = "^1.0.0"
+matplotlib = "^3.9.0"
+pyarrow = "^16.1.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.8.0"
 pytest = "^8.0.2"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `tiny_data_warehouse-0.1.6/tiny_data_warehouse/data_warehouse.py` & `tiny_data_warehouse-0.2.0/tiny_data_warehouse/data_warehouse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,64 @@
 import os
 
 from typing import Optional
 import pandas as pd
 
+
 class DataWarehouse:
-    DEFAULT_FOLDER = os.path.join(os.environ['HOME'], '.tinyws')
-    DEFAULT_EVENTS_FOLDER = os.path.join(DEFAULT_FOLDER, 'events')
+    DEFAULT_FOLDER = os.path.join(os.environ["HOME"], ".tinyws")
+    DEFAULT_EVENTS_FOLDER = os.path.join(DEFAULT_FOLDER, "events")
 
     def __init__(self, events_folder: Optional[str] = None, events_config=None) -> None:
         if not events_folder:
             events_folder = DataWarehouse.DEFAULT_EVENTS_FOLDER
 
         if not os.path.exists(events_folder):
             os.makedirs(events_folder)
-            
+
         self.base_folder = DataWarehouse.DEFAULT_FOLDER
         self.events_folder = events_folder
         self.events_config = events_config if events_config else {}
         if events_config:
             print("Events config given: ", events_config)
 
     def list_stored_events(self):
-        os.system("ls -l {}".format(self.events_folder))
+        print("Stored events in folder:  ", self.events_folder)
+        os.system("ls -lh {}".format(self.events_folder))
 
-    def write_event(self, event_name: str, event_data: dict, verbose=False, dry_run=False) -> None:
+    def write_event(
+        self, event_name: str, event_data: dict, verbose=False, dry_run=False
+    ) -> None:
         """
         if event is a dict every key will be a column in the parquet file
 
         Adds a column tdw_timestamp to the event
         """
         self._validate_event_data(event_data)
 
-        event_data['tdw_timestamp'] = pd.Timestamp.now()
+        event_data["tdw_timestamp"] = pd.Timestamp.now()
         df = pd.DataFrame([event_data])
 
         if self._exists_data(event_name):
             existing_data = self.event(event_name)
 
-            if event_name in self.events_config and 'prevent_duplicates_col' in self.events_config[event_name]:
-                check_column_name = self.events_config[event_name]['prevent_duplicates_col']
+            if (
+                event_name in self.events_config
+                and "prevent_duplicates_col" in self.events_config[event_name]
+            ):
+                check_column_name = self.events_config[event_name][
+                    "prevent_duplicates_col"
+                ]
                 possible_duplicated_value = event_data[check_column_name]
 
                 # test if in existing_data there is a duplicated value
                 if possible_duplicated_value in existing_data[check_column_name].values:
-                    raise ValueError(f"A duplicated value {event_data[check_column_name]} for key {check_column_name} was found in the event {event_name}")
+                    raise ValueError(
+                        f"A duplicated value {event_data[check_column_name]} for key {check_column_name} was found in the event {event_name}"
+                    )
 
             df = pd.concat([existing_data, df])
 
         if not dry_run:
             self._write_df(event_name, df)
         else:
             print(f"Event {event_name} written successfully")
@@ -56,48 +67,83 @@
             print(f"Event {event_name} written successfully")
 
     def _write_df(self, event_name, df):
         df.to_parquet(self._parquet_file(event_name))
 
     def _validate_event_data(self, event_data: dict) -> None:
         if type(event_data) != dict:
-            raise ValueError('event must be a dictionary got {}'.format(type(event_data)))
+            raise ValueError(
+                "event must be a dictionary got {}".format(type(event_data))
+            )
 
     def _exists_data(self, event_name: str) -> bool:
         return os.path.exists(self._parquet_file(event_name))
 
     def event(self, event_name: Optional[str]) -> pd.DataFrame:
         """
         Reads the data from the event returned as a pandas DataFrame
         """
         if not os.path.exists(self._parquet_file(event_name)):
-            raise ValueError('Event {} does not exist'.format(event_name))
+            if os.environ.get("TINYWS_CREATE_EMPTY_WHEN_NOT_FOUND"):
+                print(
+                    "Event {} not found, creating an empty one".format(event_name)
+                )
+                return pd.DataFrame()
+
+            raise ValueError("Event {} does not exist".format(event_name))
 
         df = pd.read_parquet(self._parquet_file(event_name))
 
         return df
 
     def replace_df(self, event_name: str, df: pd.DataFrame, dry_run=True) -> None:
         if dry_run:
-            print('Replace of event {}, destructive event! Disable dry run to execute it'.format(event_name))
+            print(
+                "Replace of event {}, destructive event! Disable dry run to execute it".format(
+                    event_name
+                )
+            )
         df.to_parquet(self._parquet_file(event_name))
 
     def remove_event(self, event_name: str, dry_run=True) -> None:
         if dry_run:
-            print('Dry run removal of the the event {}, destructive event! Disable dry run to execute it'.format(event_name))
+            print(
+                "Dry run removal of the the event {}, destructive event! Disable dry run to execute it".format(
+                    event_name
+                )
+            )
 
         os.remove(self._parquet_file(event_name))
 
     def print_event(self, event_name: Optional[str]) -> None:
         print(self.event(event_name))
-    
+
     def _parquet_file(self, event_name):
-        return os.path.join(self.events_folder, event_name + '.parquet')
+        return os.path.join(self.events_folder, event_name + ".parquet")
 
+    def backup_all(self):
+        date_and_time_str = pd.Timestamp.now().strftime("%Y-%m-%d_%H-%M-%S")
+        os.system(f"mkdir -p {self.events_folder}.backup/{date_and_time_str}")
+        os.system(f"cp -r {self.events_folder}/* {self.events_folder}.backup/{date_and_time_str}")
+        print("Backup done in folder: ", f"{self.events_folder}.backup/{date_and_time_str}")
+
+    def backup_restore(self, date_and_time_str, dry_run=True):
+        cmd = f"cp -r {self.events_folder}.backup/{date_and_time_str}/* {self.events_folder}"
+        if dry_run:
+            print(f"Dry run restore of the backup {date_and_time_str}. Disable dry run to execute it")
+            print(cmd)
+            return
+        os.system(cmd)
+        print("Backup restored")
+
+    def backups_list(self):
+        os.system(f"du -hs  {self.events_folder}.backup/*")
 
 
 def main():
     import fire
+
     fire.Fire(DataWarehouse)
 
+
 if __name__ == "__main__":
     main()
```

