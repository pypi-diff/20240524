# Comparing `tmp/pipemake-0.6.tar.gz` & `tmp/pipemake-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipemake-0.6.tar", last modified: Thu May  9 01:39:06 2024, max compression
+gzip compressed data, was "pipemake-0.7.tar", last modified: Fri May 24 21:09:54 2024, max compression
```

## Comparing `pipemake-0.6.tar` & `pipemake-0.7.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:39:06.200308 pipemake-0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-09 01:39:00.000000 pipemake-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-09 01:39:06.200308 pipemake-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-09 01:39:00.000000 pipemake-0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:39:06.196308 pipemake-0.6/pipemake/
--rwxr-xr-x   0 runner    (1001) docker     (127)      524 2024-05-09 01:39:00.000000 pipemake-0.6/pipemake/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4919 2024-05-09 01:39:00.000000 pipemake-0.6/pipemake/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1583 2024-05-09 01:39:00.000000 pipemake-0.6/pipemake/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12366 2024-05-09 01:39:00.000000 pipemake-0.6/pipemake/pipemake.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2521 2024-05-09 01:39:00.000000 pipemake-0.6/pipemake/processIO.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7991 2024-05-09 01:39:00.000000 pipemake-0.6/pipemake/seqIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    22816 2024-05-09 01:39:00.000000 pipemake-0.6/pipemake/snakemakeIO.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5420 2024-05-09 01:39:00.000000 pipemake-0.6/pipemake/wildcardIO.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:39:06.200308 pipemake-0.6/pipemake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-09 01:39:06.000000 pipemake-0.6/pipemake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-09 01:39:06.000000 pipemake-0.6/pipemake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:39:06.000000 pipemake-0.6/pipemake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-09 01:39:06.000000 pipemake-0.6/pipemake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 01:39:06.000000 pipemake-0.6/pipemake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 01:39:06.000000 pipemake-0.6/pipemake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 01:39:06.200308 pipemake-0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1019 2024-05-09 01:39:00.000000 pipemake-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:09:54.806649 pipemake-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-24 21:09:50.000000 pipemake-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-24 21:09:54.806649 pipemake-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 21:09:50.000000 pipemake-0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:09:54.806649 pipemake-0.7/pipemake/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      524 2024-05-24 21:09:50.000000 pipemake-0.7/pipemake/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4919 2024-05-24 21:09:50.000000 pipemake-0.7/pipemake/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1583 2024-05-24 21:09:50.000000 pipemake-0.7/pipemake/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12364 2024-05-24 21:09:50.000000 pipemake-0.7/pipemake/pipemake.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2520 2024-05-24 21:09:50.000000 pipemake-0.7/pipemake/processIO.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7946 2024-05-24 21:09:50.000000 pipemake-0.7/pipemake/seqIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22816 2024-05-24 21:09:50.000000 pipemake-0.7/pipemake/snakemakeIO.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2374 2024-05-24 21:09:50.000000 pipemake-0.7/pipemake/wildcardIO.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:09:54.806649 pipemake-0.7/pipemake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-24 21:09:54.000000 pipemake-0.7/pipemake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-24 21:09:54.000000 pipemake-0.7/pipemake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 21:09:54.000000 pipemake-0.7/pipemake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 21:09:54.000000 pipemake-0.7/pipemake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 21:09:54.000000 pipemake-0.7/pipemake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 21:09:54.000000 pipemake-0.7/pipemake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 21:09:54.806649 pipemake-0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1019 2024-05-24 21:09:50.000000 pipemake-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:09:54.806649 pipemake-0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-24 21:09:50.000000 pipemake-0.7/tests/test_processIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-24 21:09:50.000000 pipemake-0.7/tests/test_seqIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-24 21:09:50.000000 pipemake-0.7/tests/test_wildcardIO.py
```

### Comparing `pipemake-0.6/LICENSE` & `pipemake-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pipemake-0.6/PKG-INFO` & `pipemake-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipemake
-Version: 0.6
+Version: 0.7
 Summary: Pipemake: A pipeline creation tool using Snakemake
 Home-page: https://github.com/kocherlab/pipemake
 License: MIT
 Project-URL: Documentation, https://pipemake.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/kocherlab/pipemake
 Project-URL: Issue tracker, https://github.com/kocherlab/pipemake/issues
 Requires-Python: >=3.7
```

### Comparing `pipemake-0.6/pipemake/__init__.py` & `pipemake-0.7/pipemake/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 # Basic Information
 __name__ = "pipemake"
-__version__ = "0.6"
+__version__ = "0.7"
 __summary__ = "Pipemake: A pipeline creation tool using Snakemake"
 __url__ = "https://github.com/kocherlab/pipemake"
 __code__ = "https://github.com/kocherlab/pipemake"
 __issue__ = "https://github.com/kocherlab/pipemake/issues"
 __docs__ = "https://pipemake.readthedocs.io/en/latest/"
 __license__ = "MIT"
 __copyright__ = "2023"
```

### Comparing `pipemake-0.6/pipemake/config.py` & `pipemake-0.7/pipemake/config.py`

 * *Files identical despite different names*

### Comparing `pipemake-0.6/pipemake/logger.py` & `pipemake-0.7/pipemake/logger.py`

 * *Files identical despite different names*

### Comparing `pipemake-0.6/pipemake/pipemake.py` & `pipemake-0.7/pipemake/pipemake.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 				else:
 					raise Exception(f'Argument group not supported: {pipeline_arg_group}')
 				
 		# Add the common optional arguments, but at the end of the list
 		pipeline_arg_groups['optional'].add_argument('--scale-threads', help = 'Scale the threads for each task', type = float, default = 1.0)
 		pipeline_arg_groups['optional'].add_argument('--scale-mem', help = 'Scale the memory (RAM) for each task', type = float, default = 1.0)
 		pipeline_arg_groups['optional'].add_argument('--resource-yml', help = 'Create a seperate resource yaml', action = 'store_true')
-		pipeline_arg_groups['optional'].add_argument('--singularity-dir', help = 'Assign different directory of singularity images', type = str, default = '/Genomics/argo/users/aewebb/.local/images/')
+		pipeline_arg_groups['optional'].add_argument('--singularity-dir', help = 'Assign different directory of singularity images', type = str, default = '/Genomics/kocherlab/lab/Pipelines/images')
 		pipeline_arg_groups['optional'].add_argument('-h', '--help', action = 'help', help = 'show this help message and exit')
 
 	return vars(pipeline_parser.parse_args())
 
 # Create variables to store randomString and timeStamp
 random_string = None
 time_stamp = None
```

### Comparing `pipemake-0.6/pipemake/processIO.py` & `pipemake-0.7/pipemake/processIO.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pipemake.seqIO import SeqFileIO, SeqTableIO
 from pipemake.wildcardIO import WildcardIO
 
 class ProcessIO ():
 	def __init__ (self, processIO, standardize_func = None, **kwargs):
 		self.processIO = processIO
 		self.standardize_call = getattr(self.processIO, standardize_func)
-		self.samples = []
+		#self.samples = []
 
 	@classmethod
 	def fromWildcardStr (cls, wildcard_str = '', **kwargs):
 		return cls(WildcardIO.fromStr(wildcard_str, **kwargs), standardize_func = 'standardizedFiles')
 
 	@classmethod
 	def fromTableFile (cls, table_filename = '', **kwargs):
@@ -24,15 +24,14 @@
 
 	def returnSamples (self, **kwargs):
 		return self.processIO.returnSamples()
 
 	def returnPaths (self, **kwargs):
 		return self.processIO.returnPaths(**kwargs)
 
-
 def standardizeInput (method = '', args = {}):
 	
 	# Create the standardization call
 	if method == 'wildcard-str': standardize_input_call = ProcessIO.fromWildcardStr(**args)
 	elif method == 'table-file': standardize_input_call = ProcessIO.fromTableFile(**args)
 	elif method == 'file-str': standardize_input_call = ProcessIO.fromFileStr(**args)
 	else: raise Exception(f'No standardization method given for: {method}')
```

### Comparing `pipemake-0.6/pipemake/seqIO.py` & `pipemake-0.7/pipemake/seqIO.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import os
-import sys
 import gzip
 import shutil
 import logging
-import hashlib
 
 import pandas as pd
 
-from collections import defaultdict
 from snakemake.io import get_wildcard_names
 
 def checkIfGzipped (filename):
 
 	with open (filename, 'rb') as check_file:
 		check_line = check_file.readline()
 		bgzip_header = b'\x1f\x8b\x08\x04\x00\x00\x00\x00\x00\xff\x06\x00\x42\x43\x02\x00'
@@ -46,15 +43,15 @@
 	@ property
 	def args (self):
 		
 		# Create dict to store optional args
 		arg_dict = {}
 		
 		# Assign potential args
-		if self.link_path:arg_dict['bind'] = self.link_path
+		if self.link_path: arg_dict['bind'] = self.link_path
 		
 		return arg_dict
 
 	@classmethod
 	def create (cls, *args, **kwargs):
 		return cls(*args, **kwargs)
 
@@ -101,15 +98,15 @@
 
 class SeqTableIO ():
 	def __init__ (self, table_dataframe, sample_column = 'sample', **kwargs):
 
 		# Confirm wildcards were assigned
 		if not isinstance(table_dataframe, pd.DataFrame): 
 			raise Exception(f'Table must be stored as a pandas DataFrame: {table_dataframe}')
-
+		
 		# Assign the basic arguments
 		self._table_dataframe = table_dataframe
 		self._sample_column = sample_column
 		self._file_columns = set()
 		self._table_columns = set([sample_column])
 
 		if sample_column not in self._table_dataframe.columns:
@@ -138,16 +135,15 @@
 	def _file_column (self):
 		if len(self._file_columns) > 1:
 			raise Exception(f'Files may exist within a single column')
 		return list(self._file_columns)[0]
 	
 	@classmethod
 	def fromFilenameStr (cls, table_filename, sep = '\t', **kwargs):
-
-		return cls(table_dataframe = pd.read_csv(table_filename, sep = sep, dtype = str).fillna(''), **kwargs)
+		return cls(table_dataframe = pd.read_csv(table_filename, sep = sep, index_col = False, dtype = str).fillna(''), **kwargs)
 
 	def standardizedFiles (self, standardized_wildcard, **kwargs):
 
 		# Assign the standardized wildcard names
 		standardized_wildcard_names = get_wildcard_names(standardized_wildcard)
 
 		# Confirm the dataframe column are being standardized
```

### Comparing `pipemake-0.6/pipemake/snakemakeIO.py` & `pipemake-0.7/pipemake/snakemakeIO.py`

 * *Files identical despite different names*

### Comparing `pipemake-0.6/pipemake.egg-info/PKG-INFO` & `pipemake-0.7/pipemake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipemake
-Version: 0.6
+Version: 0.7
 Summary: Pipemake: A pipeline creation tool using Snakemake
 Home-page: https://github.com/kocherlab/pipemake
 License: MIT
 Project-URL: Documentation, https://pipemake.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/kocherlab/pipemake
 Project-URL: Issue tracker, https://github.com/kocherlab/pipemake/issues
 Requires-Python: >=3.7
```

### Comparing `pipemake-0.6/setup.py` & `pipemake-0.7/setup.py`

 * *Files identical despite different names*

