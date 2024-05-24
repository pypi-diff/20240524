# Comparing `tmp/enzope-0.0.8.tar.gz` & `tmp/enzope-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enzope-0.0.8.tar", last modified: Wed Dec  6 18:14:21 2023, max compression
+gzip compressed data, was "enzope-0.0.9.tar", last modified: Wed Dec  6 20:06:13 2023, max compression
```

## Comparing `enzope-0.0.8.tar` & `enzope-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 18:14:21.154510 enzope-0.0.8/
--rw-r--r--   0 lautaro   (1000) lautaro   (1000)      678 2023-12-06 18:14:21.154510 enzope-0.0.8/PKG-INFO
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        4 2023-05-11 13:40:28.000000 enzope-0.0.8/README.md
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       78 2023-12-06 18:14:21.154510 enzope-0.0.8/setup.cfg
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     1528 2023-12-06 18:14:09.000000 enzope-0.0.8/setup.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 18:14:21.154510 enzope-0.0.8/src/
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 18:14:21.154510 enzope-0.0.8/src/enzope/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      244 2023-07-31 12:50:17.000000 enzope-0.0.8/src/enzope/__init__.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 18:14:21.154510 enzope-0.0.8/src/enzope/graphs/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-06-21 16:54:29.000000 enzope-0.0.8/src/enzope/graphs/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     6768 2023-07-18 16:41:47.000000 enzope-0.0.8/src/enzope/graphs/custom_gtg.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     5608 2023-12-04 15:08:26.000000 enzope-0.0.8/src/enzope/graphs/graph_class.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 18:14:21.154510 enzope-0.0.8/src/enzope/kernels/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-11 14:05:10.000000 enzope-0.0.8/src/enzope/kernels/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     2999 2023-07-31 12:46:30.000000 enzope-0.0.8/src/enzope/kernels/k_ys.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      430 2023-07-18 16:41:47.000000 enzope-0.0.8/src/enzope/kernels/locks.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 18:14:21.154510 enzope-0.0.8/src/enzope/metrics/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-07-13 14:40:05.000000 enzope-0.0.8/src/enzope/metrics/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      465 2023-07-18 16:41:47.000000 enzope-0.0.8/src/enzope/metrics/gpu_measures.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      821 2023-12-06 18:02:12.000000 enzope-0.0.8/src/enzope/metrics/measures.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 18:14:21.154510 enzope-0.0.8/src/enzope/models/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-07-13 14:40:02.000000 enzope-0.0.8/src/enzope/models/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)    10686 2023-12-06 18:13:44.000000 enzope-0.0.8/src/enzope/models/model.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 18:14:21.154510 enzope-0.0.8/src/enzope/trades/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:37:17.000000 enzope-0.0.8/src/enzope/trades/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       63 2023-06-01 14:02:21.000000 enzope-0.0.8/src/enzope/trades/ys.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 18:14:21.154510 enzope-0.0.8/src/enzope.egg-info/
--rw-r--r--   0 lautaro   (1000) lautaro   (1000)      678 2023-12-06 18:14:21.000000 enzope-0.0.8/src/enzope.egg-info/PKG-INFO
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      609 2023-12-06 18:14:21.000000 enzope-0.0.8/src/enzope.egg-info/SOURCES.txt
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        1 2023-12-06 18:14:21.000000 enzope-0.0.8/src/enzope.egg-info/dependency_links.txt
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       40 2023-12-06 18:14:21.000000 enzope-0.0.8/src/enzope.egg-info/requires.txt
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        7 2023-12-06 18:14:21.000000 enzope-0.0.8/src/enzope.egg-info/top_level.txt
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 20:06:13.854235 enzope-0.0.9/
+-rw-r--r--   0 lautaro   (1000) lautaro   (1000)      678 2023-12-06 20:06:13.854235 enzope-0.0.9/PKG-INFO
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        4 2023-05-11 13:40:28.000000 enzope-0.0.9/README.md
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       78 2023-12-06 20:06:13.854235 enzope-0.0.9/setup.cfg
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     1528 2023-12-06 20:06:04.000000 enzope-0.0.9/setup.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 20:06:13.854235 enzope-0.0.9/src/
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 20:06:13.854235 enzope-0.0.9/src/enzope/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      244 2023-07-31 12:50:17.000000 enzope-0.0.9/src/enzope/__init__.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 20:06:13.854235 enzope-0.0.9/src/enzope/graphs/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-06-21 16:54:29.000000 enzope-0.0.9/src/enzope/graphs/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     6768 2023-07-18 16:41:47.000000 enzope-0.0.9/src/enzope/graphs/custom_gtg.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     5608 2023-12-04 15:08:26.000000 enzope-0.0.9/src/enzope/graphs/graph_class.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 20:06:13.854235 enzope-0.0.9/src/enzope/kernels/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-11 14:05:10.000000 enzope-0.0.9/src/enzope/kernels/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     2999 2023-07-31 12:46:30.000000 enzope-0.0.9/src/enzope/kernels/k_ys.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      430 2023-07-18 16:41:47.000000 enzope-0.0.9/src/enzope/kernels/locks.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 20:06:13.854235 enzope-0.0.9/src/enzope/metrics/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-07-13 14:40:05.000000 enzope-0.0.9/src/enzope/metrics/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      465 2023-07-18 16:41:47.000000 enzope-0.0.9/src/enzope/metrics/gpu_measures.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      821 2023-12-06 18:02:12.000000 enzope-0.0.9/src/enzope/metrics/measures.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 20:06:13.854235 enzope-0.0.9/src/enzope/models/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-07-13 14:40:02.000000 enzope-0.0.9/src/enzope/models/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)    10684 2023-12-06 19:30:33.000000 enzope-0.0.9/src/enzope/models/model.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 20:06:13.854235 enzope-0.0.9/src/enzope/trades/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:37:17.000000 enzope-0.0.9/src/enzope/trades/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       63 2023-06-01 14:02:21.000000 enzope-0.0.9/src/enzope/trades/ys.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-12-06 20:06:13.854235 enzope-0.0.9/src/enzope.egg-info/
+-rw-r--r--   0 lautaro   (1000) lautaro   (1000)      678 2023-12-06 20:06:13.000000 enzope-0.0.9/src/enzope.egg-info/PKG-INFO
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      609 2023-12-06 20:06:13.000000 enzope-0.0.9/src/enzope.egg-info/SOURCES.txt
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        1 2023-12-06 20:06:13.000000 enzope-0.0.9/src/enzope.egg-info/dependency_links.txt
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       40 2023-12-06 20:06:13.000000 enzope-0.0.9/src/enzope.egg-info/requires.txt
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        7 2023-12-06 20:06:13.000000 enzope-0.0.9/src/enzope.egg-info/top_level.txt
```

### Comparing `enzope-0.0.8/PKG-INFO` & `enzope-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enzope
-Version: 0.0.8
+Version: 0.0.9
 Summary: Agent based modelling in complex networks
 Author: Lautaro Giordano
 Author-email: giordanolautaro@gmail.com
 Project-URL: Source, https://github.com/lautarogiordano/enzope/
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `enzope-0.0.8/setup.py` & `enzope-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
    name="enzope",  # Required
 
-   version="0.0.8",  # Required
+   version="0.0.9",  # Required
    
    description="Agent based modelling in complex networks",  # Optional
    
    long_description=long_description,  # Optional
    long_description_content_type="text/markdown",  # Optional (see note above)
    
    author="Lautaro Giordano",  # Optional
```

### Comparing `enzope-0.0.8/src/enzope/graphs/custom_gtg.py` & `enzope-0.0.9/src/enzope/graphs/custom_gtg.py`

 * *Files identical despite different names*

### Comparing `enzope-0.0.8/src/enzope/graphs/graph_class.py` & `enzope-0.0.9/src/enzope/graphs/graph_class.py`

 * *Files identical despite different names*

### Comparing `enzope-0.0.8/src/enzope/kernels/k_ys.py` & `enzope-0.0.9/src/enzope/kernels/k_ys.py`

 * *Files identical despite different names*

### Comparing `enzope-0.0.8/src/enzope/metrics/measures.py` & `enzope-0.0.9/src/enzope/metrics/measures.py`

 * *Files identical despite different names*

### Comparing `enzope-0.0.8/src/enzope/models/model.py` & `enzope-0.0.9/src/enzope/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                 )
 
                 del c_neighs_d, neighs_d
 
             w_d.copy_to_host(self.w, self.stream)
         del w_d, r_d, m_d
 
-        # cuda.synchronize()
+        cuda.synchronize()
 
 
 class GPUEnsemble:
     def __init__(
         self, n_models=1, n_agents=1000, tpb=32, bpg=512, graphs=None, **kwargs
     ):
         self.n_streams = n_models
```

### Comparing `enzope-0.0.8/src/enzope.egg-info/PKG-INFO` & `enzope-0.0.9/src/enzope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enzope
-Version: 0.0.8
+Version: 0.0.9
 Summary: Agent based modelling in complex networks
 Author: Lautaro Giordano
 Author-email: giordanolautaro@gmail.com
 Project-URL: Source, https://github.com/lautarogiordano/enzope/
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `enzope-0.0.8/src/enzope.egg-info/SOURCES.txt` & `enzope-0.0.9/src/enzope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

