# Comparing `tmp/ms1searchpy-2.8.2-py3-none-any.whl.zip` & `tmp/ms1searchpy-2.8.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 8559135 bytes, number of entries: 18
+Zip file size: 8559168 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-16 13:01 ms1searchpy/__init__.py
 -rw-r--r--  2.0 unx     4236 b- defN 24-Apr-24 10:36 ms1searchpy/combine.py
 -rw-r--r--  2.0 unx     2746 b- defN 23-Mar-16 13:01 ms1searchpy/combine_proteins.py
--rw-r--r--  2.0 unx    24852 b- defN 24-Apr-24 14:12 ms1searchpy/directms1quant.py
--rw-r--r--  2.0 unx    16412 b- defN 24-Apr-26 10:40 ms1searchpy/directms1quantmulti.py
+-rw-r--r--  2.0 unx    24852 b- defN 24-May-21 13:28 ms1searchpy/directms1quant.py
+-rw-r--r--  2.0 unx    16454 b- defN 24-May-24 10:37 ms1searchpy/directms1quantmulti.py
 -rw-r--r--  2.0 unx     7218 b- defN 24-May-14 13:38 ms1searchpy/group_specific.py
--rw-r--r--  2.0 unx    84395 b- defN 24-Mar-29 14:28 ms1searchpy/main.py
+-rw-r--r--  2.0 unx    84411 b- defN 24-May-16 15:08 ms1searchpy/main.py
 -rw-r--r--  2.0 unx     7413 b- defN 23-Mar-16 13:01 ms1searchpy/ms1todiffacto.py
 -rw-r--r--  2.0 unx     5074 b- defN 24-Mar-14 15:01 ms1searchpy/search.py
 -rw-r--r--  2.0 unx    14862 b- defN 24-Jan-26 14:14 ms1searchpy/utils.py
 -rw-r--r--  2.0 unx    15305 b- defN 24-Mar-14 15:25 ms1searchpy/utils_figures.py
 -rw-r--r--  2.0 unx  9177032 b- defN 24-Jan-15 09:44 ms1searchpy/models/CSD_model_LCMSMS.hdf5
--rwxr-xr-x  2.0 unx      551 b- defN 24-May-14 13:44 ms1searchpy-2.8.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     8712 b- defN 24-May-14 13:44 ms1searchpy-2.8.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 13:44 ms1searchpy-2.8.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      492 b- defN 24-May-14 13:44 ms1searchpy-2.8.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-May-14 13:44 ms1searchpy-2.8.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1518 b- defN 24-May-14 13:44 ms1searchpy-2.8.2.dist-info/RECORD
-18 files, 9370922 bytes uncompressed, 8556651 bytes compressed:  8.7%
+-rwxr-xr-x  2.0 unx      551 b- defN 24-May-24 10:39 ms1searchpy-2.8.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8733 b- defN 24-May-24 10:39 ms1searchpy-2.8.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 10:39 ms1searchpy-2.8.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      492 b- defN 24-May-24 10:39 ms1searchpy-2.8.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-24 10:39 ms1searchpy-2.8.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1518 b- defN 24-May-24 10:39 ms1searchpy-2.8.3.dist-info/RECORD
+18 files, 9371001 bytes uncompressed, 8556684 bytes compressed:  8.7%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: ms1searchpy/utils_figures.py
 Comment: 
 
 Filename: ms1searchpy/models/CSD_model_LCMSMS.hdf5
 Comment: 
 
-Filename: ms1searchpy-2.8.2.dist-info/LICENSE
+Filename: ms1searchpy-2.8.3.dist-info/LICENSE
 Comment: 
 
-Filename: ms1searchpy-2.8.2.dist-info/METADATA
+Filename: ms1searchpy-2.8.3.dist-info/METADATA
 Comment: 
 
-Filename: ms1searchpy-2.8.2.dist-info/WHEEL
+Filename: ms1searchpy-2.8.3.dist-info/WHEEL
 Comment: 
 
-Filename: ms1searchpy-2.8.2.dist-info/entry_points.txt
+Filename: ms1searchpy-2.8.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ms1searchpy-2.8.2.dist-info/top_level.txt
+Filename: ms1searchpy-2.8.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ms1searchpy-2.8.2.dist-info/RECORD
+Filename: ms1searchpy-2.8.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ms1searchpy/directms1quantmulti.py

```diff
@@ -50,15 +50,15 @@
 
 def process_files(args):
 
     infolder = args['pdir']
     ms1folder = args['pdir']
     path_to_fasta = args['d']
 
-    df1 = pd.read_table(args['samples'])
+    df1 = pd.read_table(args['samples'], dtype={'group': str, 'condition': str})
     df1['sample'] = df1['group']
     if 'condition' not in df1.columns:
         df1['condition'] = ''
         
     if 'replicate' not in df1.columns:
         df1['replicate'] = 1
         
@@ -115,15 +115,17 @@
         logger.info('Starting Stage 1: Run pairwise DirectMS1Quant runs...')
 
         for i2, i1_val in all_conditions.items():
             out_name = path.join(ms1folder, '%s_directms1quant_out_%s_vs_%s%s' % (outlabel, ''.join(list(i2)), control_label, i1_val))
             dquant_params = copy(dquant_params_base)
             dquant_params['S1'] = s_files_dict[(control_label, i1_val)]
             dquant_params['S2'] = s_files_dict[i2]
+
             dquant_params['out'] = out_name
+
             directms1quant.process_files(dquant_params)
 
     else:
         logger.info('Skipping Stage 1: Run pairwise DirectMS1Quant runs...')
 
 
     pep_cnt = Counter()
```

## ms1searchpy/main.py

```diff
@@ -86,15 +86,15 @@
         if k not in prots_spc2:
             prots_spc2[k] = set([])
     prots_spc = dict((k, len(v)) for k, v in prots_spc2.items())
 
     names_arr = np.array(list(prots_spc.keys()))
     v_arr = np.array(list(prots_spc.values()))
     n_arr = np.array([protsN[k] for k in prots_spc])
-    
+
     if p is False:
         top100decoy_score = [prots_spc.get(dprot, 0) for dprot in protsN if isdecoy_key(dprot)]
         top100decoy_N = [val for key, val in protsN.items() if isdecoy_key(key)]
         p = np.mean(top100decoy_score) / np.mean(top100decoy_N)
         logger.info('Probability of random match for theoretical peptide = %.3f', (np.mean(top100decoy_score) / np.mean(top100decoy_N)))
 
 
@@ -2041,21 +2041,21 @@
     prots_spc = dict()
     all_pvals = utils.calc_sf_all(v_arr, n_arr, p)
     for idx, k in enumerate(names_arr):
         prots_spc[k] = all_pvals[idx]
 
     sf = args['separate_figures']
 
-    top_proteins = final_iteration(resdict, mass_diff, rt_diff, pept_prot, protsN, base_out_name, prefix, isdecoy, isdecoy_key, escore, fdr, args['nproc'], out_log, fname)
+    top_proteins = final_iteration(resdict, mass_diff, rt_diff, pept_prot, protsN, base_out_name, prefix, isdecoy, isdecoy_key, escore, fdr, args['nproc'], out_log, fname, separate_figures=sf)
 
     # pept_prot_limited = dict()
     # for k, v in pept_prot.items():
     #     tmp = set(zz for zz in v if zz in top_proteins)
     #     if len(tmp):
-    #         pept_prot_limited[k] = tmp 
+    #         pept_prot_limited[k] = tmp
 
     # resdict3 = get_resdict(pept_prot_limited, acc_l=25, acc_r=25, aa_mass=kwargs['aa_mass'])
 
     # p1 = set(resdict3['seqs'])
 
     # if deeplc_path:
```

## Comparing `ms1searchpy-2.8.2.dist-info/LICENSE` & `ms1searchpy-2.8.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ms1searchpy-2.8.2.dist-info/METADATA` & `ms1searchpy-2.8.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms1searchpy
-Version: 2.8.2
+Version: 2.8.3
 Summary: A proteomics search engine for LC-MS1 spectra.
 Author: Mark Ivanov
 Author-email: pyteomics@googlegroups.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Education
@@ -134,15 +134,15 @@
 IDs of significantly modified proteins (e.g. for easy copy-paste into a StringDB search window).
 
 
 ### Multi-condition protein profiling using directms1quantmulti
 
 You can make a quantitation for complex projects using script directms1quantmulti. The example below is shown for our project of time-series profiling of glioblastoma cell line under interferon treatment.
 
-Script takes a table with details for all project files. An example of a sample file table is available here in the examples folder. It should contain the following columns:
+Script takes a tab-separated table (.tsv) with details for all project files. An example of a sample file table is available here in the examples folder. It should contain the following columns:
 
 File Name - filename of raw file. For example, “QEHFX_JB_000379”.
 
 group - sample group of file. In our example, there are K (Control group), IFN30 (treatment with 30 units/ml of interferon) and IFN1000 groups. The first group mentioned in the table will be used as control for pairwise directms1quant runs.  
 
 condition - sample subgroup of file. In our example, there are multiple time points after treatment, such as 0h, 30min, 1h, 2h, etc. By default, only the same conditions will be used for pairwise comparisons. For example, IFN30 0h vs K 0h; IFN1000 0h vs K 0h, etc.
```

## Comparing `ms1searchpy-2.8.2.dist-info/RECORD` & `ms1searchpy-2.8.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ms1searchpy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ms1searchpy/combine.py,sha256=7S61Ftnv4NJUmfnV6vjVp2uHwslkDcQQJVPzWYVm1nk,4236
 ms1searchpy/combine_proteins.py,sha256=LFJuwkb8UBy-1T-kAT3H4zxkqQ6VTso6SOLP7s8o0Ow,2746
 ms1searchpy/directms1quant.py,sha256=OuInuVdPCIsRbvRSCM1mnNqh0jQwvQhhcd6Bo0AbnnM,24852
-ms1searchpy/directms1quantmulti.py,sha256=bWlUOQX7S1nWsV-Zl10s9L_IRllX6tpJJvQGXgINo40,16412
+ms1searchpy/directms1quantmulti.py,sha256=x6iFcoUt2bI-8x1Z6vLpBpxz6lUBli01bcSoB3jfkhw,16454
 ms1searchpy/group_specific.py,sha256=AqEN5xkrsEdXeVFdqHUkQa0tmip14zQQrK4pu0tFZi4,7218
-ms1searchpy/main.py,sha256=eISGaa6d5-HBZoNkbK_YjnhMGZOQopRqWPgh4sJIoDo,84395
+ms1searchpy/main.py,sha256=Gj3VqOO46Pu2CGVZiOu2fdj8KyppxEVD5bJBbUwY2Os,84411
 ms1searchpy/ms1todiffacto.py,sha256=xGxcIe8-C_vSLx5Qz5qwSKa4oULJ-8cgq4DtCTXKe3s,7413
 ms1searchpy/search.py,sha256=LzcFU_j7pilzoHo-4b_D0gkMXGwruWt4G5vluWPa-Qk,5074
 ms1searchpy/utils.py,sha256=D59l42xbMYMyL6GEuKOCOPsdexaMmo-1j3cKSNPN9lE,14862
 ms1searchpy/utils_figures.py,sha256=KfBAVLoq7U57HV-hct8CpiOL4BCHADAWIBFbH-jWB_M,15305
 ms1searchpy/models/CSD_model_LCMSMS.hdf5,sha256=7nAu3-YWKjsuQNCpgoRpTjInA-dPe7kZE1pTGKg-3OQ,9177032
-ms1searchpy-2.8.2.dist-info/LICENSE,sha256=WanbJHdVmtsm-QgIuB0GDMrtkwBHY6WmTzwvX6ZZtgs,551
-ms1searchpy-2.8.2.dist-info/METADATA,sha256=_1nBd7q4ZeyO56ocZAWJNWtapiH1VG41pVCvKCyo9DI,8712
-ms1searchpy-2.8.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ms1searchpy-2.8.2.dist-info/entry_points.txt,sha256=ACLj6QbnpM9wI-CQA2YFf_ZmWEFqN9GZpbuxO6ZEeHE,492
-ms1searchpy-2.8.2.dist-info/top_level.txt,sha256=pyjbWV_odwavqf6q4mSj2P0L0zLqKEDftX53QvxeJlc,12
-ms1searchpy-2.8.2.dist-info/RECORD,,
+ms1searchpy-2.8.3.dist-info/LICENSE,sha256=WanbJHdVmtsm-QgIuB0GDMrtkwBHY6WmTzwvX6ZZtgs,551
+ms1searchpy-2.8.3.dist-info/METADATA,sha256=5XTJiMar_D4nb1TuvLMiZ5FBXx58-7eHM8K91GRqsoE,8733
+ms1searchpy-2.8.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ms1searchpy-2.8.3.dist-info/entry_points.txt,sha256=ACLj6QbnpM9wI-CQA2YFf_ZmWEFqN9GZpbuxO6ZEeHE,492
+ms1searchpy-2.8.3.dist-info/top_level.txt,sha256=pyjbWV_odwavqf6q4mSj2P0L0zLqKEDftX53QvxeJlc,12
+ms1searchpy-2.8.3.dist-info/RECORD,,
```

