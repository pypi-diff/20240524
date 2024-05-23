# Comparing `tmp/climush-0.0.7.tar.gz` & `tmp/climush-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climush-0.0.7.tar", last modified: Mon Apr 22 22:20:56 2024, max compression
+gzip compressed data, was "climush-0.0.8.tar", last modified: Thu May 23 23:30:03 2024, max compression
```

## Comparing `climush-0.0.7.tar` & `climush-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-22 22:20:56.164366 climush-0.0.7/
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     2098 2024-04-22 22:20:56.164189 climush-0.0.7/PKG-INFO
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     1234 2024-04-04 09:14:41.000000 climush-0.0.7/README.md
-drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-22 22:20:56.163161 climush-0.0.7/climush/
--rw-r--r--   0 carolyndelevich   (501) staff       (20)      152 2024-04-07 02:45:45.000000 climush-0.0.7/climush/__init__.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)    24466 2024-02-03 09:44:16.000000 climush-0.0.7/climush/binfo_old.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)    64732 2024-04-22 21:54:33.000000 climush-0.0.7/climush/bioinfo.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)      380 2024-04-07 02:13:39.000000 climush-0.0.7/climush/config.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     1125 2024-03-12 03:14:02.000000 climush-0.0.7/climush/constants.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)    44331 2024-04-10 18:29:42.000000 climush-0.0.7/climush/utilities.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     5770 2024-02-23 04:02:34.000000 climush-0.0.7/climush/viz.py
-drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-22 22:20:56.164005 climush-0.0.7/climush.egg-info/
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     2098 2024-04-22 22:20:56.000000 climush-0.0.7/climush.egg-info/PKG-INFO
--rw-r--r--   0 carolyndelevich   (501) staff       (20)      313 2024-04-22 22:20:56.000000 climush-0.0.7/climush.egg-info/SOURCES.txt
--rw-r--r--   0 carolyndelevich   (501) staff       (20)        1 2024-04-22 22:20:56.000000 climush-0.0.7/climush.egg-info/dependency_links.txt
--rw-r--r--   0 carolyndelevich   (501) staff       (20)       50 2024-04-22 22:20:56.000000 climush-0.0.7/climush.egg-info/requires.txt
--rw-r--r--   0 carolyndelevich   (501) staff       (20)        8 2024-04-22 22:20:56.000000 climush-0.0.7/climush.egg-info/top_level.txt
--rw-r--r--   0 carolyndelevich   (501) staff       (20)      930 2024-04-22 22:19:36.000000 climush-0.0.7/pyproject.toml
--rw-r--r--   0 carolyndelevich   (501) staff       (20)       38 2024-04-22 22:20:56.164404 climush-0.0.7/setup.cfg
+drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-05-23 23:30:03.119679 climush-0.0.8/
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     2098 2024-05-23 23:30:03.119430 climush-0.0.8/PKG-INFO
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     1234 2024-04-04 09:14:41.000000 climush-0.0.8/README.md
+drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-05-23 23:30:03.118256 climush-0.0.8/climush/
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)      152 2024-04-07 02:45:45.000000 climush-0.0.8/climush/__init__.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)    24466 2024-02-03 09:44:16.000000 climush-0.0.8/climush/binfo_old.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)    78666 2024-05-21 22:12:43.000000 climush-0.0.8/climush/bioinfo.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)      380 2024-04-07 02:13:39.000000 climush-0.0.8/climush/config.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     4504 2024-05-09 21:44:54.000000 climush-0.0.8/climush/constants.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     3579 2024-04-28 22:34:49.000000 climush-0.0.8/climush/mapping.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)    64790 2024-05-23 22:17:21.000000 climush-0.0.8/climush/utilities.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     5770 2024-02-23 04:02:34.000000 climush-0.0.8/climush/viz.py
+drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-05-23 23:30:03.119188 climush-0.0.8/climush.egg-info/
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     2098 2024-05-23 23:30:03.000000 climush-0.0.8/climush.egg-info/PKG-INFO
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)      332 2024-05-23 23:30:03.000000 climush-0.0.8/climush.egg-info/SOURCES.txt
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)        1 2024-05-23 23:30:03.000000 climush-0.0.8/climush.egg-info/dependency_links.txt
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)       50 2024-05-23 23:30:03.000000 climush-0.0.8/climush.egg-info/requires.txt
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)        8 2024-05-23 23:30:03.000000 climush-0.0.8/climush.egg-info/top_level.txt
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     1553 2024-05-23 23:29:56.000000 climush-0.0.8/pyproject.toml
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)       38 2024-05-23 23:30:03.119730 climush-0.0.8/setup.cfg
```

### Comparing `climush-0.0.7/PKG-INFO` & `climush-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climush
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tools to run the CliMush bioinformatics pipeline.
 Author-email: Carolyn Delevich <cdelevic@uoregon.edu>
 Project-URL: Homepage, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline
 Project-URL: Repository, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline/climush_py-package
 Project-URL: Issues, https://github.com/cdelevich/climush/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `climush-0.0.7/README.md` & `climush-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `climush-0.0.7/climush/binfo_old.py` & `climush-0.0.8/climush/binfo_old.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.7/climush/bioinfo.py` & `climush-0.0.8/climush/bioinfo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import json, re
 from pathlib import Path
 from Bio.Seq import Seq
 from datetime import datetime
-import re
 from Bio import SeqIO
 from Bio.SeqRecord import SeqRecord
 import pandas as pd
-from climush.constants import NOPHIX_PREFIX, SEQ_FILE_GLOB, TRIMMED_PREFIX, DEREP_PREFIX, QUALFILT_PREFIX
+import numpy as np
+from climush.constants import *
 from climush.utilities import *
 
-def demultiplex(file_map, multiplexed_files, settings_dict, seq_platform='pacbio'):
+def demultiplex(output_dir, file_map, multiplexed_files, seq_platform='pacbio'):
 
     # REMOVE AFTER TESTING ############
     # DON'T FORGET TO UNCOMMENT THE RUN_SUBPROCESS LINE WHERE LIMA ACTUALLY RUNS!!! #################
     # file_map = fpm.copy()
     # multiplexed_files = pacbio_files
     # settings_dict = settings.copy()
     # seq_platform = 'pacbio'
@@ -23,21 +24,16 @@
 
     # DEFINE RELEVANT FILE PATHS ####################################################################
     # get the paths needed for demux
     mapping_dir = file_map['config']['bc_mapping']  # directory containing all mapping files
     mapping_files = list(mapping_dir.glob('*'))  # get mapping files, as list (will reuse + exhaust)
 
     # ACCESS USER SETTINGS FROM CONFIG ##############################################################
-    run_name = settings_dict['run_details']['run_name']  # name to use for this bioinformatics run
-
-    # CONSTRUCT REGEX CONSTANTS #####################################################################
-    # column name regex; column names vary among mapping files
-    FWD_COL_RE = '(fwd)|(forward)'
-    REV_COL_RE = '(rev)|(reverse)'
-    SAMPLE_ID_RE = '^sample'
+    settings = get_settings(file_map)
+    run_name = settings['run_details']['run_name']  # name to use for this bioinformatics run
 
     # CONFIRM THAT PLATFORM IS PACBIO ###############################################################
     # check that the sequence platform is set to pacbio; not suitable for others platforms right now
     if not seq_platform == 'pacbio':
         print(f'Currently, this function only accepts PacBio sequences. Not suited for demultiplexing Sanger or '
               f'Illumina sequences.\n')
         sys.exit()
@@ -48,17 +44,17 @@
 
     # link multiplexed sequence files in needs_demux to their corresponding mapping file in config directory
     demux_mapping = {}  # key is mapping file path, value(s) is sequence file path in needs_demux dir
 
     for mp_file in multiplexed_files:
 
         # get the sequencing core's queue ID from multiplexed seq file and corresponding climush sample ID for this queue ID
-        qid = re.search('^(\d{4})', mp_file.name).group(0)  # get queue ID from file name
+        qid = re.search(r'^(\d{4})', mp_file.name).group(0)  # get queue ID from file name
         queue_ids.add(qid)  # add the qid to the set of all queue ids requiring demux
-        cid = settings_dict['pacbio_demultiplexing']['multiplex'][qid]  # get climush - queue ID pairing from config
+        cid = settings['demultiplex']['multiplex'][qid]  # get climush - queue ID pairing from config
         qid_files = [f for f in mapping_files if
                      re.search(f'^{cid}', f.name)]  # all files in mapping files dir that match climush id
 
         if len(qid_files) == 1:  # should only be one mapping file; because only 1, will also be key in dict
             if qid_files[0] in demux_mapping.keys():  # if already in dict (e.g., Pool1/Pool2)
                 demux_mapping[qid_files[0]].append(mp_file)  # update list of corresponding multiplexed files w/ str
             else:
@@ -68,15 +64,16 @@
                   f'{mapping_dir.parent.name + "/" + mapping_dir.name}. Please check that a mapping file for collection '
                   f'{cid} is present in this directory, and that the CliMush collection ID ({cid}) is at the start of the '
                   f'file name (e.g., {cid + "_mapping-file.xlsx"}).\n')
         else:  # if multiple mapping files for a given queue ID
             print(f'{len(qid_files)} mapping files were located in {mapping_dir.parent.name + "/" + mapping_dir.name}. '
                   f'Please select the number corresponding to the correct file to use for the multiplexed sequencing '
                   f'file {cid}, or type \'quit\'.\n')
-            right_map = prompt_print_options(qid_files)  # get right mapping file from user input
+            right_map = prompt_print_options(qid_files,
+                                             auto_respond=settings['automate']['auto_respond'])  # get right mapping file from user input
             if right_map in demux_mapping.keys():  # add to dict
                 demux_mapping[right_map].append(mp_file)  # update list of corresponding multiplexed files w/ str
             else:
                 demux_mapping.update({right_map: [mp_file]})  # add queue ID and first multiplexed file as list
 
     # CREATE A FASTA FILE OF ALL UNIQUE BARCODES USED TO MULTIPLEX ###################################
     # define subfunctions to help locate and prepare barcodes for demultiplexing
@@ -111,31 +108,31 @@
         rev_barcodes = []
 
         # read in mapping file based on file type (.xlsx, .csv, .txt)
         mapping_tabs = import_mapping_df(df_path=map_path)
 
         # go through each tab in the df and get the barcodes
         for tab in mapping_tabs:  # go through each tab...
-            if re.search('pool', tab, re.I):  # ...only if relevant to mapping/demux
+            if re.search(r'pool', tab, re.I):  # ...only if relevant to mapping/demux
 
                 # get the name used for the fwd/rev barcode columns in this mapping file
                 fwd_col = get_col_name(FWD_COL_RE, mapping_tabs[tab])
                 rev_col = get_col_name(REV_COL_RE, mapping_tabs[tab])
 
                 # get list of values for barcodes and sample IDs
                 fwd_bc = mapping_tabs[tab][fwd_col].to_list()
                 rev_bc = mapping_tabs[tab][rev_col].to_list()
 
                 # add all barcodes in the column to the total barcode list
                 fwd_barcodes.extend(fwd_bc)  # add bc to the total list
                 rev_barcodes.extend(rev_bc)  # use extend to prevent sublists
 
         # make sure that the barcodes don't contain the primer sequences; if they do, remove primer sequence from bc
-        fwd_bc_noprimer = [re.sub(f'{primers["fwd_primer"]}$', '', fwd) for fwd in fwd_barcodes]
-        rev_bc_noprimer = [re.sub(f'{primers["rev_primer"]}$', '', rev) for rev in rev_barcodes]
+        fwd_bc_noprimer = [re.sub(f'{primers["fwd_primer"]}$', r'', fwd) for fwd in fwd_barcodes]
+        rev_bc_noprimer = [re.sub(f'{primers["rev_primer"]}$', r'', rev) for rev in rev_barcodes]
 
         # confirm that primers were properly removed from the barcodes
         def primers_removed_from_bc(pre_remove_list, post_remove_list, primer):
 
             # OBSERVED
             # get the length of each barcode after removing the primer; keep only unique length values
             len_bc_noprimer = list(set(len(f) for f in post_remove_list))
@@ -186,16 +183,16 @@
             print(f'\tprimer properly removed from...')
             print(f'\t  forward barcodes: {fwd_bc_ready}')
             print(f'\t  reverse barcodes: {rev_bc_ready}')
             return sys.exit()  # exit
 
     # get the fwd/rev primers, since they are sometimes included in the barcode sequence and need to be removed
     primer_dict = {}
-    primer_dict['fwd_primer'] = settings_dict['primers']['fwd']['sequence']['pacbio']
-    primer_dict['rev_primer'] = settings_dict['primers']['rev']['sequence']['pacbio']
+    primer_dict['fwd_primer'] = settings['primers']['fwd']['sequence']['pacbio']
+    primer_dict['rev_primer'] = settings['primers']['rev']['sequence']['pacbio']
 
     # create a dict to add all barcodes to; will be used to create the unique barcode fasta
     unique_barcodes = {'fwd_bc': set(),
                        'rev_bc': set()}
 
     # aggregate all barcodes from the mapping files that belong to the multiplexed sequences that need demux
     for dxmap in demux_mapping:
@@ -234,15 +231,15 @@
                     pass  # they are equal, as expected
 
             # regardless of above outcome, add barcodes from this mapping file to the overall dict of unique barcodes
             unique_barcodes[b].update(seq_run_bc[b])  # use update to add list to set
 
     # write out fasta file of unique barcodes; must be ordered so same numbering is used every time this is run
     # create new path in pipeline output, and use this path to create fasta file name
-    fasta_out_dir = mkdir_exist_ok(new_dir = 'barcodes', parent_dir = file_map['pipeline-output']['demultiplexed'])
+    fasta_out_dir = mkdir_exist_ok(new_dir = 'barcodes', parent_dir = output_dir)
     barcode_fasta = (fasta_out_dir / f'barcodes_{run_name}').with_suffix('.fasta')
 
     # create a dictionary with the barcode seq as the key and the value is the ID name (header) in the output fasta file
     unique_barcode_labels = {}
     bc_name_index = {}
 
     fasta_index = 0
@@ -265,73 +262,74 @@
 
                 # add barcode name and its index to the bc name index dictionary
                 bc_name_index.update({fasta_index: bc_name})
                 fasta_index += 1  # have to use counter because pulling from two sources, will reset to 0 for rev bc
 
     # DEMULTIPLEX USING LIMA #############################################################################
     # create a directory for the output files that lima produces
-    lima_output = mkdir_exist_ok(new_dir='lima_output', parent_dir=file_map['pipeline-output']['demultiplexed'])
+    lima_output = mkdir_exist_ok(new_dir='lima_output', parent_dir=output_dir)
     lima_subdirs = []  # create list of output directories to read lima output from later on
 
     for qid in queue_ids:
 
         # get the climush sequencing run ID that corresponds to this queue ID
-        seq_run = settings_dict['pacbio_demultiplexing']['multiplex'][qid]
+        seq_run = settings['demultiplex']['multiplex'][qid]
 
         # create an output directory for this sequencing run using the climush sequencing run ID
         seq_run_output = mkdir_exist_ok(new_dir=seq_run, parent_dir=lima_output) # create an output dir for each seq run
         lima_subdirs.append(seq_run_output)
 
         # located all multiplexed sequencing files that match this queue ID
         pools_to_demux = [f for f in multiplexed_files if re.search(f'^{qid}', f.name)]
 
         # alert if only one pool is detected
         if len(pools_to_demux) == 1:
             msg = f'WARNING. There is only one multiplexed sequencing file ({pools_to_demux[0].name}) for sequencing ' \
                   f'run {seq_run} when two are typically expected: one for each pool of sequences that were ' \
                   f'sequenced simultaneously on separate SMRT cells. Do you wish to continue with only half of the ' \
                   f'sequences from this sequencing run?'  # yes/no/quit automatically added by function
-            prompt_yes_no_quit(msg)  # if yes, auto-continues; if no or quit, exits
+            prompt_yes_no_quit(msg, auto_respond=settings['automate']['auto_respond'])  # if yes, auto-continues; if no or quit, exits
 
         for pool in pools_to_demux:
 
             # detect pool number from the file name; remove queue ID first to avoid any confusion
             try:  # should be able to do automatically
-                pool_num = re.search('\d', re.sub(f'^{qid}\.', '', pool.name)).group(0)
+                pool_num = re.search(r'\d', re.sub(f'^{qid}' + r'\.', r'', pool.name)).group(0)
             except AttributeError:  # but if re.search does not return a match
                 print(f'The sequencing pool number for the multiplexed file {pool.name} could not be detected in ' \
                       f'the file name. Please enter the pool number corresponding to this file as a single digit'
                       f'(i.e., no leading zeros or decimals): ')
                 pool_num = input()
 
             # define prefix to use for lima output files; include path to the output directory for this seq run
-            out_prefix = seq_run_output / f'lima-demux_{seq_run}_pool{pool_num}'
+            out_prefix = (seq_run_output / f'lima-demux_{seq_run}_pool{pool_num}').with_suffix('.fasta')
 
             # assemble list of commands required to run lima demultiplexing
             lima_cmd = ['lima', pool, barcode_fasta, out_prefix, '--min-score', '93', '--hifi-preset', 'ASYMMETRIC']
 
-            run_subprocess(cli_command_list = lima_cmd, dest_dir = lima_output)
+            run_subprocess(cli_command_list = lima_cmd, dest_dir = lima_output,
+                           auto_respond = settings['automate']['auto_respond'])
 
     # CREATE DICTIONARY OF BARCODE PAIRS FOR ALL SAMPLES
     sample_barcodes = {q:{'pool1': {},
                           'pool2': {}} for q in queue_ids}
 
     for dxmap in demux_mapping:
 
         # get the queue ID from the name of the multiplexed sequencing file; need it to find key in sample_barcodes
-        qid = re.search('^(\d{4})', list(demux_mapping[dxmap])[0].name).group(0)
+        qid = re.search(r'^(\d{4})', list(demux_mapping[dxmap])[0].name).group(0)
 
         # import the mapping file dataframe
-        mapping_df = import_mapping_df(df_path=dxmap)
+        mapping_df = import_mapping_df(df_path=dxmap, auto_respond=settings['automate']['auto_respond'])
 
         # loop through each tab (= pool1/pool2) in the df to get the sample ID and its barcode combo
         for tab in mapping_df:
 
             # get the name of the column used for the sample ID, fwd barcode, rev barcode
-            smp_col = get_col_name(pattern=SAMPLE_ID_RE, df=mapping_df[tab])
+            smp_col = get_col_name(pattern=SAMPLE_COL_RE, df=mapping_df[tab])
             fwd_col = get_col_name(pattern=FWD_COL_RE, df=mapping_df[tab])
             rev_col = get_col_name(pattern=REV_COL_RE, df=mapping_df[tab])
 
             for i in range(mapping_df[tab].shape[0]):
 
                 # from the dataframe, get the sample ID, fwd barcode sequence, and rev barcode sequence
                 smp_id = mapping_df[tab][smp_col][i]
@@ -355,47 +353,44 @@
     # dictionary for read sequences w/ barcodes removed
     read_seqs = {q:{'pool1': {},
                     'pool2': {}} for q in queue_ids}
 
     for subdir in lima_subdirs:
 
         # get the queue ID from the name of the multiplexed sequencing file; need it to find key in sample_barcodes
-        cid = re.search('^pacbio.+', subdir.name).group(0)  # get climush ID, which will be in name of file
-        mp_dict = settings_dict['pacbio_demultiplexing']['multiplex']  # make shorter for list comp below
+        cid = re.search(r'^pacbio.+', subdir.name).group(0)  # get climush ID, which will be in name of file
+        mp_dict = settings['demultiplex']['multiplex']  # make shorter for list comp below
         qid = [k for k in mp_dict if cid in mp_dict[k]][0]  # convert to qid to match dict
 
         for p in ['pool1', 'pool2']:
 
             # find the fasta file for this pool, which has the read ID and the barcode combination
-            lima_fasta = [f for f in subdir.glob('*.*') if re.search(f'{subdir.name}_{p}\.fasta', f.name, re.I)][0]
+            lima_fasta = [f for f in subdir.glob('*.*') if re.search(f'{subdir.name}_{p}' + r'\.fasta', f.name, re.I)][0]
 
             # open the fasta file and pull the indices of the forward and reverse barcodes
             with open(lima_fasta, 'r') as fin:
                 fasta_txt = fin.readlines()
                 for l, line in enumerate(fasta_txt):
                     if line.startswith('>'):
-                        read_id = re.findall('(?<=>).+?(?=\sbc)', line, re.I)[0]
-                        read_barcode_i = list(map(int, re.search('(?<=bc=)\d{1,2},\d{1,2}', line, re.I).group(0).split(',')))
+                        read_id = re.findall(r'(?<=>).+?(?=\sbc)', line, re.I)[0]
+                        read_barcode_i = list(map(int, re.search(r'(?<=bc=)\d{1,2},\d{1,2}', line, re.I).group(0).split(',')))
                         read_bc_names = [bc_name_index[i] for i in read_barcode_i]  # convert index to name
                         read_barcodes[qid][p].update({read_id: read_bc_names})  # add read's bc names to dict
                         read_seqs[qid][p].update({read_id: fasta_txt[l+1]})  # add read sequence to dict
                     else:
                         continue
 
     # COMPARE LIMA BARCODE COMBINATIONS TO MAPPING FILE BARCODE COMBINATIONS
 
     # create an output subdirectory in demultiplexed dir for all demultiplexed reads in this bioinformatics run
-    demux_dir = mkdir_exist_ok(new_dir = f'demux_{run_name}', parent_dir=file_map['pipeline-output']['demultiplexed'])
+    demux_dir = mkdir_exist_ok(new_dir = f'{DEMUX_PREFIX}_{run_name}', parent_dir=output_dir)
 
     # for each sequencing run...
     for qid in read_barcodes:
 
-        # get the name of the sequencing run for labeling the output and read headers
-        seq_run = settings['pacbio_demultiplexing']['multiplex'][qid]
-
         # for each pool in this sequencing run...
         for p in ['pool1', 'pool2']:
 
             # subset dictionary for this seq run/pool, makes more succinct code below
             sample_subdict = sample_barcodes[qid][p]
 
             # subset dictionary for this seq run/pool of read ID and barcode-free sequences from lima fasta output
@@ -413,372 +408,628 @@
                 # confirm that the read's barcode combination matches only one sample ID, as it should
                 if len(sample_ids) == 1:
 
                     # get sample ID as string, not list (now that it is confirmed there's only one)
                     sample_id = sample_ids[0]
 
                     # create read ID header from sequencing run, sample ID, and last part of original read header
-                    full_sample_id = '_'.join([seq_run, sample_id])
+                    full_sample_id = '_'.join([seq_run, str(sample_id)])  # sample ID is int (?) debugging...
                     read_id = '_'.join([full_sample_id, r.split('/')[-2]])
 
                     # get the barcode-free sequence for this read
                     read_seq = seq_subdict[r]
 
                     # write the read ID and read sequence to the sample ID demultiplexed fasta file
-                    sample_fasta = (demux_dir / f'demux_{full_sample_id}').with_suffix('.fasta')
+                    sample_fasta = (demux_dir / f'{DEMUX_PREFIX}_{full_sample_id}').with_suffix('.fasta')
                     with open(sample_fasta, 'a') as fout:
                         fout.write(f'>{read_id}\n')
                         fout.write(f'{read_seq}\n')
 
                 else:
                     print(f'ERROR. The barcode combination detected in read {r} from {p} of {seq_run} matched to '
                           f'{len(sample_ids)} sample IDs, when it should only match to one. This read was not '
                           f'sorted, and this error was recorded to the error table.\n')
-                    barcode_error = (file_map['pipeline-output']['demultiplexed'] / 'barcode_errors').with_suffix('.tsv')
+                    barcode_error = (output_dir / 'barcode_errors').with_suffix('.tsv')
 
                     # if the error file doesn't yet exist, start with writing the header
                     if not barcode_error.is_file():
                         with open(barcode_error, 'a') as fout:
                             fout.write(f'sequencing_run\tsequencing_pool\tsample_ids\tread_id\tbarcode_combination\n')
 
                     # write out details of the read that triggered this error
                     with open(barcode_error, 'a') as fout:
                         fout.write(f'{seq_run}\t{p}\t{", ".join(sample_ids)}\t{r}\t{", ".join(bc_list)}\n')
 
-def filter_out_phix(input_files, file_map, kmer=31, hdist=1, keep_log=True, keep_removed_seqs=True):
+def pair_reads(input_files):
 
-    prefilt_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output']['prefiltered'])
+    pairs_dict = {}
+    rev_reads = []
 
-    run_name = import_config_as_dict(file_path=file_map['config']['main'], file_handle='pipeline-settings',
-                                     config_section='run_details')['run_name']
+    for file in input_files:
+        # if the file is an R1 read file...
+        if re.search(r'R1', file.stem, re.I):
+            pairs_dict.update({file:''})  # add to dict, with empty str as value
+        # if the file is an R2 read file...
+        elif re.search(r'R2', file.stem, re.I):
+            rev_reads.append(file)  # add to a list, will sort to match its R1 file next
+        # if an R1/R2 tag is not detected
+        else:
+            pairs_dict.update({file:''})  # add to dict with an empty str as value, will remain w/o paired file
 
-    nophix_path = mkdir_exist_ok(new_dir=f'./{NOPHIX_PREFIX}_{run_name}', parent_dir=prefilt_parent)
-    phix_path = mkdir_exist_ok(new_dir=f'./{flip_prefix(NOPHIX_PREFIX)}_{run_name}', parent_dir=prefilt_parent)
+    # if any reverse reads are detected...
+    if len(rev_reads) > 0:
+        for rev in rev_reads:
+            # find their associated R1 file, and match these in the dict
+            sample_id = re.search(r'.+?(?=_R2)', rev.stem).group(0)
+            for k in pairs_dict.keys():
+                if re.search(sample_id, k.stem, re.I):
+                    pairs_dict[k] = rev
 
-    bbduk_log = make_log_file(file_name=Path('bbduk'), dest_path=prefilt_parent)
+    return pairs_dict
 
-    for file in input_files:
+def filter_out_phix(input_files, file_map, kmer=31, hdist=1, keep_log=True, keep_removed_seqs=True):
 
-        nophix_out = add_prefix(file_path=file, prefix=NOPHIX_PREFIX, action=None, dest_dir=nophix_path)
-        phix_out = add_prefix(file_path=file, prefix=flip_prefix(NOPHIX_PREFIX), action=None, dest_dir=phix_path)
+    # make sure parent directory exists/is created before making child
+    mkdir_exist_ok(new_dir=file_map['pipeline-output']['prefiltered']['main'])
+    phix_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output']['prefiltered']['prefilt01_no-phix'])
 
-        # bbduk does not like special characters in file path
-        # nophix_out_str = escape_path_special(nophix_out)
-        # phix_out_str = escape_path_special(phix_out)
-        # and this didn't help it work either...
+    # load in the configuration settings
+    settings = get_settings(file_map=file_map)
+    run_name = settings['run_details']['run_name']
 
-        bbduk_cmd = ['bbduk.sh', f'in={file}', f'out={nophix_out}', f'out={phix_out}',
-                     'ref=phix.fa', f'k={kmer}', f'hdist={hdist}', f'stats={bbduk_log}']
+    # create a parent directory to sort reads w/ and reads w/o PhiX into
+    nophix_path = mkdir_exist_ok(new_dir=f'./{NOPHIX_PREFIX}_{run_name}', parent_dir=phix_parent)
+    phix_path = mkdir_exist_ok(new_dir=f'./{flip_prefix(NOPHIX_PREFIX)}_{run_name}', parent_dir=phix_parent)
 
-        try:
-            run_subprocess(bbduk_cmd, dest_dir=prefilt_parent)
-        except:
-            continue
+    # create a log file
+    # bbduk_log = make_log_file(file_name=Path('bbduk'), dest_path=phix_parent)
 
+    # create pairs of R1/R2 reads in order to detect PhiX pair-wise (required)
+    pairs_dict = pair_reads(input_files)
 
-    if not check_for_input(nophix_path)[0]:  # this is a temporary work around to make copies that look like output while there's a curernt issue with Java
-        for file in input_files:
-            add_prefix(file_path=file, prefix=NOPHIX_PREFIX, action='copy', dest_dir=nophix_path)
+    for input_fwd, input_rev in pairs_dict.items():
 
-    return nophix_path
+        # format the output files based on the input files
+        # fwd (R1)
+        nophix_fwd_out = add_prefix(file_path=input_fwd, prefix=NOPHIX_PREFIX, action=None, dest_dir=nophix_path)
+        phix_fwd_out = add_prefix(file_path=input_fwd, prefix=flip_prefix(NOPHIX_PREFIX), action=None, dest_dir=phix_path)
+
+        # rev (R2)
+        nophix_rev_out = add_prefix(file_path=input_rev, prefix=NOPHIX_PREFIX, action=None, dest_dir=nophix_path)
+        phix_rev_out = add_prefix(file_path=input_rev, prefix=flip_prefix(NOPHIX_PREFIX), action=None, dest_dir=phix_path)
+
+        bbduk_cmd = ['bbduk.sh',
+                     f'in1={input_fwd}', f'out1={nophix_fwd_out}', f'outm1={phix_fwd_out}',
+                     f'in2={input_rev}', f'out2={nophix_rev_out}', f'outm2={phix_rev_out}',
+                     'ref=phix', f'k={kmer}', f'hdist={hdist}']
 
-def pair_reads(input_files):
-    pairs_dict = {}
-    rev_reads = []
-    for file in input_files:
-        if re.search('R1', file.stem, re.I):
-            pairs_dict.update({file:''})
-        else:
-            rev_reads.append(file)
-
-    for rev in rev_reads:
-        sample_id = re.search('.+?(?=_R2)', rev.stem).group(0)
-        for k in pairs_dict.keys():
-            if re.search(sample_id, k.stem, re.I):
-                pairs_dict[k] = rev
+        run_subprocess(bbduk_cmd, dest_dir=phix_parent, auto_respond=settings['automate']['auto_respond'])
 
-    return pairs_dict
+    return nophix_path
 
 def prefilter_fastx(input_files, file_map, maxn=0):
-    prefilt_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output']['prefiltered'])
+    # make sure parent directory exists/is created before making child
+    mkdir_exist_ok(new_dir=file_map['pipeline-output']['prefiltered']['main'])
+    noambig_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output']['prefiltered']['prefilt02_no-ambig'])
 
-    run_name = import_config_as_dict(file_path=file_map['config']['main'], file_handle='pipeline-settings',
-                                     config_section='run_details')['run_name']
+    settings = get_settings(file_map=file_map)
+    run_name = settings['run_details']['run_name']
 
-    noambig_path = mkdir_exist_ok(new_dir=f'./{NOAMBIG_PREFIX}_{run_name}', parent_dir=prefilt_parent)
-    ambig_path = mkdir_exist_ok(new_dir=f'./{flip_prefix(NOAMBIG_PREFIX)}_{run_name}', parent_dir=prefilt_parent)
+    noambig_path = mkdir_exist_ok(new_dir=f'./{NOAMBIG_PREFIX}_{run_name}', parent_dir=noambig_parent)
+    ambig_path = mkdir_exist_ok(new_dir=f'./{flip_prefix(NOAMBIG_PREFIX)}_{run_name}', parent_dir=noambig_parent)
 
-    fastq_maxns_log = make_log_file(file_name=Path('fastq_maxns'), dest_path=prefilt_parent)
+    fastq_maxns_log = make_log_file(file_name=Path('fastq_maxns'), dest_path=noambig_parent)
 
     # must provide pair of forward and reverse:
     pairs_dict = pair_reads(input_files)
 
     for file in pairs_dict.keys():
 
-        noambig_out_fwd = add_prefix(file_path=file, prefix=NOAMBIG_PREFIX, action=None, dest_dir=noambig_path)
-        noambig_out_rev = add_prefix(file_path=pairs_dict[file], prefix=NOAMBIG_PREFIX, action=None,
-                                     dest_dir=noambig_path)
-        ambig_out_fwd = add_prefix(file_path=file, prefix=flip_prefix(NOAMBIG_PREFIX), action=None,
-                                   dest_dir=ambig_path)
-        ambig_out_rev = add_prefix(file_path=pairs_dict[file], prefix=flip_prefix(NOAMBIG_PREFIX), action=None,
-                                   dest_dir=ambig_path)
+        # file paths post-compression, with .fastq.gz file extension
+        noambig_out_fwd_gzip = add_prefix(file_path=file, prefix=NOAMBIG_PREFIX, action=None, dest_dir=noambig_path)
+        noambig_out_rev_gzip = add_prefix(file_path=pairs_dict[file], prefix=NOAMBIG_PREFIX, action=None,
+                                          dest_dir=noambig_path)
+
+        ambig_out_fwd_gzip = add_prefix(file_path=file, prefix=flip_prefix(NOAMBIG_PREFIX), action=None,
+                                        dest_dir=ambig_path)
+        ambig_out_rev_gzip = add_prefix(file_path=pairs_dict[file], prefix=flip_prefix(NOAMBIG_PREFIX), action=None,
+                                        dest_dir=ambig_path)
+
+        # file paths pre-compression, with .fastq file extension, to use for VSEARCH cmd output paths
+        noambig_out_fwd = noambig_out_fwd_gzip.with_suffix('')
+        noambig_out_rev = noambig_out_rev_gzip.with_suffix('')
+
+        ambig_out_fwd = ambig_out_fwd_gzip.with_suffix('')
+        ambig_out_rev = ambig_out_rev_gzip.with_suffix('')
 
+        # compile CLI command for VSEARCH filtering of reads with any ambiguous bases
         vsearch_cmd = ['vsearch', '--fastq_filter', file, '--reverse', pairs_dict[file], '--fastq_maxns', str(maxn),
                        '--fastqout', noambig_out_fwd, '--fastqout_rev', noambig_out_rev, '--fastqout_discarded',
                        ambig_out_fwd, '--fastqout_discarded_rev', ambig_out_rev]
 
-        run_subprocess(vsearch_cmd, dest_dir=prefilt_parent)
+        # run CLI VSEARCH command
+        run_subprocess(vsearch_cmd, dest_dir=noambig_parent, auto_respond=settings['automate']['auto_respond'])
+
+        # compress the .fastq output from VSEARCH to .fastq.gz format; required for cutadapt input
+        # UNDER CONSTRUCTION
 
     return noambig_path
 
-def identify_primers(platform, config_dict):
+def identify_primers(platform, config_dict, verbose=True):
     primer_dict = config_dict['primers']
 
     target_primers = {}
     primer_names = []
     for d in primer_dict.keys():
         target_primers[d] = primer_dict[d]['sequence'][platform]
         primer_names.append(primer_dict[d]['name'][platform])
 
-    print(f'Searching for {primer_names[0]} and {primer_names[1]} in {platform.title()} reads...\n')
+    # add the reverse complement of each primer to this dict
+    target_primers['fwd_rc'] = str(Seq(target_primers['fwd']).reverse_complement())
+    target_primers['rev_rc'] = str(Seq(target_primers['rev']).reverse_complement())
+
+    if verbose:
+        print(f'Searching for {primer_names[0]} and {primer_names[1]} in {platform.title()} reads...\n')
 
     return target_primers
 
-def remove_primers(input_files, file_map, platform, paired_end=True):
+def confirm_no_primers(input_files, file_map, platform):
+
+    # if directory path provided, create generator of file paths
+    if input_files.is_dir():
+        input_files = input_files.glob(SEQ_FILE_GLOB)
+
+    # read in settings from the configuration file
+    settings = get_settings(file_map)
+    run_name = settings['run_details']['run_name']
+
+    # create a regex from fwd, rev, fwd_rc, and rev_rc primer sequences, to confirm no primer remains
+    primer_dict = identify_primers(platform, config_dict=settings, verbose=False)  # read in primer dict for this platform
+    # join the primer seq strings together with the 'or' pipe for regex search
+    primer_re = '|'.join(list(primer_dict.values()))  # will search for any of these primers/orients
+
+    # record read lengths to an output .json file
+    read_info_json = (file_map['pipeline-output']['primers-trimmed'] / f'{run_name}_read-info').with_suffix('.json')
+
+    # record primer detections to a .json log file
+    primer_detected_json = (file_map['pipeline-output']['primers-trimmed'] / f'{run_name}_detected-primers').with_suffix('.json')
+
+    # create an empty dictionary, whose contents will later be writen out to .json log
+    read_info_dict = {}  # for recording read count and read lengths per sample
+    p_detect_dict = {}  # for recording detection of primers in seqs
+    primers_detected = 0  # keep track of how many reads had primers detected
+    err_samples = set()  # keep track of how many samples had primers detected
+    total_samples = 0  # counter for total number of samples, since input_files is a generator, can't get len later
+    # go through each input file
+    for file in input_files:
+        total_samples += 1
+
+        # get the sample ID and add it to the .json dict as key, with empty values for read count + len
+        sample_id = get_sample_id(file, platform=platform)
+
+        # get the read orientation, i.e., R1 is fwd and R2 is rev
+        orient = get_read_orient(file)
+
+        # check if there are entries yet for these values; if not, add
+        if sample_id in read_info_dict.keys():  # if the sample_id is already in dict...
+            if orient in read_info_dict[sample_id]:  # and the orientation is too...
+                update = True  # set update var to True to inform how to add info for each read
+            else:  # if the sample_id is in dict, but the orient is not...
+                # add a nested dict for that orient
+                read_info_dict[sample_id].update({orient: {}})
+        else:  # if the sample_id is NOT in dict...
+            # add it to the dict, with the subdict for the orientation
+            read_info_dict[sample_id] = {orient: {}}
+
+        # create an empty list to append read lengths to for this sample
+        # easier to append vals to an empty list than an empty array
+        read_lens = []
+
+        # go through each read in this sample...
+        for seq in SeqIO.parse(file, 'fastq'):
+
+            # append the sequence length to the .json output
+            read_lens.append(len(seq))
+
+            # confirm that the primers in all orientations are not detected in the read
+            found = re.search(primer_re, str(seq), re.I)
+
+            if found:  # if a primer is detected..
+
+                primers_detected += 1  # add to error reads counter
+                err_samples.add(sample_id)  # add error sample id to err sample set
+
+                # first, create dict for just this read
+                err_read_dict = {seq.id.split(':')[-1]:{'seq_id': seq.id,  # full read ID
+                                                        'primer_id': [v[0] for v in primer_dict.items() if v[1] == found.group()][0],  # whether fwd/rev/fwd_rc/rev_rc primer
+                                                        'primer_seq': found.group(),  # sequence of detected primer
+                                                        'pos_start': found.span()[0],  # pos of primer start in seq
+                                                        'pos_end': found.span()[1],  # pos of primer end in seq
+                                                        'read_len': len(seq)}  # total len of read
+                                 }
+
+                # then check whether to create new entry, or update existing one
+                # if this sample already has an entry in the primer detect dict...
+                if sample_id in p_detect_dict.keys():
+                    # check if this read orientation (R1/R2) is already in primer detect dict...
+                    if orient in p_detect_dict[sample_id]:
+                        # if it is, update with the error info for this read
+                        p_detect_dict[sample_id][orient].update(err_read_dict)
+                    else:
+                        # if not, then add as new entry
+                        p_detect_dict[sample_id][orient] = err_read_dict
+                # if sample not yet in dict, add sample_id and orient together
+                else:
+                    p_detect_dict[sample_id] = {orient: err_read_dict}
+
+        # calculate summary information for each sample based on the lengths of each read
+        read_len_arr = np.array(read_lens)
+
+        # calculate all read metrics for this sample based on this array
+        # cannot have np values written to JSON, so convert to regular non-numpy int/float
+        sample_read_summary = {'read_count': int(read_len_arr.shape[0]),
+                               'read_len_mean': float(np.mean(read_len_arr).round(2)),
+                               'read_len_std': float(np.std(read_len_arr).round(2)),
+                               'read_len_min': int(np.min(read_len_arr)),
+                               'read_len_max': int(np.max(read_len_arr)),
+                               'read_len_q25': float(np.quantile(read_len_arr, 0.25).round(2)),
+                               'read_len_q50': float(np.quantile(read_len_arr, 0.50).round(2)),
+                               'read_len_q75': float(np.quantile(read_len_arr, 0.75).round(2)),
+                               'read_len_q100': float(np.quantile(read_len_arr, 1).round(2))
+                               }
+
+        # add this to the overall read dictionary
+        read_info_dict[sample_id][orient] = sample_read_summary
+
+    # dump the contents of both dictionaries to their output files
+    # always write out the sequence length
+    with open(read_info_json, 'w+') as info_out:
+        json.dump(read_info_dict, info_out)
+
+    # check whether there are errors to write out, then write out and print summary
+    if len(p_detect_dict) > 0:
+        perc_samples = (len(err_samples) / (total_samples/2))*100  # divide by 2 to account for R1/R2
+        print(f'WARNING. {primers_detected} reads from {len(err_samples)} samples ({perc_samples:.1}% of all samples) '
+              f'contained a primer sequence after trimming primers with cutadapt. Please consult the '
+              f'details in the summary file {primer_detected_json} for details.\n')
+        with open(primer_detected_json, 'w+') as err_out:
+            json.dump(p_detect_dict, err_out)
+
+    return None
+
+def remove_primers(input_files, file_map, platform, paired_end=True, verbose=False):
+
+    # make the main directory for output from primer removal
     trim_primers_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output']['primers-trimmed'])
 
-    settings = import_config_as_dict(file_path=file_map['config']['main'], file_handle='pipeline-settings')
+    # read in settings from the configuration file
+    settings = get_settings(file_map)
     run_name = settings['run_details']['run_name']
 
+    # access cutadapt settings from the configuration
+    cutadapt_settings = settings['remove_primers']
+    fwd_max_err = cutadapt_settings['max_error_rate']['fwd']
+    rev_max_err = cutadapt_settings['max_error_rate']['rev']
+    if fwd_max_err == rev_max_err:
+        max_err = fwd_max_err
+    max_untrimmed = cutadapt_settings['max_untrimmed']
+
     # get the forward and reverse primers
     primer_dict = identify_primers(platform, config_dict=settings)
     fwd_primer = primer_dict['fwd']
     rev_primer = primer_dict['rev']
+    fwd_revcomp_primer = primer_dict['fwd_rc']
+    rev_revcomp_primer = primer_dict['rev_rc']
 
-    fwd_revcomp_primer = str(Seq(fwd_primer).reverse_complement())
-    rev_revcomp_primer = str(Seq(rev_primer).reverse_complement())
-
+    # create trimmed and untrimmed read directories
     trim_path = mkdir_exist_ok(new_dir=f'./{TRIMMED_PREFIX}_{run_name}', parent_dir=trim_primers_parent)
     notrim_path = mkdir_exist_ok(new_dir=f'./{flip_prefix(TRIMMED_PREFIX)}_{run_name}', parent_dir=trim_primers_parent)
 
-    cutadapt_settings = settings['cutadapt']
-    fwd_max_err = int(cutadapt_settings['max_error_rate']['fwd'])
-    rev_max_err = int(cutadapt_settings['max_error_rate']['rev'])
-    if fwd_max_err == rev_max_err:
-        max_err = fwd_max_err
-    max_untrimmed = int(cutadapt_settings['max_untrimmed'])
+    # if verbose, then print full report
+    if verbose:  # best for troubleshooting
+        report = 'full'
+    else:  # best for large runs
+        report = 'minimal'
 
+    # compose and execute the command line command to run cutadapt for paired-end reads
     if paired_end:
         paired_dict = pair_reads(input_files)
 
         for file in paired_dict.keys():
 
             fwd_read_out = add_prefix(file_path=file, prefix=TRIMMED_PREFIX, dest_dir=trim_path, action=None)
             rev_read_out = add_prefix(file_path=paired_dict[file], prefix=TRIMMED_PREFIX, dest_dir=trim_path, action=None)
 
-            cutadapt_cmd = ['cutadapt', '--report=minimal',
-                            '-a', fwd_primer, '-A', rev_primer,
+            # this will only work on half the reads
+            # cutadapt_cmd = ['cutadapt', f'--report={report}',
+            #                 '-a', fwd_primer, '-A', rev_primer,
+            #                 '-n', '2', '-e', str(max_err),
+            #                 '-o', fwd_read_out, '-p', rev_read_out,
+            #                 file, paired_dict[file]]
+
+            # from the DADA2 cutadapt step; this will only work on half the reads
+            # cutadapt_cmd = ['cutadapt', f'--report={report}',
+            #                 '-g', fwd_primer, '-a', rev_revcomp_primer,
+            #                 '-G', rev_primer, '-A', fwd_revcomp_primer,
+            #                 '-n', '2', '-e', str(max_err),
+            #                 '-o', fwd_read_out, '-p', rev_read_out,
+            #                 file, paired_dict[file]]
+            #
+            # this worked on pacbio, does not work at all on Illumina paired-end
+            # cutadapt_cmd = ['cutadapt', f'--report={report}',
+            #                 '-a', f'^{fwd_primer}...{rev_revcomp_primer}$',
+            #                 '-a', f'^{rev_primer}...{fwd_revcomp_primer}$',
+            #                 '-n', '2', '-e', str(max_err),
+            #                 '-o', fwd_read_out, '-p', rev_read_out,
+            #                 file, paired_dict[file]]
+
+            # some combination of all, where it will search for both combos in both reads?
+            # does not work at all
+            # cutadapt_cmd = ['cutadapt', f'--report={report}',
+            #                 '-g', f'^{fwd_primer}...{rev_revcomp_primer}$',
+            #                 '-a', f'^{rev_primer}...{fwd_revcomp_primer}$',
+            #                 '-G', f'^{fwd_primer}...{rev_revcomp_primer}$',
+            #                 '-A', f'^{rev_primer}...{fwd_revcomp_primer}$',
+            #                 '-n', '2', '-e', str(max_err),
+            #                 '-o', fwd_read_out, '-p', rev_read_out,
+            #                 file, paired_dict[file]]
+
+            # DADA2 cutadapt but with --interleaved to do two passes to account for mixed R1/R2 orientation
+            # doesn't work; also tried again with remove -n 2 from both
+            # cutadapt_cmd = ['cutadapt', f'--report={report}',
+            #                 '-g', fwd_primer, '-a', rev_revcomp_primer,
+            #                 '-G', rev_primer, '-A', fwd_revcomp_primer,
+            #                 '-n', '2', '-e', str(max_err),
+            #                 '--interleaved',
+            #                 file, paired_dict[file],
+            #                 '|',
+            #                 'cutadapt', f'--report={report}',
+            #                 '-g', rev_primer, '-a', fwd_revcomp_primer,
+            #                 '-G', fwd_primer, '-A', rev_revcomp_primer,
+            #                 '-n', '2', '-e', str(max_err),
+            #                 '--interleaved',
+            #                 '-o', fwd_read_out, '-p', rev_read_out,
+            #                 '-']
+
+            # WORKS!
+            cutadapt_cmd = ['cutadapt', f'--report={report}',
+                            '-g', fwd_primer, '-a', rev_revcomp_primer,
+                            '-g', rev_primer, '-a', fwd_revcomp_primer,
+                            '-G', rev_primer, '-A', fwd_revcomp_primer,
+                            '-G', fwd_primer, '-A', rev_revcomp_primer,
                             '-n', '2', '-e', str(max_err),
                             '-o', fwd_read_out, '-p', rev_read_out,
                             file, paired_dict[file]]
 
-            run_subprocess(cutadapt_cmd, dest_dir=trim_primers_parent)
+            run_subprocess(cutadapt_cmd, dest_dir=trim_primers_parent,
+                           auto_respond=settings['automate']['auto_respond'])
 
+    # compose and execute the command line command to run cutadapt for single-end reads
     else:
 
         for file in input_files:
 
             trim_out = add_prefix(file_path=file, prefix=TRIMMED_PREFIX, dest_dir=trim_path, action=None)
 
             if cutadapt_settings['keep_untrimmed']:
                 notrim_out = add_prefix(file_path=file, prefix=flip_prefix(TRIMMED_PREFIX),
                                         dest_dir=notrim_path, action=None)
                 untrim_cmd = f'--untrimmed-output={notrim_out}'
             else:
                 untrim_cmd = ''
 
 
-            cutadapt_cmd = ['cutadapt', '--report=minimal',
+            cutadapt_cmd = ['cutadapt', f'--report={report}',
                             '-a', f'^{fwd_primer}...{rev_revcomp_primer}$',
                             '-a', f'^{rev_primer}...{fwd_revcomp_primer}$',
                             '-n', '2', '-e', str(max_err), untrim_cmd, '-o', trim_out, file]
 
             # create or append to cutadapt stderr/stdout, all output goes to one file (not one per sample)
-            run_subprocess(cutadapt_cmd, dest_dir=trim_primers_parent)
-
-    # quantify proportion untrimmed
-    # with open((trim_primers_parent / 'cutadapt.out'), 'r') as fin:
-    #     cutadapt_df = pd.read_table(fin)
-    #     sum_in = cutadapt_df['in_reads'].sum(0)
-    #     sum_out = cutadapt_df['out_reads'].sum(0)
-    #     percent_lost = ((sum_in - sum_out) / (sum_in)) * 100
-    #     if percent_lost > max_untrimmed:
-    #         msg = f'After primer trimming, {percent_lost:.2f}% of the input reads were lost, which is ' \
-    #               f'above the user-defined maximum threshold of {max_untrimmed}%.\n'
-    #         exit_process(message=msg)
-    #     else:
-    #         print(f'{percent_lost:.2f}% of input reads were lost to primer trimming. This is above the user-provided '
-    #               f'input of {max_untrimmed}%, so proceeding to next step...\n')
-
-    return None
-
-def merge_reads(input_files, file_map):
-    settings = import_config_as_dict(file_path=file_map['config']['main'], file_handle='pipeline-settings')
-    run_name = settings['run_details']['run_name']
-
-    if settings['quality_filtering']['illumina']['merge_reads']:
-
-        qfilt_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output']['quality-filtered'])
-        merge_path = mkdir_exist_ok(new_dir=f'./{MERGED_PREFIX}_{run_name}', parent_dir=qfilt_parent)
-        nomerge_path = mkdir_exist_ok(new_dir=f'./{flip_prefix(MERGED_PREFIX)}_{run_name}', parent_dir=qfilt_parent)
+            run_subprocess(cutadapt_cmd, dest_dir=trim_primers_parent,
+                           auto_respond=settings['automate']['auto_respond'])
 
-        merge_summary = qfilt_parent / 'vsearch_merged.log'
-
-        paired_dict = pair_reads(input_files)
-
-        output_list = []
-        for file in paired_dict.keys():
-
-            nomerge_fwd_out = add_prefix(file_path=file, prefix=MERGED_PREFIX,
-                                         dest_dir=nomerge_path, action=None)
-            nomerge_rev_out = add_prefix(file_path=paired_dict[file], prefix=flip_prefix(MERGED_PREFIX),
-                                         dest_dir=nomerge_path, action=None)
-
-            merge_out_base = add_prefix(file_path=file, prefix=MERGED_PREFIX, dest_dir=merge_path, action=None)
-            sample_id = re.search('.+?(?=_R1)', merge_out_base.stem).group(0)
-            merge_output = (merge_out_base.parent / sample_id).with_suffix('.fastq')
-            output_list.append(merge_output)
-
-            vsearch_merge_cmd = ['vsearch', '--fastq_mergepairs', file, '--reverse', paired_dict[file],
-                                 '--fastqout', merge_output,
-                                 '--fastqout_notmerged_fwd', nomerge_fwd_out,
-                                 '--fastqout_notmerged_rev', nomerge_rev_out,
-                                 '--eetabbedout', merge_summary]
-
-            run_subprocess(vsearch_merge_cmd, dest_dir=qfilt_parent)
-
-        return output_list
+    # also helpful to see the command that is run during troubleshooting
+    if verbose:
+        print(f'cutadapt command: {cutadapt_cmd}\n')
+        print(f'WARNING. Currently, the max proportion of untrimmed reads cannot be analyzed '
+              f'with verbose set to True. To have the max proportion check, turn verbose to False.\n')
     else:
-        return input_files
+        # quantify proportion untrimmed; only works if not verbose
+        with open((trim_primers_parent / 'cutadapt.out'), 'r') as fin:
+            cutadapt_df = pd.read_table(fin)
+            sum_in = cutadapt_df['in_reads'].sum(0)
+            sum_out = cutadapt_df['out_reads'].sum(0)
+            percent_lost = ((sum_in - sum_out) / (sum_in)) * 100
+            if percent_lost > max_untrimmed:
+                msg = f'After primer trimming, {percent_lost:.2f}% of the input reads were lost, which is ' \
+                      f'above the user-defined maximum threshold of {max_untrimmed}%.\n'
+                exit_process(message=msg)
+            else:
+                print(f'{percent_lost:.2f}% of input reads were lost to primer trimming. This is below the user-provided '
+                      f'input of {max_untrimmed}%, so proceeding to next step...\n')
+
+    return trim_path
 
 def quality_filter(input_files, platform, file_map):
 
-    settings = import_config_as_dict(file_path=file_map['config']['main'], file_handle='pipeline-settings')
+    # get filtering settings from the configuration file
+    settings = get_settings(file_map)
     run_name = settings['run_details']['run_name']
     qfilt_dict = settings['quality_filtering'][platform]
     min_len = qfilt_dict['min_len']
     max_len = qfilt_dict['max_len']
-    premerged = settings['quality_filtering']['illumina']['merge_reads']
 
+    # if these are Illumina reads, get the max expected error to use
     if platform == 'illumina':
         max_error = qfilt_dict['max_error']
     else:
         max_error = ''
 
+    # create a path to the parent directory for quality filtered output
     qfilt_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output']['quality-filtered'])
 
+    # make sudirectories for the results of quality filtering
     qfilt_path = mkdir_exist_ok(new_dir=f'./{QUALFILT_PREFIX}_{run_name}', parent_dir=qfilt_parent)
     nofilt_path = mkdir_exist_ok(new_dir=f'./{flip_prefix(QUALFILT_PREFIX)}_{run_name}', parent_dir=qfilt_parent)
 
-    if premerged:
-        for file in input_files:
+    # attempt to pair together R1/R2 reads from the input files
+    paired_dict = pair_reads(input_files)
+
+    # go through each R1 read...
+    for file in paired_dict.keys():
+        # if this R1 read does not have an associated R2 read...
+        if paired_dict[file] == '':
+
+            # then process these sequence files as individuals
             qfilt_out = add_prefix(file_path=file, prefix=QUALFILT_PREFIX,
                                            dest_dir=qfilt_path, action=None)
             nofilt_out = add_prefix(file_path=file, prefix=flip_prefix(QUALFILT_PREFIX),
                                         dest_dir=nofilt_path, action=None)
 
             vsearch_filt_cmd = ['vsearch', '--fastq_filter', file,
                                 '--fastqout', qfilt_out,
                                 '--fastqout_discarded', nofilt_out,
                                 '-fastq_maxee', str(max_error), '--fastq_maxlen', str(max_len),
                                 '--fastq_minlen', str(min_len), '--sizeout']
 
-            run_subprocess(vsearch_filt_cmd, dest_dir=qfilt_parent)
-    else:
+            run_subprocess(vsearch_filt_cmd, dest_dir=qfilt_parent,
+                           auto_respond=settings['automate']['auto_respond'])
+
+        # if the paired reads dict does have values (i.e., there are R2 files associated with the R1 files)
+        else:
+            # then process reads as R1/R2 pairs
+            for file in paired_dict.keys():
+
+                qfilt_fwd_out = add_prefix(file_path=file, prefix=QUALFILT_PREFIX,
+                                           dest_dir=qfilt_path, action=None)
+                nofilt_fwd_out = add_prefix(file_path=file, prefix=flip_prefix(QUALFILT_PREFIX),
+                                            dest_dir=nofilt_path, action=None)
+
+                qfilt_rev_out = add_prefix(file_path=paired_dict[file], prefix=QUALFILT_PREFIX,
+                                           dest_dir=qfilt_path, action=None)
+                nofilt_rev_out = add_prefix(file_path=paired_dict[file], prefix=flip_prefix(QUALFILT_PREFIX),
+                                            dest_dir=nofilt_path, action=None)
+
+                vsearch_filt_cmd = ['vsearch', '--fastq_filter', file, '--reverse', paired_dict[file],
+                                    '--fastqout', qfilt_fwd_out, '--fastqout_rev', qfilt_rev_out,
+                                    '--fastqout_discarded', nofilt_fwd_out, '--fastqout_discarded_rev', nofilt_rev_out,
+                                    '-fastq_maxee', str(max_error), '--fastq_maxlen', str(max_len),
+                                    '--fastq_minlen', str(min_len), '--sizeout']
+
+                run_subprocess(vsearch_filt_cmd, dest_dir=qfilt_parent,
+                               auto_respond=settings['automate']['auto_respond'])
+
+    return qfilt_path
+
+def merge_reads(input_files, file_map):
+    settings = get_settings(file_map)
+    run_name = settings['run_details']['run_name']
+
+    if settings['quality_filtering']['illumina']['merge_reads']:
+
+        qfilt_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output']['quality-filtered'])
+        merge_path = mkdir_exist_ok(new_dir=f'./{MERGED_PREFIX}_{run_name}', parent_dir=qfilt_parent)
+        nomerge_path = mkdir_exist_ok(new_dir=f'./{flip_prefix(MERGED_PREFIX)}_{run_name}', parent_dir=qfilt_parent)
+
+        merge_summary = qfilt_parent / 'vsearch_merged.log'
+
         paired_dict = pair_reads(input_files)
+
+        output_list = []
         for file in paired_dict.keys():
 
-            qfilt_fwd_out = add_prefix(file_path=file, prefix=QUALFILT_PREFIX,
-                                       dest_dir=qfilt_path, action=None)
-            nofilt_fwd_out = add_prefix(file_path=file, prefix=flip_prefix(QUALFILT_PREFIX),
-                                        dest_dir=nofilt_path, action=None)
+            nomerge_fwd_out = add_prefix(file_path=file, prefix=MERGED_PREFIX,
+                                         dest_dir=nomerge_path, action=None)
+            nomerge_rev_out = add_prefix(file_path=paired_dict[file], prefix=flip_prefix(MERGED_PREFIX),
+                                         dest_dir=nomerge_path, action=None)
 
-            qfilt_rev_out = add_prefix(file_path=paired_dict[file], prefix=QUALFILT_PREFIX,
-                                       dest_dir=qfilt_path, action=None)
-            nofilt_rev_out = add_prefix(file_path=paired_dict[file], prefix=flip_prefix(QUALFILT_PREFIX),
-                                        dest_dir=nofilt_path, action=None)
+            merge_out_base = add_prefix(file_path=file, prefix=MERGED_PREFIX, dest_dir=merge_path, action=None)
+            sample_id = re.search(r'.+?(?=_R1)', merge_out_base.stem).group(0)
+            merge_output = (merge_out_base.parent / sample_id).with_suffix('.fastq')
+            output_list.append(merge_output)
 
-            vsearch_filt_cmd = ['vsearch', '--fastq_filter', file, '--reverse', paired_dict[file],
-                                '--fastqout', qfilt_fwd_out, '--fastqout_rev', qfilt_rev_out,
-                                '--fastqout_discarded', nofilt_fwd_out, '--fastqout_discarded_rev', nofilt_rev_out,
-                                '-fastq_maxee', str(max_error), '--fastq_maxlen', str(max_len),
-                                '--fastq_minlen', str(min_len), '--sizeout']
+            vsearch_merge_cmd = ['vsearch', '--fastq_mergepairs', file, '--reverse', paired_dict[file],
+                                 '--fastqout', merge_output,
+                                 '--fastqout_notmerged_fwd', nomerge_fwd_out,
+                                 '--fastqout_notmerged_rev', nomerge_rev_out,
+                                 '--eetabbedout', merge_summary]
 
-            run_subprocess(vsearch_filt_cmd, dest_dir=qfilt_parent)
+            run_subprocess(vsearch_merge_cmd, dest_dir=qfilt_parent,
+                           auto_respond=settings['automate']['auto_respond'])
 
-    return None
+        # add descriptive header to the merge log file
+        # with open(merge_summary, 'w') as fout:
+        #     merge_header = '#fwd_ee_exp\trev_ee_exp\tfwd_ee_obs\trev_ee_obs\n'
+        #     with_header = merge_output.insert(0, merge_header)
+        #     fout.write(with_header)
+
+        return output_list
+    else:
+        return input_files
 
 def dereplicate(input_files, derep_step, platform, file_map):
 
     derep_prefix = DEREP_PREFIX + '0' + str(derep_step)
 
     if derep_step == 1:
         out_tag = 'derep-full-length'
     else:
         out_tag = 'derep-subregions'
 
-    settings = import_config_as_dict(file_path=file_map['config']['main'], file_handle='pipeline-settings')
+    settings = get_settings(file_map)
     run_name = settings['run_details']['run_name']
-    min_unique = settings['quality_filtering'][platform]['min_count'][f'derep0{derep_step}']
+    min_unique = settings['dereplicate'][platform]['min_count'][f'derep0{derep_step}']
     premerged = settings['quality_filtering']['illumina']['merge_reads']
 
     derep_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output'][out_tag])
 
     derep_path = mkdir_exist_ok(new_dir=f'./{derep_prefix}_{run_name}', parent_dir=derep_parent)
 
     # derep_summary = mkdir_exist_ok(new_dir=f'./{derep_prefix}_{run_name}_summaries', parent_dir=derep_parent)
     if premerged:
         pass
     else:
-        input_files = [f for f in input_files if re.search('R1', f, re.I)]  # only take fwd if not merged
+        input_files = [f for f in input_files if re.search(r'R1', f, re.I)]  # only take fwd if not merged
         # rename files to be just sample ID or keep R1 to be clear they're forward reads only?
 
     for file in input_files:
 
         # derep always outputs a fasta format, but need to provide file name as fasta format or will appear as fastq
         # even though it isn't really fastq when you open it up
         derep_output = add_prefix(file_path=file, prefix=derep_prefix, dest_dir=derep_path, action=None).with_suffix('.fasta')
 
         vsearch_derep_cmd = ['vsearch', '--derep_fulllength', file,
                              '--output', derep_output,'--minuniquesize', str(min_unique),
                              '--sizeout']
 
-        run_subprocess(vsearch_derep_cmd, dest_dir=derep_parent)
+        run_subprocess(vsearch_derep_cmd, dest_dir=derep_parent,
+                       auto_respond=settings['automate']['auto_respond'])
 
     return None
 
 def separate_subregions(input_files, file_map):
 
-    settings = import_config_as_dict(file_path=file_map['config']['main'], file_handle='pipeline-settings')
+    settings = get_settings(file_map)
     run_name = settings['run_details']['run_name']
 
-    itsx_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output']['separate-subregions'])
+    itsx_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output']['separated-subregions'])
 
     itsx_path = mkdir_exist_ok(new_dir=f'./{ITSX_PREFIX}_{run_name}',  parent_dir=itsx_parent)
 
     for file in input_files:
 
         itsx_output_basename = add_prefix(file_path=file, prefix=ITSX_PREFIX, dest_dir=itsx_path, action=None).with_suffix('')
 
         itsx_command = ['ITSx', '-i', file, '-o', itsx_output_basename, '-t', 'F', '--multi_thread', 'T',
                         '--save_regions', 'all']
 
-        run_subprocess(itsx_command, dest_dir=itsx_parent)
+        run_subprocess(itsx_command, dest_dir=itsx_parent,
+                       auto_respond=settings['automate']['auto_respond'])
 
-    return None
+    return itsx_path
 
 def concat_regions(dir_path, regions_to_concat=['ITS1', '5_8S', 'ITS2'], header_delim=';', **kwargs):
     '''
     Concatenates provided regions for each read.
 
     Looks in the provided directory for files containing the substring of the
     regions provided in the regions_to_concat list. For each region in the list,
@@ -801,26 +1052,26 @@
 
     # REMOVE AFTER TESTING
     # dir_path = Path('./04_separated-subregions/itsx_pacbio_sporocarp-f_2023-12_Q40')
     # regions_to_concat = ['ITS1', '5_8S', 'ITS2']
     # header_delim = ';'
     ######################
     for kw in kwargs.keys():
-        if re.search('suffix', kw, re.I):
+        if re.search(r'suffix', kw, re.I):
             file_suffix = f'_{kwargs[kw]}'
         else:
             file_suffix = ''
 
     # create dictionary for acceptable input
-    accepted_regions = {'(^S.+?(?=\bs)|SSU)': 'SSU',  # could be better but not going to obsess
-                        'ITS.?1': 'ITS1',  # checks for possible punctuation within
-                        '5.?8S': '5.8S',  # checks for possible punctuation within
-                        'ITS.?2': 'ITS2',  # checks for possible punctuation within
-                        '(^L.+?(?=\bs)|LSU)': 'LSU',  # similar to SSU
-                        '(full)?.?ITS(?!.?\d)': 'ITS'}  # may include full, but can't have number after (w or w/o punct)
+    accepted_regions = {r'(^S.+?(?=\bs)|SSU)': 'SSU',  # could be better but not going to obsess
+                        r'ITS.?1': 'ITS1',  # checks for possible punctuation within
+                        r'5.?8S': '5.8S',  # checks for possible punctuation within
+                        r'ITS.?2': 'ITS2',  # checks for possible punctuation within
+                        r'(^L.+?(?=\bs)|LSU)': 'LSU',  # similar to SSU
+                        r'(full)?.?ITS(?!.?\d)': 'ITS'}  # may include full, but can't have number after (w or w/o punct)
 
     # check input list for valid entries, and then format string to consistent format
     # returns dict now with formatted string as key, regex as value
     def create_region_dict(region_list):
         output_dict = {}
         for region_str in region_list:
             for r in accepted_regions.keys():  # compare input region to each regex in dict
@@ -857,45 +1108,35 @@
             return print(f'FAILURE. No files matching the provided regex {regex} were located in '
                          f'{dir_path.name}. Exiting...\n')
         else:
             return found_file_paths[0]
 
     fastas_to_concat = [search_path_with_regex(dir_path, regex=r) for r in region_search_dict.values()]
 
-    SAMPLE_ID_RE = '(?<=\w_)(pacbio|sanger|illumina).+?(?=\.)'
-    PREFIX_RE = '^\w.+?(?=_pacbio|_sanger|_illumina)'
-
-    sample_name = re.search(SAMPLE_ID_RE, fastas_to_concat[0].name, re.I).group(0)
+    sample_name = get_sample_id(file_path = fastas_to_concat[0].name)
     file_prefix = re.search(PREFIX_RE, fastas_to_concat[0].name, re.I).group(0)
 
     if list(region_search_dict.keys()) == ['ITS1', '5.8S', 'ITS2']:
         concat_name = 'full_ITS'
     else:
         concat_name = input(f'Please provide a name to assign to this combination of subregions (use '
                             f'underscores instead of spaces):\n')
 
-    # renamed header search regex
-    # WAY TO UPDATE REGEX GLOBALLY WHEN A RENAMING OCCURS?
-    READ_ID_RE = '^.+?(?=;)'
-    READ_REGION_RE = '(?<=\d;)\w.+?(?=;)'
-    READ_LEN_RE = '(?<=len=)[0-9]{1,}(?=bp)'
-    READ_COUNT_RE = '(?<=full\-len_copies=)[0-9]{1,}'
-
     # ADD THESE OPTIONS IN THE CONFIG FILE?
     details_to_include = ['sequence', 'region_len', 'full-len_copies']
 
     concat_dict = {}
     for fasta in fastas_to_concat:
         for record in SeqIO.parse(fasta, 'fasta'):
             try:
-                read_id = re.search(READ_ID_RE, record.id).group(0)
-                region = re.search(READ_REGION_RE, record.id, re.I).group(0)
+                read_id = re.search(READ_ID_RENAMED_RE, record.id).group(0)
+                region = re.search(READ_REGION_RENAMED_RE, record.id, re.I).group(0)
 
-                length = re.search(READ_LEN_RE, record.id, re.I).group(0)
-                derep01_reads = re.search(READ_COUNT_RE, record.id, re.I).group(0)
+                length = re.search(READ_LEN_RENAMED_RE, record.id, re.I).group(0)
+                derep01_reads = re.search(READ_COUNT_RENAMED_RE, record.id, re.I).group(0)
                 details = {k:v for k,v in zip(details_to_include, [record.seq, length, derep01_reads])}
 
                 if read_id in concat_dict:  # if this sample is already in the dictionary...
                     concat_dict[read_id].update({region: details})  # append the new region info to it
                 else:  # if it isn't yet in the dictionary...
                     concat_dict[read_id] = {region: details}  # add a key value pair for this sample
             except:
@@ -926,18 +1167,18 @@
                            'id':[read, concat_name]}
 
             for k in pulled_data_dict.keys():
                 if len(pulled_data_dict[k]) == len(regions_to_concat):
                     if any(isinstance(i, Seq) for i in pulled_data_dict[k]):
                         joined_data['seq'] = Seq('').join(pulled_data_dict[k])  # must join with empty seq
                     else:
-                        if re.search('len$', k, re.I):
+                        if re.search(r'len$', k, re.I):
                             val = sum([int(x) for x in pulled_data_dict[k]])
                             joined_data['id'].append(f'{k}={val}bp')
-                        elif re.search('^full\-len|count', k, re.I):
+                        elif re.search(r'^full\-len|count', k, re.I):
                             if len(set(pulled_data_dict[k])) == 1:
                                 derep = int(pulled_data_dict[k][0])  # if all same, doesn't matter which you chose
                                 joined_data['id'].append(f'{k}={derep}')  # make int so no '' surrounding num in header
                         else:
                             print(f'Could not recognized the input data type, {k}:\n'
                                   f'\t{pulled_data_dict[k]}\n')
                             return None
@@ -958,17 +1199,15 @@
         concatenated_records.append(concat_record)
 
     fasta_out = dir_path / f'{file_prefix}_{sample_name}.{concat_name}{file_suffix}.fasta'
     SeqIO.write(concatenated_records, fasta_out, 'fasta')
 
     return None
 
-def check_itsx_output(itsx_dir, full_len_dir, num_bp_compare, write_to_log=True, same_threshold=99):
-    SAMPLE_ID_RE = '(?<=\w_)(pacbio|sanger|illumina).+?(?=\.)'
-    READ_ID_RE = '[0-9]{1,}(?=\/ccs)'
+def check_concat_output(itsx_dir, full_len_dir, num_bp_compare, write_to_log=True, same_threshold=99):
 
     bp = int(num_bp_compare)
 
     # import records as dictionary, where the read ID is the key
     def name_as_key(record):
         header = record.id
         sample_read_id = header.split(';')[0]
@@ -981,16 +1220,16 @@
     # collect the full length _ bp sequences at start, full ITS _ bp sequences at start, and LSU _ bp seqs at end
     post_itsx_diffs = {'read_id':[],
                        'full_start':[],
                        'its_start':[],
                        'lsu_end':[]}
     for record in SeqIO.parse(full_len_dir, 'fasta'):
 
-        sample_id = re.search(SAMPLE_ID_RE, full_len_dir.name).group(0)
-        read_num = re.search(READ_ID_RE, record.id).group(0)
+        sample_id = get_sample_id(file_path = full_len_dir.name)
+        read_num = re.search(READ_ID_OG_RE, record.id).group(0)
         read_id = '_'.join([sample_id, read_num])
 
         renamed_record = SeqRecord(record.seq, id=read_id, description='')
 
         full_len_seq = renamed_record.seq
         full_its_seq = full_its_records[renamed_record.id].seq
         try:
@@ -1041,15 +1280,15 @@
     missing_lsu = ((diff_df[diff_df['equal_as'] == 'no_lsu'].shape[0]) /sum(diff_df['comparison']))*100
 
     if write_to_log:
         log_dir = itsx_dir / 'itsx_inspection_logs'
         log_dir.mkdir(exist_ok=True)
         diff_df.to_csv(log_dir / f'itsx_inspection_comparison.csv', index=False)
         with open((log_dir / 'itsx_inspection_summary.log'), 'wt') as fout:
-            fout.write(f'sample: {re.search(SAMPLE_ID_RE, full_len_dir.name).group(0)}\n')
+            fout.write(f'sample: {get_sample_id(file_path = full_len_dir.name)}\n')
             fout.write(f'date: {datetime.today().strftime("%Y-%M-%d")}\n\n')
             fout.write(f'All full-length reads were compared to their ITS region after running ITSx. The first'
                        f' {bp} bp of the full-length reads were aligned to the first {bp} bp of their corresponding '
                        f'full ITS read that was concatenated after running ITSx. If the first {bp} bp did not '
                        f'match, then the reverse complement of the last {bp} bp of their LSU region was compared '
                        f'to the first {bp} bp of the full-length read. This is because reads are not reoriented '
                        f'until done so by ITSx. \n\n')
@@ -1069,15 +1308,15 @@
                   f'{same_threshold}%, at {percent_same}.\n')
 
     return None
 
 def check_chimeras(input_files, file_map, ref=None):
     chim_ref_files = file_map['config']['reference-db']['chimera'].glob(SEQ_FILE_GLOB)
 
-    settings = import_config_as_dict(file_path=file_map['config']['main'], file_handle='pipeline-settings')
+    settings = get_settings(file_map)
     run_name = settings['run_details']['run_name']
 
     chim_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output']['chimera-checked'])
 
     nochim_path = mkdir_exist_ok(new_dir=f'./{NOCHIM_PREFIX}_{run_name}', parent_dir=chim_parent)
     chim_path = mkdir_exist_ok(new_dir=f'./{flip_prefix(NOCHIM_PREFIX)}_{run_name}', parent_dir=chim_parent)
 
@@ -1091,15 +1330,16 @@
                                   dest_dir=chim_path, action=None)
 
             vsearch_denovo_cmd = ['vsearch', '--uchime3_denovo', file,
                                   '--chimeras', chim_out,
                                   '--nonchimeras', nochim_out,
                                   '--uchimeout', uchime_log]
 
-            run_subprocess(vsearch_denovo_cmd, dest_dir=chim_parent)
+            run_subprocess(vsearch_denovo_cmd, dest_dir=chim_parent,
+                           auto_respond=settings['automate']['auto_respond'])
     else:
         refs_to_use = []
         for r in chim_ref_files:
             result = re.search(ref, r, re.I)
             if result:
                 refs_to_use.append(result.group(0))
             else:
@@ -1114,39 +1354,41 @@
 
                 vsearch_ref_cmd = ['vsearch', '--uchime_ref', file,
                                    '--chimeras', chim_out,
                                    '--nonchimeras', nochim_out,
                                    '--uchimeout', uchime_log,
                                    '--db', chim_ref]
 
-                run_subprocess(vsearch_ref_cmd, dest_dir=chim_parent)
+                run_subprocess(vsearch_ref_cmd, dest_dir=chim_parent,
+                               auto_respond=settings['automate']['auto_respond'])
 
     return None
 
 def combine_all_reads(input_files, file_map):
 
-    settings = import_config_as_dict(file_path=file_map['config']['main'], file_handle='pipeline-settings')
+    settings = get_settings(file_map)
     run_name = settings['run_details']['run_name']
 
     total_record_list = []
     for file in input_files:
         rename_read_header(file, header_delim=';')
         for record in SeqIO.parse(file, 'fasta'):
             total_record_list.append(record)
 
     combined_out = file_map['pipeline-output']['otus-clustered'] / f'combined_otus_{run_name}.fasta'
     SeqIO.write(total_record_list, combined_out, 'fasta')
 
     return combined_out
 
 def cluster_reads(input_files, file_map):
-    settings = import_config_as_dict(file_path=file_map['config']['main'], file_handle='pipeline-settings')
+
+    settings = get_settings(file_map)
     run_name = settings['run_details']['run_name']
 
-    min_threshold = settings['clustering']['min_threshold']
+    min_threshold = settings['otu_clustering']['min_threshold']
 
     clust_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output']['otus-clustered'])
 
     # rename headers for each file to retain source of sample
     # rename_read_headers()
 
     # combine all reads into one fasta file
@@ -1154,108 +1396,109 @@
 
     clust_out = add_prefix(file_path=combined_reads, prefix=CLUSTER_PREFIX,
                            dest_dir=clust_parent, action=None)
     # cluster
     vsearch_clust_cmd = ['vsearch', '--cluster_fast', combined_reads, '--clusters',
                          clust_out, '--id', str(min_threshold)]
 
-    run_subprocess(vsearch_clust_cmd, dest_dir=clust_parent)
+    run_subprocess(vsearch_clust_cmd, dest_dir=clust_paren,
+                   auto_respond=settings['automate']['auto_respond'])
 
     return None
 
 
-def create_blast_db(config_dict, file_map, taxa_list=None):
-    '''
-    Create a reference dataset for BLAST+ search.
-
-    :param config_dict: configuration file dictionary; required to get the list
-    of reference databases to use, as defined by user in the configuration file.
-    :param file_map: file mapping, from mapping.py
-    :param taxa_list: option; list of taxa to include if wanting to limit search
-    to a specific taxonomic group
-    :return: returns path to the newly created db for blastn search; creates a custom
-    database using BLAST+ makeblastdb from the command line
-    '''
-    tax_settings = config_dict['taxonomy']
-    db_dir = file_map['config']['reference-db']
-
-    include_genbank = tax_settings['refdb']['genbank']['include']
-    include_unite = tax_settings['refdb']['unite']['include']
-    include_custom = tax_settings['refdb']['custom']['include']
-    include_maarjam = tax_settings['refdb']['maarjam']['include']
-
-    included_tag = ''
-    db_include_list = []
-    if include_genbank:
-        genbank_fasta = db_dir.glob('*genbank*')
-        db_include_list.append(genbank_fasta)
-        included_tag += 'G'
-
-    if include_unite:
-        unite_fasta = db_dir.glob('*unite*')
-        db_include_list.append(unite_fasta)
-        included_tag += 'U'
-
-    if include_custom:
-        custom_fasta = db_dir.glob('*custom*')
-        db_include_list.append(custom_fasta)
-        included_tag += 'C'
-
-    if include_maarjam:
-        maarjam_fasta = db_dir.glob('*maarjam*')
-        db_include_list.append(maarjam_fasta)
-        included_tag += 'M'
-
-    custom_search_records = []
-    for db in db_include_list:
-        for record in SeqIO.parse(db, 'fasta'):
-            if taxa_list is None:
-                custom_search_records.append(record)
-            else:
-                pass  # NEED TO SEE HOW TO GET ONLY SPECIFIC TAXONOMY, NOT SURE HOW FORMATTED
-
-    tax_out_dir = file_map['pipeline-output']['taxonomy']
-
-    search_date = datetime.today.strftime('%Y-%M-%d')
-    output_basename = f'custom-ref-{included_tag}_{search_date}'
-    output_path = (tax_out_dir / output_basename).with_suffix('.fasta')
-
-    SeqIO.write(custom_search_records, output_path, 'fasta')
-
-    output_db = tax_out_dir / f'{output_basename}_blast'
-    blast_cmd = ['makeblastdb', '-in', output_path, '-title', output_db, '-dbtype', 'nucl',
-                 output_db]
-
-    run_subprocess(blast_cmd, dest_dir = output_db)
-
-    return output_db
-
-def assign_taxonomy(config_dict, file_map, taxa_list=None):
-    '''
-    Assign taxonomy to sequences.
-
-    :param config_dict:
-    :param file_map:
-    :return:
-    '''
-    tax_output = file_map['pipeline-output']['taxonomy']
-
-    run_name = config_dict['run_details']['run_name']
-
-    if config_dict['taxonomy']['algorithm'] == 'blastn':
-        ref_db = create_blast_db(config_dict, file_map, taxa_list=None)
-
-        blast_out = (tax_output / f'{run_name}').with_suffix('.txt')
-        blast_cmd = ['blastn', '-query', ref_db, '-out', blast_out]
-
-        run_subprocess(blast_cmd, dest_dir = tax_output)
-
-    elif config_dict['taxonomy']['algorithm'] == 'rdp':
-        print(f'Not sure how to set up RDP yet...')
-        rdp_cmd = []
-
-        run_subprocess(rbp_cmd, dest_dir = tax_output)
-
-    else:
-        print(f'I don\'t yet have an option for that algorithm.')
-
-    return None
+# def create_blast_db(config_dict, file_map, taxa_list=None):
+#     '''
+#     Create a reference dataset for BLAST+ search.
+#
+#     :param config_dict: configuration file dictionary; required to get the list
+#     of reference databases to use, as defined by user in the configuration file.
+#     :param file_map: file mapping, from mapping.py
+#     :param taxa_list: option; list of taxa to include if wanting to limit search
+#     to a specific taxonomic group
+#     :return: returns path to the newly created db for blastn search; creates a custom
+#     database using BLAST+ makeblastdb from the command line
+#     '''
+#     tax_settings = config_dict['taxonomy']
+#     db_dir = file_map['config']['reference-db']
+#
+#     include_genbank = tax_settings['refdb']['genbank']['include']
+#     include_unite = tax_settings['refdb']['unite']['include']
+#     include_custom = tax_settings['refdb']['custom']['include']
+#     include_maarjam = tax_settings['refdb']['maarjam']['include']
+#
+#     included_tag = ''
+#     db_include_list = []
+#     if include_genbank:
+#         genbank_fasta = db_dir.glob('*genbank*')
+#         db_include_list.append(genbank_fasta)
+#         included_tag += 'G'
+#
+#     if include_unite:
+#         unite_fasta = db_dir.glob('*unite*')
+#         db_include_list.append(unite_fasta)
+#         included_tag += 'U'
+#
+#     if include_custom:
+#         custom_fasta = db_dir.glob('*custom*')
+#         db_include_list.append(custom_fasta)
+#         included_tag += 'C'
+#
+#     if include_maarjam:
+#         maarjam_fasta = db_dir.glob('*maarjam*')
+#         db_include_list.append(maarjam_fasta)
+#         included_tag += 'M'
+#
+#     custom_search_records = []
+#     for db in db_include_list:
+#         for record in SeqIO.parse(db, 'fasta'):
+#             if taxa_list is None:
+#                 custom_search_records.append(record)
+#             else:
+#                 pass  # NEED TO SEE HOW TO GET ONLY SPECIFIC TAXONOMY, NOT SURE HOW FORMATTED
+#
+#     tax_out_dir = file_map['pipeline-output']['taxonomy']
+#
+#     search_date = datetime.today.strftime('%Y-%M-%d')
+#     output_basename = f'custom-ref-{included_tag}_{search_date}'
+#     output_path = (tax_out_dir / output_basename).with_suffix('.fasta')
+#
+#     SeqIO.write(custom_search_records, output_path, 'fasta')
+#
+#     output_db = tax_out_dir / f'{output_basename}_blast'
+#     blast_cmd = ['makeblastdb', '-in', output_path, '-title', output_db, '-dbtype', 'nucl',
+#                  output_db]
+#
+#     run_subprocess(blast_cmd, dest_dir = output_db)
+#
+#     return output_db
+#
+# def assign_taxonomy(config_dict, file_map, taxa_list=None):
+#     '''
+#     Assign taxonomy to sequences.
+#
+#     :param config_dict:
+#     :param file_map:
+#     :return:
+#     '''
+#     tax_output = file_map['pipeline-output']['taxonomy']
+#
+#     run_name = config_dict['run_details']['run_name']
+#
+#     if config_dict['taxonomy']['algorithm'] == 'blastn':
+#         ref_db = create_blast_db(config_dict, file_map, taxa_list=None)
+#
+#         blast_out = (tax_output / f'{run_name}').with_suffix('.txt')
+#         blast_cmd = ['blastn', '-query', ref_db, '-out', blast_out]
+#
+#         run_subprocess(blast_cmd, dest_dir = tax_output)
+#
+#     elif config_dict['taxonomy']['algorithm'] == 'rdp':
+#         print(f'Not sure how to set up RDP yet...')
+#         rdp_cmd = []
+#
+#         run_subprocess(rbp_cmd, dest_dir = tax_output)
+#
+#     else:
+#         print(f'I don\'t yet have an option for that algorithm.')
+#
+#     return None
```

### Comparing `climush-0.0.7/climush/utilities.py` & `climush-0.0.8/climush/utilities.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess, re, sys, pathlib, shutil, json, tomlkit
+import subprocess, re, sys, pathlib, shutil, json, tomlkit, gzip
 from pathlib import Path
 from datetime import datetime
 from functools import wraps
 import pandas as pd
 from climush.constants import *
 
 # tried to order by category but some required specific order due to dependencies on other functions
@@ -21,130 +21,121 @@
     file path is found to not be a valid Path object; defaults
     to true, as it tends to mess up downstream processes.
     :return: True/error message
     '''
     if isinstance(file_path, pathlib.PurePath):
         return True
     else:
-        msg = f'The provided path, {file_path}, is not a valid Path object.\n'
-        print(msg)
         if exit_if_false:
+            msg = f'The provided path, {file_path}, is not a valid Path object.\n'
             return exit_process(message=msg)
         else:
             return False
 
 # alert if multiple files matching the search pattern in the file path are returned
 # prompt for user input if multiple or no files matching the pattern are returned
 # moved here because used in continue_to_next()
-def flag_multiple_files(file_path, search_for):
+def flag_multiple_files(file_path, search_for, auto_respond=False):
     assert is_pathclass(file_path, exit_if_false=False)
 
     result = list(file_path.glob(search_for))
 
     if len(result) == 1:
         return result[0]
     elif len(result) == 0:
         all_files = file_path.glob('*')
         print(f'No files matching the pattern \'{search_for}\' were detected in the file path: {file_path}. Do '
               f'you mean any of these files in this directory?')
-        which_file = prompt_print_options([all_files, 'none of these (exit)'])
+        which_file = prompt_print_options([all_files, 'none of these (exit)'], auto_respond=auto_respond)
         if which_file in all_files:
             return which_file
         else:
             return exit_process(message=f'The response \'none of these\' was chosen when searching for the correct'
                                         f'file matching the pattern: {search_for}')
     else:
         print(f'{len(result)} files matching the pattern \'{search_for}\' were detected in the file path: '
               f'{file_path}. Please type the number corresponding to the correct file to use:')
-        which_file = prompt_print_options([result, 'none of these (exit)'])
+        which_file = prompt_print_options([result, 'none of these (exit)'], auto_respond=auto_respond)
         if which_file == 'none of these (exit)':
             return exit_process(message=f'The response \'none of these\' was chosen when searching for the correct'
                                         f'file matching the pattern: {search_for}.')
         else:
             return which_file
 
-# activate next script in python
-def continue_to_next(this_script, config_dict):
+def check_dir_exists(dir_path, auto_respond = False):
     '''
-    Continue to the next step of the pipeline.
+    Creates a Path object and checks if the directory exists.
 
-    Will activate the script from the CLI with default
-    parameters. If you do not want to use the default
-    parameters, opt out of automated continuation by
-    responding to the CLI prompt that precedes the use
-    of this function.
-    :param this_script: use __file__ always
-    :return: None, assembles and runs a shell command.
+    Takes the input path and checks whether the path is a Path object. If it is not,
+    it converts it to a Path object. Then checks whether the input path is an existing
+    directory. If it is not, it will prompt the user for a different file path. This
+    function is recursive, in that it will rerun the function if a new file path is
+    provided via the command line prompt.
+    :param dir_path: path to the directory to check; can be a Path object or a string
+    :param auto_respond: if set to True, and the provided path does not exist, then the
+    function will cause the script it is used within to exit if the dir_path is not an
+    existing file path
+    :return: a Path object of an existing file path
     '''
-    automate_dict = config_dict['automate']
-    auto = automate_dict['run_all']
-    to_run = automate_dict['run_some']
-    to_exclude = automate_dict['exclude']
 
-    current_script = Path(this_script).stem
-    current_num = int(current_script.split('_')[0])
-
-    def format_num_for_search(current_script_number):
-        if current_script_number > 9:
-            next_num_search = str(current_script_number + 1)
+    # create a path object from the input, if not already a Path object
+    if isinstance(dir_path, pathlib.PurePath):
+        if dir_path.is_absolute():  # check if absolute; needs to be to get full name of parent, etc.
+            pass
         else:
-            next_num_search = '0' + str(current_script_number + 1)
-        return next_num_search
+            dir_path = dir_path.resolve()
+    else:
+        dir_path = Path(dir_path).resolve()  # also check if absolute here
 
-    next_num_search = format_num_for_search(current_num)
-    next_script = flag_multiple_files(file_path=this_script.parent, search_for=f'{next_num_search}*')
+    # check if the path exists, which is required for this script
+    if dir_path.is_dir():  # if the input path is an existing directory...
+        return dir_path  # return the Path as is
 
-    if (auto) or ((current_num + 1) in to_run):
-        print(f'\n\nRunning next step, {next_script.name}...\n')
-        subprocess.run(['python3', next_script])
-        return None
-    elif (current_num + 1) in to_exclude:
-        i = 2
-        while (current_num + i) in to_exclude:
-            i += 1
-        next_num_search = format_num_for_search(current_num + 1)
-        next_wanted = flag_multiple_files(file_path=this_script.parent, search_for=f'{next_num_search}')
-        print(f'\n\nRunning next step, {next_wanted.name}...\n')
-        subprocess.run(['python3'], next_wanted)
-        return None
-    else:
-        to_next = input(f'The script {current_script} has completed. Would you like to continue '
-                        f'to the next step in the pipeline, {next_script.stem}?[Y/N]\n'
-                        f'\n')
-        if re.search(AFFIRM_REGEX, to_next, re.I):
-            print(f'\n\nRunning next step, {next_script.name}...\n')
-            subprocess.run(['python3', next_script])
-            return None
+    else:  # if the input path is NOT an existing directory...
+
+        # trigger yes/no/quit prompt for adding a different path
+        msg = f'The provided input path is not an existing directory:\n '\
+              f'\t{dir_path}\n'\
+              f'Would you like to provide a different directory?'  # do not include last line break, prompt_ will add
+
+        if auto_respond:
+            print(f'\tauto response: quit\n')
+            sys.exit()
         else:
-            return print(f'\n\nExiting the completed step, {current_script}.\n')
+            prompt_yes_no_quit(message=msg)  # will exit here if no/quit is selected, continue to next line if 'yes'
+
+            # if yes, then prompt for updated path
+            print(f'Please provide the new file path to use below:\n')
+            new_path = input('>  ')
+
+            # recursively run function to ensure that this new path exists
+            return check_dir_exists(dir_path)
 
 # log progress of bioinformatics pipeline
 def log_progress(file_map, run_name):
     log_file = file_map['pipeline-output']['summary'] / f'log_{run_name}.json'
 
     log_dict = {'run_name': run_name,
                 'error': {'script':'04_quality-filtering',
                           'function':''}
                 }
 
     with open(log_file, 'at') as log_out:
         log_out.write(json.dumps(log_dict))
 
-
-
 # exit current script due to error, save script and timestamp of where error occurred
 def exit_process(message, config_section='error.message'):
     script_name = sys.argv[0]  # unsure if will get name of script it is executed in or the one it is compiled in
     exit_time = datetime.today().strftime('%Y-%m-%d %H:%M:%S')
     # write_to_config(config_section=config_section, script=script_name, timestamp=exit_time, details=message)
     print(f'Exiting {script_name}...\n')
     return sys.exit()
 
 # recursive function that will seek out yes/no/quit response continuously until achieved
-def prompt_yes_no_quit(message):
+def prompt_yes_no_quit(message, auto_respond=False):
     '''
     User prompt accepting specific responses.
 
     Takes the input of a print message that shows just prior to a user prompt. The message
     should specify the potential responses of yes/y, no/n, or quit/exit (case insensitive).
     If the user inputs a response that is not one of these potential responses, it will provide
     a notification that the input response was not recognize, and relist the acceptable responses.
@@ -156,72 +147,82 @@
     script will be run; if response is no/n/quit/exit, then it will exit the current script; if the
     response is unfamiliar, it will print an alert for invalid input, and restart the prompt
     again until an acceptable answer is received.
     '''
 
     print(f'{message} [yes/no/quit]\n')
 
+    if auto_respond:
+        return print(f'\tauto response: yes\n')
+
     response = input()
 
     if re.search(YES_RE, response, re.I):
         return None
     elif re.search(NO_RE, response, re.I) or re.search(QUIT_RE, response, re.I):
         print(f'Exiting...\n')
         return sys.exit()
     else:
         print(f'Your response was not recognized out of the list of potential responses. Please respond with '
               f'\'yes\', \'no\', or \'quit\'.\n')
         return prompt_yes_no_quit(message)
 
 # print out list of options for option-based prompts
-def prompt_print_options(option_list):
+def prompt_print_options(option_list, auto_respond=False):
+
     option_list.sort()  # sort option list for easier user experience
     option_list.append('quit')  # add option to quit, listed last
 
+    if auto_respond:
+        print(f'options: {option_list}\n')
+        print(f'\tauto response: quit\n')
+        return sys.exit()
+
     for o,opt in enumerate(option_list):
         if (o+1) < len(option_list):
             print(f'\t[{o+1}]: {opt}')  # print out all options from option list, excluding final option
         else:
             selected_opt = input(f'\t[{o+1}]: {opt}\n')  # print out last option from option list as prompt
 
     result = option_list[int(selected_opt)-1]  # return the item from option list matching the user input
 
     if result == 'quit':
         return sys.exit()
     else:
         return result
 
 # print a CLI prompt when multiple files are detected when only one is expected
-def prompt_multiple_files(file_path):
+def prompt_multiple_files(file_path, auto_respond=False):
     print(f'\nWARNING: Multiple files were detected in the '
           f'{file_path.stem} folder. Please type the number '
           f'corresponding to the correct file to use:')
     file_list = [file.stem for file in file_path.glob('*') if not re.search(HIDDEN_FILE_REGEX, file.stem)]
-    return prompt_print_options(file_list)
+    return prompt_print_options(file_list, auto_respond=auto_respond)
 
 # provide options for the sequencing platform if it cannot be otherwise detected
-def prompt_sequencing_platform(sample_id):
+def prompt_sequencing_platform(sample_id, auto_respond=False):
     print(f'\nWARNING: The sequencing platform could not be inferred from the sample: {sample_id}. Please type '
           f'the number corresponding to the correct sequencing platform from the options below. ')
-    platform = prompt_print_options([SEQ_PLATFORM_OPTS, 'multiple'])
+    platform = prompt_print_options([SEQ_PLATFORM_OPTS, 'multiple'],
+                                    auto_respond=auto_respond)
     if platform == 'multiple':
         print(f'If you have a combination of sequences from multiple platforms, you will need to either:\n'
               f'(1) manually sort the files into their sequencing platform directories\n'
               f'(2) use the file renaming script, rename_sequence_files.py, to rename the files to match '
               f'the file naming convention.\n')
         return
 
 # print indented list
 def print_indented_list(print_list):
     print_list[0] = '\t' + print_list[0] # add leading tab for first item printed from list, otherwise adds after line break
     formatted_list = '\n\t'.join(print_list)
     return print(formatted_list)
 
 # run shell command and save stdout and stderr to file
-def run_subprocess(cli_command_list, dest_dir):
+def run_subprocess(cli_command_list, dest_dir, auto_respond=False):
     '''
     Run a subprocess, saving the output and error to a log file.
 
     Takes the command line (CL) argument assembled as a list, and runs
     the subprocess, saving the standard in (stdin), standard out (stdout),
     and standard error (stderr) from the process. The output of stderr and
     stdout are written to a log file in the destination directory
@@ -239,127 +240,355 @@
                                                                              f'Try shlex.split() if unsure how to '
                                                                              f'compose the list. ')
 
     # run_cmd = subprocess.run(cli_command_list, stdin=PIPE, stdout=PIPE, stderr=PIPE)
     # out, err = run_cmd.communicate()
     program = cli_command_list[0]
 
-    if re.search('.\..', program):
+    if re.search(r'.\..', program):
         program = program.split('.')[0]
 
     run_cmd = subprocess.run(cli_command_list, capture_output=True)
 
     out_path = dest_dir / f'{program}.out'
     with open(out_path, 'at') as fout:
-        as_str = run_cmd.stdout.decode('utf-8')
-        if int(out_path.stat().st_size) == 0:
-            fout.write(as_str)
-        else:
-            fout.write(as_str.split('\n')[1] + '\n')
+        out_as_str = run_cmd.stdout.decode('utf-8')
+        if not int(out_path.stat().st_size) == 0:
+            fout.write(f'-----------------------------\n')
+        if len(out_as_str) > 0:
+            fout.write(f'{out_as_str}\n')
 
     err_path = dest_dir / f'{program}.err'
-    with open(err_path, 'ab') as fout:
-        fout.write(run_cmd.stderr)
+    with open(err_path, 'at') as fout:
+        err_as_str = run_cmd.stderr.decode('utf-8')
+        if not int(err_path.stat().st_size) == 0:
+            fout.write(f'-----------------------------\n')
+        if len(err_as_str) > 0:
+            fout.write(f'{err_as_str}\n')
 
     temp_file = dest_dir / f'{program}.temp'
 
     if len(run_cmd.stderr) == 0:
         pass
     else:
-        if not temp_file.is_file():
-            continue_ok = input(f'Running {program} produced an error. Please review the output in {err_path.name}. '
-                                f'Would like to continue despite this error? [Y/N]')
-            if re.search(continue_ok, AFFIRM_REGEX, re.I):
-                with open(temp_file, 'wt') as fout:
+        if not temp_file.is_file():  # if the temp_file does not exist (i.e., prompt already responded to)
+            print(f'Running {program} produced an error. Please review the output in {err_path.name}. '
+                  f'Would like to continue despite this error? [yes/no]')
+            if auto_respond:
+                print(f'\tauto response: yes\n')
+                with open(temp_file, 'wt') as fout:  # still want to write to this file so it stops asking
                     fout.write('stop_prompt')
-                return None
             else:
-                return exit_process(message=f'Running {program} produced an error. See {err_path.name} for details.')
+                continue_ok = input()
+                if re.search(continue_ok, AFFIRM_REGEX, re.I):
+                    with open(temp_file, 'wt') as fout:
+                        fout.write('stop_prompt')
+                else:
+                    return exit_process(message=f'Running {program} produced an error. See {err_path.name} for details.')
 
     return None
 
 def func_timer(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
-        start_time = datetime.datetime.now()
+        start_time = datetime.now()
         func_output = func(*args, **kwargs)
-        end_time = datetime.datetime.now()
+        end_time = datetime.now()
         runtime = str(end_time - start_time).split('.')[0]  # round seconds down
         print(f"{func.__name__} was executed in {runtime}.\n")
         return func_output
     return wrapper()
 
-def get_seq_platform(fastx_file, delim):
+def get_seq_platform(fastx_file, delim='_'):
     if isinstance(fastx_file, str):
         sample_id = fastx_file
-    elif is_pathclass(fastx_file):
-        sample_id = fastx_file.stem
+    elif is_pathclass(fastx_file, exit_if_false=False):
+        sample_id = fastx_file.name
     else:
-        print(f'ERROR. An error occurred when trying to detect the sequencing platform from the '
-              f'sample ID: {fastx_file}\n')
+        print(f'ERROR. Could not read the file name when trying to detect the sequencing platform '
+              f'from the file name: {fastx_file}\n')
+        return None
 
+    # check the file name components for any of the expected platforms: pacbio, illumina, sanger
+    platform = []
+    for v in sample_id.split(delim):
+        if re.search(PLATFORM_ANYWHERE_RE, v, re.I):
+            platform.append(v)
+        else:
+            continue
 
-    platform = sample_id.split(delim)[0]
-    if platform in SEQ_PLATFORM_OPTS:
-        return platform
+    # confirm that only one platform was encountered in the file name
+    if len(platform) == 1:
+        return platform[0]
+    elif len(platform) > 1:
+        print(f'There were multiple sequencing platforms detected:\n'
+              f'\tfile name: {sample_id}\n'
+              f'\tplatforms detected: {platform}\n')
     else:
-        pass
+        print(f'No sequence platforms were detected:\n'
+              f'\tfile name: {sample_id}\n')
+
+    print(f'May not be able to continue without a clear sequencing platform.\n'
+          f'Exiting...\n')
+    return None
 
-def import_mapping_df(df_path):
+def import_mapping_df(df_path, auto_respond=False):
     '''
     Import .csv, .txt, or .xlsx table as a dictionary.
 
     Read in a mapping file for demultiplexing. Can accomodate the file formats
     .xlsx, .csv, and .txt. Will output a dictionary, where the key is the name
     of the tab in the dataframe and the value is the dataframe in that tab. Will
     always return a dictionary, although only .xlsx files will have tabs. Formats
     the name of the keys in the output dictionary to be 'pool1' or 'pool2'; the
     number of the pool is inferred from the name of the tab (.xlsx) or the name
     of the file (.csv, .txt). Returned as dictionary so that the output can be
     handled in the same way, regardless of file type (e.g., loop through tabs
     even if a .csv, which will have a single tab).
     :param df_path: path to the dataframe
+    :param auto_respond: True/False; whether to automatically respond to the prompt
+    within or not; this value should be provided from the settings read in from the
+    configuration file, within ['automate']['auto_respond']
     :return: dictionary, where the key is 'pool1' or 'pool2', and the value is the
     dataframe belonging to that tab, or in the case of a .csv or .txt file, the
     entirety of that dataframe file.
     '''
 
-    POOL_NUM_RE = '(?<=pool).?(\d)'
+    # if the mapping file is an excel file...
+    if re.search(r'^\.x', df_path.suffix):
 
-    if re.search('^\.x', df_path.suffix):  # if an excel file
+        # read in all tabs from the table
         mapping_tabs = pd.read_excel(df_path, sheet_name=None)  # need to set sheet_name to None to get all tabs
         old_tab_names = list(mapping_tabs.keys())  # make list of old names, otherwise cannot update key names in loop
+
+        # create a set to add pool numbers to when they are found from tabs in .xlsx file
+        # if there are multiple tabs, some of which are unrelated to pools, will need to reference this
+        found_pools = {'pool01':'',
+                       'pool02':''}
+        miscell_tabs = []
+
         for tab in old_tab_names:
+
             try:  # format the name of the tab to be uniform across all tabs/dataframes
                 pool_num = re.search(POOL_NUM_RE, tab, re.I).group(0)
-            except AttributeError:
-                print(f'The pool number could not be inferred from tab {tab} in the mapping file {df_path.name}. '
-                      f'Please type the correct pool number for this file: ')
-                pool_num = prompt_print_options(['1', '2'])  # choose from 1 or 2 (or quit, built into function)
-            mapping_tabs[f'pool{pool_num}'] = mapping_tabs.pop(tab)  # replace old tab (key) with reformatted one
-    elif re.search('^\.c|^\.txt$', df_path.suffix):  # I think you can read in .txt and .csv files the same way?
+
+                # add the found pool number to the found_pools set
+                if re.search(r'1', pool_num):
+                    found_pools['pool1'] = tab
+                elif re.search(r'2', pool_num):
+                    found_pools['pool2'] = tab
+                else:
+                    print(f'ERROR. A pool number was detected in the tab {tab} in the mapping file {df_path.name}, '
+                          f'but it could not be determined whether this was the number for pool 01 or pool 02.\n')
+                    return sys.exit()
+
+            except AttributeError:  # if this tab does not contain pool information, or at least not detected as such...
+
+                # add this tab name to the miscell_tabs list to check at end whether might be a pool tab or not
+                miscell_tabs.append(tab)
+
+            for pool_num, pool_tab in found_pools.items():
+
+                # if no tab was found matching this pool...
+                if pool_tab == '':
+
+                    # print a warning and prompt user to chose the tab that corresponds to this pool
+                    print(f'WARNING. The pool number for {pool_num} could not be inferred from tabs in the '
+                          f'mapping file {df_path.name}. Please enter the number of the tab that corresponds to '
+                          f'{pool_num}')
+
+                    # will return the name of the tab to use, so update var pool_tab to match
+                    pool_tab = prompt_print_options(miscell_tabs, auto_respond=auto_respond)
+
+                mapping_tabs[pool_num] = mapping_tabs.pop(pool_tab)  # replace old tab (key) with reformatted one
+
+
+
+    # if the mapping file is a .csv or .txt file...
+    elif re.search(r'^\.c|^\.txt$', df_path.suffix):  # I think you can read in .txt and .csv files the same way?
+
         try:  # try to get the pool number from the file name
+
             pool_num = re.search(POOL_NUM_RE, df_path.name, re.I).group(0)
+
         except AttributeError:  # if there's no detected pool number in the name, prompt user to specify one
+
             print(f'The pool number could not be inferred from the file name of the mapping file {df_path.name}. '
                   f'Please type the correct pool number for this file: ')
-            pool_num = prompt_print_options(['1', '2'])  # choose from 1 or 2 (or quit, built into function)
+            pool_num = prompt_print_options(['1', '2'], auto_respond=auto_respond)  # choose from 1 or 2 (or quit, built into function)
+
         mapping_tabs = {f'pool{pool_num}': pd.read_csv(df_path)}  # make dict to match format from .xlsx
+
+    # if the mapping file doesn't appear to be .xlsx, .csv, or .txt...
     else:
+
+        # can't use this file with the current version of the pipeline functions
         print(f'ERROR. The file format {df_path.suffix} of the mapping file {df_path.name} is not a recognized '
               f'file type. Accepted file types are: \'.xlsx\', \'.csv\', and \'.txt\'.\n')
         sys.exit()
 
     return mapping_tabs
 
+# activate next script in python
+def continue_to_next(this_script, config_dict):
+    '''
+    Continue to the next step of the pipeline.
+
+    Will activate the script from the CLI with default
+    parameters. If you do not want to use the default
+    parameters, opt out of automated continuation by
+    responding to the CLI prompt that precedes the use
+    of this function.
+    :param this_script: use __file__ always
+    :return: None, assembles and runs a shell command.
+    '''
+
+    # if the input is not a Path class, make it a Path class
+    if is_pathclass(this_script, exit_if_false=False):
+        pass
+    else:
+        this_script = Path(this_script)
+
+    # read in automation details from the configuration file
+    automate_dict = config_dict['automate']
+    auto = automate_dict['run_all']
+    to_run = automate_dict['run_some']
+
+    # get the number of the current script from its prefix, cast as int for comparison
+    current_num = int(this_script.name.split('_')[0])
+
+    # using the current script's number, create search string for next script to run
+    def format_num_for_search(current_script_number, consecutive=True):
+
+        # get int of next script based on configuration settings
+        if consecutive:  # if automate = True, run the next consecutive script
+            next_int = current_script_number + 1
+        else:  # if automate = False and len(run_sum) > 0, determine next script to run
+            if len(to_run) > 0:
+                # get the index of this current script in the to_run list
+                current_script_runlist_i = to_run.index(current_script_number)
+                # if it is the last int in this list...
+                if current_script_runlist_i == (len(to_run) - 1):
+                    # return None, which will trigger a print/exit in the parent function
+                    return None
+                # if there are more items in the scripts to run...
+                else:
+                    # next_int will be the next number in that list
+                    next_int = to_run[current_script_runlist_i + 1]
+
+        # format the next script int as a string, w/ (0-9) or w/o (10+) leading zero
+        if next_int >= 10:  # if in double-digits, don't add a leading zero
+            next_num_search = str(next_int)
+        else:  # if single digit, add leading zero
+            next_num_search = '0' + str(next_int)
+
+        return next_num_search
+
+    # give priority to numbered scripts to run, even if auto left on True
+    if len(to_run) > 0:  # if there are entries in to_run...
+
+        # find the next value in this list (*not* consecutive, but based on to_run settings)
+        next_num_search = format_num_for_search(current_num, consecutive=False)
+
+        # if there are none (i.e., current script is last one in this list)
+        if next_num_search is None:
+            # print that steps are completed, and exit
+            print(f'\nThe pipeline has run all steps designated in the run_some section of the configuration '
+                  f'settings. Exiting the pipeline...\n')
+            return sys.exit()
+
+        # if there are scripts after this current one to run
+        else:
+            # find the file of the next script, based on format_num_for_search output
+            next_script = flag_multiple_files(file_path=this_script.parent, search_for=f'{next_num_search}*',
+                                              auto_respond=config_dict['automate']['auto_respond'])
+
+    # if no specific scripts specified...
+    else:
+
+        # find the next consecutive script
+        next_num_search = format_num_for_search(current_num, consecutive=True)
+        next_script = flag_multiple_files(file_path=this_script.parent, search_for=f'{next_num_search}*',
+                                          auto_respond=config_dict['automate']['auto_respond'])
+
+        # if set to automatically run, then continue to last print/return statement
+        if auto:
+            pass
+
+        # if not set to auto-run, prompt user to determine whether to continue
+        else:
+            msg = f'The script {this_script} has completed. Would you like to continue '\
+                  f'to the next step in the pipeline, {next_script.stem}?'
+            prompt_yes_no_quit(msg, auto_respond=config_dict['automate']['auto_respond'])  # if response is yes, it will continue to next line; if no, will exit here
+
+    print(f'\n\nRunning next step, {next_script.name}...\n')
+    return subprocess.run(['python3', next_script])
 
 #######################
 # FILE PATHS ##########
 #######################
 
+
+def import_filepath(arg_value, must_exist, make_absolute=True):
+    '''
+    Import a file path from parsed command line options as a Path object.
+
+    Takes the value returned from a parsed argparse argument, typically as
+    a dictionary element. Should also accept an argparse Namespace class as
+    long as it has already been indexed into a string (makes no difference).
+    :param arg_value: value from the parsed command line argument that expects
+    a path-like string or Path object (e.g., for default values from config files)
+    :param
+    :param make_absolute: whether to convert the Path object to an absolute
+    file path if a relative file path is provided
+    :return: the input path as a Path object
+    '''
+
+    # convert input to a Path class object
+    if is_pathclass(arg_value, exit_if_false=False):
+        input_path = arg_value
+    else:
+        input_path = Path(arg_value)
+
+    # check through the rest of the settings for the path (must_exist, make_absolute)
+
+    # if the path must exist and want to make it absolute...
+    if make_absolute and must_exist:  # [T/T]
+        try:  # using strict=True will both check that the path exists and make it absolute
+            return input_path.resolve(strict=True)
+        except FileNotFoundError:  # if it doesn't exist, then FileNotFoundError will be triggered
+            # in this case, print an error message with the error-causing path, and exit function
+            # because there is one other section with same error message, just pass and will print error + exit at end
+            pass
+
+    # if only want to make the path absolute...
+    elif make_absolute:  # [T/F] if it were both, it would have already execute first if statement
+        return input_path.resolve(strict=False)
+
+    # if I only want to ensure that the path exists...
+    elif must_exist:  # [F/T] if make_absolute were true, it would have executed by now
+        if input_path.is_dir() or input_path.is_file():  # accept either directories or files
+            return input_path
+        else:
+            # because there is one other section with same error message, just pass and will print error + exit at end
+            pass
+
+    # if I don't want either setting; I don't want to require that path exists nor that the path be absolute
+    else:
+        return input_path
+
+    # print collected ERROR message, if any, and exit script if this point is reached
+    # only errors will not have returned anything by now
+    msg = (f'ERROR. The following path provided does not exist: \n'
+           f' {input_path} \n'
+           f'A path to an existing file or directory is required for this function. '
+           f'Please check this path and then rerun.\n')
+    print(msg)
+    return sys.exit()
+
 def filter_empty_files(dir_path, keep_empty=True):
     empty_files = 0
     empty_folders = 0
     for file in dir_path.glob('*'):
         if file.stat().st_size == 0:
             empty_files += 1
             if keep_empty:
@@ -374,19 +603,19 @@
                 fate = 'deleted'
         elif file.is_dir():
             try:  # empty dirs not always size 0 (hidden files); this will only rm dir if it is empty (but not 0)
                 file.rmdir()
                 fate = 'deleted'
                 empty_folders += 1
             except:
-                continue
                 fate = ''
+                continue
         else:
-            continue
             fate = ''
+            continue
 
     return print(f'{empty_files} files and {empty_folders} folders were {fate}.\n')
 
 # check whether a path exists; return path if it does or raise error if it does not
 def flag_if_not_path_exists(file_path, absolute=True, exit_if_false=True):
     '''
     Create a Path class using the provided filepath string.
@@ -483,16 +712,14 @@
     source_path.rename(full_dest_path)
 
     if full_dest_path.is_file():
         return None
     else:
         return print(f'The file {source_path.name} was not properly copied to its new destination: {dest_path}.')
 
-# sort the sequences provided in the 'sequences' input directory
-
 # count the number of files in a directory
 def count_files(file_path, search_for='*'):
     '''
     Counts the number of files in a file path, and returns as int.
 
     :param file_path: path to directory to count files in.
     :param search_for: the .glob string that describes the file types
@@ -500,15 +727,14 @@
     :return: int of the number of files in directory
     '''
     # check if it is a file path that exists
     flag_if_not_path_exists(file_path, absolute=False, exit_if_false=False)
 
     return len(list(file_path.glob(search_for)))
 
-
 def check_for_input(file_dir, seq_platform=None, file_ext=SEQ_FILE_GLOB):
     '''
     Checks if there are input files for the process.
 
     :param file_dir: the directory path to check for files and to check
     whether the path exists
     :param seq_platform: the type of sequencing files to look for ['illumina',
@@ -516,34 +742,34 @@
     non-empty directory or file is located
     :param file_ext: the expected file extension of the files to search for,
     using asterisk '*' for wildcard (used in glob)
     :return: two items; [1] Boolean T/F, whether there is a directory in this
     path that contains sequencing files; [2] a list of the files matching the
     file extension in the directory, if present
     '''
-    assert is_pathclass(file_dir)
+    assert is_pathclass(file_dir)  # must be Path class or .is_dir() won't work, and it will say dir doesn't exist
 
     # I decided to leave this out so you could put any regex in (i.e., multiplexed pacbio files will start with \d{4}
     # accepted_seq_input = [None, 'illumina', 'sanger', 'pacbio']
     # if not seq_platform in accepted_seq_input:
     #     print(f'The provided sequencing platform, {seq_platform}, is not one of the accepted '
     #           f'values: {accepted_seq_input}. Please retry with one input value from this list '
     #           f'as a string, or multiple values as a list of strings.\n')
     #     return sys.exit()
 
     if seq_platform is None:
-        seq_re = '.+?'  # will return all files in directory
+        seq_re = r'.+?'  # will return all files in directory
     elif isinstance(seq_platform, list):
         seq_re = '|'.join(seq_platform)  # returns only those in provided list
     else:
         seq_re = seq_platform  # returns only those of the provided platform
 
     if file_dir.is_dir():  # check that input is a directory
         if count_files(file_path=file_dir, search_for=file_ext) > 0:  # confirm it is not empty
-            file_list = [f for f in file_dir.glob('*') if re.search(seq_re, f.name, re.I)]  # check for specific files
+            file_list = [f for f in file_dir.glob(file_ext) if re.search(seq_re, f.name, re.I)]  # check for specific files
             if len(file_list) > 0:
                 return True, file_list  # return true if files matching criteria are found
             else:
                 print(f'The directory {file_dir} contains files, but none that match the platform-specific search '
                       f'criteria: {seq_platform}.')
                 return False, file_list  # return false if not
         else:
@@ -553,14 +779,92 @@
     else:
         file_list = []  # if input is not a directory
         print(f'The directory {file_dir} does not exist.\n')
         return False, file_list  # return false and empty list
 
 # get name of previous script
 
+# compress a fastq file to .fastq.gzip format
+# DOES NOT WORK, WILL NOT COMPRESS A .FASTQ FORMAT BECAUSE IT CAN'T DETECT BYTES
+def gzip_compress(uncompressed_path, delete_uncompressed=True, **kwargs):
+    '''
+    Compress an input file to the gzip compression format.
+
+    :param uncompressed_path: Path object describing path to the uncompressed
+    file that requires compression
+    :param delete_uncompressed: True (default), False; whether to remove the
+    uncompressed version of the file after successfully compressing it
+    :param kwargs: compressed_path may be provided, which should be a Path object
+    that is used as the output path for the compressed version of the input file; if
+    one is not provided, then the input uncompressed Path is used as the basis for
+    the compressed file name
+    :return: None; saves the gzip version
+    '''
+
+    # confirm that the input uncompressed file is a Path object
+    if is_pathclass(uncompressed_path):
+        pass
+    else:
+        try:  # try to create a Path object from the input
+            uncompressed_path = Path(uncompressed_path)
+        except:  # if it can't be converted to a Path object, then print error and exit
+            msg = (f'The path provided, {uncompressed_path}, was not originally a Path object, and could not be '
+                   f'automatically converted to a Path object. Please provide a Path object to '
+                   f'the parameter \'uncompressed_path\' to continue.\n')
+            return exit_process(message=msg)
+
+    # if the compressed path is provided as a keyword argument...
+    if 'compressed_path' in kwargs.keys():
+        # confirm that it is a Path object
+        if is_pathclass(kwargs['compressed_path']):
+            # write in to variable
+            compressed_path = kwargs['compressed_path']
+        # if it is not a Path object...
+        else:
+            try:  # try to create a Path object from the input
+                compressed_path = Path(kwargs['compressed_path'])
+            except:  # if it can't be converted to a Path object, then print error and exit
+                msg = (f'The path provided, {kwargs["compressed_path"]}, was not originally a Path object, '
+                       f'and could not be automatically converted to a Path object. Please provide a Path '
+                       f'object to the keyword \'compressed_path\' to continue.\n')
+                return exit_process(message=msg)
+    # if no keyword argument for compressed path is included...
+    else:
+        # create compressed path by adding .gz to input uncompressed path
+        compressed_path = uncompressed_path.with_suffix('.'.join([uncompressed_path.suffix, 'gz']))
+
+    # first open the uncompressed file to read content
+    with open(uncompressed_path, 'rb') as uncomp_in:
+        # then open the compressed file to write uncompressed content to
+        with gzip.open(compressed_path, 'wb') as comp_out:
+            # read uncompressed content and write to the gzip output file
+            shutil.copyfileobj(uncomp_in, comp_out)
+
+    # check that the compressed file isn't empty
+    if compressed_path.stat().st_size == 0:
+        msg = (f'ERROR. The uncompressed file, {uncompressed_path.name}, was not successfully written to the '
+               f'compressed file {compressed_path.name}, as the compressed file size is zero (0).\n')
+        return exit_process(message=msg)
+
+    # check that the compressed file is properly compressed
+    with open(compressed_path, 'r') as comp_in:
+        try:
+            comp_in.read(1)
+        except gzip.BadGzipFile:
+            msg = (f'ERROR. The uncompressed file, {uncompressed_path.name}, was not successfully written to the '
+                   f'compressed file {compressed_path.name}, as the compressed filee was flagged as BadGzipFile '
+                   f'by the gzip Python library.\n')
+            return exit_process(message=msg)
+
+    # remove uncompressed file, if delete_uncompressed set to True (default)
+    if delete_uncompressed:
+        uncompressed_path.unlink()
+
+    return None
+
 #######################
 # TEXT MANIPULATION ###
 #######################
 
 # add prefix to file name
 def add_prefix(file_path, prefix, dest_dir, action='rename', f_delim='_'):
     '''
@@ -581,15 +885,15 @@
     :return: Path object with new file name
     '''
 
     assert is_pathclass(file_path, exit_if_false=False)
 
     def prefix_single(file_name):
         old_name = file_name.name
-        platform_present = re.search('illumina|pacbio|sanger', old_name, re.I)
+        platform_present = re.search(r'illumina|pacbio|sanger', old_name, re.I)
         try:
             # if there's a match, put prefix before the platform, remove all else
             location = platform_present.span()[0]
             new_name = prefix + f_delim + old_name[location:]
         except:
             # if there's no match, just add prefix to start of file name
             new_name = prefix + f_delim + old_name
@@ -610,15 +914,16 @@
         new_path_list = []
         for file in file_path.glob('*'):
             new_path_list.append(prefix_single(file))
         return new_path_list
     elif file_path.is_file():
         return prefix_single(file_path)
     else:
-        msg = f'FAILURE. Unrecognized input file; cannot recognize as either a directory or file.\n'
+        msg = (f'FAILURE. Unrecognized '
+               f' file; cannot recognize as either a directory or file.\n')
         return exit_process(msg)
 
     # filename_start = file_name.name.split('_')[0]
     # if re.search(ANY_PLATFORM_REGEX, filename_start, re.I):
     #     return dest_path / f'{prefix}_{file_name.name}'
     # elif re.search(ANY_PLATFORM_REGEX, file_name.name.split('_')[1], re.I):
     #     return dest_path / file_name.name.replace(filename_start, prefix)
@@ -647,20 +952,20 @@
     '''
     assert is_pathclass(parent)
 
     if not parent.is_dir():
         parent = mkdir_exist_ok(new_dir=parent)
 
     script_num = Path(script_name).stem.split('_')[0]
-    script_name_nonum = re.sub('^\d+_(?=\w)','',Path(script_name).stem)
+    script_name_nonum = re.sub(r'^\d+_(?=\w)',r'', Path(script_name).stem)
     completed_name_nonum = OUTPUT_DIRS[script_name_nonum]
     completed_name = f'{script_num}_{completed_name_nonum}'
 
     if remove_num:
-        completed_name = re.sub('^\d+_(?=\w)','', completed_name)
+        completed_name = re.sub(r'^\d+_(?=\w)',r'', completed_name)
 
     if suffix:
         out_path = parent / f'{completed_name}_{suffix}'
     else:
         out_path = parent / completed_name
 
     out_path.mkdir(exist_ok=True)
@@ -671,55 +976,53 @@
     # not sure why I would check if the prefix was a path? I don't think I ever use a path, just a constant string?
     # was throwing error when checking for PhiX in prefilter step, though was creating directory, error creating file
     # if is_pathclass(prefix_const, exit_if_false=False):
     #     prefix_const = prefix_const.stem
     # else:
     #     pass
 
-    if re.search('^no-', prefix_const, re.I):  # if provided prefix starts with no, remove no
-        return re.sub('^no-', '', prefix_const, re.I)
+    if re.search(r'^no-', prefix_const, re.I):  # if provided prefix starts with no, remove no
+        return re.sub(r'^no-', r'', prefix_const, re.I)
     else:  # if it does not start with no, add no
         return 'no-' + prefix_const
 
 def rename_read_header(fasta_file, header_delim=';'):
+
     # fasta_file = next(post_itsx.glob('*.fast*'))
     parent_dir = fasta_file.parent.name
 
-    if re.search('itsx', parent_dir, re.I):  # if they are post-itsx reads...
+    # get the sequence platform, to use when searching for the sample_id from the file name
+    seq_platform = get_seq_platform(fasta_file)
 
-        READ_COUNT_RE = '(?<=size=)[0-9]{1,}'
-        READ_LEN_RE = '[0-9]{1,}(?=\sbp)'
-        READ_ID_RE = '[0-9]{1,}(?=\/ccs)'
-        READ_REGION_RE = '(?<=\|\w\|).+(?=\sExtracted)'
-        SAMPLE_ID_RE = '(?<=\w_)(pacbio|sanger|illumina).+?(?=\.)'
+    if re.search(r'itsx', parent_dir, re.I):  # if they are post-itsx reads...
 
-        # REPLACE WITH REMOVE PREFIX??
-        sample_id = re.search(SAMPLE_ID_RE, fasta_file.name).group(0)
+        sample_id = get_sample_id(file_path=fasta_file, platform=seq_platform)
 
         updated_records = []
         no_update_count = 0
         for record in SeqIO.parse(fasta_file, 'fasta'):
             header = record.description
             try:
-                read_id = re.search(READ_ID_RE, header).group(0)
-                region = re.search(READ_REGION_RE, header).group(0)
-                read_count = re.search(READ_COUNT_RE, header).group(0)
-                read_length = re.search(READ_LEN_RE, header).group(0)
+                read_id = re.search(READ_ID_OG_RE, header).group(0)
+                region = re.search(READ_REGION_OG_RE, header).group(0)
+                read_count = re.search(READ_COUNT_OG_RE, header).group(0)
+                read_length = re.search(READ_LEN_OG_RE, header).group(0)
 
                 updated_header = header_delim.join([f'{sample_id}_{read_id}', region, f'region_len={read_length}bp',
                                                     f'full-len_copies={read_count}'])
 
                 record.id = updated_header
                 record.name = f'{sample_id}_{read_id}'
                 record.description = ''
                 updated_records.append(record)
             except:
                 no_update_count += 1
                 updated_records.append(record)
 
+
         SeqIO.write(updated_records, fasta_file, 'fasta')
 
         if no_update_count == 0:
             return print(f'SUCCESS. All reads ({len(updated_records)}) were renamed '
                          f'in {fasta_file.name}.\n')
         elif no_update_count == len(updated_records):
             return print(f'FAILURE. None of the reads were renamed in {fasta_file.name}. This can '
@@ -732,178 +1035,223 @@
         return print(f'UNDER CONSTRUCTION. I haven\'t yet updated this function to work with any other '
                      f'fasta files than those produced after ITSx.\n')
 
 def escape_path_special(file_path):
     if is_pathclass(file_path):
         file_path = str(file_path)
 
-    if re.search('\(', file_path):
-        file_path = re.sub('\(', '\(', file_path)
+    if re.search(r'\(', file_path):
+        file_path = re.sub(r'\(', r'\(', file_path)
 
-    if re.search('\)', file_path):
-        file_path = re.sub('\)', '\)', file_path)
+    if re.search(r'\)', file_path):
+        file_path = re.sub(r'\)', r'\)', file_path)
 
     return file_path
 
+def get_sample_id(file_path, platform=None):
+    '''
+    Return the sample ID as a string from a file path.
+
+    :param file_path: Path object, whose .name attribute contains
+    the sample ID
+    :param platform: illumina, pacbio, sanger, or a custom platform
+    prefix used in the file name
+    :return: the sample ID of the input file, as a string
+    '''
+
+    # if at start, the platform is not provided...
+    if platform is None:
+        # try to get it from the file name
+        platform = get_seq_platform(file_path)
+        # if it is still None...
+        if platform is None:
+            platform_re = SAMPLE_ID_RE  # search for sample ID for any of the seq platforms
+        else:  # if it did find a platform, then use in regex
+            platform_re = r'(?<=_' + f'{platform.lower()}' + r'_).+?_0[1-9]'
+    else:  # if a platform was provided, then use this in the regex
+        platform_re = r'(?<=_' + f'{platform.lower()}' + r'_).+?_0[1-9]'
+
+    try:
+        sample_id = re.search(platform_re, file_path.name, re.I).group(0)
+        return sample_id
+    except AttributeError:
+        msg = (f'ERROR. The provided file name, {file_path.name}, does not follow the expected '
+               f'naming convention, so the sample ID cannot be inferred from the file name. '
+               f'This will affect the logging of summary data to output files.\n')
+        return exit_process(message=msg)
+
+def get_read_orient(file_path):
+    '''
+    Return the read orientation in file name as string (R1/R2).
+
+    :param file_path: Path object, whose .name attribute contains
+    the read orientation (R1 or R2)
+    :return: the sample ID of the input file, as a string
+    '''
+
+    try:
+        read_orient = re.search(ORIENT_RE, file_path.name, re.I).group(0)
+        return read_orient
+    except AttributeError:
+        msg = (f'ERROR. The provided file name, {file_path.name}, does not follow the expected '
+               f'naming convention, so the read direction cannot be inferred from the file name. '
+               f'This will affect the logging of summary data to output files.\n')
+        return exit_process(message=msg)
+
 #######################
 # CONFIGURATION #######
 #######################
 
 # define function to simplify import of configuration files
-def import_config_as_dict(file_path, file_handle, config_section='all'):
+def get_settings(file_map, default_only=True, config_section='all'):
     '''
-    Import a configuration file and return as a dictionary.
+    ***TEMPORARILY ONLY ACCEPTS THE DEFAULT CONFIG FILE.***
+
+    Imports user and default settings from .toml to a dictionary.
 
-    Checks the input path to ensure that the filepath exists; if
-    not, it will stop the process and exit the entire script.
-    Uses a custom parser to preserve the case of the text in the
-    configuration file (i.e., uppercase letters remain uppercase,
-    lowercase remain lowercase). Creates a dictionary where the
-    sections of the configuration file are the primary keys, if it
-    is a nested dictionary. If not a nested dictionary, will be
-    returned as an un-nested dictionary where the keys are the
-    section's keys.
-    :param file_handle: standard file handle used for the config file; will
-    default to the constants that work if the file structure of the container
-    is maintained
+    Looks for a default and a user configuration file in the config directory of
+    the bioinformatics pipeline. Reads in the information from the user configuration
+    file with priority. If a given field is empty in the user configuration, indicating
+    no user preference was provided for that setting, then the value for that field will
+    be searched for in the default configuration file.
+    :param file_map: file map describing the file organization of directories and
+    subdirectories in the pipeline; this file map is contained within the
+    mapping.py script and is typically the first item loaded into each pipeline
+    script
+    :param default_only: True; inserted this *TEMPORARY* parameter so that it will
+    only read in the default configuration file, rather than compiling the user
+    and default configuration
     :param config_section: option to output only one section of the configuration
     file.
-    :return: dictionary of values in the configuration file
+    :return: dictionary of settings, with keys as configuration file settings and
+    values as parameters chosen by the user (priority) or default settings.
     '''
-    path_to_file_abs = flag_if_not_path_exists(file_path, absolute=True)
 
-    config_file_list = list(path_to_file_abs.glob(f'*{file_handle}*'))
+    ##########################
+    # REMOVE AFTER TESTING ###
+    ##########################
+    # import tomlkit
+    # from mapping import filepath_map as file_map
+    # default_only = True
+    # config_section = 'all'
+    # ACTIVATE RETURN STATEMENTS (done)
+    ##########################
+
+    if default_only:
+        config_path_default = list(file_map['config']['main'].glob('*default-settings.toml'))
+
+        # confirm that only one of each type exists in the config directory
+        if len(config_path_default) > 1:
+            msg = f'\nERROR. Multiple default configuration files were located '\
+                  f'in the /config directory:\n'\
+                  f'\t{[file.name for file in config_path_default]}\n'\
+                  f'Please remove any extraneous default configuration files, then retry.\n'
+            return exit_process(message=msg)
+        else:  # update dict so that path is single path and not in list form
+            config_path = config_path_default[0]
+
+        # read in the config files as a new dict, with primary keys being user or default
+        with open(config_path, 'rt') as fin:
+            compiled_config = tomlkit.parse(fin.read())
+
+        # add the date to the default run name
+        # NO THIS CREATES A MESS, FIGURE OUT SOMETHING ELSE AT SOME POINT
+        # date_obj = datetime.today()
+        # date_tag = date_obj.strftime('%y%m%d')  # format is YYMMDD
+        # compiled_config['run_details']['run_name'] = (compiled_config['run_details']['run_name'] + date_tag)
+
+    else:
+        print(f'ERROR. Compilation of pipeline settings from both the user and default configuration files is '
+              f'still under construction. If you see message, ensure that default_only=True for the function '
+              f'get_settings().\n')
+        # get path to the configuration files (/config) from the mapping.py file input
+        config_path_user = list(file_map['config']['main'].glob('*user-settings.toml'))
+        config_path_default = list(file_map['config']['main'].glob('*default-settings.toml'))
+
+        # create a dictionary for a config file description (i.e., user/default) and its file path
+        config_paths = {k:v for k,v in zip(['user', 'default'], [config_path_user, config_path_default])}
+
+        # confirm that only one of each type exists in the config directory
+        for t in config_paths:
+            if len(config_paths[t]) > 1:
+                msg = f'\nERROR. Multiple {t} configuration files were located '\
+                      f'in the /config directory:\n'\
+                      f'\t{[file.name for file in config_paths[t]]}\n'\
+                      f'Please remove any extraneous {t} configuration files, then retry.\n'
+                return exit_process(message=msg)
+            else:  # update dict so that path is single path and not in list form
+                config_paths[t] = config_paths[t][0]
+
+        # read in the config files as a new dict, with primary keys being user or default
+        configs = {k:{} for k in config_paths}
+        for p in config_paths:
+            with open(config_paths[p], 'rt') as fin:
+                configs[p] = tomlkit.parse(fin.read())
+
+        # get a set of config dictionary keys for each type
+
+        # generator that produces all keys, even nested ones
+        def find_config_keys(type_dict):
+            '''
+            Find primary and nested sections of a .toml file.
+
+            :param type_dict: sectioned dictionary containing configuration values only
+            for the default or only for the user settings, e.g., configs['user']
+            :return: a set of unique keys in the given config
+            file
+            '''
+
+            for key,val in type_dict.items():
+                # if section is nested...
+                if isinstance(val, dict):
+                    # check this nested portion for more keys
+                    yield from find_config_keys(val)
+                # if section is not nested...
+                else:
+                    # return key
+                    yield key
+
+        # go through each dict and create a set of keys for each, save into another dict
+        unique_keys = {k:{} for k in configs}
+        for t in configs:
+            unique_keys[t] = set(k for k in find_config_keys(configs[t]))
+
+        # using the set of keys, compile settings from user (priority) then default
+        shared_keys = unique_keys['default'].union(unique_keys['user'])
+        default_keys = unique_keys['default'].difference(unique_keys['user'])
+        user_keys = unique_keys['user'].difference(unique_keys['default'])
+
+        compiled_config = {}
+        for s in shared_keys:
+            # if the entry in the user config is not empty...
+            if not configs['user'][s] == '':
+                # add this setting to the final config dict
+                compiled_config[s] = configs['user'][s]
+            # if the entry is empty in the user config, then use the default
+            else:
+                compiled_config[s] = configs['default'][s]
 
-    if len(config_file_list) > 1:
-        msg = f'\nERROR. Multiple configuration files matching the provided file handle, {file_handle}, were located '\
-              f'in this directory:\n'\
-              f'\t{[file.name for file in config_file_list]}\n'\
-              f'Please include more information in the file handle input, then retry.\n'
-        print(msg)
-        # return exit_process(message=msg)
-    else:
-        config_file = config_file_list[0]
 
-    with open(config_file, 'rt') as fin:
-        config_dict = tomlkit.parse(fin.read())
 
+    # return the compiled dictionary; return only specific section, if specified in function args
     if config_section == 'all':
-        return config_dict
+        return compiled_config
     else:
-        if config_section in config_dict.keys():
-            return config_dict[config_section]
+        if config_section in compiled_config.keys():
+            return compiled_config[config_section]
         else:
             msg = f'The provided configuration file section header, {config_section}, is not a valid header for ' \
-                  f'the {file_handle} configuration file. Please enter the number of the correct header that you ' \
+                  f'the configuration file. Please enter the number of the correct header that you ' \
                   f'want:'
             print(msg)
-            correct_header = prompt_print_options(list(config_dict.keys()))
-            return config_dict[correct_header]
-
-# write or update settings to the configuration file
-# NOT WORKING RIGHT NOW
-# def write_to_config(config_section, output_path, update_obj=False, overwrite=True, **kwargs):
-#     # import the pipeline configuration file directly
-#     config_section = 'error_message'
-#     config_dict = import_config_as_dict(output_path, file_handle)
-#
-#     # confirm that the provided section is in the configuration file
-#     if not config_section in config_dict.keys():
-#         msg = f'ERROR: Could not locate the provided section \'{config_section}\' in the pipeline configuration '\
-#               f'file.'
-#         print(msg)
-#         return exit_process(message=msg)
-#
-#     # update the configuration file with the provided key-value pairs
-#     for k, v in kwargs.items():
-#         if k in config_dict[config_section].keys():  # if there's already a key for this kwarg...
-#             if (config_dict[config_section][k] == '') or overwrite:  # if it has no value or if we want to overwrite...
-#                 config_dict[config_section][k] == v  # update/overwrite current key with new key value pair
-#             else:  # if there is something already there and we do not want to overwrite it...
-#                 continue  # continue to next key-value pair
-#         else:  # if there's no key matching in this section, add key-value pair without further inspection
-#             config_dict[config_section][k] == v
-#
-#     # write out this updated configuration dict to replace the previous configuration file
-#     config_filename = flag_multiple_files(output_path, search_for=f'*{PIPELINE_CONFIG_HANDLE}*{CONFIG_FILETYPE}')
-#
-#     with open(config_filename, 'wt') as fout:
-#         fout.write(tomlkit.dumps(config_dict))
-#
-#     return None
-
-# locate relevant mapping file for demultiplexing
-# moved down because it requires the import_config_as_dict function
-def find_mapping_file(path_to_mapping, path_to_plex, path_to_config, **kwargs):
-    '''
-    Locate the barcode mapping file(s) for demultiplexing.
-
-    Attempts to automatically detect the location of the mapping file
-    corresponding to the multiplexed files located in the sorted
-    directory of sequences to demultiplex. It inspects the name of the files
-    that were sorted into the needs_demux folder of the sequences folder, and
-    identifies the name of the sequencing run. It then will go into the mapping
-    file directory in the config folder, mapping-files, and looks for the mapping
-    file that shares that same sequencing run name. If multiple mapping files
-    are detected for a single sequencing run, the user will be prompted to select
-    the file that should be used. If no matching mapping file is detected, it
-    will throw an error and exit the pipeline.
-    :param path_to_mapping: defaults to expected location within structured
-    file directories; otherwise can specify the path as a Path object
-    :param path_to_plex: defaults to expected location within structured
-    file directories; otherwise can specify the path to the mapping file(s) as
-    a Path object
-    :param kwargs: specify the bioinfo-settings configuration file dictionary
-    if one is already loaded into the environment; if none is provided, the
-    function will open the configuration file to create a new instance of the
-    dictionary; adding a dictionary, if available, will likely be quicker so it
-    is recommended to do so if possible
-    :return: if found, returns mapping file(s) as a list
-    '''
-    assert is_pathclass(path_to_mapping)
-    assert is_pathclass(path_to_plex)
-
-    # get the multiplexed file's queue ID, which the UO sequencing core uses as the seq run identifier in the filename
-    multiplex_ids = [file.stem.split('.')[0] for file in path_to_plex.glob('*.fast*')]
-
-    # look up the multiplex IDs in the bioinfo-settings configuration file for its corresponding CliMush run name
-    kwargs_keys = list(kwargs.keys())
-    if kwargs_keys > 0:
-        if kwargs_keys > 1:
-            msg = f'ERROR: Too many keyword arguments (**kwargs) used. Only one kwarg is accepted and should have the '\
-                  f'name of the configuration dictionary as the value to a key with any name.\n'
-            print(msg)
-            return exit_process(message=msg)
-        else:
-            config_multiplex_dict = kwargs[kwargs_keys[0]]['pacbio-multiplex-ids']
-    else:
-        config_multiplex_dict = import_config_as_dict(file_handle=path_to_config)['pacbio-multiplex-ids']
-
-    # get the CliMush run name(s) and create regex to search for any of these at start of mapping file name
-    climush_ids = [config_multiplex_dict[q] for q in multiplex_ids]
-
-    # find the corresponding barcode mapping files for the run name(s) in the barcode-mapping dir in config
-    mapping_file_names = []
-    for id in climush_ids:
-        match = list(path_to_mapping.glob(f'*{id}*'))
-        if len(match) == 1:
-            mapping_file_names.append(match[0])
-        elif len(match) == 0:
-            msg = f'ERROR: No mapping files matching the CliMush run name {id} were located in {path_to_mapping}. ' \
-                  f'Check the mapping-files directory in the config folder, then retry.\n'
-            print(msg)
-            return exit_process(message=msg)
-        else:
-            msg = f'ERROR: {len(match)} mapping files were located for CliMush run name {id}. Please select the number ' \
-                  f'of the correctly corresponding barcode mapping file for this sample:\n'
-            print(msg)
-            mapping_file_names.append(prompt_print_options(match))
-
-    return mapping_file_names
+            correct_header = prompt_print_options(list(compiled_config.keys()),
+                                                  auto_respond=compiled_config['automate']['auto_respond'])
+            return compiled_config[correct_header]
 
+# sort the sequences provided in the 'sequences' input directory
 def sort_input_files(filepath_dict, to_sort='main'):
     '''
     Sort the input sequencing files in their respective sequence
     platform subdirectories, or into subdirectories for required
     pre-processing.
     :param input_file_path: Path object to the directory containing
     the input sequences.
@@ -917,33 +1265,33 @@
     def follows_naming_convention(filepath):
         if re.search(ANY_PLATFORM_REGEX, filepath.stem, re.I):
             return True
         else:
             return False
 
     def is_demultiplexed(filepath):
-        if follows_naming_convention(filepath) or re.search('^[A-Z]+', filepath.stem):
+        if follows_naming_convention(filepath) or re.search(r'^[A-Z]+', filepath.stem):
             return True
         else:
             return False
 
     def is_pacbio(filepath):
-        if re.search('^pacbio|^\d{4}', filepath.stem):
+        if re.search(r'^pacbio|^\d{4}', filepath.stem):
             return True
         else:
             return False
 
     def is_illumina(filepath):
-        if re.search('^illumina|^[A-Z]+', filepath.stem):
+        if re.search(r'^illumina|^[A-Z]+', filepath.stem):
             return True
         else:
             return False
 
     def is_sanger(filepath):
-        if re.search('^sanger', filepath.stem):
+        if re.search(r'^sanger', filepath.stem):
             return True
         else:
             return False
 
     # I guess converting a generator to a list (like in print statement below) exhausts it? so then loop won't work
     files_to_sort = list(filepath_dict['sequences'][to_sort].glob('*.fast*'))
 
@@ -975,7 +1323,77 @@
             else:
                 move_file(source_path=file, dest_path=mkdir_exist_ok(new_dir=filepath_dict['sequences']['demux']))
         else:
             move_file(source_path=file, dest_path=mkdir_exist_ok(new_dir=filepath_dict['sequences']['unclear']))
 
     return None
 
+# locate relevant mapping file for demultiplexing
+# moved down because it requires the import_config_as_dict function
+# def find_mapping_file(path_to_mapping, path_to_plex, path_to_config, **kwargs):
+#     '''
+#     Locate the barcode mapping file(s) for demultiplexing.
+#
+#     Attempts to automatically detect the location of the mapping file
+#     corresponding to the multiplexed files located in the sorted
+#     directory of sequences to demultiplex. It inspects the name of the files
+#     that were sorted into the needs_demux folder of the sequences folder, and
+#     identifies the name of the sequencing run. It then will go into the mapping
+#     file directory in the config folder, mapping-files, and looks for the mapping
+#     file that shares that same sequencing run name. If multiple mapping files
+#     are detected for a single sequencing run, the user will be prompted to select
+#     the file that should be used. If no matching mapping file is detected, it
+#     will throw an error and exit the pipeline.
+#     :param path_to_mapping: defaults to expected location within structured
+#     file directories; otherwise can specify the path as a Path object
+#     :param path_to_plex: defaults to expected location within structured
+#     file directories; otherwise can specify the path to the mapping file(s) as
+#     a Path object
+#     :param kwargs: specify the bioinfo-settings configuration file dictionary
+#     if one is already loaded into the environment; if none is provided, the
+#     function will open the configuration file to create a new instance of the
+#     dictionary; adding a dictionary, if available, will likely be quicker so it
+#     is recommended to do so if possible
+#     :return: if found, returns mapping file(s) as a list
+#     '''
+#     assert is_pathclass(path_to_mapping)
+#     assert is_pathclass(path_to_plex)
+#
+#     # get the multiplexed file's queue ID, which the UO sequencing core uses as the seq run identifier in the filename
+#     multiplex_ids = [file.stem.split('.')[0] for file in path_to_plex.glob('*.fast*')]
+#
+#     # look up the multiplex IDs in the bioinfo-settings configuration file for its corresponding CliMush run name
+#     kwargs_keys = list(kwargs.keys())
+#     if kwargs_keys > 0:
+#         if kwargs_keys > 1:
+#             msg = f'ERROR: Too many keyword arguments (**kwargs) used. Only one kwarg is accepted and should have the '\
+#                   f'name of the configuration dictionary as the value to a key with any name.\n'
+#             print(msg)
+#             return exit_process(message=msg)
+#         else:
+#             config_multiplex_dict = kwargs[kwargs_keys[0]]['pacbio-multiplex-ids']
+#     else:
+#         config_multiplex_dict = get_settings(file_handle=path_to_config)['pacbio-multiplex-ids']
+#
+#     # get the CliMush run name(s) and create regex to search for any of these at start of mapping file name
+#     climush_ids = [config_multiplex_dict[q] for q in multiplex_ids]
+#
+#     # find the corresponding barcode mapping files for the run name(s) in the barcode-mapping dir in config
+#     mapping_file_names = []
+#     for id in climush_ids:
+#         match = list(path_to_mapping.glob(f'*{id}*'))
+#         if len(match) == 1:
+#             mapping_file_names.append(match[0])
+#         elif len(match) == 0:
+#             msg = f'ERROR: No mapping files matching the CliMush run name {id} were located in {path_to_mapping}. ' \
+#                   f'Check the mapping-files directory in the config folder, then retry.\n'
+#             print(msg)
+#             return exit_process(message=msg)
+#         else:
+#             msg = f'ERROR: {len(match)} mapping files were located for CliMush run name {id}. Please select the number ' \
+#                   f'of the correctly corresponding barcode mapping file for this sample:\n'
+#             print(msg)
+#             mapping_file_names.append(prompt_print_options(match))
+#
+#     return mapping_file_names
+
+
```

### Comparing `climush-0.0.7/climush/viz.py` & `climush-0.0.8/climush/viz.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.7/climush.egg-info/PKG-INFO` & `climush-0.0.8/climush.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climush
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tools to run the CliMush bioinformatics pipeline.
 Author-email: Carolyn Delevich <cdelevic@uoregon.edu>
 Project-URL: Homepage, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline
 Project-URL: Repository, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline/climush_py-package
 Project-URL: Issues, https://github.com/cdelevich/climush/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

