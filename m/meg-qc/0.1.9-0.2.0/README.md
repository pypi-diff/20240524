# Comparing `tmp/meg_qc-0.1.9.tar.gz` & `tmp/meg_qc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meg_qc-0.1.9.tar", last modified: Wed May 15 13:29:05 2024, max compression
+gzip compressed data, was "meg_qc-0.2.0.tar", last modified: Fri May 24 12:44:43 2024, max compression
```

## Comparing `meg_qc-0.1.9.tar` & `meg_qc-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:29:05.391676 meg_qc-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-15 13:28:51.000000 meg_qc-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-15 13:29:05.391676 meg_qc-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-15 13:28:51.000000 meg_qc-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:29:05.395676 meg_qc-0.1.9/meg_qc/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-15 13:29:05.395676 meg_qc-0.1.9/meg_qc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:29:05.391676 meg_qc-0.1.9/meg_qc/calculation/
--rw-r--r--   0 runner    (1001) docker     (127)    26343 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/initial_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    20755 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/meg_qc_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:29:05.391676 meg_qc-0.1.9/meg_qc/calculation/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)   112596 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/ECG_EOG_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/Head_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    53766 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/PSD_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/Peaks_auto_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18689 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/Peaks_manual_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    25659 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/STD_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/calculation/metrics/muscle_meg_qc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:29:05.391676 meg_qc-0.1.9/meg_qc/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/plotting/meg_qc_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/plotting/universal_html_report.py
--rw-r--r--   0 runner    (1001) docker     (127)   130403 2024-05-15 13:28:51.000000 meg_qc-0.1.9/meg_qc/plotting/universal_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:29:05.391676 meg_qc-0.1.9/meg_qc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-15 13:29:05.000000 meg_qc-0.1.9/meg_qc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 13:29:05.000000 meg_qc-0.1.9/meg_qc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:29:05.000000 meg_qc-0.1.9/meg_qc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 13:29:05.000000 meg_qc-0.1.9/meg_qc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 13:28:51.000000 meg_qc-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-15 13:29:05.395676 meg_qc-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-15 13:28:51.000000 meg_qc-0.1.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-05-15 13:28:51.000000 meg_qc-0.1.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:44:43.136609 meg_qc-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-24 12:44:23.000000 meg_qc-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-24 12:44:43.140609 meg_qc-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-24 12:44:23.000000 meg_qc-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:44:43.140609 meg_qc-0.2.0/meg_qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-24 12:44:43.140609 meg_qc-0.2.0/meg_qc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:44:43.136609 meg_qc-0.2.0/meg_qc/calculation/
+-rw-r--r--   0 runner    (1001) docker     (127)    26085 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/calculation/initial_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20015 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/calculation/meg_qc_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:44:43.136609 meg_qc-0.2.0/meg_qc/calculation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    96659 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/calculation/metrics/ECG_EOG_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/calculation/metrics/Head_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50613 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/calculation/metrics/PSD_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/calculation/metrics/Peaks_auto_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17903 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/calculation/metrics/Peaks_manual_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25570 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/calculation/metrics/STD_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18183 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/calculation/metrics/muscle_meg_qc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:44:43.136609 meg_qc-0.2.0/meg_qc/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)    23411 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/plotting/meg_qc_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/plotting/universal_html_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137391 2024-05-24 12:44:23.000000 meg_qc-0.2.0/meg_qc/plotting/universal_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:44:43.136609 meg_qc-0.2.0/meg_qc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-24 12:44:43.000000 meg_qc-0.2.0/meg_qc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-24 12:44:43.000000 meg_qc-0.2.0/meg_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:44:43.000000 meg_qc-0.2.0/meg_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 12:44:43.000000 meg_qc-0.2.0/meg_qc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-24 12:44:23.000000 meg_qc-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-24 12:44:43.140609 meg_qc-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-24 12:44:23.000000 meg_qc-0.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-05-24 12:44:23.000000 meg_qc-0.2.0/versioneer.py
```

### Comparing `meg_qc-0.1.9/LICENSE` & `meg_qc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.9/PKG-INFO` & `meg_qc-0.2.0/meg_qc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: meg_qc
-Version: 0.1.9
+Name: meg-qc
+Version: 0.2.0
 Summary: Tool for automated MEG data quality control
 Home-page: https://github.com/AaronReer/MEGqc
 Author: ANCP
 Author-email: aaron.reer@uol.de
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
```

### Comparing `meg_qc-0.1.9/README.md` & `meg_qc-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.9/meg_qc/__main__.py` & `meg_qc-0.2.0/meg_qc/__main__.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.9/meg_qc/calculation/initial_meg_qc.py` & `meg_qc-0.2.0/meg_qc/calculation/initial_meg_qc.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,14 @@
             'run_EOG': run_EOG,
             'run_Head': run_Head,
             'run_Muscle': run_Muscle,
             'dataset_path': ds_paths,
             'plot_mne_butterfly': default_section.getboolean('plot_mne_butterfly'),
             'plot_interactive_time_series': default_section.getboolean('plot_interactive_time_series'),
             'plot_interactive_time_series_average': default_section.getboolean('plot_interactive_time_series_average'),
-            'verbose_plots': default_section.getboolean('verbose_plots'),
             'crop_tmin': tmin,
             'crop_tmax': tmax})
         all_qc_params['default'] = default_params
 
         filtering_section = config['Filtering']
         try:
             lfreq = filtering_section.getfloat('l_freq')
@@ -507,25 +506,22 @@
             time_series_derivs += plot_time_series_avg(raw_cropped, m_or_g)
 
     if time_series_derivs:
         time_series_str="For this visialisation the data is resampled to 100Hz but not filtered. If cropping was chosen in settings the cropped raw is presented here, otherwise - entire duratio."
     else:
         time_series_str = 'No time series plot was generated. To generate it, set plot_interactive_time_series or(and) plot_interactive_time_series_average to True in settings.'
 
-
-    verbose_plots = default_settings['verbose_plots'] #will only be used for metrics plots. dont output time series and 3d of sensors in any case in the notebook.
-    
     clicking_str = "<p></p><p>On each interactive plot: <br> - click twice on the legend to hide/show a group of channels;<br> - click one to hide/show individual channels;<br> - hover over the dot/line to see information about channel an metric value.</li></ul></p>"
 
     resample_str = '<p>' + resample_str + '</p>'
 
     #Extract chs_by_lobe into a data frame
     sensors_derivs = chs_dict_to_csv(chs_by_lobe,  file_name_prefix = 'Sensors')
 
-    return dict_epochs_mg, chs_by_lobe, channels, raw_cropped_filtered, raw_cropped_filtered_resampled, raw_cropped, raw, shielding_str, epoching_str, sensors_derivs, time_series_derivs, time_series_str, m_or_g_chosen, m_or_g_skipped_str, lobes_color_coding_str, clicking_str, resample_str, verbose_plots
+    return dict_epochs_mg, chs_by_lobe, channels, raw_cropped_filtered, raw_cropped_filtered_resampled, raw_cropped, raw, shielding_str, epoching_str, sensors_derivs, time_series_derivs, time_series_str, m_or_g_chosen, m_or_g_skipped_str, lobes_color_coding_str, clicking_str, resample_str
 
 
 def chs_dict_to_csv(chs_by_lobe: dict, file_name_prefix: str):
 
     #Extract chs_by_lobe into a data frame
     chs_by_lobe_df = {k1: {k2: pd.concat([channel.to_df() for channel in v2]) for k2, v2 in v1.items()} for k1, v1 in chs_by_lobe.items()}
```

### Comparing `meg_qc-0.1.9/meg_qc/calculation/meg_qc_pipeline.py` & `meg_qc-0.2.0/meg_qc/calculation/meg_qc_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,14 +124,15 @@
         avg_eog=[]
 
         print('___MEGqc___: ', 'TOTAL subs', len(list_of_subs))
         print('___MEGqc___: ', 'EMPTY room?', sorted(list_of_subs)[0], sorted(list_of_subs)[-1])
         #list_of_subs = ['009', '012', '019', '020', '021', '022', '023', '024', '025'] #especially 23 in ds 83! There doesnt detect all the ecg peaks and says bad ch, but it s good.
         
         raw=None #preassign in case no calculation will be successful
+
         for sid in list_of_subs: #[0:4]: 
             print('___MEGqc___: ', 'Dataset: ', dataset_path)
             print('___MEGqc___: ', 'Take SID: ', sid)
             
             subject_folder = derivative.create_folder(type_=schema.Subject, name='sub-'+sid)
 
             list_of_fifs = sorted(list(dataset.query(suffix='meg', extension='.fif', return_type='filename', subj=sid)))
@@ -145,18 +146,19 @@
 
             # entities = dataset.query_entities()
             # print('___MEGqc___: ', 'entities', entities)
 
 
             list_of_sub_jsons = dataset.query(sub=sid, suffix='meg', extension='.fif')
 
-            print('list_of_sub_jsons')
-            print(list_of_sub_jsons)
+            print('___MEGqc___: ', 'list_of_sub_jsons', list_of_sub_jsons)
+
+            #list_of_fifs = list_of_fifs[0:1] #DELETE THIS LINE WHEN DONE TESTING
 
-            list_of_fifs = list_of_fifs[0:1] #DELETE THIS LINE WHEN DONE TESTING
+            counter = 0
 
             for fif_ind, data_file in enumerate(list_of_fifs): 
                 print('___MEGqc___: ', 'Take fif: ', data_file)
 
                 if 'acq-crosstalk' in data_file:
                     print('___MEGqc___: ', 'Skipping crosstalk file ', data_file)
                     #read about crosstalk files here: https://bids-specification.readthedocs.io/en/stable/appendices/meg-file-formats.html
@@ -165,15 +167,15 @@
                 # Preassign strings with notes for the user to add to html report (in case some QC analysis was skipped):
                 shielding_str, m_or_g_skipped_str, epoching_str, ecg_str, eog_str, head_str, muscle_str, pp_manual_str, pp_auto_str, std_str, psd_str = '', '', '', '', '', '', '', '', '', '', ''
     
                 print('___MEGqc___: ', 'Starting initial processing...')
                 start_time = time.time()
 
                 try:
-                    dict_epochs_mg, chs_by_lobe, channels, raw_cropped_filtered, raw_cropped_filtered_resampled, raw_cropped, raw, shielding_str, epoching_str, sensors_derivs, time_series_derivs, time_series_str, m_or_g_chosen, m_or_g_skipped_str, lobes_color_coding_str, clicking_str, resample_str, verbose_plots = initial_processing(default_settings=all_qc_params['default'], filtering_settings=all_qc_params['Filtering'], epoching_params=all_qc_params['Epoching'], data_file=data_file)
+                    dict_epochs_mg, chs_by_lobe, channels, raw_cropped_filtered, raw_cropped_filtered_resampled, raw_cropped, raw, shielding_str, epoching_str, sensors_derivs, time_series_derivs, time_series_str, m_or_g_chosen, m_or_g_skipped_str, lobes_color_coding_str, clicking_str, resample_str = initial_processing(default_settings=all_qc_params['default'], filtering_settings=all_qc_params['Filtering'], epoching_params=all_qc_params['Epoching'], data_file=data_file)
                 except:
                     print('___MEGqc___: ', 'Could not process file ', data_file, '. Skipping it.')
                     #in case some file can not be processed, the pipeline will continue. To figure out the issue, run the file separately: raw=mne.io.read_raw_fif('.../filepath/...fif')
                     continue
                 
                 print('___MEGqc___: ', "Finished initial processing. --- Execution %s seconds ---" % (time.time() - start_time))
 
@@ -186,62 +188,59 @@
                 df_head_pos, head_pos = [], []
                 scores_muscle_all1, scores_muscle_all2, scores_muscle_all3 = [], [], []
                 raw1, raw2, raw3 = [], [], []
 
                 if all_qc_params['default']['run_STD'] is True:
                     print('___MEGqc___: ', 'Starting STD...')
                     start_time = time.time()
-                    std_derivs, simple_metrics_std, std_str = STD_meg_qc(all_qc_params['STD'], channels, chs_by_lobe, dict_epochs_mg, raw_cropped_filtered_resampled, m_or_g_chosen, verbose_plots)
+                    std_derivs, simple_metrics_std, std_str = STD_meg_qc(all_qc_params['STD'], channels, chs_by_lobe, dict_epochs_mg, raw_cropped_filtered_resampled, m_or_g_chosen)
                     print('___MEGqc___: ', "Finished STD. --- Execution %s seconds ---" % (time.time() - start_time))
     
                 if all_qc_params['default']['run_PSD'] is True:
                     print('___MEGqc___: ', 'Starting PSD...')
                     start_time = time.time()
-                    psd_derivs, simple_metrics_psd, psd_str, noisy_freqs_global = PSD_meg_qc(all_qc_params['PSD'], channels, chs_by_lobe , raw_cropped_filtered, m_or_g_chosen, verbose_plots, helperplots=False)
+                    psd_derivs, simple_metrics_psd, psd_str, noisy_freqs_global = PSD_meg_qc(all_qc_params['PSD'], channels, chs_by_lobe , raw_cropped_filtered, m_or_g_chosen, helper_plots=False)
                     print('___MEGqc___: ', "Finished PSD. --- Execution %s seconds ---" % (time.time() - start_time))
 
                 if all_qc_params['default']['run_PTP_manual'] is True:
                     print('___MEGqc___: ', 'Starting Peak-to-Peak manual...')
                     start_time = time.time()
-                    pp_manual_derivs, simple_metrics_pp_manual, pp_manual_str = PP_manual_meg_qc(all_qc_params['PTP_manual'], channels, chs_by_lobe, dict_epochs_mg, raw_cropped_filtered_resampled, m_or_g_chosen, verbose_plots)
+                    pp_manual_derivs, simple_metrics_pp_manual, pp_manual_str = PP_manual_meg_qc(all_qc_params['PTP_manual'], channels, chs_by_lobe, dict_epochs_mg, raw_cropped_filtered_resampled, m_or_g_chosen)
                     print('___MEGqc___: ', "Finished Peak-to-Peak manual. --- Execution %s seconds ---" % (time.time() - start_time))
 
                 if all_qc_params['default']['run_PTP_auto_mne'] is True:
                     print('___MEGqc___: ', 'Starting Peak-to-Peak auto...')
                     start_time = time.time()
                     pp_auto_derivs, bad_channels, pp_auto_str = PP_auto_meg_qc(all_qc_params['PTP_auto'], channels, raw_cropped_filtered_resampled, m_or_g_chosen)
                     print('___MEGqc___: ', "Finished Peak-to-Peak auto. --- Execution %s seconds ---" % (time.time() - start_time))
 
                 if all_qc_params['default']['run_ECG'] is True:
                     print('___MEGqc___: ', 'Starting ECG...')
                     start_time = time.time()
-                    ecg_derivs, simple_metrics_ecg, ecg_str, avg_objects_ecg = ECG_meg_qc(all_qc_params['ECG'], internal_qc_params['ECG'], raw_cropped, channels, chs_by_lobe, m_or_g_chosen, verbose_plots)
+                    ecg_derivs, simple_metrics_ecg, ecg_str, avg_objects_ecg = ECG_meg_qc(all_qc_params['ECG'], internal_qc_params['ECG'], raw_cropped, channels, chs_by_lobe, m_or_g_chosen)
                     print('___MEGqc___: ', "Finished ECG. --- Execution %s seconds ---" % (time.time() - start_time))
 
                     avg_ecg += avg_objects_ecg
 
                 if all_qc_params['default']['run_EOG'] is True:
                     print('___MEGqc___: ', 'Starting EOG...')
                     start_time = time.time()
-                    eog_derivs, simple_metrics_eog, eog_str, avg_objects_eog = EOG_meg_qc(all_qc_params['EOG'], internal_qc_params['EOG'], raw_cropped, channels, chs_by_lobe, m_or_g_chosen, verbose_plots)
+                    eog_derivs, simple_metrics_eog, eog_str, avg_objects_eog = EOG_meg_qc(all_qc_params['EOG'], internal_qc_params['EOG'], raw_cropped, channels, chs_by_lobe, m_or_g_chosen)
                     print('___MEGqc___: ', "Finished EOG. --- Execution %s seconds ---" % (time.time() - start_time))
 
                     avg_eog += avg_objects_eog
 
                 if all_qc_params['default']['run_Head'] is True:
                     print('___MEGqc___: ', 'Starting Head movement calculation...')
-                    head_derivs, simple_metrics_head, head_str, df_head_pos, head_pos = HEAD_movement_meg_qc(raw_cropped, verbose_plots, plot_annotations=False)
+                    head_derivs, simple_metrics_head, head_str, df_head_pos, head_pos = HEAD_movement_meg_qc(raw_cropped, plot_annotations=False)
                     print('___MEGqc___: ', "Finished Head movement calculation. --- Execution %s seconds ---" % (time.time() - start_time))
 
                 if all_qc_params['default']['run_Muscle'] is True:
                     print('___MEGqc___: ', 'Starting Muscle artifacts calculation...')
-                    #use the same form of raw as in the PSD func! Because psd func calculates first if there are powerline noise freqs.
-                    # muscle_derivs, simple_metrics_muscle, muscle_str, scores_muscle_all1, raw1 = MUSCLE_meg_qc(all_qc_params['Muscle'], raw_cropped_filtered, noisy_freqs_global, m_or_g_chosen, verbose_plots, interactive_matplot=False, attach_dummy = False, cut_dummy = False)
-                    # muscle_derivs, simple_metrics_muscle, muscle_str, scores_muscle_all2, raw2 = MUSCLE_meg_qc(all_qc_params['Muscle'], raw_cropped_filtered, noisy_freqs_global, m_or_g_chosen, verbose_plots, interactive_matplot=False, attach_dummy = True, cut_dummy = False)
-                    muscle_derivs, simple_metrics_muscle, muscle_str, scores_muscle_all3, raw3 = MUSCLE_meg_qc(all_qc_params['Muscle'], all_qc_params['PSD'], raw_cropped_filtered, noisy_freqs_global, m_or_g_chosen, verbose_plots, interactive_matplot=False, attach_dummy = True, cut_dummy = True)
+                    muscle_derivs, simple_metrics_muscle, muscle_str, scores_muscle_all3, raw3 = MUSCLE_meg_qc(all_qc_params['Muscle'], all_qc_params['PSD'], raw_cropped_filtered, noisy_freqs_global, m_or_g_chosen, attach_dummy = True, cut_dummy = True)
                     print('___MEGqc___: ', "Finished Muscle artifacts calculation. --- Execution %s seconds ---" % (time.time() - start_time))
 
                 
                 report_strings = {
                 'INITIAL_INFO': m_or_g_skipped_str+resample_str+epoching_str+shielding_str+lobes_color_coding_str+clicking_str,
                 'TIME_SERIES': time_series_str,
                 'STD': std_str,
@@ -267,17 +266,14 @@
                 'Peak-to-Peak manual': pp_manual_derivs, 
                 'Peak-to-Peak auto from MNE': pp_auto_derivs, 
                 'ECG': ecg_derivs, 
                 'EOG': eog_derivs,
                 'Head movement artifacts': head_derivs,
                 'High frequency (Muscle) artifacts': muscle_derivs}
 
-                print('___MEGqc___: ', 'QC_derivs', QC_derivs)  
-
-
                 QC_simple={
                 'STD': simple_metrics_std, 
                 'PSD': simple_metrics_psd,
                 'PTP_MANUAL': simple_metrics_pp_manual, 
                 'PTP_AUTO': simple_metrics_pp_auto,
                 'ECG': simple_metrics_ecg, 
                 'EOG': simple_metrics_eog,
@@ -297,15 +293,14 @@
 
                 report_html_string = make_joined_report_mne(raw, QC_derivs, report_strings, default_settings=all_qc_params['default'])
                 QC_derivs['Report_MNE']= [QC_derivative(report_html_string, 'REPORT', 'report mne')]
 
                 #Collect all simple metrics into a dictionary and add to QC_derivs:
                 QC_derivs['Simple_metrics']=[QC_derivative(QC_simple, 'SimpleMetrics', 'json')]
 
-
                 #if there are any derivs calculated in this section:
                 for section in (section for section in QC_derivs.values() if section):
                     # loop over section where deriv.content_type is not 'matplotlib' or 'plotly' or 'report'
                     for deriv in (deriv for deriv in section if deriv.content_type != 'matplotlib' and deriv.content_type != 'plotly' and deriv.content_type != 'report'):
                         
                         # print('___MEGqc___: ', 'writing deriv: ', d)
                         # print('___MEGqc___: ', deriv)
@@ -323,14 +318,18 @@
                         #     def html_writer(file_path, cont=deriv.content):
                         #         with open(file_path, "w") as file:
                         #             file.write(cont)
                         #         #'with'command doesnt work in lambda
                         #     meg_artifact.content = html_writer # function pointer instead of lambda
 
                         meg_artifact = subject_folder.create_artifact(raw=list_of_sub_jsons[fif_ind]) #shell. empty derivative
+
+                        counter +=1
+                        print('___MEGqc___: ', 'counter of subject_folder.create_artifact', counter)
+
                         meg_artifact.add_entity('desc', deriv.name) #file name
                         meg_artifact.suffix = 'meg'
                         meg_artifact.extension = '.html'
 
                         if deriv.content_type == 'df':
                             meg_artifact.extension = '.tsv'
                             meg_artifact.content = lambda file_path, cont=deriv.content: cont.to_csv(file_path, sep='\t')
```

### Comparing `meg_qc-0.1.9/meg_qc/calculation/metrics/ECG_EOG_meg_qc.py` & `meg_qc-0.2.0/meg_qc/calculation/metrics/ECG_EOG_meg_qc.py`

 * *Files 14% similar despite different names*

```diff
@@ -303,15 +303,15 @@
 
     def __repr__(self):
         """
         Returns a string representation of the object
         
         """
 
-        return 'Mean artifact for: ' + str(self.name) + '\n - peak location inside artifact epoch: ' + str(self.peak_loc) + '\n - peak magnitude: ' + str(self.peak_magnitude) +'\n - main_peak_loc: '+ str(self.main_peak_loc) +'\n - main_peak_magnitude: '+str(self.main_peak_magnitude)+'\n - wave_shape: '+ str(self.wave_shape) + '\n - artifact magnitude over threshold: ' + str(self.artif_over_threshold)+ '\n'
+        return 'Mean artifact for: ' + str(self.name) + '\n - peak location inside artifact epoch: ' + str(self.peak_loc) + '\n - peak magnitude: ' + str(self.peak_magnitude) +'\n - main_peak_loc: '+ str(self.main_peak_loc) +'\n - main_peak_magnitude: '+str(self.main_peak_magnitude)+'\n - wave_shape: '+ str(self.wave_shape) + '\n - artifact magnitude over threshold: ' + str(self.artif_over_threshold)+ '\n - corr_coef: ' + str(self.corr_coef) + '\n - p_value: ' + str(self.p_value) + '\n - lobe: ' + str(self.lobe) + '\n - color: ' + str(self.color) + '\n - peak_loc_smoothed: ' + str(self.peak_loc_smoothed) + '\n - peak_magnitude_smoothed: ' + str(self.peak_magnitude_smoothed) + '\n - wave_shape_smoothed: ' + str(self.wave_shape_smoothed) + '\n - artif_over_threshold_smoothed: ' + str(self.artif_over_threshold_smoothed) + '\n - main_peak_loc_smoothed: ' + str(self.main_peak_loc_smoothed) + '\n - main_peak_magnitude_smoothed: ' + str(self.main_peak_magnitude_smoothed) + '\n'
     
 
 
     def get_peaks_wave(self, max_n_peaks_allowed: int, thresh_lvl_peakfinder: float):
 
         """
         Find peaks in the average artifact epoch and decide if the epoch has wave shape: 
@@ -761,109 +761,14 @@
             affected_smoothed.append(potentially_affected)
         else:
             not_affected_smoothed.append(potentially_affected)
 
     return affected_orig, not_affected_orig, artif_threshold_lvl, affected_smoothed, not_affected_smoothed, artifact_lvl_smoothed
 
 
-def plot_affected_channels(artif_affected_channels: list, artifact_lvl: float, t: np.ndarray, ch_type: str, fig_tit: str, chs_by_lobe: dict, flip_data: bool or str = 'flip', smoothed: bool = False, verbose_plots: bool = True):
-
-    """
-    Plot the mean artifact amplitude for all affected (not affected) channels in 1 plot together with the artifact_lvl.
-    
-    Parameters
-    ----------
-    artif_affected_channels : list
-        List of ECG/EOG artifact affected channels.
-    artifact_lvl : float
-        The threshold for the artifact amplitude: average over all channels*norm_lvl.
-    t : np.ndarray
-        Time vector.
-    ch_type : str
-        Either 'mag' or 'grad'.
-    fig_tit: str
-        The title of the figure.
-    chs_by_lobe : dict
-        dictionary with channel objects sorted by lobe
-    flip_data : bool
-        If True, the absolute value of the data will be used for the calculation of the mean artifact amplitude. Default to 'flip'. 
-        'flip' means that the data will be flipped if the peak of the artifact is negative. 
-        This is donr to get the same sign of the artifact for all channels, then to get the mean artifact amplitude over all channels and the threshold for the artifact amplitude onbase of this mean
-        And also for the reasons of visualization: the artifact amplitude is always positive.
-    smoothed: bool
-        Plot smoothed data (true) or nonrmal (false)
-    verbose_plots : bool
-        True for showing plot in notebook.
-
-    Returns
-    -------
-    fig : plotly.graph_objects.Figure
-        The plotly figure with the mean artifact amplitude for all affected (not affected) channels in 1 plot together with the artifact_lvl.
-
-        
-    """
-
-    if artif_affected_channels: #if affected channels present:
-
-        #plot channels separated by lobes:
-        affected_names_list = []
-        affected_data_list = []
-        for ch in artif_affected_channels:
-            affected_names_list.append(ch.name)
-            if smoothed is True:
-                affected_data_list.append(ch.artif_data_smoothed)
-            else:
-                affected_data_list.append(ch.artif_data)
-
-        affected_data_arr = np.array(affected_data_list)
-
-        df_affected=pd.DataFrame(affected_data_arr.T, columns=affected_names_list)
-
-        fig = plot_df_of_channels_data_as_lines_by_lobe(chs_by_lobe, df_affected, t)
-
-        #decorate the plot:
-        ch_type_tit, unit = get_tit_and_unit(ch_type)
-        fig.update_layout(
-            xaxis_title='Time in seconds',
-            yaxis = dict(
-                showexponent = 'all',
-                exponentformat = 'e'),
-            yaxis_title='Mean artifact magnitude in '+unit,
-            title={
-                'text': fig_tit+str(len(artif_affected_channels))+' '+ch_type_tit,
-                'y':0.85,
-                'x':0.5,
-                'xanchor': 'center',
-                'yanchor': 'top'})
-
-
-    else:
-        fig=go.Figure()
-        ch_type_tit, _ = get_tit_and_unit(ch_type)
-        title=fig_tit+'0 ' +ch_type_tit
-        fig.update_layout(
-            title={
-            'text': title,
-            'x': 0.5,
-            'y': 0.9,
-            'xanchor': 'center',
-            'yanchor': 'top'})
-        
-    #in any case - add the threshold on the plot
-    fig.add_trace(go.Scatter(x=t, y=[(artifact_lvl)]*len(t), line=dict(color='red'), name='Thres=mean_peak/norm_lvl')) #add threshold level
-
-    if flip_data is False and artifact_lvl is not None: 
-        fig.add_trace(go.Scatter(x=t, y=[(-artifact_lvl)]*len(t), line=dict(color='black'), name='-Thres=mean_peak/norm_lvl'))
-
-    if verbose_plots is True:
-        fig.show()
-
-    return fig
-
-
 def flip_channels(artif_per_ch_nonflipped: list, tmin: float, tmax: float, sfreq: int, params_internal: dict):
 
     """
     Flip the channels if the peak of the artifact is negative and located close to the estimated t0.
 
     Flip approach: 
 
@@ -1228,86 +1133,14 @@
 
     for ch in artif_per_ch:
         ch.corr_coef, ch.p_value = pearsonr(ch.artif_data_smoothed, mean_rwave)
     
     return artif_per_ch
 
 
-def plot_correlation(artif_per_ch, ecg_or_eog, m_or_g, verbose_plots=False):
-
-    """
-    Plot correlation coefficient and p-value between mean R wave and each channel in artif_per_ch.
-
-    Parameters
-    ----------
-    artif_per_ch : list
-        List of channels with Avg_artif objects.
-    ecg_or_eog : str
-        Either 'ECG' or 'EOG'.
-    m_or_g : str
-        Either 'mag' or 'grad'.
-    verbose_plots : bool
-        If True, plot will be displayed in a notebook.
-
-    Returns
-    -------
-    corr_derivs : list
-        List with 1 QC_derivative instance: Figure with correlation coefficient and p-value between mean R wave and each channel in artif_per_ch.
-    
-    """
-
-    _, _, _, corr_val_of_last_most_correlated, corr_val_of_last_middle_correlated, corr_val_of_last_least_correlated = split_correlated_artifacts_into_3_groups(artif_per_ch)
-
-    print('least', corr_val_of_last_least_correlated)
-    print('middle', corr_val_of_last_middle_correlated)
-    print('most', corr_val_of_last_most_correlated)
-
-    traces = []
-
-    tit, _ = get_tit_and_unit(m_or_g)
-
-    for ch in artif_per_ch:
-        traces += [go.Scatter(x=[abs(ch.corr_coef)], y=[ch.p_value], mode='markers', marker=dict(size=5, color=ch.color), name=ch.name, legendgroup=ch.lobe, legendgrouptitle=dict(text=ch.lobe.upper()), hovertemplate='Corr coef: '+str(ch.corr_coef)+'<br>p-value: '+str(abs(ch.p_value)))]
-
-    fig = go.Figure(data=traces)
-
-    #add rectangles to the plot to separate most correlated (red), middle (yellow) and least correlated (green) channels:
-    #separate rage -1 to 1 into 6 equal parts:
-    # ranges=np.linspace(-1, 1, 7)
-    # x_most=[ranges[0], ranges[1]]
-    # x_most2=[ranges[-1], ranges[-2]]
-    # x_middle=[ranges[1], ranges[2]]
-    # x_middle2=[ranges[-2], ranges[-3]]
-    # x_least=[ranges[2], ranges[4]]
-
-    # fig.add_shape(type="rect", xref="x", yref="y", x0=x_most[0], y0=-0.1, x1=x_most[1], y1=1.1, line=dict(color="Red", width=2), fillcolor="Red", opacity=0.1)
-    # fig.add_shape(type="rect", xref="x", yref="y", x0=x_most2[0], y0=-0.1, x1=x_most2[1], y1=1.1, line=dict(color="Red", width=2), fillcolor="Red", opacity=0.1)
-    # fig.add_shape(type="rect", xref="x", yref="y", x0=x_middle[0], y0=-0.1, x1=x_middle[1], y1=1.1, line=dict(color="Yellow", width=2), fillcolor="Yellow", opacity=0.1)
-    # fig.add_shape(type="rect", xref="x", yref="y", x0=x_middle2[0], y0=-0.1, x1=x_middle2[1], y1=1.1, line=dict(color="Yellow", width=2), fillcolor="Yellow", opacity=0.1)
-    # fig.add_shape(type="rect", xref="x", yref="y", x0=x_least[0], y0=-0.1, x1=x_least[1], y1=1.1, line=dict(color="Green", width=2), fillcolor="Green", opacity=0.1)
-
-    fig.add_shape(type="rect", xref="x", yref="y", x0=0, y0=-0.1, x1=corr_val_of_last_least_correlated, y1=1.1, line=dict(color="Green", width=2), fillcolor="Green", opacity=0.1)
-    fig.add_shape(type="rect", xref="x", yref="y", x0=corr_val_of_last_least_correlated, y0=-0.1, x1=corr_val_of_last_middle_correlated, y1=1.1, line=dict(color="Yellow", width=2), fillcolor="Yellow", opacity=0.1)
-    fig.add_shape(type="rect", xref="x", yref="y", x0=corr_val_of_last_middle_correlated, y0=-0.1, x1=1, y1=1.1, line=dict(color="Red", width=2), fillcolor="Red", opacity=0.1)
-
-    #set axis titles:
-    fig.update_xaxes(title_text='Correlation coefficient')
-    fig.update_yaxes(title_text='P-value')
-
-    #set title:
-    fig.update_layout(title_text=tit+': Pearson correlation between reference '+ecg_or_eog+' epoch and '+ecg_or_eog+' epoch in each channel')
-
-    if verbose_plots is True:
-        fig.show()
-
-    corr_derivs = [QC_derivative(fig, 'Corr_values_'+ecg_or_eog, 'plotly', description_for_user='Absolute value of the correlation coefficient is shown here. The sign would only represent the position of the channel towards magnetic field. <p>- Green: 33% of all channels that have the weakest correlation with mean ' +ecg_or_eog +'; </p> <p>- Yellow: 33% of all channels that have mild correlation with mean ' +ecg_or_eog +';</p> <p>- Red: 33% of all channels that have the stronges correlation with mean ' +ecg_or_eog +'. </p>')]
-
-    return corr_derivs
-
-
 def split_correlated_artifacts_into_3_groups(artif_per_ch):
 
     """
     Collect artif_per_ch into 3 lists - for plotting:
     - a third of all channels that are the most correlated with mean_rwave
     - a third of all channels that are the least correlated with mean_rwave
     - a third of all channels that are in the middle of the correlation with mean_rwave
@@ -1354,94 +1187,15 @@
     corr_val_of_last_most_correlated = max(all_most_correlated)
     corr_val_of_last_middle_correlated = max(all_middle_correlated)
     corr_val_of_last_least_correlated = max(all_least_correlated)
 
     return most_correlated, middle_correlated, least_correlated, corr_val_of_last_most_correlated, corr_val_of_last_middle_correlated, corr_val_of_last_least_correlated
 
 
-
-def plot_artif_per_ch_correlated_lobes(artif_per_ch: list, tmin: float, tmax: float, m_or_g: str, ecg_or_eog: str, chs_by_lobe: dict, flip_data: bool, verbose_plots: bool):
-
-    """
-    Plot average artifact for each channel, colored by lobe, 
-    channels are split into 3 separate plots, based on their correlation with mean_rwave: equal number of channels in each group.
-
-    Parameters
-    ----------
-    artif_per_ch : list
-        List of objects of class Avg_artif
-    tmin : float
-        Start time of the epoch (negative value)
-    tmax : float
-        End time of the epoch
-    m_or_g : str
-        Type of the channel: mag or grad
-    ecg_or_eog : str
-        Type of the artifact: ECG or EOG
-    chs_by_lobe : dict
-        Dictionary with channels split by lobe
-    flip_data : bool
-        Use True or False, doesnt matter here. It is only passed into the plotting function and influences the threshold presentation. But since treshold is not used in correlation method, this is not used.
-    verbose_plots : bool
-        If True, plots are shown in the notebook.
-
-    Returns
-    -------
-    artif_per_ch : list
-        List of objects of class Avg_artif
-    affected_derivs : list
-        List of objects of class QC_derivative (plots)
-    
-
-    """
-
-
-    most_correlated, middle_correlated, least_correlated, _, _, _ = split_correlated_artifacts_into_3_groups(artif_per_ch)
-
-    #plot using plotly: 
-    # artif_per_ch.artif_data - a third of all channels that are the most correlated with mean_rwave, 
-    # artif_per_ch.artif_data - a third of all channels that are the less with mean_rwave, 
-    # artif_per_ch.artif_data - a third of all channels that are the least correlated with mean_rwave
-
-    artif_time_vector = np.linspace(tmin, tmax, len(artif_per_ch[0].artif_data))
-
-    fig_most_affected = plot_affected_channels(most_correlated, None, artif_time_vector, ch_type=m_or_g, fig_tit=ecg_or_eog+' most affected channels (smoothed): ', chs_by_lobe=chs_by_lobe, flip_data=flip_data, smoothed = True, verbose_plots=False)
-    fig_middle_affected = plot_affected_channels(middle_correlated, None, artif_time_vector, ch_type=m_or_g, fig_tit=ecg_or_eog+' middle affected channels (smoothed): ', chs_by_lobe=chs_by_lobe, flip_data=flip_data, smoothed = True, verbose_plots=False)
-    fig_least_affected = plot_affected_channels(least_correlated, None, artif_time_vector, ch_type=m_or_g, fig_tit=ecg_or_eog+' least affected channels (smoothed): ', chs_by_lobe=chs_by_lobe, flip_data=flip_data, smoothed = True, verbose_plots=False)
-
-    #set the same Y axis limits for all 3 figures for clear comparison:
-    
-    # combine the data lists into one numpy array
-    arr = np.array([ch.artif_data for ch in artif_per_ch])
-
-    # #find the highest and lowest value in artif_per_ch.artif_data:
-    ymin = np.min(arr)
-    ymax = np.max(arr)
-
-    ylim = [ymin*.95, ymax*1.05]
-
-    # update the layout of all three figures with the same y-axis limits
-    fig_most_affected.update_layout(yaxis_range=ylim)
-    fig_middle_affected.update_layout(yaxis_range=ylim)
-    fig_least_affected.update_layout(yaxis_range=ylim)
-
-    if verbose_plots is True:
-        fig_most_affected.show()
-        fig_middle_affected.show()
-        fig_least_affected.show()
-    
-    affected_derivs = []
-    affected_derivs += [QC_derivative(fig_most_affected, ecg_or_eog+'most_affected_channels_'+m_or_g, 'plotly')]
-    affected_derivs += [QC_derivative(fig_middle_affected, ecg_or_eog+'middle_affected_channels_'+m_or_g, 'plotly')]
-    affected_derivs += [QC_derivative(fig_least_affected, ecg_or_eog+'least_affected_channels_'+m_or_g, 'plotly')]
-        
-    return affected_derivs
-
-
-def find_affected_over_mean(artif_per_ch: list, ecg_or_eog: str, params_internal: dict, thresh_lvl_peakfinder: float, plotflag: bool, verbose_plots: bool, m_or_g: str, chs_by_lobe: dict, norm_lvl: float, flip_data: bool, gaussian_sigma: float, artif_time_vector: np.ndarray):
+def find_affected_over_mean(artif_per_ch: list, ecg_or_eog: str, params_internal: dict, thresh_lvl_peakfinder: float, m_or_g: str, chs_by_lobe: dict, norm_lvl: float, flip_data: bool, gaussian_sigma: float, artif_time_vector: np.ndarray):
     
     """
     1. Calculate average ECG epoch on the epochs from all channels. Check if average has a wave shape. 
     If no wave shape - no need to check for affected channels further.
     If it has - check further
 
     2. Set a threshold which defines a high amplitude of ECG event. (All above this threshold counted as potential ECG peak.)
@@ -1466,18 +1220,14 @@
         list of Avg_artif objects
     ecg_or_eog : str
         'ECG' or 'EOG'
     params_internal : dict
         dictionary with parameters from setings_internal file
     thresh_lvl_peakfinder : float
         threshold for peakfinder. Defines the magnitude of the peak of the average ECG/EOG epoch multiplued by norm_lvl.
-    plotflag : bool
-        if True - plots will be made
-    verbose_plots : bool
-        if True - plots will be shown in notebook
     m_or_g : str
         'mag' or 'grad'
     chs_by_lobe : dict
         dictionary with channels grouped by lobes
     norm_lvl : float
         defines the threshold for peakfinder. Threshold = mean overall artifact poch magnitude * norm_lvl
     flip_data : bool
@@ -1551,44 +1301,23 @@
         print('___MEGqc___: ', avg_artif_description2)
 
         bad_avg_str = ''
 
         # detect channels which are over the threshold defined by mean_magnitude_peak (average overall artifact) and norm_lvl (set in config):
         affected_channels, not_affected_channels, artifact_lvl, affected_channels_smoothed, not_affected_channels_smoothed, artifact_lvl_smoothed = detect_channels_above_norm(norm_lvl=norm_lvl, list_mean_artif_epochs=artif_per_ch, mean_magnitude_peak=mean_magnitude_peak, t=artif_time_vector, t0_actual=t0_actual, window_size_for_mean_threshold_method=window_size_for_mean_threshold_method, mean_magnitude_peak_smoothed=mean_magnitude_peak_smoothed, t0_actual_smoothed=t0_actual_smoothed)
 
-        if plotflag is True:
-            fig_affected = plot_affected_channels(affected_channels, artifact_lvl, artif_time_vector, ch_type=m_or_g, fig_tit=ecg_or_eog+' affected channels (orig): ', chs_by_lobe=chs_by_lobe, flip_data=flip_data, smoothed = False, verbose_plots=verbose_plots)
-            fig_affected_smoothed = plot_affected_channels(affected_channels_smoothed, artifact_lvl_smoothed, artif_time_vector, ch_type=m_or_g, fig_tit=ecg_or_eog+' affected channels (smoothed): ', chs_by_lobe=chs_by_lobe, flip_data=flip_data, smoothed = True, verbose_plots=verbose_plots)
-            fig_not_affected = plot_affected_channels(not_affected_channels, artifact_lvl, artif_time_vector, ch_type=m_or_g, fig_tit=ecg_or_eog+' not affected channels (orig): ', chs_by_lobe=chs_by_lobe, flip_data=flip_data, smoothed = False, verbose_plots=verbose_plots)
-            fig_not_affected_smoothed = plot_affected_channels(not_affected_channels_smoothed, artifact_lvl_smoothed, artif_time_vector, ch_type=m_or_g, fig_tit=ecg_or_eog+' not affected channels (smoothed): ', chs_by_lobe=chs_by_lobe, flip_data=flip_data, smoothed = True, verbose_plots=verbose_plots)
-            
-            affected_derivs += [QC_derivative(fig_affected, ecg_or_eog+'_affected_channels_'+m_or_g, 'plotly')]
-            affected_derivs += [QC_derivative(fig_not_affected, ecg_or_eog+'_not_affected_channels_smooth'+m_or_g, 'plotly')]
-            affected_derivs += [QC_derivative(fig_affected_smoothed, ecg_or_eog+'_affected_channels_'+m_or_g, 'plotly')]
-            affected_derivs += [QC_derivative(fig_not_affected_smoothed, ecg_or_eog+'_not_affected_channels_smooth'+m_or_g, 'plotly')]
-
     else: #if the average artifact is bad - end processing
         tit, _ = get_tit_and_unit(m_or_g)
         avg_artif_description = tit+": BAD " +ecg_or_eog+ " average. Detected " + str(len(avg_overall_obj.peak_magnitude)) + " peak(s). Expected 1-" + str(max_n_peaks_allowed_for_avg) + " peaks (pos+neg). Affected channels can not be estimated."
         bad_avg_str = tit+": "+ ecg_or_eog+ " signal detection/reconstruction did not produce reliable results. Affected channels can not be estimated."
         print('___MEGqc___: ', bad_avg_str)
 
-
-    if plotflag is True:
-        fig_avg = avg_overall_obj.plot_epoch_and_peak(artif_time_vector, 'Mean '+ecg_or_eog+' artifact over all data: ', m_or_g, None, plot_original = True, plot_smoothed = True)
-
-        if verbose_plots is True:
-            fig_avg.show()
-        affected_derivs.insert(0, QC_derivative(fig_avg, 'overall_average_ECG_epoch_'+m_or_g, 'plotly', description_for_user = avg_artif_description))
-        #prepend the avg plot before all other plots. because they will be added to report in the order they are in list.
-
     return affected_channels, affected_derivs, bad_avg_str, avg_overall_obj
 
 
-
 #%%
 def make_dict_global_ECG_EOG(channels_ranked: list, use_method: str):
     """
     Make a dictionary for the global part of simple metrics for ECG/EOG artifacts.
     For ECG/EOG no local metrics are calculated, so global is the only one.
     
     Parameters
@@ -1733,16 +1462,14 @@
     
     Parameters
     ----------
     ecg_params : dict
         Dictionary with ECG parameters originating from config file.
     raw : mne.io.Raw
         Raw data.
-    verbose_plots : bool
-        If True, plots are displayed in notebook.
     
         
     Returns
     -------
     use_method : str
         String with the method chosen for the analysis.
     ecg_str : str
@@ -1861,15 +1588,15 @@
     for ch in eog_data:
         event_indexes, _ = find_peaks(ch, height=height, distance=round(0.5 * fs)) #assume there are no peaks within 0.5 seconds from each other.
         event_indexes_all += [event_indexes.tolist()]
 
     return eog_str, eog_data, event_indexes_all, eog_channel_names
 
 
-def check_mean_wave(raw: mne.io.Raw, use_method: str, ecg_data: np.ndarray, ecg_or_eog: str, event_indexes: np.ndarray, tmin: float, tmax: float, sfreq: int, params_internal: dict, thresh_lvl_peakfinder: float, verbose_plots: bool):
+def check_mean_wave(raw: mne.io.Raw, use_method: str, ecg_data: np.ndarray, ecg_or_eog: str, event_indexes: np.ndarray, tmin: float, tmax: float, sfreq: int, params_internal: dict, thresh_lvl_peakfinder: float):
 
     """
     Calculate mean R wave based on either real ECG channel data or on reconstructed data (depends on the method used) 
     and check if it has an R wave shape.
     Plot Rwave with peaks.
     
     Parameters
@@ -1932,34 +1659,18 @@
     if mean_rwave_obj.wave_shape is True:
         ecg_str_checked = 'Mean event of '+ecg_or_eog+' channel has expected shape.'
         print('___MEGqc___: ', ecg_str_checked)
     else:
         ecg_str_checked = 'Mean events of '+ecg_or_eog+' channel does not have expected shape. Artifact detection was not performed.'
         print('___MEGqc___: ', ecg_str_checked)
 
-
-    #Plot:
     if mean_rwave.size > 0:
         mean_rwave_time = np.linspace(tmin, tmax, len(mean_rwave))
-        if use_method == 'correlation_reconstructed':
-            title = 'Mean data of the RECONSTRUCTED '
-        elif use_method == 'correlation':
-            title = 'Mean data of the RECORDED '
-        else:
-            title = 'Mean data of '
 
-        mean_rwave_fig = mean_rwave_obj.plot_epoch_and_peak(mean_rwave_time, title, ecg_or_eog, fig = None, plot_original = True, plot_smoothed = False)
-        if verbose_plots is True:
-            mean_rwave_fig.show()
-
-        fig_derivs = [QC_derivative(mean_rwave_fig, 'Mean_artifact'+ecg_or_eog, 'plotly', description_for_user = ecg_str_checked)]
-    else:
-        fig_derivs = []
-
-    return mean_rwave_obj.wave_shape, ecg_str_checked, mean_rwave, mean_rwave_time, fig_derivs
+    return mean_rwave_obj.wave_shape, ecg_str_checked, mean_rwave, mean_rwave_time
 
 
 # Functions for alignment of ECG with meg channels:
 
 def find_t0_mean(ch_data: np.ndarray or list):
 
     """
@@ -2145,60 +1856,14 @@
 
     t0_shift = t0_channels - t0_mean
     mean_rwave_shifted = np.roll(mean_rwave, t0_shift)
 
     return mean_rwave_shifted
 
 
-def plot_mean_rwave_shifted(mean_rwave_shifted: np.ndarray, mean_rwave: np.ndarray, ecg_or_eog: str, tmin: float, tmax: float, verbose_plots: bool):
-    
-    """
-    Only for demonstartion while running the pipeline. Dpesnt go into final report.
-
-    Plots the mean ECG wave and the mean ECG wave shifted to align with the ECG artifacts found on meg channels.
-    Probably will not be included into the report. Just for algorythm demosntration.
-    The already shifted mean ECG wave is plotted in the report.
-
-    Parameters
-    ----------
-    mean_rwave_shifted : np.ndarray
-        The mean ECG wave shifted to align with the ECG artifacts found on meg channels.
-    mean_rwave : np.ndarray
-        The mean ECG wave, not shifted, original.
-    ecg_or_eog : str
-        'ECG' or 'EOG'
-    tmin : float
-        The start time of the epoch.
-    tmax : float
-        The end time of the epoch.
-    verbose_plots : bool
-        If True, the plot will be shown in the notebook.
-
-    Returns
-    -------
-    fig_derivs : list
-        list with one QC_derivative object, which contains the plot. (in case want to input intot he report)
-    
-    """
-
-    t = np.linspace(tmin, tmax, len(mean_rwave_shifted))
-    fig = go.Figure()
-    fig.add_trace(go.Scatter(x=t, y=mean_rwave_shifted, mode='lines', name='mean_rwave_shifted'))
-    fig.add_trace(go.Scatter(x=t, y=mean_rwave, mode='lines', name='mean_rwave'))
-
-    if verbose_plots is True:
-        fig.show()
-
-    #fig_derivs = [QC_derivative(fig, 'Mean_artifact_'+ecg_or_eog+'_shifted', 'plotly')] 
-    # #activate is you want to output the shift demonstration to the report, normally dont'
-    
-    fig_derivs = []
-
-    return fig_derivs
-
 
 def align_mean_rwave(mean_rwave: np.ndarray, artif_per_ch: list, tmin: float, tmax: float):
 
     """ Aligns the mean ECG wave with the ECG artifacts found on meg channels.
     1) The average highest point of 10 most prominent meg channels is used as refernce.
     The ECG artifact is shifted multiple times, 
     2) each time the correlation of ECG channel with
@@ -2241,15 +1906,15 @@
     for t0_m in t0_mean:
         mean_rwave_shifted_variations.append(shift_mean_wave(mean_rwave, t0_channels, t0_m))
     
     return mean_rwave_shifted_variations
 
 
 #%%
-def ECG_meg_qc(ecg_params: dict, ecg_params_internal: dict, raw: mne.io.Raw, channels: list, chs_by_lobe_orig: dict, m_or_g_chosen: list, verbose_plots: bool):
+def ECG_meg_qc(ecg_params: dict, ecg_params_internal: dict, raw: mne.io.Raw, channels: list, chs_by_lobe_orig: dict, m_or_g_chosen: list):
     
     """
     Main ECG function. Calculates average ECG artifact and finds affected channels.
     
     Parameters
     ----------
     ecg_params : dict
@@ -2260,16 +1925,14 @@
         Raw data.
     channels : dict
         Dictionary with listds of channels for each channel type (mag and grad).
     chs_by_lobe : dict
         Dictionary with lists of channels by lobe.
     m_or_g_chosen : list
         List of channel types chosen for the analysis.
-    verbose_plots : bool
-        True for showing plot in notebook.
         
     Returns
     -------
     ecg_derivs : list
         List of all derivatives (plotly figures) as QC_derivative instances
     simple_metric_ECG : dict
         Dictionary with simple metrics for ECG artifacts to be exported into json file.
@@ -2279,18 +1942,14 @@
 
     """
 
     chs_by_lobe = copy.deepcopy(chs_by_lobe_orig) 
     #in case we will change this variable in any way. If not copied it might introduce errors in parallel processing. 
     # This variable is used in all modules
 
-    if verbose_plots is False:
-        matplotlib.use('Agg') 
-        #this command will suppress showing matplotlib figures produced by mne. They will still be saved for use in report but not shown when running the pipeline
-
     sfreq=raw.info['sfreq']
     tmin=ecg_params_internal['ecg_epoch_tmin']
     tmax=ecg_params_internal['ecg_epoch_tmax']
 
     #WROTE THIS BEFORE, BUT ACTUALLY NEED TO CHECK IF IT S STILL TRUE OR THE PROBLEM WAS SOLVED FOR THRESHOLD METHOD:
     #tmin, tmax can be anything from -0.1/0.1 to -0.04/0.04. for CORRELATION method. But if we do mean and threshold - time best has to be -0.04/0.04. 
     # For this method number of peaks in particular time frame is calculated and based on that good/bad rwave is decided.
@@ -2298,24 +1957,22 @@
     gaussian_sigma=ecg_params['gaussian_sigma']
     thresh_lvl_peakfinder=ecg_params['thresh_lvl_peakfinder']
 
     ecg_derivs = []
     use_method, ecg_str, ecg_ch_df, ecg_data, event_indexes = get_ECG_data_choose_method(raw, ecg_params)
     
 
-    mean_good, ecg_str_checked, mean_rwave, mean_rwave_time, rwave_derivs = check_mean_wave(raw, use_method, ecg_data, 'ECG', event_indexes, tmin, tmax, sfreq, ecg_params_internal, thresh_lvl_peakfinder, verbose_plots)
+    mean_good, ecg_str_checked, mean_rwave, mean_rwave_time = check_mean_wave(raw, use_method, ecg_data, 'ECG', event_indexes, tmin, tmax, sfreq, ecg_params_internal, thresh_lvl_peakfinder)
     
     ecg_str += ecg_str_checked
 
     ecg_ch_df['mean_rwave'] = mean_rwave.tolist() + [None] * (len(ecg_data) - len(mean_rwave))
     ecg_ch_df['mean_rwave_time'] = mean_rwave_time.tolist() + [None] * (len(ecg_data) - len(mean_rwave_time))
-    print('___MEGqc___: mean_rwave_time:', ecg_ch_df['mean_rwave_time'])
     ecg_ch_df['recorded_or_reconstructed'] = [use_method] + [None] * (len(ecg_data) - 1)
     ecg_derivs += [QC_derivative(content=ecg_ch_df, name='ECGchannel', content_type = 'df')]
-    ecg_derivs += rwave_derivs
 
     if mean_good is False:
         simple_metric_ECG = {'description': ecg_str}
         return ecg_derivs, simple_metric_ECG, ecg_str, []
 
     
     affected_channels={}
@@ -2335,74 +1992,85 @@
 
         #2 options:
         #1. find channels with peaks above threshold defined by average over all channels+multiplier set by user
         #2. find channels that have highest Pearson correlation with average R wave shape (if the ECG channel is present)
 
         if use_method == 'mean_threshold':
             artif_per_ch, artif_time_vector = flip_channels(artif_per_ch, tmin, tmax, sfreq, ecg_params_internal)
-            affected_channels[m_or_g], affected_derivs, bad_avg_str[m_or_g], avg_overall_obj = find_affected_over_mean(artif_per_ch, 'ECG', ecg_params_internal, thresh_lvl_peakfinder, plotflag=True, verbose_plots=verbose_plots, m_or_g=m_or_g, chs_by_lobe=chs_by_lobe[m_or_g], norm_lvl=norm_lvl, flip_data=True, gaussian_sigma=gaussian_sigma, artif_time_vector=artif_time_vector)
+            affected_channels[m_or_g], affected_derivs, bad_avg_str[m_or_g], avg_overall_obj = find_affected_over_mean(artif_per_ch, 'ECG', ecg_params_internal, thresh_lvl_peakfinder, m_or_g=m_or_g, chs_by_lobe=chs_by_lobe[m_or_g], norm_lvl=norm_lvl, flip_data=True, gaussian_sigma=gaussian_sigma, artif_time_vector=artif_time_vector)
             correlation_derivs = []
 
         elif use_method == 'correlation' or use_method == 'correlation_reconstructed':
 
+            #align the mean ECG wave with the ECG artifacts found on meg channels:
+            #Find the correlation value between all variations of alignment the mean ECG wave with the ECG artifacts found on meg channels.
+            #The alignment with the highest correlation is chosen as the final one.
+            #Our target is best_affected_channels[m_or_g] - the channels that are most correlated with the mean ECG wave, after all variations of alignemnt were checked.
+            #We also get best_mean_corr and best_mean_shifted - mostely useful if we wanna plot them.
+
             mean_rwave_shifted_variations = align_mean_rwave(mean_rwave, artif_per_ch, tmin, tmax)
             
             best_mean_corr = 0
+            best_mean_shifted = mean_rwave_shifted_variations[0] #preassign
             for mean_shifted in mean_rwave_shifted_variations:
                 affected_channels[m_or_g] = find_affected_by_correlation(mean_shifted, artif_per_ch)
                 #collect all correlation values for all channels:
                 all_corr_values = [abs(ch.corr_coef) for ch in affected_channels[m_or_g]]
-                #get 10 highest correlations:
+                # #get 10 highest correlations:
                 all_corr_values.sort(reverse=True)
                 all_corr_values = all_corr_values[:10]
                 mean_corr = np.mean(all_corr_values)
                 #if mean corr is better than the previous one - save it
 
-                best_mean_shifted = mean_shifted #preassign
                 if mean_corr > best_mean_corr:
                     best_mean_corr = mean_corr
                     best_mean_shifted = mean_shifted
-                    best_affected_channels[m_or_g] = affected_channels[m_or_g]
-
-            if verbose_plots is True:
-                plot_mean_rwave_shifted(best_mean_shifted, mean_rwave, 'ECG', tmin, tmax, verbose_plots)
+                    best_affected_channels[m_or_g] = copy.deepcopy(affected_channels[m_or_g])
             
-
             bad_avg_str[m_or_g] = ''
             avg_overall_obj = None
 
         else:
             raise ValueError('use_method should be either mean_threshold or correlation')
         
 
+        #calculate mean_corr for best_affected_channels and for affected_channels:
+        all_corr_values = [abs(ch.corr_coef) for ch in best_affected_channels[m_or_g]]
+        mean_corr = np.mean(all_corr_values)
+
+        all_corr_values = [abs(ch.corr_coef) for ch in affected_channels[m_or_g]]
+        mean_corr = np.mean(all_corr_values)
+
         #higher thresh_lvl_peakfinder - more peaks will be found on the eog artifact for both separate channels and average overall. As a result, average overll may change completely, since it is centered around the peaks of 5 most prominent channels.
         avg_objects_ecg.append(avg_overall_obj)
 
 
-    simple_metric_ECG = make_simple_metric_ECG_EOG(affected_channels, m_or_g_chosen, 'ECG', bad_avg_str, use_method)
+    simple_metric_ECG = make_simple_metric_ECG_EOG(best_affected_channels, m_or_g_chosen, 'ECG', bad_avg_str, use_method)
 
     #Extract chs_by_lobe into a data frame
     artif_time_vector = np.round(np.arange(tmin, tmax+1/sfreq, 1/sfreq), 3) #yes, you need to round
     #TODO: above we always use tmin, tmax, sfreq to create time vector in every fuction. here it s done again, maybe change above?
 
     for m_or_g  in m_or_g_chosen:
         for lobe, lobe_channels in chs_by_lobe[m_or_g].items():
             for lobe_ch in lobe_channels:
-                lobe_ch.add_ecg_info(affected_channels[m_or_g], artif_time_vector)
+                lobe_ch.add_ecg_info(best_affected_channels[m_or_g], artif_time_vector)
 
+    print('_____FIXED HERE____: ', best_affected_channels['mag'])
+    print('____WAS____: ', affected_channels['mag'])
 
     ecg_csv_deriv = chs_dict_to_csv(chs_by_lobe,  file_name_prefix = 'ECGs')
 
     ecg_derivs += ecg_csv_deriv
 
     return ecg_derivs, simple_metric_ECG, ecg_str, avg_objects_ecg
 
 
 #%%
-def EOG_meg_qc(eog_params: dict, eog_params_internal: dict, raw: mne.io.Raw, channels: dict, chs_by_lobe_orig: dict, m_or_g_chosen: list, verbose_plots: bool):
+def EOG_meg_qc(eog_params: dict, eog_params_internal: dict, raw: mne.io.Raw, channels: dict, chs_by_lobe_orig: dict, m_or_g_chosen: list):
     
     """
     Main EOG function. Calculates average EOG artifact and finds affected channels.
     
     Parameters
     ----------
     eog_params : dict
@@ -2413,16 +2081,14 @@
         Raw MEG data.
     channels : dict
         Dictionary with listds of channels for each channel type (mag and grad).
     chs_by_lobe : dict
         Dictionary with lists of channels separated by lobe.
     m_or_g_chosen : list
         List of channel types chosen for the analysis.
-    verbose_plots : bool
-        True for showing plot in notebook.
         
     Returns
     -------
     eog_derivs : list
         List of all derivatives (plotly figures) as QC_derivative instances
     simple_metric_EOG : dict
         Dictionary with simple metrics for ECG artifacts to be exported into json file.
@@ -2431,18 +2097,14 @@
     
     """
 
     chs_by_lobe = copy.deepcopy(chs_by_lobe_orig) 
     #in case we will change this variable in any way. If not copied it might introduce errors in parallel processing. 
     # This variable is used in all modules
 
-    if verbose_plots is False:
-        import matplotlib
-        matplotlib.use('Agg') #this command will suppress showing matplotlib figures produced by mne. They will still be saved for use in report but not shown when running the pipeline
-
     sfreq=raw.info['sfreq']
     tmin=eog_params_internal['eog_epoch_tmin']
     tmax=eog_params_internal['eog_epoch_tmax']
 
     norm_lvl=eog_params['norm_lvl']
     gaussian_sigma=eog_params['gaussian_sigma']
     thresh_lvl_peakfinder=eog_params['thresh_lvl_peakfinder']
@@ -2450,37 +2112,29 @@
     eog_str, eog_data, event_indexes, eog_ch_name = get_EOG_data(raw)
 
     eog_derivs = []
     if len(eog_data) == 0:
         simple_metric_EOG = {'description': eog_str}
         return eog_derivs, simple_metric_EOG, eog_str, []
     
-        
-    # for data, name in zip(eog_data, eog_ch_name):
-
-    #     fig = plot_ECG_EOG_channel(data, [], name, fs= raw.info['sfreq'], verbose_plots = verbose_plots)
-
-    #     eog_derivs += [QC_derivative(fig, name+' data', 'plotly')]
 
     # Now choose the channel with blinks only (if there are several):
     #(NEED TO FIGURE OUT HOW)
     eog_data = eog_data[0]
     eog_ch_name = eog_ch_name[0]
     event_indexes = event_indexes[0]
     print('___MEG_QC___: Blinks will be detected based on channel: ', eog_ch_name)
 
     
     use_method = 'correlation' #'mean_threshold' 
     #no need to choose method in EOG because we cant reconstruct channel, always correlaion (if channel present) or fail.
 
-    mean_good, eog_str_checked, mean_blink, mean_rwave_time, blink_derivs = check_mean_wave(raw, use_method, eog_data, 'EOG', event_indexes, tmin, tmax, sfreq, eog_params_internal, thresh_lvl_peakfinder, verbose_plots)
+    mean_good, eog_str_checked, mean_blink, mean_rwave_time = check_mean_wave(raw, use_method, eog_data, 'EOG', event_indexes, tmin, tmax, sfreq, eog_params_internal, thresh_lvl_peakfinder)
     eog_str += eog_str_checked
 
-    eog_derivs += blink_derivs
-
     if mean_good is False:
         simple_metric_EOG = {'description': eog_str}
         return eog_derivs, simple_metric_EOG, eog_str, []
 
 
     affected_channels={}
     bad_avg_str = {}
@@ -2496,15 +2150,15 @@
 
         #2 options:
         #1. find channels with peaks above threshold defined by average over all channels+multiplier set by user
         #2. find channels that have highest Pearson correlation with average R wave shape (if the ECG channel is present)
 
         if use_method == 'mean_threshold':
             artif_per_ch, artif_time_vector = flip_channels(artif_per_ch, tmin, tmax, sfreq, eog_params_internal)
-            affected_channels[m_or_g], affected_derivs, bad_avg_str[m_or_g], avg_overall_obj = find_affected_over_mean(artif_per_ch, 'EOG', eog_params_internal, thresh_lvl_peakfinder, plotflag=True, verbose_plots=verbose_plots, m_or_g=m_or_g, chs_by_lobe=chs_by_lobe[m_or_g], norm_lvl=norm_lvl, flip_data=True, gaussian_sigma=gaussian_sigma, artif_time_vector=artif_time_vector)
+            affected_channels[m_or_g], affected_derivs, bad_avg_str[m_or_g], avg_overall_obj = find_affected_over_mean(artif_per_ch, 'EOG', eog_params_internal, thresh_lvl_peakfinder, m_or_g=m_or_g, chs_by_lobe=chs_by_lobe[m_or_g], norm_lvl=norm_lvl, flip_data=True, gaussian_sigma=gaussian_sigma, artif_time_vector=artif_time_vector)
             correlation_derivs = []
 
         elif use_method == 'correlation' or use_method == 'correlation_reconstructed':
             
             affected_channels[m_or_g] = find_affected_by_correlation(mean_blink, artif_per_ch)
             bad_avg_str[m_or_g] = ''
             avg_overall_obj = None
```

### Comparing `meg_qc-0.1.9/meg_qc/calculation/metrics/Head_meg_qc.py` & `meg_qc-0.2.0/meg_qc/calculation/metrics/Head_meg_qc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 import numpy as np
 import pandas as pd
-import plotly.graph_objects as go
-from plotly.subplots import make_subplots
 import mne
-from mne.preprocessing import annotate_movement, compute_average_dev_head_t
 import time
 from meg_qc.plotting.universal_plots import QC_derivative
-import matplotlib #this is in case we will need to suppress mne matplotlib plots
-
-mne.viz.set_browser_backend('matplotlib')
-
 
 def compute_head_pos_std_and_max_rotation_movement(head_pos: np.ndarray):
 
     """
     Compute the standard deviation of the movement of the head over time and the maximum rotation and movement in 3 directions.
     
     Parameters
@@ -125,141 +118,14 @@
     df = pd.DataFrame(data=head_pos, columns=names)
 
     df_deriv = [QC_derivative(content = df, name = file_name_prefix, content_type = 'df')]
 
     return df_deriv
 
 
-def make_head_pos_plot(raw: mne.io.Raw, head_pos: np.ndarray, verbose_plots: bool):
-
-    """ 
-    Plot positions and rotations of the head.
-    
-    Parameters
-    ----------
-    raw : mne.io.Raw
-        Raw data.
-    head_pos : np.ndarray
-        Head positions and rotations.
-    verbose_plots : bool
-        True for showing plot in notebook.
-        
-    Returns
-    -------
-    head_derivs : list 
-        List of QC_derivative objects containing figures with head positions and rotations.
-    head_pos_baselined : np.ndarray
-        Head positions and rotations starting from 0 instead of the mne detected starting point. Can be used for plotting.
-    """
-
-    head_derivs = []
-
-    original_head_dev_t = mne.transforms.invert_transform(
-        raw.info['dev_head_t'])
-    average_head_dev_t = mne.transforms.invert_transform(
-        compute_average_dev_head_t(raw, head_pos))
-
-    if verbose_plots is False:
-        matplotlib.use('Agg') #this command will suppress showing matplotlib figures produced by mne. They will still be saved for use in report but not shown when running the pipeline
-
-    #plot using MNE:
-    fig1 = mne.viz.plot_head_positions(head_pos, mode='traces')
-    #fig1 = mne.viz.plot_head_positions(head_pos_degrees)
-    for ax, val, val_ori in zip(fig1.axes[::2], average_head_dev_t['trans'][:3, 3],
-                        original_head_dev_t['trans'][:3, 3]):
-        ax.axhline(1000*val, color='r')
-        ax.axhline(1000*val_ori, color='g')
-        #print('___MEGqc___: ', 'val', val, 'val_ori', val_ori)
-    # The green horizontal lines represent the original head position, whereas the
-    # Red lines are the new head position averaged over all the time points.
-
-
-    head_derivs += [QC_derivative(fig1, 'Head_position_rotation_average_mne', 'matplotlib', description_for_user = 'The green horizontal lines - original head position. Red lines - the new head position averaged over all the time points.')]
-
-
-    #plot head_pos using PLOTLY:
-
-    # First, for each head position subtract the first point from all the other points to make it always deviate from 0:
-    head_pos_baselined=head_pos.copy()
-    #head_pos_baselined=head_pos_degrees.copy()
-    for i, pos in enumerate(head_pos_baselined.T[1:7]):
-        pos -= pos[0]
-        head_pos_baselined.T[i]=pos
-
-    t = head_pos.T[0]
-
-    average_head_pos=average_head_dev_t['trans'][:3, 3]
-    original_head_pos=original_head_dev_t['trans'][:3, 3]
-
-    fig1p = make_subplots(rows=3, cols=2, subplot_titles=("Position (mm)", "Rotation (quat)"))
-
-    # head_pos ndarray of shape (n_pos, 10): [t, q1, q2, q3, x, y, z, gof, err, v]
-    # https://mne.tools/stable/generated/mne.chpi.compute_head_pos.html
-    indexes=[4, 5, 6, 1, 2,3]
-    names=['x', 'y', 'z', 'q1', 'q2', 'q3']
-    for counter in [0, 1, 2]:
-        position=1000*-head_pos.T[indexes][counter]
-        #position=1000*-head_pos_baselined.T[indexes][counter]
-        name_pos=names[counter]
-        fig1p.add_trace(go.Scatter(x=t, y=position, mode='lines', name=name_pos), row=counter+1, col=1)
-        fig1p.update_yaxes(title_text=name_pos, row=counter+1, col=1)
-        #print('name', name_pos, 'position', position)
-        rotation=head_pos.T[indexes][counter+3]
-        #rotation=head_pos_baselined.T[indexes][counter+3]
-        name_rot=names[counter+3]
-        fig1p.add_trace(go.Scatter(x=t, y=rotation, mode='lines', name=name_rot), row=counter+1, col=2)
-        fig1p.update_yaxes(title_text=name_rot, row=counter+1, col=2)
-        #print('name', name_rot, 'rotation', rotation)
-
-        # fig1p.add_hline(y=1000*average_head_pos[counter], line_dash="dash", line_color="red", row=counter+1, col=1)
-        # fig1p.add_hline(y=1000*original_head_pos[counter], line_dash="dash", line_color="green", row=counter+1, col=1)
-
-    fig1p.update_xaxes(title_text='Time (s)', row=3, col=1)
-    fig1p.update_xaxes(title_text='Time (s)', row=3, col=2)
-
-    if verbose_plots is True:
-        fig1p.show()
-
-    head_derivs += [QC_derivative(fig1p, 'Head_position_rotation_average_plotly', 'plotly', description_for_user = 'The green horizontal lines - original head position. Red lines - the new head position averaged over all the time points.')]
-
-    return head_derivs, head_pos_baselined
-
-
-def make_head_annots_plot(raw: mne.io.Raw, head_pos: np.ndarray):
-
-    """
-    Plot raw data with annotated head movement. Currently not used.
-
-    
-    Parameters
-    ----------
-    raw : mne.io.Raw
-        Raw data.
-    head_pos : np.ndarray
-        Head positions and rotations.
-        
-    Returns
-    -------
-    head_derivs : list
-        List of QC derivatives with annotated figures.
-        
-    """
-
-    head_derivs = []
-
-    mean_distance_limit = 0.0015  # in meters
-    annotation_movement, hpi_disp = annotate_movement(
-        raw, head_pos, mean_distance_limit=mean_distance_limit)
-    raw.set_annotations(annotation_movement)
-    fig2=raw.plot(n_channels=100, duration=20)
-    head_derivs += [QC_derivative(fig2, 'Head_position_annot', 'matplotlib')]
-
-    return head_derivs
-
-
 def get_head_positions(raw: mne.io.Raw):
     
     """
     Get head positions and rotations using MNE
     
     Parameters
     ----------
@@ -322,15 +188,15 @@
     print('___MEGqc___: ', "Finished computing head positions. --- Execution %s seconds ---" % (time.time() - start_time))
     #print('___MEGqc___: ', 'Head positions:', head_pos)
 
     return head_pos, no_head_pos_str
 
 
 
-def HEAD_movement_meg_qc(raw: mne.io.Raw, verbose_plots: bool, plot_annotations: bool =False):
+def HEAD_movement_meg_qc(raw: mne.io.Raw):
 
     """
     Main function for head movement. Calculates:
 
     - head positions (x, y, z) and rotations (q1, q2, q3)
     - maximum amplitude of positions and rotations
     - std of positions and rotations over whole time series: 
@@ -338,20 +204,14 @@
         2) calculate std of these values and get 1 std for positions and 1 std for rotations over whole time series.
     
 
     Parameters
     ----------
     raw : mne.io.Raw
         Raw data.
-    verbose_plots : bool
-        True for showing plot in notebook.
-    plot_with_lines : bool
-        If True, plot head movement with lines.
-    plot_annotations : bool
-        If True, plot head movement with annotations.
         
     Returns
     -------
     head_derivs : list
         List of QC derivatives with figures.
     simple_metrics_head : dict
         Dictionary with simple metrics for head movement.
@@ -374,33 +234,23 @@
     # see: https://en.wikipedia.org/wiki/Quaternions_and_spatial_rotation)
 
     head_pos_degrees=head_pos.T.copy()
     for q in range(1,4):
         head_pos_degrees[q]=360/(2*np.pi)*head_pos_degrees[q]
     head_pos_degrees=head_pos_degrees.transpose()
 
-    head_csv = head_pos_to_csv('Head', head_pos)
-    #f_path = head_pos_to_csv('Head', head_pos_degrees)
-
-    # MNE plot:
-    if plot_annotations is True:
-        plot_annot_derivs = make_head_annots_plot(raw, head_pos, verbose_plots=verbose_plots)
-    else:
-        plot_annot_derivs = []
+    head_derivs = head_pos_to_csv('Head', head_pos)
 
     # Calculate the standard deviation of the movement of the head over time:
     std_head_pos, std_head_rotations, max_movement_xyz, max_rotation_q, df_head_pos = compute_head_pos_std_and_max_rotation_movement(head_pos)
 
-
     print('___MEGqc___: ', 'Std of head positions in mm: ', std_head_pos*1000)
     print('___MEGqc___: ', 'Std of head rotations in quat: ', std_head_rotations)
     print('___MEGqc___: ', 'Max movement (x, y, z) in mm: ', [m*1000 for m in max_movement_xyz])
     print('___MEGqc___: ', 'Max rotation (q1, q2, q3) in quat: ', max_rotation_q)
 
     # Make a simple metric:
     simple_metrics_head = make_simple_metric_head(std_head_pos, std_head_rotations, max_movement_xyz, max_rotation_q)
-    
-    head_derivs = plot_annot_derivs + head_csv
 
     return head_derivs, simple_metrics_head, head_str, df_head_pos, head_pos
```

### Comparing `meg_qc-0.1.9/meg_qc/calculation/metrics/PSD_meg_qc.py` & `meg_qc-0.2.0/meg_qc/calculation/metrics/PSD_meg_qc.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,81 +81,14 @@
     }]
 
     fig.update_layout(updatemenus=updatemenus)
 
     return fig
 
 
-def Plot_psd_old(m_or_g:str, freqs: np.ndarray, psds:np.ndarray, channels: list, chs_by_lobe: dict, method: str, verbose_plots: bool):
-
-    """
-    Plotting Power Spectral Density for all channels. OLD version
-
-    Parameters
-    ----------
-    m_or_g : str
-        'mag' or 'grad'
-    freqs : np.ndarray
-        frequencies
-    psds : np.ndarray
-        power spectral density for each channel
-    channels : list
-        list of channel names
-    chs_by_lobe : dict
-        dictionary with channel objects sorted by lobe
-    method : str
-        'welch' or 'multitaper' or other method
-    verbose_plots : bool
-        True for showing plot in notebook.
-
-    Returns
-    -------
-    QC_derivative
-        QC_derivative object with plotly figure as content
-
-        
-    """
-
-    df_psds=pd.DataFrame(psds.T, columns=channels)
-
-    # Assuming df_psds is a DataFrame with a DateTimeIndex
-    downsampling_factor = 1  # replace with your desired downsampling factor
-    df_psds_downsampled = df_psds[::downsampling_factor]
-
-    fig = plot_df_of_channels_data_as_lines_by_lobe(chs_by_lobe, df_psds, freqs)
-
-    tit, unit = get_tit_and_unit(m_or_g)
-    fig.update_layout(
-    title={
-    'text': method[0].upper()+method[1:]+" periodogram for all "+tit,
-    'y':0.85,
-    'x':0.5,
-    'xanchor': 'center',
-    'yanchor': 'top'},
-    yaxis_title="Amplitude, "+unit,
-    yaxis = dict(
-        showexponent = 'all',
-        exponentformat = 'e'),
-    xaxis_title="Frequency (Hz)")
-
-    fig.update_traces(hovertemplate='Frequency: %{x} Hz<br>Amplitude: %{y: .2e} T/Hz')
-
-    #Add buttons to switch scale between log and linear:
-    fig = add_log_buttons(fig)
-
-    if verbose_plots is True:
-        fig.show()
-    
-    fig_name='PSD_all_data_'+tit
-
-    qc_derivative = QC_derivative(content=fig, name=fig_name, content_type='plotly')
-
-    return qc_derivative
-
-
 def get_mean_bands_amplitude(freq_bands: list, freqs: list, psds: np.ndarray or list, channels: list, bands_names: list = None):
 
     """
     Calculate the area under the curve of frequency bands (e.g. alpha, beta, gamma, delta, ...) for mag or grad.
     Adopted from: https://raphaelvallat.com/bandpower.html
     Take mean over all channels (mags/grads).
 
@@ -242,15 +175,15 @@
 
     return band_ampl_df, band_ampl_relative_to_signal_df, ampl_by_Nfreq_per_ch_list_df, total_signal_amplitude
 
 
     
 # In[53]:
 
-def get_ampl_of_brain_waves(channels: list, m_or_g: str, freqs: np.ndarray, psds: np.ndarray, avg_psd: np.ndarray, plotflag: bool, verbose_plots: bool):
+def get_ampl_of_brain_waves(channels: list, m_or_g: str, freqs: np.ndarray, psds: np.ndarray, avg_psd: np.ndarray):
 
     """
     Amplitude of frequencies calculation for all channels.
     If desired: creating a pie chart of mean amplitude of every band over the entire data.
 
     Parameters
     ----------
@@ -260,23 +193,19 @@
         'mag' or 'grad' - to choose which channels to calculate amplitude for.
     freqs : np.ndarray
         numpy array of frequencies for mag  or grad
     psds : np.ndarray
         numpy array of power spectrum dencities for mag or grad
     avg_psd : np.ndarray
         numpy array of average power spectrum dencities for mag or grad
-    plotflag : bool
-        need to plot pie chart or not
-    verbose_plots : bool
-        True for showing plot in notebook.
 
     Returns
     -------
-    psd_pie_derivative : QC_derivative object or empty list
-        If plotflag is True, returns one QC_derivative object, which is a plotly piechart figure.
+    waves_pie_df_deriv : QC_derivative object or empty list
+        If plotflag is True, returns one QC_derivative object with data for pie plot.
         If plotflag is False, returns empty list.
     dfs_with_name : list
         List of dataframes with amplitude of each frequency band in each channel
         (dfs: absolute amplitude, relative amplitude, amplitude divided by number of frequencies in the band)
     mean_brain_waves_dict : dict
         Dictionary of mean amplitude of each frequency band (used for simple metric json)
 
@@ -359,15 +288,15 @@
                 split_indexes.append(int(split_ind))
 
     #print('split_indexes', split_indexes, 'noisy_bands_final_indexes', noisy_bands_final_indexes)
 
     return noisy_bands_final_indexes, split_indexes
 
 
-def cut_the_noise_from_psd(noisy_bands_indexes: List[dict], freqs: list, one_psd: list, helper_plots: bool, ch_name: str ='', noisy_freqs_indexes: list =[], unit: str ='', verbose_plots: bool = True):
+def cut_the_noise_from_psd(noisy_bands_indexes: List[dict], freqs: list, one_psd: list, helper_plots: bool, ch_name: str ='', noisy_freqs_indexes: list =[], unit: str =''):
 
     """
     Cut the noise peaks out of PSD curve. By default, it is not used, but can be turned on.
     If turned on, in the next steps, the area under the curve will be calculated only for the cut out peaks.
 
     By default, the area under the curve is calculated under the whole peak, uncluding the 'main brain signal' psd area + peak area. 
     This is done, because in reality we can not define, which part of the 'noisy' frequency is signal and which is noise. 
@@ -394,16 +323,14 @@
     ch_name : str, optional
         channel name, by default '', used for plot display
     noisy_freqs_indexes : list, optional
         list of indexes of noisy frequencies. Indexes! not frequencies themselves. Index is defined by fequency/freq_resolution., 
         by default [] because we might have no noisy frequencies at all. Used for plot display.
     unit : str, optional
         unit of the psd values, by default '', used for plot display
-    verbose_plots : bool
-        True for showing plot in notebook.
 
     Returns
     -------
     psd_only_peaks_baselined : list
         vector of psd values for 1 channel (or 1 average over all channels) with the noise peaks cut out and baselined to 0 level.
         Later used to calculate area under the curve for the noise peaks only.
     
@@ -462,21 +389,20 @@
             fig.add_shape(type="rect", xref="x", yref="y", x0=freqs[noisy_bands_indexes[i][0]], y0=0, x1=freqs[noisy_bands_indexes[i][1]], y1=max(one_psd), line_color="LightSeaGreen", line_width=2, fillcolor="LightSeaGreen", opacity=0.3, layer="below", row=1, col=1)
             fig.add_shape(type="rect", xref="x", yref="y", x0=freqs[noisy_bands_indexes[i][0]], y0=0, x1=freqs[noisy_bands_indexes[i][1]], y1=max(one_psd), line_color="LightSeaGreen", line_width=2, fillcolor="LightSeaGreen", opacity=0.3, layer="below", row=1, col=2)
             fig.add_shape(type="rect", xref="x", yref="y", x0=freqs[noisy_bands_indexes[i][0]], y0=0, x1=freqs[noisy_bands_indexes[i][1]], y1=max(one_psd), line_color="LightSeaGreen", line_width=2, fillcolor="LightSeaGreen", opacity=0.3, layer="below", row=2, col=1)
             fig.add_shape(type="rect", xref="x", yref="y", x0=freqs[noisy_bands_indexes[i][0]], y0=0, x1=freqs[noisy_bands_indexes[i][1]], y1=max(one_psd), line_color="LightSeaGreen", line_width=2, fillcolor="LightSeaGreen", opacity=0.3, layer="below", row=2, col=2)
 
         fig.update_layout(height=800, width=1300, title_text=ch_name+' PSD before and after cutting the noise')
 
-        if verbose_plots is True:
-            fig.show()
-            #or show each figure separately:
-            # fig1.show()
-            # fig2.show()
-            # fig3.show()
-            # fig4.show()
+        fig.show()
+        #or show each figure separately:
+        # fig1.show()
+        # fig2.show()
+        # fig3.show()
+        # fig4.show()
 
     return psd_only_peaks_baselined
 
 
 def plot_one_psd(ch_name: str, freqs: List, one_psd: List, peak_indexes: List, noisy_freq_bands_indexes: List[list], unit: str):
     
     """
@@ -521,15 +447,15 @@
     
     #Add buttons to switch scale between log and linear:
     fig = add_log_buttons(fig)
     
     return fig
 
 
-def find_noisy_freq_bands_complex(ch_name: str, freqs: list, one_psd: list, helper_plots: bool, m_or_g: str, prominence_lvl_pos: int, verbose_plots: bool):
+def find_noisy_freq_bands_complex(ch_name: str, freqs: list, one_psd: list, helper_plots: bool, m_or_g: str, prominence_lvl_pos: int):
 
     """
     Detect the frequency band around the noise peaks.
     Complex approach: This function is trying to detect the actual start and end of peaks.
 
     1. Bands around the noise frequencies are created based on detected peak_width.
     2. If the found bands overlap, they are cut at the lowest point between 2 neighbouring noise peaks pn PSD curve.
@@ -548,16 +474,14 @@
         list of psd values for one channels or for the average over multiple channels
     helper_plots : bool
         if True, helper plots will be shown
     m_or_g : str
         'mag' or 'grad' - for plotting purposes only - to get the unit of the psd values
     prominence_lvl_pos : int
         prominence level for peak detection. The higher the value, the more peaks will be detected. 
-    verbose_plots : bool
-        True for showing plot in notebook.
 
 
     Returns
     -------
     noisy_freqs : list
         list of noisy frequencies
     noisy_freqs_indexes : list
@@ -578,17 +502,15 @@
     noisy_freqs_indexes, _ = find_peaks(one_psd, prominence=prominence_pos)
 
     if noisy_freqs_indexes.size==0: #if no noise found
 
         if helper_plots is True: #visual
             _, unit = get_tit_and_unit(m_or_g, True)
             fig = plot_one_psd(ch_name, freqs, one_psd, [], [], unit)
-
-            if verbose_plots is True:
-                fig.show()
+            fig.show()
 
         return [], [], [], [], [], []
 
 
     noisy_freqs=freqs[noisy_freqs_indexes]
 
     # Make frequency bands around noise frequencies on base of the detected width of the peaks:
@@ -602,27 +524,25 @@
 
     # Split the blended freqs at the lowest point between 2 peaks 
     noisy_bands_final_indexes, split_indexes = split_blended_freqs_at_the_lowest_point(noisy_bands_indexes, one_psd, noisy_freqs_indexes)
     #print(ch_name, 'LOWEST POINT ', 'noisy_bands_final_indexes: ', noisy_bands_final_indexes, 'split_indexes: ', split_indexes)
 
     if helper_plots is True: #visual of the split
         fig = plot_one_psd(ch_name, freqs, one_psd, noisy_freqs_indexes, noisy_bands_final_indexes, unit)
-
-        if verbose_plots is True:
-            fig.show()
+        fig.show()
 
     #Get actual freq bands from their indexes:
     noisy_bands_final=[]
     for fr_b in noisy_bands_final_indexes:
         noisy_bands_final.append([freqs[fr_b][0], freqs[fr_b][1]])
 
     return noisy_freqs, noisy_freqs_indexes, noisy_bands_final, noisy_bands_final_indexes, split_indexes
 
 
-def find_noisy_freq_bands_simple(ch_name: str, freqs: list, one_psd: list, helper_plots: bool, m_or_g: str, prominence_lvl_pos: int, band_half_length: float, verbose_plots: bool):
+def find_noisy_freq_bands_simple(ch_name: str, freqs: list, one_psd: list, helper_plots: bool, m_or_g: str, prominence_lvl_pos: int, band_half_length: float):
     
     """
     Form a frequency band around the noise peaks.
     Simple approach: used by default.
 
     1. Create frequency band around central noise frequency just by adding -x...+x Hz around.
     2. If the found bands overlap, they are cut at the lowest point between 2 neighbouring noise peaks pn PSD curve.
@@ -639,16 +559,14 @@
         if True, helper plots will be shown
     m_or_g : str
         'mag' or 'grad' - for plotting purposes only - to get the unit of the psd values
     prominence_lvl_pos : int
         prominence level for peak detection. The higher the value, the more peaks will be detected. 
     band_half_length : float
         length of the frequency band before and after the noise peak in Hz. The band will be created by adding -band_half_length...+band_half_length Hz around the noise peak.
-    verbose_plots : bool
-        True for showing plot in notebook.
 
     Returns
     -------
     noisy_freqs : list
         list of noisy frequencies
     noisy_freqs_indexes : list
         list of indexes of noisy frequencies in the psd
@@ -666,17 +584,15 @@
 
 
     if noisy_freqs_indexes.size==0:
 
         if helper_plots is True: #visual
             _, unit = get_tit_and_unit(m_or_g, True)
             fig = plot_one_psd(ch_name, freqs, one_psd, [], [], unit)
-
-            if verbose_plots is True:
-                fig.show()
+            fig.show()
 
         return [], [], [], [], []
 
     #make frequency bands around the central noise frequency (-1...+1 Hz band around the peak):
     freq_res = freqs[1] - freqs[0]
     noisy_bands_indexes=[]
     for i, _ in enumerate(noisy_freqs_indexes):
@@ -691,26 +607,24 @@
         
     
     # Split the blended freqs if their bands cross:
     noisy_bands_final_indexes, split_indexes = split_blended_freqs_at_the_lowest_point(noisy_bands_indexes, one_psd, noisy_freqs_indexes)
     if helper_plots is True: #visual of the split
         _, unit = get_tit_and_unit(m_or_g, True)
         fig = plot_one_psd(ch_name, freqs, one_psd, noisy_freqs_indexes, noisy_bands_final_indexes, unit)
-
-        if verbose_plots is True:
-            fig.show()
+        fig.show()
 
     noisy_freqs = freqs[noisy_freqs_indexes]
 
     noisy_bands_final = [[freqs[noisy_bands_final_indexes[i][0]], freqs[noisy_bands_final_indexes[i][1]]] for i in range(len(noisy_bands_final_indexes))]
 
     return noisy_freqs, noisy_freqs_indexes, noisy_bands_final, noisy_bands_final_indexes, split_indexes
 
 
-def find_number_and_ampl_of_noise_freqs(ch_name: str, freqs: list, one_psd: list, pie_plotflag: bool, helper_plots: bool, m_or_g: str, cut_noise_from_psd: bool, prominence_lvl_pos: int, simple_or_complex: str = 'simple', verbose_plots: bool = True):
+def find_number_and_ampl_of_noise_freqs(ch_name: str, freqs: list, one_psd: list, helper_plots: bool, m_or_g: str, cut_noise_from_psd: bool, prominence_lvl_pos: int, simple_or_complex: str = 'simple'):
 
     """
     The function finds the number and amplitude of noisy frequencies in PSD function in these steps:
 
     1. Calculate average psd curve over all channels
     2. Run peak detection on it -> get number of noise freqs. Create the bands around them. Split blended freqs.
     3. (Optional) Fit a curve to the general psd OR cut the noise peaks at the point they start and baseline them to 0. Optional. By default not used
@@ -724,29 +638,25 @@
     ----------
     ch_name : str
         name of the channel or 'average'
     freqs : list
         list of frequencies
     one_psd : list
         list of psd values for one channel or average psd
-    pie_plotflag : bool
-        if True, plot the pie chart
     helper_plots : bool
         if True, plot the helper plots (will show the noise bands, how they are split and how the peaks are cut from the psd if this is activated).
     m_or_g : str
         'mag' or 'grad'
     cut_noise_from_psd : bool
         if True, cut the noise peaks at the point they start and baseline them to 0. Optional. By default not used
     prominence_lvl_pos : int
         prominence level for peak detection (central frequencies of noise bands). The higher the value, the more peaks will be detected. 
         prominence_lvl will be different for average psd and psd of 1 channel, because average has small peaks smoothed.
     simple_or_complex : str
         'simple' or 'complex' approach to create the bands around the noise peaks. Simple by default. See functions above for details.
-    verbose_plots : bool
-        True for showing plot in notebook.
 
     Returns
     -------
     noise_pie_derivative : list
         list with QC_derivative object containing the pie chart with the noise amplitude and signal amplitude
     noise_ampl : list
         list of noise amplitudes for each noisy frequency band
@@ -761,18 +671,18 @@
     _, unit = get_tit_and_unit(m_or_g, True)
 
     #Total amplitude of the signal together with noise:
     freq_res = freqs[1] - freqs[0]
     total_amplitude = simpson(one_psd, dx=freq_res) 
 
     if simple_or_complex == 'simple':
-        noisy_freqs, noisy_freqs_indexes, noisy_bands_final, noisy_bands_indexes_final, split_indexes = find_noisy_freq_bands_simple(ch_name, freqs, one_psd, helper_plots, m_or_g, prominence_lvl_pos, band_half_length=1, verbose_plots=verbose_plots)
+        noisy_freqs, noisy_freqs_indexes, noisy_bands_final, noisy_bands_indexes_final, split_indexes = find_noisy_freq_bands_simple(ch_name, freqs, one_psd, helper_plots, m_or_g, prominence_lvl_pos, band_half_length=1)
         # band_half_length is set to 1. Means we go 1Hz left and 1 Hz right from the central freq to create a band.
     elif simple_or_complex == 'complex':
-        noisy_freqs, noisy_freqs_indexes, noisy_bands_final, noisy_bands_indexes_final, split_indexes = find_noisy_freq_bands_complex(ch_name, freqs, one_psd, helper_plots, m_or_g, prominence_lvl_pos, verbose_plots=verbose_plots)
+        noisy_freqs, noisy_freqs_indexes, noisy_bands_final, noisy_bands_indexes_final, split_indexes = find_noisy_freq_bands_complex(ch_name, freqs, one_psd, helper_plots, m_or_g, prominence_lvl_pos)
     else:
         print('simple_or_complex should be either "simple" or "complex"')
         return
 
     #3*. Cut the noise peaks at the point they start and baseline them to 0.
     if cut_noise_from_psd is True:
         psd_noise_final = cut_the_noise_from_psd(noisy_bands_indexes_final, freqs, one_psd, helper_plots, ch_name, noisy_freqs_indexes, unit)
@@ -793,34 +703,38 @@
         noise_ampl = noise_ampl_df.iloc[0, :].values.tolist() #take the first and only raw, because there is only one channel calculated by this fucntion
         noise_ampl_relative_to_signal=noise_ampl_relative_to_signal_df.iloc[0, :].values.tolist()
     else:
         noise_ampl = []
         noise_ampl_relative_to_signal = []
 
     if ch_name.lower() == 'average':
-        #need to save to tsv only if we are on the average psd curve, 
-        #dont need to save for every channel.
+
+        # Replace empty lists with [0] in case no noise was found:
+        noisy_freqs = noisy_freqs if len(noisy_freqs) else [0]
+        noise_ampl = noise_ampl if len(noise_ampl) else [0]
+        noise_ampl_relative_to_signal = noise_ampl_relative_to_signal if len(noise_ampl_relative_to_signal) else [0]
+        # will put 0 in the pie chart if no noise was found (if arrays/lists are empty and have 0 length)
 
         # Create a DataFrame
         df = pd.DataFrame({
             'noisy_freqs_'+m_or_g: noisy_freqs,
             'noise_ampl_'+m_or_g: noise_ampl,
             'noise_ampl_relative_to_signal_'+m_or_g: noise_ampl_relative_to_signal,
-            'total_amplitude_'+m_or_g: [total_amplitude] + [np.nan] * (len(noisy_freqs) - 1)})  # Add total_amplitude only once
+            'total_amplitude_'+m_or_g: [total_amplitude] + [np.nan] * (len(noisy_freqs) - len([total_amplitude]))})  # Add total_amplitude only once, rest fill with none
 
         noise_pie_df_deriv = QC_derivative(content=df, name='PSDnoise'+m_or_g.capitalize(), content_type = 'df')
 
     else:
         noise_pie_df_deriv = []
 
     return noise_pie_df_deriv, noise_ampl, noise_ampl_relative_to_signal, noisy_freqs
 
 
 
-def get_ampl_of_noisy_freqs(channels, freqs, avg_psd, psds, m_or_g, pie_plotflag=True, helperplots=True, cut_noise_from_psd=False, prominence_lvl_pos_avg=50, prominence_lvl_pos_channels=15, simple_or_complex='simple', verbose_plots: bool = True):
+def get_ampl_of_noisy_freqs(channels, freqs, avg_psd, psds, m_or_g, helper_plots, cut_noise_from_psd=False, prominence_lvl_pos_avg=50, prominence_lvl_pos_channels=15, simple_or_complex='simple'):
 
     """
     Find noisy frequencies, their absolute and relative amplitude for averages over all channel (mag or grad) PSD and for each separate channel.
 
     Parameters
     ----------
     channels : list
@@ -829,32 +743,28 @@
         list of frequencies
     avg_psd : list
         list of average PSD values over all channels
     psds : list
         list of PSD values for each channel
     m_or_g : str
         'mag' or 'grad'
-    pie_plotflag : bool
-        if True, plot pie chart of SNR
-    helperplots : bool
+    helper_plots : bool
         if True, plot helper plots
     cut_noise_from_psd : bool
         if True, cut the noise peaks at the point they start and baseline them to 0.
     prominence_lvl_pos_avg : int
         prominence level of peak detection for finding noisy frequencies in the average PSD
     prominence_lvl_pos_channels : int
         prominence level of peak detection for finding noisy frequencies in the PSD of each channel
     simple_or_complex : str
         'simple' or 'complex' - method of finding noisy frequencies. see find_number_and_ampl_of_noise_freqs() for details
-    verbose_plots : bool
-        True for showing plot in notebook.
 
     Returns
     -------
-    noise_pie_derivative : QC_derivative object or empty list if pie_plotflag is False
+    noise_pie_derivative : QC_derivative object or empty list 
         QC_derivative containig a pie chart of SNR
     noise_ampl_global : dict
         dictionary for simple metric with info about noisy frequencies in the average PSD, absolute values for bands
     noise_ampl_relative_to_all_signal_global : dict
         dictionary for simple metric with info about noisy frequencies in the average PSD, relative values for bands
     noisy_freqs_global : dict
         dictionary for simple metric with info about noisy frequencies in the average PSD, central frequencies
@@ -865,32 +775,24 @@
     noisy_freqs_local_all_ch : dict
         dictionary for simple metric with info about noisy frequencies in the PSD of each channel, central frequencies
     
     
     """
 
     #Calculate noise freqs globally: on the average psd curve over all channels together:
-    noise_pie_derivative, noise_ampl_global, noise_ampl_relative_to_all_signal_global, noisy_freqs_global = find_number_and_ampl_of_noise_freqs('Average', freqs, avg_psd, pie_plotflag, helperplots, m_or_g, cut_noise_from_psd, prominence_lvl_pos_avg, simple_or_complex, verbose_plots)
+    noise_pie_derivative, noise_ampl_global, noise_ampl_relative_to_all_signal_global, noisy_freqs_global = find_number_and_ampl_of_noise_freqs('Average', freqs, avg_psd, helper_plots, m_or_g, cut_noise_from_psd, prominence_lvl_pos_avg, simple_or_complex)
 
 
     #Calculate noise freqs locally: on the psd curve of each channel separately:
     noise_ampl_local_all_ch={}
     noise_ampl_relative_to_all_signal_local_all_ch={}
     noisy_freqs_local_all_ch={}
 
-    for ch_n, ch in enumerate(channels): 
-
-        if (ch_n==1 or ch_n==35 or ch_n==70 or ch_n==92) and helperplots is True: 
-            #plot only for some channels. For test purposes only!
-            helper_plotflag=True
-        else:
-            helper_plotflag=False
-
-        _, noise_ampl_local_all_ch[ch], noise_ampl_relative_to_all_signal_local_all_ch[ch], noisy_freqs_local_all_ch[ch] = find_number_and_ampl_of_noise_freqs(ch, freqs, psds[ch_n,:], False, helper_plotflag, m_or_g, cut_noise_from_psd, prominence_lvl_pos_channels, simple_or_complex, verbose_plots)
-        #here pie_plotflag is set to false, otherwise it ll produce a pie for each channel.
+    for ch_n, ch in enumerate(channels): #for each channel separately
+        _, noise_ampl_local_all_ch[ch], noise_ampl_relative_to_all_signal_local_all_ch[ch], noisy_freqs_local_all_ch[ch] = find_number_and_ampl_of_noise_freqs(ch, freqs, psds[ch_n,:], helper_plots, m_or_g, cut_noise_from_psd, prominence_lvl_pos_channels, simple_or_complex)
 
     return noise_pie_derivative, noise_ampl_global, noise_ampl_relative_to_all_signal_global, noisy_freqs_global, noise_ampl_local_all_ch, noise_ampl_relative_to_all_signal_local_all_ch, noisy_freqs_local_all_ch
 
 
 def make_dict_global_psd(mean_brain_waves_dict: dict, noisy_freqs_global: list, noise_ampl_global: list, noise_ampl_relative_to_all_signal_global: list):
 
     """
@@ -1071,15 +973,15 @@
         for ch_n, ch in enumerate(chs_by_lobe[lobe]):
             ch.psd = psds[ch_n]
             ch.freq = freqs
 
     return chs_by_lobe
 
 #%%
-def PSD_meg_qc(psd_params: dict, channels:dict, chs_by_lobe: dict, raw_orig: mne.io.Raw, m_or_g_chosen: list, verbose_plots: bool, helperplots: bool):
+def PSD_meg_qc(psd_params: dict, channels:dict, chs_by_lobe: dict, raw_orig: mne.io.Raw, m_or_g_chosen: list, helper_plots: bool):
     
     """
     Main psd function. Calculates:
 
     - PSD for each channel
     - amplitudes (area under the curve) of functionally distinct frequency bands, such as 
         delta (0.5-4 Hz), theta (4-8 Hz), alpha (8-12 Hz), beta (12-30 Hz), and gamma (30-100 Hz) for each channel 
@@ -1111,17 +1013,15 @@
         dictionary with channel names for each channel type: 'mag' or/and 'grad'
     chs_by_lobe : dict
         dictionary with channel objects sorted by ch type and lobe
     raw_orig : mne.io.Raw
         raw data
     m_or_g_chosen : list
         list with chosen channel types: 'mag' or/and 'grad'
-    verbose_plots : bool
-        True for showing plot in notebook.
-    helperplots : bool
+    helper_plots : bool
         if True, plots with noisy freq bands for average PSD + for 3 different channels will be created (but not added to report).
 
     Returns
     -------
     derivs_psd : list
         list with the psd derivatives as QC_derivative objects (figures)
     simple_metric : dict
@@ -1159,18 +1059,18 @@
 
         # Add psds and freqs into chs_by_lobe dict:
         chs_by_lobe_psd[m_or_g] = assign_psds_to_channels(chs_by_lobe_psd[m_or_g], freqs[m_or_g], psds[m_or_g])
 
         avg_psd=np.mean(psds[m_or_g],axis=0) # average psd over all channels
         
         #Calculate the amplitude of alpha, beta, etc bands for each channel + average over all channels:
-        bands_pie_df_deriv, dfs_wave_bands_ampl, mean_brain_waves_dict[m_or_g] = get_ampl_of_brain_waves(channels=channels[m_or_g], m_or_g = m_or_g, freqs = freqs[m_or_g], psds = psds[m_or_g], avg_psd=avg_psd, plotflag = True, verbose_plots=verbose_plots)
+        bands_pie_df_deriv, dfs_wave_bands_ampl, mean_brain_waves_dict[m_or_g] = get_ampl_of_brain_waves(channels=channels[m_or_g], m_or_g = m_or_g, freqs = freqs[m_or_g], psds = psds[m_or_g], avg_psd=avg_psd)
 
         # #Calculate noise freqs for each channel + on the average psd curve over all channels together:
-        noise_pie_derivative, noise_ampl_global[m_or_g], noise_ampl_relative_to_all_signal_global[m_or_g], noisy_freqs_global[m_or_g], noise_ampl_local[m_or_g], noise_ampl_relative_to_all_signal_local[m_or_g], noisy_freqs_local[m_or_g] = get_ampl_of_noisy_freqs(channels[m_or_g], freqs[m_or_g], avg_psd, psds[m_or_g], m_or_g, pie_plotflag=True, helperplots=helperplots, cut_noise_from_psd=False, prominence_lvl_pos_avg=50, prominence_lvl_pos_channels=15, simple_or_complex='simple', verbose_plots=verbose_plots)
+        noise_pie_derivative, noise_ampl_global[m_or_g], noise_ampl_relative_to_all_signal_global[m_or_g], noisy_freqs_global[m_or_g], noise_ampl_local[m_or_g], noise_ampl_relative_to_all_signal_local[m_or_g], noisy_freqs_local[m_or_g] = get_ampl_of_noisy_freqs(channels[m_or_g], freqs[m_or_g], avg_psd, psds[m_or_g], m_or_g, helper_plots=helper_plots, cut_noise_from_psd=False, prominence_lvl_pos_avg=50, prominence_lvl_pos_channels=15, simple_or_complex='simple')
         
         derivs_psd += dfs_wave_bands_ampl +[noise_pie_derivative] + bands_pie_df_deriv
 
 
     # Make a simple metric for PSD:
     simple_metric=make_simple_metric_psd(mean_brain_waves_dict, noise_ampl_global, noise_ampl_relative_to_all_signal_global, noisy_freqs_global, noise_ampl_local, noise_ampl_relative_to_all_signal_local, noisy_freqs_local, m_or_g_chosen, freqs, channels)
```

### Comparing `meg_qc-0.1.9/meg_qc/calculation/metrics/Peaks_auto_meg_qc.py` & `meg_qc-0.2.0/meg_qc/calculation/metrics/Peaks_auto_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.9/meg_qc/calculation/metrics/Peaks_manual_meg_qc.py` & `meg_qc-0.2.0/meg_qc/calculation/metrics/Peaks_manual_meg_qc.py`

 * *Files 3% similar despite different names*

```diff
@@ -255,15 +255,15 @@
             metric_local_content[m_or_g]=None
     
     simple_metric = simple_metric_basic(metric_global_name, metric_global_description, metric_global_content['mag'], metric_global_content['grad'], metric_local_name, metric_local_description, metric_local_content['mag'], metric_local_content['grad'])
 
     return simple_metric
 
 
-def PP_manual_meg_qc(ptp_manual_params: dict, channels: dict, chs_by_lobe: dict, dict_epochs_mg: dict, data: mne.io.Raw, m_or_g_chosen: list, verbose_plots: bool):
+def PP_manual_meg_qc(ptp_manual_params: dict, channels: dict, chs_by_lobe: dict, dict_epochs_mg: dict, data: mne.io.Raw, m_or_g_chosen: list):
 
     """
     Main Peak to peak amplitude function. Calculates:
     
     - Peak to peak amplitudes (PtP) of data for each channel over all time series.
     - Channels with big PtP (noisy) and small PtP (flat) over all time series.
     - PtP of data for each channel  in each epoch.
@@ -280,16 +280,14 @@
         dictionary with channels grouped first by ch type and then by lobe: chs_by_lobe['mag']['Left Occipital'] or chs_by_lobe['grad']['Left Occipital']
     dict_epochs_mg : dict
         Dict (mag, grad) with epochs for each channel. Should be the same for both channels. Used only to check if epochs are present.
     data : mne.io.Raw
         Raw data
     m_or_g_chosen : list
         'mag' or 'grad' or both, chosen by user in config file.
-    verbose_plots : bool
-        True for showing plot in notebook.
 
     Returns:
     --------
     derivs_ptp : list
         List with QC_deriv objects for peak-to-peak amplitude (figures and csv files)
     simple_metric_ptp_manual : dict
         Simple metric for peak-to-peak amplitude
@@ -326,22 +324,14 @@
 
     if dict_epochs_mg['mag'] is not None or dict_epochs_mg['grad'] is not None: #if epochs are present
         for m_or_g in m_or_g_chosen:
             df_ptp=get_ptp_epochs(channels[m_or_g], dict_epochs_mg[m_or_g], sfreq, ptp_manual_params['ptp_thresh_lvl'], ptp_manual_params['max_pair_dist_sec'])
             
             chs_by_lobe_ptp[m_or_g] = assign_epoched_std_ptp_to_channels(what_data='peaks', chs_by_lobe=chs_by_lobe_ptp[m_or_g], df_std_ptp=df_ptp) #for easier plotting
 
-            # fig_ptp_epoch0 += [boxplot_epoched_xaxis_channels(chs_by_lobe_copy[m_or_g], df_ptp, ch_type=m_or_g, what_data='peaks', verbose_plots=verbose_plots)]
-
-            #fig_ptp_epoch1 += [boxplot_epoched_xaxis_epochs(chs_by_lobe_copy[m_or_g], df_ptp, ch_type=m_or_g, what_data='peaks', verbose_plots=verbose_plots)]
-            
-            #older versions, no color coding:
-            #fig_ptp_epoch1 += [boxplot_epochs(df_mg=df_ptp, ch_type=m_or_g, what_data='peaks', x_axis_boxes='channels', verbose_plots=verbose_plots)] #old version
-            #fig_ptp_epoch2 += [boxplot_epochs(df_mg=df_ptp, ch_type=m_or_g, what_data='peaks', x_axis_boxes='epochs', verbose_plots=verbose_plots)]
-
             noisy_flat_epochs_derivs[m_or_g] = get_noisy_flat_std_ptp_epochs(df_ptp, m_or_g, 'ptp', ptp_manual_params['noisy_channel_multiplier'], ptp_manual_params['flat_multiplier'], ptp_manual_params['allow_percent_noisy_flat_epochs'])
             derivs_list += noisy_flat_epochs_derivs[m_or_g]
 
             metric_local=True
         pp_manual_str = ''
 
     else:
```

### Comparing `meg_qc-0.1.9/meg_qc/calculation/metrics/STD_meg_qc.py` & `meg_qc-0.2.0/meg_qc/calculation/metrics/STD_meg_qc.py`

 * *Files 1% similar despite different names*

```diff
@@ -470,15 +470,15 @@
             metric_local_content[m_or_g]=None
     
     simple_metric = simple_metric_basic(metric_global_name, metric_global_description, metric_global_content['mag'], metric_global_content['grad'], metric_local_name, metric_local_description, metric_local_content['mag'], metric_local_content['grad'])
 
     return simple_metric
 
 #%%
-def STD_meg_qc(std_params: dict, channels: dict, chs_by_lobe: dict, dict_epochs_mg: dict, data: mne.io.Raw, m_or_g_chosen: list, verbose_plots: bool):
+def STD_meg_qc(std_params: dict, channels: dict, chs_by_lobe: dict, dict_epochs_mg: dict, data: mne.io.Raw, m_or_g_chosen: list):
 
     """
     Main STD function. Calculates:
     - Std of data for each channel over all time series.
     - Channels with big std (noisy) and small std (flat) over all time series.
     - Std of data for each channel  in each epoch.
     - Epochs with big std (noisy) and small std (flat).
@@ -493,16 +493,14 @@
         dictionary with channels grouped first by ch type and then by lobe: chs_by_lobe['mag']['Left Occipital'] or chs_by_lobe['grad']['Left Occipital']
     dict_epochs_mg : dict
         dictionary with epochs for each channel type: dict_epochs_mg['mag'] or dict_epochs_mg['grad']
     data : mne.io.Raw
         raw data
     m_or_g_chosen : list
         list of strings with channel types chosen by user: ['mag', 'grad'] or ['mag'] or ['grad']
-    verbose_plots : bool
-        True for showing plot in notebook.
 
     Returns
     -------
     list
         list of QC_derivative objects containing data frames and figures for std metric.
     dict
         dictionary with simple metric for std/ptp.
```

### Comparing `meg_qc-0.1.9/meg_qc/calculation/metrics/muscle_meg_qc.py` & `meg_qc-0.2.0/meg_qc/calculation/metrics/muscle_meg_qc.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,20 +20,18 @@
 # spans of "good data" in between muscle artifacts are included in the
 # surrounding "BAD" annotation.
 # 
 
 
 import mne
 import pandas as pd
-mne.viz.set_browser_backend('matplotlib')
-import plotly.graph_objects as go
 from scipy.signal import find_peaks
 import numpy as np
 from mne.preprocessing import annotate_muscle_zscore
-from meg_qc.plotting.universal_plots import QC_derivative, get_tit_and_unit
+from meg_qc.plotting.universal_plots import QC_derivative
 
 def find_powerline_noise_short(raw, psd_params, m_or_g_chosen):
 
     method = 'welch'
     prominence_lvl_pos = 50 #this is a good level for average psd over all channels. Same should be used for PSD module.
     #WE CAN PUT THESE 2 ABOVE INTO CONFIG AS WELL.  BUT THEY ACTUALLY SHOULD NOT BE CHANGED BY USER. OR MAKE A SEPARATE CONFIG ONLY ACCED BY DEVELOPERS FOR SETTING DEFAULTS?
 
@@ -88,82 +86,14 @@
     'unit_muscle_evet_times': 'seconds',
     'unit_muscle_event_zscore': 'z-score',
     'zscore_thresholds': z_scores_dict}
 
     return simple_metric
 
 
-def plot_muscle(m_or_g: str, raw: mne.io.Raw, scores_muscle: np.ndarray, threshold_muscle: float, muscle_times: np.ndarray, high_scores_muscle: np.ndarray, verbose_plots: bool, annot_muscle: mne.Annotations = None, interactive_matplot:bool = False):
-
-    """
-    Plot the muscle events with the z-scores and the threshold.
-    
-    Parameters
-    ----------
-    m_or_g : str
-        The channel type used for muscle detection: 'mag' or 'grad'.
-    raw : mne.io.Raw
-        The raw data.
-    scores_muscle : np.ndarray
-        The z-scores of the muscle events.
-    threshold_muscle : float
-        The z-score threshold used for muscle detection.
-    muscle_times : np.ndarray
-        The times of the muscle events.
-    high_scores_muscle : np.ndarray
-        The z-scores of the muscle events over the threshold.
-    verbose_plots : bool
-        True for showing plot in notebook.
-    annot_muscle : mne.Annotations
-        The annotations of the muscle events. Used only for interactive_matplot.
-    interactive_matplot : bool
-        Whether to use interactive matplotlib plots or not. Default is False because it cant be extracted into the report.
-
-    Returns
-    -------
-    fig_derivs : list
-        A list of QC_derivative objects with plotly figures for muscle events.
-
-    """
-    fig_derivs = []
-
-    fig=go.Figure()
-    tit, _ = get_tit_and_unit(m_or_g)
-    fig.add_trace(go.Scatter(x=raw.times, y=scores_muscle, mode='lines', name='high freq (muscle scores)'))
-    fig.add_trace(go.Scatter(x=muscle_times, y=high_scores_muscle, mode='markers', name='high freq (muscle) events'))
-    #removed threshold, so this one is not plotted now:
-    #fig.add_trace(go.Scatter(x=raw.times, y=[threshold_muscle]*len(raw.times), mode='lines', name='z score threshold: '+str(threshold_muscle)))
-    fig.update_layout(xaxis_title='time, (s)', yaxis_title='zscore', title={
-    'text': "Muscle z scores (high fequency artifacts) over time based on "+tit,
-    'y':0.85,
-    'x':0.5,
-    'xanchor': 'center',
-    'yanchor': 'top'})
-
-    if verbose_plots is True:
-        fig.show()
-
-    fig_derivs += [QC_derivative(fig, 'muscle_z_scores_over_time_based_on_'+tit, 'plotly')]
-
-    # ## View the annotations (interactive_matplot)
-    if interactive_matplot is True:
-        order = np.arange(144, 164)
-        raw.set_annotations(annot_muscle)
-        fig2=raw.plot(start=5, duration=20, order=order)
-        #Change settings to show all channels!
-
-        # No suppressing of plots should be done here. This one is matplotlib interactive plot, so it ll only work with %matplotlib qt.
-        # Makes no sense to suppress it. Also, adding to QC_derivative is just formal, cos whe extracting to html it s not interactive any more. 
-        # Should not be added to report. Kept here in case mne will allow to extract interactive later.
-
-        fig_derivs += [QC_derivative(fig2, 'muscle_annotations_'+tit, 'matplotlib')]
-
-    return fig_derivs
-
-
 def filter_noise_before_muscle_detection(raw: mne.io.Raw, noisy_freqs_global: dict, muscle_freqs: list = [110, 140]):
 
     """
     Filter out power line noise and other noisy freqs in range of muscle artifacts before muscle artifact detection.
     MNE advices to filter power line noise. We also filter here noisy frequencies in range of muscle artifacts.
     List of noisy frequencies for filtering come from PSD artifact detection function. If any noise peaks were found there for mags or grads 
     they will all be passed here and checked if they are in range of muscle artifacts.
@@ -268,15 +198,15 @@
     # Concatenate the inverted data with the original data
     raw = mne.concatenate_raws([raw_dummy_start, raw, raw_dummy_end])
     print('Duration after attaching dummy data: ', raw.n_times / raw.info['sfreq'])
 
     return raw
 
 
-def calculate_muscle_over_threshold(raw, m_or_g_decided, muscle_params, threshold_muscle_list, muscle_freqs, cut_dummy, attach_sec, min_distance_between_different_muscle_events, verbose_plots, interactive_matplot, muscle_str_joined):
+def calculate_muscle_over_threshold(raw, m_or_g_decided, muscle_params, threshold_muscle_list, muscle_freqs, cut_dummy, attach_sec, min_distance_between_different_muscle_events, muscle_str_joined):
 
     muscle_derivs=[]
 
     for m_or_g in m_or_g_decided: #generally no need for loop, we will use just 1 type here. Left in case we change the principle.
 
         z_scores_dict={}
         for threshold_muscle in threshold_muscle_list:
@@ -299,29 +229,27 @@
 
             # Plot muscle z-scores across recording
             peak_locs_pos, _ = find_peaks(scores_muscle, height=threshold_muscle, distance=raw.info['sfreq']*min_distance_between_different_muscle_events)
 
             muscle_times = raw.times[peak_locs_pos]
             high_scores_muscle=scores_muscle[peak_locs_pos]
 
-            muscle_derivs += plot_muscle(m_or_g, raw, scores_muscle, threshold_muscle, muscle_times, high_scores_muscle, verbose_plots, interactive_matplot, annot_muscle)
-
             # collect all details for simple metric:
             z_score_details['muscle_event_times'] = muscle_times.tolist()
             z_score_details['muscle_event_zscore'] = high_scores_muscle.tolist()
             z_scores_dict[threshold_muscle] = {
                 'number_muscle_events': len(muscle_times), 
                 'Details': z_score_details}
             
         simple_metric = make_simple_metric_muscle(m_or_g_decided[0], z_scores_dict, muscle_str_joined)
 
     return muscle_derivs, simple_metric, scores_muscle
 
 
-def calculate_muscle_NO_threshold(raw, m_or_g_decided, muscle_params, threshold_muscle, muscle_freqs, cut_dummy, attach_sec, min_distance_between_different_muscle_events, verbose_plots, interactive_matplot, muscle_str_joined):
+def calculate_muscle_NO_threshold(raw, m_or_g_decided, muscle_params, threshold_muscle, muscle_freqs, cut_dummy, attach_sec, min_distance_between_different_muscle_events, muscle_str_joined):
 
     """
     annotate_muscle_zscore() requires threshold_muscle so define a minimal one here: 5 z-score.
     
     """
 
     for m_or_g in m_or_g_decided: #generally no need for loop, we will use just 1 type here. Left in case we change the principle.
@@ -374,15 +302,15 @@
     df=df.transpose()
 
     df_deriv = [QC_derivative(content = df, name = file_name_prefix, content_type = 'df')]
 
     return df_deriv
 
 
-def MUSCLE_meg_qc(muscle_params: dict, psd_params: dict, raw_orig: mne.io.Raw, noisy_freqs_global: dict, m_or_g_chosen:list, verbose_plots: bool, interactive_matplot:bool = False, attach_dummy:bool = True, cut_dummy:bool = True):
+def MUSCLE_meg_qc(muscle_params: dict, psd_params: dict, raw_orig: mne.io.Raw, noisy_freqs_global: dict, m_or_g_chosen:list, attach_dummy:bool = True, cut_dummy:bool = True):
 
     """
     Detect muscle artifacts in MEG data. 
     Gives the number of muscle artifacts based on the set z score threshold: artifact time + artifact z score.
     Threshold  is set by the user in the config file. Several thresholds can be used on the loop.
 
     Notes
@@ -399,19 +327,14 @@
         The parameters for PSD calculation originally defined in the config file. This in only needed to calculate powerline noise in case PSD was not calculated before.
     raw_orig : mne.io.Raw
         The raw data.
     noisy_freqs_global : list
         The powerline frequencies found in the data by previously running PSD_meg_qc.
     m_or_g_chosen : list
         The channel types chosen for the analysis: 'mag' or 'grad'.
-    verbose_plots : bool
-        True for showing plot in notebook.
-    interactive_matplot : bool
-        Whether to use interactive matplotlib plots or not. Default is False because it cant be extracted into the report. 
-        But might just be useful for beter undertanding while maintaining this function.
     attach_dummy : bool
         Whether to attach dummy data to the start and end of the recording to avoid filtering artifacts. Default is True.
     cut_dummy : bool
         Whether to cut the dummy data after filtering. Default is True.
 
     Returns
     -------
@@ -460,11 +383,11 @@
     # Filter out power line noise and other noisy freqs in range of muscle artifacts before muscle artifact detection.
     raw = filter_noise_before_muscle_detection(raw, noisy_freqs_global, muscle_freqs)
 
     # Loop through different thresholds for muscle artifact detection:
     threshold_muscle_list = muscle_params['threshold_muscle']  # z-score
     min_distance_between_different_muscle_events = muscle_params['min_distance_between_different_muscle_events']  # seconds
     
-    #muscle_derivs, simple_metric, scores_muscle = calculate_muscle_over_threshold(raw, m_or_g_decided, muscle_params, threshold_muscle_list, muscle_freqs, cut_dummy, attach_sec, min_distance_between_different_muscle_events, verbose_plots, interactive_matplot, muscle_str_joined)
-    simple_metric, scores_muscle, df_deriv = calculate_muscle_NO_threshold(raw, m_or_g_decided, muscle_params, threshold_muscle_list[0], muscle_freqs, cut_dummy, attach_sec, min_distance_between_different_muscle_events, verbose_plots, interactive_matplot, muscle_str_joined)
+    #muscle_derivs, simple_metric, scores_muscle = calculate_muscle_over_threshold(raw, m_or_g_decided, muscle_params, threshold_muscle_list, muscle_freqs, cut_dummy, attach_sec, min_distance_between_different_muscle_events, muscle_str_joined)
+    simple_metric, scores_muscle, df_deriv = calculate_muscle_NO_threshold(raw, m_or_g_decided, muscle_params, threshold_muscle_list[0], muscle_freqs, cut_dummy, attach_sec, min_distance_between_different_muscle_events, muscle_str_joined)
 
     return df_deriv, simple_metric, muscle_str_joined, scores_muscle, raw
```

### Comparing `meg_qc-0.1.9/meg_qc/plotting/meg_qc_plots.py` & `meg_qc-0.2.0/meg_qc/plotting/meg_qc_plots.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 import os
 import ancpbids
 import json
+import re
 
 from prompt_toolkit.shortcuts import checkboxlist_dialog
 from prompt_toolkit.styles import Style
 
 # Get the absolute path of the parent directory of the current script
 parent_dir = os.path.dirname(os.getcwd())
 gradparent_dir = os.path.dirname(parent_dir)
@@ -41,19 +42,20 @@
 # get it from the folders fro plotting - over ancp bids again??
 # plot only whst is requested by user: separate config + if condition like in pipeline?
 # do we save them as derivatives to write over abcp bids as report as before?
 
 
 def modify_entity_name(entities):
 
-    #old_new_categories = {'desc': 'METRIC', 'sub': 'SUBJECT', 'ses': 'SESSION', 'task': 'TASK', 'run': 'RUN'}
+    #old_new_categories = {'description': 'METRIC', 'subject': 'SUBJECT', 'session': 'SESSION', 'task': 'TASK', 'run': 'RUN'}
 
-    old_new_categories = {'desc': 'METRIC'}
+    old_new_categories = {'description': 'METRIC'}
 
     categories_copy = entities.copy()
+
     for category, subcategories in categories_copy.items():
         # Convert the set of subcategories to a sorted list
         sorted_subcategories = sorted(subcategories, key=str)
         # If the category is in old_new_categories, replace it with the new category
         if category in old_new_categories: 
             #This here is to replace the old names with new like desc -> METRIC
             #Normally we d use it only for the METRIC, but left this way in case the principle will extend to other categories
@@ -212,15 +214,14 @@
                 os.mkdir(dataset_path+'/derivatives')
 
         derivative = dataset.create_derivative(name="Meg_QC")
         derivative.dataset_description.GeneratedBy.Name = "MEG QC Pipeline"
 
 
         entities = dataset.query_entities()
-        print('___MEGqc___: ', 'entities', entities)
     
     return entities
 
 
 def csv_to_html_report(metric: str, tsv_paths: list, report_str_path: str, plot_settings):
 
     m_or_g_chosen = plot_settings['m_or_g'] 
@@ -365,19 +366,15 @@
     else:
         with open(report_str_path) as json_file:
             report_strings = json.load(json_file)
 
 
     report_html_string = make_joined_report_mne(raw, QC_derivs, report_strings, [])
 
-    for metric, values in QC_derivs.items():
-        if values and metric != 'Sensors':
-            QC_derivs['Report_MNE'] += [QC_derivative(report_html_string, 'REPORT_'+metric, 'report mne')]
-
-    return QC_derivs
+    return report_html_string 
 
 
 def make_plots_meg_qc(ds_paths):
 
     for dataset_path in ds_paths[0:1]: #run over several data sets
         dataset = ancpbids.load_dataset(dataset_path)
         schema = dataset.get_schema()
@@ -385,73 +382,116 @@
         derivative = dataset.create_derivative(name="Meg_QC")
         derivative.dataset_description.GeneratedBy.Name = "MEG QC Pipeline"
 
         entities = get_ds_entities(ds_paths) 
 
         chosen_entities, plot_settings = selector(entities)
 
-        #chosen_entities = {'sub': ['009'], 'ses': ['1'], 'task': ['deduction', 'induction'], 'run': ['1'], 'METRIC': ['ECGs', 'Muscle']}
+        #chosen_entities = {'subject': ['009'], 'session': ['1'], 'task': ['deduction', 'induction'], 'run': ['1'], 'METRIC': ['ECGs', 'Muscle']}
         
         print('___MEGqc___: CHOSEN entities to plot: ', chosen_entities)
         print('___MEGqc___: CHOSEN settings: ', plot_settings)
 
-        for sub in chosen_entities['sub']:
+        for sub in chosen_entities['subject']:
 
             print('_____sub____', sub)
 
             subject_folder = derivative.create_folder(type_=schema.Subject, name='sub-'+sub)
             list_of_sub_jsons = dataset.query(sub=sub, suffix='meg', extension='.fif')
 
             print('______list_of_sub_jsons')
             print(list_of_sub_jsons)
 
             try:
-                report_str_path = sorted(list(dataset.query(suffix='meg', extension='.json', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'ReportStrings', scope='derivatives')))[0]
+                report_str_path = sorted(list(dataset.query(suffix='meg', extension='.json', return_type='filename', subj=sub, ses = chosen_entities['session'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'ReportStrings', scope='derivatives')))[0]
             except:
                 report_str_path = '' #in case none was created yet
                 print('___MEGqc___: No report strings were created for sub ', sub)
 
             tsvs_to_plot = {}
+
             for metric in chosen_entities['METRIC']:
                 # Creating the full list of files for each combination
                 additional_str = None  # or additional_str = 'your_string'
                 desc = metric + additional_str if additional_str else metric
                 
-                tsv_path = sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = desc, scope='derivatives')))
+                tsv_path = sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['session'], task = chosen_entities['task'], run = chosen_entities['run'], desc = desc, scope='derivatives')))
 
                 if metric == 'PSDs':
-                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'PSDnoiseMag', scope='derivatives')))
-                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'PSDnoiseGrad', scope='derivatives')))
-                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'PSDwavesMag', scope='derivatives')))
-                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'PSDwavesGrad', scope='derivatives')))
+                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['session'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'PSDnoiseMag', scope='derivatives')))
+                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['session'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'PSDnoiseGrad', scope='derivatives')))
+                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['session'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'PSDwavesMag', scope='derivatives')))
+                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['session'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'PSDwavesGrad', scope='derivatives')))
                 
                 if metric == 'ECGs':
-                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'ECGchannel', scope='derivatives')))
+                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['session'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'ECGchannel', scope='derivatives')))
 
                 if metric == 'EOGs':
-                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['ses'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'EOGchannel', scope='derivatives')))
+                    tsv_path += sorted(list(dataset.query(suffix='meg', extension='.tsv', return_type='filename', subj=sub, ses = chosen_entities['session'], task = chosen_entities['task'], run = chosen_entities['run'], desc = 'EOGchannel', scope='derivatives')))
 
                 tsvs_to_plot[metric] = tsv_path
 
             print('___MEGqc___: TSVs to plot: ', tsvs_to_plot)
 
-            counter = 0
-            for metric, tsv_paths in tsvs_to_plot.items():
-                #for n_tsv, tsv_path in enumerate(files):
-
-                meg_artifact = subject_folder.create_artifact(raw=list_of_sub_jsons[counter]) #shell. empty derivative
-                meg_artifact.add_entity('desc', metric) #file name
-                meg_artifact.suffix = 'meg'
-                meg_artifact.extension = '.html'
-
-                # Here convert csv into figure and into html report:
-                deriv = csv_to_html_report(metric, tsv_paths, report_str_path, plot_settings)
+            print('___MEGqc___: list_of_sub_jsons', list_of_sub_jsons)
+            print('___MEGqc___: metric', metric)
+            print('___MEGqc___: tsvs_to_plot', tsvs_to_plot)
+
+            #We have raw files with particular entities, this raw file will be used to assign entities to final reports:
+            #in this line: meg_artifact = subject_folder.create_artifact(raw=sub_json)
+            #To make sure we assign the righ report (created on base of tsv files) to the right raw file, 
+            #we need to match the entities of the raw file with the entities of the tsv files.
+
+            #Among list_of_sub_jsons  find the one with the same subject, session, task, and run as the tsv file of tsv_paths:
+            # Get subject, session, task, and run from list_of_sub_jsons:
+            for sub_json in list_of_sub_jsons:
+                #First, loop over sub jsons - meaning over separate fif files belonging to the same subject:
+
+                # Extract sub, ses, task, and run from the name field of the JSON
+                #TODO: try to query entities instead?
+
+                match = re.search(r'sub-(\d+)_ses-(\d+)_task-(\w+)_run-(\d+)', sub_json['name'])
+                if match is not None:
+                    json_sub, json_ses, json_task, json_run = match.groups()
+                    print('___MEGqc___: ', 'json_sub', json_sub, 'json_ses', json_ses, 'json_task', json_task, 'json_run', json_run)
+
+                    for metric in tsvs_to_plot:
+                        #Second, loop over calculated metrics:
+
+                        tsv_paths_for_one_metric = []
+
+                        for tsv_path in tsvs_to_plot[metric]:
+                            # Extract sub, ses, task, and run from the tsv_paths
+                            print('___MEGqc___: ', 'tsv_path', tsv_path)
+                            match = re.search(r'sub-(\d+)_ses-(\d+)_task-(\w+)_run-(\d+)', tsv_path)
+                            if match is not None:
+                                tsv_sub, tsv_ses, tsv_task, tsv_run = match.groups()
+                                print('___MEGqc___: ', 'tsv_sub', tsv_sub, 'tsv_ses', tsv_ses, 'tsv_task', tsv_task, 'tsv_run', tsv_run)
+                    
+                                # Check if the entities match between the JSON and the TSV:
+                                if tsv_sub == json_sub and tsv_ses == json_ses and tsv_task == json_task and tsv_run == json_run:
+                                    
+                                    tsv_paths_for_one_metric += [tsv_path]
+                                    #collect all tsvs for the same metric in one list 
+                                    #to later add them all to the same report for this metric
+                                    
+
+                        # Now prepare the derivative to be written:
+                        meg_artifact = subject_folder.create_artifact(raw=sub_json)
+                        meg_artifact.add_entity('desc', metric) #file name
+                        meg_artifact.suffix = 'meg'
+                        meg_artifact.extension = '.html'
+
+                        
+                        # Here convert tsvs into figures and into html report:
+                        deriv = csv_to_html_report(metric, tsv_paths_for_one_metric, report_str_path, plot_settings)
+                        print('___MEGqc___: ', 'deriv', deriv)
 
-                meg_artifact.content = lambda file_path, cont=deriv['Report_MNE'][0].content: cont.save(file_path, overwrite=True, open_browser=False)
-                counter += 1
+                        #define method how the derivative will be written to file system:
+                        meg_artifact.content = lambda file_path, cont=deriv: cont.save(file_path, overwrite=True, open_browser=False)
 
     ancpbids.write_derivative(dataset, derivative) 
 
     return tsvs_to_plot
 
 
 # RUN IT:
```

### Comparing `meg_qc-0.1.9/meg_qc/plotting/universal_html_report.py` & `meg_qc-0.2.0/meg_qc/plotting/universal_html_report.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.9/meg_qc/plotting/universal_plots.py` & `meg_qc-0.2.0/meg_qc/plotting/universal_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 import random
 import copy
 import os
 
 from mne.preprocessing import compute_average_dev_head_t
 import matplotlib #this is in case we will need to suppress mne matplotlib plots
 
+# mne.viz.set_browser_backend('matplotlib')
+# matplotlib.use('Agg') 
+#this command will suppress showing matplotlib figures produced by mne. They will still be saved for use in report but not shown when running the pipeline
+
+
 class MEG_channels:
 
     """ 
     Channel with info for plotting: name, type, lobe area, color code, location, initial time series 
     + other data calculated by QC metrics (assigned in each metric separately while plotting).
 
     """
@@ -1811,14 +1816,16 @@
     return qc_derivative
 
 
 
 def plot_pie_chart_freq(amplitudes_relative: list, amplitudes_abs: list, total_amplitude: float, m_or_g: str, bands_names: list, fig_tit: str, fig_name: str, verbose_plots : bool):
     
     """
+    OLD VERSION, no csv 
+
     Plot pie chart representation of relative amplitude of each frequency band over the entire 
     times series of mags or grads, not separated by individual channels.
 
     Parameters
     ----------
     freq_amplitudes_relative : list
         list of relative amplitudes of each frequency band
@@ -1878,18 +1885,23 @@
     qc_derivative = QC_derivative(content=fig, name=fig_name, content_type='plotly')
 
     return qc_derivative
 
 
 def edit_legend_pie_SNR(noisy_freqs, noise_ampl, total_amplitude, noise_ampl_relative_to_signal):
 
-     #Legend for the pie chart:
+    #Legend for the pie chart:
+
     bands_names=[]
-    for fr_n, fr in enumerate(noisy_freqs):
-        bands_names.append(str(round(fr,1))+' Hz noise')
+    if noisy_freqs == [0]:
+        noisy_freqs, noise_ampl, noise_ampl_relative_to_signal = [], [], []
+        #empty lists so they dont show up on pie chart
+    else:
+        for fr_n, fr in enumerate(noisy_freqs):
+            bands_names.append(str(round(fr,1))+' Hz noise')
 
     bands_names.append('Main signal')
     
     noise_and_signal_ampl = noise_ampl.copy()
     noise_and_signal_ampl.append(total_amplitude-sum(noise_ampl)) #adding main signal ampl in the list
 
     noise_ampl_relative_to_signal.append(1-sum(noise_ampl_relative_to_signal)) #adding main signal relative ampl in the list
@@ -1924,35 +1936,35 @@
     -------
     QC_derivative
         QC_derivative object with plotly figure as content
 
     """
 
     #if it s not the right ch kind in the file
-    base_name = os.path.basename(tsv_pie_path) #name of the fimal file
+    base_name = os.path.basename(tsv_pie_path) #name of the final file
     
     if m_or_g not in base_name.lower():
         return []
     
     # Read the data from the TSV file into a DataFrame
     df = pd.read_csv(tsv_pie_path, sep='\t')
 
     if noise_or_waves == 'noise' and 'PSDnoise' in base_name:
         #check that we input tsv file with the right data
 
         fig_tit = "Ratio of signal and noise in the data: " 
         fig_name = 'PSD_SNR_all_channels_'
 
         # Extract the data
+        total_amplitude = df['total_amplitude_'+m_or_g].dropna().iloc[0]  # Get the first non-null value
         noisy_freqs = df['noisy_freqs_'+m_or_g].tolist()
+
         noise_ampl = df['noise_ampl_'+m_or_g].tolist()
-        #total_amplitude = df['total_amplitude_'+m_or_g][0]  # Assuming total_amplitude is the same for all rows
-        total_amplitude = df['total_amplitude_'+m_or_g].dropna().iloc[0]  # Get the first non-null value
         amplitudes_relative = df['noise_ampl_relative_to_signal_'+m_or_g].tolist()
-        
+
         amplitudes_abs, amplitudes_relative, bands_names = edit_legend_pie_SNR(noisy_freqs, noise_ampl, total_amplitude, amplitudes_relative)
 
     elif noise_or_waves == 'waves' and 'PSDwaves' in base_name:
 
         fig_tit = "Relative amplitude of each band: " 
         fig_name = 'PSD_Relative_band_amplitude_all_channels_'
 
@@ -1991,17 +2003,17 @@
         all_bands_names.append('other frequencies')
         all_mean_abs_values.append(total_amplitude - sum(all_mean_abs_values))
 
     labels=[None]*len(all_bands_names)
     for n, name in enumerate(all_bands_names):
         labels[n]=name + ': ' + str("%.2e" % all_mean_abs_values[n]) + ' ' + unit # "%.2e" % removes too many digits after coma
 
-    print('___here issue___')
-    print(all_mean_relative_values)
-    print(labels)
+        #if some of the all_mean_abs_values are zero - they should not be shown in pie chart:
+
+
 
     fig = go.Figure(data=[go.Pie(labels=labels, values=all_mean_relative_values)])
     fig.update_layout(
     title={
     'text': fig_tit + ch_type_tit,
     'y':0.85,
     'x':0.5,
@@ -2748,14 +2760,108 @@
         # Makes no sense to suppress it. Also, adding to QC_derivative is just formal, cos whe extracting to html it s not interactive any more. 
         # Should not be added to report. Kept here in case mne will allow to extract interactive later.
 
         fig_derivs += [QC_derivative(fig2, 'muscle_annotations_'+tit, 'matplotlib')]
     
     return fig_derivs
 
+def make_head_pos_plot_old(raw: mne.io.Raw, head_pos: np.ndarray, verbose_plots: bool):
+
+    """ 
+    Plot positions and rotations of the head.
+    
+    Parameters
+    ----------
+    raw : mne.io.Raw
+        Raw data.
+    head_pos : np.ndarray
+        Head positions and rotations.
+    verbose_plots : bool
+        True for showing plot in notebook.
+        
+    Returns
+    -------
+    head_derivs : list 
+        List of QC_derivative objects containing figures with head positions and rotations.
+    head_pos_baselined : np.ndarray
+        Head positions and rotations starting from 0 instead of the mne detected starting point. Can be used for plotting.
+    """
+
+    head_derivs = []
+
+    original_head_dev_t = mne.transforms.invert_transform(
+        raw.info['dev_head_t'])
+    average_head_dev_t = mne.transforms.invert_transform(
+        compute_average_dev_head_t(raw, head_pos))
+
+    if verbose_plots is False:
+        matplotlib.use('Agg') #this command will suppress showing matplotlib figures produced by mne. They will still be saved for use in report but not shown when running the pipeline
+
+    #plot using MNE:
+    fig1 = mne.viz.plot_head_positions(head_pos, mode='traces')
+    #fig1 = mne.viz.plot_head_positions(head_pos_degrees)
+    for ax, val, val_ori in zip(fig1.axes[::2], average_head_dev_t['trans'][:3, 3],
+                        original_head_dev_t['trans'][:3, 3]):
+        ax.axhline(1000*val, color='r')
+        ax.axhline(1000*val_ori, color='g')
+        #print('___MEGqc___: ', 'val', val, 'val_ori', val_ori)
+    # The green horizontal lines represent the original head position, whereas the
+    # Red lines are the new head position averaged over all the time points.
+
+
+    head_derivs += [QC_derivative(fig1, 'Head_position_rotation_average_mne', 'matplotlib', description_for_user = 'The green horizontal lines - original head position. Red lines - the new head position averaged over all the time points.')]
+
+
+    #plot head_pos using PLOTLY:
+
+    # First, for each head position subtract the first point from all the other points to make it always deviate from 0:
+    head_pos_baselined=head_pos.copy()
+    #head_pos_baselined=head_pos_degrees.copy()
+    for i, pos in enumerate(head_pos_baselined.T[1:7]):
+        pos -= pos[0]
+        head_pos_baselined.T[i]=pos
+
+    t = head_pos.T[0]
+
+    average_head_pos=average_head_dev_t['trans'][:3, 3]
+    original_head_pos=original_head_dev_t['trans'][:3, 3]
+
+    fig1p = make_subplots(rows=3, cols=2, subplot_titles=("Position (mm)", "Rotation (quat)"))
+
+    # head_pos ndarray of shape (n_pos, 10): [t, q1, q2, q3, x, y, z, gof, err, v]
+    # https://mne.tools/stable/generated/mne.chpi.compute_head_pos.html
+    indexes=[4, 5, 6, 1, 2,3]
+    names=['x', 'y', 'z', 'q1', 'q2', 'q3']
+    for counter in [0, 1, 2]:
+        position=1000*-head_pos.T[indexes][counter]
+        #position=1000*-head_pos_baselined.T[indexes][counter]
+        name_pos=names[counter]
+        fig1p.add_trace(go.Scatter(x=t, y=position, mode='lines', name=name_pos), row=counter+1, col=1)
+        fig1p.update_yaxes(title_text=name_pos, row=counter+1, col=1)
+        #print('name', name_pos, 'position', position)
+        rotation=head_pos.T[indexes][counter+3]
+        #rotation=head_pos_baselined.T[indexes][counter+3]
+        name_rot=names[counter+3]
+        fig1p.add_trace(go.Scatter(x=t, y=rotation, mode='lines', name=name_rot), row=counter+1, col=2)
+        fig1p.update_yaxes(title_text=name_rot, row=counter+1, col=2)
+        #print('name', name_rot, 'rotation', rotation)
+
+        # fig1p.add_hline(y=1000*average_head_pos[counter], line_dash="dash", line_color="red", row=counter+1, col=1)
+        # fig1p.add_hline(y=1000*original_head_pos[counter], line_dash="dash", line_color="green", row=counter+1, col=1)
+
+    fig1p.update_xaxes(title_text='Time (s)', row=3, col=1)
+    fig1p.update_xaxes(title_text='Time (s)', row=3, col=2)
+
+    if verbose_plots is True:
+        fig1p.show()
+
+    head_derivs += [QC_derivative(fig1p, 'Head_position_rotation_average_plotly', 'plotly', description_for_user = 'The green horizontal lines - original head position. Red lines - the new head position averaged over all the time points.')]
+
+    return head_derivs, head_pos_baselined
+
     
 def make_head_pos_plot_csv(f_path: str, verbose_plots: bool):
 
     """ 
     Plot positions and rotations of the head. On base of data from tsv file.
     
     Parameters
@@ -2809,15 +2915,14 @@
         fig1p.show()
 
     head_derivs = [QC_derivative(fig1p, 'Head_position_rotation_average_plotly', 'plotly', description_for_user = 'The green horizontal lines - original head position. Red lines - the new head position averaged over all the time points.')]
 
     return head_derivs, head_pos_baselined
 
 
-
 def make_head_pos_plot_mne(raw: mne.io.Raw, head_pos: np.ndarray, verbose_plots: bool):
 
     """
 
     Currently not used if we wanna plot solely from csv. 
     This function requires also raw as input and cant be only from csv.
 
@@ -2846,14 +2951,44 @@
     # Red lines are the new head position averaged over all the time points.
 
 
     head_derivs = [QC_derivative(fig1, 'Head_position_rotation_average_mne', 'matplotlib', description_for_user = 'The green horizontal lines - original head position. Red lines - the new head position averaged over all the time points.')]
 
     return head_derivs
 
+def make_head_annots_plot(raw: mne.io.Raw, head_pos: np.ndarray):
+
+    """
+    Plot raw data with annotated head movement. Currently not used.
+
+    
+    Parameters
+    ----------
+    raw : mne.io.Raw
+        Raw data.
+    head_pos : np.ndarray
+        Head positions and rotations.
+        
+    Returns
+    -------
+    head_derivs : list
+        List of QC derivatives with annotated figures.
+        
+    """
+
+    head_derivs = []
+
+    mean_distance_limit = 0.0015  # in meters
+    annotation_movement, hpi_disp = annotate_movement(
+        raw, head_pos, mean_distance_limit=mean_distance_limit)
+    raw.set_annotations(annotation_movement)
+    fig2=raw.plot(n_channels=100, duration=20)
+    head_derivs += [QC_derivative(fig2, 'Head_position_annot', 'matplotlib')]
+
+    return head_derivs
 
 #__________ECG/EOG__________#
 
 def plot_ECG_EOG_channel(ch_data: np.ndarray or list, peaks: np.ndarray or list, ch_name: str, fs: float, verbose_plots: bool):
 
     """
     Plot the ECG channel data and detected peaks
@@ -3363,8 +3498,54 @@
     
     if verbose_plots is True:
         fig.show()
 
     m_or_g_order = 0.1 if m_or_g == 'mag' else 0.2
     corr_derivs = [QC_derivative(fig, 'Corr_values_'+ecg_or_eog, 'plotly', description_for_user='Absolute value of the correlation coefficient is shown here. The sign would only represent the position of the channel towards magnetic field. <p>- Green: 33% of all channels that have the weakest correlation with mean ' +ecg_or_eog +'; </p> <p>- Yellow: 33% of all channels that have mild correlation with mean ' +ecg_or_eog +';</p> <p>- Red: 33% of all channels that have the stronges correlation with mean ' +ecg_or_eog +'. </p>', fig_order = 4+m_or_g_order)]
 
-    return corr_derivs
+    return corr_derivs
+
+
+def plot_mean_rwave_shifted(mean_rwave_shifted: np.ndarray, mean_rwave: np.ndarray, ecg_or_eog: str, tmin: float, tmax: float):
+    
+    """
+    Only for demonstartion while running the pipeline. Dpesnt go into final report.
+
+    Plots the mean ECG wave and the mean ECG wave shifted to align with the ECG artifacts found on meg channels.
+    Probably will not be included into the report. Just for algorythm demosntration.
+    The already shifted mean ECG wave is plotted in the report.
+
+    Parameters
+    ----------
+    mean_rwave_shifted : np.ndarray
+        The mean ECG wave shifted to align with the ECG artifacts found on meg channels.
+    mean_rwave : np.ndarray
+        The mean ECG wave, not shifted, original.
+    ecg_or_eog : str
+        'ECG' or 'EOG'
+    tmin : float
+        The start time of the epoch.
+    tmax : float
+        The end time of the epoch.
+    verbose_plots : bool
+        If True, the plot will be shown in the notebook.
+
+    Returns
+    -------
+    fig_derivs : list
+        list with one QC_derivative object, which contains the plot. (in case want to input intot he report)
+    
+    """
+
+    t = np.linspace(tmin, tmax, len(mean_rwave_shifted))
+    fig = go.Figure()
+    fig.add_trace(go.Scatter(x=t, y=mean_rwave_shifted, mode='lines', name='mean_rwave_shifted'))
+    fig.add_trace(go.Scatter(x=t, y=mean_rwave, mode='lines', name='mean_rwave'))
+
+    fig.show()
+
+    #fig_derivs = [QC_derivative(fig, 'Mean_artifact_'+ecg_or_eog+'_shifted', 'plotly')] 
+    # #activate is you want to output the shift demonstration to the report, normally dont'
+    
+    fig_derivs = []
+
+    return fig_derivs
```

### Comparing `meg_qc-0.1.9/meg_qc.egg-info/PKG-INFO` & `meg_qc-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: meg-qc
-Version: 0.1.9
+Name: meg_qc
+Version: 0.2.0
 Summary: Tool for automated MEG data quality control
 Home-page: https://github.com/AaronReer/MEGqc
 Author: ANCP
 Author-email: aaron.reer@uol.de
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
```

### Comparing `meg_qc-0.1.9/meg_qc.egg-info/SOURCES.txt` & `meg_qc-0.2.0/meg_qc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.9/setup.cfg` & `meg_qc-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.9/setup.py` & `meg_qc-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.9/versioneer.py` & `meg_qc-0.2.0/versioneer.py`

 * *Files identical despite different names*

