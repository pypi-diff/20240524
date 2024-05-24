# Comparing `tmp/krazy-0.22.0.tar.gz` & `tmp/krazy-0.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krazy-0.22.0.tar", last modified: Mon Feb 19 17:33:18 2024, max compression
+gzip compressed data, was "krazy-0.22.1.tar", last modified: Fri May 24 17:10:29 2024, max compression
```

## Comparing `krazy-0.22.0.tar` & `krazy-0.22.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 kartik     (502) staff       (20)        0 2024-02-19 17:33:18.735726 krazy-0.22.0/
--rw-rw-r--   0 kartik     (502) staff       (20)     1091 2022-09-16 19:14:22.000000 krazy-0.22.0/LICENSE
--rw-r--r--   0 kartik     (502) staff       (20)     2085 2024-02-19 17:33:18.734820 krazy-0.22.0/PKG-INFO
--rw-rw-r--   0 kartik     (502) staff       (20)     1361 2022-09-16 19:14:22.000000 krazy-0.22.0/README.md
-drwxr-xr-x   0 kartik     (502) staff       (20)        0 2024-02-19 17:33:18.728882 krazy-0.22.0/krazy/
-drwxr-xr-x   0 kartik     (502) staff       (20)        0 2024-02-19 17:33:18.731969 krazy-0.22.0/krazy/krazy/
--rw-rw-r--   0 kartik     (502) staff       (20)        0 2022-09-16 19:14:22.000000 krazy-0.22.0/krazy/krazy/__init__.py
--rw-rw-r--   0 kartik     (502) staff       (20)     6550 2024-02-19 17:15:08.000000 krazy-0.22.0/krazy/krazy/data_science.py
--rw-rw-r--   0 kartik     (502) staff       (20)    10182 2022-09-16 19:14:22.000000 krazy-0.22.0/krazy/krazy/frontend_tkinter_ready.py
--rw-rw-r--   0 kartik     (502) staff       (20)     3382 2022-09-16 19:14:22.000000 krazy-0.22.0/krazy/krazy/gsheet_initialize.py
--rw-rw-r--   0 kartik     (502) staff       (20)     6704 2024-02-19 17:27:38.000000 krazy-0.22.0/krazy/krazy/sql_utilities.py
--rw-rw-r--   0 kartik     (502) staff       (20)     2237 2022-12-07 15:43:50.000000 krazy-0.22.0/krazy/krazy/sqlite_utilities.py
--rw-rw-r--   0 kartik     (502) staff       (20)    35424 2024-02-19 17:24:19.000000 krazy-0.22.0/krazy/krazy/utility_functions.py
-drwxr-xr-x   0 kartik     (502) staff       (20)        0 2024-02-19 17:33:18.734285 krazy-0.22.0/krazy/krazy.egg-info/
--rw-r--r--   0 kartik     (502) staff       (20)     2085 2024-02-19 17:33:18.000000 krazy-0.22.0/krazy/krazy.egg-info/PKG-INFO
--rw-r--r--   0 kartik     (502) staff       (20)      417 2024-02-19 17:33:18.000000 krazy-0.22.0/krazy/krazy.egg-info/SOURCES.txt
--rw-r--r--   0 kartik     (502) staff       (20)        1 2024-02-19 17:33:18.000000 krazy-0.22.0/krazy/krazy.egg-info/dependency_links.txt
--rw-r--r--   0 kartik     (502) staff       (20)      101 2024-02-19 17:33:18.000000 krazy-0.22.0/krazy/krazy.egg-info/requires.txt
--rw-r--r--   0 kartik     (502) staff       (20)        6 2024-02-19 17:33:18.000000 krazy-0.22.0/krazy/krazy.egg-info/top_level.txt
--rw-r--r--   0 kartik     (502) staff       (20)       38 2024-02-19 17:33:18.735801 krazy-0.22.0/setup.cfg
--rw-rw-r--   0 kartik     (502) staff       (20)     1102 2024-02-19 17:14:11.000000 krazy-0.22.0/setup.py
+drwxr-xr-x   0 kartik     (502) staff       (20)        0 2024-05-24 17:10:29.788290 krazy-0.22.1/
+-rw-rw-r--   0 kartik     (502) staff       (20)     1091 2022-09-16 19:14:22.000000 krazy-0.22.1/LICENSE
+-rw-r--r--   0 kartik     (502) staff       (20)      997 2024-05-24 17:10:29.787989 krazy-0.22.1/PKG-INFO
+-rw-rw-r--   0 kartik     (502) staff       (20)      250 2024-03-23 14:19:04.000000 krazy-0.22.1/README.md
+drwxr-xr-x   0 kartik     (502) staff       (20)        0 2024-05-24 17:10:29.781419 krazy-0.22.1/krazy/
+drwxr-xr-x   0 kartik     (502) staff       (20)        0 2024-05-24 17:10:29.785565 krazy-0.22.1/krazy/krazy/
+-rw-rw-r--   0 kartik     (502) staff       (20)        0 2022-09-16 19:14:22.000000 krazy-0.22.1/krazy/krazy/__init__.py
+-rw-rw-r--   0 kartik     (502) staff       (20)     6550 2024-02-19 17:15:08.000000 krazy-0.22.1/krazy/krazy/data_science.py
+-rw-rw-r--   0 kartik     (502) staff       (20)    10182 2022-09-16 19:14:22.000000 krazy-0.22.1/krazy/krazy/frontend_tkinter_ready.py
+-rw-rw-r--   0 kartik     (502) staff       (20)     3382 2022-09-16 19:14:22.000000 krazy-0.22.1/krazy/krazy/gsheet_initialize.py
+-rw-r--r--   0 kartik     (502) staff       (20)     6238 2024-03-23 14:20:05.000000 krazy-0.22.1/krazy/krazy/reconciler.py
+-rw-rw-r--   0 kartik     (502) staff       (20)     6704 2024-02-19 17:27:38.000000 krazy-0.22.1/krazy/krazy/sql_utilities.py
+-rw-rw-r--   0 kartik     (502) staff       (20)     2237 2022-12-07 15:43:50.000000 krazy-0.22.1/krazy/krazy/sqlite_utilities.py
+-rw-rw-r--   0 kartik     (502) staff       (20)    36042 2024-03-03 13:48:28.000000 krazy-0.22.1/krazy/krazy/utility_functions.py
+drwxr-xr-x   0 kartik     (502) staff       (20)        0 2024-05-24 17:10:29.787632 krazy-0.22.1/krazy/krazy.egg-info/
+-rw-r--r--   0 kartik     (502) staff       (20)      997 2024-05-24 17:10:29.000000 krazy-0.22.1/krazy/krazy.egg-info/PKG-INFO
+-rw-r--r--   0 kartik     (502) staff       (20)      443 2024-05-24 17:10:29.000000 krazy-0.22.1/krazy/krazy.egg-info/SOURCES.txt
+-rw-r--r--   0 kartik     (502) staff       (20)        1 2024-05-24 17:10:29.000000 krazy-0.22.1/krazy/krazy.egg-info/dependency_links.txt
+-rw-r--r--   0 kartik     (502) staff       (20)      101 2024-05-24 17:10:29.000000 krazy-0.22.1/krazy/krazy.egg-info/requires.txt
+-rw-r--r--   0 kartik     (502) staff       (20)        6 2024-05-24 17:10:29.000000 krazy-0.22.1/krazy/krazy.egg-info/top_level.txt
+-rw-r--r--   0 kartik     (502) staff       (20)       38 2024-05-24 17:10:29.788334 krazy-0.22.1/setup.cfg
+-rw-rw-r--   0 kartik     (502) staff       (20)     1102 2024-03-23 14:19:15.000000 krazy-0.22.1/setup.py
```

### Comparing `krazy-0.22.0/LICENSE` & `krazy-0.22.1/LICENSE`

 * *Files identical despite different names*

### Comparing `krazy-0.22.0/krazy/krazy/data_science.py` & `krazy-0.22.1/krazy/krazy/data_science.py`

 * *Files identical despite different names*

### Comparing `krazy-0.22.0/krazy/krazy/frontend_tkinter_ready.py` & `krazy-0.22.1/krazy/krazy/frontend_tkinter_ready.py`

 * *Files identical despite different names*

### Comparing `krazy-0.22.0/krazy/krazy/gsheet_initialize.py` & `krazy-0.22.1/krazy/krazy/gsheet_initialize.py`

 * *Files identical despite different names*

### Comparing `krazy-0.22.0/krazy/krazy/sql_utilities.py` & `krazy-0.22.1/krazy/krazy/sql_utilities.py`

 * *Files identical despite different names*

### Comparing `krazy-0.22.0/krazy/krazy/sqlite_utilities.py` & `krazy-0.22.1/krazy/krazy/sqlite_utilities.py`

 * *Files identical despite different names*

### Comparing `krazy-0.22.0/krazy/krazy/utility_functions.py` & `krazy-0.22.1/krazy/krazy/utility_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,31 @@
                     dfs.append(pd.read_csv(filename,low_memory=False))
                 else:
                     dfs.append(pd.read_csv(filename,dtype=types))
     # Concatenate all data into one DataFrame
     dfjoined = pd.concat(dfs, ignore_index=True)
     return dfjoined
 
+def df_multi_csv_excel_importer(folder: Path)->list[pd.DataFrame,list]:
+    df = pd.DataFrame()
+    files_skipped = []
+
+    for file in os.listdir(folder):
+        file_path = folder.joinpath(file)
+        if file_path.suffix.lower() == '.csv':
+            df_temp = pd.read_csv(folder.joinpath(file))
+            df = pd.concat([df, df_temp], axis=0)
+        elif file_path.suffix.lower() == '.xlsx':
+            df_temp = pd.read_excel(folder.joinpath(file))
+            df = pd.concat([df, df_temp], axis=0)
+        else:
+            files_skipped.append(file)
+    
+    return [df, files_skipped]
+
 def df_to_sql(dfdata,table,colList,connection):
     # this inserts data from dataframe into database table
     # for this to work, columns and column sequence should be exactly in same manner as in database
     cur = connection.cursor()
     imFile = StringIO()
     dfdata.to_csv(imFile, index=False)
     imFile.seek(0)
```

### Comparing `krazy-0.22.0/setup.py` & `krazy-0.22.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="krazy",
-    version="0.22.0",
+    version="0.22.1",
     author="Kartik",
     author_email="kartik@live.com",
     description="My own small package of uitilities I use.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kartikjain11/krazy",
     project_urls={
```

