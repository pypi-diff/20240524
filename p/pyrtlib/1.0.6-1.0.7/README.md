# Comparing `tmp/pyrtlib-1.0.6.tar.gz` & `tmp/pyrtlib-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtlib-1.0.6.tar", last modified: Tue Apr 23 08:31:02 2024, max compression
+gzip compressed data, was "pyrtlib-1.0.7.tar", last modified: Fri May 24 07:19:56 2024, max compression
```

## Comparing `pyrtlib-1.0.6.tar` & `pyrtlib-1.0.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.621476 pyrtlib-1.0.6/pyrtlib/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.625476 pyrtlib-1.0.6/pyrtlib/_lineshape/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61798 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/h2o_lineshape.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/h2oll.py
--rw-r--r--   0 runner    (1001) docker     (127)   125023 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/o2_lineshape.nc
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/o2ll.py
--rw-r--r--   0 runner    (1001) docker     (127)    91535 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/o3_lineshape.nc
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/_lineshape/o3ll.py
--rw-r--r--   0 runner    (1001) docker     (127)    34466 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/absorption_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.625476 pyrtlib-1.0.6/pyrtlib/apiwebservices/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/apiwebservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/apiwebservices/eps_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/apiwebservices/erafive.py
--rw-r--r--   0 runner    (1001) docker     (127)    21562 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/apiwebservices/igra2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/apiwebservices/webservices.py
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/apiwebservices/wyomingupperair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/pyrtlib/climatology/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/atmospheric_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    27815 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/extrapolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26250 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/gas_minor.dat
--rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/gas_trace.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/midlatitude_summer.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/midlatitude_winter.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/subarctic_summer.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/subarctic_winter.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/tropical.dat
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/climatology/us_standard.dat
--rw-r--r--   0 runner    (1001) docker     (127)    24312 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/rt_equation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16955 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/tb_spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/pyrtlib/uncertainty/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/uncertainty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22719 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/uncertainty/absmod_uncertainty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R17/
--rw-r--r--   0 runner    (1001) docker     (127)   130507 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2018_V1.1.nc
--rw-r--r--   0 runner    (1001) docker     (127)   134781 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2019_V2.0.nc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R19/
--rw-r--r--   0 runner    (1001) docker     (127)   183368 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R19/Cov_parameters_Gallucci_et_al_ACPD_2023_V1.0.nc
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32209 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/pyrtlib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/pyrtlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-23 08:31:02.000000 pyrtlib-1.0.6/pyrtlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-23 08:31:02.000000 pyrtlib-1.0.6/pyrtlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:31:02.000000 pyrtlib-1.0.6/pyrtlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-23 08:31:02.000000 pyrtlib-1.0.6/pyrtlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 08:31:02.000000 pyrtlib-1.0.6/pyrtlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 08:31:02.629476 pyrtlib-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-23 08:30:55.000000 pyrtlib-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:56.034775 pyrtlib-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-24 07:19:56.034775 pyrtlib-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:56.026775 pyrtlib-1.0.7/pyrtlib/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:56.030775 pyrtlib-1.0.7/pyrtlib/_lineshape/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/_lineshape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59853 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/_lineshape/h2o_lineshape.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/_lineshape/h2oll.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125023 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/_lineshape/o2_lineshape.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/_lineshape/o2ll.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91535 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/_lineshape/o3_lineshape.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/_lineshape/o3ll.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34494 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/absorption_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:56.030775 pyrtlib-1.0.7/pyrtlib/apiwebservices/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/apiwebservices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/apiwebservices/eps_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/apiwebservices/erafive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21562 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/apiwebservices/igra2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/apiwebservices/webservices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/apiwebservices/wyomingupperair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:56.030775 pyrtlib-1.0.7/pyrtlib/climatology/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/climatology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/climatology/atmospheric_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27815 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/climatology/extrapolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26250 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/climatology/gas_minor.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/climatology/gas_trace.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/climatology/midlatitude_summer.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/climatology/midlatitude_winter.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/climatology/subarctic_summer.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/climatology/subarctic_winter.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/climatology/tropical.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/climatology/us_standard.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/rt_equation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16969 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/tb_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:56.034775 pyrtlib-1.0.7/pyrtlib/uncertainty/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/uncertainty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22719 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/uncertainty/absmod_uncertainty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:56.034775 pyrtlib-1.0.7/pyrtlib/uncertainty/covariance_matrix/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:56.034775 pyrtlib-1.0.7/pyrtlib/uncertainty/covariance_matrix/R17/
+-rw-r--r--   0 runner    (1001) docker     (127)   130507 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2018_V1.1.nc
+-rw-r--r--   0 runner    (1001) docker     (127)   134781 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2019_V2.0.nc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:56.034775 pyrtlib-1.0.7/pyrtlib/uncertainty/covariance_matrix/R19/
+-rw-r--r--   0 runner    (1001) docker     (127)   183368 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/uncertainty/covariance_matrix/R19/Cov_parameters_Gallucci_et_al_ACPD_2023_V1.0.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/uncertainty/covariance_matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32469 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/pyrtlib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:56.034775 pyrtlib-1.0.7/pyrtlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-24 07:19:56.000000 pyrtlib-1.0.7/pyrtlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-24 07:19:56.000000 pyrtlib-1.0.7/pyrtlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:19:56.000000 pyrtlib-1.0.7/pyrtlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-24 07:19:56.000000 pyrtlib-1.0.7/pyrtlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 07:19:56.000000 pyrtlib-1.0.7/pyrtlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-24 07:19:56.034775 pyrtlib-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-24 07:19:52.000000 pyrtlib-1.0.7/setup.py
```

### Comparing `pyrtlib-1.0.6/LICENSE` & `pyrtlib-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/PKG-INFO` & `pyrtlib-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtlib
-Version: 1.0.6
+Version: 1.0.7
 Summary: pyrtlib - Radiative Transfer library
 Author: slarosa
 Author-email: salvatore-larosa@cnr.it
 License: GPLv3
 Project-URL: Documentation, https://satclop.github.io/pyrtlib
 Project-URL: Repository, https://github.com/SatCloP/pyrtlib
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyrtlib-1.0.6/README.md` & `pyrtlib-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/_lineshape/h2o_lineshape.nc` & `pyrtlib-1.0.7/pyrtlib/_lineshape/h2o_lineshape.nc`

 * *Files 12% similar despite different names*

#### h5dump {}

```diff
@@ -1,8 +1,8 @@
-HDF5 "/tmp/diffoscope_jv4j2m_v_/tmpg58q2l11_TarContainer/0/8.nc" {
+HDF5 "/tmp/diffoscope_jv4j2m_v_/tmpeom1c6ir_TarContainer/0/8.nc" {
 GROUP "/" {
    ATTRIBUTE "_NCProperties" {
       DATATYPE  H5T_STRING {
          STRSIZE 34;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_ASCII;
          CTYPE H5T_C_S1;
@@ -136,30 +136,30 @@
             }
          }
       }
       DATASET "mtx" {
          DATATYPE  H5T_IEEE_F64LE
          DATASPACE  SIMPLE { ( 15, 9 ) / ( 15, 9 ) }
          DATA {
-         (0,0): 11, 22.2351, 1.314e-14, 2.144, 2.81, 0.69, 13.49, 0.61, 0,
-         (1,0): 11, 183.31, 2.279e-12, 0.668, 2.87, 0.64, 14.91, 0.85,
-         (1,8): -0.017,
-         (2,0): 11, 321.226, 8.058e-14, 6.179, 2.3, 0.67, 10.8, 0.54, 0,
-         (3,0): 11, 325.153, 2.701e-12, 1.541, 2.78, 0.68, 13.5, 0.74, 0,
-         (4,0): 11, 380.197, 2.444e-11, 1.048, 2.87, 0.54, 15.41, 0.89, 0,
-         (5,0): 11, 439.151, 2.185e-12, 3.595, 2.1, 0.63, 9, 0.52, 0,
-         (6,0): 11, 443.018, 4.637e-13, 5.048, 1.86, 0.6, 7.88, 0.5, 0,
-         (7,0): 11, 448.001, 2.568e-11, 1.405, 2.63, 0.66, 12.75, 0.67, 0,
-         (8,0): 11, 470.889, 8.392e-13, 3.597, 2.15, 0.66, 9.83, 0.65, 0,
-         (9,0): 11, 474.689, 3.272e-12, 2.379, 2.36, 0.65, 10.95, 0.64, 0,
-         (10,0): 11, 488.491, 6.676e-13, 2.852, 2.6, 0.69, 13.13, 0.72, 0,
-         (11,0): 11, 556.936, 1.535e-09, 0.159, 3.21, 0.69, 13.2, 1, 0,
-         (12,0): 11, 620.701, 1.711e-11, 2.391, 2.44, 0.71, 11.4, 0.68, 0,
-         (13,0): 11, 752.033, 1.014e-09, 0.396, 3.06, 0.68, 12.53, 0.84, 0,
-         (14,0): 11, 916.171, 4.238e-11, 1.441, 2.67, 0.7, 12.75, 0.78, 0
+         (0,0): 11, 22.2351, 1.314e-14, 2.144, 2.81, 0.69, 0, 13.49, 0.61,
+         (1,0): 11, 183.31, 2.279e-12, 0.668, 2.87, 0.64, -0.017, 14.91,
+         (1,8): 0.85,
+         (2,0): 11, 321.226, 8.058e-14, 6.179, 2.3, 0.67, 0, 10.8, 0.54,
+         (3,0): 11, 325.153, 2.701e-12, 1.541, 2.78, 0.68, 0, 13.5, 0.74,
+         (4,0): 11, 380.197, 2.444e-11, 1.048, 2.87, 0.54, 0, 15.41, 0.89,
+         (5,0): 11, 439.151, 2.185e-12, 3.595, 2.1, 0.63, 0, 9, 0.52,
+         (6,0): 11, 443.018, 4.637e-13, 5.048, 1.86, 0.6, 0, 7.88, 0.5,
+         (7,0): 11, 448.001, 2.568e-11, 1.405, 2.63, 0.66, 0, 12.75, 0.67,
+         (8,0): 11, 470.889, 8.392e-13, 3.597, 2.15, 0.66, 0, 9.83, 0.65,
+         (9,0): 11, 474.689, 3.272e-12, 2.379, 2.36, 0.65, 0, 10.95, 0.64,
+         (10,0): 11, 488.491, 6.676e-13, 2.852, 2.6, 0.69, 0, 13.13, 0.72,
+         (11,0): 11, 556.936, 1.535e-09, 0.159, 3.21, 0.69, 0, 13.2, 1,
+         (12,0): 11, 620.701, 1.711e-11, 2.391, 2.44, 0.71, 0, 11.4, 0.68,
+         (13,0): 11, 752.033, 1.014e-09, 0.396, 3.06, 0.68, 0, 12.53, 0.84,
+         (14,0): 11, 916.171, 4.238e-11, 1.441, 2.67, 0.7, 0, 12.75, 0.78
          }
          ATTRIBUTE "DIMENSION_LIST" {
             DATATYPE  H5T_VLEN { H5T_REFERENCE { H5T_STD_REF_OBJECT }}
             DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
             DATA {
             (0): (DATASET 3205 "/R03/rows"), (DATASET 3529 "/R03/cols")
             }
@@ -230,17 +230,17 @@
             }
          }
       }
    }
    GROUP "R16" {
       DATASET "cols" {
          DATATYPE  H5T_IEEE_F32BE
-         DATASPACE  SIMPLE { ( 15 ) / ( 15 ) }
+         DATASPACE  SIMPLE { ( 9 ) / ( 9 ) }
          DATA {
-         (0): 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
+         (0): 0, 0, 0, 0, 0, 0, 0, 0, 0
          }
          ATTRIBUTE "CLASS" {
             DATATYPE  H5T_STRING {
                STRSIZE 16;
                STRPAD H5T_STR_NULLTERM;
                CSET H5T_CSET_ASCII;
                CTYPE H5T_C_S1;
@@ -255,15 +255,15 @@
                STRSIZE 64;
                STRPAD H5T_STR_NULLTERM;
                CSET H5T_CSET_ASCII;
                CTYPE H5T_C_S1;
             }
             DATASPACE  SCALAR
             DATA {
-            (0): "This is a netCDF dimension but not a netCDF variable.        15"
+            (0): "This is a netCDF dimension but not a netCDF variable.         9"
             }
          }
          ATTRIBUTE "REFERENCE_LIST" {
             DATATYPE  H5T_COMPOUND {
                H5T_REFERENCE { H5T_STD_REF_OBJECT } "dataset";
                H5T_STD_U32LE "dimension";
             }
@@ -353,46 +353,41 @@
             DATA {
             (0): 8
             }
          }
       }
       DATASET "mtx" {
          DATATYPE  H5T_IEEE_F64LE
-         DATASPACE  SIMPLE { ( 15, 15 ) / ( 15, 15 ) }
+         DATASPACE  SIMPLE { ( 15, 9 ) / ( 15, 9 ) }
          DATA {
          (0,0): 11, 22.2351, 1.317e-14, 2.144, 2.665, 0.76, -0.0088, 13.6, 1,
-         (0,9): 6, 1, 6, 5, 2, 3,
          (1,0): 11, 183.31, 2.334e-12, 0.668, 2.936, 0.77, -0.024, 14.76,
-         (1,8): 0.85, 3, 1, 3, 2, 2, 0,
+         (1,8): 0.85,
          (2,0): 11, 321.226, 7.861e-14, 6.179, 2.426, 0.67, -0.059, 10.65,
-         (2,8): 0.54, 10, 2, 9, 9, 3, 6,
+         (2,8): 0.54,
          (3,0): 11, 325.153, 2.725e-12, 1.541, 2.847, 0.64, -0.0045, 13.95,
-         (3,8): 0.74, 5, 1, 5, 4, 2, 2,
+         (3,8): 0.74,
          (4,0): 11, 380.197, 2.473e-11, 1.048, 2.831, 0.54, -0.0278, 14.4,
-         (4,8): 0.89, 4, 1, 4, 3, 2, 1,
+         (4,8): 0.89,
          (5,0): 11, 439.151, 2.152e-12, 3.595, 2.024, 0.63, 0.0182, 9.06,
-         (5,8): 0.52, 6, 4, 3, 5, 5, 0,
-         (6,0): 11, 443.018, 4.494e-13, 5.048, 1.568, 0.6, 0, 7.96, 0.5, 7,
-         (6,10): 5, 2, 6, 6, 1,
+         (5,8): 0.52,
+         (6,0): 11, 443.018, 4.494e-13, 5.048, 1.568, 0.6, 0, 7.96, 0.5,
          (7,0): 11, 448.001, 2.586e-11, 1.405, 2.587, 0.66, -0.0464, 13.01,
-         (7,8): 0.67, 4, 2, 3, 3, 3, 0,
+         (7,8): 0.67,
          (8,0): 11, 470.889, 8.253e-13, 3.597, 2.153, 0.66, 0.024, 9.7, 0.65,
-         (8,9): 6, 4, 2, 5, 5, 1,
          (9,0): 11, 474.689, 3.274e-12, 2.379, 2.34, 0.65, -0.019, 11.24,
-         (9,8): 0.64, 5, 3, 3, 4, 4, 0,
+         (9,8): 0.64,
          (10,0): 11, 488.49, 6.721e-13, 2.852, 2.61, 0.69, 0.069, 13.58,
-         (10,8): 0.72, 6, 2, 4, 7, 1, 7,
+         (10,8): 0.72,
          (11,0): 11, 556.936, 1.561e-09, 0.159, 3.115, 0.69, 0.06, 14.24, 1,
-         (11,9): 1, 1, 0, 1, 0, 1,
          (12,0): 11, 620.701, 1.704e-11, 2.391, 2.468, 0.75, 0, 11.94, 0.68,
-         (12,9): 5, 3, 2, 4, 4, 1,
          (13,0): 11, 752.033, 1.029e-09, 0.396, 3.114, 0.68, 0.052, 13.58,
-         (13,8): 0.84, 2, 1, 1, 2, 0, 2,
+         (13,8): 0.84,
          (14,0): 11, 916.172, 4.266e-11, 1.441, 2.698, 0.72, -0.0208, 13.91,
-         (14,8): 0.78, 4, 2, 2, 3, 3, 1
+         (14,8): 0.78
          }
          ATTRIBUTE "DIMENSION_LIST" {
             DATATYPE  H5T_VLEN { H5T_REFERENCE { H5T_STD_REF_OBJECT }}
             DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
             DATA {
             (0): (DATASET 13074 "/R16/rows"), (DATASET 13398 "/R16/cols")
             }
@@ -463,17 +458,17 @@
             }
          }
       }
    }
    GROUP "R17" {
       DATASET "cols" {
          DATATYPE  H5T_IEEE_F32BE
-         DATASPACE  SIMPLE { ( 15 ) / ( 15 ) }
+         DATASPACE  SIMPLE { ( 9 ) / ( 9 ) }
          DATA {
-         (0): 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
+         (0): 0, 0, 0, 0, 0, 0, 0, 0, 0
          }
          ATTRIBUTE "CLASS" {
             DATATYPE  H5T_STRING {
                STRSIZE 16;
                STRPAD H5T_STR_NULLTERM;
                CSET H5T_CSET_ASCII;
                CTYPE H5T_C_S1;
@@ -488,15 +483,15 @@
                STRSIZE 64;
                STRPAD H5T_STR_NULLTERM;
                CSET H5T_CSET_ASCII;
                CTYPE H5T_C_S1;
             }
             DATASPACE  SCALAR
             DATA {
-            (0): "This is a netCDF dimension but not a netCDF variable.        15"
+            (0): "This is a netCDF dimension but not a netCDF variable.         9"
             }
          }
          ATTRIBUTE "REFERENCE_LIST" {
             DATATYPE  H5T_COMPOUND {
                H5T_REFERENCE { H5T_STD_REF_OBJECT } "dataset";
                H5T_STD_U32LE "dimension";
             }
@@ -586,46 +581,41 @@
             DATA {
             (0): 11
             }
          }
       }
       DATASET "mtx" {
          DATATYPE  H5T_IEEE_F64LE
-         DATASPACE  SIMPLE { ( 15, 15 ) / ( 15, 15 ) }
+         DATASPACE  SIMPLE { ( 15, 9 ) / ( 15, 9 ) }
          DATA {
          (0,0): 11, 22.2351, 1.317e-14, 2.144, 2.665, 0.76, -0.0088, 13.6, 1,
-         (0,9): 6, 1, 6, 5, 2, 3,
          (1,0): 11, 183.31, 2.334e-12, 0.668, 2.936, 0.77, -0.024, 14.76,
-         (1,8): 0.85, 3, 1, 3, 2, 2, 0,
+         (1,8): 0.85,
          (2,0): 11, 321.226, 7.861e-14, 6.179, 2.426, 0.67, -0.059, 10.65,
-         (2,8): 0.54, 10, 2, 9, 9, 3, 6,
+         (2,8): 0.54,
          (3,0): 11, 325.153, 2.725e-12, 1.541, 2.847, 0.64, -0.0045, 13.95,
-         (3,8): 0.74, 5, 1, 5, 4, 2, 2,
+         (3,8): 0.74,
          (4,0): 11, 380.197, 2.473e-11, 1.048, 2.831, 0.54, -0.0278, 14.4,
-         (4,8): 0.89, 4, 1, 4, 3, 2, 1,
+         (4,8): 0.89,
          (5,0): 11, 439.151, 2.152e-12, 3.595, 2.024, 0.63, 0.0182, 9.06,
-         (5,8): 0.52, 6, 4, 3, 5, 5, 0,
-         (6,0): 11, 443.018, 4.494e-13, 5.048, 1.568, 0.6, 0, 7.96, 0.5, 7,
-         (6,10): 5, 2, 6, 6, 1,
+         (5,8): 0.52,
+         (6,0): 11, 443.018, 4.494e-13, 5.048, 1.568, 0.6, 0, 7.96, 0.5,
          (7,0): 11, 448.001, 2.586e-11, 1.405, 2.587, 0.66, -0.0464, 13.01,
-         (7,8): 0.67, 4, 2, 3, 3, 3, 0,
+         (7,8): 0.67,
          (8,0): 11, 470.889, 8.253e-13, 3.597, 2.153, 0.66, 0.024, 9.7, 0.65,
-         (8,9): 6, 4, 2, 5, 5, 1,
          (9,0): 11, 474.689, 3.274e-12, 2.379, 2.34, 0.65, -0.019, 11.24,
-         (9,8): 0.64, 5, 3, 3, 4, 4, 0,
+         (9,8): 0.64,
          (10,0): 11, 488.49, 6.721e-13, 2.852, 2.61, 0.69, 0.069, 13.58,
-         (10,8): 0.72, 6, 2, 4, 7, 1, 7,
+         (10,8): 0.72,
          (11,0): 11, 556.936, 1.561e-09, 0.159, 3.115, 0.69, 0.06, 14.24, 1,
-         (11,9): 1, 1, 0, 1, 0, 1,
          (12,0): 11, 620.701, 1.704e-11, 2.391, 2.468, 0.75, 0, 11.94, 0.68,
-         (12,9): 5, 3, 2, 4, 4, 1,
          (13,0): 11, 752.033, 1.029e-09, 0.396, 3.114, 0.68, 0.052, 13.58,
-         (13,8): 0.84, 2, 1, 1, 2, 0, 2,
+         (13,8): 0.84,
          (14,0): 11, 916.172, 4.266e-11, 1.441, 2.698, 0.72, -0.0208, 13.91,
-         (14,8): 0.78, 4, 2, 2, 3, 3, 1
+         (14,8): 0.78
          }
          ATTRIBUTE "DIMENSION_LIST" {
             DATATYPE  H5T_VLEN { H5T_REFERENCE { H5T_STD_REF_OBJECT }}
             DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
             DATA {
             (0): (DATASET 17878 "/R17/rows"), (DATASET 18202 "/R17/cols")
             }
@@ -1292,45 +1282,45 @@
          }
       }
       DATASET "mtx" {
          DATATYPE  H5T_IEEE_F64LE
          DATASPACE  SIMPLE { ( 16, 16 ) / ( 16, 16 ) }
          DATA {
          (0,0): 11, 22.2351, 1.335e-14, 2.172, 2.74, 0.76, 13.63, 1.2,
-         (0,8): -0.033, 2.6, 0.814, 1.2, 0, 0, nan, nan,
+         (0,8): -0.033, 2.6, 0.814, 1.2, 0, 0, 0, 0,
          (1,0): 11, 183.31, 2.319e-12, 0.677, 3.028, 0.55, 15.01, 0.79,
          (1,8): -0.073, 2, 0.112, 1.43, 0, 18.3, 0.406, 1.499,
          (2,0): 11, 321.226, 7.657e-14, 6.262, 2.426, 0.73, 10.65, 0.54,
-         (2,8): -0.143, 0.73, 0.278, 0.54, 0, 0, nan, nan,
+         (2,8): -0.143, 0.73, 0.278, 0.54, 0, 0, 0, 0,
          (3,0): 11, 325.153, 2.721e-12, 1.561, 2.847, 0.64, 13.95, 0.74,
-         (3,8): -0.013, 0.64, 1.325, 0.74, 0, 0, nan, nan,
+         (3,8): -0.013, 0.64, 1.325, 0.74, 0, 0, 0, 0,
          (4,0): 11, 380.197, 2.477e-11, 1.062, 2.868, 0.54, 14.4, 0.89,
-         (4,8): -0.074, 0.54, 0.24, 0.89, 0, 0, nan, nan,
+         (4,8): -0.074, 0.54, 0.24, 0.89, 0, 0, 0, 0,
          (5,0): 11, 439.151, 2.137e-12, 3.643, 2.055, 0.69, 9.06, 0.52,
-         (5,8): 0.051, 0.69, 0.165, 0.52, 0, 0, nan, nan,
+         (5,8): 0.051, 0.69, 0.165, 0.52, 0, 0, 0, 0,
          (6,0): 11, 443.018, 4.44e-13, 5.116, 1.819, 0.7, 7.96, 0.5, 0.14,
-         (6,9): 0.7, -0.229, 0.5, 0, 0, nan, nan,
+         (6,9): 0.7, -0.229, 0.5, 0, 0, 0, 0,
          (7,0): 11, 448.001, 2.588e-11, 1.424, 2.612, 0.7, 13.01, 0.67,
-         (7,8): -0.116, 0.7, -0.615, 0.67, 0, 0, nan, nan,
+         (7,8): -0.116, 0.7, -0.615, 0.67, 0, 0, 0, 0,
          (8,0): 11, 470.889, 8.196e-13, 3.645, 2.169, 0.73, 9.7, 0.65, 0.061,
-         (8,9): 0.73, -0.465, 0.65, 0, 0, nan, nan,
+         (8,9): 0.73, -0.465, 0.65, 0, 0, 0, 0,
          (9,0): 11, 474.689, 3.268e-12, 2.411, 2.366, 0.71, 11.24, 0.64,
-         (9,8): -0.027, 0.71, -0.72, 0.64, 0, 0, nan, nan,
+         (9,8): -0.027, 0.71, -0.72, 0.64, 0, 0, 0, 0,
          (10,0): 11, 488.49, 6.628e-13, 2.89, 2.616, 0.75, 13.58, 0.72,
-         (10,8): -0.065, 0.75, -0.36, 0.72, 0, 0, nan, nan,
+         (10,8): -0.065, 0.75, -0.36, 0.72, 0, 0, 0, 0,
          (11,0): 11, 556.936, 1.57e-09, 0.161, 3.115, 0.75, 14.24, 1, 0.187,
-         (11,9): 0.75, -1.693, 1, 0, 0, nan, nan,
+         (11,9): 0.75, -1.693, 1, 0, 0, 0, 0,
          (12,0): 11, 620.701, 1.7e-11, 2.423, 2.468, 0.79, 11.94, 0.75, 0,
-         (12,9): 0.79, 0.687, 0.92, 0, 0, nan, nan,
+         (12,9): 0.79, 0.687, 0.92, 0, 0, 0, 0,
          (13,0): 11, 658.006, 9.033e-13, 7.921, 3.154, 0.73, 13.84, 1, 0.176,
-         (13,9): 0.73, -1.496, 1, 0, 0, nan, nan,
+         (13,9): 0.73, -1.496, 1, 0, 0, 0, 0,
          (14,0): 11, 752.033, 1.035e-09, 0.402, 3.114, 0.77, 13.58, 0.84,
-         (14,8): 0.162, 0.77, -0.878, 0.84, 0, 0, nan, nan,
+         (14,8): 0.162, 0.77, -0.878, 0.84, 0, 0, 0, 0,
          (15,0): 11, 916.172, 4.275e-11, 1.461, 2.695, 0.79, 13.55, 0.48, 0,
-         (15,9): 0.79, 0.521, 0.47, 0, 0, nan, nan
+         (15,9): 0.79, 0.521, 0.47, 0, 0, 0, 0
          }
          ATTRIBUTE "DIMENSION_LIST" {
             DATATYPE  H5T_VLEN { H5T_REFERENCE { H5T_STD_REF_OBJECT }}
             DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
             DATA {
             (0): (DATASET 32292 "/R19SD/rows"), (DATASET 32616 "/R19SD/cols")
             }
@@ -1780,41 +1770,41 @@
          DATASPACE  SIMPLE { ( 16, 16 ) / ( 16, 16 ) }
          DATA {
          (0,0): 11, 22.2351, 1.335e-14, 2.172, 2.74, 0.76, 13.63, 1.2,
          (0,8): -0.033, 2.6, 0.814, 1.2, 0, 0, 0.435, 1.91,
          (1,0): 11, 183.31, 2.319e-12, 0.677, 3.033, 0.62, 15.01, 0.82,
          (1,8): -0.074, 1.8, 0.136, 0.98, 0, 12.6, 0.413, 1.48,
          (2,0): 11, 321.226, 7.657e-14, 6.262, 2.426, 0.73, 10.65, 0.54,
-         (2,8): -0.143, 0.73, 0.278, 0.54, 0, 0, nan, nan,
+         (2,8): -0.143, 0.73, 0.278, 0.54, 0, 0, 0, 0,
          (3,0): 11, 325.153, 2.721e-12, 1.561, 2.847, 0.64, 13.95, 0.74,
-         (3,8): -0.013, 0.64, 1.325, 0.74, 0, 0, nan, nan,
+         (3,8): -0.013, 0.64, 1.325, 0.74, 0, 0, 0, 0,
          (4,0): 11, 380.197, 2.477e-11, 1.062, 2.868, 0.54, 14.4, 0.89,
-         (4,8): -0.074, 0.54, 0.24, 0.89, 0, 0, nan, nan,
+         (4,8): -0.074, 0.54, 0.24, 0.89, 0, 0, 0, 0,
          (5,0): 11, 439.151, 2.137e-12, 3.643, 2.055, 0.69, 9.06, 0.52,
-         (5,8): 0.051, 0.69, 0.165, 0.52, 0, 0, nan, nan,
+         (5,8): 0.051, 0.69, 0.165, 0.52, 0, 0, 0, 0,
          (6,0): 11, 443.018, 4.44e-13, 5.116, 1.819, 0.7, 7.96, 0.5, 0.14,
-         (6,9): 0.7, -0.229, 0.5, 0, 0, nan, nan,
+         (6,9): 0.7, -0.229, 0.5, 0, 0, 0, 0,
          (7,0): 11, 448.001, 2.588e-11, 1.424, 2.612, 0.7, 13.01, 0.67,
-         (7,8): -0.116, 0.7, -0.615, 0.67, 0, 0, nan, nan,
+         (7,8): -0.116, 0.7, -0.615, 0.67, 0, 0, 0, 0,
          (8,0): 11, 470.889, 8.196e-13, 3.645, 2.169, 0.73, 9.7, 0.65, 0.061,
-         (8,9): 0.73, -0.465, 0.65, 0, 0, nan, nan,
+         (8,9): 0.73, -0.465, 0.65, 0, 0, 0, 0,
          (9,0): 11, 474.689, 3.268e-12, 2.411, 2.366, 0.71, 11.24, 0.64,
-         (9,8): -0.027, 0.71, -0.72, 0.64, 0, 0, nan, nan,
+         (9,8): -0.027, 0.71, -0.72, 0.64, 0, 0, 0, 0,
          (10,0): 11, 488.49, 6.628e-13, 2.89, 2.616, 0.75, 13.58, 0.72,
-         (10,8): -0.065, 0.75, -0.36, 0.72, 0, 0, nan, nan,
+         (10,8): -0.065, 0.75, -0.36, 0.72, 0, 0, 0, 0,
          (11,0): 11, 556.936, 1.57e-09, 0.161, 3.115, 0.75, 14.24, 1, 0.187,
-         (11,9): 0.75, -1.693, 1, 0, 0, nan, nan,
+         (11,9): 0.75, -1.693, 1, 0, 0, 0, 0,
          (12,0): 11, 620.701, 1.7e-11, 2.423, 2.468, 0.79, 11.94, 0.75, 0,
-         (12,9): 0.79, 0.687, 0.92, 0, 0, nan, nan,
+         (12,9): 0.79, 0.687, 0.92, 0, 0, 0, 0,
          (13,0): 11, 658.006, 9.033e-13, 7.921, 3.154, 0.73, 13.84, 1, 0.176,
-         (13,9): 0.73, -1.496, 1, 0, 0, nan, nan,
+         (13,9): 0.73, -1.496, 1, 0, 0, 0, 0,
          (14,0): 11, 752.033, 1.035e-09, 0.402, 3.114, 0.77, 13.58, 0.84,
-         (14,8): 0.162, 0.77, -0.878, 0.84, 0, 0, nan, nan,
+         (14,8): 0.162, 0.77, -0.878, 0.84, 0, 0, 0, 0,
          (15,0): 11, 916.172, 4.275e-11, 1.461, 2.695, 0.79, 13.55, 0.48, 0,
-         (15,9): 0.79, 0.521, 0.47, 0, 0, nan, nan
+         (15,9): 0.79, 0.521, 0.47, 0, 0, 0, 0
          }
          ATTRIBUTE "DIMENSION_LIST" {
             DATATYPE  H5T_VLEN { H5T_REFERENCE { H5T_STD_REF_OBJECT }}
             DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
             DATA {
             (0): (DATASET 43164 "/R20SD/rows"), (DATASET 43488 "/R20SD/cols")
             }
@@ -1921,15 +1911,15 @@
             DATATYPE  H5T_COMPOUND {
                H5T_REFERENCE { H5T_STD_REF_OBJECT } "dataset";
                H5T_STD_U32LE "dimension";
             }
             DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
             DATA {
             (0): {
-                  DATASET 49260 "/R21SD/mtx",
+                  DATASET 50018 "/R21SD/mtx",
                   1
                }
             }
          }
          ATTRIBUTE "_Netcdf4Dimid" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
@@ -1944,15 +1934,15 @@
          DATA {
          (0): 300, 5.919e-10, 3, 1.416e-08, 7.5
          }
          ATTRIBUTE "DIMENSION_LIST" {
             DATATYPE  H5T_VLEN { H5T_REFERENCE { H5T_STD_REF_OBJECT }}
             DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
             DATA {
-            (0): (DATASET 48936 "/R21SD/ctrdim")
+            (0): (DATASET 49694 "/R21SD/ctrdim")
             }
          }
          ATTRIBUTE "_Netcdf4Coordinates" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
             DATA {
             (0): 29
@@ -1993,15 +1983,15 @@
             DATATYPE  H5T_COMPOUND {
                H5T_REFERENCE { H5T_STD_REF_OBJECT } "dataset";
                H5T_STD_U32LE "dimension";
             }
             DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
             DATA {
             (0): {
-                  DATASET 52443 "/R21SD/ctr",
+                  DATASET 53055 "/R21SD/ctr",
                   0
                }
             }
          }
          ATTRIBUTE "_Netcdf4Dimid" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
@@ -2048,15 +2038,15 @@
          (15,0): 11, 916.172, 4.275e-11, 1.461, 2.695, 0.79, 13.55, 0.48, 0,
          (15,9): 0, 0.521, 0.47, 0, 0, 0, 0, 0, 0, 0, 0
          }
          ATTRIBUTE "DIMENSION_LIST" {
             DATATYPE  H5T_VLEN { H5T_REFERENCE { H5T_STD_REF_OBJECT }}
             DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
             DATA {
-            (0): (DATASET 46171 "/R21SD/rows"), (DATASET 46495 "/R21SD/cols")
+            (0): (DATASET 49046 "/R21SD/rows"), (DATASET 49370 "/R21SD/cols")
             }
          }
          ATTRIBUTE "_Netcdf4Coordinates" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
             DATA {
             (0): 27, 28
@@ -2104,15 +2094,15 @@
             DATATYPE  H5T_COMPOUND {
                H5T_REFERENCE { H5T_STD_REF_OBJECT } "dataset";
                H5T_STD_U32LE "dimension";
             }
             DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
             DATA {
             (0): {
-                  DATASET 49260 "/R21SD/mtx",
+                  DATASET 50018 "/R21SD/mtx",
                   0
                }
             }
          }
          ATTRIBUTE "_Netcdf4Dimid" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
@@ -2157,15 +2147,15 @@
             DATATYPE  H5T_COMPOUND {
                H5T_REFERENCE { H5T_STD_REF_OBJECT } "dataset";
                H5T_STD_U32LE "dimension";
             }
             DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
             DATA {
             (0): {
-                  DATASET 54512 "/R22SD/mtx",
+                  DATASET 55124 "/R22SD/mtx",
                   1
                }
             }
          }
          ATTRIBUTE "_Netcdf4Dimid" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
@@ -2180,15 +2170,15 @@
          DATA {
          (0): 300, 5.919e-10, 3, 1.416e-08, 7.5
          }
          ATTRIBUTE "DIMENSION_LIST" {
             DATATYPE  H5T_VLEN { H5T_REFERENCE { H5T_STD_REF_OBJECT }}
             DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
             DATA {
-            (0): (DATASET 54188 "/R22SD/ctrdim")
+            (0): (DATASET 54800 "/R22SD/ctrdim")
             }
          }
          ATTRIBUTE "_Netcdf4Coordinates" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
             DATA {
             (0): 32
@@ -2229,30 +2219,30 @@
             DATATYPE  H5T_COMPOUND {
                H5T_REFERENCE { H5T_STD_REF_OBJECT } "dataset";
                H5T_STD_U32LE "dimension";
             }
             DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
             DATA {
             (0): {
-                  DATASET 58175 "/R22SD/ctr",
+                  DATASET 58947 "/R22SD/ctr",
                   0
                }
             }
          }
          ATTRIBUTE "_Netcdf4Dimid" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
             DATA {
             (0): 32
             }
          }
       }
       DATASET "mtx" {
          DATATYPE  H5T_IEEE_F64LE
-         DATASPACE  SIMPLE { ( 19, 20 ) / ( 19, 20 ) }
+         DATASPACE  SIMPLE { ( 20, 20 ) / ( 20, 20 ) }
          DATA {
          (0,0): 11, 22.2351, 1.334e-14, 2.172, 2.74, 0.76, 13.63, 1.2,
          (0,8): -0.033, 2.6, 0.814, 0, 0, 0, 0.435, 0, 1.91, 0, 0, 0,
          (1,0): 11, 183.31, 2.319e-12, 0.677, 3.033, 0.62, 15.01, 0.82,
          (1,8): -0.074, 1.8, 0.136, 0.98, 0, 12.6, 0.407, 0.412, 1.46, 0.571,
          (1,18): -0.016, 0.16,
          (2,0): 11, 321.226, 7.654e-14, 6.262, 2.426, 0.73, 10.65, 0.54,
@@ -2284,21 +2274,23 @@
          (15,0): 11, 859.966, 5.705e-13, 8.163, 3.121, 0.76, 14.08, 0.76,
          (15,8): 0.005, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
          (16,0): 11, 916.172, 4.272e-11, 1.461, 2.695, 0.79, 13.55, 0.48,
          (16,8): -0.001, 0, 0.521, 0.47, 0, 0, 0, 0, 0, 0, 0, 0,
          (17,0): 11, 970.315, 4.806e-11, 1.944, 2.574, 0.7, 25.95, 0.7,
          (17,8): -0.003, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
          (18,0): 11, 987.927, 7.528e-10, 0.261, 2.976, 0.75, 14.35, 0.75,
-         (18,8): -0.002, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
+         (18,8): -0.002, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+         (19,0): 11, 1097.36, 4.89e-09, 0.754, 3.095, 0.75, 15.27, 0.75,
+         (19,8): 0.002, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
          }
          ATTRIBUTE "DIMENSION_LIST" {
             DATATYPE  H5T_VLEN { H5T_REFERENCE { H5T_STD_REF_OBJECT }}
             DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
             DATA {
-            (0): (DATASET 53540 "/R22SD/rows"), (DATASET 53864 "/R22SD/cols")
+            (0): (DATASET 54152 "/R22SD/rows"), (DATASET 54476 "/R22SD/cols")
             }
          }
          ATTRIBUTE "_Netcdf4Coordinates" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
             DATA {
             (0): 30, 31
@@ -2310,17 +2302,17 @@
          DATASPACE  SCALAR
          DATA {
          (0): 296
          }
       }
       DATASET "rows" {
          DATATYPE  H5T_IEEE_F32BE
-         DATASPACE  SIMPLE { ( 19 ) / ( 19 ) }
+         DATASPACE  SIMPLE { ( 20 ) / ( 20 ) }
          DATA {
-         (0): 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
+         (0): 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
          }
          ATTRIBUTE "CLASS" {
             DATATYPE  H5T_STRING {
                STRSIZE 16;
                STRPAD H5T_STR_NULLTERM;
                CSET H5T_CSET_ASCII;
                CTYPE H5T_C_S1;
@@ -2335,26 +2327,26 @@
                STRSIZE 64;
                STRPAD H5T_STR_NULLTERM;
                CSET H5T_CSET_ASCII;
                CTYPE H5T_C_S1;
             }
             DATASPACE  SCALAR
             DATA {
-            (0): "This is a netCDF dimension but not a netCDF variable.        19"
+            (0): "This is a netCDF dimension but not a netCDF variable.        20"
             }
          }
          ATTRIBUTE "REFERENCE_LIST" {
             DATATYPE  H5T_COMPOUND {
                H5T_REFERENCE { H5T_STD_REF_OBJECT } "dataset";
                H5T_STD_U32LE "dimension";
             }
             DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
             DATA {
             (0): {
-                  DATASET 54512 "/R22SD/mtx",
+                  DATASET 55124 "/R22SD/mtx",
                   0
                }
             }
          }
          ATTRIBUTE "_Netcdf4Dimid" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
```

### Comparing `pyrtlib-1.0.6/pyrtlib/_lineshape/h2oll.py` & `pyrtlib-1.0.7/pyrtlib/_lineshape/h2oll.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,22 +62,22 @@
 s1 = mtx[:, 2]
 b2 = mtx[:, 3]
 w0 = mtx[:, 4] / 1000.0
 x = mtx[:, 5]
 w0s = mtx[:, 6] / 1000.0
 xs = mtx[:, 7]
 if H2OAbsModel.model == 'R03':
-    w0s = mtx[:, 6] / 1000.0
-    xs = mtx[:, 7]
-    sr = mtx[:, 8]
+    w0s = mtx[:, 7] / 1000.0
+    xs = mtx[:, 8]
+    sr = mtx[:, 6]
 elif H2OAbsModel.model in ['R16', 'R17']:
     sr = mtx[:, 6]
     w0s = mtx[:, 7] / 1000.0
     xs = mtx[:, 8]
-if H2OAbsModel.model not in ['R98', 'R03']:
+if H2OAbsModel.model not in ['R98', 'R03', 'R16', 'R17']:
     sh = mtx[:, 8] / 1000.0
     xh = mtx[:, 9]
     shs = mtx[:, 10] / 1000.0
     xhs = mtx[:, 11]
 if H2OAbsModel.model in ['R19', 'R19SD', 'R20', 'R20SD', 'R21SD', 'R22SD']:
     aair = mtx[:, 12]
     aself = mtx[:, 13]
```

### Comparing `pyrtlib-1.0.6/pyrtlib/_lineshape/o2_lineshape.nc` & `pyrtlib-1.0.7/pyrtlib/_lineshape/o2_lineshape.nc`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/_lineshape/o2ll.py` & `pyrtlib-1.0.7/pyrtlib/_lineshape/o2ll.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/_lineshape/o3_lineshape.nc` & `pyrtlib-1.0.7/pyrtlib/_lineshape/o3_lineshape.nc`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/_lineshape/o3ll.py` & `pyrtlib-1.0.7/pyrtlib/_lineshape/o3ll.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/absorption_model.py` & `pyrtlib-1.0.7/pyrtlib/absorption_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,17 +487,17 @@
                 for j in range(0, 2):
                     if np.abs(df[j]) < 750.0:
                         res += width / (df[j] ** 2 + wsq) - base
                 summ += s * res * (f / self.h2oll.fl[i]) ** 2
         # separate the following original equ. into line and continuum
         # terms, and change the units from np/km to ppm
         # abh2o = .3183e-4*den*sum + con
-        if H2OAbsModel == 'R22SD':
-            npp = (1.e-10 * rho * summ / (np.pi * gas_mass(atmp.H2O)
-                   * 1000) / db2np) / factor
+        if H2OAbsModel.model == 'R22SD':
+            h20m = 2.9915075E-23 # mass of water molecule (g)
+            npp = (1.e-10 * rho * summ / (np.pi * h20m) / db2np) / factor
         else:
             npp = (3.1831e-05 * den * summ / db2np) / factor
 
         ncpp = (con / db2np) / factor
 
         return npp, ncpp
```

### Comparing `pyrtlib-1.0.6/pyrtlib/apiwebservices/eps_sandbox.py` & `pyrtlib-1.0.7/pyrtlib/apiwebservices/eps_sandbox.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/apiwebservices/erafive.py` & `pyrtlib-1.0.7/pyrtlib/apiwebservices/erafive.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/apiwebservices/igra2.py` & `pyrtlib-1.0.7/pyrtlib/apiwebservices/igra2.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/apiwebservices/webservices.py` & `pyrtlib-1.0.7/pyrtlib/apiwebservices/webservices.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/apiwebservices/wyomingupperair.py` & `pyrtlib-1.0.7/pyrtlib/apiwebservices/wyomingupperair.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/climatology/atmospheric_profiles.py` & `pyrtlib-1.0.7/pyrtlib/climatology/atmospheric_profiles.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/climatology/extrapolation.py` & `pyrtlib-1.0.7/pyrtlib/climatology/extrapolation.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/climatology/gas_minor.dat` & `pyrtlib-1.0.7/pyrtlib/climatology/gas_minor.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/climatology/gas_trace.dat` & `pyrtlib-1.0.7/pyrtlib/climatology/gas_trace.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/climatology/midlatitude_summer.dat` & `pyrtlib-1.0.7/pyrtlib/climatology/midlatitude_summer.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/climatology/midlatitude_winter.dat` & `pyrtlib-1.0.7/pyrtlib/climatology/midlatitude_winter.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/climatology/subarctic_summer.dat` & `pyrtlib-1.0.7/pyrtlib/climatology/subarctic_summer.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/climatology/subarctic_winter.dat` & `pyrtlib-1.0.7/pyrtlib/climatology/subarctic_winter.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/climatology/tropical.dat` & `pyrtlib-1.0.7/pyrtlib/climatology/tropical.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/climatology/us_standard.dat` & `pyrtlib-1.0.7/pyrtlib/climatology/us_standard.dat`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/rt_equation.py` & `pyrtlib-1.0.7/pyrtlib/rt_equation.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,15 @@
                 return
 
         # If angle is close to 90 degrees, make ds a height difference profile.
         if (angle >= 89 and angle <= 91) or (angle >= -91 and angle <= -89):
             ds[0] = 0.0
             for i in range(1, nl):
                 ds[i] = z[i] - z[i - 1]
+            return ds
 
         # The rest of the subroutine applies only to angle other than 90 degrees.
         # Convert angle degrees to radians.  Initialize constant values.
         theta0 = np.dot(angle, deg2rad)
         rs = re + z[0] + z0
         costh0 = np.cos(theta0)
         sina = np.sin(np.dot(theta0, 0.5))
```

### Comparing `pyrtlib-1.0.6/pyrtlib/tb_spectrum.py` & `pyrtlib-1.0.7/pyrtlib/tb_spectrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,27 +345,27 @@
             for j in range(0, self.nf):
                 RTEquation._emissivity = self._es[j]
                 # Rosenkranz, personal communication, 2019/02/12 (email)
                 awet, adry = RTEquation.clearsky_absorption(self.p, self.tk, e, self.frq[j],
                                                             self.o3n, self.amu if self._uncertainty else None)
                 self.sptauwet[j, k], \
                     self.ptauwet[j, k, :] = RTEquation.exponential_integration(
-                        1, awet, ds, 0, self.nl, 1)
+                        True, awet, ds, 1, self.nl, 1)
                 self.sptaudry[j, k], \
                     self.ptaudry[j, k, :] = RTEquation.exponential_integration(
-                        1, adry, ds, 0, self.nl, 1)
+                        True, adry, ds, 1, self.nl, 1)
                 if self.cloudy:
                     aliq, aice = RTEquation.cloudy_absorption(
                         self.tk, self.denliq, self.denice, self.frq[j])
                     self.sptauliq[j, k], \
                         self.ptauliq[j, k, :] = RTEquation.exponential_integration(
-                            0, aliq, ds, 0, self.nl, 1)
+                            False, aliq, ds, 1, self.nl, 1)
                     self.sptauice[j, k], \
                         self.ptauice[j, k, :] = RTEquation.exponential_integration(
-                            0, aice, ds, 0, self.nl, 1)
+                            False, aice, ds, 1, self.nl, 1)
 
                 self.ptaulay[j, k, :] = self.ptauwet[j, k, :] + \
                     self.ptaudry[j, k, :] + \
                     self.ptauice[j, k, :] + \
                     self.ptauliq[j, k, :]
                 # [boftotl,boftatm,boftmr,PSPtauprof,hvk] = Planck_xxx(frq(j),tk,Ptaulay(j,k,:));
                 boftotl, boftatm, boftmr, psp_tauprof, hvk, _, _ = RTEquation.planck(self.frq[j], self.tk,
```

### Comparing `pyrtlib-1.0.6/pyrtlib/uncertainty/absmod_uncertainty.py` & `pyrtlib-1.0.7/pyrtlib/uncertainty/absmod_uncertainty.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2018_V1.1.nc` & `pyrtlib-1.0.7/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2018_V1.1.nc`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2019_V2.0.nc` & `pyrtlib-1.0.7/pyrtlib/uncertainty/covariance_matrix/R17/Cov_parameters_Cimini_et_al_2019_V2.0.nc`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/R19/Cov_parameters_Gallucci_et_al_ACPD_2023_V1.0.nc` & `pyrtlib-1.0.7/pyrtlib/uncertainty/covariance_matrix/R19/Cov_parameters_Gallucci_et_al_ACPD_2023_V1.0.nc`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/uncertainty/covariance_matrix/__init__.py` & `pyrtlib-1.0.7/pyrtlib/uncertainty/covariance_matrix/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/pyrtlib/utils.py` & `pyrtlib-1.0.7/pyrtlib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -905,16 +905,19 @@
                 56.660, 57.290, 58.800],
         'tem': [
             51.25, 51.75, 52.25, 52.85, 53.35, 53.85, 54.40, 54.90, 55.40,
             56.00, 56.50, 57.00
         ],
         'k2w': [23.8400, 31.4000, 72.5000, 82.5000, 90.0000, 150.000]
     }
-
-    return frequencies.get(instrument)
+    
+    try:
+        return np.array(frequencies[instrument.lower()])
+    except KeyError:
+        raise ValueError(f"Invalid instrument name. Available instruments are: {list(frequencies.keys())}")
 
 
 def to_kelvin(t: np.ndarray) -> np.ndarray:
     """Convert T from Celsius to Kelvin
 
     Args:
         t (numpy.ndarray): Temperature (°C)
@@ -964,14 +967,16 @@
     cf3 = 325.15
     cf4 = 448.00
     cf6 = 664.00
     cf118 = 118.7503
     cf165 = 165.5
     cf53 = 57.290344
     cf57 = 57.290344
+    
+    instrument = instrument.upper()
 
     if instrument == 'SAPHIR':
         freq = np.array([cf-11, cf-6.8, cf-4.2, cf-2.8, cf-1.1, cf-0.2,
                         cf+0.2, cf+1.1, cf+2.8, cf+4.2, cf+6.8, cf+11])
 
     elif instrument == 'AMSU':
         freq = np.array([89.0, 150.0, cf-7.0, cf-3.0, cf-1.0,
@@ -1000,9 +1005,11 @@
                         229])
     elif instrument == 'ICI':
         freq = np.array([cf-7.0, cf-3.4, cf-2.0, cf-0.2, cf+0.2, cf+2.0, cf+3.4, cf+7.0,
                         cf2-2.5, cf2+2.5,
                         cf3-9.5, cf3-3.5, cf3-1.5, cf3+1.5, cf3+3.5, cf3+9.5,
                         cf4-7.2, cf4-3.0, cf4-1.4, cf4+1.4, cf4+3.0, cf4+7.2,
                         cf6-4.2, cf6+4.2])
+    else:
+        raise ValueError("Instrument not found")
 
     return freq
```

### Comparing `pyrtlib-1.0.6/pyrtlib.egg-info/PKG-INFO` & `pyrtlib-1.0.7/pyrtlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtlib
-Version: 1.0.6
+Version: 1.0.7
 Summary: pyrtlib - Radiative Transfer library
 Author: slarosa
 Author-email: salvatore-larosa@cnr.it
 License: GPLv3
 Project-URL: Documentation, https://satclop.github.io/pyrtlib
 Project-URL: Repository, https://github.com/SatCloP/pyrtlib
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyrtlib-1.0.6/pyrtlib.egg-info/SOURCES.txt` & `pyrtlib-1.0.7/pyrtlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.6/setup.py` & `pyrtlib-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
 setup(
     name='pyrtlib',
-    version='1.0.6',
+    version='1.0.7',
     include_package_data=True,
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     package_data={'pyrtlib': ['_lineshape/*', 'climatology/*', 'uncertainty/covariance_matrix/*/*']},
     python_requires='>=3.8',
     install_requires=required,
     project_urls={
         'Documentation': 'https://satclop.github.io/pyrtlib',
```

