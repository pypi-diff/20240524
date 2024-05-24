# Comparing `tmp/stereoid-0.3.1.tar.gz` & `tmp/stereoid-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stereoid-0.3.1.tar", last modified: Tue Mar 26 09:09:16 2024, max compression
+gzip compressed data, was "stereoid-0.4.tar", last modified: Fri May 24 15:53:23 2024, max compression
```

## Comparing `stereoid-0.3.1.tar` & `stereoid-0.4.tar`

### file list

```diff
@@ -1,148 +1,147 @@
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.670938 stereoid-0.3.1/
--rw-r--r--   0 andreas   (1000) andreas   (1000)      669 2024-02-28 16:43:04.000000 stereoid-0.3.1/.gitignore
--rw-r--r--   0 andreas   (1000) andreas   (1000)    35149 2020-11-28 13:20:12.000000 stereoid-0.3.1/LICENSE
--rw-r--r--   0 andreas   (1000) andreas   (1000)       80 2024-03-26 09:08:36.000000 stereoid-0.3.1/MANIFEST.in
--rw-r--r--   0 andreas   (1000) andreas   (1000)     3618 2024-03-26 09:09:16.670938 stereoid-0.3.1/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2434 2024-02-28 16:43:04.000000 stereoid-0.3.1/README.rst
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1522 2024-03-26 09:08:36.000000 stereoid-0.3.1/pyproject.toml
--rw-r--r--   0 andreas   (1000) andreas   (1000)       38 2024-03-26 09:09:16.670938 stereoid-0.3.1/setup.cfg
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.658937 stereoid-0.3.1/stereoid/
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)       70 2021-06-29 13:50:14.000000 stereoid-0.3.1/stereoid/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     7653 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/cli.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.660937 stereoid-0.3.1/stereoid/land_ice/
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/land_ice/AASR_code.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     6571 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/land_ice/AASR_functions.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/land_ice/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)      307 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/land_ice/back_scatter_model.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    26892 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/land_ice/coherence_model_SAR_stack.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     7206 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/land_ice/coherence_model_baseline_volume.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     5057 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/land_ice/deterministic_data.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/land_ice/forward_model.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    14626 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/land_ice/ice_polarimetry.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    11789 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/land_ice/line_of_sight_vectors_worldwide.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     7158 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/land_ice/phase_model.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2310 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/land_ice/plot_SAR_vs_models.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     6358 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/land_ice/plot_functions.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/land_ice/radar_model.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/land_ice/retrieval_model.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    12008 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/land_ice/study_area_plots.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.660937 stereoid-0.3.1/stereoid/mission/
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)       70 2021-06-29 13:50:14.000000 stereoid-0.3.1/stereoid/mission/__init__.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)    14173 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/mission/acquisitions_script.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)    20327 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/mission/activation_analysis.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)     5927 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/mission/coverage.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)     9149 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/mission/formation_design.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.662937 stereoid-0.3.1/stereoid/oceans/
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.663937 stereoid-0.3.1/stereoid/oceans/GMF/
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)    12267 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/GMF/IWRAP_backscatter.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2752 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/GMF/Zadelhoff_crosspol.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/GMF/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     7476 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/GMF/cdop.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     6415 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/GMF/cmod5n.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)      464 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    38063 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/bistatic_pol.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     6415 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/cmod5n.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    23057 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/dca_performance.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    78076 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/forward_model.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.664937 stereoid-0.3.1/stereoid/oceans/forward_models/
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.664937 stereoid-0.3.1/stereoid/oceans/forward_models/Deprecated/
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/forward_models/Deprecated/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2563 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/forward_models/Deprecated/polarimetry.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    44954 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/forward_models/Doppler.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    12859 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/forward_models/RIM_calibration.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2376 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/forward_models/RIM_constants.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    77102 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/forward_models/SAR_spectra.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    26668 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/forward_models/SAR_spectra_broken.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/forward_models/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    34271 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/forward_models/backscatter.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2398 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/forward_models/sea_state_bias.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    24816 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/forward_models/wrappers.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)     2614 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/image_processing.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.664937 stereoid-0.3.1/stereoid/oceans/inversion/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     8128 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/inversion/RIM_inversion_deprecated.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    29340 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/inversion/wave_spectra_inversion.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     5397 2020-09-10 10:10:19.000000 stereoid-0.3.1/stereoid/oceans/l2_covariance.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     6398 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/les.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     5044 2024-01-22 16:22:18.000000 stereoid-0.3.1/stereoid/oceans/profile_add_errors.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    31089 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/radar_model.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)     3848 2021-06-29 13:50:14.000000 stereoid-0.3.1/stereoid/oceans/read_fwd.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     6897 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/read_scenario_California.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     7182 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/read_scenarios.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    41894 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/retrieval_model.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    18243 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/retrieval_performance.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    26599 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/run_scenario.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    11980 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/scene_generator.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     8525 2020-11-06 16:47:43.000000 stereoid-0.3.1/stereoid/oceans/sensitivity_distribution.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    19013 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/tc_scenario.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.665938 stereoid-0.3.1/stereoid/oceans/tools/
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/tools/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    24235 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/tools/backscatter_doppler_tools.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     5616 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/tools/observation_tools.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1945 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/tools/read_tools.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    10666 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/tools/retrieval_tools.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    12456 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/tools/scene_tools.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    32302 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/tools/spectrum_tools.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    26271 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/tools/wave_spectra_inversion_tools.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    21400 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/tools/write_tools.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    16918 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/tops_model.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.665938 stereoid-0.3.1/stereoid/oceans/visualization/
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/visualization/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    15673 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/visualization/geo_plot.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.666937 stereoid-0.3.1/stereoid/oceans/waves/
--rw-r--r--   0 andreas   (1000) andreas   (1000)    47591 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/waves/SceneGenerator_wavetrains.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/waves/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    19807 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/waves/high_resolution_var.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     3306 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/waves/spectral_conversions.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    33589 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/oceans/waves/wave_spectra.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.666937 stereoid-0.3.1/stereoid/polarimetry/
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/polarimetry/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    14801 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/polarimetry/pol_rotations.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.667938 stereoid-0.3.1/stereoid/sar_performance/
--rw-r--r--   0 andreas   (1000) andreas   (1000)      161 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/sar_performance/__init__.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)     3517 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/sar_performance/azimuth_performance.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)     3897 2021-06-29 13:50:14.000000 stereoid-0.3.1/stereoid/sar_performance/calc_rasr.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     6202 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/sar_performance/calc_sar_performance.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)     8568 2020-12-15 08:39:00.000000 stereoid-0.3.1/stereoid/sar_performance/casa_patterns.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2417 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/sar_performance/filestructure.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.668938 stereoid-0.3.1/stereoid/sea_ice/
--rw-r--r--   0 andreas   (1000) andreas   (1000)      333 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/sea_ice/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    19818 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/sea_ice/forward_model.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)    10232 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/sea_ice/image_processing.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    23099 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/sea_ice/performance.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    17217 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/sea_ice/radar_model.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1199 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/sea_ice/read_nextsim.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1694 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/sea_ice/retrieval_model.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    11191 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/sea_ice/scene_generator.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)    42757 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/sea_ice/ste_io.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.668938 stereoid-0.3.1/stereoid/tropical_cyclones/
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.669937 stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)     8753 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/California_wrappers.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)    13177 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/Doppler.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)     5810 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/RAR_model.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)    22121 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/SAR_model.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)    13403 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/backscatter.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)     1835 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/constants.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)    17572 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/high_resolution_var.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)     2638 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/polarimetry.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)    28741 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/scene_generator.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)    16893 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/wave_spectra.py
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)      164 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/tropical_cyclones/__init__.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.669937 stereoid-0.3.1/stereoid/utils/
--rw-r--r--   0 andreas   (1000) andreas   (1000)       73 2020-12-15 08:45:47.000000 stereoid-0.3.1/stereoid/utils/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     3501 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/utils/config.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    12401 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/utils/diffusion.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4898 2020-08-20 15:50:46.000000 stereoid-0.3.1/stereoid/utils/plot_helpers.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2006 2024-02-28 16:43:04.000000 stereoid-0.3.1/stereoid/utils/tools.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.670938 stereoid-0.3.1/stereoid.egg-info/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     3618 2024-03-26 09:09:16.000000 stereoid-0.3.1/stereoid.egg-info/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4649 2024-03-26 09:09:16.000000 stereoid-0.3.1/stereoid.egg-info/SOURCES.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2024-03-26 09:09:16.000000 stereoid-0.3.1/stereoid.egg-info/dependency_links.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)      245 2024-03-26 09:09:16.000000 stereoid-0.3.1/stereoid.egg-info/entry_points.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)      132 2024-03-26 09:09:16.000000 stereoid-0.3.1/stereoid.egg-info/requires.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)       65 2024-03-26 09:09:16.000000 stereoid-0.3.1/stereoid.egg-info/top_level.txt
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.669937 stereoid-0.3.1/test/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     6009 2024-02-28 16:43:04.000000 stereoid-0.3.1/test/plot_output.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-03-26 09:09:16.670938 stereoid-0.3.1/tests/
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2020-08-20 15:27:41.000000 stereoid-0.3.1/tests/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4484 2024-02-28 16:43:04.000000 stereoid-0.3.1/tests/test_config.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)      126 2022-04-08 11:54:19.000000 stereoid-0.3.1/tests/test_param.ini
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.699416 stereoid-0.4/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      700 2024-05-24 15:13:06.000000 stereoid-0.4/.gitignore
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    35149 2020-11-28 13:20:12.000000 stereoid-0.4/LICENSE
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       93 2024-05-24 15:53:02.000000 stereoid-0.4/MANIFEST.in
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     3616 2024-05-24 15:53:23.699416 stereoid-0.4/PKG-INFO
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     2434 2024-02-28 16:43:04.000000 stereoid-0.4/README.rst
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1520 2024-05-24 15:13:06.000000 stereoid-0.4/pyproject.toml
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       38 2024-05-24 15:53:23.699416 stereoid-0.4/setup.cfg
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.687416 stereoid-0.4/stereoid/
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)       70 2021-06-29 13:50:14.000000 stereoid-0.4/stereoid/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     7768 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/cli.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.688416 stereoid-0.4/stereoid/instrument/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      124 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/instrument/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    23072 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/instrument/dca_performance.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    31093 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/instrument/radar_model.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    16926 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/instrument/tops_model.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.689416 stereoid-0.4/stereoid/land_ice/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/land_ice/AASR_code.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     6571 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/land_ice/AASR_functions.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/land_ice/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      307 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/land_ice/back_scatter_model.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    26892 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/land_ice/coherence_model_SAR_stack.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     7206 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/land_ice/coherence_model_baseline_volume.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     5057 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/land_ice/deterministic_data.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/land_ice/forward_model.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    14626 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/land_ice/ice_polarimetry.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    11791 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/land_ice/line_of_sight_vectors_worldwide.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     7158 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/land_ice/phase_model.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     2310 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/land_ice/plot_SAR_vs_models.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     6358 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/land_ice/plot_functions.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/land_ice/radar_model.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/land_ice/retrieval_model.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    12008 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/land_ice/study_area_plots.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.690416 stereoid-0.4/stereoid/mission/
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)       70 2021-06-29 13:50:14.000000 stereoid-0.4/stereoid/mission/__init__.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)    14173 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/mission/acquisitions_script.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)    20327 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/mission/activation_analysis.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)     5927 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/mission/coverage.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)     9149 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/mission/formation_design.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.691416 stereoid-0.4/stereoid/oceans/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      245 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    78066 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/forward_model.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.692416 stereoid-0.4/stereoid/oceans/forward_models/
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.692416 stereoid-0.4/stereoid/oceans/forward_models/Deprecated/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/forward_models/Deprecated/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     2563 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/forward_models/Deprecated/polarimetry.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    44954 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/forward_models/Doppler.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    12859 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/forward_models/RIM_calibration.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     2376 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/forward_models/RIM_constants.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    77119 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/forward_models/SAR_spectra.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    26638 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/forward_models/SAR_spectra_broken.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/forward_models/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    34271 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/forward_models/backscatter.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    24240 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/forward_models/backscatter_doppler_tools.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     7476 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/forward_models/cdop.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     6415 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/forward_models/cmod5n.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    12267 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/forward_models/iwrap_backscatter.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     2398 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/forward_models/sea_state_bias.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    32316 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/forward_models/spectrum_tools.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    24789 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/forward_models/wrappers.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     2752 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/forward_models/zadelhoff_crosspol.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.693416 stereoid-0.4/stereoid/oceans/inversion/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     8128 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/inversion/RIM_inversion_deprecated.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/inversion/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    10663 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/inversion/retrieval_tools.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    29340 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/inversion/wave_spectra_inversion.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    26284 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/inversion/wave_spectra_inversion_tools.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.693416 stereoid-0.4/stereoid/oceans/io/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/io/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1945 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/io/read_tools.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    21400 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/io/write_tools.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     5401 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/l2_covariance.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     5036 2024-05-24 08:27:58.000000 stereoid-0.4/stereoid/oceans/profile_add_errors.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)     3848 2021-06-29 13:50:14.000000 stereoid-0.4/stereoid/oceans/read_fwd.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    41947 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/retrieval_model.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    18274 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/retrieval_performance.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    27354 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/run_scenario.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.694416 stereoid-0.4/stereoid/oceans/scene_preparation/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       95 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/scene_preparation/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     6451 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/scene_preparation/les.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     6897 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/scene_preparation/read_scenario_California.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    15265 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/scene_preparation/read_scenarios.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    11984 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/scene_preparation/scene_generator.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    12456 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/scene_preparation/scene_tools.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    19013 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/scene_preparation/tc_scenario.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     8556 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/sensitivity_distribution.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.694416 stereoid-0.4/stereoid/oceans/tools/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/tools/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     5490 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/tools/observation_tools.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.694416 stereoid-0.4/stereoid/oceans/visualization/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/visualization/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    15471 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/oceans/visualization/geo_plot.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.695416 stereoid-0.4/stereoid/oceans/waves/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    47591 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/waves/SceneGenerator_wavetrains.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/waves/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    19807 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/waves/high_resolution_var.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     3306 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/waves/spectral_conversions.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    33589 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/oceans/waves/wave_spectra.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.695416 stereoid-0.4/stereoid/polarimetry/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/polarimetry/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    38063 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/polarimetry/bistatic_pol.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    14801 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/polarimetry/pol_rotations.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.696416 stereoid-0.4/stereoid/sar_performance/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      161 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/sar_performance/__init__.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)     3517 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/sar_performance/azimuth_performance.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)     3897 2021-06-29 13:50:14.000000 stereoid-0.4/stereoid/sar_performance/calc_rasr.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     6202 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/sar_performance/calc_sar_performance.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)     8568 2020-12-15 08:39:00.000000 stereoid-0.4/stereoid/sar_performance/casa_patterns.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     2417 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/sar_performance/filestructure.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.697416 stereoid-0.4/stereoid/sea_ice/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      333 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/sea_ice/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    19818 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/sea_ice/forward_model.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)    10232 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/sea_ice/image_processing.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    23114 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/sea_ice/performance.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    17217 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/sea_ice/radar_model.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1199 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/sea_ice/read_nextsim.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1694 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/sea_ice/retrieval_model.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    11191 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/sea_ice/scene_generator.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)    42757 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/sea_ice/ste_io.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.697416 stereoid-0.4/stereoid/tropical_cyclones/
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.698416 stereoid-0.4/stereoid/tropical_cyclones/Deprecated/
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)     8758 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/tropical_cyclones/Deprecated/California_wrappers.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)    13177 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/tropical_cyclones/Deprecated/Doppler.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)     5810 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/tropical_cyclones/Deprecated/RAR_model.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)    22114 2024-05-24 15:13:06.000000 stereoid-0.4/stereoid/tropical_cyclones/Deprecated/SAR_model.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)    13403 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/tropical_cyclones/Deprecated/backscatter.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)     1835 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/tropical_cyclones/Deprecated/constants.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)    17572 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/tropical_cyclones/Deprecated/high_resolution_var.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)     2638 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/tropical_cyclones/Deprecated/polarimetry.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)    28741 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/tropical_cyclones/Deprecated/scene_generator.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)    16893 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/tropical_cyclones/Deprecated/wave_spectra.py
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)      164 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/tropical_cyclones/__init__.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.698416 stereoid-0.4/stereoid/utils/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       73 2020-12-15 08:45:47.000000 stereoid-0.4/stereoid/utils/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     3501 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/utils/config.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    12401 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/utils/diffusion.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     4898 2020-08-20 15:50:46.000000 stereoid-0.4/stereoid/utils/plot_helpers.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     2006 2024-02-28 16:43:04.000000 stereoid-0.4/stereoid/utils/tools.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.698416 stereoid-0.4/stereoid.egg-info/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     3616 2024-05-24 15:53:23.000000 stereoid-0.4/stereoid.egg-info/PKG-INFO
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     4825 2024-05-24 15:53:23.000000 stereoid-0.4/stereoid.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2024-05-24 15:53:23.000000 stereoid-0.4/stereoid.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      245 2024-05-24 15:53:23.000000 stereoid-0.4/stereoid.egg-info/entry_points.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      132 2024-05-24 15:53:23.000000 stereoid-0.4/stereoid.egg-info/requires.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       72 2024-05-24 15:53:23.000000 stereoid-0.4/stereoid.egg-info/top_level.txt
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-05-24 15:53:23.698416 stereoid-0.4/test/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     6009 2024-02-28 16:43:04.000000 stereoid-0.4/test/plot_output.py
```

### Comparing `stereoid-0.3.1/LICENSE` & `stereoid-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/PKG-INFO` & `stereoid-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stereoid
-Version: 0.3.1
+Version: 0.4
 Summary: The stereoid tools for the Harmony mission.
 Author-email: Paco Lopez Dekker <F.LopezDekker@tudelft.nl>, Andreas Theodosiou <a.theodosiou@tudelft.nl>, Marcel Kleinherenbrink <M.Kleinherenbrink@tudelft.nl>
 Project-URL: Repository, https://gitlab.tudelft.nl/drama/stereoid.git
 Project-URL: Bug Tracker, https://gitlab.tudelft.nl/drama/stereoid/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `stereoid-0.3.1/README.rst` & `stereoid-0.4/README.rst`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/pyproject.toml` & `stereoid-0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stereoid"
-version = "0.3.1"
+version = "0.4"
 dependencies = [
     "numba",
     "numpy",
     "scipy",
     "numexpr>=2.7",
     "netcdf4",
     "xarray",
```

### Comparing `stereoid-0.3.1/stereoid/cli.py` & `stereoid-0.4/stereoid/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,29 @@
 from pathlib import Path
 
 import numpy as np
 from drama.geo import QuickRadarGeometry
 
 import stereoid.utils.tools as tools
 import stereoid.oceans.run_scenario as run_scenario
-import stereoid.oceans.tools.write_tools as write_tools
+import stereoid.oceans.io.write_tools as write_tools
 
 
 def setup_arg_parser():
     parser = argparse.ArgumentParser()
-    parser.add_argument('params_file', nargs='?', type=str, default=None,
-                        help='Path of the parameters file')
-    parser.add_argument('--debug', action='store_true', default=False,
-                        help='Display debug log messages')
+    parser.add_argument(
+        "params_file",
+        nargs="?",
+        type=str,
+        default=None,
+        help="Path of the parameters file",
+    )
+    parser.add_argument(
+        "--debug", action="store_true", default=False, help="Display debug log messages"
+    )
     return parser
 
 
 def partition_swan():
     """
     Partitions the output of the SWAN model into a smaller dataset.
 
@@ -38,32 +44,37 @@
     main_logger.handlers = []
     handler = logging.StreamHandler()
     handler.setLevel(logging.DEBUG)
     main_logger.addHandler(handler)
     main_logger.setLevel(logging.INFO)
 
     parser = setup_arg_parser()
-    parser.add_argument('--partition', action='store_true', default=False,
-                        help='Partition the SWAN dataset according to the sizeaz and sizer parameters of the parameter file. If this flag is not set the entire SWAN dataset is read in memory and saved to disk as a netCDF file.')
+    parser.add_argument(
+        "--partition",
+        action="store_true",
+        default=False,
+        help="Partition the SWAN dataset according to the sizeaz and sizer parameters of the parameter file. If this "
+        "flag is not set the entire SWAN dataset is read in memory and saved to disk as a netCDF file.",
+    )
     args = parser.parse_args()
     if args.params_file is None:
-        main_logger.error('Please specify a parameter file')
+        main_logger.error("Please specify a parameter file")
         sys.exit(1)
     if args.debug is True:
         main_logger.setLevel(logging.DEBUG)
 
     file_param = args.params_file
     p = tools.load_python_file(file_param)
 
     # Read model Data and SWAN spectra
 
     try:
         run_scenario.run_partition_swan(p, args.partition)
     except KeyboardInterrupt:
-        main_logger.error('\nInterrupted by user (Ctrl+C)')
+        main_logger.error("\nInterrupted by user (Ctrl+C)")
         sys.exit(1)
     sys.exit(0)
 
 
 def run_harmony_fwd():
     """
     Run the scientific workbench for Harmony.
@@ -74,25 +85,25 @@
     handler.setLevel(logging.DEBUG)
     main_logger.addHandler(handler)
     main_logger.setLevel(logging.INFO)
 
     parser = setup_arg_parser()
     args = parser.parse_args()
     if args.params_file is None:
-        main_logger.error('Please specify a parameter file')
+        main_logger.error("Please specify a parameter file")
         sys.exit(1)
     if args.debug is True:
         main_logger.setLevel(logging.DEBUG)
 
     file_param = args.params_file
     p = tools.load_python_file(file_param)
     try:
         run_scenario.run_stereoid_fwd(p)  # , args.die_on_error)
     except KeyboardInterrupt:
-        main_logger.error('\nInterrupted by user (Ctrl+C)')
+        main_logger.error("\nInterrupted by user (Ctrl+C)")
         sys.exit(1)
     sys.exit(0)
 
 
 def compute_lut():
     """
     Run the scientific workbench for Harmony.
@@ -103,25 +114,25 @@
     handler.setLevel(logging.DEBUG)
     main_logger.addHandler(handler)
     main_logger.setLevel(logging.INFO)
 
     parser = setup_arg_parser()
     args = parser.parse_args()
     if args.params_file is None:
-        main_logger.error('Please specify a parameter file')
+        main_logger.error("Please specify a parameter file")
         sys.exit(1)
     if args.debug is True:
         main_logger.setLevel(logging.DEBUG)
 
     file_param = args.params_file
     p = tools.load_python_file(file_param)
     try:
         run_scenario.compute_lut(p)  # , args.die_on_error)
     except KeyboardInterrupt:
-        main_logger.error('\nInterrupted by user (Ctrl+C)')
+        main_logger.error("\nInterrupted by user (Ctrl+C)")
         sys.exit(1)
     sys.exit(0)
 
 
 def run_harmony_inv():
     """
     Run the scientific workbench for Harmony.
@@ -132,25 +143,25 @@
     handler.setLevel(logging.DEBUG)
     main_logger.addHandler(handler)
     main_logger.setLevel(logging.INFO)
 
     parser = setup_arg_parser()
     args = parser.parse_args()
     if args.params_file is None:
-        main_logger.error('Please specify a parameter file')
+        main_logger.error("Please specify a parameter file")
         sys.exit(1)
     if args.debug is True:
         main_logger.setLevel(logging.DEBUG)
 
     file_param = args.params_file
     p = tools.load_python_file(file_param)
     try:
         run_scenario.run_inversion(p)  # , args.die_on_error)
     except KeyboardInterrupt:
-        main_logger.error('\nInterrupted by user (Ctrl+C)')
+        main_logger.error("\nInterrupted by user (Ctrl+C)")
         sys.exit(1)
     sys.exit(0)
 
 
 def convert_to_netcdf():
     """
     Convert the pickled output of the scientific workbench to NETCDF format.
@@ -159,59 +170,78 @@
     main_logger.handlers = []
     handler = logging.StreamHandler()
     handler.setLevel(logging.DEBUG)
     main_logger.addHandler(handler)
     main_logger.setLevel(logging.INFO)
 
     parser = argparse.ArgumentParser()
-    parser.add_argument('input_file', type=str, default=None,
-                        help='Path of the pickled file')
-    parser.add_argument('params_file', nargs='?', type=str, default=None,
-                        help='Path of the parameters file')
-    parser.add_argument('--debug', action='store_true', default=False,
-                        help='Display debug log messages')
+    parser.add_argument(
+        "input_file", type=str, default=None, help="Path of the pickled file"
+    )
+    parser.add_argument(
+        "params_file",
+        nargs="?",
+        type=str,
+        default=None,
+        help="Path of the parameters file",
+    )
+    parser.add_argument(
+        "--debug", action="store_true", default=False, help="Display debug log messages"
+    )
     args = parser.parse_args()
     if args.input_file is None:
-        main_logger.error('Please specify a pickle file')
+        main_logger.error("Please specify a pickle file")
         sys.exit(1)
     if args.debug is True:
         main_logger.setLevel(logging.DEBUG)
     input_path = Path(args.input_file).expanduser()
     if args.params_file:
         p = tools.load_python_file(args.params_file)
         run_scenario.make_default(p)
         run_scenario.make_default_fwd(p)
         output_path = f"{p.obs_file}.nc"
     else:
         p = None
         output_path = input_path.with_suffix(".nc")
     with open(input_path, "rb") as f:
         result = pickle.load(f)
-        qgeo = QuickRadarGeometry(693E3, degrees=False)
+        qgeo = QuickRadarGeometry(693e3, degrees=False)
         gr_v = qgeo.inc_to_gr(result["inc_m"])
-        dic_geometry = {"inc": np.stack((result["inc_m"][0],
-                                         result["inc_b_c"][0],
-                                         result["inc_b_d"][0]), axis=-1),
-                    "bist_ang": np.stack((np.zeros_like(result["bist_ang_c"][0]),
-                                          result["bist_ang_c"][0],
-                                          result["bist_ang_d"][0]), axis=-1),
-                    "grg": gr_v[0],
-                    "az": np.arange(0, result["model"]["sst"].shape[0], 1) *result["model"]["dy"],
-                    }
+        dic_geometry = {
+            "inc": np.stack(
+                (result["inc_m"][0], result["inc_b_c"][0], result["inc_b_d"][0]),
+                axis=-1,
+            ),
+            "bist_ang": np.stack(
+                (
+                    np.zeros_like(result["bist_ang_c"][0]),
+                    result["bist_ang_c"][0],
+                    result["bist_ang_d"][0],
+                ),
+                axis=-1,
+            ),
+            "grg": gr_v[0],
+            "az": np.arange(0, result["model"]["sst"].shape[0], 1)
+            * result["model"]["dy"],
+        }
         # The old pickled output have dimensions called "lon" and "lat" but
         # save_scene expects "longitude" and "latitude"
         vars_to_rename = {"lon": "longitude", "lat": "latitude"}
         for key in vars_to_rename:
             if key in result["model"]:
                 result["model"][vars_to_rename[key]] = result["model"].pop(key)
         if "sar" in input_path.name:
             for key in dic_geometry:
-                dic_geometry[key] = dic_geometry[key][::p.spec_samp[1]]
+                dic_geometry[key] = dic_geometry[key][:: p.spec_samp[1]]
             if result["model"]["latitude"].shape != result["imacs"]["HA"]["M"].shape:
                 for item in vars_to_rename.items():
-                    result["model"][item] = result["model"][item][::p.spec_samp[0], ::p.spec_samp[1]]
+                    result["model"][item] = result["model"][item][
+                        :: p.spec_samp[0], :: p.spec_samp[1]
+                    ]
             result |= dic_geometry
-            write_tools.save_scene(output_path, ("imacs", "cut_off"), result, global_attr=p)
+            write_tools.save_scene(
+                output_path, ("imacs", "cut_off"), result, global_attr=p
+            )
         else:
             result |= dic_geometry
             write_tools.save_scene(output_path, ("nrcs", "dop"), result, global_attr=p)
     sys.exit(0)
```

### Comparing `stereoid-0.3.1/stereoid/land_ice/AASR_functions.py` & `stereoid-0.4/stereoid/land_ice/AASR_functions.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/land_ice/coherence_model_SAR_stack.py` & `stereoid-0.4/stereoid/land_ice/coherence_model_SAR_stack.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/land_ice/coherence_model_baseline_volume.py` & `stereoid-0.4/stereoid/land_ice/coherence_model_baseline_volume.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/land_ice/deterministic_data.py` & `stereoid-0.4/stereoid/land_ice/deterministic_data.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/land_ice/ice_polarimetry.py` & `stereoid-0.4/stereoid/land_ice/ice_polarimetry.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/land_ice/line_of_sight_vectors_worldwide.py` & `stereoid-0.4/stereoid/land_ice/line_of_sight_vectors_worldwide.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from drama.performance.sar import SARModeFromCfg
 from drama.io import cfg
 from drama.mission.timeline import LatLonTimeline
 
 
 class LOSVectors():
 
-    def __init__(self):
+    def __init__(self, run_id = "2021_1"):
         # Set up radar parameters
         # Change the second parameter of `SARModeFromCfg` to the acquisition mode of interest: `"EW"`, `"WM"`, `"stripmap"`.
 
         config = st_config.parse()
-        run_id = "2020_1"
+        
         self.par_file = config["par"] / f"Hrmny_{run_id}.cfg"
         self.mode = SARModeFromCfg(cfg.ConfigFile(self.par_file), "IWS")
 
     def interpolate_satellite_orbits(self, min_lat=-90, max_lat=85, orbit_resolution=0.05):
         """
         Apply the actual interpolation of the orbits.
```

### Comparing `stereoid-0.3.1/stereoid/land_ice/phase_model.py` & `stereoid-0.4/stereoid/land_ice/phase_model.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/land_ice/plot_SAR_vs_models.py` & `stereoid-0.4/stereoid/land_ice/plot_SAR_vs_models.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/land_ice/plot_functions.py` & `stereoid-0.4/stereoid/land_ice/plot_functions.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/land_ice/study_area_plots.py` & `stereoid-0.4/stereoid/land_ice/study_area_plots.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/mission/acquisitions_script.py` & `stereoid-0.4/stereoid/mission/acquisitions_script.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/mission/activation_analysis.py` & `stereoid-0.4/stereoid/mission/activation_analysis.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/mission/coverage.py` & `stereoid-0.4/stereoid/mission/coverage.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/mission/formation_design.py` & `stereoid-0.4/stereoid/mission/formation_design.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/GMF/IWRAP_backscatter.py` & `stereoid-0.4/stereoid/oceans/forward_models/iwrap_backscatter.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/GMF/Zadelhoff_crosspol.py` & `stereoid-0.4/stereoid/oceans/forward_models/zadelhoff_crosspol.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/GMF/cdop.py` & `stereoid-0.4/stereoid/oceans/forward_models/cdop.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/GMF/cmod5n.py` & `stereoid-0.4/stereoid/oceans/forward_models/cmod5n.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/bistatic_pol.py` & `stereoid-0.4/stereoid/polarimetry/bistatic_pol.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/dca_performance.py` & `stereoid-0.4/stereoid/instrument/dca_performance.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 __email__ = "F.LopezDekker@tudeft.nl"
 
 import numpy as np
 import scipy.interpolate as interp
 from matplotlib import pyplot as plt
 import matplotlib
 import drama.performance.doppler_centroid as doppler_centroid
-import stereoid.oceans.cmod5n as cmod5
+import stereoid.oceans.forward_models.cmod5n as cmod5
 import drama.constants as cnst
 # import drama.geo.geometry as sargeo
 from drama.orbits import orbit_to_vel
 import os
 import drama.performance.insar as insar
 from drama.performance import sar as sar
```

### Comparing `stereoid-0.3.1/stereoid/oceans/forward_model.py` & `stereoid-0.4/stereoid/oceans/forward_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 import os
 
 import numpy as np
 import xarray as xr
 from matplotlib import pyplot as plt
 from netCDF4 import Dataset
-from scipy.ndimage.interpolation import map_coordinates as spmp
+from scipy.ndimage import map_coordinates as spmp
 
 import drama.utils as drtls
-from stereoid.oceans import ObsGeo
+from stereoid.instrument import ObsGeo
 
 
 def ind_clip(ind, n):
     if type(ind) is np.ndarray:
         ind = np.where(ind > 0, ind, 0)
         ind = np.where(ind > (n - 1), n - 1, ind)
         return ind
```

### Comparing `stereoid-0.3.1/stereoid/oceans/forward_models/Deprecated/polarimetry.py` & `stereoid-0.4/stereoid/oceans/forward_models/Deprecated/polarimetry.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/forward_models/Doppler.py` & `stereoid-0.4/stereoid/oceans/forward_models/Doppler.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/forward_models/RIM_calibration.py` & `stereoid-0.4/stereoid/oceans/forward_models/RIM_calibration.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/forward_models/RIM_constants.py` & `stereoid-0.4/stereoid/oceans/forward_models/RIM_constants.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/forward_models/SAR_spectra.py` & `stereoid-0.4/stereoid/oceans/forward_models/SAR_spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 __author__ = "Marcel Kleinherenbrink"
 __email__ = "M.Kleinherenbrink@tudelft.nl"
 
-import stereoid.oceans.GMF.cmod5n as cmod5n
+import stereoid.oceans.forward_models.cmod5n as cmod5n
 import numpy as np
 import math
 import copy
-from typing import Optional, Tuple
+from typing import Optional
 from scipy.optimize import curve_fit
 from stereoid.oceans.waves.wave_spectra import tuning_param_wb
 from stereoid.oceans.forward_models.RIM_constants import constants as co
 from stereoid.oceans.forward_models.Doppler import tilt_transfer_func
 from stereoid.oceans.waves.wave_spectra import elfouhaily
 from stereoid.oceans.waves.wave_spectra import elfouhaily_spread
-from stereoid.oceans.bistatic_pol import elfouhaily_coefficient
+from stereoid.polarimetry.bistatic_pol import elfouhaily_coefficient
 from stereoid.oceans.forward_models.wrappers import (
     interp_weights as griddata_step1,
     interpolate as griddata_step2,
 )
-from stereoid.oceans.radar_model import SpectralNoiseModel
+from stereoid.instrument.radar_model import SpectralNoiseModel
 import stereoid.oceans.forward_models.wrappers as wrappers
-from stereoid.oceans import ObsGeoAngles
+from stereoid.instrument import ObsGeoAngles
 from stereoid.polarimetry import pol_rotations as polrot
 import stereoid.oceans.tools.observation_tools as obs_tools
 from stereoid.oceans.forward_models.backscatter import backscatter_Kudry2023
 from stereoid.oceans.forward_models.backscatter import backscatter_Kudry2023_polar
 import logging
 
 logger = logging.getLogger(__name__)
```

### Comparing `stereoid-0.3.1/stereoid/oceans/forward_models/SAR_spectra_broken.py` & `stereoid-0.4/stereoid/oceans/forward_models/SAR_spectra_broken.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 __author__ = "Marcel Kleinherenbrink"
 __email__ = "M.Kleinherenbrink@tudelft.nl"
 
-import stereoid.oceans.GMF.cmod5n as cmod5n
-import numpy as np
+import stereoid.oceans.forward_models.cmod5n as cmod5n
 import math
 
 
 # Implementation of Engen and Johnsen (1995)
 # This works with linear spacing in kx and ky, maybe we have to change this
 # I will make another function for a log-scale spacing
 def corr_func(S, kx, ky, mu=0.5, theta=35, R=850E3, V=7000, mtf='Schulz',
@@ -37,16 +36,16 @@
     T_y[ T_y != T_y ] = 0
     T_I = np.zeros( k.shape )
     if mtf == 'Schulz':
         T_I = -1j * 4 * kx / (np.tan( theta ) * (1 + np.sin( theta ) ** 2)) - 1j * kx / np.tan(
             theta ) + 4.5 * omega * kx ** 2 * (omega - 1j * mu) / (k * (omega ** 2 + mu ** 2))
     if mtf == 'S1':
         dth = 0.001
-        sigma = cmod5n.cmod5n_forward( np.array( [ ws, ws ] ), np.array( [ phi_w, phi_w ] ),
-                                       np.rad2deg( np.array( [ theta, theta + dth ] ) ) )  # use CMOD5n here
+        sigma = cmod5n.cmod5n_forward(np.array([ws, ws]), np.array([phi_w, phi_w]),
+                                      np.rad2deg( np.array( [ theta, theta + dth ] ) ))  # use CMOD5n here
         dsigma = (sigma[ 1 ] - sigma[ 0 ]) / dth
         T_I = kx * dsigma / sigma[ 0 ] / np.cos( theta ) * (
                 kx / k * np.sin( theta ) + 1j * np.cos( theta ))  # combination of both equations (37)
     T_I[ T_I != T_I ] = 0
 
     # cross-spectral functions
     N_II_pos = 0.5 * T_I * np.conj( T_I )
@@ -206,16 +205,16 @@
         # I guss that (kx * np.cos( alpha / 2 ) - ky * np.sin( alpha / 2 )) ** 2 has to be scaled with np.cos( alpha / 2 )
         # and k also
         T_I = -1j * 4 * k_l / (np.tan( theta_m ) * (1 + np.sin( theta_m ) ** 2)) - 1j * k_l / np.tan(
             theta_m ) + 4.5 * omega * k_l ** 2 * (omega - 1j * mu) / (k * (omega ** 2 + mu ** 2))
     if mtf == 'S1':
         # FIXME I guess this k_l should be like below, but this should be rigorously checked
         dth = 0.001
-        sigma = cmod5n.cmod5n_forward( np.array( [ ws, ws ] ), np.array( [ phi_w, phi_w ] ),
-                                       np.rad2deg( np.array( [ theta_m, theta_m + dth ] ) ) )  # use CMOD5n here
+        sigma = cmod5n.cmod5n_forward(np.array([ws, ws]), np.array([phi_w, phi_w]),
+                                      np.rad2deg( np.array( [ theta_m, theta_m + dth ] ) ))  # use CMOD5n here
         dsigma = (sigma[ 1 ] - sigma[ 0 ]) / dth
         T_I = k_l * dsigma / sigma[ 0 ] / np.cos( theta_m ) * (
                 k_l / k * np.sin( theta_m ) + 1j * np.cos( theta_m ))  # combination of both equations (37)
 
     T_x[ T_x != T_x ] = 0
     T_y[ T_y != T_y ] = 0
     T_I[ T_I != T_I ] = 0
```

### Comparing `stereoid-0.3.1/stereoid/oceans/forward_models/backscatter.py` & `stereoid-0.4/stereoid/oceans/forward_models/backscatter.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/forward_models/sea_state_bias.py` & `stereoid-0.4/stereoid/oceans/forward_models/sea_state_bias.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/forward_models/wrappers.py` & `stereoid-0.4/stereoid/oceans/forward_models/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 Author: Marcel Kleinherenbrink
 """
-from typing import Optional, Tuple
+from typing import Optional
 import numpy as np
-import scipy as sp
 import stereoid.oceans.forward_models.backscatter as backscatter
 from stereoid.oceans.forward_models.backscatter import backscatter_Kudry2023, backscatter_Kudry2023_polar
 from stereoid.oceans.forward_models.Doppler import DopRIM, DopRIM_DP, DopRIM2023_DP, DopRIM2023_DP_polar
-from stereoid.oceans.bistatic_pol import elfouhaily as Elf_pol
-import scipy.spatial.qhull as qhull
+from stereoid.polarimetry.bistatic_pol import elfouhaily as Elf_pol
+from scipy.spatial import Delaunay
 from matplotlib import pyplot as plt
 
 LIST_MONO = ['Bragg', 'specular', 'wave_breaking', 'wave_breaking_cross']
 LIST_BI =['Bragg', 'specular', 'wave_breaking', 'Bragg_cross',
           'specular_cross', 'wave_breaking_cross']
 LIST_BI_DOP = ['Bragg_hh','Bragg_vv', 'specular', 'wave_breaking', 'Bragg_cross',
                'specular_cross', 'wave_breaking_cross']
@@ -429,15 +428,15 @@
             'wave_breaking_cross': db1_wbcr}
 
     return s_me, d_bi
 
 # this breaks up the griddata interpolator to get indices
 # got this from: https://stackoverflow.com/questions/20915502/speedup-scipy-griddata-for-multiple-interpolations-between-two-irregular-grids
 def interp_weights(xy, uv,d=2):
-    tri = qhull.Delaunay(xy)
+    tri = Delaunay(xy)
     simplex = tri.find_simplex(uv)
     vertices = np.take(tri.simplices, simplex, axis=0)
     temp = np.take(tri.transform, simplex, axis=0)
     delta = uv - temp[:, d]
     bary = np.einsum('njk,nk->nj', temp[:, :d, :], delta)
     return vertices, np.hstack((bary, 1 - bary.sum(axis=1, keepdims=True)))
 
@@ -579,8 +578,8 @@
     db1_spcr = rat[ 0 ] * (c_sp_bar + c_sp)
     db1_brcr = rat[ 1 ] * (c_br_bar + c_br)
     db1_wbcr = rat[ 2 ] * (c_wb_bar + c_wb)
     d_bi = {'Bragg': db1_br, 'specular': db1_sp, 'wave_breaking': db1_wb,
             'Bragg_cross': db1_brcr, 'specular_cross': db1_spcr,
             'wave_breaking_cross': db1_wbcr}
 
-    return s_bi, d_bi
+    return s_bi, d_bi
```

### Comparing `stereoid-0.3.1/stereoid/oceans/inversion/RIM_inversion_deprecated.py` & `stereoid-0.4/stereoid/oceans/inversion/RIM_inversion_deprecated.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/inversion/wave_spectra_inversion.py` & `stereoid-0.4/stereoid/oceans/inversion/wave_spectra_inversion.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/l2_covariance.py` & `stereoid-0.4/stereoid/oceans/l2_covariance.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     """
 
     def __init__(self, radar_model, inc_master_d, forward_model):
         """Initialise L2Cov. Extract the nrcs and jacobian from the forward_model
 
         Parameters
         ----------
-        radar_model : stereoid.oceans.radar_model.RadarModel
+        radar_model : stereoid.instrument.radar_model.RadarModel
             The radar model for which to compute the covariance matrices. Holds information regarding the geometry and NESZ.
 
         inc_master_d : float
             Incidence angle of the master satellite. Covariance matrices are computed for this angle. [degree]
 
         forward_model : stereoid.oceans.forward_model.FwdModel
             The forward model relating the NRCS to wind speeds.
```

### Comparing `stereoid-0.3.1/stereoid/oceans/les.py` & `stereoid-0.4/stereoid/oceans/scene_preparation/les.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,17 @@
     ur = u * np.cos(np.radians(angle)) + v * np.sin(np.radians(angle))
     vr = - u * np.sin(np.radians(angle)) + v * np.cos(np.radians(angle))
     return ur, vr
 
 
 #%%
 if __name__ == '__main__':
-    from stereoid.oceans import FwdModel, SceneGenerator, RetrievalModel
-    from stereoid.oceans import ObsGeo, RadarModel
+    from stereoid.oceans import FwdModel, RetrievalModel
+    from stereoid.oceans.scene_preparation import SceneGenerator
+    from stereoid.instrument import ObsGeo, RadarModel
     import stereoid.sar_performance as strsarperf
     import stereoid.utils.config as st_config
     from drama import geo as sargeo
     paths = st_config.parse(section="Paths")
     main_dir = paths["main"]
     datadir = paths["data"]
     pardir = paths["par"]
```

### Comparing `stereoid-0.3.1/stereoid/oceans/profile_add_errors.py` & `stereoid-0.4/stereoid/oceans/profile_add_errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from scipy.interpolate import CubicSpline
 import xarray as xr
 import drama.io.cfg as cfg
 import drama.geo.geometry as d_geo
 import drama.geo.swath_geo as d_swath_geo
 import drama.constants as d_constants
 
-from stereoid.oceans.radar_model import ObsGeo, RadarModel
+from stereoid.instrument.radar_model import ObsGeo
 from stereoid.oceans.tops_model import TopsModel
 import stereoid.utils.config as st_config
 import stereoid.sar_performance as sar_perf
 
 
 def get_burst(subswath, burst_nr):
     burst_beginning = az_start + ((burst_nr - 1) * (burst_length - overlap_length))
```

### Comparing `stereoid-0.3.1/stereoid/oceans/radar_model.py` & `stereoid-0.4/stereoid/instrument/radar_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import scipy.interpolate as interp
 
 import drama.utils as drtls
 from drama.performance.sar import NESZdata
 import drama.geo as geo
 from drama.geo import QuickRadarGeometry
 from drama.geo.derived_geo import BistaticRadarGeometry
-from stereoid.oceans import ATIPerf, DCAPerf
+from stereoid.instrument import ATIPerf, DCAPerf
 
 
 __author__ = "Paco Lopez Dekker"
 __email__ = "F.LopezDekker@tudeft.nl"
 # Define logger level for debug purposes
 logger = logging.getLogger(__name__)
 T = TypeVar("T")
```

### Comparing `stereoid-0.3.1/stereoid/oceans/read_fwd.py` & `stereoid-0.4/stereoid/oceans/read_fwd.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/read_scenario_California.py` & `stereoid-0.4/stereoid/oceans/scene_preparation/read_scenario_California.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/retrieval_model.py` & `stereoid-0.4/stereoid/oceans/retrieval_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional, Tuple
 
 from numba import njit
 from drama import constants as cnst
 import drama.utils as drtls
 
 # import stereoid.utils.tools as tools
-from stereoid.oceans import ObsGeo
+from stereoid.instrument import ObsGeo
 from stereoid.oceans.forward_model import ind_clip
 
 __author__ = "Paco Lopez Dekker"
 __email__ = "F.LopezDekker@tudeft.nl"
 
 # %% RetrievalModel class
 G = 9.81
@@ -866,15 +866,16 @@
                                      np.sin(inc_b_r_a) * np.sin(bist_ang_r_a)])
         return a
 
 
 # %% End of class
 if __name__ == '__main__':
     # %% Prepare....
-    from stereoid.oceans import FwdModel, SceneGenerator
+    from stereoid.oceans import FwdModel
+    from stereoid.oceans.scene_preparation import SceneGenerator
     datadir = "/Users/plopezdekker/Documents/WORK/STEREOID/DATA/ScatteringModels/Oceans"
     fname = "C_band_nrcs_dop_ocean_simulation.nc"
     fnameisv = "C_band_isv_ocean_simulation.nc"
     obsgeo = ObsGeo(35, 36, 40)
     # %% Forward model, this takes some time
     fwdm = FwdModel(datadir, os.path.join(datadir, fnameisv),
                     dspd=2, duvec=0.25)
```

### Comparing `stereoid-0.3.1/stereoid/oceans/retrieval_performance.py` & `stereoid-0.4/stereoid/oceans/retrieval_performance.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 # from matplotlib import rc
 # rc('text', usetex=False)
 
 import drama.geo as sargeo
 from drama.io import cfg
 from drama.performance.sar import NESZdata
 import stereoid.sar_performance as strsarperf
-from stereoid.oceans import ObsGeo, FwdModel, RadarModel, RetrievalModel,FwdModelRIM
+from stereoid.oceans import FwdModel, RetrievalModel,FwdModelRIM
+from stereoid.instrument import ObsGeo, RadarModel
 from drama.geo.derived_geo import BistaticRadarGeometry
 
 # %%
 class RetrievalPerformance(object):
     """Class to compute wind and TSC retirieval performance."""
 
     def __init__(self, maindir, run_id, parfile, fwd_model, d_at=350e3, prod_res=2e3, mode="IWS",
```

### Comparing `stereoid-0.3.1/stereoid/oceans/run_scenario.py` & `stereoid-0.4/stereoid/oceans/run_scenario.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import os
 import logging
 import pickle
 
-import numpy
+import numpy as np
 import xarray as xr
 from scipy.signal import convolve2d
 from scipy.ndimage import median_filter
-#from scipy.interpolate import RBFInterpolator
 import drama.utils.resample as dr_resample
 
-import stereoid.oceans.read_scenario_California as read_scenario_California
-import stereoid.oceans.read_scenarios as read_scenarios
-import stereoid.oceans.tools.scene_tools as scene_tools
-import stereoid.oceans.tools.spectrum_tools as spectrum_tools
-import stereoid.oceans.tools.backscatter_doppler_tools as bkscatter_doppler
+import stereoid.oceans.scene_preparation.read_scenario_California as read_scenario_California
+import stereoid.oceans.scene_preparation.read_scenarios as read_scenarios
+import stereoid.oceans.scene_preparation.scene_tools as scene_tools
+import stereoid.oceans.forward_models.spectrum_tools as spectrum_tools
+import stereoid.oceans.forward_models.backscatter_doppler_tools as bkscatter_doppler
 import stereoid.oceans.tools.observation_tools as obs_tools
-import stereoid.oceans.tools.write_tools as write_tools
-import stereoid.oceans.tools.read_tools as read_tools
+import stereoid.oceans.io.write_tools as write_tools
+import stereoid.oceans.io.read_tools as read_tools
 
 # Define logger level for debug purposes
 logger = logging.getLogger(__name__)
 logging.getLogger('numba').setLevel(logging.WARNING)
 
 
 def tolist(x):
@@ -65,14 +64,15 @@
 
     # SAR spectrum parameters
     p.SAR_spectra_lambda_max = getattr(p, "SAR_spectra_lambda_max", 2000)
     p.spec_samp = tolist(getattr(p, 'spec_samp', [10, 10]))
     if len(p.spec_samp) < 2:
         p.spec_samp = [p.spec_samp[0], p.spec_samp[0]]
     p.SAR_spectra_looks = getattr(p, "SAR_spectra_looks", 25)
+    p.SAR_spectra_noise = getattr(p, "SAR_spectra_noise", True)
 
     # Output parameters
     p.main_out = getattr(p, 'main_out', './')
     p.obs_nonoise_file = getattr(p, 'obs_nonoise_file', 'default_harmony')
     p.obs_file = getattr(p, 'obs_file', 'default_harmony')
     lvariable = ["Doppler", "Backscatter", "imacs", "cut_off"]
     p.list_variable = getattr(p, 'list_variable', lvariable)
@@ -126,70 +126,76 @@
 
 
 def run_stereoid_fwd(par):
     logger.info("Build observation and geometry")
     make_default(par)
     make_default_fwd(par)
     # Observation geometry
-    incident = numpy.deg2rad(par.incident_angle)
+    # FIXME this should be called the near range incidence angle, or something like that.
+    incident = np.deg2rad(par.incident_angle)
     obs_geo = obs_tools.build_geometry(par.parfile, incident, dau=par.dau)
 
     # Observation Performance
     fstr_dual, fstr_ati, fstr_s1 = obs_tools.build_performance_file(par)
 
     # Read model Data and SWAN spectra
     logger.info("Read model Data")
     sizeaz = par.sizeaz
     sizer = par.sizer
     rot_angle = par.rot_angle
     model_readers = {"California" : read_scenario_California.read_scenario_California,
-                     "DALES": read_scenarios.read_scenario_DALES_KNMI}
+                     "DALES": read_scenarios.read_scenario_DALES_KNMI,
+                     "Ifremer": read_scenarios.read_scenario_ifremer} 
     model, _ = scene_tools.read_scene(par.scn_file, (sizeaz, sizer),
                                       model_readers[par.model_reader], rot_angle,
                                       l1_resolution=par.l1_resolution)
     model_shape = model["sst"].shape
+    # FIXME We need to read WWIII spectra where available
     if par.read_from_netcdf:
         swan_nc_file = scene_tools.construct_swan_filepath(
             par.swan_file, par.swan_dir, sizeaz, sizer
         )
-        logger.info(f"Read SWAN spectra from netCDF file at {par.swan_as_nc}")
+        logger.info(f"Read SWAN spectra from netCDF file at {swan_nc_file}")
         ws = xr.open_dataset(swan_nc_file)
     else:
-        logger.info("Read SWAN spectra from SWAN model.")
+        logger.info(f"Read SWAN spectra from SWAN model at {par.swan_file}.")
         ws = scene_tools.read_swan_spectra(par.swan_file, sizeaz, sizer,
                                            par.swan_as_nc, rot_angle)
-        ind = numpy.isnan(ws['efth'][0, :, 0, 0].values)
+        ind = np.isnan(ws['efth'][0, :, 0, 0].values)
         ws['efth'][0, ind, :, :] = ws['efth'][0, 0, :, :]
         # find the index of the first element that is not nan
         not_nan_index = (~ind).nonzero()[0][0]
         # nonzero returns a tuple of an array so index twice
         ws['efth'][0, ind, :, :] = ws['efth'][0, not_nan_index, :, :]
     # adjust observation geometry to match the width of model's swath
     shp1 = model_shape[1]
-    _spac = numpy.arange(shp1).reshape((1, shp1)) * model["dx"]
+    _spac = np.arange(shp1).reshape((1, shp1)) * model["dx"]
     # set_swath modifies the properties of obs_geo!
     obs_geo.concordia.set_swath(incident, _spac)
     obs_geo.discordia.set_swath(incident, _spac)
 
     # Spectrum for short waves
     logger.info("Spectrum for short waves")
+    # The next line computes the transfer functions that will be used later to  model
+    # the effect of surface currrent gradients and wind variations on the small waves
+    # with some assumptions (transfer functions computed on mean wind)
     mod_transfer, wn = spectrum_tools.spectrum_short_waves_swan(
         model, par.lambda_min, par.lambda_max, par.n_k, fetch=par.fetch
     )
 
     # Polarimetric bistatics backscatter and Doppler
-    dic_geometry = {"inc": numpy.stack((obs_geo.concordia.inc_m[0],
+    dic_geometry = {"inc": np.stack((obs_geo.concordia.inc_m[0],
                                         obs_geo.concordia.inc_b[0],
                                         obs_geo.discordia.inc_b[0]), axis=-1),
-                    "bist_ang": numpy.stack((numpy.zeros_like(obs_geo.concordia.bist_ang[0]),
+                    "bist_ang": np.stack((np.zeros_like(obs_geo.concordia.bist_ang[0]),
                                              obs_geo.concordia.bist_ang[0],
                                              obs_geo.discordia.bist_ang[0]),
                                             axis=-1),
                     "grg": obs_geo.concordia.gr[0],
-                    "az": numpy.arange(0, model_shape[0], 1) * model["dy"],
+                    "az": np.arange(0, model_shape[0], 1) * model["dy"],
                     }
     if any(item in par.list_variable for item in ("Doppler", "Backscatter")):
         logger.info("Polarimetrics backscatter and Doppler")
         _res = bkscatter_doppler.backscatter_doppler(
             ws,
             model,
             obs_geo,
@@ -230,50 +236,65 @@
             # consider both geometries for the noise?
             dgeom = {
                 "obs_geo": obs_geo.concordia,
                 "fstr_dual": fstr_dual,
                 "fstr_ati": fstr_ati,
                 "fstr_s1": fstr_s1,
             }
+            # FIXME: this is initialiting the radar model and running it;
+            # that should not be in forward_models. 
             nrcsd_o, dopd_o, isv_o, dgeom = bkscatter_doppler.add_noise(
                 nrcsd, dopd, model["dx"], par, dic_geom=dgeom
             )
 
             dic_final["nrcs"] = nrcsd_o
             dic_final["dop"] = dopd_o
 
-        nfile = f"{par.obs_file}.pyo"
-        with open(nfile, "wb") as pf:
-            pickle.dump(dic_final, pf)
-        nfile = f"{par.obs_file}.nc"
-        write_tools.save_scene(nfile, ("nrcs", "dop"), dic_final,
-                               global_attr=par)
-        _str = "\nSaved the NRCS and Doppler with noise"
-        logger.info(f"{_str} in:\n{os.path.dirname(nfile)}.\n")
+            nfile = f"{par.obs_file}.pyo"
+            with open(nfile, "wb") as pf:
+                pickle.dump(dic_final, pf)
+            nfile = f"{par.obs_file}.nc"
+            write_tools.save_scene(nfile, ("nrcs", "dop"), dic_final,
+                                   global_attr=par)
+            _str = "\nSaved the NRCS and Doppler with noise"
+            logger.info(f"{_str} in:\n{os.path.dirname(nfile)}.\n")
         # Save model data in netcdf
         nfile = f'{par.obs_file}_model.nc'
         par.description = "Model interpolated on swath"
         dicm = {}
         list_model_key = ("longitude", "latitude", "sst", "tsc_v", "tsc_u", "wnd_u",
                           "wnd_v")
         for key in list_model_key:
             dicm[key] = dic_final["model"][key]
             write_tools.save_L2(nfile, dicm, global_attr=par)
     dic_geometry_s = {}
     for key in dic_geometry.keys():
         dic_geometry_s[key] = dic_geometry[key][::par.spec_samp[1]]
     # Polarimetric SAR co-spectra, cross-spectra imacs and cut_off
     if any(item in par.list_variable for item in ("imacs", "cut_off")):
-        logger.info("SAR co-spectra, cross-spectra, Emacs and Cut Off")
+        logger.info("SAR co-spectra, cross-spectra, iMACS and Cut Off")
         _msar = spectrum_tools.make_SAR_spectra
-        _specres = _msar(ws, model, obs_geo, mod_transfer, wn, par.spec_samp,
-                         par.SAR_spectra_lambda_max, par.SAR_spectra_looks,
-                         pol=par.txpol, rxpol=par.rxpolbase, swell=False,
-                         spec_type=par.spec_type_imacs_cutoff,
-                         fetch=par.fetch, k_l=par.k_l, progress_bar=True)
+        _specres = _msar(
+            ws,
+            model,
+            obs_geo,
+            mod_transfer,
+            wn,
+            par.spec_samp,
+            par.SAR_spectra_lambda_max,
+            par.SAR_spectra_looks,
+            pol=par.txpol,
+            rxpol=par.rxpolbase,
+            swell=False,
+            spec_type=par.spec_type_imacs_cutoff,
+            fetch=par.fetch,
+            k_l=par.k_l,
+            noise=par.SAR_spectra_noise,
+            progress_bar=True,
+        )
         for key in ("longitude", "latitude"):
             model[key] = _specres[5][key]
         dic_final = {"wn": wn, "model": model, "cospectrum": _specres[0],
                      "cross-spectrum": _specres[1],
                      "imacs": _specres[2], "cut_off": _specres[3]}
         dic_final |= dic_geometry_s
         nfile = f"{par.obs_file}_sar.pyo"
@@ -312,15 +333,15 @@
     make_default(par)
     make_default_lut(par)
     THREADS = par.nprocessor
     pool = multiprocessing.Pool(THREADS)
 
     logger.info("Build observation and geometry")
     # Observation geometry
-    incident = numpy.deg2rad(par.incident_angle)
+    incident = np.deg2rad(par.incident_angle)
     obs_geo = obs_tools.build_geometry(par.parfile, incident,
                                        dau=par.dau)
 
     logger.debug("Prepare jobs")
 
     # Specification for the case of the LUT:
     range_length, nb_points = par.lut_incidence_range
@@ -328,18 +349,18 @@
                       "progress_bar", "obs_nonoise_file", "main_out",
                       "save_iwa", "spec_samp", "list_variable",
                       "SAR_spectra_lambda_max", "SAR_spectra_looks", "k_l"]
     from_param = {}
     for key in list_key_param:
         from_param[key] = getattr(par, key)
     # inverses wave age
-    iwa = numpy.arange(par.lut_iwa_range[0], par.lut_iwa_range[1],
+    iwa = np.arange(par.lut_iwa_range[0], par.lut_iwa_range[1],
                        par.lut_iwa_range[2])
 
-    _spac = numpy.linspace(0, range_length,
+    _spac = np.linspace(0, range_length,
                            num=nb_points).reshape((1, nb_points))
     # set_swath modifies the properties of obs_geo!
     obs_geo.concordia.set_swath(incident, _spac)
     obs_geo.discordia.set_swath(incident, _spac)
     jobs = []
     wi = par.lut_wind_range
     logger.debug("Launch jobs")
@@ -347,30 +368,30 @@
         for _iwa in iwa:
             job = (_wnd_norm, _iwa, nb_points, from_param, obs_geo)
             jobs.append(job)
     pool.map(worker_lut, jobs)
     pool.close()
     _path,  _file = os.path.split(par.obs_file)
     if par.save_iwa is False:
-        pattern = "wind_(?P<wind>\d{2})_fetch_(?P<fetch>\d{6}).nc"
+        pattern = r"wind_(?P<wind>\d{2})_fetch_(?P<fetch>\d{6}).nc"
         if "Doppler" in par.list_variable:
             _pat = f"dop_{_file}"
             write_tools.aggregate_luts_fetch(_pat, pattern, par.main_out)
         if "Backscatter" in par.list_variable:
             _pat = f"nrcs_{_file}"
             write_tools.aggregate_luts_fetch(_pat, pattern, par.main_out)
         if "imacs" in par.list_variable:
             _pat = f"imacs_{_file}"
             write_tools.aggregate_luts_fetch(_pat, pattern, par.main_out)
         if "cut_off" in par.list_variable:
             _pat = f"cut_off_{_file}"
             write_tools.aggregate_luts_fetch(_pat, pattern, par.main_out)
 
     else:
-        pattern = "wind_(?P<wind>\d{2})_iwa_(?P<iwa>\d{3}).nc"
+        pattern = r"wind_(?P<wind>\d{2})_iwa_(?P<iwa>\d{3}).nc"
         if "Doppler" in par.list_variable:
             _pat = f"dop_{_file}"
             write_tools.aggregate_luts_iwa(_pat, pattern, par.main_out)
         if "Backscatter" in par.list_variable:
             _pat = f"nrcs_{_file}"
             write_tools.aggregate_luts_iwa(_pat, pattern, par.main_out)
         if "imacs" in par.list_variable:
@@ -383,34 +404,34 @@
 
 def worker_lut(*args):
     _wnd_norm, _iwa, nb_points, par, obs_geo = args[0]
     # dimensionless fetch scalar
     X_0 = 22E3
     g = 9.81
     # compute fetch from iwa
-    X = numpy.arctanh((_iwa / 0.84) ** (-1/0.75)) ** (1 / 0.4) * X_0
+    X = np.arctanh((_iwa / 0.84) ** (-1/0.75)) ** (1 / 0.4) * X_0
     k_0 = g / _wnd_norm ** 2
     fetch = X / k_0
     ws = None
-    if ~numpy.isfinite(fetch):
+    if ~np.isfinite(fetch):
         return None
 
     # model dict should contain wnd_u, wnd_v, wnd_norm, wnd_anomaly
     model = scene_tools.generate_wind(nb_points, _wnd_norm)
     # Spectrum for short waves
     logger.info("Spectrum for short waves")
     mod_transfer, wn = spectrum_tools.spectrum_short_waves_swan(
         model, par["lambda_min"], par["lambda_max"], par["n_k"], fetch=fetch
     )
     # override model transfer functions
     # FIXME: I do not think this is really necessary, but it is a precaution
-    mod_transfer['ux'] = numpy.zeros(mod_transfer['ux'].shape)
-    mod_transfer['uy'] = numpy.zeros(mod_transfer['ux'].shape)
-    mod_transfer['vx'] = numpy.zeros(mod_transfer['ux'].shape)
-    mod_transfer['vy'] = numpy.zeros(mod_transfer['ux'].shape)
+    mod_transfer['ux'] = np.zeros(mod_transfer['ux'].shape)
+    mod_transfer['uy'] = np.zeros(mod_transfer['ux'].shape)
+    mod_transfer['vx'] = np.zeros(mod_transfer['ux'].shape)
+    mod_transfer['vy'] = np.zeros(mod_transfer['ux'].shape)
 
 
 
     iwn = int(_wnd_norm)
     fm = int(fetch)
     wan = int(_iwa*100)
     _obsf = par["obs_nonoise_file"]
@@ -440,20 +461,20 @@
         # covariance matrices with the correct correlation between the
         # polarizations
         # We will also have to think a bit how we treat the noise, which is now
         # implemented for the diagonal elements of the covariance but not for
         # the cross terms, where the expected value is zero but the variance
         # isn't.
         # A bit of thinking and validation required.
-        incidence = numpy.rad2deg(nrcsd["incidence"])
+        incidence = np.rad2deg(nrcsd["incidence"])
         nrcsd.pop("incidence", None)
 
         dic_final = {"wn": wn, "model": model, "nrcs": nrcsd, "dop": dopd,
                      "cov": covd}
-        wnd_dir = numpy.rad2deg(dic_final['model']['wnd_dir'][:, 0])
+        wnd_dir = np.rad2deg(dic_final['model']['wnd_dir'][:, 0])
         dic_dim = {'wind_direction': wnd_dir,
                    'incidence': incidence,
                    'wind_norm': dic_final['model']['wnd_norm'][0, 0],
                    'fetch': fetch,
                    'wave_age': _iwa,
                    }
         if par["save_iwa"]:
@@ -462,45 +483,45 @@
             _pat = f"{_obsf}wind_{iwn:02d}_fetch_{fm:06d}"
         # nfile = f"{_pat}.pyo"
         # with open(nfile, "wb") as pf:
         #    pickle.dump(dic_final, pf)
         nfile = f"{_pat}.nc"
         write_tools.save_lut(nfile, dic_final, dic_dim, ["nrcs", "dop"])
     if any(item in par["list_variable"] for item in ("imacs", "cut_off")):
-        logger.info("SAR co-spectra, cross-spectra, Emacs and Cut Off")
+        logger.info("SAR co-spectra, cross-spectra, iMACS and Cut Off")
         _msar = spectrum_tools.make_SAR_spectra
         _specres = _msar(ws, model, obs_geo, mod_transfer, wn,
                          par["spec_samp"], par["SAR_spectra_lambda_max"],
                          par["SAR_spectra_looks"], pol=par["txpol"],
                          rxpol=par["rxpolbase"], swell=False,
                          spec_type="LUT", fetch=fetch, k_l=par["k_l"],
                          noise=False, progress_bar=True)
         dic_final = {"wn": wn, "model": model, "cospectrum": _specres[0],
                      "cross-spectrum": _specres[1],
                      "imacs": _specres[2], "cut_off": _specres[3]}
-        wnd_dir = numpy.rad2deg(dic_final['model']['wnd_dir'][:, 0])
+        wnd_dir = np.rad2deg(dic_final['model']['wnd_dir'][:, 0])
         dic_dim = {'wind_direction': wnd_dir,
-                   'incidence': numpy.rad2deg(_specres[4]),
+                   'incidence': np.rad2deg(_specres[4]),
                    'wind_norm': dic_final['model']['wnd_norm'][0, 0],
                    'fetch': fetch,
                    'wave_age': _iwa,
                    }
         if par["save_iwa"]:
             _pat = f"{_obsf}wind_{iwn:02d}_iwa_{wan:03d}"
         else:
             _pat = f"{_obsf}wind_{iwn:02d}_fetch_{fm:06d}"
         nfile = f"{_pat}.nc"
         write_tools.save_lut(nfile, dic_final, dic_dim, ["imacs", "cut_off"])
 
 def conv2(x, y, mode='same'):
-    return numpy.rot90(convolve2d(numpy.rot90(x, 2), numpy.rot90(y, 2), mode=mode), 2)
+    return np.rot90(convolve2d(np.rot90(x, 2), np.rot90(y, 2), mode=mode), 2)
 
 def run_inversion(par):
     ''' reconstruct wind and current using inversion algorithm '''
-    import stereoid.oceans.tools.retrieval_tools as retrieval_tools
+    import stereoid.oceans.inversion.retrieval_tools as retrieval_tools
     make_default_inv(par)
 
     # # -- Read Lut
     logger.info('Read LUT')
     list_lut = {}
     for key in ('nrcs', 'dop', 'imacs', 'cut_off'):
         slut = f'{key}_{par.lut_pattern}'
@@ -512,45 +533,45 @@
     dic_l1 = {}
     for key in ('nrcs', 'imacs', 'dop', 'cut_off'):
         _pat = os.path.join(par.data_directory, f'{par.data_pattern[key]}')
         dic_l1[key], lon, lat, inc = retrieval_tools.read_L1(_pat, key, normalise_imacs=par.normalise_imacs)
         if key == 'nrcs':
             longitude = + lon
             latitude = + lat
-            incident = + numpy.array(inc)
+            incident = + np.array(inc)
     for key, value in dic_l1.items():
         # the imacs and cutoff have to be resampled as they are generated on a lower resolution than the NRCS
         if key == 'cut_off' or key == 'imacs':
-            resampled_array = numpy.zeros_like(dic_l1["nrcs"])
+            resampled_array = np.zeros_like(dic_l1["nrcs"])
 
             for i_sat in range(value.shape[2]):
                 for i_pol in range(value.shape[3]):
 
                     # this gives the opportunity to filter the imacs and cutoff before resampling
                     if par.filt_imacs != None and key == 'imacs':
 
                         if par.filt_type == 'median':
                             dic_l1[key][..., i_sat, i_pol] = median_filter(dic_l1[key][..., i_sat, i_pol],
                                                                            (par.filt_imacs, par.filt_imacs))
                         else:
                             sig = par.filt_imacs*1.
-                            n = numpy.arange(-3 * sig, 3 * sig + 1)
-                            filt = numpy.outer(numpy.exp(-0.5 * n ** 2 / sig ** 2), numpy.exp(-0.5 * n ** 2 / sig ** 2))
-                            filt = filt / numpy.sum(filt)
+                            n = np.arange(-3 * sig, 3 * sig + 1)
+                            filt = np.outer(np.exp(-0.5 * n ** 2 / sig ** 2), np.exp(-0.5 * n ** 2 / sig ** 2))
+                            filt = filt / np.sum(filt)
                             dic_l1[key][..., i_sat, i_pol]=conv2(dic_l1[key][..., i_sat, i_pol],filt,'same')
 
                     if par.filt_cutoff != None and key == 'cut_off':
                         if par.filt_type == 'median':
                             dic_l1[key][..., i_sat, i_pol] = median_filter(dic_l1[key][..., i_sat, i_pol],
                                                                        (par.filt_cutoff, par.filt_cutoff))
                         else:
                             sig = par.filt_cutoff*1.
-                            n = numpy.arange(-3 * sig, 3 * sig + 1)
-                            filt = numpy.outer(numpy.exp(-0.5 * n ** 2 / sig ** 2), numpy.exp(-0.5 * n ** 2 / sig ** 2))
-                            filt = filt / numpy.sum(filt)
+                            n = np.arange(-3 * sig, 3 * sig + 1)
+                            filt = np.outer(np.exp(-0.5 * n ** 2 / sig ** 2), np.exp(-0.5 * n ** 2 / sig ** 2))
+                            filt = filt / np.sum(filt)
                             dic_l1[key][..., i_sat, i_pol]=conv2(dic_l1[key][..., i_sat, i_pol],filt,'same')
 
                     # this removes the iwa dependence, so that cut_off is not used in the minimization
                     if par.no_iwa == 1 and key == 'cut_off':
                         dic_l1[key][..., i_sat, i_pol]=0
                         print('Warning! No iwa considered. Only for retrieval type 2.')
```

### Comparing `stereoid-0.3.1/stereoid/oceans/scene_generator.py` & `stereoid-0.4/stereoid/oceans/scene_preparation/scene_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 import numpy as np
 #from collections import namedtuple
 from matplotlib import pyplot as plt
 import drama.utils as drtls
 from drama import constants as cnst
-from stereoid.oceans import ObsGeo
+from stereoid.instrument import ObsGeo
 
 
 class SceneGenerator(object):
     def __init__(self, fwdm, shp, wspd=6, wdir=45, tsc=0,
                  grid_spacing=1e3, wave_doppler_corr_length=20e3, cartesian=True):
         """
```

### Comparing `stereoid-0.3.1/stereoid/oceans/sensitivity_distribution.py` & `stereoid-0.4/stereoid/oceans/sensitivity_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import numpy as np
 
 import drama.geo as sargeo
 from drama.io import cfg
 from drama.performance.sar import NESZdata
 import stereoid.sar_performance as strsarperf
-from stereoid.oceans import ObsGeo, FwdModel, RadarModel, RetrievalModel
+from stereoid.oceans import FwdModel, RetrievalModel
+from stereoid.instrument import ObsGeo, RadarModel
 
 
 class SensitivityDistribution:
     """Class to computer wind and TSC retirieval performance."""
 
     def __init__(
         self,
```

### Comparing `stereoid-0.3.1/stereoid/oceans/tc_scenario.py` & `stereoid-0.4/stereoid/oceans/scene_preparation/tc_scenario.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/tools/backscatter_doppler_tools.py` & `stereoid-0.4/stereoid/oceans/forward_models/backscatter_doppler_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import logging
 from collections import namedtuple
 from typing import Tuple, Optional
 
 import numpy
-import stereoid.oceans.waves.wave_spectra as swave_spectra
-import stereoid.oceans.waves.spectral_conversions as spectral_conv
 import stereoid.utils.tools as tools
 import stereoid.oceans.forward_models.wrappers as wrappers
-from stereoid.oceans import ObsGeoAngles, RadarModel
+from stereoid.instrument import ObsGeoAngles, RadarModel
 from stereoid.polarimetry import pol_rotations as polrot
 import stereoid.oceans.tools.observation_tools as obs_tools
-import stereoid.oceans.tools.spectrum_tools as spec_tools
+import stereoid.oceans.forward_models.spectrum_tools as spec_tools
 
 # Define logger level for debug purposes
 logger = logging.getLogger(__name__)
 ObsGeoTrio = namedtuple("ObsGeoTrio", ["concordia", "discordia", "sentinel1"])
 
 
 def rotation_companion(obs_geo, inc_tx: float, ws: dict
@@ -554,14 +552,15 @@
     if cross is True:
         _res = sum(dic[item] for item in dic if "cross" in item)
     else:
         _res = sum(dic[item] for item in dic if "cross" not in item)
     return _res
 
 
+# FIXME move thist to instrument/something
 def add_noise(
     nrcs: dict, dop: dict, dx: float, par, dic_geom: Optional[dict] = {}
 ) -> None:
     nrcs.pop("incidence", None)
     if "obs_geo" in dic_geom.keys():
         obs_geo = dic_geom["obs_geo"]
     else:
@@ -575,14 +574,15 @@
         fstr_ati = dic_geom["fstr_ati"]
         fstr_s1 = dic_geom["fstr_s1"]
     else:
         fstr_dual, fstr_ati, fstr_s1 = obs_tools.build_performance_file(par)
         dic_geom["fstr_dual"] = fstr_dual
         dic_geom["fstr_ati"] = fstr_ati
         dic_geom["fstr_s1"] = fstr_s1
+    # FIXME this could also be the TOPS model, so this needs to be handled
     radarm = RadarModel(
         obs_geo,
         fstr_s1,
         fstr_dual,
         fstr_ati,
         az_res=par.az_res,
         prod_res=dx,
```

### Comparing `stereoid-0.3.1/stereoid/oceans/tools/observation_tools.py` & `stereoid-0.4/stereoid/oceans/tools/observation_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
-import numpy
-from scipy import interpolate
 from collections import namedtuple
 from typing import Tuple, Optional
 
+import numpy
 from drama.geo.bistatic_pol import CompanionPolarizations
-import stereoid.sar_performance as sar_perf
-from stereoid.oceans import ObsGeo
-from stereoid.oceans.waves.wave_spectra import Kudry_spec_polar
+from scipy import interpolate
 
+import stereoid.sar_performance as sar_perf
+from stereoid.instrument import ObsGeo
 
 # Define logger level for debug purposes
 logger = logging.getLogger(__name__)
 ObsGeoTrio = namedtuple("ObsGeoTrio", ["concordia", "discordia", "sentinel1"])
 
 
 def build_geometry(par_geometry: str, incident: float,
@@ -114,18 +113,16 @@
     for i in range(0,S.shape[1]):
         f = interpolate.interp1d(phi,S[:,i])
         S_int[:,i]=f(phi_int)
 
     return S_int
 
 if __name__ == '__main__':
-    import numpy as np
-    from matplotlib import pyplot as plt
     from pylab import *
-    #import stereoid.oceans.forward_models.backscatter as backscatter
+    from stereoid.oceans.waves.wave_spectra import Kudry_spec_polar
 
     g = 9.81
     n_k=100
     lambda_min=0.005
     lambda_max=1000
     k_min = 2 * np.pi / lambda_max  # minimum wave number
     k_max = 2 * np.pi / lambda_min  # should at least pass the Bragg wave
```

### Comparing `stereoid-0.3.1/stereoid/oceans/tools/read_tools.py` & `stereoid-0.4/stereoid/oceans/io/read_tools.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/tools/retrieval_tools.py` & `stereoid-0.4/stereoid/oceans/inversion/retrieval_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import numpy as np
 import xarray as xr
 import logging
 from typing import Optional, Tuple
 from scipy.ndimage import gaussian_filter
 from stereoid.oceans import RetrievalModel, FwdModelRIM
-import stereoid.oceans.tools.read_tools as read_tools
+import stereoid.oceans.io.read_tools as read_tools
 from drama.utils.filtering import smooth1d
 import drama.utils as drtls
 from scipy.signal import medfilt
 
 
 # Define logger level for debug purposes
 logger = logging.getLogger(__name__)
```

### Comparing `stereoid-0.3.1/stereoid/oceans/tools/scene_tools.py` & `stereoid-0.4/stereoid/oceans/scene_preparation/scene_tools.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/tools/spectrum_tools.py` & `stereoid-0.4/stereoid/oceans/forward_models/spectrum_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from scipy.signal import convolve2d
 import numpy.typing as npt
 import stereoid.oceans.waves.wave_spectra as swave_spectra
 import stereoid.oceans.waves.spectral_conversions as spectral_conv
 import stereoid.oceans.waves.high_resolution_var as hr_var
 import stereoid.utils.tools as tools
 from stereoid.oceans.forward_models import SAR_spectra as SAR_model
-from stereoid.oceans import ObsGeoAngles
+from stereoid.instrument import ObsGeoAngles
 import stereoid.oceans.tools.observation_tools as obs_tools
 from stereoid.oceans.forward_models.wrappers import (
     interp_weights as griddata_step1,
     interpolate as griddata_step2,
 )
 
 # Define logger level for debug purposes
@@ -728,15 +728,15 @@
 
     # mean wind direction
     # scene size cannot be too big
     if short_wave_spec_type == 'polar':
         wave_number = wave_number_grids_polar(lambda_min, lambda_max, n_k)
     else:
         wave_number = wave_number_grids(lambda_min, lambda_max, n_k)
-    phi_w = (numpy.mean(numpy.arctan2(model["wnd_v"], model["wnd_u"])))
+    phi_w = numpy.arctan2(numpy.mean(model["wnd_v"]), numpy.mean(model["wnd_u"]))
 
     wave_number["phi_w"] = phi_w
     # (short-wave) spectrum from Kudry1999, Kudry2003, Kudry2005 based on
     # appendices from Yuroyskaya2013, KCM2014
     # we use one reference spectrum here for short waves, maybe it is better
     # to directly put the long waves into Kudry_spec to get right equilibrium
     U_mean = numpy.nanmean(model["wnd_norm"])
```

### Comparing `stereoid-0.3.1/stereoid/oceans/tools/wave_spectra_inversion_tools.py` & `stereoid-0.4/stereoid/oceans/inversion/wave_spectra_inversion_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 __author__ = "Marcel Kleinherenbrink"
 __email__ = "M.Kleinherenbrink@tudelft.nl"
 
 import numpy as np
 import glob
 import pickle
 from stereoid.oceans.forward_models import SAR_spectra as SAR_model
-from stereoid.oceans import ObsGeoAngles
+from stereoid.instrument import ObsGeoAngles
 from stereoid.oceans.forward_models.wrappers import interp_weights as griddata_step1
 import stereoid.oceans.inversion.wave_spectra_inversion as wav_inv
-import stereoid.oceans.tools.spectrum_tools as spectrum_tools
+import stereoid.oceans.forward_models.spectrum_tools as spectrum_tools
 
 # this method converts the inverted parameters (for example k_s*np.cos(phi) and k_s*np.sin(phi)) to swell-wave parameters
 def inversion2swellparameters(yhat,var,incs,ref_inc,Hs=0,sigma_Hs=0):
     """
 
     Parameters
     ----------
```

### Comparing `stereoid-0.3.1/stereoid/oceans/tools/write_tools.py` & `stereoid-0.4/stereoid/oceans/io/write_tools.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/tops_model.py` & `stereoid-0.4/stereoid/instrument/tops_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import drama.io.cfg as cfg
 import numpy as np
 import numpy.typing as npt
 import scipy.linalg as linalg
 from scipy.interpolate import CubicSpline, RegularGridInterpolator
 import xarray as xr
 
-import stereoid.oceans.radar_model
+import stereoid.instrument.radar_model
 import stereoid.utils.config as st_config
 
 BURST_DURATION = 3  # focus burst length in seconds
 BURST_OVERLAP = 0.22  # in seconds
 SLC_AZ_SAMPLING = 2e-3  # in seconds
 SLC_NR_DEMARC_LINES = 20
 
@@ -354,15 +354,15 @@
         inc_near,
         inc_far,
         r_s,
         par_data.IWS.burst_length,
     )
 
 
-class TopsModel(stereoid.oceans.radar_model.RadarModel):
+class TopsModel(stereoid.instrument.radar_model.RadarModel):
     def __init__(
         self,
         t_in_bs: Union[float, npt.ArrayLike],
         posting: float,
         *args,
         **kwargs,
     ):
```

### Comparing `stereoid-0.3.1/stereoid/oceans/visualization/geo_plot.py` & `stereoid-0.4/stereoid/oceans/visualization/geo_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 import os
 import matplotlib.pyplot as plt
 import matplotlib
-from cartopy import config
 import cartopy
 import cartopy.crs as ccrs
 import drama.utils as drutl
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
-import numpy.ma as ma
 import numpy as np
-from cartopy.io.shapereader import Reader
-from cartopy.feature import ShapelyFeature
 from cartopy.mpl.gridliner import LONGITUDE_FORMATTER, LATITUDE_FORMATTER
-import matplotlib.ticker as mticker
 from scipy.signal import convolve2d
 
 def guess_cmap(vmin, vmax):
     if vmax < 0:
         cmap = 'bone'
     elif vmin >= 0:
         # Coherence
@@ -298,17 +293,16 @@
                     verticalalignment='top', bbox=props, zorder=6)
 
 #%%
 if __name__ == '__main__':
 
     import xarray as xr
 
-    import stereoid.sar_performance as strsarperf
     import stereoid.utils.config as st_config
-    from stereoid.oceans.read_scenario_California import read_scenario_California
+    from stereoid.oceans.scene_preparation.read_scenario_California import read_scenario_California
 
     paths = st_config.parse(section="Paths")
     # Unpack the paths read from user.cfg. If user.cfg is not found user_defaults.cfg is used.
     main_dir = paths["main"]
     datadir = paths["data"]
     pardir = paths["par"]
     resultsdir = paths["results"]
```

### Comparing `stereoid-0.3.1/stereoid/oceans/waves/SceneGenerator_wavetrains.py` & `stereoid-0.4/stereoid/oceans/waves/SceneGenerator_wavetrains.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/waves/high_resolution_var.py` & `stereoid-0.4/stereoid/oceans/waves/high_resolution_var.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/waves/spectral_conversions.py` & `stereoid-0.4/stereoid/oceans/waves/spectral_conversions.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/oceans/waves/wave_spectra.py` & `stereoid-0.4/stereoid/oceans/waves/wave_spectra.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/polarimetry/pol_rotations.py` & `stereoid-0.4/stereoid/polarimetry/pol_rotations.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/sar_performance/azimuth_performance.py` & `stereoid-0.4/stereoid/sar_performance/azimuth_performance.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/sar_performance/calc_rasr.py` & `stereoid-0.4/stereoid/sar_performance/calc_rasr.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/sar_performance/calc_sar_performance.py` & `stereoid-0.4/stereoid/sar_performance/calc_sar_performance.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/sar_performance/casa_patterns.py` & `stereoid-0.4/stereoid/sar_performance/casa_patterns.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/sar_performance/filestructure.py` & `stereoid-0.4/stereoid/sar_performance/filestructure.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/sea_ice/forward_model.py` & `stereoid-0.4/stereoid/sea_ice/forward_model.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/sea_ice/image_processing.py` & `stereoid-0.4/stereoid/sea_ice/image_processing.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/sea_ice/performance.py` & `stereoid-0.4/stereoid/sea_ice/performance.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 __email__ = "F.LopezDekker@tudeft.nl"
 
 import numpy as np
 import scipy.interpolate as interp
 from matplotlib import pyplot as plt
 import matplotlib
 import drama.performance.doppler_centroid as doppler_centroid
-import stereoid.oceans.cmod5n as cmod5
+import stereoid.oceans.forward_models.cmod5n as cmod5
 import drama.constants as cnst
 # import drama.geo.geometry as sargeo
 from drama.orbits import orbit_to_vel
 import os
 import drama.performance.insar as insar
 from drama.performance import sar as sar
```

### Comparing `stereoid-0.3.1/stereoid/sea_ice/radar_model.py` & `stereoid-0.4/stereoid/sea_ice/radar_model.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/sea_ice/read_nextsim.py` & `stereoid-0.4/stereoid/sea_ice/read_nextsim.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/sea_ice/retrieval_model.py` & `stereoid-0.4/stereoid/sea_ice/retrieval_model.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/sea_ice/scene_generator.py` & `stereoid-0.4/stereoid/sea_ice/scene_generator.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/sea_ice/ste_io.py` & `stereoid-0.4/stereoid/sea_ice/ste_io.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/California_wrappers.py` & `stereoid-0.4/stereoid/tropical_cyclones/Deprecated/California_wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import stereoid.tropical_cyclones.Deprecated.backscatter as backscatter
 from stereoid.tropical_cyclones.Deprecated.Doppler import DopRIM
-from stereoid.oceans.bistatic_pol import elfouhaily as Elf_pol
+from stereoid.polarimetry.bistatic_pol import elfouhaily as Elf_pol
 import scipy.spatial.qhull as qhull
 from matplotlib import pyplot as plt
 
 def make_grids_mono(SHP):
     # monostatic (completely unnecessary, but okay)
     s_sp = np.zeros( SHP )  # specular scattering
     s_br = np.zeros( SHP )  # Bragg scattering
```

### Comparing `stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/Doppler.py` & `stereoid-0.4/stereoid/tropical_cyclones/Deprecated/Doppler.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/RAR_model.py` & `stereoid-0.4/stereoid/tropical_cyclones/Deprecated/RAR_model.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/SAR_model.py` & `stereoid-0.4/stereoid/tropical_cyclones/Deprecated/SAR_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Marcel Kleinherenbrink"
 __email__ = "M.Kleinherenbrink@tudelft.nl"
 
-import stereoid.oceans.cmod5n as cmod5n
+import stereoid.oceans.forward_models.cmod5n as cmod5n
 
 
 # Implementation of Engen and Johnsen (1995)
 # This works with linear spacing in kx and ky, maybe we have to change this
 # I will make another function for a log-scale spacing
 def corr_func( S, kx, ky, mu = 0.5, theta = 35, R = 850E3, V = 7000, mtf = 'Schulz', phi_w = 0.0, ws = 15.0 ):
     # S: two-dimensional directional wave spectrum (Krogstad 1992: it is not symmetrical, but directional)
@@ -26,16 +26,16 @@
     T_y[ T_y != T_y ] = 0
     T_I = np.zeros( k.shape )
     if mtf == 'Schulz':
         T_I = -1j * 4 * kx / (np.tan( theta ) * (1 + np.sin( theta ) ** 2)) - 1j * kx / np.tan(
             theta ) + 4.5 * omega * kx ** 2 * (omega - 1j * mu) / (k * (omega ** 2 + mu ** 2))
     if mtf == 'S1':
         dth = 0.001
-        sigma = cmod5n.cmod5n_forward( np.array( [ ws, ws ] ), np.array( [ phi_w, phi_w ] ),
-                                       np.rad2deg( np.array( [ theta, theta + dth ] ) ) )  # use CMOD5n here
+        sigma = cmod5n.cmod5n_forward(np.array([ws, ws]), np.array([phi_w, phi_w]),
+                                      np.rad2deg( np.array( [ theta, theta + dth ] ) ))  # use CMOD5n here
         dsigma = (sigma[ 1 ] - sigma[ 0 ]) / dth
         T_I = kx * dsigma / sigma[ 0 ] / np.cos( theta ) * (
                 kx / k * np.sin( theta ) + 1j * np.cos( theta ))  # combination of both equations (37)
     T_I[ T_I != T_I ] = 0
 
     # cross-spectral functions
     N_II_pos = 0.5 * T_I * np.conj( T_I )
@@ -171,16 +171,16 @@
         # I guss that (kx * np.cos( alpha / 2 ) - ky * np.sin( alpha / 2 )) ** 2 has to be scaled with np.cos( alpha / 2 )
         # and k also
         T_I = -1j * 4 * k_l / (np.tan( theta_m ) * (1 + np.sin( theta_m ) ** 2)) - 1j * k_l / np.tan(
             theta_m ) + 4.5 * omega * k_l ** 2 * (omega - 1j * mu) / (k * (omega ** 2 + mu ** 2))
     if mtf == 'S1':
         # FIXME I guess this k_l should be like below, but this should be rigorously checked
         dth = 0.001
-        sigma = cmod5n.cmod5n_forward( np.array( [ ws, ws ] ), np.array( [ phi_w, phi_w ] ),
-                                       np.rad2deg( np.array( [ theta_m, theta_m + dth ] ) ) )  # use CMOD5n here
+        sigma = cmod5n.cmod5n_forward(np.array([ws, ws]), np.array([phi_w, phi_w]),
+                                      np.rad2deg( np.array( [ theta_m, theta_m + dth ] ) ))  # use CMOD5n here
         dsigma = (sigma[ 1 ] - sigma[ 0 ]) / dth
         T_I = k_l * dsigma / sigma[ 0 ] / np.cos( theta_m ) * (
                 k_l / k * np.sin( theta_m ) + 1j * np.cos( theta_m ))  # combination of both equations (37)
 
     T_x[ T_x != T_x ] = 0
     T_y[ T_y != T_y ] = 0
     T_I[ T_I != T_I ] = 0
```

### Comparing `stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/backscatter.py` & `stereoid-0.4/stereoid/tropical_cyclones/Deprecated/backscatter.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/constants.py` & `stereoid-0.4/stereoid/tropical_cyclones/Deprecated/constants.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/high_resolution_var.py` & `stereoid-0.4/stereoid/tropical_cyclones/Deprecated/high_resolution_var.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/polarimetry.py` & `stereoid-0.4/stereoid/tropical_cyclones/Deprecated/polarimetry.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/scene_generator.py` & `stereoid-0.4/stereoid/tropical_cyclones/Deprecated/scene_generator.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/tropical_cyclones/Deprecated/wave_spectra.py` & `stereoid-0.4/stereoid/tropical_cyclones/Deprecated/wave_spectra.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/utils/config.py` & `stereoid-0.4/stereoid/utils/config.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/utils/diffusion.py` & `stereoid-0.4/stereoid/utils/diffusion.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/utils/plot_helpers.py` & `stereoid-0.4/stereoid/utils/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid/utils/tools.py` & `stereoid-0.4/stereoid/utils/tools.py`

 * *Files identical despite different names*

### Comparing `stereoid-0.3.1/stereoid.egg-info/PKG-INFO` & `stereoid-0.4/stereoid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stereoid
-Version: 0.3.1
+Version: 0.4
 Summary: The stereoid tools for the Harmony mission.
 Author-email: Paco Lopez Dekker <F.LopezDekker@tudelft.nl>, Andreas Theodosiou <a.theodosiou@tudelft.nl>, Marcel Kleinherenbrink <M.Kleinherenbrink@tudelft.nl>
 Project-URL: Repository, https://gitlab.tudelft.nl/drama/stereoid.git
 Project-URL: Bug Tracker, https://gitlab.tudelft.nl/drama/stereoid/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `stereoid-0.3.1/stereoid.egg-info/SOURCES.txt` & `stereoid-0.4/stereoid.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 stereoid/cli.py
 stereoid.egg-info/PKG-INFO
 stereoid.egg-info/SOURCES.txt
 stereoid.egg-info/dependency_links.txt
 stereoid.egg-info/entry_points.txt
 stereoid.egg-info/requires.txt
 stereoid.egg-info/top_level.txt
+stereoid/instrument/__init__.py
+stereoid/instrument/dca_performance.py
+stereoid/instrument/radar_model.py
+stereoid/instrument/tops_model.py
 stereoid/land_ice/AASR_code.py
 stereoid/land_ice/AASR_functions.py
 stereoid/land_ice/__init__.py
 stereoid/land_ice/back_scatter_model.py
 stereoid/land_ice/coherence_model_SAR_stack.py
 stereoid/land_ice/coherence_model_baseline_volume.py
 stereoid/land_ice/deterministic_data.py
@@ -29,68 +33,65 @@
 stereoid/land_ice/study_area_plots.py
 stereoid/mission/__init__.py
 stereoid/mission/acquisitions_script.py
 stereoid/mission/activation_analysis.py
 stereoid/mission/coverage.py
 stereoid/mission/formation_design.py
 stereoid/oceans/__init__.py
-stereoid/oceans/bistatic_pol.py
-stereoid/oceans/cmod5n.py
-stereoid/oceans/dca_performance.py
 stereoid/oceans/forward_model.py
-stereoid/oceans/image_processing.py
 stereoid/oceans/l2_covariance.py
-stereoid/oceans/les.py
 stereoid/oceans/profile_add_errors.py
-stereoid/oceans/radar_model.py
 stereoid/oceans/read_fwd.py
-stereoid/oceans/read_scenario_California.py
-stereoid/oceans/read_scenarios.py
 stereoid/oceans/retrieval_model.py
 stereoid/oceans/retrieval_performance.py
 stereoid/oceans/run_scenario.py
-stereoid/oceans/scene_generator.py
 stereoid/oceans/sensitivity_distribution.py
-stereoid/oceans/tc_scenario.py
-stereoid/oceans/tops_model.py
-stereoid/oceans/GMF/IWRAP_backscatter.py
-stereoid/oceans/GMF/Zadelhoff_crosspol.py
-stereoid/oceans/GMF/__init__.py
-stereoid/oceans/GMF/cdop.py
-stereoid/oceans/GMF/cmod5n.py
 stereoid/oceans/forward_models/Doppler.py
 stereoid/oceans/forward_models/RIM_calibration.py
 stereoid/oceans/forward_models/RIM_constants.py
 stereoid/oceans/forward_models/SAR_spectra.py
 stereoid/oceans/forward_models/SAR_spectra_broken.py
 stereoid/oceans/forward_models/__init__.py
 stereoid/oceans/forward_models/backscatter.py
+stereoid/oceans/forward_models/backscatter_doppler_tools.py
+stereoid/oceans/forward_models/cdop.py
+stereoid/oceans/forward_models/cmod5n.py
+stereoid/oceans/forward_models/iwrap_backscatter.py
 stereoid/oceans/forward_models/sea_state_bias.py
+stereoid/oceans/forward_models/spectrum_tools.py
 stereoid/oceans/forward_models/wrappers.py
+stereoid/oceans/forward_models/zadelhoff_crosspol.py
 stereoid/oceans/forward_models/Deprecated/__init__.py
 stereoid/oceans/forward_models/Deprecated/polarimetry.py
 stereoid/oceans/inversion/RIM_inversion_deprecated.py
+stereoid/oceans/inversion/__init__.py
+stereoid/oceans/inversion/retrieval_tools.py
 stereoid/oceans/inversion/wave_spectra_inversion.py
+stereoid/oceans/inversion/wave_spectra_inversion_tools.py
+stereoid/oceans/io/__init__.py
+stereoid/oceans/io/read_tools.py
+stereoid/oceans/io/write_tools.py
+stereoid/oceans/scene_preparation/__init__.py
+stereoid/oceans/scene_preparation/les.py
+stereoid/oceans/scene_preparation/read_scenario_California.py
+stereoid/oceans/scene_preparation/read_scenarios.py
+stereoid/oceans/scene_preparation/scene_generator.py
+stereoid/oceans/scene_preparation/scene_tools.py
+stereoid/oceans/scene_preparation/tc_scenario.py
 stereoid/oceans/tools/__init__.py
-stereoid/oceans/tools/backscatter_doppler_tools.py
 stereoid/oceans/tools/observation_tools.py
-stereoid/oceans/tools/read_tools.py
-stereoid/oceans/tools/retrieval_tools.py
-stereoid/oceans/tools/scene_tools.py
-stereoid/oceans/tools/spectrum_tools.py
-stereoid/oceans/tools/wave_spectra_inversion_tools.py
-stereoid/oceans/tools/write_tools.py
 stereoid/oceans/visualization/__init__.py
 stereoid/oceans/visualization/geo_plot.py
 stereoid/oceans/waves/SceneGenerator_wavetrains.py
 stereoid/oceans/waves/__init__.py
 stereoid/oceans/waves/high_resolution_var.py
 stereoid/oceans/waves/spectral_conversions.py
 stereoid/oceans/waves/wave_spectra.py
 stereoid/polarimetry/__init__.py
+stereoid/polarimetry/bistatic_pol.py
 stereoid/polarimetry/pol_rotations.py
 stereoid/sar_performance/__init__.py
 stereoid/sar_performance/azimuth_performance.py
 stereoid/sar_performance/calc_rasr.py
 stereoid/sar_performance/calc_sar_performance.py
 stereoid/sar_performance/casa_patterns.py
 stereoid/sar_performance/filestructure.py
@@ -115,11 +116,8 @@
 stereoid/tropical_cyclones/Deprecated/scene_generator.py
 stereoid/tropical_cyclones/Deprecated/wave_spectra.py
 stereoid/utils/__init__.py
 stereoid/utils/config.py
 stereoid/utils/diffusion.py
 stereoid/utils/plot_helpers.py
 stereoid/utils/tools.py
-test/plot_output.py
-tests/__init__.py
-tests/test_config.py
-tests/test_param.ini
+test/plot_output.py
```

### Comparing `stereoid-0.3.1/test/plot_output.py` & `stereoid-0.4/test/plot_output.py`

 * *Files identical despite different names*

