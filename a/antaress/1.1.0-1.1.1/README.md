# Comparing `tmp/antaress-1.1.0.tar.gz` & `tmp/antaress-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antaress-1.1.0.tar", last modified: Fri May  3 19:52:22 2024, max compression
+gzip compressed data, was "antaress-1.1.1.tar", last modified: Thu May 23 14:06:59 2024, max compression
```

## Comparing `antaress-1.1.0.tar` & `antaress-1.1.1.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.128793 antaress-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-03 19:50:33.000000 antaress-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2063 2024-05-03 19:52:22.128793 antaress-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1101 2024-05-03 19:50:34.000000 antaress-1.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-03 19:50:34.000000 antaress-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 19:52:22.128793 antaress-1.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.105790 antaress-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.107791 antaress-1.1.0/src/antaress/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.113791 antaress-1.1.0/src/antaress/ANTARESS_analysis/
--rwxrwxrwx   0 root         (0) root         (0)   195099 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_analysis/ANTARESS_ana_comm.py
--rw-rw-rw-   0 root         (0) root         (0)    12027 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_analysis/ANTARESS_inst_resp.py
--rwxrwxrwx   0 root         (0) root         (0)     1247 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_analysis/ANTARESS_joined_atm.py
--rwxrwxrwx   0 root         (0) root         (0)    60997 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_analysis/ANTARESS_joined_star.py
--rw-rw-rw-   0 root         (0) root         (0)    24209 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_analysis/ANTARESS_model_prof.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_analysis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.117792 antaress-1.1.0/src/antaress/ANTARESS_conversions/
--rw-rw-rw-   0 root         (0) root         (0)   103488 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_conversions/ANTARESS_binning.py
--rw-rw-rw-   0 root         (0) root         (0)    50846 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_conversions/ANTARESS_conv.py
--rw-rw-rw-   0 root         (0) root         (0)    11472 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_conversions/ANTARESS_masks_gen.py
--rw-rw-rw-   0 root         (0) root         (0)    15598 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_conversions/ANTARESS_sp_cont.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.119792 antaress-1.1.0/src/antaress/ANTARESS_conversions/KitCat/
--rw-rw-rw-   0 root         (0) root         (0)    62059 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_conversions/KitCat/KitCat_main.py
--rw-rw-rw-   0 root         (0) root         (0)    22807 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_conversions/KitCat/Kitcat_classes.py
--rw-rw-rw-   0 root         (0) root         (0)     9261 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_conversions/KitCat/Kitcat_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_conversions/KitCat/setup_lbl_fit.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_conversions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.123792 antaress-1.1.0/src/antaress/ANTARESS_corrections/
--rw-rw-rw-   0 root         (0) root         (0)    29437 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_calib.py
--rw-rw-rw-   0 root         (0) root         (0)    53772 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_detrend.py
--rwxrwxrwx   0 root         (0) root         (0)    58484 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_flux_balance.py
--rwxrwxrwx   0 root         (0) root         (0)   254060 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_interferences.py
--rwxrwxrwx   0 root         (0) root         (0)    28412 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_peaks.py
--rwxrwxrwx   0 root         (0) root         (0)    15185 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_sp_reduc.py
--rwxrwxrwx   0 root         (0) root         (0)    50990 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_tellurics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.123792 antaress-1.1.0/src/antaress/ANTARESS_corrections/Telluric_processing/
--rw-rw-rw-   0 root         (0) root         (0)    58000 2024-05-03 19:50:34.000000 antaress-1.1.0/src/antaress/ANTARESS_corrections/Telluric_processing/Create_static_files.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_corrections/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.124792 antaress-1.1.0/src/antaress/ANTARESS_general/
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_general/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29812 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_general/constant_data.py
--rw-rw-rw-   0 root         (0) root         (0)   110123 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_general/minim_routines.py
--rwxrwxrwx   0 root         (0) root         (0)    30542 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_general/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.125793 antaress-1.1.0/src/antaress/ANTARESS_grids/
--rw-rw-rw-   0 root         (0) root         (0)    45505 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_grids/ANTARESS_coord.py
--rw-rw-rw-   0 root         (0) root         (0)    80236 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_grids/ANTARESS_plocc_grid.py
--rw-rw-rw-   0 root         (0) root         (0)    28205 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_grids/ANTARESS_prof_grid.py
--rw-rw-rw-   0 root         (0) root         (0)    70647 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_grids/ANTARESS_spots.py
--rw-rw-rw-   0 root         (0) root         (0)    22749 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_grids/ANTARESS_star_grid.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_grids/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.125793 antaress-1.1.0/src/antaress/ANTARESS_launch/
--rw-rw-rw-   0 root         (0) root         (0)     2356 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_launch/ANTARESS_gridrun.py
--rw-rw-rw-   0 root         (0) root         (0)     5409 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_launch/ANTARESS_launcher.py
--rw-rw-rw-   0 root         (0) root         (0)   191131 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_launch/ANTARESS_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    15931 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_launch/ANTARESS_systems.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_launch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.126793 antaress-1.1.0/src/antaress/ANTARESS_plots/
--rw-rw-rw-   0 root         (0) root         (0)    92327 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_plots/ANTARESS_plot_settings.py
--rwxrwxrwx   0 root         (0) root         (0)   633197 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_plots/ANTARESS_plots_all.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23987 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_plots/utils_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.127793 antaress-1.1.0/src/antaress/ANTARESS_process/
--rw-rw-rw-   0 root         (0) root         (0)     6378 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_process/ANTARESS_data_align.py
--rw-rw-rw-   0 root         (0) root         (0)   103192 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_process/ANTARESS_data_process.py
--rw-rw-rw-   0 root         (0) root         (0)   192213 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_process/ANTARESS_main.py
--rw-rw-rw-   0 root         (0) root         (0)    38212 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_process/ANTARESS_plocc_spec.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/ANTARESS_process/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-03 19:50:35.000000 antaress-1.1.0/src/antaress/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 19:52:22.127793 antaress-1.1.0/src/antaress.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2063 2024-05-03 19:52:22.000000 antaress-1.1.0/src/antaress.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2727 2024-05-03 19:52:22.000000 antaress-1.1.0/src/antaress.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 19:52:22.000000 antaress-1.1.0/src/antaress.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2024-05-03 19:52:22.000000 antaress-1.1.0/src/antaress.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      151 2024-05-03 19:52:22.000000 antaress-1.1.0/src/antaress.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-03 19:52:22.000000 antaress-1.1.0/src/antaress.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.612913 antaress-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-23 14:05:30.000000 antaress-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2063 2024-05-23 14:06:59.612913 antaress-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2024-05-23 14:05:30.000000 antaress-1.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-23 14:05:30.000000 antaress-1.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 14:06:59.612913 antaress-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      298 2024-05-23 14:05:30.000000 antaress-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.589911 antaress-1.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.591911 antaress-1.1.1/src/antaress/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.596912 antaress-1.1.1/src/antaress/ANTARESS_analysis/
+-rwxrwxrwx   0 root         (0) root         (0)   205187 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_ana_comm.py
+-rw-rw-rw-   0 root         (0) root         (0)    12027 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_inst_resp.py
+-rwxrwxrwx   0 root         (0) root         (0)     1247 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_joined_atm.py
+-rwxrwxrwx   0 root         (0) root         (0)    90944 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_joined_star.py
+-rw-rw-rw-   0 root         (0) root         (0)    24209 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_model_prof.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.597912 antaress-1.1.1/src/antaress/ANTARESS_analysis/C_grid/
+-rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/C_grid/Gauss_star_grid.c
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_analysis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.599912 antaress-1.1.1/src/antaress/ANTARESS_conversions/
+-rw-rw-rw-   0 root         (0) root         (0)   104496 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_binning.py
+-rw-rw-rw-   0 root         (0) root         (0)    50846 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_conv.py
+-rw-rw-rw-   0 root         (0) root         (0)    11472 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_masks_gen.py
+-rw-rw-rw-   0 root         (0) root         (0)    15598 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_sp_cont.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.601912 antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/
+-rw-rw-rw-   0 root         (0) root         (0)    62059 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/KitCat_main.py
+-rw-rw-rw-   0 root         (0) root         (0)    22807 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/Kitcat_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9261 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/Kitcat_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/setup_lbl_fit.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_conversions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.607913 antaress-1.1.1/src/antaress/ANTARESS_corrections/
+-rw-rw-rw-   0 root         (0) root         (0)    29437 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_calib.py
+-rw-rw-rw-   0 root         (0) root         (0)    53772 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_detrend.py
+-rwxrwxrwx   0 root         (0) root         (0)    58484 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_flux_balance.py
+-rwxrwxrwx   0 root         (0) root         (0)   254034 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_interferences.py
+-rwxrwxrwx   0 root         (0) root         (0)    28412 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_peaks.py
+-rwxrwxrwx   0 root         (0) root         (0)    15185 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_sp_reduc.py
+-rwxrwxrwx   0 root         (0) root         (0)    50990 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_tellurics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.607913 antaress-1.1.1/src/antaress/ANTARESS_corrections/Telluric_processing/
+-rw-rw-rw-   0 root         (0) root         (0)    58000 2024-05-23 14:05:30.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/Telluric_processing/Create_static_files.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_corrections/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.608913 antaress-1.1.1/src/antaress/ANTARESS_general/
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_general/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27026 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_general/constant_data.py
+-rw-rw-rw-   0 root         (0) root         (0)   111761 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_general/minim_routines.py
+-rwxrwxrwx   0 root         (0) root         (0)    30542 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_general/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.609913 antaress-1.1.1/src/antaress/ANTARESS_grids/
+-rw-rw-rw-   0 root         (0) root         (0)    45505 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_coord.py
+-rw-rw-rw-   0 root         (0) root         (0)   117508 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_occ_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)    33059 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_prof_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)    22950 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_star_grid.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_grids/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.610913 antaress-1.1.1/src/antaress/ANTARESS_launch/
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_gridrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     5749 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_launcher.py
+-rw-rw-rw-   0 root         (0) root         (0)   192615 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    15931 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_systems.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_launch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.611914 antaress-1.1.1/src/antaress/ANTARESS_plots/
+-rw-rw-rw-   0 root         (0) root         (0)    92437 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_plots/ANTARESS_plot_settings.py
+-rwxrwxrwx   0 root         (0) root         (0)   647371 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_plots/ANTARESS_plots_all.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25189 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_plots/utils_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.612913 antaress-1.1.1/src/antaress/ANTARESS_process/
+-rw-rw-rw-   0 root         (0) root         (0)     6378 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_data_align.py
+-rw-rw-rw-   0 root         (0) root         (0)   106409 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_data_process.py
+-rw-rw-rw-   0 root         (0) root         (0)   193806 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_main.py
+-rw-rw-rw-   0 root         (0) root         (0)    45382 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_plocc_spec.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/ANTARESS_process/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       47 2024-05-23 14:05:32.000000 antaress-1.1.1/src/antaress/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:06:59.612913 antaress-1.1.1/src/antaress.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2063 2024-05-23 14:06:59.000000 antaress-1.1.1/src/antaress.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2744 2024-05-23 14:06:59.000000 antaress-1.1.1/src/antaress.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 14:06:59.000000 antaress-1.1.1/src/antaress.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-23 14:06:59.000000 antaress-1.1.1/src/antaress.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2024-05-23 14:06:59.000000 antaress-1.1.1/src/antaress.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-23 14:06:59.000000 antaress-1.1.1/src/antaress.egg-info/top_level.txt
```

### Comparing `antaress-1.1.0/LICENSE` & `antaress-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/PKG-INFO` & `antaress-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antaress
-Version: 1.1.0
+Version: 1.1.1
 Summary: High-resolution spectroscopy pipeline
 Author-email: Vincent Bourrier <vincent.bourrier@unige.ch>
 Project-URL: Homepage, https://gitlab.unige.ch/bourrier/ANTARESS
 Project-URL: Issues, https://gitlab.unige.ch/bourrier/ANTARESS/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `antaress-1.1.0/README.md` & `antaress-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/pyproject.toml` & `antaress-1.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools >= 61.0", "wheel", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "antaress"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name = "Vincent Bourrier", email = "vincent.bourrier@unige.ch" },
 ]
 description = "High-resolution spectroscopy pipeline"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_analysis/ANTARESS_ana_comm.py` & `antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_ana_comm.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 import lmfit
 import numpy as np
 import bindensity as bind
 from ..ANTARESS_general.utils import stop,np_where1D,npint,dataload_npz,gen_specdopshift,closest,def_edge_tab,check_data
 from ..ANTARESS_general.minim_routines import init_fit,call_MCMC,postMCMCwrapper_1,postMCMCwrapper_2,save_fit_results,fit_merit,call_lmfit,gen_hrand_chain
 from ..ANTARESS_general.constant_data import Rsun,c_light
 from ..ANTARESS_grids.ANTARESS_star_grid import calc_CB_RV,get_LD_coeff
-# from ..ANTARESS_grids.ANTARESS_plocc_grid import sub_calc_plocc_spot_prop,up_plocc_prop
-from ..ANTARESS_grids.ANTARESS_prof_grid import init_custom_DI_par,init_custom_DI_prof,custom_DI_prof,theo_intr2loc
+from ..ANTARESS_grids.ANTARESS_occ_grid import sub_calc_plocc_spot_prop,up_plocc_prop
+from ..ANTARESS_grids.ANTARESS_prof_grid import init_custom_DI_par,init_custom_DI_prof,custom_DI_prof,theo_intr2loc,def_Cfunc_prof
 from ..ANTARESS_analysis.ANTARESS_model_prof import para_cust_mod_true_prop,proc_cust_mod_true_prop,cust_mod_true_prop,gauss_intr_prop,calc_biss,\
     dgauss,gauss_poly,voigt,gauss_herm_lin,gen_fit_prof
-from ..ANTARESS_analysis.ANTARESS_inst_resp import calc_FWHM_inst
-from ..ANTARESS_analysis.ANTARESS_inst_resp import convol_prof,def_st_prof_tab,cond_conv_st_prof_tab,resamp_st_prof_tab,get_FWHM_inst
+from ..ANTARESS_analysis.ANTARESS_inst_resp import convol_prof,def_st_prof_tab,cond_conv_st_prof_tab,resamp_st_prof_tab,get_FWHM_inst,calc_FWHM_inst
 from ..ANTARESS_grids.ANTARESS_coord import excl_plrange
 
 
 ##################################################################################################    
 #%%% Definition functions
 ################################################################################################## 
 
@@ -91,15 +90,18 @@
 
         #Variable parameter
         if fit_used and (par in p_start) and p_start[par].vary:
             
             #Chi2 fit
             #    - overwrite default priors
             if (fit_dic['fit_mode']=='chi2'):
-                if (par in priors_prop) and (priors_prop[par]['mod']=='uf'): 
+                if (par in priors_prop) and (priors_prop[par]['mod']=='uf'):
+                    if ('ang' in par) and (priors_prop[par]['high']>90):stop('Prior error: Spot angular size cannot exceed 90 deg. Re-define your priors.')
+                    elif ('veq' in par) and (priors_prop[par]['low']<0):stop('Prior error: Cannot have negative stellar rotation velocity. Re-define your priors.')
+                    elif ('Tcenter' in par) and ((priors_prop[par]['low'] <= p_start[par].value - fixed_args['Peq']) or (priors_prop[par]['high'] >= p_start[par].value + fixed_args['Peq'])):stop('Prior error: Spot crossing time priors should be less/more than the rotational period to avoid aliases.')
                     p_start[par].min = priors_prop[par]['low']
                     p_start[par].max = priors_prop[par]['high']
 
                 #Change guess value if beyond prior range
                 if (not np.isinf(p_start[par].min)) and (np.isinf(p_start[par].max)) and (p_start[par].value<p_start[par].min):p_start[par].value=p_start[par].min
                 if (np.isinf(p_start[par].min)) and (not np.isinf(p_start[par].max)) and (p_start[par].value>p_start[par].max):p_start[par].value=p_start[par].max
                 if (not np.isinf(p_start[par].min)) and (not np.isinf(p_start[par].max)) and ((p_start[par].value<p_start[par].min) or (p_start[par].value>p_start[par].max)):p_start[par].value=0.5*(p_start[par].min+p_start[par].max)
@@ -110,20 +112,29 @@
                 #Range for walkers initialization
                 if (par in model_prop):fit_dic['uf_bd'][par]=model_prop_par['bd']
                 else:
                     uf_bd=[-1e6,1e6]
                     if (not np.isinf(p_start[par].min)):uf_bd[0]=p_start[par].min
                     if (not np.isinf(p_start[par].max)):uf_bd[1]=p_start[par].max
                     fit_dic['uf_bd'][par]=uf_bd
+                if 'ang' in par and fit_dic['uf_bd'][par][1]>90:fit_dic['uf_bd'][par][1]=90
+                elif 'veq' in par and fit_dic['uf_bd'][par][0]<0:fit_dic['uf_bd'][par][0]=0
+                elif ('Tcenter' in par) and ((fit_dic['uf_bd'][par][0] <= p_start[par].value - fixed_args['Peq']) or (fit_dic['uf_bd'][par][1] >= p_start[par].value + fixed_args['Peq'])):fit_dic['uf_bd'][par] = [p_start[par].value - fixed_args['Peq'] + 0.001, p_start[par].value + fixed_args['Peq'] - 0.001]
                 
                 #Priors
                 if (par in priors_prop):
-                    fixed_args['varpar_priors'][par] = priors_prop[par]                          
+                    fixed_args['varpar_priors'][par] = priors_prop[par]    
+                    if 'ang' in par and priors_prop[par]['high']>90:stop('Prior error: Spot angular size cannot exceed 90deg. Re-define your priors.')
+                    elif 'veq' in par and priors_prop[par]['low']<0:stop('Prior error: Cannot have negative stellar rotation velocity. Re-define your priors.')
+                    elif ('Tcenter' in par) and ((priors_prop[par]['low'] <= p_start[par].value - fixed_args['Peq']) or (priors_prop[par]['high'] >= p_start[par].value + fixed_args['Peq'])):stop('Prior error: Spot crossing time priors should be less/more than the rotational period to avoid aliases.')
                 else:
                     if par == 'jitter':varpar_priors=[0.,1e6]
+                    elif par == 'veq':varpar_priors=[0.,100.]
+                    elif 'ang' in par:varpar_priors=[0.,90.]
+                    elif 'Tcenter' in par:varpar_priors=[p_start[par].value - fixed_args['Peq'] + 0.001, p_start[par].value + fixed_args['Peq'] - 0.001]
                     else:varpar_priors=[-1e6,1e6]
                     if (not np.isinf(p_start[par].min)):varpar_priors[0]=p_start[par].min
                     if (not np.isinf(p_start[par].max)):varpar_priors[1]=p_start[par].max                
                     fixed_args['varpar_priors'][par]={'mod':'uf','low':varpar_priors[0],'high':varpar_priors[1]}
              
                 #Change if guess value is beyond prior range
                 if fixed_args['varpar_priors'][par]['mod']=='uf':
@@ -229,27 +240,27 @@
                                 par_input = root_par+'__IS'+inst+'_VS'+vis 
                                 fixed_args['name_prop2input'][par_input] = root_par+'__IS'+inst+'_VS'+vis   
                                 if deg_coeff is not None:fixed_args['coeff_ord2name'][inst][vis][gen_root_par][deg_coeff]=root_par+'__IS'+inst+'_VS'+vis  
        
     return p_start
 
 
-def model_par_names():
+def model_par_names(par):
     r"""**Naming function**
 
-    Returns dictionary associating plain name to variable.
+    Returns name and unit of input variable for plot display.
 
     Args:
         None
 
     Returns:
-        name_dic (dict): dictionary of names
+        name_par (str): parameter name
 
     Example:
-        >>> model_par_names()[x]
+        >>> model_par_names(x)
         x_name
         
     """
     name_dic = {
         'veq':'v$_\mathrm{eq}$ (km s$^{-1}$)','vsini':'v$_\mathrm{eq}$sin i$_{*}$ (km/s)',
         'Peq':'P$_\mathrm{eq}$ (d)',
         'alpha_rot':r'$\alpha_\mathrm{rot}$','beta_rot':r'$\beta_\mathrm{rot}$',       
@@ -268,19 +279,64 @@
         'FWHM':'FWHM (km/s)',
         'rv_l2c':'RV$_{l}$-RV$_{c}$','amp_l2c':'A$_{l}$/A$_{c}$','FWHM_l2c':'FWHM$_{l}$/FWHM$_{c}$',
         'cont':'P$_\mathrm{cont}$',
         'c1_pol':'c$_1$','c2_pol':'c$_2$','c3_pol':'c$_3$','c4_pol':'c$_4$',
         'LD_u1':'LD$_1$','LD_u2':'LD$_2$','LD_u3':'LD$_3$','LD_u4':'LD$_4$',
         'f_GD':'f$_{\rm GD}$','beta_GD':'$\beta_{\rm GD}$','Tpole':'T$_{\rm pole}$',
         'eta_R':r'$\eta_{\rm R}$','eta_T':r'$\eta_{\rm T}$','ksi_R':r'\Ksi$_\mathrm{R}$','ksi_T':r'\Ksi$_\mathrm{T}$',
-        'Tcenter' : 'T$_{sp}$', 'ang' : r'$\alpha_{sp}$', 'lat' : 'lat$_{sp}$', 'ctrst_sp' : 'F$_{sp}$',
+        'Tcenter' : 'T$_{sp}$', 'ang' : r'$\alpha_{sp}$', 'lat' : 'lat$_{sp}$', 'Fctrst' : 'F$_{sp}$',
         } 
-    return name_dic
+    if par in name_dic:name_par = name_dic[par]
+    else:name_par = par
+    return name_par
 
+def model_par_units(par):
+    r"""**Unit function**
 
+    Returns plain text unit of input variable.
+
+    Args:
+        None
+
+    Returns:
+        unit_par (str): parameter unit
+
+    Example:
+        >>> model_par_units(x)
+        x_name
+        
+    """
+    unit_dic = {
+        'veq':'km/s','vsini':'km/s',
+        'Peq':'d',
+        'alpha_rot':'','beta_rot':'',       
+        'cos_istar':'','istar_deg':'deg',
+        'lambda_rad':'rad', 
+        'c1_CB':'km/s','c2_CB':'km/s','c3_CB':'km/s',  
+        'inclination':'deg','inclin_rad':'rad',
+        'aRs':'',
+        'Rstar':'Rsun',
+        'ctrst':'','ctrst_ord0':'','ctrst_ord1':'','ctrst_ord2':'','ctrst_ord3':'','ctrst_ord4':'', 
+        'FWHM_ord0':'km/s','FWHM_ord1':'km/s','FWHM_ord2':'km/s','FWHM_ord3':'km/s','FWHM_ord4':'km/s',
+        'FWHM_LOR':'km/s',
+        'a_damp':'',
+        'amp':'',
+        'rv':'km/s',
+        'FWHM':'km/s',
+        'rv_l2c':'km/s','amp_l2c':'','FWHM_l2c':'',
+        'cont':'',
+        'c1_pol':'','c2_pol':'','c3_pol':'','c4_pol':'',
+        'LD_u1':'','LD_u2':'','LD_u3':'LD$_3$','LD_u4':'LD$_4$',
+        'f_GD':'f$_{\rm GD}$','beta_GD':'$\beta_{\rm GD}$','Tpole':'T$_{\rm pole}$',
+        'eta_R':r'$\eta_{\rm R}$','eta_T':r'$\eta_{\rm T}$','ksi_R':r'\Ksi$_\mathrm{R}$','ksi_T':r'\Ksi$_\mathrm{T}$',
+        'Tcenter' : 'BJD',
+        } 
+    if par in unit_dic:unit_par = unit_dic[par]
+    else:unit_par = ''
+    return unit_par
 
 
 
 ##################################################################################################    
 #%%% Initialization functions
 ################################################################################################## 
 
@@ -296,57 +352,69 @@
         TBD
     
     """
     
     #Fit dictionary
     fit_dic={
         'merit':{},
+        'verbose':fit_prop_dic['verbose'],
+        'verb_shift':'   ',
+        'print_par':fit_prop_dic['print_par'],
         'fit_mode':fit_prop_dic['fit_mode'],
         'uf_bd':{},
         'nx_fit':0,
         'run_name':'_'+gen_dic['main_pl_text'],
         'save_dir' : gen_dic['save_data_dir']+'/Joined_fits/'+data_mode+'/'+fit_prop_dic['fit_mode']+'/'}
     
     #--------------------------------------------------------------------------------
 
     #Arguments to be passed to the fit function
     fixed_args={
             
         #Global model properties        
         'system_param':deepcopy(system_param),
-        'system_prop':deepcopy(data_dic['DI']['system_prop']), 
+        'system_prop':deepcopy(data_dic['DI']['system_prop']),
         'system_spot_prop':deepcopy(data_dic['DI']['spots_prop']), 
         'DI_grid':False,
         'coord_line':fit_prop_dic['dim_fit'],
         'pol_mode':fit_prop_dic['pol_mode'],
 
         #Fit parameters
         'par_list':[],
         
         #Exposures to be fitted
         'nexp_fit_all':{},
-        'idx_in_fit':{},
-        
+        'idx_in_fit':{},        
+        'master_out':{},
+
         #Intrinsic continuum flux
         #    - IntrProp: required for the intensity weighing but absolute value does not matter
         #    - IntrProf: required for parameter initialization, but set within the fit function to the visit-specific flux
         'flux_cont':1.,     
         
         
         'inst_list':[],
         'prior_func':fit_prop_dic['prior_func'], 
         'inst_vis_list':{},
         'transit_pl':{},
+        'cond_transit_pl':False,
         'transit_sp':{},
+        'cond_transit_sp':False,
         'bin_mode':{},
-        'fit' : {'chi2':True,'':False,'mcmc':True}[fit_prop_dic['fit_mode']],     
+        'update_crosstime':False,
+        'fit' : {'chi2':True,'':False,'mcmc':True}[fit_prop_dic['fit_mode']], 
+        'unthreaded_op':fit_prop_dic['unthreaded_op'],     
         }
    
     #Checks
     if len(fit_prop_dic['idx_in_fit'])==0:stop('No exposures are included in the fit')
+    
+    #Initializes C-based profile calculation
+    if 1==0:
+        fixed_args['fun_to_use'],fixed_args['fun_to_free'] = def_Cfunc_prof()
 
     return fixed_args,fit_dic
 
 def init_joined_routines_inst(rout_mode,inst,fit_prop_dic,fixed_args):
     r"""**Joined fits: instrument initialization.**
 
     Initializes properties for the joined fits to stellar and planetary lines.
@@ -361,16 +429,15 @@
     
     """
     #Instrument is fitted
     fit_prop_dic[inst]={}
     fixed_args['inst_list']+=[inst]
     fixed_args['inst_vis_list'][inst]=[]  
     for key in ['ph_fit','nexp_fit_all','transit_pl','transit_sp','bin_mode','idx_in_fit']:fixed_args[key][inst]={}
-    if ('Intr' in rout_mode) or ('Res' in rout_mode):fixed_args['coord_pl_fit'][inst]={}
-    if ('Prof' in rout_mode):fixed_args['coord_spot_fit'][inst]={}
+    if ('Intr' in rout_mode) or ('Res' in rout_mode):fixed_args['coord_fit'][inst]={}
 
     return None
 
 def init_joined_routines_vis(inst,vis,fit_prop_dic,fixed_args):
     r"""**Joined fits: visit initialization.**
 
     Initializes properties for the joined fits to stellar and planetary lines.
@@ -402,62 +469,84 @@
         TBD
     
     Returns:
         TBD
     
     """
     fit_prop_dic[inst][vis]={}
-    
-    #Check for multi-transits
-    #    - if two planets are transiting the properties derived from the fits to intrinsic profiles cannot be fitted, as the model only contains a single line profile
-    if rout_mode=='IntrProp':
-        if len(data_vis['transit_pl'])>1:stop('Multi-planet transit must be modelled with full intrinsic profiles')
-        fixed_args['transit_pl'][inst][vis]=[data_vis['transit_pl'][0]] 
-    else:fixed_args['transit_pl'][inst][vis]=data_vis['transit_pl'] 
-    # if ('Prof' in rout_mode):fixed_args['transit_sp'][inst][vis]=data_vis['transit_sp']
 
     #Binned data
     if fixed_args['bin_mode'][inst][vis]=='_bin':
-        data_vis_bin = dataload_npz(gen_dic['save_data_dir']+'/Intrbin_data/'+inst+'_'+vis+'_'+data_dic['Intr']['dim_bin']+'_add')
+        if 'Intr' in fixed_args['rout_mode']:data_vis_bin = dataload_npz(gen_dic['save_data_dir']+'/Intrbin_data/'+inst+'_'+vis+'_'+data_dic['Intr']['dim_bin']+'_add')
+        elif 'Res' in fixed_args['rout_mode']:data_vis_bin = dataload_npz(gen_dic['save_data_dir']+'/Resbin_data/'+inst+'_'+vis+'_'+data_dic['Res']['dim_bin']+'_add')  
+        data_mode = data_vis_bin['type']      
         n_in_tr = data_vis_bin['n_in_tr']
+        n_in_visit = data_vis_bin['n_in_visit']
 
     #Original data
     else:
         data_vis_bin = None
         n_in_tr = data_vis['n_in_tr']    
-    
+        n_in_visit = data_vis['n_in_visit']
+        data_mode = data_dic[inst][vis]['type']
+        
+    #Planets are transiting
+    if len(data_vis['transit_pl'] )>0:
+        fixed_args['cond_transit_pl'] = True
+        
+        #Check for multi-transits
+        #    - if two planets are transiting the properties derived from the fits to intrinsic profiles cannot be fitted, as the model only contains a single line profile
+        if rout_mode=='IntrProp':
+            if len(data_vis['transit_pl'])>1:stop('Multi-planet transit must be modelled with full intrinsic profiles')
+            fixed_args['transit_pl'][inst][vis]=[data_vis['transit_pl'][0]] 
+        else:fixed_args['transit_pl'][inst][vis]=data_vis['transit_pl'] 
+        fixed_args['transit_pl'][inst][vis]=data_vis['transit_pl'] 
+
+    #Spots are visible
+    if len(data_vis['transit_sp'] )>0:
+        fixed_args['cond_transit_sp'] = True    
+        fixed_args['transit_sp'][inst][vis]=data_vis['transit_sp']
+        
     #Fitted exposures
+    if rout_mode in ['DIprof', 'ResProf']:n_default_fit = n_in_visit
+    else: n_default_fit = n_in_tr
     fixed_args['inst_vis_list'][inst]+=[vis]
-    if fit_prop_dic['idx_in_fit'][inst][vis]=='all':fixed_args['idx_in_fit'][inst][vis]=range(n_in_tr)
-    else:fixed_args['idx_in_fit'][inst][vis]=np.intersect1d(fit_prop_dic['idx_in_fit'][inst][vis],range(n_in_tr))
-    
-    #Keep defined intrinsic profiles
-    if 'Intr' in rout_mode:fixed_args['idx_in_fit'][inst][vis]=np.intersect1d(fixed_args['idx_in_fit'][inst][vis],data_dic['Intr'][inst][vis+fixed_args['bin_mode'][inst][vis]]['idx_def'])
+    if fit_prop_dic['idx_in_fit'][inst][vis]=='all':fixed_args['idx_in_fit'][inst][vis]=range(n_default_fit)
+    else:fixed_args['idx_in_fit'][inst][vis]=np.intersect1d(fit_prop_dic['idx_in_fit'][inst][vis],range(n_default_fit))
+
+    #Keep defined profiles
+    if (data_mode in ['Intr','Res']):fixed_args['idx_in_fit'][inst][vis]=np.intersect1d(fixed_args['idx_in_fit'][inst][vis],data_dic[data_mode][inst][vis+fixed_args['bin_mode'][inst][vis]]['idx_def'])
     fixed_args['nexp_fit_all'][inst][vis]=len(fixed_args['idx_in_fit'][inst][vis])     
 
     #Store coordinates of fitted exposures in global table
     if fixed_args['bin_mode'][inst][vis]=='_bin':
         sub_idx_in_fit = fixed_args['idx_in_fit'][inst][vis]
         coord_vis = data_vis_bin['coord']
     else:
-        sub_idx_in_fit = gen_dic[inst][vis]['idx_in'][fixed_args['idx_in_fit'][inst][vis]]
+        if rout_mode=='ResProf':sub_idx_in_fit = fixed_args['idx_in_fit'][inst][vis]        
+        else:sub_idx_in_fit = gen_dic[inst][vis]['idx_in'][fixed_args['idx_in_fit'][inst][vis]]
         coord_vis = coord_dic[inst][vis]
-    for par in ['coord_pl_fit','ph_fit']:fixed_args[par][inst][vis]={}
-    for pl_loc in fixed_args['transit_pl'][inst][vis]:
-        fixed_args['ph_fit'][inst][vis][pl_loc] = np.vstack((coord_vis[pl_loc]['st_ph'][sub_idx_in_fit],coord_vis[pl_loc]['cen_ph'][sub_idx_in_fit],coord_vis[pl_loc]['end_ph'][sub_idx_in_fit]) ) 
-        fixed_args['coord_pl_fit'][inst][vis][pl_loc] = {}
-        for key in ['cen_pos','st_pos','end_pos']:fixed_args['coord_pl_fit'][inst][vis][pl_loc][key] = coord_vis[pl_loc][key][:,sub_idx_in_fit]    
-        fixed_args['coord_pl_fit'][inst][vis][pl_loc]['ecl'] = coord_vis[pl_loc]['ecl'][sub_idx_in_fit]    
-    # if ('Prof' in rout_mode):
-    #     fixed_args['coord_spot_fit'][inst][vis]={}
-    #     for spot in fixed_args['transit_sp'][inst][vis]:
-    #         fixed_args['coord_spot_fit'][inst][vis][spot] = {}
-    #         for key in ['cen_pos','st_pos','end_pos']:fixed_args['coord_spot_fit'][inst][vis][spot][key] = coord_vis[spot][key][:,sub_idx_in_fit]
-    #         for key in ['cen_tbjd','st_tbjd','end_tbjd']:fixed_args['coord_spot_fit'][inst][vis][spot][key]=coord_vis[spot][key][sub_idx_in_fit] 
-
+    for par in ['coord_fit','ph_fit']:fixed_args[par][inst][vis]={}
+    if fixed_args['cond_transit_pl']:
+        for pl_loc in fixed_args['transit_pl'][inst][vis]:
+            fixed_args['ph_fit'][inst][vis][pl_loc] = np.vstack((coord_vis[pl_loc]['st_ph'][sub_idx_in_fit],coord_vis[pl_loc]['cen_ph'][sub_idx_in_fit],coord_vis[pl_loc]['end_ph'][sub_idx_in_fit]) ) 
+            fixed_args['coord_fit'][inst][vis][pl_loc] = {}
+            for key in ['cen_pos','st_pos','end_pos']:fixed_args['coord_fit'][inst][vis][pl_loc][key] = coord_vis[pl_loc][key][:,sub_idx_in_fit]    
+            fixed_args['coord_fit'][inst][vis][pl_loc]['ecl'] = coord_vis[pl_loc]['ecl'][sub_idx_in_fit]  
+    if fixed_args['cond_transit_sp']:
+        for spot in fixed_args['transit_sp'][inst][vis]:
+            fixed_args['coord_fit'][inst][vis][spot] = {}
+            for key in ['Tcenter', 'ang', 'ang_rad', 'lat', 'ctrst']:
+                fixed_args['coord_fit'][inst][vis][spot][key] = coord_vis[spot][key][sub_idx_in_fit] 
+            for key in ['lat_rad_exp','sin_lat_exp','cos_lat_exp','long_rad_exp','sin_long_exp','cos_long_exp','x_sky_exp','y_sky_exp','z_sky_exp']:
+                fixed_args['coord_fit'][inst][vis][spot][key] = coord_vis[spot][key][:,sub_idx_in_fit] 
+            fixed_args['coord_fit'][inst][vis][spot]['is_visible'] = coord_vis[spot]['is_visible'][:,sub_idx_in_fit] 
+        fixed_args['coord_fit'][inst][vis]['bjd']=coord_vis['bjd'][sub_idx_in_fit]
+        fixed_args['coord_fit'][inst][vis]['t_dur']=coord_vis['t_dur'][sub_idx_in_fit]
+    
     return data_vis_bin
     
     
 
 
 
 ##################################################################################################    
@@ -529,95 +618,128 @@
     p_start = init_custom_DI_par(fixed_args,gen_dic,data_dic['DI']['system_prop'],fixed_args['system_param']['star'],p_start,[0.,None,None])
 
     #Condition to calculate CB
     if ('c1_CB' in mod_prop) or ('c2_CB' in mod_prop)  or ('c3_CB' in mod_prop):fixed_args['par_list']+=['CB_RV']
     
     #Fit spin-orbit angle by default when relevant
     #    - assuming common values to all datasets
-    if ((fixed_args['rout_mode']=='IntrProp') and (fixed_args['prop_fit']=='rv')) or (rout_mode=='IntrProf'):
+    if ((rout_mode=='IntrProp') and (fixed_args['prop_fit']=='rv')) or (rout_mode in ['IntrProf','ResProf']):
         for pl_loc in gen_dic['studied_pl']:
             if 'lambda_rad__pl'+pl_loc not in mod_prop:p_start.add_many(('lambda_rad__pl'+pl_loc, 0.,   True, -2.*np.pi,2.*np.pi,None))
         
     #Initialize line properties
     #    - using Gaussian line as default for intrinsic profiles
-    if ((fixed_args['rout_mode']=='IntrProp') and (fixed_args['prop_fit']=='ctrst')) or (rout_mode=='IntrProf'):    
+    if ((rout_mode=='IntrProp') and (fixed_args['prop_fit']=='ctrst')) or (rout_mode in ['IntrProf','ResProf']):
         if not any(['ctrst_' in prop for prop in mod_prop]):p_start.add_many(('ctrst_ord0__IS__VS_', 0.5,   True, 0.,1.  ,None))
-    if ((fixed_args['rout_mode']=='IntrProp') and (fixed_args['prop_fit']=='FWHM')) or (rout_mode=='IntrProf'):    
+    if ((rout_mode=='IntrProp') and (fixed_args['prop_fit']=='FWHM')) or (rout_mode in ['IntrProf','ResProf']):
         if not any(['FWHM_' in prop for prop in mod_prop]):p_start.add_many(('FWHM_ord0__IS__VS_', 5.,   True, 0.,100.  ,None))
         
+    #Re-defining the spot's Tcenter bounds, guess and priors with the cross-time supplement
+    if fixed_args['update_crosstime']:
+        for inst in list(fixed_args['spot_crosstime_supp'].keys()):
+            for vis in list(fixed_args['spot_crosstime_supp'][inst].keys()):
+                for par in mod_prop:
+                    if ('Tcenter' in par) and (inst in par) and (vis in par):
+                        mod_prop[par]['guess'] -= fixed_args['spot_crosstime_supp'][inst][vis]
+                        mod_prop[par]['bd'] = list(np.array(mod_prop[par]['bd']))-fixed_args['spot_crosstime_supp'][inst][vis]
+                        fit_prop_dic['priors'][par]['low'] -= fixed_args['spot_crosstime_supp'][inst][vis]
+                        fit_prop_dic['priors'][par]['high'] -= fixed_args['spot_crosstime_supp'][inst][vis]
+    
+    #Retrieving the rotational period - to set the priors on the Tcenter and prevent aliases
+    #    - in days
+    if 'veq' in mod_prop:fixed_args['Peq'] = (2*np.pi*fixed_args['system_param']['star']['Rstar_km'])/(mod_prop['veq']['guess']*24*3600)
+    else:fixed_args['Peq'] = deepcopy(fixed_args['system_param']['star']['Peq'])
+        
     #Initializing stellar properties
-    if fixed_args['rout_mode']=='IntrProp':    
+    if rout_mode=='IntrProp':    
         fixed_args['grid_dic'] = deepcopy(theo_dic)
         fixed_args['grid_dic']['precision'] = 'low'      #to calculate intensity-weighted properties
         line_type='ana'                                  #to avoid raising warning, even though properties are not used to calculate a line profile
 
     #Initializing stellar profiles
     else: line_type = fixed_args['mode']
 
     #Parameter initialization
     #    - default system properties are overwritten in p_start if they are defined in 'mod_prop', whether the model is fitted or called in forward mode
     p_start = par_formatting(p_start,mod_prop,fit_prop_dic['priors'],fit_dic,fixed_args,'','',line_type)
    
     #Initializing stellar profile grid
     #    - must be done after 'par_formatting' to identify variable line parameters
-    if fixed_args['rout_mode']!='IntrProp':       
-        fixed_args = init_custom_DI_prof(fixed_args,gen_dic,data_dic['DI']['system_prop'],{},theo_dic,fixed_args['system_param']['star'],p_start)
-    
+    if rout_mode!='IntrProp':  
+        if fixed_args['cond_transit_sp']:     
+            fixed_args = init_custom_DI_prof(fixed_args,gen_dic,data_dic['DI']['system_prop'],data_dic['DI']['spots_prop'],theo_dic,fixed_args['system_param']['star'],p_start)
+        else:
+            fixed_args = init_custom_DI_prof(fixed_args,gen_dic,data_dic['DI']['system_prop'],{},theo_dic,fixed_args['system_param']['star'],p_start)
+
     #Stellar grid properties
-    fixed_args['grid_dic'].update({'Ssub_Sstar_pl':theo_dic['Ssub_Sstar_pl'],'x_st_sky_grid_pl':theo_dic['x_st_sky_grid_pl'],'y_st_sky_grid_pl':theo_dic['y_st_sky_grid_pl'],'nsub_Dpl':theo_dic['nsub_Dpl'],'d_oversamp':theo_dic['d_oversamp'],'Istar_norm_achrom':theo_dic['Istar_norm_achrom']})             
+    fixed_args['grid_dic'].update({'Ssub_Sstar_pl':theo_dic['Ssub_Sstar_pl'],'x_st_sky_grid_pl':theo_dic['x_st_sky_grid_pl'],'y_st_sky_grid_pl':theo_dic['y_st_sky_grid_pl'],'nsub_Dpl':theo_dic['nsub_Dpl'],'d_oversamp':theo_dic['d_oversamp'],'Istar_norm_achrom':theo_dic['Istar_norm_achrom']})
+    if fixed_args['cond_transit_sp']:
+        fixed_args['grid_dic'].update({'Ssub_Sstar_sp':theo_dic['Ssub_Sstar_sp'],'x_st_sky_grid_sp':theo_dic['x_st_sky_grid_sp'],'y_st_sky_grid_sp':theo_dic['y_st_sky_grid_sp'],'nsub_Dspot':theo_dic['nsub_Dspot'],'d_oversamp_spot':theo_dic['d_oversamp_spot']})
 
     #Determine if orbital and light curve properties are fitted or whether nominal values are used
     #    - this depends on whether parameters required to calculate coordinates of planet-occulted regions are fitted  
     #    - in case the model is calculate in forward mode, we activate the condition as well so that the nominal system properties are updated with those defined in 'mod_prop'  
-    par_orb=['inclin_rad','aRs','lambda_rad']
-    par_LC=['RpRs']    
-    for par in par_orb+par_LC:fixed_args[par+'_pl']=[]
-    fixed_args['fit_orbit']=False
-    fixed_args['fit_RpRs']=False
+    if fixed_args['cond_transit_pl']:
+        par_orb=['inclin_rad','aRs','lambda_rad']
+        par_LC=['RpRs']    
+        for par in par_orb+par_LC:fixed_args[par+'_pl']=[]
+        fixed_args['fit_orbit']=False
+        fixed_args['fit_RpRs']=False
+    if fixed_args['cond_transit_sp']:
+        par_spot=['lat', 'Tcenter', 'ang', 'ctrst']    
+        for par in par_spot:fixed_args[par+'_sp']=[]
+        fixed_args['fit_spot']=False
+        fixed_args['fit_spot_ang']=[]
     for par in p_start:
         
         #Check if rootname of orbital/LC properties is one of the parameters left free to vary for a given planet    
         #    - if so, store name of planet for this property
-        for par_check in par_orb:
-            if (par_check in par):
-                if ('__IS' in par):pl_name = (par.split('__pl')[1]).split('__IS')[0]                  
-                else:pl_name = (par.split('__pl')[1]) 
-                if (p_start[par].vary) or fit_dic['fit_mode']=='':
-                    fixed_args[par_check+'_pl']+= [pl_name]
-                    fixed_args['fit_orbit']=True                     
-        for par_check in par_LC:
-            if (par_check in par):
-                if ('__IS' in par):pl_name = (par.split('__pl')[1]).split('__IS')[0]                  
-                else:pl_name = (par.split('__pl')[1])                 
-                if (p_start[par].vary) or fit_dic['fit_mode']=='':
-                    fixed_args[par_check+'_pl'] += [pl_name]
-                    fixed_args['fit_RpRs']=True 
-
-    #Unique list of planets with variable properties                
-    for par in par_orb:fixed_args[par+'_pl'] = list(np.unique(fixed_args[par+'_pl']))
-    for par in par_LC:fixed_args[par+'_pl'] = list(np.unique(fixed_args[par+'_pl']))
-    fixed_args['b_pl'] = list(np.unique(fixed_args['inclin_rad_pl']+fixed_args['aRs_pl']))
+        if fixed_args['cond_transit_pl']:
+            for par_check in par_orb:
+                if (par_check in par):
+                    if ('__IS' in par):pl_name = (par.split('__pl')[1]).split('__IS')[0]                  
+                    else:pl_name = (par.split('__pl')[1]) 
+                    if (p_start[par].vary) or fit_dic['fit_mode']=='':
+                        fixed_args[par_check+'_pl']+= [pl_name]
+                        fixed_args['fit_orbit']=True                     
+            for par_check in par_LC:
+                if (par_check in par):
+                    if ('__IS' in par):pl_name = (par.split('__pl')[1]).split('__IS')[0]                  
+                    else:pl_name = (par.split('__pl')[1])                 
+                    if (p_start[par].vary) or fit_dic['fit_mode']=='':
+                        fixed_args[par_check+'_pl'] += [pl_name]
+                        fixed_args['fit_RpRs']=True 
+
+        #Check if rootname of spot orbital properties is one of the parameters left free to vary for a given spot    
+        #    - if so, store name of spot for this property 
+        if fixed_args['cond_transit_sp']:        
+            for par_check in par_spot:
+                if (par_check in par) and ('_SP' in par):
+                    spot_name = par.split('_SP')[1]
+                    if (p_start[par].vary) or fit_dic['fit_mode']=='':
+                        fixed_args[par_check+'_sp']+= [spot_name]
+                        fixed_args['fit_spot']=True
+                    if ('ang' in par_check) and p_start[par].vary:
+                             fixed_args['fit_spot_ang']+=[spot_name]
+            
+    #Unique list of planets with variable properties  
+    if fixed_args['cond_transit_pl']:                
+        for par in par_orb:fixed_args[par+'_pl'] = list(np.unique(fixed_args[par+'_pl']))
+        for par in par_LC:fixed_args[par+'_pl'] = list(np.unique(fixed_args[par+'_pl']))
+        fixed_args['b_pl'] = list(np.unique(fixed_args['inclin_rad_pl']+fixed_args['aRs_pl']))
    
-    # Stage Théo : on utilise des valeurs par défaut pour les propriétés suivantes (si elles ne sont pas fittées) : 
-    #    - CB coef, 'alpha_rot', 'beta_rot', 'cos_istar' , 'veq' : les valeurs définies dans fixed_args['star_params']
-    #    - aRs, inclin_rad, lambda_rad : les valeurs définies dans fixed_args['planet_params']
-    #    - 'rv' : la vitesse systémique des CCF_DI, pas important, fixée à 0 dans tous les cas. 
-    #    - 'slope' : demandée par Di_prof_from_intr, fixée à 0 si pas fitté
-    #
-    #           -> Philosophie : mettre dans param tout ce qui est susceptible d'être fitté, en jouant avec le champ 'vary'
-    #           -> param a la même tête quelque soit le fit mené, aux champs 'vary' près.
-        
-    if rout_mode == 'ResProf' : #   or    (rout_mode == 'IntrProf' and fit_prop_dic['use_version2'])  :
+    #Unique list of spots with variable properties
+    if fixed_args['cond_transit_sp']:  
+        for par in par_spot:fixed_args[par+'_sp'] = list(np.unique(fixed_args[par+'_sp']))
 
-        for par in par_orb: 
-            if par+'__pl'+fixed_args['pl_loc'] not in p_start : 
-                p_start.add(par+'__pl'+fixed_args['pl_loc'] ,value=fixed_args['planet_params'][par], vary=False , min=None , max=None)
+    #Store the number of threads - needed when fitting joined residual profiles
+    fixed_args['nthreads']=fit_prop_dic['nthreads']
 
     #Fit initialization
-    init_fit(fit_dic,fixed_args,p_start,model_par_names(),fit_prop_dic)     
+    init_fit(fit_dic,fixed_args,p_start,fit_prop_dic,model_par_names,model_par_units)     
     merged_chain = None
     
     ########################################################################################################  
     #Calculating a first model to check all in-transit model exposures are defined
     if fit_dic['fit_mode'] in ['chi2','mcmc'] and ('Intr' in rout_mode):
         mod_dic,coeff_line_dic,mod_prop_dic = fixed_args['mod_func'](p_start,fixed_args)
         if rout_mode=='IntrProp':
@@ -650,15 +772,15 @@
     if fit_dic['fit_mode']=='chi2':
         fixed_args['fit'] = True
         print('       Chi2 fit')   
         p_final = call_lmfit(p_start,fixed_args['x_val'],fixed_args['y_val'],fixed_args['cov_val'],fixed_args['fit_func'],verbose=fit_prop_dic['verbose'],fixed_args=fixed_args)[2]
 
     ########################################################################################################    
     #Fit par emcmc 
-    elif fit_prop_dic['fit_mode']=='mcmc':  
+    elif fit_dic['fit_mode']=='mcmc':  
         fixed_args['fit'] = True
         print('       MCMC fit')
         
         #Default options
         if 'nwalkers' not in fit_prop_dic['mcmc_set']:fit_dic['nwalkers'] = int(3*fit_dic['merit']['n_free'])
         else:fit_dic['nwalkers'] = fit_prop_dic['mcmc_set']['nwalkers']
         if 'nsteps' not in fit_prop_dic['mcmc_set']:fit_dic['nsteps'] = 5000
@@ -674,15 +796,15 @@
         if fit_prop_dic['mcmc_run_mode']=='use':
             print('         Applying MCMC') 
 
             #Complex prior function
             if (len(fixed_args['prior_func'])>0):fixed_args['global_ln_prior_func']=global_ln_prior_func
 
             #Call to MCMC
-            walker_chains=call_MCMC(mcmc_threads,fixed_args,fit_dic,run_name=fit_dic['run_name'])
+            walker_chains=call_MCMC(mcmc_threads,fixed_args,fit_dic,run_name=fit_dic['run_name'],verbose=fit_dic['verbose'])
                
         #---------------------------------------------------------------  
        
         #Reuse MCMC
         elif fit_prop_dic['mcmc_run_mode']=='reuse':
             print('         Retrieving MCMC') 
             if len(fit_prop_dic['mcmc_reuse'])==0:
@@ -802,15 +924,15 @@
         #------------------------------------------------------------------------------------------------            
  
         #Processing:
         #    - best-fit parameters for model calculation
         #    - 1-sigma and envelope samples for plot
         #    - plot of model parameter chains
         #    - save file 
-        p_final,merged_chain,par_sample_sig1,par_sample=postMCMCwrapper_1(fit_dic,fixed_args,walker_chains,mcmc_threads,fixed_args['par_names'])
+        p_final,merged_chain,par_sample_sig1,par_sample=postMCMCwrapper_1(fit_dic,fixed_args,walker_chains,mcmc_threads,fixed_args['par_names'],verbose=fit_dic['verbose'],verb_shift=fit_dic['verb_shift']+'    ')
 
     ########################################################################################################  
     #No fit is performed: guess parameters are kept
     else:
         fixed_args['fit'] = False
         print('       Fixed model')
         p_final = deepcopy(p_start)   
@@ -1539,14 +1661,17 @@
     if (model_choice=='custom') and (prof_type=='DI'):
         
         #Custom model initialization
         fixed_args.update({
             'mac_mode':theo_dic['mac_mode'], 
             'inst':inst,
             'vis':vis})
+        
+        #Assuming no spots are fitted
+        fixed_args['unquiet_star'] = None
 
         #Grid initialization
         fixed_args['DI_grid'] = True
         fixed_args['conv2intr'] = False
         p_start = init_custom_DI_par(fixed_args,gen_dic,data_dic[inst]['system_prop'],star_params,p_start,RV_guess_tab)
 
         #Model function
@@ -1663,14 +1788,16 @@
 
     ######################################################################################################## 
 
     #Fit dictionary
     fit_dic={
         'merit':{},
         'fit_mode':fit_prop_dic['fit_mode'],
+        'print_par':fit_prop_dic['print_par'],
+        'verb_shift':'',
         'uf_bd':{},
         'nx_fit':len(fixed_args['y_val'])
         }
     fixed_args['fit'] = {'chi2':True,'':False,'mcmc':True}[fit_prop_dic['fit_mode']]
 
     #Parameter initialization
     p_start = par_formatting(p_start,model_prop,line_fit_priors,fit_dic,fixed_args,inst,vis,fixed_args['mode'])
@@ -1682,15 +1809,15 @@
         
         #Flux grid will be updated within custom_DI_prof() if args['fit'] and args['var_star_grid']
         if (not fixed_args['fit']) or (not fixed_args['var_star_grid']):
             fixed_args['Fsurf_grid_spec'] = theo_intr2loc(fixed_args['grid_dic'],fixed_args['system_prop'],fixed_args['args_exp'],fixed_args['args_exp']['ncen_bins'],fixed_args['grid_dic']['nsub_star'])         
         
     #Fit initialization
     fit_dic['save_dir'] = fixed_args['save_dir']+'iexp'+str(fixed_args['iexp'])+'/'
-    init_fit(fit_dic,fixed_args,p_start,model_par_names(),fit_prop_dic)  
+    init_fit(fit_dic,fixed_args,p_start,fit_prop_dic,model_par_names,model_par_units)     
 
     #--------------------------------------------------------------
     #Fit by chi2 minimization
     if fit_prop_dic['fit_mode']=='chi2':
         p_final = call_lmfit(p_start,fixed_args['x_val'],fixed_args['y_val'],fixed_args['cov_val'],fixed_args['fit_func'],verbose=verbose,fixed_args=fixed_args)[2]
      
     #--------------------------------------------------------------   
@@ -1839,15 +1966,16 @@
                     if 'ctrst' in fixed_args['var_par_list']:ctrst_chain=merged_chain[:,np_where1D(fixed_args['var_par_list']=='ctrst')[0]]
                     else:cont_chain=p_final['ctrst']
                     if 'cont' in fixed_args['var_par_list']:cont_chain=merged_chain[:,np_where1D(fixed_args['var_par_list']=='cont')[0]]
                     else:cont_chain=p_final['cont']
                     chain_loc=fixed_args['amp_sign']*ctrst_chain*cont_chain
                     merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)            
                 fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],'amp')
-                fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],'Amp')       
+                fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],'Amp') 
+                fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],'')      
 
             #Integral under the gaussian model
             #    - formula valid if there is no asymetry to the gaussian shape:
             # A = 0.5*amp*FWHM*sqrt(pi/ln(2))
             if ('area' in fit_prop_dic['deriv_prop']) and (model_choice=='gauss') and (p_final['skewA']==0.) and (p_final['kurtA']==0.):    
                 if fit_dic['fit_mode'] in ['chi2','']:
                     p_final['area']=np.abs(p_final['amp'])*p_final['FWHM']*np.sqrt(np.pi)/(2.*np.sqrt(np.log(2))) 
@@ -1863,15 +1991,16 @@
                     if 'amp' in fixed_args['var_par_list']:amp_chain=merged_chain[:,np_where1D(fixed_args['var_par_list']=='amp')[0]]
                     else:amp_chain=p_final['amp']
                     if 'FWHM' in fixed_args['var_par_list']:FWHM_chain=merged_chain[:,np_where1D(fixed_args['var_par_list']=='FWHM')[0]]
                     else:FWHM_chain=p_final['FWHM']
                     chain_loc=np.abs(amp_chain)*FWHM_chain*np.sqrt(np.pi)/(2.*np.sqrt(np.log(2))) 
                     merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)   
                 fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],'area')
-                fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],'Area')         
+                fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],'Area') 
+                fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],'')        
     
     
         if (prof_type in ['DI','Intr']):
     
             #FWHM of the Lorentzian and Voigt profiles
             #    - see function definition
             #    - fL = a*fG/sqrt(ln(2))
@@ -1909,15 +2038,16 @@
                     if 'a_damp' in fixed_args['var_par_list']:a_damp_chain = merged_chain[:,np_where1D(fixed_args['var_par_list']=='a_damp')[0]]
                     else:a_damp_chain = p_final['a_damp']                
                     fwhm_lor_chain = a_damp_chain*fwhm_gauss_chain/np.sqrt(np.log(2.))                
                     merged_chain=np.concatenate((merged_chain,fwhm_lor_chain[:,None]),axis=1) 
                     chain_loc=0.5436*fwhm_lor_chain+ np.sqrt(0.2166*fwhm_lor_chain**2.+fwhm_gauss_chain**2.) 
                     merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)          
                 fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],['FWHM_LOR','FWHM_voigt'])
-                fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],['a$_\mathrm{damp}$','FWHM$_\mathrm{Voigt}$'])                
+                fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],['a$_\mathrm{damp}$','FWHM$_\mathrm{Voigt}$']) 
+                fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],['','km/s'])               
                     
     
             #True properties of the global line
             #    - mesured on the high-resolution model, after instrumental convolution if requested
             if (model_choice in ['dgauss','custom']):
                 if any([par_name in fit_prop_dic['deriv_prop'] for par_name in ['true_ctrst','true_FWHM','true_amp']]):
                     if fit_dic['fit_mode'] in ['chi2','']:
@@ -1931,14 +2061,15 @@
                         p_final_loc=deepcopy(p_final)
                         fixed_args['cen_bins_HR'] = output_prop_dic['cen_bins_HR']
                         if fixed_args['nthreads']>1:chain_loc=para_cust_mod_true_prop(proc_cust_mod_true_prop,fixed_args['nthreads'],fit_dic['nsteps_final_merged'],[merged_chain],(fixed_args,p_final_loc,))                           
                         else:chain_loc=proc_cust_mod_true_prop(merged_chain,fixed_args,p_final_loc)       
                         merged_chain=np.concatenate((merged_chain,chain_loc.T),axis=1)  
                     fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],['true_ctrst','true_FWHM','true_amp',])
                     fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],['C$_\mathrm{true}$','FWHM$_\mathrm{true}$','A$_\mathrm{true}$'])
+                    fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],['','km/s',''])
         
                 #Stellar rotational velocity
                 if (model_choice=='custom') and ('vsini' in fit_prop_dic['deriv_prop']):
                     if ('veq' in fixed_args['var_par_list']):iveq=np_where1D(fixed_args['var_par_list']=='veq')[0] 
                     if ('cos_istar' in fixed_args['var_par_list']):iistar = np_where1D(fixed_args['var_par_list']=='cos_istar')[0] 
                     if fit_dic['fit_mode']=='chi2':             
                         #    - vsini = veq*sin(i)
@@ -1962,15 +2093,16 @@
                         else:veq_chain=deepcopy(merged_chain[:,iveq])  
                         if ('cos_istar' in fixed_args['var_par_list']):cosistar_chain=merged_chain[:,iistar]  
                         else:cosistar_chain=p_final['cos_istar']
                         cosistar_chain = (cosistar_chain-(1.)) % 2 - 1.
                         chain_loc = veq_chain*np.sqrt(1.-cosistar_chain*cosistar_chain)
                         merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)                 
                     fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],'vsini')            
-                    fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],'v$_\mathrm{eq}$sin i$_{*}$ (km/s)')     
+                    fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],'v$_\mathrm{eq}$sin i$_{*}$ (km/s)')
+                    fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],'km/s')     
         
                     #Convert cos(istar[rad]) into istar[deg]
                     conv_cosistar('conv',fixed_args,fit_dic,p_final,merged_chain)
                 
                 
                 if (model_choice=='dgauss'):
             
@@ -2013,14 +2145,15 @@
                             else:amp_l2c_chain=p_final['amp_l2c']         
                             amp_chain = ctrst_chain*cont_chain/( amp_l2c_chain - 1. )
                             cont_amp_chain=-fixed_args['amp_sign']*amp_chain*(amp_l2c_chain-1.)   
                             merged_chain=np.concatenate((merged_chain,cont_amp_chain[:,None],amp_chain[:,None]),axis=1)   
                     
                         fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],['cont_amp','amp'])
                         fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],['Acont','Amp'])
+                        fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],['',''])
         
         
                     #Lobe properties
                     if ('RV_lobe' in fit_prop_dic['deriv_prop']):                      
                         irv = np_where1D(fixed_args['var_par_list']=='rv')[0] 
                         if fit_dic['fit_mode']=='chi2': 
                             if 'rv_l2c' in fixed_args['var_par_list']:err_rv_l2c=fit_dic['sig_parfinal_err']['1s'][0,np_where1D(fixed_args['var_par_list']=='rv_l2c')[0]]  
@@ -2030,30 +2163,32 @@
                             fit_dic['sig_parfinal_err']['1s']= np.hstack((fit_dic['sig_parfinal_err']['1s'],[[sig_loc],[sig_loc]]))         
                         elif fit_dic['fit_mode']=='mcmc': 
                             if 'rv_l2c' in fixed_args['var_par_list']:rv_l2c_chain=merged_chain[:,np_where1D(fixed_args['var_par_list']=='rv_l2c')[0]]
                             else:rv_l2c_chain=p_final['rv_l2c']
                             chain_loc = merged_chain[:,irv] + rv_l2c_chain
                             merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)
                         fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],['RV_lobe'])
-                        fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],['rv$_\mathrm{lobe}$ (km s$^{-1}$)'])                    
+                        fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],['rv$_\mathrm{lobe}$ (km s$^{-1}$)'])  
+                        fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],['km/s'])                   
                     
                     if ('amp_lobe' in fit_prop_dic['deriv_prop']):            
                         if fit_dic['fit_mode']=='chi2': 
                             if 'amp_l2c' in fixed_args['var_par_list']:err_amp_l2c=fit_dic['sig_parfinal_err']['1s'][0,np_where1D(fixed_args['var_par_list']=='amp_l2c')[0]]  
                             else:err_amp_l2c=0.
                             p_final['amp_lobe']=p_final['amp']*p_final['amp_l2c']
                             sig_loc=np.sqrt((sig_Ac*p_final['amp_l2c'])**2.+(err_amp_l2c*p_final['amp'])**2.)
                             fit_dic['sig_parfinal_err']['1s']= np.hstack((fit_dic['sig_parfinal_err']['1s'],[[sig_loc],[sig_loc]])) 
                         elif fit_dic['fit_mode']=='mcmc': 
                             if 'amp_l2c' in fixed_args['var_par_list']:amp_l2c_chain=merged_chain[:,np_where1D(fixed_args['var_par_list']=='amp_l2c')[0]]
                             else:amp_l2c_chain=p_final['amp_l2c']
                             chain_loc=merged_chain[:,np_where1D(fixed_args['var_par_list']=='amp')[0]]*amp_l2c_chain
                             merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)
                         fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],['amp_lobe'])
-                        fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],['A$_\mathrm{lobe}$'])                    
+                        fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],['A$_\mathrm{lobe}$'])   
+                        fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],[''])                  
                     
                     if ('FWHM_lobe' in fit_prop_dic['deriv_prop']):                     
                         if fit_dic['fit_mode']=='chi2': 
                             if 'FWHM_l2c' in fixed_args['var_par_list']:err_FWHM_l2c=fit_dic['sig_parfinal_err']['1s'][0,np_where1D(fixed_args['var_par_list']=='FWHM_l2c')[0]]  
                             else:err_FWHM_l2c=0.
                             if 'FWHM' in fixed_args['var_par_list']:err_FWHM=fit_dic['sig_parfinal_err']['1s'][0,np_where1D(fixed_args['var_par_list']=='FWHM')[0]]  
                             else:err_FWHM=0.     
@@ -2065,14 +2200,15 @@
                             else:FWHM_l2c_chain=p_final['FWHM_l2c']
                             if 'FWHM' in fixed_args['var_par_list']:FWHM_chain=merged_chain[:,np_where1D(fixed_args['var_par_list']=='FWHM')[0]]
                             else:FWHM_chain=p_final['FWHM']
                             chain_loc=FWHM_chain*FWHM_l2c_chain
                             merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)
                         fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],['FWHM_lobe'])
                         fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],['FWHM$_\mathrm{lobe}$ (km s$^{-1}$)'])
+                        fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],['km/s'])
             
 
          
             
 
 
     ########################################################################################################   
@@ -2398,16 +2534,16 @@
     args = deepcopy(args_in)
     args['grid_dic']['precision']='low'
     for inst in args['inst_list']:
         args['inst']=inst
         for vis in args['inst_vis_list'][inst]:   
             args['vis']=vis
             pl_vis = args['transit_pl'][inst][vis][0]
-            system_param_loc,coord_pl,param_val = up_plocc_prop(inst,vis,args,p_step_loc,[pl_vis],args['nexp_fit_all'][inst][vis],args['ph_fit'][inst][vis],args['coord_pl_fit'][inst][vis])
-            surf_prop_dic,spot_prop_dic = sub_calc_plocc_spot_prop([args['chrom_mode']],args,[args['coord_line']],[pl_vis],system_param_loc,args['grid_dic'],args['system_prop'],param_val,args['coord_pl_fit'][inst][vis],range(args['nexp_fit_all'][inst][vis]),False)
+            system_param_loc,coord_pl,param_val = up_plocc_prop(inst,vis,args,p_step_loc,[pl_vis],args['ph_fit'][inst][vis],args['coord_fit'][inst][vis])
+            surf_prop_dic,spot_prop_dic,surf_prop_dic_common = sub_calc_plocc_spot_prop([args['chrom_mode']],args,[args['coord_line']],[pl_vis],system_param_loc,args['grid_dic'],args['system_prop'],param_val,args['coord_fit'][inst][vis],range(args['nexp_fit_all'][inst][vis]),False)
             ctrst_vis = surf_prop_dic[pl_vis]['ctrst'][0]       
             break_cond = (ctrst_vis<0.) | (ctrst_vis>1.)
             if True in break_cond:
                 ln_p_loc+= -np.inf	
                 break 
     return ln_p_loc
 
@@ -2545,15 +2681,16 @@
                         Rstar_med = 0.784  
                         Rstar_err=0.007   
                     Rstar_chain = np.random.normal(Rstar_med, Rstar_err, n_chain)
                 iPeq = np_where1D(fixed_args['var_par_list']=='Peq')
                 chain_loc=(2.*np.pi*Rstar_chain*Rsun)/(np.squeeze(merged_chain[:,iPeq])*3600.*24.)
                 merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)  
             fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],'veq')
-            fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],'v$_{eq}$(km/s)')
+            fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],'v$_{eq}$ (km/s)')
+            fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],'km/s')
     
     
         #Convert veq into veq*sin(istar) to be comparable with solid-body values
         #    - must be done before modification of istar chain
         if ('vsini' in deriv_prop) and ((fixed_args['rout_mode'] in ['IntrProf','ResProf']) or ((fixed_args['rout_mode']=='IntrProp') and (fixed_args['prop_fit']=='rv'))):
             print('        + Converting veq to vsini')
             if 'veq' in fixed_args['var_par_list']:iveq=np_where1D(fixed_args['var_par_list']=='veq')
@@ -2581,15 +2718,16 @@
                     
                 #Folding cos(istar) within -1 : 1
                 cosistar_chain = (cosistar_chain-(1.)) % 2 - 1.
                     
                 veq_chain=deepcopy(merged_chain[:,iveq])            
                 merged_chain[:,iveq]=veq_chain*np.sqrt(1.-cosistar_chain*cosistar_chain)
             fixed_args['var_par_list'][iveq]='vsini'            
-            fixed_args['var_par_names'][iveq]=model_par_names()['vsini']             
+            fixed_args['var_par_names'][iveq]=model_par_names('vsini') 
+            fixed_args['var_par_units'][iveq]=model_par_units('vsini')            
     
             
         #-------------------------------------------------            
 
         #Replace cos(istar[rad]) by istar[deg]
         if ('istar_deg_conv' in deriv_prop) or ('istar_deg_add' in deriv_prop):
             print('        + Converting cos(istar) to istar')
@@ -2726,15 +2864,16 @@
                 chain_loc=np.arcsin( sinistar_chain )*180./np.pi 
                 
                 # #pi-istar chain
                 # chain_loc=180.-chain_loc   
                 
                 merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)  
             fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],'istar_deg')
-            fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],model_par_names()['istar_deg'])
+            fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],model_par_names('istar_deg'))
+            fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],model_par_units('istar_deg'))
     
         #-------------------------------------------------
         #Add Peq using the value derived from veq and independent measurement of Rstar
         #    - Peq = (2*pi*Rstar/veq)
         if 'Peq_veq' in deriv_prop:
             if ('cos_istar' in fixed_args['var_par_list']):stop('    istar has been fitted')
             print('        + Deriving Peq from veq ')
@@ -2757,15 +2896,16 @@
                 Rstar_chain = np.random.normal(Rstar_med, Rstar_err, len(merged_chain[:,0]))
                 
                 #Calculate Peq chain
                 iveq = np_where1D(fixed_args['var_par_list']=='veq')
                 chain_loc=(2.*np.pi*Rstar_chain)/(np.squeeze(merged_chain[:,iveq])*3600.*24.)
                 merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)  
             fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],'Peq')
-            fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],model_par_names()['Peq'])
+            fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],model_par_names('Peq'))
+            fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],model_par_units('Peq'))
     
         #-------------------------------------------------
         #Add Peq using the value derived from vsini and independent measurement of Rstar and istar
         #    - Peq = (2*pi*Rstar*sin(istar)/vsini)
         if 'Peq_vsini' in deriv_prop:
             print('        + Deriving Peq from vsini')
             
@@ -2798,15 +2938,16 @@
                 
                 #Calculate Peq chain
                 if 'vsini' not in fixed_args['var_par_list']:stop('Add vsini chain')
                 ivsini = np_where1D(fixed_args['var_par_list']=='vsini')
                 chain_loc=(2.*np.pi*Rstar_chain*sinistar_chain)/(np.squeeze(merged_chain[:,ivsini])*3600.*24.)
                 merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)  
             fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],'Peq')
-            fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],model_par_names()['Peq'])   
+            fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],model_par_names('Peq'))  
+            fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],model_par_units('Peq')) 
     
         #-------------------------------------------------
                 
         #Add true obliquity
         #    - psi = acos(sin(istar)*cos(lamba)*sin(ip) + cos(istar)*cos(ip))
         #    - must be done before modification of istar and lambda chains
         if ('psi' in deriv_prop) or ('psi_lambda' in deriv_prop):
@@ -2974,18 +3115,20 @@
                             merged_chain=np.concatenate((merged_chain,PsiS_chain[:,None]),axis=1)   
                             merged_chain=np.concatenate((merged_chain,Psi_chain[:,None]),axis=1)   
                 
                 if lambda_rad_pl in fixed_args['genpar_instvis']:  
                     for inst in fixed_args['genpar_instvis'][lambda_rad_pl]:
                         for vis in fixed_args['genpar_instvis'][lambda_rad_pl][inst]:
                             fixed_args['var_par_list']=np.concatenate((fixed_args['var_par_list'],['PsiN__pl'+pl_loc+'__IS'+inst+'_VS'+vis,'PsiS__pl'+pl_loc+'__IS'+inst+'_VS'+vis]))
-                            fixed_args['var_par_names']=np.concatenate((fixed_args['var_par_names'],[pl_loc+'_$\psi_{N}$['+inst+']('+vis+')',pl_loc+'_$\psi_{S}$',pl_loc+'_$\psi$['+inst+']('+vis+')']))          
+                            fixed_args['var_par_names']=np.concatenate((fixed_args['var_par_names'],[pl_loc+'_$\psi_{N}$['+inst+']('+vis+')',pl_loc+'_$\psi_{S}$',pl_loc+'_$\psi$['+inst+']('+vis+')']))   
+                            fixed_args['var_par_units']=np.concatenate((fixed_args['var_par_units'],['deg','deg','deg']))        
                 else:
                     fixed_args['var_par_list']=np.concatenate((fixed_args['var_par_list'],['PsiN__pl'+pl_loc,'PsiS__pl'+pl_loc,'Psi__pl'+pl_loc]))
                     fixed_args['var_par_names']=np.concatenate((fixed_args['var_par_names'],[pl_loc+'_$\psi_{N}$',pl_loc+'_$\psi_{S}$',pl_loc+'_$\psi$']))   
+                    fixed_args['var_par_units']=np.concatenate((fixed_args['var_par_units'],['deg','deg','deg']))   
              
         #-------------------------------------------------
             
         #Add argument of ascending node
         #    - Om = np.arctan( -sin(lambda)*tan(ip) )
         #    - must be done before modification of ip and lambda chains
         if 'om' in deriv_prop:
@@ -3019,17 +3162,19 @@
                             merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)   
 
                 if lambda_rad_pl in fixed_args['genpar_instvis']:  
                     for inst in fixed_args['genpar_instvis'][lambda_rad_pl]:
                         for vis in fixed_args['genpar_instvis'][lambda_rad_pl][inst]:
                             fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],'Omega__pl'+pl_loc+'__IS'+inst+'_VS'+vis)
                             fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],pl_loc+'_$\Omega$['+inst+']('+vis+')') 
+                            fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],'deg') 
                 else:
                     fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],'Omega__pl'+pl_loc)
-                    fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],pl_loc+'_$\Omega$')               
+                    fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],pl_loc+'_$\Omega$')  
+                    fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],'deg')               
 
         #-------------------------------------------------
             
         #Add impact parameter
         #    - b = aRs*cos(ip)
         if ('b' in deriv_prop) and (fixed_args['fit_orbit']):
             print('        + Adding impact parameter')
@@ -3057,14 +3202,15 @@
                 elif fit_dic['fit_mode']=='mcmc':             
                     if ('inclin_rad__pl'+pl_loc in fixed_args['var_par_list']):ip_loc=merged_chain[:,iip]
                     if ('aRs__pl'+pl_loc in fixed_args['var_par_list']):aRs_loc=merged_chain[:,iaRs]          
                     chain_loc=aRs_loc*np.abs(np.cos(ip_loc))
                     merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)   
                 fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],pl_loc+'_b')
                 fixed_args['var_par_names']=np.append(fixed_args['var_par_names'],pl_loc+'_b')
+                fixed_args['var_par_units']=np.append(fixed_args['var_par_units'],'')
     
         #-------------------------------------------------            
             
         #Orbital inclination
         #    - convert ip[rad] to ip[deg]
         if ('ip' in deriv_prop) and (fixed_args['fit_orbit']):
             print('        + Converting ip in degrees')
@@ -3084,14 +3230,15 @@
                     w_lt_0=(ip_temp < 0.)
                     if True in w_lt_0:
                         i_mod=npint(np.abs(ip_temp[w_lt_0])/90.)+1.
                         merged_chain[w_lt_0,iip] = ip_temp[w_lt_0]+i_mod*90.                    
                     
                 fixed_args['var_par_list'][iip]='ip_deg__pl'+pl_loc            
                 fixed_args['var_par_names'][iip]='i$_\mathrm{p}$['+pl_loc+']($^{\circ}$)'  
+                fixed_args['var_par_units'][iip]='deg' 
     
         #-------------------------------------------------            
             
         #Convert lambda[rad] to lambda[deg]
         if ('lambda_deg' in deriv_prop) and ((fixed_args['rout_mode'] in ['IntrProf','ResProf']) or ((fixed_args['rout_mode']=='IntrProp') and (fixed_args['prop_fit']=='rv'))):  
             print('        + Converting lambda in degrees')       
             for pl_loc in fixed_args['lambda_rad_pl']:
@@ -3107,15 +3254,16 @@
                             i_mod=npint(np.abs(lambda_temp)/360.)+1.
                             lambda_temp += i_mod*360.+mid_shift  
                         else:lambda_temp += mid_shift
                         p_final[new_lamb_name] = lambda_temp
                         sig_temp  = fit_dic['sig_parfinal_err']['1s'][0,ilamb]*180./np.pi 
                         fit_dic['sig_parfinal_err']['1s'][:,ilamb] = sig_temp  
                         fixed_args['var_par_list'][ilamb]=new_lamb_name       
-                        fixed_args['var_par_names'][ilamb]= new_lamb_name_txt                           
+                        fixed_args['var_par_names'][ilamb]= new_lamb_name_txt   
+                        fixed_args['var_par_units'][ilamb]= 'deg'                         
                         return None
                     
                     if lambda_rad_pl in fixed_args['genpar_instvis']:
                         for inst in fixed_args['genpar_instvis'][lambda_rad_pl]:
                             for vis in fixed_args['genpar_instvis'][lambda_rad_pl][inst]:
                                 sub_func(lambda_rad_pl+'__IS'+inst+'_VS'+vis,lambda_deg_pl+'__IS'+inst+'_VS'+vis,'$\lambda$['+pl_loc+']['+inst+']('+vis+')($^{\circ}$)')
                     else:sub_func(lambda_rad_pl,lambda_deg_pl,'$\lambda$['+pl_loc+']($^{\circ}$)')   
@@ -3151,15 +3299,16 @@
                             merged_chain[w_gt_360,ilamb]=np.mod(lambda_temp[w_gt_360],360.)+mid_shift
                         w_lt_0=(lambda_temp < 0.)
                         if True in w_lt_0:
                             i_mod=npint(np.abs(lambda_temp[w_lt_0])/360.)+1.
                             merged_chain[w_lt_0,ilamb] = lambda_temp[w_lt_0]+i_mod*360.+mid_shift
                 
                         fixed_args['var_par_list'][ilamb]=new_lamb_name
-                        fixed_args['var_par_names'][ilamb]=new_lamb_name_txt       
+                        fixed_args['var_par_names'][ilamb]=new_lamb_name_txt  
+                        fixed_args['var_par_units'][ilamb]='deg'      
                         
                         return None
     
                     if lambda_rad_pl in fixed_args['genpar_instvis']:
                         for inst in fixed_args['genpar_instvis'][lambda_rad_pl]:
                             for vis in fixed_args['genpar_instvis'][lambda_rad_pl][inst]:
                                 sub_func(lambda_rad_pl+'__IS'+inst+'_VS'+vis,lambda_deg_pl+'__IS'+inst+'_VS'+vis,'$\lambda$['+pl_loc+']['+inst+']('+vis+')($^{\circ}$)')
@@ -3187,30 +3336,32 @@
                         if len(fixed_args['linked_par_expr'])>0:exec(str(par)+'='+str(p_final_loc[par]))
                     for par in fixed_args['linked_par_expr']:
                         p_final_loc[par]=eval(fixed_args['linked_par_expr'][par])
                     c0_CB = calc_CB_RV(get_LD_coeff(fixed_args['system_prop']['achrom'],0),fixed_args['system_prop']['achrom']['LD'][0],p_final['c1_CB'],p_final['c2_CB'],p_final['c3_CB'],fixed_args['system_param']['star'])[0]            
                     chain_loc=np.append(chain_loc,c0_CB)
                 merged_chain=np.concatenate((merged_chain,chain_loc[:,None]),axis=1)   
             fixed_args['var_par_list']=np.append(fixed_args['var_par_list'],'c0_CB')
-            fixed_args['var_par_names'] = np.append(fixed_args['var_par_names'],'CB$_{0}$')           
+            fixed_args['var_par_names'] = np.append(fixed_args['var_par_names'],'CB$_{0}$')  
+            fixed_args['var_par_units'] = np.append(fixed_args['var_par_units'],'km/s')           
     
     
         #-------------------------------------------------            
          
         #Convert CB coefficients from km/s to m/s
         if 'CB_ms' in deriv_prop: 
             print('        + Converting CB coefficients to m/s') 
             ipar_mult_loc=[]
             for ipar_name in ['c0_CB','c1_CB','c2_CB','c3_CB']:
                 ipar_loc=np_where1D(fixed_args['var_par_list']==ipar_name)
                 if len(ipar_loc)>0:ipar_mult_loc+=[ipar_loc]
                 if ipar_name=='c0_CB':fixed_args['var_par_names'][ipar_loc]='CB$_{0}$ (m s$^{-1}$)'
                 if ipar_name=='c1_CB':fixed_args['var_par_names'][ipar_loc]='CB$_{1}$ (m s$^{-1}$)'
                 if ipar_name=='c2_CB':fixed_args['var_par_names'][ipar_loc]='CB$_{2}$ (m s$^{-1}$)'
-                if ipar_name=='c3_CB':fixed_args['var_par_names'][ipar_loc]='CB$_{3}$ (m s$^{-1}$)'             
+                if ipar_name=='c3_CB':fixed_args['var_par_names'][ipar_loc]='CB$_{3}$ (m s$^{-1}$)'  
+                fixed_args['var_par_units'][ipar_loc]='m/s'            
                 if fit_dic['fit_mode']=='chi2': 
                     p_final[ipar_name]*=1e3 
                     fit_dic['sig_parfinal_err']['1s'][:,ipar_loc]*=1e3  
                 elif fit_dic['fit_mode']=='mcmc':  
                     merged_chain[:,ipar_loc]*=1e3 
     
         #-------------------------------------------------            
@@ -3273,17 +3424,19 @@
             cosistar_chain = (merged_chain_in[:,iistar]-(1.)) % 2 - 1.
             chain_loc = np.arccos(cosistar_chain)*180./np.pi     
             if ('istar_deg_conv') in deriv_prop:merged_chain_in[:,iistar]= chain_loc
             elif ('istar_deg_add') in deriv_prop:merged_chain_in=np.concatenate((merged_chain_in,chain_loc[:,None]),axis=1)  
         if ('istar_deg_conv') in deriv_prop:    
             fixed_args_in['var_par_list'][iistar]='istar_deg'            
             fixed_args_in['var_par_names'][iistar]='i$_{*}(^{\circ}$)'   
+            fixed_args_in['var_par_units'][iistar]='deg'   
         elif ('istar_deg_add') in deriv_prop: 
             fixed_args_in['var_par_list']=np.append(fixed_args_in['var_par_list'],'istar_deg')
             fixed_args_in['var_par_names']=np.append(fixed_args_in['var_par_names'],'i$_{*}(^{\circ}$)') 
+            fixed_args_in['var_par_units']=np.append(fixed_args_in['var_par_units'],'deg')
     else:
         if fit_dic_in['fit_mode']=='chi2':p_final_in['istar_deg']=np.arccos(p_final_in['cos_istar'])*180./np.pi  
         elif fit_dic_in['fit_mode']=='mcmc':fixed_args_in['fixed_par_val']['istar_deg']=np.arccos(p_final_in['cos_istar'])*180./np.pi                          
     return merged_chain_in
 
 
 
@@ -3353,20 +3506,24 @@
                 elif ('CF0_meas_conv' in deriv_prop) or ('CF0_DG_conv' in deriv_prop):   #replace parameters
                     if varC:merged_chain[:,ictrst_loc] = chain_ctrst_temp
                     if varF:merged_chain[:,iFWHM_loc] = chain_FWHM_temp              
             if ('CF0_meas_add' in deriv_prop) or ('CF0_DG_add' in deriv_prop):
                 if varC:
                     fixed_args['var_par_list']=np.concatenate((fixed_args['var_par_list'],[fixed_args['var_par_list'][ictrst_loc]+'_'+inst]))
                     fixed_args['var_par_names']=np.concatenate((fixed_args['var_par_names'],['Contrast$_\mathrm{'+inst+'}$']))
+                    fixed_args['var_par_units']=np.concatenate((fixed_args['var_par_units'],['']))
                 if varF:
                     fixed_args['var_par_list']=np.concatenate((fixed_args['var_par_list'][fixed_args['var_par_list'][iFWHM_loc]+'_'+inst]))
                     fixed_args['var_par_names']=np.concatenate((fixed_args['var_par_names']['FWHM$_\mathrm{'+inst+'}$(km/s)']))
+                    fixed_args['var_par_units']=np.concatenate((fixed_args['var_par_units'],['km/s']))
             elif ('CF0_meas_conv' in deriv_prop) or ('CF0_DG_conv' in deriv_prop):
                 if varC:
                     fixed_args['var_par_list'][ictrst_loc] = fixed_args['var_par_list'][ictrst_loc]+'_'+inst
                     fixed_args['var_par_names'][ictrst_loc] = 'Contrast$_\mathrm{'+inst+'}$'
+                    fixed_args['var_par_units'][ictrst_loc] = ''
                 if varF:                                
                     fixed_args['var_par_list'][iFWHM_loc] = fixed_args['var_par_list'][iFWHM_loc]+'_'+inst
                     fixed_args['var_par_names'][iFWHM_loc] = 'FWHM$_\mathrm{'+inst+'}$(km/s)'
+                    fixed_args['var_par_units'][iFWHM_loc] = ''
 
     return merged_chain
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_analysis/ANTARESS_inst_resp.py` & `antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_inst_resp.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_analysis/ANTARESS_joined_atm.py` & `antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_joined_atm.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_analysis/ANTARESS_model_prof.py` & `antaress-1.1.1/src/antaress/ANTARESS_analysis/ANTARESS_model_prof.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_conversions/ANTARESS_binning.py` & `antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_binning.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 import bindensity as bind
 from copy import deepcopy
 from ..ANTARESS_general.utils import stop,np_where1D,dataload_npz,default_func,check_data
 from ..ANTARESS_general.constant_data import c_light
 from ..ANTARESS_grids.ANTARESS_coord import excl_plrange,calc_pl_coord,conv_phase
-from ..ANTARESS_grids.ANTARESS_plocc_grid import sub_calc_plocc_spot_prop
+from ..ANTARESS_grids.ANTARESS_occ_grid import sub_calc_plocc_spot_prop,retrieve_spots_prop_from_param
 
-def process_bin_prof(mode,data_type_gen,gen_dic,inst,vis_in,data_dic,coord_dic,data_prop,system_param,theo_dic,plot_dic,mock_dic={},masterDI=False):
+def process_bin_prof(mode,data_type_gen,gen_dic,inst,vis_in,data_dic,coord_dic,data_prop,system_param,theo_dic,plot_dic,spot_dic={},masterDI=False):
     r"""**Binning routine**
 
     Bins series of input spectral profile into a new series along the chosen temporal/spatial dimension.
     
      - for a given visit or between several visits
      - binned profiles are calculated as weighted means with weights specific to the type of profiles
      - binned profiles are used for analysis purposes
@@ -325,26 +325,14 @@
             dur_to_bin = np.zeros(len(idx_to_bin),dtype=float)
             for loc, indiv_idx in enumerate(idx_to_bin):
                 time_to_bin[loc] = data_to_bin[indiv_idx]['bjd']
                 dur_to_bin[loc] = data_to_bin[indiv_idx]['t_dur']
             binned_time[i_new] = np.average(time_to_bin)
             binned_t_dur[i_new] = np.average(dur_to_bin)
            
-
-            # # Stage Théo : Saving extra data for the module 'fit_ResProf'
-            
-            # if (gen_dic['fit_ResProf'] and masterDI) : 
-            #     data_exp_new['idx_to_bin'] = idx_to_bin
-            #     data_exp_new['weight'] = {}
-            #     for iexp_off in idx_to_bin : data_exp_new['weight'][iexp_off] = data_to_bin[iexp_off]['weight']
-            #     data_exp_new['dx_ov'] = dx_ov
-
-
-
-
         #Store path to weighing master 
         if masterDI:
             np.savez_compressed(data_dic[inst][vis_in]['mast_'+data_type+'_data_paths'][0],data=data_exp_new,allow_pickle=True) 
 
         #Store common table of binned profiles
         data_glob_new['cen_bins'] = data_com['cen_bins']
         data_glob_new['edge_bins'] = data_com['edge_bins']
@@ -404,37 +392,54 @@
             data_glob_new['idx_in2exp'] = np.arange(data_glob_new['n_exp'],dtype=int)[data_glob_new['idx_in']]
             data_glob_new['dim_in'] = [data_glob_new['n_in_tr']]+data_glob_new['dim_exp']
  
             #Binned exposure timestamp and duration
             data_glob_new['coord']['bjd'] = binned_time
             data_glob_new['coord']['t_dur'] = binned_t_dur
 
-            #Properties of planet-occulted and spot regions 
+            #Properties of planet-occulted and spot-occulted regions 
             params = deepcopy(system_param['star'])
             params.update({'rv':0.,'cont':1.}) 
-            if mock_dic!={} and (inst in mock_dic['spots_prop']):
-                #Samson: I think we said there is no need to define mock_dic['use_spots'], the condition (inst in mock_dic['spots_prop']) is sufficient to activate or not the use of spots
+            params['use_spots']=False
+            if (inst in spot_dic):
                 if mode=='multivis':
                     print('WARNING: spots properties are not propagated for multiple visits.')
-                elif vis_in in mock_dic['spots_prop'][inst]:
-                    for spot_param in list(mock_dic['spots_prop'][inst][vis_in].keys()):
-                        params[spot_param]=mock_dic['spots_prop'][inst][vis_in][spot_param]
-                        
-                    #Figuring out the number of spots
-                    num_spots = 0
-                    for par in params:
-                        if 'lat__IS'+inst+'_VS'+vis_in+'_SP' in par:num_spots +=1
-                    params['num_spots']=num_spots
-                    params['inst']=inst
-                    params['vis']=vis_in  
+                elif vis_in in spot_dic[inst]:
+
+                    #Trigger spot use
+                    params['use_spots']=True
+
+                    #Initialize entries for spot coordinates 
+                    for spot in data_dic[inst][vis_in]['transit_sp']:
+                        data_glob_new['coord'][spot]={}
+                        for key in ['Tcenter', 'ang', 'ang_rad', 'lat', 'ctrst']:data_glob_new['coord'][spot][key] = np.zeros(n_bin,dtype=float)*np.nan
+                        for key in ['lat_rad_exp','sin_lat_exp','cos_lat_exp','long_rad_exp','sin_long_exp','cos_long_exp','x_sky_exp','y_sky_exp','z_sky_exp']:data_glob_new['coord'][spot][key] = np.zeros([3,n_bin],dtype=float)*np.nan
+                        data_glob_new['coord'][spot]['is_visible'] = np.zeros([3,n_bin],dtype=float)
+
+                    #Retrieve spot coordinates/properties for new exposures
+                    spot_dic[inst][vis_in]['cos_istar']=system_param['star']['cos_istar']
+
+                    for i_new in range(n_bin):
+                        spots_prop = retrieve_spots_prop_from_param(system_param['star'],spot_dic[inst][vis_in],inst,vis_in,data_glob_new['coord']['bjd'][i_new],exp_dur=data_glob_new['coord']['t_dur'][i_new])
+                        for spot in data_dic[inst][vis_in]['transit_sp']:
+                            for key in ['Tcenter', 'ang', 'ang_rad', 'lat', 'ctrst']:
+                                data_glob_new['coord'][spot][key][i_new] = spots_prop[spot][key]
+
+                            for key in ['lat_rad_exp','sin_lat_exp','cos_lat_exp','long_rad_exp','sin_long_exp','cos_long_exp','x_sky_exp','y_sky_exp','z_sky_exp']:
+                                data_glob_new['coord'][spot][key][:, i_new] = [spots_prop[spot][key+'_start'],spots_prop[spot][key+'_center'],spots_prop[spot][key+'_end']]
+
+                            data_glob_new['coord'][spot]['is_visible'][:, i_new]=[spots_prop[spot]['is_start_visible'],spots_prop[spot]['is_center_visible'],spots_prop[spot]['is_end_visible']]
+
+                    spot_dic[inst][vis_in].pop('cos_istar')
+                                        
             par_list=['rv','CB_RV','mu','lat','lon','x_st','y_st','SpSstar','xp_abs','r_proj']
             key_chrom = ['achrom']
             if ('spec' in data_mode) and ('chrom' in system_prop):key_chrom+=['chrom']
-            data_glob_new['plocc_prop'],data_glob_new['spot_prop'] = sub_calc_plocc_spot_prop(key_chrom,{},par_list,data_inst[vis_save]['transit_pl'],system_param,theo_dic,system_prop,params,data_glob_new['coord'],range(n_bin),system_spot_prop_in=data_dic['DI']['spots_prop'],out_ranges=True) 
-
+            data_glob_new['plocc_prop'],data_glob_new['spot_prop'],data_glob_new['common_prop'] = sub_calc_plocc_spot_prop(key_chrom,{},par_list,data_inst[vis_save]['transit_pl'],system_param,theo_dic,system_prop,params,data_glob_new['coord'],range(n_bin),system_spot_prop_in=data_dic['DI']['spots_prop'],out_ranges=True)
+            
         #---------------------------------------------------------------------------
 
         #Saving global tables for new exposures
         if not masterDI:
             if (data_type=='DI'):data_glob_new['sysvel'] = sysvel
         np.savez_compressed(save_pref+'_add',data=data_glob_new,allow_pickle=True)
 
@@ -610,15 +615,15 @@
 
 
 
 
 
 
 
-def weights_bin_prof(iord_orig_list,scaled_data_paths,inst,vis,gen_corr_Fbal,gen_corr_Fbal_ord,save_data_dir,gen_type,nord,iexp_glob,data_type,data_mode,dim_exp,tell_exp,mean_gdet,cen_bins,dt,flux_ref_exp,cov_ref_exp,flux_est_loc_exp=None,cov_est_loc_exp=None,SpSstar_spec=None,bdband_flux_sc=False,glob_flux_sc=None,corr_Fbal = True):
+def weights_bin_prof(iord_orig_list,scaled_data_paths,inst,vis,gen_corr_Fbal,gen_corr_Fbal_ord,save_data_dir,gen_type,nord,iexp_glob,data_type,data_mode,dim_exp,tell_exp,mean_gdet,cen_bins,dt,flux_ref_exp,cov_ref_exp,ref_val=0.,flux_est_loc_exp=None,cov_est_loc_exp=None,SpSstar_spec=None,bdband_flux_sc=False,glob_flux_sc=None,corr_Fbal = True):
     r"""**Binning routine: weights**
 
     Defines weights to be used when binning profiles.
     Weights should only be defined using the inverse squared error if the weighted values are comparable, so that all profiles should have been scaled to comparable flux levels prior to binning.
     Profiles must be defined on the same spectral table to be binned together.
 
     Args:
@@ -777,15 +782,15 @@
     #                    = LC_theo(band,t,v)^2*Ccorr(w,t,v)*[  gcal(band)*MFstar_meas(w,v) + (Ccorr(w,t,v)/(dt*globF(t,v)))*( EMFstar_meas(t,w)^2 - MFstar_meas(t,w)*gcal(band)*Twstar2(w) )/Twstar(w)  ]/(dt*globF(t,v))
     #                    = LC_theo(band,t,v)^2*Ccorr(w,t,v)*[  gcal(band)*MFstar_meas(w,v)    - (Ccorr(w,t,v)/(dt*globF(t,v)))* MFstar_meas(t,w)*gcal(band)*Twstar2(w) /Twstar(w)         + (Ccorr(w,t,v)/(dt*globF(t,v)))*EMFstar_meas(t,w)^2/Twstar(w)  ]/(dt*globF(t,v))
     #                    = LC_theo(band,t,v)^2*Ccorr(w,t,v)*[  MFstar_meas(w,v)*gcal(band)*( 1 - (Ccorr(w,t,v)*Twstar2(w)/(dt*globF(t,v)*Twstar(w)))) + (Ccorr(w,t,v)/(dt*globF(t,v)))*EMFstar_meas(t,w)^2/Twstar(w)  ]/(dt*globF(t,v))
     #                    = LC_theo(band,t,v)^2*Ccorr(w,t,v)*[  MFstar_meas(w,v)*gcal(band)*( Twstar(w)*dt*globF(t,v) - Ccorr(w,t,v)*Twstar2(w)) + Ccorr(w,t,v)*EMFstar_meas(t,w)^2  ]/((dt*globF(t,v))^2*Twstar(w))
     #--------------------------------------------------------     
 
     #Calculate weights at pixels where the master stellar spectrum is defined and positive
-    cond_def_weights = (~np.isnan(flux_ref_exp)) & (flux_ref_exp>0.)
+    cond_def_weights = (~np.isnan(flux_ref_exp)) & (flux_ref_exp>ref_val)
     if np.sum(cond_def_weights)==0:stop('Issue with master definition')
 
     #Spectral corrections
     #    - all corrections that are applied between the input spectra and the spectra processed per visit should be included in this function:
     # > instrumental calibration: uploaded from 'gcal_inputs' for every type of data
     #   for original 2D or 1D spectra, it returns the estimated spectral calibration profiles for each exposure 
     #   for original CCFs or after conversion into CCFs or from 2D/1D it returns a global calibration
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_conversions/ANTARESS_conv.py` & `antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_conv.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_conversions/ANTARESS_masks_gen.py` & `antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_masks_gen.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_conversions/ANTARESS_sp_cont.py` & `antaress-1.1.1/src/antaress/ANTARESS_conversions/ANTARESS_sp_cont.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_conversions/KitCat/KitCat_main.py` & `antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/KitCat_main.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_conversions/KitCat/Kitcat_classes.py` & `antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/Kitcat_classes.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_conversions/KitCat/Kitcat_functions.py` & `antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/Kitcat_functions.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_conversions/KitCat/setup_lbl_fit.py` & `antaress-1.1.1/src/antaress/ANTARESS_conversions/KitCat/setup_lbl_fit.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_calib.py` & `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_calib.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_detrend.py` & `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_detrend.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_flux_balance.py` & `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_flux_balance.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_interferences.py` & `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_interferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 import matplotlib.pyplot as plt
 from scipy.interpolate import interp1d,CubicSpline
 from astropy.timeseries import LombScargle
 from scipy import stats
 import itertools
 from scipy.signal import savgol_filter
 from matplotlib.ticker import MultipleLocator
-from ..ANTARESS_plots.utils_plots import autom_x_tick_prop,autom_y_tick_prop,custom_axis
+from ..ANTARESS_plots.utils_plots import autom_tick_prop,custom_axis
 from ..ANTARESS_conversions.ANTARESS_binning import calc_bin_prof,resample_func,sub_calc_bins,sub_def_bins,weights_bin_prof
 from ..ANTARESS_grids.ANTARESS_coord import get_timeorbit,calc_tr_contacts
-from ..ANTARESS_analysis.ANTARESS_ana_comm import model_par_names,par_formatting
+from ..ANTARESS_analysis.ANTARESS_ana_comm import par_formatting
 from ..ANTARESS_general.utils import stop,np_where1D,is_odd,closest,dataload_npz,gen_specdopshift,check_data,datasave_npz
 from ..ANTARESS_general.constant_data import c_light
 from ..ANTARESS_general.minim_routines import init_fit,fit_merit,call_lmfit
 
 
 def MAIN_corr_wig(inst,gen_dic,data_dic,coord_dic,data_prop,plot_dic,system_param):
     r"""**Main wiggle correction routine.**    
@@ -73,29 +73,29 @@
     if len(gen_dic['wig_vis'])==0:gen_dic['wig_vis']=data_inst['visit_list']
 
     #Calculating data
     if gen_dic['calc_wig'] :
         print('         Fitting/correcting wiggles') 
         fixed_args = {'rasterized':True}
 
+        #Optional arguments to be passed to the fit functions
+        #    - common to all steps in the module
+        fixed_args['use_cov'] = False 
+
         #Wiggle filter
         if gen_dic['wig_exp_filt']['mode']: 
             if gen_dic['wig_norm_ord']:print("WARNING: it is advised to disable gen_dic['wig_norm_ord'] with filter mode")
             fit_dic = {}
 
             #Disable analytical steps
             for key in ['wig_exp_samp','wig_exp_nu_ana','wig_exp_fit','wig_exp_point_ana','wig_vis_fit']:gen_dic[key]['mode'] = False
 
         #Analytical wiggle model
         else:
 
-            #Optional arguments to be passed to the fit functions
-            #    - common to all steps in the module
-            fixed_args['use_cov'] = False 
-
             #Reference nu for frequency calculations
             fixed_args['nu_ref'] = c_light/6000. 
         
             #Maximum number of fit evaluations
             fixed_args['max_nfev'] = 10000
 
             #Maximum degree of polynomial frequency variations
@@ -998,15 +998,15 @@
                                         if (vis in gen_dic['wig_exp_samp']['fix_freq2vismod']): 
                                             params_par = {par+sub:coord_fit[par+sub].value for sub in suf_hyper_vis}
                                         fit_prop_dic['mod_prop'][par+'_off']['guess'] = wig_submod_coord_discont(1,params_par,args_loc)[0]
 
                             #Model parameters
                             p_start = Parameters()  
                             par_formatting(p_start,fit_prop_dic['mod_prop'],fit_prop_dic['varpar_priors'],fit_dic,fixed_args_loc,'','',None)
-                            init_fit(fit_dic,fixed_args_loc,p_start,model_par_names(),fit_prop_dic)                          
+                            init_fit(fit_dic,fixed_args_loc,p_start,fit_prop_dic,model_par_names,model_par_units)                    
 
                             #Initialize band fit results
                             #    - we only store constant coefficients of the amplitude and frequency hyper-parameters, for the highest fitted component
                             #    - set main amplitude and frequency coefficients as constant fit properties
                             fit_results = {'par_list' : [] }   
                             for par in ['AmpGlob'+str(fixed_args_loc['comp_id_max'])+'_c0_off','Freq'+str(fixed_args_loc['comp_id_max'])+'_c0_off']:
                                 if not (('Freq' in par) and (fixed_args_loc['comp_id_max'] in comp_freqfixed)):
@@ -1177,15 +1177,15 @@
                                         fit_prop_dic['mod_prop']['Freq'+comp_str+'_c0_off']={'guess':np.nan,'vary':False,'expr':'Freq'+str(comp_id-1)+'_c0_off - '+delta_freq}
                                         fit_prop_dic['varpar_priors']['Freq'+comp_str+'_c0_off']={'low':0.,'high':5.} 
                        
                             #Model parameters
                             #    - initialized with generic parameter values
                             p_start = Parameters()  
                             par_formatting(p_start,fit_prop_dic['mod_prop'],fit_prop_dic['varpar_priors'],fit_dic,fixed_args_loc,'','',None)
-                            init_fit(fit_dic,fixed_args_loc,p_start,model_par_names(),fit_prop_dic)  
+                            init_fit(fit_dic,fixed_args_loc,p_start,fit_prop_dic,model_par_names,model_par_units)     
 
                             #------------------------------
     
                             #Fit model to data
                             p_best = p_start
                             if gen_dic['wig_exp_fit']['use']:
                       
@@ -2135,15 +2135,15 @@
                             for pref,suf in zip(pref_names_freq[comp_id],suf_names_freq[comp_id]):
                                 for suf_coord in suf_hyper_vis:fit_prop_dic['mod_prop'][pref+comp_str+suf+suf_coord]['vary']  = False                                          
     
     
                     #Parameter initialization
                     p_start = Parameters()  
                     par_formatting(p_start,fit_prop_dic['mod_prop'],fit_prop_dic['varpar_priors'],fit_dic,fixed_args_loc,'','',None)
-                    init_fit(fit_dic,fixed_args_loc,p_start,model_par_names(),fit_prop_dic) 
+                    init_fit(fit_dic,fixed_args_loc,p_start,fit_prop_dic,model_par_names,model_par_units)     
                 
                 #Retrieve previous fit
                 if vis in gen_dic['wig_vis_fit']['reuse']:
                     globvisfit_results = np.load(gen_dic['wig_vis_fit']['reuse'][vis],allow_pickle=True)['data'].item()
                     p_start = globvisfit_results['p_best']   
 
                 #Parameter initialization
@@ -2421,16 +2421,16 @@
                             plt.plot([cen_ph_mer,cen_ph_mer],y_range_plot,linestyle=':',color='black',zorder=1)  
                             if cen_ph_guid is not None:plt.plot([cen_ph_guid,cen_ph_guid],y_range_plot,linestyle='--',color='black',zorder=1)  
 
                             #Main planet contacts
                             for cont_ph in contact_phases:plt.plot([cont_ph,cont_ph],y_range_plot,color='black',linestyle=':',lw=0.5,zorder=0)
 
                             #Frame
-                            xmajor_int,xminor_int,xmajor_form=autom_x_tick_prop(x_range_plot[1]-x_range_plot[0]) 
-                            ymajor_int,yminor_int,ymajor_form=autom_y_tick_prop(y_range_plot[1]-y_range_plot[0]) 
+                            xmajor_int,xminor_int,xmajor_form=autom_tick_prop(x_range_plot[1]-x_range_plot[0]) 
+                            ymajor_int,yminor_int,ymajor_form=autom_tick_prop(y_range_plot[1]-y_range_plot[0]) 
                             custom_axis(plt,position=[0.15,0.15,0.95,0.7],
                                         x_range=x_range_plot,xmajor_int=xmajor_int,xminor_int=xminor_int,xmajor_form=xmajor_form,
                                         y_range=y_range_plot,ymajor_int=ymajor_int,yminor_int=yminor_int,ymajor_form=ymajor_form,dir_y='out',
                                         x_title='Orbital phase',y_title=chrompar,font_size=14,xfont_size=14,yfont_size=14)
                             plt.savefig(path_loc+chrompar+'.png')                  
                             plt.close() 
 
@@ -2476,15 +2476,15 @@
                                 #Plot model for current exposure
                                 plt.plot(fixed_args_loc['nu_HR'],par_mod,linestyle='-',lw=lw_plot,color = col_exp)
                                 y_min=np.min([np.min(par_mod),y_min])
                                 y_max=np.max([np.max(par_mod),y_max])   
                             
                             #Frame
                             y_range_plot=np.array([y_min,y_max]) 
-                            ymajor_int,yminor_int,ymajor_form=autom_y_tick_prop(y_range_plot[1]-y_range_plot[0]) 
+                            ymajor_int,yminor_int,ymajor_form=autom_tick_prop(y_range_plot[1]-y_range_plot[0]) 
                             custom_axis(plt,position=[0.15,0.15,0.95,0.7],
                                         x_range=x_range_plot,xmajor_int=5,xminor_int=1.,
                                         y_range=y_range_plot,ymajor_int=ymajor_int,yminor_int=yminor_int,ymajor_form=ymajor_form,dir_y='out',
                                         xmajor_form='%i',x_title=r'$\nu$ (10$^{-10}$ s$^{-1}$)',y_title=prop_name,font_size=14,xfont_size=14,yfont_size=14)
                             
                             plt.savefig(path_loc+prop_name+'_comp'+str(comp_id)+'.png')                  
                             plt.close()                             
@@ -2966,27 +2966,27 @@
         #Index of global order
         if iexp_plt==expbin_list[0]:
             dsign_txt = 1. if is_odd(iord_plt) else -1.
             plt.text(np.mean(Fr_bin_fit['nu'][ibin_group]),y_range[1]+(0.1+dsign_txt*0.05)*(y_range[1]-y_range[0]),str(iord_plt),verticalalignment='center', horizontalalignment='center',fontsize=10.,zorder=15,color='black') 
  
     #Binned data
     #    - we use resample_func() rather than bind.resampling because input tables are not necessarily continuous, and because the calculations here are less generic than those in process_bin_prof()
-    plot_bin_spec(plt.gca(),Fr_bin_fit['low_nu'],Fr_bin_fit['high_nu'],Fr_bin_fit['Fr'],min_plot,max_plot,0.27/5.,Fr_bin_fit)
+    plot_bin_spec(plt.gca(),Fr_bin_fit['low_nu'],Fr_bin_fit['high_nu'],Fr_bin_fit['Fr'],min_plot,max_plot,0.27/5.)
 
     #Constant unity level
     plt.plot(x_range,[1.,1.],linestyle=':',color='black',zorder=-1,rasterized=fixed_args['rasterized'])
  
     #Dispersion of fitted spectrum
     dx_range = x_range[1]-x_range[0]
     dy_range = y_range[1]-y_range[0]
     plt.text(x_range[1]-0.1*dx_range,y_range[1]-0.2*dy_range,'RMS ='+"{0:.4e}".format(rms),verticalalignment='center', horizontalalignment='left',fontsize=9.,zorder=10,color='black')     
  
     #Frame
-    xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(x_range[1]-x_range[0])
-    ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(y_range[1]-y_range[0])  
+    xmajor_int,xminor_int,xmajor_form = autom_tick_prop(x_range[1]-x_range[0])
+    ymajor_int,yminor_int,ymajor_form = autom_tick_prop(y_range[1]-y_range[0])  
     xmajor_int = 1.
     xminor_int = 0.5
     custom_axis(plt,position=[0.15,0.15,0.95,0.7],
                 x_range=x_range,xmajor_int=xmajor_int,xminor_int=xminor_int,
                 y_range=y_range,ymajor_int=ymajor_int,yminor_int=yminor_int,ymajor_form=ymajor_form,dir_y='out',
                 xmajor_form=xmajor_form,x_title=r'$\nu$ (10$^{-10}$ s$^{-1}$)',y_title='Flux ratio',font_size=16,xfont_size=16,yfont_size=16)
     plt.savefig(plot_path+'.png')
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_peaks.py` & `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_peaks.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_sp_reduc.py` & `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_sp_reduc.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_corrections/ANTARESS_tellurics.py` & `antaress-1.1.1/src/antaress/ANTARESS_corrections/ANTARESS_tellurics.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_corrections/Telluric_processing/Create_static_files.py` & `antaress-1.1.1/src/antaress/ANTARESS_corrections/Telluric_processing/Create_static_files.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_general/constant_data.py` & `antaress-1.1.1/src/antaress/ANTARESS_general/constant_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -190,89 +190,90 @@
     # + alpha: evaporation coefficient that parameterises kinetic inhibition of the sublimation process (from Van Lieshout et al. 2014)
     #          set arbitrarily to 0.1 when unknown  
     #    - see change_state for how to obtain L and Pinf from A and B in Van Lieshout+2014 
     #################################################################
  
     # Alumina (gamma alumina)
     #    - from Budaj+2015
+    #    - we assume sublimation releases 2 Al (Mg = 26.981539 amu) and 3 O (15.999 amu)
     'alumina':{
         'nature':'dust',
         'rho':2.9,
-        'Mg':np.nan,
+        'Mg':101.96, #=2*26.981539 + 3*15.999
         'L':np.nan,
         'Pinf':np.nan,
         'alpha':0.1 #arbitrary
     }, 
     # Ammonia
     #    - from Budaj+2015
-    'Ammonia':{   
+    'ammonia':{   
         'nature':'dust', 
         'rho': 0.88,
         'Mg':np.nan,
         'L':np.nan,
         'Pinf':np.nan,
         'alpha':0.1 #arbitrary
     },      
     # Carbon at T=400°C 
     #    - opacity in Budaj+2015 is calculated for T=400°C
     #    - we assume the properties for Graphite in Van Lieshout et al. 2014 are valid for this type of carbon   
-    'carb400':{
+    'carbon0400':{
         'nature':'dust',
         'rho':1.435,            #Budaj+2015 (T=400°C). Van Lieshout et al. 2014 gives 2.16 for graphite 
         'Mg':12.011,            #Van Lieshout et al. 2014
         'L':64825562.918477856, #=93646.*k_boltz/(12.011*amu), from Van Lieshout et al. 2014
         'Pinf':8.68175420053e14,#=0.1*np.exp(36.7), from Van Lieshout et al. 2014
         'alpha':0.1             #arbitrary
     },
     # Carbon at T=1000°C 
     #    - opacity in Budaj+2015 is calculated for T=1000°C
-    'carb1000':{
+    'carbon1000':{
         'nature':'dust',
         'rho':1.988,            #Budaj+2015 (T=400°C). Van Lieshout et al. 2014 gives 2.16 for graphite
         'Mg':12.011,            #Van Lieshout et al. 2014
         'L':64825562.918477856, #=93646.*k_boltz/(12.011*amu), from Van Lieshout et al. 2014
         'Pinf':8.68175420053e14,#=0.1*np.exp(36.7), from Van Lieshout et al. 2014
         'alpha':0.1             #arbitrary 
     },    
     # Corundum (Al2O3 = alpha alumina)
     #    - from Van Lieshout et al. 2014
-    'Corundum':{
+    'corundum':{
         'nature':'dust',
         'rho':2.9, #from Budaj+2015, for consistency with its opacity table (see note in their section 4.1)
         'Mg':101.961,
         'L':6308798.7788943825, #=77365.*k_boltz/(101.961*amu)
         'Pinf':1.16888864240e16,#=0.1*np.exp(39.3)
         'alpha':0.1 #arbitrary
     }, 
     # Cryst. enstatite (MgSiO3)
     #    - from Van Lieshout et al. 2014
     #    - considered as an iron-free pyroxene in Budaj+2015
-    'Enstatite':{
+    'enstatite':{
         'nature':'dust',
         'rho':3.20,
         'Mg':100.389,
         'L':5707156.068029924, #=68908.*k_boltz/(100.389*amu)
         'Pinf':3.5206249346e15,#=0.1*np.exp(38.1)
         'alpha':0.1 #arbitrary
     },   
     # Cryst. fayalite (Fe2SiO4)
     #    - from Van Lieshout et al. 2014
     #    - no associated cross-section
-    'Fayalite':{
+    'fayalite':{
         'nature':'dust',
         'rho':4.39,
         'Mg':203.774,
         'L':2463536.4452695027, #=60377.*k_boltz/(203.774*amu)
         'Pinf':2.35994546824e15,#=0.1*np.exp(37.7)
         'alpha':0.1
     }, 
     # Cryst. forsterite (Mg2SiO4)
     #    - from Van Lieshout et al. 2014
     #    - considered as an iron-free olivine in Budaj+2015
-    'Forsterite':{
+    'forsterite':{
         'nature':'dust',
         'rho':3.27,
         'Mg':140.694,
         'L':3859464.3979731086, #=65308.*k_boltz/(140.694*amu)   
         'Pinf':6.44824949651e13,#=0.1*np.exp(34.1)
         'alpha':0.1 #arbitrary
     },       
@@ -287,57 +288,57 @@
         'Pinf':4.8017425537e11, #=0.1*np.exp(29.2)
 #        'Pinf':7.801e9,   ????
         'alpha':1.
     }, 
     # Olivine
     #    - Budaj+2015 opacities are for iron-enriched olivine (Mg(1) Fe(1) SiO4) with half–half of Mg–Fe atoms 
     #      Kimura+2002 values are for (Mg(1.1) Fe(0.9) SiO(4) ) olivine     
-    'Olivine50':{
+    'olmg50':{
         'nature':'dust',
         'rho': 3.0,     #Budaj+2015 
         'Mg': 169.0809, #Kimura+2002
         'L':3.21e6,     #Kimura+2002
         'Pinf':6.72e13, #Kimura+2002
         'alpha':0.1 #arbitrary
     },       
     # Perovskite (CaTiO3)
     #    - from Budaj+2015
-    'Perovskite':{
+    'perovskite':{
         'nature':'dust',
         'rho': 4.1,
         'Mg':np.nan,
         'L':np.nan,
         'Pinf':np.nan,
         'alpha':0.1      #arbitrary
     },  
     # Pyroxene 20% iron
-    #    - opacity in Budaj+2015 is calculated for Mg(0.8) Fe(0.2) SiO3  , but note they correspond to SiO2 alone 
-    'Pyroxene80':{
+    #    - opacity in Budaj+2015 is calculated for Mg(0.8) Fe(0.2) SiO3, but note they correspond to SiO2 alone 
+    'pyrmg80':{
         'nature':'dust',
         'rho': 3.0,      #Budaj+2015  
         'Mg':106.6955,   #=0.8*24.305+0.2*55.845+28.0855+3.*15.999     
         'L':9.61e6,      #Kimura et al. 2002   
         'Pinf':3.13e10,  #Kimura et al. 2002
         'alpha':0.1      #arbitrary
     },
     # Pyroxene 60% iron
     #    - opacity in Budaj+2015 is calculated for Mg(0.4) Fe(0.6) SiO3
     #      we assume the sublimation properties from Kimura+2002 are valid for this composition, but note they correspond to SiO2 alone 
-    'Pyroxene40':{
+    'pyrmg40':{
         'nature':'dust',
         'rho': 3.0,      #Budaj+2015
         'Mg':119.3115,   #=0.4*24.305+0.6*55.845+28.0855+3.*15.999
-        'L':9.61e6,     #Kimura et al. 2002
+        'L':5e6,     #Kimura et al. 2002
         'Pinf':3.13e10, #Kimura et al. 2002
         'alpha':0.1     #arbitrary
     }, 
     # Quartz (SiO2)
     #    - from Van Lieshout et al. 2014
     #    - no associated cross-section
-    'Quartz':{
+    'quartz':{
         'nature':'dust',
         'rho':2.60,
         'Mg':60.084,
         'L':9609750.740329912, #=69444.*k_boltz/(60.084*amu)
         'Pinf':2.3721784213e13,#=0.1*np.exp(33.1)
         'alpha':1.0
     }, 
@@ -361,25 +362,25 @@
         'Mg':44.085,
         'L':9339551.536356324,  #=49520.*k_boltz/(44.085*amu)
         'Pinf':1.30187912050e13,#=0.1*np.exp(32.5)
         'alpha':0.04
     },
     # Water Ice
     #    - from Budaj+2015
-    'wtrice':{
+    'waterice':{
         'nature':'dust',
         'rho': 1.0 ,
         'Mg':np.nan,
         'L':np.nan,
         'Pinf':np.nan,
         'alpha':0.1 #arbitrary
     },
     # Water Liquid
     #    - from Budaj+2015
-    'wtrliq':{
+    'waterliq':{
         'nature':'dust',
         'rho': 1.0 ,
         'Mg':np.nan,
         'L':np.nan,
         'Pinf':np.nan,
         'alpha':0.1 #arbitrary
     },
@@ -507,114 +508,10 @@
     #Rayleigh scattering from He
     'He_Rayleigh':{'type':'broadband','species':'He_0+_g','dependance':False},
 
     #Hydrogen photoionization
     'H0_XUV':{'type':'broadband','species':'H_0+_g','dependance':False},
 
 
-    #################################################################
-    #Tabulated processes
-    #    - file indicate path to tabulated cross-section, stored in 'EVE/Tabulated_cs/'
-    #################################################################
-
-    # Alumina (gamma alumina)
-    'alum_abs_scat':{
-        'type':'tabulated',
-        'species':'alumina',
-        'file':'Dust_Budaj2015/alumina_opac_all',
-        'dependance':True
-    }, 
-    # Ammonia
-    'ammo_abs_scat':{    
-        'type':'tabulated',
-        'species':'Ammonia',
-        'file':'Dust_Budaj2015/ammonia_opac_all',
-        'dependance':True
-    },
-    # Carbon at 400°C
-    'carb400_abs_scat':{
-        'type':'tabulated',
-        'species':'carb400',
-        'file':'Dust_Budaj2015/carbon0400_opac_all',
-        'dependance':True
-    },
-    # Carbon at 1000°C 
-    'carb1000_abs_scat':{
-        'type':'tabulated',
-        'species':'carb1000',
-        'file':'Dust_Budaj2015/carbon1000_opac_all',
-        'dependance':True
-    },    
-    # Corundum (Al2O3 = alpha alumina)
-    'corun_abs_scat':{
-        'type':'tabulated',
-        'species':'Corundum',
-        'file':'Dust_Budaj2015/corundum_opac_all',
-        'dependance':True
-    },  
-    # Enstatite
-    'ensta_abs_scat':{
-        'type':'tabulated',
-        'species':'Enstatite',
-        'file':'Dust_Budaj2015/enstatite_opac_all',
-        'dependance':True
-    },    
-    # Iron
-    'iron_abs_scat':{
-        'type':'tabulated',
-        'species':'iron',
-        'file':'Dust_Budaj2015/iron_opac_all',
-        'dependance':True
-    },   
-    # Forsterite
-    'fost_abs_scat':{
-        'type':'tabulated',
-        'species':'Forsterite',
-        'file':'Dust_Budaj2015/forsterite_opac_all',
-        'dependance':True
-    }, 
-    # Olivine
-    'olmg50_abs_scat':{
-        'type':'tabulated',
-        'species':'Olivine50',
-        'file':'Dust_Budaj2015/olmg50_opac_all',
-        'dependance':True
-    },    
-    # Perovskite (CaTiO3)
-    'perov_abs_scat':{
-        'type':'tabulated',
-        'species':'Perovskite',
-        'file':'Dust_Budaj2015/perovskite_opac_all',
-        'dependance':True
-    },    
-    # Pyroxene 60% iron
-    'pyr40_abs_scat':{
-        'type':'tabulated',
-        'species':'Pyroxene40',
-        'file':'Dust_Budaj2015/pyrmg40_opac_all',
-        'dependance':True
-    },
-    # Pyroxene 20% iron
-    'pyr80_abs_scat':{
-        'type':'tabulated',
-        'species':'Pyroxene80',
-        'file':'Dust_Budaj2015/pyrmg80_opac_all',
-        'dependance':True
-    },    
-    # Water Ice
-    'wtrice_abs_scat':{
-        'type':'tabulated',
-        'species':'wtrice',
-        'file':'Dust_Budaj2015/waterice_opac_all',
-        'dependance':True
-    },
-    # Water Liquid
-    'wtrliq_abs_scat':{
-        'type':'tabulated',
-        'species':'wtrliq',
-        'file':'Dust_Budaj2015/waterliq_opac_all',
-        'dependance':True
-    }
-
    
 }
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_general/minim_routines.py` & `antaress-1.1.1/src/antaress/ANTARESS_general/minim_routines.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 import os as os_system
 from pathos.multiprocessing import Pool
 import scipy.linalg
 from scipy import stats
 from copy import deepcopy
 from lmfit import minimize, report_fit
 from scipy import special
-from ..ANTARESS_plots.utils_plots import custom_axis,autom_y_tick_prop
+from ..ANTARESS_plots.utils_plots import custom_axis,autom_tick_prop
 from ..ANTARESS_general.utils import np_where1D,stop,npint,init_parallel_func,get_time
-
     
 ##################################################################################################
 #%%% Probability distributions
 ##################################################################################################   
 
 def ln_prior_func(p_step,fixed_args): 
     r"""**Log(prior)**
@@ -228,22 +227,29 @@
             fixed_args['fixed_par_val'][par]=eval(fixed_args['linked_par_expr'][par])
          
     #Include fixed parameters into local input dictionary
     p_step_all.update(fixed_args['fixed_par_val'])
     
     #Prior function
     ln_prior = ln_prior_func(p_step_all,fixed_args)
-        
-    #Likelihood function
-    ln_lkhood = ln_lkhood_func_mcmc(p_step_all,fixed_args)[0]
     
-    #Set log-probability to -inf if likelihood is nan
-    #    - happens when parameters go beyond their boundaries (hence ln_prior=-inf) but the model fails (hence ln_lkhood = nan)
-    ln_prob=-np.inf if np.isnan(ln_lkhood) else ln_prior + ln_lkhood
-  
+    #Undefined log-prior
+    #     - if the walker move to parameters outside the defined prior range, then the log-prior will be set to inf.
+    #       as a result, there is no point in calculating the log-likelihood in this case.
+    if not np.isinf(ln_prior):
+
+        #Likelihood function
+        ln_lkhood = ln_lkhood_func_mcmc(p_step_all,fixed_args)[0]
+
+        #Set log-probability to -inf if likelihood is nan
+        #    - happens when parameters go beyond their boundaries (hence ln_prior=-inf) but the model fails (hence ln_lkhood = nan)
+        ln_prob=-np.inf if np.isnan(ln_lkhood) else ln_prior + ln_lkhood
+
+    else: ln_prob=-np.inf
+
     return ln_prob
 
 
  
 def ln_prob_func_lmfit(p_step, x_val, fixed_args=None):
     r"""**Log-probability function: lmfit**
 
@@ -327,15 +333,15 @@
 
 
 
 ##################################################################################################
 #%%% Minimization routines
 ##################################################################################################   
 
-def init_fit(fit_dic,fixed_args,p_start,par_names_txt,fit_prop_dic):
+def init_fit(fit_dic,fixed_args,p_start,fit_prop_dic,model_par_names,model_par_units):
     r"""**Fit initialization**
 
     Initializes lmfit and MCMC.
       
     Args:
         TBD
     
@@ -363,53 +369,69 @@
     var_par_list=[]
     ivar_par_list=[]
     ifix_par_list=[]
     fix_par_list=[]
     iexp_par_list=[]
     exp_par_list=[]
     var_par_names=[]
+    var_par_units=[]
     for ipar,par in enumerate(fixed_args['par_names']):
         if p_start[par].vary:
             var_par_list+=[par]
             ivar_par_list+=[ipar]
+            par_name_fit = par.split('__')[0]
+            par_name_loc = model_par_names(par_name_fit)
             if ('__' in par):
-                par_name_loc = par.split('__')[0]
-                if par_name_loc in par_names_txt:par_name_loc = par_names_txt[par_name_loc]
                 inst_par = '_'
                 vis_par = '_'
-                pl_name = None
+                pl_name = None                
+                sp_name = None
+                
+                #Parameter depends on epoch
                 if ('__IS') and ('_VS') in par:
                     inst_vis_par = par.split('__IS')[1]
                     inst_par  = inst_vis_par.split('_VS')[0]
-                    vis_par  = inst_vis_par.split('_VS')[1]       
+                    vis_par  = inst_vis_par.split('_VS')[1]   
+                    if ('__sp' in par):sp_name = (par.split('__IS')[0]).split('__sp')[1]                    
                     if ('__pl' in par):pl_name = (par.split('__IS')[0]).split('__pl')[1]
+                
+                #Parameter does not depend on epoch
                 else:
-                    pl_name = par.split('__pl')[1]                                                                 
+                    if ('__sp' in par):sp_name = par.split('__sp')[1]   
+                    if ('__pl' in par):pl_name = par.split('__pl')[1]                                                                 
+                if sp_name is not None:par_name_loc+='['+sp_name+']'
                 if pl_name is not None:par_name_loc+='['+pl_name+']'                             
                 if inst_par != '_':
                     par_name_loc+='['+inst_par+']'
                     if vis_par != '_':par_name_loc+='('+vis_par+')'
-                var_par_names+=[par_name_loc]
-            else:
-                if par in par_names_txt:var_par_names+=[par_names_txt[par]]
-                else:var_par_names+=[par]
+            var_par_names+=[par_name_loc]
+            var_par_units+=[model_par_units(par_name_fit)]
+
         else:
             ifix_par_list+=[ipar]
             fix_par_list+=[par]
         if p_start[par].expr!=None:
             p_start[par].vary=False
             iexp_par_list+=[ipar]
             exp_par_list+=[par]
     fixed_args['var_par_list']=np.array(var_par_list,dtype='U50')  
     fixed_args['ivar_par_list']=ivar_par_list
     fixed_args['ifix_par_list']=ifix_par_list
     fixed_args['fix_par_list']=fix_par_list
     fixed_args['iexp_par_list']=iexp_par_list
     fixed_args['exp_par_list']=exp_par_list
     fixed_args['var_par_names']=np.array(var_par_names,dtype='U50')
+    fixed_args['var_par_units']=np.array(var_par_units,dtype='U50')
+
+    #Retrieve the number of spots that are present (whether their parameters are fixed or fitted)
+    spot_names=[]
+    for par in fixed_args['par_names']:
+        if '__sp' in par:
+            spot_names.append(par.split('__sp')[1])
+    fixed_args['num_spots']=len(np.unique(spot_names))
 
     #Update value of fixed parameters linked to variable parameters through an expression
     if len(fixed_args['linked_par_expr'])>0:
         
         #Attribute their fixed value to parameters that are not variable and not linked via an expression, but might be used in the expression of other non-variable parameters
         fixed_args['fixed_par_val_noexp_list']=[par for par in fixed_args['fixed_par_val'] if par not in fixed_args['linked_par_expr']]
 
@@ -651,28 +673,31 @@
 
     #Save temporary walkers in case of crash
     if ('monitor' in fit_dic) and fit_dic['monitor']:
         backend = emcee.backends.HDFBackend(fit_dic['save_dir']+'monitor'+str(fit_dic['nwalkers'])+'_steps'+str(fit_dic['nsteps'])+run_name+'.h5')
         backend.reset(fit_dic['nwalkers'], fit_dic['merit']['n_free'])
     else:backend=None
 
-    #Multiprocessing
-    if nthreads>1:pool_proc = Pool(processes=nthreads)  
-    print('         Running with '+str(nthreads)+' threads')
     
     #Call to MCMC
     st0=get_time()
     n_free=np.shape(fit_dic['initial_distribution'])[1]
-    sampler = emcee.EnsembleSampler(fit_dic['nwalkers'],            #Number of walkers
-                                    n_free,                         #Number of free parameters in the model
-                                    ln_prob_func_mcmc,              #Log-probability function 
-                                    args=[fixed_args],              #Fixed arguments for the calculation of the likelihood and priors
-                                    pool = pool_proc,
-                                    backend=backend)                #Monitor chain progress 
 
+    #Multiprocessing
+    if nthreads>1:
+        pool_proc = Pool(processes=nthreads)  
+        print('         Running with '+str(nthreads)+' threads')    
+        sampler = emcee.EnsembleSampler(fit_dic['nwalkers'],            #Number of walkers
+                                        n_free,                         #Number of free parameters in the model
+                                        ln_prob_func_mcmc,              #Log-probability function 
+                                        args=[fixed_args],              #Fixed arguments for the calculation of the likelihood and priors
+                                        pool = pool_proc,
+                                        backend=backend)                #Monitor chain progress 
+    else:sampler = emcee.EnsembleSampler(fit_dic['nwalkers'],n_free,ln_prob_func_mcmc,args=[fixed_args],backend=backend)         
+        
     #Run MCMC
     #    - possible options:
     # + iterations: number of iterations to run            
     sampler.run_mcmc(fit_dic['initial_distribution'], fit_dic['nsteps'],progress=fit_dic['progress'])
     if verbose:print('   duration : '+str((get_time()-st0)/60.)+' mn')
    
     #Walkers chain
@@ -1170,28 +1195,28 @@
         #Calculate intervals from density distribution
         jumpind,bins_in_HDI,sorted_binnumber = prep_MCMC_HDI(dbin_par,dens_par,frac_search) 
     
     #Single interval
     if len(jumpind)==0:
         HDI_sub=[np.min(bin_edges_par[bins_in_HDI]),np.max(bin_edges_par[bins_in_HDI+1])]
         HDI_interv_par+=[HDI_sub]
-        HDI_interv_txt_par+='['+"{0:.8e}".format(HDI_sub[0])+' ; '+"{0:.8e}".format(HDI_sub[1])+']'
-        HDI_sig_txt_par+='[-'+"{0:.8e}".format(med_par-HDI_sub[0])+' +'+"{0:.3e}".format(HDI_sub[1]-med_par)+']'
+        HDI_interv_txt_par+='['+"{0:.3e}".format(HDI_sub[0])+' ; '+"{0:.3e}".format(HDI_sub[1])+']'
+        HDI_sig_txt_par+='[-'+"{0:.3e}".format(med_par-HDI_sub[0])+' +'+"{0:.3e}".format(HDI_sub[1]-med_par)+']'
     
     #Multiple intervals
     else:        
         for i_int in range(len(jumpind)+1):
             if i_int==0:ji=0
             else:ji=jumpind[i_int-1]+1     
             if i_int==len(jumpind):jf=-1
             else:jf=jumpind[i_int]
             HDI_sub=[bin_edges_par[sorted_binnumber[ji]],bin_edges_par[sorted_binnumber[jf]+1]]
             HDI_interv_par+=[HDI_sub]
-            HDI_interv_txt_par+='['+"{0:.8e}".format(HDI_sub[0])+' ; '+"{0:.8e}".format(HDI_sub[1])+']' 
-            HDI_sig_txt_par+='[-'+"{0:.8e}".format(med_par-HDI_sub[0])+' +'+"{0:.3e}".format(HDI_sub[1]-med_par)+']' 
+            HDI_interv_txt_par+='['+"{0:.3e}".format(HDI_sub[0])+' ; '+"{0:.3e}".format(HDI_sub[1])+']' 
+            HDI_sig_txt_par+='[-'+"{0:.3e}".format(med_par-HDI_sub[0])+' +'+"{0:.3e}".format(HDI_sub[1]-med_par)+']' 
    
     #Convert into array
     HDI_interv_par=np.array(HDI_interv_par)            
 
     #Calculate HDI fraction for verification
     HDI_frac_par=np.sum(dens_par[bins_in_HDI],dtype=float)/np.sum(dens_par,dtype=float)
     HDI_interv_txt_par+=' ('+"{0:.2f}".format(100.*HDI_frac_par)+' %)'    
@@ -1321,28 +1346,28 @@
         cdf = np.cumsum(sw)[:-1]
         cdf /= cdf[-1]
         cdf = np.append(0, cdf)
         return np.interp(q, cdf, x[idx]).tolist()
 
 
  
-def MCMC_estimates(merged_chain,fixed_args,fit_dic,verbose=True,print_par=True,calc_quant=True):
+def MCMC_estimates(merged_chain,fixed_args,fit_dic,verbose=True,print_par=True,calc_quant=True,verb_shift=''):
     r"""**MCMC post-proc: best fit**
 
     Calculates best estimates and confidence intervals for fitted MCMC parameters.
       
     Args:
         TBD
     
     Returns:
         TBD
     
     """  
     n_par=len(merged_chain[0,:])
-    
+  
     #Median
     med_par=np.median(merged_chain, axis=0)   
     
     #Use median values of variable parameters as best estimate for the nominal model
     #    - parameters in 'merged_chain' and thus 'med_par' have the same order as in var_par_list
     #    - p_best is a regular dictionary and thus loses the order of the initial p_best
     #    - fixed parameters defined through expressions are defined after the best-fit variable values
@@ -1450,41 +1475,42 @@
         HDI_interv=None
         HDI_interv_txt=None
         HDI_sig_txt_par = None
             
     #----------------------------------------------------        
 
     #Print results
-    if verbose:
-        print('-------------------------------')      
-        print('Results')
-        print('-------------------------------')
-        print("Chain covariance: "+str(np.cov(np.transpose(merged_chain))))
-        print("Chain coefficient correlations: "+str(np.corrcoef(np.transpose(merged_chain))))
-    if print_par:
-        print('-------------------------------')                
-        for ipar,parname in enumerate(fixed_args['var_par_list']):
-            print('Parameter '+parname)
-            print('  > med :'+"{0:.8e}".format(med_par[ipar]))            
-            for sig in fit_dic['sig_list']:
-                print('  > '+sig+' err : -'+"{0:.3e}".format(sig_par_err[sig][0,ipar])+' +'+"{0:.3e}".format(sig_par_err[sig][1,ipar]))  
-                print('  > '+sig+' int : ['+"{0:.3e}".format(sig_par_val[sig][0,ipar])+' ; '+"{0:.3e}".format(sig_par_val[sig][1,ipar])+']')  
+    if verbose or print_par:
+        print(verb_shift+'-------------------------------') 
+        print(verb_shift+'> Results')       
+    if verbose:    
+        print(verb_shift+"  Chain covariance: "+str(np.cov(np.transpose(merged_chain))))
+        print(verb_shift+"  Chain coefficient correlations: "+str(np.corrcoef(np.transpose(merged_chain))))
+    if print_par:             
+        for ipar,(parname,parunit) in enumerate(zip(fixed_args['var_par_list'],fixed_args['var_par_units'])):
+            if ipar>0:print(verb_shift+'-------------------------------') 
+            print(verb_shift+'  Parameter '+parname+' ['+parunit+']')
+            print(verb_shift+'    med : '+"{0:.3e}".format(med_par[ipar]))            
             if fit_dic['HDI'] is not None:
-                print('  > HDI '+fit_dic['HDI']+' err: '+str(HDI_sig_txt_par[ipar]))
-                print('  > HDI '+fit_dic['HDI']+' int : '+str(HDI_interv_txt[ipar]))
+                print(verb_shift+'    HDI    '+fit_dic['HDI']+' err : '+str(HDI_sig_txt_par[ipar]))
+                print(verb_shift+'              int : '+str(HDI_interv_txt[ipar]))
+            else:
+                for sig in fit_dic['sig_list']:
+                    print(verb_shift+'    quant. '+sig+' err : -'+"{0:.3e}".format(sig_par_err[sig][0,ipar])+' +'+"{0:.3e}".format(sig_par_err[sig][1,ipar]))  
+                    print(verb_shift+'              int : ['+"{0:.3e}".format(sig_par_val[sig][0,ipar])+' ; '+"{0:.3e}".format(sig_par_val[sig][1,ipar])+']')  
             if parname in fit_dic['conf_limits']:
                 for lev in fit_dic['conf_limits'][parname]['level']: 
-                    print('  > '+fit_dic['conf_limits'][parname]['limits'][lev] )
+                    print(verb_shift+'    '+fit_dic['conf_limits'][parname]['limits'][lev] )
 
     return p_best,med_par,sig_par_val,sig_par_err,HDI_interv,HDI_interv_txt,HDI_sig_txt_par  
     
     
 
    
-def postMCMCwrapper_1(fit_dic,fixed_args,walker_chains,nthreads,par_names,verbose=True):    
+def postMCMCwrapper_1(fit_dic,fixed_args,walker_chains,nthreads,par_names,verbose=True,verb_shift=''):    
     r"""**MCMC post-proc: raw chains**
 
     Process and analyze MCMC chains of original parameters.
       
     Args:
         TBD
     
@@ -1531,15 +1557,15 @@
         keep_chain = np.repeat(True,fit_dic['nwalkers'])
         low_thresh_par_val,high_thresh_par_val=None,None
 
     #Plot burnt chains
     if (not os_system.path.exists(fit_dic['save_dir'])):os_system.makedirs(fit_dic['save_dir'])
     if (fit_dic['save_MCMC_chains']!=''):
         MCMC_plot_chains(fit_dic['save_MCMC_chains'],fit_dic['save_dir'],fixed_args['var_par_list'],fixed_args['var_par_names'],walker_chains,burnt_chains,fit_dic['nsteps'],fit_dic['nsteps_pb_walk'],
-                    fit_dic['nwalkers'],fit_dic['nburn'],keep_chain,low_thresh_par_val,high_thresh_par_val,fit_dic['exclu_walk_autom'],verbose=verbose)
+                    fit_dic['nwalkers'],fit_dic['nburn'],keep_chain,low_thresh_par_val,high_thresh_par_val,fit_dic['exclu_walk_autom'],verbose=verbose,verb_shift=verb_shift)
      
     #Remove chains if required
     if (False in keep_chain):
         unburnt_chains = unburnt_chains[keep_chain]
         burnt_chains = burnt_chains[keep_chain]
         fit_dic['nwalkers']=np.sum(keep_chain)  
         
@@ -1581,19 +1607,19 @@
         corr_length=MCMC_corr_length(fit_dic,fit_dic['max_corr_length'],nthreads,fixed_args['var_par_list'],merged_chain,0,fit_dic['nsteps_final_merged'],verbose=True)        
  
         #Thin the chain by keeping only one point every maximum correlation length
         #    - in this way the merged_chain over all pararameters are uncorrelated
         fit_dic['nsteps_final_merged'],merged_chain=MCMC_thin_chains(corr_length,merged_chain)
 
     #Best-fit parameters for model calculations
-    p_final,fit_dic['med_parfinal'],fit_dic['sig_parfinal_val'],fit_dic['sig_parfinal_err'],fit_dic['HDI_interv'],fit_dic['HDI_interv_txt'],fit_dic['HDI_sig_txt']=MCMC_estimates(merged_chain,fixed_args,fit_dic,verbose=verbose,print_par=verbose,calc_quant=fit_dic['calc_quant'])
+    p_final,fit_dic['med_parfinal'],fit_dic['sig_parfinal_val'],fit_dic['sig_parfinal_err'],fit_dic['HDI_interv'],fit_dic['HDI_interv_txt'],fit_dic['HDI_sig_txt']=MCMC_estimates(merged_chain,fixed_args,fit_dic,verbose=verbose,print_par=fit_dic['print_par'],calc_quant=fit_dic['calc_quant'],verb_shift=verb_shift)
 
     #Plot merged chains for MCMC parameters
     if (fit_dic['save_MCMC_chains']!=''):
-        MCMC_plot_merged_chains(fit_dic['save_MCMC_chains'],fit_dic['save_dir'],fixed_args['var_par_list'],fixed_args['var_par_names'],merged_chain,fit_dic['nsteps_final_merged'],verbose=verbose)
+        MCMC_plot_merged_chains(fit_dic['save_MCMC_chains'],fit_dic['save_dir'],fixed_args['var_par_list'],fixed_args['var_par_names'],merged_chain,fit_dic['nsteps_final_merged'],verbose=verbose,verb_shift=verb_shift)
  
     #Save 1-sigma and envelope samples for plot in ANTARESS_main
     if fit_dic['calc_envMCMC'] or fit_dic['calc_sampMCMC']:
         par_sample_sig1,par_sample=MCMC_retrieve_sample(fixed_args,fixed_args['fix_par_list'],fixed_args['exp_par_list'],fixed_args['iexp_par_list'],fixed_args['ifix_par_list'],par_names,fixed_args['fixed_par_val'],fit_dic['calc_envMCMC'],merged_chain,fit_dic['merit']['n_free'],fit_dic['nsteps_final_merged'],
                                                         p_final,fixed_args['var_par_list'],fixed_args['ivar_par_list'],fit_dic['calc_sampMCMC'],fixed_args['linked_par_expr'],fit_dic,fit_dic['st_samp'],fit_dic['end_samp'],fit_dic['n_samp'])
         if fit_dic['calc_envMCMC']:print('Saved ',len(par_sample_sig1),'1-sigma samples')
         if fit_dic['calc_sampMCMC']:print('Saved ',len(par_sample),' random samples')
@@ -1617,15 +1643,15 @@
         TBD
     
     """    
     #Parameter estimates and confidence interval
     #    - define confidence levels to be printed
     #    - use the modified chains that can contain different parameters than those used in the model
     #      the best-fit model will not be modified, but the PDFs, best-fit parameters and associated uncertainties will be derived from the modified chains
-    p_final,fit_dic['med_parfinal'],fit_dic['sig_parfinal_val'],fit_dic['sig_parfinal_err'],fit_dic['HDI_interv'],fit_dic['HDI_interv_txt'],fit_dic['HDI_sig_txt']=MCMC_estimates(merged_chain,fixed_args,fit_dic,verbose=False,print_par=False,calc_quant=fit_dic['calc_quant'])
+    p_final,fit_dic['med_parfinal'],fit_dic['sig_parfinal_val'],fit_dic['sig_parfinal_err'],fit_dic['HDI_interv'],fit_dic['HDI_interv_txt'],fit_dic['HDI_sig_txt']=MCMC_estimates(merged_chain,fixed_args,fit_dic,verbose=False,print_par=False,calc_quant=fit_dic['calc_quant'],verb_shift=fit_dic['verb_shift'])
 
     #Save merged chains for derived parameters and various estimates
     data_save = {'merged_chain':merged_chain,'HDI_interv':fit_dic['HDI_interv'],'sig_parfinal_val':fit_dic['sig_parfinal_val']['1s'],'var_par_list':fixed_args['var_par_list'],'var_par_names':fixed_args['var_par_names'],'med_parfinal':fit_dic['med_parfinal']}
     np.savez(fit_dic['save_dir']+'merged_deriv_chains_walk'+str(fit_dic['nwalkers'])+'_steps'+str(fit_dic['nsteps'])+fit_dic['run_name'],data=data_save,allow_pickle=True)
 
     #Plot correlation diagram for all param    
     if fit_dic['save_MCMC_corner']!='':
@@ -1706,29 +1732,29 @@
   
   
 
 ##################################################################################################
 #%%%% MCMC plots
 ##################################################################################################   
  
-def MCMC_plot_chains(save_mode,save_dir_MCMC,var_par_list,var_par_names,chain,burnt_chains,nsteps,nsteps_pb_walk,nwalkers,nburn,keep_chain,low_thresh_par_val,high_thresh_par_val,exclu_walk_autom,verbose=True):
+def MCMC_plot_chains(save_mode,save_dir_MCMC,var_par_list,var_par_names,chain,burnt_chains,nsteps,nsteps_pb_walk,nwalkers,nburn,keep_chain,low_thresh_par_val,high_thresh_par_val,exclu_walk_autom,verbose=True,verb_shift=''):
     r"""**MCMC post-proc: walker chains plot**
 
     Plots the chains for each fitted parameter over all walkers. 
       
     Args:
         TBD
     
     Returns:
         TBD
     
     """
     if verbose:
-        print(' -----------------------------------')
-        print(' > Plotting chains')
+        print(verb_shift+'-----------------------------------')
+        print(verb_shift+'> Plotting walker chains')
 
     #Font size
     font_size=14
     
     #Taille plot
     margins=[0.15,0.15,0.95,0.8] 
         
@@ -1762,43 +1788,43 @@
         
         #Plot frame  
         plt.title('Chain for param '+partxt)
         y_min = np.min(chain[:,:,ipar])
         y_max = np.max(chain[:,:,ipar])
         dy_range = y_max-y_min
         y_range = [y_min-0.05*dy_range,y_max+0.05*dy_range]    
-        ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)
+        ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)
         custom_axis(plt,position=margins,
                     y_range=y_range,dir_y='out', 
                     ymajor_int=ymajor_int,yminor_int=yminor_int,ymajor_form=ymajor_form,
                     x_title='Steps',y_title=partxt,
                     font_size=font_size,xfont_size=font_size,yfont_size=font_size)
 
         plt.savefig(save_dir_MCMC+'/Chain_'+parname+'.'+save_mode) 
         plt.close()
 
     return None  
 
 
 
-def MCMC_plot_merged_chains(save_mode,save_dir_MCMC,var_par_list,var_par_names,merged_chain,nsteps_final_merged,verbose=True):
+def MCMC_plot_merged_chains(save_mode,save_dir_MCMC,var_par_list,var_par_names,merged_chain,nsteps_final_merged,verbose=True,verb_shift=''):
     r"""**MCMC post-proc: merged chains plot**
 
     Plots the cleaned, merged chains from all workers for each fitted parameter.
       
     Args:
         TBD
     
     Returns:
         TBD
     
     """
     if verbose:
-        print(' -----------------------------------')
-        print(' > Plotting merged chains')
+        print(verb_shift+'-----------------------------------')
+        print(verb_shift+'> Plotting merged chains')
 
     #Font size
     font_size=14
     
     #Taille plot
     margins=[0.15,0.15,0.95,0.8] 
         
@@ -1823,15 +1849,15 @@
         #Plot frame  
         parname_txt=parname.replace('_','-')
         plt.title('Merged chain for param '+parname_txt)
         y_min = np.min(merged_chain[x_tab,ipar])
         y_max = np.max(merged_chain[x_tab,ipar])
         dy_range = y_max-y_min
         y_range = [y_min-0.05*dy_range,y_max+0.05*dy_range]    
-        ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)
+        ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)
         custom_axis(plt,position=margins,
                     # x_range=x_range,
                     y_range=y_range,dir_y='out', 
                     ymajor_int=ymajor_int,yminor_int=yminor_int,ymajor_form=ymajor_form,
                     #		    xmajor_int=1.,xminor_int=0.5,
                     #xmajor_form='%.1f',ymajor_form='%.3f',
                     x_title='Steps',y_title=parname_txt,
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_general/utils.py` & `antaress-1.1.1/src/antaress/ANTARESS_general/utils.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_grids/ANTARESS_coord.py` & `antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_coord.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_grids/ANTARESS_plocc_grid.py` & `antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_occ_grid.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,204 +1,215 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import numpy as np
 from itertools import product as it_product
 from copy import deepcopy
 import lmfit
 from lmfit import Parameters
-from ..ANTARESS_grids.ANTARESS_coord import frameconv_skyorb_to_skystar,frameconv_skystar_to_skyorb,frameconv_skystar_to_star,calc_pl_coord
+from ..ANTARESS_grids.ANTARESS_coord import frameconv_skyorb_to_skystar,frameconv_skystar_to_skyorb,frameconv_skystar_to_star,calc_pl_coord,frameconv_star_to_skystar,calc_zLOS_oblate
 from ..ANTARESS_process.ANTARESS_data_align import align_data
 from ..ANTARESS_analysis.ANTARESS_inst_resp import convol_prof
 from ..ANTARESS_grids.ANTARESS_star_grid import calc_CB_RV,get_LD_coeff,calc_st_sky,calc_Isurf_grid,calc_RVrot
 from ..ANTARESS_analysis.ANTARESS_model_prof import calc_polymodu,polycoeff_def
-from ..ANTARESS_grids.ANTARESS_prof_grid import coadd_loc_line_prof,calc_loc_line_prof,init_st_intr_prof,calc_linevar_coord_grid
-from ..ANTARESS_grids.ANTARESS_spots import is_spot_visible, calc_spotted_tiles, retrieve_spots_prop_from_param, new_new_calc_spotted_region_prop, spot_occ_region_grid
+from ..ANTARESS_grids.ANTARESS_prof_grid import coadd_loc_line_prof,coadd_loc_gauss_prof,calc_loc_line_prof,init_st_intr_prof,calc_linevar_coord_grid, use_C_coadd_loc_gauss_prof
 from ..ANTARESS_general.utils import stop,closest,np_poly,npint,np_interp,np_where1D,datasave_npz,dataload_npz,gen_specdopshift,check_data
 from ..ANTARESS_general.constant_data import Rsun,c_light
 
+
 def calc_plocc_spot_prop(system_param,gen_dic,theo_dic,coord_dic,inst,vis,data_dic,calc_pl_atm=False,spot_dic={}):
     r"""**Planet-occulted / spot properties: workflow**
 
     Calls function to calculate theoretical properties of the regions occulted by all transiting planets and/or spotted. 
 
     Args:
         TBD
     
     Returns:
         TBD
     
     """ 
-    #Samson: same as for mock_dic, the condition (inst in spot_dic) is sufficient, not need to define an additional field spot_dic['use_spots']
+ 
     #Check for spots
-    if (inst in spot_dic) and (vis in spot_dic[inst]):
+    if (spot_dic != {}) and (inst in spot_dic['spots_prop']):
         txt_spot = ' and spotted '
         cond_spot = True
     else:
         txt_spot = ' '
         cond_spot = False
     
     print('   > Calculating properties of planet-occulted'+txt_spot+'regions')    
     if gen_dic['calc_theoPlOcc']:
         print('         Calculating data')
         
         #Theoretical properties of spotted regions
         params = deepcopy(system_param['star'])
         params['use_spots']=cond_spot
-        if params['use_spots']:
-            for spot_param in list(spot_dic['spots_prop'][inst][vis].keys()):
-                params[spot_param]=spot_dic['spots_prop'][inst][vis][spot_param]
-            
-            #Figuring out the number of spots
-            num_spots = 0
-            for par in params:
-                if 'lat__IS'+inst+'_VS'+vis+'_SP' in par:
-                    num_spots +=1
-            params['num_spots']=num_spots
-            params['inst']=inst
-            params['vis']=vis
             
         #Theoretical properties of planet occulted-regions
         #    - calculated for the nominal and broadband planet properties 
         #    - for the nominal properties we retrieve the range of some properties covered by the planet during each exposures
         #    - chromatic transit required if local profiles are in spectral mode  
         params.update({'rv':0.,'cont':1.})
         par_list=['rv','CB_RV','mu','lat','lon','x_st','y_st','SpSstar','xp_abs','r_proj']
         key_chrom = ['achrom']
         if ('spec' in data_dic[inst][vis]['type']) and ('chrom' in data_dic[inst][vis]['system_prop']):key_chrom+=['chrom']
 
         #Calculate properties
-        plocc_prop,spot_prop = sub_calc_plocc_spot_prop(key_chrom,{},par_list,data_dic[inst][vis]['transit_pl'],system_param,theo_dic,data_dic[inst][vis]['system_prop'],params,coord_dic[inst][vis],gen_dic[inst][vis]['idx_in'], system_spot_prop_in = data_dic['DI']['spots_prop'], out_ranges=True)
+        plocc_prop,spot_prop,common_prop = sub_calc_plocc_spot_prop(key_chrom,{},par_list,data_dic[inst][vis]['transit_pl'],system_param,theo_dic,data_dic[inst][vis]['system_prop'],params,coord_dic[inst][vis],gen_dic[inst][vis]['idx_in'], system_spot_prop_in = data_dic['DI']['spots_prop'], out_ranges=True)
         
         #Save spot-occulted region properties
         if cond_spot:
             datasave_npz(gen_dic['save_data_dir']+'Introrig_prop/Spot_Prop_'+inst+'_'+vis,spot_prop)    
 
+            #Save properties combined from planet-occulted and spotted regions
+            datasave_npz(gen_dic['save_data_dir']+'Introrig_prop/Common_Prop_'+inst+'_'+vis,common_prop) 
+
         #Save planet-occulted region properties
         datasave_npz(gen_dic['save_data_dir']+'Introrig_prop/PlOcc_Prop_'+inst+'_'+vis,plocc_prop) 
 
     else:
         check_data({'path':gen_dic['save_data_dir']+'Introrig_prop/PlOcc_Prop_'+inst+'_'+vis})        
 
     return None
 
 
 
 
 
 
-def up_plocc_prop(inst,vis,args,param_in,transit_pl,nexp_fit,ph_fit,coord_pl_fit, transit_spots=[]):
+def up_plocc_prop(inst,vis,args,param_in,transit_pl,ph_grid,coord_grid, transit_spots=[]):
     r"""**Planet-occulted and spotted region properties: update**
 
     Updates properties of the planet-occulted region, planetary orbit, and spotted region for fitted step. 
 
     Args:
         inst (str) : Instrument considered.
         vis (str) : Visit considered. 
         args (dict) : Additional parameters needed to evaluate the fitted function.
         param_in (dict) : Model parameters for the fitted step considered.
         transit_pl (list) : Transiting planets for the instrument and visit considered.
-        nexp_fit : Not called in the function so could be removed.
-        ph_fit (dict) : Dictionary containing the phase of each planet.
-        coord_pl_fit (dict) : Dictionary containing the various coordinates of each planet (e.g., exposure time, exposure x/y/z coordinate).
+        ph_grid (dict) : Dictionary containing the phase of each planet.
+        coord_grid (dict) : Dictionary containing the various coordinates of each planet and spot (e.g., exposure time, exposure x/y/z coordinate).
         transit_spots (list) : Spots present for the instrument and visit considered.
     
     Returns:
         system_param_loc (dict) : System (star+planet+spot) properties.
-        coord_pl (dict) : Updated planet coordinates.
+        coords (dict) : Updated planet and spot coordinates.
         param (dict) : Model parameter names and values.
     
     """ 
     system_param_loc=deepcopy(args['system_param'])
    
     #In case param_in is defined as a Parameters structure, retrieve values and define dictionary
     param={}
     if isinstance(param_in,lmfit.parameter.Parameters):
         for par in param_in:param[par]=param_in[par].value
     else:param=param_in
 
+    #Update stellar parameters if necessary
+    if 'cos_istar' in args['var_par_list']:
+        system_param_loc['star']['cos_istar'] = param['cos_istar']
+        system_param_loc['star']['istar_rad'] = np.arccos(param['cos_istar'])
+
     #Coefficients describing the polynomial variation of spectral line properties as a function of the chosen coordinate
     #    - coefficients can be specific to a given spectral line model
     if (args['mode']=='ana') and (len(args['linevar_par'])>0):
         args['coeff_line'] = {}
         for par_loc in args['linevar_par'][inst][vis]:    
             args['coeff_line'][par_loc] = polycoeff_def(param,args['coeff_ord2name'][inst][vis][par_loc])
 
     #Instrument or visit-specific line continuum
     if ('cont' in args['genpar_instvis']):param['cont'] = param[args['name_prop2input']['cont__IS'+inst+'_VS'+vis]] 
 
     #Recalculate coordinates of occulted regions or use nominal values
     #    - the 'fit_X' conditions are only True if at least one parameter is varying, so that param_fit is True if fit_X is True
-    if args['fit_orbit']:coord_pl = {}
-    else:coord_pl = deepcopy(coord_pl_fit)
+    coords = deepcopy(coord_grid)
     for pl_loc in transit_pl:
 
         #Recalculate planet grid if relevant
         if args['fit_RpRs'] and ('RpRs__pl'+pl_loc in args['var_par_list']):
             args['system_prop']['achrom'][pl_loc][0]=param['RpRs__pl'+pl_loc] 
             args['grid_dic']['Ssub_Sstar_pl'][pl_loc],args['grid_dic']['x_st_sky_grid_pl'][pl_loc],args['grid_dic']['y_st_sky_grid_pl'][pl_loc],r_sub_pl2=occ_region_grid(args['system_prop']['achrom'][pl_loc][0],args['grid_dic']['nsub_Dpl'][pl_loc])  
             args['system_prop']['achrom']['cond_in_RpRs'][pl_loc] = [(r_sub_pl2<args['system_prop']['achrom'][pl_loc][0]**2.)]        
 
         #Recalculate planet coordinates if relevant        
         if args['fit_orbit']:
-            coord_pl[pl_loc]={}
+            coords[pl_loc]={}
             pl_params_loc = system_param_loc[pl_loc]
             
             #Update fitted system properties for current step 
             if ('lambda_rad__pl'+pl_loc in args['genpar_instvis']):lamb_name = 'lambda_rad__pl'+pl_loc+'__IS'+inst+'_VS'+vis 
             else:lamb_name = 'lambda_rad__pl'+pl_loc 
             if (lamb_name in args['var_par_list']):pl_params_loc['lambda_rad'] = param[lamb_name]                     
             if ('inclin_rad__pl'+pl_loc in args['var_par_list']):pl_params_loc['inclin_rad']=param['inclin_rad__pl'+pl_loc]       
             if ('aRs__pl'+pl_loc in args['var_par_list']):pl_params_loc['aRs']=param['aRs__pl'+pl_loc]  
             
             #Calculate coordinates
             #    - start/end phase have been set to None if no oversampling is requested, in which case start/end positions are not calculated
-            if args['grid_dic']['d_oversamp'] is not None:phases = ph_fit[pl_loc]
-            else:phases = ph_fit[pl_loc][1]
+            if args['grid_dic']['d_oversamp'] is not None:phases = ph_grid[pl_loc]
+            else:phases = ph_grid[pl_loc][1]
             x_pos_pl,y_pos_pl,_,_,_,_,_,_,ecl_pl = calc_pl_coord(pl_params_loc['ecc'],pl_params_loc['omega_rad'],pl_params_loc['aRs'],pl_params_loc['inclin_rad'],phases,args['system_prop']['achrom'][pl_loc][0],pl_params_loc['lambda_rad'],system_param_loc['star'])
             if args['grid_dic']['d_oversamp'] is not None:
-                coord_pl[pl_loc]['st_pos'] = np.vstack((x_pos_pl[0],y_pos_pl[0]))
-                coord_pl[pl_loc]['cen_pos'] = np.vstack((x_pos_pl[1],y_pos_pl[1]))
-                coord_pl[pl_loc]['end_pos'] = np.vstack((x_pos_pl[2],y_pos_pl[2]))
-            else:coord_pl[pl_loc]['cen_pos'] = np.vstack((x_pos_pl,y_pos_pl))
-            coord_pl[pl_loc]['ecl'] = ecl_pl
-            
-    #Samson : are those two fields are only needed when spots are present ?         
-    # coord_pl['bjd']= coord_pl_fit['bjd']
-    # coord_pl['t_dur']= coord_pl_fit['t_dur']
-            
+                coords[pl_loc]['st_pos'] = np.vstack((x_pos_pl[0],y_pos_pl[0]))
+                coords[pl_loc]['cen_pos'] = np.vstack((x_pos_pl[1],y_pos_pl[1]))
+                coords[pl_loc]['end_pos'] = np.vstack((x_pos_pl[2],y_pos_pl[2]))
+            else:coords[pl_loc]['cen_pos'] = np.vstack((x_pos_pl,y_pos_pl))
+            coords[pl_loc]['ecl'] = ecl_pl
+
     #Process spots
     if len(transit_spots)>0:
-            
+
         #Set up properties of spotted regions for the spot coordinate retrieval in sub_calc_plocc_spot_prop
         for spot in transit_spots:
             
             #Recalculate spot grid if relevant
-            if args['fit_spot_ang'][spot]:
+            if spot in args['fit_spot_ang']:
                 args['system_spot_prop']['achrom'][spot][0]=param['ang__IS'+inst+'_VS'+vis+'_SP'+spot] * np.pi/180
-                args['grid_dic']['x_st_sky_grid_sp'][spot],args['grid_dic']['x_st_sky_grid_sp'][spot],args['grid_dic']['Ssub_Sstar_sp'][spot] = spot_occ_region_grid(args['system_spot_prop']['achrom'][spot][0],args['grid_dic']['nsub_Dspot'][spot])  
+                _,args['grid_dic']['Ssub_Sstar_sp'][spot],args['grid_dic']['x_st_sky_grid_sp'][spot],args['grid_dic']['y_st_sky_grid_sp'][spot],_ = occ_region_grid(args['system_spot_prop']['achrom'][spot][0],args['grid_dic']['nsub_Dspot'][spot],spot=True)  
+
     
         #Recalculate spot coordinates if relevant        
         if args['fit_spot']:
     
-            #Trigger use of spots in the function computing the DI profile deviation
-            param['use_spots']=True
-            param['inst']=inst
-            param['vis']=vis
-            param['num_spots']=args['num_spots']
-            param['RpoleReq']=system_param_loc['star']['RpoleReq']
-            param['om_eq_spots']=system_param_loc['star']['om_eq_spots']
+            #Update spot crossing time before doing spot parameters' retrieval
+            for par in param:
+                if ('Tcenter' in par) and args['update_crosstime']:param[par] += args['spot_crosstime_supp'][inst][vis]
+
+            #Initialize entries for spot coordinates 
+            for spot in transit_spots:
+                coords[spot] = {}
+                for key in ['Tcenter', 'ang', 'ang_rad', 'lat', 'ctrst']:coords[spot][key] = np.zeros(len(coords['bjd']),dtype=float)*np.nan
+                for key in ['lat_rad_exp','sin_lat_exp','cos_lat_exp','long_rad_exp','sin_long_exp','cos_long_exp','x_sky_exp','y_sky_exp','z_sky_exp']:coords[spot][key] = np.zeros([3,len(coords['bjd'])],dtype=float)*np.nan
+                coords[spot]['is_visible'] = np.zeros([3,len(coords['bjd'])],dtype=bool)
+                
+            #Retrieving the spot coordinates for all the times that we have
+            for ifit_tstamp, fit_tstamp in enumerate(coords['bjd']):                
+                spots_prop = retrieve_spots_prop_from_param(system_param_loc['star'],param,inst,vis,fit_tstamp,exp_dur=coords['t_dur'][ifit_tstamp])
+                for spot in transit_spots:
+
+                    for key in ['Tcenter', 'ang', 'ang_rad', 'lat', 'ctrst']:
+                        coords[spot][key][ifit_tstamp] = spots_prop[spot][key]
 
-    return system_param_loc,coord_pl,param
+                    for key in ['lat_rad_exp','sin_lat_exp','cos_lat_exp','long_rad_exp','sin_long_exp','cos_long_exp','x_sky_exp','y_sky_exp','z_sky_exp']:
+                        coords[spot][key][:, ifit_tstamp] = [spots_prop[spot][key+'_start'],spots_prop[spot][key+'_center'],spots_prop[spot][key+'_end']]
 
+                    coords[spot]['is_visible'][:, ifit_tstamp] = [spots_prop[spot]['is_start_visible'],spots_prop[spot]['is_center_visible'],spots_prop[spot]['is_end_visible']]
 
+        #Trigger use of spots in the function computing the DI profile deviation
+        param['use_spots']=True
 
+    #Useful if spots are present but the spot parameters are fixed
+    else:param['use_spots']=False
 
+    return system_param_loc,coords,param
 
 
-def sub_calc_plocc_spot_prop(key_chrom,args,par_list_gen,transit_pl,system_param,theo_dic,system_prop_in,param,coord_pl_in,iexp_list,system_spot_prop_in = {} , out_ranges=False,Ftot_star=False):
+
+
+def sub_calc_plocc_spot_prop(key_chrom,args,par_list_gen,transit_pl,system_param,theo_dic,system_prop_in,param,coord_in,iexp_list,system_spot_prop_in={},out_ranges=False,Ftot_star=False):
     r"""**Planet-occulted and spot properties: exposure**
 
     Calculates average theoretical properties of the stellar surface occulted by all transiting planets and/or spotted during an exposure
     
      - we normalize all quantities by the flux emitted by the occulted regions
      - all positions are in units of :math:`R_\star` 
     
@@ -207,23 +218,24 @@
         args (dict) : parameters used to generate analytical profiles.
         par_list_gen (list) : parameters whose value we want to calculate over each planet-occulted/spotted region.
         transit_pl (list) : list of transiting planets in the exposures considered.
         system_param (dict) : system (star + planet + spot) properties.
         theo_dic (dict) : parameters used to generate and describe the stellar grid and planet/spot-occulted regions grid.
         system_prop_in (dict) : planet limb-darkening properties.
         param (dict) : fitted or fixed star/planet/spot properties.
-        coord_pl_in (dict) : dictionary containing the various coordinates of each planet (e.g., exposure time, exposure phase, exposure x/y/z coordinate)
+        coord_in (dict) : dictionary containing the various coordinates of each planet and spot (e.g., exposure time, exposure phase, exposure x/y/z coordinate)
         iexp_list (list) : exposures to process.
         system_spot_prop_in (dict) : optional, spot limb-darkening properties.
         out_ranges (bool) : optional, whether or not to calculate the range of values the parameters of interest (par_list_gen) will take. Turned off by default.
         Ftot_star (bool) : optional, whether or not to calculate the normalized stellar flux after accounting for the spot/planet occultations. Turned off by default.
     
     Returns:
         surf_prop_dic_pl (dict) : average value of all the properties of interest over all the planet-occulted regions, in each exposure and chromatic mode considered.
-        surf_prop_dic_spot (dict) : average value of all the properties of interest over all the spot-occulted regions, in each exposure and chromatic mode considered.
+        surf_prop_dic_spot (dict) : average value of all the properties of interest over all the spotted regions, in each exposure and chromatic mode considered.
+        surf_prop_dic_common (dict) : average value of all the properties of interest considering the contributions from both the planet-occulted and spotted regions, in each exposure and chromatic mode considered.
 
     """ 
     system_prop = deepcopy(system_prop_in)
     system_spot_prop = deepcopy(system_spot_prop_in)
     par_list_in = deepcopy(par_list_gen)
     n_exp = len(iexp_list)
     
@@ -263,21 +275,22 @@
                 if (args['mode']=='ana'):stop('Analytical model not suited for wide spectral bands') 
                 if (theo_dic['precision']=='high'):stop('High precision not possible for wide spectral bands') 
                 key_chrom=['achrom','chrom']
 
     #Calculation of achromatic and/or chromatic values
     surf_prop_dic_pl = {}
     surf_prop_dic_spot = {}
+    surf_prop_dic_common = {}
     for subkey_chrom in key_chrom:
         surf_prop_dic_pl[subkey_chrom] = {}        
-        if cond_spot:surf_prop_dic_spot[subkey_chrom] = {}
+        surf_prop_dic_spot[subkey_chrom] = {}
     if 'line_prof' in par_list_in:
         for subkey_chrom in key_chrom:
             surf_prop_dic_pl[subkey_chrom]['line_prof']=np.zeros([args['ncen_bins'],n_exp],dtype=float)
-            if cond_spot:surf_prop_dic_spot[subkey_chrom]['line_prof']=np.zeros([args['ncen_bins'],n_exp],dtype=float)
+            surf_prop_dic_spot[subkey_chrom]['line_prof']=np.zeros([args['ncen_bins'],n_exp],dtype=float)
 
     #Properties to be calculated
     #    - properties in 'param' have the nominal values from system properties only if the property was not defined in the model property dictionary from settings 
     par_star = deepcopy(param)
     par_list = ['Ftot']
     for par_loc in par_list_in:
         if par_loc=='rv':
@@ -290,15 +303,17 @@
     cb_band_dic = {}
     if cond_spot:cb_band_spot_dic = {}
     for subkey_chrom in key_chrom:
 
         #Disk-integrated stellar flux
         if Ftot_star:
             surf_prop_dic_pl[subkey_chrom]['Ftot_star']=np.zeros([system_prop[subkey_chrom]['nw'],n_exp])*np.nan 
-            if cond_spot:surf_prop_dic_spot[subkey_chrom]['Ftot_star']=np.zeros([system_prop[subkey_chrom]['nw'],n_exp])*np.nan 
+            if cond_spot:
+                surf_prop_dic_spot[subkey_chrom]['Ftot_star']=np.zeros([system_prop[subkey_chrom]['nw'],n_exp])*np.nan 
+                surf_prop_dic_common[subkey_chrom]['Ftot_star']=np.ones([system_prop[subkey_chrom]['nw'],n_exp])
 
         #Convective blueshift
         #    - physically, it makes sense for us to define different CB coefficients for a spot since spotted regions are regions of magnetic suppression and would have different CB.
         #However, we make the simplifying assumption that the c1_CB, c2_CB, and c3_CB coefficient are the same for the spotted region as for the quiet star regions, with c0_CB being
         #the only coefficient that varies, and which is calculated with the same condition as before. 
         #Even though our assumption is not correct, we think that the RV shift induced by the difference in CB for the spot can be captured in the RV parameter used to describe the
         #line profiles with which the spotted region is tiled.
@@ -322,108 +337,106 @@
     #List of parameters whose range we're interested in
     range_par_list=[]
     if (len(theo_dic['d_oversamp'])>0) and out_ranges:range_par_list = list(np.intersect1d(['mu','lat','lon','x_st','y_st','xp_abs','r_proj'],par_list))
  
     #Initializing spot variables
     #    - must be initialized in anyy case since they will be called later, even if spots are not activated.
     cond_spots_all = np.zeros([n_exp,1], dtype=bool)
-    spots_prop_all_exp = {}
     list_spot_names = []
 
     #Initializing list that will contain the oversampled step for spots, if they are oversampled.
-    dx_exp_in_sp={}
-    dy_exp_in_sp={}
-    dz_exp_in_sp={}
+    dcoord_exp_in_sp = {'x':{},'y':{},'z':{}}
 
     #Initialize a list which will tell us the oversampling rate for each exposure
     n_osamp_exp_all_sp = np.repeat(1,n_exp)
 
     #Define spot properties
     if cond_spot:
         
         #High precision is required for spots
         if (theo_dic['precision']!='high'):stop('High precision required for spots')
         
         #Figure out the number of spots
-        n_spots = param['num_spots']
+        n_spots = 0
+        for key in coord_in.keys():
+            if 'spot' in key:
+                n_spots+=1
+                list_spot_names.append(key)
         
         #Initialize the dictionary that will contain spot presence
         cond_spots_all = np.zeros([n_exp,n_spots], dtype=bool)
 
         #Looping over all exposures
         for isub_exp, iexp in enumerate(iexp_list):
-            
-            #Get the time in BJD of the exposure we're considering.
-            exp_time = coord_pl_in['bjd'][iexp]
-
-            #Extract spot properties for the exposure we're considering.
-            spots_prop = retrieve_spots_prop_from_param(par_star, param, param['inst'], param['vis'], exp_time, exp_dur=coord_pl_in['t_dur'][iexp])
 
             #Check if at least one spot is visible.
-            #To do so, we need a more precise estimate of the spot location.
-            spot_within_grid_all=np.zeros(len(spots_prop.keys()), dtype=bool)
+            #    - to do so, we need a more precise estimate of the spot location.
+            spot_within_grid_all=np.zeros(n_spots, dtype=bool)
 
             #Go through the spots and see if they are *roughly* visible.
-            for spot_index, spot in enumerate(spots_prop):
-                if spots_prop[spot]['is_center_visible']:
+            for spot_index, spot in enumerate(list_spot_names):
+
+                #See if spot is visible at the center of the exposure.
+                if (np.sum(coord_in[spot]['is_visible'][:, iexp])>=1):
+
+                    #Need to make a dictionary of spot coordinates which will be used in calc_spotted_tiles.
+                    mini_spot_dic = {}
+                    mini_spot_dic['x_sky_exp_start'],mini_spot_dic['x_sky_exp_center'],mini_spot_dic['x_sky_exp_end']=coord_in[spot]['x_sky_exp'][:, iexp]
+                    mini_spot_dic['y_sky_exp_start'],mini_spot_dic['y_sky_exp_center'],mini_spot_dic['y_sky_exp_end']=coord_in[spot]['y_sky_exp'][:, iexp]
+                    mini_spot_dic['ang_rad']=coord_in[spot]['ang_rad'][iexp]
+                    mini_spot_dic['cos_long_exp_start'],mini_spot_dic['cos_long_exp_center'],mini_spot_dic['cos_long_exp_end']=coord_in[spot]['cos_long_exp'][:, iexp]
+                    mini_spot_dic['sin_long_exp_start'],mini_spot_dic['sin_long_exp_center'],mini_spot_dic['sin_long_exp_end']=coord_in[spot]['sin_long_exp'][:, iexp]
+                    mini_spot_dic['cos_lat_exp_start'],mini_spot_dic['cos_lat_exp_center'],mini_spot_dic['cos_lat_exp_end']=coord_in[spot]['cos_lat_exp'][:, iexp]
+                    mini_spot_dic['sin_lat_exp_start'],mini_spot_dic['sin_lat_exp_center'],mini_spot_dic['sin_lat_exp_end']=coord_in[spot]['sin_lat_exp'][:, iexp]
+    
                     #See if spot is *precisely* visible.
-                    spot_within_grid, _ = calc_spotted_tiles(spots_prop[spot],
-                                    theo_dic['x_st_sky'], theo_dic['y_st_sky'], theo_dic['z_st_sky'], theo_dic,
-                                    par_star, True)
+                    spot_within_grid, _ = calc_spotted_tiles(mini_spot_dic,theo_dic['x_st_sky'], theo_dic['y_st_sky'], theo_dic['z_st_sky'], theo_dic,par_star, True)
                     if spot_within_grid:
                         spot_within_grid_all[spot_index]=True
 
                     #Check if oversampling is turned on for this spot and force all spots to have same oversampling rate
                     if len(theo_dic['n_oversamp_spot'])>0 and theo_dic['n_oversamp_spot'][spot]>0:
-                        dx_exp_in_sp[spot] = spots_prop[spot]['x_sky_exp_end'] - spots_prop[spot]['x_sky_exp_start']
-                        dy_exp_in_sp[spot] = spots_prop[spot]['y_sky_exp_end'] - spots_prop[spot]['y_sky_exp_start']
-                        dz_exp_in_sp[spot] = spots_prop[spot]['z_sky_exp_end'] - spots_prop[spot]['z_sky_exp_start']
+                        for key in ['x','y','z']:dcoord_exp_in_sp[key][spot] = coord_in[spot][key+'_sky_exp'][2,iexp] - coord_in[spot][key+'_sky_exp'][0,iexp]
                         n_osamp_exp_all_sp[isub_exp] = np.maximum(n_osamp_exp_all_sp[isub_exp], theo_dic['n_oversamp_spot'][spot])
 
                     #Spot-dependent properties - initialize dictionaries
                     for subkey_chrom in key_chrom:
                         surf_prop_dic_spot[subkey_chrom][spot]={}
                         for par_loc in par_list:
                             surf_prop_dic_spot[subkey_chrom][spot][par_loc]=np.zeros([system_spot_prop[subkey_chrom]['nw'],n_exp])*np.nan        
                         for par_loc in range_par_list:surf_prop_dic_spot[subkey_chrom][spot][par_loc+'_range']=np.zeros([system_spot_prop[subkey_chrom]['nw'],n_exp,2])*np.nan
 
-            # Update cond_spots_all
+            #Update cond_spots_all
             cond_spots_all[isub_exp]=spot_within_grid_all
 
-            # Put an entry in the dictionary storing spot properties over all exposures
-            spots_prop_all_exp[iexp] = spots_prop
-     
-        #Storing the 'names' of the spots for later use.
-        list_spot_names = list(spots_prop.keys())
-
     #If spots are not present, need to initialize the spot LD dictionary entry for later purposes
     else:
         for subkey_chrom in key_chrom:system_spot_prop[subkey_chrom]={}
 
     #Occulted planet zones properties
     n_osamp_exp_all = np.repeat(1,n_exp)
     lambda_rad_pl = {}
     dx_exp_in={}
     dy_exp_in={}
     cond_transit_all = np.zeros([n_exp,len(transit_pl)],dtype=bool)
     for ipl,pl_loc in enumerate(transit_pl):
         
         #Check for planet transit
-        if np.sum(np.abs(coord_pl_in[pl_loc]['ecl'][iexp_list])!=1.)>0:
-            cond_transit_all[:,ipl]|=(np.abs(coord_pl_in[pl_loc]['ecl'][iexp_list])!=1.)   
+        if np.sum(np.abs(coord_in[pl_loc]['ecl'][iexp_list])!=1.)>0:
+            cond_transit_all[:,ipl]|=(np.abs(coord_in[pl_loc]['ecl'][iexp_list])!=1.)   
 
             #Obliquities for multiple planets
             #    - for now only defined for a single planet if fitted  
             #    - the nominal lambda has been overwritten in 'system_param[pl_loc]' if fitted
             lambda_rad_pl[pl_loc]=system_param[pl_loc]['lambda_rad']
             
             #Exposure distance (Rstar) 
             if len(theo_dic['d_oversamp'])>0:
-                dx_exp_in[pl_loc]=abs(coord_pl_in[pl_loc]['end_pos'][0,iexp_list]-coord_pl_in[pl_loc]['st_pos'][0,iexp_list])
-                dy_exp_in[pl_loc]=abs(coord_pl_in[pl_loc]['end_pos'][1,iexp_list]-coord_pl_in[pl_loc]['st_pos'][1,iexp_list])
+                dx_exp_in[pl_loc]=abs(coord_in[pl_loc]['end_pos'][0,iexp_list]-coord_in[pl_loc]['st_pos'][0,iexp_list])
+                dy_exp_in[pl_loc]=abs(coord_in[pl_loc]['end_pos'][1,iexp_list]-coord_in[pl_loc]['st_pos'][1,iexp_list])
              
                 #Number of oversampling points for current exposure  
                 #    - for each exposure we take the maximum oversampling all planets considered 
                 if pl_loc in theo_dic['d_oversamp']:
                     d_exp_in = np.sqrt(dx_exp_in[pl_loc]**2 + dy_exp_in[pl_loc]**2)
                     n_osamp_exp_all=np.maximum(n_osamp_exp_all,npint(np.round(d_exp_in/theo_dic['d_oversamp'][pl_loc]))+1)
                     
@@ -440,24 +453,22 @@
     cond_transit = np.sum(cond_transit_all,axis=1)>0
     cond_spotted = np.sum(cond_spots_all, axis=1)>0
     cond_iexp_proc = cond_spotted|cond_transit
 
     #Enforcing a common oversampling factor to the spots and planets
     n_osamp_exp_all_total = np.maximum(n_osamp_exp_all, n_osamp_exp_all_sp)
 
-
     #Processing each exposure 
-    for i_in,(iexp,n_osamp_exp) in enumerate(zip(iexp_list,n_osamp_exp_all_total)):
+    for isub_exp,(iexp,n_osamp_exp) in enumerate(zip(iexp_list,n_osamp_exp_all_total)):
    
         #Planets in exposure
-        transit_pl_exp = np.array(transit_pl)[cond_transit_all[i_in]]
+        transit_pl_exp = np.array(transit_pl)[cond_transit_all[isub_exp]]
 
         #Spots in exposure 
-        if cond_spot and spots_prop_all_exp != {}:
-            spots_in_exp = np.array(list_spot_names)[cond_spots_all[i_in]]
+        if cond_spot:spots_in_exp = np.array(list_spot_names)[cond_spots_all[isub_exp]]
         else:spots_in_exp = {}
    
         #Initialize averaged and range values
         Focc_star_pl={}
         if cond_spot:Focc_star_sp={}
         sum_prop_dic={}
         coord_reg_dic={}
@@ -493,63 +504,53 @@
                 coord_reg_dic[subkey_chrom][spot]={}
                 range_dic[subkey_chrom][spot]={}
                 for par_loc in par_list:    
                     sum_prop_dic[subkey_chrom][spot][par_loc]=np.zeros(system_spot_prop[subkey_chrom]['nw'],dtype=float)
                     coord_reg_dic[subkey_chrom][spot][par_loc]=np.zeros(system_spot_prop[subkey_chrom]['nw'],dtype=float)
                     if par_loc in range_par_list:range_dic[subkey_chrom][spot][par_loc+'_range']=np.tile([1e100,-1e100],[system_spot_prop[subkey_chrom]['nw'],1])
                 sum_prop_dic[subkey_chrom][spot]['nocc']=0. 
-                if ('line_prof' in par_list_in):
-                    if (theo_dic['precision'] in ['low','medium']):
-                        coord_reg_dic[subkey_chrom][spot]['rv_broad']=np.zeros(system_spot_prop[subkey_chrom]['nw'],dtype=float)
-                    elif (theo_dic['precision']=='high'):
-                        sum_prop_dic[subkey_chrom][spot]['line_prof'] = np.zeros(args['ncen_bins'],dtype=float)
+                if ('line_prof' in par_list_in):sum_prop_dic[subkey_chrom][spot]['line_prof'] = np.zeros(args['ncen_bins'],dtype=float)
                                         
             #Line profile can be calculated over each stellar cell only in achromatic / closest-achromatic mode 
             if ('line_prof' in par_list_in):line_occ_HP[subkey_chrom] = np.repeat(theo_dic['precision'],system_prop[subkey_chrom]['nw'])
             else:line_occ_HP[subkey_chrom] = np.repeat('',system_prop[subkey_chrom]['nw'])  
             
-        #Theoretical properties from regions occulted by each planet or spotted, at exposure center       
-        if cond_iexp_proc[i_in]:        
+        #Theoretical properties from spotted regions or regions occulted by planets, at exposure center       
+        if cond_iexp_proc[isub_exp]:        
             x_oversamp_pl={}
             y_oversamp_pl={}
             
             #Planet oversampled positions
             for pl_loc in transit_pl_exp:
             
                 #No oversampling
                 if n_osamp_exp==1:
-                    x_oversamp_pl[pl_loc] = [coord_pl_in[pl_loc]['cen_pos'][0,iexp]]
-                    y_oversamp_pl[pl_loc] = [coord_pl_in[pl_loc]['cen_pos'][1,iexp]]
+                    x_oversamp_pl[pl_loc] = [coord_in[pl_loc]['cen_pos'][0,iexp]]
+                    y_oversamp_pl[pl_loc] = [coord_in[pl_loc]['cen_pos'][1,iexp]]
     
                 #Theoretical properties from regions occulted by each planet, averaged over full exposure duration  
                 #    - only if oversampling is effective for this exposure
                 else:
-                    x_oversamp_pl[pl_loc] = coord_pl_in[pl_loc]['st_pos'][0][iexp]+np.arange(n_osamp_exp)*dx_exp_in[pl_loc][i_in]/(n_osamp_exp-1.)  
-                    y_oversamp_pl[pl_loc] = coord_pl_in[pl_loc]['st_pos'][1][iexp]+np.arange(n_osamp_exp)*dy_exp_in[pl_loc][i_in]/(n_osamp_exp-1.) 
+                    x_oversamp_pl[pl_loc] = coord_in[pl_loc]['st_pos'][0][iexp]+np.arange(n_osamp_exp)*dx_exp_in[pl_loc][isub_exp]/(n_osamp_exp-1.)  
+                    y_oversamp_pl[pl_loc] = coord_in[pl_loc]['st_pos'][1][iexp]+np.arange(n_osamp_exp)*dy_exp_in[pl_loc][isub_exp]/(n_osamp_exp-1.) 
                     
             #Spot oversampled positions initialization
             if cond_spot:
-                x_oversamp_sp={}
-                y_oversamp_sp={}
-                z_oversamp_sp={}
+                coord_oversamp = {'x':{},'y':{},'z':{}}
     
                 #Spot oversampled positions
                 for spot in spots_in_exp:
                     
                     #No oversampling
                     if n_osamp_exp==1:
-                        x_oversamp_sp[spot] = [spots_prop_all_exp[iexp][spot]['x_sky_exp_center']]
-                        y_oversamp_sp[spot] = [spots_prop_all_exp[iexp][spot]['y_sky_exp_center']]
-                        z_oversamp_sp[spot] = [spots_prop_all_exp[iexp][spot]['z_sky_exp_center']]
-                    
+                        for key in ['x','y','z']:coord_oversamp[key][spot] = [coord_in[spot][key+'_sky_exp'][1,iexp]]
+                   
                     #If we want to oversample
                     else:
-                        x_oversamp_sp[spot] = spots_prop_all_exp[iexp][spot]['x_sky_exp_start'] + np.arange(n_osamp_exp)*dx_exp_in_sp[spot]/(n_osamp_exp-1.)  
-                        y_oversamp_sp[spot] = spots_prop_all_exp[iexp][spot]['y_sky_exp_start'] + np.arange(n_osamp_exp)*dy_exp_in_sp[spot]/(n_osamp_exp-1.) 
-                        z_oversamp_sp[spot] = spots_prop_all_exp[iexp][spot]['z_sky_exp_start'] + np.arange(n_osamp_exp)*dz_exp_in_sp[spot]/(n_osamp_exp-1.) 
+                        for key in ['x','y','z']:coord_in[spot][key+'_sky_exp'][0,iexp] + np.arange(n_osamp_exp)*dcoord_exp_in_sp[key][spot]/(n_osamp_exp-1.)                
 
             #Variables to keep track of how many oversampled positions in this exposure were occulting the star
             n_osamp_exp_eff_pl = 0
             n_osamp_exp_eff_sp = 0
 
             #Loop on oversampled exposure positions 
             #    - after x_oversamp_pl has been defined for all planets
@@ -560,22 +561,23 @@
 
                 #Need to define a reduced version of the spot dictionary in this oversampled position. This is required
                 #if we want to account for presence of spots in planet-occulted regions.
                 spots_are_visible = False
                 reduced_spot_prop_oversamp={}
                 for spot in spots_in_exp:
                     reduced_spot_prop_oversamp[spot]={}
-                    reduced_spot_prop_oversamp[spot]['ctrst']=spots_prop_all_exp[iexp][spot]['ctrst']
-                    reduced_spot_prop_oversamp[spot]['ang_rad']=spots_prop_all_exp[iexp][spot]['ang_rad']
-                    temp_long = np.arcsin(x_oversamp_sp[spot][iosamp] / np.cos(spots_prop_all_exp[iexp][spot]['lat_rad_exp_center']))
-                    reduced_spot_prop_oversamp[spot]['cos_lat_exp_center'] = np.cos(spots_prop_all_exp[iexp][spot]['lat_rad_exp_center'])
+                    reduced_spot_prop_oversamp[spot]['ctrst']=coord_in[spot]['ctrst'][iexp]
+                    reduced_spot_prop_oversamp[spot]['ang_rad']=coord_in[spot]['ang_rad'][iexp]
+                    temp_long = np.arcsin(coord_oversamp['x'][spot][iosamp] / np.cos(coord_in[spot]['lat_rad_exp'][1,iexp]))
+                    reduced_spot_prop_oversamp[spot]['cos_lat_exp_center'] = np.cos(coord_in[spot]['lat_rad_exp'][1,iexp])
                     reduced_spot_prop_oversamp[spot]['cos_long_exp_center'] = np.cos(temp_long)
-                    reduced_spot_prop_oversamp[spot]['sin_lat_exp_center'] = np.sin(spots_prop_all_exp[iexp][spot]['lat_rad_exp_center'])
+                    reduced_spot_prop_oversamp[spot]['sin_lat_exp_center'] = np.sin(coord_in[spot]['lat_rad_exp'][1,iexp])
                     reduced_spot_prop_oversamp[spot]['sin_long_exp_center'] = np.sin(temp_long)
-                    spots_are_visible |= is_spot_visible(par_star['istar_rad'], temp_long, spots_prop_all_exp[iexp][spot]['lat_rad_exp_center'], reduced_spot_prop_oversamp[spot]['ang_rad'], par_star['f_GD'], par_star['RpoleReq'])
+                    spots_are_visible |= is_spot_visible(par_star['istar_rad'], temp_long, coord_in[spot]['lat_rad_exp'][1,iexp], reduced_spot_prop_oversamp[spot]['ang_rad'], par_star['f_GD'], (1-par_star['f_GD']))
+
 
                 #------------------------------------------------------------
                 #Planet-occulted regions
                 
                 #Dictionary telling us which planets have been processed in which chromatic mode and band.
                 pl_proc={subkey_chrom:{iband:[] for iband in range(system_prop[subkey_chrom]['nw'])} for subkey_chrom in key_chrom}
                 cond_occ_pl = False
@@ -587,148 +589,146 @@
                     #Largest possible square grid enclosing the planet shifted to current planet position     
                     x_st_sky_max = x_st_sky_pos+theo_dic['x_st_sky_grid_pl'][pl_loc]
                     y_st_sky_max = y_st_sky_pos+theo_dic['y_st_sky_grid_pl'][pl_loc]
 
                     #Calculating properties
                     for subkey_chrom in key_chrom:
                         for iband in range(system_prop[subkey_chrom]['nw']):
-                            Focc_star_pl[subkey_chrom][iband],cond_occ_pl = calc_occ_region_prop(line_occ_HP[subkey_chrom][iband],cond_occ_pl,iband,args,system_prop[subkey_chrom],iosamp,pl_loc,pl_proc[subkey_chrom][iband],theo_dic['Ssub_Sstar_pl'][pl_loc],x_st_sky_max,y_st_sky_max,system_prop[subkey_chrom]['cond_in_RpRs'][pl_loc][iband],par_list,par_star,theo_dic['Istar_norm_'+subkey_chrom],\
+                            Focc_star_pl[subkey_chrom][iband],cond_occ_pl = calc_occ_region_prop(line_occ_HP[subkey_chrom][iband],cond_occ_pl,iband,args,system_prop[subkey_chrom],system_spot_prop[subkey_chrom],iosamp,pl_loc,pl_proc[subkey_chrom][iband],theo_dic['Ssub_Sstar_pl'][pl_loc],x_st_sky_max,y_st_sky_max,system_prop[subkey_chrom]['cond_in_RpRs'][pl_loc][iband],par_list,theo_dic['Istar_norm_'+subkey_chrom],\
                                                                                   x_oversamp_pl,y_oversamp_pl,lambda_rad_pl,par_star,sum_prop_dic[subkey_chrom][pl_loc],coord_reg_dic[subkey_chrom][pl_loc],range_dic[subkey_chrom][pl_loc],range_par_list,Focc_star_pl[subkey_chrom][iband],cb_band_dic[subkey_chrom][iband],theo_dic, spot_occ=spots_are_visible, reduced_spot_prop=reduced_spot_prop_oversamp)
             
                             #Cumulate line profile from planet-occulted cells
                             #    - in high-precision mode there is a single subkey_chrom and achromatic band, but several planets may have been processed
                             if ('line_prof' in par_list_in):
-                                if (theo_dic['precision']=='low'):surf_prop_dic_pl[subkey_chrom][pl_loc]['rv_broad'][iband,i_in] = np.max([coord_reg_dic[subkey_chrom][pl_loc]['rv_broad'][iband],surf_prop_dic_pl[subkey_chrom][pl_loc]['rv_broad'][iband,i_in]])
-                                elif (theo_dic['precision']=='high'):surf_prop_dic_pl[subkey_chrom]['line_prof'][:,i_in]+=sum_prop_dic[subkey_chrom][pl_loc]['line_prof']
+                                if (theo_dic['precision']=='low'):surf_prop_dic_pl[subkey_chrom][pl_loc]['rv_broad'][iband,isub_exp] = np.max([coord_reg_dic[subkey_chrom][pl_loc]['rv_broad'][iband],surf_prop_dic_pl[subkey_chrom][pl_loc]['rv_broad'][iband,isub_exp]])
+                                elif (theo_dic['precision']=='high'):surf_prop_dic_pl[subkey_chrom]['line_prof'][:,isub_exp]+=sum_prop_dic[subkey_chrom][pl_loc]['line_prof']
                     
                 #Star was effectively occulted at oversampled position
                 if cond_occ_pl:
                     n_osamp_exp_eff_pl+=1
                     
                     #Calculate line profile from planet-occulted region 
                     #    - profile is scaled to the total flux from current occulted region, stored in coord_reg_dic_pl['Ftot']
                     if ('line_prof' in par_list_in) and (theo_dic['precision']=='medium'):
                         idx_w = {'achrom':range(system_prop['achrom']['nw'])}
                         if ('chrom' in key_chrom):idx_w['chrom'] = range(system_prop['chrom']['nw'])
-                        surf_prop_dic_pl[key_chrom[-1]]['line_prof'][:,i_in]+=plocc_prof(args,transit_pl_exp,coord_reg_dic,idx_w,system_prop,key_chrom,par_star,theo_dic)
+                        surf_prop_dic_pl[key_chrom[-1]]['line_prof'][:,isub_exp]+=plocc_prof(args,transit_pl_exp,coord_reg_dic,idx_w,system_prop,key_chrom,par_star,theo_dic)
 
                 #------------------------------------------------------------
                 #Spotted regions
                 if cond_spot:
                     cond_occ_sp = False
                     
-                    #Retrieving the properties of the region occulted by each spot
+                    #Need to make a new dictionary that contains the spot properties for this oversampled exposure
+                    spot_prop_oversamp = {}
+
+                    #Building the spot dictionary - we need to extract this information for all the spots to find their overlap
                     for spot in spots_in_exp:
                         
                         #Make a rough estimate of the spot-occulted grid - has a different resolution than the stellar grid - is in inclined star rest frame
-                        x_st_sky_max_sp = x_oversamp_sp[spot][iosamp] + theo_dic['x_st_sky_grid_sp'][spot]
-                        y_st_sky_max_sp = y_oversamp_sp[spot][iosamp] + theo_dic['y_st_sky_grid_sp'][spot]
-    
-                        #Need to make a new dictionary that contains the spot properties for this oversampled exposure
-                        spot_prop_oversamp = {}
-                        
-                        #Setting the properties in spot_prop_oversamp to those of the oversampled exposure
-                        spot_prop_oversamp['ctrst'] = spots_prop_all_exp[iexp][spot]['ctrst']
-                        spot_prop_oversamp['x_sky_grid'] = x_st_sky_max_sp
-                        spot_prop_oversamp['y_sky_grid'] = y_st_sky_max_sp
-                        spot_prop_oversamp['x_sky_exp_center'] = x_oversamp_sp[spot][iosamp]
-                        spot_prop_oversamp['y_sky_exp_center'] = y_oversamp_sp[spot][iosamp]
-                        spot_prop_oversamp['z_sky_exp_center'] = z_oversamp_sp[spot][iosamp]
-                        spot_prop_oversamp['lat_rad_exp_center'] = spots_prop_all_exp[iexp][spot]['lat_rad_exp_center']
-                        spot_prop_oversamp['ang_rad'] = spots_prop_all_exp[iexp][spot]['ang_rad']
-                        spot_prop_oversamp['long_rad_exp_center'] = np.arcsin(x_oversamp_sp[spot][iosamp] / np.cos(spots_prop_all_exp[iexp][spot]['lat_rad_exp_center']))
-                        spot_prop_oversamp['cos_long_exp_center'] = np.cos(spot_prop_oversamp['long_rad_exp_center'])
-                        spot_prop_oversamp['sin_long_exp_center'] = np.sin(spot_prop_oversamp['long_rad_exp_center'])
-                        spot_prop_oversamp['cos_lat_exp_center'] = np.cos(spot_prop_oversamp['lat_rad_exp_center'])
-                        spot_prop_oversamp['sin_lat_exp_center'] = np.sin(spot_prop_oversamp['lat_rad_exp_center'])
-                        spot_prop_oversamp['is_visible'] = is_spot_visible(par_star['istar_rad'], spot_prop_oversamp['long_rad_exp_center'], spot_prop_oversamp['lat_rad_exp_center'], spot_prop_oversamp['ang_rad'], par_star['f_GD'], par_star['RpoleReq'])
+                        x_st_sky_max_sp = coord_oversamp['x'][spot][iosamp] + theo_dic['x_st_sky_grid_sp'][spot]
+                        y_st_sky_max_sp = coord_oversamp['y'][spot][iosamp] + theo_dic['y_st_sky_grid_sp'][spot]
+                        spot_prop_oversamp[spot] = {}
+                        spot_prop_oversamp[spot]['ctrst'] = coord_in[spot]['ctrst'][iexp]
+                        spot_prop_oversamp[spot]['x_sky_grid'] = x_st_sky_max_sp
+                        spot_prop_oversamp[spot]['y_sky_grid'] = y_st_sky_max_sp
+                        spot_prop_oversamp[spot]['x_sky_exp_center'] = coord_oversamp['x'][spot][iosamp]
+                        spot_prop_oversamp[spot]['y_sky_exp_center'] = coord_oversamp['y'][spot][iosamp]
+                        spot_prop_oversamp[spot]['z_sky_exp_center'] = coord_oversamp['z'][spot][iosamp]
+                        spot_prop_oversamp[spot]['lat_rad_exp_center'] = coord_in[spot]['lat_rad_exp'][1,iexp]
+                        spot_prop_oversamp[spot]['ang_rad'] = coord_in[spot]['ang_rad'][iexp]
+                        spot_prop_oversamp[spot]['long_rad_exp_center'] = np.arcsin(coord_oversamp['x'][spot][iosamp] / np.cos(coord_in[spot]['lat_rad_exp'][1,iexp]))
+                        spot_prop_oversamp[spot]['cos_long_exp_center'] = np.cos(spot_prop_oversamp[spot]['long_rad_exp_center'])
+                        spot_prop_oversamp[spot]['sin_long_exp_center'] = np.sin(spot_prop_oversamp[spot]['long_rad_exp_center'])
+                        spot_prop_oversamp[spot]['cos_lat_exp_center'] = np.cos(spot_prop_oversamp[spot]['lat_rad_exp_center'])
+                        spot_prop_oversamp[spot]['sin_lat_exp_center'] = np.sin(spot_prop_oversamp[spot]['lat_rad_exp_center'])
+                        spot_prop_oversamp[spot]['is_visible'] = is_spot_visible(par_star['istar_rad'], spot_prop_oversamp[spot]['long_rad_exp_center'], spot_prop_oversamp[spot]['lat_rad_exp_center'], spot_prop_oversamp[spot]['ang_rad'], par_star['f_GD'], (1-par_star['f_GD']))
     
+                    #Dictionary telling us which spots remain to be processed in which chromatic mode and band.
+                    sp_proc={subkey_chrom:{iband:[] for iband in range(system_spot_prop[subkey_chrom]['nw'])} for subkey_chrom in key_chrom}
+
+                    #Retrieving the properties of the region occulted by each spot
+                    for spot in spots_in_exp:
+   
                         #Going over the chromatic modes
                         for subkey_chrom in key_chrom:
                             
                             #Going over the bands in each chromatic mode
                             for iband in range(system_spot_prop[subkey_chrom]['nw']):
-                                
-                                Focc_star_sp[subkey_chrom][iband], cond_occ_sp = new_new_calc_spotted_region_prop(line_occ_HP[subkey_chrom][iband], cond_occ_sp, spot_prop_oversamp, iband, system_spot_prop[subkey_chrom], par_star, theo_dic['Ssub_Sstar_sp'][spot], 
-                                                                theo_dic['Ssub_Sstar'], theo_dic['Istar_norm_'+subkey_chrom], sum_prop_dic[subkey_chrom][spot], coord_reg_dic[subkey_chrom][spot], 
-                                                                range_dic[subkey_chrom][spot], Focc_star_sp[subkey_chrom][iband], par_list, range_par_list, args, cb_band_dic[subkey_chrom][iband], 
+                                Focc_star_sp[subkey_chrom][iband], cond_occ_sp = calc_spotted_region_prop(line_occ_HP[subkey_chrom][iband], cond_occ_sp, spot_prop_oversamp, iband, system_prop[subkey_chrom], 
+                                                                system_spot_prop[subkey_chrom], par_star, sp_proc[subkey_chrom][iband],spot,theo_dic['Ssub_Sstar_sp'][spot], 
+                                                                theo_dic['Ssub_Sstar'], theo_dic['Istar_norm_'+subkey_chrom], sum_prop_dic[subkey_chrom][spot], coord_reg_dic[subkey_chrom][spot],
+                                                                range_dic[subkey_chrom][spot], Focc_star_sp[subkey_chrom][iband], par_list, range_par_list, args, cb_band_spot_dic[subkey_chrom][iband], 
                                                                 pl_loc_x = x_oversamp_pl, pl_loc_y = y_oversamp_pl, oversamp_idx = iosamp, RpRs = system_prop[subkey_chrom], plocc = (n_osamp_exp_eff_pl>=1))
     
                                 #Cumulate line profile from spot-occulted cells
                                 #    - in high-precision mode there is a single subkey_chrom and achromatic band, but several spots may have been processed
                                 if ('line_prof' in par_list_in):
-                                    if (theo_dic['precision']=='low'):surf_prop_dic_spot[subkey_chrom][spot]['rv_broad'][iband,i_in] = np.max([coord_reg_dic[subkey_chrom][spot]['rv_broad'][iband],surf_prop_dic_spot[subkey_chrom][spot]['rv_broad'][iband,i_in]])
-                                    elif (theo_dic['precision']=='high'):surf_prop_dic_spot[subkey_chrom]['line_prof'][:,i_in]+=sum_prop_dic[subkey_chrom][spot]['line_prof']
-                                
+                                    surf_prop_dic_spot[subkey_chrom]['line_prof'][:,isub_exp]+=sum_prop_dic[subkey_chrom][spot]['line_prof']
+
                                 emit_coord_reg_dic = deepcopy(coord_reg_dic)
-                                emit_coord_reg_dic[subkey_chrom][spot]['Ftot'][iband] *= (1-spot_prop_oversamp['ctrst'])
-    
+                                emit_coord_reg_dic[subkey_chrom][spot]['Ftot'][iband] *= (1-spot_prop_oversamp[spot]['ctrst'])
+
                                 emit_surf_prop_dic_spot = deepcopy(surf_prop_dic_spot)
-                                emit_surf_prop_dic_spot[subkey_chrom][spot]['Ftot'][iband] *= (1-spot_prop_oversamp['ctrst'])
-    
+                                emit_surf_prop_dic_spot[subkey_chrom][spot]['Ftot'][iband] *= (1-spot_prop_oversamp[spot]['ctrst'])
+
                     #Star was effectively occulted at oversampled position
                     if cond_occ_sp:
                         n_osamp_exp_eff_sp+=1
-                        
-                        #Calculate line profile from spot-occulted region 
-                        #    - profile is scaled to the total flux from current occulted region, stored in coord_reg_dic_pl['Ftot']
-                        if ('line_prof' in par_list_in) and (theo_dic['precision']=='medium'):
-                            idx_w = {'achrom':range(system_spot_prop['achrom']['nw'])}
-                            if ('chrom' in key_chrom):idx_w['chrom'] = range(system_spot_prop['chrom']['nw'])
-                            
-                            #Line profile of region occulted by the spot
-                            surf_prop_dic_spot[key_chrom[-1]]['line_prof'][:,i_in]+=plocc_prof(args,spots_in_exp,coord_reg_dic,idx_w,system_spot_prop,key_chrom,par_star,theo_dic)
-                            
-                            #Line profile emitted by the spot
-                            surf_prop_dic_spot[key_chrom[-1]]['line_prof'][:,i_in]-=plocc_prof(args,spots_in_exp,emit_coord_reg_dic,idx_w,system_spot_prop,key_chrom,par_star,theo_dic)
                     
             #------------------------------------------------------------
 
             #Averaged values behind all occulted regions during exposure
             #    - with the oversampling, positions at the center of exposure will weigh more in the sum than those at start and end of exposure, like in reality
             #    - parameters are retrieved in both oversampled/not-oversampled case after they are updated within the sum_prop_dic dictionary 
             #    - undefined values remain set to nan, and are otherwise normalized by the flux from the planet-occulted region
             #    - we use a single Itot as condition that the planet occulted the star
-            calc_mean_occ_region_prop(transit_pl_exp,surf_prop_dic_pl,n_osamp_exp_eff_pl,sum_prop_dic,key_chrom,par_list,i_in,out_ranges,range_par_list,range_dic)     
+            calc_mean_occ_region_prop(transit_pl_exp,surf_prop_dic_pl,n_osamp_exp_eff_pl,sum_prop_dic,key_chrom,par_list,isub_exp,out_ranges,range_par_list,range_dic)     
             if cond_spot:                
-                calc_mean_occ_region_prop(spots_in_exp,surf_prop_dic_spot,n_osamp_exp_eff_sp,sum_prop_dic,key_chrom,par_list,i_in,out_ranges,range_par_list,range_dic)                            
+                calc_mean_occ_region_prop(spots_in_exp,surf_prop_dic_spot,n_osamp_exp_eff_sp,sum_prop_dic,key_chrom,par_list,isub_exp,out_ranges,range_par_list,range_dic)                            
                             
             #Normalized stellar flux after occultation by all planets and by all spots
             #    - the intensity from each cell is calculated in the same way as that of the full pre-calculated stellar grid
             if Ftot_star:
                 for subkey_chrom in key_chrom:
-                    surf_prop_dic_pl[subkey_chrom]['Ftot_star'][:,i_in] = 1.
-                    
+                    surf_prop_dic_pl[subkey_chrom]['Ftot_star'][:,isub_exp] = 1.
+                    surf_prop_dic_common[subkey_chrom]['Ftot_star'][:,isub_exp] = 1.
+                    if cond_spot:surf_prop_dic_spot[subkey_chrom]['Ftot_star'][:,isub_exp] = 1.
+
                     #Planets
                     if n_osamp_exp_eff_pl>0:
-                        surf_prop_dic_pl[subkey_chrom]['Ftot_star'][:,i_in] -= Focc_star_pl[subkey_chrom]/(n_osamp_exp_eff_pl*theo_dic['Ftot_star_'+subkey_chrom])
+                        surf_prop_dic_pl[subkey_chrom]['Ftot_star'][:,isub_exp] -= Focc_star_pl[subkey_chrom]/(n_osamp_exp_eff_pl*theo_dic['Ftot_star_'+subkey_chrom])
+                        surf_prop_dic_common[subkey_chrom]['Ftot_star'][:,isub_exp] -= Focc_star_pl[subkey_chrom]/(n_osamp_exp_eff_pl*theo_dic['Ftot_star_'+subkey_chrom])
                     
                     #Spots
                     if cond_spot and (n_osamp_exp_eff_sp>0):
-                        surf_prop_dic_spot[subkey_chrom]['Ftot_star'][:,i_in] -= Focc_star_sp[subkey_chrom]/(n_osamp_exp_eff_sp*theo_dic['Ftot_star_'+subkey_chrom])
+                        surf_prop_dic_spot[subkey_chrom]['Ftot_star'][:,isub_exp] -= (Focc_star_sp[subkey_chrom])/(n_osamp_exp_eff_sp*theo_dic['Ftot_star_'+subkey_chrom])
+                        surf_prop_dic_common[subkey_chrom]['Ftot_star'][:,isub_exp] -= (Focc_star_sp[subkey_chrom])/(n_osamp_exp_eff_sp*theo_dic['Ftot_star_'+subkey_chrom])
+
 
             #Local line profiles from current exposure
             if ('line_prof' in par_list_in):
 
                 #Planet-occulted line profile         
                 if (n_osamp_exp_eff_pl>0):
-                    calc_mean_occ_region_line(theo_dic['precision'],system_prop,i_in,key_chrom,n_osamp_exp_eff_pl,Focc_star_pl,surf_prop_dic_pl,transit_pl_exp,args,par_star,theo_dic)
+                    calc_mean_occ_region_line(theo_dic['precision'],system_prop,isub_exp,key_chrom,n_osamp_exp_eff_pl,Focc_star_pl,surf_prop_dic_pl,transit_pl_exp,args,par_star,theo_dic)
             
                 #Spotted line profile 
                 if cond_spot and (n_osamp_exp_eff_sp > 0):
-                    calc_mean_occ_region_line(theo_dic['precision'],system_prop,key_chrom,n_osamp_exp_eff_sp,Focc_star_sp,surf_prop_dic_spot,spots_in_exp,args,par_star,theo_dic)
+                    calc_mean_occ_region_line(theo_dic['precision'],system_prop,isub_exp,key_chrom,n_osamp_exp_eff_sp,Focc_star_sp,surf_prop_dic_spot,spots_in_exp,args,par_star,theo_dic)
 
     ### end of exposure            
  
     #Output properties in chromatic mode if calculated in closest-achromatic mode
     if ('line_prof' in par_list_in) and switch_chrom:
         surf_prop_dic_pl = {'chrom':surf_prop_dic_pl['achrom']}
         surf_prop_dic_spot = {'chrom':surf_prop_dic_spot['achrom']}
+        surf_prop_dic_common = {'chrom':surf_prop_dic_common['achrom']}
 
-    return surf_prop_dic_pl, surf_prop_dic_spot
+    return surf_prop_dic_pl, surf_prop_dic_spot , surf_prop_dic_common
 
 
 
 def calc_mean_occ_region_prop(occulters,surf_prop_dic,n_osamp_exp_eff,sum_prop_dic,key_chrom,par_list,i_in,out_ranges,range_par_list,range_dic):
     r"""**Planet-occulted properties: average properties**
 
     Calculates the properties from the cumulated stellar surface regions occulted during an exposure.
@@ -793,43 +793,68 @@
         if (theo_dic['precision']=='high') and args['conv2intr']:
             Focc_star_achrom=Focc_star[key_chrom[-1]]/n_osamp_exp_eff
             surf_prop_dic[key_chrom[-1]]['line_prof'][:,i_in] /=Focc_star_achrom   
 
     return None
 
 
-
-
-def calc_occ_region_prop(line_occ_HP_band,cond_occ,iband,args,system_prop,idx,pl_loc,pl_proc_band,Ssub_Sstar,x_st_sky_max,y_st_sky_max,cond_in_RpRs,par_list,param,Istar_norm_band,x_pos_pl,y_pos_pl,lambda_rad_pl,par_star,sum_prop_dic_pl,\
-                         coord_reg_dic_pl,range_reg_pl,range_par_list,Focc_star_band,cb_band,theo_dic,spot_occ = False, reduced_spot_prop={}):
+def calc_occ_region_prop(line_occ_HP_band,cond_occ,iband,args,system_prop,system_spot_prop,idx,pl_loc,pl_proc_band,Ssub_Sstar,x_st_sky_max,y_st_sky_max,cond_in_RpRs,par_list,Istar_norm_band,x_pos_pl,y_pos_pl,lambda_rad_pl,par_star,sum_prop_dic_pl,\
+                         coord_reg_dic_pl,range_reg,range_par_list,Focc_star_band,cb_band,theo_dic,spot_occ = False,reduced_spot_prop={}):
     r"""**Planet-occulted properties: region**
 
     Calculates the average and summed properties from a planet-occulted stellar surface region during an exposure.
 
     Args:
-        TBD
+        line_occ_HP_band (str) : The precision with which to process the exposure.
+        cond_occ (bool) : Boolean telling us whether there is an occultation by at least one planet in the oversampled exposure considered.
+        iband (int) : Index of the band of interest.
+        system_prop (dict) : Planet limb-darkening properties.
+        system_spot_prop (dict) : Spot limb-darkening properties.
+        idx (int) : Index of the oversampled exposure considered.
+        pl_loc (str) : Planet considered.
+        pl_proc_band (dict) : Dictionary telling us which planets have been processed in the chromatic mode and band considered.
+        Ssub_Sstar (float) : Surface ratio of a planet-occulted region grid cell to a stellar grid cell.
+        x_st_sky_max (array) : x coordinates of the maximum square planet-occulted region grid.
+        x_st_sky_max (array) : y coordinates of the maximum square planet-occulted region grid.
+        cond_in_RpRs (array) : Booleans telling us which cells in the maximum square planet-occulted region grid are within the circular planet-occulted region.
+        par_list (list) : List of parameters of interest, whose value in sum_prop_dic_pl will be updated.
+        Istar_norm_band (float) : total intensity of the star in the band considered.
+        x_pos_pl (float) : x coordinate of the planet in the sky-projected orbital frame.
+        y_pos_pl (float) : y coordinate of the planet in the sky-projected orbital frame.
+        lambda_rad_pl (float) : Spin-orbit angle of the planet.
+        par_star (dict) : Variable stellar parameters.
+        sum_prop_dic_pl (dict) : dictionary containing the value of all parameters of interest (par_list), summed over the planet-occulted region in the exposure considered, and for the band of interest.
+        coord_reg_dic_pl (dict) : dictionary containing the value of all parameters of interest (par_list), averaged over the planet-occulted region in the exposure considered, and for the band of interest.
+        range_reg (dict) : dictionary containing the range of average values the parameters of interest (range_par_list) can take during this exposure.
+        range_par_list (list) : list of parameters of interest, whose range of values, stored in range_reg_dic_spot, will be updated.
+        Focc_star_band (float) : total flux occulted by the spot in the exposure and band considered. 
+        cb_band (list) : Polynomial coefficients used to compute thr RV component of the planet-occulted region due to convective blueshift.
+        theo_dic (dict) : parameters used to generate and describe the stellar grid and planet-occulted regions grid.
+        spot_occ (bool) : Optional, whether spotted regions are present in the oversampled exposure considered. Default is False.
+        reduced_spot_prop (dict) : Optional, spot properties used to account for the possible presence of spotted cells in the planet-occulted region. Default is an empty dictionary.
+        fit_Ftot_star (bool) : Optional, whether to include the continuum in the calculation of Focc_star_band.
     
     Returns:
-        TBD
+        Focc_star_band (float) : the input Focc_star_band updated with the flux occulted by the planet considered.
+        cond_occ (bool) : updated version of the input cond_occ. Tells us whether or not the planet occulted the exposure considered.
+
     
     """ 
+
+    parameter_list = deepcopy(par_list)
+    range_parameter_list = deepcopy(range_par_list)
         
     #Reduce maximum square planet grid to size of planet in current band
     coord_grid = {}
     coord_grid['x_st_sky']=x_st_sky_max[cond_in_RpRs] 
     coord_grid['y_st_sky']=y_st_sky_max[cond_in_RpRs]   
 
     #Identifying occulted stellar cells in the sky-projected and star star rest frame
     n_pl_occ = calc_st_sky(coord_grid,par_star)
 
-    #Making an array that will keep track of which cells are occulted by the spots
-    if spot_occ:
-        for spots in list(reduced_spot_prop.keys()):
-            coord_grid[spots+'_flag_map']=np.zeros(len(coord_grid['x_st_sky']), dtype=bool)
-    
     #Star is effectively occulted
     #    - when the expositions are oversampled, some oversampled positions may put the planet beyond the stellar disk, with no points behind the star
     if n_pl_occ>0:
         cond_occ = True
         
         #Removing current planet cells already processed for previous occultations
         if len(pl_proc_band)>0:
@@ -848,69 +873,84 @@
       
         #Store planet as processed in current band
         pl_proc_band+=[pl_loc]     
 
         #--------------------------------
         #Account for spot occultation in planet-occulted region
         if spot_occ:
+
+            #Making a reference spot to extract the contrast
+            ref_spot = list(reduced_spot_prop.keys())[0]
             
             #Identify the cells in the planet-occulted region that are spotted
             for spot in list(reduced_spot_prop.keys()):
                 
-                #Samson: the new_z_sky_grid below is only for a spherical star; however, I think it's already been calculated in calc_st_sky() just above for any kind  of star, so you can just retrieve it.
-                
+                #Making individual spot maps
+                coord_grid[spot+'_flag_map']=np.zeros(len(coord_grid['x_st_sky']), dtype=bool)
+
                 #Retrieve coordinates of the planet-occulted region in the inclined star frame
                 new_x_sky_grid = coord_grid['x_st_sky']
                 new_y_sky_grid = coord_grid['y_st_sky']
-                new_z_sky_grid = np.sqrt(1 - new_x_sky_grid**2 - new_y_sky_grid**2)
+                new_z_sky_grid = coord_grid['z_st_sky']
+
 
                 #Move coordinates to the (non-inclined) star frame and then the spot reference frame
                 x_st_grid, y_st_grid, z_st_grid = frameconv_skystar_to_star(new_x_sky_grid, new_y_sky_grid, new_z_sky_grid, par_star['istar_rad'])
                 x_spot_grid = x_st_grid*reduced_spot_prop[spot]['cos_long_exp_center'] - z_st_grid*reduced_spot_prop[spot]['sin_long_exp_center']
                 y_spot_grid = y_st_grid*reduced_spot_prop[spot]['cos_lat_exp_center'] - (z_st_grid*reduced_spot_prop[spot]['cos_long_exp_center'] + x_st_grid*reduced_spot_prop[spot]['sin_long_exp_center']) * reduced_spot_prop[spot]['sin_lat_exp_center']
                 cond_in_sp = (x_spot_grid**2. + y_spot_grid**2. <= reduced_spot_prop[spot]['ang_rad']**2)
 
                 #Updating the flag map
                 coord_grid[spot+'_flag_map'] |= cond_in_sp
 
+            coord_grid['gen_spot_flag_map'] = coord_grid[ref_spot+'_flag_map']
+
+            #Accounting for possible overlap
+            if len(list(reduced_spot_prop.keys()))>1:
+                for spot in list(reduced_spot_prop.keys()):
+                    coord_grid['gen_spot_flag_map'] |= (coord_grid[spot+'_flag_map'] & ~coord_grid['gen_spot_flag_map'])
+
+
         #--------------------------------
 
         #Local flux grid over current planet-occulted region, in current band
         coord_grid['nsub_star'] = n_pl_occ
         _,_,mu_grid_star,Fsurf_grid_star,Ftot_star,_ = calc_Isurf_grid([iband],coord_grid['nsub_star'],system_prop,coord_grid,par_star,Ssub_Sstar,Istar_norm = Istar_norm_band,region = 'pl',Ssub_Sstar_ref = theo_dic['Ssub_Sstar'])
         coord_grid['mu'] = mu_grid_star[:,0]
 
         #Accounting for the spots' emission
         if spot_occ:
-            for spot in list(reduced_spot_prop.keys()):
-                Fsurf_grid_star[:, iband] = np.where(coord_grid[spot+'_flag_map'] == True, Fsurf_grid_star[:, iband] - (Fsurf_grid_star[:, iband] * (1-reduced_spot_prop[spot]['ctrst'])), Fsurf_grid_star[:, iband])
+            
+            #Retrieve the flux-grid with the LD coefficients of the spot
+            _,_,_,Fsurf_spot_emit_grid,_,_ = calc_Isurf_grid([iband],coord_grid['nsub_star'],system_spot_prop,coord_grid,par_star,Ssub_Sstar,Istar_norm = Istar_norm_band,region = 'pl',Ssub_Sstar_ref = theo_dic['Ssub_Sstar'])
+            Fsurf_grid_star[:, iband] = np.where(coord_grid['gen_spot_flag_map'] == True, Fsurf_grid_star[:, iband] - (Fsurf_spot_emit_grid[:, iband] * reduced_spot_prop[ref_spot]['ctrst']), Fsurf_grid_star[:, iband])
             Ftot_star = np.sum(Fsurf_grid_star, axis=0)
 
         #Scale continuum level
-        Fsurf_grid_star*=param['cont']
-        Ftot_star*=param['cont']
+        Fsurf_grid_star*=par_star['cont']
+        Ftot_star*=par_star['cont']
        
         #Flux and number of cells occulted from all planets, cumulated over oversampled positions
         Focc_star_band+= Ftot_star[0]   
         sum_prop_dic_pl['nocc']+=coord_grid['nsub_star']
         
         #--------------------------------
 
         #Co-adding properties from current region to the cumulated values over oversampled planet positions 
-        sum_region_prop(line_occ_HP_band,iband,args,system_prop,par_list,Fsurf_grid_star[:,0],coord_grid,Ssub_Sstar,cb_band,range_par_list,range_reg_pl,sum_prop_dic_pl,coord_reg_dic_pl,par_star,lambda_rad_pl[pl_loc],theo_dic,param)
+        sum_region_prop(line_occ_HP_band,iband,args,parameter_list,Fsurf_grid_star[:,0],None,coord_grid,Ssub_Sstar,cb_band,range_parameter_list,range_reg,sum_prop_dic_pl,coord_reg_dic_pl,par_star,lambda_rad_pl[pl_loc],None)
 
     return Focc_star_band,cond_occ
 
 
 
 
-def sum_region_prop(line_occ_HP_band,iband,args,system_prop,par_list,Fsurf_grid_band,coord_grid,Ssub_Sstar,cb_band,range_par_list,range_reg_pl,sum_prop_dic_pl,coord_reg_dic_pl,par_star,lambda_rad_pl_loc,theo_dic,param):
-    r"""**Planet-occulted properties: calculations**
+def sum_region_prop(line_occ_HP_band,iband,args,par_list,Fsurf_grid_band,Fsurf_grid_emit_band,coord_grid,Ssub_Sstar,cb_band,range_par_list,range_reg,sum_prop_dic,coord_reg_dic,par_star,lambda_rad_pl_loc,spot_contrast):
+    r"""**Planet-occulted or spotted region properties: calculations**
 
-    Calculates the average and summed properties from a planet-occulted stellar surface region during an exposure.
+    Calculates the average and summed properties from a local (planet-occulted or spotted) stellar surface region during an exposure.
     
     The flux emitted by a local element writes
     
     .. math::  
        dF[\nu] =  I[\nu](\cos{\theta})  dA \, \vec{N}(dA).\vec{N}(\mathrm{LOS})
     
     with :math:`dF[\nu]` emitted in the direction :math:`\vec{N}(\mathrm{LOS})` of the LOS, :math:`dA = R_\mathrm{\star}^2 \sin{\theta} d\theta d\phi` the spherical surface element 
@@ -990,18 +1030,32 @@
        ie that we 'add' successively the `N(xy)` times a given surface element flux was occulted. 
        The normalization factor corresponds to :math:`F_\mathrm{tot}^\mathrm{oversamp}`.
        To ensure that this approximation is good, `N(xy)` must be high enough, ie :math:`t_\mathrm{exp}^\mathrm{oversamp}` and :math:`d_\mathrm{exp}^\mathrm{oversamp}` small enough 
      
      - note that :math:`S_\mathrm{sub}/S_\mathrm{\star}` is normalized by :math:`R_\mathrm{\star}^2`, since :math:`d_\mathrm{grid}` is defined from :math:`R_\mathrm{p}/R_\mathrm{\star}`
 
     Args:
-        TBD
-    
+        line_occ_HP_band (str) : The precision with which to process the exposure.
+        iband (int) : Index of the band of interest.
+        args (dict) : Parameters used to generate the intrinsic profiles.
+        par_list (list) : List of parameters of interest, whose value in sum_prop_dic will be updated.
+        Fsurf_grid_band (array) : Stellar flux grid over local region in the band of interest.
+        coord_grid (dict) : Dictionary of coordinates for the local region.
+        Ssub_Sstar (float) : Surface ratio of a local region grid cell to a stellar grid cell.
+        cb_band (list) : Polynomial coefficients used to compute thr RV component of the planet-occulted region due to convective blueshift.
+        range_par_list (list) : List of parameters of interest, whose range of values, stored in range_reg_dic, will be updated.
+        range_reg (dict) : Dictionary containing the range of average values the parameters of interest (range_par_list) can take during this exposure.
+        sum_prop_dic (dict) : Dictionary containing the value of all parameters of interest (par_list), summed over the local region in the exposure considered, and for the band of interest.
+        coord_reg_dic (dict) : Dictionary containing the value of all parameters of interest (par_list), averaged over the local region in the exposure considered, and for the band of interest.
+        par_star (dict) : Fixed/variable stellar parameters.
+        lambda_rad_pl_loc (float) : Spin-orbit angle of the planet.
+        spot_contrast (float) : Contrast level of the spot considered.
+
     Returns:
-        TBD
+        None
     
     """     
     #Distance from projected orbital normal in the sky plane, in absolute value
     if ('xp_abs' in par_list) or (('coord_line' in args) and (args['coord_line']=='xp_abs')):coord_grid['xp_abs'] = frameconv_skystar_to_skyorb(lambda_rad_pl_loc,coord_grid['x_st_sky'],coord_grid['y_st_sky'],coord_grid['z_st_sky'])[0]  
 
     #Sky-projected distance from star center
     if ('r_proj' in par_list) or (('coord_line' in args) and (args['coord_line']=='r_proj')):coord_grid['r_proj'] = np.sqrt(coord_grid['r2_st_sky'])                   
@@ -1010,16 +1064,16 @@
     for par_loc in par_list:
         
         #Occultation ratio
         #    - ratio = Sp/S* = sum(x,sp(x))/(pi*Rstar^2) = sum(x,dp(x)^2)/(pi*Rstar^2) = sum(x,d_surfloc(x)*Rstar^2)/(pi*Rstar^2) = sum(x,d_surfloc(x))/pi
         #      since we use a square grid, sum(x,d_surfloc(x)) = nx*d_surfloc
         #      this quantity is not limb-darkening weighted
         if par_loc=='SpSstar':
-            sum_prop_dic_pl[par_loc][iband]+=Ssub_Sstar*coord_grid['nsub_star']
-            coord_reg_dic_pl[par_loc][iband] = Ssub_Sstar*coord_grid['nsub_star']
+            sum_prop_dic[par_loc][iband]+=Ssub_Sstar*coord_grid['nsub_star']
+            coord_reg_dic[par_loc][iband] = Ssub_Sstar*coord_grid['nsub_star']
          
         else:
         
             #Flux level from region occulted by the planet alone
             #    - set to 1 since it is weighted by flux afterward
             if par_loc=='Ftot':coord_grid[par_loc] = 1.                    
 
@@ -1040,66 +1094,95 @@
                          
             #Disk-integrated-corrected convective blueshift polynomial (km/s)
             elif par_loc=='CB_RV':coord_grid[par_loc] = np_poly(cb_band)(coord_grid['mu'])          
     
             #Full RV (km/s)
             #    - accounting for an additional constant offset to model jitter or global shifts, and for visit-specific offset to model shifts specific to a given transition
             elif par_loc=='rv':
-                coord_grid[par_loc] = deepcopy(coord_grid['Rot_RV']) + param['rv']
+                coord_grid[par_loc] = deepcopy(coord_grid['Rot_RV']) + par_star['rv']
                 if 'CB_RV' in par_list:coord_grid[par_loc]+=coord_grid['CB_RV']
                 if 'rv_line' in par_list:coord_grid[par_loc]+=coord_grid['rv_line']
                 
             #------------------------------------------------
     
             #Sum property over occulted region, weighted by stellar flux
-            #    - we use flux rather than intensity, because local flux level depend on the planet grid resolution
-            #    - total RVs from planet-occulted region is set last in par_list to calculate all rv contributions first:
+            #    - we use flux rather than intensity, because local flux level depend on the local region grid resolution
+            #    - total RVs from local region is set last in par_list to calculate all rv contributions first:
             # + rotational contribution is always included
             # + disk-integrated-corrected convective blueshift polynomial (in km/s)   
             coord_grid[par_loc+'_sum'] = np.sum(coord_grid[par_loc]*Fsurf_grid_band)
             if par_loc=='xp_abs':coord_grid[par_loc+'_sum'] = np.abs(coord_grid[par_loc+'_sum'])
               
             #Cumulate property over successively occulted regions
-            sum_prop_dic_pl[par_loc][iband]+=coord_grid[par_loc+'_sum'] 
+            sum_prop_dic[par_loc][iband]+=coord_grid[par_loc+'_sum'] 
 
             #Total flux from current occulted region
-            if par_loc=='Ftot':coord_reg_dic_pl['Ftot'][iband] = coord_grid['Ftot_sum']
+            if par_loc=='Ftot':coord_reg_dic['Ftot'][iband] = coord_grid['Ftot_sum']
 
             #Calculate average property over current occulted region  
             #    - <X> = sum(cell, xcell*fcell)/sum(cell,fcell)           
-            else:coord_reg_dic_pl[par_loc][iband] = coord_grid[par_loc+'_sum']/coord_grid['Ftot_sum'] 
+            else:coord_reg_dic[par_loc][iband] = coord_grid[par_loc+'_sum']/coord_grid['Ftot_sum'] 
 
             #Range of values covered during the exposures (normalized)
             #    - for spatial-related coordinates
             if par_loc in range_par_list:
-                range_reg_pl[par_loc+'_range'][iband][0]=np.min([range_reg_pl[par_loc+'_range'][iband][0],coord_reg_dic_pl[par_loc][iband]])
-                range_reg_pl[par_loc+'_range'][iband][1]=np.max([range_reg_pl[par_loc+'_range'][iband][1],coord_reg_dic_pl[par_loc][iband]])
+                range_reg[par_loc+'_range'][iband][0]=np.min([range_reg[par_loc+'_range'][iband][0],coord_reg_dic[par_loc][iband]])
+                range_reg[par_loc+'_range'][iband][1]=np.max([range_reg[par_loc+'_range'][iband][1],coord_reg_dic[par_loc][iband]])
      
     #------------------------------------------------    
     #Calculate line profile from average of cell profiles over current region
     #    - this high precision mode is only possible for achromatic or closest-achromatic mode 
     if line_occ_HP_band=='high':    
         
         #Attribute intrinsic profile to each cell 
-        init_st_intr_prof(args,coord_grid,param)
+        init_st_intr_prof(args,coord_grid,par_star)
+
+        #Whether to use the over-simplified grid building function or not
+        use_OS_grid=False
+        use_C_OS_grid=False
+        if 'OS_grid' in args and args['OS_grid']:use_OS_grid=True
+        if 'C_OS_grid' in args and args['C_OS_grid']:
+            use_OS_grid=False
+            use_C_OS_grid=True
 
         #Calculate individual local line profiles from all region cells
         #    - analytical intrinsic profiles are fully calculated 
         #      theoretical and measured intrinsic profiles have been pre-defined and are just shifted to their position
         #    - in both cases a scaling is then applied to convert them into local profiles
-        line_prof_grid=coadd_loc_line_prof(coord_grid['rv'],range(coord_grid['nsub_star']),Fsurf_grid_band,args['flux_intr_grid'],coord_grid['mu'],param,args)          
-      
+        if not args['fit']:line_prof_grid=coadd_loc_line_prof(coord_grid['rv'],range(coord_grid['nsub_star']),Fsurf_grid_band,args['flux_intr_grid'],coord_grid['mu'],par_star,args)          
+        else:
+            if use_OS_grid:
+                fit_Fsurf_grid_band = np.tile(Fsurf_grid_band, (args['ncen_bins'], 1)).T
+                line_prof_grid=coadd_loc_gauss_prof(coord_grid['rv'],fit_Fsurf_grid_band,args)
+            elif use_C_OS_grid:
+                line_prof_grid = use_C_coadd_loc_gauss_prof(coord_grid['rv'],Fsurf_grid_band,args)
+            else:line_prof_grid=coadd_loc_line_prof(coord_grid['rv'],range(coord_grid['nsub_star']),Fsurf_grid_band,args['flux_intr_grid'],coord_grid['mu'],par_star,args)
+
         #Coadd line profiles over planet-occulted region
-        sum_prop_dic_pl['line_prof'] = np.sum(line_prof_grid,axis=0) 
+        sum_prop_dic['line_prof'] = np.sum(line_prof_grid,axis=0) 
+
+        #Calculate profile emitted by a spot
+        if spot_contrast is not None:
+            if not args['fit']:emit_line_prof_grid = coadd_loc_line_prof(coord_grid['rv'],range(coord_grid['nsub_star']),(1-spot_contrast)*Fsurf_grid_emit_band,args['flux_intr_grid'],coord_grid['mu'],par_star,args)          
+            else:
+                if use_OS_grid:
+                    fit_Fsurf_grid_emit_band = np.tile((1-spot_contrast)*Fsurf_grid_emit_band, (args['ncen_bins'], 1)).T
+                    emit_line_prof_grid = coadd_loc_gauss_prof(coord_grid['rv'],fit_Fsurf_grid_emit_band,args)
+                elif use_C_OS_grid:
+                    emit_line_prof_grid = use_C_coadd_loc_gauss_prof(coord_grid['rv'],(1-spot_contrast)*Fsurf_grid_emit_band,args)
+                else:emit_line_prof_grid = coadd_loc_line_prof(coord_grid['rv'],range(coord_grid['nsub_star']),(1-spot_contrast)*Fsurf_grid_emit_band,args['flux_intr_grid'],coord_grid['mu'],par_star,args)        
+
+            #Remove line profiles over spotted region
+            sum_prop_dic['line_prof'] -= np.sum(emit_line_prof_grid,axis=0)
   
     #Define rotational broadening of planet-occulted region
     elif line_occ_HP_band in ['low','medium']:
-        drv_min = coord_reg_dic_pl['rv'][iband]-np.min(coord_grid['rv'])
-        drv_max = np.max(coord_grid['rv'])-coord_reg_dic_pl['rv'][iband] 
-        coord_reg_dic_pl['rv_broad'][iband] = 0.5*(drv_min+drv_max)       
+        drv_min = coord_reg_dic['rv'][iband]-np.min(coord_grid['rv'])
+        drv_max = np.max(coord_grid['rv'])-coord_reg_dic['rv'][iband] 
+        coord_reg_dic['rv_broad'][iband] = 0.5*(drv_min+drv_max)       
 
     return None
 
 
 
 
 
@@ -1224,57 +1307,69 @@
             #Co-add contribution from current planet
             line_prof+=data_av_pl['flux'][0]
             
     return line_prof
 
 
 
+def occ_region_grid(RregRs, nsub_Dreg , spot = False):
+    r"""**Local region grid** 
 
-
-
-
-
-def occ_region_grid(RpRs,nsub_Dpl):
-    r"""**Planet grid**
-
-    Defines grid discretizing planet disk, in the 'inclined' star frame
+    Defines a square x/y/z grid enclosing a local region of the stellar surface in the 'inclined' star frame, with:
       
      - X axis is parallel to the star equator
      - Y axis is the projected spin axis
-     - Z axis is the LOS
+     - Z axis is along the LOS
 
     Args:
-        TBD
+        RregRs (float) : the radius of the region in the XY plane. 
+                         Because it is normalized by the stellar radius, `RregRs` also corresponds to the (half) angle defining the chord of the region along the stellar surface. 
+                         For a planet the projected region keeps a constant radius in the XY plane and its angular aperture increases toward the limbs.
+                         For a spot the angular aperture is fixed and it is the radius of the projection that decreases toward the limb. The input `RregRs` corresponds to the angular aperture and thus defines the largest square enclosing the spot as it would be seen at the center of the star.   
+        nsub_Dreg (int) : the number of grid cells desired.
     
     Returns:
-        TBD
+        x_st_sky_grid (1D dict) : The x-coordinates of the grid cells.
+        y_st_sky_grid (1D dict) : The y-coordinates of the grid cells.
+        Ssub_Sstar (float) : The surface of each grid cell.
     
     """ 
     
     #Subcell width (in units of Rstar) and surface (in units of Rstar^2 and pi*Rstar^2) 
-    d_sub=2.*RpRs/nsub_Dpl
+    d_sub=2.*RregRs/nsub_Dreg
     Ssub_Sstar=d_sub*d_sub/np.pi
 
     #Coordinates of points discretizing the enclosing square
-    cen_sub=-RpRs+(np.arange(nsub_Dpl)+0.5)*d_sub            
+    cen_sub=-RregRs+(np.arange(-2, nsub_Dreg+2)+0.5)*d_sub       
     xy_st_sky_grid=np.array(list(it_product(cen_sub,cen_sub)))
+    
+    #Keeping grid points behind the planet-occulted region
+    #    - because the planet-occulted region is a disk with constant radius in the XY plane we can reduce the grid to this disk
+    if not spot:
+
+        #Distance to region center (squared)
+        r_sub_pl2=xy_st_sky_grid[:,0]*xy_st_sky_grid[:,0]+xy_st_sky_grid[:,1]*xy_st_sky_grid[:,1]
+
+        #Keeping only grid points behind the planet
+        cond_in_pldisk = ( r_sub_pl2 < RregRs*RregRs)           
+        x_st_sky_grid=xy_st_sky_grid[cond_in_pldisk,0]
+        y_st_sky_grid=xy_st_sky_grid[cond_in_pldisk,1] 
+        r_sub_pl2=r_sub_pl2[cond_in_pldisk] 
 
-    #Distance to planet center (squared)
-    r_sub_pl2=xy_st_sky_grid[:,0]*xy_st_sky_grid[:,0]+xy_st_sky_grid[:,1]*xy_st_sky_grid[:,1]
-
-    #Keeping only grid points behind the planet
-    cond_in_pldisk = ( r_sub_pl2 < RpRs*RpRs)           
-    x_st_sky_grid=xy_st_sky_grid[cond_in_pldisk,0]
-    y_st_sky_grid=xy_st_sky_grid[cond_in_pldisk,1] 
-    r_sub_pl2=r_sub_pl2[cond_in_pldisk] 
+    else:
+        x_st_sky_grid=xy_st_sky_grid[:,0]
+        y_st_sky_grid=xy_st_sky_grid[:,1] 
+        r_sub_pl2 = None
 
     return d_sub,Ssub_Sstar,x_st_sky_grid,y_st_sky_grid,r_sub_pl2
 
 
 
+
+
 def init_surf_shift(gen_dic,inst,vis,data_dic,align_mode):
     r"""**Planet-occulted rv**
 
     Returns measured or theoretical planet-occulted rv
 
     Args:
         TBD
@@ -1344,7 +1439,502 @@
             rv_surf_star = dic_rv['achrom'][pl_ref]['rv'][0,i_in]  
             rv_surf_star_edge=None
 
     return rv_surf_star,rv_surf_star_edge
 
 
 
+
+
+
+
+
+
+
+#%% Spot-specific routines
+
+def is_spot_visible(istar, long_rad, lat_rad, ang_rad, f_GD, RpoleReq) :
+    r"""**Spot visibility**
+
+    Performs a rough estimation of the visibility of a spot, based on star inclination (istar), spot coordinates in star rest frame (long, lat) and spot angular size (ang).
+    To do so, we discretize the spot edge and check if at least one point is visible. The visibility criterion is derived as follows. 
+
+    Let :math:`\mathrm{P} = (x_{\mathrm{st}}, y_{\mathrm{st}}, z_{\mathrm{st}})` be a point on the stellar surface, in the star rest frame (i.e. X axis parallel to the star 
+    equator and  Y axis along the stellar spin), that is on the edge of a spot.
+    
+    Expressing P in spherical coordinates gives
+
+    .. math::
+        & x_{\mathrm{st}} = \mathrm{sin}(long) \mathrm{cos}(lat)
+        & y_{\mathrm{st}} = \mathrm{sin}(lat)
+        & z_{\mathrm{st}} = \mathrm{cos}(long) \mathrm{cos}(lat)
+    
+    Moving P to the 'inclined' star rest frame gives 
+
+    .. math::
+        & x_{\mathrm{sky}} = x_{\mathrm{st}}
+        & y_{\mathrm{sky}} = \mathrm{sin}(i_*) y_{\mathrm{st}} - \mathrm{cos}(i_*) z_{\mathrm{st}}
+        & z_{\mathrm{sky}} = \mathrm{cos}(i_*) y_{\mathrm{st}} + \mathrm{sin}(i_*) z_{\mathrm{st}}
+    
+    The condition for P to be visible is then :math:`z_{\mathrm{sky}} > 0` or 
+    
+    .. math::
+        & \mathrm{cos}(i_*) \mathrm{sin}(lat) + \mathrm{sin}(i_*) \mathrm{cos}(long) \mathrm{cos}(lat) > 0
+
+    WIP : Doing this with gravity darkening
+
+    Args:
+        istar (float) : stellar inclination (in radians)
+        long_rad (float) : spot longitude (in radians)
+        lat_rad (float) : spot latitude (in radians)
+        ang_rad (float) : spot angular size (in radians)
+        f_GD (float) : oblateness coefficient.
+        RpoleReq (float) : pole to equatoral radius ratio.
+     
+    Returns:
+        spot_visible (bool) : spot visibility criterion.
+        
+    """ 
+    spot_visible = False
+    
+    for arg in np.linspace(0,2*np.pi, 20) :
+        
+        #Define the edges of the spots
+        long_edge = long_rad + ang_rad * np.sin(arg)
+        lat_edge  = lat_rad  + ang_rad * np.cos(arg)
+
+        #Define the corresponding x, y, and z coordinates of the edges of the spots in the un-inclined star rest frame
+        x_st_edge = np.sin(long_edge)*np.cos(lat_edge)
+        y_st_edge = np.sin(lat_edge)
+        z_st_edge = np.cos(long_edge)*np.cos(lat_edge)
+
+        #Move the x, y, and z coordinates of the spot edges into the inclined star rest frame 
+        x_sky_edge, y_sky_edge, z_sky_edge = frameconv_star_to_skystar(x_st_edge, y_st_edge, z_st_edge, istar)
+
+        ##### WIP #####
+        #Checking the value of the z coordinate for each edge point to see if the point is visible
+        if f_GD>0:
+            #We take the modulo in case the spot is plotted over a very long time.
+            long_edge_deg = (long_edge * 180/np.pi)%360
+            #Checking if the spot is in the front - rough estimate that doesn't account for the star inclination or spot latitude
+            additive = 90 - (istar * 180/np.pi)
+            first_criterion = (-90-additive <= long_edge_deg and long_edge_deg <= 90+additive) or (270-additive <= long_edge_deg and long_edge_deg <=360) or (-360 <= long_edge_deg and long_edge_deg <= -270+additive)
+            #Now that we known the spot is in front, combine with the condition "is in stellar photosphere"
+            criteria = calc_zLOS_oblate(np.array([x_sky_edge]),np.array([y_sky_edge/(1-f_GD)]),istar, RpoleReq)[2]
+            criterion = first_criterion and criteria
+        #####    #####
+        else:
+            criterion = (z_sky_edge > 0)
+        
+        spot_visible |= criterion
+
+    return spot_visible
+
+def calc_plocced_tiles(pl_prop, x_sky_grid, y_sky_grid):
+    r"""**'Planet-occulted' tiles** 
+    
+    Args:
+        pl_prop (dict) : planet properties.
+        x_sky_grid (1D array) : x coordinates of the stellar / planetary grid in the inclined star frame. (at st, cen, and end)
+        y_sky_grid (1D array) : y coordinates of the stellar / planetary grid in the inclined star frame. (at st, cen, and end)
+     
+    Returns:
+        cond_in_pl (1D array) : array of booleans telling us which cells in the original grid are occulted by the planet.
+
+    """          
+    cond_in_pl = np.zeros(len(x_sky_grid), dtype=bool)
+
+    for i in range(len(pl_prop['x_orb_exp'])):
+
+                
+   
+   
+   
+        pl_prop['x_sky_exp'],pl_prop['y_sky_exp'],_ = frameconv_skyorb_to_skystar(pl_prop['lambda'],pl_prop['x_orb_exp'][i],pl_prop['y_orb_exp'][i],0)
+     
+        pos_cond_close_to_pl = (x_sky_grid - pl_prop['x_sky_exp'])**2 + (y_sky_grid - pl_prop['y_sky_exp'])**2 < pl_prop['RpRs']**2  
+
+        cond_in_pl |=   pos_cond_close_to_pl
+
+    return cond_in_pl
+
+
+
+def retrieve_spots_prop_from_param(star_params, param, inst, vis, t_bjd, exp_dur=None): 
+    r"""**Spot parameters: retrieval and formatting**
+
+    Transforms a dictionary with 'raw' spot properties in the format param_ISinstrument_VSvisit_SPspotname to a more convenient spot dictionary of the form : 
+    spot_prop = { spotname : {'lat' : , 'Tcenter' : , ....}}
+    The formatted contains the initial spot properties as well as additional derived spot properties, such as the longitude and latitude of the spot as well as 
+    its visibility criterion (see is_spot_visible).
+    We assume spot parameter are never defined as common across multiple visits / instruments.
+
+    Args:
+        star_params (dict) : star properties.
+        param (dict) : 'raw' spot properties.
+        inst (str) : instrument considered. Should match the instrument in the 'raw' spot parameter name (see format above).
+        vis (str) : visit considered. Should match the visit in the 'raw' spot parameter name (see format above).
+        t_BJD (float) : timestamp of the exposure considered. Needed to calculate the spot longitude.
+        exp_dur (float) : optional, duration of the exposure considered. If left as None, only the spot properties at the center of the exposure will be computed.
+                            Otherwise, the spot properties at the start, center and end of exposure will be computed. 
+     
+    Returns:
+        spots_prop (dict) : formatted spot dictionary.
+
+    """ 
+
+    spots_prop = {}
+    ctrst_param = []
+    for par in param : 
+        # Parameter is spot-related and linked to the right visit and instrument
+        if ('_SP' in par) and ('_IS'+inst in par) and ('_VS'+vis in par): 
+            if 'ctrst' not in par:
+                spot_par = par.split('__IS')[0]
+                spot_name = par.split('_SP')[1]
+                if spot_name not in spots_prop : spots_prop[spot_name] = {}
+                spots_prop[spot_name][spot_par] = param[par]
+            else:
+                ctrst_param.append(param[par])
+
+    #Ensuring that only one contrast is provided for the spots in each visit
+    if len(ctrst_param)>1:
+        stop('WARNING: All spots in a given visit must share a contrast value. Please provide only one spot contrast parameter.')
+    
+    #Assigning contrast value to each spot
+    for spot_name in spots_prop.keys():
+        spots_prop[spot_name]['ctrst'] = ctrst_param[0]
+ 
+    # Retrieve properties, if spots are visible in the exposures considered
+    for spot in spots_prop : 
+        
+        #Finding the times at the center, start and end of each exposure considered
+        t_bjd_center = deepcopy(t_bjd)
+
+        # Spot lattitude - constant in time
+        lat_rad = spots_prop[spot]['lat']*np.pi/180.
+        
+        # Spot longitude - varies over time
+        sin_lat = np.sin(lat_rad)
+        P_spot = 2*np.pi/((1.-star_params['alpha_rot_spots']*sin_lat**2.-star_params['beta_rot_spots']*sin_lat**4.)*star_params['om_eq_spots']*3600.*24.)
+        Tcen_sp = spots_prop[spot]['Tcenter'] - 2400000.
+        long_rad_center = (t_bjd_center-Tcen_sp)/P_spot * 2*np.pi
+        
+        # Spot center coordinates in star rest frame
+        #Exposure center
+        x_st_center = np.sin(long_rad_center)*np.cos(lat_rad)
+        y_st_center = np.sin(lat_rad)
+        z_st_center = np.cos(long_rad_center)*np.cos(lat_rad)
+
+        # inclined frame
+        istar = np.arccos(param['cos_istar'])
+
+        #Exposure center
+        x_sky_center,y_sky_center,z_sky_center = frameconv_star_to_skystar(x_st_center,y_st_center,z_st_center,istar)
+
+       
+        #Store properties common across the exposure
+        spots_prop[spot]['ang_rad'] = spots_prop[spot]['ang'] * np.pi/180
+        # Store properties at exposure center
+        spots_prop[spot]['lat_rad_exp_center'] = lat_rad
+        spots_prop[spot]['sin_lat_exp_center'] = np.sin(lat_rad)
+        spots_prop[spot]['cos_lat_exp_center'] = np.cos(lat_rad)
+        spots_prop[spot]['long_rad_exp_center'] = long_rad_center
+        spots_prop[spot]['sin_long_exp_center'] = np.sin(long_rad_center)
+        spots_prop[spot]['cos_long_exp_center'] = np.cos(long_rad_center)
+        spots_prop[spot]['x_sky_exp_center'] = x_sky_center
+        spots_prop[spot]['y_sky_exp_center'] = y_sky_center
+        spots_prop[spot]['z_sky_exp_center'] = z_sky_center
+        spots_prop[spot]['is_center_visible'] = is_spot_visible(istar,long_rad_center, lat_rad, spots_prop[spot]['ang_rad'], star_params['f_GD'], star_params['RpoleReq'])
+
+        if exp_dur is not None:
+            t_dur_days = exp_dur/(24.*3600.)
+            t_bjd_start = t_bjd - t_dur_days/2
+            t_bjd_end = t_bjd + t_dur_days/2
+            long_rad_start = (t_bjd_start-Tcen_sp)/P_spot * 2*np.pi
+            long_rad_end = (t_bjd_end-Tcen_sp)/P_spot * 2*np.pi
+            
+            #Exposure start positions
+            x_st_start = np.sin(long_rad_start)*np.cos(lat_rad)
+            y_st_start = np.sin(lat_rad)
+            z_st_start = np.cos(long_rad_start)*np.cos(lat_rad)
+            x_sky_start,y_sky_start,z_sky_start = frameconv_star_to_skystar(x_st_start,y_st_start,z_st_start,istar)
+
+            #Exposure end position
+            x_st_end = np.sin(long_rad_end)*np.cos(lat_rad)
+            y_st_end = np.sin(lat_rad)
+            z_st_end = np.cos(long_rad_end)*np.cos(lat_rad)
+            x_sky_end,y_sky_end,z_sky_end = frameconv_star_to_skystar(x_st_end,y_st_end,z_st_end,istar)
+
+            # Store properties at exposure start
+            spots_prop[spot]['lat_rad_exp_start'] = lat_rad
+            spots_prop[spot]['sin_lat_exp_start'] = np.sin(lat_rad)
+            spots_prop[spot]['cos_lat_exp_start'] = np.cos(lat_rad)
+            spots_prop[spot]['long_rad_exp_start'] = long_rad_start
+            spots_prop[spot]['sin_long_exp_start'] = np.sin(long_rad_start)
+            spots_prop[spot]['cos_long_exp_start'] = np.cos(long_rad_start)
+            spots_prop[spot]['x_sky_exp_start'] = x_sky_start
+            spots_prop[spot]['y_sky_exp_start'] = y_sky_start
+            spots_prop[spot]['z_sky_exp_start'] = z_sky_start
+            spots_prop[spot]['is_start_visible'] = is_spot_visible(istar,long_rad_start, lat_rad, spots_prop[spot]['ang_rad'], star_params['f_GD'], star_params['RpoleReq'])
+
+            # Store properties at exposure end
+            spots_prop[spot]['lat_rad_exp_end'] = lat_rad
+            spots_prop[spot]['sin_lat_exp_end'] = np.sin(lat_rad)
+            spots_prop[spot]['cos_lat_exp_end'] = np.cos(lat_rad)
+            spots_prop[spot]['long_rad_exp_end'] = long_rad_end
+            spots_prop[spot]['sin_long_exp_end'] = np.sin(long_rad_end)
+            spots_prop[spot]['cos_long_exp_end'] = np.cos(long_rad_end)
+            spots_prop[spot]['x_sky_exp_end'] = x_sky_end
+            spots_prop[spot]['y_sky_exp_end'] = y_sky_end
+            spots_prop[spot]['z_sky_exp_end'] = z_sky_end
+            spots_prop[spot]['is_end_visible'] = is_spot_visible(istar,long_rad_end, lat_rad, spots_prop[spot]['ang_rad'], star_params['f_GD'], star_params['RpoleReq'])
+
+    return spots_prop
+
+
+
+def calc_spotted_tiles(spot_prop, x_sky_grid, y_sky_grid, z_sky_grid, grid_dic, star_param, use_grid_dic = False, disc_exp = True) :
+    r"""**'Spotted' tiles** 
+
+    Identification of which cells on the provided grid are covered by spots a.k.a. which cells are 'spotted'. Two methods are available: 
+        
+    - use_grid_dic = False : calculation will be performed on the x_sky_grid, y_sky_grid, z_sky_grid, by moving these grids from the inclined star frame to the star rest frame.
+                            This option can be used for identifiying spotted stellar tiles, when istar is fitted.
+    - use_grid_dic = True : calculation will be performed on the grid contained in grid_dic['x/y/z_st'], which is already in star rest frame (no frame conversion needed). 
+
+
+    To identify which cells in the provided grid are 'spotted', we move the grid cells to the spot reference frame and check which cells are within the spot. 
+    This is a necessary step to obtain the correct shape for the spots, as the spherical nature of the stellar surface must be accounted for. The calculation is as follows:
+    
+    Using the x/y/z grid in the star rest frame (obtained either with a frame conversion function or from the grid dictionary), we rotate the x/y/z grid around the stellar spin axis 
+    to the longitude of the spot
+
+    .. math::
+        & x_{\mathrm{sp}'} = x_{\mathrm{st}} \mathrm{cos}(long) - z_{\mathrm{st}} \mathrm{sin}(long)
+        & y_{\mathrm{sp}'} = y_{\mathrm{st}}
+        & z_{\mathrm{sp}'} = x_{\mathrm{st}} \mathrm{sin}(long) + z_{\mathrm{st}} \mathrm{cos}(long)
+
+    We then rotate the new grid to the latitude of the spot to obtain the x/y/z grid in the spot rest frame
+    
+    .. math::
+        & x_{\mathrm{sp}} = x_{\mathrm{sp}'}
+        & y_{\mathrm{sp}} = y_{\mathrm{sp}'} \mathrm{cos}(lat) - z_{\mathrm{sp}'} \mathrm{sin}(lat)
+        & z_{\mathrm{sp}} = y_{\mathrm{sp}'} \mathrm{sin}(lat) + z_{\mathrm{sp}'} \mathrm{cos}(lat)
+    
+    Finally, we check which cells are within the spot
+
+    .. math::
+        & arctan2(\sqrt{x_{\mathrm{sp}}^{2} + y_{\mathrm{sp}}^{2}}, z_{\mathrm{sp}}) < R_{\mathrm{sp}}
+
+    With R_{\mathrm{sp}} the angular size of the spot in radians.
+
+
+    Args:
+        spot_prop (dict) : formatted spot properties (see retrieve_spots_prop_from_param).
+        x_sky_grid (1D array) : x coordinates of the stellar / planetary grid in the inclined star frame.
+        y_sky_grid (1D array) : y coordinates of the stellar / planetary grid in the inclined star frame.
+        z_sky_grid (1D array) : z coordinates of the stellar / planetary grid in the inclined star frame.
+        grid_dic (dict) : dictionary containing the x/y/z grids in various reference frames, including the star rest frame and inclined star frame.
+        star_param (dict) : star properties.
+        use_grid_dic (bool) : whether or not to use the grid_dic provided to retrieve the x/y/z grids in the star rest frame. Turned off by default.
+        disc_exp (bool) : whether we use the start, center and end of the exposures to figure out if the star is spotted and where the star is spotted, or just the center.
+     
+    Returns:
+        spot_within_grid (bool) : a finer estimate of the spot visibility that can be obtained with is_spot_visible. Essentially, it tells us if at least one tile on the grid is 'spotted'.
+        cond_in_sp (1D array) : array of booleans telling us which cells in the original grid are 'spotted'.
+    
+    """                                      
+
+    if disc_exp:positions = ['start','center','end']
+    else:positions = ['center']
+    cond_in_sp = np.zeros(len(x_sky_grid), dtype=bool)
+
+    for pos in positions:
+
+        if use_grid_dic :
+            cond_close_to_spot = (grid_dic['x_st_sky'] - spot_prop['x_sky_exp_'+pos])**2 + (grid_dic['y_st_sky'] - spot_prop['y_sky_exp_'+pos])**2 < spot_prop['ang_rad']**2
+         
+            x_st_grid, y_st_grid, z_st_grid = grid_dic['x_st'][cond_close_to_spot], grid_dic['y_st'][cond_close_to_spot], grid_dic['z_st'][cond_close_to_spot]
+            
+            
+        else :  
+            cond_close_to_spot = (x_sky_grid - spot_prop['x_sky_exp_'+pos])**2 + (y_sky_grid - spot_prop['y_sky_exp_'+pos])**2 < spot_prop['ang_rad']**2
+        
+            x_st_grid, y_st_grid, z_st_grid = frameconv_skystar_to_star(x_sky_grid[cond_close_to_spot],
+                                                                                        y_sky_grid[cond_close_to_spot],
+                                                                                        z_sky_grid[cond_close_to_spot],
+                                                                                        np.arccos(star_param['cos_istar']))
+            
+            
+        
+        # Retrieve angular coordinates of spot
+        cos_long, sin_long, cos_lat, sin_lat = spot_prop['cos_long_exp_'+pos], spot_prop['sin_long_exp_'+pos], spot_prop['cos_lat_exp_'+pos], spot_prop['sin_lat_exp_'+pos]
+        
+        # Calculate coordinates in spot rest frame
+        x_sp =                       x_st_grid*cos_long - z_st_grid*sin_long
+        y_sp = y_st_grid*cos_lat  - (x_st_grid*sin_long + z_st_grid*cos_long)   *   sin_lat
+        z_sp = y_st_grid*sin_lat  + (x_st_grid*sin_long + z_st_grid*cos_long)   *   cos_lat
+        
+        # Deduce which cells are within the spot
+        phi_sp = np.arctan2(np.sqrt(x_sp**2. + y_sp**2.),z_sp)
+        pos_cond_in_sp = cond_close_to_spot
+        pos_cond_in_sp[cond_close_to_spot] = (phi_sp <= spot_prop['ang_rad'])
+    
+        cond_in_sp |= pos_cond_in_sp
+
+    # Check if at least one tile is within the spot
+    spot_within_grid = (True in cond_in_sp)   
+    
+
+    return spot_within_grid, cond_in_sp
+
+
+
+
+
+def calc_spotted_region_prop(line_occ_HP_band,cond_occ,spot_prop,iband,system_prop,system_spot_prop, par_star, sp_proc_band, spot_consid, Ssub_Sstar_sp, Ssub_Sstar_ref, Istar_norm_band, sum_prop_dic_spot,\
+                                    coord_reg_dic_spot, range_reg, Focc_star_band, par_list, range_par_list, args, cb_band, pl_loc_x = {}, pl_loc_y = {}, oversamp_idx = None, RpRs = None, plocc = False) :
+    
+    r"""**Spot-occulted properties: define and update**
+    
+    Identify the spot-occulted region in each exposure provided and calculate its properties. 
+    Update the provided dictionaries which contain the average and sum of the properties of interest over the spot-occulted region.
+
+    Args:
+        line_occ_HP_band (str) : the precision with which to process the exposure.
+        cond_occ (bool) : whether there is an occultation by at least one spot in the exposure considered.
+        spot_prop (dict) : formatted spot properties Dictionary (see retrieve_spots_prop_from_param).
+        iband (int) : index of the band used to retrieve the corresponding planet and spot limb-darkening properties.
+        system_prop (dict) : quiet star limb-darkening properties.
+        system_spot_prop (dict) : spot limb-darkening properties.
+        star_params (dict) : star properties.
+        sp_proc_band (list) : spots previously processed. Used to account for the overlap of spots.
+        spot_consid (str) : name of the spot being processed.
+        Ssub_Sstar_sp (float): surface of grid cells in the spot-occulted region grid.
+        Ssub_Sstar_ref (float) : surface of grid cells in the stellar grid.
+        Istar_norm_band (float) : total intensity of the star in the band considered.
+        sum_prop_dic_spot (dict) : dictionary containing the value of all parameters of interest (par_list), summed over the spotted region in the exposure considered, and for the band of interest.
+        coord_reg_dic_spot (dict) : dictionary containing the value of all parameters of interest (par_list), averaged over the spotted region in the exposure considered, and for the band of interest.
+        range_reg (dict) : dictionary containing the range of average values the parameters of interest (range_par_list) can take during this exposure.
+        Focc_star_band (float) : total flux occulted by the spot in the exposure and band considered. 
+        par_list (list) : List of parameters of interest, whose value in sum_prop_dict_spot will be updated.
+        range_par_list (list) : list of parameters of interest, whose range of values, stored in range_reg, will be updated.
+        args (dict) : parameters used to generate the intrinsic profiles.
+        cb_band (list) : coefficients used to calculate the convective blueshift RV contribution.
+        pl_loc_x (dict) : optional, x coordinates of the planets' oversampled positions in the exposure considered. Used to account for the cells in the spot-occulted region that are occulted by the planet.
+        pl_loc_y (dict) : optional, y coordinates of the planets' oversampled positions in the exposure considered. Used to account for the cells in the spot-occulted region that are occulted by the planet.
+        oversamp_idx (int) : optional, index of the oversampled exposure being processed.
+        RpRs (dict) : optional, planets' limb-darkening properties.
+        plocc (bool) : optional, whether the exposure considered is being occulted by planets or not. Turned off by default.
+
+    Returns:
+        Focc_star_band (float) : the input Focc_star_band updated with the flux occulted by the spot considered.
+        cond_occ (bool) : updated version of the input cond_occ. Tells us whether or not the spot occulted the exposure considered.
+    
+    """ 
+    
+    parameter_list = deepcopy(par_list)
+    range_parameter_list = deepcopy(range_par_list)
+    
+    #We have as input a grid discretizing the spot.
+    #We have a condition to find the cells in the input grid that are in the stellar grid.
+    cond_in_star = spot_prop[spot_consid]['x_sky_grid']**2 + spot_prop[spot_consid]['y_sky_grid']**2 < 1.
+
+    #We have a condition to figure out which cells in this input grid are occulted.
+    ##Take the cells that are in the stellar grid.
+    new_x_sky_grid = spot_prop[spot_consid]['x_sky_grid'][cond_in_star]
+    new_y_sky_grid = spot_prop[spot_consid]['y_sky_grid'][cond_in_star]
+
+    ##Retrieve the z-coordinate for the cells.
+    new_z_sky_grid = np.sqrt(1 - new_x_sky_grid**2 - new_y_sky_grid**2)
+
+    ##Move coordinates to the star reference frame and then the spot reference frame
+    x_st_grid, y_st_grid, z_st_grid = frameconv_skystar_to_star(new_x_sky_grid, new_y_sky_grid, new_z_sky_grid, par_star['istar_rad'])
+    x_spot_grid = x_st_grid*spot_prop[spot_consid]['cos_long_exp_center'] - z_st_grid*spot_prop[spot_consid]['sin_long_exp_center']
+    y_spot_grid = y_st_grid*spot_prop[spot_consid]['cos_lat_exp_center'] - (z_st_grid*spot_prop[spot_consid]['cos_long_exp_center'] + x_st_grid*spot_prop[spot_consid]['sin_long_exp_center']) * spot_prop[spot_consid]['sin_lat_exp_center']
+    z_spot_grid = y_st_grid*spot_prop[spot_consid]['sin_lat_exp_center'] + (z_st_grid*spot_prop[spot_consid]['cos_long_exp_center'] + x_st_grid*spot_prop[spot_consid]['sin_long_exp_center']) * spot_prop[spot_consid]['cos_lat_exp_center']
+    cond_in_sp = x_spot_grid**2. + y_spot_grid**2. <= spot_prop[spot_consid]['ang_rad']**2
+
+    #Making our refined spot-occultation grid and calculating the number of points it has
+    spot_x_sky_grid = new_x_sky_grid[cond_in_sp]
+    spot_y_sky_grid = new_y_sky_grid[cond_in_sp]
+    spot_z_sky_grid = new_z_sky_grid[cond_in_sp]
+    n_occ_sp = np.sum(cond_in_sp)
+
+    #--------------------------------
+    # Accounting for planet occultation of the spot
+    if plocc:
+        for planet in list(pl_loc_x.keys()):
+            cond_in_planet_disk = (spot_x_sky_grid - pl_loc_x[planet][oversamp_idx])**2 + (spot_y_sky_grid -  pl_loc_y[planet][oversamp_idx])**2 < RpRs[planet][iband]**2
+            spot_x_sky_grid = spot_x_sky_grid[~cond_in_planet_disk]
+            spot_y_sky_grid = spot_y_sky_grid[~cond_in_planet_disk]
+            spot_z_sky_grid = spot_z_sky_grid[~cond_in_planet_disk]
+            n_occ_sp -= np.sum(cond_in_planet_disk)
+
+    # Accounting for overlap with other spots - spot's have the same contrast so we can just remove the overlapping cells
+    if len(sp_proc_band)>0:
+        for sp_prev in sp_proc_band:
+
+            #Move current spot coordinates to the star reference frame and then the other spot's reference frame
+            updated_x_st_grid, updated_y_st_grid, updated_z_st_grid = frameconv_skystar_to_star(spot_x_sky_grid, spot_y_sky_grid, spot_z_sky_grid, par_star['istar_rad'])
+            x_prev_spot_grid = updated_x_st_grid*spot_prop[sp_prev]['cos_long_exp_center'] - updated_z_st_grid*spot_prop[sp_prev]['sin_long_exp_center']
+            y_prev_spot_grid = updated_y_st_grid*spot_prop[sp_prev]['cos_lat_exp_center'] - (updated_z_st_grid*spot_prop[sp_prev]['cos_long_exp_center'] + updated_x_st_grid*spot_prop[sp_prev]['sin_long_exp_center']) * spot_prop[sp_prev]['sin_lat_exp_center']
+            cond_in_prev_spot = x_prev_spot_grid**2. + y_prev_spot_grid**2 <= system_spot_prop[sp_prev][iband]**2
+
+            #Remove cells that overlap
+            spot_x_sky_grid = spot_x_sky_grid[~cond_in_prev_spot]
+            spot_y_sky_grid = spot_y_sky_grid[~cond_in_prev_spot]
+            spot_z_sky_grid = spot_z_sky_grid[~cond_in_prev_spot]
+            n_occ_sp -= np.sum(cond_in_prev_spot)
+    sp_proc_band += [spot_consid]
+
+
+    #--------------------------------
+
+    #Figure out the number of cells occulted and store it
+    if n_occ_sp > 0:
+        cond_occ = True
+
+    #Making the grid of coordinates for the calc_Isurf_grid function.
+    coord_grid = {}
+    #Getting, x, y, z, sky-projected radius, and number of occulted cells.
+    coord_grid['x_st_sky'] = spot_x_sky_grid
+    coord_grid['y_st_sky'] = spot_y_sky_grid
+    coord_grid['z_st_sky'] = spot_z_sky_grid
+
+    coord_grid['r2_st_sky']=coord_grid['x_st_sky']*coord_grid['x_st_sky']+coord_grid['y_st_sky']*coord_grid['y_st_sky']
+
+    coord_grid['nsub_star'] = n_occ_sp
+
+    #Getting the coordinates in the star rest frame
+    coord_grid['x_st'], coord_grid['y_st'], coord_grid['z_st'] = frameconv_skystar_to_star(coord_grid['x_st_sky'], coord_grid['y_st_sky'], coord_grid['z_st_sky'], par_star['istar_rad'])
+    
+    #Retrieve the stellar flux grids over this local occulted-region grid.
+    _,_,mu_grid_occ,Fsurf_grid_occ,Ftot_occ,_ = calc_Isurf_grid([iband], coord_grid['nsub_star'], system_prop, coord_grid, par_star, Ssub_Sstar_sp, Istar_norm_band, region='pl', Ssub_Sstar_ref=Ssub_Sstar_ref)
+
+    #Retrieve the flux grid for the spot's emission (since spots have different LD law compared to the 'quiet' stellar surface)
+    _,_,_,Fsurf_grid_emit,Ftot_emit,_ = calc_Isurf_grid([iband], coord_grid['nsub_star'], system_spot_prop, coord_grid, par_star, Ssub_Sstar_sp, Istar_norm_band, region='pl', Ssub_Sstar_ref=Ssub_Sstar_ref)
+
+    #Scale the flux grid to the desired level
+    Fsurf_grid_occ *= par_star['cont']
+    Fsurf_grid_emit *= par_star['cont']
+    Ftot_occ *= par_star['cont']
+    Ftot_emit *= par_star['cont']
+
+    #--------------------------------
+
+    #Updating the provided dictionaries 
+    coord_grid['mu'] = mu_grid_occ[:,0]
+    Focc_star_band += (Ftot_occ[0] - (Ftot_emit[0]*(1-spot_prop[spot_consid]['ctrst'])))
+    sum_prop_dic_spot['nocc'] += coord_grid['nsub_star']
+    
+    #Distance from projected orbital normal in the sky plane, in absolute value
+    if 'xp_abs' in par_list : par_list.remove('xp_abs')
+    if 'xp_abs' in range_par_list : range_par_list.remove('xp_abs')    
+    
+    #--------------------------------
+    #Co-adding properties from current region to the cumulated values over oversampled spot positions 
+    sum_region_prop(line_occ_HP_band,iband,args,parameter_list,Fsurf_grid_occ[:,0],Fsurf_grid_emit[:,0],coord_grid,Ssub_Sstar_sp,cb_band,range_parameter_list,range_reg,sum_prop_dic_spot,coord_reg_dic_spot,par_star,None,spot_prop[spot_consid]['ctrst']) 
+
+    return Focc_star_band, cond_occ
+
+
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_grids/ANTARESS_prof_grid.py` & `antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_prof_grid.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,51 @@
 import astropy.convolution.convolve as astro_conv
 import bindensity as bind
 from pysme import sme as SME
 from pysme.linelist.vald import ValdFile
 from pysme.abund         import Abund
 from pysme.synthesize import synthesize_spectrum
 import lmfit
+from ctypes import CDLL,c_double,c_int,c_void_p,cast,POINTER
+import os as os_system
 from ..ANTARESS_analysis.ANTARESS_model_prof import pol_cont,dispatch_func_prof,polycoeff_def,calc_polymodu,calc_linevar_coord_grid
 from ..ANTARESS_grids.ANTARESS_star_grid import up_model_star,calc_RVrot,calc_CB_RV,get_LD_coeff
 from ..ANTARESS_general.utils import closest,np_poly,np_interp,gen_specdopshift,closest_arr,MAIN_multithread,stop,def_edge_tab
 
+def def_Cfunc_prof():
+    r"""**C profile calculation**
+
+    Defines the C function and its parameters used in the optimization
+
+    Args:
+        TBD
+    
+    Returns:
+        TBD
+    
+    """ 
+
+    code_dir = os_system.path.dirname(__file__).split('ANTARESS_grids')[0]
+    myfunctions = CDLL(code_dir+'/ANTARESS_analysis/C_grid/Gauss_star_grid.so')
+    fun_to_use = myfunctions.C_coadd_loc_gauss_prof
+    fun_to_free = myfunctions.free_gaussian_line_grid
+    fun_to_use.argtypes = [np.ctypeslib.ndpointer(c_double),
+                    np.ctypeslib.ndpointer(c_double),
+                    np.ctypeslib.ndpointer(c_double),
+                    np.ctypeslib.ndpointer(c_double),
+                    np.ctypeslib.ndpointer(c_double),
+                    c_int,
+                    c_int]
+    fun_to_use.restype = c_void_p
+    fun_to_free.argtypes = [np.ctypeslib.ndpointer(c_double)]
+    fun_to_free.restype = None
+    
+    return fun_to_use,fun_to_free
+
+
 
 def custom_DI_prof(param,x,args=None):
     r"""**Disk-integrated profile: model function**
 
     Calculates custom disk-integrated stellar profile.
     The disk-integrated profile is built upon a discretized grid of the stellar surface to allow accounting for any type of intensity and velocity field.
     This routine is separated from init_custom_DI_prof() so that it can be used in fitting routines with varying parameters.
@@ -34,16 +67,16 @@
     #Updating stellar grid and line profile grid
     #    - only if routine is called in fit mode, otherwise the default pipeline stellar grid and the scaling from init_custom_DI_prof() are used
     #--------------------------------------------------------------------------------
     if args['fit']:    
 
         #Updating stellar grid
         #    - if stellar grid is different from the default one 
-        if args['var_star_grid']:
-            
+        if args['var_star_grid'] and (args['unquiet_star'] is None):
+
             #Update variable stellar properties and stellar grid
             up_model_star(args,param)
 
             #Update broadband scaling of intrinsic profiles into local profiles
             #    - only necessary if stellar grid is updated
             args['Fsurf_grid_spec'] = theo_intr2loc(args['grid_dic'],args['system_prop'],args,args['ncen_bins'],args['grid_dic']['nsub_star'])     
     
@@ -62,21 +95,52 @@
     if np.max(np.abs(cb_band))!=0.:rv_surf_star_grid += np_poly(cb_band)(args['grid_dic']['mu']).flatten()
 
     #--------------------------------------------------------------------------------        
     #Coadding local line profiles over stellar disk
     #--------------------------------------------------------------------------------
     icell_list = np.arange(args['grid_dic']['nsub_star'])
     
+    #Reducing grid to quiet cells
+    if args['unquiet_star'] is not None:
+        cond_quiet_star = ~args['unquiet_star']
+        rv_surf_star_grid=rv_surf_star_grid[cond_quiet_star]
+        args['grid_dic']['mu']=args['grid_dic']['mu'][cond_quiet_star]
+        args['flux_intr_grid']=args['flux_intr_grid'][cond_quiet_star]
+        icell_list=icell_list[cond_quiet_star]
+        args['Fsurf_grid_spec']=args['Fsurf_grid_spec'][cond_quiet_star]
+        nsub_star=len(icell_list)
+    else:
+        nsub_star = len(icell_list)
+        cond_quiet_star = np.repeat(True,nsub_star)
+
+    #Set up properties for fast line profile grid calculation
+    use_OS_grid=False
+    use_C_OS_grid=False
+    if 'OS_grid' in args and args['OS_grid']:use_OS_grid=True
+    if 'C_OS_grid' in args and args['C_OS_grid']:
+        use_OS_grid=False
+        use_C_OS_grid=True
+    
     #Multithreading
     #    - disabled with theoretical profiles, there seems to be an incompatibility with sme
     if (args['nthreads']>1) and (args['mode']!='theo') and ('prof_grid' not in args['unthreaded_op']) :
-        flux_DI_sum=MAIN_multithread(coadd_loc_line_prof,args['nthreads'],args['grid_dic']['nsub_star'],[rv_surf_star_grid,icell_list,args['Fsurf_grid_spec'],args['flux_intr_grid'],args['grid_dic']['mu']],(param,args,),output = True)                           
-    
+        simplified_args={}
+        for key in ['mode', 'mac_mode', 'input_cell_all', 'func_prof', 'cen_bins', 'nthreads']:simplified_args[key]=args[key]
+        flux_DI_sum=MAIN_multithread(coadd_loc_line_prof,args['nthreads'],nsub_star,[rv_surf_star_grid,icell_list,args['Fsurf_grid_spec'],args['flux_intr_grid'],args['grid_dic']['mu']],(param,simplified_args,),output = True)              
+
     #Direct call
-    else:flux_DI_sum=coadd_loc_line_prof(rv_surf_star_grid,icell_list,args['Fsurf_grid_spec'],args['flux_intr_grid'],args['grid_dic']['mu'],param,args)
+    else:
+        if use_OS_grid:
+            for pol_par in args['input_cell_all']:args['input_cell_all'][pol_par]=args['input_cell_all'][pol_par][cond_quiet_star]
+            flux_DI_sum=coadd_loc_gauss_prof(rv_surf_star_grid,args['Fsurf_grid_spec'],args)
+        elif use_C_OS_grid:
+            for pol_par in args['input_cell_all']:args['input_cell_all'][pol_par]=args['input_cell_all'][pol_par][cond_quiet_star]
+            Fsurf_grid_spec = args['Fsurf_grid_spec'][:, 0]
+            flux_DI_sum = use_C_coadd_loc_gauss_prof(rv_surf_star_grid,Fsurf_grid_spec,args)
+        else:flux_DI_sum=coadd_loc_line_prof(rv_surf_star_grid,icell_list,args['Fsurf_grid_spec'],args['flux_intr_grid'],args['grid_dic']['mu'],param,args)
     
     #Co-adding profiles
     DI_flux_norm = np.sum(flux_DI_sum,axis=0)
 
     #Scaling disk-integrated profile to requested continuum
     #    - DI_flux_norm is returned by the function normalized to unity  
     DI_flux_cont = param['cont']*DI_flux_norm
@@ -264,18 +328,18 @@
     Returns:
         TBD
     
     """ 
     #Stellar grid properties
     #    - all stellar properties are initialized to default stellar values
     #      those defined as variable properties through the settings will be overwritten in 'par_formatting'
-    for key,vary,bd_min,bd_max in zip(['veq','alpha_rot','beta_rot','c1_CB','c2_CB','c3_CB','cos_istar','f_GD','beta_GD','Tpole','A_R','ksi_R','A_T','ksi_T','eta_R','eta_T'],
-                                      [False,  False,     False,     False,  False,  False,  False,      False, False,    False,  False, False, False,False,  False,   False],
-                                      [0.,    None,       None,      None,   None,   None,   -1.,        0.,     0.,      0.,     0. , 0.,     0. ,  0.,     0. ,    0.],
-                                      [1e4,   None,       None,      None,   None,   None,    1.,        1.,     1.,      1e5,    1.,  1e5,    1e5,  1e5,    100.,   100.]):
+    for key,vary,bd_min,bd_max in zip(['veq','veq_spots','alpha_rot','alpha_rot_spots','beta_rot','beta_rot_spots','c1_CB','c2_CB','c3_CB','c1_CB_spots','c2_CB_spots','c3_CB_spots','cos_istar','f_GD','beta_GD','Tpole','A_R','ksi_R','A_T','ksi_T','eta_R','eta_T'],
+                                      [False,   False,      False,         False,        False,        False,        False, False,  False,   False,         False,          False,   False,    False,  False,   False, False, False, False, False,  False,   False],
+                                      [0.,      0.,         None,          None,         None,         None,         None,  None,   None,    None,          None,           None,     -1.,       0.,     0.,      0.,     0. ,   0.,    0. ,   0.,     0. ,      0.],
+                                      [1e4,     1e4,        None,          None,         None,         None,         None,  None,   None,    None,          None,           None,      1.,       1.,     1.,      1e5,    1.,   1e5,    1e5,  1e5,    100.,    100.]):
         if key in star_params:params.add_many((key, star_params[key],   vary,    bd_min,bd_max,None))
 
     #Properties specific to disk-integrated profiles
     if fixed_args['DI_grid']:
         for ideg in range(1,5):params.add_many(('LD_u'+str(ideg),  system_prop['achrom']['LD_u'+str(ideg)][0],              False,    None,None,None))   
 
     #Line model properties
@@ -592,13 +656,63 @@
     for isub,(icell,rv_surf_star,flux_intr_cell,mu_cell) in enumerate(zip(icell_list,rv_surf_star_grid,flux_intr_grid,mu_grid)):
         flux_DI_sum+=[calc_loc_line_prof(icell,rv_surf_star,Fsurf_grid_spec[isub],flux_intr_cell,mu_cell,args,param)]
     return flux_DI_sum
 
 
 
 
+def coadd_loc_gauss_prof(rv_surf_star_grid, Fsurf_grid_spec, args):
+    r"""**Local Gaussian line co-addition**
+
+    Oversimplified way of cumulating the local profiles from each cell of the stellar disk. 
+    This version assumes gaussian line profiles in each cell.
+
+    Args:
+        TBD
+    
+    Returns:
+        TBD
+    
+    """ 
+    #Define necessay grids    
+    true_rv_surf_star_grid = np.tile(rv_surf_star_grid, (args['ncen_bins'], 1)).T
+    model_table = np.ones((Fsurf_grid_spec.shape[0], args['ncen_bins']), dtype=float) * args['cen_bins']
+    cont_grid = np.ones((Fsurf_grid_spec.shape[0], args['ncen_bins']))
+    sqrt_log2 = np.sqrt(np.log(2.))
+    ctrst_grid = np.tile(args['input_cell_all']['ctrst'], (args['ncen_bins'], 1)).T
+    FWHM_grid = np.tile(args['input_cell_all']['FWHM'], (args['ncen_bins'], 1)).T
+    
+    #Make grid of profiles    
+    gaussian_line_grid = cont_grid*(1.-ctrst_grid*np.exp(-(2.*sqrt_log2*(model_table-true_rv_surf_star_grid)/FWHM_grid)**2))
+
+    gaussian_line_grid *= Fsurf_grid_spec
+
+    return gaussian_line_grid
+
+
+
+def use_C_coadd_loc_gauss_prof(rv_surf_star_grid, Fsurf_grid_spec, args):
+    r"""**C++ local Gaussian line co-addition**
+
+    C++ implementation of `coadd_loc_gauss_prof()`.
+
+    Args:
+        TBD
+    
+    Returns:
+        TBD
+    
+    """ 
+    Fsurf_grid_spec_shape0 = len(Fsurf_grid_spec)
+    ncen_bins = args['ncen_bins']
+    gauss_grid_ptr = args['fun_to_use'](rv_surf_star_grid, args['input_cell_all']['ctrst'], args['input_cell_all']['FWHM'], 
+        args['cen_bins'], Fsurf_grid_spec*10, ncen_bins, Fsurf_grid_spec_shape0)
+    gauss_grid = np.frombuffer(cast(gauss_grid_ptr, POINTER(c_double * (ncen_bins * Fsurf_grid_spec_shape0))).contents, dtype=np.float64)
+    truegauss_grid = gauss_grid.reshape((Fsurf_grid_spec_shape0, ncen_bins))/10
+    args['fun_to_free'](gauss_grid)
+    return truegauss_grid
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_grids/ANTARESS_star_grid.py` & `antaress-1.1.1/src/antaress/ANTARESS_grids/ANTARESS_star_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,18 +252,19 @@
 
 def get_LD_coeff(transit_prop,iband):
     r"""**Limb-Darkening coefficients**
 
     Store input limb-darkening coefficients in common structure [LD_u1,LD_u2,LD_u3,LD_u4].
 
     Args:
-        TBD
-    
+        transit_prop (dict) : dictionary containing the planet/spot limb-darkening properties.
+        iband (int) : index of the band considered.
+
     Returns:
-        TBD
+        ld_coeff (list) : formatted list of the limb-darkening coefficients used.
     
     """     
     
     LD_mod = transit_prop['LD'][iband]
     #Uniform
     if LD_mod == 'uniform':
         ld_coeff=[np.nan,np.nan,np.nan,np.nan]
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_launch/ANTARESS_gridrun.py` & `antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_gridrun.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_launch/ANTARESS_launcher.py` & `antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_launcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import os as os_system
+import sys
 import argparse
+import json
+import logging
+from fontTools import configLogger
 #The following relative imports are necessary to create an executable command
 from ..ANTARESS_process.ANTARESS_main import ANTARESS_main,ANTARESS_settings_overwrite
 from ..ANTARESS_launch.ANTARESS_gridrun import ANTARESS_gridrun
 from ..ANTARESS_general.utils import import_module
  
 
-def ANTARESS_launcher(custom_systems = '',custom_settings = '',custom_plot_settings = '',working_path='',nbook_dic = {}):
+def ANTARESS_launcher(custom_systems = '',custom_settings = '',custom_plot_settings = '',working_path='',nbook_dic = {} , exec_comm = True):
     r"""**ANTARESS launch routine.**
     
     Runs ANTARESS with default or manual settings.  
     
     Args:
         custom_systems (str): name of custom systems file (default "": ANTARESS_systems.py file is used)
         custom_settings (str): name of custom settings file (default "": ANTARESS_settings.py file is used)
@@ -20,29 +24,34 @@
         working_path (str): path to the working directory, in which the workflow outputs will be stored (default "": current directory is used)
                             if custom files are used, they should be placed in the working directory 
     
     Returns:
         None
     
     """ 
-
+    
+    # Suppress log messages from the fontTools package
+    fontTools_logger = logging.getLogger('fontTools')
+    fontTools_logger.addHandler(logging.NullHandler())
+    
     #Read executable arguments
     #    - will be used when ANTARESS is called as an executable through terminal
-    parser=argparse.ArgumentParser(prog = "antaress",description='Launch ANTARESS workflow')
-    parser.add_argument("--custom_systems",      type=str, default='',help = 'Name of custom systems file (default "": default file ANTARESS_systems.py is used)')
-    parser.add_argument("--custom_settings",     type=str, default='',help = 'Name of custom settings file (default "": default file ANTARESS_settings.py is used)')
-    parser.add_argument("--custom_plot_settings",type=str, default='',help = 'Name of custom plot settings file (default "": default file ANTARESS_plot_settings.py is used)')
-    parser.add_argument("--working_path", type=str, default='' ,help = 'Path to user settings files (default "./": user files are retrieved from current directory)')
-    parser.add_argument("--nbook_dic", type=dict, default={})
-    input_args=parser.parse_args()
-    custom_systems = input_args.custom_systems
-    custom_settings = input_args.custom_settings
-    custom_plot_settings = input_args.custom_plot_settings
-    working_path = input_args.working_path
-    nbook_dic = input_args.nbook_dic
+    if exec_comm:
+        parser=argparse.ArgumentParser(prog = "antaress",description='Launch ANTARESS workflow')
+        parser.add_argument("--custom_systems",      type=str, default='',help = 'Name of custom systems file (default "": default file ANTARESS_systems.py is used)')
+        parser.add_argument("--custom_settings",     type=str, default='',help = 'Name of custom settings file (default "": default file ANTARESS_settings.py is used)')
+        parser.add_argument("--custom_plot_settings",type=str, default='',help = 'Name of custom plot settings file (default "": default file ANTARESS_plot_settings.py is used)')
+        parser.add_argument("--working_path", type=str, default='' ,help = 'Path to user settings files (default "./": user files are retrieved from current directory)')
+        parser.add_argument("-d", "--nbook_dic", type=json.loads, default={})
+        input_args=parser.parse_args()
+        custom_systems = input_args.custom_systems
+        custom_settings = input_args.custom_settings
+        custom_plot_settings = input_args.custom_plot_settings
+        working_path = input_args.working_path
+        nbook_dic = input_args.nbook_dic 
 
     #Initializes main dictionaries
     gen_dic={}
     plot_dic={}
     corr_spot_dic={}
     data_dic={
         'DI':{'fit_prof':{},'mask':{}},
@@ -92,15 +101,15 @@
     #Retrieve chosen system
     system_params = all_system_params[gen_dic['star_name']]
 
     print('****************************************')
     print('Launching ANTARESS')
     print('****************************************')
     print('')
-    
+
     #Moving to code directory
     os_system.chdir(code_dir)
   
     #Run over nominal settings properties
     #    - notebook settings have already been used to overwrite congiguration settings, and are only passed on to overwrite the plot settings if relevant
     if not gen_dic['grid_run']:
         ANTARESS_main(data_dic,mock_dic,gen_dic,theo_dic,plot_dic,glob_fit_dic,detrend_prof_dic, corr_spot_dic,system_params,nbook_dic,custom_plot_settings)
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_launch/ANTARESS_settings.py` & `antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,21 +24,27 @@
     #%%%% Planetary system
     
     #%%%%% Star name
     gen_dic['star_name']='Arda' 
     
     
     #%%%%% Transiting planets
-    #    - indicate names of the transiting planets to be processed
+    #    - indicate names (as defined in ANTARESS_systems) of the transiting planets to be processed
     #    - required to retrieve parameters for the stellar system and light curve
-    #    - name as given in all_systems_params
     #    - for each planet, indicate the instrument and visits in which its transit should be taken into account (visit names are those given through 'data_dir_list')
     #      if the pipeline is runned with no data, indicate the names of the mock dataset created artifially with the pipeline
     #    - format is 'planet':{'inst':['vis']}
-    gen_dic['transit_pl']={}     
+    gen_dic['transit_pl']={}  
+    
+
+    #%%%%% Visible spots
+    #    - indicate names (defined here) of the visible spots to be processed
+    #    - for each spot, indicate the instrument and visits in which its transit should be taken into account (visit names are those given through 'data_dir_list')
+    #    - format is 'spot':{'inst':['vis']}
+    gen_dic['transit_sp']={}  
     
     
     #%%%%% TTVs
     #    - if a visit is defined in this dictionary, the mid-transit time for this visit will be set to the specific value defined here
     #    - format is {'planet':{'inst':{'vis': value}}}
     gen_dic['Tcenter_visits'] = {}
     
@@ -219,14 +225,21 @@
     gen_dic['mock_data'] =  False
     
     
     #%%%% Multi-threading
     mock_dic['nthreads'] = int(0.8*cpu_count())       
     
     
+    #%%%%% Unthreaded operations
+    #    - all operations are multi-threaded by default, but overheads of sharing data between threads may counterbalance the benefits of threading the model
+    #    - select here which operations not to thread:
+    # + 'prof_grid'
+    mock_dic['unthreaded_op'] = []    
+    
+    
     #%%%% Defining artificial visits
     #    - exposures are defined for each instrument/visit
     #    - exposures can be defined
     # + manually: indicate lower/upper exposure boundaries ('bin_low' and 'bin_high', ordered)
     # + automatically : indicate total range ('exp_range' in BJD) and number of exposures ( 'nexp')
     #    - indicate times in BJD
     mock_dic['visit_def']={}
@@ -608,17 +621,14 @@
     #    - for all analytical line models in the pipeline
     #    - in km/s (profiles in wavelength space are modelled in RV space and then converted) 
     #    - can be relevant to fit profiles measured at low resolution
     #    - set to None for no oversampling
     theo_dic['rv_osamp_line_mod']=None
 
 
-    #%%%% Spots
-    gen_dic['theo_spots'] = False #Samson: is this field still useful ?
-    
     #%%%%% Discretization         
     theo_dic['nsub_Dspot']={} 
 
 
     #%%%%% Exposure oversampling
     theo_dic['n_oversamp_spot']={}  
     
@@ -1874,14 +1884,15 @@
     #%%%%% Fitting mode 
     #    - 'chi2', 'mcmc', ''
     data_dic['DI']['fit_mode']='chi2'  
     
     
     #%%%%% Printing fits results
     data_dic['DI']['verbose']= False
+    data_dic['DI']['print_par'] = True
 
     
     #%%%%% Monitor MCMC
     data_dic['DI']['progress']= True
     
     
     #%%%%% Priors on variable properties
@@ -2040,14 +2051,15 @@
     #%%%%% Fitting mode 
     #    - 'chi2', 'mcmc', ''
     glob_fit_dic['DIProp']['fit_mode']='chi2'  
     
     
     #%%%%% Printing fits results
     glob_fit_dic['DIProp']['verbose'] = False
+    glob_fit_dic['DIProp']['print_par'] = True
 
 
     #%%%%% Monitor MCMC
     glob_fit_dic['DIProp']['progress']= True
     
     
     #%%%%% Priors on variable properties
@@ -2666,21 +2678,21 @@
     plot_dic['DImask_RVdisp'] = ''
     
  
     
 
     
     ##################################################################################################
-    #%% Residual and intrinsic profiles
+    #%% Differential and intrinsic profiles
     ##################################################################################################  
     
     
     
     ##################################################################################################
-    #%%% Module: extracting residual profiles
+    #%%% Module: extracting differential profiles
     #    - potentially affected by the planetary atmosphere
     ##################################################################################################   
     
     #%%%% Activating
     gen_dic['res_data'] = False
     
     
@@ -2798,16 +2810,16 @@
     
     
     
     
     
     
     ##################################################################################################
-    #%%% Module: CCF conversion for residual & intrinsic spectra 
-    #    - calculating CCFs from OT residual and intrinsic stellar spectra
+    #%%% Module: CCF conversion for differential & intrinsic spectra 
+    #    - calculating CCFs from OT differential and intrinsic stellar spectra
     #    - for analysis purpose, ie do not apply if atmospheric extraction is later requested
     #    - every analysis afterwards will be performed on those CCFs
     #    - ANTARESS will stop if intrinsic profiles are simultaneously required to extract atmospheric spectra 
     ##################################################################################################   
      
     
     #%%%% Activating
@@ -2815,32 +2827,32 @@
     
      
     #%%%% Calculating/retrieving 
     gen_dic['calc_Intr_CCF'] = True 
     
     
     #%%%% Error definition
-    #    - force errors on out-of-transit residual and intrinsic CCFs to their continuum dispersion
+    #    - force errors on out-of-transit differential and intrinsic CCFs to their continuum dispersion
     data_dic['Intr']['disp_err']=False
     
     
     
     
     
     
     
     
     
     
     
     
     ##################################################################################################
-    #%%% Module: PCA of out-of-transit residual profiles
+    #%%% Module: PCA of out-of-transit differential profiles
     #    - for now only coded for CCF data type
-    #    - use this module to derive PC and match their combination to residual and intrinsic profiles in the fit module
+    #    - use this module to derive PC and match their combination to differential and intrinsic profiles in the fit module
     #      correction is then applied through the CCF correction module
     #    - pca is applied to the pre-transit, post-transit, and out-of-transit data independently
     #      the noise model is fitted using the out-PC
     ##################################################################################################
     
     
     #%%%% Activating
@@ -2934,15 +2946,15 @@
     
 
     
     
     
         
     ##################################################################################################
-    #%%% Module: 2D->1D conversion for residual & intrinsic spectra
+    #%%% Module: 2D->1D conversion for differential & intrinsic spectra
     #    - every analysis afterwards will be performed on those profiles
     ##################################################################################################
     
     #%%%% Activating
     gen_dic['spec_1D_Intr'] = False
     
     
@@ -3198,14 +3210,15 @@
     #%%%%% Fitting mode 
     #    - chi2 or MCMC
     data_dic['Intr']['fit_mode']='chi2'
     
     
     #%%%%% Printing fits results
     data_dic['Intr']['verbose'] = False  
+    data_dic['Intr']['print_par'] = False  
     
     
     #%%%%% Monitor MCMC
     data_dic['Intr']['progress']= True
     
         
     #%%%%% Priors on variable properties
@@ -3295,14 +3308,21 @@
     
     #%%%% Activating 
     gen_dic['fit_IntrProp'] = False
     
     
     #%%%% Multi-threading
     glob_fit_dic['IntrProp']['nthreads'] = int(0.8*cpu_count())
+
+    
+    #%%%%% Unthreaded operations
+    #    - all operations are multi-threaded by default, but overheads of sharing data between threads may counterbalance the benefits of threading the model
+    #    - select here which operations not to thread:
+    # + 'emcee'
+    glob_fit_dic['IntrProp']['unthreaded_op'] = []  
     
     
     #%%%% Fitted data
     
     #%%%%% Exposures to be fitted
     #    - indexes are relative to in-transit tables
     #    - define instruments and visits to be fitted (they will not be fitted if not used as keys, or if set to [], which is the default value), set their value to 'all' for all in-transit exposures to be fitted
@@ -3349,15 +3369,16 @@
     #%%%%% Fitting mode 
     #    - 'chi2', 'mcmc', ''
     glob_fit_dic['IntrProp']['fit_mode']='chi2'  
     
     
     #%%%%% Printing fits results
     glob_fit_dic['IntrProp']['verbose'] = False
-
+    glob_fit_dic['IntrProp']['print_par'] = True
+    
 
     #%%%%% Monitor MCMC
     glob_fit_dic['IntrProp']['progress']= True
     
     
     #%%%%% Priors on variable properties
     #    - see gen_dic['fit_DI'] for details
@@ -3432,202 +3453,233 @@
         
         
         
         
         
         
     ##################################################################################################       
-    #%%% Module: fitting joined residual profiles    
+    #%%% Module: fitting joined differential profiles    
+    #    - fitting joined differential profiles from combined (unbinned) instruments and visits 
+    #    - structure is similar to the joined intrinsic profiles fit
+    #    - fits are performed on all in-transit and out-transit exposures
+    #    - allows including spot properties (latitude, size, Tcenter, flux level) in the fitted properties
     ##################################################################################################     
             
     #%%%% Activating 
     gen_dic['fit_ResProf'] = False        
  
-    ##### RECODER
     
-        # '''
-        # Fitting joined residual stellar profiles from combined (unbinned) instruments and visits 
-        #     - structure is similar to the joined intrinsic profiles fit
-        #     - fits are performed on all in-transit and out-transit exposures
-        #     - allows including spot properties (latitude, size, Tcenter, flux level) in the fitted properties
-            
-        # '''  
-        # 
+    #%%%% Multi-threading
     
-        #Activating 
-        #gen_dic['fit_ResProf'] = True  &  False
+    #%%%%% Allocated threads
+    glob_fit_dic['ResProf']['nthreads'] = int(0.8*cpu_count())
     
-        # #Indexes of exposures to be fitted, in each visit
-        # #    - define instruments and visits to be fitted (they will not be fitted if not used as keys, or if set to []), set their value to 'all' for all in-transit exposures to be fitted
-        # if gen_dic['star_name'] == 'V1298tau' :        
-        #     glob_fit_dic['ResProf']['idx_in_fit']={'HARPN':{'mock_vis': range(40,50)}} 
-        
     
-        # #Model line
-        # #    - specific to the instrument
-        # if gen_dic['star_name'] == 'V1298tau' :
-        #     glob_fit_dic['ResProf']['func_prof_name']={'HARPN':'gauss'}
+    #%%%%% Unthreaded operations
+    #    - all operations are multi-threaded by default, but overheads of sharing data between threads may counterbalance the benefits of threading the model
+    #    - select here which operations not to thread:
+    # + 'emcee'
+    # + 'prof_grid'
+    glob_fit_dic['ResProf']['unthreaded_op'] = []
     
     
-        # #Fit coordinate for the line properties : mu or r_proj
-        # glob_fit_dic['ResProf']['dim_fit']='mu'
+    #%%%% Fitted data
     
+    #%%%%% Exposures to be fitted
+    #    - indexes are relative to in-transit tables
+    #    - define instruments and visits to be fitted (they will not be fitted if not used as keys, or if set to []), set their value to 'all' for all in-transit exposures to be fitted
+    #    - add '_bin' at the end of a visit name for its binned exposures to be fitted instead of the original ones (must have been calculated with the binning module)
+    #      all other mentions of the visit (eg in parameter names) can still refer to the original visit name
+    glob_fit_dic['ResProf']['idx_in_fit']={}
     
-        # #Define fitted range
-        # glob_fit_dic['ResProf']['fit_range'] = {}
-        # if gen_dic['star_name']=='V1298tau':
-        #     fit_range = [[-30,30]] 
-        #     glob_fit_dic['ResProf']['fit_range']['HARPN']={'mock_vis':fit_range} 
     
+    #%%%% Master out data
+
+    #%%%%% Exposures to be used in the calculation of the master-out
+    glob_fit_dic['ResProf']['idx_in_master_out']={}
+
+
+    #%%%%% Common table on which we want to define the master-out
+    #     - Define the borders and the number of points of the table (e.g. [low_end, high_end, num_pts].
+    glob_fit_dic['ResProf']['master_out_tab']=[]
+
+
+    #%%%%% Reference planet
+    #     - Choosing which planet to use as the reference
+    glob_fit_dic['ResProf']['ref_pl']={}
+
+
+    #%%%%% Trimming
+    glob_fit_dic['ResProf']['trim_range'] = {}
     
-        # #Fit mode
-        # #    - 'chi2', 'mcmc', or ''
-        # glob_fit_dic['ResProf']['fit_mode']='mcmc' 
     
+    #%%%%% Order to be fitted
+    glob_fit_dic['ResProf']['order']={}  
     
     
+    #%%%%% Continuum range
+    glob_fit_dic['ResProf']['cont_range'] = {}
+    
+                      
+    #%%%%% Spectral range(s) to be fitted
+    glob_fit_dic['ResProf']['fit_range'] = {}
     
-        # #Fit line property as absolute ('abs') or modulated ('modul') polynomial        
-        # glob_fit_dic['ResProf']['pol_mode']='abs'  
-            
-        # #Model properties
-        # #    - we define here coefficients specific to the line model:
-        # # + polynomial coefficients to describe the line contrast and FWHM (km/s) variations with a chosen dimension
-        # # + core/lobe relations for double-gaussian models
-        # #    - properties names must be defined as 'prop__ISinst_VSvis'  
-        # # + 'inst' is the name of the instrument, which should be set to '_' for the property to be common to all instruments and their visits
-        # # + 'vis' is the name of the visit, which should be set to '_' for the property to be common to all visits of this instrument
-        # # + the properties set here define the lines before instrumental convolution, which is then applied automatically for each instrument 
-        # glob_fit_dic['ResProf']['mod_prop']={}
-        
-        
-        
     
-                                          
+    #%%%% Line profile model         
         
-        # if gen_dic['star_name']=='V1298tau' :
-        #     bjd_obs = 2458877.6306
-        #     bjd_sp1 = 2458877.6306 - 12/24
-        #     bjd_sp2 = 2458877.6306 +  5/24
+    #%%%%% Transition wavelength
+    glob_fit_dic['ResProf']['line_trans']=None        
     
     
-        #     glob_fit_dic['ResProf']['mod_prop']={'veq':{'vary':True,'guess':23.,'bd':[23,24],'physical':True},
-        #                                 'lambda_rad__plV1298tau_b':{'vary':True,'guess':0,'bd':[-np.pi , np.pi], 'physical':True},           
-        #                                 'ctrst_ord0__ISHARPN_VSmock_vis':{'vary':True ,'guess':0.7,'bd':[0,1]},   
-        #                                 'FWHM_ord0__ISHARPN_VSmock_vis': {'vary':True ,'guess':4, 'bd':[0.,10.]}, 
-                    
-        #                                 # # Pour le spot 'spot1' : 
-        #                                 # 'lat__ISHARPN_VSmock_vis_SPspot1'     : {'vary':True ,'guess':30,       'bd' : [-80,80]},
-        #                                 # 'Tcenter__ISHARPN_VSmock_vis_SPspot1' : {'vary':True ,'guess':bjd_sp1, 'bd' : [bjd_sp1-1/3, bjd_sp1+1/3]},
-        #                                 # 'ang__ISHARPN_VSmock_vis_SPspot1'     : {'vary':True ,'guess':20,      'bd' : [10,30]},
-        #                                 # 'flux__ISHARPN_VSmock_vis_SPspot1'    : {'vary':True ,'guess':0.4,     'bd' : [0,1]},
-        #                                 # 
-        #                                 # # Pour le spot 'spot2' : 
-        #                                 # 'lat__ISHARPN_VSmock_vis_SPspot2'     : {'vary':True ,'guess':40,       'bd' : [-80,80]},
-        #                                 # 'Tcenter__ISHARPN_VSmock_vis_SPspot2' : {'vary':True ,'guess':bjd_sp2, 'bd' : [bjd_sp2-1/3, bjd_sp2+1/3]},
-        #                                 # 'ang__ISHARPN_VSmock_vis_SPspot2'     : {'vary':True ,'guess':25,      'bd' : [10,30]},
-        #                                 # 'flux__ISHARPN_VSmock_vis_SPspot2'    : {'vary':True ,'guess':0.4,     'bd' : [0,1]},
-        #                                    }
-                                           
-                    
+    #%%%%% Model type
+    glob_fit_dic['ResProf']['mode'] = 'ana' 
+    
+     
+    #%%%%% Analytical profile
+    #    - default: 'gauss' 
+    glob_fit_dic['ResProf']['func_prof_name'] = {}
     
-        # #------------------------------------------
-        # #MCMC options
-        # #------------------------------------------
         
-        # #Run mcmc or retrieve results
-        # glob_fit_dic['ResProf']['mcmc_run_mode']='use'   # reuse
+    #%%%%% Analytical profile coordinate
+    #    - fit coordinate for the line properties of analytical profiles
+    #    - see possibilities in gen_dic['fit_IntrProp']
+    glob_fit_dic['ResProf']['dim_fit']='mu'
     
     
+    #%%%%% Analytical profile variation
+    #    - fit line property as absolute ('abs') or modulated ('modul') polynomial        
+    glob_fit_dic['ResProf']['pol_mode']='abs'  
     
     
-        # #Walkers settings 
-        # glob_fit_dic['ResProf']['mcmc_set']={}
+    #%%%%% Fixed/variable properties
+    #    - structure is the same as glob_fit_dic['IntrProp']['mod_prop']
+    #    - intrinsic properties define the lines before instrumental convolution, which can then be applied specifically to each instrument  
+    glob_fit_dic['ResProf']['mod_prop']={}
+                 
+    
+    #%%%%% PC noise model
+    #    - indicate for each visit:
+    # + the path to the PC matrix, already reduced to the PC requested to correct the visit in the PCA module
+    #   beware that the correction will be applied only over the range of definition of the PC set in the PCA
+    #   beware that one PC adds the number of fitted intrinsic profiles to the free parameters of the joint fit
+    # + whether to account or not (idx_out = []) for the PCA fit in the calculation of the fit merit values, using all out exposures (idx_out = 'all') or a selection
+    # + set noPC = True to account for the chi2 of the null hypothesis (no noise) on the out-of-transit data, without including PC to the RMR fit
+    glob_fit_dic['ResProf']['PC_model']={}  
+
+
+    #%%%%% Optimization levels
+    # + Level -1: nothing is turned on/off. In this default case multithreading is controlled by the number of threads provided by the user, un-optimized profile building is used
+    # and over-simplified grid building is not used.
+    # + Level 0: multithreading activated (AND Optimized profile building)
+    # + Level 1: multithreading turned off (AND Optimized profile building)
+    # + Level 2: multithreading turned off AND over-simplified grid building (AND Optimized profile building)
+    # + Level 3: multithreading turned off AND over-simplified grid building AND grid building function coded in C (AND Optimized profile building)
+    #
+    # - Optimized profile building (always turned on): We generate residual profiles by initially constructing profiles for each exposure. Each exposure's profile is built by removing the deviations 
+    # caused by spotted and occulted regions from the base disk-integrated profile. Subsequently, we create a master-out profile and subtract each exposure's profile from it to obtain 
+    # the residual profiles. To expedite this process, cells that are never spotted or occulted are identified and excluded from profile construction, resulting in faster model processing.
+    #
+    # - Over-simplified grid building: Instead of assigning complex profiles to individual cells and summing them for the entire disk, we now use Gaussian profiles for each cell. 
+    # Additionally, we optimize performance by representing the grid of profiles as an array rather than a list.
+    glob_fit_dic['ResProf']['Opt_Lvl']=-1
+    
+    
+    #%%%% Fit settings 
         
-        # if gen_dic['star_name'] == 'V1298tau':
-        #     glob_fit_dic['ResProf']['mcmc_set']={'nwalkers':20,'nsteps':1,'nburn':0}          
+    #%%%%% Fitting mode
+    #    - 'chi2', 'mcmc', or ''
+    glob_fit_dic['ResProf']['fit_mode']='' 
     
     
-            
-        # #Priors on variable model parameters
-        # #    - see gen_dic['fit_DI'] for details
-        # glob_fit_dic['ResProf']['priors']={}
-        # if gen_dic['star_name'] == 'V1298tau' :
-        #     bjd_obs = 2458877.6306
-        #     bjd_sp1 = 2458877.6306 - 12/24
-        #     bjd_sp2 = 2458877.6306 +  5/24
-    
-        #     glob_fit_dic['ResProf']['priors'].update({
-        #         'veq':{'mod':'uf','low':23.,'high':24.},    
-        #         'lambda_rad__plV1298tau_b':{'mod':'uf','low':-np.pi,'high':np.pi},       
-        #         'FWHM_ord0__ISHARPN_VSmock_vis':{'mod':'uf','low':0.,'high':10.},
-        #         'ctrst_ord0__ISHARPN_VSmock_vis':{'mod':'uf','low':0.,'high':1.},
-                    
-        #         # # Pour le spot 'spot1' : 
-        #         # 'lat__ISHARPN_VSmock_vis_SPspot1'     : {'mod':'uf' , 'low':-80,              'high':80},
-        #         # 'Tcenter__ISHARPN_VSmock_vis_SPspot1' : {'mod':'uf' , 'low':bjd_sp1-1/3,      'high':bjd_sp1+1/3},
-        #         # 'ang__ISHARPN_VSmock_vis_SPspot1'     : {'mod':'uf' , 'low':10,               'high':30},
-        #         # 'flux__ISHARPN_VSmock_vis_SPspot1'    : {'mod':'uf' , 'low':0,                'high':1},
-        #         # 
-        #         # # Pour le spot 'spot2' : 
-        #         # 'lat__ISHARPN_VSmock_vis_SPspot2'     : {'mod':'uf' , 'low':-80,           'high':80},
-        #         # 'Tcenter__ISHARPN_VSmock_vis_SPspot2' : {'mod':'uf' , 'low': bjd_sp2-1/3,  'high': bjd_sp2 + 1/3},
-        #         # 'ang__ISHARPN_VSmock_vis_SPspot2'     : {'mod':'uf' , 'low':10,            'high':30},
-        #         # 'flux__ISHARPN_VSmock_vis_SPspot2'    : {'mod':'uf' , 'low':0,             'high':1},
-                
-                                        
-        #                                 })
+    #%%%%% Printing fits results
+    glob_fit_dic['ResProf']['verbose']= False
+    glob_fit_dic['ResProf']['print_par'] = True
+    
+    
+    #%%%%% Priors on variable properties
+    #    - see gen_dic['fit_DI'] for details
+    glob_fit_dic['ResProf']['priors']={}
+
+
+    #%%%%% Derived properties
+    #    - each field calls a specific function (see routine for more details)
+    glob_fit_dic['ResProf']['deriv_prop'] = []
+    
+    
+    #%%%%% MCMC settings
     
+    #%%%%%% Calculating/retrieving
+    glob_fit_dic['ResProf']['mcmc_run_mode']='use'
+    
+    
+    #%%%%%% Runs to re-use
+    #    - list of mcmc runs to reuse
+    #    - if 'reuse' is requested, leave empty to automatically retrieve the mcmc run available in the default directory
+    #  or set the list of mcmc runs to retrieve (they must have been run with the same settings, but the burnin can be specified for each run)
+    glob_fit_dic['ResProf']['mcmc_reuse']={} 
     
     
+    #%%%%%% Runs to re-start
+    #    - indicate path to a 'raw_chains' file
+    #      the mcmc will restart the same walkers from their last step, and run from the number of steps indicated in 'mcmc_set'
+    glob_fit_dic['ResProf']['mcmc_reboot']=''
     
     
+    #%%%%%% Walkers
+    glob_fit_dic['ResProf']['mcmc_set']={}
     
     
+    #%%%%%% Complex priors
+    glob_fit_dic['ResProf']['prior_func']={}     
     
         
-        # #Use complex prior function
-        # glob_fit_dic['ResProf']['prior_func']={}        
+    #%%%%%% Walkers exclusion  
+    #    - define conditions within routine
+    glob_fit_dic['ResProf']['exclu_walk']=False       
     
-        # #Excluding manually some of the walkers
-        # #    - define conditions within routine
-        # glob_fit_dic['ResProf']['exclu_walk']=True   & False       
     
-        # #Automatic exclusion of outlying chains
-        # #    - set to None, or exclusion threshold
-        # glob_fit_dic['ResProf']['exclu_walk_autom']=None  #  5.
+    #%%%%%% Automatic exclusion of outlying chains
+    #    - set to None, or exclusion threshold
+    glob_fit_dic['ResProf']['exclu_walk_autom']=None  
     
-        # #Define lower/upper limits to be calculated
-        # # glob_fit_dic['ResProf']['conf_limits']={'ecc_pl1':{'bound':0.,'type':'upper','level':['1s','3s']}} 
     
-        # #Plot chains for MCMC parameters
-        # glob_fit_dic['ResProf']['save_MCMC_chains']='png'   #png  
+    #%%%%%% Derived errors
+    #    - 'quant' or 'HDI'
+    glob_fit_dic['ResProf']['out_err_mode']='HDI'
+    glob_fit_dic['ResProf']['HDI']='1s'
     
-        # #Choose list of modifications to be made to the final chains 
-        # #    - each field calls a specific function (see routine for more details)
-        # glob_fit_dic['ResProf']['deriv_prop'] = ['vsini','lambda_deg']
     
-        # #Define HDI interval to be calculated 
-        # glob_fit_dic['ResProf']['HDI']='1s'   #None   #'3s'   
+    #%%%%%% Derived lower/upper limits
+    glob_fit_dic['ResProf']['conf_limits']={}
     
     
+    #%%%% Plot settings
     
-        
-        # #Options for corner plot
-        # #    - see function for options
-        # glob_fit_dic['ResProf']['corner_options']={
-        #     'plot_HDI':True , 
-        #     'plot1s_1D':False,
-        #     'color_levels':['deepskyblue','lime'],
-        #     'fontsize':8,
-        #     }    
+    #%%%%% MCMC chains
+    glob_fit_dic['ResProf']['save_MCMC_chains']=''  
+    
+    
+    #%%%%% MCMC corner plot
+    #    - see function for options
+    glob_fit_dic['ResProf']['corner_options']={}      
+
+    
+    #%%%% Plot settings
+            
+    #%%%%% Plot best-fit 2D residual map
+    glob_fit_dic['ResProf']['map_Res_prof']=''
+
+
+    #%%%%% Plot best-fit 2D residual map
+    plot_dic['map_BF_Res_prof']=''   
     
     
-        # #Print on-screen fit information
-        # glob_fit_dic['ResProf']['verbose']=True  &  False
+    #%%%%% 2D maps : Plot residuals from best-fit 2D residual map
+    plot_dic['map_BF_Res_prof_re']='' 
+
     
     
         
         
         
         
         
@@ -3750,14 +3802,15 @@
     #%%%%% Fitting mode
     #    - 'chi2', 'mcmc', or ''
     glob_fit_dic['IntrProf']['fit_mode']='chi2' 
     
     
     #%%%%% Printing fits results
     glob_fit_dic['IntrProf']['verbose']= False
+    glob_fit_dic['IntrProf']['print_par'] = True
 
     
     #%%%%% Monitor MCMC
     glob_fit_dic['IntrProf']['progress']= True
     
     
     #%%%%% Priors on variable properties
@@ -3881,14 +3934,15 @@
     # + see possible bin dimensions in data_dic['Intr']['dim_bin']  
     # + see possible bin table definition in data_dic['Intr']['prop_bin']
     # > 'glob_mod': models derived from global fit to intrinsic profiles (default)
     # + 'mode' : 'ana' or 'theo'
     # + can be specific to the visit or common to all, depending on the fit
     # + line coordinate choice is retrieved automatically 
     # + indicate path to saved properties determining the line property variations in the processed dataset
+    #   bulk system properties will be retrieved and used if fitted
     # + default options are used if left undefined
     # > 'indiv_mod': models fitted to each individual intrinsic profile in each visit
     # + 'mode' : 'ana' or 'theo'
     # + works only in exposures where the stellar line could be fitted after planet exclusion
     # > 'rec_prof':
     # + define each undefined pixel via a polynomial fit to defined pixels in complementary exposures
     #   or via a 2D interpolation ('linear' or 'cubic') over complementary exposures and a narrow spectral band (defined in band_pix_hw pixels on each side of undefined pixels)
@@ -3912,14 +3966,32 @@
     plot_dic['map_Intr_prof_res']=''   
     
    
         
         
         
         
+    ##################################################################################################       
+    #%%% Module: estimates for differential profiles 
+    ##################################################################################################     
+    
+    #%%%% Activating
+    #    - for original and binned exposures in each visit
+    gen_dic['diff_data_corr'] = False        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
         
         
         
         
         
     
     ##################################################################################################
@@ -4279,14 +4351,15 @@
     #%%%%% Fitting mode 
     #    - chi2 or MCMC
     data_dic['Atm']['fit_mode']='chi2'
     
     
     #%%%%% Printing fits results
     data_dic['Atm']['verbose'] = False  
+    data_dic['Atm']['print_par'] = True
     
     
     #%%%%% Monitor MCMC
     data_dic['Atm']['progress']= True
     
         
     #%%%%% Priors on variable properties
@@ -4405,14 +4478,15 @@
     #%%%%% Fitting mode 
     #    - 'chi2', 'mcmc', ''
     glob_fit_dic['AtmProp']['fit_mode']='chi2'  
     
     
     #%%%%% Printing fits results
     glob_fit_dic['AtmProp']['verbose'] = False
+    glob_fit_dic['AtmProp']['print_par'] = True
     
     
     #%%%%% Monitor MCMC
     glob_fit_dic['AtmProp']['progress']= True
     
         
     #%%%%% Priors on variable properties
@@ -4556,14 +4630,15 @@
     #%%%%% Fitting mode
     #    - 'chi2', 'mcmc', or ''
     glob_fit_dic['AtmProf']['fit_mode']='chi2' 
     
     
     #%%%%% Printing fits results
     glob_fit_dic['AtmProf']['verbose']= False
+    glob_fit_dic['AtmProf']['print_par'] = True
 
     
     #%%%%% Monitor MCMC
     glob_fit_dic['AtmProf']['progress']= True
     
     
     #%%%%% Priors on variable properties
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_launch/ANTARESS_systems.py` & `antaress-1.1.1/src/antaress/ANTARESS_launch/ANTARESS_systems.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_plots/ANTARESS_plot_settings.py` & `antaress-1.1.1/src/antaress/ANTARESS_plots/ANTARESS_plot_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import numpy as np
 from copy import deepcopy
-from ..ANTARESS_general.utils import stop
+from antaress.ANTARESS_general.utils import stop
 
 def gen_plot_default(plot_options,key_plot,plot_dic,gen_dic):
     r"""**Default plot settings.**
     
     Set default values for the following fields. 
     Manual values can be given to all fields through `ANTARESS_plot_settings.py`, depending on their relevance for the chosen plot function. 
     
@@ -278,22 +278,26 @@
         
     #--------------------------------------              
     if (key_plot in ['Fbal_corr','input_LC','plocc_ranges','prop_DI_mcmc_PDFs','prop_Intr_mcmc_PDFs']):
 
         #Plot exposure indexes
         plot_options[key_plot]['plot_expid'] = True
         
-    #--------------------------------------        
+    #--------------------------------------   
+    #2D map settings     
     if ('map_' in key_plot) or ('bin' in key_plot) or ('prop_' in key_plot) or (key_plot in ['occulted_regions']):
 
         #Bin dimension
         #    - 'phase' (see details and routine)
         #    - coordinates are only available if binning was performed over 'phase'
         plot_options[key_plot]['dim_plot']='phase' 
 
+        #Print information
+        plot_options[key_plot]['verbose']=True 
+
     #--------------------------------------   
     if ('prop_' in key_plot):
 
         #Abscissa
         plot_options[key_plot]['prop_DI_absc']='phase'                
         plot_options[key_plot]['prop_Intr_absc']='phase'
         
@@ -1658,15 +1662,15 @@
     ##################################################################################################
     for key_plot in ['map_Intr_prof_est','map_Intr_prof_res']:
         if plot_dic[key_plot]!='':
 
             #%%%%% Generic settings
             plot_settings=gen_plot_default(plot_settings,key_plot,plot_dic,gen_dic) 
 
-            #%%%%% Mode to retrieve
+            #%%%%% Model to retrieve
             plot_settings[key_plot]['mode_loc_data_corr'] = 'glob_mod'
 
             ##############################################################################
             #%%%%% Estimates
             if key_plot=='map_Intr_prof_est':
 
                 #%%%%%% Model always required
@@ -1682,17 +1686,14 @@
                 #%%%%%% Correct only for continuum level
                 plot_settings[key_plot]['cont_only']=True
                 plot_settings[key_plot]['plot_line_model'] = False
                 plot_settings[key_plot]['st_cont']=None
                 
         
 
-
-
-
  
     ################################################################################################################ 
     #%%%% PC-based noise model 
     ################################################################################################################   
     if (plot_dic['map_pca_prof']!=''):
         key_plot = 'map_pca_prof'
 
@@ -2174,18 +2175,18 @@
         plot_settings[key_plot]['plot_stspin_hid']=  False
         
         #%%%% Plot stellar spin
         plot_settings[key_plot]['plot_stspin']=True 
         
         #%%%% Plot stellar poles
         plot_settings[key_plot]['plot_poles']=True  
-        plot_settings[key_plot]['plot_hidden_pole']= False  
-
+        plot_settings[key_plot]['plot_hidden_pole']= False 
+        
         #%%%% Plot stellar spots
-        plot_settings[key_plot]['stellar_spot'] = {}
+        plot_settings[key_plot]['plot_spots'] = False
         
         #%%%% Number of positions of the spots to be plotted, equally distributed within the given time range.
         plot_settings[key_plot]['n_image_spots'] = 15
 
         #%%%% Use stellar rotation period to distribute the positions, instead of time
         plot_settings[key_plot]['plot_spot_all_Peq'] = True
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_plots/ANTARESS_plots_all.py` & `antaress-1.1.1/src/antaress/ANTARESS_plots/ANTARESS_plots_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 import copy
 from astropy.io import fits
 import glob
 import imageio
 from ..ANTARESS_general.constant_data import c_light
 from ..ANTARESS_general.minim_routines import call_lmfit
 from ..ANTARESS_general.utils import closest,stop,np_where1D,closest_Ndim,np_interp,init_parallel_func,is_odd,dataload_npz,air_index,gen_specdopshift,import_module
-from ..ANTARESS_plots.utils_plots import custom_axis,autom_x_tick_prop,autom_y_tick_prop,stackrel,scaled_title,autom_range_ext,plot_shade_range
+from ..ANTARESS_plots.utils_plots import custom_axis,autom_tick_prop,stackrel,scaled_title,autom_range_ext,plot_shade_range
 from ..ANTARESS_conversions.ANTARESS_binning import resample_func,calc_bin_prof,weights_bin_prof
 from ..ANTARESS_analysis.ANTARESS_inst_resp import calc_FWHM_inst,return_pix_size
 from ..ANTARESS_analysis.ANTARESS_model_prof import gauss_intr_prop,dgauss,cust_mod_true_prop,voigt
 from ..ANTARESS_corrections.ANTARESS_detrend import detrend_prof_gen
 from ..ANTARESS_corrections.ANTARESS_interferences import def_wig_tab,calc_chrom_coord,calc_wig_mod_nu_t
 from ..ANTARESS_grids.ANTARESS_coord import calc_pl_coord_plots,calc_pl_coord,calc_rv_star_HR,frameconv_skyorb_to_skystar,frameconv_skystar_to_skyorb,get_timeorbit,\
     calc_zLOS_oblate,frameconv_star_to_skystar,calc_tr_contacts
 from ..ANTARESS_corrections.ANTARESS_calib import cal_piecewise_func
 from ..ANTARESS_grids.ANTARESS_star_grid import get_LD_coeff,calc_CB_RV,calc_RVrot,calc_Isurf_grid,calc_st_sky
-from ..ANTARESS_grids.ANTARESS_plocc_grid import occ_region_grid,sub_calc_plocc_spot_prop
-from ..ANTARESS_grids.ANTARESS_spots import retrieve_spots_prop_from_param, calc_spotted_tiles, spot_occ_region_grid
+from ..ANTARESS_grids.ANTARESS_occ_grid import occ_region_grid,sub_calc_plocc_spot_prop,retrieve_spots_prop_from_param, calc_spotted_tiles
 
 
 def ANTARESS_plot_functions(system_param,plot_dic,data_dic,gen_dic,coord_dic,theo_dic,data_prop,glob_fit_dic,mock_dic,nbook_dic,custom_plot_settings):
     print()
     print('-----------------------------------')
     print('Plots')  
     print('-----------------------------------')
@@ -76,16 +75,16 @@
     '''
     if (plot_dic['occulted_regions']!='') or any('map_' in key for key in list(plot_dic.keys())) or (plot_dic['prop_Intr']!='') or (plot_dic['prop_DI']!='') or (plot_dic['input_LC']!='') or (plot_dic['pca_ana']!=''): 
 
         #Contacts
         contact_phases={}
         for pl_loc in gen_dic['studied_pl']:
             contact_phases[pl_loc]=calc_tr_contacts(data_dic['DI']['system_prop']['achrom'][pl_loc][0],system_param[pl_loc],plot_dic['stend_ph'],system_param['star'])
-            T14_pl = (contact_phases[pl_loc][3]-contact_phases[pl_loc][0])*system_param[pl_loc]['period']
-            print('Numerical T14['+str(pl_loc)+']='+"{0:.6f}".format(T14_pl*24.)+' h')                  
+            system_param[pl_loc]['T14_num'] = (contact_phases[pl_loc][3]-contact_phases[pl_loc][0])*system_param[pl_loc]['period']
+            print('Numerical T14['+str(pl_loc)+']='+"{0:.6f}".format(system_param[pl_loc]['T14_num']*24.)+' h')                  
 
             #Stellar mass derived from orbital motion of main planets
             print('Numerical Kp_orb='+"{0:.2f}".format(system_param[pl_loc]['Kp_orb'])+' km/s (Mstar = '+"{0:.3f}".format(system_param[pl_loc]['Mstar_orb'])+' Msun)')  
     
         #Function to calculate coordinates of planets and occulted regions in a given visit
         #    - in achromatic mode
         def calc_occ_plot(data_bin,theo_dic_loc,inst,vis,genpar_instvis,param_loc,args,system_param_loc,iband=0,par_list = ['rv','CB_RV','mu','xp_abs','r_proj','y_st','lat']):
@@ -141,15 +140,15 @@
             bjd_HR = bjd_HR[cond_occ_HR]
             args['inst'] = inst
             args['vis'] = vis
             for pl_loc in gen_dic['studied_pl']:
                 coord_pl_in[pl_loc]['cen_pos'] = coord_pl_in[pl_loc]['cen_pos'][:,cond_occ_HR]
                 coord_pl_in[pl_loc]['phase'] = coord_pl_in[pl_loc]['phase'][cond_occ_HR]     
                 coord_pl_in[pl_loc]['ecl'] = coord_pl_in[pl_loc]['ecl'][cond_occ_HR] 
-            surf_prop_dic, surf_prop_dic_spot = sub_calc_plocc_spot_prop(['achrom'],args,par_list,gen_dic['studied_pl'],system_param_loc,theo_dic_loc,system_prop_loc,param_loc,coord_pl_in,range(coord_pl_in['nph_HR']))
+            surf_prop_dic, surf_prop_dic_spot, surf_prop_dic_common = sub_calc_plocc_spot_prop(['achrom'],args,par_list,gen_dic['studied_pl'],system_param_loc,theo_dic_loc,system_prop_loc,param_loc,coord_pl_in,range(coord_pl_in['nph_HR']))
             theo_HR_prop_plocc = surf_prop_dic['achrom']
             theo_HR_prop_plocc['nph_HR'] = coord_pl_in['nph_HR']
             for pl_loc in gen_dic['studied_pl']:
                 theo_HR_prop_plocc[pl_loc].update(coord_pl_in[pl_loc])
                 
                 #Reduce to chosen band
                 cond_def_HR = ~np.isnan(theo_HR_prop_plocc[pl_loc]['Ftot'][iband])
@@ -339,17 +338,24 @@
                 None
             
             """            
            
             #Options
             sc_fact=10**plot_options['sc_fact10']            
 
+            if plot_mod in ['map_Res_prof_clean_pl_est','map_Res_prof_clean_sp_est','map_Res_prof_unclean_sp_est','map_Res_prof_unclean_pl_est',
+                        'map_Res_prof_clean_sp_res','map_Res_prof_clean_pl_res','map_Res_prof_unclean_sp_res','map_Res_prof_unclean_pl_res']:
+        
+                #Defining whether we are plotting the planet-occulted or spotted profiles and if they are clean or uncleaned
+                supp_name = plot_mod.split('_')[4]
+                corr_plot_mod = plot_mod.split('_')[3]
+
             #Plotting separate visits on different plots because of the possible overlap between exposures
             for inst in np.intersect1d(data_dic['instrum_list'],list(plot_options['visits_to_plot'].keys())):             
-                print('      - Instrument :',inst)
+                print('   - Instrument :',inst)
     
                 #Data to plot
                 maink_list = []
                 data_list = []
                 plot_options['plot_pre']=None
                 maink_list=['post']
                 data_list=['all']     
@@ -364,15 +370,15 @@
                 data_type_gen,data_mode,data_type,add_txt_path,txt_aligned=sub_plot_prof_init(plot_mod,plot_options,inst)        
 
                 #Frame properties
                 title_name=''   
 
                 #Plot for each visit
                 for ivis,vis in enumerate(np.intersect1d(list(data_dic[inst].keys())+['binned'],plot_options['visits_to_plot'][inst])):                 
-                    print('        - Visit :',vis)
+                    print('     - Visit :',vis)
                     data_inst=data_dic[inst]
                     data_vis = data_inst[vis]
                     
                     #Data
                     # data_com = dataload_npz(data_vis['proc_com_data_paths'])   
                     fixed_args_loc = {}
                     pl_ref,txt_conv,iexp_plot,iexp_orig,prof_fit_vis,fit_results,data_path_all,rest_frame,data_path_dic,nexp_plot,inout_flag,path_loc,iexp_mast_list,nord_data,data_bin = sub_plot_prof_dir(inst,vis,plot_options,data_mode,'Map',add_txt_path,plot_mod,txt_aligned,data_type,data_type_gen)
@@ -474,15 +480,39 @@
                         if (plot_mod=='map_pca_prof'):
                             var_map[isub] = data_exp['flux']*sc_fact
                             cond_def_map[isub] = ~np.isnan(var_map[isub])   
                             
                         #Data
                         else:     
                             
-                            if plot_mod in ['map_Intr_prof_est','map_Intr_prof_res']: 
+                            if plot_mod in ['map_Res_prof_clean_pl_est','map_Res_prof_clean_sp_est','map_Res_prof_unclean_sp_est','map_Res_prof_unclean_pl_est',
+                                            'map_Res_prof_clean_sp_res','map_Res_prof_clean_pl_res','map_Res_prof_unclean_sp_res','map_Res_prof_unclean_pl_res']:
+                                
+                                cond_def_map[isub] = data_exp['cond_def']
+                                #Retrieving flux for these regions
+                                if '_est' in plot_mod:
+                                    var_map[isub] = data_exp[corr_plot_mod+'_'+supp_name+'_flux'] 
+                                #Building residuals
+                                elif '_res' in plot_mod:
+                                    data_exp_est = dataload_npz(gen_dic['save_data_dir']+'Spot_Loc_estimates/'+plot_options['mode_loc_data_corr']+'/'+inst+'_'+vis+'_'+str(iexp)) 
+                                    var_map[isub] = data_exp['flux'] - data_exp_est[corr_plot_mod+'_'+supp_name+'_flux']
+                            
+                            elif plot_mod in ['map_BF_Res_prof', 'map_BF_Res_prof_re']:
+                                cond_def_map[isub] = data_exp['cond_def_fit']
+                                
+                                flux_2_use = data_exp['flux']
+                                if plot_mod == 'map_BF_Res_prof_re':
+                                    raw_prof_loc = gen_dic['save_data_dir']+'Res_data/'+inst+'_'+vis+'_'+str(iexp)
+                                    raw_prof = dataload_npz(raw_prof_loc)
+                                    flux_2_use -= raw_prof['flux']
+                                
+                                var_map[isub] = flux_2_use
+                            
+                            elif plot_mod in ['map_Intr_prof_est','map_Intr_prof_res']: 
+
 
                                 #Check that model exists for in-transit profiles 
                                 if (gen_dic[inst][vis]['idx_exp2in'][iexp_or]==-1.) or \
                                   ((gen_dic[inst][vis]['idx_exp2in'][iexp_or]>-1) and \
                                         (plot_options['cont_only'] or \
                                         ((plot_options['line_model']=='fit') and (iexp in prof_fit_vis)) or \
                                         ((plot_options['line_model']=='rec') and (iexp in prof_fit_vis['idx_est_loc'])))): 
@@ -516,15 +546,15 @@
                                             #Exosure is effectively in-transit
                                             if not data_scaling['null_loc_flux_scaling']:
                                                 if not plot_options['cont_only']:data_exp_est = dataload_npz(gen_dic['save_data_dir']+'Loc_estimates/'+plot_options['mode_loc_data_corr']+'/'+inst+'_'+vis+'_'+str(iexp)) 
                                                 intr_flux_est = np.zeros(dim_exp_proc)*np.nan 
                                                 intr2res_sc = np.zeros(dim_exp_proc)*np.nan 
                                                 for iord in range(nord_proc):
     
-                                                    #Conversion from intrinsic to residual flux levels
+                                                    #Conversion from intrinsic to differential flux levels
                                                     loc_flux_scaling_exp_ord =  data_scaling['loc_flux_scaling'](data_exp['cen_bins'][iord])
                                                     intr2res_sc[iord] = loc_flux_scaling_exp_ord/(1. - loc_flux_scaling_exp_ord)                                                
     
                                                     #Correct for local continuum level only
                                                     if plot_options['cont_only']: 
     
                                                         #Broadband continuum profile
@@ -540,25 +570,25 @@
                                                     #Correct for full local stellar profile
                                                     else:
                                                         
                                                         #Model intrinsic profiles
                                                         if data_dic['Intr']['plocc_prof_type']=='Intr': 
                                                             intr_flux_est[iord] = data_exp_est['flux'][iord]
                                                         
-                                                        #Conversion from model residual to intrinsic profiles
+                                                        #Conversion from model differential to intrinsic profiles
                                                         elif data_dic['Intr']['plocc_prof_type']=='Res':          
                                                             intr_flux_est[iord] = data_exp_est['flux'][iord]/loc_flux_scaling_exp_ord
         
-                                                #Residuals
+                                                #Differential profiles
                                                 var_map[isub] =  (data_exp['flux'] - intr_flux_est)*intr2res_sc
 
                                             #Exosure is effectively out-transit
                                             else:var_map[isub]=data_exp['flux']                                                
                                                 
-                                        #Out-of-transit residual profile
+                                        #Out-of-transit differential profile
                                         else:var_map[isub]=data_exp['flux']
 
                                 #Plot scaling
                                 var_map[isub]*=sc_fact
                                 cond_def_map[isub] = ~np.isnan(var_map[isub])                             
     
                             else:
@@ -614,15 +644,15 @@
                         delta_ordi_tab = high_ordi_tab[0:-1]-low_ordi_tab[1::]
                         for iexp_olap,delta_exp in zip( range(1,nexp_plot),delta_ordi_tab):
                             if delta_exp>0:
                                 low_ordi_tab[iexp_olap::]+=delta_exp
                                 high_ordi_tab[iexp_olap::]+=delta_exp
                                    
                     ordi_range = np.array([np.min(low_ordi_tab),np.max(high_ordi_tab)])
-                    print('      range for '+ordi_name+' table:',"{0:.5f}".format(ordi_range[0]),' ; ',"{0:.5f}".format(ordi_range[1]))
+                    if plot_options['verbose']:print('      range for '+ordi_name+' table:',"{0:.5f}".format(ordi_range[0]),' ; ',"{0:.5f}".format(ordi_range[1]))
                     
                     #Processing each order 
                     for iord in order_list:
 
                         #Data to be plotted
                         low_ordi_tab_loc = deepcopy(low_ordi_tab)
                         high_ordi_tab_loc = deepcopy(high_ordi_tab)
@@ -694,15 +724,15 @@
                                 var_loc/=mean_flux
                              
                             #Automatic ranges detection
                             if (inst in plot_options['v_range_all']) and (vis in plot_options['v_range_all'][inst]) and (plot_options['v_range_all'][inst][vis] is not None):
                                 v_range=np.array(plot_options['v_range_all'][inst][vis])*sc_fact
                             else:
                                 v_range=np.array([np.nanmin(var_loc),np.nanmax(var_loc)])
-                                if data_type == 'CCF':print('      range for color table:',"{0:.5f}".format(v_range[0]),' ; ',"{0:.5f}".format(v_range[1]))
+                                if (data_type == 'CCF') and (plot_options['verbose']):print('      range for color table:',"{0:.5f}".format(v_range[0]),' ; ',"{0:.5f}".format(v_range[1]))
 
                             #Plot data for each exposure   
                             for iexp,(var_exp,low_phase_exp,high_phase_exp) in enumerate(zip(var_loc,low_ordi_tab_loc,high_ordi_tab_loc)):
                                 low_sp_exp=low_sp_loc[iexp]
                                 high_sp_exp = high_sp_loc[iexp]
                                 cond_def_exp = ~np.isnan(var_exp) 
                                 
@@ -863,15 +893,15 @@
                                         doppler_track_plots('surf',line_mask,rest_frame,col_loc,cond_track,cond_range,lw_mod,ls_loc,data_dic[inst][vis]['transit_pl'],pl_ref,theo_HR_prop_plocc_align,line_range,iexp_plot,iexp_range,plot_options['reverse_2D'],data_type,x_range_loc,y_range_loc)
 
                             #------------------------------------  
                                       
                             #Modelled and measured local stellar surface RVs
                             if (data_type == 'CCF'):
     
-                                #Local stellar residual profiles
+                                #Local differential and intrinsic profiles
                                 if (plot_mod in ['map_Res_prof','map_Intr_prof_est','map_Intr_prof_res','map_Intrbin']) or ((plot_mod in ['map_Intr_prof']) and (not plot_options['aligned'])):
                                 
                                     #Model at each exposure                        
                                     if plot_options['plot_theoRV']:
                                         RV_plocc = dataload_npz(gen_dic['save_data_dir']+'Introrig_prop/PlOcc_Prop_'+inst+'_'+vis)['achrom']['rv'][0]
                                         ph_theoRV=np.vstack((coord_dic[inst][vis][pl_ref]['cen_ph'][gen_dic[inst][vis]['idx_in']],RV_plocc))
                                         if plot_options['reverse_2D']:
@@ -929,18 +959,20 @@
                                     i_in=0
                                     for iexp in range(data_dic[inst][vis]['n_in_visit']):
                                         col_face_symb='magenta'  #'black'
                                         col_symb='magenta'
                                         RV_rest = 0.
                                         plot_rv = False
                                         
-                                        #Local stellar residual or atmospheric profiles
+                                        #Local differential profiles
                                         if (plot_mod=='map_Res_prof') and ('prof_fit_dic' in data_dic['Res'][inst][vis]) and (iexp in gen_dic[inst][vis]['idx_in']): 
                                             CCF_fit_loc = data_dic['Res'][inst][vis]['prof_fit_dic'][i_in] 
                                             plot_rv = True
+                                        
+                                        #Local atmospheric profiles
                                         if plot_mod=='map_Atm_prof':
                                             if (data_dic['Atm']['pl_atm_sign']=='Absorption') and (iexp in gen_dic[inst][vis]['idx_in']):CCF_fit_loc = data_dic['Atm'][inst][vis]['prof_fit_dic'][i_in]
                                             if data_dic['Atm']['pl_atm_sign']=='Emission':CCF_fit_loc = data_dic['Atm'][inst][vis]['prof_fit_dic'][iexp]
                                             if (rest_frame=='star'):RV_rest = coord_dic[inst][vis]['rv_pl'][iexp] 
                                             plot_rv = True
                                         if (iexp in gen_dic[inst][vis]['idx_in']):i_in+=1 
                                                                         
@@ -952,16 +984,16 @@
                                             if (plot_options['plot_measRV']=='all') and (not CCF_fit_loc['detected']):col_face_symb='none' 
                                             if plot_options['reverse_2D']:plt.errorbar(ph_loc,RV_loc,yerr=eRV_loc,color=col_symb,linestyle='',markeredgewidth=mew_RV,zorder=15,marker='|',markersize=msize_RV,markerfacecolor=col_face_symb,markeredgecolor=col_symb,elinewidth=1)
                                             else: plt.errorbar(RV_loc,ph_loc,xerr=eRV_loc,color=col_symb,linestyle='',markeredgewidth=mew_RV,zorder=15,marker='|',markersize=msize_RV,markerfacecolor=col_face_symb,markeredgecolor=col_symb,elinewidth=1)
                             
                             #----------------------------------------------
                                         
                             #Plot frame 
-                            xmajor_int,xminor_int,xmajor_form=autom_x_tick_prop(x_range_loc[1]-x_range_loc[0])
-                            ymajor_int,yminor_int,ymajor_form=autom_y_tick_prop(y_range_loc[1]-y_range_loc[0])                        
+                            xmajor_int,xminor_int,xmajor_form=autom_tick_prop(x_range_loc[1]-x_range_loc[0])
+                            ymajor_int,yminor_int,ymajor_form=autom_tick_prop(y_range_loc[1]-y_range_loc[0])                        
     
                             #Suppress ticks if exposures were plotted sequentially
                             no_xticks,no_yticks=False,False
                             if (plot_mod in ['map_Intr_prof','map_Intr_1D','map_Intr_prof_est','map_Intr_prof_res','map_pca_prof','map_Atm_prof','map_Atm_1D']) and (ordi_name!='phase'):
                                 if plot_options['reverse_2D']:no_xticks=True
                                 else:
                                     no_yticks=True
@@ -983,15 +1015,17 @@
                             if plot_options['reverse_2D']:cbar_pos=fig.add_axes([plot_options['margins'][0],plot_options['margins'][3]+0.01,(plot_options['margins'][2]-plot_options['margins'][0]),0.03])   
                             else:cbar_pos=fig.add_axes([plot_options['margins'][2]+0.01,plot_options['margins'][1],0.015,(plot_options['margins'][3]-plot_options['margins'][1])])   
                         						
                             #Values	
                             cb = plt.cm.ScalarMappable(cmap=cmap_2D,norm=plt.Normalize(vmin=v_range[0], vmax=v_range[1]))										
                             cb.set_array(v_range) 	
                         
-                            if plot_mod in ['map_DIbin','map_DI_prof','map_Res_prof','map_Intr_prof','map_Intr_prof_est','map_Intr_prof_res','map_pca_prof','map_Intrbin','map_Intr_1D']:cbar_txt='flux'
+                            if plot_mod in ['map_DIbin','map_DI_prof','map_Res_prof','map_Intr_prof','map_BF_Res_prof','map_BF_Res_prof_re','map_Intr_prof_est','map_Intr_prof_res','map_pca_prof','map_Intrbin',
+                                            'map_Intr_1D','map_Res_prof_clean_pl_est','map_Res_prof_clean_sp_est','map_Res_prof_unclean_sp_est','map_Res_prof_unclean_pl_est','map_Res_prof_clean_sp_res',
+                                            'map_Res_prof_clean_pl_res','map_Res_prof_unclean_sp_res','map_Res_prof_unclean_pl_res']:cbar_txt='flux'
                             elif plot_mod in ['map_Atm_prof','map_Atmbin','map_Atm_1D']:cbar_txt=plot_options['pl_atm_sign']
                             cbar_txt = scaled_title(plot_options['sc_fact10'],cbar_txt)  
                             if plot_options['reverse_2D']:
                                 cbar=fig.colorbar(cb,cax=cbar_pos,format="%.1f", orientation='horizontal')
                                 cbar.set_label(cbar_txt,labelpad=-55,fontsize=plot_options['font_size']-2)	
                                 cbar.ax.tick_params(labelsize=plot_options['font_size']-2,labeltop='on')
                                 cbar.ax.xaxis.set_ticks_position('top')
@@ -1006,18 +1040,23 @@
                                 cbar.ax.tick_params(labelsize=plot_options['font_size']-2)
                                 			
                             #----------------------------------------------
                             #Saving plot
                             plt.gcf().set_rasterized(plot_options['rasterized'])
                             add_str = 'iord'+str(iord)   
                             if plot_mod in ['map_Intr_prof_est','map_Intr_prof_res']:
-                                if plot_options['line_model']=='rec':add_str+='_rec'
-                                else:
-                                    add_str+='_'+plot_options['mode_loc_data_corr']  
-                                    if plot_mod=='map_Intr_prof_res':add_str+='_res'
+                                add_str+='_'+plot_options['mode_loc_data_corr']+'_'+plot_options['line_model'] 
+                                if plot_mod=='map_Intr_prof_res':add_str+='_res'
+                            elif plot_mod in ['map_BF_Res_prof', 'map_BF_Res_prof_re']:
+                                add_str += 'BestFit'
+                                if plot_mod=='map_BF_Res_prof_re': add_str += 'Differential'
+                            elif plot_mod in ['map_Res_prof_clean_pl_est','map_Res_prof_clean_sp_est','map_Res_prof_unclean_sp_est','map_Res_prof_unclean_pl_est',
+                                            'map_Res_prof_clean_sp_res','map_Res_prof_clean_pl_res','map_Res_prof_unclean_sp_res','map_Res_prof_unclean_pl_res']:
+                                prof_typ = plot_mod.split('_')[-1]
+                                add_str += '_'+corr_plot_mod+'_'+supp_name+'_'+prof_typ                            
                             if ('bin' in plot_mod):add_str+='_'+plot_options['dim_plot'] 
                             plt.savefig(path_loc+'/'+add_str+'.'+save_res_map)                        
                             plt.close() 
                
                             ### End of order                          
            
             return None
@@ -1073,19 +1112,20 @@
         #Reference planet for the visit
         pl_ref=plot_options['pl_ref'][inst][vis] 
         
         #Upload model
         prof_fit_vis = None
         fit_results = None
         if plot_options['plot_line_model'] or plot_options['plot_line_model_HR'] or (('_res' in plot_mod) & (not plot_options['cont_only'])):
-            
+        
             #Planet-occulted models from reconstruction
-            if (('Res' in plot_mod) or ('Intr' in plot_mod)) and (plot_options['line_model']=='rec'):
-                prof_fit_vis = dataload_npz(gen_dic['save_data_dir']+'Loc_estimates/'+plot_options['mode_loc_data_corr']+'/'+inst+'_'+vis+'_add')
-                
+            if plot_options['line_model']=='rec':
+                if 'Intr' in plot_mod:prof_fit_vis = dataload_npz(gen_dic['save_data_dir']+'Loc_estimates/'+plot_options['mode_loc_data_corr']+'/'+inst+'_'+vis+'_add')
+                elif 'Res' in plot_mod:prof_fit_vis = dataload_npz(gen_dic['save_data_dir']+'Spot_Loc_estimates/'+plot_options['mode_loc_data_corr']+'/'+inst+'_'+vis+'_add')
+        
             #Line profile from best-fit
             else:
                 if (plot_options['fit_type']=='indiv'):
                     if not os_system.path.exists(gen_dic['save_data_dir']+data_type_gen+data_mode+'_prop/'+add_txt_path+inst+'_'+vis+'.npz'):stop('No existing fit results')
                     prof_fit_vis=dataload_npz(gen_dic['save_data_dir']+data_type_gen+data_mode+'_prop/'+add_txt_path+inst+'_'+vis)  
                 elif (plot_options['fit_type']=='global'):
                     if (data_type_gen in ['Intr','Atm']) and (inst in glob_fit_dic['IntrProf']['idx_in_fit']) and (vis in glob_fit_dic['IntrProf']['idx_in_fit'][inst]):
@@ -1176,17 +1216,18 @@
         
         #PCA results
         if plot_mod=='map_pca_prof':
             data_path_all = [gen_dic['save_data_dir']+'PCA_results/'+inst+'_'+vis+'_model'+str(iexp) for iexp in iexp_plot] 
             rest_frame = 'star'
               
         #Reconstructed line profiles
-        elif '_est' in plot_mod:        
-             data_path_all = [gen_dic['save_data_dir']+'Loc_estimates/'+plot_options['mode_loc_data_corr']+'/'+inst+'_'+vis+'_'+str(iexp) for iexp in iexp_plot]
-             rest_frame = 'star'
+        elif '_est' in plot_mod:
+            if 'Intr' in plot_mod:data_path_all = [gen_dic['save_data_dir']+'Loc_estimates/'+plot_options['mode_loc_data_corr']+'/'+inst+'_'+vis+'_'+str(iexp) for iexp in iexp_plot]
+            elif 'Res' in plot_mod:data_path_all = [gen_dic['save_data_dir']+'Spot_Loc_estimates/'+plot_options['mode_loc_data_corr']+'/'+inst+'_'+vis+'_'+str(iexp) for iexp in iexp_plot]
+            rest_frame = 'star'
          
         #Residual maps from Intrinsic and out-of-transit Residual profiles
         #    - data_path_all contains the path to Intrinsic profiles, from which will later be subtracted the model profiles
         #      if out-of-transit residuals are requested, we add the path to out-of-transit Residual profiles
         elif (plot_mod=='map_Intr_prof_res'): 
             inout_flag=np.repeat('in',len(iexp_plot))  
             if plot_options['cont_only']:
@@ -1203,14 +1244,27 @@
                 iexp_plot=np.append(iexp_plot,iexp_out) 
                 nexp_plot+=len(iexp_out)
                 iexp_orig=np.append(iexp_orig,iexp_out)
                 if plot_options['cont_only']:
                     data_path_all+=[data_dic[inst][vis]['proc_Res_data_paths']+str(iexp) for iexp in iexp_out]
                 else:
                     data_path_all+=[prof_fit_vis['loc_data_corr_outpath']+str(iexp) for iexp in iexp_out]
+
+        #Residual maps from Residual profiles
+        #    - data_path_all contains the path to Residual profiles, from which will later be subtracted the model profiles
+        elif plot_mod in ['map_Res_prof_clean_sp_res','map_Res_prof_clean_pl_res','map_Res_prof_unclean_sp_res','map_Res_prof_unclean_pl_res']:
+            data_path_all = [prof_fit_vis['loc_data_corr_path']+str(iexp) for iexp in iexp_plot]
+            rest_frame = prof_fit_vis['rest_frame']              
+        elif (plot_mod in ['map_BF_Res_prof', 'map_BF_Res_prof_re']):
+            #Retrieving the bin mode
+            if vis+'_bin' in data_dic['Res']['idx_in_bin'][inst]:bin_mode='_bin'
+            else:bin_mode = ''
+            #Retrieving the best-fit exposures
+            data_path_all = [gen_dic['save_data_dir']+'Joined_fits/ResProf/'+glob_fit_dic['ResProf']['fit_mode']+'/'+inst+'/'+vis+'/'+'BestFit'+bin_mode+'_'+str(iexp) for iexp in iexp_plot]
+            rest_frame = 'star'
         
         #Measured data
         else:         
             if (data_mode == 'bin'):
                 data_path_all = [gen_dic['save_data_dir']+data_type_gen+'bin_data/'+add_txt_path+'/'+inst+'_'+vis+'_'+plot_options['dim_plot']+str(iexp) for iexp in iexp_plot]
                 rest_frame = data_bin['rest_frame']
             elif (data_mode == 'orig'): 
@@ -1233,29 +1287,31 @@
                             #Spectral profiles
                             if ('spec' in data_type):         
                                 
                                 #Over correction steps
                                 if ('plot_pre' in plot_options) or ('plot_post' in plot_options):
                                     if plot_options['plot_post'] is not None:data_path_all = [data_path_dic[plot_options['plot_post']]+str(iexp) for iexp in iexp_plot]
                                     else:data_path_all = [None for iexp in iexp_plot]
+                                    rest_frame='input'   
                                 
                                 #Over processing steps
                                 else:
                                     if plot_options['step']=='sp_corr':
                                         data_path = data_dic[inst][vis]['corr_exp_data_paths']
                                         rest_frame='input'   
                                     elif plot_options['step']=='detrend':
                                         data_path = gen_dic['save_data_dir']+'Detrend_prof/'+inst+'_'+vis+'_'  
                                         rest_frame='input'                
                                     elif plot_options['step']=='aligned':
                                         data_path = gen_dic['save_data_dir']+'Aligned_DI_data/'+inst+'_'+vis+'_' 
                                         rest_frame='star'   
                                     elif plot_options['step']=='scaled':
                                         data_path = gen_dic['save_data_dir']+'Scaled_data/'+inst+'_'+vis+'_' 
-                                        rest_frame = dataload_npz(data_path+'add')['rest_frame']
+                                        rest_frame = dataload_npz(data_path+'add')['rest_frame']                                   
+                                    data_path_all = [data_path+str(iexp) for iexp in iexp_plot] 
                                 
                             #CCF profiles
                             elif (data_type=='CCF'):
                                 if plot_options['step']=='raw':
                                     data_path = data_dic[inst][vis]['raw_exp_data_paths']
                                     rest_frame = 'input'
                                 elif plot_options['step']=='conv':    
@@ -1263,30 +1319,35 @@
                                     rest_frame = 'input'
                                 elif plot_options['step']=='scaled':
                                     data_path = gen_dic['save_data_dir']+'Scaled_data/'+inst+'_'+vis+'_' 
                                     rest_frame = dataload_npz(data_path+'add')['rest_frame']
                                 elif plot_options['step']=='latest':
                                     data_path = data_dic[inst][vis]['proc_DI_data_paths']
                                     rest_frame = dataload_npz(data_path+'add')['rest_frame']                                    
-                            data_path_all = [data_path+str(iexp) for iexp in iexp_plot]                  
+                                data_path_all = [data_path+str(iexp) for iexp in iexp_plot]                  
                           
                     #Other types of profiles
                     else:  
                         data_path_all = [gen_dic['save_data_dir']+txt_aligned+data_type_gen+'_data/'+add_txt_path+'/'+txt_conv+'/'+inst+'_'+vis+'_'+str(iexp) for iexp in iexp_plot]   
                         if 'Res' in plot_mod:rest_frame='star'   
                         elif 'Intr' in plot_mod:
                             if plot_options['aligned']:rest_frame='surf' 
                             else:rest_frame='star'   
                         if 'Atm' in plot_mod:
                             if plot_options['aligned']:rest_frame='pl' 
                             else:rest_frame='star'   
             
         #Data dimensions
         if data_path_all[0] is not None:
-            dim_exp_data = list(np.shape(dataload_npz(data_path_all[0])['flux']))
+            if ('Res_prof' in plot_mod) and ('_est' in plot_mod):
+                flux_supp = plot_mod.split('_')[4]
+                corr_plot_mod = plot_mod.split('_')[3]
+                flux_name=corr_plot_mod+'_'+flux_supp+'_flux'
+            else:flux_name='flux'
+            dim_exp_data = list(np.shape(dataload_npz(data_path_all[0])[flux_name]))
             nord_data = dim_exp_data[0] 
         else:
             nord_data = None
                             
         return pl_ref,txt_conv,iexp_plot,iexp_orig,prof_fit_vis,fit_results,data_path_all,rest_frame,data_path_dic,nexp_plot,inout_flag,path_loc,iexp_mast_list,nord_data,data_bin
     
     
@@ -1321,15 +1382,15 @@
         
         #Options
         sc_fact=10**plot_options['sc_fact10']
         hide_yticks=False  
 
         #Plot for each instrument        
         for inst in np.intersect1d(data_dic['instrum_list'],list(plot_options['visits_to_plot'].keys())): 
-            print('      - Instrument :',inst)
+            print('   - Instrument :',inst)
             for key in ['color_dic','color_dic_sec','color_dic_bin','color_dic_bin_sec']:
                 if inst not in plot_options[key]:plot_options[key][inst]={}
 
             #Data to plot
             maink_list = []
             data_list = []
             if plot_options['plot_pre'] is not None:
@@ -1378,15 +1439,15 @@
             # elif (plot_mod in ['sp_Intr_1D','sp_Atm_1D']) and (plot_options['dim_plot']=='bin'):
             #     ref_name = dim_bin_1D
             else:
                 ref_name = 'phase'  
 
             #Plot for each visit
             for vis in np.intersect1d(list(data_dic[inst].keys())+['binned'],plot_options['visits_to_plot'][inst]): 
-                print('        - Visit :',vis)
+                print('     - Visit :',vis)
                 data_inst=data_dic[inst]
 
                 #Data
                 if vis=='binned':data_com = dataload_npz(data_inst['proc_com_data_path'])  
                 else:data_com = dataload_npz(data_inst[vis]['proc_com_data_paths'])  
                 fixed_args_loc = {}
                 pl_ref,txt_conv,iexp_plot,iexp_orig,prof_fit_vis,fit_results,data_path_all,rest_frame,data_path_dic,nexp_plot,inout_flag,path_loc,iexp_mast_list,nord_data,data_bin = sub_plot_prof_dir(inst,vis,plot_options,data_mode,'Indiv',add_txt_path,plot_mod,txt_aligned,data_type,data_type_gen)
@@ -2056,16 +2117,16 @@
                                         # + a single exposure per order is plotted, or last exposure has been processed
                                         #----------------------------------------
                                         if ((not plot_options['multi_exp']) or (isub==len(iexp_plot)-1)): 
                                             filename = end_plot_prof(pl_ref,inst,vis,all_figs[key_frame],all_ax[key_frame],x_range_loc[key_frame],y_range_loc[key_frame],hide_yticks,plot_options,iexp_or,plot_mod,title_name,ref_name,iord,plot_ext,x_title,y_title,path_loc,data_bin)
      
                                             #Store image for GIF generation
                                             if (images_to_make_GIF is not None): 
-                                                if (not plot_options['multi_exp']):images_to_make_GIF[iord].append(imageio.imread(filename))   
-                                                else:images_to_make_GIF.append(imageio.imread(filename))   
+                                                if (not plot_options['multi_exp']):images_to_make_GIF[iord].append(imageio.v2.imread(filename))   
+                                                else:images_to_make_GIF.append(imageio.v2.imread(filename))   
                 
                         ### End of loop on orders         
 
                         #----------------------------------------
                         #Plot frame 
                         #    - end frame after current exposure and all orders have been processed if :
                         # + a single exposure per order is plotted, or last exposure has been processed
@@ -2091,18 +2152,18 @@
                 if (images_to_make_GIF is not None):
                     
                     #For each order, over exposure series
                     if (not plot_options['multi_exp']):
                         for iord in images_to_make_GIF:
                             if (plot_mod in ['DI_prof','DImast','Res','Intr','atm']) and (data_dic['Res']['type'][inst]=='spec2D'):str_add='_iord'+str(iord)
                             else:str_add=''                            
-                            imageio.mimsave(path_loc+'/'+ref_name+str_add+'.gif', images_to_make_GIF[iord],fps=plot_options['fps'])
+                            imageio.mimsave(path_loc+'/'+ref_name+str_add+'.gif', images_to_make_GIF[iord],duration=(1000 * 1/plot_options['fps']))
                     
                     #Over order series, with multiple exposures per plot
-                    else:imageio.mimsave(path_loc+'/multi_exp_'+ref_name+'.gif', images_to_make_GIF,fps=plot_options['fps'])
+                    else:imageio.mimsave(path_loc+'/multi_exp_'+ref_name+'.gif', images_to_make_GIF,duration=(1000 * 1/plot_options['fps']))
 
                
         return None
 
     def pre_proc_exp(plot_options,inst,vis,maink_list,iexp_plot,iexp_mast_list,data_inst,data_vis,data_path_dic,idx_sel_ord,cen_bins_com,edge_bins_com,nord_proc,dim_exp_proc,data_list,fixed_args_loc):
         print('           Pre-processing exposures')
         data_proc = {} 
@@ -2155,25 +2216,26 @@
                 for isub in range(nord_proc):
                     flux_glob+= np.sum(dcen_wav[isub][cond_def[isub]])/np.sum(data_proc[maink][iexp]['flux'][isub][cond_def[isub]]*dcen_wav[isub][cond_def[isub]])
                 for isub in range(nord_proc):
                     data_proc[maink][iexp]['flux'][isub],data_proc[maink][iexp]['cov'][isub] = bind.mul_array(data_proc[maink][iexp]['flux'][isub] , data_proc[maink][iexp]['cov'][isub],np.repeat(flux_glob,data_vis['nspec']))
    
                 #Exposures used in master calculations
                 if iexp in iexp_mast_list:
+                    data4mast[maink][iexp]={}
                     for key in ['cen_bins','edge_bins','flux','cov','cond_def']:data4mast[maink][iexp][key]=deepcopy(data_proc[maink][iexp][key])
                     
                     #Weight definition   
                     #    - at this stage, no broadband flux scaling has been applied to the data
                     data4mast[maink][iexp]['weight'] = weights_bin_prof(idx_sel_ord,None,inst,vis,gen_dic['corr_Fbal'],gen_dic['corr_FbalOrd'],gen_dic['save_data_dir'],gen_dic['type'],nord_proc,iexp,'DI',data_inst['type'],dim_exp_proc,data_proc[maink][iexp]['tell'],data_proc[maink][iexp]['mean_gdet'],data_proc[maink][iexp]['cen_bins'],1.,flux_ref,None,glob_flux_sc = 1./flux_glob)                       
        
                     #Resampling if exposures do not share a common table
                     if (not data_vis['comm_sp_tab']):   
                         for isub in range(nord_proc):
-                            data4mast[maink][iexp]['flux'][isub],data4mast[maink][iexp]['cov'][isub] = bind.resampling(edge_bins_com[isub], data_proc[maink][iexp]['edge_bins'][isub], data_proc[maink][iexp]['flux'][isub] , cov = data_proc[maink][iexp]['cov'][isub], kind=gen_dic['resamp_mode'])                                                        
-                            data4mast[maink][iexp]['weight'][isub] = bind.resampling(edge_bins_com[isub], data_proc[maink][iexp]['edge_bins'][isub], data_proc[maink][iexp]['weight'][isub] ,kind=gen_dic['resamp_mode'])   
+                            data4mast[maink][iexp]['flux'][isub],data4mast[maink][iexp]['cov'][isub] = bind.resampling(edge_bins_com[isub], data4mast[maink][iexp]['edge_bins'][isub], data_proc[maink][iexp]['flux'][isub] , cov = data_proc[maink][iexp]['cov'][isub], kind=gen_dic['resamp_mode'])                                                        
+                            data4mast[maink][iexp]['weight'][isub] = bind.resampling(edge_bins_com[isub], data4mast[maink][iexp]['edge_bins'][isub], data4mast[maink][iexp]['weight'][isub] ,kind=gen_dic['resamp_mode'])   
                         data4mast[maink][iexp]['cond_def'] = ~np.isnan(data4mast[maink][iexp]['flux']) 
                         data4mast[maink][iexp]['cen_bins'] = cen_bins_com
                         data4mast[maink][iexp]['edge_bins'] = edge_bins_com
               
             #Calculating wiggle model for current exposure and shifting it from the telluric (source) to the star (receiver) rest frame
             #    - see gen_specdopshift():
             # w_receiver = w_source * (1+ (rv[s/r]/c))
@@ -2212,16 +2274,16 @@
             dx_range=x_range_frame[1]-x_range_frame[0]
             x_range_frame = [x_range_frame[0]-0.05*dx_range,x_range_frame[1]+0.05*dx_range]
         else:x_range_frame = plot_options['x_range']
         if plot_options['y_range'] is None:y_range_frame = [0.95*y_range_frame[0],1.05*y_range_frame[1]]
         else:y_range_frame = plot_options['y_range']
         dx_range=x_range_frame[1]-x_range_frame[0]
         dy_range=y_range_frame[1]-y_range_frame[0]
-        xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-        ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)
+        xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+        ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)
         custom_axis(plt,fig = fig_frame,ax=ax_frame,position=plot_options['margins'],x_range=x_range_frame,y_range=y_range_frame,
                     xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,
                     xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                     hide_yticks = hide_yticks,dir_x = 'out',
                     # dir_y='out',
                     # axis_thick=plot_options['axis_thick']
                     hide_axis = plot_options['hide_axis'],
@@ -2265,15 +2327,15 @@
         - for disk-integrated data in the star rest frame
         - a common master is used
     '''
     def sub_plot_DI_trans(plot_options,plot_mod,plot_ext):
         
         #Plot for each instrument        
         for inst in np.intersect1d(data_dic['instrum_list'],list(plot_options['visits_to_plot'].keys())): 
-            print('      - Instrument :',inst)
+            print('   - Instrument :',inst)
             for key in ['color_dic','color_dic_sec','color_dic_bin','color_dic_bin_sec']:
                 if inst not in plot_options[key]:plot_options[key][inst]={}
                 data_type = data_dic['DI']['type'][inst]
             
             #Data to plot
             maink_list = []
             data_list = []
@@ -2285,15 +2347,15 @@
                 data_list+=[plot_options['plot_post']]       
 
             #Frame properties
             title_name=''
             
             #Plot for each visit
             for vis in np.intersect1d(list(data_dic[inst].keys()),plot_options['visits_to_plot'][inst]): 
-                print('        - Visit :',vis)
+                print('     - Visit :',vis)
                 if vis not in plot_options['color_dic'][inst]:plot_options['color_dic'][inst][vis] ='red' 
                 if vis not in plot_options['color_dic_bin'][inst]:plot_options['color_dic_bin'][inst][vis] ='limegreen' 
                 if vis not in plot_options['color_dic_sec'][inst]:plot_options['color_dic_sec'][inst][vis] ='dodgerblue' 
                 if vis not in plot_options['color_dic_bin_sec'][inst]:plot_options['color_dic_bin_sec'][inst][vis] ='orange' 
   
                 #Create directory if required
                 path_loc = gen_dic['save_plot_dir']+'Spec_raw/DI_trans/'+inst+'_'+vis+'/'
@@ -2558,16 +2620,16 @@
                                 plt.text(x_ord[iord],y_range_loc[1]+delt_txt*dy_range,str(iord),verticalalignment='center', horizontalalignment='center',fontsize=6.,zorder=15,color='black') 
 
                     #Shade ranges not included in the fit
                     if ('wiggle' in data_list) and (plot_options['shade_unfit']) and (vis in data_com_wig['wig_range_fit']):
                         plot_shade_range(plt.gca(),data_com_wig['wig_range_fit'][vis],x_range_loc,y_range_loc,mode='fill',facecolor='dodgerblue',compl=True)                  
 
                     #Frame
-                    xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                    ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)
+                    xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                    ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)
                     if plot_options['sp_var']=='nu':x_title=r'Nu (10$^{-10}$s$^{-1}$)'
                     elif plot_options['sp_var']=='wav':x_title=r'Wavelength (A)'
                     custom_axis(plt,position=plot_options['margins'],x_range=x_range_loc,y_range=y_range_loc,xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                 x_title=x_title,y_title='Flux ratio',font_size=plot_options['font_size'],xfont_size=plot_options['font_size'],yfont_size=plot_options['font_size'])
                     plt.savefig(path_loc+'idx'+str(iexp)+'.'+plot_dic['trans_sp']) 
                     plt.close()      
                  
@@ -2640,16 +2702,16 @@
                                 xtxt =x_range_loc[1]-0.4*dx_range
                                 if bin_type=='raw':col_loc = plot_options['color_dic_sec'][inst][vis]
                                 elif bin_type=='bin':col_loc = plot_options['color_dic_bin_sec'][inst][vis] 
                             rms_txt = 'RMS['+datak+'.]'+ " = {0:.2e}".format(mean_disp[maink][bin_type])+' ('+bin_type+')'
                             plt.text(xtxt,ytxt,rms_txt,verticalalignment='center', horizontalalignment='left',fontsize=8.,zorder=10,color=col_loc)
             
                     #Frame                                                 
-                    xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                    ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)
+                    xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                    ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)
                     custom_axis(plt,position=plot_options['margins'],x_range=x_range_loc,y_range=y_range_loc,xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                 x_title=r'Orbital Phase',y_title='RMS (ppm)',font_size=plot_options['font_size'],xfont_size=plot_options['font_size'],yfont_size=plot_options['font_size'])
                     plt.savefig(path_loc+'Dispersion.'+plot_dic['trans_sp']) 
                     plt.close() 
 
         return None
 
@@ -2781,16 +2843,16 @@
                             # if plot_options['plot_cont']:plt.plot(data_exp['cen_bins'][0][cond_cont],var_loc[cond_cont],color='black',linestyle='',marker='d',markersize=1,zorder=10,rasterized=plot_options['rasterized'])      
                             
                     #Plot frame               
                     if plot_options['title']:plt.title(al_txt+title_name+' CCFs in '+xt_str+' rest frame',fontsize=plot_options['font_size'])
                     y_title = scaled_title(plot_options['sc_fact10'],y_title)                       
                     dx_range=x_range_loc[1]-x_range_loc[0]
                     dy_range=y_range_loc[1]-y_range_loc[0]
-                    xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                    ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range) 
+                    xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                    ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range) 
                     custom_axis(plt,position=plot_options['margins'],x_range=x_range_loc,y_range=y_range_loc,
                                 xmajor_int=xmajor_int,xminor_int=xminor_int,
                                 ymajor_int=ymajor_int,yminor_int=yminor_int,
                                 xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                 x_title='Velocity in '+xt_str+' rest frame (km s$^{-1}$)',y_title=y_title,
                                 font_size=plot_options['font_size'],xfont_size=plot_options['font_size'],yfont_size=plot_options['font_size'])
                   						
@@ -2894,16 +2956,16 @@
                             if data_type=='spec1D':str_add=''
                             elif data_type=='spec2D':str_add=' (iord = '+str(iord)+')'                        
                             if plot_options['title']:plt.title(al_txt+title_name+' spectra in '+xt_str+' rest frame'+str_add)
                             y_title='Flux'
                             y_title = scaled_title(plot_options['sc_fact10'],y_title)
                             dx_range=x_range_loc[1]-x_range_loc[0]
                             dy_range=y_range_loc[1]-y_range_loc[0]
-                            xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                            ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)
+                            xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                            ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)
                             custom_axis(plt,position=plot_options['margins'],x_range=x_range_loc,y_range=y_range_loc,
                                         xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,
                                         xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                         x_title='Wavelength in '+xt_str+' rest frame (A)',y_title=y_title,
                                         font_size=plot_options['font_size'],xfont_size=plot_options['font_size'],yfont_size=plot_options['font_size'])
             
                             if (data_type=='spec2D'):str_add='_iord'+str(iord)
@@ -2978,16 +3040,16 @@
                
                     #Plot frame
                     if plot_options['title']:plt.title('Binned disk-integrated and intrinsic CCFs',fontsize=plot_options['font_size'])
                     y_title='Flux'
                     y_title = scaled_title(plot_options['sc_fact10'],y_title)                   
                     dx_range=x_range_loc[1]-x_range_loc[0]
                     dy_range=y_range_loc[1]-y_range_loc[0]
-                    xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                    ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range) 
+                    xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                    ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range) 
                     custom_axis(plt,position=plot_options['margins'],x_range=x_range_loc,y_range=y_range_loc,
                                 xmajor_int=xmajor_int,xminor_int=xminor_int,
                                 ymajor_int=ymajor_int,yminor_int=yminor_int,
                                 xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                 x_title='Velocity (km s$^{-1}$)',y_title=y_title,
                                 font_size=plot_options['font_size'],xfont_size=plot_options['font_size'],yfont_size=plot_options['font_size'])                 						
                     plt.savefig(path_loc+'CCF.'+plot_ext) 
@@ -3040,16 +3102,16 @@
                         if plot_options['data_type']=='spec1D':str_add=''
                         elif plot_options['data_type']=='spec2D':str_add=' (iord = '+str(iord)+')'                        
                         if plot_options['title']==True:plt.title('Binned disk-integrated and intrinsic '+str_add)
                         y_title='Flux'
                         y_title = scaled_title(plot_options['sc_fact10'],y_title) 
                         dx_range=x_range_loc[1]-x_range_loc[0]
                         dy_range=y_range_loc[1]-y_range_loc[0]
-                        xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                        ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)
+                        xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                        ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)
                         custom_axis(plt,position=plot_options['margins'],x_range=x_range_loc,y_range=y_range_loc,
                                     xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,
                                     xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                     x_title='Wavelength (A)',y_title=y_title,
                                     font_size=plot_options['font_size'],xfont_size=plot_options['font_size'],yfont_size=plot_options['font_size'])
                         str_add=''
                         if (plot_options['data_type']=='spec2D'):str_add='_iord'+str(iord)
@@ -3104,16 +3166,16 @@
             
         #---------------------------------------------------------------------------------------- 
 
         #Plot frame 
         x_range_loc=autom_range_ext(plot_options['x_range'],x_min,x_max)
         y_range_loc=autom_range_ext(plot_options['y_range'],0.,y_max)
         if plot_options['title']:plt.title('$\Chi^2$ per exposure',fontsize=plot_options['font_size'])     
-        xmajor_int,xminor_int,xmajor_form=autom_x_tick_prop(x_range_loc[1]-x_range_loc[0])
-        ymajor_int,yminor_int,ymajor_form=autom_y_tick_prop(y_range_loc[1]-y_range_loc[0])                          
+        xmajor_int,xminor_int,xmajor_form=autom_tick_prop(x_range_loc[1]-x_range_loc[0])
+        ymajor_int,yminor_int,ymajor_form=autom_tick_prop(y_range_loc[1]-y_range_loc[0])                          
         custom_axis(plt,position=plot_options['margins'],x_range=x_range_loc,y_range=y_range_loc,
     		        xmajor_int=xmajor_int,xminor_int=xminor_int,xmajor_form=xmajor_form,
                     ymajor_form=ymajor_form,ymajor_int=ymajor_int,yminor_int=yminor_int,     
         		    x_title=data_upload['coord_line'],y_title='$\chi^2$',
                     font_size=plot_options['font_size'],xfont_size=plot_options['font_size'],yfont_size=plot_options['font_size'])
         plt.savefig(path_loc+'Chi2_per_exp.'+plot_ext)                        
         plt.close() 
@@ -3339,15 +3401,15 @@
                                 RV_stsurf_HR_thread=np.empty([nsamp,theo_HR_prop_plocc['nph_HR']])
                                 
                                 #For each sample, calculate and overwrite surface rv alone
                                 coord_pl_in_samp = deepcopy(theo_HR_prop_plocc)
                                 theo_dic_samp = deepcopy(theo_dic)
                                 theo_dic_samp['d_oversamp'] = []
                                 for isamp in range(nsamp):
-                                    surf_prop_dic,_ = sub_calc_plocc_spot_prop(['achrom'],{},['rv'],[pl_loc],system_param,theo_dic_samp,data_dic['DI']['system_prop'],par_subsample[0][isamp],coord_pl_in_samp,range(theo_HR_prop_plocc['nph_HR']))        
+                                    surf_prop_dic,_,_ = sub_calc_plocc_spot_prop(['achrom'],{},['rv'],[pl_loc],system_param,theo_dic_samp,data_dic['DI']['system_prop'],par_subsample[0][isamp],coord_pl_in_samp,range(theo_HR_prop_plocc['nph_HR']))        
                                     RV_stsurf_HR_thread[isamp,:] =surf_prop_dic['achrom'][pl_loc]['rv'][0,:]                                
                                 return RV_stsurf_HR_thread
                             
                             def sub_calc_plocc_spot_prop_par(pool_proc,func_input,nthreads,n_elem,y_inputs,common_args):     
                                 ind_chunk_list=init_parallel_func(nthreads,n_elem)
                                 chunked_args=[(y_inputs[0][ind_chunk[0]:ind_chunk[1]],)+common_args for ind_chunk in ind_chunk_list]	
                                 all_results=tuple(tab for tab in pool_proc.map(func_input,chunked_args))			
@@ -3431,16 +3493,16 @@
                             if plot_options['prop_'+data_mode+'_absc']!='phase':stop('Use correct binning dimension')
                             data_bin = dataload_npz(gen_dic['save_data_dir']+'DIbin_data/'+inst+'_'+vis+'_phase')
                             if gen_dic['fit_DIbin'] or gen_dic['fit_DIbinmultivis']:prof_fit_vis=dataload_npz(gen_dic['save_data_dir']+'DIbin_prop/'+inst+'_'+vis)
                         else:
                             coord_vis = coord_dic[inst][vis][pl_ref]
                             data_prop_vis = data_prop[inst][vis]
                             # if gen_dic['fit_DI'] or gen_dic['fit_DI_1D']:prof_fit_vis=np.load(gen_dic['save_data_dir']+'DIorig_prop/'+inst+'_'+vis+'.npz',allow_pickle=True)['data'].item()
-                            prof_fit_vis=np.load(gen_dic['save_data_dir']+'DIorig_prop/'+inst+'_'+vis+'.npz',allow_pickle=True)['data'].item()
-                        transit_prop_nom = (np.load(gen_dic['save_data_dir']+'Introrig_prop/PlOcc_Prop_'+inst+'_'+vis+'.npz',allow_pickle=True)['data'].item())['achrom'][pl_ref]
+                            prof_fit_vis=dataload_npz(gen_dic['save_data_dir']+'DIorig_prop/'+inst+'_'+vis)
+                        transit_prop_nom = dataload_npz(gen_dic['save_data_dir']+'Introrig_prop/PlOcc_Prop_'+inst+'_'+vis)['achrom'][pl_ref]
 
                     elif data_mode=='Intr':
                         if data_type=='Introrig':
                             coord_vis = coord_dic[inst][vis][pl_ref]
                             if plot_options['plot_data']:prof_fit_vis=dataload_npz(gen_dic['save_data_dir']+'Introrig_prop/'+inst+'_'+vis)
                             transit_prop_nom = (np.load(gen_dic['save_data_dir']+'Introrig_prop/PlOcc_Prop_'+inst+'_'+vis+'.npz',allow_pickle=True)['data'].item())['achrom'][pl_ref]                                                      
                         elif data_type=='Intrbin': 
@@ -4132,32 +4194,37 @@
                             val_ref=Bin_prof_fit_vis[prop_loc]
                         plt.plot([min(x_obs),max(x_obs)],np.repeat(val_ref,2),color=col_loc,linestyle=':',lw=plot_options['lw_plot'],zorder=0)
     
     
                     #Contacts
                     if plot_options['prop_'+data_mode+'_absc']=='phase':
                         for ipl,pl_loc in enumerate(data_dic[inst][vis]['transit_pl']):
-                            if (i_visit==1) or ((pl_loc in gen_dic['Tcenter_visits']) and (inst in gen_dic['Tcenter_visits'][pl_loc]) and (vis in gen_dic['Tcenter_visits'][pl_loc][inst])):                               
+                            if (i_visit==0) or ((pl_loc in gen_dic['Tcenter_visits']) and (inst in gen_dic['Tcenter_visits'][pl_loc]) and (vis in gen_dic['Tcenter_visits'][pl_loc][inst])): 
                                 if pl_loc==pl_ref:
                                     cen_ph = 0.
                                     contact_phases_vis = contact_phases[pl_ref]
                                 else:
                                     contact_times = coord_dic[inst][vis][pl_loc]['Tcenter']+contact_phases[pl_loc]*system_param[pl_loc]["period"]
                                     contact_phases_vis = (contact_times-coord_dic[inst][vis][pl_ref]['Tcenter'])/system_param[pl_ref]["period"]  
                                     cen_ph = (coord_dic[inst][vis][pl_loc]['Tcenter']-coord_dic[inst][vis][pl_ref]['Tcenter'])/system_param[pl_ref]["period"] 
                                 ls_pl = {0:':',1:'--'}[ipl]
                                 for cont_ph in contact_phases_vis:
                                     plt.plot([cont_ph,cont_ph],[-1e6,1e6],color='black',linestyle=ls_pl,lw=plot_options['lw_plot'],zorder=0)
-                         
+                
                                 #Overplot transit duration from system properties
                                 if (data_mode=='DI') and plot_options['plot_T14']:
                                     T14_phase = system_param[pl_loc]['TLength']/(system_param[pl_ref]['period'])
                                     plt.plot([cen_ph-0.5*T14_phase,cen_ph-0.5*T14_phase],[-1e6,1e6],color='black',linestyle='--',lw=plot_options['lw_plot'],zorder=0)
                                     plt.plot([cen_ph+0.5*T14_phase,cen_ph+0.5*T14_phase],[-1e6,1e6],color='black',linestyle='--',lw=plot_options['lw_plot'],zorder=0)                              
-    
+
+                        #Use main planet contact as plot range if undefined
+                        if (plot_options['x_range'] is None) and (data_mode=='Intr'):
+                            delt_range = 0.05*system_param[pl_ref]['T14_num']/system_param[pl_ref]["period"]
+                            plot_options['x_range'] = np.array([contact_phases[pl_ref][0]-delt_range,contact_phases[pl_ref][3]+delt_range])   
+                                              
                     #-------------------------------------------------------
                     #Predicted local RVs measurements from nominal system properties
                     if (data_mode=='Intr') and ('predic' in plot_options) and (len(plot_options['predic'])>0) and (prop_mode=='rv') and (plot_options['prop_'+data_mode+'_absc']=='phase'):                 
                   
                         #Sub-function predicting errors on local RVs (in km/s)
                         #    - the error on the RV measurement derived from a CCF writes as (see Boisse et al.  (2010), A&A 523, 88)
                         # eRV(t) = 1 / Q_CCF * sqrt( sum( i, CCF[i,t] ) )
@@ -4291,17 +4358,17 @@
 
         #-------------------------------------------------------
         #Ranges   
         if plot_options['plot_bounds']:
             print('     Max X range =',np.array([x_min,x_max])  )
             print('     Max Y range =',np.array([y_min,y_max])  )                               
         if plot_options['x_range'] is not None:x_range_loc=plot_options['x_range']
-        else:
-            dx_range = x_max-x_min
-            x_range_loc = np.array([x_min-0.05*dx_range,x_max+0.05*dx_range])   
+        else:   
+            delt_range = 0.05*( x_max-x_min )
+            x_range_loc = np.array([x_min-delt_range,x_max+delt_range])   
         if plot_options['y_range'] is not None:y_range_loc=plot_options['y_range'] 
         else:
             dy_range = y_max-y_min
             y_range_loc = np.array([y_min-0.05*dy_range,y_max+0.05*dy_range])  
 
         #Reference level
         if plot_options['plot_ref']:
@@ -4444,27 +4511,26 @@
             plot_title_dic['true_ctrst'] = 'True contrast of '+sub_key+' CCFs'
             plt.title(plot_title_dic[prop_mode])
 
         #Invert horizontal axis
         if plot_options['retro_orbit']:x_range_loc=-np.array(x_range_loc)
 
         #Frame
-        xmajor_int,xminor_int,xmajor_form=autom_x_tick_prop(x_range_loc[1]-x_range_loc[0])
-        ymajor_int,yminor_int,ymajor_form=autom_y_tick_prop(y_range_loc[1]-y_range_loc[0])       
+        xmajor_int,xminor_int,xmajor_form=autom_tick_prop(x_range_loc[1]-x_range_loc[0])
+        ymajor_int,yminor_int,ymajor_form=autom_tick_prop(y_range_loc[1]-y_range_loc[0])       
         custom_axis(plt,position=plot_options['margins'],x_range=x_range_loc,y_range=y_range_loc,
                     dir_x = 'out',dir_y = 'out',
     		        xmajor_int=xmajor_int,xminor_int=xminor_int,xmajor_form=xmajor_form,
                     ymajor_form=ymajor_form,ymajor_int=ymajor_int,yminor_int=yminor_int,                
                     x_title=x_title_dic[plot_options['prop_'+data_mode+'_absc']],y_title=y_title_dic[prop_mode],
                     font_size=plot_options['font_size'],xfont_size=plot_options['font_size'],yfont_size=plot_options['font_size'])
         if data_mode=='DI':sub_key = 'DI'
         elif data_mode=='Intr':sub_key = 'Intr'
         plt.savefig(path_loc+prop_mode+'_'+plot_options['prop_'+data_mode+'_absc']+'.'+plot_dic['prop_'+sub_key]) 
         plt.close()
-        print('   ---------------')
     		
         return None   
 
 
 
 
 
@@ -4889,16 +4955,16 @@
             if (thresh_test is not None):
                 n_test = np.sum(cond_sel_test)             
                 axes[1,0].text(x_range_loc[1]+0.2*dx_range,y_range_loc[1]+0.1*dy_range,'Trial = '+str(n_test),verticalalignment='bottom', horizontalalignment='left',fontsize=plot_options['font_size_txt'],zorder=4,color='gold') 
             
             #Set up the axes
             axes[1,0].set_xlim(x_range_loc)
             axes[1,0].set_ylim(y_range_loc)
-            xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-            ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)
+            xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+            ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)
             axes[1,0].xaxis.set_major_locator(MultipleLocator(xmajor_int))
             axes[1,0].yaxis.set_major_locator(MultipleLocator(ymajor_int))
             x_lab_name = {
                 'ld':'Continuum depth',
                 'ld_lw':r'$log_{10}$(Width)',
                 'morphasym':'Continuum difference',
                 'morphshape':'Width (km/s)',
@@ -5127,16 +5193,16 @@
                     x_range_loc = plot_set_key['x_range'] if plot_set_key['x_range'] is not None else [np.nanmin(cen_bins_mean),np.nanmax(cen_bins_mean)] 
                     y_range_loc = plot_set_key['y_range'] if plot_set_key['y_range'] is not None else [np.nanmin(gdet_bins_mean),np.nanmax(gdet_bins_mean)] 
                    
                     #Plot frame  
                     if plot_set_key['title']:plt.title('Calibration for visit '+vis+' in '+inst)
                     dx_range=x_range_loc[1]-x_range_loc[0]
                     dy_range=y_range_loc[1]-y_range_loc[0]
-                    xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                    ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)                    
+                    xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                    ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)                    
                     custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
                                 xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,
                                 xmajor_form=xmajor_form,ymajor_form=ymajor_form,hide_axis=plot_set_key['hide_axis'],
                                 x_title='Wavelength (A)',y_title=r'10$^{-5}$ Calibration',
                                 font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                     plt.savefig(path_loc+'Global'+'.'+plot_dic[key_plot],transparent=plot_set_key['transparent']) 
                     plt.close()                     
@@ -5184,16 +5250,16 @@
                             plt.plot([wav_trans_all[0,isub_ord,isub_iexp],wav_trans_all[0,isub_ord,isub_iexp]],y_range_loc,linestyle='--',color=col_visit[isub_iexp],lw=0.5,rasterized=plot_set_key['rasterized'])
                             plt.plot([wav_trans_all[1,isub_ord,isub_iexp],wav_trans_all[1,isub_ord,isub_iexp]],y_range_loc,linestyle='--',color=col_visit[isub_iexp],lw=0.5,rasterized=plot_set_key['rasterized'])
                                                         
                         #Plot frame                          
                         if plot_set_key['title']:plt.title('Calibration for visit '+vis+' in '+inst+' (order '+str(iord)+')')
                         dx_range=x_range_loc[1]-x_range_loc[0]
                         dy_range=y_range_loc[1]-y_range_loc[0]
-                        xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                        ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)
+                        xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                        ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)
                         custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
                                     xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,
                                     xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                     x_title='Wavelength (A)',y_title=r'10$^{-3}$ Calibration',hide_axis=plot_set_key['hide_axis'],
                                     font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                         plt.savefig(path_loc+'ord'+str(iord)+'.'+plot_dic['gcal_ord'],transparent=plot_set_key['transparent']) 
                         plt.close() 
@@ -5203,27 +5269,27 @@
 
 
 
     ################################################################################################################    
     #%%%% Telluric CCF
     ################################################################################################################  
     if ('tell_CCF' in plot_settings):
-        key_plot = 'gcal'
+        key_plot = 'tell_CCF'
         plot_set_key = plot_settings[key_plot]
           
         print('-----------------------------------')
         print('+ Telluric CCF')
 
         #Process original visits   
         for inst in np.intersect1d(data_dic['instrum_list'],list(plot_set_key['visits_to_plot'].keys())): 
-            print('      - Instrument :',inst)
+            print('   - Instrument :',inst)
             if inst not in plot_set_key['color_dic']:plot_set_key['color_dic'][inst]={}
             if inst not in plot_set_key['color_dic_sec']:plot_set_key['color_dic_sec'][inst]={}
             for vis in np.intersect1d(list(data_dic[inst].keys()),plot_set_key['visits_to_plot'][inst]): 
-                print('        - Visit :',vis)
+                print('     - Visit :',vis)
                 if vis not in plot_set_key['color_dic'][inst]:plot_set_key['color_dic'][inst][vis]='red'
                 if vis not in plot_set_key['color_dic_sec'][inst]:plot_set_key['color_dic_sec'][inst][vis]='dodgerblue'
                 
                 #Create directory if required
                 path_loc = gen_dic['save_plot_dir']+'Spec_raw/Tell_corr/'+inst+'_'+vis+'/Tell_CCF/'
                 if not os_system.path.exists(path_loc):os_system.makedirs(path_loc)  
 
@@ -5275,16 +5341,16 @@
                                 #Frame
                                 x_range_loc=plot_set_key['x_range'] if plot_set_key['x_range'] is not None else np.array([x_min,x_max])
                                 if (plot_set_key['y_range'] is not None) and (inst in plot_set_key['y_range']) and (vis in plot_set_key['y_range'][inst]) and (molec in plot_set_key['y_range'][inst][vis]):
                                     y_range_loc = plot_set_key['y_range'][inst][vis][molec]
                                 else:y_range_loc=np.array([y_min,y_max])                            
                                 dx_range=x_range_loc[1]-x_range_loc[0]        
                                 dy_range=y_range_loc[1]-y_range_loc[0]                         
-                                xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                                ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)
+                                xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                                ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)
                                 custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                             x_title=r'Velocity in telluric rest frame (km s$^{-1}$)',y_title='Flux',font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                                 plt.savefig(path_loc+molec+'_idx'+str(iexp)+'.'+plot_dic['tell_CCF']) 
                                 plt.close()  
 
                 #Dispersion plots
                 if plot_set_key['print_disp'] is not None:
@@ -5318,16 +5384,16 @@
                         mean_disp = np.mean(disp_molec)
                         plt.plot(x_range_loc,[mean_disp,mean_disp],color='dodgerblue',linestyle='-',zorder=1)
                         plt.text(0.05,1.1,'$\sigma$ ='+"{0:.2e}".format(mean_disp),verticalalignment='center', horizontalalignment='left',fontsize=10.,zorder=10,color='black',transform=plt.gca().transAxes) 
                         
                         #Frame                         
                         dx_range=x_range_loc[1]-x_range_loc[0]        
                         dy_range=y_range_loc[1]-y_range_loc[0]                         
-                        xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                        ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)
+                        xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                        ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)
                         custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                     x_title=r'Orbital Phase',y_title='Dispersion',font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                         plt.savefig(path_loc+molec+'_disp.'+plot_dic['tell_CCF']) 
                         plt.close() 
 
 
 
@@ -5341,19 +5407,19 @@
         plot_set_key = plot_settings[key_plot]    
     
         print('-----------------------------------')
         print('+ Telluric properties')
 
         #Process original visits   
         for inst in np.intersect1d(data_dic['instrum_list'],list(plot_set_key['visits_to_plot'].keys())): 
-            print('      - Instrument :',inst)
+            print('   - Instrument :',inst)
             if inst not in plot_set_key['color_dic']:plot_set_key['color_dic'][inst]={}
             
             for vis in np.intersect1d(list(data_dic[inst].keys()),plot_set_key['visits_to_plot'][inst]): 
-                print('        - Visit :',vis)
+                print('     - Visit :',vis)
                 if vis not in plot_set_key['color_dic'][inst]:plot_set_key['color_dic'][inst][vis]='dodgerblue'
                 data_vis = data_dic[inst][vis]
                 cen_ph_vis = coord_dic[inst][vis][plot_set_key['pl_ref'][inst][vis]]['cen_ph']
                 
                 #Create directory if required
                 path_loc = gen_dic['save_plot_dir']+'Spec_raw/Tell_corr/'+inst+'_'+vis+'/Tell_prop/'
                 if not os_system.path.exists(path_loc):os_system.makedirs(path_loc)  
@@ -5418,16 +5484,16 @@
                             else:
                                 ymin = np.min(tell_prop[molec][key][0][cond_def][sub_cond_def]-tell_prop[molec][key][1][cond_def][sub_cond_def])
                                 ymax = np.max(tell_prop[molec][key][0][cond_def][sub_cond_def]+tell_prop[molec][key][1][cond_def][sub_cond_def])
                                 dy_range = ymax-ymin
                                 y_range_loc = [ymin-0.05*dy_range,ymax+0.05*dy_range]  
                             dx_range=x_range_loc[1]-x_range_loc[0]        
                             dy_range=y_range_loc[1]-y_range_loc[0]     
-                            xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                            ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)
+                            xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                            ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)
                             y_title = {'Temperature':'Temperature (K)','IWV_LOS':'Column density (cm$^{-2}$)','Pressure_ground':'Pressure (atm)'}[key]
                             custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                         x_title='Orbital phase',y_title=y_title,font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                             plt.savefig(path_loc+molec+'_'+key+'.'+plot_dic['tell_prop']) 
                             plt.close()  
             
             
@@ -5496,16 +5562,18 @@
                 #Horizontal range
                 if plot_set_key['x_range'] is not None:x_range_loc = deepcopy(plot_set_key['x_range'])
                 else:
                     data_com = np.load(data_vis['proc_com_data_paths']+'.npz',allow_pickle=True)['data'].item() 
                     if plot_set_key['sp_var'] == 'nu' :x_range_loc = [c_light/data_com['edge_bins'][-1,-1],c_light/data_com['edge_bins'][0,0]]
                     elif plot_set_key['sp_var'] == 'wav' :x_range_loc = [data_com['edge_bins'][0,0],data_com['edge_bins'][-1,-1]]
                 if plot_set_key['plot_model']:
-                    if plot_set_key['sp_var'] == 'wav' :min_wav,max_wav = x_range_loc[0],x_range_loc[1]
-                    elif plot_set_key['sp_var'] == 'nu' :min_wav,max_wav = c_light/x_range_loc[1],c_light/x_range_loc[0] 
+                    if plot_set_key['sp_var'] == 'wav' :
+                        min_wav,max_wav = x_range_loc[0],x_range_loc[1]
+                    elif plot_set_key['sp_var'] == 'nu' :
+                        min_wav,max_wav = c_light/x_range_loc[1],c_light/x_range_loc[0] 
                     nspec_plot = int( np.floor(   np.log(max_wav/min_wav)/np.log( plot_set_key['dlnw_plot'] + 1. ) )  ) 
                     cen_bin_plot = min_wav*( plot_set_key['dlnw_plot'] + 1. )**(0.5+np.arange(nspec_plot))  
                     nu_bin_plot = c_light/cen_bin_plot[::-1]
 
                 #Binned ratio of spectrum with stellar reference, measured and fitted
                 if (inst in plot_set_key['iexp_plot']) and (vis in plot_set_key['iexp_plot'][inst]) and (len(plot_set_key['iexp_plot'][inst][vis])>0):iexp_plot_vis = deepcopy(plot_set_key['iexp_plot'][inst][vis])
                 else:iexp_plot_vis=np.arange(data_vis['n_in_visit'])
@@ -5527,17 +5595,20 @@
                         y_max=np.max([np.max(lev_exp+Fbal_T_binned_plot),y_max]) 
                         for cen_bin,val_bin,cond_bin in zip(Fbal_cen_bin_plot,Fbal_T_binned_plot,cond_fit_plot):
                             markerfacecolor = col_visit[iexp] if cond_bin else 'None'
                             plt.plot(cen_bin,lev_exp+val_bin,linestyle='',marker='o',markerfacecolor=markerfacecolor  ,markeredgecolor=col_visit[iexp],markersize=plot_set_key['markersize'],rasterized=plot_set_key['rasterized'])
 
                     #Best-fit model
                     if plot_set_key['plot_model']:
-                        y_mod = data_Fbal['corr_func'](nu_bin_plot)
-                        if plot_set_key['sp_var'] == 'nu' :mod_cen_bin_plot = nu_bin_plot
-                        elif plot_set_key['sp_var'] == 'wav' :mod_cen_bin_plot = cen_bin_plot
+                        if plot_set_key['sp_var'] == 'nu' :
+                            mod_cen_bin_plot = nu_bin_plot
+                            y_mod = data_Fbal['corr_func'](nu_bin_plot)
+                        elif plot_set_key['sp_var'] == 'wav' :
+                            mod_cen_bin_plot = cen_bin_plot
+                            y_mod = data_Fbal['corr_func'](nu_bin_plot[::-1])
                         plt.plot(mod_cen_bin_plot,lev_exp+y_mod,linestyle='-',color=col_visit[iexp],lw=1) 
 
                     #Plot exposure indexes
                     if plot_set_key['plot_expid']:
                         if plot_set_key['plot_data']:ytxt = np.median(Fbal_T_binned_plot)
                         if plot_set_key['plot_model']: ytxt = np.median(y_mod)
                         plt.text(x_range_loc[1]+0.01*(x_range_loc[1]-x_range_loc[0]),lev_exp+ytxt,str(iexp),verticalalignment='center', horizontalalignment='left',fontsize=5.,zorder=15,color=col_visit[iexp]) 
@@ -5575,16 +5646,16 @@
                     for iord in np.arange(0,len(cen_ord),ord_freq):
                         plt.text(cen_ord[iord],y_range_loc[1]+delt_txt*dy_range,str(iord),verticalalignment='center', horizontalalignment='center',fontsize=fontsize_ord,zorder=15,color='black') 
                         plt.plot([cen_ord[iord],cen_ord[iord]],y_range_loc,linestyle='--',zorder=-15,color='darkgrey',lw=1) 
             
                 #Plot frame  
                 if plot_set_key['title']:plt.title('Global flux balance for visit '+vis+' in '+inst)               
                 dx_range=x_range_loc[1]-x_range_loc[0]
-                xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)     
+                xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)     
                 if plot_set_key['sp_var'] == 'nu' :x_title=r'$\nu$ (10$^{-10}$s$^{-1}$)'
                 elif plot_set_key['sp_var'] == 'wav' :x_title='Wavelength (A)'
                 custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
                             xmajor_int=xmajor_int,xminor_int=xminor_int,xmajor_form=xmajor_form,
                             ymajor_int=ymajor_int,yminor_int=yminor_int,ymajor_form=ymajor_form,
                             # x_mode='log',
                             x_title=x_title,y_title='Flux ratio',
@@ -5726,17 +5797,20 @@
                     y_max=np.max([np.max(lev_exp+Fbal_T_binned_plot),y_max]) 
                     for cen_bin,val_bin,cond_bin in zip(Fbal_cen_bin_plot,Fbal_T_binned_plot,cond_fit_plot):
                         markerfacecolor = col_visit if cond_bin else 'None'
                         plt.plot(cen_bin,lev_exp+val_bin,linestyle='',marker='o',markerfacecolor=markerfacecolor  ,markeredgecolor=col_visit,markersize=plot_set_key['markersize'],rasterized=plot_set_key['rasterized'])
 
                 #Best-fit model
                 if plot_set_key['plot_model']:
-                    y_mod = data_Fbal['corr_func_vis'](nu_bin_plot)
-                    if plot_set_key['sp_var'] == 'nu' :mod_cen_bin_plot = nu_bin_plot
-                    elif plot_set_key['sp_var'] == 'wav' :mod_cen_bin_plot = cen_bin_plot
+                    if plot_set_key['sp_var'] == 'nu' :
+                        mod_cen_bin_plot = nu_bin_plot
+                        y_mod = data_Fbal['corr_func_vis'](nu_bin_plot)
+                    elif plot_set_key['sp_var'] == 'wav' :
+                        mod_cen_bin_plot = cen_bin_plot
+                        y_mod = data_Fbal['corr_func_vis'](nu_bin_plot)[::-1]
                     plt.plot(mod_cen_bin_plot,lev_exp+y_mod,linestyle='-',color=col_visit,lw=1) 
 
                 #Plot visit names
                 if plot_set_key['plot_expid']:
                     if plot_set_key['plot_data']:ytxt = np.median(Fbal_T_binned_plot)
                     if plot_set_key['plot_model']: ytxt = np.median(y_mod)
                     plt.text(x_range_loc[1]+0.01*(x_range_loc[1]-x_range_loc[0]),lev_exp+ytxt,vis,verticalalignment='center', horizontalalignment='left',fontsize=5.,zorder=15,color=col_visit) 
@@ -5772,16 +5846,16 @@
                 for iord in np.arange(0,len(cen_ord),ord_freq):
                     plt.text(cen_ord[iord],y_range_loc[1]+delt_txt*dy_range,str(iord),verticalalignment='center', horizontalalignment='center',fontsize=fontsize_ord,zorder=15,color='black') 
                     plt.plot([cen_ord[iord],cen_ord[iord]],y_range_loc,linestyle='--',zorder=-15,color='darkgrey',lw=1) 
         
             #Plot frame  
             if plot_set_key['title']:plt.title('Global flux balance for instrument '+inst)               
             dx_range=x_range_loc[1]-x_range_loc[0]
-            xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-            ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)     
+            xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+            ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)     
             if plot_set_key['sp_var'] == 'nu' :x_title=r'$\nu$ (10$^{-10}$s$^{-1}$)'
             elif plot_set_key['sp_var'] == 'wav' :x_title='Wavelength (A)'
             custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
                         xmajor_int=xmajor_int,xminor_int=xminor_int,xmajor_form=xmajor_form,
                         ymajor_int=ymajor_int,yminor_int=yminor_int,ymajor_form=ymajor_form,
                         # x_mode='log',
                         x_title=x_title,y_title='Flux ratio',
@@ -5957,14 +6031,15 @@
 
 
     ################################################################################################################ 
     #%%% Cosmics correction
     ################################################################################################################ 
     if ('cosm_corr' in plot_settings): 
         key_plot = 'cosm_corr'
+        plot_set_key=plot_settings[key_plot]
 
         print('-----------------------------------')
         print('+ Plotting cosmics correction')
         
         #Process original visits
         for inst in np.intersect1d(data_dic['instrum_list'],list(plot_set_key['visits_to_plot'].keys())): 
             print('  > Instrument: '+inst)
@@ -6032,16 +6107,16 @@
                             #Threshold
                             plt.plot(x_range_loc,[0,0],linestyle='--',color='grey',lw=1)
                             plt.plot(x_range_loc,[gen_dic['cosm_thresh'][inst][vis],gen_dic['cosm_thresh'][inst][vis]],linestyle='--',color='red',lw=1)
                             
                             #Plot frame  
                             if plot_set_key['title']:plt.title('Cosmics detections for visit '+vis+' in '+inst)
                             dx_range=x_range_loc[1]-x_range_loc[0]
-                            xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                            ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)  
+                            xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                            ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)  
                             custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
                                         xmajor_int=xmajor_int,xminor_int=xminor_int,xmajor_form=xmajor_form,
                                         ymajor_int=ymajor_int,yminor_int=yminor_int,ymajor_form=ymajor_form,
                                         x_title='Wavelength in input rest frame (A)',y_title='(F-<F$_\mathrm{compl}$>)/$\sigma$',
                                         font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                             if gen_dic['type'][inst]=='spec1D':str_add=''
                             elif  gen_dic['type'][inst]=='spec2D':str_add='_iord'+str(iord)
@@ -6066,16 +6141,16 @@
                     n_cosmics_vis_tot=n_cosmics_vis_tot*y_range_loc[1]/np.max(n_cosmics_vis_tot)
                     plt.plot(gen_dic['wav_ord_inst'][inst][order_list],n_cosmics_vis_tot,linestyle='-',color='black',rasterized=plot_set_key['rasterized'],zorder=0,drawstyle='steps-mid',lw=plot_set_key['lw_plot'])
                     
                     #Plot frame  
                     if plot_set_key['title']:plt.title('Cosmics detections for visit '+vis+' in '+inst)
                     dx_range=x_range_loc[1]-x_range_loc[0]
                     dy_range=y_range_loc[1]-y_range_loc[0]
-                    xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                    ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)  
+                    xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                    ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)  
                     custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
                                 xmajor_int=xmajor_int,xminor_int=xminor_int,xmajor_form=xmajor_form,
                                 ymajor_int=ymajor_int,yminor_int=yminor_int,ymajor_form=ymajor_form,
                                 x_title='Wavelength in input rest frame (A)',y_title='Cosmics occurrence',
                                 font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                     plt.savefig(path_loc+'Occurrences.'+plot_dic['cosm_corr'])
                     plt.close()  
@@ -6146,16 +6221,16 @@
                         dy_range = ymax-ymin
                         y_range_loc = [ymin-0.05*dy_range,ymax+0.1*dy_range]                      
                     dx_range=x_range_loc[1]-x_range_loc[0]
                     dy_range=y_range_loc[1]-y_range_loc[0]
                       
                     #Plot frame  
                     if plot_set_key['title']:plt.title('Master for persistent peaks correction for visit '+vis+' in '+inst)
-                    xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                    ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)  
+                    xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                    ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)  
                     custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
                                 xmajor_int=xmajor_int,xminor_int=xminor_int,xmajor_form=xmajor_form,
                                 ymajor_int=ymajor_int,yminor_int=yminor_int,ymajor_form=ymajor_form,
                                 x_title='Wavelength in Earth rest frame (A)',y_title='Flux',
                                 font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                     if  gen_dic['type'][inst]=='spec1D':str_add=''
                     elif  gen_dic['type'][inst]=='spec2D':str_add='iord'+str(iord)
@@ -6255,18 +6330,17 @@
         key_plot = 'map_DI_prof'
         
         print('-----------------------------------')
         print('+ 2D map : disk-integrated stellar profiles')   
 
         #Plot map
         sub_2D_map(key_plot,plot_dic[key_plot],plot_settings[key_plot])
-                
-        
-        
-        
+
+
+
 
     ##################################################################################################
     #%%%% Binned profiles
     ##################################################################################################
     if ('map_DIbin' in plot_settings):
         key_plot = 'map_DIbin'
 
@@ -6442,14 +6516,15 @@
                          'phase':'Phase','mu':'Center-to-Limb angle','lat':'Stellar latitude','lon':'Stellar longitude','x_st':'Stellar X coordinate','y_st':'Stellar Y coordinate',
                          'AM':'Airmass','flux_airmass':'Airmass absorption','seeing':'Seeing','snr':'SNR','snr_quad':'Quadratic SNR (ESPRESSO)','snr_R':'SNR ratio','colcorrmin':r'C$_\mathrm(corr}^\mathrm{min}$', 'colcorrmax':r'C$_\mathrm(corr}^\mathrm{max}$', 'colcorrR':r'C$_\mathrm(corr}^\mathrm{ratio}$','colcorr450':r'C$_\mathrm(corr}^\mathrm{450nm}$', 'colcorr550':r'C$_\mathrm(corr}^\mathrm{550nm}$', 'colcorr650':r'C$_\mathrm(corr}^\mathrm{650nm}$',\
                          'PSFx':'', 'PSFy':'','PSFr':'','PSFang':'',
                          'glob_flux_sc':'Global flux scaling','satur_check':'Saturation check','ADC1 POS':'ESPRESSO ADC1 Position','ADC1 RA':'ESPRESSO ADC1 Right Ascension','ADC1 DEC':'ESPRESSO ADC1 Declination','ADC2 POS':'ESPRESSO ADC2 Position','ADC2 RA':'ESPRESSO ADC2 Right Ascension','ADC2 DEC':'ESPRESSO ADC2 Declination',
                          'alt':'Telescope altitude','az':'Azimuth angle','TILT1 VAL1':'ESPRESSO TILT1 VAL1','TILT1 VAL2':'ESPRESSO TILT1 VAL2','TILT2 VAL1':'ESPRESSO TILT2 VAL1','TILT2 VAL2':'ESPRESSO TILT2 VAL2'}
             for ideg in range(1,5):txt_print['c'+str(ideg)+'_pol']=r'Polynomial continuum (deg. '+str(ideg)+')'
             for ideg in range(0,11):txt_print['PC'+str(ideg)]=r'Coefficient PCA (deg. '+str(ideg)+')'
+            print('   ---------------')
             print('   > '+txt_print[plot_prop])
 
             #%%%%% Plot   
             sub_plot_CCF_prop(plot_prop,plot_settings[key_plot],'DI')  
             		 
                 
             
@@ -6655,16 +6730,16 @@
                 if plot_set_key['line_rej_range']:
                     plot_shade_range(ax,plot_info['line_rej_range'],x_range_loc,y_range_loc,mode='fill',zorder=4)    
     
                 #Plot unity level
                 ax.axhline(1.,color='black', lw=plot_set_key['lw_plot'],linestyle='--',zorder=10,rasterized=plot_set_key['rasterized'])              
     
                 #Frame
-                xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range) 
+                xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range) 
                 if data_type_gen=='DI':txt_rest='star'                 
                 elif data_type_gen=='Intr':txt_rest='surface'    
                 custom_axis(plt,ax=ax,position=plot_set_key['margins'] ,x_range=x_range_loc,y_range=y_range_loc,dir_y='out',dir_x='out', 
                 		    xmajor_int=xmajor_int,xminor_int=xminor_int,xmajor_form=xmajor_form,
                 		    ymajor_int=ymajor_int,yminor_int=yminor_int,ymajor_form=ymajor_form,
                             x_title='Wavelength in '+txt_rest+' rest frame (A)',y_title='Normalized flux',
                          font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
@@ -7060,16 +7135,16 @@
                         for cont_ph in contact_phases_vis:
                             plt.plot([cont_ph,cont_ph],y_range_loc,color='black',linestyle=ls_pl,lw=plot_set_key['lw_plot'])
 
                 #Plot frame                 
                 if plot_set_key['title']:plt.title('Input light curves')
                 dx_range=x_range_loc[1]-x_range_loc[0]
                 dy_range=y_range_loc[1]-y_range_loc[0]
-                xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(dx_range)
-                ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(dy_range)               
+                xmajor_int,xminor_int,xmajor_form = autom_tick_prop(dx_range)
+                ymajor_int,yminor_int,ymajor_form = autom_tick_prop(dy_range)               
                 custom_axis(plt,position=plot_set_key['margins'] ,x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
                 		     xmajor_int=xmajor_int,xminor_int=xminor_int,xmajor_form=xmajor_form,
                 		     ymajor_int=ymajor_int,yminor_int=yminor_int,ymajor_form=ymajor_form,
                          x_title='Orbital phase',y_title='Flux',
                          font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                 
                 save_path = path_loc+inst
@@ -7159,34 +7234,116 @@
                 plt.savefig(path_loc+inst+'_'+vis+'.'+plot_dic['spectral_LC'])                        
                 plt.close()  
 
 
 
 
     ################################################################################################################  
-    #%% Residual profiles
+    #%% Differential profiles
     ################################################################################################################        
         
     ################################################################################################################  
     #%%% 2D maps
     ################################################################################################################  
 
     ################################################################################################################  
-    #%%% Original profiles 
+    #%%%% Original profiles 
     ################################################################################################################  
     if ('map_Res_prof' in plot_settings):
         key_plot = 'map_Res_prof'
 
         print('-----------------------------------')
-        print('+ 2D map of residual profiles')    
+        print('+ 2D map : differential profiles')    
 
         #Plot map
         sub_2D_map(key_plot,plot_dic[key_plot],plot_settings[key_plot])
                    
 
+                
+        
+
+    ################################################################################################################  
+    #%%%%% Best-fit profiles 
+    ################################################################################################################  
+    if ('map_BF_Res_prof' in plot_settings):
+        key_plot = 'map_BF_Res_prof'
+        print('-----------------------------------')
+        print('+ 2D map : best-fit differential profiles')    
+        
+        #Plot map
+        sub_2D_map(key_plot,plot_dic[key_plot],plot_settings[key_plot])
+        
+        
+        
+        
+    ################################################################################################################  
+    #%%%%% Residual from best-fit profiles 
+    ################################################################################################################  
+    if ('map_BF_Res_prof_re' in plot_settings):
+        key_plot = 'map_BF_Res_prof_re'
+        
+        print('-----------------------------------')
+        print('+ 2D map : residuals from best-fit differential profiles') 
+        
+        #Plot map
+        sub_2D_map(key_plot,plot_dic[key_plot],plot_settings[key_plot])
+
+
+        
+    ################################################################################################################ 
+    #%%%%% Estimates and residual profiles
+    ################################################################################################################ 
+    for key_plot in ['map_Res_prof_clean_pl_est','map_Res_prof_clean_sp_est','map_Res_prof_unclean_sp_est','map_Res_prof_unclean_pl_est',
+                     'map_Res_prof_clean_sp_res','map_Res_prof_clean_pl_res','map_Res_prof_unclean_sp_res','map_Res_prof_unclean_pl_res']:
+        if (key_plot in plot_settings):
+            ##############################################################################
+            #%%%%%% Un-cleaned estimates
+            if key_plot == 'map_Res_prof_unclean_sp_est':
+                print('-----------------------------------')
+                print('+ 2D map: un-cleaned theoretical spotted profiles') 
+            
+            if key_plot == 'map_Res_prof_unclean_pl_est':
+                print('-----------------------------------')
+                print('+ 2D map: un-cleaned theoretical planet-occulted profiles') 
+            ##############################################################################
+            #%%%%%% Cleaned estimates
+            if key_plot == 'map_Res_prof_clean_sp_est':
+                print('-----------------------------------')
+                print('+ 2D map: cleaned theoretical spotted profiles') 
+            
+            if key_plot == 'map_Res_prof_clean_pl_est':
+                print('-----------------------------------')
+                print('+ 2D map: cleaned theoretical planet-occulted profiles') 
+            ##############################################################################
+            #%%%%%% Residuals    
+            if key_plot == 'map_Res_prof_clean_sp_res':
+                print('-----------------------------------')
+                print('+ 2D map: residuals from cleaned spotted profiles') 
+            if key_plot == 'map_Res_prof_clean_pl_res':
+                print('-----------------------------------')
+                print('+ 2D map: residuals from cleaned planet-occulted profiles') 
+            if key_plot == 'map_Res_prof_unclean_sp_res':
+                print('-----------------------------------')
+                print('+ 2D map: residuals from un-cleaned spotted profiles') 
+            if key_plot == 'map_Res_prof_unclean_pl_res':
+                print('-----------------------------------')
+                print('+ 2D map: residuals from un-cleaned planet-occulted profiles') 
+            
+            #Plot map
+            sub_2D_map(key_plot,plot_dic[key_plot],plot_settings[key_plot])  
+        
+        
+        
+        
+        
+        
+        
+        
+        
+        
 
 
 
     ################################################################################################################ 
     #%%% Individual profiles
     ################################################################################################################  
 
@@ -7255,16 +7412,16 @@
                             y_min=np.min([np.min(var_noise_explained),y_min])
                             y_max=np.max([np.max(var_noise_explained),y_max]) 
 
                     #Plot frame  
                     x_range_loc=plot_set_key['x_range_var'] if plot_set_key['x_range_var'] is not None else np.array([0.,n_pc])
                     y_range_loc=plot_set_key['y_range_var'] if plot_set_key['y_range_var'] is not None else np.array([y_min,y_max])
                     if plot_set_key['title']:plt.title('PC variance for visit '+vis+' in '+inst)
-                    xmajor_int,xminor_int,xmajor_form=autom_x_tick_prop(x_range_loc[1]-x_range_loc[0])
-                    ymajor_int,yminor_int,ymajor_form=autom_y_tick_prop(y_range_loc[1]-y_range_loc[0]) 
+                    xmajor_int,xminor_int,xmajor_form=autom_tick_prop(x_range_loc[1]-x_range_loc[0])
+                    ymajor_int,yminor_int,ymajor_form=autom_tick_prop(y_range_loc[1]-y_range_loc[0]) 
                     custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
                                 xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,
                                 xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                 x_title='PC',y_title='Variance explained (%)',
                                 font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                     plt.savefig(path_loc+inst+'_'+vis+'_PCvar.'+plot_dic['pca_ana']) 
                     plt.close()                 
@@ -7298,16 +7455,16 @@
                     #Contacts
                     y_range_loc=plot_set_key['y_range_rms'] if plot_set_key['y_range_rms'] is not None else np.array([y_min,y_max])
                     for cont_ph in contact_phases[pl_ref]:plt.plot([cont_ph,cont_ph],y_range_loc,color='black',linestyle=':',lw=plot_set_key['lw_plot'],zorder=0)
 
                     #Plot frame  
                     x_range_loc=plot_set_key['x_range_rms'] if plot_set_key['x_range_rms'] is not None else np.array([np.min(cen_ph),np.max(cen_ph)])
                     if plot_set_key['title']:plt.title('RMS for visit '+vis+' in '+inst)
-                    xmajor_int,xminor_int,xmajor_form=autom_x_tick_prop(x_range_loc[1]-x_range_loc[0])
-                    ymajor_int,yminor_int,ymajor_form=autom_y_tick_prop(y_range_loc[1]-y_range_loc[0]) 
+                    xmajor_int,xminor_int,xmajor_form=autom_tick_prop(x_range_loc[1]-x_range_loc[0])
+                    ymajor_int,yminor_int,ymajor_form=autom_tick_prop(y_range_loc[1]-y_range_loc[0]) 
                     custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
                                 xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,
                                 xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                 x_title='Orbital phase',y_title='RMS',
                                 font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                     plt.savefig(path_loc+inst+'_'+vis+'_PCrms.'+plot_dic['pca_ana']) 
                     plt.close()           
@@ -7344,16 +7501,16 @@
                     x_range_loc=plot_set_key['x_range_bic'] if plot_set_key['x_range_bic'] is not None else np.array([np.min(cen_ph),np.max(cen_ph)])
                     y_range_loc=plot_set_key['y_range_bic'] if plot_set_key['y_range_bic'] is not None else np.array([y_min,y_max])
                     for cont_ph in contact_phases[pl_ref]:plt.plot([cont_ph,cont_ph],y_range_loc,color='black',linestyle=':',lw=plot_set_key['lw_plot'],zorder=0)
                     plt.plot(x_range_loc,[0.,0.],color='black',linestyle='--',lw=plot_set_key['lw_plot'],zorder=0)
 
                     #Plot frame  
                     if plot_set_key['title']:plt.title('Delta-BIC for visit '+vis+' in '+inst)
-                    xmajor_int,xminor_int,xmajor_form=autom_x_tick_prop(x_range_loc[1]-x_range_loc[0])
-                    ymajor_int,yminor_int,ymajor_form=autom_y_tick_prop(y_range_loc[1]-y_range_loc[0]) 
+                    xmajor_int,xminor_int,xmajor_form=autom_tick_prop(x_range_loc[1]-x_range_loc[0])
+                    ymajor_int,yminor_int,ymajor_form=autom_tick_prop(y_range_loc[1]-y_range_loc[0]) 
                     custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
                                 xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,
                                 xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                 x_title='Orbital phase',y_title='Delta-BIC',
                                 font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                     plt.savefig(path_loc+inst+'_'+vis+'_PCdBIC.'+plot_dic['pca_ana']) 
                     plt.close()               
@@ -7470,16 +7627,16 @@
                         y_max=np.max([np.max(data_upload['eig_res_matr'][ipc]),y_max])                      
     
                     #Plot frame  
                     x_range_loc=plot_set_key['x_range_pc'] if plot_set_key['x_range_pc'] is not None else np.array([np.min(data_upload['cen_bins']),np.max(data_upload['cen_bins'])])
                     plt.plot(x_range_loc,[0,0],color='black',linestyle='--')
                     y_range_loc=plot_set_key['y_range_pc'] if plot_set_key['y_range_pc'] is not None else np.array([y_min,y_max])
                     if plot_set_key['title']:plt.title('PC profiles for visit '+vis+' in '+inst)
-                    xmajor_int,xminor_int,xmajor_form=autom_x_tick_prop(x_range_loc[1]-x_range_loc[0])
-                    ymajor_int,yminor_int,ymajor_form=autom_y_tick_prop(y_range_loc[1]-y_range_loc[0]) 
+                    xmajor_int,xminor_int,xmajor_form=autom_tick_prop(x_range_loc[1]-x_range_loc[0])
+                    ymajor_int,yminor_int,ymajor_form=autom_tick_prop(y_range_loc[1]-y_range_loc[0]) 
                     custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
                                 xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,
                                 xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                 x_title='Velocity in star rest frame (km/s)',y_title='PC profile',
                                 font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                     plt.savefig(path_loc+inst+'_'+vis+'_PCprof.'+plot_dic['pca_ana']) 
                     plt.close()  
@@ -7514,16 +7671,16 @@
                         #Plot frame  
                         y_range_loc=plot_set_key['y_range_fft'] if plot_set_key['y_range_fft'] is not None else np.array([y_min,y_max])
                         if plot_set_key['title']:
                             if fft_loc=='res':txt = 'residual profiles'
                             elif fft_loc=='corr':txt = 'corr. residual profiles'
                             elif fft_loc=='boot':txt = 'boot. corr. residual profiles'
                             plt.title('FFT from '+txt+' for visit '+vis+' in '+inst)
-                        xmajor_int,xminor_int,xmajor_form=autom_x_tick_prop(x_range_loc[1]-x_range_loc[0])
-                        ymajor_int,yminor_int,ymajor_form=autom_y_tick_prop(y_range_loc[1]-y_range_loc[0]) 
+                        xmajor_int,xminor_int,xmajor_form=autom_tick_prop(x_range_loc[1]-x_range_loc[0])
+                        ymajor_int,yminor_int,ymajor_form=autom_tick_prop(y_range_loc[1]-y_range_loc[0]) 
                         custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
                                     xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,
                                     xmajor_form=xmajor_form,ymajor_form=ymajor_form,
                                     x_title='Velocity in star rest frame (km/s)',y_title='max(| FFT |)^2',
                                     font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
                         plt.savefig(path_loc+inst+'_'+vis+'_FFTprof_'+fft_loc+'.'+plot_dic['pca_ana']) 
                         plt.close()  
@@ -7657,27 +7814,27 @@
 
         #Plot map
         sub_2D_map(key_plot,plot_dic[key_plot],plot_settings[key_plot])
                    
 
 
     ################################################################################################################ 
-    #%%%% Estimates for intrinsic stellar profiles, residuals from observed profiles
+    #%%%% Estimate and residual profiles
     ################################################################################################################ 
     for key_plot in ['map_Intr_prof_est','map_Intr_prof_res']:
         if (key_plot in plot_settings):
 
             ##############################################################################
-            #%%%% Estimates
+            #%%%%% Estimates
             if key_plot == 'map_Intr_prof_est':
                 print('-----------------------------------')
                 print('+ 2D map: theoretical intrinsic stellar profiles') 
 
             ##############################################################################
-            #%%%% Residuals    
+            #%%%%% Residuals    
             if key_plot == 'map_Intr_prof_res':
                 print('-----------------------------------')
                 print('+ 2D map: residuals from intrinsic stellar profiles') 
 
             #Plot map
             sub_2D_map(key_plot,plot_dic[key_plot],plot_settings[key_plot])    
 
@@ -7846,15 +8003,15 @@
                     new_x_high = np.array(bin_prop['bin_high'])   
                 elif 'bin_range' in bin_prop:
                     min_x = bin_prop['bin_range'][0]
                     max_x = bin_prop['bin_range'][1]
                     new_dx =  (max_x-min_x)/bin_prop['nbins']
                     new_nx = int((max_x-min_x)/new_dx)
                     new_x_low = min_x + new_dx*np.arange(new_nx)
-                    new_x_high = new_x_low_in+new_dx 
+                    new_x_high = new_x_low+new_dx 
             
             #Plot all visits
             vis_list = np.intersect1d(list(data_dic[inst].keys()),plot_set_key['visits_to_plot'][inst])
             y_min=-5.*plot_set_key['y_gap']
             y_max=0.
             if plot_set_key['x_range'] is None:stop('Define plot range')
             for ivis,vis in enumerate(vis_list): 
@@ -7905,16 +8062,16 @@
             else:
                 dx_range = x_max-x_min
                 x_range_loc = np.array([x_min-0.05*dx_range,x_max+0.05*dx_range])   
             if plot_set_key['y_range'] is not None:y_range_loc=plot_set_key['y_range'] 
             else:
                 dy_range = y_max-y_min
                 y_range_loc = np.array([y_min-0.05*dy_range,y_max+0.05*dy_range])                          
-            xmajor_int,xminor_int,xmajor_form=autom_x_tick_prop(x_range_loc[1]-x_range_loc[0])
-            ymajor_int,yminor_int,ymajor_form=autom_y_tick_prop(y_range_loc[1]-y_range_loc[0]) 
+            xmajor_int,xminor_int,xmajor_form=autom_tick_prop(x_range_loc[1]-x_range_loc[0])
+            ymajor_int,yminor_int,ymajor_form=autom_tick_prop(y_range_loc[1]-y_range_loc[0]) 
             custom_axis(plt,position=plot_set_key['margins'],x_range=x_range_loc,y_range=y_range_loc,dir_y='out', 
             		     xmajor_int=xmajor_int,xminor_int=xminor_int,xmajor_form=xmajor_form,
             		     ymajor_int=None,yminor_int=yminor_int,ymajor_form=ymajor_form,
                          x_title=x_title,
                          y_title='Exposures',
                          font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
             plt.savefig(path_loc+inst+'_'+plot_set_key['x_prop']+'.'+plot_dic['plocc_ranges'])                        
@@ -7963,14 +8120,15 @@
         print('+ Properties of intrinsic stellar profiles')
 
         #%%%% Processing properties      
         for plot_prop in plot_settings['prop_Intr_ordin']:
             key_plot = 'prop_Intr_'+plot_prop 
             txt_print = {'rv':'RV','rv_res':'RV residuals','rv_l2c':'RV lobe-to-core difference','RV_lobe':'Lobe RV','FWHM':'FWHM','FWHM_voigt':'','FWHM_l2c':'FWHM lobe-to-core ratio','FWHM_lobe':'Lobe FWHM','true_FWHM':'True FWHM',
                          'ctrst':'Contrast','true_ctrst':'True contrast','amp':'Amplitude','amp_l2c':'Amplitude lobe-to-core ratio','amp_lobe':'Lobe amplitude','area':'Area','a_damp':'Damping coefficient'}
+            print('   ---------------')
             print('   > '+txt_print[plot_prop])
 
             #%%%%% Plot routine   
             sub_plot_CCF_prop(plot_prop,plot_settings[key_plot],'Intr')                  
 
 
         
@@ -8026,29 +8184,55 @@
                 #Identifying original or binned data
                 orig_vis = vis.split('_bin')[0]
                 if 'bin' in vis:data_type = 'Intrbin'
                 else:data_type = 'Introrig'           
                 if orig_vis in list(data_dic['Res'][inst].keys()):
                     plt.ioff()        
                     fig = plt.figure(figsize=(size_x,size_y))
-        
+
                     #Oblate star
-                    #    - see definition of star boundary in 'system_view'
-                    if system_param['star']['f_GD']>0.:                        
-                        cen_sub=-1.+(np.arange(1000)+0.5)*d_sub            
-                        xy_sky_grid=np.array(list(it_product(cen_sub,cen_sub))) 
-                        x_grid_all = xy_sky_grid[:,0] 
-                        y_grid_all = xy_sky_grid[:,1]                        
-                        cond_in_stphot=calc_zLOS_oblate(x_grid_all,y_grid_all,system_param['star']['istar_rad'],system_param['star']['RpoleReq'])[2]               
-                        y_grid_all[~cond_in_stphot] = 0.         
-                        ysky_limb = np.nanmax(y_grid_all,axis=1)            
-                        xsky_limb = np.append(xsky_limb,xsky_limb[::-1])             
-                        ysky_limb = np.append(ysky_limb,-ysky_limb[::-1])
-                        plt.plot(xsky_limb,ysky_limb,zorder=1, color='black',lw=1)
-        
+                    #    - see definition of star boundary in 'system_view'        
+                    if system_param['star']['f_GD']>0.: 
+                        #Oblate star parameters
+                        star_params = system_param['star']
+                        Rpole = star_params['RpoleReq']
+                        mRp2 = (1. - Rpole**2.)
+                        istar_rad=star_params['istar_rad']
+                        ci = cos(istar_rad)
+                        si = sin(istar_rad)  
+                        #X position initialization
+                        r_inner=1.
+                        r_outer=1.7
+                        x_annulus = np.linspace(-r_outer, r_outer, 3000, endpoint=True)
+                        #Oblate star
+                        #there is no simple expression of the projection of the photosphere envelope in the plane of the sky
+                        #for each x value of the grid, we thus find the condition for y values on a grid to belong to the photosphere (ie, having defined z values), and we take the maximum of the y values fulfilling the condition   
+                        ygrid = np.linspace(-1., 1., 3000, endpoint=True)
+                        y_grid_all = np.tile(ygrid,(3000,1)) 
+                        Aquad =  1. - si**2.*mRp2 
+                        r_grid2 = x_annulus[:,None]**2.+ y_grid_all**2. 
+                        Bquad = 2.*y_grid_all*ci*si*mRp2        
+                        Cquad_in = y_grid_all**2.*si**2.*mRp2 + Rpole**2.*(r_grid2 - r_inner**2.)   
+                        det_in = Bquad**2.-4.*Aquad*Cquad_in
+                        cond_in = det_in<0.
+                        y_grid_in = deepcopy(y_grid_all)                
+                        y_grid_in[cond_in] = 0.         
+                        yin_up = np.nanmax(y_grid_in,axis=1)
+                        yin_down = -yin_up            
+                        #Finding the spot where we the yin_up values go to 0, so as to keep one of the zeros for plotting.
+                        #Finding indexes where yin_up is zero.
+                        up_zeros_indexes = np.where(yin_up==0)
+                        #Finding indexes where the zero to non-zero value switch occurs (happens at two places).
+                        zero_shift_index_low = np.where(np.diff(up_zeros_indexes[0])>1)[0][0]
+                        zero_shift_index_high = up_zeros_indexes[0][zero_shift_index_low+1]
+                        #The spot where we swap from zero to non-zero values is the same in yin_up and yin_down.
+                        #Plotting the oblate star outline
+                        plt.plot(x_annulus[zero_shift_index_low:zero_shift_index_high+1], yin_up[zero_shift_index_low:zero_shift_index_high+1], color="black",zorder=0,lw=1)
+                        plt.plot(x_annulus[zero_shift_index_low:zero_shift_index_high+1], yin_down[zero_shift_index_low:zero_shift_index_high+1], color="black",zorder=0,lw=1)  
+
                     #Spherical star
                     else: 
                         star_circle=plt.Circle((0.,0.),1.,color='black',fill=False,lw=1,zorder=0)   
                         fig.gca().add_artist(star_circle)
 
                     #Planet orbit
                     #    - 'coord_orbit' is defined in the Sky-projected orbital frame: Xsky,Ysky,Zsky	
@@ -8554,14 +8738,17 @@
 
         #Making a GIF if we have multiple exposures of the system
         if (plot_set_key['t_BJD'] is not None) and plot_set_key['GIF_generation']:
             if plot_dic['system_view']!='png':stop('GIF generation requires png format')
 
             #Initialize a list to store the images used to make the GIF.
             images_to_make_GIF = [] 
+
+            #Initializing a list to store the image paths.
+            filenames = []
             
         else:images_to_make_GIF = None
         
         #Processing exposures
         for idx_pl,plot_t in enumerate(plot_series):
             
             #--------------------------------------------
@@ -8867,90 +9054,133 @@
                     else:alph_loc = 0.3
                     plt.plot(coord_Spole[0],coord_Spole[1],zorder=4., color='black',marker='o',markersize=6,alpha = alph_loc,markerfacecolor='black') 
                 
 
             #-------------------------------------------------------
             #Spotted cells 
             #-------------------------------------------------------
-            if (1==0) and mock_dic['use_spots']:    #Samson: plotting spots should not depend on the use of mock_dic
-                #Retrieve spot parameters defined by the user in plot_settings, if they are provided.
-                if len(plot_set_key['stellar_spot'])>0:
+            if plot_set_key['plot_spots']:
+
+                #Custom spot properties
+                if len(plot_set_key['custom_spot_prop'])>0:
+                    if idx_pl==0: print('   + With custom spot properties')
+
                     # Initialize params to use the retrieve_spots_prop_from_param function.
                     params = {'cos_istar' : star_params['cos_istar'], 'alpha_rot' : star_params['alpha_rot'], 'beta_rot' : star_params['beta_rot'] }        
-                    for spot in plot_set_key['stellar_spot'] : 
-                        params['lat__IS__VS__SP'+spot]     = plot_set_key['stellar_spot'][spot]['lat']
-                        params['ang__IS__VS__SP'+spot]     = plot_set_key['stellar_spot'][spot]['ang']
-                        params['Tcenter__IS__VS__SP'+spot] = plot_set_key['stellar_spot'][spot]['Tcenter']
-                        params['atten__IS__VS__SP'+spot]    = plot_set_key['stellar_spot'][spot]['atten']
-                else:
-                # If the user did not provide any spot properties for the plotting (ANTARESS_plot_settings.py) then default to
-                # the spot properties from the first instrument and visit provided in the mock dictionary section for the spots.
+                    for spot in plot_set_key['custom_spot_prop'] : 
+                        params['lat__IS__VS__SP'+spot]     = plot_set_key['custom_spot_prop'][spot]['lat']
+                        params['ang__IS__VS__SP'+spot]     = plot_set_key['custom_spot_prop'][spot]['ang']
+                        params['Tcenter__IS__VS__SP'+spot] = plot_set_key['custom_spot_prop'][spot]['Tcenter']
+                        params['ctrst__IS__VS__SP'+spot]    = plot_set_key['custom_spot_prop'][spot]['ctrst']
+                    
+                #Mock dataset spot properties
+                elif plot_set_key['mock_spot_prop']:
+                    if idx_pl==0: print('   + With mock dataset spot properties')
+                    if (mock_dic['spots_prop'] != {}):
+                            inst_to_use = plot_set_key['inst_to_plot'][0]
+                            vis_to_use = plot_set_key['visits_to_plot'][inst_to_use][0]
+                            
+                            #Retrieve the spot parameters from the mock dictionary
+                            params = deepcopy(mock_dic['spots_prop'][inst_to_use][vis_to_use])
+                            params['cos_istar'] = star_params['cos_istar'] 
+                            params['alpha_rot'] = star_params['alpha_rot']
+                            params['beta_rot'] = star_params['beta_rot']   
+                    else:stop('Mock spot properties undefined for this system.')   
+                    
+                #Fitted spot properties
+                elif plot_set_key['fit_spot_prop']:
+                    if idx_pl==0: print('   + With fitted spot properties')
                     inst_to_use = plot_set_key['inst_to_plot'][0]
                     vis_to_use = plot_set_key['visits_to_plot'][inst_to_use][0]
-                    #Retrieve the spot parameters from the mock dictionary
-                    params = deepcopy(mock_dic['spots_prop'][inst_to_use][vis_to_use])
-                    params['cos_istar'] = star_params['cos_istar'] 
-                    params['alpha_rot'] = star_params['alpha_rot']
-                    params['beta_rot'] = star_params['beta_rot']       
-                 
-                #Retrieve spot rotational velocity
-                star_params['om_eq_spots']=star_params['veq_spots']/star_params['Rstar_km']
+                    if plot_set_key['fit_results_file'] !='':fit_res = dataload_npz(plot_set_key['fit_results_file'])
+                    else:stop('No best-fit output file provided.')
+                    params = fit_res['p_final']
+                else:stop('System view unavailable : Spot generation initialized with no spot properties provided')
+  
+                #Spot Equatorial rotation rate (rad/s)
+                if 'veq_spots' in star_params:star_params['om_eq_spots']=star_params['veq_spots']/star_params['Rstar_km']
+                else:star_params['om_eq_spots']=star_params['om_eq']
+
                 #Calculate the flux of star grid, at all the exposures considered
                 star_flux_before_spot = deepcopy(Fsurf_grid_star[:,iband])
-                for t_exp in t_all_spot :
-                    star_flux_exp = deepcopy(star_flux_before_spot)
-                    spots_prop = retrieve_spots_prop_from_param(system_param['star'], params, '_', '_', t_exp) 
 
                 #Check if we have provided times for the plotting
                 if plot_set_key['t_BJD'] is not None:
+                    
+                    #Accounting for spot overlap
+                    shared_spotted_tiles = np.zeros(len(coord_grid['x_st_sky']), dtype=bool)
+                                        
                     #Defining a new flux array, such that we don't see the previous spot when plotting the next spot
                     Flux_for_nonredundant_spot_plotting = deepcopy(Fsurf_grid_star[:,iband])
-                    if len(plot_set_key['stellar_spot'])>0:
+                    if len(plot_set_key['custom_spot_prop'])>0:
                         spots_prop = retrieve_spots_prop_from_param(star_params, params, '_', '_', plot_t) 
                     else:
                         spots_prop = retrieve_spots_prop_from_param(star_params, params, inst_to_use, vis_to_use, plot_t) 
+
+                    #Defining a reference spot contrast - since all spots share the same contrast
+                    ref_ctrst = spots_prop[list(spots_prop.keys())[0]]['ctrst']
+
                     for spot in spots_prop :
-                        if spots_prop[spot]['is_visible']: 
-                            _, spotted_tiles = calc_spotted_tiles( plot_set_key['spots_prop'][spot], coord_grid['x_st_sky'], coord_grid['y_st_sky'], coord_grid['z_st_sky'], 
-                                                                   {}, {}, params, use_grid_dic = False)
+                        if spots_prop[spot]['is_center_visible']: 
                             _, spotted_tiles = calc_spotted_tiles(spots_prop[spot], coord_grid['x_st_sky'], coord_grid['y_st_sky'], coord_grid['z_st_sky'], 
-                                                                   {}, params, use_grid_dic = False)
-                                                                   
-                            star_flux_exp[spotted_tiles] *=  plot_set_key['spots_prop'][spot]['flux'] 
-                            star_flux_before_spot[spotted_tiles] *=  (1-spots_prop[spot]['atten'])
+                                                                   {}, params, use_grid_dic = False, disc_exp = False)
+
+                            #Accounting for spot overlap - figure out which cells of the stellar grid are spotted
+                            shared_spotted_tiles |= spotted_tiles
+                            
+                    #Accounting for spot overlap - all spots share the same contrast. As such we figure out which cells are spotted by either spot1, or spot2, or...
+                    #Once we have all the spotted cells we scale their flux with the shared contrast. This prevents us of counting shared cells multiple times and 
+                    #lowering their flux more than necessary.
+                    star_flux_before_spot[shared_spotted_tiles] *=  (1-ref_ctrst)
+
                     
                     if plot_set_key['spot_overlap']:      
                         Fsurf_grid_star[:,iband] = np.minimum(Fsurf_grid_star[:,iband], star_flux_before_spot)
                     else:
                         Flux_for_nonredundant_spot_plotting = np.minimum(Fsurf_grid_star[:,iband], star_flux_before_spot)
                 #If no times provided for the plotting, then generate some
                 else:
                     # Compute BJD of images 
-                    if plot_set_key['plot_spot_all_Peq'] : t_all_spot = np.linspace(   0  ,   2*np.pi/((1.-star_params['alpha_rot_spots']*sin_lat**2.-star_params['beta_rot_spots']*sin_lat**4.)*star_params['om_eq_spots']*3600.*24.) ,plot_set_key['n_image_spots'])
+                    if plot_set_key['plot_spot_all_Peq'] :
+                        #Getting reference spot and latitude
+                        for par in params:
+                            if 'lat' in par:
+                                ref_lat = params[par]
+                                break
+                        sin_lat = np.sin(ref_lat) 
+                        t_all_spot = np.linspace(0,2*np.pi/((1.-star_params['alpha_rot_spots']*sin_lat**2.-star_params['beta_rot_spots']*sin_lat**4.)*star_params['om_eq_spots']*3600.*24.),plot_set_key['n_image_spots'])
                     else:
                         dbjd =  (plot_set_key['time_range_spot'][1]-plot_set_key['time_range_spot'][0])/plot_set_key['n_image_spots']
                         n_in_visit = int((plot_set_key['time_range_spot'][1]-plot_set_key['time_range_spot'][0])/dbjd)
                         bjd_exp_low = plot_set_key['time_range_spot'][0] + dbjd*np.arange(n_in_visit)
                         bjd_exp_high = bjd_exp_low+dbjd      
                         t_all_spot = 0.5*(bjd_exp_low+bjd_exp_high) - 2400000.
                     for t_exp in t_all_spot :
                         star_flux_exp = deepcopy(star_flux_before_spot)
-                        if len(plot_set_key['stellar_spot'])>0:
+                        #Accounting for spot overlap
+                        shared_spotted_tiles = np.zeros(len(coord_grid['x_st_sky']), dtype=bool)
+                        if len(plot_set_key['custom_spot_prop'])>0:
                             spots_prop = retrieve_spots_prop_from_param(star_params, params, '_', '_', t_exp) 
                         else:
                             spots_prop = retrieve_spots_prop_from_param(star_params, params, inst_to_use, vis_to_use, t_exp) 
+                            
+                        #Defining a reference spot contrast - since all spots share the same contrast
+                        ref_ctrst = spots_prop[list(spots_prop.keys())[0]]['ctrst']
+                            
                         for spot in spots_prop :
-                            if spots_prop[spot]['is_visible']:
+                            if spots_prop[spot]['is_center_visible']:
                                 _, spotted_tiles = calc_spotted_tiles(spots_prop[spot], coord_grid['x_st_sky'], coord_grid['y_st_sky'], coord_grid['z_st_sky'], 
-                                                                        {}, params, use_grid_dic = False)
+                                                                       {}, params, use_grid_dic = False, disc_exp = False)
+
+                                #Accounting for spot overlap - figure out which cells of the stellar grid are spotted
+                                shared_spotted_tiles |= spotted_tiles
+                        
+                        star_flux_exp[shared_spotted_tiles] *=  (1-ref_ctrst)
+                        Fsurf_grid_star[:,iband] = np.minimum(Fsurf_grid_star[:,iband], star_flux_exp)
 
-                                star_flux_exp[spotted_tiles] *=  (1-spots_prop[spot]['atten'])
-                            
-                          
-                    Fsurf_grid_star[:,iband] = np.minimum(Fsurf_grid_star[:,iband], star_flux_exp)
 
         
 
     
             #------------------------------------------------------------          
             #Color table (from 0 to 1)
             #    - put '_r' at the end to reverse color table 
@@ -8964,16 +9194,16 @@
                 cmap = plt.get_cmap('YlOrRd_r')
             elif plot_set_key['disk_color']=='GD':
                 val_disk=gd_grid_star[:,iband]
                 cmap = plt.get_cmap('GnBu_r')
             elif plot_set_key['disk_color']=='F':
                 val_disk=Fsurf_grid_star[:,iband]  
                 
-                if (1==0) and mock_dic['use_spots'] and not plot_set_key['spot_overlap'] and plot_set_key['t_BJD'] is not None:
-                    val_disk = Flux_for_nonredundant_spot_plotting
+                if plot_set_key['plot_spots'] and (not plot_set_key['spot_overlap']) and (plot_set_key['t_BJD'] is not None):val_disk = Flux_for_nonredundant_spot_plotting
+
                 
                 # cmap = plt.get_cmap('GnBu_r')
                 # cmap = plt.get_cmap('jet')
                 cmap = plt.get_cmap('rainbow')
                 sc_fact10 = -np.floor(np.log10(np.abs(np.median(val_disk))))
                 val_disk*=10**sc_fact10
             min_col=0
@@ -8993,15 +9223,15 @@
             #Intensity shade
             if (plot_set_key['disk_color']=='RV') and (plot_set_key['shade_overlay']): 
                 cmap_f = plt.get_cmap('Greys_r')
                 min_f=np.nanmin(Fsurf_grid_star[:,iband])
                 max_f=np.nanmax(Fsurf_grid_star[:,iband])
                 color_f=cmap_f( (min_col+ (Fsurf_grid_star[:,iband]-min_f)*(max_col-min_col)/ (max_f-min_f)) )
 
-                if (1==0) and mock_dic['use_spots'] and not plot_set_key['spot_overlap'] and plot_set_key['t_BJD'] is not None:
+                if plot_set_key['plot_spots'] and (not plot_set_key['spot_overlap']) and (plot_set_key['t_BJD'] is not None): 
                     min_f=np.nanmin(Flux_for_nonredundant_spot_plotting)
                     max_f=np.nanmax(Flux_for_nonredundant_spot_plotting)
                     color_f=cmap_f( (min_col+ (Flux_for_nonredundant_spot_plotting-min_f)*(max_col-min_col)/ (max_f-min_f)) )
         
 
             #Disk colored with RV or specific intensity
             cond_in_plot = (coord_grid['x_st_sky']+0.5*d_stcell>=plot_set_key['x_range'][0]) & (coord_grid['x_st_sky']-0.5*d_stcell<=plot_set_key['x_range'][1])\
@@ -9081,37 +9311,40 @@
                 cb.set_array(val_disk)		
                 cbar=fig.colorbar(cb,cax=cbar_pos,format=format_cbar)	
                 cbar.ax.tick_params(labelsize=plot_set_key['font_size']) 
                 cbar.set_label(colbar_title, rotation=270,labelpad=25+2,size=plot_set_key['font_size'])	
         
             #-----------------------
             #Main axis 
-            xmajor_int,xminor_int,xmajor_form = autom_x_tick_prop(plot_set_key['x_range'][1]-plot_set_key['x_range'][0])
-            ymajor_int,yminor_int,ymajor_form = autom_y_tick_prop(plot_set_key['y_range'][1]-plot_set_key['y_range'][0])
+            xmajor_int,xminor_int,xmajor_form = autom_tick_prop(plot_set_key['x_range'][1]-plot_set_key['x_range'][0])
+            ymajor_int,yminor_int,ymajor_form = autom_tick_prop(plot_set_key['y_range'][1]-plot_set_key['y_range'][0])
             custom_axis(plt,ax=ax1,x_range=plot_set_key['x_range'],y_range=plot_set_key['y_range'],
                         xmajor_int=xmajor_int,xminor_int=xminor_int,ymajor_int=ymajor_int,yminor_int=yminor_int,
                         # xmajor_int=0.5,xminor_int=0.1,ymajor_int=0.5,yminor_int=0.1,
         #                xmajor_length=8,xminor_length=4,ymajor_length=8,yminor_length=4,
             		    xmajor_form='%.1f',ymajor_form='%.1f',
                         top_xticks='on',
                         x_title='Distance (R$_{*}$)',y_title='Distance (R$_{*}$)',
                         font_size=plot_set_key['font_size'],xfont_size=plot_set_key['font_size'],yfont_size=plot_set_key['font_size'])
             
             #-----------------------	
-            filename = path_loc+'System'+str(idx_pl)+'_'+str(plot_t)+'.'+plot_dic['system_view']		
+            filename = path_loc+'System'+str(idx_pl)+'_'+str(plot_t)+'.'+plot_dic['system_view']	
+            if images_to_make_GIF is not None:filenames += [filename]		
             plt.savefig(filename) 
             plt.close()
             
             #Store image for GIF generation
-            if images_to_make_GIF is not None:images_to_make_GIF.append(imageio.imread(filename))
+            if images_to_make_GIF is not None:images_to_make_GIF.append(imageio.v2.imread(filename))
 
         ### End of loop on plotted timesteps    
 
         #Produce and store the GIF.
-        if images_to_make_GIF is not None:imageio.mimsave(path_loc+'System.gif', images_to_make_GIF,fps=plot_set_key['fps'])
+        if images_to_make_GIF is not None:
+            imageio.mimsave(path_loc+'System.gif', images_to_make_GIF,duration=(1000 * 1/plot_set_key['fps']))
+            for film in filenames:os_system.remove(film)
 
 
 
 
 
 
 
@@ -9198,15 +9431,15 @@
     if ('all_atm_data' in plot_settings):
         key_plot = 'all_atm_data'
 
         print('-----------------------------------')
         print('+ Plotting all atmospheric profiles in each visit')
         
         #Plot        
-        sub_plot_all_prof(plot_options,'atm',plot_settings[key_plot])          
+        sub_plot_all_prof(plot_settings,'atm',plot_settings[key_plot])          
         
 
 
 
 
     ##################################################################################################
     #%%%% Original profiles
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_plots/utils_plots.py` & `antaress-1.1.1/src/antaress/ANTARESS_plots/utils_plots.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from matplotlib.ticker import MultipleLocator, FormatStrFormatter
+from matplotlib.ticker import MultipleLocator, FormatStrFormatter,ScalarFormatter
 import matplotlib.colors as colors
 import numpy as np
 from copy import deepcopy
 from ..ANTARESS_general.utils import stop
 
 
-'''
-Symbols
-'''
+#%% Symbols
 degree_sign= u'\N{DEGREE SIGN}'
 
 
-'''
-Routine to define axis properties
-'''
+#%% Routines
+
 def custom_axis(plt,ax=None,fig = None, x_range=None,y_range=None,z_range=None,position=None,colback=None,
 		    x_mode=None,y_mode=None,z_mode=None,
 		    x_title=None,y_title=None,z_title=None,x_title_dist=None,y_title_dist=None,z_title_dist=None,
 		    no_xticks=False,no_yticks=False,no_zticks=True,
 		    top_xticks=None,right_yticks=None,   
             hide_xticks = False,hide_yticks = False,		
 		    xmajor_int=None,xminor_int=None,ymajor_int=None,yminor_int=None,zmajor_int=None,zminor_int=None,
@@ -29,52 +26,60 @@
 		    axis_thick=None,xmajor_thick=None,xminor_thick=None,ymajor_thick=None,yminor_thick=None,zmajor_thick=None,zminor_thick=None,
 		    dir_x=None,dir_y=None,dir_z=None,
             xtick_pad=None,ytick_pad=None,ztick_pad=None,
             xlab_col=None,ylab_col=None,zlab_col=None,
             hide_axis=None,
             right_axis=False,secy_title=None,secy_range=None,secy_title_dist=None,no_secyticks=None,secymajor_int=None,dir_secy=None,secyfont_size=None,
             secymajor_length=None,secymajor_thick=None,secyminor_length=None,secyminor_thick=None,secymajor_form=None,secyminor_int=None,secylab_col=None):
+    r"""**Plot axis.**
     
-						
-#TODO: en fait on peut ajouter dans une figure des sousplots ou on veut avec
-#ax=fig.add_axes([left,right,width,height])    en fraction de 0,1
-							
-					
+    General routines to set up plot axis to default or user-selected values.  
+    
+    Args:
+        TBD
+    
+    Returns:
+        None
+    
+    """ 
+		
     #Font
     #    - thick: 'light', 'normal', 'medium', 'semibold', 'bold', 'heavy', 'black'					
     font_size_loc=font_size if font_size is not None else 10.
     font_thick_loc=font_thick if font_thick is not None else 'normal'
     plt.rc('font', size=font_size_loc,weight=font_thick_loc,**{'family':'sans-serif','sans-serif':['Helvetica']})
 # 	plt.rc('text', usetex=True)
     plt.rcParams['pdf.fonttype'] = 42
 
     #Axis
-    if ax==None:
-        ax=plt.gca()
+    if ax==None:ax=plt.gca()
 
     #Axis frame position
     #    - corresponds to the corners of the image
     if position is not None:
         if fig is None:plt.subplots_adjust(left=position[0],bottom=position[1],right=position[2],top=position[3]) 
         else:fig.subplots_adjust(left=position[0],bottom=position[1],right=position[2],top=position[3]) 
 
-    #Set axis to log mode if required
-    if x_mode=='log':ax.set_xscale('log')
-    if y_mode=='log':ax.set_yscale('log')
-
     #Axis ranges
     if x_range is not None:ax.set_xlim([x_range[0], x_range[1]])
     else:x_range = ax.get_xlim()
     dx_range = x_range[1]-x_range[0]
     if y_range is not None:ax.set_ylim([y_range[0], y_range[1]])
     else:y_range = ax.get_ylim()
     dy_range = y_range[1]-y_range[0]
     if z_range is not None:ax.set_zlim([z_range[0], z_range[1]])
-    # else:z_range = ax.get_zlim()
-    # dz_range = z_range[1]-z_range[0]
+
+    #Set axis to log mode if required
+    if x_mode=='log':
+        ax.set_xscale('log')
+    if y_mode=='log':
+        ax.set_yscale('log')
+    if z_mode=='log':
+        ax.set_zscale('log')
+
 
     #Axis titles	
     xfont_size_loc=xfont_size if xfont_size is not None else 10.
     yfont_size_loc=yfont_size if yfont_size is not None else 10. 
     zfont_size_loc=zfont_size if zfont_size is not None else 10. 
     if x_title is not None:
             ax.set_xlabel(x_title,fontsize=xfont_size_loc,weight=font_thick_loc)
@@ -134,16 +139,20 @@
         xminor_length_loc=xminor_length if xminor_length is not None else xmajor_length_loc/2.	
         xminor_thick_loc=xminor_thick if xminor_thick is not None else 1.5		
         ax.tick_params('x', length=xminor_length_loc, which='minor',width=xminor_thick_loc,
 					  direction=dir_x,labelsize=xfont_size_loc,top=True)
         
         #Major ticks label format		
         if xmajor_form is not None:ax.xaxis.set_major_formatter(FormatStrFormatter(xmajor_form))
+        if x_mode=='log':
+            if xmajor_form is not None:ax.xaxis.set_major_formatter(ScalarFormatter(xmajor_form))
+            else:ax.xaxis.set_major_formatter(ScalarFormatter())
 	
 	    #Interval between minor ticks	
+        if x_mode=='log':xminor_int=None
         if xminor_int is not None:ax.xaxis.set_minor_locator(MultipleLocator(xminor_int))		
 
         #Ticks labels color
         if xlab_col is not None:[i_col.set_color(xlab_col) for i_col in ax.get_xticklabels()]
 
         #Hide top ticks
         if hide_xticks:ax.xaxis.set_ticks_position('bottom')
@@ -175,16 +184,20 @@
         yminor_length_loc=yminor_length if yminor_length is not None else ymajor_length_loc/2.
         yminor_thick_loc=yminor_thick if yminor_thick is not None else 1.5			
         ax.tick_params('y', length=yminor_length_loc, which='minor',width=yminor_thick_loc,
         					  direction=dir_y,labelsize=yfont_size_loc, right=True)
 
    	    #Major ticks label format		
         if ymajor_form is not None:ax.yaxis.set_major_formatter(FormatStrFormatter(ymajor_form))	
-  
+        if y_mode=='log':
+            if ymajor_form is not None:ax.yaxis.set_major_formatter(ScalarFormatter(ymajor_form))
+            else:ax.yaxis.set_major_formatter(ScalarFormatter())    
+
 	    #Interval between minor ticks	
+        if y_mode=='log':yminor_int=None
         if yminor_int is not None:
             n_ticks = int(ymajor_int/yminor_int)
             if n_ticks>50:yminor_int = ymajor_int/50.
             ax.yaxis.set_minor_locator(MultipleLocator(yminor_int))		
 
 	    #Ticks labels color
         if ylab_col is not None:[i_col.set_color(ylab_col) for i_col in ax.get_yticklabels()]
@@ -294,106 +307,133 @@
           ax.spines['top'].set_color('white')  
           ax.spines['left'].set_color('white')  
           ax.spines['right'].set_color('white')  
     
               
     return None 
 	
-'''
-Scaling factor
-'''
+
 def scaled_title(sc_fact10,y_title):
+    r"""**Title scaling.**
+    
+    Applies power-of-ten scaling to title value.  
+    
+    Args:
+        sc_fact10 (int): power of ten scaling
+        y_title (str): title
+    
+    Returns:
+        y_title (str): title preceded by scaling value
+    
+    """ 
     if sc_fact10!=0.:
         sc_sign='-' if sc_fact10<0. else ''
         y_title='10$^{'+sc_sign+'%i' % abs(sc_fact10)+'}$ '+y_title
     return y_title                        
 
-'''
-Automatic range extension
-'''
+
+
 def autom_range_ext(ax_range_in,ax_min,ax_max,ext_fact=0.05):  
+    r"""**Automatic range.**
+    
+    Defines axis range automatically.  
+    
+    Args:
+        ax_range_in (list): axis range to be set, if user-defined
+        ax_min (float): minimum value on the axis
+        ax_max (float): maximum value on the axis
+        ext_fact (float): extension of axis on both sides compared to min and max values
+    
+    Returns:
+        ax_range (list): axis range
+    
+    """ 
+
     if ax_range_in is None:
         ax_range = np.array([ax_min,ax_max])   
         dx_range=ax_range[1]-ax_range[0]
         ax_range[0]-=ext_fact*dx_range
         ax_range[1]+=ext_fact*dx_range
         dx_range=ax_range[1]-ax_range[0]
     else:ax_range=ax_range_in
     return ax_range
 
-'''
-Automatic tick definition
-'''
-def autom_x_tick_prop(dax_range):   
-    if dax_range>1000.1:axmajor_int,axminor_int,axmajor_form=500.,100.,'%i' 
-    elif dax_range>200.1:axmajor_int,axminor_int,axmajor_form=100.,10.,'%i'     
-    elif dax_range>100.1:axmajor_int,axminor_int,axmajor_form=50.,10.,'%i' 
-    elif dax_range>50.1:axmajor_int,axminor_int,axmajor_form=10.,1.,'%i' 
-    elif dax_range>20.1:axmajor_int,axminor_int,axmajor_form=5.,1.,'%i' 
-    elif dax_range>15.1:axmajor_int,axminor_int,axmajor_form=4.,1,'%i'    
-    elif dax_range>10.1:axmajor_int,axminor_int,axmajor_form=2.,0.5,'%i'
-    elif dax_range>3.1:axmajor_int,axminor_int,axmajor_form=1.,0.5,'%i'     
-    elif dax_range>1.1:axmajor_int,axminor_int,axmajor_form=5e-1,1e-1,'%.1f'     
-    elif dax_range>5.1e-1:axmajor_int,axminor_int,axmajor_form=2e-1,1e-1,'%.1f'    
-    elif dax_range>1.1e-1:axmajor_int,axminor_int,axmajor_form=5e-2,1e-2,'%.2f'
-    elif dax_range>4.1e-2:axmajor_int,axminor_int,axmajor_form=1e-2,5e-3,'%.2f'
-    elif dax_range>1.1e-2:axmajor_int,axminor_int,axmajor_form=5e-3,1e-3,'%.3f'
-    elif dax_range>5.1e-3:axmajor_int,axminor_int,axmajor_form=2e-3,1e-3,'%.3f'    
-    elif dax_range>2.1e-3:axmajor_int,axminor_int,axmajor_form=1e-3,5e-4,'%.3f'      
-    elif dax_range>5.1e-4:axmajor_int,axminor_int,axmajor_form=5e-4,1e-4,'%.4f' 
-    elif dax_range>1.1e-4:axmajor_int,axminor_int,axmajor_form=2e-4,1e-4,'%.4f' 
-    else:axmajor_int,axminor_int,axmajor_form=None,None,None 
+
+def autom_tick_prop(dax_range):
+    r"""**Automatic ticks.**
     
+    Defines tick spacings and format automatically.  
+    
+    Args:
+        dax_range (float): axis extension
+    
+    Returns:
+        axmajor_int (float): major ticks spacing
+        axminor_int (float): minor ticks spacing
+        axmajor_form (str): major tick format
+    
+    """ 
+    if   dax_range>1e11+0.1:axmajor_int,axminor_int,axmajor_form=5e10,1e10,'%.1e' 
+    elif dax_range>1e10+0.1:axmajor_int,axminor_int,axmajor_form=5e9,1e9,'%.1e' 
+    elif dax_range>1e9+0.1: axmajor_int,axminor_int,axmajor_form=5e8,1e8,'%.1e'     
+    elif dax_range>1e8+0.1: axmajor_int,axminor_int,axmajor_form=5e7,1e7,'%.1e'     
+    elif dax_range>1e7+0.1: axmajor_int,axminor_int,axmajor_form=5e6,1e6,'%.1e' 
+    elif dax_range>1e6+0.1: axmajor_int,axminor_int,axmajor_form=5e5,1e5,'%.1e' 
+    elif dax_range>1e5+0.1: axmajor_int,axminor_int,axmajor_form=5e4,1e4,'%.1e' 
+    elif dax_range>1e4+0.1: axmajor_int,axminor_int,axmajor_form=5000.,1000.,'%.1e' 
+    elif dax_range>5e3+0.1: axmajor_int,axminor_int,axmajor_form=1000.,500.,'%i'     
+    elif dax_range>1e3+0.1: axmajor_int,axminor_int,axmajor_form=500.,100.,'%i' 
+    elif dax_range>500.1:   axmajor_int,axminor_int,axmajor_form=200.,50.,'%i' 
+    elif dax_range>200.1:   axmajor_int,axminor_int,axmajor_form=100.,10.,'%i'     
+    elif dax_range>100.1:   axmajor_int,axminor_int,axmajor_form=50.,10.,'%i' 
+    elif dax_range>50.1:    axmajor_int,axminor_int,axmajor_form=10.,1.,'%i' 
+    elif dax_range>20.1:    axmajor_int,axminor_int,axmajor_form=5.,1.,'%i' 
+    elif dax_range>15.1:    axmajor_int,axminor_int,axmajor_form=4.,1,'%i'    
+    elif dax_range>10.1:    axmajor_int,axminor_int,axmajor_form=2.,1.,'%i'
+    elif dax_range>6.1:     axmajor_int,axminor_int,axmajor_form=2.,1.,'%i' 
+    elif dax_range>3.5:     axmajor_int,axminor_int,axmajor_form=1.,0.5,'%i'  
+    elif dax_range>3.1:     axmajor_int,axminor_int,axmajor_form=1.,0.5,'%i'     
+    elif dax_range>1.1:     axmajor_int,axminor_int,axmajor_form=5e-1,1e-1,'%.1f'     
+    elif dax_range>7.1e-1:  axmajor_int,axminor_int,axmajor_form=2e-1,5e-2,'%.1f'     
+    elif dax_range>5.1e-1:  axmajor_int,axminor_int,axmajor_form=2e-1,5e-2,'%.1f'    
+    elif dax_range>3.1e-1:  axmajor_int,axminor_int,axmajor_form=1e-1,5e-2,'%.1f'     
+    elif dax_range>1.1e-1:  axmajor_int,axminor_int,axmajor_form=5e-2,1e-2,'%.2f'
+    elif dax_range>5.1e-2:  axmajor_int,axminor_int,axmajor_form=2e-2,1e-2,'%.2f'       
+    elif dax_range>4.1e-2:  axmajor_int,axminor_int,axmajor_form=1e-2,5e-3,'%.2f'
+    elif dax_range>3.1e-2:  axmajor_int,axminor_int,axmajor_form=1e-2,5e-3,'%.2f' 
+    elif dax_range>1.1e-2:  axmajor_int,axminor_int,axmajor_form=5e-3,1e-3,'%.3f'
+    elif dax_range>5.1e-3:  axmajor_int,axminor_int,axmajor_form=2e-3,1e-3,'%.3f'    
+    elif dax_range>2.1e-3:  axmajor_int,axminor_int,axmajor_form=1e-3,5e-4,'%.3f'   
+    elif dax_range>1.1e-3:  axmajor_int,axminor_int,axmajor_form=5e-4,1e-4,'%.4f'     
+    elif dax_range>5.1e-4:  axmajor_int,axminor_int,axmajor_form=5e-4,1e-4,'%.4f' 
+    elif dax_range>1.1e-4:  axmajor_int,axminor_int,axmajor_form=2e-4,1e-4,'%.4f' 
+    else:axmajor_int,axminor_int,axmajor_form=None,None,None 
     return axmajor_int,axminor_int,axmajor_form    
     
-def autom_y_tick_prop(dax_range): 
-    if dax_range>  1e11+0.1:axmajor_int,axminor_int,axmajor_form=5e10,1e10,'%.1e' 
-    elif dax_range>  1e10+0.1:axmajor_int,axminor_int,axmajor_form=5e9,1e9,'%.1e' 
-    elif dax_range>  1e9+0.1:axmajor_int,axminor_int,axmajor_form=5e8,1e8,'%.1e'     
-    elif dax_range>  1e8+0.1:axmajor_int,axminor_int,axmajor_form=5e7,1e7,'%.1e'     
-    elif dax_range>  1e7+0.1:axmajor_int,axminor_int,axmajor_form=5e6,1e6,'%.1e' 
-    elif dax_range>  1e6+0.1:axmajor_int,axminor_int,axmajor_form=5e5,1e5,'%.1e' 
-    elif dax_range>1e5+0.1:axmajor_int,axminor_int,axmajor_form=5e4,1e4,'%.1e' 
-    elif dax_range>10000.1:axmajor_int,axminor_int,axmajor_form=5000.,1000.,'%.1e' 
-    elif dax_range>5000.1:axmajor_int,axminor_int,axmajor_form=1000.,500.,'%i' 
-    elif dax_range>1000.1:axmajor_int,axminor_int,axmajor_form=500.,100.,'%i' 
-    elif dax_range>500.1:axmajor_int,axminor_int,axmajor_form=200.,50.,'%i' 
-    elif dax_range>200.1:axmajor_int,axminor_int,axmajor_form=50.,10.,'%i' 
-    elif dax_range>100.1:axmajor_int,axminor_int,axmajor_form=20.,5.,'%i' 
-    elif dax_range>50.1:axmajor_int,axminor_int,axmajor_form=10.,5.,'%i'     
-    elif dax_range>10.1:axmajor_int,axminor_int,axmajor_form=5.,1.,'%i' 
-    elif dax_range>6.1:axmajor_int,axminor_int,axmajor_form=2.,1.,'%i' 
-    elif dax_range>3.5:axmajor_int,axminor_int,axmajor_form=1.,0.5,'%i'     
-    elif dax_range>1.1:axmajor_int,axminor_int,axmajor_form=0.5,0.1,'%.1f' 
-    elif dax_range>0.71:axmajor_int,axminor_int,axmajor_form=0.2,0.05,'%.1f' 
-    elif dax_range>0.31:axmajor_int,axminor_int,axmajor_form=0.1,0.05,'%.1f'     
-    elif dax_range>0.11:axmajor_int,axminor_int,axmajor_form=0.05,0.01,'%.2f' 
-    elif dax_range>0.051:axmajor_int,axminor_int,axmajor_form=0.02,0.01,'%.2f'
-    elif dax_range>0.031:axmajor_int,axminor_int,axmajor_form=0.01,0.005,'%.2f'            
-    elif dax_range>0.011:axmajor_int,axminor_int,axmajor_form=0.005,0.001,'%.3f'
-    elif dax_range>5.1e-3:axmajor_int,axminor_int,axmajor_form=0.002,0.001,'%.3f'
-    elif dax_range>2.1e-3:axmajor_int,axminor_int,axmajor_form=0.001,0.0005,'%.3f'    
-    elif dax_range>1.1e-3:axmajor_int,axminor_int,axmajor_form=5e-4,1e-4,'%.4f'
-    elif dax_range>5.1e-4:axmajor_int,axminor_int,axmajor_form=2e-4,1e-4,'%.4f'
-    else:axmajor_int,axminor_int,axmajor_form=None,None,None  
-    return axmajor_int,axminor_int,axmajor_form
-
 
 
 
-
-'''
-Routine to adjust the size and position of the plot window, maintaining isotropy
-    #    - the variables corresponding to x and y must have the same units
-    #    - the lower left corner of the axis is set in input
-    #    - the variable 'x_pos1' and 'y_pos1' define the maximum value of the right side and the upper sides of the plot
-    #    - depending on the respective width/height of the plot, the larger side (within the axes) is set to 'max_window_size' 
-    # while the smallest side of the plot is then defined to have isotropy
-'''
 def adjust_isosize(real_bounds,xpos0,ypos0,xpos1,ypos1,max_window_size):
+    r"""**2D isotropic plot scaling.**
+    
+    Adjusts the size and position of the plot window, maintaining isotropy.
+    
+    Variables along the X and Y axis must have the same units.
+    
+    The lower left corner of the plot at `(xpos0,ypos0)` is taken as reference. 
+    The `(x_pos1,y_pos1)` defines the maximum extension of the plot at the top right corner. 
+    Depending on the respective width/height of the original plot, the larger side (within the axes) is scaled to `max_window_size` while the smallest side is then scaled by isotropy.    
+    
+    Args:
+        TBD
+    
+    Returns:
+        TBD
+    
+    """     
 
     #We use a square plot
     height=max_window_size					
     width=max_window_size	
 
     #Real ranges of the plot
     #    - real_bounds must be [min_x,max_x,min_y,max_y]
@@ -413,71 +453,121 @@
 	    #We set the upper limit to ypos1 and adjust instead the right side  
 	    #    - in fraction of 1				
 	    xpos1=xpos0+(ypos1-ypos0)*(sub_width_set/sub_height_set)			
     else:
 	    ypos1=ypos1_temp
 					
     return width,height,[xpos0,ypos0,xpos1,ypos1]
-				
-'''
-Routine to adjust the size of a 3D plot
-'''
+
+
 def adjust_3D_isosize(ax,x_range,y_range,z_range):
+    r"""**3D isotropic plot scaling.**
+    
+    Adjusts the size of the plot window, maintaining isotropy.
+      
+    
+    Args:
+        TBD
+    
+    Returns:
+        TBD
+
+    """  
+    max_range = np.array([x_range[1]-x_range[0],y_range[1]-y_range[0], z_range[1]-z_range[0]]).max() / 2.0	
+    mean_x = 0.5*(x_range[1]+x_range[0])
+    mean_y = 0.5*(y_range[1]+y_range[0])
+    mean_z = 0.5*(z_range[1]+z_range[0])
+    ax.set_xlim(mean_x - max_range, mean_x + max_range)
+    ax.set_ylim(mean_y - max_range, mean_y + max_range)
+    ax.set_zlim(mean_z - max_range, mean_z + max_range)
+    
+    return ax							
+
 
-	max_range = np.array([x_range[1]-x_range[0],y_range[1]-y_range[0], z_range[1]-z_range[0]]).max() / 2.0	
-	mean_x = 0.5*(x_range[1]+x_range[0])
-	mean_y = 0.5*(y_range[1]+y_range[0])
-	mean_z = 0.5*(z_range[1]+z_range[0])
-	ax.set_xlim(mean_x - max_range, mean_x + max_range)
-	ax.set_ylim(mean_y - max_range, mean_y + max_range)
-	ax.set_zlim(mean_z - max_range, mean_z + max_range)
-								
-	return ax							
-
-'''
-Routine to truncate a colormap
-'''
 def truncate_colormap(cmap, minval=0.0, maxval=1.0, n=100):
+    r"""**Colormap truncation.**
+    
+    Limits colormap to the chosen range for the plotted variable.
+    
+    Args:
+        TBD
+    
+    Returns:
+        TBD
+    
+    """   
     new_cmap = colors.LinearSegmentedColormap.from_list('trunc({n},{a:.2f},{b:.2f})'.format(n=cmap.name, a=minval, b=maxval),
         cmap(np.linspace(minval, maxval, n)))
     return new_cmap
 
-'''
-Routine to reproduce the old stackrel
-'''
+
 def stackrel(val,sub,sup,form):
+    r"""**Stackrel truncation.**
+    
+    Print value with upper and lower error bars.
+    
+    Args:
+        TBD
+    
+    Returns:
+        TBD
+    
+    """ 
     form = deepcopy("{"+form+"}")
     return r"$"+form.format(val)+"\genfrac{}{}{0}{}{+"+form.format(sup)+"}{-"+form.format(sub)+"}$"
 
-'''Overrides plt.scatter to have various markers in one command'''
+
+
 def mscatter(plt ,x, y, ax=None, m=None, **kw):
+    r"""**Multiple markers.**
+    
+    Overrides plt.scatter to have various markers in one command.
+    
+    Args:
+        TBD
+    
+    Returns:
+        TBD
+    
+    """ 
+    import matplotlib.markers as mmarkers
+
+    if not ax: ax = plt.gca()
+
+    sc = ax.scatter(x, y, **kw)
+    
+    if (m is not None) and (len(m) == len(x)):
+        paths = []
+        for marker in m:
+            if isinstance(marker, mmarkers.MarkerStyle):
+                marker_obj = marker
+            else:
+                marker_obj = mmarkers.MarkerStyle(marker)
+            path = marker_obj.get_path().transformed(marker_obj.get_transform())
+            paths.append(path)
+        sc.set_paths(paths)
+        
+    return sc
 
-	import matplotlib.markers as mmarkers
 
-	if not ax: ax = plt.gca()
 
-	sc = ax.scatter(x, y, **kw)
 
-	if (m is not None) and (len(m) == len(x)):
-		paths = []
-		for marker in m:
-			if isinstance(marker, mmarkers.MarkerStyle):
-				marker_obj = marker
-			else:
-				marker_obj = mmarkers.MarkerStyle(marker)
-			path = marker_obj.get_path().transformed(marker_obj.get_transform())
-			paths.append(path)
-		sc.set_paths(paths)
-	
-	return sc
 
-'''
-Sub-function to shade ranges
-'''
 def plot_shade_range(ax,shade_range,x_range_loc,y_range_loc,mode='fill',facecolor='grey',zorder=-1,alpha=0.2,compl=False):
+    r"""**Shaded ranges.**
+    
+    Shades list of ranges.
+    
+    Args:
+        TBD
+    
+    Returns:
+        TBD
+    
+    """ 
     for i_int,bd_int in enumerate(shade_range):
         if compl:
             if (i_int==0 and bd_int[0]>x_range_loc[0]):
                 bd_int_loc=[x_range_loc[0],bd_int[0]] #shade area before first interval                 
                 if mode=='span':ax.axvspan(bd_int_loc[0],bd_int_loc[1], facecolor=facecolor, alpha=alpha,zorder=zorder)
                 elif mode=='fill':ax.fill([bd_int_loc[0],bd_int_loc[1],bd_int_loc[1],bd_int_loc[0]],[y_range_loc[0],y_range_loc[0],y_range_loc[1],y_range_loc[1]], fill=True,color='dodgerblue',alpha=alpha,zorder=zorder,ls='')  
                 elif mode=='hatch':ax.fill([bd_int_loc[0],bd_int_loc[1],bd_int_loc[1],bd_int_loc[0]],[y_range_loc[0],y_range_loc[0],y_range_loc[1],y_range_loc[1]], fill=False, hatch='\\',color=facecolor,zorder=zorder)
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_process/ANTARESS_data_align.py` & `antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_data_align.py`

 * *Files identical despite different names*

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_process/ANTARESS_data_process.py` & `antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_data_process.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-#!/usr/bin/env python3# -*- coding: utf-8 -*-import numpy as npfrom copy import deepcopyimport bindensity as bindfrom scipy.interpolate import interp1dimport pandas as pdimport batmanfrom ..ANTARESS_grids.ANTARESS_plocc_grid import init_surf_shift,def_surf_shift,sub_calc_plocc_spot_propfrom ..ANTARESS_grids.ANTARESS_coord import get_timeorbit,calc_pl_coord,excl_plrangefrom ..ANTARESS_conversions.ANTARESS_binning import init_bin_prof,weights_bin_prof,calc_bin_proffrom ..ANTARESS_process.ANTARESS_data_align import align_datafrom ..ANTARESS_general.utils import dataload_npz,gen_specdopshift,stop,np_where1D,datasave_npz,np_interp,npint,MAIN_multithread,check_data################################################################################################## #%% Alignment routines##################################################################################################     #NB: cannot be put in file data_align.py with align_data() due to circular import issuesdef align_profiles(data_type,data_dic,inst,vis,gen_dic,coord_dic):    r"""**Main alignment routine.**        Aligns time-series of disk-integrated, intrinsic, and planetary profiles.      Profiles used as weights throughout the workflow are shifted in the same way as their associated profiles.    Args:        TBD        Returns:        None        """         data_inst = data_dic[inst]      data_vis=data_inst[vis]    print('   > Aligning '+gen_dic['type_name'][data_type]+' profiles')     prop_dic = data_dic[data_type]      proc_gen_data_paths_new = gen_dic['save_data_dir']+'Aligned_'+data_type+'_data/'+gen_dic['add_txt_path'][data_type]+'/'+inst+'_'+vis+'_'    if (data_type=='DI') and (data_dic['DI']['sysvel'][inst][vis]==0.):print('         WARNING: sysvel = 0 km/s')    if data_type=='Intr':proc_gen_data_paths_new+='in'      proc_mast = True if ((gen_dic['DImast_weight']) and (data_type in ['Intr','Atm'])) else False    proc_locEst = True if ((data_type=='Atm') and ((data_dic['Atm']['pl_atm_sign']=='Absorption') or ((data_dic['Atm']['pl_atm_sign']=='Emission')) and data_dic['Intr']['cov_loc_star'])) else False    #Resample aligned profiles on the common visit table if relevant    #    - for CCFs the common table is shifted by the systemic velocity to be centered in the star rest frame, as operations using this table will now be performed in the star rest frame, and the     # table can be short enough that resampling on the original table would lead to lost pixels    #      the input velocity table is usually centered around the CCF, ie around RV(CDM_star/CDM_sun)    #      resampling the CCFs corrected for this motion onto the input table would put them on a side, or even outside the table    #      we thus shift the table itself to keep the CCFs roughly centered in the table (there is no need to interpolate since this shift is common to all exposures)        if (data_vis['comm_sp_tab']):        data_com = dataload_npz(data_vis['proc_com_data_paths'])        if (data_type=='DI') and (data_vis['type']=='CCF'):                         #Use comon systemic velocity to keep all tables the same in case they are common to an instrument            if (data_inst['comm_sp_tab']) and (data_inst['n_visits_inst']>1):comm_sysvel = data_dic['DI']['sysvel'][inst][data_inst['com_vis']]              else:comm_sysvel=data_dic['DI']['sysvel'][inst][vis]                                     #Align common table            data_com['cen_bins'] -= comm_sysvel            data_com['edge_bins'] -= comm_sysvel            data_dic[inst][vis]['proc_com_data_paths'] = gen_dic['save_data_dir']+'Processed_data/'+inst+'_'+vis+'_com_star'            datasave_npz(data_dic[inst][vis]['proc_com_data_paths'],data_com)               cen_bins_resamp, edge_bins_resamp , dim_exp_resamp = data_com['cen_bins'],data_com['edge_bins'],data_com['dim_exp']     else:cen_bins_resamp, edge_bins_resamp , dim_exp_resamp = None,None,None       #Calculating aligned data    if gen_dic['calc_align_'+data_type]:        print('         Calculating data')        #Define RV shifts        #    - shifts are saved independently so that they can be used to account for the combined Doppler shifts        data_comp = {'rv_starbar_solbar':data_dic['DI']['sysvel'][inst][vis],'star_starbar' : {}}        if data_type=='DI':                         #Reflex motion and systemic velocity            prop_dic[inst][vis]['idx_def'] = range(data_vis['n_in_visit'])            rv_shifts = coord_dic[inst][vis]['RV_star_stelCDM'][prop_dic[inst][vis]['idx_def']] + data_dic['DI']['sysvel'][inst][vis]        elif data_type=='Intr':             data_comp['surf_star'] = {}                        #Surface RV             #    - indexes relative to in-transit table            ref_pl,dic_rv,prop_dic[inst][vis]['idx_def'] = init_surf_shift(gen_dic,inst,vis,data_dic,data_dic['Intr']['align_mode'])                    #Remove chromatic RVs            #    - chromatic deviations from the 'white' average rv of the occulted stellar surface (due to variations in the planet size and stellar intensity) were already             # corrected for when extracting the intrinsic profiles            if ('chrom' in dic_rv):dic_rv.pop('chrom')        elif data_type=='Atm':             data_comp['pl_star'] = {}                        #Orbital radial velocity of the planet calculated for each exposure in the star rest frame            if data_dic['Atm']['pl_atm_sign']=='Absorption':idx_def_atm = list(np.array(gen_dic[inst][vis]['idx_in'])[prop_dic[inst][vis]['idx_def']])            elif data_dic['Atm']['pl_atm_sign']=='Emission':idx_def_atm = prop_dic[inst][vis]['idx_def']            rv_shifts = coord_dic[inst][vis][data_dic['Atm']['ref_pl_align']]['rv_pl'][idx_def_atm]            v_orb = coord_dic[inst][vis][data_dic['Atm']['ref_pl_align']]['v_pl'][idx_def_atm]        #Processing each in-transit exposure        data_comp['idx_aligned'] = prop_dic[inst][vis]['idx_def']        for isub,iexp in enumerate(prop_dic[inst][vis]['idx_def']):                #Upload latest processed data            data_exp = dataload_npz(data_dic[inst][vis]['proc_'+data_type+'_data_paths']+str(iexp))            #RV shifts            data_comp['star_starbar'][iexp] = coord_dic[inst][vis]['RV_star_stelCDM'][iexp]            if data_type=='DI':                rv_shift_cen = rv_shifts[isub]                spec_dopshift = 1./gen_specdopshift(rv_shift_cen)                            elif data_type=='Intr':                                #Achromatic planet-occulted surface rv in the star rest frame                rv_shift_cen = def_surf_shift(prop_dic['align_mode'],dic_rv,iexp,data_exp,ref_pl,data_vis['type'],data_dic['DI']['system_prop'],data_dic[inst][vis]['dim_exp'],data_dic[inst]['nord'],data_dic[inst][vis]['nspec'])[0]                data_comp['surf_star'][iexp] = rv_shift_cen                spec_dopshift = 1./gen_specdopshift(rv_shift_cen)                            elif data_type=='Atm':                rv_shift_cen = rv_shifts[isub]                data_comp['pl_star'][iexp] = rv_shifts[isub]                spec_dopshift = 1./gen_specdopshift(rv_shift_cen , v_s = v_orb)                            #Doppler shift            #Aligning exposure profile and complementary tables            #    - the calibration profile is common to all exposures of a processed instrument, and is originally sampled over the table of each exposure in the detector rest frame            #    - the calibration profile is then used as weight in temporal binning, or to scale back profiles from flux to count units            #      in both cases the calibration profile must follow the same shifts as the exposure            if data_vis['tell_sp']:data_exp['tell'] = dataload_npz(data_vis['tell_'+data_type+'_data_paths'][iexp])['tell']             if data_vis['mean_gdet']:data_exp['mean_gdet'] = dataload_npz(data_vis['mean_gdet_'+data_type+'_data_paths'][iexp])['mean_gdet']             data_align=align_data(data_exp,data_vis['type'],data_dic[inst]['nord'],dim_exp_resamp,gen_dic['resamp_mode'],cen_bins_resamp, edge_bins_resamp,rv_shift_cen,spec_dopshift)            #Saving aligned exposure and complementary tables            if data_vis['tell_sp']:                np.savez_compressed(proc_gen_data_paths_new+'_tell'+str(iexp), data = {'tell':data_align['tell']},allow_pickle=True)                 data_align.pop('tell')            if data_vis['mean_gdet']:                np.savez_compressed(proc_gen_data_paths_new+'_mean_gdet'+str(iexp), data = {'mean_gdet':data_align['mean_gdet']},allow_pickle=True)                 data_align.pop('mean_gdet')            np.savez_compressed(proc_gen_data_paths_new+str(iexp),data=data_align,allow_pickle=True)            #Aligning weighing master            #    - called for intrinsic and atmospheric profiles, when they are shifted from the star rest frame to other frames            #      it is not called for DI profiles, since it is computed from DI profiles after alignment (ie, the disk-integrated master does not need further alignment)            #    - master is shifted for Intr and Atm types             #    - the master is originally defined in the star rest frame, like the residual and then intrinsic profiles, but on the common table for the visit            # + if profiles are shifted and resampled on the common table, this will also be the case of the associated master            # + if profiles are shifted but kept on their individual tables, the master will remain defined on the common table without being resampled, and it is this table that is shifted            #   the master table thus becomes specific to each exposure, but is still different from the table of the exposure            #    - path to the master associated with current profile is updated            if proc_mast:                data_ref = dataload_npz(data_vis['mast_'+data_type+'_data_paths'][iexp])                data_ref_align=align_data(data_ref,data_vis['type'],data_dic[inst]['nord'],dim_exp_resamp,gen_dic['resamp_mode'],cen_bins_resamp,edge_bins_resamp,rv_shift_cen,spec_dopshift)                np.savez_compressed(proc_gen_data_paths_new+'_ref'+str(iexp),data={'edge_bins':data_ref_align['edge_bins'],'flux':data_ref_align['flux'],'cov':data_ref_align['cov']},allow_pickle=True)                       #Retrieve and align estimate of local stellar profile for current exposure, if based on measured profiles            #    - required to weigh binned atmospheric profiles                            #    - only defined for in-transit exposures            if proc_locEst and (iexp in data_vis['LocEst_Atm_data_paths']):                data_est_loc=np.load(data_vis['LocEst_Atm_data_paths'][iexp]+'.npz',allow_pickle=True)['data'].item()                 data_est_loc_align=align_data(data_est_loc,data_vis['type'],data_dic[inst]['nord'],dim_exp_resamp,gen_dic['resamp_mode'],cen_bins_resamp, edge_bins_resamp,rv_shift_cen,spec_dopshift,nocov = ~data_dic['Intr']['cov_loc_star'])                 np.savez_compressed(proc_gen_data_paths_new+'estloc'+str(iexp),data=data_est_loc_align,allow_pickle=True)        #Updating path to processed data and saving complementary data        np.savez_compressed(proc_gen_data_paths_new+'_add',data=data_comp,allow_pickle=True)                                #Retrieving data    else:         #Updating path to processed data and checking it has been calculated        check_data({'path':proc_gen_data_paths_new+'_add'})     data_vis['proc_'+data_type+'_data_paths'] = proc_gen_data_paths_new     prop_dic[inst][vis]['idx_def'] = dataload_npz(data_vis['proc_'+data_type+'_data_paths']+'_add')['idx_aligned']        #Updating rest frame    #    - rest frame of disk-integrated spectra is not updated if systemic velocity is 0    if (data_type!='DI') or (data_dic['DI']['sysvel'][inst][vis]!=0.):        data_dic[data_type][inst][vis]['rest_frame'] = {'DI':'star','Intr':'surf','Atm':'pl'}[data_type]    if proc_mast:data_vis['mast_'+data_type+'_data_paths']={}    if proc_locEst:data_vis['LocEst_Atm_data_paths'] = {}    if data_vis['tell_sp']:data_vis['tell_'+data_type+'_data_paths']={}      if data_vis['mean_gdet']:data_vis['mean_gdet_'+data_type+'_data_paths']={}      for iexp in prop_dic[inst][vis]['idx_def']:        if proc_mast:data_vis['mast_'+data_type+'_data_paths'][iexp]=proc_gen_data_paths_new+'_ref'+str(iexp)        if proc_locEst and (iexp in data_vis['LocEst_Atm_data_paths']):data_vis['LocEst_Atm_data_paths'][iexp] = proc_gen_data_paths_new+'estloc'+str(iexp)         if data_vis['tell_sp']:data_vis['tell_'+data_type+'_data_paths'][iexp] = proc_gen_data_paths_new+'_tell'+str(iexp)        if data_vis['mean_gdet']:data_vis['mean_gdet_'+data_type+'_data_paths'][iexp] = proc_gen_data_paths_new+'_mean_gdet'+str(iexp)                  return None################################################################################################## #%% Flux scaling routines################################################################################################## def rescale_profiles(data_inst,inst,vis,data_dic,coord_dic,exp_dur_d,gen_dic,plot_dic,system_param,theo_dic):    r"""**Main flux scaling routine.**        Scales profiles to the correct relative broadband flux level.    Spectra :math:`F_\mathrm{corr}(\lambda,t,v)` should have been set to the same flux balance as a reference spectrum at low resolution using `corr_Fbal()`.    .. math::       F_\mathrm{corr}(\lambda,t,v) = F_{\star}(\lambda,v) C_\mathrm{ref}(\lambda,v) L(t)          Where :math:`C_\mathrm{ref}(\mathrm{\lambda \, in \, band \, B},v) \sim C_\mathrm{ref}(B,v)` represents a possible low-frequency deviation from the true stellar spectrum, and     `L(t)` represents the global flux deviation from the true stellar spectrum, not corrected for in previous modules.         We first convert all spectra from flux to (temporal) flux density units, so that they are equivalent except for flux variations.        We then correct for `L(t)` by dividing the profiles by     .. math::          F^\mathrm{glob}(v,t) &= \frac{\mathrm{TF}_\mathrm{corr}(v,t)}{\mathrm{median}(t_k, \mathrm{TF}_\mathrm{corr}(v,t_k) )}  \\       \mathrm{or}&  \\           F^\mathrm{glob}(v,t) &= \frac{\mathrm{TF}_\mathrm{corr}(v,t)}{F_\mathrm{sc} \int_{\mathrm{\lambda \, in \, full \, B}}{d\lambda }}            Where     .. math::         \mathrm{TF}_\mathrm{corr}(v,t) &= \int_{\mathrm{\lambda \, in \, full \, B}}{F_\mathrm{corr}(\lambda,t,v) d\lambda } \\                                      &= L(t) C     The exact value of the (unocculted) global flux level does not matter within a visit and is set to the median flux of all spectra,     unless the user choses to impose a common flux density for all visits (in case disk-integrated data needs to be combined between visits).              We then need to rescale spectrally the data so that     .. math::             F_\mathrm{sc}(\lambda,t) &= c(\lambda,t) F_\mathrm{corr}(\lambda,t) \\                                 &= F(\lambda,t)      To do so we use broadband spectral light curves, which by definition correspond to the ratio of in- and out-of-transit flux integrated over the band    .. math::             LC(B,v,t) &= \frac{ \int_{\mathrm{\lambda \, in \, B}}{F(\lambda,t) d\lambda }}{\int_{\mathrm{\lambda \, in \, B}}{F_{\star}(\lambda,v) d\lambda } } \\                    &= \frac{ \mathrm{TF}(B,t) }{ \mathrm{TF}_{\star}(B,v) }         We assume that :math:`c(\lambda,t)` has low-frequency variations (which should be the case, since the difference between :math:`F_\mathrm{corr}` and `F` comes from the changes in color balance).    The correction thus implies    .. math::             & \int_{\mathrm{\lambda \, in \, B}}{c(\lambda,t) F_\mathrm{corr}(\lambda,t) } = \int_{\mathrm{\lambda \, in \, B}}{ F(\lambda,t) }       \\                    & c(B,t) \int_{\mathrm{\lambda \, in \, B}}{F_\mathrm{corr}(\lambda,t) } = \mathrm{TF}(B,t)     \\       & c(B,t) = \frac{ \mathrm{TF}_{\star}(B,v) \mathrm{LC}(B,v,t) }{ \int_{\mathrm{\lambda \, in \, B}}{F_{\star}(\lambda,v) C_\mathrm{ref}(B,v) }  }   \\       & c(B,t) = \frac{ \mathrm{TF}_{\star}(B,v) \mathrm{LC}(B,v,t)}{  \mathrm{TF}_{\star}(B,v) C_\mathrm{ref}(B,v)  }  \\       & c(B,t) = \frac{ \mathrm{LC}(B,v,t) }{ C_\mathrm{ref}(B,v) }     We set :math:`c(B,t) = \mathrm{LC}_\mathrm{theo}(B,t)` and interpolate the chromatic `c(B,t)` at all wavelengths in the spectrum to define :math:`c(\lambda,t)`        .. math::             F_\mathrm{sc}(\lambda,t,v) &= \frac{ \mathrm{LC}_\mathrm{theo}(\lambda,t) F_\mathrm{corr}(\lambda,t)}{F^\mathrm{glob}(v,t)   }  \\                                  &= F(\lambda,t,v) C_\mathrm{ref}(B,v)                  Care must be taken about :math:`C_\mathrm{ref}(B,v)` when several visits are exploited        (1) if the stellar emission remains the same in all visits, then we can use a single theoretical spectrum / master as reference, and a constant normalized light curve               .. math::                F_\mathrm{sc}(\lambda,t,v) = F(\lambda,t,v) C_\mathrm{ref}(B)     (2) if the stellar emission changes in amplitude uniformly over the star, the normalized light curve remains the same, and the stellar spectrum keeps the same profile           .. math::                    &F_\mathrm{sc}(\lambda,t,v) = \frac{F(\lambda,t,v) C_\mathrm{ref}(B)}{F_r(v)}   \\           &\mathrm{where \,} F_r(v) = \frac{F_{\star}(\lambda,v)}{F_{\star}(\lambda,v_\mathrm{ref})}        The stellar spectrum of one of the visit :math:`F_{\star}(\lambda,v_\mathrm{ref})` is taken as reference, with                                                                                            .. math::            \mathrm{LC}_\mathrm{theo}(\lambda,t) &= \frac{F(\lambda,v_\mathrm{ref},t)}{F_{\star}(\lambda,v_\mathrm{ref})}  \\                                             &= \frac{F(\lambda,t,v)}{F_{\star}(\lambda,v)}         Thus                 .. math::            F_\mathrm{sc}(\lambda,t,v) &= \frac{F(\lambda,t,v) C_\mathrm{ref}(B) F_{\star}(\lambda,v_\mathrm{ref})}{F_{\star}(\lambda,v) }     \\                                              &= \frac{F(\lambda,v_\mathrm{ref},t) C_\mathrm{ref}(B) F_{\star}(\lambda,v_\mathrm{ref})}{F_{\star}(\lambda,v_\mathrm{ref}) }       \\                                            &= F(\lambda,v_\mathrm{ref},t) C_\mathrm{ref}(B)               Scaled spectra thus keep the same profile, deviating from the true profile by a common :math:`C_\mathrm{ref}(B)` in all visits.    (3) if the stellar emission changes in amplitude and shape uniformely over the star, the normalized light curve remains the same but the stellar spectrum has not the same profile        .. math::                   F_\mathrm{sc}(\lambda,t,v) &= \mathrm{LC}_\mathrm{theo}(\lambda,t) F(\lambda,v) C_\mathrm{ref}(\lambda,v) \\                                      &= (F(\lambda,v,t)/F_{\star}(\lambda,v)) F_{\star}(\lambda,t) C_\mathrm{ref}(B,v)  \\                                      &= F(\lambda,t,v) C_\mathrm{ref}(B,v)                    By using a reference spectrum specific to each visit when correcting the color balance, with the correct shape and relative flux, we would get                .. math::                        F_\mathrm{sc}(\lambda,t,v) = F(\lambda,t,v) C_\mathrm{ref}        Where :math:`C_\mathrm{ref}` is the deviation from the absolute flux level, common to all visits.     (4) if local stellar spectra in specific regions of the star change between visits, eg due to (un)occulted spots, then the normalized light curve changes as well.        Both a reference spectrum and a light curve specific to each visit must be used to remove the stellar contribution :math:`F_{\star}(\lambda,v)` and avoid introducing a different balance to the planet-occulted spectra.     If there is emission/reflection from the planet, then the true flux writes as        .. math::        F(\lambda,v,t) &= F_{\star}(\lambda,v) \mathrm{LC}^\mathrm{tr}(\lambda,v,t) + F_{\star}(\lambda,v) \mathrm{LC}^\mathrm{refl}(\lambda,v,t) + F_\mathrm{p}^\mathrm{thermal}(\lambda,v,t)      \\                      &= F_{\star}(\lambda,v) ( \delta_p^\mathrm{tr}(\lambda,v,t) + \delta_p^\mathrm{refl}(\lambda,v,t) + \delta_p^\mathrm{thermal}(\lambda,v,t) )   \\                      &= F_{\star}(\lambda,v) \delta_p(\lambda,v,t)                   The correction should still ensure that          .. math::             c(B,t) &= \frac{ \mathrm{TF}(B,v,t) }{  \mathrm{TF}_{\star}(B,v) C_\mathrm{ref}(B)  }    \\                 &= \frac{ \mathrm{LC}(B,v,t) \mathrm{TF}_{\star}(B,v) }{  \mathrm{TF}_{\star}(B,v) C_\mathrm{ref}(B)  }    \\                 &= \frac{ \mathrm{LC}(B,v,t) }{ C_\mathrm{ref}(B) }     But broadband spectral light curves correspond to          .. math::             \mathrm{LC}(B,v,t) &=  \frac{ \mathrm{TF}(B,v,t) }{   \mathrm{TF}_{\star}(B,v) }  \\                              &=  \frac{ \int_{\mathrm{\lambda \, in \, B}}, F_{\star}(\lambda,v) \delta_p(\lambda,v,t) d\lambda ) }{   \mathrm{TF}_{\star}(B,v)   }        So that care must be taken to use light curves that integrate the different spectral contributions and are then normalized by the integrated stellar flux, rather than integrating the pure planet contribution.                   For spectra, we can use the flux integrated over bands including the planetary absorption, as we can match it with the same band over which the light curve was measured.    Ideally the input light curves should be defined with a fine enough resolution to sample the low-frequency variations of the planetary atmosphere and stellar limb-darkening     For CCFs, a light curve does not match the cumulated flux of the different spectral regions used to calculate the CCF.     If we assume that the signature of the planet and of the RM effect is similar in all lines used to calculate the CCF, and that the light curve is achromatic, then it is similar to the scaling of a spectrum with a single line.    Thus, as with spectra, CCFs should be scaled using the flux of their full profile and not just the continuum (although there will always be a bias in using CCFs at this stage and the use of spectra should be preferred).    Since the scaling is imposed by a light curve independent of the spectra, bin by bin, it does not need to be applied to the full spectra like the flux balance color correction, and can be applied to any spectral range.     Note that the measured light curve corresponds to         .. math::           \mathrm{LC}(B,t) &= \frac{ \int_{\lambda \, in \, B}{ F_\mathrm{in}(\lambda,t) d\lambda } }{ \int_{\lambda \, in \, B}{ F_{\star}(\lambda,v) d\lambda }} \\                           &= 1 - \frac{\int_{ \lambda \, in \, B}{ f_p(\lambda) ( S_\mathrm{thick}(B,t) + S_\mathrm{thin}(\lambda,t) ) d\lambda} }{ <F_{\star}(\mathrm{\lambda \, in \, B},v)> }                          The theoretical light curves fitted to the measured one assume a constant, uniform stellar intensity `I` and limb-darkening law, and a constant average radius over the band        .. math::             \mathrm{LC}^\mathrm{theo}(B,t) &= \frac{ \mathrm{TF}^\mathrm{theo}(B,t) }{ \mathrm{TF}_{\star}^\mathrm{theo}(B) } \\                                         &= \frac{ F^\mathrm{theo}(B,t) }{ F_{\star}^\mathrm{theo}(B)  } \\                                         &= 1 - \frac{ I^\mathrm{theo}(B) \mathrm{LD}(B,t) S_p(B,t)}{\sum_{k}{ I^\mathrm{theo}(B) \mathrm{LD}_k(B) S_k }  } \\                                         &= 1 - \frac{ \mathrm{LD}(B,t) S_p(B,t)}{\sum_{k}{ \mathrm{LD}_k(B) S_k} } \\                                         &= 1 - \frac{ \mathrm{LD}(B,t) S_p(B,t)}{S_{\star}^\mathrm{LD}(B) }                     The fact that this is an approximation does not matter as long as the measured light curve is correctly reproduced, in which case the rescaling with the theoretical light curve is correct.    In the following we assume that the theoretical LD matches the true LD.                    Out-of-transit data is rescaled as well, to account for possible variations of stellar origin in the disk-integrated flux.      Args:        TBD        Returns:        None        """      print('   > Broadband flux scaling')     data_vis=data_inst[vis]    if data_dic['DI']['rescale_DI']:proc_DI_data_paths_new = gen_dic['save_data_dir']+'Scaled_data/'+inst+'_'+vis+'_'    else:proc_DI_data_paths_new = deepcopy(data_vis['proc_DI_data_paths'])    data_vis['scaled_DI_data_paths'] = proc_DI_data_paths_new+'scaling_'             #Default transit model    if (vis not in data_dic['DI']['transit_prop'][inst]):        data_dic['DI']['transit_prop'][inst][vis] = {'mode':'model','dt':np.min(coord_dic[inst][vis]['t_dur']/60.)/5.}        print('         Default transit model')    transit_prop=data_dic['DI']['transit_prop'][inst][vis]        #Flux scaling    if not data_dic['DI']['rescale_DI']:print('         No flux scaling applied')            #Calculating rescaled data    if (gen_dic['calc_flux_sc']):        print('         Calculating data')        dic_save={}            #Light curve for all bands and all exposures        #    - chromatic values are used if provided and if disk-integrated profiles are in spectral mode        if ('spec' in data_vis['type']) and ('chrom' in data_vis['system_prop']):key_chrom = ['chrom']        else:key_chrom = ['achrom']        system_prop = data_vis['system_prop'][key_chrom[0]]        LC_flux_band_all = np.zeros([data_vis['n_in_visit'],system_prop['nw']])*np.nan                    #Simulated light curves        if transit_prop['mode']=='simu':            params_LC = deepcopy(system_param['star'])            params_LC.update({'rv':0.,'cont':1.})         #Calculate light curve for plotting                if (plot_dic['input_LC']!='') or (plot_dic['prop_Intr']!=''):                        #High-resolution time table over visit            min_bjd = coord_dic[inst][vis]['bjd'][0]            max_bjd = coord_dic[inst][vis]['bjd'][-1]            dbjd_HR = plot_dic['dt_LC']/(3600.*24.)            nbjd_HR = round((max_bjd-min_bjd)/dbjd_HR)            bjd_HR=min_bjd+dbjd_HR*np.arange(nbjd_HR)                  #Corresponding orbital phases and coordinates for each planet            #    - high-resolution tables are calculated assuming no exposure duration            coord_pl_HR = {}            LC_HR=np.ones([nbjd_HR,system_prop['nw']],dtype=float)              if transit_prop['mode']=='simu':ecl_all_HR = np.zeros(nbjd_HR,dtype=bool)            for pl_loc in data_inst[vis]['transit_pl']:                pl_params_loc=system_param[pl_loc]                coord_pl_HR[pl_loc]={'cen_ph':get_timeorbit(pl_loc,coord_dic[inst][vis],bjd_HR,pl_params_loc,None)[1]}                   #Definition of coordinates for all transiting planets                if transit_prop['mode']=='simu':                     x_pos_pl,y_pos_pl,z_pos_pl,Dprojp,_,_,_,_,ecl_pl = calc_pl_coord(pl_params_loc['ecc'],pl_params_loc['omega_rad'],pl_params_loc['aRs'],pl_params_loc['inclin_rad'],coord_pl_HR[pl_loc]['cen_ph'],data_dic['DI']['system_prop']['achrom'][pl_loc][0],pl_params_loc['lambda_rad'],system_param['star'])                    coord_pl_HR[pl_loc].update({'ecl':ecl_pl,'cen_pos':np.vstack((x_pos_pl,y_pos_pl,z_pos_pl))})                        #Exposure considered out-of-transit if no planet at all is transiting                    ecl_all_HR |= abs(ecl_pl)!=1                              #------------------------------------------------------------------------                        #Light curves from import        #    - defined over a set of wavelengths that can be different for each visit        #    - here we import the light curves, so that they can be interpolated for each visit after their exposures have been defined        if transit_prop['mode']=='imp':            t_dur_d=coord_dic[inst][vis]['t_dur']/(3600.*24.)            cen_bjd = coord_dic[inst][vis]['bjd']                      #Retrieving light curve            #    - first column must be absolute time (BJD), to be independent of a specific planet             #    - next columns must be normalized stellar flux for all chosen bands, in the same order as data_dic['DI']['system_prop']['chrom']['w']            ext = transit_prop['path'].split('.')[-1]            if (ext=='csv'):                imp_LC = (pd.read_csv(transit_prop['path'])).values            elif (ext in ['txt','dat']):                imp_LC = np.loadtxt(transit_prop['path']).T                      else:                stop('Light curve path extension TBD')             imp_LC[0] -= 2400000.             if (plot_dic['input_LC']!=''):dic_save['imp_LC'] = imp_LC                     #Average imported light curve within the exposure time windows            #    - the light curve must be imported with sufficient temporal resolution            for iexp,(bjd_loc,dt_loc) in enumerate(zip(cen_bjd,t_dur_d)):                #Imported points within exposure                id_impLC=np_where1D( (imp_LC[0]>=bjd_loc-0.5*dt_loc) & (imp_LC[0]<=bjd_loc+0.5*dt_loc))                              #Normalized flux averaged within exposure                if len(id_impLC)>0:LC_flux_band_all[iexp,:]=np.mean(imp_LC[1::,id_impLC],axis=1)                else:stop('No LC measurements within exposure')            #Calculate light curve for plotting                    if (plot_dic['input_LC']!='') or (plot_dic['prop_Intr']!=''):                     for iband in range(system_prop['nw']):LC_HR[:,iband] = np_interp(bjd_HR,imp_LC[0],imp_LC[1+iband],left=imp_LC[1+iband,0],right=imp_LC[1+iband,-1])        #------------------------------------------------------------------------                #Model light curve for a single planet        #    - can be oversampled           #    - defined over a set of wavelengths but constant for each visit        elif transit_prop['mode']=='model':            if len(data_inst[vis]['transit_pl'])>1:stop('Multiple planets transiting')            pl_vis = data_inst[vis]['transit_pl'][0]            LC_params = batman.TransitParams()            LC_pl_params = system_param[pl_vis]                    #Phase reference for inferior conjunction            LC_params.t0 = 0.                         #Orbital period in phase            LC_params.per = 1.                         #Semi-major axis (in units of stellar radii)            LC_params.a = LC_pl_params['aRs']                        #Orbital inclination (in degrees)            #    - from the line of sight to the normal to the orbital plane            LC_params.inc = LC_pl_params['inclination']                         #Eccentricity            LC_params.ecc = LC_pl_params['ecc']                        #Longitude of periastron (in degrees)            LC_params.w = LC_pl_params['omega_deg']                        #Oversampling             if ('dt' not in transit_prop):LC_osamp = np.repeat(10,data_vis['n_in_visit'])            else:LC_osamp = npint(np.ceil(coord_dic[inst][vis]['t_dur']/(60.*transit_prop['dt'])))            if np.min(LC_osamp)<2.:print('WARNING: no oversampling of model light curve')                        #Calculate white or chromatic light curves            cen_ph_pl = coord_dic[inst][vis][pl_vis]['cen_ph']            ph_dur_pl=coord_dic[inst][vis][pl_vis]['ph_dur']            for iband,wband in enumerate(system_prop['w']):                    #Light curve properties for the band                LC_params_band = deepcopy(LC_params)                    #LD law                 LD_mod = system_prop['LD'][iband]                        #Limb darkening coefficients in the format required for batman                LC_params_band.limb_dark = LD_mod                if LD_mod == 'uniform':                    ld_coeff=[]                elif LD_mod == 'linear':                    ld_coeff=[system_prop['LD_u1'][iband]]                elif LD_mod in ['quadratic' ,'squareroot','logarithmic', 'power2' ,'exponential']:                    ld_coeff=[system_prop['LD_u1'][iband],system_prop['LD_u2'][iband]]                elif LD_mod == 'nonlinear':                       ld_coeff=[system_prop['LD_u1'][iband],system_prop['LD_u2'][iband],system_prop['LD_u3'][iband],system_prop['LD_u4'][iband]]                           else:                    stop('Limb-darkening not supported by batman')                  LC_params_band.u=ld_coeff                        #Planet-to-star radius ratio                LC_params_band.rp=system_prop[pl_vis][iband]                #All exposures have same duration                #    - process each band for all exposures together                if coord_dic[inst][vis]['cst_tdur']:                    LC_flux_band_all[:,iband] = batman.TransitModel(LC_params_band, cen_ph_pl, supersample_factor = LC_osamp[0], exp_time = ph_dur_pl[0]).light_curve(LC_params_band)                                    #Exposures have different durations                #    - process each band and each exposure                else:                                          for iexp,(cen_ph_exp,ph_dur_exp,LC_osamp_exp) in enumerate(zip(cen_ph_pl,ph_dur_pl,LC_osamp)):                                            LC_flux_band_all[iexp,iband]=float(batman.TransitModel(LC_params_band, np.array([cen_ph_exp]), supersample_factor = LC_osamp_exp, exp_time = np.array([ph_dur_exp])).light_curve(LC_params_band))                                        #Calculate light curve for plotting                        if (plot_dic['input_LC']!='') or (plot_dic['prop_Intr']!=''):                    LC_HR[:,iband] = batman.TransitModel(LC_params_band,coord_pl_HR[pl_vis]['cen_ph']).light_curve(LC_params_band)                      #------------------------------------------------------------------------             #Simulated light curve           #    - can account for multiple transiting planets        elif transit_prop['mode']=='simu':                            #Set out-of-transit values to unity            LC_flux_band_all[gen_dic[inst][vis]['idx_out'],:]=1.                              #Oversampling factor, in units of RpRs            theo_dic_LC= deepcopy(theo_dic)            theo_dic_LC['d_oversamp']={}            if (transit_prop['n_oversamp']>0.):                for pl_loc in data_inst[vis]['transit_pl']:theo_dic_LC['d_oversamp'][pl_loc]=data_dic['DI']['system_prop']['achrom'][pl_loc][0]/transit_prop['n_oversamp']             #Calculate transit light curves accounting for all planets in the visit            plocc_prop,spot_prop = sub_calc_plocc_spot_prop(key_chrom,{},[],data_inst[vis]['transit_pl'],system_param,theo_dic_LC,data_dic['DI']['system_prop'],params_LC,coord_dic[inst][vis],gen_dic[inst][vis]['idx_in'],Ftot_star=True)             LC_flux_band_all[gen_dic[inst][vis]['idx_in'],:]=plocc_prop[key_chrom[0]]['Ftot_star'].T                           #Calculate light curve for plotting                    if (plot_dic['input_LC']!='') or (plot_dic['prop_Intr']!=''):                theo_dic_LC['d_oversamp']={}                idx_in_HR = np_where1D(ecl_all_HR)                plocc_prop_HR,spot_prop_HR = sub_calc_plocc_spot_prop(key_chrom,{},[],data_inst[vis]['transit_pl'],system_param,theo_dic_LC,data_dic['DI']['system_prop'],params_LC,coord_pl_HR,idx_in_HR,Ftot_star=True)                 LC_HR[idx_in_HR,:]=plocc_prop_HR[key_chrom[0]]['Ftot_star'].T           #Store for plots        if (plot_dic['input_LC']!='') or (plot_dic['prop_Intr']!=''):            dic_save['flux_band_all'] = LC_flux_band_all            dic_save['coord_HR'] = coord_pl_HR            dic_save['LC_HR'] = LC_HR        #------------------------------------------------------------------------        #Upload common spectral table        #    - if profiles are defined on different tables they are resampled on this one        #      if they are already defined on a common table, it is this one, which has been kept the same since the beginning of the routine        edge_bins_com = (np.load(data_vis['proc_com_data_paths']+'.npz',allow_pickle=True)['data'].item())['edge_bins']        #Spectral scaling table and global scaling range        loc_flux_scaling = np.zeros(data_vis['n_in_visit'],dtype=object)         flux_all = np.zeros(data_vis['dim_all'],dtype=float)*np.nan        cond_def_all = np.zeros(data_vis['dim_all'],dtype=bool)        cond_def_scal_all  = np.zeros(data_vis['dim_all'],dtype=bool)        null_loc_flux_scaling = np.ones(data_vis['n_in_visit'],dtype=bool)        for iexp in range(data_vis['n_in_visit']):                         #Latest processed DI data            data_exp = dataload_npz(data_vis['proc_DI_data_paths']+str(iexp))            #Resampling and conversion to temporal flux density            #    - if data were kept on independent tables they need to be resampled on a common one to calculate equivalent fluxes            if (not data_vis['comm_sp_tab']):                for iord in range(data_inst['nord']):                     flux_all[iexp,iord] = bind.resampling(edge_bins_com[iord], data_exp['edge_bins'][iord], data_exp['flux'][iord] , kind=gen_dic['resamp_mode'])                                                                        cond_def_all[iexp] = ~np.isnan(flux_all[iexp])               else:                flux_all[iexp] = data_exp['flux']                cond_def_all[iexp] = data_exp['cond_def']            flux_all[iexp]/=coord_dic[inst][vis]['t_dur'][iexp]            #Spectral scaling table                                                    #    - scale to the expected flux level at all wavelengths, using the broadband flux interpolated over the full spectrum range, unless a single band is used            #    - accounts for the potentially chromatic signature of the planet             #    - if the planet is not actually transiting (based on the determination of transit contacts) the 'null_loc_flux_scaling' flag is set to True            #      profile are still rescaled, with a light curve unity and 'loc_flux_scaling' equal to 0            if np.max(np.abs(1.-LC_flux_band_all[iexp]))>0.:null_loc_flux_scaling[iexp] = False            if (system_prop['nw']==1):loc_flux_scaling[iexp] = np.poly1d([1.-LC_flux_band_all[iexp,0]])            else:loc_flux_scaling[iexp] = interp1d(system_prop['w'],1.-LC_flux_band_all[iexp],fill_value=(1.-LC_flux_band_all[iexp,0],1.-LC_flux_band_all[iexp,-1]), bounds_error=False)                            #Requested scaling range            if len(data_dic['DI']['scaling_range'])>0:                cond_def_scal=False                 for bd_int in data_dic['DI']['scaling_range']:cond_def_scal |= (edge_bins_com[:,0:-1]>=bd_int[0]) & (edge_bins_com[:,1:]<=bd_int[1])               else:cond_def_scal=True             #Accounting for undefined pixels in scaling range                        cond_def_scal_all[iexp] = cond_def_all[iexp]  & cond_def_scal                    #Scaling pixels common to all exposures        #    - planetary signatures should not be excluded from the range of summation, for the same reason as they are included in the spectral scaling : the light curves used for the scaling include those ranges potentially absorbed by the planet        #      the same logic applies to CCF: their full range must be used for the scaling, and not just the continuum              cond_scal_com  = np.all(cond_def_scal_all,axis=0)        if np.sum(cond_scal_com)==0.:stop('No pixels in common scaling range')                  #Defining global scaling values        #    - used to set all profiles to a common global flux level        #    - spectral profiles have been trimmed, corrected, and aligned        #      it might thus be more accurate to rescale them using their own flux rather than the flux of the original spectra        #      furthermore masters afterward will be calculated from these profiles, scaled, thus they do not need to be set to the level of the original global master        #      we thus use the total flux summed over the full range of the current profiles, with their median taken as reference        #    - defined on temporal flux density (not cumulated photoelectrons counts)        Tflux_all = np.zeros(data_vis['n_in_visit'],dtype=float)        dcen_bin_comm = (edge_bins_com[:,1::] - edge_bins_com[:,0:-1])        Tcen_bin_comm = 0.        for iord in range(data_inst['nord']):                Tflux_all += np.sum(flux_all[:,iord,cond_scal_com[iord]]*dcen_bin_comm[iord,cond_scal_com[iord]],axis=1)            Tcen_bin_comm += np.sum(dcen_bin_comm[iord,cond_scal_com[iord]])        if data_dic['DI']['scaling_val'] is None:Tflux_ref = np.median(Tflux_all)        else:Tflux_ref=Tcen_bin_comm*data_dic['DI']['scaling_val']        norm_exp_glob = Tflux_all/Tflux_ref        #Scaling each exposure        #    - only defined bins are scaled (the flux in undefined bins remain set to nan), but the scaling spectrum was calculated at all wavelengths so that it can be used later with data for which different bins are defined or not        #    - all defined bins remain defined         #    - operation depends on condition 'rescale_DI' because flux scaling tbales may be required even if data needs not be scaled        for iexp in range(data_vis['n_in_visit']):                          #Scale and save exposure            if data_dic['DI']['rescale_DI']:                 data_exp = np.load(data_vis['proc_DI_data_paths']+str(iexp)+'.npz',allow_pickle=True)['data'].item()                 for iord in range(data_inst['nord']):                     LC_exp_spec_ord = 1.-loc_flux_scaling[iexp](data_exp['cen_bins'][iord])                    data_exp['flux'][iord],data_exp['cov'][iord] = bind.mul_array(data_exp['flux'][iord],data_exp['cov'][iord],LC_exp_spec_ord/(coord_dic[inst][vis]['t_dur'][iexp]*norm_exp_glob[iexp]))                datasave_npz(proc_DI_data_paths_new+str(iexp),data_exp)                        #Save scaling            #    - must be saved for each exposure because (for some reason) the interp1d function cannot be saved once passed out of multiprocessing             #    - in-transit scaling can be used later to manipulate local profiles from the planet-occulted regions             data_scaling = {'loc_flux_scaling':loc_flux_scaling[iexp],'glob_flux_scaling':norm_exp_glob[iexp],'null_loc_flux_scaling':null_loc_flux_scaling[iexp]}            if system_prop['nw']>1:data_scaling['chrom']=True            else:data_scaling['chrom']=False            datasave_npz(data_vis['scaled_DI_data_paths']+str(iexp),data_scaling)                          #Saving complementary data        dic_save['rest_frame']=data_dic['DI'][inst][vis]['rest_frame']        datasave_npz(proc_DI_data_paths_new+'add',dic_save)                       #Updating path to processed data and checking it has been calculated    else:           check_data({'path':proc_DI_data_paths_new+str(0)})       data_vis['proc_DI_data_paths'] = proc_DI_data_paths_new    return None    ################################################################################################## #%% Residual profiles routines################################################################################################## def extract_res_profiles(gen_dic,data_dic,inst,vis,data_prop,coord_dic):    r"""**Main residual profile routine.**     Extracts residual profiles in the stellar rest frame.    The real measured spectrum can be written as         .. math::           F(\lambda,t,v) = F_{\star}(\lambda,t,v) \delta_p(\lambda,t,v)      It can also be decomposed spatially as           .. math::       F(\lambda,t,v) &= (\sum_\mathrm{i \, not \, occulted}{F_i(\lambda,t,v)}) + f_p(\lambda,v) (S_\mathrm{occ}(t) - S_\mathrm{thick}(B,t) - S_\mathrm{thin}(\lambda,t) ) + F_p(\lambda,t)       \\                      &= F_{\star}(\lambda,t,v) - f_p(\lambda,v) ( S_\mathrm{thick}(B,t) + S_\mathrm{thin}(\lambda,t) ) + F_p(\lambda,t)               With          - :math:`\lambda` the absolute wavelength in the stellar rest frame, within a given spectral band.      - `F` the flux received from the star - planet system :math:`[erg \, s^{-1} \,  A^{-1} \, cm^{-2}]` at a given distance       :math:`F_i(\lambda,v) = f_i(\lambda,v) S_i` is the flux emitted by the region `i` of surface :math:`S_i`.     - the surface density flux can be written as :math:`f_i(\lambda,v) = I_i(\lambda) \mathrm{LD}_i(\lambda) \mathrm{GD}_i(\lambda)`.               + :math:`I_i(\lambda)` is the specific intensity in the direction of the LOS :math:`[erg \, s^{-1} \,  A^{-1} \, cm^{-2} \, sr^{-1}]`         which can be written as :math:`I_0(\lambda-\lambda_{\star}(t))` if the local stellar emission is constant over the stellar disk, and simply shifted by :math:`\lambda_{\star}(t)` because of surface velocity.       + :math:`\mathrm{LD}_i(\lambda)` is the spectral limb-darkening law.       + :math:`\mathrm{GD}_i(\lambda)` the gravity-darkening law.     - :math:`F_p(\lambda,t)` is the flux emitted or reflected by the planet.                       The planet and its atmosphere occult a surface :math:`S_\mathrm{occ}(t)`, time-dependent because of partial occultation at ingress/egress.           + :math:`S_\mathrm{thick}(B,t)` is the equivalent surface of the planet disk opaque to light in the local spectral band.        + :math:`S_\mathrm{thin}(\lambda,t)` is the equivalent surface of the atmospheric annulus optically thin to light in the band, varying at high frequency and null outside of narrow absorption lines.         + :math:`F_p(\lambda,t)` and :math:`S_\mathrm{thin}(\lambda,t)` are sensitive to the planet orbital motion, and shifted in the star rest frame by :math:`\lambda_\mathrm{pl}(t)`.        The measured profiles are now defined in the most general case as (see `rescale_profiles()`)        .. math::       F_\mathrm{sc}(\lambda,t,v) = F(\lambda,t,v) C_\mathrm{ref}(\lambda_\mathrm{B},v)     With :math:`F(\lambda,t,v)` the true spectrum.    Since all spectra were set to the same balance, corresponding to the stellar spectrum times a low-frequency coefficient, the master out corresponds in a given visit to     .. math::            F^\mathrm{mast}_{\star}(\lambda,v) = F_{\star}(\lambda,v) C_\mathrm{ref}(\lambda_\mathrm{B},v)      Note that the unknown scaling of the flux due to the distance to the star is implicitely included in :math:`C_\mathrm{ref}`.    We can decompose :math:`F_{\star}` as:               .. math::       F_{\star}(\lambda,v) = (\sum_\mathrm{i \, not \, occulted}{F_i(\lambda,v)}) + f_p(\lambda,v) S_\mathrm{occ}(t)                The local residual profiles are calculated as         .. math::       F_\mathrm{res}(\lambda,t,v) &= F^\mathrm{mast}_{\star}(\lambda,v) - F_\mathrm{sc}(\lambda,t,v)   \\                                                 &= F_{\star}(\lambda,v) C_\mathrm{ref}(\lambda_\mathrm{B},v)  - F(\lambda,t,v) C_\mathrm{ref}(\lambda_\mathrm{B},v)   \\                                   &= ( F_{\star}(\lambda,v) - F(\lambda,t,v) ) C_\mathrm{ref}(\lambda_\mathrm{B},v)   \\                                   &= ( F_{\star}(\lambda,v) - F_{\star}(\lambda,t,v) + f_p(\lambda,v) ( S_\mathrm{thick}(B,t) + S_\mathrm{thin}(\lambda,t) ) - F_p(\lambda,t)  ) C_\mathrm{ref}(\lambda_\mathrm{B},v)          Here we make the assumption that :math:`F_{\star}(\lambda,t,v) \sim F_{\star}(\lambda,v)`, but care must be taken not to neglect uncertainties on :math:`F_{\star}(\lambda,t,v)` when propagating errors, even if uncertainties on the reference :math:`F_{\star}(\lambda,v)` can be neglected.    .. math::       F_\mathrm{res}(\lambda,t,v) &= ( f_p(\lambda,v) ( S_\mathrm{thick}(B,t) + S_\mathrm{thin}(\lambda,t) ) -  F_p(\lambda,t) ) C_\mathrm{ref}(\lambda_\mathrm{B},v)  \\                                &= ( f_p(\lambda,v) S_p(\lambda,t) -  F_p(\lambda,t) ) C_\mathrm{ref}(\lambda_\mathrm{B},v)                                       Where :math:`S_p(\lambda,t)` represents the equivalent surface occulted by the opaque planetary disk and its optically thin atmosphere, at each wavelength.    If there is no contribution from the atmosphere, or its contamination is excluded         .. math::       F_\mathrm{res}(\lambda,t,v) = f_p(\lambda,v) S_\mathrm{thick}(B,t) C_\mathrm{ref}(\lambda_\mathrm{B},v)      CCFs computed on these :math:`F_\mathrm{res}` have the same contrast, FWHM, and RV between visits, as long as the intrinsic lines are comparable.            It is possible that :math:`F_{\star}(\lambda,v)` varies with time, during or outside of the transit, eg if a spot/plage is present on the star and changes during the observations (in particular with the star's rotation).    In that case, rather than :math:`F^\mathrm{mast}_{\star}(\lambda,v)` we would need to use a :math:`F_{\star}(\lambda,t,v)` representative of the star at the time of each exposure.    Binned disk-integrated profiles are calculated from spectra resampled directly on the table of each exposure, to avoid blurring spectral features, losing resolution, and introducing spurious features    when doing differences and ratio between the master and individual spectra (which we found to be the case if using a single master calculated on a common table and then resampled on the table of each exposure).    If a bin is undefined in the master and/or the exposure, it will be undefined in the local profile.    Args:        TBD        Returns:        None        """      print('   > Extracting residual profiles')    data_inst = data_dic[inst]    data_vis = data_inst[vis]        #Current rest frame    if data_dic['DI'][inst][vis]['rest_frame']!='star':print('         WARNING: disk-integrated profiles must be aligned')    data_dic['Res'][inst][vis]['rest_frame'] = 'star'    #Path to initialized local data    proc_gen_data_paths_new=gen_dic['save_data_dir']+'Res_data/'+inst+'_'+vis+'_'    #Exposures for which local profiles will be extracted    #    - the user can request extraction for in-transit exposures alone (to avoid computing time)    #      we force the extraction for all exposures if a common master is used for the extraction (ie, when exposures are resampled on a common table) and no time is required to recalculate the master for each exposure    if data_dic['Res']['extract_in'] and ('spec' in data_dic['Res']['type'][inst]) and (not data_vis['comm_sp_tab']):data_dic['Res'][inst][vis]['idx_to_extract'] = deepcopy(gen_dic[inst][vis]['idx_in'])    else:data_dic['Res'][inst][vis]['idx_to_extract'] =  np.arange(data_vis['n_in_visit'],dtype=int)     #Calculating    if (gen_dic['calc_res_data']):        print('         Calculating data')             #Phase range from which original exposures contributing to the master are taken        #    - we impose that a single master be used            bin_prop = {'bin_low':[-0.5],'bin_high':[0.5]}          #Binning mode        #   - using current visit exposures only, or exposures from multiple visits        if (inst in data_dic['Res']['vis_in_bin']) and (len(data_dic['Res']['vis_in_bin'][inst])>0):            mode='multivis'            vis_to_bin = data_dic['Res']['vis_in_bin'][inst]                          #Planets associated with the binned visits            transit_pl = []            for vis_bin in vis_to_bin:                transit_pl+=data_inst[vis_bin]['transit_pl']                if data_dic[inst][vis_bin]['type']!=data_vis['type']:stop('Binned disk-integrated profiles must be of the same type as processed visit')            transit_pl = list(np.unique(transit_pl))                                else:            mode=''            vis_to_bin = [vis]               transit_pl=data_vis['transit_pl']        #Automatic definition of reference planet for single-transiting planet          #    - for multiple planets the reference planet for the phase does not matter, we just requie that all exposures are selected and then the selection is done via their indexes        bin_prop['ref_pl'] = transit_pl[0]          if (len(transit_pl)>1) and (('pl_in_bin' in data_dic['DI']) and (inst in data_dic['DI']['pl_in_bin'])):bin_prop['ref_pl'] = data_dic['DI']['pl_in_bin'][inst]        #Initialize binning        #    - output tables contain a single value, associated with the single master (=binned profiles) used for the extraction         _,_,_,_,n_in_bin_all,idx_to_bin_all,dx_ov_all,_,idx_bin2orig,idx_bin2vis,idx_to_bin_unik = init_bin_prof('DI',bin_prop,data_dic['Res']['idx_in_bin'],'phase',coord_dic,inst,vis_to_bin,data_dic,gen_dic)        scaled_data_paths_vis = {}          iexp_no_plrange_vis = {}        exclu_rangestar_vis = {}        for vis_bin in vis_to_bin:            if gen_dic['flux_sc']:scaled_data_paths_vis[vis_bin] = data_dic[inst][vis_bin]['scaled_DI_data_paths']            else:scaled_data_paths_vis[vis_bin] = None            if ('DI_Mast' in data_dic['Atm']['no_plrange']):iexp_no_plrange_vis[vis_bin] = data_dic['Atm'][inst][vis_bin]['iexp_no_plrange']            else:iexp_no_plrange_vis[vis_bin] = {}            exclu_rangestar_vis[vis_bin] = data_dic['Atm'][inst][vis_bin]['exclu_range_star']                #Retrieving data that will be used in the binning to define the master disk-integrated profile        #    - in process_bin_prof() all profiles are resampled on the common table before being binned, thus they can be resampled when uploaded the first time        #    - here the binned profiles must be defined on the table of each processed exposure, so the components of the weight profile are retrieved here and then either copied or resampled if necessary for each exposure        #      here a single binned profile (the master) is calculated, thus 'idx_to_bin_unik' is the same as idx_to_bin_all, which contains a single element        data_to_bin_gen={}            gdet4weight = gen_dic['cal_weight'] & data_vis['mean_gdet']        for iexp_off in idx_to_bin_unik:            data_to_bin_gen[iexp_off]={}            #Original index and visit of contributing exposure            #    - index is relative to the global table            iexp_glob = idx_bin2orig[iexp_off]            vis_bin = idx_bin2vis[iexp_off]                        #Latest processed disk-integrated data and associated tables            #    - profiles should have been aligned in the star rest frame and rescaled to their correct flux level, if necessary                      data_exp_off = dataload_npz(data_inst[vis_bin]['proc_DI_data_paths']+str(iexp_glob))            for key in ['cen_bins','edge_bins','flux','cond_def','cov']:data_to_bin_gen[iexp_off][key] = data_exp_off[key]            if data_vis['tell_sp']:data_to_bin_gen[iexp_off]['tell'] = dataload_npz(data_inst[vis_bin]['tell_DI_data_paths'][iexp_glob])['tell']                else:data_to_bin_gen[iexp_off]['tell'] = None            if gdet4weight:data_to_bin_gen[iexp_off]['mean_gdet'] = dataload_npz(data_inst[vis_bin]['mean_gdet_DI_data_paths'][iexp_glob])['mean_gdet']             else:data_to_bin_gen[iexp_off]['mean_gdet'] = None                                      #Master disk-integrated spectrum for weighing            #    - profile has been shifted to the same frame as the residual profiles, but is still defined on the common table, not the table of current exposure            #    - see process_binned_prof() for details            if gen_dic['DImast_weight']:                data_ref = dataload_npz(data_dic[inst][vis_bin]['mast_DI_data_paths'][iexp_glob])                data_to_bin_gen[iexp_off]['edge_bins_ref'] = data_ref['edge_bins']                data_to_bin_gen[iexp_off]['flux_ref'] = data_ref['flux']            #Weight profile            #    - only calculated here on a common table if:            # + binned profiles come from a single visit, defined on a common table for the visit            # + binned profiles come from multiple visits, defined on a common table for all visits                #    - the master spectrum should be processed in the star rest frame, so that the stellar lines do not contribute to weighing                     if ((mode=='') and data_vis['comm_sp_tab']) or ((mode=='multivis') and data_inst['comm_sp_tab']):                flux_ref_exp = np.ones(data_dic[inst][vis_bin]['dim_exp'])                  data_to_bin_gen[iexp_off]['weight'] = weights_bin_prof(range(data_inst['nord']),scaled_data_paths_vis[vis_bin],inst,vis_bin,gen_dic['corr_Fbal'],gen_dic['corr_FbalOrd'],gen_dic['save_data_dir'],gen_dic['type'],data_inst['nord'],iexp_glob,'DI',data_dic[inst]['type'],data_vis['dim_exp'],data_to_bin_gen[iexp_off]['tell'],data_to_bin_gen[iexp_off]['mean_gdet'],data_to_bin_gen[iexp_off]['cen_bins'],1.,flux_ref_exp,None,bdband_flux_sc = gen_dic['flux_sc'])              #Processing each exposure of current visit selected for extraction        iexp_proc = data_dic['Res'][inst][vis]['idx_to_extract']        common_args = (data_vis['proc_DI_data_paths'],mode,data_vis['comm_sp_tab'],data_inst['comm_sp_tab'],proc_gen_data_paths_new,idx_to_bin_all[0],n_in_bin_all[0],dx_ov_all[0],idx_bin2orig,idx_bin2vis,data_inst['com_vis'],data_dic[inst]['nord'],data_vis['dim_exp'],data_vis['tell_sp'],data_vis['nspec'],gen_dic['flux_sc'],gdet4weight,data_to_bin_gen,gen_dic['resamp_mode'],\                       scaled_data_paths_vis,inst,iexp_no_plrange_vis,exclu_rangestar_vis,data_dic[inst]['type'],gen_dic['type'],gen_dic['corr_Fbal'],gen_dic['corr_FbalOrd'],gen_dic['save_data_dir'])                       if gen_dic['nthreads_res_data']>1:MAIN_multithread(sub_extract_res_profiles,gen_dic['nthreads_res_data'],len(iexp_proc),[iexp_proc],common_args)                                   else:sub_extract_res_profiles(iexp_proc,*common_args)        #Checking that local data has been calculated for all exposures    else:        data_paths={iexp:proc_gen_data_paths_new+str(iexp) for iexp in range(data_vis['n_in_visit'])}        check_data(data_paths)                #Path to weighing master and calibration profile    #    - residual profiles are extracted in the same rest frame as the disk-integrated master, so that it can directly be used    #    - at this stage a single master has been defined over the common spectral table, it will be resampled in the binning routine    #    - calibration paths are updated even if they are not used as weights, to be used in flux/count scalings    data_vis['proc_Res_data_paths']=proc_gen_data_paths_new    if gen_dic['DImast_weight']:data_vis['mast_Res_data_paths'] = data_vis['mast_DI_data_paths']    if data_vis['tell_sp']:data_vis['tell_Res_data_paths'] = data_vis['tell_DI_data_paths']    if gen_dic['flux_sc']:data_vis['scaled_Res_data_paths'] = data_vis['scaled_DI_data_paths']    if data_vis['mean_gdet']:data_vis['mean_gdet_Res_data_paths'] = data_vis['mean_gdet_DI_data_paths']    return Nonedef sub_extract_res_profiles(iexp_proc,proc_DI_data_paths,mode,comm_sp_tab_vis,comm_sp_tab_inst,proc_gen_data_paths_new,idx_to_bin_mast,n_in_bin_mast,dx_ov_mast,idx_bin2orig,idx_bin2vis,com_vis,nord,dim_exp,tell_sp,nspec,flux_sc,gdet4weight,data_to_bin_gen,resamp_mode,\                             scaled_data_paths_vis,inst,iexp_no_plrange_vis,exclu_rangestar_vis,vis_type,gen_type,corr_Fbal,corr_FbalOrd,save_data_dir):    r"""**Residual profile extraction.**     Calculates residual profiles.        Args:        TBD        Returns:        None        """         #Processing each exposure of current visit selected for extraction    #    - extraction can be limited to in-transit exposures to gain computing time, e.g if one only needs to analyze the local stellar profiles     for isub,iexp in enumerate(iexp_proc):                       #Upload latest processed DI data from which to extract local profile        data_exp = dataload_npz(proc_DI_data_paths+str(iexp))        #Calculating master disk-integrated profile        #    - the master is calculated in a given exposure:        # + if it is the first one        # + if it is another one and binned profiles         #       come from a single visit, and do not share a common table for the visit        #       come from multiple visits, do not share a common table for all visits, and visit of the processed exposure is not the one used as reference for the common table of all visits (in which case resampling is not needed)        if (isub==0) or ((mode=='') and (not comm_sp_tab_vis)) or ((mode=='multivis') and (not comm_sp_tab_inst)):                            data_to_bin={}            for iexp_off in idx_to_bin_mast:                #Original index and visit of contributing exposure                #    - index is relative to the global table                iexp_glob = idx_bin2orig[iexp_off]                vis_bin = idx_bin2vis[iexp_off]                                    #Resampling on common spectral table if required                #    - data is stored with the same indexes as in idx_to_bin_all                #    - all exposures must be defined on the same spectral table before being binned                #    - if multiple visits are used and do not share a common table, they do not need resampling if their table is the one used as reference to set the common table                if ((mode=='') and (not comm_sp_tab_vis)) or ((mode=='multivis') and (not comm_sp_tab_inst) and (vis_bin!=com_vis)):                    data_to_bin[iexp_off]={}                                        #Resampling exposure profile                    data_to_bin[iexp_off]['flux']=np.zeros(dim_exp,dtype=float)*np.nan                    data_to_bin[iexp_off]['cov']=np.zeros(nord,dtype=object)                     tell_exp=np.ones(dim_exp,dtype=float) if tell_sp else None                    mean_gdet_exp=np.ones(dim_exp,dtype=float) if gdet4weight else None                    for iord in range(nord):                         data_to_bin[iexp_off]['flux'][iord],data_to_bin[iexp_off]['cov'][iord] = bind.resampling(data_exp['edge_bins'][iord], data_to_bin_gen[iexp_off]['edge_bins'][iord], data_to_bin_gen[iexp_off]['flux'][iord] , cov = data_to_bin_gen[iexp_off]['cov'][iord], kind=resamp_mode)                                                                                if tell_sp:tell_exp[iord] = bind.resampling(data_exp['edge_bins'][iord], data_to_bin_gen[iexp_off]['edge_bins'][iord], data_to_bin_gen[iexp_off]['tell'][iord] , kind=resamp_mode)                         if gdet4weight:mean_gdet_exp[iord] = bind.resampling(data_exp['edge_bins'][iord], data_to_bin_gen[iexp_off]['edge_bins'][iord],data_to_bin_gen[iexp_off]['mean_gdet'][iord], kind=resamp_mode)                           data_to_bin[iexp_off]['cond_def'] = ~np.isnan(data_to_bin[iexp_off]['flux'])                       #Weight definition                             flux_ref_exp = np.ones(dim_exp,dtype=float)                    data_to_bin[iexp_off]['weight'] = weights_bin_prof(range(nord),scaled_data_paths_vis[vis_bin],inst,vis_bin,corr_Fbal,corr_FbalOrd,save_data_dir,gen_type,nord,iexp_glob,'DI',vis_type,dim_exp,tell_exp,mean_gdet_exp,data_exp['cen_bins'],1.,flux_ref_exp,None,bdband_flux_sc = flux_sc)                #Weighing components and current exposure are defined on the same table common to the visit                 else:data_to_bin[iexp_off] = deepcopy(data_to_bin_gen[iexp_off])                  #Exclude planet-contaminated bins                  #    - condition that 'DI_Mast' is in 'no_plrange' is included in the definition of 'iexp_no_plrange_vis'                if (iexp_glob in iexp_no_plrange_vis[vis_bin]):                    for iord in range(nord):                                           data_to_bin[iexp_off]['cond_def'][iord] &=  excl_plrange(data_to_bin[iexp_off]['cond_def'][iord],exclu_rangestar_vis[vis_bin],iexp_off,data_exp['edge_bins'][iord],vis_type)[0]            #Calculate master on current exposure table            data_mast = calc_bin_prof(idx_to_bin_mast,nord,dim_exp,nspec,data_to_bin,inst,n_in_bin_mast,data_exp['cen_bins'],data_exp['edge_bins'],dx_ov_in = dx_ov_mast)        #Extracting residual stellar profiles          #    - the master is defined for each individual exposures if they are defined on different spectral table        #      otherwise defined on a single common spectral table, in which case we repeat the master to have the same structure as individual exposures                  data_loc = {'cen_bins':data_exp['cen_bins'],                    'edge_bins':data_exp['edge_bins'],                    'flux' : np.zeros(dim_exp, dtype=float),                    'cov' : np.zeros(nord, dtype=object)}        for iord in range(nord):            data_loc['flux'][iord],data_loc['cov'][iord]=bind.add(data_mast['flux'][iord], data_mast['cov'][iord], -data_exp['flux'][iord], data_exp['cov'][iord])                         data_loc['cond_def'] = ~np.isnan(data_loc['flux'])               #Saving data        #    - saved for each exposure, as the files are too large otherwise                        np.savez_compressed(proc_gen_data_paths_new+str(iexp),data=data_loc,allow_pickle=True)            return None################################################################################################## #%% Intrinsic profiles routines################################################################################################## def extract_intr_profiles(data_dic,gen_dic,inst,vis,star_params,coord_dic,theo_dic,plot_dic):    r"""**Main intrinsic profile routine.**     Extracts intrinsic profiles in the stellar rest frame.        The in-transit residual spectra, at wavelengths where planetary contamination was masked, correspond to    .. math::               F_\mathrm{res}(\mathrm{\lambda \, in \, B},t,v) &= ( f_p(\lambda,v) S(\lambda,t) -  F_p(\lambda,t) ) C_\mathrm{ref}(B,v)   \\                                                          &= f_p(\lambda,v) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v)                             With          - :math:`f_p` the surface density flux spectrum, assumed spatially constant over the region occulted by the planet,        known to a scaling factor :math:`C_\mathrm{ref}(B,v)`, assumed to be constant over the band, and accounting for the absolute flux level and deviations from the stellar SED.       - :math:`S_\mathrm{thick}(B,p)` the effective planet surface occulting the star in the band, assumed spectrally constant over the band, varying spatially during ingress/egress, and set by our choice of light curve.         The above expression consider only wavelengths :math:`\lambda` where there are no narrow absorption lines from the planetary atmosphere (absorbed wavelengths have been masked).            We scale back residual spectra to get back to the intrinsic stellar profiles (ie, without broadband planetary absorption and limb/grav-darkening), assuming that     .. math::             f_p(\mathrm{\lambda \, in \, B},v) = I(\mathrm{\lambda \, in \, B},t) \mathrm{LD}(B,t)            i.e. that the limb-darkening has low-frequency variations and does not affect the shape of the local intrinsic spectra.    The theoretical light curve used to rescale the data writes as (see `rescale_profiles()`) :    .. math::                 1 - \mathrm{LC}_\mathrm{theo}(B,t) = \mathrm{LC}_p(B,t) \frac{S_p(B,t)}{S_{\star}^\mathrm{LD}(B) }          Where the fluxes are constant and spatially uniform over the band and stellar disk, and the planet is described by a constant, mean radius over the band.    If we normalize the local spectra by this factor, we obtain the intrinsic spectra as    .. math::         F_\mathrm{intr}(\lambda,t,v) &= \frac{F_\mathrm{res}(\mathrm{\lambda \, in \, B},t,v)}{1 - \mathrm{LC}_\mathrm{theo}(B,t)} \\                                    &= \frac{f_p(\lambda,v) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v)}{1 - \mathrm{LC}_\mathrm{theo}(B,t)}  \\                                    &= \frac{I(\lambda,t) \mathrm{LD}(B,t) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v) S_{\star}^\mathrm{LD}(B)}{LD(B,t) S_p(B,t)}   \\                                    &= \frac{I(\lambda,t) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v) S_{\star}^\mathrm{LD}(B)}{Sp(B,t) }        During the full transit, the ratio :math:`S_r(B) = S_\mathrm{thick}(B,t)/S_p(B,t)` is constant over time.     During ingress/egress, we assume that the ratio remains the same, so that      .. math::             F_\mathrm{intr}(\lambda,t,v) = I(\lambda,t) F^\mathrm{norm}_\mathrm{ref}(B)        With     .. math::            F^\mathrm{norm}_\mathrm{ref} = S_r(B) C_\mathrm{ref}(B,v) S_{\star}^\mathrm{LD}(B)            Only dependent on the band. The normalized local spectra then allow comparing the shape of the intrinsic spectra along the transit chord in a given band.                    The continuum of the residual profiles is        .. math::         F_\mathrm{res}(B_\mathrm{cont},t,v) &= \sum_{\lambda \, in \, B_\mathrm{cont}}(I_p(\lambda,t) \mathrm{LD}_p(B,t) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v) d\lambda(\lambda,v))   \\                                           &= \sum_{\lambda \, in \, B_\mathrm{cont}}(I_p(\lambda,t) d\lambda(\lambda,v)) \mathrm{LD}_p(B,t) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v)   \\                                            &= I_p(B_\mathrm{cont},v) \mathrm{LD}_p(B,t) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v)                             If we define the continuum as a spectral range where the flux only varies due to broadband limb-darkening, we have :math:`I_p(B_\mathrm{cont},v) = I(B_\mathrm{cont},v)`        .. math::         F_{\star}(B_\mathrm{cont},v) &= \sum_{ x }(\sum_{\lambda \, in \, B_\mathrm{cont}}(I_x(\lambda,v) d\lambda(\lambda,v)) \mathrm{LD}_x(B,v) S_x )  \\                                    &= I(B_\mathrm{cont},v) S_{\star}^\mathrm{LD}(B)                         Thus the intrinsic continuum writes as        .. math::         F_\mathrm{intr}(B_\mathrm{cont},t,v) &= I(B_\mathrm{cont},v) S_r(B) C_\mathrm{ref}(B,v) S_{\star}^\mathrm{LD}(B)  \\                                            &= F_{\star}(B_\mathrm{cont},v) S_r(B) C_\mathrm{ref}(B,v)                            And the residual continuum writes as     .. math::                    F_\mathrm{res}(B_\mathrm{cont},t,v) &= \frac{F_{\star}(B_\mathrm{cont},v) \mathrm{LD}_p(B,t) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v)}{S_{\star}^\mathrm{LD}(B) }   \\                                                                   &= F_{\star}(B_\mathrm{cont},v) ( 1 - \mathrm{LC}_\mathrm{theo}(B,t) ) S_r(B,t) C_\mathrm{ref}(B,v)                          If :math:`S_r \sim 1` the intrinsic profiles have the same flux as the disk-integrated spectra before the relative broadband flux scaling.        .. math::         \sum_{\lambda \, in \, B_\mathrm{cont}}( \frac{F_\mathrm{sc}(\lambda,t,v) d\lambda(\lambda,t,v)}{\mathrm{LC}_\mathrm{theo}(B,t)} ) &= \sum_{\lambda \, in \, B_\mathrm{cont}}( \frac{ F_\mathrm{sc}(\lambda,t,v) d\lambda(\lambda,t,v) }{ \mathrm{LC}_\mathrm{theo}(B,t) } ) \\                                                                                                                                          &= \sum_{\lambda \, in \, B_\mathrm{cont}}( F_{\star}(\lambda,v) C_\mathrm{ref}(B,v) d\lambda(\lambda,t,v)) \\                                                                                                                                          &= F_{\star}(B_\mathrm{cont},v) C_\mathrm{ref}(B,v)                                                           Intrinsic profiles thus have the same continuum as the scaled out-of-transit and master disk-integrated profiles, within a range controlled by broadband flux variations (ie, outside of planetary and stellar lines) but this continuum may not be exactly unity.    Bins affected by the planet absorption must be included in the scaling band (rescale_profiles())), but after this operation is done we set all bins affected by the planetary atmosphere to nan so that the final profiles are purely stellar.          Here we do not shift the intrinsic stellar profiles to a common rest wavelength, as they can be later used to derive the velocity of the stellar surface.     The approach is the same with CCFs, except that everything is performed with a single band, and the scaling can be carried out in the CCF continuum (thus avoiding potential variations in the line shape)     - when CCFs are given as input or calculated before the flux scaling, their continuum is normalized to unity outside of the transit     - when CCFs are calculated from residual spectra the continuum is unknown a priori, as it depends on the reference spectrum to which each DI spectrum corresponds to, times the spectral flux scaling during transit.       The residual spectra write as :math:`F_\mathrm{res}(\lambda,t,v) = F_\mathrm{intr}(\lambda,t,v) (1 - \mathrm{LC}_\mathrm{theo}(B,t))`       when converting them into :math:`CCF_\mathrm{res}`, we also compute the equivalent :math:`CCF_\mathrm{sc}` of :math:`(1 - \mathrm{LC}_\mathrm{theo}(B,t))`       :math:`CCF_\mathrm{res}` are then converted into :math:`CCF_\mathrm{intr}` in this routine by dividing their continuum using :math:`CCF_\mathrm{sc}`        this is an approximation, since the spectral scaling cannot be isolated from :math:`F_\mathrm{intr}(\lambda,t,v)` when computing :math:`CCF_\mathrm{res}`, but it is the same approximation we do when scaling DI CCFs with a white light transit       we take this approach rather than first calculate :math:`F_\mathrm{intr}` and then its CCF because we need :math:`CCF_\mathrm{res}` to later derive the atmospheric CCFs       ideally though, one should keep processing spectra rather than convert residual profiles into CCFs        Args:        TBD        Returns:        None        """          print('   > Extracting intrinsic stellar profiles')      data_vis=data_dic[inst][vis]    gen_vis = gen_dic[inst][vis]        #Current rest frame    if data_dic['Res'][inst][vis]['rest_frame']!='star':print('WARNING: residual profiles must be aligned')    data_dic['Intr'][inst][vis]['rest_frame'] = 'star'    #Path to initialized intrinsic data    proc_gen_data_paths_new = gen_dic['save_data_dir']+'Intr_data/'+inst+'_'+vis    #Updating paths    #    - if no shifts are applied the associated profiles remain the same as those of the residual profiles, and their paths are not updated    #    - calibration paths are updated even if they are not used as weights, to be used in flux/count scalings    #    - paths are defined for each exposure for associated tables, to avoid copying tables from residual profiles and simply point from in-transit to global residual profiles    data_vis['proc_Intr_data_paths']=proc_gen_data_paths_new+'_'     if gen_dic['flux_sc']:data_vis['scaled_Intr_data_paths'] = data_vis['scaled_Res_data_paths']    if gen_dic['DImast_weight']:data_vis['mast_Intr_data_paths'] = {}    if data_vis['tell_sp']:data_vis['tell_Intr_data_paths'] = {}    if data_vis['mean_gdet']:data_vis['mean_gdet_Intr_data_paths'] = {}     for i_in,iexp in enumerate(gen_vis['idx_in']):        if gen_dic['DImast_weight']:data_vis['mast_Intr_data_paths'][i_in] = data_vis['mast_Res_data_paths'][iexp]        if data_vis['tell_sp']:data_vis['tell_Intr_data_paths'][i_in] = data_vis['tell_Res_data_paths'][iexp]        if data_vis['mean_gdet']:data_vis['mean_gdet_Intr_data_paths'][i_in] = data_vis['mean_gdet_Res_data_paths'][iexp]    #Correcting for relative chromatic shift        if ('spec' in data_vis['type']) and ('chrom' in data_dic['DI']['system_prop']):intr_rv_corr = True    else:intr_rv_corr=False    #Processing intrinsic data    if (gen_dic['calc_intr_data']):        print('         Calculating data')        plAtm_vis = data_dic['Atm'][inst][vis]        #Initialize in-transit indexes of defined intrinsic profiles        data_dic['Intr'][inst][vis]['idx_def'] = np.arange(data_vis['n_in_tr'],dtype=int)         #Correcting for relative chromatic shift        #    - for spectral data and chromatic occultation: the planet occults region of different size across the spectrum, so that        # the lines in a given spectral band are shifted by an average RV over the corresponding chromatic surface        #    - here we correct the intrinsic spectra for the chromatic RV deviation around the nominal planet-occulted RV        #    - this correction is performed here so that intrinsic profiles can be converted into CCF prior to the alignment module, in which        # a constant RV shift can then be applied        if intr_rv_corr:            ref_pl,dic_rv,idx_aligned = init_surf_shift(gen_dic,inst,vis,data_dic,'theo')                        #Resample aligned profiles on the common visit table if relevant            #    - for CCFs the common table has been centered on the systemic velocity             if (data_vis['comm_sp_tab']):                data_com = dataload_npz(data_vis['proc_com_data_paths'])                cen_bins_resamp, edge_bins_resamp = data_com['cen_bins'],data_com['edge_bins']            else:cen_bins_resamp, edge_bins_resamp = None,None          #Definition of intrinsic stellar profiles        for i_in,iexp in enumerate(gen_vis['idx_in']):            #Upload local stellar profile            data_exp = dataload_npz(data_vis['proc_Res_data_paths']+str(iexp))                        #Upload flux scaling            data_scaling_exp = dataload_npz(data_vis['scaled_Res_data_paths']+str(iexp))                  #Rescale local stellar profiles to a common flux level            #    - correcting for LD variation and planetary occultation            #    - the scaling spectrum is defined at all wavelengths, thus defined bins are unchanged             #      the scaling equals 0 for undefined pixels, thus we set the rescaling to 1 to avoid warnings            #    - the scaling may be entirely null, if the exposure is not actually overlapping with the stellar disk            #      in that case the profile is set to nan            if (data_scaling_exp['null_loc_flux_scaling']):                                #Set exposure as undefined                print('         Profile at idx '+str(iexp),'(global) = '+str(i_in)+' (in-tr) is undefined')                data_dic['Intr'][inst][vis]['idx_def'] = np.delete( data_dic['Intr'][inst][vis]['idx_def'], data_dic['Intr'][inst][vis]['idx_def']==i_in)                for iord in range(data_dic[inst]['nord']):                    data_exp['flux'][iord,:] = np.nan                    data_exp['cond_def'][iord,:] = False             else:                for iord in range(data_dic[inst]['nord']):                    cond_exp_ord = data_exp['cond_def'][iord]                    resc_ord = np.ones(data_vis['nspec'],dtype=float)                    resc_ord[cond_exp_ord] = 1./data_scaling_exp['loc_flux_scaling'](data_exp['cen_bins'][iord,cond_exp_ord])                    data_exp['flux'][iord],data_exp['cov'][iord] = bind.mul_array(data_exp['flux'][iord],data_exp['cov'][iord],resc_ord)                                #Correct for relative chromatic shift                if intr_rv_corr:                        #Radial velocity shifts set to the opposite of the planet-occulted surface rv associated with current exposure                    rv_surf_star,rv_surf_star_edge = def_surf_shift('theo_rel',dic_rv,i_in,data_exp,ref_pl,data_vis['type'],data_dic['DI']['system_prop'],data_dic[inst][vis]['dim_exp'],data_dic[inst]['nord'],data_dic[inst][vis]['nspec'])                     #Doppler shift                    spec_dopshift_cen = 1./gen_specdopshift(rv_surf_star)                    spec_dopshift_edge = 1./gen_specdopshift(rv_surf_star_edge)                        #Spectral RV correction of current exposure and complementary tables                    if data_vis['tell_sp']:data_exp['tell'] = dataload_npz(data_vis['tell_Res_data_paths'][iexp])['tell']                     if data_vis['mean_gdet']:data_exp['mean_gdet'] = dataload_npz(data_vis['mean_gdet_Res_data_paths'][iexp] )['mean_gdet']                     data_exp=align_data(data_exp,data_vis['type'],data_dic[inst]['nord'],data_dic[inst][vis]['dim_exp'],gen_dic['resamp_mode'],cen_bins_resamp,edge_bins_resamp,rv_surf_star,spec_dopshift_cen,rv_shift_edge = rv_surf_star_edge,spec_dopshift_edge=spec_dopshift_edge)                        #Saving aligned exposure and complementary tables                    if ('spec' in data_vis['type']):                        if data_vis['tell_sp']:                            data_vis['tell_Intr_data_paths'][i_in] = proc_gen_data_paths_new+'_tell'+str(i_in)                            np.savez_compressed(data_vis['tell_Intr_data_paths'][i_in], data = {'tell':data_exp['tell']},allow_pickle=True)                             data_exp.pop('tell')                        if data_vis['mean_gdet']:                            data_vis['mean_gdet_Intr_data_paths'][i_in] = proc_gen_data_paths_new+'_mean_gdet'+str(i_in)                            np.savez_compressed(data_vis['mean_gdet_Intr_data_paths'][i_in], data = {'mean_gdet':data_exp['mean_gdet']},allow_pickle=True)                             data_exp.pop('mean_gdet')                        #Spectral RV correction of weighing master                    if gen_dic['DImast_weight']:                        data_ref = dataload_npz(data_vis['mast_Res_data_paths'][iexp])                         data_ref_align=align_data(data_ref,data_vis['type'],data_dic[inst]['nord'],data_dic[inst][vis]['dim_exp'],gen_dic['resamp_mode'],cen_bins_resamp,edge_bins_resamp,rv_surf_star,spec_dopshift_cen,rv_shift_edge = rv_surf_star_edge,spec_dopshift_edge=spec_dopshift_edge)                                          data_vis['mast_Intr_data_paths'][i_in] = proc_gen_data_paths_new+'_ref'+str(i_in)                        np.savez_compressed(data_vis['mast_Intr_data_paths'][i_in],data=data_ref_align,allow_pickle=True)                    #Set to nan planetary ranges                #    - only if intrinsic spectra are not to be converted into CCFs, in which case the exclusion is applied after their conversion                if ('Intr' in data_dic['Atm']['no_plrange']) and (not gen_dic['Intr_CCF']) and (iexp in plAtm_vis['iexp_no_plrange']):                    cond_out_pl = np.ones(data_vis['dim_exp'],dtype=bool)                    for iord in range(data_dic[inst]['nord']):                                                cond_out_pl[iord] &=excl_plrange(data_exp['cond_def'][iord],plAtm_vis['exclu_range_star'],iexp,data_exp['edge_bins'][iord],data_vis['type'])[0]                    cond_in_pl = ~cond_out_pl                    data_exp['flux'][cond_in_pl]=np.nan                    data_exp['cond_def'][cond_in_pl]=False                            #Saving exclusion flag                    data_exp['plrange_exc'] = True                else:data_exp['plrange_exc'] = False                       #Saving data using in-transit indexes                          np.savez_compressed(proc_gen_data_paths_new+'_'+str(i_in),data=data_exp,allow_pickle=True)          #Save complementary data        np.savez_compressed(proc_gen_data_paths_new+'_add',data={'idx_def':data_dic['Intr'][inst][vis]['idx_def']},allow_pickle=True)                  else:        check_data({0:proc_gen_data_paths_new+'_add'})          data_dic['Intr'][inst][vis]['idx_def'] = dataload_npz(proc_gen_data_paths_new+'_add')['idx_def']      #Continuum level and correction    #    - at this stage, profiles in CCF mode always come from input CCF data    #      continuum is only calculated for spectral data if not converted later on (in which case continuum is calculated later on)    #    - if applied to intrinsic profiles derived from CCF data, planetary ranges have been excluded if requested    #      for spectral data the full order range is taken as continuum    if (data_vis['type']=='CCF') or (('spec' in data_vis['type']) and ((not gen_dic['Intr_CCF']) and (not gen_dic['spec_1D_Intr']))):        if data_dic['Intr']['calc_cont']:                       data_dic['Intr'][inst][vis]['mean_cont']=calc_Intr_mean_cont(data_vis['n_in_tr'],data_dic[inst]['nord'],data_dic[inst][vis]['nspec'],data_vis['proc_Intr_data_paths'],data_vis['type'],data_dic['Intr']['cont_range'],inst,data_dic['Intr']['cont_norm'],gen_dic['flag_err_inst'][inst])            np.savez_compressed(data_vis['proc_Intr_data_paths']+'_add',data={'mean_cont':data_dic['Intr'][inst][vis]['mean_cont']},allow_pickle=True)        else:            check_data({'0':data_vis['proc_Intr_data_paths']+'_add'},silent=True)            data_dic['Intr'][inst][vis]['mean_cont'] = dataload_npz(data_vis['proc_Intr_data_paths']+'_add')['mean_cont']    return Nonedef calc_Intr_mean_cont(n_in_tr,nord,nspec,proc_Intr_data_paths,data_type,cont_range,inst,cont_norm,flag_err_inst):    r"""**Intrinsic continuum calculation.**          Calculates common continuum level for intrinsic profiles.        The continuum level is defined as a weighted mean because local CCFs at the limbs can be very poorly defined due to the partial occultation and limb-darkening.        If intrinsic CCFs were calculated from input CCF profiles, their continuum flux should match that of the out-of-transit CCFs (beware however that the scaling of disk-integrated profiles is done over their full range, not just the continuum).    If residual or intrinsic profiles were converted from spectra, then their continuum is not know a priori.    As a general approach we thus calculate the continuum value here            Args:        TBD        Returns:        None        """         #Continuum level    cond_def_cont_all  = np.zeros([n_in_tr,nord,nspec],dtype=bool)    for i_in in range(n_in_tr):        data_exp = dataload_npz(proc_Intr_data_paths+str(i_in))          for iord in range(nord):            if np.sum(data_exp['cond_def'][iord])==0:cond_def_cont_all[i_in,iord] = True            else:                if (inst in cont_range) and (iord in cont_range[inst]):                    for bd_int in cont_range[inst][iord]:cond_def_cont_all[i_in,iord] |= (data_exp['edge_bins'][iord,0:-1]>=bd_int[0]) & (data_exp['edge_bins'][iord,1:]<=bd_int[1])                     else:cond_def_cont_all[i_in,:] = True                      cond_def_cont_all[i_in,iord] &= data_exp['cond_def'][iord]                cond_cont_com  = np.all(cond_def_cont_all,axis=0)     cont_intr = np.ones([n_in_tr,nord])    wcont_intr = np.ones([n_in_tr,nord])    for i_in in range(n_in_tr):        data_exp = dataload_npz(proc_Intr_data_paths+str(i_in))        for iord in range(nord):            if np.sum(data_exp['cond_def'][iord])>0:                cond_cont_com_ord = cond_cont_com[iord]                if np.sum(cond_cont_com_ord)==0.:stop('No pixels in common continuum')                 dcen_bins = data_exp['edge_bins'][iord,1:][cond_cont_com_ord] - data_exp['edge_bins'][iord,0:-1][cond_cont_com_ord]                                #Continuum flux of the intrinsic CCF and corresponding error                #    - calculated over the defined bins common to all residual and intrinsic profiles                #    - we use the covariance diagonal to define a representative weight, unless no errors are defined                              cont_intr[i_in,iord] = np.sum(data_exp['flux'][iord,cond_cont_com_ord]*dcen_bins)/np.sum(dcen_bins)                if flag_err_inst:wcont_intr[i_in,iord] = np.sum(dcen_bins**2.)/np.sum( data_exp['cov'][iord][0,cond_cont_com_ord]*dcen_bins**2. )                            else:                cont_intr[i_in,iord] = 0.                wcont_intr[i_in,iord] = 0.    #Continuum flux over all in-transit exposures    mean_cont=np.sum(cont_intr*wcont_intr,axis=0)/np.sum(wcont_intr,axis=0)          #Continuum correction    #    - intrinsic profiles can show deviations from the common continuum level they should have     #      here we set manually their continuum to the mean continuum of all intrinsic profiles before the correction    if cont_norm:            print('         Correcting intrinsic continuum')        for i_in in range(n_in_tr):            data_exp = dataload_npz(proc_Intr_data_paths+str(i_in))            for iord in range(nord):                cond_cont_com_ord = cond_cont_com[iord]                                #Continuum of current exposure                dcen_bins = data_exp['edge_bins'][iord,1:][cond_cont_com_ord] - data_exp['edge_bins'][iord,0:-1][cond_cont_com_ord]                cont_intr_exp = np.sum(data_exp['flux'][iord][cond_cont_com_ord]*dcen_bins)/np.sum(dcen_bins)                                #Correction factor                corr_exp = mean_cont[iord]/cont_intr_exp                    #Overwrite exposure data                data_exp['flux'][iord],data_exp['cov'][iord] = bind.mul_array(data_exp['flux'][iord],data_exp['cov'][iord],np.repeat(corr_exp,nspec))            datasave_npz(proc_Intr_data_paths+str(i_in),data_exp)           return mean_cont################################################################################################## #%% Planetary profiles routines################################################################################################## def extract_pl_profiles(data_dic,inst,vis,gen_dic):    r"""**Main atmospheric profile routine.**          Extracts planetary atmospheric profiles in the stellar rest frame.    Args:        TBD        Returns:        None        """      print('   > Extracting atmospheric stellar profiles')    data_vis = data_dic[inst][vis]    plAtm_vis = data_dic['Atm'][inst][vis]    #Current rest frame    if data_dic['Res'][inst][vis]['rest_frame']!='star':print('WARNING: residual profiles must be aligned')    data_dic['Atm'][inst][vis]['rest_frame'] = 'star'    #Indexes of in-transit exposures with defined estimates of local stellar profiles    idx_est_loc = dataload_npz(gen_dic['save_data_dir']+'Loc_estimates/'+data_dic['Intr']['opt_loc_data_corr']['corr_mode']+'/'+inst+'_'+vis)['idx_est_loc']    #Indexes of exposures with retrieved signal    if (data_dic['Atm']['pl_atm_sign']=='Absorption'):        #In-transit indexes        plAtm_vis['idx_def'] = idx_est_loc        #Corresponding global indexes        iexp_glob = np.array(gen_dic[inst][vis]['idx_in'])[idx_est_loc]    elif (data_dic['Atm']['pl_atm_sign']=='Emission'):        #Global indexes        plAtm_vis['idx_def'] = list(gen_dic[inst][vis]['idx_out']) + list(np.array(gen_dic[inst][vis]['idx_in'])[idx_est_loc])        iexp_glob = plAtm_vis['idx_def']             #Initializing path to atmospheric data    data_vis['proc_Atm_data_paths']=gen_dic['save_data_dir']+'Atm_data/'+data_dic['Atm']['pl_atm_sign']+'/'+inst+'_'+vis+'_'                    #Initialize path of weighing profiles for atmospheric exposures    #    - the weighing profiles include the master disk-integrated profile, and the best estimates of the local stellar profiles (if measured)    #    - best estimates are only defined for in-transit profiles, and paths must be defined relative to the indexes used to call atmpospheric profiles    #    - weighing master is defined on the common table for the visit    if (data_dic['Atm']['pl_atm_sign']=='Absorption') or ((data_dic['Atm']['pl_atm_sign']=='Emission') and data_dic['Intr']['cov_loc_star']):        data_vis['LocEst_Atm_data_paths'] = {}        if (data_dic['Atm']['pl_atm_sign']=='Absorption'):iexp_paths = idx_est_loc     #in-transit indexes        elif (data_dic['Atm']['pl_atm_sign']=='Emission'):iexp_paths = np.array(gen_dic[inst][vis]['idx_in'])[idx_est_loc]    #global indexes, limited to in-transit values        data_vis['LocEst_Atm_data_paths'] = {iexp:gen_dic['save_data_dir']+'Loc_estimates/'+data_dic['Intr']['opt_loc_data_corr']['corr_mode']+'/'+inst+'_'+vis+'_'+str(i_in) for iexp,i_in in zip(iexp_paths,idx_est_loc)}        #Calculating    if (gen_dic['calc_pl_atm']):        print('         Calculating data')             #Data for absorption signal        if (data_dic['Atm']['pl_atm_sign']=='Absorption'):            #Properties of planet-occulted regions            dic_plocc_prop = np.load(gen_dic['save_data_dir']+'Introrig_prop/PlOcc_Prop_'+inst+'_'+vis+'.npz',allow_pickle=True)['data'].item()                                  #Process all exposures        for iexp,i_in in zip(range(data_vis['n_in_visit']),gen_dic[inst][vis]['idx_exp2in']):            #Upload local profile            #    - the local stellar profiles defined in the star rest frame write as             # Fres(w,t,vis) = ( fp(w,vis)*(Sthick(band,t) + Sthin(w-wp,t) ) -  Fatm(w-wp,t) )*Cref(band)/Fr(vis)             #      we want to retrieve the atmospheric emission signal Fatm, and the atmospheric absorption surface Sthin            data_loc = np.load(data_vis['proc_Res_data_paths']+str(iexp)+'.npz',allow_pickle=True)['data'].item()                                         #Upload estimate of local stellar profile for in-transit exposures            #    - we distinguish between theoretical estimates and ones derived from data in the calculation of the covariance below             if (i_in>-1) and (i_in in idx_est_loc):data_loc_star = np.load(gen_dic['save_data_dir']+'Loc_estimates/'+data_dic['Intr']['opt_loc_data_corr']['corr_mode']+'/'+inst+'_'+vis+'_'+str(i_in)+'.npz',allow_pickle=True)['data'].item()                                       #Extraction of emission signal            #    - out-of-transit we take the opposite of the local profiles to retrieve the emission signal            # F_em(w,t,vis) = - Fres(w,t,vis)             #               = Fatm(w-wp,t)*Cref(band)/Fr(vis)              #    - in-transit, the estimates of local stellar profiles correspond to             # Fstar_loc(w,t) = fp(w,vis)*Sthick(band,t)*Cref(band)/Fr(vis)             #      and we define the emission signal as                # F_em(w,t,vis) = Fstar_loc(w,t) - Fres(w,t,vis)             #               = Fatm(w-wp,t)*Cref(band)/Fr(vis) - fp(w,vis)*Sthin(w-wp,t )*Cref(band)/Fr(vis)            #      thus the emission signal will remain contaminated if there is an absorption signal            #    - unless the exact stellar SED for each visit was used to correct for the color balance, and to set spectra to the correct overall flux level in each visit, the            # emission signals will be known to a scaling factor Cref(band)/Fr(vis)                                                                                     if (data_dic['Atm']['pl_atm_sign']=='Emission') and (iexp in plAtm_vis['idx_def']):                data_em = {'cen_bins':data_loc['cen_bins'],'edge_bins':data_loc['edge_bins'],'tell':data_loc['tell']}                                              #Out-of-transit signal                if (i_in == -1):                    data_em['flux'] = -data_loc['flux']                    for key in ['cov','cond_def']:data_em[key] = data_loc[key]                #In-transit signal                #    - in-transit exposures with no estimates of local stellar profiles cannot be retrieved                elif (i_in in idx_est_loc):                    if not data_dic['Intr']['cov_loc_star']:                        data_em['flux'] = data_loc_star['flux']-data_loc['flux']                        data_em['cov'] = data_loc['cov']                    else:                        data_em['flux'] = np.zeros(data_vis['dim_exp'], dtype=float)                        data_em['cov'] = np.zeros(data_dic[inst]['nord'], dtype=object)                        for iord in range(data_dic[inst]['nord']):                            data_em['flux'][iord],data_em['cov'][iord]=bind.add(data_loc_star['flux'][iord], data_loc_star['cov'][iord],-data_loc['flux'][iord], data_loc['cov'][iord])                                     data_em['cond_def'] = ~np.isnan(data_em['flux'])                                 #Saving data                               np.savez_compressed(data_vis['proc_Atm_data_paths']+str(iexp),data=data_em,allow_pickle=True)                              #------------------------------------------------------------------------------------------------------------            #Extraction of absorption signal            #    - the absorption signal in-transit is retrieved as            # Abs(w,t,vis) = ( F_res(w,t,vis) - Fstar_loc(w,t,vis) ) / ( Fstar_loc(w,t,vis)/( Sthick(band,t)/Sstar ) )                                #      subtracting Fstar_loc(w,t,vis) removes the local stellar profile absorbed by the planetary continuum            #      dividing by Fstar_loc(w,t,vis) then removes the contribution of the local stellar profile            #      rescaling by Sthick(band,t)/Sstar finally replaces the scaling of the planet-occulted region surface by the full stellar surface, so that the result is comparable with classical absorption signal            #              = ( [ ( fp(w,vis)*(Sthick(band,t) + Sthin(w-wp,t) ) -  Fatm(w-wp,t) )*Cref(band)/Fr(vis) ]  - [ fp(w,vis)*Sthick(band,t)*Cref(band)/Fr(vis) ]  ) / ( [ fp(w,vis)*Sthick(band,t)*Cref(band)/Fr(vis) ]/( Sthick(band,t)/Sstar ) )                #              = ( ( fp(w,vis)*(Sthick(band,t) + Sthin(w-wp,t) ) -  Fatm(w-wp,t) )  -  fp(w,vis)*Sthick(band,t)  ) / ( fp(w,vis)*Sstar )                                 #              = ( fp(w,vis)*Sthin(w-wp,t) -  Fatm(w-wp,t) )/ ( fp(w,vis)*Sstar )                                 #              = Sthin(w-wp,t)/Sstar -  Fatm(w-wp,t)/( fp(w,vis)*Sstar )               #    - the calculation sums up as:            # Abs(w,t,vis) = [ F_res(w,t,vis)/Fstar_loc(w,t,vis)  - 1 ]*( Sthick(band,t)/Sstar )            #    - the absorption signal can be contaminated by an emission signal, however the latter likely varies over the planet orbit (thus preventing us to compute an out-of-transit master to be corrected from             # in-transit exposures) and is unlikely to be visible during transit in any case as it would arise from nightside emission            #      if no emission is present, the corrected spectra correspond to:            # Signal(w,t) = Sthin(w-wp,t )/Sstar            #    - we use a numerical estimate of Sthick(band,t)/Sstar with a constant Sstar, so that we extract the pure atmospheric spectral surface, normalized            # by a constant stellar surface to be equivalent to an absorption signal, but unbiased by a spectral stellar surface            #    - if we consider that there is an absorption signal outside of the transit defined by the input light curve, ie that a region of the planetary atmosphere is absorbing            # in a specific line but not in the continuum:            # F_res(w,t,vis) = ( fp(w,vis)*Sthin(w-wp,t) -  Fatm(w-wp,t) )*Cref(band)/Fr(vis)             if (data_dic['Atm']['pl_atm_sign']=='Absorption') and (i_in>-1) and (i_in in idx_est_loc):                #Planet-to-star surface ratios                SpSstar_spec = np.zeros([data_dic[inst]['nord'],data_vis['nspec']],dtype=float)                                                             #Achromatic/chromatic planet-to-star radius ratio                #    - for now a single transiting planet is considered                if ('spec' in data_vis['type']) and ('chrom' in data_dic['DI']['system_prop']):SpSstar_chrom = True                else:                    if len(data_vis['transit_pl'])>1:stop()                    SpSstar_spec[:,:] = dic_plocc_prop['achrom'][data_vis['transit_pl'][0]]['SpSstar'][0,i_in]                     SpSstar_chrom = False                             #Processing each order                data_abs = {'cen_bins':data_loc['cen_bins'],'edge_bins':data_loc['edge_bins'],                            'flux' : np.zeros(data_vis['dim_exp'], dtype=float),                            'cov' : np.zeros(data_dic[inst]['nord'], dtype=object)}                for iord in range(data_dic[inst]['nord']):                                        #Chromatic planet-to-star radius ratio                    if SpSstar_chrom:                         SpSstar_spec[iord] = np_interp(data_loc['cen_bins'][iord],data_dic['DI']['system_prop']['chrom']['w'],dic_plocc_prop['chrom']['SpSstar'][:,i_in],left=dic_plocc_prop['chrom']['SpSstar'][0,i_in],right=dic_plocc_prop['chrom']['SpSstar'][-1,i_in])                    #Calculation of absorption signal                                                                if data_dic['Intr']['cov_loc_star']:dat_temp,cov_temp = bind.div(data_loc['flux'][iord],data_loc['cov'][iord],data_loc_star['flux'][iord], data_loc_star['cov'][iord])                    else:dat_temp,cov_temp = bind.mul_array(data_loc['flux'][iord],data_loc['cov'][iord],1./data_loc_star['flux'][iord])                    data_abs['flux'][iord],data_abs['cov'][iord] = bind.mul_array(dat_temp-1.,cov_temp,SpSstar_spec[iord])                data_abs['cond_def'] = ~np.isnan(data_abs['flux'])                                                          data_abs['SpSstar_spec'] = SpSstar_spec                                       #Saving data                               np.savez_compressed(data_vis['proc_Atm_data_paths']+str(i_in),data=data_abs,allow_pickle=True)                    #------------------------------------------------------------------------------------------------------------                    #Checking that local data has been calculated for all exposures    else:        data_paths={iexp:data_vis['proc_Atm_data_paths']+str(iexp) for iexp in plAtm_vis['idx_def']}                check_data(data_paths)    #Path to associated tables    #    - atmospheric profiles are extracted in the same frame as residual profiles    #    - indexes may be limited to in-transit indexes if absorption signals are extracted    if gen_dic['DImast_weight']:data_vis['mast_Atm_data_paths'] = {}    if data_vis['tell_sp']:data_vis['tell_Atm_data_paths'] = {}    if data_vis['mean_gdet']:data_vis['mean_gdet_Atm_data_paths'] = {}    for iexp_atm,iexp in zip(plAtm_vis['idx_def'],iexp_glob):        if gen_dic['DImast_weight']:data_vis['mast_Atm_data_paths'][iexp_atm] = data_dic[inst][vis]['mast_Res_data_paths'][iexp]         if data_vis['tell_sp']:data_vis['tell_Atm_data_paths'][iexp_atm] = data_vis['tell_Res_data_paths'][iexp]         if data_vis['mean_gdet']:data_vis['mean_gdet_Atm_data_paths'][iexp_atm] = data_vis['mean_gdet_Res_data_paths'][iexp]     return None    
+#!/usr/bin/env python3# -*- coding: utf-8 -*-import numpy as npfrom copy import deepcopyimport bindensity as bindfrom scipy.interpolate import interp1dimport pandas as pdimport batmanfrom ..ANTARESS_grids.ANTARESS_occ_grid import init_surf_shift,def_surf_shift,sub_calc_plocc_spot_prop,retrieve_spots_prop_from_paramfrom ..ANTARESS_grids.ANTARESS_coord import get_timeorbit,calc_pl_coord,excl_plrangefrom ..ANTARESS_conversions.ANTARESS_binning import init_bin_prof,weights_bin_prof,calc_bin_proffrom ..ANTARESS_process.ANTARESS_data_align import align_datafrom ..ANTARESS_general.utils import dataload_npz,gen_specdopshift,stop,np_where1D,datasave_npz,np_interp,npint,MAIN_multithread,check_data################################################################################################## #%% Alignment routines##################################################################################################     #NB: cannot be put in file data_align.py with align_data() due to circular import issuesdef align_profiles(data_type,data_dic,inst,vis,gen_dic,coord_dic):    r"""**Main alignment routine.**        Aligns time-series of disk-integrated, intrinsic, and planetary profiles.      Profiles used as weights throughout the workflow are shifted in the same way as their associated profiles.    Args:        TBD        Returns:        None        """         data_inst = data_dic[inst]      data_vis=data_inst[vis]    print('   > Aligning '+gen_dic['type_name'][data_type]+' profiles')     prop_dic = data_dic[data_type]      proc_gen_data_paths_new = gen_dic['save_data_dir']+'Aligned_'+data_type+'_data/'+gen_dic['add_txt_path'][data_type]+'/'+inst+'_'+vis+'_'    if (data_type=='DI') and (data_dic['DI']['sysvel'][inst][vis]==0.):print('         WARNING: sysvel = 0 km/s')    if data_type=='Intr':proc_gen_data_paths_new+='in'      proc_mast = True if ((gen_dic['DImast_weight']) and (data_type in ['Intr','Atm'])) else False    proc_locEst = True if ((data_type=='Atm') and ((data_dic['Atm']['pl_atm_sign']=='Absorption') or ((data_dic['Atm']['pl_atm_sign']=='Emission')) and data_dic['Intr']['cov_loc_star'])) else False    #Resample aligned profiles on the common visit table if relevant    #    - for CCFs the common table is shifted by the systemic velocity to be centered in the star rest frame, as operations using this table will now be performed in the star rest frame, and the     # table can be short enough that resampling on the original table would lead to lost pixels    #      the input velocity table is usually centered around the CCF, ie around RV(CDM_star/CDM_sun)    #      resampling the CCFs corrected for this motion onto the input table would put them on a side, or even outside the table    #      we thus shift the table itself to keep the CCFs roughly centered in the table (there is no need to interpolate since this shift is common to all exposures)        if (data_vis['comm_sp_tab']):        data_com = dataload_npz(data_vis['proc_com_data_paths'])        if (data_type=='DI') and (data_vis['type']=='CCF'):                         #Use comon systemic velocity to keep all tables the same in case they are common to an instrument            if (data_inst['comm_sp_tab']) and (data_inst['n_visits_inst']>1):comm_sysvel = data_dic['DI']['sysvel'][inst][data_inst['com_vis']]              else:comm_sysvel=data_dic['DI']['sysvel'][inst][vis]                                     #Align common table            data_com['cen_bins'] -= comm_sysvel            data_com['edge_bins'] -= comm_sysvel            data_dic[inst][vis]['proc_com_data_paths'] = gen_dic['save_data_dir']+'Processed_data/'+inst+'_'+vis+'_com_star'            datasave_npz(data_dic[inst][vis]['proc_com_data_paths'],data_com)               cen_bins_resamp, edge_bins_resamp , dim_exp_resamp = data_com['cen_bins'],data_com['edge_bins'],data_com['dim_exp']     else:cen_bins_resamp, edge_bins_resamp , dim_exp_resamp = None,None,None       #Calculating aligned data    if gen_dic['calc_align_'+data_type]:        print('         Calculating data')        #Define RV shifts        #    - shifts are saved independently so that they can be used to account for the combined Doppler shifts        data_comp = {'rv_starbar_solbar':data_dic['DI']['sysvel'][inst][vis],'star_starbar' : {}}        if data_type=='DI':                         #Reflex motion and systemic velocity            prop_dic[inst][vis]['idx_def'] = range(data_vis['n_in_visit'])            rv_shifts = coord_dic[inst][vis]['RV_star_stelCDM'][prop_dic[inst][vis]['idx_def']] + data_dic['DI']['sysvel'][inst][vis]        elif data_type=='Intr':             data_comp['surf_star'] = {}                        #Surface RV             #    - indexes relative to in-transit table            ref_pl,dic_rv,prop_dic[inst][vis]['idx_def'] = init_surf_shift(gen_dic,inst,vis,data_dic,data_dic['Intr']['align_mode'])                    #Remove chromatic RVs            #    - chromatic deviations from the 'white' average rv of the occulted stellar surface (due to variations in the planet size and stellar intensity) were already             # corrected for when extracting the intrinsic profiles            if ('chrom' in dic_rv):dic_rv.pop('chrom')        elif data_type=='Atm':             data_comp['pl_star'] = {}                        #Orbital radial velocity of the planet calculated for each exposure in the star rest frame            if data_dic['Atm']['pl_atm_sign']=='Absorption':idx_def_atm = list(np.array(gen_dic[inst][vis]['idx_in'])[prop_dic[inst][vis]['idx_def']])            elif data_dic['Atm']['pl_atm_sign']=='Emission':idx_def_atm = prop_dic[inst][vis]['idx_def']            rv_shifts = coord_dic[inst][vis][data_dic['Atm']['ref_pl_align']]['rv_pl'][idx_def_atm]            v_orb = coord_dic[inst][vis][data_dic['Atm']['ref_pl_align']]['v_pl'][idx_def_atm]        #Processing each in-transit exposure        data_comp['idx_aligned'] = prop_dic[inst][vis]['idx_def']        for isub,iexp in enumerate(prop_dic[inst][vis]['idx_def']):                #Upload latest processed data            data_exp = dataload_npz(data_dic[inst][vis]['proc_'+data_type+'_data_paths']+str(iexp))            #RV shifts            data_comp['star_starbar'][iexp] = coord_dic[inst][vis]['RV_star_stelCDM'][iexp]            if data_type=='DI':                rv_shift_cen = rv_shifts[isub]                spec_dopshift = 1./gen_specdopshift(rv_shift_cen)                            elif data_type=='Intr':                                #Achromatic planet-occulted surface rv in the star rest frame                rv_shift_cen = def_surf_shift(prop_dic['align_mode'],dic_rv,iexp,data_exp,ref_pl,data_vis['type'],data_dic['DI']['system_prop'],data_dic[inst][vis]['dim_exp'],data_dic[inst]['nord'],data_dic[inst][vis]['nspec'])[0]                data_comp['surf_star'][iexp] = rv_shift_cen                spec_dopshift = 1./gen_specdopshift(rv_shift_cen)                            elif data_type=='Atm':                rv_shift_cen = rv_shifts[isub]                data_comp['pl_star'][iexp] = rv_shifts[isub]                spec_dopshift = 1./gen_specdopshift(rv_shift_cen , v_s = v_orb)                            #Doppler shift            #Aligning exposure profile and complementary tables            #    - the calibration profile is common to all exposures of a processed instrument, and is originally sampled over the table of each exposure in the detector rest frame            #    - the calibration profile is then used as weight in temporal binning, or to scale back profiles from flux to count units            #      in both cases the calibration profile must follow the same shifts as the exposure            if data_vis['tell_sp']:data_exp['tell'] = dataload_npz(data_vis['tell_'+data_type+'_data_paths'][iexp])['tell']             if data_vis['mean_gdet']:data_exp['mean_gdet'] = dataload_npz(data_vis['mean_gdet_'+data_type+'_data_paths'][iexp])['mean_gdet']             data_align=align_data(data_exp,data_vis['type'],data_dic[inst]['nord'],dim_exp_resamp,gen_dic['resamp_mode'],cen_bins_resamp, edge_bins_resamp,rv_shift_cen,spec_dopshift)            #Saving aligned exposure and complementary tables            if data_vis['tell_sp']:                np.savez_compressed(proc_gen_data_paths_new+'_tell'+str(iexp), data = {'tell':data_align['tell']},allow_pickle=True)                 data_align.pop('tell')            if data_vis['mean_gdet']:                np.savez_compressed(proc_gen_data_paths_new+'_mean_gdet'+str(iexp), data = {'mean_gdet':data_align['mean_gdet']},allow_pickle=True)                 data_align.pop('mean_gdet')            np.savez_compressed(proc_gen_data_paths_new+str(iexp),data=data_align,allow_pickle=True)            #Aligning weighing master            #    - called for intrinsic and atmospheric profiles, when they are shifted from the star rest frame to other frames            #      it is not called for DI profiles, since it is computed from DI profiles after alignment (ie, the disk-integrated master does not need further alignment)            #    - master is shifted for Intr and Atm types             #    - the master is originally defined in the star rest frame, like the residual and then intrinsic profiles, but on the common table for the visit            # + if profiles are shifted and resampled on the common table, this will also be the case of the associated master            # + if profiles are shifted but kept on their individual tables, the master will remain defined on the common table without being resampled, and it is this table that is shifted            #   the master table thus becomes specific to each exposure, but is still different from the table of the exposure            #    - path to the master associated with current profile is updated            if proc_mast:                data_ref = dataload_npz(data_vis['mast_'+data_type+'_data_paths'][iexp])                data_ref_align=align_data(data_ref,data_vis['type'],data_dic[inst]['nord'],dim_exp_resamp,gen_dic['resamp_mode'],cen_bins_resamp,edge_bins_resamp,rv_shift_cen,spec_dopshift)                np.savez_compressed(proc_gen_data_paths_new+'_ref'+str(iexp),data={'edge_bins':data_ref_align['edge_bins'],'flux':data_ref_align['flux'],'cov':data_ref_align['cov']},allow_pickle=True)                       #Retrieve and align estimate of local stellar profile for current exposure, if based on measured profiles            #    - required to weigh binned atmospheric profiles                            #    - only defined for in-transit exposures            if proc_locEst and (iexp in data_vis['LocEst_Atm_data_paths']):                data_est_loc=np.load(data_vis['LocEst_Atm_data_paths'][iexp]+'.npz',allow_pickle=True)['data'].item()                 data_est_loc_align=align_data(data_est_loc,data_vis['type'],data_dic[inst]['nord'],dim_exp_resamp,gen_dic['resamp_mode'],cen_bins_resamp, edge_bins_resamp,rv_shift_cen,spec_dopshift,nocov = ~data_dic['Intr']['cov_loc_star'])                 np.savez_compressed(proc_gen_data_paths_new+'estloc'+str(iexp),data=data_est_loc_align,allow_pickle=True)        #Updating path to processed data and saving complementary data        np.savez_compressed(proc_gen_data_paths_new+'_add',data=data_comp,allow_pickle=True)                                #Retrieving data    else:         #Updating path to processed data and checking it has been calculated        check_data({'path':proc_gen_data_paths_new+'_add'})     data_vis['proc_'+data_type+'_data_paths'] = proc_gen_data_paths_new     prop_dic[inst][vis]['idx_def'] = dataload_npz(data_vis['proc_'+data_type+'_data_paths']+'_add')['idx_aligned']        #Updating rest frame    #    - rest frame of disk-integrated spectra is not updated if systemic velocity is 0    if (data_type!='DI') or (data_dic['DI']['sysvel'][inst][vis]!=0.):        data_dic[data_type][inst][vis]['rest_frame'] = {'DI':'star','Intr':'surf','Atm':'pl'}[data_type]    if proc_mast:data_vis['mast_'+data_type+'_data_paths']={}    if proc_locEst:data_vis['LocEst_Atm_data_paths'] = {}    if data_vis['tell_sp']:data_vis['tell_'+data_type+'_data_paths']={}      if data_vis['mean_gdet']:data_vis['mean_gdet_'+data_type+'_data_paths']={}      for iexp in prop_dic[inst][vis]['idx_def']:        if proc_mast:data_vis['mast_'+data_type+'_data_paths'][iexp]=proc_gen_data_paths_new+'_ref'+str(iexp)        if proc_locEst and (iexp in data_vis['LocEst_Atm_data_paths']):data_vis['LocEst_Atm_data_paths'][iexp] = proc_gen_data_paths_new+'estloc'+str(iexp)         if data_vis['tell_sp']:data_vis['tell_'+data_type+'_data_paths'][iexp] = proc_gen_data_paths_new+'_tell'+str(iexp)        if data_vis['mean_gdet']:data_vis['mean_gdet_'+data_type+'_data_paths'][iexp] = proc_gen_data_paths_new+'_mean_gdet'+str(iexp)                  return None################################################################################################## #%% Flux scaling routines################################################################################################## def rescale_profiles(data_inst,inst,vis,data_dic,coord_dic,exp_dur_d,gen_dic,plot_dic,system_param,theo_dic,spot_dic={}):    r"""**Main flux scaling routine.**        Scales profiles to the correct relative broadband flux level.    Spectra :math:`F_\mathrm{corr}(\lambda,t,v)` should have been set to the same flux balance as a reference spectrum at low resolution using `corr_Fbal()`.    .. math::       F_\mathrm{corr}(\lambda,t,v) = F_{\star}(\lambda,v) C_\mathrm{ref}(\lambda,v) L(t)          Where :math:`C_\mathrm{ref}(\mathrm{\lambda \, in \, band \, B},v) \sim C_\mathrm{ref}(B,v)` represents a possible low-frequency deviation from the true stellar spectrum, and     `L(t)` represents the global flux deviation from the true stellar spectrum, not corrected for in previous modules.         We first convert all spectra from flux to (temporal) flux density units, so that they are equivalent except for flux variations.        We then correct for `L(t)` by dividing the profiles by     .. math::          F^\mathrm{glob}(v,t) &= \frac{\mathrm{TF}_\mathrm{corr}(v,t)}{\mathrm{median}(t_k, \mathrm{TF}_\mathrm{corr}(v,t_k) )}  \\       \mathrm{or}&  \\           F^\mathrm{glob}(v,t) &= \frac{\mathrm{TF}_\mathrm{corr}(v,t)}{F_\mathrm{sc} \int_{\mathrm{\lambda \, in \, full \, B}}{d\lambda }}            Where     .. math::         \mathrm{TF}_\mathrm{corr}(v,t) &= \int_{\mathrm{\lambda \, in \, full \, B}}{F_\mathrm{corr}(\lambda,t,v) d\lambda } \\                                      &= L(t) C     The exact value of the (unocculted) global flux level does not matter within a visit and is set to the median flux of all spectra,     unless the user choses to impose a common flux density for all visits (in case disk-integrated data needs to be combined between visits).              We then need to rescale spectrally the data so that     .. math::             F_\mathrm{sc}(\lambda,t) &= c(\lambda,t) F_\mathrm{corr}(\lambda,t) \\                                 &= F(\lambda,t)      To do so we use broadband spectral light curves, which by definition correspond to the ratio of in- and out-of-transit flux integrated over the band    .. math::             LC(B,v,t) &= \frac{ \int_{\mathrm{\lambda \, in \, B}}{F(\lambda,t) d\lambda }}{\int_{\mathrm{\lambda \, in \, B}}{F_{\star}(\lambda,v) d\lambda } } \\                    &= \frac{ \mathrm{TF}(B,t) }{ \mathrm{TF}_{\star}(B,v) }         We assume that :math:`c(\lambda,t)` has low-frequency variations (which should be the case, since the difference between :math:`F_\mathrm{corr}` and `F` comes from the changes in color balance).    The correction thus implies    .. math::             & \int_{\mathrm{\lambda \, in \, B}}{c(\lambda,t) F_\mathrm{corr}(\lambda,t) } = \int_{\mathrm{\lambda \, in \, B}}{ F(\lambda,t) }       \\                    & c(B,t) \int_{\mathrm{\lambda \, in \, B}}{F_\mathrm{corr}(\lambda,t) } = \mathrm{TF}(B,t)     \\       & c(B,t) = \frac{ \mathrm{TF}_{\star}(B,v) \mathrm{LC}(B,v,t) }{ \int_{\mathrm{\lambda \, in \, B}}{F_{\star}(\lambda,v) C_\mathrm{ref}(B,v) }  }   \\       & c(B,t) = \frac{ \mathrm{TF}_{\star}(B,v) \mathrm{LC}(B,v,t)}{  \mathrm{TF}_{\star}(B,v) C_\mathrm{ref}(B,v)  }  \\       & c(B,t) = \frac{ \mathrm{LC}(B,v,t) }{ C_\mathrm{ref}(B,v) }     We set :math:`c(B,t) = \mathrm{LC}_\mathrm{theo}(B,t)` and interpolate the chromatic `c(B,t)` at all wavelengths in the spectrum to define :math:`c(\lambda,t)`        .. math::             F_\mathrm{sc}(\lambda,t,v) &= \frac{ \mathrm{LC}_\mathrm{theo}(\lambda,t) F_\mathrm{corr}(\lambda,t)}{F^\mathrm{glob}(v,t)   }  \\                                  &= F(\lambda,t,v) C_\mathrm{ref}(B,v)                  Care must be taken about :math:`C_\mathrm{ref}(B,v)` when several visits are exploited        (1) if the stellar emission remains the same in all visits, then we can use a single theoretical spectrum / master as reference, and a constant normalized light curve               .. math::                F_\mathrm{sc}(\lambda,t,v) = F(\lambda,t,v) C_\mathrm{ref}(B)     (2) if the stellar emission changes in amplitude uniformly over the star, the normalized light curve remains the same, and the stellar spectrum keeps the same profile           .. math::                    &F_\mathrm{sc}(\lambda,t,v) = \frac{F(\lambda,t,v) C_\mathrm{ref}(B)}{F_r(v)}   \\           &\mathrm{where \,} F_r(v) = \frac{F_{\star}(\lambda,v)}{F_{\star}(\lambda,v_\mathrm{ref})}        The stellar spectrum of one of the visit :math:`F_{\star}(\lambda,v_\mathrm{ref})` is taken as reference, with                                                                                            .. math::            \mathrm{LC}_\mathrm{theo}(\lambda,t) &= \frac{F(\lambda,v_\mathrm{ref},t)}{F_{\star}(\lambda,v_\mathrm{ref})}  \\                                             &= \frac{F(\lambda,t,v)}{F_{\star}(\lambda,v)}         Thus                 .. math::            F_\mathrm{sc}(\lambda,t,v) &= \frac{F(\lambda,t,v) C_\mathrm{ref}(B) F_{\star}(\lambda,v_\mathrm{ref})}{F_{\star}(\lambda,v) }     \\                                              &= \frac{F(\lambda,v_\mathrm{ref},t) C_\mathrm{ref}(B) F_{\star}(\lambda,v_\mathrm{ref})}{F_{\star}(\lambda,v_\mathrm{ref}) }       \\                                            &= F(\lambda,v_\mathrm{ref},t) C_\mathrm{ref}(B)               Scaled spectra thus keep the same profile, deviating from the true profile by a common :math:`C_\mathrm{ref}(B)` in all visits.    (3) if the stellar emission changes in amplitude and shape uniformely over the star, the normalized light curve remains the same but the stellar spectrum has not the same profile        .. math::                   F_\mathrm{sc}(\lambda,t,v) &= \mathrm{LC}_\mathrm{theo}(\lambda,t) F(\lambda,v) C_\mathrm{ref}(\lambda,v) \\                                      &= (F(\lambda,v,t)/F_{\star}(\lambda,v)) F_{\star}(\lambda,t) C_\mathrm{ref}(B,v)  \\                                      &= F(\lambda,t,v) C_\mathrm{ref}(B,v)                    By using a reference spectrum specific to each visit when correcting the color balance, with the correct shape and relative flux, we would get                .. math::                        F_\mathrm{sc}(\lambda,t,v) = F(\lambda,t,v) C_\mathrm{ref}        Where :math:`C_\mathrm{ref}` is the deviation from the absolute flux level, common to all visits.     (4) if local stellar spectra in specific regions of the star change between visits, eg due to (un)occulted spots, then the normalized light curve changes as well.        Both a reference spectrum and a light curve specific to each visit must be used to remove the stellar contribution :math:`F_{\star}(\lambda,v)` and avoid introducing a different balance to the planet-occulted spectra.     If there is emission/reflection from the planet, then the true flux writes as        .. math::        F(\lambda,v,t) &= F_{\star}(\lambda,v) \mathrm{LC}^\mathrm{tr}(\lambda,v,t) + F_{\star}(\lambda,v) \mathrm{LC}^\mathrm{refl}(\lambda,v,t) + F_\mathrm{p}^\mathrm{thermal}(\lambda,v,t)      \\                      &= F_{\star}(\lambda,v) ( \delta_p^\mathrm{tr}(\lambda,v,t) + \delta_p^\mathrm{refl}(\lambda,v,t) + \delta_p^\mathrm{thermal}(\lambda,v,t) )   \\                      &= F_{\star}(\lambda,v) \delta_p(\lambda,v,t)                   The correction should still ensure that          .. math::             c(B,t) &= \frac{ \mathrm{TF}(B,v,t) }{  \mathrm{TF}_{\star}(B,v) C_\mathrm{ref}(B)  }    \\                 &= \frac{ \mathrm{LC}(B,v,t) \mathrm{TF}_{\star}(B,v) }{  \mathrm{TF}_{\star}(B,v) C_\mathrm{ref}(B)  }    \\                 &= \frac{ \mathrm{LC}(B,v,t) }{ C_\mathrm{ref}(B) }     But broadband spectral light curves correspond to          .. math::             \mathrm{LC}(B,v,t) &=  \frac{ \mathrm{TF}(B,v,t) }{   \mathrm{TF}_{\star}(B,v) }  \\                              &=  \frac{ \int_{\mathrm{\lambda \, in \, B}}, F_{\star}(\lambda,v) \delta_p(\lambda,v,t) d\lambda ) }{   \mathrm{TF}_{\star}(B,v)   }        So that care must be taken to use light curves that integrate the different spectral contributions and are then normalized by the integrated stellar flux, rather than integrating the pure planet contribution.                   For spectra, we can use the flux integrated over bands including the planetary absorption, as we can match it with the same band over which the light curve was measured.    Ideally the input light curves should be defined with a fine enough resolution to sample the low-frequency variations of the planetary atmosphere and stellar limb-darkening     For CCFs, a light curve does not match the cumulated flux of the different spectral regions used to calculate the CCF.     If we assume that the signature of the planet and of the RM effect is similar in all lines used to calculate the CCF, and that the light curve is achromatic, then it is similar to the scaling of a spectrum with a single line.    Thus, as with spectra, CCFs should be scaled using the flux of their full profile and not just the continuum (although there will always be a bias in using CCFs at this stage and the use of spectra should be preferred).    Since the scaling is imposed by a light curve independent of the spectra, bin by bin, it does not need to be applied to the full spectra like the flux balance color correction, and can be applied to any spectral range.     Note that the measured light curve corresponds to         .. math::           \mathrm{LC}(B,t) &= \frac{ \int_{\lambda \, in \, B}{ F_\mathrm{in}(\lambda,t) d\lambda } }{ \int_{\lambda \, in \, B}{ F_{\star}(\lambda,v) d\lambda }} \\                           &= 1 - \frac{\int_{ \lambda \, in \, B}{ f_p(\lambda) ( S_\mathrm{thick}(B,t) + S_\mathrm{thin}(\lambda,t) ) d\lambda} }{ <F_{\star}(\mathrm{\lambda \, in \, B},v)> }                          The theoretical light curves fitted to the measured one assume a constant, uniform stellar intensity `I` and limb-darkening law, and a constant average radius over the band        .. math::             \mathrm{LC}^\mathrm{theo}(B,t) &= \frac{ \mathrm{TF}^\mathrm{theo}(B,t) }{ \mathrm{TF}_{\star}^\mathrm{theo}(B) } \\                                         &= \frac{ F^\mathrm{theo}(B,t) }{ F_{\star}^\mathrm{theo}(B)  } \\                                         &= 1 - \frac{ I^\mathrm{theo}(B) \mathrm{LD}(B,t) S_p(B,t)}{\sum_{k}{ I^\mathrm{theo}(B) \mathrm{LD}_k(B) S_k }  } \\                                         &= 1 - \frac{ \mathrm{LD}(B,t) S_p(B,t)}{\sum_{k}{ \mathrm{LD}_k(B) S_k} } \\                                         &= 1 - \frac{ \mathrm{LD}(B,t) S_p(B,t)}{S_{\star}^\mathrm{LD}(B) }                     The fact that this is an approximation does not matter as long as the measured light curve is correctly reproduced, in which case the rescaling with the theoretical light curve is correct.    In the following we assume that the theoretical LD matches the true LD.                    Out-of-transit data is rescaled as well, to account for possible variations of stellar origin in the disk-integrated flux.      Args:        TBD        Returns:        None        """      print('   > Broadband flux scaling')     data_vis=data_inst[vis]    if data_dic['DI']['rescale_DI']:proc_DI_data_paths_new = gen_dic['save_data_dir']+'Scaled_data/'+inst+'_'+vis+'_'    else:proc_DI_data_paths_new = deepcopy(data_vis['proc_DI_data_paths'])    data_vis['scaled_DI_data_paths'] = proc_DI_data_paths_new+'scaling_'             #Default transit model    if (vis not in data_dic['DI']['transit_prop'][inst]):        data_dic['DI']['transit_prop'][inst][vis] = {'mode':'model','dt':np.min(coord_dic[inst][vis]['t_dur']/60.)/5.}        print('         Default transit model')    transit_prop=data_dic['DI']['transit_prop'][inst][vis]        #Flux scaling    if not data_dic['DI']['rescale_DI']:print('         No flux scaling applied')            #Calculating rescaled data    if (gen_dic['calc_flux_sc']):        print('         Calculating data')        dic_save={}            #Light curve for all bands and all exposures        #    - chromatic values are used if provided and if disk-integrated profiles are in spectral mode        if ('spec' in data_vis['type']) and ('chrom' in data_vis['system_prop']):key_chrom = ['chrom']        else:key_chrom = ['achrom']        system_prop = data_vis['system_prop'][key_chrom[0]]        LC_flux_band_all = np.zeros([data_vis['n_in_visit'],system_prop['nw']])*np.nan                    #Simulated light curves        if transit_prop['mode']=='simu':            params_LC = deepcopy(system_param['star'])            params_LC.update({'rv':0.,'cont':1.})             #Include spots in the LC generation            if (data_dic['DI']['spots_prop']!={}) and (inst in spot_dic['spots_prop']):params_LC['use_spots']=True            else:params_LC['use_spots']=False        #Calculate light curve for plotting                if (plot_dic['input_LC']!='') or (plot_dic['prop_Intr']!=''):                        #High-resolution time table over visit            min_bjd = coord_dic[inst][vis]['bjd'][0]            max_bjd = coord_dic[inst][vis]['bjd'][-1]            dbjd_HR = plot_dic['dt_LC']/(3600.*24.)            nbjd_HR = round((max_bjd-min_bjd)/dbjd_HR)            bjd_HR=min_bjd+dbjd_HR*np.arange(nbjd_HR)                  #Corresponding orbital phases and coordinates for each planet            #    - high-resolution tables are calculated assuming no exposure duration            coord_HR = {}            LC_HR=np.ones([nbjd_HR,system_prop['nw']],dtype=float)              if transit_prop['mode']=='simu':ecl_all_HR = np.zeros(nbjd_HR,dtype=bool)            for pl_loc in data_inst[vis]['transit_pl']:                pl_params_loc=system_param[pl_loc]                coord_HR[pl_loc]={'cen_ph':get_timeorbit(pl_loc,coord_dic[inst][vis],bjd_HR,pl_params_loc,None)[1]}                   #Definition of coordinates for all transiting planets                if transit_prop['mode']=='simu':                     x_pos_pl,y_pos_pl,z_pos_pl,Dprojp,_,_,_,_,ecl_pl = calc_pl_coord(pl_params_loc['ecc'],pl_params_loc['omega_rad'],pl_params_loc['aRs'],pl_params_loc['inclin_rad'],coord_HR[pl_loc]['cen_ph'],data_dic['DI']['system_prop']['achrom'][pl_loc][0],pl_params_loc['lambda_rad'],system_param['star'])                    coord_HR[pl_loc].update({'ecl':ecl_pl,'cen_pos':np.vstack((x_pos_pl,y_pos_pl,z_pos_pl))})                        #Exposure considered out-of-transit if no planet at all is transiting                    ecl_all_HR |= abs(ecl_pl)!=1                                  #Corresponding orbital phases and coordinates for each spot            for spot in data_inst[vis]['transit_sp']:                coord_HR[spot]={}                for key in ['Tcenter', 'ang', 'ang_rad', 'lat', 'ctrst']:coord_HR[spot][key] = np.zeros(len(bjd_HR),dtype=float)*np.nan                for key in ['lat_rad_exp','sin_lat_exp','cos_lat_exp','long_rad_exp','sin_long_exp','cos_long_exp','x_sky_exp','y_sky_exp','z_sky_exp']:coord_HR[spot][key] = np.zeros([3,len(bjd_HR)],dtype=float)*np.nan                coord_HR[spot]['is_visible'] = np.zeros([3,len(bjd_HR)],dtype=bool)            #Retrieving the spot coordinates for all the times that we have            if spot_dic!={} and ('spots_prop' in spot_dic) and (inst in spot_dic['spots_prop']) and (vis in spot_dic['spots_prop'][inst]):                HR_spot_params = deepcopy(spot_dic['spots_prop'][inst][vis])                HR_spot_params['cos_istar']=system_param['star']['cos_istar']                for itstamp, tstamp in enumerate(bjd_HR):                    spots_prop = retrieve_spots_prop_from_param(system_param['star'],HR_spot_params,inst,vis,tstamp,exp_dur=dbjd_HR)                    for spot in data_inst[vis]['transit_sp']:                        for key in ['Tcenter', 'ang', 'ang_rad', 'lat', 'ctrst']:                            coord_HR[spot][key][itstamp] = spots_prop[spot][key]                        for key in ['lat_rad_exp','sin_lat_exp','cos_lat_exp','long_rad_exp','sin_long_exp','cos_long_exp','x_sky_exp','y_sky_exp','z_sky_exp']:                            coord_HR[spot][key][:, itstamp] = [spots_prop[spot][key+'_start'],spots_prop[spot][key+'_center'],spots_prop[spot][key+'_end']]                        coord_HR[spot]['is_visible'][:, itstamp] = [spots_prop[spot]['is_start_visible'],spots_prop[spot]['is_center_visible'],spots_prop[spot]['is_end_visible']]        #------------------------------------------------------------------------                        #Light curves from import        #    - defined over a set of wavelengths that can be different for each visit        #    - here we import the light curves, so that they can be interpolated for each visit after their exposures have been defined        if transit_prop['mode']=='imp':            t_dur_d=coord_dic[inst][vis]['t_dur']/(3600.*24.)            cen_bjd = coord_dic[inst][vis]['bjd']                      #Retrieving light curve            #    - first column must be absolute time (BJD), to be independent of a specific planet             #    - next columns must be normalized stellar flux for all chosen bands, in the same order as data_dic['DI']['system_prop']['chrom']['w']            ext = transit_prop['path'].split('.')[-1]            if (ext=='csv'):                imp_LC = (pd.read_csv(transit_prop['path'])).values            elif (ext in ['txt','dat']):                imp_LC = np.loadtxt(transit_prop['path']).T                      else:                stop('Light curve path extension TBD')             imp_LC[0] -= 2400000.             if (plot_dic['input_LC']!=''):dic_save['imp_LC'] = imp_LC                     #Average imported light curve within the exposure time windows            #    - the light curve must be imported with sufficient temporal resolution            for iexp,(bjd_loc,dt_loc) in enumerate(zip(cen_bjd,t_dur_d)):                #Imported points within exposure                id_impLC=np_where1D( (imp_LC[0]>=bjd_loc-0.5*dt_loc) & (imp_LC[0]<=bjd_loc+0.5*dt_loc))                              #Normalized flux averaged within exposure                if len(id_impLC)>0:LC_flux_band_all[iexp,:]=np.mean(imp_LC[1::,id_impLC],axis=1)                else:stop('No LC measurements within exposure')            #Calculate light curve for plotting                    if (plot_dic['input_LC']!='') or (plot_dic['prop_Intr']!=''):                     for iband in range(system_prop['nw']):LC_HR[:,iband] = np_interp(bjd_HR,imp_LC[0],imp_LC[1+iband],left=imp_LC[1+iband,0],right=imp_LC[1+iband,-1])        #------------------------------------------------------------------------                #Model light curve for a single planet        #    - can be oversampled           #    - defined over a set of wavelengths but constant for each visit        elif transit_prop['mode']=='model':            if len(data_inst[vis]['transit_pl'])>1:stop('Multiple planets transiting')            pl_vis = data_inst[vis]['transit_pl'][0]            LC_params = batman.TransitParams()            LC_pl_params = system_param[pl_vis]                    #Phase reference for inferior conjunction            LC_params.t0 = 0.                         #Orbital period in phase            LC_params.per = 1.                         #Semi-major axis (in units of stellar radii)            LC_params.a = LC_pl_params['aRs']                        #Orbital inclination (in degrees)            #    - from the line of sight to the normal to the orbital plane            LC_params.inc = LC_pl_params['inclination']                         #Eccentricity            LC_params.ecc = LC_pl_params['ecc']                        #Longitude of periastron (in degrees)            LC_params.w = LC_pl_params['omega_deg']                        #Oversampling             if ('dt' not in transit_prop):LC_osamp = np.repeat(10,data_vis['n_in_visit'])            else:LC_osamp = npint(np.ceil(coord_dic[inst][vis]['t_dur']/(60.*transit_prop['dt'])))            if np.min(LC_osamp)<2.:print('WARNING: no oversampling of model light curve')                        #Calculate white or chromatic light curves            cen_ph_pl = coord_dic[inst][vis][pl_vis]['cen_ph']            ph_dur_pl=coord_dic[inst][vis][pl_vis]['ph_dur']            for iband,wband in enumerate(system_prop['w']):                    #Light curve properties for the band                LC_params_band = deepcopy(LC_params)                    #LD law                 LD_mod = system_prop['LD'][iband]                        #Limb darkening coefficients in the format required for batman                LC_params_band.limb_dark = LD_mod                if LD_mod == 'uniform':                    ld_coeff=[]                elif LD_mod == 'linear':                    ld_coeff=[system_prop['LD_u1'][iband]]                elif LD_mod in ['quadratic' ,'squareroot','logarithmic', 'power2' ,'exponential']:                    ld_coeff=[system_prop['LD_u1'][iband],system_prop['LD_u2'][iband]]                elif LD_mod == 'nonlinear':                       ld_coeff=[system_prop['LD_u1'][iband],system_prop['LD_u2'][iband],system_prop['LD_u3'][iband],system_prop['LD_u4'][iband]]                           else:                    stop('Limb-darkening not supported by batman')                  LC_params_band.u=ld_coeff                        #Planet-to-star radius ratio                LC_params_band.rp=system_prop[pl_vis][iband]                #All exposures have same duration                #    - process each band for all exposures together                if coord_dic[inst][vis]['cst_tdur']:                    LC_flux_band_all[:,iband] = batman.TransitModel(LC_params_band, cen_ph_pl, supersample_factor = LC_osamp[0], exp_time = ph_dur_pl[0]).light_curve(LC_params_band)                                    #Exposures have different durations                #    - process each band and each exposure                else:                                          for iexp,(cen_ph_exp,ph_dur_exp,LC_osamp_exp) in enumerate(zip(cen_ph_pl,ph_dur_pl,LC_osamp)):                                            LC_flux_band_all[iexp,iband]=float(batman.TransitModel(LC_params_band, np.array([cen_ph_exp]), supersample_factor = LC_osamp_exp, exp_time = np.array([ph_dur_exp])).light_curve(LC_params_band))                                        #Calculate light curve for plotting                        if (plot_dic['input_LC']!='') or (plot_dic['prop_Intr']!=''):                    LC_HR[:,iband] = batman.TransitModel(LC_params_band,coord_HR[pl_vis]['cen_ph']).light_curve(LC_params_band)                      #------------------------------------------------------------------------             #Simulated light curve           #    - can account for multiple transiting planets        elif transit_prop['mode']=='simu':                            #Set out-of-transit values to unity            if not params_LC['use_spots']:LC_flux_band_all[gen_dic[inst][vis]['idx_out'],:]=1.                                #Oversampling factor, in units of RpRs            theo_dic_LC= deepcopy(theo_dic)            theo_dic_LC['d_oversamp']={}            theo_dic_LC['n_oversamp_spot']={}            if (transit_prop['n_oversamp']>0.):                for pl_loc in data_inst[vis]['transit_pl']:theo_dic_LC['d_oversamp'][pl_loc]=data_dic['DI']['system_prop']['achrom'][pl_loc][0]/transit_prop['n_oversamp']             if params_LC['use_spots']:                for spot in data_inst[vis]['transit_sp']:theo_dic_LC['n_oversamp_spot'][spot]=1                            #Calculate transit light curves accounting for all planets in the visit            plocc_prop,spot_prop,_ = sub_calc_plocc_spot_prop(key_chrom,{},[],data_inst[vis]['transit_pl'],system_param,theo_dic_LC,data_dic['DI']['system_prop'],params_LC,coord_dic[inst][vis],gen_dic[inst][vis]['idx_in'],Ftot_star=True)             LC_flux_band_all[gen_dic[inst][vis]['idx_in'],:]=plocc_prop[key_chrom[0]]['Ftot_star'].T                           #Calculate transit light curves accounting for all planets in the visit            plocc_prop,spot_prop,common_prop = sub_calc_plocc_spot_prop(key_chrom,{},[],data_inst[vis]['transit_pl'],system_param,theo_dic_LC,data_dic['DI']['system_prop'],params_LC,coord_dic[inst][vis],gen_dic[inst][vis]['idx_in_and_out'],system_spot_prop_in=data_dic['DI']['spots_prop'],Ftot_star=True)             if not params_LC['use_spots']:                LC_flux_band_all[gen_dic[inst][vis]['idx_in'],:]=plocc_prop[key_chrom[0]]['Ftot_star'][:, gen_dic[inst][vis]['idx_in']].T            else:                LC_flux_band_all[gen_dic[inst][vis]['idx_in_and_out'],:]=common_prop[key_chrom[0]]['Ftot_star'].T                                                                                    #Calculate light curve for plotting                    if (plot_dic['input_LC']!='') or (plot_dic['prop_Intr']!=''):                theo_dic_LC['d_oversamp']={}                idx_in_HR = np_where1D(ecl_all_HR)                plocc_prop_HR,spot_prop_HR,_ = sub_calc_plocc_spot_prop(key_chrom,{},[],data_inst[vis]['transit_pl'],system_param,theo_dic_LC,data_dic['DI']['system_prop'],params_LC,coord_HR,idx_in_HR,Ftot_star=True)                 LC_HR[idx_in_HR,:]=plocc_prop_HR[key_chrom[0]]['Ftot_star'].T           #Store for plots        if (plot_dic['input_LC']!='') or (plot_dic['prop_Intr']!=''):            dic_save['flux_band_all'] = LC_flux_band_all            dic_save['coord_HR'] = coord_HR            dic_save['LC_HR'] = LC_HR        #------------------------------------------------------------------------        #Upload common spectral table        #    - if profiles are defined on different tables they are resampled on this one        #      if they are already defined on a common table, it is this one, which has been kept the same since the beginning of the routine        edge_bins_com = (np.load(data_vis['proc_com_data_paths']+'.npz',allow_pickle=True)['data'].item())['edge_bins']        #Spectral scaling table and global scaling range        loc_flux_scaling = np.zeros(data_vis['n_in_visit'],dtype=object)         flux_all = np.zeros(data_vis['dim_all'],dtype=float)*np.nan        cond_def_all = np.zeros(data_vis['dim_all'],dtype=bool)        cond_def_scal_all  = np.zeros(data_vis['dim_all'],dtype=bool)        null_loc_flux_scaling = np.ones(data_vis['n_in_visit'],dtype=bool)        for iexp in range(data_vis['n_in_visit']):                         #Latest processed DI data            data_exp = dataload_npz(data_vis['proc_DI_data_paths']+str(iexp))            #Resampling and conversion to temporal flux density            #    - if data were kept on independent tables they need to be resampled on a common one to calculate equivalent fluxes            if (not data_vis['comm_sp_tab']):                for iord in range(data_inst['nord']):                     flux_all[iexp,iord] = bind.resampling(edge_bins_com[iord], data_exp['edge_bins'][iord], data_exp['flux'][iord] , kind=gen_dic['resamp_mode'])                                                                        cond_def_all[iexp] = ~np.isnan(flux_all[iexp])               else:                flux_all[iexp] = data_exp['flux']                cond_def_all[iexp] = data_exp['cond_def']            flux_all[iexp]/=coord_dic[inst][vis]['t_dur'][iexp]            #Spectral scaling table                                                    #    - scale to the expected flux level at all wavelengths, using the broadband flux interpolated over the full spectrum range, unless a single band is used            #    - accounts for the potentially chromatic signature of the planet             #    - if the planet is not actually transiting (based on the determination of transit contacts) the 'null_loc_flux_scaling' flag is set to True            #      profile are still rescaled, with a light curve unity and 'loc_flux_scaling' equal to 0            if np.max(np.abs(1.-LC_flux_band_all[iexp]))>0.:null_loc_flux_scaling[iexp] = False            if (system_prop['nw']==1):loc_flux_scaling[iexp] = np.poly1d([1.-LC_flux_band_all[iexp,0]])            else:loc_flux_scaling[iexp] = interp1d(system_prop['w'],1.-LC_flux_band_all[iexp],fill_value=(1.-LC_flux_band_all[iexp,0],1.-LC_flux_band_all[iexp,-1]), bounds_error=False)                            #Requested scaling range            if len(data_dic['DI']['scaling_range'])>0:                cond_def_scal=False                 for bd_int in data_dic['DI']['scaling_range']:cond_def_scal |= (edge_bins_com[:,0:-1]>=bd_int[0]) & (edge_bins_com[:,1:]<=bd_int[1])               else:cond_def_scal=True             #Accounting for undefined pixels in scaling range                        cond_def_scal_all[iexp] = cond_def_all[iexp]  & cond_def_scal                    #Scaling pixels common to all exposures        #    - planetary signatures should not be excluded from the range of summation, for the same reason as they are included in the spectral scaling : the light curves used for the scaling include those ranges potentially absorbed by the planet        #      the same logic applies to CCF: their full range must be used for the scaling, and not just the continuum              cond_scal_com  = np.all(cond_def_scal_all,axis=0)        if np.sum(cond_scal_com)==0.:stop('No pixels in common scaling range')                  #Defining global scaling values        #    - used to set all profiles to a common global flux level        #    - spectral profiles have been trimmed, corrected, and aligned        #      it might thus be more accurate to rescale them using their own flux rather than the flux of the original spectra        #      furthermore masters afterward will be calculated from these profiles, scaled, thus they do not need to be set to the level of the original global master        #      we thus use the total flux summed over the full range of the current profiles, with their median taken as reference        #    - defined on temporal flux density (not cumulated photoelectrons counts)        Tflux_all = np.zeros(data_vis['n_in_visit'],dtype=float)        dcen_bin_comm = (edge_bins_com[:,1::] - edge_bins_com[:,0:-1])        Tcen_bin_comm = 0.        for iord in range(data_inst['nord']):                Tflux_all += np.sum(flux_all[:,iord,cond_scal_com[iord]]*dcen_bin_comm[iord,cond_scal_com[iord]],axis=1)            Tcen_bin_comm += np.sum(dcen_bin_comm[iord,cond_scal_com[iord]])        if data_dic['DI']['scaling_val'] is None:Tflux_ref = np.median(Tflux_all)        else:Tflux_ref=Tcen_bin_comm*data_dic['DI']['scaling_val']        norm_exp_glob = Tflux_all/Tflux_ref        #Scaling each exposure        #    - only defined bins are scaled (the flux in undefined bins remain set to nan), but the scaling spectrum was calculated at all wavelengths so that it can be used later with data for which different bins are defined or not        #    - all defined bins remain defined         #    - operation depends on condition 'rescale_DI' because flux scaling tbales may be required even if data needs not be scaled        for iexp in range(data_vis['n_in_visit']):                          #Scale and save exposure            if data_dic['DI']['rescale_DI']:                 data_exp = np.load(data_vis['proc_DI_data_paths']+str(iexp)+'.npz',allow_pickle=True)['data'].item()                 for iord in range(data_inst['nord']):                     LC_exp_spec_ord = 1.-loc_flux_scaling[iexp](data_exp['cen_bins'][iord])                    data_exp['flux'][iord],data_exp['cov'][iord] = bind.mul_array(data_exp['flux'][iord],data_exp['cov'][iord],LC_exp_spec_ord/(coord_dic[inst][vis]['t_dur'][iexp]*norm_exp_glob[iexp]))                datasave_npz(proc_DI_data_paths_new+str(iexp),data_exp)                        #Save scaling            #    - must be saved for each exposure because (for some reason) the interp1d function cannot be saved once passed out of multiprocessing             #    - in-transit scaling can be used later to manipulate local profiles from the planet-occulted regions             data_scaling = {'loc_flux_scaling':loc_flux_scaling[iexp],'glob_flux_scaling':norm_exp_glob[iexp],'null_loc_flux_scaling':null_loc_flux_scaling[iexp]}            if system_prop['nw']>1:data_scaling['chrom']=True            else:data_scaling['chrom']=False            datasave_npz(data_vis['scaled_DI_data_paths']+str(iexp),data_scaling)                          #Saving complementary data        dic_save['rest_frame']=data_dic['DI'][inst][vis]['rest_frame']        datasave_npz(proc_DI_data_paths_new+'add',dic_save)                       #Updating path to processed data and checking it has been calculated    else:           check_data({'path':proc_DI_data_paths_new+str(0)})       data_vis['proc_DI_data_paths'] = proc_DI_data_paths_new    return None    ################################################################################################## #%% Residual profiles routines################################################################################################## def extract_res_profiles(gen_dic,data_dic,inst,vis,data_prop,coord_dic):    r"""**Main residual profile routine.**     Extracts residual profiles in the stellar rest frame.    The real measured spectrum can be written as         .. math::           F(\lambda,t,v) = F_{\star}(\lambda,t,v) \delta_p(\lambda,t,v)      It can also be decomposed spatially as           .. math::       F(\lambda,t,v) &= (\sum_\mathrm{i \, not \, occulted}{F_i(\lambda,t,v)}) + f_p(\lambda,v) (S_\mathrm{occ}(t) - S_\mathrm{thick}(B,t) - S_\mathrm{thin}(\lambda,t) ) + F_p(\lambda,t)       \\                      &= F_{\star}(\lambda,t,v) - f_p(\lambda,v) ( S_\mathrm{thick}(B,t) + S_\mathrm{thin}(\lambda,t) ) + F_p(\lambda,t)               With          - :math:`\lambda` the absolute wavelength in the stellar rest frame, within a given spectral band.      - `F` the flux received from the star - planet system :math:`[erg \, s^{-1} \,  A^{-1} \, cm^{-2}]` at a given distance       :math:`F_i(\lambda,v) = f_i(\lambda,v) S_i` is the flux emitted by the region `i` of surface :math:`S_i`.     - the surface density flux can be written as :math:`f_i(\lambda,v) = I_i(\lambda) \mathrm{LD}_i(\lambda) \mathrm{GD}_i(\lambda)`.               + :math:`I_i(\lambda)` is the specific intensity in the direction of the LOS :math:`[erg \, s^{-1} \,  A^{-1} \, cm^{-2} \, sr^{-1}]`         which can be written as :math:`I_0(\lambda-\lambda_{\star}(t))` if the local stellar emission is constant over the stellar disk, and simply shifted by :math:`\lambda_{\star}(t)` because of surface velocity.       + :math:`\mathrm{LD}_i(\lambda)` is the spectral limb-darkening law.       + :math:`\mathrm{GD}_i(\lambda)` the gravity-darkening law.     - :math:`F_p(\lambda,t)` is the flux emitted or reflected by the planet.                       The planet and its atmosphere occult a surface :math:`S_\mathrm{occ}(t)`, time-dependent because of partial occultation at ingress/egress.           + :math:`S_\mathrm{thick}(B,t)` is the equivalent surface of the planet disk opaque to light in the local spectral band.        + :math:`S_\mathrm{thin}(\lambda,t)` is the equivalent surface of the atmospheric annulus optically thin to light in the band, varying at high frequency and null outside of narrow absorption lines.         + :math:`F_p(\lambda,t)` and :math:`S_\mathrm{thin}(\lambda,t)` are sensitive to the planet orbital motion, and shifted in the star rest frame by :math:`\lambda_\mathrm{pl}(t)`.        The measured profiles are now defined in the most general case as (see `rescale_profiles()`)        .. math::       F_\mathrm{sc}(\lambda,t,v) = F(\lambda,t,v) C_\mathrm{ref}(\lambda_\mathrm{B},v)     With :math:`F(\lambda,t,v)` the true spectrum.    Since all spectra were set to the same balance, corresponding to the stellar spectrum times a low-frequency coefficient, the master out corresponds in a given visit to     .. math::            F^\mathrm{mast}_{\star}(\lambda,v) = F_{\star}(\lambda,v) C_\mathrm{ref}(\lambda_\mathrm{B},v)      Note that the unknown scaling of the flux due to the distance to the star is implicitely included in :math:`C_\mathrm{ref}`.    We can decompose :math:`F_{\star}` as:               .. math::       F_{\star}(\lambda,v) = (\sum_\mathrm{i \, not \, occulted}{F_i(\lambda,v)}) + f_p(\lambda,v) S_\mathrm{occ}(t)                The local residual profiles are calculated as         .. math::       F_\mathrm{res}(\lambda,t,v) &= F^\mathrm{mast}_{\star}(\lambda,v) - F_\mathrm{sc}(\lambda,t,v)   \\                                                 &= F_{\star}(\lambda,v) C_\mathrm{ref}(\lambda_\mathrm{B},v)  - F(\lambda,t,v) C_\mathrm{ref}(\lambda_\mathrm{B},v)   \\                                   &= ( F_{\star}(\lambda,v) - F(\lambda,t,v) ) C_\mathrm{ref}(\lambda_\mathrm{B},v)   \\                                   &= ( F_{\star}(\lambda,v) - F_{\star}(\lambda,t,v) + f_p(\lambda,v) ( S_\mathrm{thick}(B,t) + S_\mathrm{thin}(\lambda,t) ) - F_p(\lambda,t)  ) C_\mathrm{ref}(\lambda_\mathrm{B},v)          Here we make the assumption that :math:`F_{\star}(\lambda,t,v) \sim F_{\star}(\lambda,v)`, but care must be taken not to neglect uncertainties on :math:`F_{\star}(\lambda,t,v)` when propagating errors, even if uncertainties on the reference :math:`F_{\star}(\lambda,v)` can be neglected.    .. math::       F_\mathrm{res}(\lambda,t,v) &= ( f_p(\lambda,v) ( S_\mathrm{thick}(B,t) + S_\mathrm{thin}(\lambda,t) ) -  F_p(\lambda,t) ) C_\mathrm{ref}(\lambda_\mathrm{B},v)  \\                                &= ( f_p(\lambda,v) S_p(\lambda,t) -  F_p(\lambda,t) ) C_\mathrm{ref}(\lambda_\mathrm{B},v)                                       Where :math:`S_p(\lambda,t)` represents the equivalent surface occulted by the opaque planetary disk and its optically thin atmosphere, at each wavelength.    If there is no contribution from the atmosphere, or its contamination is excluded         .. math::       F_\mathrm{res}(\lambda,t,v) = f_p(\lambda,v) S_\mathrm{thick}(B,t) C_\mathrm{ref}(\lambda_\mathrm{B},v)      CCFs computed on these :math:`F_\mathrm{res}` have the same contrast, FWHM, and RV between visits, as long as the intrinsic lines are comparable.            It is possible that :math:`F_{\star}(\lambda,v)` varies with time, during or outside of the transit, eg if a spot/plage is present on the star and changes during the observations (in particular with the star's rotation).    In that case, rather than :math:`F^\mathrm{mast}_{\star}(\lambda,v)` we would need to use a :math:`F_{\star}(\lambda,t,v)` representative of the star at the time of each exposure.    Binned disk-integrated profiles are calculated from spectra resampled directly on the table of each exposure, to avoid blurring spectral features, losing resolution, and introducing spurious features    when doing differences and ratio between the master and individual spectra (which we found to be the case if using a single master calculated on a common table and then resampled on the table of each exposure).    If a bin is undefined in the master and/or the exposure, it will be undefined in the local profile.    Args:        TBD        Returns:        None        """      print('   > Extracting residual profiles')    data_inst = data_dic[inst]    data_vis = data_inst[vis]        #Current rest frame    if data_dic['DI'][inst][vis]['rest_frame']!='star':print('         WARNING: disk-integrated profiles must be aligned')    data_dic['Res'][inst][vis]['rest_frame'] = 'star'    #Path to initialized local data    proc_gen_data_paths_new=gen_dic['save_data_dir']+'Res_data/'+inst+'_'+vis+'_'    #Exposures for which local profiles will be extracted    #    - the user can request extraction for in-transit exposures alone (to avoid computing time)    #      we force the extraction for all exposures if a common master is used for the extraction (ie, when exposures are resampled on a common table) and no time is required to recalculate the master for each exposure    if data_dic['Res']['extract_in'] and ('spec' in data_dic['Res']['type'][inst]) and (not data_vis['comm_sp_tab']):data_dic['Res'][inst][vis]['idx_to_extract'] = deepcopy(gen_dic[inst][vis]['idx_in'])    else:data_dic['Res'][inst][vis]['idx_to_extract'] =  np.arange(data_vis['n_in_visit'],dtype=int)     data_dic['Res'][inst][vis]['idx_def'] = data_dic['Res'][inst][vis]['idx_to_extract']     #Calculating    if (gen_dic['calc_res_data']):        print('         Calculating data')             #Phase range from which original exposures contributing to the master are taken        #    - we impose that a single master be used            bin_prop = {'bin_low':[-0.5],'bin_high':[0.5]}          #Binning mode        #   - using current visit exposures only, or exposures from multiple visits        if (inst in data_dic['Res']['vis_in_bin']) and (len(data_dic['Res']['vis_in_bin'][inst])>0):            mode='multivis'            vis_to_bin = data_dic['Res']['vis_in_bin'][inst]                          #Planets associated with the binned visits            transit_pl = []            for vis_bin in vis_to_bin:                transit_pl+=data_inst[vis_bin]['transit_pl']                if data_dic[inst][vis_bin]['type']!=data_vis['type']:stop('Binned disk-integrated profiles must be of the same type as processed visit')            transit_pl = list(np.unique(transit_pl))                                else:            mode=''            vis_to_bin = [vis]               transit_pl=data_vis['transit_pl']        #Automatic definition of reference planet for single-transiting planet          #    - for multiple planets the reference planet for the phase does not matter, we just requie that all exposures are selected and then the selection is done via their indexes        bin_prop['ref_pl'] = transit_pl[0]          if (len(transit_pl)>1) and (('pl_in_bin' in data_dic['DI']) and (inst in data_dic['DI']['pl_in_bin'])):bin_prop['ref_pl'] = data_dic['DI']['pl_in_bin'][inst]        #Initialize binning        #    - output tables contain a single value, associated with the single master (=binned profiles) used for the extraction         _,_,_,_,n_in_bin_all,idx_to_bin_all,dx_ov_all,_,idx_bin2orig,idx_bin2vis,idx_to_bin_unik = init_bin_prof('DI',bin_prop,data_dic['Res']['idx_in_bin'],'phase',coord_dic,inst,vis_to_bin,data_dic,gen_dic)        scaled_data_paths_vis = {}          iexp_no_plrange_vis = {}        exclu_rangestar_vis = {}        for vis_bin in vis_to_bin:            if gen_dic['flux_sc']:scaled_data_paths_vis[vis_bin] = data_dic[inst][vis_bin]['scaled_DI_data_paths']            else:scaled_data_paths_vis[vis_bin] = None            if ('DI_Mast' in data_dic['Atm']['no_plrange']):iexp_no_plrange_vis[vis_bin] = data_dic['Atm'][inst][vis_bin]['iexp_no_plrange']            else:iexp_no_plrange_vis[vis_bin] = {}            exclu_rangestar_vis[vis_bin] = data_dic['Atm'][inst][vis_bin]['exclu_range_star']                #Retrieving data that will be used in the binning to define the master disk-integrated profile        #    - in process_bin_prof() all profiles are resampled on the common table before being binned, thus they can be resampled when uploaded the first time        #    - here the binned profiles must be defined on the table of each processed exposure, so the components of the weight profile are retrieved here and then either copied or resampled if necessary for each exposure        #      here a single binned profile (the master) is calculated, thus 'idx_to_bin_unik' is the same as idx_to_bin_all, which contains a single element        data_to_bin_gen={}            gdet4weight = gen_dic['cal_weight'] & data_vis['mean_gdet']        for iexp_off in idx_to_bin_unik:            data_to_bin_gen[iexp_off]={}            #Original index and visit of contributing exposure            #    - index is relative to the global table            iexp_glob = idx_bin2orig[iexp_off]            vis_bin = idx_bin2vis[iexp_off]                        #Latest processed disk-integrated data and associated tables            #    - profiles should have been aligned in the star rest frame and rescaled to their correct flux level, if necessary                      data_exp_off = dataload_npz(data_inst[vis_bin]['proc_DI_data_paths']+str(iexp_glob))            for key in ['cen_bins','edge_bins','flux','cond_def','cov']:data_to_bin_gen[iexp_off][key] = data_exp_off[key]            if data_vis['tell_sp']:data_to_bin_gen[iexp_off]['tell'] = dataload_npz(data_inst[vis_bin]['tell_DI_data_paths'][iexp_glob])['tell']                else:data_to_bin_gen[iexp_off]['tell'] = None            if gdet4weight:data_to_bin_gen[iexp_off]['mean_gdet'] = dataload_npz(data_inst[vis_bin]['mean_gdet_DI_data_paths'][iexp_glob])['mean_gdet']             else:data_to_bin_gen[iexp_off]['mean_gdet'] = None                                      #Master disk-integrated spectrum for weighing            #    - profile has been shifted to the same frame as the residual profiles, but is still defined on the common table, not the table of current exposure            #    - see process_binned_prof() for details            if gen_dic['DImast_weight']:                data_ref = dataload_npz(data_dic[inst][vis_bin]['mast_DI_data_paths'][iexp_glob])                data_to_bin_gen[iexp_off]['edge_bins_ref'] = data_ref['edge_bins']                data_to_bin_gen[iexp_off]['flux_ref'] = data_ref['flux']            #Weight profile            #    - only calculated here on a common table if:            # + binned profiles come from a single visit, defined on a common table for the visit            # + binned profiles come from multiple visits, defined on a common table for all visits                #    - the master spectrum should be processed in the star rest frame, so that the stellar lines do not contribute to weighing                     if ((mode=='') and data_vis['comm_sp_tab']) or ((mode=='multivis') and data_inst['comm_sp_tab']):                flux_ref_exp = np.ones(data_dic[inst][vis_bin]['dim_exp'])                  data_to_bin_gen[iexp_off]['weight'] = weights_bin_prof(range(data_inst['nord']),scaled_data_paths_vis[vis_bin],inst,vis_bin,gen_dic['corr_Fbal'],gen_dic['corr_FbalOrd'],gen_dic['save_data_dir'],gen_dic['type'],data_inst['nord'],iexp_glob,'DI',data_dic[inst]['type'],data_vis['dim_exp'],data_to_bin_gen[iexp_off]['tell'],data_to_bin_gen[iexp_off]['mean_gdet'],data_to_bin_gen[iexp_off]['cen_bins'],1.,flux_ref_exp,None,bdband_flux_sc = gen_dic['flux_sc'])              #Processing each exposure of current visit selected for extraction        iexp_proc = data_dic['Res'][inst][vis]['idx_to_extract']        common_args = (data_vis['proc_DI_data_paths'],mode,data_vis['comm_sp_tab'],data_inst['comm_sp_tab'],proc_gen_data_paths_new,idx_to_bin_all[0],n_in_bin_all[0],dx_ov_all[0],idx_bin2orig,idx_bin2vis,data_inst['com_vis'],data_dic[inst]['nord'],data_vis['dim_exp'],data_vis['tell_sp'],data_vis['nspec'],gen_dic['flux_sc'],gdet4weight,data_to_bin_gen,gen_dic['resamp_mode'],\                       scaled_data_paths_vis,inst,iexp_no_plrange_vis,exclu_rangestar_vis,data_dic[inst]['type'],gen_dic['type'],gen_dic['corr_Fbal'],gen_dic['corr_FbalOrd'],gen_dic['save_data_dir'])                       if gen_dic['nthreads_res_data']>1:MAIN_multithread(sub_extract_res_profiles,gen_dic['nthreads_res_data'],len(iexp_proc),[iexp_proc],common_args)                                   else:sub_extract_res_profiles(iexp_proc,*common_args)        #Checking that local data has been calculated for all exposures    else:        data_paths={iexp:proc_gen_data_paths_new+str(iexp) for iexp in range(data_vis['n_in_visit'])}        check_data(data_paths)                #Path to weighing master and calibration profile    #    - residual profiles are extracted in the same rest frame as the disk-integrated master, so that it can directly be used    #    - at this stage a single master has been defined over the common spectral table, it will be resampled in the binning routine    #    - calibration paths are updated even if they are not used as weights, to be used in flux/count scalings    data_vis['proc_Res_data_paths']=proc_gen_data_paths_new    if gen_dic['DImast_weight']:data_vis['mast_Res_data_paths'] = data_vis['mast_DI_data_paths']    if data_vis['tell_sp']:data_vis['tell_Res_data_paths'] = data_vis['tell_DI_data_paths']    if gen_dic['flux_sc']:data_vis['scaled_Res_data_paths'] = data_vis['scaled_DI_data_paths']    if data_vis['mean_gdet']:data_vis['mean_gdet_Res_data_paths'] = data_vis['mean_gdet_DI_data_paths']    return Nonedef sub_extract_res_profiles(iexp_proc,proc_DI_data_paths,mode,comm_sp_tab_vis,comm_sp_tab_inst,proc_gen_data_paths_new,idx_to_bin_mast,n_in_bin_mast,dx_ov_mast,idx_bin2orig,idx_bin2vis,com_vis,nord,dim_exp,tell_sp,nspec,flux_sc,gdet4weight,data_to_bin_gen,resamp_mode,\                             scaled_data_paths_vis,inst,iexp_no_plrange_vis,exclu_rangestar_vis,vis_type,gen_type,corr_Fbal,corr_FbalOrd,save_data_dir):    r"""**Residual profile extraction.**     Calculates residual profiles.        Args:        TBD        Returns:        None        """         #Processing each exposure of current visit selected for extraction    #    - extraction can be limited to in-transit exposures to gain computing time, e.g if one only needs to analyze the local stellar profiles     for isub,iexp in enumerate(iexp_proc):                       #Upload latest processed DI data from which to extract local profile        data_exp = dataload_npz(proc_DI_data_paths+str(iexp))        #Calculating master disk-integrated profile        #    - the master is calculated in a given exposure:        # + if it is the first one        # + if it is another one and binned profiles         #       come from a single visit, and do not share a common table for the visit        #       come from multiple visits, do not share a common table for all visits, and visit of the processed exposure is not the one used as reference for the common table of all visits (in which case resampling is not needed)        if (isub==0) or ((mode=='') and (not comm_sp_tab_vis)) or ((mode=='multivis') and (not comm_sp_tab_inst)):                            data_to_bin={}            for iexp_off in idx_to_bin_mast:                #Original index and visit of contributing exposure                #    - index is relative to the global table                iexp_glob = idx_bin2orig[iexp_off]                vis_bin = idx_bin2vis[iexp_off]                                    #Resampling on common spectral table if required                #    - data is stored with the same indexes as in idx_to_bin_all                #    - all exposures must be defined on the same spectral table before being binned                #    - if multiple visits are used and do not share a common table, they do not need resampling if their table is the one used as reference to set the common table                if ((mode=='') and (not comm_sp_tab_vis)) or ((mode=='multivis') and (not comm_sp_tab_inst) and (vis_bin!=com_vis)):                    data_to_bin[iexp_off]={}                                        #Resampling exposure profile                    data_to_bin[iexp_off]['flux']=np.zeros(dim_exp,dtype=float)*np.nan                    data_to_bin[iexp_off]['cov']=np.zeros(nord,dtype=object)                     tell_exp=np.ones(dim_exp,dtype=float) if tell_sp else None                    mean_gdet_exp=np.ones(dim_exp,dtype=float) if gdet4weight else None                    for iord in range(nord):                         data_to_bin[iexp_off]['flux'][iord],data_to_bin[iexp_off]['cov'][iord] = bind.resampling(data_exp['edge_bins'][iord], data_to_bin_gen[iexp_off]['edge_bins'][iord], data_to_bin_gen[iexp_off]['flux'][iord] , cov = data_to_bin_gen[iexp_off]['cov'][iord], kind=resamp_mode)                                                                                if tell_sp:tell_exp[iord] = bind.resampling(data_exp['edge_bins'][iord], data_to_bin_gen[iexp_off]['edge_bins'][iord], data_to_bin_gen[iexp_off]['tell'][iord] , kind=resamp_mode)                         if gdet4weight:mean_gdet_exp[iord] = bind.resampling(data_exp['edge_bins'][iord], data_to_bin_gen[iexp_off]['edge_bins'][iord],data_to_bin_gen[iexp_off]['mean_gdet'][iord], kind=resamp_mode)                           data_to_bin[iexp_off]['cond_def'] = ~np.isnan(data_to_bin[iexp_off]['flux'])                       #Weight definition                             flux_ref_exp = np.ones(dim_exp,dtype=float)                    data_to_bin[iexp_off]['weight'] = weights_bin_prof(range(nord),scaled_data_paths_vis[vis_bin],inst,vis_bin,corr_Fbal,corr_FbalOrd,save_data_dir,gen_type,nord,iexp_glob,'DI',vis_type,dim_exp,tell_exp,mean_gdet_exp,data_exp['cen_bins'],1.,flux_ref_exp,None,bdband_flux_sc = flux_sc)                #Weighing components and current exposure are defined on the same table common to the visit                 else:data_to_bin[iexp_off] = deepcopy(data_to_bin_gen[iexp_off])                  #Exclude planet-contaminated bins                  #    - condition that 'DI_Mast' is in 'no_plrange' is included in the definition of 'iexp_no_plrange_vis'                if (iexp_glob in iexp_no_plrange_vis[vis_bin]):                    for iord in range(nord):                                           data_to_bin[iexp_off]['cond_def'][iord] &=  excl_plrange(data_to_bin[iexp_off]['cond_def'][iord],exclu_rangestar_vis[vis_bin],iexp_off,data_exp['edge_bins'][iord],vis_type)[0]            #Calculate master on current exposure table            data_mast = calc_bin_prof(idx_to_bin_mast,nord,dim_exp,nspec,data_to_bin,inst,n_in_bin_mast,data_exp['cen_bins'],data_exp['edge_bins'],dx_ov_in = dx_ov_mast)        #Extracting residual stellar profiles          #    - the master is defined for each individual exposures if they are defined on different spectral table        #      otherwise defined on a single common spectral table, in which case we repeat the master to have the same structure as individual exposures                  data_loc = {'cen_bins':data_exp['cen_bins'],                    'edge_bins':data_exp['edge_bins'],                    'flux' : np.zeros(dim_exp, dtype=float),                    'cov' : np.zeros(nord, dtype=object)}        for iord in range(nord):            data_loc['flux'][iord],data_loc['cov'][iord]=bind.add(data_mast['flux'][iord], data_mast['cov'][iord], -data_exp['flux'][iord], data_exp['cov'][iord])                         data_loc['cond_def'] = ~np.isnan(data_loc['flux'])               #Saving data        #    - saved for each exposure, as the files are too large otherwise                        np.savez_compressed(proc_gen_data_paths_new+str(iexp),data=data_loc,allow_pickle=True)            return None################################################################################################## #%% Intrinsic profiles routines################################################################################################## def extract_intr_profiles(data_dic,gen_dic,inst,vis,star_params,coord_dic,theo_dic,plot_dic):    r"""**Main intrinsic profile routine.**     Extracts intrinsic profiles in the stellar rest frame.        The in-transit residual spectra, at wavelengths where planetary contamination was masked, correspond to    .. math::               F_\mathrm{res}(\mathrm{\lambda \, in \, B},t,v) &= ( f_p(\lambda,v) S(\lambda,t) -  F_p(\lambda,t) ) C_\mathrm{ref}(B,v)   \\                                                          &= f_p(\lambda,v) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v)                             With          - :math:`f_p` the surface density flux spectrum, assumed spatially constant over the region occulted by the planet,        known to a scaling factor :math:`C_\mathrm{ref}(B,v)`, assumed to be constant over the band, and accounting for the absolute flux level and deviations from the stellar SED.       - :math:`S_\mathrm{thick}(B,p)` the effective planet surface occulting the star in the band, assumed spectrally constant over the band, varying spatially during ingress/egress, and set by our choice of light curve.         The above expression consider only wavelengths :math:`\lambda` where there are no narrow absorption lines from the planetary atmosphere (absorbed wavelengths have been masked).            We scale back residual spectra to get back to the intrinsic stellar profiles (ie, without broadband planetary absorption and limb/grav-darkening), assuming that     .. math::             f_p(\mathrm{\lambda \, in \, B},v) = I(\mathrm{\lambda \, in \, B},t) \mathrm{LD}(B,t)            i.e. that the limb-darkening has low-frequency variations and does not affect the shape of the local intrinsic spectra.    The theoretical light curve used to rescale the data writes as (see `rescale_profiles()`) :    .. math::                 1 - \mathrm{LC}_\mathrm{theo}(B,t) = \mathrm{LC}_p(B,t) \frac{S_p(B,t)}{S_{\star}^\mathrm{LD}(B) }          Where the fluxes are constant and spatially uniform over the band and stellar disk, and the planet is described by a constant, mean radius over the band.    If we normalize the local spectra by this factor, we obtain the intrinsic spectra as    .. math::         F_\mathrm{intr}(\lambda,t,v) &= \frac{F_\mathrm{res}(\mathrm{\lambda \, in \, B},t,v)}{1 - \mathrm{LC}_\mathrm{theo}(B,t)} \\                                    &= \frac{f_p(\lambda,v) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v)}{1 - \mathrm{LC}_\mathrm{theo}(B,t)}  \\                                    &= \frac{I(\lambda,t) \mathrm{LD}(B,t) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v) S_{\star}^\mathrm{LD}(B)}{LD(B,t) S_p(B,t)}   \\                                    &= \frac{I(\lambda,t) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v) S_{\star}^\mathrm{LD}(B)}{Sp(B,t) }        During the full transit, the ratio :math:`S_r(B) = S_\mathrm{thick}(B,t)/S_p(B,t)` is constant over time.     During ingress/egress, we assume that the ratio remains the same, so that      .. math::             F_\mathrm{intr}(\lambda,t,v) = I(\lambda,t) F^\mathrm{norm}_\mathrm{ref}(B)        With     .. math::            F^\mathrm{norm}_\mathrm{ref} = S_r(B) C_\mathrm{ref}(B,v) S_{\star}^\mathrm{LD}(B)            Only dependent on the band. The normalized local spectra then allow comparing the shape of the intrinsic spectra along the transit chord in a given band.                    The continuum of the residual profiles is        .. math::         F_\mathrm{res}(B_\mathrm{cont},t,v) &= \sum_{\lambda \, in \, B_\mathrm{cont}}(I_p(\lambda,t) \mathrm{LD}_p(B,t) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v) d\lambda(\lambda,v))   \\                                           &= \sum_{\lambda \, in \, B_\mathrm{cont}}(I_p(\lambda,t) d\lambda(\lambda,v)) \mathrm{LD}_p(B,t) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v)   \\                                            &= I_p(B_\mathrm{cont},v) \mathrm{LD}_p(B,t) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v)                             If we define the continuum as a spectral range where the flux only varies due to broadband limb-darkening, we have :math:`I_p(B_\mathrm{cont},v) = I(B_\mathrm{cont},v)`        .. math::         F_{\star}(B_\mathrm{cont},v) &= \sum_{ x }(\sum_{\lambda \, in \, B_\mathrm{cont}}(I_x(\lambda,v) d\lambda(\lambda,v)) \mathrm{LD}_x(B,v) S_x )  \\                                    &= I(B_\mathrm{cont},v) S_{\star}^\mathrm{LD}(B)                         Thus the intrinsic continuum writes as        .. math::         F_\mathrm{intr}(B_\mathrm{cont},t,v) &= I(B_\mathrm{cont},v) S_r(B) C_\mathrm{ref}(B,v) S_{\star}^\mathrm{LD}(B)  \\                                            &= F_{\star}(B_\mathrm{cont},v) S_r(B) C_\mathrm{ref}(B,v)                            And the residual continuum writes as     .. math::                    F_\mathrm{res}(B_\mathrm{cont},t,v) &= \frac{F_{\star}(B_\mathrm{cont},v) \mathrm{LD}_p(B,t) S_\mathrm{thick}(B,t) C_\mathrm{ref}(B,v)}{S_{\star}^\mathrm{LD}(B) }   \\                                                                   &= F_{\star}(B_\mathrm{cont},v) ( 1 - \mathrm{LC}_\mathrm{theo}(B,t) ) S_r(B,t) C_\mathrm{ref}(B,v)                          If :math:`S_r \sim 1` the intrinsic profiles have the same flux as the disk-integrated spectra before the relative broadband flux scaling.        .. math::         \sum_{\lambda \, in \, B_\mathrm{cont}}( \frac{F_\mathrm{sc}(\lambda,t,v) d\lambda(\lambda,t,v)}{\mathrm{LC}_\mathrm{theo}(B,t)} ) &= \sum_{\lambda \, in \, B_\mathrm{cont}}( \frac{ F_\mathrm{sc}(\lambda,t,v) d\lambda(\lambda,t,v) }{ \mathrm{LC}_\mathrm{theo}(B,t) } ) \\                                                                                                                                          &= \sum_{\lambda \, in \, B_\mathrm{cont}}( F_{\star}(\lambda,v) C_\mathrm{ref}(B,v) d\lambda(\lambda,t,v)) \\                                                                                                                                          &= F_{\star}(B_\mathrm{cont},v) C_\mathrm{ref}(B,v)                                                           Intrinsic profiles thus have the same continuum as the scaled out-of-transit and master disk-integrated profiles, within a range controlled by broadband flux variations (ie, outside of planetary and stellar lines) but this continuum may not be exactly unity.    Bins affected by the planet absorption must be included in the scaling band (rescale_profiles())), but after this operation is done we set all bins affected by the planetary atmosphere to nan so that the final profiles are purely stellar.          Here we do not shift the intrinsic stellar profiles to a common rest wavelength, as they can be later used to derive the velocity of the stellar surface.     The approach is the same with CCFs, except that everything is performed with a single band, and the scaling can be carried out in the CCF continuum (thus avoiding potential variations in the line shape)     - when CCFs are given as input or calculated before the flux scaling, their continuum is normalized to unity outside of the transit     - when CCFs are calculated from residual spectra the continuum is unknown a priori, as it depends on the reference spectrum to which each DI spectrum corresponds to, times the spectral flux scaling during transit.       The residual spectra write as :math:`F_\mathrm{res}(\lambda,t,v) = F_\mathrm{intr}(\lambda,t,v) (1 - \mathrm{LC}_\mathrm{theo}(B,t))`       when converting them into :math:`CCF_\mathrm{res}`, we also compute the equivalent :math:`CCF_\mathrm{sc}` of :math:`(1 - \mathrm{LC}_\mathrm{theo}(B,t))`       :math:`CCF_\mathrm{res}` are then converted into :math:`CCF_\mathrm{intr}` in this routine by dividing their continuum using :math:`CCF_\mathrm{sc}`        this is an approximation, since the spectral scaling cannot be isolated from :math:`F_\mathrm{intr}(\lambda,t,v)` when computing :math:`CCF_\mathrm{res}`, but it is the same approximation we do when scaling DI CCFs with a white light transit       we take this approach rather than first calculate :math:`F_\mathrm{intr}` and then its CCF because we need :math:`CCF_\mathrm{res}` to later derive the atmospheric CCFs       ideally though, one should keep processing spectra rather than convert residual profiles into CCFs        Args:        TBD        Returns:        None        """          print('   > Extracting intrinsic stellar profiles')      data_vis=data_dic[inst][vis]    gen_vis = gen_dic[inst][vis]        #Current rest frame    if data_dic['Res'][inst][vis]['rest_frame']!='star':print('WARNING: residual profiles must be aligned')    data_dic['Intr'][inst][vis]['rest_frame'] = 'star'    #Path to initialized intrinsic data    proc_gen_data_paths_new = gen_dic['save_data_dir']+'Intr_data/'+inst+'_'+vis    #Updating paths    #    - if no shifts are applied the associated profiles remain the same as those of the residual profiles, and their paths are not updated    #    - calibration paths are updated even if they are not used as weights, to be used in flux/count scalings    #    - paths are defined for each exposure for associated tables, to avoid copying tables from residual profiles and simply point from in-transit to global residual profiles    data_vis['proc_Intr_data_paths']=proc_gen_data_paths_new+'_'     if gen_dic['flux_sc']:data_vis['scaled_Intr_data_paths'] = data_vis['scaled_Res_data_paths']    if gen_dic['DImast_weight']:data_vis['mast_Intr_data_paths'] = {}    if data_vis['tell_sp']:data_vis['tell_Intr_data_paths'] = {}    if data_vis['mean_gdet']:data_vis['mean_gdet_Intr_data_paths'] = {}     for i_in,iexp in enumerate(gen_vis['idx_in']):        if gen_dic['DImast_weight']:data_vis['mast_Intr_data_paths'][i_in] = data_vis['mast_Res_data_paths'][iexp]        if data_vis['tell_sp']:data_vis['tell_Intr_data_paths'][i_in] = data_vis['tell_Res_data_paths'][iexp]        if data_vis['mean_gdet']:data_vis['mean_gdet_Intr_data_paths'][i_in] = data_vis['mean_gdet_Res_data_paths'][iexp]    #Correcting for relative chromatic shift        if ('spec' in data_vis['type']) and ('chrom' in data_dic['DI']['system_prop']):intr_rv_corr = True    else:intr_rv_corr=False    #Processing intrinsic data    if (gen_dic['calc_intr_data']):        print('         Calculating data')        plAtm_vis = data_dic['Atm'][inst][vis]        #Initialize in-transit indexes of defined intrinsic profiles        data_dic['Intr'][inst][vis]['idx_def'] = np.arange(data_vis['n_in_tr'],dtype=int)         #Correcting for relative chromatic shift        #    - for spectral data and chromatic occultation: the planet occults region of different size across the spectrum, so that        # the lines in a given spectral band are shifted by an average RV over the corresponding chromatic surface        #    - here we correct the intrinsic spectra for the chromatic RV deviation around the nominal planet-occulted RV        #    - this correction is performed here so that intrinsic profiles can be converted into CCF prior to the alignment module, in which        # a constant RV shift can then be applied        if intr_rv_corr:            ref_pl,dic_rv,idx_aligned = init_surf_shift(gen_dic,inst,vis,data_dic,'theo')                        #Resample aligned profiles on the common visit table if relevant            #    - for CCFs the common table has been centered on the systemic velocity             if (data_vis['comm_sp_tab']):                data_com = dataload_npz(data_vis['proc_com_data_paths'])                cen_bins_resamp, edge_bins_resamp = data_com['cen_bins'],data_com['edge_bins']            else:cen_bins_resamp, edge_bins_resamp = None,None          #Definition of intrinsic stellar profiles        for i_in,iexp in enumerate(gen_vis['idx_in']):            #Upload local stellar profile            data_exp = dataload_npz(data_vis['proc_Res_data_paths']+str(iexp))                        #Upload flux scaling            data_scaling_exp = dataload_npz(data_vis['scaled_Res_data_paths']+str(iexp))                  #Rescale local stellar profiles to a common flux level            #    - correcting for LD variation and planetary occultation            #    - the scaling spectrum is defined at all wavelengths, thus defined bins are unchanged             #      the scaling equals 0 for undefined pixels, thus we set the rescaling to 1 to avoid warnings            #    - the scaling may be entirely null, if the exposure is not actually overlapping with the stellar disk            #      in that case the profile is set to nan            if (data_scaling_exp['null_loc_flux_scaling']):                                #Set exposure as undefined                print('         Profile at idx '+str(iexp),'(global) = '+str(i_in)+' (in-tr) is undefined')                data_dic['Intr'][inst][vis]['idx_def'] = np.delete( data_dic['Intr'][inst][vis]['idx_def'], data_dic['Intr'][inst][vis]['idx_def']==i_in)                for iord in range(data_dic[inst]['nord']):                    data_exp['flux'][iord,:] = np.nan                    data_exp['cond_def'][iord,:] = False             else:                for iord in range(data_dic[inst]['nord']):                    cond_exp_ord = data_exp['cond_def'][iord]                    resc_ord = np.ones(data_vis['nspec'],dtype=float)                    resc_ord[cond_exp_ord] = 1./data_scaling_exp['loc_flux_scaling'](data_exp['cen_bins'][iord,cond_exp_ord])                    data_exp['flux'][iord],data_exp['cov'][iord] = bind.mul_array(data_exp['flux'][iord],data_exp['cov'][iord],resc_ord)                                #Correct for relative chromatic shift                if intr_rv_corr:                        #Radial velocity shifts set to the opposite of the planet-occulted surface rv associated with current exposure                    rv_surf_star,rv_surf_star_edge = def_surf_shift('theo_rel',dic_rv,i_in,data_exp,ref_pl,data_vis['type'],data_dic['DI']['system_prop'],data_dic[inst][vis]['dim_exp'],data_dic[inst]['nord'],data_dic[inst][vis]['nspec'])                     #Doppler shift                    spec_dopshift_cen = 1./gen_specdopshift(rv_surf_star)                    spec_dopshift_edge = 1./gen_specdopshift(rv_surf_star_edge)                        #Spectral RV correction of current exposure and complementary tables                    if data_vis['tell_sp']:data_exp['tell'] = dataload_npz(data_vis['tell_Res_data_paths'][iexp])['tell']                     if data_vis['mean_gdet']:data_exp['mean_gdet'] = dataload_npz(data_vis['mean_gdet_Res_data_paths'][iexp] )['mean_gdet']                     data_exp=align_data(data_exp,data_vis['type'],data_dic[inst]['nord'],data_dic[inst][vis]['dim_exp'],gen_dic['resamp_mode'],cen_bins_resamp,edge_bins_resamp,rv_surf_star,spec_dopshift_cen,rv_shift_edge = rv_surf_star_edge,spec_dopshift_edge=spec_dopshift_edge)                        #Saving aligned exposure and complementary tables                    if ('spec' in data_vis['type']):                        if data_vis['tell_sp']:                            data_vis['tell_Intr_data_paths'][i_in] = proc_gen_data_paths_new+'_tell'+str(i_in)                            np.savez_compressed(data_vis['tell_Intr_data_paths'][i_in], data = {'tell':data_exp['tell']},allow_pickle=True)                             data_exp.pop('tell')                        if data_vis['mean_gdet']:                            data_vis['mean_gdet_Intr_data_paths'][i_in] = proc_gen_data_paths_new+'_mean_gdet'+str(i_in)                            np.savez_compressed(data_vis['mean_gdet_Intr_data_paths'][i_in], data = {'mean_gdet':data_exp['mean_gdet']},allow_pickle=True)                             data_exp.pop('mean_gdet')                        #Spectral RV correction of weighing master                    if gen_dic['DImast_weight']:                        data_ref = dataload_npz(data_vis['mast_Res_data_paths'][iexp])                         data_ref_align=align_data(data_ref,data_vis['type'],data_dic[inst]['nord'],data_dic[inst][vis]['dim_exp'],gen_dic['resamp_mode'],cen_bins_resamp,edge_bins_resamp,rv_surf_star,spec_dopshift_cen,rv_shift_edge = rv_surf_star_edge,spec_dopshift_edge=spec_dopshift_edge)                                          data_vis['mast_Intr_data_paths'][i_in] = proc_gen_data_paths_new+'_ref'+str(i_in)                        np.savez_compressed(data_vis['mast_Intr_data_paths'][i_in],data=data_ref_align,allow_pickle=True)                    #Set to nan planetary ranges                #    - only if intrinsic spectra are not to be converted into CCFs, in which case the exclusion is applied after their conversion                if ('Intr' in data_dic['Atm']['no_plrange']) and (not gen_dic['Intr_CCF']) and (iexp in plAtm_vis['iexp_no_plrange']):                    cond_out_pl = np.ones(data_vis['dim_exp'],dtype=bool)                    for iord in range(data_dic[inst]['nord']):                                                cond_out_pl[iord] &=excl_plrange(data_exp['cond_def'][iord],plAtm_vis['exclu_range_star'],iexp,data_exp['edge_bins'][iord],data_vis['type'])[0]                    cond_in_pl = ~cond_out_pl                    data_exp['flux'][cond_in_pl]=np.nan                    data_exp['cond_def'][cond_in_pl]=False                            #Saving exclusion flag                    data_exp['plrange_exc'] = True                else:data_exp['plrange_exc'] = False                       #Saving data using in-transit indexes                          np.savez_compressed(proc_gen_data_paths_new+'_'+str(i_in),data=data_exp,allow_pickle=True)          #Save complementary data        np.savez_compressed(proc_gen_data_paths_new+'_add',data={'idx_def':data_dic['Intr'][inst][vis]['idx_def']},allow_pickle=True)                  else:        check_data({0:proc_gen_data_paths_new+'_add'})          data_dic['Intr'][inst][vis]['idx_def'] = dataload_npz(proc_gen_data_paths_new+'_add')['idx_def']      #Continuum level and correction    #    - at this stage, profiles in CCF mode always come from input CCF data    #      continuum is only calculated for spectral data if not converted later on (in which case continuum is calculated later on)    #    - if applied to intrinsic profiles derived from CCF data, planetary ranges have been excluded if requested    #      for spectral data the full order range is taken as continuum    if (data_vis['type']=='CCF') or (('spec' in data_vis['type']) and ((not gen_dic['Intr_CCF']) and (not gen_dic['spec_1D_Intr']))):        if data_dic['Intr']['calc_cont']:                       data_dic['Intr'][inst][vis]['mean_cont']=calc_Intr_mean_cont(data_vis['n_in_tr'],data_dic[inst]['nord'],data_dic[inst][vis]['nspec'],data_vis['proc_Intr_data_paths'],data_vis['type'],data_dic['Intr']['cont_range'],inst,data_dic['Intr']['cont_norm'],gen_dic['flag_err_inst'][inst])            np.savez_compressed(data_vis['proc_Intr_data_paths']+'_add',data={'mean_cont':data_dic['Intr'][inst][vis]['mean_cont']},allow_pickle=True)        else:            check_data({'0':data_vis['proc_Intr_data_paths']+'_add'},silent=True)            data_dic['Intr'][inst][vis]['mean_cont'] = dataload_npz(data_vis['proc_Intr_data_paths']+'_add')['mean_cont']    return Nonedef calc_Intr_mean_cont(n_in_tr,nord,nspec,proc_Intr_data_paths,data_type,cont_range,inst,cont_norm,flag_err_inst):    r"""**Intrinsic continuum calculation.**          Calculates common continuum level for intrinsic profiles.        The continuum level is defined as a weighted mean because local CCFs at the limbs can be very poorly defined due to the partial occultation and limb-darkening.        If intrinsic CCFs were calculated from input CCF profiles, their continuum flux should match that of the out-of-transit CCFs (beware however that the scaling of disk-integrated profiles is done over their full range, not just the continuum).    If residual or intrinsic profiles were converted from spectra, then their continuum is not know a priori.    As a general approach we thus calculate the continuum value here            Args:        TBD        Returns:        None        """         #Continuum level    cond_def_cont_all  = np.zeros([n_in_tr,nord,nspec],dtype=bool)    for i_in in range(n_in_tr):        data_exp = dataload_npz(proc_Intr_data_paths+str(i_in))          for iord in range(nord):            if np.sum(data_exp['cond_def'][iord])==0:cond_def_cont_all[i_in,iord] = True            else:                if (inst in cont_range) and (iord in cont_range[inst]):                    for bd_int in cont_range[inst][iord]:cond_def_cont_all[i_in,iord] |= (data_exp['edge_bins'][iord,0:-1]>=bd_int[0]) & (data_exp['edge_bins'][iord,1:]<=bd_int[1])                     else:cond_def_cont_all[i_in,:] = True                      cond_def_cont_all[i_in,iord] &= data_exp['cond_def'][iord]                cond_cont_com  = np.all(cond_def_cont_all,axis=0)     cont_intr = np.ones([n_in_tr,nord])    wcont_intr = np.ones([n_in_tr,nord])    for i_in in range(n_in_tr):        data_exp = dataload_npz(proc_Intr_data_paths+str(i_in))        for iord in range(nord):            if np.sum(data_exp['cond_def'][iord])>0:                cond_cont_com_ord = cond_cont_com[iord]                if np.sum(cond_cont_com_ord)==0.:stop('No pixels in common continuum')                 dcen_bins = data_exp['edge_bins'][iord,1:][cond_cont_com_ord] - data_exp['edge_bins'][iord,0:-1][cond_cont_com_ord]                                #Continuum flux of the intrinsic CCF and corresponding error                #    - calculated over the defined bins common to all residual and intrinsic profiles                #    - we use the covariance diagonal to define a representative weight, unless no errors are defined                              cont_intr[i_in,iord] = np.sum(data_exp['flux'][iord,cond_cont_com_ord]*dcen_bins)/np.sum(dcen_bins)                if flag_err_inst:wcont_intr[i_in,iord] = np.sum(dcen_bins**2.)/np.sum( data_exp['cov'][iord][0,cond_cont_com_ord]*dcen_bins**2. )                            else:                cont_intr[i_in,iord] = 0.                wcont_intr[i_in,iord] = 0.    #Continuum flux over all in-transit exposures    mean_cont=np.sum(cont_intr*wcont_intr,axis=0)/np.sum(wcont_intr,axis=0)          #Continuum correction    #    - intrinsic profiles can show deviations from the common continuum level they should have     #      here we set manually their continuum to the mean continuum of all intrinsic profiles before the correction    if cont_norm:            print('         Correcting intrinsic continuum')        for i_in in range(n_in_tr):            data_exp = dataload_npz(proc_Intr_data_paths+str(i_in))            for iord in range(nord):                cond_cont_com_ord = cond_cont_com[iord]                                #Continuum of current exposure                dcen_bins = data_exp['edge_bins'][iord,1:][cond_cont_com_ord] - data_exp['edge_bins'][iord,0:-1][cond_cont_com_ord]                cont_intr_exp = np.sum(data_exp['flux'][iord][cond_cont_com_ord]*dcen_bins)/np.sum(dcen_bins)                                #Correction factor                corr_exp = mean_cont[iord]/cont_intr_exp                    #Overwrite exposure data                data_exp['flux'][iord],data_exp['cov'][iord] = bind.mul_array(data_exp['flux'][iord],data_exp['cov'][iord],np.repeat(corr_exp,nspec))            datasave_npz(proc_Intr_data_paths+str(i_in),data_exp)           return mean_cont################################################################################################## #%% Planetary profiles routines################################################################################################## def extract_pl_profiles(data_dic,inst,vis,gen_dic):    r"""**Main atmospheric profile routine.**          Extracts planetary atmospheric profiles in the stellar rest frame.    Args:        TBD        Returns:        None        """      print('   > Extracting atmospheric stellar profiles')    data_vis = data_dic[inst][vis]    plAtm_vis = data_dic['Atm'][inst][vis]    #Current rest frame    if data_dic['Res'][inst][vis]['rest_frame']!='star':print('WARNING: residual profiles must be aligned')    data_dic['Atm'][inst][vis]['rest_frame'] = 'star'    #Indexes of in-transit exposures with defined estimates of local stellar profiles    idx_est_loc = dataload_npz(gen_dic['save_data_dir']+'Loc_estimates/'+data_dic['Intr']['opt_loc_data_corr']['corr_mode']+'/'+inst+'_'+vis)['idx_est_loc']    #Indexes of exposures with retrieved signal    if (data_dic['Atm']['pl_atm_sign']=='Absorption'):        #In-transit indexes        plAtm_vis['idx_def'] = idx_est_loc        #Corresponding global indexes        iexp_glob = np.array(gen_dic[inst][vis]['idx_in'])[idx_est_loc]    elif (data_dic['Atm']['pl_atm_sign']=='Emission'):        #Global indexes        plAtm_vis['idx_def'] = list(gen_dic[inst][vis]['idx_out']) + list(np.array(gen_dic[inst][vis]['idx_in'])[idx_est_loc])        iexp_glob = plAtm_vis['idx_def']             #Initializing path to atmospheric data    data_vis['proc_Atm_data_paths']=gen_dic['save_data_dir']+'Atm_data/'+data_dic['Atm']['pl_atm_sign']+'/'+inst+'_'+vis+'_'                    #Initialize path of weighing profiles for atmospheric exposures    #    - the weighing profiles include the master disk-integrated profile, and the best estimates of the local stellar profiles (if measured)    #    - best estimates are only defined for in-transit profiles, and paths must be defined relative to the indexes used to call atmpospheric profiles    #    - weighing master is defined on the common table for the visit    if (data_dic['Atm']['pl_atm_sign']=='Absorption') or ((data_dic['Atm']['pl_atm_sign']=='Emission') and data_dic['Intr']['cov_loc_star']):        data_vis['LocEst_Atm_data_paths'] = {}        if (data_dic['Atm']['pl_atm_sign']=='Absorption'):iexp_paths = idx_est_loc     #in-transit indexes        elif (data_dic['Atm']['pl_atm_sign']=='Emission'):iexp_paths = np.array(gen_dic[inst][vis]['idx_in'])[idx_est_loc]    #global indexes, limited to in-transit values        data_vis['LocEst_Atm_data_paths'] = {iexp:gen_dic['save_data_dir']+'Loc_estimates/'+data_dic['Intr']['opt_loc_data_corr']['corr_mode']+'/'+inst+'_'+vis+'_'+str(i_in) for iexp,i_in in zip(iexp_paths,idx_est_loc)}        #Calculating    if (gen_dic['calc_pl_atm']):        print('         Calculating data')             #Data for absorption signal        if (data_dic['Atm']['pl_atm_sign']=='Absorption'):            #Properties of planet-occulted regions            dic_plocc_prop = np.load(gen_dic['save_data_dir']+'Introrig_prop/PlOcc_Prop_'+inst+'_'+vis+'.npz',allow_pickle=True)['data'].item()                                  #Process all exposures        for iexp,i_in in zip(range(data_vis['n_in_visit']),gen_dic[inst][vis]['idx_exp2in']):            #Upload local profile            #    - the local stellar profiles defined in the star rest frame write as             # Fres(w,t,vis) = ( fp(w,vis)*(Sthick(band,t) + Sthin(w-wp,t) ) -  Fatm(w-wp,t) )*Cref(band)/Fr(vis)             #      we want to retrieve the atmospheric emission signal Fatm, and the atmospheric absorption surface Sthin            data_loc = np.load(data_vis['proc_Res_data_paths']+str(iexp)+'.npz',allow_pickle=True)['data'].item()                                         #Upload estimate of local stellar profile for in-transit exposures            #    - we distinguish between theoretical estimates and ones derived from data in the calculation of the covariance below             if (i_in>-1) and (i_in in idx_est_loc):data_loc_star = np.load(gen_dic['save_data_dir']+'Loc_estimates/'+data_dic['Intr']['opt_loc_data_corr']['corr_mode']+'/'+inst+'_'+vis+'_'+str(i_in)+'.npz',allow_pickle=True)['data'].item()                                       #Extraction of emission signal            #    - out-of-transit we take the opposite of the local profiles to retrieve the emission signal            # F_em(w,t,vis) = - Fres(w,t,vis)             #               = Fatm(w-wp,t)*Cref(band)/Fr(vis)              #    - in-transit, the estimates of local stellar profiles correspond to             # Fstar_loc(w,t) = fp(w,vis)*Sthick(band,t)*Cref(band)/Fr(vis)             #      and we define the emission signal as                # F_em(w,t,vis) = Fstar_loc(w,t) - Fres(w,t,vis)             #               = Fatm(w-wp,t)*Cref(band)/Fr(vis) - fp(w,vis)*Sthin(w-wp,t )*Cref(band)/Fr(vis)            #      thus the emission signal will remain contaminated if there is an absorption signal            #    - unless the exact stellar SED for each visit was used to correct for the color balance, and to set spectra to the correct overall flux level in each visit, the            # emission signals will be known to a scaling factor Cref(band)/Fr(vis)                                                                                     if (data_dic['Atm']['pl_atm_sign']=='Emission') and (iexp in plAtm_vis['idx_def']):                data_em = {'cen_bins':data_loc['cen_bins'],'edge_bins':data_loc['edge_bins'],'tell':data_loc['tell']}                                              #Out-of-transit signal                if (i_in == -1):                    data_em['flux'] = -data_loc['flux']                    for key in ['cov','cond_def']:data_em[key] = data_loc[key]                #In-transit signal                #    - in-transit exposures with no estimates of local stellar profiles cannot be retrieved                elif (i_in in idx_est_loc):                    if not data_dic['Intr']['cov_loc_star']:                        data_em['flux'] = data_loc_star['flux']-data_loc['flux']                        data_em['cov'] = data_loc['cov']                    else:                        data_em['flux'] = np.zeros(data_vis['dim_exp'], dtype=float)                        data_em['cov'] = np.zeros(data_dic[inst]['nord'], dtype=object)                        for iord in range(data_dic[inst]['nord']):                            data_em['flux'][iord],data_em['cov'][iord]=bind.add(data_loc_star['flux'][iord], data_loc_star['cov'][iord],-data_loc['flux'][iord], data_loc['cov'][iord])                                     data_em['cond_def'] = ~np.isnan(data_em['flux'])                                 #Saving data                               np.savez_compressed(data_vis['proc_Atm_data_paths']+str(iexp),data=data_em,allow_pickle=True)                              #------------------------------------------------------------------------------------------------------------            #Extraction of absorption signal            #    - the absorption signal in-transit is retrieved as            # Abs(w,t,vis) = ( F_res(w,t,vis) - Fstar_loc(w,t,vis) ) / ( Fstar_loc(w,t,vis)/( Sthick(band,t)/Sstar ) )                                #      subtracting Fstar_loc(w,t,vis) removes the local stellar profile absorbed by the planetary continuum            #      dividing by Fstar_loc(w,t,vis) then removes the contribution of the local stellar profile            #      rescaling by Sthick(band,t)/Sstar finally replaces the scaling of the planet-occulted region surface by the full stellar surface, so that the result is comparable with classical absorption signal            #              = ( [ ( fp(w,vis)*(Sthick(band,t) + Sthin(w-wp,t) ) -  Fatm(w-wp,t) )*Cref(band)/Fr(vis) ]  - [ fp(w,vis)*Sthick(band,t)*Cref(band)/Fr(vis) ]  ) / ( [ fp(w,vis)*Sthick(band,t)*Cref(band)/Fr(vis) ]/( Sthick(band,t)/Sstar ) )                #              = ( ( fp(w,vis)*(Sthick(band,t) + Sthin(w-wp,t) ) -  Fatm(w-wp,t) )  -  fp(w,vis)*Sthick(band,t)  ) / ( fp(w,vis)*Sstar )                                 #              = ( fp(w,vis)*Sthin(w-wp,t) -  Fatm(w-wp,t) )/ ( fp(w,vis)*Sstar )                                 #              = Sthin(w-wp,t)/Sstar -  Fatm(w-wp,t)/( fp(w,vis)*Sstar )               #    - the calculation sums up as:            # Abs(w,t,vis) = [ F_res(w,t,vis)/Fstar_loc(w,t,vis)  - 1 ]*( Sthick(band,t)/Sstar )            #    - the absorption signal can be contaminated by an emission signal, however the latter likely varies over the planet orbit (thus preventing us to compute an out-of-transit master to be corrected from             # in-transit exposures) and is unlikely to be visible during transit in any case as it would arise from nightside emission            #      if no emission is present, the corrected spectra correspond to:            # Signal(w,t) = Sthin(w-wp,t )/Sstar            #    - we use a numerical estimate of Sthick(band,t)/Sstar with a constant Sstar, so that we extract the pure atmospheric spectral surface, normalized            # by a constant stellar surface to be equivalent to an absorption signal, but unbiased by a spectral stellar surface            #    - if we consider that there is an absorption signal outside of the transit defined by the input light curve, ie that a region of the planetary atmosphere is absorbing            # in a specific line but not in the continuum:            # F_res(w,t,vis) = ( fp(w,vis)*Sthin(w-wp,t) -  Fatm(w-wp,t) )*Cref(band)/Fr(vis)             if (data_dic['Atm']['pl_atm_sign']=='Absorption') and (i_in>-1) and (i_in in idx_est_loc):                #Planet-to-star surface ratios                SpSstar_spec = np.zeros([data_dic[inst]['nord'],data_vis['nspec']],dtype=float)                                                             #Achromatic/chromatic planet-to-star radius ratio                #    - for now a single transiting planet is considered                if ('spec' in data_vis['type']) and ('chrom' in data_dic['DI']['system_prop']):SpSstar_chrom = True                else:                    if len(data_vis['transit_pl'])>1:stop()                    SpSstar_spec[:,:] = dic_plocc_prop['achrom'][data_vis['transit_pl'][0]]['SpSstar'][0,i_in]                     SpSstar_chrom = False                             #Processing each order                data_abs = {'cen_bins':data_loc['cen_bins'],'edge_bins':data_loc['edge_bins'],                            'flux' : np.zeros(data_vis['dim_exp'], dtype=float),                            'cov' : np.zeros(data_dic[inst]['nord'], dtype=object)}                for iord in range(data_dic[inst]['nord']):                                        #Chromatic planet-to-star radius ratio                    if SpSstar_chrom:                         SpSstar_spec[iord] = np_interp(data_loc['cen_bins'][iord],data_dic['DI']['system_prop']['chrom']['w'],dic_plocc_prop['chrom']['SpSstar'][:,i_in],left=dic_plocc_prop['chrom']['SpSstar'][0,i_in],right=dic_plocc_prop['chrom']['SpSstar'][-1,i_in])                    #Calculation of absorption signal                                                                if data_dic['Intr']['cov_loc_star']:dat_temp,cov_temp = bind.div(data_loc['flux'][iord],data_loc['cov'][iord],data_loc_star['flux'][iord], data_loc_star['cov'][iord])                    else:dat_temp,cov_temp = bind.mul_array(data_loc['flux'][iord],data_loc['cov'][iord],1./data_loc_star['flux'][iord])                    data_abs['flux'][iord],data_abs['cov'][iord] = bind.mul_array(dat_temp-1.,cov_temp,SpSstar_spec[iord])                data_abs['cond_def'] = ~np.isnan(data_abs['flux'])                                                          data_abs['SpSstar_spec'] = SpSstar_spec                                       #Saving data                               np.savez_compressed(data_vis['proc_Atm_data_paths']+str(i_in),data=data_abs,allow_pickle=True)                    #------------------------------------------------------------------------------------------------------------                    #Checking that local data has been calculated for all exposures    else:        data_paths={iexp:data_vis['proc_Atm_data_paths']+str(iexp) for iexp in plAtm_vis['idx_def']}                check_data(data_paths)    #Path to associated tables    #    - atmospheric profiles are extracted in the same frame as residual profiles    #    - indexes may be limited to in-transit indexes if absorption signals are extracted    if gen_dic['DImast_weight']:data_vis['mast_Atm_data_paths'] = {}    if data_vis['tell_sp']:data_vis['tell_Atm_data_paths'] = {}    if data_vis['mean_gdet']:data_vis['mean_gdet_Atm_data_paths'] = {}    for iexp_atm,iexp in zip(plAtm_vis['idx_def'],iexp_glob):        if gen_dic['DImast_weight']:data_vis['mast_Atm_data_paths'][iexp_atm] = data_dic[inst][vis]['mast_Res_data_paths'][iexp]         if data_vis['tell_sp']:data_vis['tell_Atm_data_paths'][iexp_atm] = data_vis['tell_Res_data_paths'][iexp]         if data_vis['mean_gdet']:data_vis['mean_gdet_Atm_data_paths'][iexp_atm] = data_vis['mean_gdet_Res_data_paths'][iexp]     return None
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_process/ANTARESS_main.py` & `antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,27 @@
 from os.path import exists as path_exist
 import glob
 from astropy.io import fits
 from dace_query.spectroscopy import Spectroscopy
 from scipy.interpolate import CubicSpline
 from ..ANTARESS_analysis.ANTARESS_model_prof import calc_macro_ker_anigauss,calc_macro_ker_rt 
 from ..ANTARESS_grids.ANTARESS_star_grid import model_star
-from ..ANTARESS_grids.ANTARESS_plocc_grid import occ_region_grid,sub_calc_plocc_spot_prop,calc_plocc_spot_prop
+from ..ANTARESS_grids.ANTARESS_occ_grid import occ_region_grid,sub_calc_plocc_spot_prop,calc_plocc_spot_prop
 from ..ANTARESS_grids.ANTARESS_prof_grid import init_custom_DI_prof,custom_DI_prof,theo_intr2loc,gen_theo_atm
 from ..ANTARESS_grids.ANTARESS_coord import calc_mean_anom_TR,calc_Kstar,calc_tr_contacts,calc_rv_star,coord_expos
 from ..ANTARESS_analysis.ANTARESS_inst_resp import return_pix_size,def_st_prof_tab,cond_conv_st_prof_tab,conv_st_prof_tab,get_FWHM_inst,resamp_st_prof_tab
 from ..ANTARESS_analysis.ANTARESS_ana_comm import par_formatting
 from ..ANTARESS_corrections.ANTARESS_sp_reduc import red_sp_data_instru
 from ..ANTARESS_analysis.ANTARESS_joined_star import joined_Star_ana
 from ..ANTARESS_analysis.ANTARESS_joined_atm import joined_Atm_ana
 from ..ANTARESS_plots.ANTARESS_plots_all import ANTARESS_plot_functions
 from ..ANTARESS_corrections.ANTARESS_calib import calc_gcal
-from ..ANTARESS_process.ANTARESS_plocc_spec import def_plocc_profiles
+from ..ANTARESS_process.ANTARESS_plocc_spec import def_in_plocc_profiles,def_diff_profiles
 from ..ANTARESS_conversions.ANTARESS_masks_gen import def_masks
 from ..ANTARESS_conversions.ANTARESS_conv import CCF_from_spec,ResIntr_CCF_from_spec,conv_2D_to_1D_spec
-from ..ANTARESS_grids.ANTARESS_spots import corr_spot,spot_occ_region_grid
 from ..ANTARESS_conversions.ANTARESS_binning import process_bin_prof
 from ..ANTARESS_corrections.ANTARESS_detrend import detrend_prof,pc_analysis
 from ..ANTARESS_process.ANTARESS_data_process import align_profiles,rescale_profiles,extract_res_profiles,extract_intr_profiles,extract_pl_profiles 
 from ..ANTARESS_analysis.ANTARESS_ana_comm import MAIN_single_anaprof
 from ..ANTARESS_conversions.ANTARESS_sp_cont import process_spectral_cont
 from ..ANTARESS_general.utils import air_index,dataload_npz,gen_specdopshift,stop,np_where1D,closest,datasave_npz,def_edge_tab,check_data
 from ..ANTARESS_general.constant_data import Rsun,Rjup,c_light,G_usi,Msun,AU_1
@@ -136,16 +135,16 @@
                 CCF_from_spec(data_type_gen,inst,vis,data_dic,gen_dic,data_dic[data_type_gen])
         
             #Single line detrending    
             if gen_dic['detrend_prof'] and (not detrend_prof_dic['full_spec']):
                 detrend_prof(detrend_prof_dic,data_dic,coord_dic,inst,vis,data_dic,data_prop,gen_dic,plot_dic)
 
             #Calculating theoretical properties of the planet-occulted and/or spotted regions 
-            if gen_dic['theoPlOcc'] or gen_dic['theo_spots']:
-                calc_plocc_spot_prop(system_param,gen_dic,theo_dic,coord_dic,inst,vis,data_dic,calc_pl_atm=gen_dic['calc_pl_atm'],spot_dic=mock_dic)
+            if gen_dic['theoPlOcc'] or (data_dic['DI']['spots_prop'] != {}):
+                calc_plocc_spot_prop(system_param,gen_dic,theo_dic,coord_dic,inst,vis,data_dic,calc_pl_atm=gen_dic['calc_pl_atm'],spot_dic=data_dic['DI']['spots_prop'])
                 
             #Analyzing original disk-integrated profiles
             if gen_dic['fit_'+data_type_gen]:
                 MAIN_single_anaprof('',data_type_gen+'orig',data_dic,gen_dic,inst,vis,coord_dic,theo_dic,plot_dic,system_param['star'])
 
             #Aligning disk-integrated profiles to star rest frame
             if (gen_dic['align_'+data_type_gen]):
@@ -157,15 +156,15 @@
               
             #Rescaling profiles to their correct flux level                  
             if gen_dic['flux_sc']:                   
                 rescale_profiles(data_dic[inst],inst,vis,data_dic,coord_dic,coord_dic[inst][vis]['t_dur_d'],gen_dic,plot_dic,system_param,theo_dic)   
          
             #Calculating master spectrum of the disk-integrated star used in weighted averages and continuum-normalization
             if gen_dic['DImast_weight']:              
-                process_bin_prof('',data_type_gen,gen_dic,inst,vis,data_dic,coord_dic,data_prop,system_param,theo_dic,plot_dic,masterDI=True,mock_dic=mock_dic)
+                process_bin_prof('',data_type_gen,gen_dic,inst,vis,data_dic,coord_dic,data_prop,system_param,theo_dic,plot_dic,masterDI=True,spot_dic=data_dic['DI']['spots_prop'])
 
             #Processing converted 2D disk-integrated profiles
             if gen_dic['spec_1D']:                
                 conv_2D_to_1D_gen_functions(data_type_gen,data_dic,inst,vis,gen_dic,coord_dic,theo_dic,plot_dic,system_param)
  
             #Processing binned disk-integrated profiles
             if gen_dic['bin']:
@@ -204,17 +203,22 @@
             if gen_dic['spec_1D']:                
                 conv_2D_to_1D_gen_functions(data_type_gen,data_dic,inst,vis,gen_dic,coord_dic,theo_dic,plot_dic,system_param)
 
             #Processing binned intrinsic profiles
             if gen_dic['bin']:
                 bin_gen_functions(data_type_gen,'',inst,gen_dic,data_dic,coord_dic,data_prop,system_param,theo_dic,plot_dic,vis=vis)
 
-            #Building estimates for complete local stellar profiles
+            #Building estimates for planet-occulted stellar profiles in in-transit exposures
             if gen_dic['loc_data_corr']:
-                def_plocc_profiles(inst,vis,gen_dic,data_dic,data_prop,coord_dic,system_param,theo_dic,glob_fit_dic,plot_dic)
+                def_in_plocc_profiles(inst,vis,gen_dic,data_dic,data_prop,coord_dic,system_param,theo_dic,glob_fit_dic,plot_dic)
+
+            #Building estimates for differential profiles in all exposures
+            #    - in-transit profiles include planet-occulted and spotted stellar profiles
+            if gen_dic['diff_data_corr']:
+                def_diff_profiles(inst,vis,gen_dic,data_dic,data_prop,coord_dic,system_param,theo_dic,glob_fit_dic,plot_dic)
         
             #--------------------------------------------------------------------------------------------------
             #Processing atmospheric profiles
             data_type_gen = 'Atm'
             #--------------------------------------------------------------------------------------------------
 
             #Extracting atmospheric profiles
@@ -714,16 +718,20 @@
         star_params['RpoleReq'] = 1.
         
     #Oblate star
     elif star_params['f_GD']>0.:
         print('Star is oblate')
         star_params['RpoleReq']=1.-star_params['f_GD']
 
+    #Stellar equatorial rotation period (d)
+    #    - P = 2*pi*R/v
+    star_params['Peq'] = (2.*np.pi*star_params['Rstar_km'])/(star_params['veq']*24*3600)
+
     #Stellar equatorial rotation rate (rad/s)
-    #    - om = 2*pi/P
+    #    - om = 2*pi/P = v/R
     star_params['om_eq'] = star_params['veq']/star_params['Rstar_km']
 
     #Spot Equatorial rotation rate (rad/s)
     if 'veq_spots' in star_params:star_params['om_eq_spots']=star_params['veq_spots']/star_params['Rstar_km']
     else:star_params['om_eq_spots']=star_params['om_eq']
 
     #No GD
@@ -907,25 +915,32 @@
             data_dic['DI']['system_prop']['chrom']['cond_in_RpRs'][pl_loc]={}
             for iband in range(data_dic['DI']['system_prop']['chrom']['nw']):
                 data_dic['DI']['system_prop']['chrom']['cond_in_RpRs'][pl_loc][iband] = (r_sub_pl2<data_dic['DI']['system_prop']['chrom'][pl_loc][iband]**2.)
 
     #------------------------------------------------------------------------------
     #Spots
     #------------------------------------------------------------------------------
-    if 1==0:   #Samson: need for a generic condition to initialize or not spots
-    
+
+    #Initialize spot use
+    gen_dic['studied_sp'] = list(gen_dic['transit_sp'].keys()) 
+    theo_dic['x_st_sky_grid_sp']={}
+    theo_dic['y_st_sky_grid_sp']={}
+    theo_dic['Ssub_Sstar_sp'] = {}
+    theo_dic['d_oversamp_spot']={}
+
+    #If spot activation has been triggered
+    if (data_dic['DI']['spots_prop'] != {}):
+
         #Oversampling factor for spot-occulted regions
         #    - use the spot radius provided as input
-        theo_dic['d_oversamp_spot']={}
         for spot in theo_dic['n_oversamp_spot']:
             if (theo_dic['n_oversamp_spot'][spot]>0.):
                 theo_dic['d_oversamp_spot'][spot] = np.sin(data_dic['DI']['spots_prop']['achrom'][spot][0])/theo_dic['n_oversamp_spot'][spot]
     
         #Spot surface chromatic properties
-        #Need to define the LD coefficients if they are not defined
         for ideg in range(2,5):
             if 'LD_u'+str(ideg) not in data_dic['DI']['spots_prop']['achrom']:data_dic['DI']['spots_prop']['achrom']['LD_u'+str(ideg)] = [0.]
     
         #Need to define chromatic band properties
         data_dic['DI']['spots_prop']['achrom']['w']=[None]
         data_dic['DI']['spots_prop']['achrom']['nw']=1
         data_dic['DI']['spots_prop']['chrom_mode'] = 'achrom'
@@ -938,24 +953,21 @@
                 
                 #Typical scale of chromatic variations
                 w_edge = def_edge_tab(data_dic['DI']['spots_prop']['chrom']['w'][None,:][None,:])[0,0]    
                 data_dic['DI']['spots_prop']['chrom']['dw'] = w_edge[1::]-w_edge[0:-1]
                 data_dic['DI']['spots_prop']['chrom']['med_dw'] = np.median(data_dic['DI']['spots_prop']['chrom']['dw'])
     
         #Definition of grids discretizing planets disk to calculate planet-occulted properties
-        theo_dic['x_st_sky_grid_sp']={}
-        theo_dic['y_st_sky_grid_sp']={}
-        theo_dic['Ssub_Sstar_sp'] = {}
         for spot in theo_dic['nsub_Dspot']:
             
             #Retrieve spot size
             spot_size = data_dic['DI']['spots_prop']['achrom'][spot][0]
     
             #Define a default grid size if the spot grid hasn't been defined (should be done outside of for loop)
-            theo_dic['x_st_sky_grid_sp'][spot], theo_dic['y_st_sky_grid_sp'][spot], theo_dic['Ssub_Sstar_sp'][spot] = spot_occ_region_grid(spot_size, theo_dic['nsub_Dspot'][spot])
+            _,theo_dic['Ssub_Sstar_sp'][spot],theo_dic['x_st_sky_grid_sp'][spot], theo_dic['y_st_sky_grid_sp'][spot],_ = occ_region_grid(spot_size, theo_dic['nsub_Dspot'][spot],spot=True)
 
     #------------------------------------------------------------------------------------------------------------------------
     #Model star
     #------------------------------------------------------------------------------------------------------------------------
     grid_type=[]
     if any('spec' in s for s in data_dic['DI']['type'].values()):grid_type+=['spec']
     if ('CCF' in data_dic['DI']['type'].values()):grid_type+=['ccf']    
@@ -964,15 +976,15 @@
     if gen_dic['calc_flux_sc'] and (data_dic['DI']['transit_prop']['nsub_Dstar'] is not None): 
         model_star('Ftot',theo_dic,grid_type,data_dic['DI']['system_prop'],data_dic['DI']['transit_prop']['nsub_Dstar'],star_params) 
                     
     #Definition of model stellar grid to calculate local or disk-integrated properties
     #    - used througout the pipeline, unless stellar properties are fitted
     if gen_dic['theoPlOcc'] or (gen_dic['theo_spots']) or (gen_dic['fit_DI_gen'] and (('custom' in data_dic['DI']['model'].values()) or ('RT_ani_macro' in data_dic['DI']['model'].values()))) or gen_dic['mock_data'] \
         or gen_dic['fit_ResProf'] or gen_dic['correct_spots'] or gen_dic['fit_IntrProf'] or gen_dic['loc_data_corr']:
-            
+
         #Stellar grid
         model_star('grid',theo_dic,grid_type,data_dic['DI']['system_prop'],theo_dic['nsub_Dstar'],star_params) 
        
         #Theoretical atmosphere
         cond_st_atm = False
         if gen_dic['mock_data']:
             for inst in mock_dic['intr_prof']:
@@ -1077,14 +1089,17 @@
     if gen_dic['DImast_weight'] and (not path_exist(gen_dic['save_data_dir']+'DI_data/Master/')):makedirs(gen_dic['save_data_dir']+'DI_data/Master/')
     if (gen_dic['res_data']) and (not path_exist(gen_dic['save_data_dir']+'Res_data/')):makedirs(gen_dic['save_data_dir']+'Res_data/')
     if gen_dic['pca_ana'] and (not path_exist(gen_dic['save_data_dir']+'PCA_results/')):makedirs(gen_dic['save_data_dir']+'PCA_results/')   
     if (gen_dic['intr_data']) and (not path_exist(gen_dic['save_data_dir']+'Intr_data/')):makedirs(gen_dic['save_data_dir']+'Intr_data/')
     if gen_dic['loc_data_corr']:
         if (not path_exist(gen_dic['save_data_dir']+'Loc_estimates/')):makedirs(gen_dic['save_data_dir']+'Loc_estimates/')        
         if (not path_exist(gen_dic['save_data_dir']+'Loc_estimates/'+data_dic['Intr']['opt_loc_data_corr']['corr_mode']+'/')):makedirs(gen_dic['save_data_dir']+'Loc_estimates/'+data_dic['Intr']['opt_loc_data_corr']['corr_mode']+'/')  
+    if gen_dic['diff_data_corr']:
+        if (not path_exist(gen_dic['save_data_dir']+'Diff_estimates/')):makedirs(gen_dic['save_data_dir']+'Diff_estimates/')        
+        if (not path_exist(gen_dic['save_data_dir']+'Diff_estimates/'+data_dic['Res']['opt_loc_data_corr']['corr_mode']+'/')):makedirs(gen_dic['save_data_dir']+'Diff_estimates/'+data_dic['Res']['opt_loc_data_corr']['corr_mode']+'/')          
     if (gen_dic['pl_atm']):
         if (not path_exist(gen_dic['save_data_dir']+'Atm_data/')):makedirs(gen_dic['save_data_dir']+'Atm_data/')        
         if (not path_exist(gen_dic['save_data_dir']+'Atm_data/'+data_dic['Atm']['pl_atm_sign']+'/')):makedirs(gen_dic['save_data_dir']+'Atm_data/'+data_dic['Atm']['pl_atm_sign']+'/')
     
     for data_type in ['DI','Intr','Atm']:
         if gen_dic['align_'+data_type] and (not path_exist(gen_dic['save_data_dir']+'Aligned_'+data_type+'_data/'+gen_dic['add_txt_path'][data_type])):makedirs(gen_dic['save_data_dir']+'Aligned_'+data_type+'_data/'+gen_dic['add_txt_path'][data_type])    
         if gen_dic['spec_1D_'+data_type]:
@@ -1336,15 +1351,15 @@
                     if len(vis_path_skysub_exp)==0:stop('No sky-sub data found. Check path.') 
                     
                     #Orders to be replaced
                     if gen_dic['fibB_corr'][inst][vis]=='all':idx_ord_skysub = 'all'
                     else:idx_ord_skysub = gen_dic['fibB_corr'][inst][vis]
                     
                 else:vis_path_skysub_exp = None
-                
+              
                 #Path of visits exposures
                 if inst not in ['EXPRES']:vis_path+='A'
                 vis_path_exp = np.array(glob.glob(vis_path+'.fits'))
                 n_in_visit=len(vis_path_exp) 
                 if n_in_visit==0:stop('No data found. Check path.')
 
             #Remove/keep visits
@@ -1403,14 +1418,16 @@
                 #Initializing dictionaries for visit
                 theo_dic[inst][vis]={}
                 data_dic['Atm'][inst][vis]={}   
                 data_inst[vis] = {'n_in_visit':n_in_visit,'transit_pl':[],'transit_sp':[],'comm_sp_tab':True} 
                 coord_dic[inst][vis] = {}
                 for pl_loc in gen_dic['studied_pl']:
                     if (inst in gen_dic['transit_pl'][pl_loc]) and (vis in gen_dic['transit_pl'][pl_loc][inst]):data_inst[vis]['transit_pl']+=[pl_loc]
+                for spot in gen_dic['studied_sp']:
+                    if (inst in gen_dic['transit_sp'][spot]) and (vis in gen_dic['transit_sp'][spot][inst]):data_inst[vis]['transit_sp']+=[spot]                    
                 data_prop[inst][vis] = {}
                 data_dic_temp={}
                 gen_dic[inst][vis] = {}
                 DI_data_inst[vis] = {}  
                          
                 #Associating telluric spectrum with each exposure
                 if not gen_dic['mock_data']:data_inst[vis]['tell_DI_data_paths']={}
@@ -1622,19 +1639,21 @@
                             if inst not in mock_dic['sysvel']:mock_dic['sysvel'][inst]={}
                             if vis not in mock_dic['sysvel'][inst]:mock_dic['sysvel'][inst][vis] = 0.
                             fixed_args.update({ 
                                 'mac_mode':theo_dic['mac_mode'],
                                 'type':data_inst[vis]['type'],  
                                 'nord':data_inst['nord'],
                                 'nthreads':mock_dic['nthreads'], 
+                                'unthreaded_op':mock_dic['unthreaded_op'], 
                                 'resamp_mode' : gen_dic['resamp_mode'], 
                                 'conv2intr':False,
                                 'inst':inst,
                                 'vis':vis, 
                                 'fit':False,
+                                'unquiet_star':None,
                                 })
 
                             #Spots properties
                             if (inst in mock_dic['spots_prop']) and (vis in mock_dic['spots_prop'][inst]):
                                 params_mock['use_spots']=True
                                 par_formatting(params_mock,mock_dic['spots_prop'][inst][vis],None,None,fixed_args,inst,vis) 
                                 
@@ -1642,15 +1661,15 @@
                                 num_spots = 0
                                 for par in params_mock:
                                     if 'lat__IS'+inst+'_VS'+vis+'_SP' in par:num_spots+=1
                                 params_mock['num_spots']=num_spots
                                 params_mock['inst']=inst
                                 params_mock['vis']=vis
                             else:params_mock['use_spots']=False 
-
+                                
                         #Observational data            
                         else:   
                             data_inst[vis]['mock'] = False                      
     
                             #VLT UT used by ESPRESSO
                             if inst=='ESPRESSO':
                                 tel_inst = {
@@ -1771,15 +1790,15 @@
                                     if (par_drift=='rv'):param_exp[par_drift] += mock_dic['drift_intr'][inst][vis][par_drift][iexp]
                                     else:param_exp[par_drift] *= mock_dic['drift_intr'][inst][vis][par_drift][iexp]
 
                         #Disk-integrated stellar line     
                         base_DI_prof = custom_DI_prof(param_exp,None,args=args_exp)[0]
 
                         #Deviation from nominal stellar profile 
-                        surf_prop_dic, surf_prop_dic_sp = sub_calc_plocc_spot_prop([data_dic['DI']['system_prop']['chrom_mode']],args_exp,['line_prof'],data_dic[inst][vis]['transit_pl'],deepcopy(system_param),theo_dic,args_exp['system_prop'],param_exp,coord_dic[inst][vis],[iexp], system_spot_prop_in=args_exp['system_spot_prop'])
+                        surf_prop_dic, surf_prop_dic_sp,_ = sub_calc_plocc_spot_prop([data_dic['DI']['system_prop']['chrom_mode']],args_exp,['line_prof'],data_dic[inst][vis]['transit_pl'],deepcopy(system_param),theo_dic,args_exp['system_prop'],param_exp,coord_dic[inst][vis],[iexp], system_spot_prop_in=args_exp['system_spot_prop'])
 
                         #Correcting the disk-integrated profile for planet and spot contributions
                         if param_exp['use_spots']:
                             DI_prof_exp = base_DI_prof - surf_prop_dic[data_dic['DI']['system_prop']['chrom_mode']]['line_prof'][:,0] - surf_prop_dic_sp[data_dic['DI']['system_prop']['chrom_mode']]['line_prof'][:,0]
                         
                         #Correcting the disk-integrated profile for planet contribution alone
                         else:
@@ -1799,15 +1818,15 @@
                         DI_prof_exp[DI_prof_exp<0.] = 0.
 
                         #Define number of photoelectrons extracted during the exposure
                         #   - the model is a density of photoelectrons per unit of time, with continuum set to the input mean flux density
                         if (inst in mock_dic['gcal']):mock_gcal = mock_dic['gcal'][inst]
                         else:mock_gcal = 1.
                         DI_prof_exp_Ftrue = mock_gcal*DI_prof_exp*coord_dic[inst][vis]['t_dur'][iexp] 
-
+                        
                         #Keplerian motion and systemic shift of the disk-integrated profile 
                         #    - we shift profiles from the star rest frame (source) to the solar barycentric rest frame (receiver)
                         #      see gen_specdopshift() :
                         # w_receiver = w_source * (1+ rv[s/r]/c))
                         # w_solbar = w_star * (1+ rv[star/starbar]/c))* (1+ rv[starbar/solbar]/c))
                         #      we include variations in the systemic rv if requested
                         RV_star_stelCDM_mock = calc_rv_star(coord_dic,inst,vis,system_param,gen_dic, coord_dic[inst][vis]['bjd'][iexp],coord_dic[inst][vis]['t_dur'][iexp],mock_dic['sysvel'][inst][vis])[0]
@@ -2528,21 +2547,23 @@
         for vis in gen_dic['unused_visits'][inst]:
             if vis in data_dic[inst]['visit_list']:data_dic[inst]['visit_list'].remove(vis)
 
         #Retrieve/initialize visit dictionaries
         for vis in data_dic[inst]['visit_list']:     
             data_load = np.load(gen_dic['save_data_dir']+'Processed_data/Global/'+inst+'_'+vis+'.npz',allow_pickle=True)
             data_dic[inst][vis]=data_load['data_add'].item()
+            data_dic[inst][vis]['proc_DI_data_paths']  = gen_dic['save_data_dir']+'Processed_data/'+inst+'_'+vis+'_'
+            data_dic[inst][vis]['proc_com_data_paths'] = gen_dic['save_data_dir']+'Processed_data/'+inst+'_'+vis+'_com'
             coord_dic[inst][vis]=data_load['coord_add'].item()
             data_prop[inst][vis]=data_load['data_prop_add'].item() 
             gen_dic[inst][vis]=data_load['gen_add'].item()
             data_dic['DI'][inst][vis]=data_load['DI_data_add'].item()
             theo_dic[inst][vis]={}
             data_dic['Atm'][inst][vis]={} 
-
+            
     #Default transit model
     if (inst not in data_dic['DI']['transit_prop']):data_dic['DI']['transit_prop'][inst] = {}
 
     #Duplicate chromatic properties so that they are not overwritten by conversions
     data_dic[inst]['system_prop'] = deepcopy(data_dic['DI']['system_prop'])
 
     #Final processing
```

### Comparing `antaress-1.1.0/src/antaress/ANTARESS_process/ANTARESS_plocc_spec.py` & `antaress-1.1.1/src/antaress/ANTARESS_process/ANTARESS_plocc_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import numpy as np
 from scipy.interpolate import griddata
 from copy import deepcopy
 import bindensity as bind
+import glob
 from ..ANTARESS_conversions.ANTARESS_binning import calc_bin_prof,weights_bin_prof,init_bin_prof
 from ..ANTARESS_grids.ANTARESS_prof_grid import init_custom_DI_prof,theo_intr2loc
-from ..ANTARESS_grids.ANTARESS_plocc_grid import init_surf_shift,def_surf_shift,sub_calc_plocc_spot_prop
+from ..ANTARESS_grids.ANTARESS_occ_grid import init_surf_shift,def_surf_shift,sub_calc_plocc_spot_prop,up_plocc_prop
 from ..ANTARESS_grids.ANTARESS_coord import excl_plrange
 from ..ANTARESS_process.ANTARESS_data_align import align_data
 from ..ANTARESS_analysis.ANTARESS_inst_resp import def_st_prof_tab,cond_conv_st_prof_tab,get_FWHM_inst,resamp_st_prof_tab,conv_st_prof_tab
 from ..ANTARESS_general.utils import stop,dataload_npz,datasave_npz,closest_arr,np_where1D,gen_specdopshift,check_data
 
+#%% Planet-occulted exposure profiles.
 
-def def_plocc_profiles(inst,vis,gen_dic,data_dic,data_prop,coord_dic,system_param,theo_dic,glob_fit_dic,plot_dic):
+def def_in_plocc_profiles(inst,vis,gen_dic,data_dic,data_prop,coord_dic,system_param,theo_dic,glob_fit_dic,plot_dic):
     r"""**Planet-occulted exposure profiles.**
     
     Calls requested function to define planet-occulted profiles associated with each observed exposure
     
      - local profiles are used to correct residual profiles from stellar contamination
      - intrinsic profiles are used to assess fit quality
 
@@ -42,27 +44,27 @@
 
     #Calculating
     if (gen_dic['calc_loc_data_corr']):
         print('         Calculating data')     
  
         #Using disk-integrated master or binned intrinsic profiles
         if corr_mode in ['DIbin','Intrbin']:
-            data_add = loc_prof_meas(opt_dic,corr_mode,inst,vis,data_dic['Intr'],gen_dic,data_dic,data_prop,data_dic['Atm'],coord_dic)
+            data_add = plocc_prof_meas(opt_dic,corr_mode,inst,vis,data_dic['Intr'],gen_dic,data_dic,data_prop,data_dic['Atm'],coord_dic)
             
         #Using global profile model
         elif corr_mode=='glob_mod': 
-            data_add = loc_prof_globmod(opt_dic,corr_mode,inst,vis,gen_dic,data_dic,data_prop,system_param,theo_dic,coord_dic,glob_fit_dic)
+            data_add = plocc_spocc_prof_globmod(opt_dic,corr_mode,inst,vis,gen_dic,data_dic,data_prop,system_param,theo_dic,coord_dic,glob_fit_dic,False)
             
         #Using individual profile models
         elif corr_mode=='indiv_mod': 
-            data_add = loc_prof_indivmod(opt_dic,corr_mode,inst,vis,gen_dic,data_dic)
+            data_add = plocc_prof_indivmod(opt_dic,corr_mode,inst,vis,gen_dic,data_dic)
 
         #Defining undefined pixels via a polynomial fit to defined pixels in complementary exposures, or via a 2D interpolation over complementary exposures and a narrow spectral band
         elif corr_mode=='rec_prof': 
-            data_add = loc_prof_rec(opt_dic,corr_mode,inst,vis,gen_dic,data_dic,coord_dic)
+            data_add = plocc_prof_rec(opt_dic,corr_mode,inst,vis,gen_dic,data_dic,coord_dic)
             
         #Saving complementary data for plots
         if plot_dic['map_Intr_prof_res']!='':
             data_add['loc_data_corr_inpath'] = data_dic[inst][vis]['proc_Intr_data_paths']
             data_add['loc_data_corr_outpath'] = data_dic[inst][vis]['proc_Res_data_paths']
             data_add['rest_frame'] = data_dic['Intr'][inst][vis]['rest_frame']
         datasave_npz(gen_dic['save_data_dir']+'Loc_estimates/'+corr_mode+'/'+inst+'_'+vis+'_add',data_add)
@@ -73,15 +75,15 @@
         data_paths={i_in:gen_dic['save_data_dir']+'Loc_estimates/'+corr_mode+'/'+inst+'_'+vis+'_'+str(i_in) for i_in in idx_est_loc}
         check_data(data_paths)
 
     return None
 
 
 
-def loc_prof_meas(opt_dic,corr_mode,inst,vis,gen_dic,data_dic,data_prop,coord_dic):
+def plocc_prof_meas(opt_dic,corr_mode,inst,vis,gen_dic,data_dic,data_prop,coord_dic):
     r"""**Planet-occulted exposure profiles: measured**
     
     Sub-function to define planet-occulted profiles using measured profiles as best estimates of intrinsic profiles
     
     When binned intrinsic profiles are used
     
      - we first define the range and center of the binned profiles, along the bin dimension
@@ -233,131 +235,230 @@
 
     return data_add
 
 
 
 
 
-def loc_prof_globmod(opt_dic,corr_mode,inst,vis,gen_dic,data_dic,data_prop,system_param,theo_dic,coord_dic,glob_fit_dic):
-    r"""**Planet-occulted exposure profiles: global model**
+def plocc_spocc_prof_globmod(opt_dic,corr_mode,inst,vis,gen_dic,data_dic,data_prop,system_param,theo_dic,coord_dic,glob_fit_dic,spot_on):
+    r"""**Planet-occulted / spotted exposure profiles: global model**
     
-    Sub-function to define planet-occulted profiles using line profile model fitted to all intrinsic lines together in `fit_IntrProf_all()`.
-    This model can be based on analytical, measured, or theoretical profiles.
+    Sub-function to define planet-occulted and spotted profiles using line profile models fitted to all
+        - intrinsic profiles together in `fit_IntrProf_all()`.
+          This model can be based on analytical, measured, or theoretical profiles.        
+        - to all differential profiles together with `fit_ResProf_all()`.
+          This model is based on analytical profiles.  
     
     Flux scaling is not applied to a global intrinsic profile using the chromatic light curve, but re-calculated for each planet-occulted intrinsic line profile for more flexibility (the cumulated scaling should be equivalent).
     rv used to shift the profiles are similarly re-calculated theoretically. 
 
     Args:
         TBD
     
     Returns:
         TBD
     
     """ 
     data_vis = data_dic[inst][vis]
-    
     def_iord = opt_dic['def_iord']
     if (data_dic['Intr']['align_mode']=='meas'):stop('This mode cannot be used with measured RVs')
 
     #Retrieving selected model properties
-    if ('IntrProf_prop_path' not in opt_dic):
-        print('         Trying to retrieve chi2 fit by default')
-        opt_dic['IntrProf_prop_path']={inst:{vis:gen_dic['save_data_dir']+'/Joined_fits/IntrProf/chi2/Fit_results'}}
-    data_prop = dataload_npz(opt_dic['IntrProf_prop_path'][inst][vis])
+    fit_txt = None
+    if (not spot_on) and ('IntrProf_prop_path' not in opt_dic):fit_txt = 'Intr'
+    if (spot_on) and ('ResProf_prop_path' not in opt_dic):fit_txt = 'Res'
+    if fit_txt is not None:
+        fit_subdirs = glob.glob(gen_dic['save_data_dir']+'/Joined_fits/'+fit_txt+'Prof/*/')
+        if len(fit_subdirs)==0:stop('         No existing fit directory. Run a fit to the '+{'Intr':'intrinsic','Res':'differential'}[fit_txt]+' line profiles.')
+        else:
+            fit_types = [fit_subdir.split('/')[-2] for fit_subdir in fit_subdirs]
+            if 'mcmc' in fit_types:fit_used  ='mcmc'
+            else:fit_used  ='chi2'
+            print('         Using existing '+fit_used+' fit as default')
+            opt_dic[fit_txt+'Prof_prop_path']={inst:{vis:gen_dic['save_data_dir']+'/Joined_fits/'+fit_txt+'Prof/'+fit_used+'/Fit_results'}}  
+    if spot_on:prof_type = 'Res'
+    else:prof_type='Intr'        
+    data_prop = dataload_npz(opt_dic[prof_type+'Prof_prop_path'][inst][vis])
     params=data_prop['p_final'] 
     fixed_args={  
         'mode':opt_dic['mode'],
-        'type':data_dic[inst][vis]['type'],
+        'type':data_vis['type'],
         'nord':data_dic[inst]['nord'],
         'nthreads': opt_dic['nthreads'],
         'resamp_mode' : gen_dic['resamp_mode'], 
         'inst':inst,
         'vis':vis,  
         'fit':False,
+        'ph_fit':data_prop['ph_fit'],
+        'system_param':system_param,
+        'genpar_instvis':data_prop['genpar_instvis'],
+        'name_prop2input':data_prop['name_prop2input'],
+        'fit_orbit':data_prop['fit_orbit'],
+        'fit_RpRs':data_prop['fit_RpRs'],
+        'var_par_list':data_prop['var_par_list'],
+        'system_prop':data_prop['system_prop'],
+        'grid_dic':data_prop['grid_dic'],
     } 
     if fixed_args['mode']=='ana':
         fixed_args.update({  
             'mac_mode':theo_dic['mac_mode'], 
             'coeff_line':data_prop['coeff_line_dic'][inst][vis],
             'func_prof_name':data_prop['func_prof_name'][inst]
         })        
         for key in ['coeff_ord2name','pol_mode','coord_line','linevar_par']:fixed_args[key] = data_prop[key]
-    if data_dic['Intr']['plocc_prof_type']=='Intr':fixed_args['conv2intr'] = True
-    else:fixed_args['conv2intr'] = False
-    chrom_mode = data_dic[inst][vis]['system_prop']['chrom_mode']
-
+    if spot_on:  
+        fixed_args.update({          
+        'fit_spot_ang':data_prop['fit_spot_ang'],
+        'fit_spot':data_prop['fit_spot'],
+        'system_spot_prop':data_prop['system_spot_prop'],
+        'update_crosstime':False,    
+        'conv2intr' :False,           
+            })
+        transit_spots=data_vis['transit_sp']
+        iexp_list = range(data_vis['n_in_visit'])
+        spots_prop = data_vis['spots_prop']
+        plocc_prof_type = 'Res'
+        
+        #Defining parameters for the clean version of profiles
+        if opt_dic['clean_calc']:
+            clean_params = deepcopy(params)
+            clean_params['use_spots']=False        
+        
+    else:
+        fixed_args.update({          
+        'system_spot_prop':{},          
+            })
+        plocc_prof_type = data_dic['Intr']['plocc_prof_type']
+        if data_dic['Intr']['plocc_prof_type']=='Intr':fixed_args['conv2intr'] = True
+        else:fixed_args['conv2intr'] = False 
+        transit_spots={}
+        spots_prop ={}
+        iexp_list = range(data_vis['n_in_tr'])
+    chrom_mode = data_vis['system_prop']['chrom_mode']
+  
     #Activation of spectral conversion and resampling 
-    cond_conv_st_prof_tab(theo_dic['rv_osamp_line_mod'],fixed_args,data_dic[inst][vis]['type']) 
+    cond_conv_st_prof_tab(theo_dic['rv_osamp_line_mod'],fixed_args,data_vis['type']) 
 
-    #Processing in-transit exposures
-    for isub,i_in in enumerate(range(data_dic[inst][vis]['n_in_tr'])):
-      
-        #Upload spectral tables from residual or intrinsic profile of current exposure
-        if data_dic['Intr']['plocc_prof_type']=='Intr':iexp_eff = i_in
-        else:iexp_eff = gen_dic[inst][vis]['idx_in2exp'][i_in]
-        data_loc_exp = dataload_npz(data_vis['proc_'+data_dic['Intr']['plocc_prof_type']+'_data_paths']+str(iexp_eff))
+    #Updating coordinates with the best-fit properties
+    ph_rec = {}
+    coord_vis = coord_dic[inst][vis]
+    for pl_loc in data_vis['transit_pl']:
+        ph_rec[pl_loc] = np.vstack((coord_vis[pl_loc]['st_ph'],coord_vis[pl_loc]['cen_ph'],coord_vis[pl_loc]['end_ph']) ) 
+    _,coord_pl_sp,_ = up_plocc_prop(inst,vis,fixed_args,params,data_vis['transit_pl'],ph_rec,coord_vis,transit_spots=transit_spots)
+
+    #Processing relevant exposures
+    for isub,iexp in enumerate(iexp_list):
+        if not spot_on:
+            iexp_glob = gen_dic[inst][vis]['idx_in2exp'][iexp]
+            if plocc_prof_type=='Intr':iexp_eff = iexp
+            else:iexp_eff = iexp_glob
+        else:
+            iexp_glob =iexp
+            iexp_eff = iexp
 
+        #Upload spectral tables from residual profile of current exposure
+        data_loc_exp = dataload_npz(data_vis['proc_'+plocc_prof_type+'_data_paths']+str(iexp_eff))
+    
         #Limit model table to requested definition range
-        if len(opt_dic['def_range'])==0:cond_calc_pix = np.ones(data_dic[inst][vis]['nspec'] ,dtype=bool)    
+        if len(opt_dic['def_range'])==0:cond_calc_pix = np.ones(data_vis['nspec'] ,dtype=bool)    
         else:cond_calc_pix = (data_loc_exp['edge_bins'][def_iord][0:-1]>=opt_dic['def_range'][0]) & (data_loc_exp['edge_bins'][def_iord][1:]<=opt_dic['def_range'][1])             
         idx_calc_pix = np_where1D(cond_calc_pix)
-
+        cond_def_full = np.zeros(data_vis['nspec'],dtype=bool)
+        cond_def_full[idx_calc_pix] = True
+    
+        #Saves
+        data_store = {'cen_bins':data_loc_exp['cen_bins'],'edge_bins':data_loc_exp['edge_bins'],'cond_def':np.array([cond_def_full])}
+    
         #Final table for model line profile
         fixed_args['ncen_bins']=len(idx_calc_pix)
         fixed_args['dim_exp'] = [1,fixed_args['ncen_bins']] 
         fixed_args['cen_bins'] = data_loc_exp['cen_bins'][def_iord,idx_calc_pix]
         fixed_args['edge_bins']=data_loc_exp['edge_bins'][def_iord,idx_calc_pix[0]:idx_calc_pix[-1]+2]
         fixed_args['dcen_bins']=fixed_args['edge_bins'][1::] - fixed_args['edge_bins'][0:-1] 
-
+    
         #Initializing stellar profiles
         #    - can be defined using the first exposure table
         if isub==0:
-            fixed_args = init_custom_DI_prof(fixed_args,gen_dic,data_dic[inst][vis]['system_prop'],{},theo_dic,system_param['star'],params)                  
-
+            fixed_args = init_custom_DI_prof(fixed_args,gen_dic,data_vis['system_prop'],spots_prop,theo_dic,system_param['star'],params)                  
+    
             #Effective instrumental convolution
             fixed_args['FWHM_inst'] = get_FWHM_inst(inst,fixed_args,fixed_args['cen_bins'])
-
+    
         #Resampled spectral table for model line profile
         if fixed_args['resamp']:resamp_st_prof_tab(None,None,None,fixed_args,gen_dic,1,theo_dic['rv_osamp_line_mod'])
         
         #Table for model calculation
-        args_exp = def_st_prof_tab(None,None,None,fixed_args)      
-
+        args_exp = def_st_prof_tab(None,None,None,fixed_args) 
+    
         #Define broadband scaling of intrinsic profiles into local profiles
-        if data_dic['Intr']['plocc_prof_type']=='Res':
+        if plocc_prof_type=='Res':
             args_exp['Fsurf_grid_spec'] = theo_intr2loc(fixed_args['grid_dic'],fixed_args['system_prop'],args_exp,args_exp['ncen_bins'],fixed_args['grid_dic']['nsub_star']) 
+    
+        #Planet-occulted properties
+        surf_prop_dic,spot_prop_dic,_ = sub_calc_plocc_spot_prop([chrom_mode],args_exp,['line_prof'],data_vis['transit_pl'],deepcopy(system_param),theo_dic,fixed_args['system_prop'],params,coord_pl_sp,[iexp_glob],system_spot_prop_in=fixed_args['system_spot_prop'])
 
-        #Planet-occulted line profile 
-        surf_prop_dic,spot_prop_dic = sub_calc_plocc_spot_prop([chrom_mode],args_exp,['line_prof'],data_dic[inst][vis]['transit_pl'],deepcopy(system_param),theo_dic,fixed_args['system_prop'],params,coord_dic[inst][vis],[gen_dic[inst][vis]['idx_in2exp'][i_in]])
-        sp_line_model = surf_prop_dic[chrom_mode]['line_prof'][:,0]
+        #With spots
+        if spot_on:
+            save_path = gen_dic['save_data_dir']+'Diff_estimates/'+corr_mode+'/'+inst+'_'+vis+'_'+str(iexp)
+
+            #Planet-occulted and spotted line profiles - unclean
+            pl_line_model = surf_prop_dic[chrom_mode]['line_prof'][:,0]
+            sp_line_model = spot_prop_dic[chrom_mode]['line_prof'][:,0]
+            line_prof_cons = {'unclean_pl_flux':pl_line_model, 'unclean_sp_flux':sp_line_model}
+            
+            #Planet-occulted and spotted line profiles - clean
+            if opt_dic['clean_calc']:
+                
+                #Only planet-occulted profiles
+                clean_surf_prop_dic,_,_ = sub_calc_plocc_spot_prop([chrom_mode],args_exp,['line_prof'],data_vis['transit_pl'],deepcopy(system_param),theo_dic,fixed_args['system_prop'],clean_params,coord_pl_sp,[iexp])
+                
+                #Only spotted profiles
+                _,clean_spot_prop_dic,_ = sub_calc_plocc_spot_prop([chrom_mode],args_exp,['line_prof'],[],deepcopy(system_param),theo_dic,fixed_args['system_prop'],params,coord_pl_sp,[iexp],system_spot_prop_in=fixed_args['system_spot_prop'])
+    
+                #Storing
+                clean_pl_line_model = clean_surf_prop_dic[chrom_mode]['line_prof'][:,0]
+                clean_sp_line_model = clean_spot_prop_dic[chrom_mode]['line_prof'][:,0]
+                line_prof_cons.update({'clean_pl_flux':clean_pl_line_model, 'clean_sp_flux':clean_sp_line_model})
 
-        #Scaling to fitted intrinsic continuum level
-        if (data_dic['Intr']['plocc_prof_type']=='Intr'):sp_line_model*=params['cont']   
- 
-        #Conversion and resampling 
-        flux_loc = conv_st_prof_tab(None,None,None,fixed_args,args_exp,sp_line_model,fixed_args['FWHM_inst'])
+        #Without spots
+        else:
+            save_path = gen_dic['save_data_dir']+'Loc_estimates/'+corr_mode+'/'+inst+'_'+vis+'_'+str(iexp)
+    
+            #Planet-occulted line profile 
+            sp_line_model = surf_prop_dic[chrom_mode]['line_prof'][:,0]
+            line_prof_cons = {'flux':sp_line_model}
         
-        #Filling full table with defined reconstructed profile
-        flux_full = np.zeros(data_dic[inst][vis]['nspec'],dtype=float)*np.nan
-        flux_full[idx_calc_pix] = flux_loc
-        cond_def_full = np.zeros(data_dic[inst][vis]['nspec'],dtype=bool)
-        cond_def_full[idx_calc_pix] = True
-
-        #Saving estimate of local profile for current exposure                   
-        np.savez_compressed(gen_dic['save_data_dir']+'Loc_estimates/'+corr_mode+'/'+inst+'_'+vis+'_'+str(i_in),
-                            data={'cen_bins':data_loc_exp['cen_bins'],'edge_bins':data_loc_exp['edge_bins'],'cond_def':np.array([cond_def_full]),'flux' : np.array([flux_full])},allow_pickle=True)
+        #Exposure profiles
+        for line_prof in list(line_prof_cons.keys()):
+           
+            #Scaling to fitted intrinsic continuum level
+            #    - model profiles have been output with a continuum level unity (through the option 'conv2intr') and are thus scaled to the fitted level
+            if plocc_prof_type=='Intr':line_prof_cons['flux']*=params['cont']
+         
+            #Conversion and resampling 
+            flux_loc = conv_st_prof_tab(None,None,None,fixed_args,args_exp,line_prof_cons['flux'],fixed_args['FWHM_inst'])
+        
+            #Filling full table with defined reconstructed profile
+            plocc_prof = np.zeros(data_vis['nspec'],dtype=float)*np.nan
+            plocc_prof[idx_calc_pix] = flux_loc
+            
+            #Store
+            data_store.update({line_prof:np.array([plocc_prof])})
+        
+        #Saving estimate of local profile for current exposure                 
+        np.savez_compressed(save_path,data=data_store,allow_pickle=True)
 
     #Complementary data
-    data_add={'idx_est_loc':range(data_dic[inst][vis]['n_in_tr']),'cont':params['cont']}
+    data_add={'idx_est_loc':iexp_list,'cont':params['cont']}
 
     return data_add
 
 
 
-def loc_prof_indivmod(opt_dic,corr_mode,inst,vis,gen_dic,data_dic):
+def plocc_prof_indivmod(opt_dic,corr_mode,inst,vis,gen_dic,data_dic):
     r"""**Planet-occulted exposure profiles: individual model**
     
     Sub-function to define planet-occulted profiles using line profile model fitted to individual intrinsic lines.
     These models correspond directly to the measured profile and needs only be rescaled to the level of the local profile.
     This approach only works for exposures in which the stellar line could be fitted correctly after excluding the planet-contaminated range
 
     Args:
@@ -374,15 +475,15 @@
     data_prop=(np.load(gen_dic['save_data_dir']+'Introrig_prop/'+inst+'_'+vis+'.npz',allow_pickle=True)['data'].item())['prof_fit_dic']
     idx_aligned = np_where1D(data_prop['cond_detected'])
 
     #Processing in-transit exposures
     for i_in in idx_aligned:
      
         #Model intrinsic profile
-        data_est_loc={'cen_bins':data_prop[i_in]['cen_bins'],'edge_bins':data_prop[i_in]['edge_bins'],'flux':data_prop[i_in]['flux'][:,None],'cond_def':np.ones(data_dic[inst][vis]['dim_exp'],dtype=bool)}
+        data_est_loc={'cen_bins':data_prop[i_in]['cen_bins'],'edge_bins':data_prop[i_in]['edge_bins'],'flux':data_prop[i_in]['flux'][:,None],'cond_def':np.ones(data_vis['dim_exp'],dtype=bool)}
 
         #Rescaling model intrinsic profile to the level of the local profile
         if data_dic['Intr']['plocc_prof_type']=='Res':
             loc_flux_scaling = dataload_npz(data_vis['scaled_Intr_data_paths']+str(gen_dic[inst][vis]['idx_in2exp'][i_in]))['loc_flux_scaling']
             data_est_loc['flux'][0] *= loc_flux_scaling(data_est_loc['cen_bins'][0]) 
 
         #Saving estimate of local profile for current exposure                   
@@ -391,15 +492,15 @@
     #Complementary data
     data_add={'idx_est_loc':idx_aligned}
       
     return data_add
 
 
 
-def loc_prof_rec(opt_dic,corr_mode,inst,vis,gen_dic,data_dic,coord_dic):
+def plocc_prof_rec(opt_dic,corr_mode,inst,vis,gen_dic,data_dic,coord_dic):
     r"""**Planet-occulted exposure profiles: reconstructed**
     
     Sub-function to define planet-occulted profiles by reconstructing undefined pixels via a polynomial fit to defined pixels in complementary exposures, or via a 2D interpolation over complementary exposures and a narrow spectral band.
     
      - providing the planetary track shifts sufficiently during the transit, we can reconstruct the local spectra at all wavelengths by interpolating the surrounding spectra at the wavelengths masked for planetary absorption.
        this approach allows accounting for changes in the shape of the local stellar spectra between exposures.
      - we reconstruct undefined pixels in the map of intrinsic profiles aligned in the null rest frame and resampled on the common spectral table.
@@ -579,35 +680,94 @@
 
         #Upload residual or intrinsic profile for current exposure to get its spectral tables
         if data_dic['Intr']['plocc_prof_type']=='Intr':iexp_eff = i_in
         else:iexp_eff = gen_dic[inst][vis]['idx_in2exp'][i_in]
         data_loc_exp = dataload_npz(data_vis['proc_'+data_dic['Intr']['plocc_prof_type']+'_data_paths']+str(iexp_eff))  
 
         #Radial velocity shifts set to the opposite of the planet-occulted surface rv associated with current exposure
-        rv_surf_star,rv_surf_star_edge = def_surf_shift(data_dic['Intr']['align_mode'],dic_rv,i_in,data_rec[isub],ref_pl,data_vis['type'],data_dic[inst][vis]['system_prop'],data_dic[inst][vis]['dim_exp'],data_dic[inst]['nord'],data_dic[inst][vis]['nspec'])
+        rv_surf_star,rv_surf_star_edge = def_surf_shift(data_dic['Intr']['align_mode'],dic_rv,i_in,data_rec[isub],ref_pl,data_vis['type'],data_vis['system_prop'],data_vis['dim_exp'],data_dic[inst]['nord'],data_vis['nspec'])
 
         #Aligning reconstructed profile at current exposure stellar surface rv 
         #    - reconstructed profile is already aligned in a null rest frame and resampled on a common table
         #    - aligned profiles are resampled on the table of current exposure, which is common to all exposures if a common table is used 
         rv_shift_cen = -rv_surf_star
         spec_dopshift_cen = gen_specdopshift(rv_surf_star)
         if rv_surf_star_edge is not None:
             rv_shift_edge = -rv_surf_star_edge
             spec_dopshift_edge = gen_specdopshift(rv_surf_star_edge)
         else:
             rv_shift_edge = None
             spec_dopshift_edge = None  
-        data_est_loc=align_data(data_rec[isub],data_vis['type'],data_dic[inst]['nord'],data_dic[inst][vis]['dim_exp'],gen_dic['resamp_mode'],data_loc_exp['cen_bins'],data_loc_exp['edge_bins'],rv_shift_cen,spec_dopshift_cen,rv_shift_edge = rv_shift_edge,spec_dopshift_edge = spec_dopshift_edge, nocov = True)
+        data_est_loc=align_data(data_rec[isub],data_vis['type'],data_dic[inst]['nord'],data_vis['dim_exp'],gen_dic['resamp_mode'],data_loc_exp['cen_bins'],data_loc_exp['edge_bins'],rv_shift_cen,spec_dopshift_cen,rv_shift_edge = rv_shift_edge,spec_dopshift_edge = spec_dopshift_edge, nocov = True)
 
         #Rescaling reconstructed intrinsic profile to the level of the local profile
         if data_dic['Intr']['plocc_prof_type']=='Res':
             loc_flux_scaling = dataload_npz(data_vis['scaled_Intr_data_paths']+str(gen_dic[inst][vis]['idx_in2exp'][i_in]))['loc_flux_scaling']
             for iord in range(data_dic[inst]['nord']):data_est_loc['flux'][iord] *=loc_flux_scaling(data_est_loc['cen_bins'][iord]) 
 
         #Saving estimate of local profile for current exposure                   
         np.savez_compressed(gen_dic['save_data_dir']+'Loc_estimates/'+corr_mode+'/'+inst+'_'+vis+'_'+str(i_in),data=data_est_loc,allow_pickle=True)
 
 
     #Complementary data
     data_add={'idx_est_loc':idx_aligned}
 
     return data_add
+
+
+
+#%% Differential exposure profiles.
+#    - accounting for planet-occulted and spotted stellar profiles
+
+def def_diff_profiles(inst,vis,gen_dic,data_dic,data_prop,coord_dic,system_param,theo_dic,glob_fit_dic,plot_dic):
+    r"""**Planet-occulted and spotted exposure profiles.**
+    
+    Calls requested function to define planet-occulted and spotted profiles associated with each observed exposure
+
+    Args:
+        TBD
+    
+    Returns:
+        TBD
+    
+    """ 
+    print('   > Building estimates for planet-occulted and spotted stellar profiles')
+    if data_dic[inst][vis]['spots_prop']=={}:stop('Spot properties are not provided. We recommended using the separate routine dedicated to the extraction of planet-occulted profiles instead.')
+    opt_dic = data_dic['Res']['opt_loc_data_corr'] 
+    corr_mode = opt_dic['corr_mode']
+    print('         Using global model')  
+
+    #Calculating
+    if (gen_dic['calc_res_loc_data_corr']):
+        print('         Calculating data')     
+             
+        #Calculating the clean version of the data
+        opt_dic['clean_calc']=False
+        if (plot_dic['map_Res_prof_clean_pl_est']!='') or (plot_dic['map_Res_prof_clean_sp_est']!=''):
+            opt_dic['clean_calc']=True
+
+        #Using global profile model
+        if corr_mode=='glob_mod': 
+            data_add = plocc_spocc_prof_globmod(opt_dic,corr_mode,inst,vis,gen_dic,data_dic,data_prop,system_param,theo_dic,coord_dic,glob_fit_dic,False)
+        
+        else:stop('WARNING: Only joined-fit results can be used at the moment. Set corr_mode to \'glob_mod\'')
+
+        #Saving complementary data for plots
+        if (plot_dic['map_Res_prof_clean_sp_res']!='') or (plot_dic['map_Res_prof_clean_pl_res']!='') or (plot_dic['map_Res_prof_unclean_sp_res']!='') or (plot_dic['map_Res_prof_unclean_pl_res']!=''):
+            data_add['loc_data_corr_path'] = data_dic[inst][vis]['proc_Res_data_paths']
+            data_add['rest_frame'] = data_dic['Res'][inst][vis]['rest_frame']
+        datasave_npz(gen_dic['save_data_dir']+'Diff_estimates/'+corr_mode+'/'+inst+'_'+vis+'_add',data_add)
+
+    #Checking that local data has been calculated for all exposures
+    else:
+        idx_est_loc = dataload_npz(gen_dic['save_data_dir']+'Diff_estimates/'+corr_mode+'/'+inst+'_'+vis+'_add')['idx_est_loc']
+        data_paths={i_in:gen_dic['save_data_dir']+'Diff_estimates/'+corr_mode+'/'+inst+'_'+vis+'_'+str(i_in) for i_in in idx_est_loc}
+        check_data(data_paths)
+
+    return None
+
+
+
+
+
+
+
```

### Comparing `antaress-1.1.0/src/antaress.egg-info/PKG-INFO` & `antaress-1.1.1/src/antaress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antaress
-Version: 1.1.0
+Version: 1.1.1
 Summary: High-resolution spectroscopy pipeline
 Author-email: Vincent Bourrier <vincent.bourrier@unige.ch>
 Project-URL: Homepage, https://gitlab.unige.ch/bourrier/ANTARESS
 Project-URL: Issues, https://gitlab.unige.ch/bourrier/ANTARESS/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `antaress-1.1.0/src/antaress.egg-info/SOURCES.txt` & `antaress-1.1.1/src/antaress.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE
 README.md
 pyproject.toml
+setup.py
 src/antaress/__init__.py
 src/antaress.egg-info/PKG-INFO
 src/antaress.egg-info/SOURCES.txt
 src/antaress.egg-info/dependency_links.txt
 src/antaress.egg-info/entry_points.txt
 src/antaress.egg-info/requires.txt
 src/antaress.egg-info/top_level.txt
 src/antaress/ANTARESS_analysis/ANTARESS_ana_comm.py
 src/antaress/ANTARESS_analysis/ANTARESS_inst_resp.py
 src/antaress/ANTARESS_analysis/ANTARESS_joined_atm.py
 src/antaress/ANTARESS_analysis/ANTARESS_joined_star.py
 src/antaress/ANTARESS_analysis/ANTARESS_model_prof.py
 src/antaress/ANTARESS_analysis/__init__.py
+src/antaress/ANTARESS_analysis/C_grid/Gauss_star_grid.c
 src/antaress/ANTARESS_conversions/ANTARESS_binning.py
 src/antaress/ANTARESS_conversions/ANTARESS_conv.py
 src/antaress/ANTARESS_conversions/ANTARESS_masks_gen.py
 src/antaress/ANTARESS_conversions/ANTARESS_sp_cont.py
 src/antaress/ANTARESS_conversions/__init__.py
 src/antaress/ANTARESS_conversions/KitCat/KitCat_main.py
 src/antaress/ANTARESS_conversions/KitCat/Kitcat_classes.py
@@ -33,17 +35,16 @@
 src/antaress/ANTARESS_corrections/__init__.py
 src/antaress/ANTARESS_corrections/Telluric_processing/Create_static_files.py
 src/antaress/ANTARESS_general/__init__.py
 src/antaress/ANTARESS_general/constant_data.py
 src/antaress/ANTARESS_general/minim_routines.py
 src/antaress/ANTARESS_general/utils.py
 src/antaress/ANTARESS_grids/ANTARESS_coord.py
-src/antaress/ANTARESS_grids/ANTARESS_plocc_grid.py
+src/antaress/ANTARESS_grids/ANTARESS_occ_grid.py
 src/antaress/ANTARESS_grids/ANTARESS_prof_grid.py
-src/antaress/ANTARESS_grids/ANTARESS_spots.py
 src/antaress/ANTARESS_grids/ANTARESS_star_grid.py
 src/antaress/ANTARESS_grids/__init__.py
 src/antaress/ANTARESS_launch/ANTARESS_gridrun.py
 src/antaress/ANTARESS_launch/ANTARESS_launcher.py
 src/antaress/ANTARESS_launch/ANTARESS_settings.py
 src/antaress/ANTARESS_launch/ANTARESS_systems.py
 src/antaress/ANTARESS_launch/__init__.py
```

