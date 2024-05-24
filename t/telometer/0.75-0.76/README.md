# Comparing `tmp/telometer-0.75.tar.gz` & `tmp/telometer-0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telometer-0.75.tar", last modified: Wed May 22 16:07:55 2024, max compression
+gzip compressed data, was "telometer-0.76.tar", last modified: Fri May 24 05:24:10 2024, max compression
```

## Comparing `telometer-0.75.tar` & `telometer-0.76.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-05-22 16:07:55.491780 telometer-0.75/
--rw-r--r--   0 santiago   (501) staff       (20)     1074 2024-05-22 15:01:09.000000 telometer-0.75/LICENSE.txt
--rw-r--r--   0 santiago   (501) staff       (20)      613 2024-05-22 16:07:55.487092 telometer-0.75/PKG-INFO
--rw-r--r--   0 santiago   (501) staff       (20)      148 2024-05-22 15:03:15.000000 telometer-0.75/README.md
--rw-r--r--   0 santiago   (501) staff       (20)       38 2024-05-22 16:07:55.491881 telometer-0.75/setup.cfg
--rw-r--r--   0 santiago   (501) staff       (20)      826 2024-05-22 16:07:45.000000 telometer-0.75/setup.py
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-05-22 16:07:55.474724 telometer-0.75/telometer/
--rw-r--r--   0 santiago   (501) staff       (20)       91 2023-12-02 23:50:44.000000 telometer-0.75/telometer/__init__.py
--rw-r--r--   0 santiago   (501) staff       (20)     6855 2024-05-22 16:07:27.000000 telometer-0.75/telometer/telometer.py
-drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-05-22 16:07:55.486161 telometer-0.75/telometer.egg-info/
--rw-r--r--   0 santiago   (501) staff       (20)      613 2024-05-22 16:07:55.000000 telometer-0.75/telometer.egg-info/PKG-INFO
--rw-r--r--   0 santiago   (501) staff       (20)      243 2024-05-22 16:07:55.000000 telometer-0.75/telometer.egg-info/SOURCES.txt
--rw-r--r--   0 santiago   (501) staff       (20)        1 2024-05-22 16:07:55.000000 telometer-0.75/telometer.egg-info/dependency_links.txt
--rw-r--r--   0 santiago   (501) staff       (20)       66 2024-05-22 16:07:55.000000 telometer-0.75/telometer.egg-info/entry_points.txt
--rw-r--r--   0 santiago   (501) staff       (20)       10 2024-05-22 16:07:55.000000 telometer-0.75/telometer.egg-info/top_level.txt
+drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-05-24 05:24:10.780628 telometer-0.76/
+-rw-r--r--   0 santiago   (501) staff       (20)     1074 2024-05-22 15:01:09.000000 telometer-0.76/LICENSE.txt
+-rw-r--r--   0 santiago   (501) staff       (20)      613 2024-05-24 05:24:10.775558 telometer-0.76/PKG-INFO
+-rw-r--r--   0 santiago   (501) staff       (20)      148 2024-05-22 15:03:15.000000 telometer-0.76/README.md
+-rw-r--r--   0 santiago   (501) staff       (20)       38 2024-05-24 05:24:10.780696 telometer-0.76/setup.cfg
+-rw-r--r--   0 santiago   (501) staff       (20)      826 2024-05-24 05:23:49.000000 telometer-0.76/setup.py
+drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-05-24 05:24:10.756821 telometer-0.76/telometer/
+-rw-r--r--   0 santiago   (501) staff       (20)       91 2023-12-02 23:50:44.000000 telometer-0.76/telometer/__init__.py
+-rw-r--r--   0 santiago   (501) staff       (20)     6969 2024-05-24 05:23:57.000000 telometer-0.76/telometer/telometer.py
+drwxr-xr-x   0 santiago   (501) staff       (20)        0 2024-05-24 05:24:10.771441 telometer-0.76/telometer.egg-info/
+-rw-r--r--   0 santiago   (501) staff       (20)      613 2024-05-24 05:24:10.000000 telometer-0.76/telometer.egg-info/PKG-INFO
+-rw-r--r--   0 santiago   (501) staff       (20)      243 2024-05-24 05:24:10.000000 telometer-0.76/telometer.egg-info/SOURCES.txt
+-rw-r--r--   0 santiago   (501) staff       (20)        1 2024-05-24 05:24:10.000000 telometer-0.76/telometer.egg-info/dependency_links.txt
+-rw-r--r--   0 santiago   (501) staff       (20)       66 2024-05-24 05:24:10.000000 telometer-0.76/telometer.egg-info/entry_points.txt
+-rw-r--r--   0 santiago   (501) staff       (20)       10 2024-05-24 05:24:10.000000 telometer-0.76/telometer.egg-info/top_level.txt
```

### Comparing `telometer-0.75/LICENSE.txt` & `telometer-0.76/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `telometer-0.75/PKG-INFO` & `telometer-0.76/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telometer
-Version: 0.75
+Version: 0.76
 Summary: a simple regular expression based method for measuring individual, chromosome-specific telomere lengths from long-read sequencing data
 Author: Santiago E Sanchez
 Author-email: ses94@stanford.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `telometer-0.75/setup.py` & `telometer-0.76/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="telometer",
-    version="0.75",
+    version="0.76",
     author="Santiago E Sanchez",
     author_email="ses94@stanford.edu",
     description="a simple regular expression based method for measuring individual, chromosome-specific telomere lengths from long-read sequencing data",
     packages=setuptools.find_packages(),
     license='MIT',
     long_description=open('README.md').read(),
     classifiers=[
```

### Comparing `telometer-0.75/telometer/telometer.py` & `telometer-0.76/telometer/telometer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# Telometer v0.75
+# Telometer v0.76
 # Created by: Santiago E Sanchez
 # Artandi Lab, Stanford University, 2023
 # Measures telomeres from ONT or PacBio long reads aligned to a T2T genome assembly
 # Simple Usage: telometer -b sorted_t2t.bam -o output.tsv
 
 import pysam
 import re
@@ -117,16 +117,16 @@
         'is_unmapped': read.is_unmapped,
         'is_reverse': read.is_reverse,
         'reference_start': read.reference_start,
         'reference_end': read.reference_end,
         'reference_name': read.reference_name,
         'mapping_quality': read.mapping_quality,
         'query_sequence': read.query_sequence,
-        'reference_length': bam_file.get_reference_length(read.reference_name)
-    } for read in bam_file]
+        'reference_length': bam_file.get_reference_length(read.reference_name) if read.reference_name is not None else None
+    } for read in bam_file if read.reference_name is not None and read.reference_name != 'chrM']
 
     with Pool(processes=cpu_count()) as pool:
         results = pool.map(
             process_read,
             [(read_data, telomere_repeats_re, adapters, args.minreadlen) for read_data in read_data_list]
         )
```

### Comparing `telometer-0.75/telometer.egg-info/PKG-INFO` & `telometer-0.76/telometer.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telometer
-Version: 0.75
+Version: 0.76
 Summary: a simple regular expression based method for measuring individual, chromosome-specific telomere lengths from long-read sequencing data
 Author: Santiago E Sanchez
 Author-email: ses94@stanford.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

