# Comparing `tmp/nodeocc-1.0.8.tar.gz` & `tmp/nodeocc-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodeocc-1.0.8.tar", last modified: Tue Mar 12 22:17:38 2024, max compression
+gzip compressed data, was "nodeocc-1.0.9.tar", last modified: Fri May 24 08:42:14 2024, max compression
```

## Comparing `nodeocc-1.0.8.tar` & `nodeocc-1.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-03-12 22:17:38.235540 nodeocc-1.0.8/
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     1402 2024-03-12 22:17:38.231540 nodeocc-1.0.8/PKG-INFO
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)      804 2024-02-15 15:41:39.000000 nodeocc-1.0.8/README.md
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)      857 2024-03-12 22:17:06.000000 nodeocc-1.0.8/pyproject.toml
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)       38 2024-03-12 22:17:38.235540 nodeocc-1.0.8/setup.cfg
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)       38 2024-02-15 15:41:39.000000 nodeocc-1.0.8/setup.py
-drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-03-12 22:17:38.195541 nodeocc-1.0.8/src/
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)       17 2024-02-15 15:41:39.000000 nodeocc-1.0.8/src/__init__.py
-drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-03-12 22:17:38.195541 nodeocc-1.0.8/src/controller/
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)    11302 2024-03-12 16:34:59.000000 nodeocc-1.0.8/src/controller/controller.py
-drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-03-12 22:17:38.199541 nodeocc-1.0.8/src/model/
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     3407 2024-03-12 22:02:39.000000 nodeocc-1.0.8/src/model/infrastructure.py
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     2482 2024-02-15 15:41:39.000000 nodeocc-1.0.8/src/model/job.py
-drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-03-12 22:17:38.231540 nodeocc-1.0.8/src/nodeocc.egg-info/
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     1402 2024-03-12 22:17:38.000000 nodeocc-1.0.8/src/nodeocc.egg-info/PKG-INFO
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)      529 2024-03-12 22:17:38.000000 nodeocc-1.0.8/src/nodeocc.egg-info/SOURCES.txt
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)        1 2024-03-12 22:17:38.000000 nodeocc-1.0.8/src/nodeocc.egg-info/dependency_links.txt
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)       56 2024-03-12 22:17:38.000000 nodeocc-1.0.8/src/nodeocc.egg-info/entry_points.txt
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)       13 2024-03-12 22:17:38.000000 nodeocc-1.0.8/src/nodeocc.egg-info/requires.txt
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)       39 2024-03-12 22:17:38.000000 nodeocc-1.0.8/src/nodeocc.egg-info/top_level.txt
-drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-03-12 22:17:38.215540 nodeocc-1.0.8/src/readers/
--rwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)      804 2024-02-15 15:41:39.000000 nodeocc-1.0.8/src/readers/compute_wait_time.py
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)    13698 2024-03-12 17:41:21.000000 nodeocc-1.0.8/src/readers/slurmreader.py
-drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-03-12 22:17:38.227540 nodeocc-1.0.8/src/view/
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)      697 2024-03-12 21:56:28.000000 nodeocc-1.0.8/src/view/__init__.py
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)    23501 2024-03-11 23:05:45.000000 nodeocc-1.0.8/src/view/curses_multiwindow.py
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     5684 2024-03-11 23:01:56.000000 nodeocc-1.0.8/src/view/slurm_list.py
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)    28943 2024-03-12 22:12:44.000000 nodeocc-1.0.8/src/view/slurm_viz.py
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     2812 2024-02-15 15:41:39.000000 nodeocc-1.0.8/src/view/styles.py
--rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     1834 2024-02-15 15:41:39.000000 nodeocc-1.0.8/src/view/utils.py
+drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-05-24 08:42:14.012946 nodeocc-1.0.9/
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     1402 2024-05-24 08:42:14.008946 nodeocc-1.0.9/PKG-INFO
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)      804 2024-02-15 15:41:39.000000 nodeocc-1.0.9/README.md
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)      857 2024-05-24 08:41:54.000000 nodeocc-1.0.9/pyproject.toml
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)       38 2024-05-24 08:42:14.012946 nodeocc-1.0.9/setup.cfg
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)       38 2024-02-15 15:41:39.000000 nodeocc-1.0.9/setup.py
+drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-05-24 08:42:13.976947 nodeocc-1.0.9/src/
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)       17 2024-02-15 15:41:39.000000 nodeocc-1.0.9/src/__init__.py
+drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-05-24 08:42:13.976947 nodeocc-1.0.9/src/controller/
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)    11302 2024-03-12 16:34:59.000000 nodeocc-1.0.9/src/controller/controller.py
+drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-05-24 08:42:13.980947 nodeocc-1.0.9/src/model/
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     3407 2024-03-12 22:02:39.000000 nodeocc-1.0.9/src/model/infrastructure.py
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     2482 2024-02-15 15:41:39.000000 nodeocc-1.0.9/src/model/job.py
+drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-05-24 08:42:14.008946 nodeocc-1.0.9/src/nodeocc.egg-info/
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     1402 2024-05-24 08:42:13.000000 nodeocc-1.0.9/src/nodeocc.egg-info/PKG-INFO
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)      529 2024-05-24 08:42:13.000000 nodeocc-1.0.9/src/nodeocc.egg-info/SOURCES.txt
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)        1 2024-05-24 08:42:13.000000 nodeocc-1.0.9/src/nodeocc.egg-info/dependency_links.txt
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)       56 2024-05-24 08:42:13.000000 nodeocc-1.0.9/src/nodeocc.egg-info/entry_points.txt
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)       13 2024-05-24 08:42:13.000000 nodeocc-1.0.9/src/nodeocc.egg-info/requires.txt
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)       39 2024-05-24 08:42:13.000000 nodeocc-1.0.9/src/nodeocc.egg-info/top_level.txt
+drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-05-24 08:42:13.992946 nodeocc-1.0.9/src/readers/
+-rwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)      804 2024-02-15 15:41:39.000000 nodeocc-1.0.9/src/readers/compute_wait_time.py
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)    13892 2024-05-24 08:24:41.000000 nodeocc-1.0.9/src/readers/slurmreader.py
+drwxr-xr-x   0 lbonicelli (47182) dottorandi   (502)        0 2024-05-24 08:42:14.004946 nodeocc-1.0.9/src/view/
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)      697 2024-03-12 21:56:28.000000 nodeocc-1.0.9/src/view/__init__.py
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)    23501 2024-03-11 23:05:45.000000 nodeocc-1.0.9/src/view/curses_multiwindow.py
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     5684 2024-03-11 23:01:56.000000 nodeocc-1.0.9/src/view/slurm_list.py
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)    28943 2024-03-12 22:12:44.000000 nodeocc-1.0.9/src/view/slurm_viz.py
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     2812 2024-02-15 15:41:39.000000 nodeocc-1.0.9/src/view/styles.py
+-rw-r--r--   0 lbonicelli (47182) dottorandi   (502)     1914 2024-05-24 08:37:41.000000 nodeocc-1.0.9/src/view/utils.py
```

### Comparing `nodeocc-1.0.8/PKG-INFO` & `nodeocc-1.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodeocc
-Version: 1.0.8
+Version: 1.0.9
 Summary: TUI application for viewing the status of GPU allocations on a Slurm cluster
 Author: Matteo Boschini
 Maintainer: Lorenzo Bonicelli, Aniello Panariello
 License: MIT
 Project-URL: Repository, https://github.com/apanariello4/slurm_nodeocc
 Keywords: Slurm,GPU,TUI,CLI,HPC,cluster,allocations,nodeocc
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nodeocc-1.0.8/README.md` & `nodeocc-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nodeocc-1.0.8/pyproject.toml` & `nodeocc-1.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nodeocc"
-version = "1.0.8"
+version = "1.0.9"
 authors = [{ name = "Matteo Boschini" }]
 maintainers = [{ name = "Lorenzo Bonicelli" }, { name = "Aniello Panariello" }]
 description = "TUI application for viewing the status of GPU allocations on a Slurm cluster"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
     "Slurm",
```

### Comparing `nodeocc-1.0.8/src/controller/controller.py` & `nodeocc-1.0.9/src/controller/controller.py`

 * *Files identical despite different names*

### Comparing `nodeocc-1.0.8/src/model/infrastructure.py` & `nodeocc-1.0.9/src/model/infrastructure.py`

 * *Files identical despite different names*

### Comparing `nodeocc-1.0.8/src/model/job.py` & `nodeocc-1.0.9/src/model/job.py`

 * *Files identical despite different names*

### Comparing `nodeocc-1.0.8/src/nodeocc.egg-info/PKG-INFO` & `nodeocc-1.0.9/src/nodeocc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodeocc
-Version: 1.0.8
+Version: 1.0.9
 Summary: TUI application for viewing the status of GPU allocations on a Slurm cluster
 Author: Matteo Boschini
 Maintainer: Lorenzo Bonicelli, Aniello Panariello
 License: MIT
 Project-URL: Repository, https://github.com/apanariello4/slurm_nodeocc
 Keywords: Slurm,GPU,TUI,CLI,HPC,cluster,allocations,nodeocc
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nodeocc-1.0.8/src/nodeocc.egg-info/SOURCES.txt` & `nodeocc-1.0.9/src/nodeocc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nodeocc-1.0.8/src/readers/compute_wait_time.py` & `nodeocc-1.0.9/src/readers/compute_wait_time.py`

 * *Files identical despite different names*

### Comparing `nodeocc-1.0.8/src/readers/slurmreader.py` & `nodeocc-1.0.9/src/readers/slurmreader.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,16 +81,18 @@
 def _read_maintenances():
     # create dataframe
     reservations = os.popen(r'scontrol show reservation 2>/dev/null').read().split('\n\n')
     reservations = [{c.split('=')[0]: c.split('=')[1] for c in r.split()} for r in reservations if len(r) and '=' in r]
     if not len(reservations):
         return [], None, None
     reservations = pd.DataFrame.from_records(reservations)
-    reservations['StartTime'] = str(pd.to_datetime(reservations['StartTime']))
-    reservations['EndTime'] = str(pd.to_datetime(reservations['EndTime']))
+    reservations['StartTime'] = reservations['StartTime'].apply(lambda x:str(pd.to_datetime(x)))
+    reservations['EndTime'] = reservations['EndTime'].apply(lambda x:str(pd.to_datetime(x)))
+    # reservations['StartTime'] = str(pd.to_datetime(reservations['StartTime']))
+    # reservations['EndTime'] = str(pd.to_datetime(reservations['EndTime']))
     reservations = _split_column(reservations, 'Nodes')
     maint_flag = reservations['Flags'].str.contains('MAINT') & \
         reservations['Flags'].str.contains('SPEC_NODES') & \
         reservations['Flags'].str.contains('ALL_NODES')
     # | reservations['ReservationName'].str.contains('limit_temp')
 
     maintenances = _maint_from_reservations(reservations[maint_flag])
```

### Comparing `nodeocc-1.0.8/src/view/__init__.py` & `nodeocc-1.0.9/src/view/__init__.py`

 * *Files identical despite different names*

### Comparing `nodeocc-1.0.8/src/view/curses_multiwindow.py` & `nodeocc-1.0.9/src/view/curses_multiwindow.py`

 * *Files identical despite different names*

### Comparing `nodeocc-1.0.8/src/view/slurm_list.py` & `nodeocc-1.0.9/src/view/slurm_list.py`

 * *Files identical despite different names*

### Comparing `nodeocc-1.0.8/src/view/slurm_viz.py` & `nodeocc-1.0.9/src/view/slurm_viz.py`

 * *Files identical despite different names*

### Comparing `nodeocc-1.0.8/src/view/styles.py` & `nodeocc-1.0.9/src/view/styles.py`

 * *Files identical despite different names*

### Comparing `nodeocc-1.0.8/src/view/utils.py` & `nodeocc-1.0.9/src/view/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,20 @@
     return job.partition == 'all_usr_prod'
 
 
 def to_datetime(time_str):
     return np.datetime64(re.match(r'\d+\s+(.*)\n', str(time_str)).group(1))
 
 
-def to_datetime(time_str):
-    return np.datetime64(re.match(r'\d+\s+(.*)\n', str(time_str)).group(1))
+def to_datetime(time_str): 
+    try:
+        dt = np.datetime64(re.match(r'\d+\s+(.*)\n', str(time_str)).group(1))
+    except:
+        dt = np.datetime64(str(time_str))
+    return dt
 
 
 def maintenance_status(infrastructure):
     onmain = False
     waitString = ''
     if len(infrastructure.maintenances):
         # time format: '0   2023-12-04 14:00:00\nName: StartTime, dtype: datetime64[ns]'
```

