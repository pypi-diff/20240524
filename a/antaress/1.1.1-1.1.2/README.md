# Comparing `tmp/antaress-1.1.1.tar.gz` & `tmp/antaress-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antaress-1.1.1.tar", last modified: Thu May 23 14:06:59 2024, max compression
+gzip compressed data, was "antaress-1.1.2.tar", last modified: Fri May 24 07:48:26 2024, max compression
```

## Comparing `antaress-1.1.1.tar` & `antaress-1.1.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.612913 antaress-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-23 14:05:30.000000 antaress-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2063 2024-05-23 14:06:59.612913 antaress-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1101 2024-05-23 14:05:30.000000 antaress-1.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-23 14:05:30.000000 antaress-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 14:06:59.612913 antaress-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      298 2024-05-23 14:05:30.000000 antaress-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.589911 antaress-1.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.591911 antaress-1.1.1/src/antaress/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.596912 antaress-1.1.1/src/antaress/ANTARESS_analysis/
--rwxrwxrwx   0 root         (0) root         (0)   205187 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_ana_comm.py
--rw-rw-rw-   0 root         (0) root         (0)    12027 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_inst_resp.py
--rwxrwxrwx   0 root         (0) root         (0)     1247 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_joined_atm.py
--rwxrwxrwx   0 root         (0) root         (0)    90944 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_joined_star.py
--rw-rw-rw-   0 root         (0) root         (0)    24209 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_model_prof.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.597912 antaress-1.1.1/src/antaress/ANTARESS_analysis/C_grid/
--rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/C_grid/Gauss_star_grid.c
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.599912 antaress-1.1.1/src/antaress/ANTARESS_conversions/
--rw-rw-rw-   0 root         (0) root         (0)   104496 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_binning.py
--rw-rw-rw-   0 root         (0) root         (0)    50846 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_conv.py
--rw-rw-rw-   0 root         (0) root         (0)    11472 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_masks_gen.py
--rw-rw-rw-   0 root         (0) root         (0)    15598 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_sp_cont.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.601912 antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/
--rw-rw-rw-   0 root         (0) root         (0)    62059 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/KitCat_main.py
--rw-rw-rw-   0 root         (0) root         (0)    22807 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/Kitcat_classes.py
--rw-rw-rw-   0 root         (0) root         (0)     9261 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/Kitcat_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/setup_lbl_fit.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.607913 antaress-1.1.1/src/antaress/ANTARESS_corrections/
--rw-rw-rw-   0 root         (0) root         (0)    29437 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_calib.py
--rw-rw-rw-   0 root         (0) root         (0)    53772 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_detrend.py
--rwxrwxrwx   0 root         (0) root         (0)    58484 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_flux_balance.py
--rwxrwxrwx   0 root         (0) root         (0)   254034 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_interferences.py
--rwxrwxrwx   0 root         (0) root         (0)    28412 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_peaks.py
--rwxrwxrwx   0 root         (0) root         (0)    15185 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_sp_reduc.py
--rwxrwxrwx   0 root         (0) root         (0)    50990 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_tellurics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.607913 antaress-1.1.1/src/antaress/ANTARESS_corrections/Telluric_processing/
--rw-rw-rw-   0 root         (0) root         (0)    58000 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/Telluric_processing/Create_static_files.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.608913 antaress-1.1.1/src/antaress/ANTARESS_general/
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_general/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27026 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_general/constant_data.py
--rw-rw-rw-   0 root         (0) root         (0)   111761 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_general/minim_routines.py
--rwxrwxrwx   0 root         (0) root         (0)    30542 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_general/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.609913 antaress-1.1.1/src/antaress/ANTARESS_grids/
--rw-rw-rw-   0 root         (0) root         (0)    45505 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_coord.py
--rw-rw-rw-   0 root         (0) root         (0)   117508 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_occ_grid.py
--rw-rw-rw-   0 root         (0) root         (0)    33059 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_prof_grid.py
--rw-rw-rw-   0 root         (0) root         (0)    22950 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_star_grid.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_grids/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.610913 antaress-1.1.1/src/antaress/ANTARESS_launch/
--rw-rw-rw-   0 root         (0) root         (0)     2356 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_gridrun.py
--rw-rw-rw-   0 root         (0) root         (0)     5749 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_launcher.py
--rw-rw-rw-   0 root         (0) root         (0)   192615 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    15931 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_systems.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_launch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.611914 antaress-1.1.1/src/antaress/ANTARESS_plots/
--rw-rw-rw-   0 root         (0) root         (0)    92437 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_plots/ANTARESS_plot_settings.py
--rwxrwxrwx   0 root         (0) root         (0)   647371 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_plots/ANTARESS_plots_all.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25189 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_plots/utils_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.612913 antaress-1.1.1/src/antaress/ANTARESS_process/
--rw-rw-rw-   0 root         (0) root         (0)     6378 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_data_align.py
--rw-rw-rw-   0 root         (0) root         (0)   106409 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_data_process.py
--rw-rw-rw-   0 root         (0) root         (0)   193806 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_main.py
--rw-rw-rw-   0 root         (0) root         (0)    45382 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_plocc_spec.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_process/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.612913 antaress-1.1.1/src/antaress.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2063 2024-05-23 14:06:59.000000 antaress-1.1.1/src/antaress.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2744 2024-05-23 14:06:59.000000 antaress-1.1.1/src/antaress.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 14:06:59.000000 antaress-1.1.1/src/antaress.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2024-05-23 14:06:59.000000 antaress-1.1.1/src/antaress.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      151 2024-05-23 14:06:59.000000 antaress-1.1.1/src/antaress.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-23 14:06:59.000000 antaress-1.1.1/src/antaress.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.846780 antaress-1.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-24 07:47:00.000000 antaress-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2063 2024-05-24 07:48:26.846780 antaress-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2024-05-24 07:47:00.000000 antaress-1.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-24 07:47:00.000000 antaress-1.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 07:48:26.847781 antaress-1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      298 2024-05-24 07:47:00.000000 antaress-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.815777 antaress-1.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.817777 antaress-1.1.2/src/antaress/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.824778 antaress-1.1.2/src/antaress/ANTARESS_analysis/
+-rwxrwxrwx   0 root         (0) root         (0)   205187 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_analysis/ANTARESS_ana_comm.py
+-rw-rw-rw-   0 root         (0) root         (0)    12027 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_analysis/ANTARESS_inst_resp.py
+-rwxrwxrwx   0 root         (0) root         (0)     1247 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_analysis/ANTARESS_joined_atm.py
+-rwxrwxrwx   0 root         (0) root         (0)    90944 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_analysis/ANTARESS_joined_star.py
+-rw-rw-rw-   0 root         (0) root         (0)    24209 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_analysis/ANTARESS_model_prof.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.824778 antaress-1.1.2/src/antaress/ANTARESS_analysis/C_grid/
+-rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_analysis/C_grid/Gauss_star_grid.c
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_analysis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.829779 antaress-1.1.2/src/antaress/ANTARESS_conversions/
+-rw-rw-rw-   0 root         (0) root         (0)   104496 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_conversions/ANTARESS_binning.py
+-rw-rw-rw-   0 root         (0) root         (0)    50846 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_conversions/ANTARESS_conv.py
+-rw-rw-rw-   0 root         (0) root         (0)    11472 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_conversions/ANTARESS_masks_gen.py
+-rw-rw-rw-   0 root         (0) root         (0)    15598 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_conversions/ANTARESS_sp_cont.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.832779 antaress-1.1.2/src/antaress/ANTARESS_conversions/KitCat/
+-rw-rw-rw-   0 root         (0) root         (0)    62059 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_conversions/KitCat/KitCat_main.py
+-rw-rw-rw-   0 root         (0) root         (0)    22807 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_conversions/KitCat/Kitcat_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9261 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_conversions/KitCat/Kitcat_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_conversions/KitCat/setup_lbl_fit.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_conversions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.840780 antaress-1.1.2/src/antaress/ANTARESS_corrections/
+-rw-rw-rw-   0 root         (0) root         (0)    29437 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_calib.py
+-rw-rw-rw-   0 root         (0) root         (0)    53772 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_detrend.py
+-rwxrwxrwx   0 root         (0) root         (0)    58484 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_flux_balance.py
+-rwxrwxrwx   0 root         (0) root         (0)   254034 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_interferences.py
+-rwxrwxrwx   0 root         (0) root         (0)    28412 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_peaks.py
+-rwxrwxrwx   0 root         (0) root         (0)    15185 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_sp_reduc.py
+-rwxrwxrwx   0 root         (0) root         (0)    50990 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_tellurics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.840780 antaress-1.1.2/src/antaress/ANTARESS_corrections/Telluric_processing/
+-rw-rw-rw-   0 root         (0) root         (0)    58000 2024-05-24 07:47:00.000000 antaress-1.1.2/src/antaress/ANTARESS_corrections/Telluric_processing/Create_static_files.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_corrections/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.842780 antaress-1.1.2/src/antaress/ANTARESS_general/
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_general/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27026 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_general/constant_data.py
+-rw-rw-rw-   0 root         (0) root         (0)   111761 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_general/minim_routines.py
+-rwxrwxrwx   0 root         (0) root         (0)    30542 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_general/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.843780 antaress-1.1.2/src/antaress/ANTARESS_grids/
+-rw-rw-rw-   0 root         (0) root         (0)    45505 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_grids/ANTARESS_coord.py
+-rw-rw-rw-   0 root         (0) root         (0)   117508 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_grids/ANTARESS_occ_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)    33059 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_grids/ANTARESS_prof_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)    22950 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_grids/ANTARESS_star_grid.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_grids/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.844780 antaress-1.1.2/src/antaress/ANTARESS_launch/
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_launch/ANTARESS_gridrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     5749 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_launch/ANTARESS_launcher.py
+-rw-rw-rw-   0 root         (0) root         (0)   192615 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_launch/ANTARESS_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    15931 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_launch/ANTARESS_systems.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_launch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.845780 antaress-1.1.2/src/antaress/ANTARESS_plots/
+-rw-rw-rw-   0 root         (0) root         (0)    92437 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_plots/ANTARESS_plot_settings.py
+-rwxrwxrwx   0 root         (0) root         (0)   647371 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_plots/ANTARESS_plots_all.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25189 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_plots/utils_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.846780 antaress-1.1.2/src/antaress/ANTARESS_process/
+-rw-rw-rw-   0 root         (0) root         (0)     6378 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_process/ANTARESS_data_align.py
+-rw-rw-rw-   0 root         (0) root         (0)   106409 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_process/ANTARESS_data_process.py
+-rw-rw-rw-   0 root         (0) root         (0)   193806 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_process/ANTARESS_main.py
+-rw-rw-rw-   0 root         (0) root         (0)    45382 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_process/ANTARESS_plocc_spec.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/ANTARESS_process/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-24 07:47:02.000000 antaress-1.1.2/src/antaress/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:48:26.846780 antaress-1.1.2/src/antaress.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2063 2024-05-24 07:48:26.000000 antaress-1.1.2/src/antaress.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2744 2024-05-24 07:48:26.000000 antaress-1.1.2/src/antaress.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 07:48:26.000000 antaress-1.1.2/src/antaress.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-24 07:48:26.000000 antaress-1.1.2/src/antaress.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2024-05-24 07:48:26.000000 antaress-1.1.2/src/antaress.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-24 07:48:26.000000 antaress-1.1.2/src/antaress.egg-info/top_level.txt
```

### Comparing `antaress-1.1.1/LICENSE` & `antaress-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/PKG-INFO` & `antaress-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antaress
-Version: 1.1.1
+Version: 1.1.2
 Summary: High-resolution spectroscopy pipeline
 Author-email: Vincent Bourrier <vincent.bourrier@unige.ch>
 Project-URL: Homepage, https://gitlab.unige.ch/bourrier/ANTARESS
 Project-URL: Issues, https://gitlab.unige.ch/bourrier/ANTARESS/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `antaress-1.1.1/README.md` & `antaress-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/pyproject.toml` & `antaress-1.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools >= 61.0", "wheel", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "antaress"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name = "Vincent Bourrier", email = "vincent.bourrier@unige.ch" },
 ]
 description = "High-resolution spectroscopy pipeline"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_ana_comm.py` & `antaress-1.1.2/src/antaress/ANTARESS_analysis/ANTARESS_ana_comm.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_inst_resp.py` & `antaress-1.1.2/src/antaress/ANTARESS_analysis/ANTARESS_inst_resp.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_joined_atm.py` & `antaress-1.1.2/src/antaress/ANTARESS_analysis/ANTARESS_joined_atm.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_joined_star.py` & `antaress-1.1.2/src/antaress/ANTARESS_analysis/ANTARESS_joined_star.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_model_prof.py` & `antaress-1.1.2/src/antaress/ANTARESS_analysis/ANTARESS_model_prof.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_analysis/C_grid/Gauss_star_grid.c` & `antaress-1.1.2/src/antaress/ANTARESS_analysis/C_grid/Gauss_star_grid.c`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_binning.py` & `antaress-1.1.2/src/antaress/ANTARESS_conversions/ANTARESS_binning.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_conv.py` & `antaress-1.1.2/src/antaress/ANTARESS_conversions/ANTARESS_conv.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_masks_gen.py` & `antaress-1.1.2/src/antaress/ANTARESS_conversions/ANTARESS_masks_gen.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_sp_cont.py` & `antaress-1.1.2/src/antaress/ANTARESS_conversions/ANTARESS_sp_cont.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/KitCat_main.py` & `antaress-1.1.2/src/antaress/ANTARESS_conversions/KitCat/KitCat_main.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/Kitcat_classes.py` & `antaress-1.1.2/src/antaress/ANTARESS_conversions/KitCat/Kitcat_classes.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/Kitcat_functions.py` & `antaress-1.1.2/src/antaress/ANTARESS_conversions/KitCat/Kitcat_functions.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/setup_lbl_fit.py` & `antaress-1.1.2/src/antaress/ANTARESS_conversions/KitCat/setup_lbl_fit.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_calib.py` & `antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_calib.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_detrend.py` & `antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_detrend.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_flux_balance.py` & `antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_flux_balance.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_interferences.py` & `antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_interferences.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_peaks.py` & `antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_peaks.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_sp_reduc.py` & `antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_sp_reduc.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_tellurics.py` & `antaress-1.1.2/src/antaress/ANTARESS_corrections/ANTARESS_tellurics.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_corrections/Telluric_processing/Create_static_files.py` & `antaress-1.1.2/src/antaress/ANTARESS_corrections/Telluric_processing/Create_static_files.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_general/constant_data.py` & `antaress-1.1.2/src/antaress/ANTARESS_general/constant_data.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_general/minim_routines.py` & `antaress-1.1.2/src/antaress/ANTARESS_general/minim_routines.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_general/utils.py` & `antaress-1.1.2/src/antaress/ANTARESS_general/utils.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_coord.py` & `antaress-1.1.2/src/antaress/ANTARESS_grids/ANTARESS_coord.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_occ_grid.py` & `antaress-1.1.2/src/antaress/ANTARESS_grids/ANTARESS_occ_grid.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_prof_grid.py` & `antaress-1.1.2/src/antaress/ANTARESS_grids/ANTARESS_prof_grid.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_star_grid.py` & `antaress-1.1.2/src/antaress/ANTARESS_grids/ANTARESS_star_grid.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_gridrun.py` & `antaress-1.1.2/src/antaress/ANTARESS_launch/ANTARESS_gridrun.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_launcher.py` & `antaress-1.1.2/src/antaress/ANTARESS_launch/ANTARESS_launcher.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_settings.py` & `antaress-1.1.2/src/antaress/ANTARESS_launch/ANTARESS_settings.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_systems.py` & `antaress-1.1.2/src/antaress/ANTARESS_launch/ANTARESS_systems.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_plots/ANTARESS_plot_settings.py` & `antaress-1.1.2/src/antaress/ANTARESS_plots/ANTARESS_plot_settings.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_plots/ANTARESS_plots_all.py` & `antaress-1.1.2/src/antaress/ANTARESS_plots/ANTARESS_plots_all.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_plots/utils_plots.py` & `antaress-1.1.2/src/antaress/ANTARESS_plots/utils_plots.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_data_align.py` & `antaress-1.1.2/src/antaress/ANTARESS_process/ANTARESS_data_align.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_data_process.py` & `antaress-1.1.2/src/antaress/ANTARESS_process/ANTARESS_data_process.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_main.py` & `antaress-1.1.2/src/antaress/ANTARESS_process/ANTARESS_main.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_plocc_spec.py` & `antaress-1.1.2/src/antaress/ANTARESS_process/ANTARESS_plocc_spec.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.1/src/antaress.egg-info/PKG-INFO` & `antaress-1.1.2/src/antaress.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antaress
-Version: 1.1.1
+Version: 1.1.2
 Summary: High-resolution spectroscopy pipeline
 Author-email: Vincent Bourrier <vincent.bourrier@unige.ch>
 Project-URL: Homepage, https://gitlab.unige.ch/bourrier/ANTARESS
 Project-URL: Issues, https://gitlab.unige.ch/bourrier/ANTARESS/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `antaress-1.1.1/src/antaress.egg-info/SOURCES.txt` & `antaress-1.1.2/src/antaress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

