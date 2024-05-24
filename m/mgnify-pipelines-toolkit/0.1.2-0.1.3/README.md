# Comparing `tmp/mgnify_pipelines_toolkit-0.1.2.tar.gz` & `tmp/mgnify_pipelines_toolkit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgnify_pipelines_toolkit-0.1.2.tar", last modified: Fri Apr 26 11:43:50 2024, max compression
+gzip compressed data, was "mgnify_pipelines_toolkit-0.1.3.tar", last modified: Fri May 24 14:05:24 2024, max compression
```

## Comparing `mgnify_pipelines_toolkit-0.1.2.tar` & `mgnify_pipelines_toolkit-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.835709 mgnify_pipelines_toolkit-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-26 11:43:50.835709 mgnify_pipelines_toolkit-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.827709 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.827709 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.831709 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/amplicon_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/are_there_primers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/assess_inflection_point_mcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/assess_mcp_proportions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18392 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/classify_var_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/find_mcp_inflection_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/make_asv_count_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/mapseq_to_asv_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/remove_ambiguous_reads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/rev_comp_se_primers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/standard_primer_matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.831709 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/get_subunits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/get_subunits_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/mapseq2biom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.831709 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/regex_ambiguous_bases.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/tax_ranks.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/thresholds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/var_region_coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:43:50.831709 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-26 11:43:50.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-26 11:43:50.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:43:50.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-26 11:43:50.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-26 11:43:50.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-26 11:43:50.000000 mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-26 11:43:45.000000 mgnify_pipelines_toolkit-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 11:43:50.835709 mgnify_pipelines_toolkit-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:05:24.905618 mgnify_pipelines_toolkit-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-24 14:05:24.905618 mgnify_pipelines_toolkit-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:05:24.897618 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:05:24.901618 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:05:24.901618 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/amplicon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/are_there_primers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/assess_inflection_point_mcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/assess_mcp_proportions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18392 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/classify_var_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/find_mcp_inflection_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/make_asv_count_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/mapseq_to_asv_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/primer_val_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/remove_ambiguous_reads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/rev_comp_se_primers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/standard_primer_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:05:24.901618 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/shared/get_subunits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/shared/get_subunits_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/shared/mapseq2biom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:05:24.905618 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/constants/regex_ambiguous_bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/constants/tax_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/constants/thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/constants/var_region_coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:05:24.905618 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-24 14:05:24.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-24 14:05:24.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 14:05:24.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-24 14:05:24.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-24 14:05:24.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 14:05:24.000000 mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-24 14:05:20.000000 mgnify_pipelines_toolkit-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 14:05:24.905618 mgnify_pipelines_toolkit-0.1.3/setup.cfg
```

### Comparing `mgnify_pipelines_toolkit-0.1.2/LICENSE` & `mgnify_pipelines_toolkit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/PKG-INFO` & `mgnify_pipelines_toolkit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgnify_pipelines_toolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: Collection of scripts and tools for MGnify pipelines
 Author-email: MGnify team <metagenomics-help@ebi.ac.uk>
 License: Apache Software License 2.0
 Keywords: bioinformatics,pipelines,metagenomics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `mgnify_pipelines_toolkit-0.1.2/README.md` & `mgnify_pipelines_toolkit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/amplicon_utils.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/amplicon_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,25 +43,18 @@
         cmd = [
             'zcat',
             read_path
         ]
         zcat_proc = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
         cmd = [
-            'sed',
-            '-n',
-            '1~4p',
-        ]
-        sed_proc = subprocess.Popen(cmd, stdin=zcat_proc.stdout, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-
-        cmd = [
             'wc',
             '-l'
         ]
-        wc_proc = subprocess.Popen(cmd, stdin=sed_proc.stdout, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        wc_proc = subprocess.Popen(cmd, stdin=zcat_proc.stdout, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         stdout, stderr = wc_proc.communicate()
 
     elif type == 'fasta':
         cmd = [
             'grep',
             '-c',
             '^>',
@@ -74,14 +67,17 @@
 
     if not read_count.isdigit():
         logging.error(f"Read count is not a digit, something is wrong. stdout: '{stdout}', stderr: '{stderr}'")
         exit(1)
 
     read_count = int(read_count)
 
+    if type == 'fastq':
+        read_count /= 4
+
     return read_count
 
 def build_cons_seq(cons_list, read_count, cons_threshold=0.80, do_not_include=None, counter=1, max_line_count=None):
     """
     Generate consensus sequence using a list of base conservation dictionaries most likely
     generated by the `build_mcp_cons_dict_list()` function.
     Also returns a list containing the conservation value of the most conserved base at every
```

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/are_there_primers.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/are_there_primers.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/assess_inflection_point_mcp.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/assess_inflection_point_mcp.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/assess_mcp_proportions.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/assess_mcp_proportions.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/classify_var_regions.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/classify_var_regions.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/find_mcp_inflection_points.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/find_mcp_inflection_points.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/make_asv_count_table.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/make_asv_count_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,22 @@
 import pandas as pd
 
 from mgnify_pipelines_toolkit.constants.tax_ranks import _SILVA_TAX_RANKS, _PR2_TAX_RANKS
 
 logging.basicConfig(level=logging.DEBUG)
 
 def parse_args():
-
     parser = argparse.ArgumentParser()
 
     parser.add_argument("-t", "--taxa", required=True, type=str, help="Path to taxa file")
     parser.add_argument("-f", "--fwd", required=True, type=str, help="Path to DADA2 forward map file")
     parser.add_argument("-r", "--rev", required=False, type=str, help="Path to DADA2 reverse map file")
-    parser.add_argument("-a", "--amp", required=True, type=str, help="Path to extracted amp_region reads from inference subworkflow")
+    parser.add_argument(
+        "-a", "--amp", required=True, type=str, help="Path to extracted amp_region reads from inference subworkflow"
+    )
     parser.add_argument("-hd", "--headers", required=True, type=str, help="Path to fastq headers")
     parser.add_argument("-s", "--sample", required=True, type=str, help="Sample ID")
 
     args = parser.parse_args()
   
     _TAXA = args.taxa
     _FWD = args.fwd
@@ -44,45 +45,42 @@
     _HEADERS = args.headers
     _SAMPLE = args.sample
 
     return _TAXA, _FWD, _REV, _AMP, _HEADERS, _SAMPLE
 
 
 def order_df(taxa_df):
-
     if len(taxa_df.columns) == 9:
         taxa_df = taxa_df.sort_values(_SILVA_TAX_RANKS, ascending=True)
     elif len(taxa_df.columns) == 10:
         taxa_df = taxa_df.sort_values(_PR2_TAX_RANKS, ascending=True)
     else:
         logging.error("Data frame not the right size, something wrong.")
         exit(1)
 
     return taxa_df
 
 def make_tax_assignment_dict_silva(taxa_df, asv_dict):
-
     tax_assignment_dict = defaultdict(int)
 
     for i in range(len(taxa_df)):
-        
         sorted_index = taxa_df.index[i]
         asv_num = taxa_df.iloc[i, 0]
         asv_count = asv_dict[asv_num]
 
         if asv_count == 0:
             continue
 
         sk = taxa_df.loc[sorted_index, "Superkingdom"]
         k = taxa_df.loc[sorted_index, "Kingdom"]
         p = taxa_df.loc[sorted_index, "Phylum"]
         c = taxa_df.loc[sorted_index, "Class"]
         o = taxa_df.loc[sorted_index, "Order"]
         f = taxa_df.loc[sorted_index, "Family"]
-        g = taxa_df.loc[sorted_index, "Genus"]        
+        g = taxa_df.loc[sorted_index, "Genus"]
         s = taxa_df.loc[sorted_index, "Species"]
 
         tax_assignment = ""
 
         while True:
 
             if sk != "0":
@@ -138,19 +136,17 @@
             continue
 
         tax_assignment_dict[tax_assignment] += asv_count
     
     return tax_assignment_dict
 
 def make_tax_assignment_dict_pr2(taxa_df, asv_dict):
-
     tax_assignment_dict = defaultdict(int)
 
     for i in range(len(taxa_df)):
-        
         sorted_index = taxa_df.index[i]
         asv_num = taxa_df.iloc[i, 0]
         asv_count = asv_dict[asv_num]
 
         if asv_count == 0:
             continue
 
@@ -158,20 +154,19 @@
         sg = taxa_df.loc[sorted_index, "Supergroup"]
         dv = taxa_df.loc[sorted_index, "Division"]
         sdv = taxa_df.loc[sorted_index, "Subdivision"]
         c = taxa_df.loc[sorted_index, "Class"]
         o = taxa_df.loc[sorted_index, "Order"]
         f = taxa_df.loc[sorted_index, "Family"]
         g = taxa_df.loc[sorted_index, "Genus"]
-        s = taxa_df.loc[sorted_index, "Species"]         
+        s = taxa_df.loc[sorted_index, "Species"]
 
         tax_assignment = ""
 
         while True:
-
             if d != "0":
                 d = "_".join(d.split(" "))
                 tax_assignment += d
             else:
                 break
 
             if sg != "0":
@@ -225,59 +220,58 @@
             continue
 
         tax_assignment_dict[tax_assignment] += asv_count
 
     return tax_assignment_dict
 
 def main():
-
     _TAXA, _FWD, _REV, _AMP, _HEADERS, _SAMPLE = parse_args()
-    
+
     fwd_fr = open(_FWD, "r")
     paired_end = True
 
     if _REV == None:
         paired_end = False
         rev_fr = [True]
     else:
         rev_fr = open(_REV, "r")
 
     taxa_df = pd.read_csv(_TAXA, sep="\t", dtype=str)
     taxa_df = taxa_df.fillna("0")
     taxa_df = order_df(taxa_df)
-    
-    amp_reads = [ read.strip() for read in list(open(_AMP, "r")) ]
-    headers = [ read.split(" ")[0][1:] for read in list(open(_HEADERS, "r")) ]
+
+    amp_reads = [read.strip() for read in list(open(_AMP, "r"))]
+    headers = [read.split(" ")[0][1:] for read in 
+               list(open(_HEADERS, "r"))]
     amp_region = ".".join(_AMP.split(".")[1:3])
 
     asv_dict = defaultdict(int)
 
     counter = -1
     for line_fwd in fwd_fr:
-
         counter += 1
         line_fwd = line_fwd.strip()
         fwd_asvs = line_fwd.split(",")
 
         if paired_end:
             line_rev = next(rev_fr).strip()
-            rev_asvs = line_rev.split(",")        
+            rev_asvs = line_rev.split(",")
             asv_intersection = list(set(fwd_asvs).intersection(rev_asvs))
-            
+
             if len(asv_intersection) == 0:
                 continue
-            
+
             if len(asv_intersection) == 1 and asv_intersection[0] == "0":
                 continue
         else:
             asv_intersection = fwd_asvs
 
         if headers[counter] in amp_reads:
             asv_dict[f"seq_{int(asv_intersection[0]) - 1}"] += 1
-    
+
     fwd_fr.close()
     if paired_end:
         rev_fr.close()
 
     ref_db = ""
 
     if len(taxa_df.columns) == 9:
@@ -286,11 +280,11 @@
     elif len(taxa_df.columns) == 10:
         tax_assignment_dict = make_tax_assignment_dict_pr2(taxa_df, asv_dict)
         ref_db = "pr2"
 
     with open(f"./{_SAMPLE}_{amp_region}_{ref_db}_asv_krona_counts.txt", "w") as fw:
         for tax_assignment, count in tax_assignment_dict.items():
             fw.write(f"{count}\t{tax_assignment}\n")
-    
+
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/mapseq_to_asv_table.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/mapseq_to_asv_table.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,108 +19,121 @@
 import logging
 
 import pandas as pd
 
 logging.basicConfig(level=logging.DEBUG)
 
 def parse_args():
-
     parser = argparse.ArgumentParser()
     parser.add_argument("-i", "--input", required=True, type=str, help="Input from MAPseq output")
-    parser.add_argument("-l", "--label", choices=['DADA2-SILVA', 'DADA2-PR2'], required=True, type=str, help="Database label - either DADA2-SILVA or DADA2-PR2")
+    parser.add_argument(
+        "-l",
+        "--label",
+        choices=["DADA2-SILVA", "DADA2-PR2"],
+        required=True,
+        type=str,
+        help="Database label - either DADA2-SILVA or DADA2-PR2",
+    )
     parser.add_argument("-s", "--sample", required=True, type=str, help="Sample ID")
 
     args = parser.parse_args()
 
     _INPUT = args.input
     _LABEL = args.label
     _SAMPLE = args.sample
 
     return _INPUT, _LABEL, _SAMPLE
 
 def parse_label(label):
-
     silva_short_ranks = ["sk__", "k__", "p__", "c__", "o__", "f__", "g__", "s__"]
     pr2_short_ranks = ["d__", "sg__", "dv__", "sdv__", "c__", "o__", "f__", "g__", "s__"]
 
     silva_long_ranks = ["Superkingdom", "Kingdom", "Phylum", "Class", "Order", "Family", "Genus", "Species"]
     pr2_long_ranks = ["Domain", "Supergroup", "Division", "Subdivision", "Class", "Order", "Family", "Genus", "Species"]
 
-    chosen_short_ranks = ''
-    chosen_long_ranks = ''
+    chosen_short_ranks = ""
+    chosen_long_ranks = ""
 
-    if label == 'DADA2-SILVA':
+    if label == "DADA2-SILVA":
         chosen_short_ranks = silva_short_ranks
         chosen_long_ranks = silva_long_ranks
-    elif label == 'DADA2-PR2':
+    elif label == "DADA2-PR2":
         chosen_short_ranks = pr2_short_ranks
         chosen_long_ranks = pr2_long_ranks
     else:
         logging.error("Incorrect database label - exiting.")
         exit(1)
 
     return chosen_short_ranks, chosen_long_ranks
 
 def parse_mapseq(mseq_df, short_ranks, long_ranks):
-
     res_dict = defaultdict(list)
 
     for i in range(len(mseq_df)):
         asv_id = mseq_df.iloc[i, 0]
-        tax_ass = mseq_df.iloc[i, 1].split(';')
 
-        res_dict['ASV'].append(asv_id)
-        
-        for j in range(len(short_ranks)):
+        if pd.isna(mseq_df.iloc[i, 1]):
+            tax_ass = [short_ranks[0]]
+        else:
+            tax_ass = mseq_df.iloc[i, 1].split(";")
+
+        res_dict["ASV"].append(asv_id)
 
+        for j in range(len(short_ranks)):
             curr_rank = long_ranks[j]
-            
+
             if j >= len(tax_ass):
                 # This would only be true if the assigned taxonomy is shorter than the total reference database taxononmy
                 # so fill each remaining rank with its respective short rank blank
                 curr_tax = short_ranks[j]
             else:
                 curr_tax = tax_ass[j]
-            
+
             res_dict[curr_rank].append(curr_tax)
     res_df = pd.DataFrame.from_dict(res_dict)
 
     return(res_df)
 
 def process_blank_tax_ends(res_df, ranks):
     # Necessary function as we want to replace consecutive blank assignments that start at the last rank as NAs
     # while avoiding making blanks in the middle as NAs
 
     for i in range(len(res_df)):
-        last_empty_rank = ''
+        last_empty_rank = ""
         currently_empty = False
-        for j in reversed(range(len(ranks))): # Parse an assignment backwards, from Species all the way to Superkingdom/Domain
-            curr_rank = res_df.iloc[i, j+1]
+        for j in reversed(
+            range(len(ranks))
+        ):  # Parse an assignment backwards, from Species all the way to Superkingdom/Domain
+            curr_rank = res_df.iloc[i, j + 1]
             if curr_rank in ranks:
-                if last_empty_rank == '': # Last rank is empty, start window of consecutive blanks 
-                    last_empty_rank = j+1
+                if last_empty_rank == "":  # Last rank is empty, start window of consecutive blanks
+                    last_empty_rank = j + 1
                     currently_empty = True
-                elif currently_empty: # If we're in a window of consecutive blank assignments that started at the beginning
-                    last_empty_rank = j+1
+                elif (
+                    currently_empty
+                ):  # If we're in a window of consecutive blank assignments that started at the beginning
+                    last_empty_rank = j + 1
                 else:
                     break
             else:
                 break
-        if last_empty_rank != '':
-            res_df.iloc[i, last_empty_rank:] = 'NA'
+        if last_empty_rank != "":
+            res_df.iloc[i, last_empty_rank:] = "NA"
+        if last_empty_rank == 1:
+            res_df.iloc[i, 1] = ranks[0]
 
     return res_df
 
-def main():
-    
+
+def main():    
     _INPUT, _LABEL, _SAMPLE = parse_args()
 
     mseq_df = pd.read_csv(_INPUT, header=1, delim_whitespace=True, usecols=[0, 12])
 
     short_ranks, long_ranks = parse_label(_LABEL)
     res_df = parse_mapseq(mseq_df, short_ranks, long_ranks)
     final_res_df = process_blank_tax_ends(res_df, short_ranks)
 
     final_res_df.to_csv(f"./{_SAMPLE}_{_LABEL}_asv_taxa.tsv", sep="\t", index=False)
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/remove_ambiguous_reads.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/remove_ambiguous_reads.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/rev_comp_se_primers.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/rev_comp_se_primers.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/amplicon/standard_primer_matching.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/amplicon/standard_primer_matching.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/get_subunits.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/shared/get_subunits.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/get_subunits_coords.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/shared/get_subunits_coords.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/analysis/shared/mapseq2biom.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/analysis/shared/mapseq2biom.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/regex_ambiguous_bases.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/constants/regex_ambiguous_bases.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/tax_ranks.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/constants/tax_ranks.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit/constants/thresholds.py` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit/constants/thresholds.py`

 * *Files identical despite different names*

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/PKG-INFO` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgnify_pipelines_toolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: Collection of scripts and tools for MGnify pipelines
 Author-email: MGnify team <metagenomics-help@ebi.ac.uk>
 License: Apache Software License 2.0
 Keywords: bioinformatics,pipelines,metagenomics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/SOURCES.txt` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 mgnify_pipelines_toolkit/analysis/amplicon/are_there_primers.py
 mgnify_pipelines_toolkit/analysis/amplicon/assess_inflection_point_mcp.py
 mgnify_pipelines_toolkit/analysis/amplicon/assess_mcp_proportions.py
 mgnify_pipelines_toolkit/analysis/amplicon/classify_var_regions.py
 mgnify_pipelines_toolkit/analysis/amplicon/find_mcp_inflection_points.py
 mgnify_pipelines_toolkit/analysis/amplicon/make_asv_count_table.py
 mgnify_pipelines_toolkit/analysis/amplicon/mapseq_to_asv_table.py
+mgnify_pipelines_toolkit/analysis/amplicon/primer_val_classification.py
 mgnify_pipelines_toolkit/analysis/amplicon/remove_ambiguous_reads.py
 mgnify_pipelines_toolkit/analysis/amplicon/rev_comp_se_primers.py
 mgnify_pipelines_toolkit/analysis/amplicon/standard_primer_matching.py
 mgnify_pipelines_toolkit/analysis/shared/__init__.py
 mgnify_pipelines_toolkit/analysis/shared/get_subunits.py
 mgnify_pipelines_toolkit/analysis/shared/get_subunits_coords.py
 mgnify_pipelines_toolkit/analysis/shared/mapseq2biom.py
```

### Comparing `mgnify_pipelines_toolkit-0.1.2/mgnify_pipelines_toolkit.egg-info/entry_points.txt` & `mgnify_pipelines_toolkit-0.1.3/mgnify_pipelines_toolkit.egg-info/entry_points.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,10 +5,11 @@
 classify_var_regions = mgnify_pipelines_toolkit.analysis.amplicon.classify_var_regions:main
 find_mcp_inflection_points = mgnify_pipelines_toolkit.analysis.amplicon.find_mcp_inflection_points:main
 get_subunits = mgnify_pipelines_toolkit.analysis.shared.get_subunits:main
 get_subunits_coords = mgnify_pipelines_toolkit.analysis.shared.get_subunits_coords:main
 make_asv_count_table = mgnify_pipelines_toolkit.analysis.amplicon.make_asv_count_table:main
 mapseq2biom = mgnify_pipelines_toolkit.analysis.shared.mapseq2biom:main
 mapseq_to_asv_table = mgnify_pipelines_toolkit.analysis.amplicon.mapseq_to_asv_table:main
+primer_val_classification = mgnify_pipelines_toolkit.analysis.amplicon.primer_val_classification:main
 remove_ambiguous_reads = mgnify_pipelines_toolkit.analysis.amplicon.remove_ambiguous_reads:main
 rev_comp_se_primers = mgnify_pipelines_toolkit.analysis.amplicon.rev_comp_se_primers:main
 standard_primer_matching = mgnify_pipelines_toolkit.analysis.amplicon.standard_primer_matching:main
```

### Comparing `mgnify_pipelines_toolkit-0.1.2/pyproject.toml` & `mgnify_pipelines_toolkit-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mgnify_pipelines_toolkit"
-version = "0.1.2"
+version = "0.1.3"
 readme = "README.md"
 license = {text = "Apache Software License 2.0"}
 authors = [
   { name = "MGnify team", email = "metagenomics-help@ebi.ac.uk" },
 ]
 keywords = ["bioinformatics", "pipelines", "metagenomics"]
 description = "Collection of scripts and tools for MGnify pipelines"
@@ -46,14 +46,15 @@
 classify_var_regions = "mgnify_pipelines_toolkit.analysis.amplicon.classify_var_regions:main"
 find_mcp_inflection_points = "mgnify_pipelines_toolkit.analysis.amplicon.find_mcp_inflection_points:main"
 make_asv_count_table = "mgnify_pipelines_toolkit.analysis.amplicon.make_asv_count_table:main"
 remove_ambiguous_reads = "mgnify_pipelines_toolkit.analysis.amplicon.remove_ambiguous_reads:main"
 rev_comp_se_primers = "mgnify_pipelines_toolkit.analysis.amplicon.rev_comp_se_primers:main"
 standard_primer_matching = "mgnify_pipelines_toolkit.analysis.amplicon.standard_primer_matching:main"
 mapseq_to_asv_table = "mgnify_pipelines_toolkit.analysis.amplicon.mapseq_to_asv_table:main"
+primer_val_classification = "mgnify_pipelines_toolkit.analysis.amplicon.primer_val_classification:main"
 
 [project.optional-dependencies]
 tests = [
     "pytest==7.4.0",
     "pytest-md==0.2.0",
     "pytest-workflow==2.0.1",
     "biopython==1.82",
```

