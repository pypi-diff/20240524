# Comparing `tmp/samadb-0.2.6.tar.gz` & `tmp/samadb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samadb-0.2.6.tar", last modified: Sun May 14 21:43:40 2023, max compression
+gzip compressed data, was "samadb-0.3.0.tar", last modified: Fri May 24 17:21:40 2024, max compression
```

## Comparing `samadb-0.2.6.tar` & `samadb-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2023-05-14 21:43:40.222530 samadb-0.2.6/
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1075 2023-05-14 21:43:40.222595 samadb-0.2.6/PKG-INFO
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)      460 2023-05-14 18:20:14.000000 samadb-0.2.6/README.md
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)       79 2023-05-14 21:43:40.222844 samadb-0.2.6/setup.cfg
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1758 2023-05-14 21:43:06.000000 samadb-0.2.6/setup.py
-drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2023-05-14 21:43:40.221279 samadb-0.2.6/src/
-drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2023-05-14 21:43:40.222400 samadb-0.2.6/src/samadb.egg-info/
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1075 2023-05-14 21:43:40.000000 samadb-0.2.6/src/samadb.egg-info/PKG-INFO
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)      211 2023-05-14 21:43:40.000000 samadb-0.2.6/src/samadb.egg-info/SOURCES.txt
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)        1 2023-05-14 21:43:40.000000 samadb-0.2.6/src/samadb.egg-info/dependency_links.txt
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)       26 2023-05-14 21:43:40.000000 samadb-0.2.6/src/samadb.egg-info/requires.txt
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)        7 2023-05-14 21:43:40.000000 samadb-0.2.6/src/samadb.egg-info/top_level.txt
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)    25882 2023-05-14 17:09:49.000000 samadb-0.2.6/src/samadb.py
+drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2024-05-24 17:21:40.174661 samadb-0.3.0/
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1156 2024-05-24 17:21:40.174568 samadb-0.3.0/PKG-INFO
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)      460 2023-05-14 18:20:14.000000 samadb-0.3.0/README.md
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)       79 2024-05-24 17:21:40.174895 samadb-0.3.0/setup.cfg
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1866 2024-05-24 17:11:10.000000 samadb-0.3.0/setup.py
+drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2024-05-24 17:21:40.171980 samadb-0.3.0/src/
+drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2024-05-24 17:21:40.172886 samadb-0.3.0/src/samadb/
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)      194 2024-05-24 17:20:11.000000 samadb-0.3.0/src/samadb/__init__.py
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)    26004 2024-05-24 16:56:57.000000 samadb-0.3.0/src/samadb/samadb.py
+drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2024-05-24 17:21:40.174274 samadb-0.3.0/src/samadb.egg-info/
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1156 2024-05-24 17:21:40.000000 samadb-0.3.0/src/samadb.egg-info/PKG-INFO
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)      241 2024-05-24 17:21:40.000000 samadb-0.3.0/src/samadb.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)        1 2024-05-24 17:21:40.000000 samadb-0.3.0/src/samadb.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)       26 2024-05-24 17:21:40.000000 samadb-0.3.0/src/samadb.egg-info/requires.txt
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)        7 2024-05-24 17:21:40.000000 samadb-0.3.0/src/samadb.egg-info/top_level.txt
```

### Comparing `samadb-0.2.6/setup.py` & `samadb-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,39 +7,40 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name='samadb',
-    version='0.2.6',
-    description='An python providing access to a relational database with macroeconomic data for South Africa.',
+    version='0.3.0',
+    description='An API providing access to a relational database with macroeconomic data for South Africa.',
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",
     # url='',
     author="Sebastian Krantz",
     author_email='sebastian.krantz@graduateinstitute.ch',
     # Classifiers help users find your project by categorizing it.
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         # Pick your license as you wish
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate you support Python 3. These classifiers are *not*
         # checked by 'pip install'. See instead 'python_requires' below.
         "Programming Language :: Python :: 3",
     ],
     keywords='south africa, macroeconomic, data, API',
     package_dir={"": "src"},  # Optional
-    py_modules=["samadb"],
+    packages=find_packages(where="src"),  # Automatically discover all packages and subpackages
+    # py_modules=["samadb"],
     python_requires=">=3.1",
     install_requires=['connectorx', 'pyarrow', 'polars'],
     license='GPL-3',
     project_urls={  # Optional
         "Bug Reports": "https://github.com/Stellenbosch-Econometrics/SAMADB-Issues/issues",
     },
 )
```

### Comparing `samadb-0.2.6/src/samadb.py` & `samadb-0.3.0/src/samadb/samadb.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 import polars as _pl
 from datetime import datetime as _datetime, timedelta as _timedelta
 
 SAMADB_ID = ["dsid", "series"]
 
 SAMADB_T = ["date", "year", "quarter", "month", "day"]
 
-__uri__ = "mysql://SAMADB_READ:0c7Wg975vj@102.214.9.99:3306/SAMADB"
+__uri__ = "mysql://SAMADB_READ:0c7Wg975vj@102.214.9.244:3306/SAMADB"
 
 
 
 def datasources(ordered = True):
     """Retrieve Data Sources Table.
     
         This function pulls and returns a table called 'DATASOURCE' from the database. The 'DATASOURCE' table gives 
@@ -59,15 +59,15 @@
 
         Returns:
             A Polars DataFrame providing information about the sources of data in the database.
     """
     query = "SELECT * FROM DATASOURCE"
     if ordered:
         query += " ORDER BY src_order"
-    res = _pl.read_sql(query, __uri__)
+    res = _pl.read_database_uri(query, __uri__)
     if len(res) == 0:
         raise Exception("Query resulted in empty dataset. This means something is wrong with your internet connection, the connection to the database or with the database itself.")
     return res.drop("src_order")
   
   
 def datasets(ordered = True):
     """Retrieve Datasets Table.
@@ -82,15 +82,15 @@
 
         Returns:
             A Polars DataFrame providing information about the available datasets in the database.
     """
     query = "SELECT * FROM DATASET"
     if ordered:
         query += " ORDER BY ds_order"
-    res = _pl.read_sql(query, __uri__)
+    res = _pl.read_database_uri(query, __uri__)
     if len(res) == 0:
         raise Exception("Query resulted in empty dataset. This means something is wrong with your internet connection, the connection to the database or with the database itself.")
     return res.drop("ds_order")
 
 
 def series(dsid = None,
            series = None,
@@ -151,15 +151,15 @@
           
   if ordered:
       query += " ORDER BY s_order"
 
   if return_query:
       return query
     
-  res = _pl.read_sql(query, __uri__)
+  res = _pl.read_database_uri(query, __uri__)
   if len(res) == 0:
       raise Exception("Query resulted in empty dataset. This means something is wrong with your internet connection, the connection to the database or with the database itself.")
   return res.drop("s_order")
 
 
 # dt.strftime(dt.strptime("2011-01-01", "%Y-%m-%d"), "%Y-%m-%d")
 #
@@ -180,16 +180,15 @@
 # print(result_1)
 #
 # x[5:7]
 # strptime("2011-01-01", pl.Date, "%Y-%m-%d")
 
 is_date = lambda x: (type(x) is _datetime.date or
           str(type(x)) in ["<class 'datetime.date'>", "<class 'datetime.datetime'>"] or
-          (str(type(x)) == "<class 'polars.internals.series.series.Series'>" and
-           x.dtype is _pl.datatypes.Date))
+          (isinstance(x, _pl.Series) and x.dtype == _pl.datatypes.Date))
 
         
 
 
 def as_date(x, end = False):
   """Coerce Input to Date-String.
 
@@ -460,23 +459,25 @@
     if d0 and s0 and cond != "":
         cond = cond[5:]
 
     query = "SELECT " + vars + " FROM " + data + where + cond + (" ORDER BY " + ord if ordered else "")
     if return_query:
         return query
 
-    res = _pl.read_sql(query, __uri__)
+    res = _pl.read_database_uri(query, __uri__)
     if len(res) == 0:
         raise Exception("Query resulted in empty dataset. Please make sure that the dsid, series-codes or the date-range supplied in your query are consistent with the available data. See datasets() and series(). Alternatively check your connection to the database.")
     
     # Constructing enhanced label
     if labels:
-        res = res.with_columns((_pl.col("label")  + ' (' + _pl.col("unit") +
+        # https://stackoverflow.com/questions/78062891/polars-how-to-use-pl-when-to-output-a-string-value
+        res = res.with_columns((_pl.col("label") + ' (' + _pl.col("unit") + 
           _pl.when((_pl.col("seas_adj") == 1) & (~_pl.col("label").str.contains(r"(?i)seasonally")))
-            .then(', Seasonally Adjusted)').otherwise(')')).alias("label")).drop(["unit", "seas_adj"])
+             .then(_pl.lit(', Seasonally Adjusted)')).otherwise(_pl.lit(')'))).alias("label")).drop(["unit", "seas_adj"])
+
 
     if wide:
         if labels:
             kwargs["return_labels"] = True
             res, labels_df = pivot_wider(res, **kwargs)
         else:
             res = pivot_wider(res, **kwargs)
@@ -536,24 +537,24 @@
     if type(id_cols) is str and id_cols == "auto":
         id_cols = [c for c in x.columns if c in SAMADB_T]
 
     # Reshape wider
     res = x.pivot(index = id_cols,
                   columns = names_from,
                   values = values_from,
-                  aggregate_fn = 'first',
+                  aggregate_function = 'first',
                   maintain_order = True,
                   sort_columns = False).sort(id_cols)
     
     # Get names and labels
     if return_labels and labels_from in x.columns:
         labels_df = x.select([names_from, labels_from]).unique()
         # Check that columns match labels
-        if not all(labels_df.get_column(names_from) == res.columns[len(id_cols):]):
-            raise Exception("Mismatch of aggregated names")
+        # if not all(labels_df.get_column(names_from) == res.columns[len(id_cols):]):
+        #     raise Exception("Mismatch of aggregated names")
         return (res, labels_df)
     else:
         return res
 
 
 # TODO: what about the row-order of the output ??
 def pivot_longer(x,
```

