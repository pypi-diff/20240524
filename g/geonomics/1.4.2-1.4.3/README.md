# Comparing `tmp/geonomics-1.4.2.tar.gz` & `tmp/geonomics-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geonomics-1.4.2.tar", last modified: Wed May 22 02:03:54 2024, max compression
+gzip compressed data, was "geonomics-1.4.3.tar", last modified: Fri May 24 04:11:50 2024, max compression
```

## Comparing `geonomics-1.4.2.tar` & `geonomics-1.4.3.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.467279 geonomics-1.4.2/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     1112 2024-01-03 01:50:01.000000 geonomics-1.4.2/LICENSE.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)       74 2021-03-24 04:15:31.000000 geonomics-1.4.2/MANIFEST.in
--rw-rw-r--   0 deth      (1000) deth      (1000)     9507 2024-05-22 02:03:54.467279 geonomics-1.4.2/PKG-INFO
--rw-rw-r--   0 deth      (1000) deth      (1000)     8326 2022-01-01 18:34:30.000000 geonomics-1.4.2/README.rst
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.067278 geonomics-1.4.2/geonomics/
--rwxrwxr-x   0 deth      (1000) deth      (1000)      499 2022-01-01 17:50:26.000000 geonomics-1.4.2/geonomics/__init__.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.059278 geonomics-1.4.2/geonomics/data/
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.075278 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     1573 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/MMRR.R
--rwxrwxr-x   0 deth      (1000) deth      (1000)     2807 2023-06-14 19:20:14.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/MMRR.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.075278 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/__pycache__/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     3091 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc
--rwxrwxr-x   0 deth      (1000) deth      (1000)     3067 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc
--rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/env.csv
--rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/gen.csv
--rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/geo.csv
--rwxrwxr-x   0 deth      (1000) deth      (1000)      898 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/IBD_IBE_demo/run_mantel.R
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.075278 geonomics-1.4.2/geonomics/data/default_models/
--rw-rw-r--   0 deth      (1000) deth      (1000)    14817 2021-10-09 01:45:22.000000 geonomics-1.4.2/geonomics/data/default_models/selection_params.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.075278 geonomics-1.4.2/geonomics/data/yosemite_demo/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35632 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.083278 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.087278 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34429 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34424 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34399 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34379 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34604 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34326 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34361 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34407 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34382 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34292 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34435 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34351 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34256 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    34516 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    29050 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.095278 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35877 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36099 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35864 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35990 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35953 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35962 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36177 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35922 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35932 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35896 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36275 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36218 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36091 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36181 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    35874 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36217 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36109 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.155278 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31648 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31717 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31807 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31507 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31710 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31645 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31584 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31437 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31454 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31455 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31446 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31556 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31499 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31484 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31434 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31516 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31416 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    31225 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif
--rwxrwxr-x   0 deth      (1000) deth      (1000)    20497 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.287279 geonomics-1.4.2/geonomics/demos/
--rwxrwxr-x   0 deth      (1000) deth      (1000)    40012 2021-08-30 15:43:03.000000 geonomics-1.4.2/geonomics/demos/_IBD_IBE.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)       76 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/demos/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    23746 2021-08-30 20:54:50.000000 geonomics-1.4.2/geonomics/demos/_simult_select.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    40559 2021-08-30 20:54:24.000000 geonomics-1.4.2/geonomics/demos/_yosemite.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.287279 geonomics-1.4.2/geonomics/help/
--rwxrwxr-x   0 deth      (1000) deth      (1000)      728 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/help/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     2260 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/help/_memory_help.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    19956 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/help/_param_help.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    42853 2024-04-01 12:51:51.000000 geonomics-1.4.2/geonomics/main.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.335279 geonomics-1.4.2/geonomics/ops/
--rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/ops/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    36149 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/ops/change.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    11819 2024-05-21 23:43:48.000000 geonomics-1.4.2/geonomics/ops/demography.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    10192 2021-09-21 22:53:47.000000 geonomics-1.4.2/geonomics/ops/mating.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     6555 2021-03-24 04:15:27.000000 geonomics-1.4.2/geonomics/ops/movement.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     9065 2024-05-22 01:10:47.000000 geonomics-1.4.2/geonomics/ops/mutation.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     5094 2021-07-09 03:11:40.000000 geonomics-1.4.2/geonomics/ops/selection.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.379279 geonomics-1.4.2/geonomics/sim/
--rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/sim/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     3405 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/sim/burnin.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    23562 2022-12-26 20:26:33.000000 geonomics-1.4.2/geonomics/sim/data.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)   144014 2024-05-22 01:42:33.000000 geonomics-1.4.2/geonomics/sim/model.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    49072 2024-05-03 04:17:20.000000 geonomics-1.4.2/geonomics/sim/params.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    19972 2024-05-03 05:10:11.000000 geonomics-1.4.2/geonomics/sim/stats.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.467279 geonomics-1.4.2/geonomics/structs/
--rwxrwxr-x   0 deth      (1000) deth      (1000)      116 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/structs/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     5851 2024-04-30 00:00:02.000000 geonomics-1.4.2/geonomics/structs/community.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    88196 2024-04-29 23:24:41.000000 geonomics-1.4.2/geonomics/structs/genome.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)     8671 2024-05-21 23:17:26.000000 geonomics-1.4.2/geonomics/structs/individual.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    32867 2024-05-21 22:48:18.000000 geonomics-1.4.2/geonomics/structs/landscape.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)   153536 2024-05-22 00:59:51.000000 geonomics-1.4.2/geonomics/structs/species.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.467279 geonomics-1.4.2/geonomics/utils/
--rwxrwxr-x   0 deth      (1000) deth      (1000)       82 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/utils/__init__.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)      607 2021-03-24 04:15:28.000000 geonomics-1.4.2/geonomics/utils/_str_repr_.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    10991 2023-04-13 17:58:34.000000 geonomics-1.4.2/geonomics/utils/io.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    21410 2022-12-26 20:39:40.000000 geonomics-1.4.2/geonomics/utils/spatial.py
--rwxrwxr-x   0 deth      (1000) deth      (1000)    16746 2021-03-24 04:15:29.000000 geonomics-1.4.2/geonomics/utils/viz.py
--rw-rw-r--   0 deth      (1000) deth      (1000)       22 2024-05-22 01:46:45.000000 geonomics-1.4.2/geonomics/version.py
-drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-22 02:03:54.067278 geonomics-1.4.2/geonomics.egg-info/
--rwxrwxr-x   0 deth      (1000) deth      (1000)     9507 2024-05-22 02:03:52.000000 geonomics-1.4.2/geonomics.egg-info/PKG-INFO
--rwxrwxr-x   0 deth      (1000) deth      (1000)     5542 2024-05-22 02:03:53.000000 geonomics-1.4.2/geonomics.egg-info/SOURCES.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)        1 2024-05-22 02:03:53.000000 geonomics-1.4.2/geonomics.egg-info/dependency_links.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)       86 2024-05-22 02:03:53.000000 geonomics-1.4.2/geonomics.egg-info/requires.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)       10 2024-05-22 02:03:53.000000 geonomics-1.4.2/geonomics.egg-info/top_level.txt
--rwxrwxr-x   0 deth      (1000) deth      (1000)      107 2024-05-22 02:03:54.471279 geonomics-1.4.2/setup.cfg
--rwxrwxr-x   0 deth      (1000) deth      (1000)     2659 2024-05-08 01:39:40.000000 geonomics-1.4.2/setup.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.466626 geonomics-1.4.3/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     1112 2024-01-03 01:50:01.000000 geonomics-1.4.3/LICENSE.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       74 2021-03-24 04:15:31.000000 geonomics-1.4.3/MANIFEST.in
+-rw-rw-r--   0 deth      (1000) deth      (1000)     9507 2024-05-24 04:11:50.466626 geonomics-1.4.3/PKG-INFO
+-rw-rw-r--   0 deth      (1000) deth      (1000)     8326 2022-01-01 18:34:30.000000 geonomics-1.4.3/README.rst
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.418625 geonomics-1.4.3/geonomics/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      499 2022-01-01 17:50:26.000000 geonomics-1.4.3/geonomics/__init__.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.414626 geonomics-1.4.3/geonomics/data/
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.430626 geonomics-1.4.3/geonomics/data/IBD_IBE_demo/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     1573 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/IBD_IBE_demo/MMRR.R
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     2807 2023-06-14 19:20:14.000000 geonomics-1.4.3/geonomics/data/IBD_IBE_demo/MMRR.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.430626 geonomics-1.4.3/geonomics/data/IBD_IBE_demo/__pycache__/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     3091 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     3067 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc
+-rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/IBD_IBE_demo/env.csv
+-rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/IBD_IBE_demo/gen.csv
+-rwxrwxr-x   0 deth      (1000) deth      (1000)  1392400 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/IBD_IBE_demo/geo.csv
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      898 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/IBD_IBE_demo/run_mantel.R
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.430626 geonomics-1.4.3/geonomics/data/default_models/
+-rw-rw-r--   0 deth      (1000) deth      (1000)    14817 2021-10-09 01:45:22.000000 geonomics-1.4.3/geonomics/data/default_models/selection_params.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.430626 geonomics-1.4.3/geonomics/data/yosemite_demo/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35632 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.430626 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.438625 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34429 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34424 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34399 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34379 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34604 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34326 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34361 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34407 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34382 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34292 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34435 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34386 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34416 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34351 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34256 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    34516 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    29050 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.446626 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35877 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36099 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35864 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35990 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35953 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35962 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36177 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35922 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35932 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35896 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35910 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36275 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36218 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36091 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36181 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    35874 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36217 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36109 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.450626 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31648 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31717 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31807 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31507 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31710 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31645 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31584 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31437 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31454 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31455 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31446 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31556 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31499 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31484 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31434 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31516 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31416 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    31225 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    20497 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.450626 geonomics-1.4.3/geonomics/demos/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    40012 2021-08-30 15:43:03.000000 geonomics-1.4.3/geonomics/demos/_IBD_IBE.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       76 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/demos/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    23746 2021-08-30 20:54:50.000000 geonomics-1.4.3/geonomics/demos/_simult_select.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    40559 2021-08-30 20:54:24.000000 geonomics-1.4.3/geonomics/demos/_yosemite.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.454625 geonomics-1.4.3/geonomics/help/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      728 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/help/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     2260 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/help/_memory_help.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    19956 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/help/_param_help.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    42853 2024-04-01 12:51:51.000000 geonomics-1.4.3/geonomics/main.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.454625 geonomics-1.4.3/geonomics/ops/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/ops/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    36149 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/ops/change.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    11818 2024-05-23 02:45:39.000000 geonomics-1.4.3/geonomics/ops/demography.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    10192 2021-09-21 22:53:47.000000 geonomics-1.4.3/geonomics/ops/mating.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     6555 2021-03-24 04:15:27.000000 geonomics-1.4.3/geonomics/ops/movement.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     9065 2024-05-22 01:10:47.000000 geonomics-1.4.3/geonomics/ops/mutation.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     5094 2021-07-09 03:11:40.000000 geonomics-1.4.3/geonomics/ops/selection.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.458625 geonomics-1.4.3/geonomics/sim/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)        0 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/sim/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     3405 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/sim/burnin.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    23562 2022-12-26 20:26:33.000000 geonomics-1.4.3/geonomics/sim/data.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)   144086 2024-05-23 03:31:15.000000 geonomics-1.4.3/geonomics/sim/model.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    49072 2024-05-03 04:17:20.000000 geonomics-1.4.3/geonomics/sim/params.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    19972 2024-05-03 05:10:11.000000 geonomics-1.4.3/geonomics/sim/stats.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.462626 geonomics-1.4.3/geonomics/structs/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      116 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/structs/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     5851 2024-04-30 00:00:02.000000 geonomics-1.4.3/geonomics/structs/community.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    88196 2024-04-29 23:24:41.000000 geonomics-1.4.3/geonomics/structs/genome.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     8671 2024-05-21 23:17:26.000000 geonomics-1.4.3/geonomics/structs/individual.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    32867 2024-05-21 22:48:18.000000 geonomics-1.4.3/geonomics/structs/landscape.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)   154199 2024-05-24 02:28:19.000000 geonomics-1.4.3/geonomics/structs/species.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.466626 geonomics-1.4.3/geonomics/utils/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       82 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/utils/__init__.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      607 2021-03-24 04:15:28.000000 geonomics-1.4.3/geonomics/utils/_str_repr_.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    10991 2023-04-13 17:58:34.000000 geonomics-1.4.3/geonomics/utils/io.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    21410 2022-12-26 20:39:40.000000 geonomics-1.4.3/geonomics/utils/spatial.py
+-rwxrwxr-x   0 deth      (1000) deth      (1000)    16746 2021-03-24 04:15:29.000000 geonomics-1.4.3/geonomics/utils/viz.py
+-rw-rw-r--   0 deth      (1000) deth      (1000)       22 2024-05-24 04:08:25.000000 geonomics-1.4.3/geonomics/version.py
+drwxrwxr-x   0 deth      (1000) deth      (1000)        0 2024-05-24 04:11:50.418625 geonomics-1.4.3/geonomics.egg-info/
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     9507 2024-05-24 04:11:49.000000 geonomics-1.4.3/geonomics.egg-info/PKG-INFO
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     5542 2024-05-24 04:11:50.000000 geonomics-1.4.3/geonomics.egg-info/SOURCES.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)        1 2024-05-24 04:11:49.000000 geonomics-1.4.3/geonomics.egg-info/dependency_links.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       86 2024-05-24 04:11:50.000000 geonomics-1.4.3/geonomics.egg-info/requires.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)       10 2024-05-24 04:11:50.000000 geonomics-1.4.3/geonomics.egg-info/top_level.txt
+-rwxrwxr-x   0 deth      (1000) deth      (1000)      107 2024-05-24 04:11:50.466626 geonomics-1.4.3/setup.cfg
+-rwxrwxr-x   0 deth      (1000) deth      (1000)     2659 2024-05-08 01:39:40.000000 geonomics-1.4.3/setup.py
```

### Comparing `geonomics-1.4.2/LICENSE.txt` & `geonomics-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/PKG-INFO` & `geonomics-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: geonomics
-Version: 1.4.2
+Version: 1.4.3
 Summary: A package for landscape genomic simulation
 Home-page: https://github.com/drewhart/geonomics
-Download-URL: https://github.com/drewhart/geonomics/archive/1.4.2.tar.gz
+Download-URL: https://github.com/drewhart/geonomics/archive/1.4.3.tar.gz
 Author: Drew Ellison Hart
 Author-email: drew.ellison.hart@gmail.com
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/drewhart/geonomics/blob/master/doc/built/doc.html
 Project-URL: Methods Paper, https://doi.org/10.1093/molbev/msab175
 Project-URL: Source, https://github.com/drewhart/geonomics
 Keywords: landscape genomics genetics ecology evolution simulation model environmental model agent-based
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geonomics-1.4.2/README.rst` & `geonomics-1.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/MMRR.R` & `geonomics-1.4.3/geonomics/data/IBD_IBE_demo/MMRR.R`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/MMRR.py` & `geonomics-1.4.3/geonomics/data/IBD_IBE_demo/MMRR.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc` & `geonomics-1.4.3/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc` & `geonomics-1.4.3/geonomics/data/IBD_IBE_demo/__pycache__/MMRR.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/env.csv` & `geonomics-1.4.3/geonomics/data/IBD_IBE_demo/env.csv`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/gen.csv` & `geonomics-1.4.3/geonomics/data/IBD_IBE_demo/gen.csv`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/geo.csv` & `geonomics-1.4.3/geonomics/data/IBD_IBE_demo/geo.csv`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/IBD_IBE_demo/run_mantel.R` & `geonomics-1.4.3/geonomics/data/IBD_IBE_demo/run_mantel.R`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/default_models/selection_params.py` & `geonomics-1.4.3/geonomics/data/default_models/selection_params.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_DEM_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/509_ppt_2015_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/514_ppt_2020_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/519_ppt_2025_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/524_ppt_2030_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/529_ppt_2035_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/534_ppt_2040_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/539_ppt_2045_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/544_ppt_2050_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/549_ppt_2055_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/554_ppt_2060_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/559_ppt_2065_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/564_ppt_2070_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/569_ppt_2075_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/574_ppt_2080_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/579_ppt_2085_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/584_ppt_2090_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/589_ppt_2095_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt/594_ppt_2100_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/ppt_1980-2010_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/509_sdm_2015_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/514_sdm_2020_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/519_sdm_2025_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/524_sdm_2030_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/529_sdm_2035_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/534_sdm_2040_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/539_sdm_2045_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/544_sdm_2050_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/549_sdm_2055_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/554_sdm_2060_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/559_sdm_2065_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/564_sdm_2070_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/569_sdm_2075_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/574_sdm_2080_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/579_sdm_2085_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/584_sdm_2090_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/589_sdm_2095_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm/594_sdm_2100_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/sdm_1980-2010_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/509_tmp_2015_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/514_tmp_2020_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/519_tmp_2025_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/524_tmp_2030_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/529_tmp_2035_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/534_tmp_2040_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/539_tmp_2045_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/544_tmp_2050_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/549_tmp_2055_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/554_tmp_2060_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/559_tmp_2065_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/564_tmp_2070_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/569_tmp_2075_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/574_tmp_2080_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/579_tmp_2085_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/584_tmp_2090_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/589_tmp_2095_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp/594_tmp_2100_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif` & `geonomics-1.4.3/geonomics/data/yosemite_demo/yosemite_lyrs/tmp_1980-2010_90x90.tif`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/demos/_IBD_IBE.py` & `geonomics-1.4.3/geonomics/demos/_IBD_IBE.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/demos/_simult_select.py` & `geonomics-1.4.3/geonomics/demos/_simult_select.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/demos/_yosemite.py` & `geonomics-1.4.3/geonomics/demos/_yosemite.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/help/__init__.py` & `geonomics-1.4.3/geonomics/help/__init__.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/help/_memory_help.py` & `geonomics-1.4.3/geonomics/help/_memory_help.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/help/_param_help.py` & `geonomics-1.4.3/geonomics/help/_param_help.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/main.py` & `geonomics-1.4.3/geonomics/main.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/ops/change.py` & `geonomics-1.4.3/geonomics/ops/change.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/ops/demography.py` & `geonomics-1.4.3/geonomics/ops/demography.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     #in each cell) Calculate d as simply N_d/N, then control for some
     #numerical artefacts that an inappropriate
     # NOTE: ignore x/0. and 0./0. warnings
     with np.errstate(divide='ignore', invalid='ignore'):
         d = N_d/N
     #fix infinties and NaNs and negatives if they arise
     #(they occur where N ==0 or where N_d == 0)
-    d[np.isnan(d)] = 0 
+    d[np.isnan(d)] = 0
     #constrain to the min and max d values
     d = np.clip(a = d, a_min = d_min, a_max = d_max)
 
     #NOTE: DEH: 12-08-18: Got rid of the infinity check, because it was
     #coercing all infinities to 0, but in many cases infinities should actually
     #have been 1s, so it created numerous problems that just clipping to d_min
     #and d_max takes care of anyhow; commented out the NaN check below, but not
```

### Comparing `geonomics-1.4.2/geonomics/ops/mating.py` & `geonomics-1.4.3/geonomics/ops/mating.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/ops/movement.py` & `geonomics-1.4.3/geonomics/ops/movement.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/ops/mutation.py` & `geonomics-1.4.3/geonomics/ops/mutation.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/ops/selection.py` & `geonomics-1.4.3/geonomics/ops/selection.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/sim/burnin.py` & `geonomics-1.4.3/geonomics/sim/burnin.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/sim/data.py` & `geonomics-1.4.3/geonomics/sim/data.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/sim/model.py` & `geonomics-1.4.3/geonomics/sim/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 '''
 Defines the core Model class, as well as its public and private methods
 '''
 
 #geonomics imports
 from geonomics.structs.landscape import _make_landscape
 from geonomics.structs.community import _make_community
+from geonomics.structs.species import Species
 from geonomics.structs.genome import _make_genomic_architecture
 from geonomics.sim.data import (_DataCollector, _tskit_table_to_pandas,
                                 _get_adhoc_sample, _format_vcf, _format_fasta)
 
 from geonomics.sim.stats import _StatsCollector
 from geonomics.utils.io import (_write_csv, _write_shapefile, _write_geojson,
                                 _write_file)
@@ -3016,14 +3017,15 @@
         # get the desired species
         spp = self.comm[self._get_spp_num(spp)]
 
         # call that species' corresponding method
         spp._remove_individuals(individs=individs,
                                 n=n,
                                 n_left=n_left,
+                                verbose=True,
                                )
 
 
     def add_individuals(self,
                         n,
                         coords,
                         recip_spp=0,
@@ -3101,15 +3103,15 @@
         assert ((source_spp is not None and source_msprime_params is None) or
                 (source_spp is None and source_msprime_params is not None)), (
                         "Source population must be provided either as "
                         "a gnx Species object ('source_spp') "
                         "or as a set of valid args for gnx.run_msprime_sim() "
                         "('source_msprime_params'), but not both.")
         if source_spp is not None:
-            assert (isinstance(source_spp, gnx.structs.species.Species) or
+            assert (isinstance(source_spp, Species) or
                     isinstance(source_spp, int) or
                     isinstnace(source_spp, str)), ("The "
                         "value given to 'source_spp' identifies a gnx "
                         "Species object that will serve as the source "
                         "population, so must be either a gnx Species "
                         "instance (i.e., an object of the class "
                         "gnx.structs.species.Species) whose Individuals will "
```

### Comparing `geonomics-1.4.2/geonomics/sim/params.py` & `geonomics-1.4.3/geonomics/sim/params.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/sim/stats.py` & `geonomics-1.4.3/geonomics/sim/stats.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/structs/community.py` & `geonomics-1.4.3/geonomics/structs/community.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/structs/genome.py` & `geonomics-1.4.3/geonomics/structs/genome.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/structs/individual.py` & `geonomics-1.4.3/geonomics/structs/individual.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/structs/landscape.py` & `geonomics-1.4.3/geonomics/structs/landscape.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/structs/species.py` & `geonomics-1.4.3/geonomics/structs/species.py`

 * *Files 1% similar despite different names*

```diff
@@ -4456,5141 +4456,5183 @@
 00011670: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011680: 2020 2020 6b65 6570 5f73 6974 6573 5f74      keep_sites_t
 00011690: 6162 3d46 616c 7365 2c0a 2020 2020 2020  ab=False,.      
 000116a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000116b0: 2020 2020 2020 6368 6563 6b5f 6578 7469        check_exti
 000116c0: 6e63 743d 4661 6c73 652c 0a20 2020 2020  nct=False,.     
 000116d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116e0: 2020 2020 2020 293a 0a0a 2020 2020 2020        ):..      
-000116f0: 2020 2320 7661 6c69 6461 7465 2061 7267    # validate arg
-00011700: 730a 2020 2020 2020 2020 6173 7365 7274  s.        assert
-00011710: 2028 6e70 2e73 756d 285b 7020 6973 204e   (np.sum([p is N
-00011720: 6f6e 6520 666f 7220 7020 696e 205b 696e  one for p in [in
-00011730: 6469 7669 6473 2c20 6e2c 206e 5f6c 6566  divids, n, n_lef
-00011740: 745d 5d29 203d 3d20 3220 616e 640a 2020  t]]) == 2 and.  
-00011750: 2020 2020 2020 2020 2020 2020 2020 6e70                np
-00011760: 2e73 756d 285b 7020 6973 206e 6f74 204e  .sum([p is not N
-00011770: 6f6e 6520 666f 7220 7020 696e 205b 696e  one for p in [in
-00011780: 6469 7669 6473 2c20 6e2c 206e 5f6c 6566  divids, n, n_lef
-00011790: 745d 5d29 203d 3d20 3129 2c20 280a 2020  t]]) == 1), (.  
-000117a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117c0: 2020 224f 6e65 206f 6620 2769 6e64 6976    "One of 'indiv
-000117d0: 6964 7327 2c20 276e 272c 2061 6e64 2027  ids', 'n', and '
-000117e0: 6e5f 6c65 6674 2720 6d75 7374 220a 2020  n_left' must".  
-000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011810: 2020 2262 6520 7072 6f76 6964 6564 2c20    "be provided, 
-00011820: 7468 6520 6f74 6865 7220 7477 6f20 6d75  the other two mu
-00011830: 7374 2062 6520 4e6f 6e65 2e22 290a 2020  st be None.").  
-00011840: 2020 2020 2020 6966 2069 6e64 6976 6964        if individ
-00011850: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00011860: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00011870: 6420 696e 2069 6e64 6976 6964 733a 0a20  d in individs:. 
-00011880: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00011890: 7373 6572 7420 6964 2069 6e20 7365 6c66  ssert id in self
-000118a0: 2e6b 6579 7328 292c 2066 2249 6e64 6976  .keys(), f"Indiv
-000118b0: 6964 7561 6c20 7b69 647d 2064 6f65 7320  idual {id} does 
-000118c0: 6e6f 7420 6578 6973 742e 220a 2020 2020  not exist.".    
-000118d0: 2020 2020 6966 2069 6e64 6976 6964 7320      if individs 
-000118e0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-000118f0: 2020 2020 2069 6620 6e5f 6c65 6674 2069       if n_left i
-00011900: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00011910: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00011920: 7274 206e 5f6c 6566 7420 3e3d 2030 2061  rt n_left >= 0 a
-00011930: 6e64 206e 5f6c 6566 743c 3d20 6c65 6e28  nd n_left<= len(
-00011940: 7365 6c66 292c 2028 2227 6e5f 6c65 6674  self), ("'n_left
-00011950: 2720 6d75 7374 2062 6520 220a 2020 2020  ' must be ".    
-00011960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011980: 2020 2020 2020 2020 2020 2020 2261 206e              "a n
-00011990: 756d 6265 7220 6574 7765 656e 2030 2061  umber etween 0 a
-000119a0: 6e64 2022 0a20 2020 2020 2020 2020 2020  nd ".           
-000119b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119d0: 2020 2020 2022 7468 6520 6375 7272 656e       "the curren
-000119e0: 7420 7369 7a65 206f 6620 7468 6520 220a  t size of the ".
+000116e0: 2020 2020 2020 2076 6572 626f 7365 3d46         verbose=F
+000116f0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00011700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011710: 2029 3a0a 0a20 2020 2020 2020 2023 2076   ):..        # v
+00011720: 616c 6964 6174 6520 6172 6773 0a20 2020  alidate args.   
+00011730: 2020 2020 2061 7373 6572 7420 286e 702e       assert (np.
+00011740: 7375 6d28 5b70 2069 7320 4e6f 6e65 2066  sum([p is None f
+00011750: 6f72 2070 2069 6e20 5b69 6e64 6976 6964  or p in [individ
+00011760: 732c 206e 2c20 6e5f 6c65 6674 5d5d 2920  s, n, n_left]]) 
+00011770: 3d3d 2032 2061 6e64 0a20 2020 2020 2020  == 2 and.       
+00011780: 2020 2020 2020 2020 206e 702e 7375 6d28           np.sum(
+00011790: 5b70 2069 7320 6e6f 7420 4e6f 6e65 2066  [p is not None f
+000117a0: 6f72 2070 2069 6e20 5b69 6e64 6976 6964  or p in [individ
+000117b0: 732c 206e 2c20 6e5f 6c65 6674 5d5d 2920  s, n, n_left]]) 
+000117c0: 3d3d 2031 292c 2028 0a20 2020 2020 2020  == 1), (.       
+000117d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117e0: 2020 2020 2020 2020 2020 2020 2022 4f6e               "On
+000117f0: 6520 6f66 2027 696e 6469 7669 6473 272c  e of 'individs',
+00011800: 2027 6e27 2c20 616e 6420 276e 5f6c 6566   'n', and 'n_lef
+00011810: 7427 206d 7573 7422 0a20 2020 2020 2020  t' must".       
+00011820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011830: 2020 2020 2020 2020 2020 2020 2022 6265               "be
+00011840: 2070 726f 7669 6465 642c 2074 6865 206f   provided, the o
+00011850: 7468 6572 2074 776f 206d 7573 7420 6265  ther two must be
+00011860: 204e 6f6e 652e 2229 0a20 2020 2020 2020   None.").       
+00011870: 2069 6620 696e 6469 7669 6473 2069 7320   if individs is 
+00011880: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00011890: 2020 2020 2020 666f 7220 6964 2069 6e20        for id in 
+000118a0: 696e 6469 7669 6473 3a0a 2020 2020 2020  individs:.      
+000118b0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+000118c0: 2069 6420 696e 2073 656c 662e 6b65 7973   id in self.keys
+000118d0: 2829 2c20 6622 496e 6469 7669 6475 616c  (), f"Individual
+000118e0: 207b 6964 7d20 646f 6573 206e 6f74 2065   {id} does not e
+000118f0: 7869 7374 2e22 0a20 2020 2020 2020 2069  xist.".        i
+00011900: 6620 696e 6469 7669 6473 2069 7320 4e6f  f individs is No
+00011910: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00011920: 6966 206e 5f6c 6566 7420 6973 206e 6f74  if n_left is not
+00011930: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00011940: 2020 2020 2020 2061 7373 6572 7420 6e5f         assert n_
+00011950: 6c65 6674 203e 3d20 3020 616e 6420 6e5f  left >= 0 and n_
+00011960: 6c65 6674 3c3d 206c 656e 2873 656c 6629  left<= len(self)
+00011970: 2c20 2822 276e 5f6c 6566 7427 206d 7573  , ("'n_left' mus
+00011980: 7420 6265 2022 0a20 2020 2020 2020 2020  t be ".         
+00011990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119b0: 2020 2020 2020 2022 6120 6e75 6d62 6572         "a number
+000119c0: 2065 7477 6565 6e20 3020 616e 6420 220a   etween 0 and ".
+000119d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000119f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a20: 6622 706f 7075 6c61 7469 6f6e 2028 7b6c  f"population ({l
-00011a30: 656e 2873 656c 6629 7d29 2e22 290a 2020  en(self)}).").  
-00011a40: 2020 2020 2020 2020 2020 2020 2020 6e20                n 
-00011a50: 3d20 6c65 6e28 7365 6c66 2920 2d20 6e5f  = len(self) - n_
-00011a60: 6c65 6674 0a20 2020 2020 2020 2020 2020  left.           
-00011a70: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
-00011a80: 6365 286e 2c20 696e 7429 2061 6e64 206e  ce(n, int) and n
-00011a90: 203e 3d20 302c 2028 2227 6e27 206d 7573   >= 0, ("'n' mus
-00011aa0: 7420 6569 7468 6572 2062 6520 220a 2020  t either be ".  
-00011ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ae0: 2022 6120 6e6f 6e2d 6e65 6761 7469 7665   "a non-negative
-00011af0: 2069 6e74 2022 0a20 2020 2020 2020 2020   int ".         
-00011b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b20: 2020 2020 2020 2020 2020 226f 7220 4e6f            "or No
-00011b30: 6e65 2e22 290a 2020 2020 2020 2020 2020  ne.").          
-00011b40: 2020 6173 7365 7274 206e 203c 3d20 6c65    assert n <= le
-00011b50: 6e28 7365 6c66 292c 2028 2243 616e 6e6f  n(self), ("Canno
-00011b60: 7420 7265 6d6f 7665 206d 6f72 6520 496e  t remove more In
-00011b70: 6469 7669 6475 616c 7320 7468 616e 2022  dividuals than "
-00011b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ba0: 2020 2020 2263 7572 7265 6e74 6c79 2065      "currently e
-00011bb0: 7869 7374 2028 6375 7272 656e 7420 706f  xist (current po
-00011bc0: 7075 6c61 7469 6f6e 2073 697a 6520 220a  pulation size ".
-00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bf0: 2020 2066 2269 7320 7b6c 656e 2873 656c     f"is {len(sel
-00011c00: 6629 7d29 2e22 290a 0a20 2020 2020 2020  f)}).")..       
-00011c10: 2023 2064 7261 7720 7261 6e64 6f6d 2049   # draw random I
-00011c20: 6e64 6976 6964 7561 6c73 2c20 6966 206e  ndividuals, if n
-00011c30: 6563 6573 7361 7279 0a20 2020 2020 2020  ecessary.       
-00011c40: 2069 6620 696e 6469 7669 6473 2069 7320   if individs is 
-00011c50: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00011c60: 2020 6964 7320 3d20 5b2a 7365 6c66 5d0a    ids = [*self].
-00011c70: 2020 2020 2020 2020 2020 2020 696e 6469              indi
-00011c80: 7669 6473 203d 206e 702e 7261 6e64 6f6d  vids = np.random
-00011c90: 2e63 686f 6963 6528 6964 732c 206e 2c20  .choice(ids, n, 
-00011ca0: 7265 706c 6163 653d 4661 6c73 6529 0a0a  replace=False)..
-00011cb0: 2020 2020 2020 2020 2320 6765 7420 6e75          # get nu
-00011cc0: 6d62 6572 206f 6620 496e 6469 7669 6475  mber of Individu
-00011cd0: 616c 7320 6265 666f 7265 206f 7065 7261  als before opera
-00011ce0: 7469 6f6e 0a20 2020 2020 2020 204e 5f62  tion.        N_b
-00011cf0: 3420 3d20 6c65 6e28 7365 6c66 290a 0a20  4 = len(self).. 
-00011d00: 2020 2020 2020 2023 2072 656d 6f76 6520         # remove 
-00011d10: 7468 6520 496e 6469 7669 6475 616c 730a  the Individuals.
-00011d20: 2020 2020 2020 2020 666f 7220 6964 2069          for id i
-00011d30: 6e20 696e 6469 7669 6473 3a0a 2020 2020  n individs:.    
-00011d40: 2020 2020 2020 2020 676f 6f64 6279 6520          goodbye 
-00011d50: 3d20 7365 6c66 2e70 6f70 2869 6429 0a0a  = self.pop(id)..
-00011d60: 2020 2020 2020 2020 2320 6173 7365 7274          # assert
-00011d70: 2074 6861 7420 706f 7075 6c61 7469 6f6e   that population
-00011d80: 2073 697a 6520 6861 7320 6368 616e 6765   size has change
-00011d90: 6420 7468 6520 636f 7272 6563 7420 616d  d the correct am
-00011da0: 6f75 6e74 0a20 2020 2020 2020 204e 5f61  ount.        N_a
-00011db0: 6620 3d20 6c65 6e28 7365 6c66 290a 2020  f = len(self).  
-00011dc0: 2020 2020 2020 6173 7365 7274 2028 4e5f        assert (N_
-00011dd0: 6234 202d 204e 5f61 6629 203d 3d20 6c65  b4 - N_af) == le
-00011de0: 6e28 696e 6469 7669 6473 292c 2028 2249  n(individs), ("I
-00011df0: 6e63 6f72 7265 6374 206e 756d 6265 7220  ncorrect number 
-00011e00: 6f66 2022 0a20 2020 2020 2020 2020 2020  of ".           
-00011e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e30: 2020 2020 2022 496e 6469 7669 6475 6c73       "Individuls
-00011e40: 2072 656d 6f76 6564 2122 290a 0a20 2020   removed!")..   
-00011e50: 2020 2020 2023 2075 7064 6174 6520 7468       # update th
-00011e60: 6520 5461 626c 6543 6f6c 6c65 6374 696f  e TableCollectio
-00011e70: 6e2c 2069 6620 6e65 6365 7373 6172 790a  n, if necessary.
-00011e80: 2020 2020 2020 2020 2320 2862 7574 206b          # (but k
-00011e90: 6565 7020 616e 6420 636f 7079 2062 6163  eep and copy bac
-00011ea0: 6b20 696e 2074 6865 2073 6974 6573 2074  k in the sites t
-00011eb0: 6162 6c65 2c20 6966 206e 6563 6573 7361  able, if necessa
-00011ec0: 7279 2c0a 2020 2020 2020 2020 2320 652e  ry,.        # e.
-00011ed0: 672e 2c20 7768 656e 2069 6e69 7420 7061  g., when init pa
-00011ee0: 7261 6d73 2061 7265 2072 656d 6f76 696e  rams are removin
-00011ef0: 6720 616e 6420 7265 706c 6163 696e 6720  g and replacing 
-00011f00: 616c 6c20 676e 782d 7369 6d75 6c61 7465  all gnx-simulate
-00011f10: 640a 2020 2020 2020 2020 2320 496e 6469  d.        # Indi
-00011f20: 7669 6475 616c 7329 0a20 2020 2020 2020  viduals).       
-00011f30: 2069 6620 7365 6c66 2e67 656e 5f61 7263   if self.gen_arc
-00011f40: 682e 7573 655f 7473 6b69 743a 0a20 2020  h.use_tskit:.   
-00011f50: 2020 2020 2020 2020 2069 6620 6b65 6570           if keep
-00011f60: 5f73 6974 6573 5f74 6162 3a0a 2020 2020  _sites_tab:.    
-00011f70: 2020 2020 2020 2020 2020 2020 7369 7465              site
-00011f80: 735f 7461 6220 3d20 7365 6c66 2e5f 7463  s_tab = self._tc
-00011f90: 2e73 6974 6573 0a20 2020 2020 2020 2020  .sites.         
-00011fa0: 2020 2073 656c 662e 5f73 6f72 745f 616e     self._sort_an
-00011fb0: 645f 7369 6d70 6c69 6679 5f74 6162 6c65  d_simplify_table
-00011fc0: 5f63 6f6c 6c65 6374 696f 6e28 290a 2020  _collection().  
-00011fd0: 2020 2020 2020 2020 2020 6966 206b 6565            if kee
-00011fe0: 705f 7369 7465 735f 7461 623a 0a20 2020  p_sites_tab:.   
-00011ff0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00012000: 662e 5f74 632e 7369 7465 732e 7265 706c  f._tc.sites.repl
-00012010: 6163 655f 7769 7468 2873 6974 6573 5f74  ace_with(sites_t
-00012020: 6162 290a 0a20 2020 2020 2020 2023 2075  ab)..        # u
-00012030: 7064 6174 6520 7365 6c66 2e63 6f6f 7264  pdate self.coord
-00012040: 7320 616e 6420 7365 6c66 2e63 656c 6c73  s and self.cells
-00012050: 2061 7474 7269 6275 7465 730a 2020 2020   attributes.    
-00012060: 2020 2020 7365 6c66 2e5f 7365 745f 636f      self._set_co
-00012070: 6f72 6473 5f61 6e64 5f63 656c 6c73 2829  ords_and_cells()
-00012080: 0a0a 2020 2020 2020 2020 2320 616e 6420  ..        # and 
-00012090: 7570 6461 7465 2065 7874 696e 6374 2066  update extinct f
-000120a0: 6c61 670a 2020 2020 2020 2020 6966 2063  lag.        if c
-000120b0: 6865 636b 5f65 7874 696e 6374 3a0a 2020  heck_extinct:.  
-000120c0: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-000120d0: 7874 696e 6374 203d 2073 656c 662e 5f63  xtinct = self._c
-000120e0: 6865 636b 5f65 7874 696e 6374 2829 0a0a  heck_extinct()..
-000120f0: 2020 2020 2020 2020 2320 7072 696e 7420          # print 
-00012100: 696e 666f 726d 6174 6976 6520 6f75 7470  informative outp
-00012110: 7574 0a20 2020 2020 2020 2070 7269 6e74  ut.        print
-00012120: 2866 225c 6e7b 6c65 6e28 696e 6469 7669  (f"\n{len(indivi
-00012130: 6473 297d 2049 6e64 6976 6964 7561 6c73  ds)} Individuals
-00012140: 2073 7563 6365 7373 6675 6c6c 7920 7265   successfully re
-00012150: 6d6f 7665 642e 5c6e 2229 0a20 2020 2020  moved.\n").     
-00012160: 2020 2072 6574 7572 6e0a 0a0a 2020 2020     return...    
-00012170: 6465 6620 5f61 6464 5f69 6e64 6976 6964  def _add_individ
-00012180: 7561 6c73 2873 656c 662c 0a20 2020 2020  uals(self,.     
-00012190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121a0: 2020 2020 6e2c 0a20 2020 2020 2020 2020      n,.         
-000121b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121c0: 636f 6f72 6473 2c0a 2020 2020 2020 2020  coords,.        
+00011a00: 2274 6865 2063 7572 7265 6e74 2073 697a  "the current siz
+00011a10: 6520 6f66 2074 6865 2022 0a20 2020 2020  e of the ".     
+00011a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a40: 2020 2020 2020 2020 2020 2066 2270 6f70             f"pop
+00011a50: 756c 6174 696f 6e20 287b 6c65 6e28 7365  ulation ({len(se
+00011a60: 6c66 297d 292e 2229 0a20 2020 2020 2020  lf)}).").       
+00011a70: 2020 2020 2020 2020 206e 203d 206c 656e           n = len
+00011a80: 2873 656c 6629 202d 206e 5f6c 6566 740a  (self) - n_left.
+00011a90: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00011aa0: 7274 2069 7369 6e73 7461 6e63 6528 6e2c  rt isinstance(n,
+00011ab0: 2069 6e74 2920 616e 6420 6e20 3e3d 2030   int) and n >= 0
+00011ac0: 2c20 2822 276e 2720 6d75 7374 2065 6974  , ("'n' must eit
+00011ad0: 6865 7220 6265 2022 0a20 2020 2020 2020  her be ".       
+00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b00: 2020 2020 2020 2020 2020 2020 2261 206e              "a n
+00011b10: 6f6e 2d6e 6567 6174 6976 6520 696e 7420  on-negative int 
+00011b20: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b50: 2020 2020 2022 6f72 204e 6f6e 652e 2229       "or None.")
+00011b60: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00011b70: 6572 7420 6e20 3c3d 206c 656e 2873 656c  ert n <= len(sel
+00011b80: 6629 2c20 2822 4361 6e6e 6f74 2072 656d  f), ("Cannot rem
+00011b90: 6f76 6520 6d6f 7265 2049 6e64 6976 6964  ove more Individ
+00011ba0: 7561 6c73 2074 6861 6e20 220a 2020 2020  uals than ".    
+00011bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00011bd0: 6375 7272 656e 746c 7920 6578 6973 7420  currently exist 
+00011be0: 2863 7572 7265 6e74 2070 6f70 756c 6174  (current populat
+00011bf0: 696f 6e20 7369 7a65 2022 0a20 2020 2020  ion size ".     
+00011c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c10: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00011c20: 6973 207b 6c65 6e28 7365 6c66 297d 292e  is {len(self)}).
+00011c30: 2229 0a0a 2020 2020 2020 2020 2320 6472  ")..        # dr
+00011c40: 6177 2072 616e 646f 6d20 496e 6469 7669  aw random Indivi
+00011c50: 6475 616c 732c 2069 6620 6e65 6365 7373  duals, if necess
+00011c60: 6172 790a 2020 2020 2020 2020 6966 2069  ary.        if i
+00011c70: 6e64 6976 6964 7320 6973 204e 6f6e 653a  ndivids is None:
+00011c80: 0a20 2020 2020 2020 2020 2020 2069 6473  .            ids
+00011c90: 203d 205b 2a73 656c 665d 0a20 2020 2020   = [*self].     
+00011ca0: 2020 2020 2020 2069 6e64 6976 6964 7320         individs 
+00011cb0: 3d20 6e70 2e72 616e 646f 6d2e 6368 6f69  = np.random.choi
+00011cc0: 6365 2869 6473 2c20 6e2c 2072 6570 6c61  ce(ids, n, repla
+00011cd0: 6365 3d46 616c 7365 290a 0a20 2020 2020  ce=False)..     
+00011ce0: 2020 2023 2067 6574 206e 756d 6265 7220     # get number 
+00011cf0: 6f66 2049 6e64 6976 6964 7561 6c73 2062  of Individuals b
+00011d00: 6566 6f72 6520 6f70 6572 6174 696f 6e0a  efore operation.
+00011d10: 2020 2020 2020 2020 4e5f 6234 203d 206c          N_b4 = l
+00011d20: 656e 2873 656c 6629 0a0a 2020 2020 2020  en(self)..      
+00011d30: 2020 2320 7265 6d6f 7665 2074 6865 2049    # remove the I
+00011d40: 6e64 6976 6964 7561 6c73 0a20 2020 2020  ndividuals.     
+00011d50: 2020 2066 6f72 2069 6420 696e 2069 6e64     for id in ind
+00011d60: 6976 6964 733a 0a20 2020 2020 2020 2020  ivids:.         
+00011d70: 2020 2067 6f6f 6462 7965 203d 2073 656c     goodbye = sel
+00011d80: 662e 706f 7028 6964 290a 0a20 2020 2020  f.pop(id)..     
+00011d90: 2020 2023 2061 7373 6572 7420 7468 6174     # assert that
+00011da0: 2070 6f70 756c 6174 696f 6e20 7369 7a65   population size
+00011db0: 2068 6173 2063 6861 6e67 6564 2074 6865   has changed the
+00011dc0: 2063 6f72 7265 6374 2061 6d6f 756e 740a   correct amount.
+00011dd0: 2020 2020 2020 2020 4e5f 6166 203d 206c          N_af = l
+00011de0: 656e 2873 656c 6629 0a20 2020 2020 2020  en(self).       
+00011df0: 2061 7373 6572 7420 284e 5f62 3420 2d20   assert (N_b4 - 
+00011e00: 4e5f 6166 2920 3d3d 206c 656e 2869 6e64  N_af) == len(ind
+00011e10: 6976 6964 7329 2c20 2822 496e 636f 7272  ivids), ("Incorr
+00011e20: 6563 7420 6e75 6d62 6572 206f 6620 220a  ect number of ".
+00011e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e60: 2249 6e64 6976 6964 756c 7320 7265 6d6f  "Individuls remo
+00011e70: 7665 6421 2229 0a0a 2020 2020 2020 2020  ved!")..        
+00011e80: 2320 7570 6461 7465 2074 6865 2054 6162  # update the Tab
+00011e90: 6c65 436f 6c6c 6563 7469 6f6e 2c20 6966  leCollection, if
+00011ea0: 206e 6563 6573 7361 7279 0a20 2020 2020   necessary.     
+00011eb0: 2020 2023 2028 6275 7420 6b65 6570 2061     # (but keep a
+00011ec0: 6e64 2063 6f70 7920 6261 636b 2069 6e20  nd copy back in 
+00011ed0: 7468 6520 7369 7465 7320 7461 626c 652c  the sites table,
+00011ee0: 2069 6620 6e65 6365 7373 6172 792c 0a20   if necessary,. 
+00011ef0: 2020 2020 2020 2023 2065 2e67 2e2c 2077         # e.g., w
+00011f00: 6865 6e20 696e 6974 2070 6172 616d 7320  hen init params 
+00011f10: 6172 6520 7265 6d6f 7669 6e67 2061 6e64  are removing and
+00011f20: 2072 6570 6c61 6369 6e67 2061 6c6c 2067   replacing all g
+00011f30: 6e78 2d73 696d 756c 6174 6564 0a20 2020  nx-simulated.   
+00011f40: 2020 2020 2023 2049 6e64 6976 6964 7561       # Individua
+00011f50: 6c73 290a 2020 2020 2020 2020 6966 2073  ls).        if s
+00011f60: 656c 662e 6765 6e5f 6172 6368 2e75 7365  elf.gen_arch.use
+00011f70: 5f74 736b 6974 3a0a 2020 2020 2020 2020  _tskit:.        
+00011f80: 2020 2020 6966 206b 6565 705f 7369 7465      if keep_site
+00011f90: 735f 7461 623a 0a20 2020 2020 2020 2020  s_tab:.         
+00011fa0: 2020 2020 2020 2073 6974 6573 5f74 6162         sites_tab
+00011fb0: 203d 2073 656c 662e 5f74 632e 7369 7465   = self._tc.site
+00011fc0: 730a 2020 2020 2020 2020 2020 2020 7365  s.            se
+00011fd0: 6c66 2e5f 736f 7274 5f61 6e64 5f73 696d  lf._sort_and_sim
+00011fe0: 706c 6966 795f 7461 626c 655f 636f 6c6c  plify_table_coll
+00011ff0: 6563 7469 6f6e 2829 0a20 2020 2020 2020  ection().       
+00012000: 2020 2020 2069 6620 6b65 6570 5f73 6974       if keep_sit
+00012010: 6573 5f74 6162 3a0a 2020 2020 2020 2020  es_tab:.        
+00012020: 2020 2020 2020 2020 7365 6c66 2e5f 7463          self._tc
+00012030: 2e73 6974 6573 2e72 6570 6c61 6365 5f77  .sites.replace_w
+00012040: 6974 6828 7369 7465 735f 7461 6229 0a0a  ith(sites_tab)..
+00012050: 2020 2020 2020 2020 2320 7570 6461 7465          # update
+00012060: 2073 656c 662e 636f 6f72 6473 2061 6e64   self.coords and
+00012070: 2073 656c 662e 6365 6c6c 7320 6174 7472   self.cells attr
+00012080: 6962 7574 6573 0a20 2020 2020 2020 2073  ibutes.        s
+00012090: 656c 662e 5f73 6574 5f63 6f6f 7264 735f  elf._set_coords_
+000120a0: 616e 645f 6365 6c6c 7328 290a 0a20 2020  and_cells()..   
+000120b0: 2020 2020 2023 2061 6e64 2075 7064 6174       # and updat
+000120c0: 6520 6578 7469 6e63 7420 666c 6167 0a20  e extinct flag. 
+000120d0: 2020 2020 2020 2069 6620 6368 6563 6b5f         if check_
+000120e0: 6578 7469 6e63 743a 0a20 2020 2020 2020  extinct:.       
+000120f0: 2020 2020 2073 656c 662e 6578 7469 6e63       self.extinc
+00012100: 7420 3d20 7365 6c66 2e5f 6368 6563 6b5f  t = self._check_
+00012110: 6578 7469 6e63 7428 290a 0a20 2020 2020  extinct()..     
+00012120: 2020 2023 2070 7269 6e74 2069 6e66 6f72     # print infor
+00012130: 6d61 7469 7665 206f 7574 7075 740a 2020  mative output.  
+00012140: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
+00012150: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00012160: 696e 7428 6622 5c6e 7b6c 656e 2869 6e64  int(f"\n{len(ind
+00012170: 6976 6964 7329 7d20 496e 6469 7669 6475  ivids)} Individu
+00012180: 616c 7320 7375 6363 6573 7366 756c 6c79  als successfully
+00012190: 2072 656d 6f76 6564 2e5c 6e22 290a 2020   removed.\n").  
+000121a0: 2020 2020 2020 7265 7475 726e 0a0a 0a20        return... 
+000121b0: 2020 2064 6566 205f 6164 645f 696e 6469     def _add_indi
+000121c0: 7669 6475 616c 7328 7365 6c66 2c0a 2020  viduals(self,.  
 000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121e0: 206c 616e 642c 0a20 2020 2020 2020 2020   land,.         
+000121e0: 2020 2020 2020 206e 2c0a 2020 2020 2020         n,.      
 000121f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012200: 736f 7572 6365 5f73 7070 3d4e 6f6e 652c  source_spp=None,
-00012210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012220: 2020 2020 2020 2020 2020 736f 7572 6365            source
-00012230: 5f6d 7370 7269 6d65 5f70 6172 616d 733d  _msprime_params=
-00012240: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00012250: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00012260: 6e64 6976 6964 733d 4e6f 6e65 2c0a 2020  ndivids=None,.  
-00012270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012280: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-00012290: 2022 2222 0a20 2020 2020 2020 2041 6464   """.        Add
-000122a0: 2069 6e64 6976 6964 7561 6c73 2074 6f20   individuals to 
-000122b0: 7468 6973 2072 6563 6970 6965 6e74 2053  this recipient S
-000122c0: 7065 6369 6573 206f 626a 6563 742c 2065  pecies object, e
-000122d0: 6974 6865 7220 7573 696e 6720 6120 7365  ither using a se
-000122e0: 636f 6e64 0a20 2020 2020 2020 2053 7065  cond.        Spe
-000122f0: 6369 6573 206f 626a 6563 7420 6173 2074  cies object as t
-00012300: 6865 2073 6f75 7263 6520 706f 7075 6c61  he source popula
-00012310: 7469 6f6e 206f 7220 6665 6564 696e 6720  tion or feeding 
-00012320: 6120 6469 6374 206f 6620 7061 7261 6d65  a dict of parame
-00012330: 7465 7273 0a20 2020 2020 2020 2069 6e74  ters.        int
-00012340: 6f20 6d73 7072 696d 6520 746f 2073 696d  o msprime to sim
-00012350: 756c 6174 6520 7468 6520 736f 7572 6365  ulate the source
-00012360: 2070 6f70 756c 6174 696f 6e2e 0a20 2020   population..   
-00012370: 2020 2020 2028 646f 6373 2069 6e20 7468       (docs in th
-00012380: 6520 6d6f 6465 6c2e 7079 2077 7261 7070  e model.py wrapp
-00012390: 6572 206d 6574 686f 6429 0a20 2020 2020  er method).     
-000123a0: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-000123b0: 206d 616b 6520 7375 7265 2073 6f75 7263   make sure sourc
-000123c0: 655f 7370 7020 6973 2065 6974 6865 7220  e_spp is either 
-000123d0: 6120 5370 6563 6965 7320 6f62 6a65 6374  a Species object
-000123e0: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
-000123f0: 2061 7373 6572 7420 2869 7369 6e73 7461   assert (isinsta
-00012400: 6e63 6528 736f 7572 6365 5f73 7070 2c20  nce(source_spp, 
-00012410: 5370 6563 6965 7329 206f 7220 736f 7572  Species) or sour
-00012420: 6365 5f73 7070 2069 7320 4e6f 6e65 292c  ce_spp is None),
-00012430: 2028 2254 6865 2022 0a20 2020 2020 2020   ("The ".       
-00012440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012450: 2022 736f 7572 6365 5f73 7070 2070 6172   "source_spp par
-00012460: 616d 206d 7573 7420 6265 2065 6974 6865  am must be eithe
-00012470: 7220 4e6f 6e65 206f 7220 616e 6f74 6865  r None or anothe
-00012480: 7220 220a 2020 2020 2020 2020 2020 2020  r ".            
-00012490: 2020 2020 2020 2020 2020 2020 2253 7065              "Spe
-000124a0: 6369 6573 206f 626a 6563 742e 2229 0a0a  cies object.")..
-000124b0: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
-000124c0: 6520 6e65 7874 206e 2067 6e78 2049 6e64  e next n gnx Ind
-000124d0: 6976 6964 7561 6c73 2720 6964 730a 2020  ividuals' ids.  
-000124e0: 2020 2020 2020 6e65 7874 5f6e 5f69 6478        next_n_idx
-000124f0: 7320 3d20 5b2a 7261 6e67 6528 7365 6c66  s = [*range(self
-00012500: 2e6d 6178 5f69 6e64 5f69 6478 202b 2031  .max_ind_idx + 1
-00012510: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012520: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012530: 6c66 2e6d 6178 5f69 6e64 5f69 6478 202b  lf.max_ind_idx +
-00012540: 206e 202b 2031 295d 0a0a 2020 2020 2020   n + 1)]..      
-00012550: 2020 2320 6368 6563 6b20 616e 6420 6861    # check and ha
-00012560: 6e64 6c65 2074 6865 2063 6f6f 7264 7320  ndle the coords 
-00012570: 7061 7261 6d0a 2020 2020 2020 2020 6173  param.        as
-00012580: 7365 7274 206e 702e 6174 6c65 6173 745f  sert np.atleast_
-00012590: 3264 2863 6f6f 7264 7329 2e73 6861 7065  2d(coords).shape
-000125a0: 2069 6e20 5b28 312c 3229 2c20 286e 2c32   in [(1,2), (n,2
-000125b0: 295d 2c20 280a 2020 2020 2020 2020 2020  )], (.          
-000125c0: 2020 2254 6865 2027 636f 6f72 6473 2720    "The 'coords' 
-000125d0: 6172 6720 6d75 7374 2062 6520 7072 6f76  arg must be prov
-000125e0: 6964 6564 2065 6974 6865 7220 220a 2020  ided either ".  
-000125f0: 2020 2020 2020 2020 2020 2261 2073 696e            "a sin
-00012600: 676c 6520 782c 7920 636f 6f72 6469 6e61  gle x,y coordina
-00012610: 7465 2070 6169 7220 2861 7420 7768 6963  te pair (at whic
-00012620: 6820 616c 6c20 496e 6469 7669 6475 616c  h all Individual
-00012630: 7320 220a 2020 2020 2020 2020 2020 2020  s ".            
-00012640: 2277 696c 6c20 6265 2069 6e74 726f 6475  "will be introdu
-00012650: 6365 6429 206f 7220 616e 206e 7832 2061  ced) or an nx2 a
-00012660: 7272 6179 206f 6620 782c 7920 636f 6f72  rray of x,y coor
-00012670: 6469 6e61 7465 2070 6169 7273 2022 0a20  dinate pairs ". 
-00012680: 2020 2020 2020 2020 2020 2022 2869 6e64             "(ind
-00012690: 6963 6174 696e 6720 7468 6520 696e 7472  icating the intr
-000126a0: 6f64 7563 7469 6f6e 206c 6f63 6174 696f  oduction locatio
-000126b0: 6e73 2066 6f72 2022 0a20 2020 2020 2020  ns for ".       
-000126c0: 2020 2020 2022 6561 6368 206f 6620 7468       "each of th
-000126d0: 6520 6e20 496e 6469 7669 6475 616c 7320  e n Individuals 
-000126e0: 6265 696e 6720 696e 7472 6f64 7563 6564  being introduced
-000126f0: 2e22 290a 2020 2020 2020 2020 6966 206e  .").        if n
-00012700: 702e 6174 6c65 6173 745f 3264 2863 6f6f  p.atleast_2d(coo
-00012710: 7264 7329 2e73 6861 7065 203d 3d20 2831  rds).shape == (1
-00012720: 2c20 3229 3a0a 2020 2020 2020 2020 2020  , 2):.          
-00012730: 2020 636f 6f72 6473 203d 206e 702e 7374    coords = np.st
-00012740: 6163 6b28 5b63 6f6f 7264 7320 666f 7220  ack([coords for 
-00012750: 5f20 696e 2072 616e 6765 286e 295d 290a  _ in range(n)]).
-00012760: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00012770: 7274 2063 6f6f 7264 732e 7368 6170 6520  rt coords.shape 
-00012780: 3d3d 2028 6e2c 2032 290a 2020 2020 2020  == (n, 2).      
-00012790: 2020 2320 6d61 6b65 2073 7572 6520 636f    # make sure co
-000127a0: 6f72 6473 2061 7265 2061 6c6c 2077 6974  ords are all wit
-000127b0: 6869 6e20 7468 6520 6c61 6e64 7363 6170  hin the landscap
-000127c0: 650a 2020 2020 2020 2020 666f 7220 636f  e.        for co
-000127d0: 6f72 6420 696e 2063 6f6f 7264 733a 0a20  ord in coords:. 
-000127e0: 2020 2020 2020 2020 2020 2023 204e 4f54             # NOT
-000127f0: 453a 2073 7562 7472 6163 7469 6e67 2030  E: subtracting 0
-00012800: 2e30 3031 2066 726f 6d20 6469 6d73 2c20  .001 from dims, 
-00012810: 746f 206d 6174 6368 2068 6f77 2064 696d  to match how dim
-00012820: 7320 6172 6520 6861 6e64 6c65 640a 2020  s are handled.  
-00012830: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00012840: 2020 666f 7220 7374 6172 7469 6e67 2063    for starting c
-00012850: 6f6f 7264 696e 6174 6520 6173 7369 676e  oordinate assign
-00012860: 6d65 6e74 2069 6e0a 2020 2020 2020 2020  ment in.        
-00012870: 2020 2020 2320 2020 2020 2020 696e 6469      #       indi
-00012880: 7669 6475 616c 732e 5f6d 616b 655f 696e  viduals._make_in
-00012890: 6469 7669 6475 616c 0a20 2020 2020 2020  dividual.       
-000128a0: 2020 2020 2023 204e 4f54 453a 206c 616e       # NOTE: lan
-000128b0: 6420 6469 6d73 2061 7265 206f 7264 6572  d dims are order
-000128c0: 6564 2061 7320 5b78 2c79 5d2c 2069 2e65  ed as [x,y], i.e
-000128d0: 2e2c 205b 6a2c 695d 0a20 2020 2020 2020  ., [j,i].       
-000128e0: 2020 2020 2061 7373 6572 7420 2830 203c       assert (0 <
-000128f0: 3d20 636f 6f72 645b 305d 203c 3d20 7365  = coord[0] <= se
-00012900: 6c66 2e5f 6c61 6e64 5f64 696d 5b30 5d20  lf._land_dim[0] 
-00012910: 2d20 302e 3030 3120 616e 640a 2020 2020  - 0.001 and.    
-00012920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012930: 3020 3c3d 2063 6f6f 7264 5b31 5d20 3c3d  0 <= coord[1] <=
+00012200: 2020 2063 6f6f 7264 732c 0a20 2020 2020     coords,.     
+00012210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012220: 2020 2020 6c61 6e64 2c0a 2020 2020 2020      land,.      
+00012230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012240: 2020 2073 6f75 7263 655f 7370 703d 4e6f     source_spp=No
+00012250: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00012260: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
+00012270: 7263 655f 6d73 7072 696d 655f 7061 7261  rce_msprime_para
+00012280: 6d73 3d4e 6f6e 652c 0a20 2020 2020 2020  ms=None,.       
+00012290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122a0: 2020 696e 6469 7669 6473 3d4e 6f6e 652c    individs=None,
+000122b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000122c0: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+000122d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000122e0: 4164 6420 696e 6469 7669 6475 616c 7320  Add individuals 
+000122f0: 746f 2074 6869 7320 7265 6369 7069 656e  to this recipien
+00012300: 7420 5370 6563 6965 7320 6f62 6a65 6374  t Species object
+00012310: 2c20 6569 7468 6572 2075 7369 6e67 2061  , either using a
+00012320: 2073 6563 6f6e 640a 2020 2020 2020 2020   second.        
+00012330: 5370 6563 6965 7320 6f62 6a65 6374 2061  Species object a
+00012340: 7320 7468 6520 736f 7572 6365 2070 6f70  s the source pop
+00012350: 756c 6174 696f 6e20 6f72 2066 6565 6469  ulation or feedi
+00012360: 6e67 2061 2064 6963 7420 6f66 2070 6172  ng a dict of par
+00012370: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00012380: 696e 746f 206d 7370 7269 6d65 2074 6f20  into msprime to 
+00012390: 7369 6d75 6c61 7465 2074 6865 2073 6f75  simulate the sou
+000123a0: 7263 6520 706f 7075 6c61 7469 6f6e 2e0a  rce population..
+000123b0: 2020 2020 2020 2020 2864 6f63 7320 696e          (docs in
+000123c0: 2074 6865 206d 6f64 656c 2e70 7920 7772   the model.py wr
+000123d0: 6170 7065 7220 6d65 7468 6f64 290a 2020  apper method).  
+000123e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000123f0: 2020 2320 6d61 6b65 2073 7572 6520 736f    # make sure so
+00012400: 7572 6365 5f73 7070 2069 7320 6569 7468  urce_spp is eith
+00012410: 6572 2061 2053 7065 6369 6573 206f 626a  er a Species obj
+00012420: 6563 7420 6f72 204e 6f6e 650a 2020 2020  ect or None.    
+00012430: 2020 2020 6173 7365 7274 2028 6973 696e      assert (isin
+00012440: 7374 616e 6365 2873 6f75 7263 655f 7370  stance(source_sp
+00012450: 702c 2053 7065 6369 6573 2920 6f72 2073  p, Species) or s
+00012460: 6f75 7263 655f 7370 7020 6973 204e 6f6e  ource_spp is Non
+00012470: 6529 2c20 2822 5468 6520 220a 2020 2020  e), ("The ".    
+00012480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012490: 2020 2020 2273 6f75 7263 655f 7370 7020      "source_spp 
+000124a0: 7061 7261 6d20 6d75 7374 2062 6520 6569  param must be ei
+000124b0: 7468 6572 204e 6f6e 6520 6f72 2061 6e6f  ther None or ano
+000124c0: 7468 6572 2022 0a20 2020 2020 2020 2020  ther ".         
+000124d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000124e0: 5370 6563 6965 7320 6f62 6a65 6374 2e22  Species object."
+000124f0: 290a 0a20 2020 2020 2020 2023 2067 6574  )..        # get
+00012500: 2074 6865 206e 6578 7420 6e20 676e 7820   the next n gnx 
+00012510: 496e 6469 7669 6475 616c 7327 2069 6473  Individuals' ids
+00012520: 0a20 2020 2020 2020 206e 6578 745f 6e5f  .        next_n_
+00012530: 6964 7873 203d 205b 2a72 616e 6765 2873  idxs = [*range(s
+00012540: 656c 662e 6d61 785f 696e 645f 6964 7820  elf.max_ind_idx 
+00012550: 2b20 312c 0a20 2020 2020 2020 2020 2020  + 1,.           
+00012560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012570: 2073 656c 662e 6d61 785f 696e 645f 6964   self.max_ind_id
+00012580: 7820 2b20 6e20 2b20 3129 5d0a 0a20 2020  x + n + 1)]..   
+00012590: 2020 2020 2023 2063 6865 636b 2061 6e64       # check and
+000125a0: 2068 616e 646c 6520 7468 6520 636f 6f72   handle the coor
+000125b0: 6473 2070 6172 616d 0a20 2020 2020 2020  ds param.       
+000125c0: 2061 7373 6572 7420 6e70 2e61 746c 6561   assert np.atlea
+000125d0: 7374 5f32 6428 636f 6f72 6473 292e 7368  st_2d(coords).sh
+000125e0: 6170 6520 696e 205b 2831 2c32 292c 2028  ape in [(1,2), (
+000125f0: 6e2c 3229 5d2c 2028 0a20 2020 2020 2020  n,2)], (.       
+00012600: 2020 2020 2022 5468 6520 2763 6f6f 7264       "The 'coord
+00012610: 7327 2061 7267 206d 7573 7420 6265 2070  s' arg must be p
+00012620: 726f 7669 6465 6420 6569 7468 6572 2022  rovided either "
+00012630: 0a20 2020 2020 2020 2020 2020 2022 6120  .            "a 
+00012640: 7369 6e67 6c65 2078 2c79 2063 6f6f 7264  single x,y coord
+00012650: 696e 6174 6520 7061 6972 2028 6174 2077  inate pair (at w
+00012660: 6869 6368 2061 6c6c 2049 6e64 6976 6964  hich all Individ
+00012670: 7561 6c73 2022 0a20 2020 2020 2020 2020  uals ".         
+00012680: 2020 2022 7769 6c6c 2062 6520 696e 7472     "will be intr
+00012690: 6f64 7563 6564 2920 6f72 2061 6e20 6e78  oduced) or an nx
+000126a0: 3220 6172 7261 7920 6f66 2078 2c79 2063  2 array of x,y c
+000126b0: 6f6f 7264 696e 6174 6520 7061 6972 7320  oordinate pairs 
+000126c0: 220a 2020 2020 2020 2020 2020 2020 2228  ".            "(
+000126d0: 696e 6469 6361 7469 6e67 2074 6865 2069  indicating the i
+000126e0: 6e74 726f 6475 6374 696f 6e20 6c6f 6361  ntroduction loca
+000126f0: 7469 6f6e 7320 666f 7220 220a 2020 2020  tions for ".    
+00012700: 2020 2020 2020 2020 2265 6163 6820 6f66          "each of
+00012710: 2074 6865 206e 2049 6e64 6976 6964 7561   the n Individua
+00012720: 6c73 2062 6569 6e67 2069 6e74 726f 6475  ls being introdu
+00012730: 6365 642e 2229 0a20 2020 2020 2020 2069  ced.").        i
+00012740: 6620 6e70 2e61 746c 6561 7374 5f32 6428  f np.atleast_2d(
+00012750: 636f 6f72 6473 292e 7368 6170 6520 3d3d  coords).shape ==
+00012760: 2028 312c 2032 293a 0a20 2020 2020 2020   (1, 2):.       
+00012770: 2020 2020 2063 6f6f 7264 7320 3d20 6e70       coords = np
+00012780: 2e73 7461 636b 285b 636f 6f72 6473 2066  .stack([coords f
+00012790: 6f72 205f 2069 6e20 7261 6e67 6528 6e29  or _ in range(n)
+000127a0: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
+000127b0: 7373 6572 7420 636f 6f72 6473 2e73 6861  ssert coords.sha
+000127c0: 7065 203d 3d20 286e 2c20 3229 0a20 2020  pe == (n, 2).   
+000127d0: 2020 2020 2023 206d 616b 6520 7375 7265       # make sure
+000127e0: 2063 6f6f 7264 7320 6172 6520 616c 6c20   coords are all 
+000127f0: 7769 7468 696e 2074 6865 206c 616e 6473  within the lands
+00012800: 6361 7065 0a20 2020 2020 2020 2066 6f72  cape.        for
+00012810: 2063 6f6f 7264 2069 6e20 636f 6f72 6473   coord in coords
+00012820: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00012830: 4e4f 5445 3a20 7375 6274 7261 6374 696e  NOTE: subtractin
+00012840: 6720 302e 3030 3120 6672 6f6d 2064 696d  g 0.001 from dim
+00012850: 732c 2074 6f20 6d61 7463 6820 686f 7720  s, to match how 
+00012860: 6469 6d73 2061 7265 2068 616e 646c 6564  dims are handled
+00012870: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+00012880: 2020 2020 2066 6f72 2073 7461 7274 696e       for startin
+00012890: 6720 636f 6f72 6469 6e61 7465 2061 7373  g coordinate ass
+000128a0: 6967 6e6d 656e 7420 696e 0a20 2020 2020  ignment in.     
+000128b0: 2020 2020 2020 2023 2020 2020 2020 2069         #       i
+000128c0: 6e64 6976 6964 7561 6c73 2e5f 6d61 6b65  ndividuals._make
+000128d0: 5f69 6e64 6976 6964 7561 6c0a 2020 2020  _individual.    
+000128e0: 2020 2020 2020 2020 2320 4e4f 5445 3a20          # NOTE: 
+000128f0: 6c61 6e64 2064 696d 7320 6172 6520 6f72  land dims are or
+00012900: 6465 7265 6420 6173 205b 782c 795d 2c20  dered as [x,y], 
+00012910: 692e 652e 2c20 5b6a 2c69 5d0a 2020 2020  i.e., [j,i].    
+00012920: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
+00012930: 3020 3c3d 2063 6f6f 7264 5b30 5d20 3c3d  0 <= coord[0] <=
 00012940: 2073 656c 662e 5f6c 616e 645f 6469 6d5b   self._land_dim[
-00012950: 315d 202d 2030 2e30 3031 292c 2028 0a20  1] - 0.001), (. 
+00012950: 305d 202d 2030 2e30 3031 2061 6e64 0a20  0] - 0.001 and. 
 00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012990: 2020 2020 2243 6f6f 7264 7320 6d75 7374      "Coords must
-000129a0: 2062 6520 220a 2020 2020 2020 2020 2020   be ".          
+00012970: 2020 2030 203c 3d20 636f 6f72 645b 315d     0 <= coord[1]
+00012980: 203c 3d20 7365 6c66 2e5f 6c61 6e64 5f64   <= self._land_d
+00012990: 696d 5b31 5d20 2d20 302e 3030 3129 2c20  im[1] - 0.001), 
+000129a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
 000129b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000129c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129d0: 2020 2020 2020 2020 2020 2022 7661 6c69             "vali
-000129e0: 6420 666f 7220 7468 6520 7265 6369 7069  d for the recipi
-000129f0: 656e 7420 220a 2020 2020 2020 2020 2020  ent ".          
+000129d0: 2020 2020 2020 2022 436f 6f72 6473 206d         "Coords m
+000129e0: 7573 7420 6265 2022 0a20 2020 2020 2020  ust be ".       
+000129f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a20: 2020 2020 2020 2020 2020 2022 5370 6563             "Spec
-00012a30: 6965 7327 204c 616e 6473 6361 7065 2022  ies' Landscape "
-00012a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012a10: 2020 2020 2020 2020 2020 2020 2020 2276                "v
+00012a20: 616c 6964 2066 6f72 2074 6865 2072 6563  alid for the rec
+00012a30: 6970 6965 6e74 2022 0a20 2020 2020 2020  ipient ".       
+00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a70: 2020 2020 2020 2228 692e 652e 2c20 7820        "(i.e., x 
-00012a80: 616e 6420 7920 6d75 7374 2062 6520 220a  and y must be ".
+00012a60: 2020 2020 2020 2020 2020 2020 2020 2253                "S
+00012a70: 7065 6369 6573 2720 4c61 6e64 7363 6170  pecies' Landscap
+00012a80: 6520 220a 2020 2020 2020 2020 2020 2020  e ".            
 00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ac0: 2020 2020 2022 696e 2074 6865 2069 6e63       "in the inc
-00012ad0: 6c75 7369 7665 2022 0a20 2020 2020 2020  lusive ".       
+00012ab0: 2020 2020 2020 2020 2022 2869 2e65 2e2c           "(i.e.,
+00012ac0: 2078 2061 6e64 2079 206d 7573 7420 6265   x and y must be
+00012ad0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
 00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b00: 2020 2020 2020 2020 2020 2020 2020 2220                " 
-00012b10: 696e 7465 7276 616c 7320 220a 2020 2020  intervals ".    
+00012b00: 2020 2020 2020 2020 2269 6e20 7468 6520          "in the 
+00012b10: 696e 636c 7573 6976 6520 220a 2020 2020  inclusive ".    
 00012b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b50: 2022 5b30 2c20 6c61 6e64 5f64 696d 5f78   "[0, land_dim_x
-00012b60: 5d20 616e 6422 0a20 2020 2020 2020 2020  ] and".         
+00012b50: 2022 2069 6e74 6572 7661 6c73 2022 0a20   " intervals ". 
+00012b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b90: 2020 2020 2020 2020 2020 2020 225b 302c              "[0,
-00012ba0: 206c 616e 645f 6469 6d5f 795d 2c20 220a   land_dim_y], ".
+00012b90: 2020 2020 225b 302c 206c 616e 645f 6469      "[0, land_di
+00012ba0: 6d5f 785d 2061 6e64 220a 2020 2020 2020  m_x] and".      
 00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012be0: 2020 2020 2022 7265 7370 6563 7469 7665       "respective
-00012bf0: 6c79 2e22 290a 0a20 2020 2020 2020 2023  ly.")..        #
-00012c00: 2065 6974 6865 7220 6765 7420 496e 6469   either get Indi
-00012c10: 7669 6475 616c 7320 616e 6420 7468 6569  viduals and thei
-00012c20: 7220 7473 6b69 742e 5461 626c 6543 6f6c  r tskit.TableCol
-00012c30: 6c65 6374 696f 6e0a 2020 2020 2020 2020  lection.        
-00012c40: 2320 6672 6f6d 2074 6865 2067 6976 656e  # from the given
-00012c50: 2067 6e78 2053 7065 6369 6573 206f 626a   gnx Species obj
-00012c60: 6563 742e 2e2e 0a20 2020 2020 2020 2069  ect....        i
-00012c70: 6620 736f 7572 6365 5f73 7070 2069 7320  f source_spp is 
-00012c80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00012c90: 2020 2020 2020 2320 7261 6973 6520 7761        # raise wa
-00012ca0: 726e 696e 6720 6162 6f75 7420 706f 7465  rning about pote
-00012cb0: 6e74 6961 6c20 756e 666f 7265 7365 656e  ntial unforeseen
-00012cc0: 2065 6666 6563 7473 206f 6620 696e 7472   effects of intr
-00012cd0: 6f64 7563 696e 670a 2020 2020 2020 2020  oducing.        
-00012ce0: 2020 2020 2320 496e 6469 7669 6475 616c      # Individual
-00012cf0: 7320 6672 6f6d 2061 6e20 696e 636f 7272  s from an incorr
-00012d00: 6563 746c 7920 7061 7261 6d65 7465 7269  ectly parameteri
-00012d10: 7a65 6420 736f 7572 6365 2053 7065 6369  zed source Speci
-00012d20: 6573 0a20 2020 2020 2020 2020 2020 2077  es.            w
-00012d30: 6172 6e69 6e67 732e 7761 726e 2828 2249  arnings.warn(("I
-00012d40: 6e74 726f 6475 6369 6e67 2049 6e64 6976  ntroducing Indiv
-00012d50: 6964 7561 6c73 2066 726f 6d20 6f6e 6520  iduals from one 
-00012d60: 5370 6563 6965 7320 6f62 6a65 6374 2022  Species object "
-00012d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012d80: 2020 2020 2022 696e 746f 2061 6e6f 7468       "into anoth
-00012d90: 6572 2063 6f75 6c64 2063 6175 7365 2075  er could cause u
-00012da0: 6e6e 6f74 6963 6564 2069 7373 7565 732e  nnoticed issues.
-00012db0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00012dc0: 2020 2020 2020 2022 4765 6f6e 6f6d 6963         "Geonomic
-00012dd0: 7320 7769 6c6c 2063 6865 636b 2061 6e64  s will check and
-00012de0: 2070 7265 7665 6e74 2063 6f6e 666c 6963   prevent conflic
-00012df0: 7420 6265 7477 6565 6e20 220a 2020 2020  t between ".    
-00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e10: 2273 7472 6963 746c 7920 696e 636f 6d70  "strictly incomp
-00012e20: 6174 6962 6c65 2061 7474 7269 6275 7465  atible attribute
-00012e30: 7320 6f66 2074 6865 2053 7065 6369 6573  s of the Species
-00012e40: 2c20 220a 2020 2020 2020 2020 2020 2020  , ".            
-00012e50: 2020 2020 2020 2020 2247 656e 6f6d 6963          "Genomic
-00012e60: 4172 6368 6974 6563 7475 7265 732c 2061  Architectures, a
-00012e70: 6e64 2054 7261 6974 732e 2048 6f77 6576  nd Traits. Howev
-00012e80: 6572 2c20 6174 7472 6962 7574 6573 2022  er, attributes "
-00012e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ea0: 2020 2020 2022 7768 6f73 6520 636f 6d70       "whose comp
-00012eb0: 6174 6962 696c 6974 7920 6465 7065 6e64  atibility depend
-00012ec0: 7320 6f6e 2074 6865 2073 6369 656e 7469  s on the scienti
-00012ed0: 6669 6320 220a 2020 2020 2020 2020 2020  fic ".          
-00012ee0: 2020 2020 2020 2020 2020 2272 6561 736f            "reaso
-00012ef0: 6e69 6e67 2062 6568 696e 6420 7468 6520  ning behind the 
-00012f00: 7363 656e 6172 696f 2062 6569 6e67 2073  scenario being s
-00012f10: 696d 756c 6174 6564 2022 0a20 2020 2020  imulated ".     
-00012f20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00012f30: 2865 2e67 2e2c 206d 7574 6174 696f 6e61  (e.g., mutationa
-00012f40: 6c20 7061 7261 6d65 7465 7273 2c20 220a  l parameters, ".
-00012f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f60: 2020 2020 2263 6172 7279 696e 6720 6361      "carrying ca
-00012f70: 7061 6369 7479 2070 6172 616d 6574 6572  pacity parameter
-00012f80: 732c 2065 7463 2e29 2022 0a20 2020 2020  s, etc.) ".     
-00012f90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00012fa0: 7769 6c6c 2062 6520 616c 6c6f 7765 6420  will be allowed 
-00012fb0: 746f 2064 6966 6665 7220 6265 7477 6565  to differ betwee
-00012fc0: 6e20 7468 6520 736f 7572 6365 2061 6e64  n the source and
-00012fd0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00012fe0: 2020 2020 2020 2022 7265 6369 7069 656e         "recipien
-00012ff0: 7420 5370 6563 6965 7320 6f62 6a65 6374  t Species object
-00013000: 7320 616e 642c 2022 0a20 2020 2020 2020  s and, ".       
-00013010: 2020 2020 2020 2020 2020 2020 2022 6966               "if
-00013020: 2074 6865 7365 2064 6966 6665 7265 6e63   these differenc
-00013030: 6573 2077 6572 6520 756e 696e 7465 6e64  es were unintend
-00013040: 6564 2062 7574 2067 6f20 220a 2020 2020  ed but go ".    
+00012bd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00012be0: 5b30 2c20 6c61 6e64 5f64 696d 5f79 5d2c  [0, land_dim_y],
+00012bf0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c20: 2020 2020 2020 2020 2272 6573 7065 6374          "respect
+00012c30: 6976 656c 792e 2229 0a0a 2020 2020 2020  ively.")..      
+00012c40: 2020 2320 6569 7468 6572 2067 6574 2049    # either get I
+00012c50: 6e64 6976 6964 7561 6c73 2061 6e64 2074  ndividuals and t
+00012c60: 6865 6972 2074 736b 6974 2e54 6162 6c65  heir tskit.Table
+00012c70: 436f 6c6c 6563 7469 6f6e 0a20 2020 2020  Collection.     
+00012c80: 2020 2023 2066 726f 6d20 7468 6520 6769     # from the gi
+00012c90: 7665 6e20 676e 7820 5370 6563 6965 7320  ven gnx Species 
+00012ca0: 6f62 6a65 6374 2e2e 2e0a 2020 2020 2020  object....      
+00012cb0: 2020 6966 2073 6f75 7263 655f 7370 7020    if source_spp 
+00012cc0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00012cd0: 2020 2020 2020 2020 2023 2072 6169 7365           # raise
+00012ce0: 2077 6172 6e69 6e67 2061 626f 7574 2070   warning about p
+00012cf0: 6f74 656e 7469 616c 2075 6e66 6f72 6573  otential unfores
+00012d00: 6565 6e20 6566 6665 6374 7320 6f66 2069  een effects of i
+00012d10: 6e74 726f 6475 6369 6e67 0a20 2020 2020  ntroducing.     
+00012d20: 2020 2020 2020 2023 2049 6e64 6976 6964         # Individ
+00012d30: 7561 6c73 2066 726f 6d20 616e 2069 6e63  uals from an inc
+00012d40: 6f72 7265 6374 6c79 2070 6172 616d 6574  orrectly paramet
+00012d50: 6572 697a 6564 2073 6f75 7263 6520 5370  erized source Sp
+00012d60: 6563 6965 730a 2020 2020 2020 2020 2020  ecies.          
+00012d70: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
+00012d80: 2822 496e 7472 6f64 7563 696e 6720 496e  ("Introducing In
+00012d90: 6469 7669 6475 616c 7320 6672 6f6d 206f  dividuals from o
+00012da0: 6e65 2053 7065 6369 6573 206f 626a 6563  ne Species objec
+00012db0: 7420 220a 2020 2020 2020 2020 2020 2020  t ".            
+00012dc0: 2020 2020 2020 2020 2269 6e74 6f20 616e          "into an
+00012dd0: 6f74 6865 7220 636f 756c 6420 6361 7573  other could caus
+00012de0: 6520 756e 6e6f 7469 6365 6420 6973 7375  e unnoticed issu
+00012df0: 6573 2e20 220a 2020 2020 2020 2020 2020  es. ".          
+00012e00: 2020 2020 2020 2020 2020 2247 656f 6e6f            "Geono
+00012e10: 6d69 6373 2077 696c 6c20 6368 6563 6b20  mics will check 
+00012e20: 616e 6420 7072 6576 656e 7420 636f 6e66  and prevent conf
+00012e30: 6c69 6374 2062 6574 7765 656e 2022 0a20  lict between ". 
+00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e50: 2020 2022 7374 7269 6374 6c79 2069 6e63     "strictly inc
+00012e60: 6f6d 7061 7469 626c 6520 6174 7472 6962  ompatible attrib
+00012e70: 7574 6573 206f 6620 7468 6520 5370 6563  utes of the Spec
+00012e80: 6965 732c 2022 0a20 2020 2020 2020 2020  ies, ".         
+00012e90: 2020 2020 2020 2020 2020 2022 4765 6e6f             "Geno
+00012ea0: 6d69 6341 7263 6869 7465 6374 7572 6573  micArchitectures
+00012eb0: 2c20 616e 6420 5472 6169 7473 2e20 486f  , and Traits. Ho
+00012ec0: 7765 7665 722c 2061 7474 7269 6275 7465  wever, attribute
+00012ed0: 7320 220a 2020 2020 2020 2020 2020 2020  s ".            
+00012ee0: 2020 2020 2020 2020 2277 686f 7365 2063          "whose c
+00012ef0: 6f6d 7061 7469 6269 6c69 7479 2064 6570  ompatibility dep
+00012f00: 656e 6473 206f 6e20 7468 6520 7363 6965  ends on the scie
+00012f10: 6e74 6966 6963 2022 0a20 2020 2020 2020  ntific ".       
+00012f20: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+00012f30: 6173 6f6e 696e 6720 6265 6869 6e64 2074  asoning behind t
+00012f40: 6865 2073 6365 6e61 7269 6f20 6265 696e  he scenario bein
+00012f50: 6720 7369 6d75 6c61 7465 6420 220a 2020  g simulated ".  
+00012f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f70: 2020 2228 652e 672e 2c20 6d75 7461 7469    "(e.g., mutati
+00012f80: 6f6e 616c 2070 6172 616d 6574 6572 732c  onal parameters,
+00012f90: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00012fa0: 2020 2020 2020 2022 6361 7272 7969 6e67         "carrying
+00012fb0: 2063 6170 6163 6974 7920 7061 7261 6d65   capacity parame
+00012fc0: 7465 7273 2c20 6574 632e 2920 220a 2020  ters, etc.) ".  
+00012fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fe0: 2020 2277 696c 6c20 6265 2061 6c6c 6f77    "will be allow
+00012ff0: 6564 2074 6f20 6469 6666 6572 2062 6574  ed to differ bet
+00013000: 7765 656e 2074 6865 2073 6f75 7263 6520  ween the source 
+00013010: 616e 6420 220a 2020 2020 2020 2020 2020  and ".          
+00013020: 2020 2020 2020 2020 2020 2272 6563 6970            "recip
+00013030: 6965 6e74 2053 7065 6369 6573 206f 626a  ient Species obj
+00013040: 6563 7473 2061 6e64 2c20 220a 2020 2020  ects and, ".    
 00013050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013060: 2275 6e64 6574 6563 7465 642c 2063 6f75  "undetected, cou
-00013070: 6c64 206c 6561 6420 746f 2069 6e63 6f72  ld lead to incor
-00013080: 7265 6374 206f 7220 6d69 736c 6561 6469  rect or misleadi
-00013090: 6e67 2064 6174 6120 220a 2020 2020 2020  ng data ".      
-000130a0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-000130b0: 6e64 2072 6573 756c 7473 2e20 506c 6561  nd results. Plea
-000130c0: 7365 2075 7365 2063 6172 6520 7768 656e  se use care when
-000130d0: 2070 6c61 6e6e 696e 672c 2022 0a20 2020   planning, ".   
+00013060: 2269 6620 7468 6573 6520 6469 6666 6572  "if these differ
+00013070: 656e 6365 7320 7765 7265 2075 6e69 6e74  ences were unint
+00013080: 656e 6465 6420 6275 7420 676f 2022 0a20  ended but go ". 
+00013090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130a0: 2020 2022 756e 6465 7465 6374 6564 2c20     "undetected, 
+000130b0: 636f 756c 6420 6c65 6164 2074 6f20 696e  could lead to in
+000130c0: 636f 7272 6563 7420 6f72 206d 6973 6c65  correct or misle
+000130d0: 6164 696e 6720 6461 7461 2022 0a20 2020  ading data ".   
 000130e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130f0: 2022 696d 706c 656d 656e 7469 6e67 2c20   "implementing, 
-00013100: 616e 6420 6368 6563 6b69 6e67 2079 6f75  and checking you
-00013110: 7220 636f 6465 2e22 2929 0a0a 2020 2020  r code."))..    
-00013120: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
-00013130: 6520 736f 7572 6365 2053 7065 6369 6573  e source Species
-00013140: 2066 726f 6d20 7769 7468 696e 2074 6869   from within thi
-00013150: 7320 6d6f 6465 6c2c 2069 6620 6e65 6365  s model, if nece
-00013160: 7373 6172 790a 2020 2020 2020 2020 2020  ssary.          
-00013170: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00013180: 736f 7572 6365 5f73 7070 2c20 696e 7429  source_spp, int)
-00013190: 206f 7220 6973 696e 7374 616e 6365 2873   or isinstance(s
-000131a0: 6f75 7263 655f 7370 702c 2073 7472 293a  ource_spp, str):
-000131b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000131c0: 2073 6f75 7263 655f 7370 7020 3d20 7365   source_spp = se
-000131d0: 6c66 2e63 6f6d 6d5b 7365 6c66 2e5f 6765  lf.comm[self._ge
-000131e0: 745f 7370 705f 6e75 6d28 736f 7572 6365  t_spp_num(source
-000131f0: 5f73 7070 295d 0a0a 2020 2020 2020 2020  _spp)]..        
-00013200: 2020 2020 2320 6173 7365 7274 2074 6861      # assert tha
-00013210: 7420 6578 6163 746c 7920 6f6e 6520 6f66  t exactly one of
-00013220: 2074 6865 2027 6e27 2061 6e64 2027 696e   the 'n' and 'in
-00013230: 6469 7669 6473 270a 2020 2020 2020 2020  divids'.        
-00013240: 2020 2020 2320 7061 7261 6d73 2069 7320      # params is 
-00013250: 7072 6f76 6964 6564 2c20 616e 6420 7468  provided, and th
-00013260: 6174 2074 6865 2073 697a 6520 6f66 2027  at the size of '
-00013270: 6e27 0a20 2020 2020 2020 2020 2020 2023  n'.            #
-00013280: 206f 7220 7369 7a65 2061 6e64 2063 6f6e   or size and con
-00013290: 7465 6e74 7320 6f66 2027 696e 6469 7669  tents of 'indivi
-000132a0: 6473 2720 6172 6520 7661 6c69 640a 2020  ds' are valid.  
-000132b0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-000132c0: 2028 286e 2069 7320 6e6f 7420 4e6f 6e65   ((n is not None
-000132d0: 2061 6e64 2069 6e64 6976 6964 7320 6973   and individs is
-000132e0: 204e 6f6e 6529 206f 720a 2020 2020 2020   None) or.      
-000132f0: 2020 2020 2020 2020 2020 2020 2020 286e                (n
-00013300: 2069 7320 4e6f 6e65 2061 6e64 2069 6e64   is None and ind
-00013310: 6976 6964 7320 6973 206e 6f74 204e 6f6e  ivids is not Non
-00013320: 6529 292c 2028 2249 6620 7573 696e 6720  e)), ("If using 
-00013330: 616e 6f74 6865 7220 220a 2020 2020 2020  another ".      
-00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013370: 2020 2247 656f 6e6f 6d69 6373 2053 7065    "Geonomics Spe
-00013380: 6369 6573 2022 0a20 2020 2020 2020 2020  cies ".         
+000130f0: 2022 616e 6420 7265 7375 6c74 732e 2050   "and results. P
+00013100: 6c65 6173 6520 7573 6520 6361 7265 2077  lease use care w
+00013110: 6865 6e20 706c 616e 6e69 6e67 2c20 220a  hen planning, ".
+00013120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013130: 2020 2020 2269 6d70 6c65 6d65 6e74 696e      "implementin
+00013140: 672c 2061 6e64 2063 6865 636b 696e 6720  g, and checking 
+00013150: 796f 7572 2063 6f64 652e 2229 290a 0a20  your code.")).. 
+00013160: 2020 2020 2020 2020 2020 2023 2067 6574             # get
+00013170: 2074 6865 2073 6f75 7263 6520 5370 6563   the source Spec
+00013180: 6965 7320 6672 6f6d 2077 6974 6869 6e20  ies from within 
+00013190: 7468 6973 206d 6f64 656c 2c20 6966 206e  this model, if n
+000131a0: 6563 6573 7361 7279 0a20 2020 2020 2020  ecessary.       
+000131b0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+000131c0: 6365 2873 6f75 7263 655f 7370 702c 2069  ce(source_spp, i
+000131d0: 6e74 2920 6f72 2069 7369 6e73 7461 6e63  nt) or isinstanc
+000131e0: 6528 736f 7572 6365 5f73 7070 2c20 7374  e(source_spp, st
+000131f0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00013200: 2020 2020 736f 7572 6365 5f73 7070 203d      source_spp =
+00013210: 2073 656c 662e 636f 6d6d 5b73 656c 662e   self.comm[self.
+00013220: 5f67 6574 5f73 7070 5f6e 756d 2873 6f75  _get_spp_num(sou
+00013230: 7263 655f 7370 7029 5d0a 0a20 2020 2020  rce_spp)]..     
+00013240: 2020 2020 2020 2023 2061 7373 6572 7420         # assert 
+00013250: 7468 6174 2065 7861 6374 6c79 206f 6e65  that exactly one
+00013260: 206f 6620 7468 6520 276e 2720 616e 6420   of the 'n' and 
+00013270: 2769 6e64 6976 6964 7327 0a20 2020 2020  'individs'.     
+00013280: 2020 2020 2020 2023 2070 6172 616d 7320         # params 
+00013290: 6973 2070 726f 7669 6465 642c 2061 6e64  is provided, and
+000132a0: 2074 6861 7420 7468 6520 7369 7a65 206f   that the size o
+000132b0: 6620 276e 270a 2020 2020 2020 2020 2020  f 'n'.          
+000132c0: 2020 2320 6f72 2073 697a 6520 616e 6420    # or size and 
+000132d0: 636f 6e74 656e 7473 206f 6620 2769 6e64  contents of 'ind
+000132e0: 6976 6964 7327 2061 7265 2076 616c 6964  ivids' are valid
+000132f0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00013300: 6572 7420 2828 6e20 6973 206e 6f74 204e  ert ((n is not N
+00013310: 6f6e 6520 616e 6420 696e 6469 7669 6473  one and individs
+00013320: 2069 7320 4e6f 6e65 2920 6f72 0a20 2020   is None) or.   
+00013330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013340: 2028 6e20 6973 204e 6f6e 6520 616e 6420   (n is None and 
+00013350: 696e 6469 7669 6473 2069 7320 6e6f 7420  individs is not 
+00013360: 4e6f 6e65 2929 2c20 2822 4966 2075 7369  None)), ("If usi
+00013370: 6e67 2061 6e6f 7468 6572 2022 0a20 2020  ng another ".   
+00013380: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013390: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000133a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000133c0: 6f62 6a65 6374 2061 7320 7468 6520 736f  object as the so
-000133d0: 7572 6365 2022 0a20 2020 2020 2020 2020  urce ".         
+000133b0: 2020 2020 2022 4765 6f6e 6f6d 6963 7320       "Geonomics 
+000133c0: 5370 6563 6965 7320 220a 2020 2020 2020  Species ".      
+000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000133e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000133f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013400: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00013410: 706f 7075 6c61 7469 6f6e 2074 6865 6e20  population then 
-00013420: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00013400: 2020 226f 626a 6563 7420 6173 2074 6865    "object as the
+00013410: 2073 6f75 7263 6520 220a 2020 2020 2020   source ".      
+00013420: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013450: 2020 2020 2020 2020 2020 2265 6974 6865            "eithe
-00013460: 7220 606e 6020 6f72 2022 0a20 2020 2020  r `n` or ".     
+00013450: 2020 2270 6f70 756c 6174 696f 6e20 7468    "population th
+00013460: 656e 2022 0a20 2020 2020 2020 2020 2020  en ".           
 00013470: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134a0: 2020 2022 6069 6e64 6976 6964 7360 206d     "`individs` m
-000134b0: 7573 7420 6265 2022 0a20 2020 2020 2020  ust be ".       
+00013490: 2020 2020 2020 2020 2020 2020 2022 6569               "ei
+000134a0: 7468 6572 2060 6e60 206f 7220 220a 2020  ther `n` or ".  
+000134b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000134c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000134d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134f0: 2022 7072 6f76 6964 6564 2c20 220a 2020   "provided, ".  
+000134e0: 2020 2020 2020 2260 696e 6469 7669 6473        "`individs
+000134f0: 6020 6d75 7374 2062 6520 220a 2020 2020  ` must be ".    
 00013500: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013530: 2020 2020 2020 2262 7574 206e 6f74 2062        "but not b
-00013540: 6f74 682e 2229 0a20 2020 2020 2020 2020  oth.").         
-00013550: 2020 2069 6620 696e 6469 7669 6473 2069     if individs i
-00013560: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00013570: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
-00013580: 203c 3d20 6c65 6e28 736f 7572 6365 5f73   <= len(source_s
-00013590: 7070 292c 2028 2260 6e60 206d 7573 7420  pp), ("`n` must 
-000135a0: 6e6f 7420 6265 2067 7265 6174 6572 2074  not be greater t
-000135b0: 6861 6e20 220a 2020 2020 2020 2020 2020  han ".          
-000135c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135e0: 2020 2020 2274 6865 2070 6f70 756c 6174      "the populat
-000135f0: 696f 6e20 7369 7a65 206f 6620 220a 2020  ion size of ".  
+00013530: 2020 2020 2270 726f 7669 6465 642c 2022      "provided, "
+00013540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013570: 2020 2020 2020 2020 2022 6275 7420 6e6f           "but no
+00013580: 7420 626f 7468 2e22 290a 2020 2020 2020  t both.").      
+00013590: 2020 2020 2020 6966 2069 6e64 6976 6964        if individ
+000135a0: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
+000135b0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+000135c0: 7420 6e20 3c3d 206c 656e 2873 6f75 7263  t n <= len(sourc
+000135d0: 655f 7370 7029 2c20 2822 606e 6020 6d75  e_spp), ("`n` mu
+000135e0: 7374 206e 6f74 2062 6520 6772 6561 7465  st not be greate
+000135f0: 7220 7468 616e 2022 0a20 2020 2020 2020  r than ".       
 00013600: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013620: 2020 2020 2020 2020 2020 2020 2260 736f              "`so
-00013630: 7572 6365 5f73 7070 602e 2229 0a20 2020  urce_spp`.").   
-00013640: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00013650: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00013660: 7373 6572 7420 286c 656e 286e 702e 756e  ssert (len(np.un
-00013670: 6971 7565 2869 6e64 6976 6964 7329 2920  ique(individs)) 
-00013680: 3c3d 206c 656e 2873 6f75 7263 655f 7370  <= len(source_sp
-00013690: 7029 2061 6e64 0a20 2020 2020 2020 2020  p) and.         
-000136a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000136b0: 702e 616c 6c28 5b69 6e64 2069 6e20 736f  p.all([ind in so
-000136c0: 7572 6365 5f73 7070 2066 6f72 2069 6e64  urce_spp for ind
-000136d0: 2069 6e20 696e 6469 7669 6473 5d29 292c   in individs])),
-000136e0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-000136f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00013700: 6069 6e64 6976 6964 7360 2063 6f6e 7461  `individs` conta
-00013710: 696e 7320 496e 6469 7669 6475 616c 2069  ins Individual i
-00013720: 6e64 6963 6573 2074 6861 7420 646f 2022  ndices that do "
-00013730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013740: 2020 2020 2020 2020 2020 2020 2022 6e6f               "no
-00013750: 7420 6578 6973 7420 696e 2060 736f 7572  t exist in `sour
-00013760: 6365 5f73 7070 602e 2229 0a0a 2020 2020  ce_spp`.")..    
-00013770: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
-00013780: 7468 6174 2061 6c6c 2053 7065 6369 6573  that all Species
-00013790: 2070 6172 616d 7320 7468 6174 206e 6565   params that nee
-000137a0: 6420 746f 206d 6174 6368 2061 7265 2074  d to match are t
-000137b0: 6865 2073 616d 650a 2020 2020 2020 2020  he same.        
-000137c0: 2020 2020 2320 696e 2074 6865 2073 6f75      # in the sou
-000137d0: 7263 6520 706f 7075 6c61 7469 6f6e 2773  rce population's
-000137e0: 2053 7065 6369 6573 2061 6e64 2069 6e20   Species and in 
-000137f0: 7468 6973 2053 7065 6369 6573 2720 706f  this Species' po
-00013800: 700a 2020 2020 2020 2020 2020 2020 7370  p.            sp
-00013810: 705f 6174 7472 735f 746f 5f63 6865 636b  p_attrs_to_check
-00013820: 203d 205b 274b 5f6c 6179 6572 272c 0a20   = ['K_layer',. 
-00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013850: 2027 7365 6c65 6374 696f 6e27 2c0a 2020   'selection',.  
-00013860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013880: 2773 6578 5f72 6174 696f 272c 0a20 2020  'sex_ratio',.   
-00013890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000138b0: 6d6f 7665 272c 0a20 2020 2020 2020 2020  move',.         
-000138c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138d0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-000138e0: 2020 2020 2020 666f 7220 6174 7472 2069        for attr i
-000138f0: 6e20 7370 705f 6174 7472 735f 746f 5f63  n spp_attrs_to_c
-00013900: 6865 636b 3a0a 2020 2020 2020 2020 2020  heck:.          
-00013910: 2020 2020 2020 6173 7365 7274 206e 702e        assert np.
-00013920: 616c 6c28 6765 7461 7474 7228 736f 7572  all(getattr(sour
-00013930: 6365 5f73 7070 2c20 6174 7472 2920 3d3d  ce_spp, attr) ==
-00013940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013950: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00013960: 6574 6174 7472 2873 656c 662c 2061 7474  etattr(self, att
-00013970: 7229 292c 2028 0a20 2020 2020 2020 2020  r)), (.         
-00013980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013990: 2020 2020 2020 2020 2022 626f 7468 2074           "both t
-000139a0: 6865 2073 6f75 7263 6520 616e 6420 7265  he source and re
-000139b0: 6369 7069 656e 7420 5370 6563 6965 7320  cipient Species 
-000139c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000139d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139e0: 2020 2020 226d 7573 7420 6861 7665 2069      "must have i
-000139f0: 6465 6e74 6963 616c 2076 616c 7565 7320  dentical values 
-00013a00: 666f 7220 220a 2020 2020 2020 2020 2020  for ".          
+00013620: 2020 2020 2020 2022 7468 6520 706f 7075         "the popu
+00013630: 6c61 7469 6f6e 2073 697a 6520 6f66 2022  lation size of "
+00013640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013660: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00013670: 6073 6f75 7263 655f 7370 7060 2e22 290a  `source_spp`.").
+00013680: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00013690: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000136a0: 2020 6173 7365 7274 2028 6c65 6e28 6e70    assert (len(np
+000136b0: 2e75 6e69 7175 6528 696e 6469 7669 6473  .unique(individs
+000136c0: 2929 203c 3d20 6c65 6e28 736f 7572 6365  )) <= len(source
+000136d0: 5f73 7070 2920 616e 640a 2020 2020 2020  _spp) and.      
+000136e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136f0: 2020 6e70 2e61 6c6c 285b 696e 6420 696e    np.all([ind in
+00013700: 2073 6f75 7263 655f 7370 7020 666f 7220   source_spp for 
+00013710: 696e 6420 696e 2069 6e64 6976 6964 735d  ind in individs]
+00013720: 2929 2c20 280a 2020 2020 2020 2020 2020  )), (.          
+00013730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013740: 2020 2260 696e 6469 7669 6473 6020 636f    "`individs` co
+00013750: 6e74 6169 6e73 2049 6e64 6976 6964 7561  ntains Individua
+00013760: 6c20 696e 6469 6365 7320 7468 6174 2064  l indices that d
+00013770: 6f20 220a 2020 2020 2020 2020 2020 2020  o ".            
+00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013790: 226e 6f74 2065 7869 7374 2069 6e20 6073  "not exist in `s
+000137a0: 6f75 7263 655f 7370 7060 2e22 290a 0a20  ource_spp`.").. 
+000137b0: 2020 2020 2020 2020 2020 2023 2063 6865             # che
+000137c0: 636b 2074 6861 7420 616c 6c20 5370 6563  ck that all Spec
+000137d0: 6965 7320 7061 7261 6d73 2074 6861 7420  ies params that 
+000137e0: 6e65 6564 2074 6f20 6d61 7463 6820 6172  need to match ar
+000137f0: 6520 7468 6520 7361 6d65 0a20 2020 2020  e the same.     
+00013800: 2020 2020 2020 2023 2069 6e20 7468 6520         # in the 
+00013810: 736f 7572 6365 2070 6f70 756c 6174 696f  source populatio
+00013820: 6e27 7320 5370 6563 6965 7320 616e 6420  n's Species and 
+00013830: 696e 2074 6869 7320 5370 6563 6965 7327  in this Species'
+00013840: 2070 6f70 0a20 2020 2020 2020 2020 2020   pop.           
+00013850: 2073 7070 5f61 7474 7273 5f74 6f5f 6368   spp_attrs_to_ch
+00013860: 6563 6b20 3d20 5b27 4b5f 6c61 7965 7227  eck = ['K_layer'
+00013870: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013890: 2020 2020 2773 656c 6563 7469 6f6e 272c      'selection',
+000138a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000138b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138c0: 2020 2027 7365 785f 7261 7469 6f27 2c0a     'sex_ratio',.
+000138d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138f0: 2020 276d 6f76 6527 2c0a 2020 2020 2020    'move',.      
+00013900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013910: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00013920: 2020 2020 2020 2020 2066 6f72 2061 7474           for att
+00013930: 7220 696e 2073 7070 5f61 7474 7273 5f74  r in spp_attrs_t
+00013940: 6f5f 6368 6563 6b3a 0a20 2020 2020 2020  o_check:.       
+00013950: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00013960: 6e70 2e61 6c6c 2867 6574 6174 7472 2873  np.all(getattr(s
+00013970: 6f75 7263 655f 7370 702c 2061 7474 7229  ource_spp, attr)
+00013980: 203d 3d0a 2020 2020 2020 2020 2020 2020   ==.            
+00013990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139a0: 2020 6765 7461 7474 7228 7365 6c66 2c20    getattr(self, 
+000139b0: 6174 7472 2929 2c20 280a 2020 2020 2020  attr)), (.      
+000139c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139d0: 2020 2020 2020 2020 2020 2020 2262 6f74              "bot
+000139e0: 6820 7468 6520 736f 7572 6365 2061 6e64  h the source and
+000139f0: 2072 6563 6970 6965 6e74 2053 7065 6369   recipient Speci
+00013a00: 6573 2022 0a20 2020 2020 2020 2020 2020  es ".           
 00013a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a20: 2020 2020 2020 2020 6622 7468 6520 6174          f"the at
-00013a30: 7472 6962 7574 6520 277b 6174 7472 7d27  tribute '{attr}'
-00013a40: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
-00013a50: 2320 6368 6563 6b20 7468 6174 2061 6c6c  # check that all
-00013a60: 2067 656e 5f61 7263 6820 7061 7261 6d73   gen_arch params
-00013a70: 2074 6861 7420 6e65 6564 2074 6f20 6d61   that need to ma
-00013a80: 7463 6820 6172 6520 7468 6520 7361 6d65  tch are the same
-00013a90: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-00013aa0: 6e20 7468 6520 736f 7572 6365 2070 6f70  n the source pop
-00013ab0: 756c 6174 696f 6e27 7320 5370 6563 6965  ulation's Specie
-00013ac0: 7320 616e 6420 7468 6973 2053 7065 6369  s and this Speci
-00013ad0: 6573 0a20 2020 2020 2020 2020 2020 2073  es.            s
-00013ae0: 6f75 7263 655f 6765 6e5f 6172 6368 203d  ource_gen_arch =
-00013af0: 2073 6f75 7263 655f 7370 702e 6765 6e5f   source_spp.gen_
-00013b00: 6172 6368 0a20 2020 2020 2020 2020 2020  arch.           
-00013b10: 2073 656c 662e 6765 6e5f 6172 6368 203d   self.gen_arch =
-00013b20: 2073 656c 662e 6765 6e5f 6172 6368 0a20   self.gen_arch. 
-00013b30: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00013b40: 7420 736f 7572 6365 5f67 656e 5f61 7263  t source_gen_arc
-00013b50: 682e 4c20 3d3d 2073 656c 662e 6765 6e5f  h.L == self.gen_
-00013b60: 6172 6368 2e4c 2c20 2822 736f 7572 6365  arch.L, ("source
-00013b70: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00013b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ba0: 2253 7065 6369 6573 206d 7573 7420 6861  "Species must ha
-00013bb0: 7665 2061 2022 0a20 2020 2020 2020 2020  ve a ".         
+00013a20: 2020 2020 2020 2022 6d75 7374 2068 6176         "must hav
+00013a30: 6520 6964 656e 7469 6361 6c20 7661 6c75  e identical valu
+00013a40: 6573 2066 6f72 2022 0a20 2020 2020 2020  es for ".       
+00013a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a60: 2020 2020 2020 2020 2020 2066 2274 6865             f"the
+00013a70: 2061 7474 7269 6275 7465 2027 7b61 7474   attribute '{att
+00013a80: 727d 2722 290a 0a20 2020 2020 2020 2020  r}'")..         
+00013a90: 2020 2023 2063 6865 636b 2074 6861 7420     # check that 
+00013aa0: 616c 6c20 6765 6e5f 6172 6368 2070 6172  all gen_arch par
+00013ab0: 616d 7320 7468 6174 206e 6565 6420 746f  ams that need to
+00013ac0: 206d 6174 6368 2061 7265 2074 6865 2073   match are the s
+00013ad0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+00013ae0: 2320 696e 2074 6865 2073 6f75 7263 6520  # in the source 
+00013af0: 706f 7075 6c61 7469 6f6e 2773 2053 7065  population's Spe
+00013b00: 6369 6573 2061 6e64 2074 6869 7320 5370  cies and this Sp
+00013b10: 6563 6965 730a 2020 2020 2020 2020 2020  ecies.          
+00013b20: 2020 736f 7572 6365 5f67 656e 5f61 7263    source_gen_arc
+00013b30: 6820 3d20 736f 7572 6365 5f73 7070 2e67  h = source_spp.g
+00013b40: 656e 5f61 7263 680a 2020 2020 2020 2020  en_arch.        
+00013b50: 2020 2020 7365 6c66 2e67 656e 5f61 7263      self.gen_arc
+00013b60: 6820 3d20 7365 6c66 2e67 656e 5f61 7263  h = self.gen_arc
+00013b70: 680a 2020 2020 2020 2020 2020 2020 6173  h.            as
+00013b80: 7365 7274 2073 6f75 7263 655f 6765 6e5f  sert source_gen_
+00013b90: 6172 6368 2e4c 203d 3d20 7365 6c66 2e67  arch.L == self.g
+00013ba0: 656e 5f61 7263 682e 4c2c 2028 2273 6f75  en_arch.L, ("sou
+00013bb0: 7263 6520 220a 2020 2020 2020 2020 2020  rce ".          
 00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013be0: 2020 2020 2273 696d 756c 6174 6564 2067      "simulated g
-00013bf0: 656e 6f6d 6520 6f66 2074 6865 2073 616d  enome of the sam
-00013c00: 6520 220a 2020 2020 2020 2020 2020 2020  e ".            
+00013be0: 2020 2022 5370 6563 6965 7320 6d75 7374     "Species must
+00013bf0: 2068 6176 6520 6120 220a 2020 2020 2020   have a ".      
+00013c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c30: 2022 6c65 6e67 7468 2061 7320 7468 6520   "length as the 
-00013c40: 7265 6370 6965 6e74 2053 7065 6369 6573  recpient Species
-00013c50: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-00013c60: 6765 6e5f 6172 6368 5f61 7474 7273 5f74  gen_arch_attrs_t
-00013c70: 6f5f 6368 6563 6b20 3d20 5b27 7365 7827  o_check = ['sex'
-00013c80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00013c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ca0: 2020 2020 2020 2020 2027 7573 655f 7473           'use_ts
-00013cb0: 6b69 7427 2c0a 2020 2020 2020 2020 2020  kit',.          
-00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cd0: 2020 2020 2020 2020 2020 2020 2027 7827               'x'
-00013ce0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00013cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d00: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00013d10: 2020 2020 2020 2320 4e4f 5445 3a20 6e6f        # NOTE: no
-00013d20: 7420 7265 7175 6972 696e 6720 7020 746f  t requiring p to
-00013d30: 2062 6520 7361 6d65 2069 6e20 626f 7468   be same in both
-00013d40: 2070 6f70 756c 6174 696f 6e73 2066 6163   populations fac
-00013d50: 696c 6974 6174 6573 0a20 2020 2020 2020  ilitates.       
-00013d60: 2020 2020 2023 2020 2020 2020 2063 7265       #       cre
-00013d70: 6174 696e 6720 6c6f 6369 2074 6861 7420  ating loci that 
-00013d80: 6469 6666 6572 2069 6e20 7374 616e 6469  differ in standi
-00013d90: 6e67 2067 656e 6574 6963 2076 6172 6961  ng genetic varia
-00013da0: 7469 6f6e 2069 6e0a 2020 2020 2020 2020  tion in.        
-00013db0: 2020 2020 2320 2020 2020 2020 7468 6520      #       the 
-00013dc0: 7477 6f20 706f 7075 6c61 7469 6f6e 732c  two populations,
-00013dd0: 206f 7220 6576 656e 206c 6f63 6920 7468   or even loci th
-00013de0: 6174 2061 7265 2066 6978 6564 2064 6966  at are fixed dif
-00013df0: 6665 7265 6e74 6c79 0a20 2020 2020 2020  ferently.       
-00013e00: 2020 2020 2023 2020 2020 2020 2069 6e20       #       in 
-00013e10: 6f6e 6520 6f72 206d 6f72 6520 706f 7075  one or more popu
-00013e20: 6c61 7469 6f6e 730a 2020 2020 2020 2020  lations.        
-00013e30: 2020 2020 2320 4e4f 5445 3a20 6d61 6b69      # NOTE: maki
-00013e40: 6e67 2069 7420 736f 2074 6861 7420 6174  ng it so that at
-00013e50: 7472 7320 6c69 6b65 206d 7574 2072 6174  trs like mut rat
-00013e60: 652c 2064 6f6d 696e 616e 6365 2070 6172  e, dominance par
-00013e70: 616d 732c 0a20 2020 2020 2020 2020 2020  ams,.           
-00013e80: 2023 2020 2020 2020 2061 6e64 2074 6865   #       and the
-00013e90: 2061 7272 6179 7320 6f66 206e 6575 7472   arrays of neutr
-00013ea0: 616c 2061 6e64 2064 656c 6574 206c 6f63  al and delet loc
-00013eb0: 6920 6e65 6564 6e27 7420 6265 2074 6865  i needn't be the
-00013ec0: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-00013ed0: 2020 2020 2073 616d 6520 286d 7574 6174       same (mutat
-00013ee0: 6564 206c 6f63 6920 616c 6d6f 7374 2063  ed loci almost c
-00013ef0: 6572 7461 696e 6c79 2077 6f75 6c64 6e27  ertainly wouldn'
-00013f00: 7420 6265 0a20 2020 2020 2020 2020 2020  t be.           
-00013f10: 2023 2020 2020 2020 2069 6620 6e6f 6e2d   #       if non-
-00013f20: 6e65 7574 7261 6c20 6d75 7461 7469 6f6e  neutral mutation
-00013f30: 2068 6173 2062 6565 6e20 6861 7070 656e   has been happen
-00013f40: 696e 6720 696e 6465 7065 6e64 656e 746c  ing independentl
-00013f50: 7920 696e 0a20 2020 2020 2020 2020 2020  y in.           
-00013f60: 2023 2020 2020 2020 2062 6f74 6820 706f   #       both po
-00013f70: 7075 6c61 7469 6f6e 7329 2e20 6974 2069  pulations). it i
-00013f80: 736e 2774 2065 6e74 6972 656c 7920 7265  sn't entirely re
-00013f90: 616c 6973 7469 6320 746f 206d 6f64 656c  alistic to model
-00013fa0: 2074 6869 730a 2020 2020 2020 2020 2020   this.          
-00013fb0: 2020 2320 2020 2020 2020 7468 6973 2077    #       this w
-00013fc0: 6179 2c20 6275 7420 616c 736f 206e 6f74  ay, but also not
-00013fd0: 2065 6e74 6972 656c 7920 756e 7265 616c   entirely unreal
-00013fe0: 6973 7469 6320 666f 7220 7468 6520 6d6f  istic for the mo
-00013ff0: 6465 6c20 746f 0a20 2020 2020 2020 2020  del to.         
-00014000: 2020 2023 2020 2020 2020 2062 6568 6176     #       behav
-00014010: 6520 7375 6368 2074 6861 7420 6c6f 6369  e such that loci
-00014020: 2074 6861 7420 7765 7265 206e 6575 7420   that were neut 
-00014030: 696e 2061 2070 6f70 756c 6174 696f 6e27  in a population'
-00014040: 7320 7072 696f 720a 2020 2020 2020 2020  s prior.        
-00014050: 2020 2020 2320 2020 2020 2020 656e 7669      #       envi
-00014060: 726f 6e6d 656e 7420 6172 6520 7375 6464  ronment are sudd
-00014070: 656e 6c79 206e 6f74 206e 6575 7472 616c  enly not neutral
-00014080: 2069 6e20 7468 6520 6e65 7720 656e 7669   in the new envi
-00014090: 726f 6e6d 656e 740a 2020 2020 2020 2020  ronment.        
-000140a0: 2020 2020 666f 7220 6174 7472 2069 6e20      for attr in 
-000140b0: 6765 6e5f 6172 6368 5f61 7474 7273 5f74  gen_arch_attrs_t
-000140c0: 6f5f 6368 6563 6b3a 0a20 2020 2020 2020  o_check:.       
-000140d0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-000140e0: 6e70 2e61 6c6c 2867 6574 6174 7472 2873  np.all(getattr(s
-000140f0: 6f75 7263 655f 6765 6e5f 6172 6368 2c20  ource_gen_arch, 
-00014100: 6174 7472 2920 3d3d 0a20 2020 2020 2020  attr) ==.       
-00014110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014120: 2020 2020 2020 2067 6574 6174 7472 2873         getattr(s
-00014130: 656c 662e 6765 6e5f 6172 6368 2c20 6174  elf.gen_arch, at
-00014140: 7472 2929 2c20 2822 626f 7468 2074 6865  tr)), ("both the
-00014150: 2073 6f75 7263 6522 0a20 2020 2020 2020   source".       
-00014160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014180: 2020 2020 2020 2020 2020 2020 2022 2061               " a
-00014190: 6e64 2072 6563 6970 6965 6e74 2053 7065  nd recipient Spe
-000141a0: 6369 6573 2720 220a 2020 2020 2020 2020  cies' ".        
+00013c20: 2020 2020 2020 2022 7369 6d75 6c61 7465         "simulate
+00013c30: 6420 6765 6e6f 6d65 206f 6620 7468 6520  d genome of the 
+00013c40: 7361 6d65 2022 0a20 2020 2020 2020 2020  same ".         
+00013c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c70: 2020 2020 226c 656e 6774 6820 6173 2074      "length as t
+00013c80: 6865 2072 6563 7069 656e 7420 5370 6563  he recpient Spec
+00013c90: 6965 732e 2229 0a20 2020 2020 2020 2020  ies.").         
+00013ca0: 2020 2067 656e 5f61 7263 685f 6174 7472     gen_arch_attr
+00013cb0: 735f 746f 5f63 6865 636b 203d 205b 2773  s_to_check = ['s
+00013cc0: 6578 272c 0a20 2020 2020 2020 2020 2020  ex',.           
+00013cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ce0: 2020 2020 2020 2020 2020 2020 2775 7365              'use
+00013cf0: 5f74 736b 6974 272c 0a20 2020 2020 2020  _tskit',.       
+00013d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d20: 2778 272c 0a20 2020 2020 2020 2020 2020  'x',.           
+00013d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d40: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00013d50: 2020 2020 2020 2020 2023 204e 4f54 453a           # NOTE:
+00013d60: 206e 6f74 2072 6571 7569 7269 6e67 2070   not requiring p
+00013d70: 2074 6f20 6265 2073 616d 6520 696e 2062   to be same in b
+00013d80: 6f74 6820 706f 7075 6c61 7469 6f6e 7320  oth populations 
+00013d90: 6661 6369 6c69 7461 7465 730a 2020 2020  facilitates.    
+00013da0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00013db0: 6372 6561 7469 6e67 206c 6f63 6920 7468  creating loci th
+00013dc0: 6174 2064 6966 6665 7220 696e 2073 7461  at differ in sta
+00013dd0: 6e64 696e 6720 6765 6e65 7469 6320 7661  nding genetic va
+00013de0: 7269 6174 696f 6e20 696e 0a20 2020 2020  riation in.     
+00013df0: 2020 2020 2020 2023 2020 2020 2020 2074         #       t
+00013e00: 6865 2074 776f 2070 6f70 756c 6174 696f  he two populatio
+00013e10: 6e73 2c20 6f72 2065 7665 6e20 6c6f 6369  ns, or even loci
+00013e20: 2074 6861 7420 6172 6520 6669 7865 6420   that are fixed 
+00013e30: 6469 6666 6572 656e 746c 790a 2020 2020  differently.    
+00013e40: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00013e50: 696e 206f 6e65 206f 7220 6d6f 7265 2070  in one or more p
+00013e60: 6f70 756c 6174 696f 6e73 0a20 2020 2020  opulations.     
+00013e70: 2020 2020 2020 2023 204e 4f54 453a 206d         # NOTE: m
+00013e80: 616b 696e 6720 6974 2073 6f20 7468 6174  aking it so that
+00013e90: 2061 7474 7273 206c 696b 6520 6d75 7420   attrs like mut 
+00013ea0: 7261 7465 2c20 646f 6d69 6e61 6e63 6520  rate, dominance 
+00013eb0: 7061 7261 6d73 2c0a 2020 2020 2020 2020  params,.        
+00013ec0: 2020 2020 2320 2020 2020 2020 616e 6420      #       and 
+00013ed0: 7468 6520 6172 7261 7973 206f 6620 6e65  the arrays of ne
+00013ee0: 7574 7261 6c20 616e 6420 6465 6c65 7420  utral and delet 
+00013ef0: 6c6f 6369 206e 6565 646e 2774 2062 6520  loci needn't be 
+00013f00: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00013f10: 2320 2020 2020 2020 7361 6d65 2028 6d75  #       same (mu
+00013f20: 7461 7465 6420 6c6f 6369 2061 6c6d 6f73  tated loci almos
+00013f30: 7420 6365 7274 6169 6e6c 7920 776f 756c  t certainly woul
+00013f40: 646e 2774 2062 650a 2020 2020 2020 2020  dn't be.        
+00013f50: 2020 2020 2320 2020 2020 2020 6966 206e      #       if n
+00013f60: 6f6e 2d6e 6575 7472 616c 206d 7574 6174  on-neutral mutat
+00013f70: 696f 6e20 6861 7320 6265 656e 2068 6170  ion has been hap
+00013f80: 7065 6e69 6e67 2069 6e64 6570 656e 6465  pening independe
+00013f90: 6e74 6c79 2069 6e0a 2020 2020 2020 2020  ntly in.        
+00013fa0: 2020 2020 2320 2020 2020 2020 626f 7468      #       both
+00013fb0: 2070 6f70 756c 6174 696f 6e73 292e 2069   populations). i
+00013fc0: 7420 6973 6e27 7420 656e 7469 7265 6c79  t isn't entirely
+00013fd0: 2072 6561 6c69 7374 6963 2074 6f20 6d6f   realistic to mo
+00013fe0: 6465 6c20 7468 6973 0a20 2020 2020 2020  del this.       
+00013ff0: 2020 2020 2023 2020 2020 2020 2074 6869       #       thi
+00014000: 7320 7761 792c 2062 7574 2061 6c73 6f20  s way, but also 
+00014010: 6e6f 7420 656e 7469 7265 6c79 2075 6e72  not entirely unr
+00014020: 6561 6c69 7374 6963 2066 6f72 2074 6865  ealistic for the
+00014030: 206d 6f64 656c 2074 6f0a 2020 2020 2020   model to.      
+00014040: 2020 2020 2020 2320 2020 2020 2020 6265        #       be
+00014050: 6861 7665 2073 7563 6820 7468 6174 206c  have such that l
+00014060: 6f63 6920 7468 6174 2077 6572 6520 6e65  oci that were ne
+00014070: 7574 2069 6e20 6120 706f 7075 6c61 7469  ut in a populati
+00014080: 6f6e 2773 2070 7269 6f72 0a20 2020 2020  on's prior.     
+00014090: 2020 2020 2020 2023 2020 2020 2020 2065         #       e
+000140a0: 6e76 6972 6f6e 6d65 6e74 2061 7265 2073  nvironment are s
+000140b0: 7564 6465 6e6c 7920 6e6f 7420 6e65 7574  uddenly not neut
+000140c0: 7261 6c20 696e 2074 6865 206e 6577 2065  ral in the new e
+000140d0: 6e76 6972 6f6e 6d65 6e74 0a20 2020 2020  nvironment.     
+000140e0: 2020 2020 2020 2066 6f72 2061 7474 7220         for attr 
+000140f0: 696e 2067 656e 5f61 7263 685f 6174 7472  in gen_arch_attr
+00014100: 735f 746f 5f63 6865 636b 3a0a 2020 2020  s_to_check:.    
+00014110: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00014120: 7274 206e 702e 616c 6c28 6765 7461 7474  rt np.all(getatt
+00014130: 7228 736f 7572 6365 5f67 656e 5f61 7263  r(source_gen_arc
+00014140: 682c 2061 7474 7229 203d 3d0a 2020 2020  h, attr) ==.    
+00014150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014160: 2020 2020 2020 2020 2020 6765 7461 7474            getatt
+00014170: 7228 7365 6c66 2e67 656e 5f61 7263 682c  r(self.gen_arch,
+00014180: 2061 7474 7229 292c 2028 2262 6f74 6820   attr)), ("both 
+00014190: 7468 6520 736f 7572 6365 220a 2020 2020  the source".    
+000141a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000141b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000141c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141d0: 2020 2020 2020 2020 2020 2020 2247 656e              "Gen
-000141e0: 6f6d 6963 4172 6368 6974 6563 7475 7265  omicArchitecture
-000141f0: 7320 220a 2020 2020 2020 2020 2020 2020  s ".            
+000141d0: 2220 616e 6420 7265 6369 7069 656e 7420  " and recipient 
+000141e0: 5370 6563 6965 7327 2022 0a20 2020 2020  Species' ".     
+000141f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014220: 2020 2020 2020 2020 226f 626a 6563 7473          "objects
-00014230: 206d 7573 7420 6861 7665 2022 0a20 2020   must have ".   
+00014210: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00014220: 4765 6e6f 6d69 6341 7263 6869 7465 6374  GenomicArchitect
+00014230: 7572 6573 2022 0a20 2020 2020 2020 2020  ures ".         
 00014240: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014270: 2022 6964 656e 7469 6361 6c20 7661 6c75   "identical valu
-00014280: 6573 2066 6f72 2074 6865 2022 0a20 2020  es for the ".   
+00014260: 2020 2020 2020 2020 2020 2022 6f62 6a65             "obje
+00014270: 6374 7320 6d75 7374 2068 6176 6520 220a  cts must have ".
+00014280: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014290: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000142a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142c0: 2066 2261 7474 7269 6275 7465 2027 7b61   f"attribute '{a
-000142d0: 7474 727d 2722 290a 2020 2020 2020 2020  ttr}'").        
-000142e0: 2020 2020 2320 6368 6563 6b20 7265 636f      # check reco
-000142f0: 6d62 696e 6174 696f 6e20 6174 7472 6962  mbination attrib
-00014300: 7574 6573 0a20 2020 2020 2020 2020 2020  utes.           
-00014310: 2072 6563 6f6d 625f 6174 7472 735f 746f   recomb_attrs_to
-00014320: 5f63 6865 636b 203d 205b 275f 7261 7465  _check = ['_rate
-00014330: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
-00014340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014350: 2020 2020 2020 2020 2027 5f72 5f64 6973           '_r_dis
-00014360: 7472 5f61 6c70 6861 272c 0a20 2020 2020  tr_alpha',.     
-00014370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142b0: 2020 2020 2269 6465 6e74 6963 616c 2076      "identical v
+000142c0: 616c 7565 7320 666f 7220 7468 6520 220a  alues for the ".
+000142d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014300: 2020 2020 6622 6174 7472 6962 7574 6520      f"attribute 
+00014310: 277b 6174 7472 7d27 2229 0a20 2020 2020  '{attr}'").     
+00014320: 2020 2020 2020 2023 2063 6865 636b 2072         # check r
+00014330: 6563 6f6d 6269 6e61 7469 6f6e 2061 7474  ecombination att
+00014340: 7269 6275 7465 730a 2020 2020 2020 2020  ributes.        
+00014350: 2020 2020 7265 636f 6d62 5f61 7474 7273      recomb_attrs
+00014360: 5f74 6f5f 6368 6563 6b20 3d20 5b27 5f72  _to_check = ['_r
+00014370: 6174 6573 272c 0a20 2020 2020 2020 2020  ates',.         
 00014380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014390: 275f 725f 6469 7374 725f 6265 7461 272c  '_r_distr_beta',
-000143a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014390: 2020 2020 2020 2020 2020 2020 275f 725f              '_r_
+000143a0: 6469 7374 725f 616c 7068 6127 2c0a 2020  distr_alpha',.  
 000143b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143c0: 2020 2020 2020 275f 6a69 7474 6572 5f62        '_jitter_b
-000143d0: 7265 616b 706f 696e 7473 272c 0a20 2020  reakpoints',.   
-000143e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143d0: 2020 2027 5f72 5f64 6973 7472 5f62 6574     '_r_distr_bet
+000143e0: 6127 2c0a 2020 2020 2020 2020 2020 2020  a',.            
 000143f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014400: 205d 0a20 2020 2020 2020 2020 2020 2066   ].            f
-00014410: 6f72 2061 7474 7220 696e 2072 6563 6f6d  or attr in recom
-00014420: 625f 6174 7472 735f 746f 5f63 6865 636b  b_attrs_to_check
-00014430: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014440: 2020 6173 7365 7274 206e 702e 616c 6c28    assert np.all(
-00014450: 6765 7461 7474 7228 736f 7572 6365 5f67  getattr(source_g
-00014460: 656e 5f61 7263 682e 7265 636f 6d62 696e  en_arch.recombin
-00014470: 6174 696f 6e73 2c20 6174 7472 2920 3d3d  ations, attr) ==
-00014480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014490: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-000144a0: 6574 6174 7472 2873 656c 662e 6765 6e5f  etattr(self.gen_
-000144b0: 6172 6368 2e72 6563 6f6d 6269 6e61 7469  arch.recombinati
-000144c0: 6f6e 732c 2061 7474 7229 292c 2028 0a20  ons, attr)), (. 
+00014400: 2020 2020 2020 2020 2027 5f6a 6974 7465           '_jitte
+00014410: 725f 6272 6561 6b70 6f69 6e74 7327 2c0a  r_breakpoints',.
+00014420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014440: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+00014450: 2020 666f 7220 6174 7472 2069 6e20 7265    for attr in re
+00014460: 636f 6d62 5f61 7474 7273 5f74 6f5f 6368  comb_attrs_to_ch
+00014470: 6563 6b3a 0a20 2020 2020 2020 2020 2020  eck:.           
+00014480: 2020 2020 2061 7373 6572 7420 6e70 2e61       assert np.a
+00014490: 6c6c 2867 6574 6174 7472 2873 6f75 7263  ll(getattr(sourc
+000144a0: 655f 6765 6e5f 6172 6368 2e72 6563 6f6d  e_gen_arch.recom
+000144b0: 6269 6e61 7469 6f6e 732c 2061 7474 7229  binations, attr)
+000144c0: 203d 3d0a 2020 2020 2020 2020 2020 2020   ==.            
 000144d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014500: 2020 2020 2262 6f74 6820 7468 6520 736f      "both the so
-00014510: 7572 6365 2022 0a20 2020 2020 2020 2020  urce ".         
+000144e0: 2020 6765 7461 7474 7228 7365 6c66 2e67    getattr(self.g
+000144f0: 656e 5f61 7263 682e 7265 636f 6d62 696e  en_arch.recombin
+00014500: 6174 696f 6e73 2c20 6174 7472 2929 2c20  ations, attr)), 
+00014510: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
 00014520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014540: 2020 2020 2020 2020 2020 2020 2261 6e64              "and
-00014550: 2072 6563 6970 6965 6e74 2053 7065 6369   recipient Speci
-00014560: 6573 2720 220a 2020 2020 2020 2020 2020  es' ".          
+00014540: 2020 2020 2020 2022 626f 7468 2074 6865         "both the
+00014550: 2073 6f75 7263 6520 220a 2020 2020 2020   source ".      
+00014560: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014590: 2020 2020 2020 2020 2020 2022 5265 636f             "Reco
-000145a0: 6d62 696e 6174 696f 6e73 206f 626a 6563  mbinations objec
-000145b0: 7473 2022 0a20 2020 2020 2020 2020 2020  ts ".           
+00014580: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00014590: 616e 6420 7265 6369 7069 656e 7420 5370  and recipient Sp
+000145a0: 6563 6965 7327 2022 0a20 2020 2020 2020  ecies' ".       
+000145b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000145c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145e0: 2020 2020 2020 2020 2020 226d 7573 7420            "must 
-000145f0: 6861 7665 2069 6465 6e74 6963 616c 2022  have identical "
-00014600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000145d0: 2020 2020 2020 2020 2020 2020 2020 2252                "R
+000145e0: 6563 6f6d 6269 6e61 7469 6f6e 7320 6f62  ecombinations ob
+000145f0: 6a65 6374 7320 220a 2020 2020 2020 2020  jects ".        
+00014600: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014630: 2020 2020 2020 2276 616c 7565 7320 666f        "values fo
-00014640: 7220 7468 6520 220a 2020 2020 2020 2020  r the ".        
+00014620: 2020 2020 2020 2020 2020 2020 2022 6d75               "mu
+00014630: 7374 2068 6176 6520 6964 656e 7469 6361  st have identica
+00014640: 6c20 220a 2020 2020 2020 2020 2020 2020  l ".            
 00014650: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014670: 2020 2020 2020 2020 2020 2020 2066 2261               f"a
-00014680: 7474 7269 6275 7465 2027 7b61 7474 727d  ttribute '{attr}
-00014690: 2722 290a 0a20 2020 2020 2020 2020 2020  '")..           
-000146a0: 2023 2063 6865 636b 2074 7261 6974 7320   # check traits 
-000146b0: 616e 6420 7468 6569 7220 7061 7261 6d73  and their params
-000146c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000146d0: 7365 6c66 2e67 656e 5f61 7263 682e 7472  self.gen_arch.tr
-000146e0: 6169 7473 2069 7320 4e6f 6e65 3a0a 2020  aits is None:.  
-000146f0: 2020 2020 2020 2020 2020 2020 2020 6173                as
-00014700: 7365 7274 2073 6f75 7263 655f 6765 6e5f  sert source_gen_
-00014710: 6172 6368 2e74 7261 6974 7320 6973 204e  arch.traits is N
-00014720: 6f6e 652c 2028 2249 6e64 6976 6964 7561  one, ("Individua
-00014730: 6c73 2022 0a20 2020 2020 2020 2020 2020  ls ".           
-00014740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014760: 2020 2020 2020 2022 6672 6f6d 2061 2053         "from a S
-00014770: 7065 6369 6573 2077 6974 6820 220a 2020  pecies with ".  
+00014670: 2020 2020 2020 2020 2022 7661 6c75 6573           "values
+00014680: 2066 6f72 2074 6865 2022 0a20 2020 2020   for the ".     
+00014690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146c0: 6622 6174 7472 6962 7574 6520 277b 6174  f"attribute '{at
+000146d0: 7472 7d27 2229 0a0a 2020 2020 2020 2020  tr}'")..        
+000146e0: 2020 2020 2320 6368 6563 6b20 7472 6169      # check trai
+000146f0: 7473 2061 6e64 2074 6865 6972 2070 6172  ts and their par
+00014700: 616d 730a 2020 2020 2020 2020 2020 2020  ams.            
+00014710: 6966 2073 656c 662e 6765 6e5f 6172 6368  if self.gen_arch
+00014720: 2e74 7261 6974 7320 6973 204e 6f6e 653a  .traits is None:
+00014730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014740: 2061 7373 6572 7420 736f 7572 6365 5f67   assert source_g
+00014750: 656e 5f61 7263 682e 7472 6169 7473 2069  en_arch.traits i
+00014760: 7320 4e6f 6e65 2c20 2822 496e 6469 7669  s None, ("Indivi
+00014770: 6475 616c 7320 220a 2020 2020 2020 2020  duals ".        
 00014780: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147b0: 2254 7261 6974 7320 6361 6e6e 6f74 2062  "Traits cannot b
-000147c0: 6520 6164 6465 6420 746f 2061 2022 0a20  e added to a ". 
+000147a0: 2020 2020 2020 2020 2020 2266 726f 6d20            "from 
+000147b0: 6120 5370 6563 6965 7320 7769 7468 2022  a Species with "
+000147c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000147d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000147e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014800: 2022 5370 6563 6965 7320 7769 7468 6f75   "Species withou
-00014810: 7420 7468 656d 2e22 290a 2020 2020 2020  t them.").      
-00014820: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00014830: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00014840: 7274 2028 6c65 6e28 736f 7572 6365 5f67  rt (len(source_g
-00014850: 656e 5f61 7263 682e 7472 6169 7473 2920  en_arch.traits) 
-00014860: 3d3d 0a20 2020 2020 2020 2020 2020 2020  ==.             
-00014870: 2020 2020 2020 2020 2020 206c 656e 2873             len(s
-00014880: 656c 662e 6765 6e5f 6172 6368 2e74 7261  elf.gen_arch.tra
-00014890: 6974 7329 292c 2028 2254 6865 2073 6f75  its)), ("The sou
-000148a0: 7263 6520 706f 7075 6c61 7469 6f6e 2773  rce population's
-000148b0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-000148c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148d0: 2020 2020 2020 2020 2020 2022 5370 6563             "Spec
-000148e0: 6965 7320 6f62 6a65 6374 206d 7573 7420  ies object must 
-000148f0: 6861 7665 2074 6865 2022 0a20 2020 2020  have the ".     
+000147f0: 2020 2022 5472 6169 7473 2063 616e 6e6f     "Traits canno
+00014800: 7420 6265 2061 6464 6564 2074 6f20 6120  t be added to a 
+00014810: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00014820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014840: 2020 2020 2253 7065 6369 6573 2077 6974      "Species wit
+00014850: 686f 7574 2074 6865 6d2e 2229 0a20 2020  hout them.").   
+00014860: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00014870: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00014880: 7373 6572 7420 286c 656e 2873 6f75 7263  ssert (len(sourc
+00014890: 655f 6765 6e5f 6172 6368 2e74 7261 6974  e_gen_arch.trait
+000148a0: 7329 203d 3d0a 2020 2020 2020 2020 2020  s) ==.          
+000148b0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+000148c0: 6e28 7365 6c66 2e67 656e 5f61 7263 682e  n(self.gen_arch.
+000148d0: 7472 6169 7473 2929 2c20 2822 5468 6520  traits)), ("The 
+000148e0: 736f 7572 6365 2070 6f70 756c 6174 696f  source populatio
+000148f0: 6e27 7320 220a 2020 2020 2020 2020 2020  n's ".          
 00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014920: 2020 2022 7361 6d65 206e 756d 6265 7220     "same number 
-00014930: 6f66 2054 7261 6974 7320 220a 2020 2020  of Traits ".    
+00014910: 2020 2020 2020 2020 2020 2020 2020 2253                "S
+00014920: 7065 6369 6573 206f 626a 6563 7420 6d75  pecies object mu
+00014930: 7374 2068 6176 6520 7468 6520 220a 2020  st have the ".  
 00014940: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014960: 2020 2020 2261 7320 7468 6520 7265 6369      "as the reci
-00014970: 7069 656e 7420 5370 6563 6965 732e 2229  pient Species.")
-00014980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014990: 2074 7274 5f61 7474 7273 5f74 6f5f 6368   trt_attrs_to_ch
-000149a0: 6563 6b20 3d20 5b27 6e61 6d65 272c 0a20  eck = ['name',. 
-000149b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149d0: 2020 2020 2027 7068 6927 2c0a 2020 2020       'phi',.    
-000149e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a00: 2020 276c 7972 5f6e 756d 272c 0a20 2020    'lyr_num',.   
-00014a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014960: 2020 2020 2020 2273 616d 6520 6e75 6d62        "same numb
+00014970: 6572 206f 6620 5472 6169 7473 2022 0a20  er of Traits ". 
+00014980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149a0: 2020 2020 2020 2022 6173 2074 6865 2072         "as the r
+000149b0: 6563 6970 6965 6e74 2053 7065 6369 6573  ecipient Species
+000149c0: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+000149d0: 2020 2020 7472 745f 6174 7472 735f 746f      trt_attrs_to
+000149e0: 5f63 6865 636b 203d 205b 276e 616d 6527  _check = ['name'
+000149f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a10: 2020 2020 2020 2020 2770 6869 272c 0a20          'phi',. 
 00014a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a30: 2020 2027 6d61 785f 616c 7068 615f 6d61     'max_alpha_ma
-00014a40: 6727 2c0a 2020 2020 2020 2020 2020 2020  g',.            
+00014a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a40: 2020 2020 2027 6c79 725f 6e75 6d27 2c0a       'lyr_num',.
 00014a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a60: 2020 2020 2020 2020 2020 2767 616d 6d61            'gamma
-00014a70: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00014a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a90: 2020 2020 2020 2020 2027 756e 6976 5f61           'univ_a
-00014aa0: 6476 272c 0a20 2020 2020 2020 2020 2020  dv',.           
-00014ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ac0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00014ad0: 2020 2020 2020 2020 2020 2020 2320 4e4f              # NO
-00014ae0: 5445 3a20 6e6f 7420 7265 7175 6972 696e  TE: not requirin
-00014af0: 6720 276e 5f6c 6f63 6927 2074 6f20 6265  g 'n_loci' to be
-00014b00: 2074 6865 2073 616d 6520 6265 6361 7573   the same becaus
-00014b10: 6520 7468 6579 2772 650a 2020 2020 2020  e they're.      
-00014b20: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00014b30: 2020 756e 6c69 6b65 6c79 2074 6f20 6265    unlikely to be
-00014b40: 2074 6865 2073 616d 6520 6966 206e 6f6e   the same if non
-00014b50: 2d6e 6575 7472 616c 206d 7574 6174 696f  -neutral mutatio
-00014b60: 6e20 0a20 2020 2020 2020 2020 2020 2020  n .             
-00014b70: 2020 2023 2020 2020 2020 2068 6173 2062     #       has b
-00014b80: 6565 6e20 6861 7070 656e 696e 6720 696e  een happening in
-00014b90: 6465 7065 6e64 656e 746c 7920 696e 2062  dependently in b
-00014ba0: 6f74 6820 706f 7075 6c61 7469 6f6e 730a  oth populations.
-00014bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bc0: 666f 7220 6e2c 2074 7274 2069 6e20 7365  for n, trt in se
-00014bd0: 6c66 2e67 656e 5f61 7263 682e 7472 6169  lf.gen_arch.trai
-00014be0: 7473 2e69 7465 6d73 2829 3a0a 2020 2020  ts.items():.    
-00014bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c00: 666f 7220 6174 7472 2069 6e20 7472 745f  for attr in trt_
-00014c10: 6174 7473 5f74 6f5f 6368 6563 6b3a 0a20  atts_to_check:. 
-00014c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c30: 2020 2020 2020 2061 7373 6572 7420 6e70         assert np
-00014c40: 2e61 6c6c 2867 6574 6174 7472 2874 7274  .all(getattr(trt
-00014c50: 2c20 6174 7472 2920 3d3d 0a20 2020 2020  , attr) ==.     
-00014c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c70: 2020 2020 2020 2020 2020 2067 6574 6174             getat
-00014c80: 7472 2873 6f75 7263 655f 6765 6e5f 6172  tr(source_gen_ar
-00014c90: 6368 2e74 7261 6974 735b 6e5d 2c20 6174  ch.traits[n], at
-00014ca0: 7472 2929 2c20 280a 2020 2020 2020 2020  tr)), (.        
-00014cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cd0: 2066 2241 7474 7269 6275 7465 2027 7b61   f"Attribute '{a
-00014ce0: 7474 727d 2720 6f66 2074 7261 6974 207b  ttr}' of trait {
-00014cf0: 6e7d 2022 0a20 2020 2020 2020 2020 2020  n} ".           
+00014a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a70: 2020 2020 2020 276d 6178 5f61 6c70 6861        'max_alpha
+00014a80: 5f6d 6167 272c 0a20 2020 2020 2020 2020  _mag',.         
+00014a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014aa0: 2020 2020 2020 2020 2020 2020 2027 6761               'ga
+00014ab0: 6d6d 6127 2c0a 2020 2020 2020 2020 2020  mma',.          
+00014ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ad0: 2020 2020 2020 2020 2020 2020 2775 6e69              'uni
+00014ae0: 765f 6164 7627 2c0a 2020 2020 2020 2020  v_adv',.        
+00014af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b00: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
+00014b10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00014b20: 204e 4f54 453a 206e 6f74 2072 6571 7569   NOTE: not requi
+00014b30: 7269 6e67 2027 6e5f 6c6f 6369 2720 746f  ring 'n_loci' to
+00014b40: 2062 6520 7468 6520 7361 6d65 2062 6563   be the same bec
+00014b50: 6175 7365 2074 6865 7927 7265 0a20 2020  ause they're.   
+00014b60: 2020 2020 2020 2020 2020 2020 2023 2020               #  
+00014b70: 2020 2020 2075 6e6c 696b 656c 7920 746f       unlikely to
+00014b80: 2062 6520 7468 6520 7361 6d65 2069 6620   be the same if 
+00014b90: 6e6f 6e2d 6e65 7574 7261 6c20 6d75 7461  non-neutral muta
+00014ba0: 7469 6f6e 200a 2020 2020 2020 2020 2020  tion .          
+00014bb0: 2020 2020 2020 2320 2020 2020 2020 6861        #       ha
+00014bc0: 7320 6265 656e 2068 6170 7065 6e69 6e67  s been happening
+00014bd0: 2069 6e64 6570 656e 6465 6e74 6c79 2069   independently i
+00014be0: 6e20 626f 7468 2070 6f70 756c 6174 696f  n both populatio
+00014bf0: 6e73 0a20 2020 2020 2020 2020 2020 2020  ns.             
+00014c00: 2020 2066 6f72 206e 2c20 7472 7420 696e     for n, trt in
+00014c10: 2073 656c 662e 6765 6e5f 6172 6368 2e74   self.gen_arch.t
+00014c20: 7261 6974 732e 6974 656d 7328 293a 0a20  raits.items():. 
+00014c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c40: 2020 2066 6f72 2061 7474 7220 696e 2074     for attr in t
+00014c50: 7274 5f61 7474 735f 746f 5f63 6865 636b  rt_atts_to_check
+00014c60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014c70: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00014c80: 206e 702e 616c 6c28 6765 7461 7474 7228   np.all(getattr(
+00014c90: 7472 742c 2061 7474 7229 203d 3d0a 2020  trt, attr) ==.  
+00014ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cb0: 2020 2020 2020 2020 2020 2020 2020 6765                ge
+00014cc0: 7461 7474 7228 736f 7572 6365 5f67 656e  tattr(source_gen
+00014cd0: 5f61 7263 682e 7472 6169 7473 5b6e 5d2c  _arch.traits[n],
+00014ce0: 2061 7474 7229 292c 2028 0a20 2020 2020   attr)), (.     
+00014cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00014d20: 696e 2074 6865 2073 6f75 7263 6520 706f  in the source po
-00014d30: 7075 6c61 7469 6f6e 2773 2053 7065 6369  pulation's Speci
-00014d40: 6573 2022 0a20 2020 2020 2020 2020 2020  es ".           
+00014d10: 2020 2020 6622 4174 7472 6962 7574 6520      f"Attribute 
+00014d20: 277b 6174 7472 7d27 206f 6620 7472 6169  '{attr}' of trai
+00014d30: 7420 7b6e 7d20 220a 2020 2020 2020 2020  t {n} ".        
+00014d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00014d70: 6f62 6a65 6374 206d 7573 7420 6265 2074  object must be t
-00014d80: 6865 2073 616d 6520 6173 2022 0a20 2020  he same as ".   
+00014d60: 2020 2269 6e20 7468 6520 736f 7572 6365    "in the source
+00014d70: 2070 6f70 756c 6174 696f 6e27 7320 5370   population's Sp
+00014d80: 6563 6965 7320 220a 2020 2020 2020 2020  ecies ".        
 00014d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014db0: 2020 2020 2020 2022 7468 6174 2061 7474         "that att
-00014dc0: 7269 6275 7465 2069 6e20 7468 6520 7265  ribute in the re
-00014dd0: 6369 7069 656e 7420 220a 2020 2020 2020  cipient ".      
+00014db0: 2020 226f 626a 6563 7420 6d75 7374 2062    "object must b
+00014dc0: 6520 7468 6520 7361 6d65 2061 7320 220a  e the same as ".
+00014dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e00: 2020 2020 2270 6f70 756c 6174 696f 6e27      "population'
-00014e10: 7320 5370 6563 6965 732e 2229 0a0a 2020  s Species.")..  
-00014e20: 2020 2020 2020 2020 2020 2320 6465 6570            # deep
-00014e30: 636f 7079 2074 6865 2073 6f75 7263 655f  copy the source_
-00014e40: 7370 7020 6f62 6a65 6374 2c20 7468 656e  spp object, then
-00014e50: 2073 7562 7365 7420 746f 206f 6e6c 7920   subset to only 
-00014e60: 7468 6520 736f 7572 6365 0a20 2020 2020  the source.     
-00014e70: 2020 2020 2020 2023 2069 6e64 6976 6964         # individ
-00014e80: 7561 6c73 206e 6565 6465 642c 2077 6869  uals needed, whi
-00014e90: 6368 2077 696c 6c20 616c 736f 2073 6f72  ch will also sor
-00014ea0: 7420 616e 6420 7369 6d70 6c69 6679 2074  t and simplify t
-00014eb0: 6865 0a20 2020 2020 2020 2020 2020 2023  he.            #
-00014ec0: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
-00014ed0: 2073 6f20 7468 6174 2061 6c6c 2065 7874   so that all ext
-00014ee0: 616e 7420 6e6f 6465 7320 6172 6520 6e6f  ant nodes are no
-00014ef0: 6465 7320 746f 2062 6520 756e 696f 6e65  des to be unione
-00014f00: 640a 2020 2020 2020 2020 2020 2020 2320  d.            # 
-00014f10: 696e 746f 2074 6869 7320 5370 6563 6965  into this Specie
-00014f20: 7327 2054 6162 6c65 436f 6c6c 6563 7469  s' TableCollecti
-00014f30: 6f6e 200a 2020 2020 2020 2020 2020 2020  on .            
-00014f40: 736f 7572 6365 5f73 7070 5f63 6f70 7920  source_spp_copy 
-00014f50: 3d20 6465 6570 636f 7079 2873 6f75 7263  = deepcopy(sourc
-00014f60: 655f 7370 7029 0a20 2020 2020 2020 2020  e_spp).         
-00014f70: 2020 2023 2067 6574 2069 6e64 6976 6964     # get individ
-00014f80: 7561 6c73 2066 726f 6d20 7468 6520 6769  uals from the gi
-00014f90: 7665 6e20 5370 6563 6965 7320 6f62 6a65  ven Species obje
-00014fa0: 6374 0a20 2020 2020 2020 2020 2020 2069  ct.            i
-00014fb0: 6620 696e 6469 7669 6473 2069 7320 6e6f  f individs is no
-00014fc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00014fd0: 2020 2020 2020 2020 696e 6469 7669 6473          individs
-00014fe0: 5f74 6f5f 7265 6d6f 7665 203d 205b 696e  _to_remove = [in
-00014ff0: 6420 666f 7220 696e 6420 696e 0a20 2020  d for ind in.   
-00015000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015020: 2020 2073 6f75 7263 655f 7370 705f 636f     source_spp_co
-00015030: 7079 2069 6620 696e 6420 6e6f 7420 696e  py if ind not in
-00015040: 2069 6e64 6976 6964 735d 0a20 2020 2020   individs].     
-00015050: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00015060: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
-00015070: 6976 6964 735f 746f 5f72 656d 6f76 6520  ivids_to_remove 
-00015080: 3d20 5b2a 736f 7572 6365 5f73 7070 5f63  = [*source_spp_c
-00015090: 6f70 795d 5b6e 3a5d 0a20 2020 2020 2020  opy][n:].       
-000150a0: 2020 2020 2073 6f75 7263 655f 7370 705f       source_spp_
-000150b0: 636f 7079 2e5f 7265 6d6f 7665 5f69 6e64  copy._remove_ind
-000150c0: 6976 6964 7561 6c73 2869 6e64 6976 6964  ividuals(individ
-000150d0: 733d 696e 6469 7669 6473 5f74 6f5f 7265  s=individs_to_re
-000150e0: 6d6f 7665 290a 2020 2020 2020 2020 2020  move).          
-000150f0: 2020 6966 2069 6e64 6976 6964 7320 6973    if individs is
-00015100: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00015110: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00015120: 7420 6c65 6e28 736f 7572 6365 5f73 7070  t len(source_spp
-00015130: 5f63 6f70 7929 203d 3d20 6c65 6e28 696e  _copy) == len(in
-00015140: 6469 7669 6473 290a 2020 2020 2020 2020  divids).        
-00015150: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00015160: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00015170: 206c 656e 2873 6f75 7263 655f 7370 705f   len(source_spp_
-00015180: 636f 7079 2920 3d3d 206e 0a0a 2020 2020  copy) == n..    
-00015190: 2020 2020 2020 2020 2320 6761 7468 6572          # gather
-000151a0: 2061 6c6c 2072 656d 6169 6e69 6e67 2049   all remaining I
-000151b0: 6e64 6976 6964 7561 6c73 2069 6e74 6f20  ndividuals into 
-000151c0: 6120 6c69 7374 0a20 2020 2020 2020 2020  a list.         
-000151d0: 2020 2069 6e64 6976 6964 7320 3d20 5b2a     individs = [*
-000151e0: 736f 7572 6365 5f73 7070 5f63 6f70 792e  source_spp_copy.
-000151f0: 7661 6c75 6573 2829 5d0a 0a20 2020 2020  values()]..     
-00015200: 2020 2020 2020 2023 2064 6f75 626c 652d         # double-
-00015210: 6368 6563 6b20 7468 6174 2074 6865 2073  check that the s
-00015220: 6f75 7263 655f 7370 705f 636f 7079 2773  ource_spp_copy's
-00015230: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
-00015240: 2068 6173 2062 6565 6e0a 2020 2020 2020   has been.      
-00015250: 2020 2020 2020 2320 736f 7274 6564 2061        # sorted a
-00015260: 6e64 2073 696d 706c 6966 6965 640a 2020  nd simplified.  
-00015270: 2020 2020 2020 2020 2020 736f 7572 6365            source
-00015280: 5f73 7070 5f63 6f70 792e 5f73 6f72 745f  _spp_copy._sort_
-00015290: 616e 645f 7369 6d70 6c69 6679 5f74 6162  and_simplify_tab
-000152a0: 6c65 5f63 6f6c 6c65 6374 696f 6e28 290a  le_collection().
-000152b0: 0a20 2020 2020 2020 2020 2020 2023 2066  .            # f
-000152c0: 6f72 6d61 7420 5461 626c 6543 6f6c 6c65  ormat TableColle
-000152d0: 6374 696f 6e20 616e 6420 7265 7475 726e  ction and return
-000152e0: 2074 6865 206c 6973 7420 6f66 206e 6577   the list of new
-000152f0: 2067 6e78 2049 6e64 6976 6964 2069 6478   gnx Individ idx
-00015300: 730a 2020 2020 2020 2020 2020 2020 2320  s.            # 
-00015310: 7468 6174 2054 6162 6c65 2773 2069 6e64  that Table's ind
-00015320: 6976 6964 7561 6c73 2077 696c 6c20 6265  ividuals will be
-00015330: 2061 7373 6967 6e65 6420 772f 696e 2074   assigned w/in t
-00015340: 6869 7320 5370 6563 6965 730a 2020 2020  his Species.    
-00015350: 2020 2020 2020 2020 736f 7572 6365 5f74          source_t
-00015360: 6320 3d20 736f 7572 6365 5f73 7070 5f63  c = source_spp_c
-00015370: 6f70 792e 5f74 630a 2020 2020 2020 2020  opy._tc.        
-00015380: 2020 2020 6e65 7874 5f67 6e78 5f69 6478      next_gnx_idx
-00015390: 7320 3d20 5f70 7265 705f 7473 6b69 745f  s = _prep_tskit_
-000153a0: 7461 6263 6f6c 6c5f 666f 725f 676e 785f  tabcoll_for_gnx_
-000153b0: 7370 705f 756e 696f 6e28 7463 3d73 6f75  spp_union(tc=sou
-000153c0: 7263 655f 7463 2c0a 2020 2020 2020 2020  rce_tc,.        
-000153d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015400: 7265 6369 705f 7370 703d 7365 6c66 2c0a  recip_spp=self,.
-00015410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015440: 2020 2020 2020 2020 636f 6f72 6473 3d63          coords=c
-00015450: 6f6f 7264 732c 0a20 2020 2020 2020 2020  oords,.         
-00015460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015480: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015490: 6f75 7263 655f 736f 6674 7761 7265 3d27  ource_software='
-000154a0: 676e 7827 2c0a 2020 2020 2020 2020 2020  gnx',.          
-000154b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014df0: 2020 2020 2020 2020 2020 2274 6861 7420            "that 
+00014e00: 6174 7472 6962 7574 6520 696e 2074 6865  attribute in the
+00014e10: 2072 6563 6970 6965 6e74 2022 0a20 2020   recipient ".   
+00014e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e40: 2020 2020 2020 2022 706f 7075 6c61 7469         "populati
+00014e50: 6f6e 2773 2053 7065 6369 6573 2e22 290a  on's Species.").
+00014e60: 0a20 2020 2020 2020 2020 2020 2023 2064  .            # d
+00014e70: 6565 7063 6f70 7920 7468 6520 736f 7572  eepcopy the sour
+00014e80: 6365 5f73 7070 206f 626a 6563 742c 2074  ce_spp object, t
+00014e90: 6865 6e20 7375 6273 6574 2074 6f20 6f6e  hen subset to on
+00014ea0: 6c79 2074 6865 2073 6f75 7263 650a 2020  ly the source.  
+00014eb0: 2020 2020 2020 2020 2020 2320 696e 6469            # indi
+00014ec0: 7669 6475 616c 7320 6e65 6564 6564 2c20  viduals needed, 
+00014ed0: 7768 6963 6820 7769 6c6c 2061 6c73 6f20  which will also 
+00014ee0: 736f 7274 2061 6e64 2073 696d 706c 6966  sort and simplif
+00014ef0: 7920 7468 650a 2020 2020 2020 2020 2020  y the.          
+00014f00: 2020 2320 5461 626c 6543 6f6c 6c65 6374    # TableCollect
+00014f10: 696f 6e20 736f 2074 6861 7420 616c 6c20  ion so that all 
+00014f20: 6578 7461 6e74 206e 6f64 6573 2061 7265  extant nodes are
+00014f30: 206e 6f64 6573 2074 6f20 6265 2075 6e69   nodes to be uni
+00014f40: 6f6e 6564 0a20 2020 2020 2020 2020 2020  oned.           
+00014f50: 2023 2069 6e74 6f20 7468 6973 2053 7065   # into this Spe
+00014f60: 6369 6573 2720 5461 626c 6543 6f6c 6c65  cies' TableColle
+00014f70: 6374 696f 6e20 0a20 2020 2020 2020 2020  ction .         
+00014f80: 2020 2073 6f75 7263 655f 7370 705f 636f     source_spp_co
+00014f90: 7079 203d 2064 6565 7063 6f70 7928 736f  py = deepcopy(so
+00014fa0: 7572 6365 5f73 7070 290a 2020 2020 2020  urce_spp).      
+00014fb0: 2020 2020 2020 2320 6765 7420 696e 6469        # get indi
+00014fc0: 7669 6475 616c 7320 6672 6f6d 2074 6865  viduals from the
+00014fd0: 2067 6976 656e 2053 7065 6369 6573 206f   given Species o
+00014fe0: 626a 6563 740a 2020 2020 2020 2020 2020  bject.          
+00014ff0: 2020 6966 2069 6e64 6976 6964 7320 6973    if individs is
+00015000: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00015010: 2020 2020 2020 2020 2020 2069 6e64 6976             indiv
+00015020: 6964 735f 746f 5f72 656d 6f76 6520 3d20  ids_to_remove = 
+00015030: 5b69 6e64 2066 6f72 2069 6e64 2069 6e0a  [ind for ind in.
+00015040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015060: 2020 2020 2020 736f 7572 6365 5f73 7070        source_spp
+00015070: 5f63 6f70 7920 6966 2069 6e64 206e 6f74  _copy if ind not
+00015080: 2069 6e20 696e 6469 7669 6473 5d0a 2020   in individs].  
+00015090: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000150a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150b0: 696e 6469 7669 6473 5f74 6f5f 7265 6d6f  individs_to_remo
+000150c0: 7665 203d 205b 2a73 6f75 7263 655f 7370  ve = [*source_sp
+000150d0: 705f 636f 7079 5d5b 6e3a 5d0a 2020 2020  p_copy][n:].    
+000150e0: 2020 2020 2020 2020 736f 7572 6365 5f73          source_s
+000150f0: 7070 5f63 6f70 792e 5f72 656d 6f76 655f  pp_copy._remove_
+00015100: 696e 6469 7669 6475 616c 7328 696e 6469  individuals(indi
+00015110: 7669 6473 3d69 6e64 6976 6964 735f 746f  vids=individs_to
+00015120: 5f72 656d 6f76 652c 0a20 2020 2020 2020  _remove,.       
+00015130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015150: 2020 2020 2020 2020 2076 6572 626f 7365           verbose
+00015160: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+00015170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015190: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000151a0: 2020 2020 2069 6620 696e 6469 7669 6473       if individs
+000151b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000151c0: 2020 2020 2020 2020 2020 2020 2020 6173                as
+000151d0: 7365 7274 206c 656e 2873 6f75 7263 655f  sert len(source_
+000151e0: 7370 705f 636f 7079 2920 3d3d 206c 656e  spp_copy) == len
+000151f0: 2869 6e64 6976 6964 7329 0a20 2020 2020  (individs).     
+00015200: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00015210: 2020 2020 2020 2020 2020 2020 2061 7373               ass
+00015220: 6572 7420 6c65 6e28 736f 7572 6365 5f73  ert len(source_s
+00015230: 7070 5f63 6f70 7929 203d 3d20 6e0a 0a20  pp_copy) == n.. 
+00015240: 2020 2020 2020 2020 2020 2023 2067 6174             # gat
+00015250: 6865 7220 616c 6c20 7265 6d61 696e 696e  her all remainin
+00015260: 6720 496e 6469 7669 6475 616c 7320 696e  g Individuals in
+00015270: 746f 2061 206c 6973 740a 2020 2020 2020  to a list.      
+00015280: 2020 2020 2020 696e 6469 7669 6473 203d        individs =
+00015290: 205b 2a73 6f75 7263 655f 7370 705f 636f   [*source_spp_co
+000152a0: 7079 2e76 616c 7565 7328 295d 0a0a 2020  py.values()]..  
+000152b0: 2020 2020 2020 2020 2020 2320 646f 7562            # doub
+000152c0: 6c65 2d63 6865 636b 2074 6861 7420 7468  le-check that th
+000152d0: 6520 736f 7572 6365 5f73 7070 5f63 6f70  e source_spp_cop
+000152e0: 7927 7320 5461 626c 6543 6f6c 6c65 6374  y's TableCollect
+000152f0: 696f 6e20 6861 7320 6265 656e 0a20 2020  ion has been.   
+00015300: 2020 2020 2020 2020 2023 2073 6f72 7465           # sorte
+00015310: 6420 616e 6420 7369 6d70 6c69 6669 6564  d and simplified
+00015320: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
+00015330: 7263 655f 7370 705f 636f 7079 2e5f 736f  rce_spp_copy._so
+00015340: 7274 5f61 6e64 5f73 696d 706c 6966 795f  rt_and_simplify_
+00015350: 7461 626c 655f 636f 6c6c 6563 7469 6f6e  table_collection
+00015360: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00015370: 2320 666f 726d 6174 2054 6162 6c65 436f  # format TableCo
+00015380: 6c6c 6563 7469 6f6e 2061 6e64 2072 6574  llection and ret
+00015390: 7572 6e20 7468 6520 6c69 7374 206f 6620  urn the list of 
+000153a0: 6e65 7720 676e 7820 496e 6469 7669 6420  new gnx Individ 
+000153b0: 6964 7873 0a20 2020 2020 2020 2020 2020  idxs.           
+000153c0: 2023 2074 6861 7420 5461 626c 6527 7320   # that Table's 
+000153d0: 696e 6469 7669 6475 616c 7320 7769 6c6c  individuals will
+000153e0: 2062 6520 6173 7369 676e 6564 2077 2f69   be assigned w/i
+000153f0: 6e20 7468 6973 2053 7065 6369 6573 0a20  n this Species. 
+00015400: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+00015410: 655f 7463 203d 2073 6f75 7263 655f 7370  e_tc = source_sp
+00015420: 705f 636f 7079 2e5f 7463 0a20 2020 2020  p_copy._tc.     
+00015430: 2020 2020 2020 206e 6578 745f 676e 785f         next_gnx_
+00015440: 6964 7873 203d 205f 7072 6570 5f74 736b  idxs = _prep_tsk
+00015450: 6974 5f74 6162 636f 6c6c 5f66 6f72 5f67  it_tabcoll_for_g
+00015460: 6e78 5f73 7070 5f75 6e69 6f6e 2874 633d  nx_spp_union(tc=
+00015470: 736f 7572 6365 5f74 632c 0a20 2020 2020  source_tc,.     
+00015480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154b0: 2020 2072 6563 6970 5f73 7070 3d73 656c     recip_spp=sel
+000154c0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
 000154d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154e0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-000154f0: 2020 2320 2e2e 2e20 6f72 2073 696d 756c    # ... or simul
-00015500: 6174 6520 7468 656d 2077 2f20 7468 6520  ate them w/ the 
-00015510: 6769 7665 6e20 6d73 7072 696d 6520 6172  given msprime ar
-00015520: 6773 0a20 2020 2020 2020 2023 2061 6e64  gs.        # and
-00015530: 2074 6865 2074 6869 7320 5370 6563 6965   the this Specie
-00015540: 7327 2067 656e 6f6d 6963 2061 7263 6869  s' genomic archi
-00015550: 7465 6374 7572 650a 2020 2020 2020 2020  tecture.        
-00015560: 656c 6966 2073 6f75 7263 655f 7370 7020  elif source_spp 
-00015570: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00015580: 2020 2020 2061 7373 6572 7420 696e 6469       assert indi
-00015590: 7669 6473 2069 7320 4e6f 6e65 2c20 2822  vids is None, ("
-000155a0: 5468 6520 2769 6e64 6976 6964 7327 2061  The 'individs' a
-000155b0: 7267 756d 656e 7420 696e 6469 6361 7465  rgument indicate
-000155c0: 7320 7468 6520 220a 2020 2020 2020 2020  s the ".        
-000155d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155e0: 2020 2020 2020 2020 2020 2020 2269 6e64              "ind
-000155f0: 6963 6573 206f 6620 496e 6469 7669 6475  ices of Individu
-00015600: 616c 7320 746f 2062 6520 6164 6465 6420  als to be added 
-00015610: 6672 6f6d 2022 0a20 2020 2020 2020 2020  from ".         
-00015620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015630: 2020 2020 2020 2020 2020 2022 6120 676e             "a gn
-00015640: 7820 5370 6563 6965 7320 6f62 6a65 6374  x Species object
-00015650: 2073 6572 7669 6e67 2061 7320 6120 736f   serving as a so
-00015660: 7572 6365 2022 0a20 2020 2020 2020 2020  urce ".         
-00015670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015680: 2020 2020 2020 2020 2020 2022 706f 7075             "popu
-00015690: 6c61 7469 6f6e 2c20 736f 2063 616e 206f  lation, so can o
-000156a0: 6e6c 7920 6265 2075 7365 6420 6966 2022  nly be used if "
-000156b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000156c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156d0: 2020 2020 2022 2773 6f75 7263 655f 6d73       "'source_ms
-000156e0: 7072 696d 655f 7061 7261 6d73 2720 6973  prime_params' is
-000156f0: 204e 6f6e 6520 616e 6420 220a 2020 2020   None and ".    
-00015700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015720: 2227 736f 7572 6365 5f73 7070 2720 6973  "'source_spp' is
-00015730: 2070 726f 7669 6465 642e 2229 0a0a 2020   provided.")..  
-00015740: 2020 2020 2020 2020 2020 2320 6d61 6b65            # make
-00015750: 2073 7572 6520 5370 6563 6965 7320 6861   sure Species ha
-00015760: 7320 6e6f 2073 656c 6563 7469 6f6e 2062  s no selection b
-00015770: 6566 6f72 6520 616c 6c6f 7769 6e67 2075  efore allowing u
-00015780: 7365 206f 6620 6d73 7072 696d 650a 2020  se of msprime.  
-00015790: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-000157a0: 206e 6f74 2073 656c 662e 7365 6c65 6374   not self.select
-000157b0: 696f 6e2c 2028 226d 7370 7269 6d65 2069  ion, ("msprime i
-000157c0: 7320 6120 636f 616c 6573 6365 6e74 2022  s a coalescent "
-000157d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000157e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157f0: 2020 2020 2020 2020 2020 2273 696d 756c            "simul
-00015800: 6174 6f72 2c20 736f 2063 616e 6e6f 7420  ator, so cannot 
-00015810: 7369 6d75 6c61 7465 2022 0a20 2020 2020  simulate ".     
-00015820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015840: 2020 2020 2273 656c 6563 7469 6f6e 2e20      "selection. 
-00015850: 436f 6e73 6964 6572 2075 7369 6e67 2061  Consider using a
-00015860: 2073 6563 6f6e 6420 220a 2020 2020 2020   second ".      
-00015870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015890: 2020 2022 4765 6f6e 6f6d 6963 7320 6d6f     "Geonomics mo
-000158a0: 6465 6c20 746f 2073 696d 756c 6174 6520  del to simulate 
-000158b0: 6120 736f 7572 6365 2022 0a20 2020 2020  a source ".     
-000158c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154f0: 2020 2020 2020 2020 2020 2063 6f6f 7264             coord
+00015500: 733d 636f 6f72 6473 2c0a 2020 2020 2020  s=coords,.      
+00015510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015540: 2020 736f 7572 6365 5f73 6f66 7477 6172    source_softwar
+00015550: 653d 2767 6e78 272c 0a20 2020 2020 2020  e='gnx',.       
+00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015590: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000155a0: 2020 2020 2023 202e 2e2e 206f 7220 7369       # ... or si
+000155b0: 6d75 6c61 7465 2074 6865 6d20 772f 2074  mulate them w/ t
+000155c0: 6865 2067 6976 656e 206d 7370 7269 6d65  he given msprime
+000155d0: 2061 7267 730a 2020 2020 2020 2020 2320   args.        # 
+000155e0: 616e 6420 7468 6520 7468 6973 2053 7065  and the this Spe
+000155f0: 6369 6573 2720 6765 6e6f 6d69 6320 6172  cies' genomic ar
+00015600: 6368 6974 6563 7475 7265 0a20 2020 2020  chitecture.     
+00015610: 2020 2065 6c69 6620 736f 7572 6365 5f73     elif source_s
+00015620: 7070 2069 7320 4e6f 6e65 3a0a 2020 2020  pp is None:.    
+00015630: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+00015640: 6e64 6976 6964 7320 6973 204e 6f6e 652c  ndivids is None,
+00015650: 2028 2254 6865 2027 696e 6469 7669 6473   ("The 'individs
+00015660: 2720 6172 6775 6d65 6e74 2069 6e64 6963  ' argument indic
+00015670: 6174 6573 2074 6865 2022 0a20 2020 2020  ates the ".     
+00015680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015690: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000156a0: 696e 6469 6365 7320 6f66 2049 6e64 6976  indices of Indiv
+000156b0: 6964 7561 6c73 2074 6f20 6265 2061 6464  iduals to be add
+000156c0: 6564 2066 726f 6d20 220a 2020 2020 2020  ed from ".      
+000156d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156e0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+000156f0: 2067 6e78 2053 7065 6369 6573 206f 626a   gnx Species obj
+00015700: 6563 7420 7365 7276 696e 6720 6173 2061  ect serving as a
+00015710: 2073 6f75 7263 6520 220a 2020 2020 2020   source ".      
+00015720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015730: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00015740: 6f70 756c 6174 696f 6e2c 2073 6f20 6361  opulation, so ca
+00015750: 6e20 6f6e 6c79 2062 6520 7573 6564 2069  n only be used i
+00015760: 6620 220a 2020 2020 2020 2020 2020 2020  f ".            
+00015770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015780: 2020 2020 2020 2020 2227 736f 7572 6365          "'source
+00015790: 5f6d 7370 7269 6d65 5f70 6172 616d 7327  _msprime_params'
+000157a0: 2069 7320 4e6f 6e65 2061 6e64 2022 0a20   is None and ". 
+000157b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157d0: 2020 2022 2773 6f75 7263 655f 7370 7027     "'source_spp'
+000157e0: 2069 7320 7072 6f76 6964 6564 2e22 290a   is provided.").
+000157f0: 0a20 2020 2020 2020 2020 2020 2023 206d  .            # m
+00015800: 616b 6520 7375 7265 2053 7065 6369 6573  ake sure Species
+00015810: 2068 6173 206e 6f20 7365 6c65 6374 696f   has no selectio
+00015820: 6e20 6265 666f 7265 2061 6c6c 6f77 696e  n before allowin
+00015830: 6720 7573 6520 6f66 206d 7370 7269 6d65  g use of msprime
+00015840: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00015850: 6572 7420 6e6f 7420 7365 6c66 2e73 656c  ert not self.sel
+00015860: 6563 7469 6f6e 2c20 2822 6d73 7072 696d  ection, ("msprim
+00015870: 6520 6973 2061 2063 6f61 6c65 7363 656e  e is a coalescen
+00015880: 7420 220a 2020 2020 2020 2020 2020 2020  t ".            
+00015890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000158a0: 2020 2020 2020 2020 2020 2020 2022 7369               "si
+000158b0: 6d75 6c61 746f 722c 2073 6f20 6361 6e6e  mulator, so cann
+000158c0: 6f74 2073 696d 756c 6174 6520 220a 2020  ot simulate ".  
 000158d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158e0: 2020 2020 2270 6f70 756c 6174 696f 6e20      "population 
-000158f0: 7769 7468 2073 656c 6563 7469 6f6e 2e22  with selection."
-00015900: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00015910: 2063 6865 636b 2074 6861 7420 7265 7175   check that requ
-00015920: 6972 6564 206d 7370 7269 6d65 2070 6172  ired msprime par
-00015930: 616d 7320 6172 6520 7072 6f76 6964 6564  ams are provided
-00015940: 2061 6e64 2061 6e79 206f 7468 6572 730a   and any others.
-00015950: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
-00015960: 6f76 6964 6564 2061 7265 2061 6d6f 6e67  ovided are among
-00015970: 2074 686f 7365 2061 6c6c 6f77 6564 0a20   those allowed. 
-00015980: 2020 2020 2020 2020 2020 2072 6571 7569             requi
-00015990: 7265 645f 6d73 7072 696d 655f 7061 7261  red_msprime_para
-000159a0: 6d73 203d 205b 2772 6563 6f6d 625f 7261  ms = ['recomb_ra
-000159b0: 7465 272c 2027 6d75 745f 7261 7465 275d  te', 'mut_rate']
-000159c0: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
-000159d0: 6f77 6564 5f6d 7370 7269 6d65 5f70 6172  owed_msprime_par
-000159e0: 616d 7320 3d20 5b27 6465 6d6f 6772 6170  ams = ['demograp
-000159f0: 6879 272c 2027 706f 7075 6c61 7469 6f6e  hy', 'population
-00015a00: 5f73 697a 6527 2c0a 2020 2020 2020 2020  _size',.        
-00015a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a20: 2020 2020 2020 2020 2020 2020 2020 2761                'a
-00015a30: 6e63 6573 7472 795f 6d6f 6465 6c27 2c20  ncestry_model', 
-00015a40: 2772 616e 646f 6d5f 7365 6564 272c 0a20  'random_seed',. 
-00015a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a70: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
-00015a80: 2020 616c 6c5f 6d73 7072 696d 655f 7061    all_msprime_pa
-00015a90: 7261 6d73 203d 2028 7265 7175 6972 6564  rams = (required
-00015aa0: 5f6d 7370 7269 6d65 5f70 6172 616d 7320  _msprime_params 
-00015ab0: 2b0a 2020 2020 2020 2020 2020 2020 2020  +.              
+000158e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000158f0: 2020 2020 2020 2022 7365 6c65 6374 696f         "selectio
+00015900: 6e2e 2043 6f6e 7369 6465 7220 7573 696e  n. Consider usin
+00015910: 6720 6120 7365 636f 6e64 2022 0a20 2020  g a second ".   
+00015920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015940: 2020 2020 2020 2247 656f 6e6f 6d69 6373        "Geonomics
+00015950: 206d 6f64 656c 2074 6f20 7369 6d75 6c61   model to simula
+00015960: 7465 2061 2073 6f75 7263 6520 220a 2020  te a source ".  
+00015970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015990: 2020 2020 2020 2022 706f 7075 6c61 7469         "populati
+000159a0: 6f6e 2077 6974 6820 7365 6c65 6374 696f  on with selectio
+000159b0: 6e2e 2229 0a0a 2020 2020 2020 2020 2020  n.")..          
+000159c0: 2020 2320 6368 6563 6b20 7468 6174 2072    # check that r
+000159d0: 6571 7569 7265 6420 6d73 7072 696d 6520  equired msprime 
+000159e0: 7061 7261 6d73 2061 7265 2070 726f 7669  params are provi
+000159f0: 6465 6420 616e 6420 616e 7920 6f74 6865  ded and any othe
+00015a00: 7273 0a20 2020 2020 2020 2020 2020 2023  rs.            #
+00015a10: 2070 726f 7669 6465 6420 6172 6520 616d   provided are am
+00015a20: 6f6e 6720 7468 6f73 6520 616c 6c6f 7765  ong those allowe
+00015a30: 640a 2020 2020 2020 2020 2020 2020 7265  d.            re
+00015a40: 7175 6972 6564 5f6d 7370 7269 6d65 5f70  quired_msprime_p
+00015a50: 6172 616d 7320 3d20 5b27 7265 636f 6d62  arams = ['recomb
+00015a60: 5f72 6174 6527 2c20 276d 7574 5f72 6174  _rate', 'mut_rat
+00015a70: 6527 5d0a 2020 2020 2020 2020 2020 2020  e'].            
+00015a80: 616c 6c6f 7765 645f 6d73 7072 696d 655f  allowed_msprime_
+00015a90: 7061 7261 6d73 203d 205b 2764 656d 6f67  params = ['demog
+00015aa0: 7261 7068 7927 2c20 2770 6f70 756c 6174  raphy', 'populat
+00015ab0: 696f 6e5f 7369 7a65 272c 0a20 2020 2020  ion_size',.     
 00015ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ad0: 2020 2020 616c 6c6f 7765 645f 6d73 7072      allowed_mspr
-00015ae0: 696d 655f 7061 7261 6d73 290a 2020 2020  ime_params).    
-00015af0: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
-00015b00: 702e 616c 6c28 5b6b 2069 6e20 616c 6c5f  p.all([k in all_
-00015b10: 6d73 7072 696d 655f 7061 7261 6d73 2066  msprime_params f
-00015b20: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
-00015b30: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00015b40: 2069 6e20 736f 7572 6365 5f6d 7370 7269   in source_mspri
-00015b50: 6d65 5f70 6172 616d 735d 292c 2028 2254  me_params]), ("T
-00015b60: 6865 206f 6e6c 7920 7061 7261 6d65 7465  he only paramete
-00015b70: 7273 220a 2020 2020 2020 2020 2020 2020  rs".            
-00015b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b90: 2020 2020 2020 2020 2220 6163 6365 7074          " accept
-00015ba0: 6564 2069 6e20 2773 6f75 7263 655f 6d73  ed in 'source_ms
-00015bb0: 7072 696d 655f 7061 7261 6d73 2720 6172  prime_params' ar
-00015bc0: 653a 2022 0a20 2020 2020 2020 2020 2020  e: ".           
-00015bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015be0: 2020 2020 2020 2020 6622 7b27 2c20 272e          f"{', '.
-00015bf0: 6a6f 696e 2861 6c6c 5f6d 7370 7269 6d65  join(all_msprime
-00015c00: 5f70 6172 616d 7329 7d2e 2229 0a20 2020  _params)}.").   
-00015c10: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00015c20: 6e70 2e61 6c6c 285b 6b20 696e 2073 6f75  np.all([k in sou
-00015c30: 7263 655f 6d73 7072 696d 655f 7061 7261  rce_msprime_para
-00015c40: 6d73 2066 6f72 0a20 2020 2020 2020 2020  ms for.         
-00015c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c60: 2020 206b 2069 6e20 7265 7175 6972 6564     k in required
-00015c70: 5f6d 7370 7269 6d65 5f70 6172 616d 735d  _msprime_params]
-00015c80: 292c 2028 2242 6f74 6820 220a 2020 2020  ), ("Both ".    
-00015c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ca0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00015cb0: 227b 2720 616e 6420 272e 6a6f 696e 2872  "{' and '.join(r
-00015cc0: 6571 7569 7265 645f 6d73 7072 696d 655f  equired_msprime_
-00015cd0: 7061 7261 6d73 297d 2022 0a20 2020 2020  params)} ".     
-00015ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cf0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00015d00: 6d75 7374 2062 6520 7072 6f76 6964 6564  must be provided
-00015d10: 2077 6974 6869 6e20 220a 2020 2020 2020   within ".      
-00015d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d30: 2020 2020 2020 2020 2020 2020 2020 2227                "'
-00015d40: 736f 7572 6365 5f6d 7370 7269 6d65 5f70  source_msprime_p
-00015d50: 6172 616d 7327 2e22 290a 0a20 2020 2020  arams'.")..     
-00015d60: 2020 2020 2020 2023 2072 756e 2074 6865         # run the
-00015d70: 2073 696d 756c 6174 696f 6e20 616e 6420   simulation and 
-00015d80: 7265 7475 726e 2074 656d 706c 6174 6520  return template 
-00015d90: 496e 6469 7669 6475 616c 730a 2020 2020  Individuals.    
-00015da0: 2020 2020 2020 2020 7573 655f 7473 6b69          use_tski
-00015db0: 7420 3d20 7365 6c66 2e67 656e 5f61 7263  t = self.gen_arc
-00015dc0: 682e 7573 655f 7473 6b69 740a 2020 2020  h.use_tskit.    
-00015dd0: 2020 2020 2020 2020 696e 6469 7669 6473          individs
-00015de0: 2c20 736f 7572 6365 5f74 6320 3d20 5f73  , source_tc = _s
-00015df0: 696d 5f6d 7370 7269 6d65 5f69 6e64 6976  im_msprime_indiv
-00015e00: 6964 7561 6c73 286e 3d6e 2c0a 2020 2020  iduals(n=n,.    
-00015e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e40: 4c3d 7365 6c66 2e67 656e 5f61 7263 682e  L=self.gen_arch.
-00015e50: 4c2c 0a20 2020 2020 2020 2020 2020 2020  L,.             
-00015e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e80: 2020 2020 2020 2075 7365 5f74 736b 6974         use_tskit
-00015e90: 3d75 7365 5f74 736b 6974 2c0a 2020 2020  =use_tskit,.    
-00015ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ae0: 2027 616e 6365 7374 7279 5f6d 6f64 656c   'ancestry_model
+00015af0: 272c 2027 7261 6e64 6f6d 5f73 6565 6427  ', 'random_seed'
+00015b00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00015b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b20: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00015b30: 2020 2020 2061 6c6c 5f6d 7370 7269 6d65       all_msprime
+00015b40: 5f70 6172 616d 7320 3d20 2872 6571 7569  _params = (requi
+00015b50: 7265 645f 6d73 7072 696d 655f 7061 7261  red_msprime_para
+00015b60: 6d73 202b 0a20 2020 2020 2020 2020 2020  ms +.           
+00015b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b80: 2020 2020 2020 2061 6c6c 6f77 6564 5f6d         allowed_m
+00015b90: 7370 7269 6d65 5f70 6172 616d 7329 0a20  sprime_params). 
+00015ba0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00015bb0: 7420 6e70 2e61 6c6c 285b 6b20 696e 2061  t np.all([k in a
+00015bc0: 6c6c 5f6d 7370 7269 6d65 5f70 6172 616d  ll_msprime_param
+00015bd0: 7320 666f 720a 2020 2020 2020 2020 2020  s for.          
+00015be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015bf0: 2020 6b20 696e 2073 6f75 7263 655f 6d73    k in source_ms
+00015c00: 7072 696d 655f 7061 7261 6d73 5d29 2c20  prime_params]), 
+00015c10: 2822 5468 6520 6f6e 6c79 2070 6172 616d  ("The only param
+00015c20: 6574 6572 7322 0a20 2020 2020 2020 2020  eters".         
+00015c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c40: 2020 2020 2020 2020 2020 2022 2061 6363             " acc
+00015c50: 6570 7465 6420 696e 2027 736f 7572 6365  epted in 'source
+00015c60: 5f6d 7370 7269 6d65 5f70 6172 616d 7327  _msprime_params'
+00015c70: 2061 7265 3a20 220a 2020 2020 2020 2020   are: ".        
+00015c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c90: 2020 2020 2020 2020 2020 2066 227b 272c             f"{',
+00015ca0: 2027 2e6a 6f69 6e28 616c 6c5f 6d73 7072   '.join(all_mspr
+00015cb0: 696d 655f 7061 7261 6d73 297d 2e22 290a  ime_params)}.").
+00015cc0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00015cd0: 7274 206e 702e 616c 6c28 5b6b 2069 6e20  rt np.all([k in 
+00015ce0: 736f 7572 6365 5f6d 7370 7269 6d65 5f70  source_msprime_p
+00015cf0: 6172 616d 7320 666f 720a 2020 2020 2020  arams for.      
+00015d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d10: 2020 2020 2020 6b20 696e 2072 6571 7569        k in requi
+00015d20: 7265 645f 6d73 7072 696d 655f 7061 7261  red_msprime_para
+00015d30: 6d73 5d29 2c20 2822 426f 7468 2022 0a20  ms]), ("Both ". 
+00015d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d60: 2020 6622 7b27 2061 6e64 2027 2e6a 6f69    f"{' and '.joi
+00015d70: 6e28 7265 7175 6972 6564 5f6d 7370 7269  n(required_mspri
+00015d80: 6d65 5f70 6172 616d 7329 7d20 220a 2020  me_params)} ".  
+00015d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015db0: 2020 226d 7573 7420 6265 2070 726f 7669    "must be provi
+00015dc0: 6465 6420 7769 7468 696e 2022 0a20 2020  ded within ".   
+00015dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015df0: 2022 2773 6f75 7263 655f 6d73 7072 696d   "'source_msprim
+00015e00: 655f 7061 7261 6d73 272e 2229 0a0a 2020  e_params'.")..  
+00015e10: 2020 2020 2020 2020 2020 2320 7275 6e20            # run 
+00015e20: 7468 6520 7369 6d75 6c61 7469 6f6e 2061  the simulation a
+00015e30: 6e64 2072 6574 7572 6e20 7465 6d70 6c61  nd return templa
+00015e40: 7465 2049 6e64 6976 6964 7561 6c73 0a20  te Individuals. 
+00015e50: 2020 2020 2020 2020 2020 2075 7365 5f74             use_t
+00015e60: 736b 6974 203d 2073 656c 662e 6765 6e5f  skit = self.gen_
+00015e70: 6172 6368 2e75 7365 5f74 736b 6974 0a20  arch.use_tskit. 
+00015e80: 2020 2020 2020 2020 2020 2069 6e64 6976             indiv
+00015e90: 6964 732c 2073 6f75 7263 655f 7463 203d  ids, source_tc =
+00015ea0: 205f 7369 6d5f 6d73 7072 696d 655f 696e   _sim_msprime_in
+00015eb0: 6469 7669 6475 616c 7328 6e3d 6e2c 0a20  dividuals(n=n,. 
 00015ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ed0: 2a2a 736f 7572 6365 5f6d 7370 7269 6d65  **source_msprime
-00015ee0: 5f70 6172 616d 732c 0a20 2020 2020 2020  _params,.       
-00015ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f10: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-00015f20: 2020 2020 2020 2020 2020 2020 2320 7275              # ru
-00015f30: 6e20 616c 6c20 5461 626c 6543 6f6c 6c65  n all TableColle
-00015f40: 6374 696f 6e20 6564 6974 7320 7468 6174  ction edits that
-00015f50: 2061 7265 206e 6563 6573 7361 7279 2074   are necessary t
-00015f60: 6f20 616c 6967 6e20 6d73 7072 696d 650a  o align msprime.
-00015f70: 2020 2020 2020 2020 2020 2020 2320 6f75              # ou
-00015f80: 7470 7574 2077 6974 6820 7468 6520 5461  tput with the Ta
-00015f90: 626c 6543 6f6c 6c65 6374 696f 6e20 636f  bleCollection co
-00015fa0: 6e76 656e 7469 6f6e 7320 7573 6564 2069  nventions used i
-00015fb0: 6e20 676e 780a 2020 2020 2020 2020 2020  n gnx.          
-00015fc0: 2020 2320 4e4f 5445 3a20 6564 6974 7320    # NOTE: edits 
-00015fd0: 7468 6520 5461 626c 6543 6f6c 6c65 6374  the TableCollect
-00015fe0: 696f 6e20 696e 2070 6c61 6365 3b0a 2020  ion in place;.  
-00015ff0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00016000: 2020 7265 7475 726e 7320 7468 6520 6e65    returns the ne
-00016010: 7874 206e 2067 6e78 2049 6e64 6976 6964  xt n gnx Individ
-00016020: 7561 6c20 6964 7873 2061 7373 6967 6e65  ual idxs assigne
-00016030: 6420 746f 2074 686f 7365 0a20 2020 2020  d to those.     
-00016040: 2020 2020 2020 2023 2020 2020 2020 2049         #       I
-00016050: 6e64 6976 6964 7561 6c73 2066 6f72 2069  ndividuals for i
-00016060: 6e63 6f72 706f 7261 7469 6f6e 2069 6e74  ncorporation int
-00016070: 6f20 7468 6520 6769 7665 6e20 5370 6563  o the given Spec
-00016080: 6965 730a 2020 2020 2020 2020 2020 2020  ies.            
-00016090: 6e65 7874 5f67 6e78 5f69 6478 7320 3d20  next_gnx_idxs = 
-000160a0: 5f70 7265 705f 7473 6b69 745f 7461 6263  _prep_tskit_tabc
-000160b0: 6f6c 6c5f 666f 725f 676e 785f 7370 705f  oll_for_gnx_spp_
-000160c0: 756e 696f 6e28 7463 3d73 6f75 7263 655f  union(tc=source_
-000160d0: 7463 2c0a 2020 2020 2020 2020 2020 2020  tc,.            
-000160e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016100: 2020 2020 2020 2020 2020 7265 6369 705f            recip_
-00016110: 7370 703d 7365 6c66 2c0a 2020 2020 2020  spp=self,.      
-00016120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016150: 636f 6f72 6473 3d63 6f6f 7264 732c 0a20  coords=coords,. 
-00016160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016190: 2020 2020 2073 6f75 7263 655f 736f 6674       source_soft
-000161a0: 7761 7265 3d27 6d73 7072 696d 6527 2c0a  ware='msprime',.
-000161b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ef0: 2020 204c 3d73 656c 662e 6765 6e5f 6172     L=self.gen_ar
+00015f00: 6368 2e4c 2c0a 2020 2020 2020 2020 2020  ch.L,.          
+00015f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f30: 2020 2020 2020 2020 2020 7573 655f 7473            use_ts
+00015f40: 6b69 743d 7573 655f 7473 6b69 742c 0a20  kit=use_tskit,. 
+00015f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f80: 2020 202a 2a73 6f75 7263 655f 6d73 7072     **source_mspr
+00015f90: 696d 655f 7061 7261 6d73 2c0a 2020 2020  ime_params,.    
+00015fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015fd0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+00015fe0: 2072 756e 2061 6c6c 2054 6162 6c65 436f   run all TableCo
+00015ff0: 6c6c 6563 7469 6f6e 2065 6469 7473 2074  llection edits t
+00016000: 6861 7420 6172 6520 6e65 6365 7373 6172  hat are necessar
+00016010: 7920 746f 2061 6c69 676e 206d 7370 7269  y to align mspri
+00016020: 6d65 0a20 2020 2020 2020 2020 2020 2023  me.            #
+00016030: 206f 7574 7075 7420 7769 7468 2074 6865   output with the
+00016040: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
+00016050: 2063 6f6e 7665 6e74 696f 6e73 2075 7365   conventions use
+00016060: 6420 696e 2067 6e78 0a20 2020 2020 2020  d in gnx.       
+00016070: 2020 2020 2023 204e 4f54 453a 2065 6469       # NOTE: edi
+00016080: 7473 2074 6865 2054 6162 6c65 436f 6c6c  ts the TableColl
+00016090: 6563 7469 6f6e 2069 6e20 706c 6163 653b  ection in place;
+000160a0: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+000160b0: 2020 2020 2072 6574 7572 6e73 2074 6865       returns the
+000160c0: 206e 6578 7420 6e20 676e 7820 496e 6469   next n gnx Indi
+000160d0: 7669 6475 616c 2069 6478 7320 6173 7369  vidual idxs assi
+000160e0: 676e 6564 2074 6f20 7468 6f73 650a 2020  gned to those.  
+000160f0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+00016100: 2020 496e 6469 7669 6475 616c 7320 666f    Individuals fo
+00016110: 7220 696e 636f 7270 6f72 6174 696f 6e20  r incorporation 
+00016120: 696e 746f 2074 6865 2067 6976 656e 2053  into the given S
+00016130: 7065 6369 6573 0a20 2020 2020 2020 2020  pecies.         
+00016140: 2020 206e 6578 745f 676e 785f 6964 7873     next_gnx_idxs
+00016150: 203d 205f 7072 6570 5f74 736b 6974 5f74   = _prep_tskit_t
+00016160: 6162 636f 6c6c 5f66 6f72 5f67 6e78 5f73  abcoll_for_gnx_s
+00016170: 7070 5f75 6e69 6f6e 2874 633d 736f 7572  pp_union(tc=sour
+00016180: 6365 5f74 632c 0a20 2020 2020 2020 2020  ce_tc,.         
+00016190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161b0: 2020 2020 2020 2020 2020 2020 2072 6563               rec
+000161c0: 6970 5f73 7070 3d73 656c 662c 0a20 2020  ip_spp=self,.   
 000161d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000161e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161f0: 2029 0a0a 2020 2020 2020 2020 2320 7365   )..        # se
-00016200: 7420 7468 6520 736f 7572 6365 2049 6e64  t the source Ind
-00016210: 6976 6964 7561 6c73 2720 636f 6f72 6469  ividuals' coordi
-00016220: 6e61 7465 730a 2020 2020 2020 2020 5b69  nates.        [i
-00016230: 6e64 2e5f 7365 745f 706f 7328 2a63 6f6f  nd._set_pos(*coo
-00016240: 7264 735b 692c 3a5d 2920 666f 7220 692c  rds[i,:]) for i,
-00016250: 2069 6e64 2069 6e20 656e 756d 6572 6174   ind in enumerat
-00016260: 6528 696e 6469 7669 6473 295d 0a0a 2020  e(individs)]..  
-00016270: 2020 2020 2020 2320 7570 6461 7465 2074        # update t
-00016280: 6865 2069 6e64 6578 2076 616c 7565 7320  he index values 
-00016290: 6964 656e 7469 6679 696e 6720 496e 6469  identifying Indi
-000162a0: 7669 6475 616c 7320 696e 2067 6e78 2061  viduals in gnx a
-000162b0: 6e64 2074 736b 6974 2064 6174 610a 2020  nd tskit data.  
-000162c0: 2020 2020 2020 6d61 785f 6964 785f 6234        max_idx_b4
-000162d0: 203d 2073 656c 662e 6d61 785f 696e 645f   = self.max_ind_
-000162e0: 6964 780a 2020 2020 2020 2020 6e65 775f  idx.        new_
-000162f0: 6964 7873 203d 205b 5d0a 2020 2020 2020  idxs = [].      
-00016300: 2020 666f 7220 692c 2069 6e64 2069 6e20    for i, ind in 
-00016310: 656e 756d 6572 6174 6528 696e 6469 7669  enumerate(indivi
-00016320: 6473 293a 0a20 2020 2020 2020 2020 2020  ds):.           
-00016330: 2023 2069 6e63 7265 6d65 6e74 2074 6865   # increment the
-00016340: 206d 6178 5f69 6e64 5f69 6478 0a20 2020   max_ind_idx.   
-00016350: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-00016360: 785f 696e 645f 6964 7820 2b3d 2031 0a20  x_ind_idx += 1. 
-00016370: 2020 2020 2020 2020 2020 2023 2073 6574             # set
-00016380: 2074 6865 2049 6e64 6976 6964 7561 6c27   the Individual'
-00016390: 7320 676e 7820 696e 6465 780a 2020 2020  s gnx index.    
-000163a0: 2020 2020 2020 2020 696e 642e 6964 7820          ind.idx 
-000163b0: 3d20 7365 6c66 2e6d 6178 5f69 6e64 5f69  = self.max_ind_i
-000163c0: 6478 0a20 2020 2020 2020 2020 2020 206e  dx.            n
-000163d0: 6577 5f69 6478 732e 6170 7065 6e64 2873  ew_idxs.append(s
-000163e0: 656c 662e 6d61 785f 696e 645f 6964 7829  elf.max_ind_idx)
-000163f0: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-00016400: 6574 2074 6865 2049 6e64 6976 6964 7561  et the Individua
-00016410: 6c73 2720 6964 7320 666f 7220 7468 6520  ls' ids for the 
-00016420: 7473 6b69 7420 6e6f 6465 7320 7461 626c  tskit nodes tabl
-00016430: 650a 2020 2020 2020 2020 2020 2020 696e  e.            in
-00016440: 642e 5f6e 6f64 6573 5f74 6162 5f69 6473  d._nodes_tab_ids
-00016450: 203d 207b 6b3a 2076 202b 2073 656c 662e   = {k: v + self.
-00016460: 5f74 632e 6e6f 6465 732e 6e75 6d5f 726f  _tc.nodes.num_ro
-00016470: 7773 2066 6f72 0a20 2020 2020 2020 2020  ws for.         
-00016480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000164a0: 2020 206b 2c20 7620 696e 2069 6e64 2e5f     k, v in ind._
-000164b0: 6e6f 6465 735f 7461 625f 6964 732e 6974  nodes_tab_ids.it
-000164c0: 656d 7328 297d 0a20 2020 2020 2020 2020  ems()}.         
-000164d0: 2020 2023 2073 6574 2074 6865 2049 6e64     # set the Ind
-000164e0: 6976 6964 7561 6c73 2720 6964 7320 666f  ividuals' ids fo
-000164f0: 7220 7468 6520 7473 6b69 7420 696e 6469  r the tskit indi
-00016500: 7669 6475 616c 7320 7461 626c 650a 2020  viduals table.  
-00016510: 2020 2020 2020 2020 2020 2320 4e4f 5445            # NOTE
-00016520: 3a20 7468 6520 696e 7665 7273 6520 2874  : the inverse (t
-00016530: 6865 2049 6e64 6976 6964 7561 6c73 2720  he Individuals' 
-00016540: 676e 7820 6964 7820 7661 6c75 6573 2c0a  gnx idx values,.
-00016550: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-00016560: 2020 2020 6173 2072 6563 6f72 6564 2069      as recored i
-00016570: 6e20 7468 6520 7473 6b69 7420 696e 6469  n the tskit indi
-00016580: 7669 6475 616c 7320 7461 626c 6527 730a  viduals table's.
-00016590: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-000165a0: 2020 2020 6d65 7461 6461 7461 2920 7368      metadata) sh
-000165b0: 6f75 6c64 2061 6c72 6561 6479 2062 6520  ould already be 
-000165c0: 636f 7272 6563 740a 2020 2020 2020 2020  correct.        
-000165d0: 2020 2020 2320 2020 2020 2020 6265 6361      #       beca
-000165e0: 7573 6520 5f70 7265 705f 7473 6b69 745f  use _prep_tskit_
-000165f0: 7461 6263 6f6c 6c5f 666f 725f 676e 785f  tabcoll_for_gnx_
-00016600: 7370 705f 756e 696f 6e0a 2020 2020 2020  spp_union.      
-00016610: 2020 2020 2020 2320 2020 2020 2020 6765        #       ge
-00016620: 6e65 7261 7465 6420 7468 6520 696e 6465  nerated the inde
-00016630: 7820 7661 6c75 6573 0a20 2020 2020 2020  x values.       
-00016640: 2020 2020 2023 2020 2020 2020 2061 6e64       #       and
-00016650: 2073 6574 2074 6865 6d20 696e 2074 6865   set them in the
-00016660: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
-00016670: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
-00016680: 2e5f 696e 6469 7669 6475 616c 735f 7461  ._individuals_ta
-00016690: 625f 6964 202b 3d20 7365 6c66 2e5f 7463  b_id += self._tc
-000166a0: 2e69 6e64 6976 6964 7561 6c73 2e6e 756d  .individuals.num
-000166b0: 5f72 6f77 730a 2020 2020 2020 2020 6d61  _rows.        ma
-000166c0: 785f 6964 785f 6166 203d 2073 656c 662e  x_idx_af = self.
-000166d0: 6d61 785f 696e 645f 6964 780a 2020 2020  max_ind_idx.    
-000166e0: 2020 2020 6173 7365 7274 206d 6178 5f69      assert max_i
-000166f0: 6478 5f61 6620 2d20 6d61 785f 6964 785f  dx_af - max_idx_
-00016700: 6234 203d 3d20 6c65 6e28 696e 6469 7669  b4 == len(indivi
-00016710: 6473 290a 2020 2020 2020 2020 2320 636f  ds).        # co
-00016720: 6d70 6172 6520 7468 6520 6964 7820 7661  mpare the idx va
-00016730: 6c75 6573 2074 6861 7420 7765 7265 2073  lues that were s
-00016740: 6574 206f 6e20 7468 6520 496e 6469 7669  et on the Indivi
-00016750: 6475 616c 7320 746f 2074 686f 7365 2074  duals to those t
-00016760: 6861 740a 2020 2020 2020 2020 2320 7765  hat.        # we
-00016770: 7265 2073 6574 2069 6e20 7468 6520 5461  re set in the Ta
-00016780: 626c 6543 6f6c 6c65 6374 696f 6e2e 696e  bleCollection.in
-00016790: 6469 7669 6475 616c 7320 7461 626c 650a  dividuals table.
-000167a0: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
-000167b0: 702e 616c 6c28 6e70 2e61 7272 6179 286e  p.all(np.array(n
-000167c0: 6578 745f 676e 785f 6964 7873 2920 3d3d  ext_gnx_idxs) ==
-000167d0: 206e 702e 6172 7261 7928 6e65 775f 6964   np.array(new_id
-000167e0: 7873 2929 2c20 280a 2020 2020 2020 2020  xs)), (.        
-000167f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016800: 2020 2020 2020 2020 2022 496e 6469 7669           "Indivi
-00016810: 6461 756c 2069 6478 2076 616c 7565 7320  daul idx values 
-00016820: 7365 7420 696e 2074 6865 2022 0a20 2020  set in the ".   
-00016830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016850: 2022 5461 626c 6543 6f6c 6c65 6374 696f   "TableCollectio
-00016860: 6e2e 696e 6469 7669 6475 616c 7320 220a  n.individuals ".
-00016870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016890: 2020 2020 2274 6162 6c65 2064 6f20 6e6f      "table do no
-000168a0: 7420 6167 7265 6520 7769 7468 2074 686f  t agree with tho
-000168b0: 7365 2073 6574 206f 6e20 7468 6520 220a  se set on the ".
-000168c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168e0: 2020 2020 2249 6e64 6976 6964 7561 6c73      "Individuals
-000168f0: 2074 6865 6d73 656c 7665 732e 2229 0a0a   themselves.")..
-00016900: 2020 2020 2020 2020 2320 736f 7274 2061          # sort a
-00016910: 6e64 2073 696d 706c 6966 7920 7468 6520  nd simplify the 
-00016920: 7473 6b69 742e 5461 626c 6543 6f6c 6c65  tskit.TableColle
-00016930: 6374 696f 6e0a 2020 2020 2020 2020 7365  ction.        se
-00016940: 6c66 2e5f 736f 7274 5f61 6e64 5f73 696d  lf._sort_and_sim
-00016950: 706c 6966 795f 7461 626c 655f 636f 6c6c  plify_table_coll
-00016960: 6563 7469 6f6e 2829 0a0a 2020 2020 2020  ection()..      
-00016970: 2020 2320 756e 696f 6e20 736f 7572 6365    # union source
-00016980: 2069 6e64 6976 6964 7561 6c73 2720 5461   individuals' Ta
-00016990: 626c 6543 6f6c 6c65 6374 696f 6e20 696e  bleCollection in
-000169a0: 746f 2074 6869 7320 5370 6563 6965 7327  to this Species'
-000169b0: 2054 6162 6c65 436f 6c6c 0a20 2020 2020   TableColl.     
-000169c0: 2020 206e 6f64 6573 5f74 6162 5f6c 656e     nodes_tab_len
-000169d0: 5f62 3420 3d20 7365 6c66 2e5f 7463 2e6e  _b4 = self._tc.n
-000169e0: 6f64 6573 2e6e 756d 5f72 6f77 730a 2020  odes.num_rows.  
-000169f0: 2020 2020 2020 696e 6469 7669 6473 5f74        individs_t
-00016a00: 6162 5f6c 656e 5f62 3420 3d20 7365 6c66  ab_len_b4 = self
-00016a10: 2e5f 7463 2e69 6e64 6976 6964 7561 6c73  ._tc.individuals
-00016a20: 2e6e 756d 5f72 6f77 730a 2020 2020 2020  .num_rows.      
-00016a30: 2020 7365 6c66 2e5f 7463 2e75 6e69 6f6e    self._tc.union
-00016a40: 2873 6f75 7263 655f 7463 2c0a 2020 2020  (source_tc,.    
+000161f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016200: 2020 2063 6f6f 7264 733d 636f 6f72 6473     coords=coords
+00016210: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016240: 2020 2020 2020 2020 736f 7572 6365 5f73          source_s
+00016250: 6f66 7477 6172 653d 276d 7370 7269 6d65  oftware='msprime
+00016260: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00016270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162a0: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+000162b0: 2073 6574 2074 6865 2073 6f75 7263 6520   set the source 
+000162c0: 496e 6469 7669 6475 616c 7327 2063 6f6f  Individuals' coo
+000162d0: 7264 696e 6174 6573 0a20 2020 2020 2020  rdinates.       
+000162e0: 205b 696e 642e 5f73 6574 5f70 6f73 282a   [ind._set_pos(*
+000162f0: 636f 6f72 6473 5b69 2c3a 5d29 2066 6f72  coords[i,:]) for
+00016300: 2069 2c20 696e 6420 696e 2065 6e75 6d65   i, ind in enume
+00016310: 7261 7465 2869 6e64 6976 6964 7329 5d0a  rate(individs)].
+00016320: 0a20 2020 2020 2020 2023 2075 7064 6174  .        # updat
+00016330: 6520 7468 6520 696e 6465 7820 7661 6c75  e the index valu
+00016340: 6573 2069 6465 6e74 6966 7969 6e67 2049  es identifying I
+00016350: 6e64 6976 6964 7561 6c73 2069 6e20 676e  ndividuals in gn
+00016360: 7820 616e 6420 7473 6b69 7420 6461 7461  x and tskit data
+00016370: 0a20 2020 2020 2020 206d 6178 5f69 6478  .        max_idx
+00016380: 5f62 3420 3d20 7365 6c66 2e6d 6178 5f69  _b4 = self.max_i
+00016390: 6e64 5f69 6478 0a20 2020 2020 2020 206e  nd_idx.        n
+000163a0: 6577 5f69 6478 7320 3d20 5b5d 0a20 2020  ew_idxs = [].   
+000163b0: 2020 2020 2066 6f72 2069 2c20 696e 6420       for i, ind 
+000163c0: 696e 2065 6e75 6d65 7261 7465 2869 6e64  in enumerate(ind
+000163d0: 6976 6964 7329 3a0a 2020 2020 2020 2020  ivids):.        
+000163e0: 2020 2020 2320 696e 6372 656d 656e 7420      # increment 
+000163f0: 7468 6520 6d61 785f 696e 645f 6964 780a  the max_ind_idx.
+00016400: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016410: 2e6d 6178 5f69 6e64 5f69 6478 202b 3d20  .max_ind_idx += 
+00016420: 310a 2020 2020 2020 2020 2020 2020 2320  1.            # 
+00016430: 7365 7420 7468 6520 496e 6469 7669 6475  set the Individu
+00016440: 616c 2773 2067 6e78 2069 6e64 6578 0a20  al's gnx index. 
+00016450: 2020 2020 2020 2020 2020 2069 6e64 2e69             ind.i
+00016460: 6478 203d 2073 656c 662e 6d61 785f 696e  dx = self.max_in
+00016470: 645f 6964 780a 2020 2020 2020 2020 2020  d_idx.          
+00016480: 2020 6e65 775f 6964 7873 2e61 7070 656e    new_idxs.appen
+00016490: 6428 7365 6c66 2e6d 6178 5f69 6e64 5f69  d(self.max_ind_i
+000164a0: 6478 290a 2020 2020 2020 2020 2020 2020  dx).            
+000164b0: 2320 7365 7420 7468 6520 496e 6469 7669  # set the Indivi
+000164c0: 6475 616c 7327 2069 6473 2066 6f72 2074  duals' ids for t
+000164d0: 6865 2074 736b 6974 206e 6f64 6573 2074  he tskit nodes t
+000164e0: 6162 6c65 0a20 2020 2020 2020 2020 2020  able.           
+000164f0: 2069 6e64 2e5f 6e6f 6465 735f 7461 625f   ind._nodes_tab_
+00016500: 6964 7320 3d20 7b6b 3a20 7620 2b20 7365  ids = {k: v + se
+00016510: 6c66 2e5f 7463 2e6e 6f64 6573 2e6e 756d  lf._tc.nodes.num
+00016520: 5f72 6f77 7320 666f 720a 2020 2020 2020  _rows for.      
+00016530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016550: 2020 2020 2020 6b2c 2076 2069 6e20 696e        k, v in in
+00016560: 642e 5f6e 6f64 6573 5f74 6162 5f69 6473  d._nodes_tab_ids
+00016570: 2e69 7465 6d73 2829 7d0a 2020 2020 2020  .items()}.      
+00016580: 2020 2020 2020 2320 7365 7420 7468 6520        # set the 
+00016590: 496e 6469 7669 6475 616c 7327 2069 6473  Individuals' ids
+000165a0: 2066 6f72 2074 6865 2074 736b 6974 2069   for the tskit i
+000165b0: 6e64 6976 6964 7561 6c73 2074 6162 6c65  ndividuals table
+000165c0: 0a20 2020 2020 2020 2020 2020 2023 204e  .            # N
+000165d0: 4f54 453a 2074 6865 2069 6e76 6572 7365  OTE: the inverse
+000165e0: 2028 7468 6520 496e 6469 7669 6475 616c   (the Individual
+000165f0: 7327 2067 6e78 2069 6478 2076 616c 7565  s' gnx idx value
+00016600: 732c 0a20 2020 2020 2020 2020 2020 2023  s,.            #
+00016610: 2020 2020 2020 2061 7320 7265 636f 7265         as recore
+00016620: 6420 696e 2074 6865 2074 736b 6974 2069  d in the tskit i
+00016630: 6e64 6976 6964 7561 6c73 2074 6162 6c65  ndividuals table
+00016640: 2773 0a20 2020 2020 2020 2020 2020 2023  's.            #
+00016650: 2020 2020 2020 206d 6574 6164 6174 6129         metadata)
+00016660: 2073 686f 756c 6420 616c 7265 6164 7920   should already 
+00016670: 6265 2063 6f72 7265 6374 0a20 2020 2020  be correct.     
+00016680: 2020 2020 2020 2023 2020 2020 2020 2062         #       b
+00016690: 6563 6175 7365 205f 7072 6570 5f74 736b  ecause _prep_tsk
+000166a0: 6974 5f74 6162 636f 6c6c 5f66 6f72 5f67  it_tabcoll_for_g
+000166b0: 6e78 5f73 7070 5f75 6e69 6f6e 0a20 2020  nx_spp_union.   
+000166c0: 2020 2020 2020 2020 2023 2020 2020 2020           #      
+000166d0: 2067 656e 6572 6174 6564 2074 6865 2069   generated the i
+000166e0: 6e64 6578 2076 616c 7565 730a 2020 2020  ndex values.    
+000166f0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00016700: 616e 6420 7365 7420 7468 656d 2069 6e20  and set them in 
+00016710: 7468 6520 5461 626c 6543 6f6c 6c65 6374  the TableCollect
+00016720: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00016730: 696e 642e 5f69 6e64 6976 6964 7561 6c73  ind._individuals
+00016740: 5f74 6162 5f69 6420 2b3d 2073 656c 662e  _tab_id += self.
+00016750: 5f74 632e 696e 6469 7669 6475 616c 732e  _tc.individuals.
+00016760: 6e75 6d5f 726f 7773 0a20 2020 2020 2020  num_rows.       
+00016770: 206d 6178 5f69 6478 5f61 6620 3d20 7365   max_idx_af = se
+00016780: 6c66 2e6d 6178 5f69 6e64 5f69 6478 0a20  lf.max_ind_idx. 
+00016790: 2020 2020 2020 2061 7373 6572 7420 6d61         assert ma
+000167a0: 785f 6964 785f 6166 202d 206d 6178 5f69  x_idx_af - max_i
+000167b0: 6478 5f62 3420 3d3d 206c 656e 2869 6e64  dx_b4 == len(ind
+000167c0: 6976 6964 7329 0a20 2020 2020 2020 2023  ivids).        #
+000167d0: 2063 6f6d 7061 7265 2074 6865 206e 6578   compare the nex
+000167e0: 7420 6964 7820 7661 6c75 6573 2067 656e  t idx values gen
+000167f0: 6572 6174 6564 2061 7420 746f 7020 6f66  erated at top of
+00016800: 2074 6869 7320 6675 6e63 7469 6f6e 2077   this function w
+00016810: 6974 680a 2020 2020 2020 2020 2320 7468  ith.        # th
+00016820: 6f73 6520 7265 7475 726e 6564 2062 7920  ose returned by 
+00016830: 5f70 7265 705f 7473 6b69 745f 7461 6263  _prep_tskit_tabc
+00016840: 6f6c 6c5f 666f 725f 676e 785f 7370 705f  oll_for_gnx_spp_
+00016850: 756e 696f 6e0a 2020 2020 2020 2020 6173  union.        as
+00016860: 7365 7274 2073 6574 286e 6578 745f 6e5f  sert set(next_n_
+00016870: 6964 7873 2920 3d3d 2073 6574 286e 6578  idxs) == set(nex
+00016880: 745f 676e 785f 6964 7873 292c 2028 2274  t_gnx_idxs), ("t
+00016890: 6865 206e 6578 7420 6e20 6964 7873 2022  he next n idxs "
+000168a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000168b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168c0: 2022 6361 6c63 756c 6174 6564 2062 7920   "calculated by 
+000168d0: 5f61 6464 5f69 6e64 6976 6964 7561 6c73  _add_individuals
+000168e0: 2064 6966 6665 7220 6672 6f6d 2022 0a20   differ from ". 
+000168f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016900: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00016910: 7468 6f73 6520 7265 7475 726e 6564 2062  those returned b
+00016920: 7920 220a 2020 2020 2020 2020 2020 2020  y ".            
+00016930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016940: 2020 2020 225f 7072 6570 5f74 736b 6974      "_prep_tskit
+00016950: 5f74 6162 636f 6c6c 5f66 6f72 5f67 6e78  _tabcoll_for_gnx
+00016960: 5f73 7070 5f75 6e69 6f6e 2229 0a20 2020  _spp_union").   
+00016970: 2020 2020 2023 2063 6f6d 7061 7265 2074       # compare t
+00016980: 6865 2069 6478 2076 616c 7565 7320 7468  he idx values th
+00016990: 6174 2077 6572 6520 7365 7420 6f6e 2074  at were set on t
+000169a0: 6865 2049 6e64 6976 6964 7561 6c73 2074  he Individuals t
+000169b0: 6f20 7468 6f73 6520 7468 6174 0a20 2020  o those that.   
+000169c0: 2020 2020 2023 2077 6572 6520 7365 7420       # were set 
+000169d0: 696e 2074 6865 2054 6162 6c65 436f 6c6c  in the TableColl
+000169e0: 6563 7469 6f6e 2e69 6e64 6976 6964 7561  ection.individua
+000169f0: 6c73 2074 6162 6c65 0a20 2020 2020 2020  ls table.       
+00016a00: 2061 7373 6572 7420 6e70 2e61 6c6c 286e   assert np.all(n
+00016a10: 702e 6172 7261 7928 6e65 7874 5f67 6e78  p.array(next_gnx
+00016a20: 5f69 6478 7329 203d 3d20 6e70 2e61 7272  _idxs) == np.arr
+00016a30: 6179 286e 6577 5f69 6478 7329 292c 2028  ay(new_idxs)), (
+00016a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00016a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a60: 2020 2020 2020 2020 2320 4e4f 5445 3a20          # NOTE: 
-00016a70: 2866 6f72 206e 6f77 2061 7420 6c65 6173  (for now at leas
-00016a80: 7429 2061 7373 756d 696e 6720 2074 6865  t) assuming  the
-00016a90: 2069 6e74 726f 6475 6365 640a 2020 2020   introduced.    
-00016aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ab0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00016ac0: 696e 6469 7669 6475 616c 7320 636f 6d65  individuals come
-00016ad0: 2066 726f 6d20 746f 7461 6c6c 7920 696e   from totally in
-00016ae0: 6465 7020 706f 702c 0a20 2020 2020 2020  dep pop,.       
-00016af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b00: 2020 2020 2023 2020 2020 2020 2064 6f20       #       do 
-00016b10: 6e6f 7420 7368 6172 6520 6120 4d52 4341  not share a MRCA
-00016b20: 2077 6974 6869 6e20 6f75 7220 6461 7461   within our data
-00016b30: 2c20 616e 6420 e288 b420 2020 0a20 2020  , and ...   .   
-00016b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b50: 2020 2020 2020 2020 2023 2020 2020 2020           #      
-00016b60: 2068 6176 6520 6e6f 2063 6f6d 6d6f 6e20   have no common 
-00016b70: 6e6f 6465 7320 7468 6174 206e 6565 6420  nodes that need 
-00016b80: 746f 2062 6520 6d61 7070 6564 2c0a 2020  to be mapped,.  
-00016b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ba0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00016bb0: 2020 6865 6e63 6520 7765 2070 726f 7669    hence we provi
-00016bc0: 6465 2061 206c 6973 7420 6f66 2074 736b  de a list of tsk
-00016bd0: 6974 2e4e 554c 4c73 0a20 2020 2020 2020  it.NULLs.       
-00016be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bf0: 2020 2020 2023 2020 2020 2020 2074 6f20       #       to 
-00016c00: 756e 696f 6e28 2927 7320 6e6f 6465 5f6d  union()'s node_m
-00016c10: 6170 7069 6e67 2061 7267 756d 656e 740a  apping argument.
-00016c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c30: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
-00016c40: 5f6d 6170 7069 6e67 3d5b 7473 6b69 742e  _mapping=[tskit.
-00016c50: 4e55 4c4c 5d20 2a73 6f75 7263 655f 7463  NULL] *source_tc
-00016c60: 2e6e 6f64 6573 2e6e 756d 5f72 6f77 732c  .nodes.num_rows,
-00016c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016c80: 2020 2020 2020 2020 2020 2020 2023 204e               # N
-00016c90: 4f54 453a 2070 6f70 756c 6174 696f 6e73  OTE: populations
-00016ca0: 206f 6620 7468 6520 6e65 776c 7920 6164   of the newly ad
-00016cb0: 6465 6420 6e6f 6465 730a 2020 2020 2020  ded nodes.      
-00016cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cd0: 2020 2020 2020 2320 2020 2020 2020 7769        #       wi
-00016ce0: 6c6c 2062 6520 666c 6167 6765 6420 6279  ll be flagged by
-00016cf0: 2061 6e20 696e 7465 6765 720a 2020 2020   an integer.    
+00016a60: 2020 2249 6e64 6976 6964 6175 6c20 6964    "Individaul id
+00016a70: 7820 7661 6c75 6573 2073 6574 2069 6e20  x values set in 
+00016a80: 7468 6520 220a 2020 2020 2020 2020 2020  the ".          
+00016a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016aa0: 2020 2020 2020 2020 2020 2254 6162 6c65            "Table
+00016ab0: 436f 6c6c 6563 7469 6f6e 2e69 6e64 6976  Collection.indiv
+00016ac0: 6964 7561 6c73 2022 0a20 2020 2020 2020  iduals ".       
+00016ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ae0: 2020 2020 2020 2020 2020 2020 2022 7461               "ta
+00016af0: 626c 6520 646f 206e 6f74 2061 6772 6565  ble do not agree
+00016b00: 2077 6974 6820 7468 6f73 6520 7365 7420   with those set 
+00016b10: 6f6e 2074 6865 2022 0a20 2020 2020 2020  on the ".       
+00016b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b30: 2020 2020 2020 2020 2020 2020 2022 496e               "In
+00016b40: 6469 7669 6475 616c 7320 7468 656d 7365  dividuals themse
+00016b50: 6c76 6573 2e22 290a 0a20 2020 2020 2020  lves.")..       
+00016b60: 2023 2073 6f72 7420 616e 6420 7369 6d70   # sort and simp
+00016b70: 6c69 6679 2074 6865 2074 736b 6974 2e54  lify the tskit.T
+00016b80: 6162 6c65 436f 6c6c 6563 7469 6f6e 0a20  ableCollection. 
+00016b90: 2020 2020 2020 2073 656c 662e 5f73 6f72         self._sor
+00016ba0: 745f 616e 645f 7369 6d70 6c69 6679 5f74  t_and_simplify_t
+00016bb0: 6162 6c65 5f63 6f6c 6c65 6374 696f 6e28  able_collection(
+00016bc0: 290a 0a20 2020 2020 2020 2023 2075 6e69  )..        # uni
+00016bd0: 6f6e 2073 6f75 7263 6520 696e 6469 7669  on source indivi
+00016be0: 6475 616c 7327 2054 6162 6c65 436f 6c6c  duals' TableColl
+00016bf0: 6563 7469 6f6e 2069 6e74 6f20 7468 6973  ection into this
+00016c00: 2053 7065 6369 6573 2720 5461 626c 6543   Species' TableC
+00016c10: 6f6c 6c0a 2020 2020 2020 2020 6e6f 6465  oll.        node
+00016c20: 735f 7461 625f 6c65 6e5f 6234 203d 2073  s_tab_len_b4 = s
+00016c30: 656c 662e 5f74 632e 6e6f 6465 732e 6e75  elf._tc.nodes.nu
+00016c40: 6d5f 726f 7773 0a20 2020 2020 2020 2069  m_rows.        i
+00016c50: 6e64 6976 6964 735f 7461 625f 6c65 6e5f  ndivids_tab_len_
+00016c60: 6234 203d 2073 656c 662e 5f74 632e 696e  b4 = self._tc.in
+00016c70: 6469 7669 6475 616c 732e 6e75 6d5f 726f  dividuals.num_ro
+00016c80: 7773 0a20 2020 2020 2020 2073 656c 662e  ws.        self.
+00016c90: 5f74 632e 756e 696f 6e28 736f 7572 6365  _tc.union(source
+00016ca0: 5f74 632c 0a20 2020 2020 2020 2020 2020  _tc,.           
+00016cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016cc0: 2023 204e 4f54 453a 2028 666f 7220 6e6f   # NOTE: (for no
+00016cd0: 7720 6174 206c 6561 7374 2920 6173 7375  w at least) assu
+00016ce0: 6d69 6e67 2020 7468 6520 696e 7472 6f64  ming  the introd
+00016cf0: 7563 6564 0a20 2020 2020 2020 2020 2020  uced.           
 00016d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d10: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00016d20: 7468 6174 2069 7320 3120 6772 6561 7465  that is 1 greate
-00016d30: 7220 7468 616e 2074 6865 206c 6172 6765  r than the large
-00016d40: 7374 0a20 2020 2020 2020 2020 2020 2020  st.             
-00016d50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00016d60: 2020 2020 2020 2070 6f70 756c 6174 696f         populatio
-00016d70: 6e2d 666c 6167 2069 6e74 6567 6572 2069  n-flag integer i
-00016d80: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00016d90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00016da0: 2020 2020 2020 7468 6520 7072 652d 696e        the pre-in
-00016db0: 7472 6f64 7563 7469 6f6e 2054 6162 6c65  troduction Table
-00016dc0: 436f 6c6c 6563 7469 6f6e 0a20 2020 2020  Collection.     
-00016dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016de0: 2020 2020 2020 2023 2020 2020 2020 206f         #       o
-00016df0: 6620 7468 6973 2053 7065 6369 6573 0a20  f this Species. 
-00016e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e10: 2020 2020 2020 2020 2020 2061 6464 5f70             add_p
-00016e20: 6f70 756c 6174 696f 6e73 3d54 7275 652c  opulations=True,
-00016e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016e40: 2020 2020 2020 2020 2020 2020 2023 204e               # N
-00016e50: 4f54 453a 2062 6573 7420 746f 206a 7573  OTE: best to jus
-00016e60: 7420 616c 6c6f 7720 6974 2074 6f20 646f  t allow it to do
-00016e70: 2074 6869 732c 0a20 2020 2020 2020 2020   this,.         
+00016d10: 2023 2020 2020 2020 2069 6e64 6976 6964   #       individ
+00016d20: 7561 6c73 2063 6f6d 6520 6672 6f6d 2074  uals come from t
+00016d30: 6f74 616c 6c79 2069 6e64 6570 2070 6f70  otally indep pop
+00016d40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016d50: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00016d60: 2020 2020 2020 646f 206e 6f74 2073 6861        do not sha
+00016d70: 7265 2061 204d 5243 4120 7769 7468 696e  re a MRCA within
+00016d80: 206f 7572 2064 6174 612c 2061 6e64 20e2   our data, and .
+00016d90: 88b4 2020 200a 2020 2020 2020 2020 2020  ..   .          
+00016da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016db0: 2020 2320 2020 2020 2020 6861 7665 206e    #       have n
+00016dc0: 6f20 636f 6d6d 6f6e 206e 6f64 6573 2074  o common nodes t
+00016dd0: 6861 7420 6e65 6564 2074 6f20 6265 206d  hat need to be m
+00016de0: 6170 7065 642c 0a20 2020 2020 2020 2020  apped,.         
+00016df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e00: 2020 2023 2020 2020 2020 2068 656e 6365     #       hence
+00016e10: 2077 6520 7072 6f76 6964 6520 6120 6c69   we provide a li
+00016e20: 7374 206f 6620 7473 6b69 742e 4e55 4c4c  st of tskit.NULL
+00016e30: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00016e40: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00016e50: 2020 2020 2020 746f 2075 6e69 6f6e 2829        to union()
+00016e60: 2773 206e 6f64 655f 6d61 7070 696e 6720  's node_mapping 
+00016e70: 6172 6775 6d65 6e74 0a20 2020 2020 2020  argument.       
 00016e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e90: 2020 2023 2020 2020 2020 2069 6e20 6361     #       in ca
-00016ea0: 7365 2077 6520 6765 6e65 7261 6c69 7a65  se we generalize
-00016eb0: 2074 6869 6e67 7320 6c61 7465 7220 6f6e   things later on
-00016ec0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00016ed0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00016ee0: 2020 2020 2020 6275 7420 666f 7220 6e6f        but for no
-00016ef0: 7720 7468 6572 6520 7769 6c6c 2061 6374  w there will act
-00016f00: 7561 6c6c 7920 6265 0a20 2020 2020 2020  ually be.       
-00016f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f20: 2020 2020 2023 2020 2020 2020 206e 6f74       #       not
-00016f30: 6869 6e67 2074 6f20 6368 6563 6b20 6265  hing to check be
-00016f40: 6361 7573 6520 7765 2061 7373 756d 6520  cause we assume 
-00016f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016f60: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-00016f70: 2020 2020 206e 6f20 7368 6172 6564 206e       no shared n
-00016f80: 6f64 6573 2062 6574 7765 656e 0a20 2020  odes between.   
-00016f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fa0: 2020 2020 2020 2020 2023 2020 2020 2020           #      
-00016fb0: 2073 6f75 7263 6520 616e 6420 7265 6369   source and reci
-00016fc0: 7069 656e 7420 5461 626c 6543 6f6c 6c65  pient TableColle
-00016fd0: 6374 696f 6e73 0a20 2020 2020 2020 2020  ctions.         
+00016e90: 2020 2020 206e 6f64 655f 6d61 7070 696e       node_mappin
+00016ea0: 673d 5b74 736b 6974 2e4e 554c 4c5d 202a  g=[tskit.NULL] *
+00016eb0: 736f 7572 6365 5f74 632e 6e6f 6465 732e  source_tc.nodes.
+00016ec0: 6e75 6d5f 726f 7773 2c0a 2020 2020 2020  num_rows,.      
+00016ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ee0: 2020 2020 2020 2320 4e4f 5445 3a20 706f        # NOTE: po
+00016ef0: 7075 6c61 7469 6f6e 7320 6f66 2074 6865  pulations of the
+00016f00: 206e 6577 6c79 2061 6464 6564 206e 6f64   newly added nod
+00016f10: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00016f20: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00016f30: 2020 2020 2020 2077 696c 6c20 6265 2066         will be f
+00016f40: 6c61 6767 6564 2062 7920 616e 2069 6e74  lagged by an int
+00016f50: 6567 6572 0a20 2020 2020 2020 2020 2020  eger.           
+00016f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f70: 2023 2020 2020 2020 2074 6861 7420 6973   #       that is
+00016f80: 2031 2067 7265 6174 6572 2074 6861 6e20   1 greater than 
+00016f90: 7468 6520 6c61 7267 6573 740a 2020 2020  the largest.    
+00016fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fb0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00016fc0: 706f 7075 6c61 7469 6f6e 2d66 6c61 6720  population-flag 
+00016fd0: 696e 7465 6765 7220 696e 0a20 2020 2020  integer in.     
 00016fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ff0: 2020 2023 2054 4f44 4f3a 2048 4f57 4556     # TODO: HOWEV
-00017000: 4552 2c20 4551 5541 4c49 5459 2043 4845  ER, EQUALITY CHE
-00017010: 434b 2053 5449 4c4c 2046 4149 4c53 2120  CK STILL FAILS! 
-00017020: 5748 593f 0a20 2020 2020 2020 2020 2020  WHY?.           
+00016ff0: 2020 2020 2020 2023 2020 2020 2020 2074         #       t
+00017000: 6865 2070 7265 2d69 6e74 726f 6475 6374  he pre-introduct
+00017010: 696f 6e20 5461 626c 6543 6f6c 6c65 6374  ion TableCollect
+00017020: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
 00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017040: 2063 6865 636b 5f73 6861 7265 645f 6571   check_shared_eq
-00017050: 7561 6c69 7479 3d46 616c 7365 2c0a 2020  uality=False,.  
+00017040: 2320 2020 2020 2020 6f66 2074 6869 7320  #       of this 
+00017050: 5370 6563 6965 730a 2020 2020 2020 2020  Species.        
 00017060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017070: 2020 2020 2020 2020 2020 2320 4e4f 5445            # NOTE
-00017080: 3a20 7368 6f75 6c64 2063 6f70 7920 7072  : should copy pr
-00017090: 6f76 656e 616e 6365 2069 6e66 6f20 6f76  ovenance info ov
-000170a0: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
-000170b0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000170c0: 2020 2020 2020 2066 726f 6d20 7468 6520         from the 
-000170d0: 736f 7572 6365 2049 6e64 6976 6964 7561  source Individua
-000170e0: 6c73 2720 5461 626c 6543 6f6c 6c65 6374  ls' TableCollect
-000170f0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00017100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017110: 2320 2020 2020 2020 746f 2074 6861 7420  #       to that 
-00017120: 6f66 2074 6865 2072 6563 6569 7069 656e  of the receipien
-00017130: 7420 5370 6563 6965 730a 2020 2020 2020  t Species.      
-00017140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017150: 2020 2020 2020 7265 636f 7264 5f70 726f        record_pro
-00017160: 7665 6e61 6e63 653d 5472 7565 2c0a 2020  venance=True,.  
-00017170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017180: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00017190: 0a20 2020 2020 2020 206e 6f64 6573 5f74  .        nodes_t
-000171a0: 6162 5f6c 656e 5f61 6620 3d20 7365 6c66  ab_len_af = self
-000171b0: 2e5f 7463 2e6e 6f64 6573 2e6e 756d 5f72  ._tc.nodes.num_r
-000171c0: 6f77 730a 2020 2020 2020 2020 696e 6469  ows.        indi
-000171d0: 7669 6473 5f74 6162 5f6c 656e 5f61 6620  vids_tab_len_af 
-000171e0: 3d20 7365 6c66 2e5f 7463 2e69 6e64 6976  = self._tc.indiv
-000171f0: 6964 7561 6c73 2e6e 756d 5f72 6f77 730a  iduals.num_rows.
-00017200: 0a20 2020 2020 2020 2023 2063 6865 636b  .        # check
-00017210: 2075 6e69 6f6e 6564 2074 6162 6c65 7320   unioned tables 
-00017220: 6861 7665 2063 6f72 7265 6374 206c 656e  have correct len
-00017230: 6774 6873 0a20 2020 2020 2020 2061 7373  gths.        ass
-00017240: 6572 7420 286e 6f64 6573 5f74 6162 5f6c  ert (nodes_tab_l
-00017250: 656e 5f61 6620 2d20 6e6f 6465 735f 7461  en_af - nodes_ta
-00017260: 625f 6c65 6e5f 6234 2920 3d3d 2073 6f75  b_len_b4) == sou
-00017270: 7263 655f 7463 2e6e 6f64 6573 2e6e 756d  rce_tc.nodes.num
-00017280: 5f72 6f77 730a 2020 2020 2020 2020 6173  _rows.        as
-00017290: 7365 7274 2028 2869 6e64 6976 6964 735f  sert ((individs_
-000172a0: 7461 625f 6c65 6e5f 6166 202d 2069 6e64  tab_len_af - ind
-000172b0: 6976 6964 735f 7461 625f 6c65 6e5f 6234  ivids_tab_len_b4
-000172c0: 2920 3d3d 0a20 2020 2020 2020 2020 2020  ) ==.           
-000172d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172f0: 2020 2020 2073 6f75 7263 655f 7463 2e69       source_tc.i
-00017300: 6e64 6976 6964 7561 6c73 2e6e 756d 5f72  ndividuals.num_r
-00017310: 6f77 7329 0a0a 2020 2020 2020 2020 2320  ows)..        # 
-00017320: 6368 6563 6b20 7468 6174 2061 6c6c 2067  check that all g
-00017330: 6e78 2069 6478 7320 7374 6f72 6564 2069  nx idxs stored i
-00017340: 6e20 7468 6520 696e 6469 7669 6475 616c  n the individual
-00017350: 7320 7461 626c 6527 730a 2020 2020 2020  s table's.      
-00017360: 2020 2320 6d65 7461 6461 7461 2063 6f6c    # metadata col
-00017370: 756d 6e20 6f63 6375 7220 6f6e 6c79 206f  umn occur only o
-00017380: 6e63 6520 2861 7369 6465 2066 726f 6d20  nce (aside from 
-00017390: 302c 0a20 2020 2020 2020 2023 2077 6869  0,.        # whi
-000173a0: 6368 2069 7320 6120 6e75 6c6c 2076 616c  ch is a null val
-000173b0: 7565 2066 6f72 2069 6e64 6976 6964 7561  ue for individua
-000173c0: 6c73 2074 6861 740a 2020 2020 2020 2020  ls that.        
-000173d0: 2320 6e65 7665 7220 6578 6973 7465 6420  # never existed 
-000173e0: 6173 2027 7265 616c 2720 676e 7820 496e  as 'real' gnx In
-000173f0: 6469 7669 6475 616c 206f 626a 6563 7473  dividual objects
-00017400: 2062 6563 6175 7365 0a20 2020 2020 2020   because.       
-00017410: 2023 2074 6865 7920 7765 7265 2069 6e20   # they were in 
-00017420: 7468 6520 7061 7374 206f 6620 6120 636f  the past of a co
-00017430: 616c 6573 6365 6e74 2073 696d 756c 6174  alescent simulat
-00017440: 696f 6e29 0a20 2020 2020 2020 2072 6563  ion).        rec
-00017450: 6970 5f74 635f 696e 6469 7669 6475 616c  ip_tc_individual
-00017460: 735f 6964 7320 3d20 5b69 6e74 2e66 726f  s_ids = [int.fro
-00017470: 6d5f 6279 7465 7328 0a20 2020 2020 2020  m_bytes(.       
-00017480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017490: 2020 2020 2073 656c 662e 5f74 632e 696e       self._tc.in
-000174a0: 6469 7669 6475 616c 735b 695d 2e6d 6574  dividuals[i].met
-000174b0: 6164 6174 612c 2027 6c69 7474 6c65 2729  adata, 'little')
-000174c0: 2066 6f72 0a20 2020 2020 2020 2020 2020   for.           
-000174d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174e0: 2020 2020 2069 2069 6e20 7261 6e67 6528       i in range(
-000174f0: 7365 6c66 2e5f 7463 2e69 6e64 6976 6964  self._tc.individ
-00017500: 7561 6c73 2e6e 756d 5f72 6f77 7329 5d0a  uals.num_rows)].
-00017510: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
-00017520: 6c65 6e28 7265 6369 705f 7463 5f69 6e64  len(recip_tc_ind
-00017530: 6976 6964 7561 6c73 5f69 6473 2920 3d3d  ividuals_ids) ==
-00017540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017550: 2073 656c 662e 5f74 632e 696e 6469 7669   self._tc.indivi
-00017560: 6475 616c 732e 6e75 6d5f 726f 7773 290a  duals.num_rows).
-00017570: 2020 2020 2020 2020 636f 756e 7473 203d          counts =
-00017580: 2043 2872 6563 6970 5f74 635f 696e 6469   C(recip_tc_indi
-00017590: 7669 6475 616c 735f 6964 7329 0a20 2020  viduals_ids).   
-000175a0: 2020 2020 2066 6f72 206b 2c20 7620 696e       for k, v in
-000175b0: 2063 6f75 6e74 732e 6974 656d 7328 293a   counts.items():
-000175c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000175d0: 6b20 213d 2030 3a0a 2020 2020 2020 2020  k != 0:.        
-000175e0: 2020 2020 2020 2020 6173 7365 7274 2076          assert v
-000175f0: 203d 3d20 312c 2028 6622 676e 7820 496e   == 1, (f"gnx In
-00017600: 6469 7669 6475 616c 2069 6478 207b 697d  dividual idx {i}
-00017610: 206f 6363 7572 7320 6d6f 7265 2074 6861   occurs more tha
-00017620: 6e20 6f6e 6365 2022 0a20 2020 2020 2020  n once ".       
-00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017640: 2020 2020 2020 2020 2020 2269 6e20 7468            "in th
-00017650: 6520 6d65 7461 6461 7461 2063 6f6c 756d  e metadata colum
-00017660: 6e20 6f66 2074 6865 2075 6e69 6f6e 206f  n of the union o
-00017670: 6620 220a 2020 2020 2020 2020 2020 2020  f ".            
-00017680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017690: 2020 2020 2022 7468 6520 7265 6369 7069       "the recipi
-000176a0: 656e 7420 616e 6420 736f 7572 6365 2053  ent and source S
-000176b0: 7065 6369 6573 2720 220a 2020 2020 2020  pecies' ".      
-000176c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176d0: 2020 2020 2020 2020 2020 2022 5461 626c             "Tabl
-000176e0: 6543 6f6c 6c65 6374 696f 6e73 2069 6e64  eCollections ind
-000176f0: 6976 6964 7561 6c73 2074 6162 6c65 732e  ividuals tables.
-00017700: 2229 0a0a 2020 2020 2020 2020 2320 6164  ")..        # ad
-00017710: 6420 696e 2074 6865 2049 6e64 6976 6964  d in the Individ
-00017720: 7561 6c73 2c20 6b65 7965 6420 6279 2069  uals, keyed by i
-00017730: 6478 0a20 2020 2020 2020 2070 6f70 5f73  dx.        pop_s
-00017740: 697a 655f 6234 203d 206c 656e 2873 656c  ize_b4 = len(sel
-00017750: 6629 0a20 2020 2020 2020 2066 6f72 2069  f).        for i
-00017760: 6e64 2069 6e20 696e 6469 7669 6473 3a0a  nd in individs:.
-00017770: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017780: 5b69 6e64 2e69 6478 5d20 3d20 696e 640a  [ind.idx] = ind.
-00017790: 2020 2020 2020 2020 706f 705f 7369 7a65          pop_size
-000177a0: 5f61 6620 3d20 6c65 6e28 7365 6c66 290a  _af = len(self).
-000177b0: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
-000177c0: 706f 705f 7369 7a65 5f61 6620 2d20 706f  pop_size_af - po
-000177d0: 705f 7369 7a65 5f62 3429 203d 3d20 6c65  p_size_b4) == le
-000177e0: 6e28 696e 6469 7669 6473 292c 2028 2249  n(individs), ("I
-000177f0: 6e63 6f72 7265 6374 206e 756d 6265 7222  ncorrect number"
-00017800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017820: 2022 206f 6620 496e 6469 7669 6475 616c   " of Individual
-00017830: 7320 6164 6465 6420 746f 2072 6563 6970  s added to recip
-00017840: 6965 6e74 2053 7065 6369 6573 2e22 290a  ient Species.").
-00017850: 0a20 2020 2020 2020 2023 2075 7064 6174  .        # updat
-00017860: 6520 6561 6368 2049 6e64 6976 6964 7561  e each Individua
-00017870: 6c27 7320 5f69 6e64 6976 6964 7561 6c73  l's _individuals
-00017880: 5f74 6162 5f69 6420 616e 6420 5f6e 6f64  _tab_id and _nod
-00017890: 6573 5f74 6162 5f69 6473 0a20 2020 2020  es_tab_ids.     
-000178a0: 2020 2023 2074 6f20 6d61 7463 6820 7468     # to match th
-000178b0: 6520 6e65 772c 2075 6e69 6f6e 6564 2054  e new, unioned T
-000178c0: 6162 6c65 436f 6c6c 6563 7469 6f6e 0a20  ableCollection. 
-000178d0: 2020 2020 2020 206e 6f64 6573 5f74 6162         nodes_tab
-000178e0: 5f69 6e64 6976 6964 7561 6c73 203d 2073  _individuals = s
-000178f0: 656c 662e 5f74 632e 6e6f 6465 732e 696e  elf._tc.nodes.in
-00017900: 6469 7669 6475 616c 0a20 2020 2020 2020  dividual.       
-00017910: 2066 6f72 2069 6478 2c20 696e 6420 696e   for idx, ind in
-00017920: 2073 656c 662e 6974 656d 7328 293a 0a20   self.items():. 
-00017930: 2020 2020 2020 2020 2020 2069 6e64 6976             indiv
-00017940: 6964 7561 6c73 5f74 6162 5f69 6420 3d20  iduals_tab_id = 
-00017950: 6e70 2e61 7267 7768 6572 6528 0a20 2020  np.argwhere(.   
-00017960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017970: 2020 2020 2020 2020 206e 702e 6172 7261           np.arra
-00017980: 7928 7265 6369 705f 7463 5f69 6e64 6976  y(recip_tc_indiv
-00017990: 6964 7561 6c73 5f69 6473 2920 3d3d 2069  iduals_ids) == i
-000179a0: 6478 292e 7261 7665 6c28 290a 2020 2020  dx).ravel().    
-000179b0: 2020 2020 2020 2020 6173 7365 7274 206c          assert l
-000179c0: 656e 2869 6e64 6976 6964 7561 6c73 5f74  en(individuals_t
-000179d0: 6162 5f69 6429 203d 3d20 310a 2020 2020  ab_id) == 1.    
-000179e0: 2020 2020 2020 2020 696e 6469 7669 6475          individu
-000179f0: 616c 735f 7461 625f 6964 203d 2069 6e64  als_tab_id = ind
-00017a00: 6976 6964 7561 6c73 5f74 6162 5f69 645b  ividuals_tab_id[
-00017a10: 305d 0a20 2020 2020 2020 2020 2020 2069  0].            i
-00017a20: 6e64 2e5f 696e 6469 7669 6475 616c 735f  nd._individuals_
-00017a30: 7461 625f 6964 203d 2069 6e64 6976 6964  tab_id = individ
-00017a40: 7561 6c73 5f74 6162 5f69 640a 2020 2020  uals_tab_id.    
-00017a50: 2020 2020 2020 2020 6e6f 6465 735f 7461          nodes_ta
-00017a60: 625f 6964 7320 3d20 6e70 2e61 7267 7768  b_ids = np.argwh
-00017a70: 6572 6528 6e6f 6465 735f 7461 625f 696e  ere(nodes_tab_in
-00017a80: 6469 7669 6475 616c 7320 3d3d 0a20 2020  dividuals ==.   
-00017a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ab0: 2020 2020 2069 6e64 6976 6964 7561 6c73       individuals
-00017ac0: 5f74 6162 5f69 6429 2e72 6176 656c 2829  _tab_id).ravel()
-00017ad0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00017ae0: 6572 7420 6c65 6e28 6e6f 6465 735f 7461  ert len(nodes_ta
-00017af0: 625f 6964 7329 203d 3d20 320a 2020 2020  b_ids) == 2.    
-00017b00: 2020 2020 2020 2020 696e 642e 5f6e 6f64          ind._nod
-00017b10: 6573 5f74 6162 5f69 6473 203d 207b 693a  es_tab_ids = {i:
-00017b20: 2069 6420 666f 7220 692c 2069 6420 696e   id for i, id in
-00017b30: 2065 6e75 6d65 7261 7465 286e 6f64 6573   enumerate(nodes
-00017b40: 5f74 6162 5f69 6473 297d 0a0a 2020 2020  _tab_ids)}..    
-00017b50: 2020 2020 2320 6669 6e61 6c20 6368 6563      # final chec
-00017b60: 6b20 7468 6174 2069 6e64 6963 6573 2063  k that indices c
-00017b70: 6865 636b 206f 7574 2069 6e20 7468 6520  heck out in the 
-00017b80: 6f74 6865 7220 6469 7265 6374 696f 6e0a  other direction.
-00017b90: 2020 2020 2020 2020 2320 2869 2e65 2e2c          # (i.e.,
-00017ba0: 2066 726f 6d20 6e6f 6465 7320 7461 6220   from nodes tab 
-00017bb0: 746f 2069 6e64 6976 6964 7561 6c73 2074  to individuals t
-00017bc0: 6162 2074 6f20 676e 7820 496e 6469 7669  ab to gnx Indivi
-00017bd0: 6475 616c 730a 2020 2020 2020 2020 2320  duals.        # 
-00017be0: 616e 6420 7468 6174 206e 6f64 6573 2069  and that nodes i
-00017bf0: 6473 2063 6865 636b 206f 7574 2074 6f6f  ds check out too
-00017c00: 0a20 2020 2020 2020 2063 7572 725f 6e6f  .        curr_no
-00017c10: 6465 5f63 7420 3d20 300a 2020 2020 2020  de_ct = 0.      
-00017c20: 2020 666f 7220 6e6f 6465 5f69 642c 206e    for node_id, n
-00017c30: 6f64 6520 696e 2065 6e75 6d65 7261 7465  ode in enumerate
-00017c40: 2873 656c 662e 5f74 632e 6e6f 6465 7329  (self._tc.nodes)
-00017c50: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00017c60: 4e4f 5445 3a20 6967 6e6f 7265 202d 3173  NOTE: ignore -1s
-00017c70: 3b20 7468 6579 2061 7265 206d 7370 7269  ; they are mspri
-00017c80: 6d65 2066 6c61 6773 2066 6f72 206e 6f6e  me flags for non
-00017c90: 2d73 616d 706c 6520 6e6f 6465 7320 6275  -sample nodes bu
-00017ca0: 740a 2020 2020 2020 2020 2020 2020 2320  t.            # 
-00017cb0: 2020 2020 2020 6265 6168 7665 2061 7320        beahve as 
-00017cc0: 6120 5079 7468 6f6e 2069 6e64 6578 6572  a Python indexer
-00017cd0: 206f 6620 7468 6520 6c61 7374 2049 6e64   of the last Ind
-00017ce0: 6976 6964 7561 6c20 696e 2074 6865 0a20  ividual in the. 
-00017cf0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-00017d00: 2020 2053 7065 6369 6573 2061 6e64 2074     Species and t
-00017d10: 6875 7320 7468 726f 7720 616e 2065 7272  hus throw an err
-00017d20: 6f72 0a20 2020 2020 2020 2020 2020 2069  or.            i
-00017d30: 6620 6e6f 6465 2e69 6e64 6976 6964 7561  f node.individua
-00017d40: 6c20 213d 202d 313a 0a20 2020 2020 2020  l != -1:.       
-00017d50: 2020 2020 2020 2020 2067 6e78 5f69 6e64           gnx_ind
-00017d60: 6976 6964 7561 6c5f 6964 203d 2069 6e74  ividual_id = int
-00017d70: 2e66 726f 6d5f 6279 7465 7328 7365 6c66  .from_bytes(self
-00017d80: 2e5f 7463 2e69 6e64 6976 6964 7561 6c73  ._tc.individuals
-00017d90: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00017da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017db0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00017dc0: 6465 2e69 6e64 6976 6964 7561 6c5d 2e6d  de.individual].m
-00017dd0: 6574 6164 6174 612c 2027 6c69 7474 6c65  etadata, 'little
-00017de0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00017df0: 2020 2069 6620 676e 785f 696e 6469 7669     if gnx_indivi
-00017e00: 6475 616c 5f69 6420 696e 205b 2a73 656c  dual_id in [*sel
-00017e10: 665d 3a0a 2020 2020 2020 2020 2020 2020  f]:.            
-00017e20: 2020 2020 2020 2020 6375 7272 5f6e 6f64          curr_nod
-00017e30: 655f 6374 202b 3d20 310a 2020 2020 2020  e_ct += 1.      
-00017e40: 2020 2020 2020 2020 2020 2020 2020 6173                as
-00017e50: 7365 7274 2028 7365 6c66 5b67 6e78 5f69  sert (self[gnx_i
-00017e60: 6e64 6976 6964 7561 6c5f 6964 5d2e 5f69  ndividual_id]._i
-00017e70: 6e64 6976 6964 7561 6c73 5f74 6162 5f69  ndividuals_tab_i
-00017e80: 6420 3d3d 0a20 2020 2020 2020 2020 2020  d ==.           
-00017e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ea0: 206e 6f64 652e 696e 6469 7669 6475 616c   node.individual
-00017eb0: 2061 6e64 206e 6f64 655f 6964 2069 6e0a   and node_id in.
-00017ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ed0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017ee0: 5b67 6e78 5f69 6e64 6976 6964 7561 6c5f  [gnx_individual_
-00017ef0: 6964 5d2e 5f6e 6f64 6573 5f74 6162 5f69  id]._nodes_tab_i
-00017f00: 6473 2e76 616c 7565 7328 2929 0a20 2020  ds.values()).   
-00017f10: 2020 2020 2061 7373 6572 7420 6375 7272       assert curr
-00017f20: 5f6e 6f64 655f 6374 203d 3d20 322a 6c65  _node_ct == 2*le
-00017f30: 6e28 7365 6c66 292c 2028 224e 756d 6265  n(self), ("Numbe
-00017f40: 7220 6f66 2063 7572 7265 6e74 2049 6e64  r of current Ind
-00017f50: 6976 6964 7561 6c73 2022 0a20 2020 2020  ividuals ".     
-00017f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f80: 2020 2020 2020 2020 2020 2269 6e20 7468            "in th
-00017f90: 6520 7265 6369 7069 656e 7420 5370 6563  e recipient Spec
-00017fa0: 6965 7320 646f 6573 206e 6f74 2022 0a20  ies does not ". 
-00017fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fd0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-00017fe0: 6174 6368 2074 6865 206e 756d 6265 7220  atch the number 
-00017ff0: 6578 7065 6374 6564 2062 6173 6564 206f  expected based o
-00018000: 6e20 220a 2020 2020 2020 2020 2020 2020  n ".            
-00018010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018030: 2020 2022 5461 626c 6543 6f6c 6c65 6374     "TableCollect
-00018040: 696f 6e20 636f 6e74 656e 7473 2e22 290a  ion contents.").
-00018050: 0a20 2020 2020 2020 2023 2073 6f72 7420  .        # sort 
-00018060: 616e 6420 7369 6d70 6c69 6679 2074 6865  and simplify the
-00018070: 2074 736b 6974 2e54 6162 6c65 436f 6c6c   tskit.TableColl
-00018080: 6563 7469 6f6e 2061 6761 696e 0a20 2020  ection again.   
-00018090: 2020 2020 2073 656c 662e 5f73 6f72 745f       self._sort_
-000180a0: 616e 645f 7369 6d70 6c69 6679 5f74 6162  and_simplify_tab
-000180b0: 6c65 5f63 6f6c 6c65 6374 696f 6e28 290a  le_collection().
-000180c0: 0a20 2020 2020 2020 2023 2072 6573 6574  .        # reset
-000180d0: 2074 6865 2063 6f6f 7264 7320 616e 6420   the coords and 
-000180e0: 6365 6c6c 7320 6174 7472 730a 2020 2020  cells attrs.    
-000180f0: 2020 2020 7365 6c66 2e5f 7365 745f 636f      self._set_co
-00018100: 6f72 6473 5f61 6e64 5f63 656c 6c73 2829  ords_and_cells()
-00018110: 0a0a 2020 2020 2020 2020 2320 7265 7365  ..        # rese
-00018120: 7420 7468 6520 4b44 5472 6565 2061 6674  t the KDTree aft
-00018130: 6572 2061 6464 696e 6720 7468 6520 6e65  er adding the ne
-00018140: 7720 696e 6469 7669 6475 616c 730a 2020  w individuals.  
-00018150: 2020 2020 2020 7365 6c66 2e5f 7365 745f        self._set_
-00018160: 6b64 5f74 7265 6528 290a 0a20 2020 2020  kd_tree()..     
-00018170: 2020 2023 2072 6573 6574 2074 6865 2064     # reset the d
-00018180: 656e 7369 7479 2067 7269 6473 0a20 2020  ensity grids.   
-00018190: 2020 2020 2073 656c 662e 5f73 6574 5f64       self._set_d
-000181a0: 656e 735f 6772 6964 7328 6c61 6e64 290a  ens_grids(land).
-000181b0: 0a20 2020 2020 2020 2023 2072 6573 6574  .        # reset
-000181c0: 2f73 6574 2073 6f75 7263 6520 496e 6469  /set source Indi
-000181d0: 7669 6475 616c 7327 2065 6e76 6972 6f6e  viduals' environ
-000181e0: 6d65 6e74 616c 2061 6e64 2066 6974 6e65  mental and fitne
-000181f0: 7373 2076 616c 7565 730a 2020 2020 2020  ss values.      
-00018200: 2020 7365 6c66 2e5f 7365 745f 6528 6c61    self._set_e(la
-00018210: 6e64 290a 0a20 2020 2020 2020 2023 7265  nd)..        #re
-00018220: 7365 7420 7068 656e 6f74 7970 6573 2061  set phenotypes a
-00018230: 6e64 2066 6974 6e65 7373 6573 0a20 2020  nd fitnesses.   
-00018240: 2020 2020 2069 6620 7365 6c66 2e67 656e       if self.gen
-00018250: 5f61 7263 6820 6973 206e 6f74 204e 6f6e  _arch is not Non
-00018260: 6520 616e 6420 7365 6c66 2e67 656e 5f61  e and self.gen_a
-00018270: 7263 682e 7472 6169 7473 2069 7320 6e6f  rch.traits is no
-00018280: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00018290: 2020 2020 5b69 6e64 2e5f 7365 745f 7a28      [ind._set_z(
-000182a0: 7365 6c66 2e67 656e 5f61 7263 6829 2066  self.gen_arch) f
-000182b0: 6f72 2069 6e64 2069 6e20 7365 6c66 2e76  or ind in self.v
-000182c0: 616c 7565 7328 295d 0a20 2020 2020 2020  alues()].       
-000182d0: 2020 2020 2073 656c 662e 5f63 616c 635f       self._calc_
-000182e0: 6669 746e 6573 7328 7365 745f 6669 743d  fitness(set_fit=
-000182f0: 5472 7565 290a 0a20 2020 2020 2020 2023  True)..        #
-00018300: 2070 7269 6e74 2069 6e66 6f72 6d61 7469   print informati
-00018310: 7665 206f 7574 7075 740a 2020 2020 2020  ve output.      
-00018320: 2020 7072 696e 7428 6622 5c6e 7b6c 656e    print(f"\n{len
-00018330: 2869 6e64 6976 6964 7329 7d20 496e 6469  (individs)} Indi
-00018340: 7669 6475 616c 7320 7375 6363 6573 7366  viduals successf
-00018350: 756c 6c79 2022 0a20 2020 2020 2020 2020  ully ".         
-00018360: 2020 2020 2066 2261 6464 6564 2074 6f20       f"added to 
-00018370: 5370 6563 6965 7320 7b73 656c 662e 6964  Species {self.id
-00018380: 787d 2028 277b 7365 6c66 2e6e 616d 657d  x} ('{self.name}
-00018390: 2729 2e5c 6e22 290a 0a0a 2020 2020 6465  ').\n")...    de
-000183a0: 6620 5f69 6e69 745f 6d73 7072 696d 655f  f _init_msprime_
-000183b0: 706f 7028 7365 6c66 2c20 6c61 6e64 2c20  pop(self, land, 
-000183c0: 6d73 7072 696d 655f 696e 6974 5f70 6172  msprime_init_par
-000183d0: 616d 7329 3a0a 2020 2020 2020 2020 2320  ams):.        # 
-000183e0: 6765 7420 696e 7465 6e64 6564 2074 6f74  get intended tot
-000183f0: 616c 2069 6e69 7469 616c 2070 6f70 2073  al initial pop s
-00018400: 697a 650a 2020 2020 2020 2020 7461 7267  ize.        targ
-00018410: 6574 5f73 697a 6520 3d20 6e70 2e73 756d  et_size = np.sum
-00018420: 285b 5b2a 762e 6b65 7973 2829 5d5b 305d  ([[*v.keys()][0]
-00018430: 2066 6f72 0a20 2020 2020 2020 2020 2020   for.           
-00018440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018460: 2076 2069 6e20 6d73 7072 696d 655f 696e   v in msprime_in
-00018470: 6974 5f70 6172 616d 732e 7661 6c75 6573  it_params.values
-00018480: 2829 5d29 0a20 2020 2020 2020 2023 2072  ()]).        # r
-00018490: 656d 6f76 6520 616c 6c20 6375 7272 656e  emove all curren
-000184a0: 7420 696e 6469 7669 6473 0a20 2020 2020  t individs.     
-000184b0: 2020 2073 656c 662e 5f72 656d 6f76 655f     self._remove_
-000184c0: 696e 6469 7669 6475 616c 7328 6e3d 6c65  individuals(n=le
-000184d0: 6e28 7365 6c66 292c 0a20 2020 2020 2020  n(self),.       
-000184e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184f0: 2020 2020 2020 2020 2020 6b65 6570 5f73            keep_s
-00018500: 6974 6573 5f74 6162 3d46 616c 7365 2c0a  ites_tab=False,.
-00018510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018530: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-00018540: 206c 656e 2873 656c 6629 203d 3d20 300a   len(self) == 0.
-00018550: 2020 2020 2020 2020 2320 6c6f 6f70 206f          # loop o
-00018560: 7665 7220 736f 7572 6365 2070 6f70 7320  ver source pops 
-00018570: 616e 6420 6164 6420 696e 6469 7669 6475  and add individu
-00018580: 616c 7320 6672 6f6d 2065 6163 6820 6f6e  als from each on
-00018590: 650a 2020 2020 2020 2020 666f 7220 706f  e.        for po
-000185a0: 7020 696e 206d 7370 7269 6d65 5f69 6e69  p in msprime_ini
-000185b0: 745f 7061 7261 6d73 2e76 616c 7565 7328  t_params.values(
-000185c0: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
-000185d0: 7373 6572 7420 6c65 6e28 706f 702e 6b65  ssert len(pop.ke
-000185e0: 7973 2829 2920 3d3d 2031 2c20 2822 4561  ys()) == 1, ("Ea
-000185f0: 6368 206d 7370 7269 6d65 2073 6f75 7263  ch msprime sourc
-00018600: 6520 706f 7075 6c61 7469 6f6e 2022 0a20  e population ". 
-00018610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018620: 2020 2020 2020 2022 7061 7261 6d65 7465         "paramete
-00018630: 7269 7a65 6420 696e 2061 2053 7065 6369  rized in a Speci
-00018640: 6573 2720 2769 6e69 7427 2073 6563 7469  es' 'init' secti
-00018650: 6f6e 2022 0a20 2020 2020 2020 2020 2020  on ".           
-00018660: 2020 2020 2020 2020 2020 2020 2022 6f66               "of
-00018670: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
-00018680: 6669 6c65 220a 2020 2020 2020 2020 2020  file".          
-00018690: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-000186a0: 7573 7420 6265 2072 6570 7265 7365 6e74  ust be represent
-000186b0: 6564 2062 7920 6120 6469 6374 2077 6974  ed by a dict wit
-000186c0: 6820 6120 7369 6e67 6c65 206b 6579 2028  h a single key (
-000186d0: 7468 6520 220a 2020 2020 2020 2020 2020  the ".          
-000186e0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-000186f0: 756d 6265 7220 6f66 2049 6e64 6976 6964  umber of Individ
-00018700: 7561 6c73 2074 6f20 7361 6d70 6c65 2066  uals to sample f
-00018710: 726f 6d20 7468 6520 706f 7075 6c61 7469  rom the populati
-00018720: 6f6e 2920 220a 2020 2020 2020 2020 2020  on) ".          
-00018730: 2020 2020 2020 2020 2020 2020 2020 2277                "w
-00018740: 686f 7365 2076 616c 7565 2069 7320 6120  hose value is a 
-00018750: 6469 6374 2063 6f6e 7461 696e 696e 6720  dict containing 
-00018760: 312e 2920 6120 2763 6f6f 7264 7327 206b  1.) a 'coords' k
-00018770: 6579 2022 0a20 2020 2020 2020 2020 2020  ey ".           
-00018780: 2020 2020 2020 2020 2020 2020 2022 696e               "in
-00018790: 6469 6361 7469 6e67 2074 6865 206c 6f63  dicating the loc
-000187a0: 6174 696f 6e2f 7320 746f 2070 6c61 6365  ation/s to place
-000187b0: 2074 6865 2022 0a20 2020 2020 2020 2020   the ".         
-000187c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000187d0: 7361 6d70 6c65 6420 496e 6469 7669 6475  sampled Individu
-000187e0: 616c 7320 6174 2061 6e64 2032 2e29 2022  als at and 2.) "
-000187f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018800: 2020 2020 2020 2020 2022 6120 7365 7420           "a set 
-00018810: 6f66 2076 616c 6964 206b 6579 776f 7264  of valid keyword
-00018820: 2061 7267 756d 656e 7473 2074 6861 7420   arguments that 
-00018830: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00018840: 2020 2020 2020 2020 2020 2263 616e 2062            "can b
-00018850: 6520 7072 6f76 6964 6564 2074 6f20 4d6f  e provided to Mo
-00018860: 6465 6c2e 6164 645f 696e 6469 7669 6475  del.add_individu
-00018870: 616c 7320 220a 2020 2020 2020 2020 2020  als ".          
-00018880: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-00018890: 7320 7468 6520 2773 6f75 7263 655f 6d73  s the 'source_ms
-000188a0: 7072 696d 655f 7061 7261 6d73 2720 6469  prime_params' di
-000188b0: 6374 2e22 290a 2020 2020 2020 2020 2020  ct.").          
-000188c0: 2020 6e20 3d20 5b2a 706f 702e 6b65 7973    n = [*pop.keys
-000188d0: 2829 5d5b 305d 0a20 2020 2020 2020 2020  ()][0].         
-000188e0: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
-000188f0: 616e 6365 286e 2c20 696e 7429 2c20 2822  ance(n, int), ("
-00018900: 5468 6520 6b65 7920 6f66 2065 6163 6820  The key of each 
-00018910: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00018920: 2020 2020 2020 2020 2020 226d 7370 7269            "mspri
-00018930: 6d65 2073 6f75 7263 6520 706f 7075 6c61  me source popula
-00018940: 7469 6f6e 2069 6e20 6120 5370 6563 6965  tion in a Specie
-00018950: 7327 2027 696e 6974 2720 220a 2020 2020  s' 'init' ".    
+00017070: 2020 2020 6164 645f 706f 7075 6c61 7469      add_populati
+00017080: 6f6e 733d 5472 7565 2c0a 2020 2020 2020  ons=True,.      
+00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170a0: 2020 2020 2020 2320 4e4f 5445 3a20 6265        # NOTE: be
+000170b0: 7374 2074 6f20 6a75 7374 2061 6c6c 6f77  st to just allow
+000170c0: 2069 7420 746f 2064 6f20 7468 6973 2c0a   it to do this,.
+000170d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170e0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+000170f0: 2020 2020 696e 2063 6173 6520 7765 2067      in case we g
+00017100: 656e 6572 616c 697a 6520 7468 696e 6773  eneralize things
+00017110: 206c 6174 6572 206f 6e2c 0a20 2020 2020   later on,.     
+00017120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017130: 2020 2020 2020 2023 2020 2020 2020 2062         #       b
+00017140: 7574 2066 6f72 206e 6f77 2074 6865 7265  ut for now there
+00017150: 2077 696c 6c20 6163 7475 616c 6c79 2062   will actually b
+00017160: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00017170: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00017180: 2020 2020 2020 6e6f 7468 696e 6720 746f        nothing to
+00017190: 2063 6865 636b 2062 6563 6175 7365 2077   check because w
+000171a0: 6520 6173 7375 6d65 200a 2020 2020 2020  e assume .      
+000171b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171c0: 2020 2020 2020 2320 2020 2020 2020 6e6f        #       no
+000171d0: 2073 6861 7265 6420 6e6f 6465 7320 6265   shared nodes be
+000171e0: 7477 6565 6e0a 2020 2020 2020 2020 2020  tween.          
+000171f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017200: 2020 2320 2020 2020 2020 736f 7572 6365    #       source
+00017210: 2061 6e64 2072 6563 6970 6965 6e74 2054   and recipient T
+00017220: 6162 6c65 436f 6c6c 6563 7469 6f6e 730a  ableCollections.
+00017230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017240: 2020 2020 2020 2020 2020 2020 2320 544f              # TO
+00017250: 444f 3a20 484f 5745 5645 522c 2045 5155  DO: HOWEVER, EQU
+00017260: 414c 4954 5920 4348 4543 4b20 5354 494c  ALITY CHECK STIL
+00017270: 4c20 4641 494c 5321 2057 4859 3f0a 2020  L FAILS! WHY?.  
+00017280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017290: 2020 2020 2020 2020 2020 6368 6563 6b5f            check_
+000172a0: 7368 6172 6564 5f65 7175 616c 6974 793d  shared_equality=
+000172b0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+000172c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172d0: 2020 2023 204e 4f54 453a 2073 686f 756c     # NOTE: shoul
+000172e0: 6420 636f 7079 2070 726f 7665 6e61 6e63  d copy provenanc
+000172f0: 6520 696e 666f 206f 7665 720a 2020 2020  e info over.    
+00017300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017310: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00017320: 6672 6f6d 2074 6865 2073 6f75 7263 6520  from the source 
+00017330: 496e 6469 7669 6475 616c 7327 2054 6162  Individuals' Tab
+00017340: 6c65 436f 6c6c 6563 7469 6f6e 0a20 2020  leCollection.   
+00017350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017360: 2020 2020 2020 2020 2023 2020 2020 2020           #      
+00017370: 2074 6f20 7468 6174 206f 6620 7468 6520   to that of the 
+00017380: 7265 6365 6970 6965 6e74 2053 7065 6369  receipient Speci
+00017390: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+000173a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000173b0: 6563 6f72 645f 7072 6f76 656e 616e 6365  ecord_provenance
+000173c0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+000173d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000173f0: 2020 6e6f 6465 735f 7461 625f 6c65 6e5f    nodes_tab_len_
+00017400: 6166 203d 2073 656c 662e 5f74 632e 6e6f  af = self._tc.no
+00017410: 6465 732e 6e75 6d5f 726f 7773 0a20 2020  des.num_rows.   
+00017420: 2020 2020 2069 6e64 6976 6964 735f 7461       individs_ta
+00017430: 625f 6c65 6e5f 6166 203d 2073 656c 662e  b_len_af = self.
+00017440: 5f74 632e 696e 6469 7669 6475 616c 732e  _tc.individuals.
+00017450: 6e75 6d5f 726f 7773 0a0a 2020 2020 2020  num_rows..      
+00017460: 2020 2320 6368 6563 6b20 756e 696f 6e65    # check unione
+00017470: 6420 7461 626c 6573 2068 6176 6520 636f  d tables have co
+00017480: 7272 6563 7420 6c65 6e67 7468 730a 2020  rrect lengths.  
+00017490: 2020 2020 2020 6173 7365 7274 2028 6e6f        assert (no
+000174a0: 6465 735f 7461 625f 6c65 6e5f 6166 202d  des_tab_len_af -
+000174b0: 206e 6f64 6573 5f74 6162 5f6c 656e 5f62   nodes_tab_len_b
+000174c0: 3429 203d 3d20 736f 7572 6365 5f74 632e  4) == source_tc.
+000174d0: 6e6f 6465 732e 6e75 6d5f 726f 7773 0a20  nodes.num_rows. 
+000174e0: 2020 2020 2020 2061 7373 6572 7420 2828         assert ((
+000174f0: 696e 6469 7669 6473 5f74 6162 5f6c 656e  individs_tab_len
+00017500: 5f61 6620 2d20 696e 6469 7669 6473 5f74  _af - individs_t
+00017510: 6162 5f6c 656e 5f62 3429 203d 3d0a 2020  ab_len_b4) ==.  
+00017520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017540: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00017550: 7572 6365 5f74 632e 696e 6469 7669 6475  urce_tc.individu
+00017560: 616c 732e 6e75 6d5f 726f 7773 290a 0a20  als.num_rows).. 
+00017570: 2020 2020 2020 2023 2063 6865 636b 2074         # check t
+00017580: 6861 7420 616c 6c20 676e 7820 6964 7873  hat all gnx idxs
+00017590: 2073 746f 7265 6420 696e 2074 6865 2069   stored in the i
+000175a0: 6e64 6976 6964 7561 6c73 2074 6162 6c65  ndividuals table
+000175b0: 2773 0a20 2020 2020 2020 2023 206d 6574  's.        # met
+000175c0: 6164 6174 6120 636f 6c75 6d6e 206f 6363  adata column occ
+000175d0: 7572 206f 6e6c 7920 6f6e 6365 2028 6173  ur only once (as
+000175e0: 6964 6520 6672 6f6d 2030 2c0a 2020 2020  ide from 0,.    
+000175f0: 2020 2020 2320 7768 6963 6820 6973 2061      # which is a
+00017600: 206e 756c 6c20 7661 6c75 6520 666f 7220   null value for 
+00017610: 696e 6469 7669 6475 616c 7320 7468 6174  individuals that
+00017620: 0a20 2020 2020 2020 2023 206e 6576 6572  .        # never
+00017630: 2065 7869 7374 6564 2061 7320 2772 6561   existed as 'rea
+00017640: 6c27 2067 6e78 2049 6e64 6976 6964 7561  l' gnx Individua
+00017650: 6c20 6f62 6a65 6374 7320 6265 6361 7573  l objects becaus
+00017660: 650a 2020 2020 2020 2020 2320 7468 6579  e.        # they
+00017670: 2077 6572 6520 696e 2074 6865 2070 6173   were in the pas
+00017680: 7420 6f66 2061 2063 6f61 6c65 7363 656e  t of a coalescen
+00017690: 7420 7369 6d75 6c61 7469 6f6e 290a 2020  t simulation).  
+000176a0: 2020 2020 2020 7265 6369 705f 7463 5f69        recip_tc_i
+000176b0: 6e64 6976 6964 7561 6c73 5f69 6473 203d  ndividuals_ids =
+000176c0: 205b 696e 742e 6672 6f6d 5f62 7974 6573   [int.from_bytes
+000176d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000176e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000176f0: 6c66 2e5f 7463 2e69 6e64 6976 6964 7561  lf._tc.individua
+00017700: 6c73 5b69 5d2e 6d65 7461 6461 7461 2c20  ls[i].metadata, 
+00017710: 276c 6974 746c 6527 2920 666f 720a 2020  'little') for.  
+00017720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017730: 2020 2020 2020 2020 2020 2020 2020 6920                i 
+00017740: 696e 2072 616e 6765 2873 656c 662e 5f74  in range(self._t
+00017750: 632e 696e 6469 7669 6475 616c 732e 6e75  c.individuals.nu
+00017760: 6d5f 726f 7773 295d 0a20 2020 2020 2020  m_rows)].       
+00017770: 2061 7373 6572 7420 286c 656e 2872 6563   assert (len(rec
+00017780: 6970 5f74 635f 696e 6469 7669 6475 616c  ip_tc_individual
+00017790: 735f 6964 7329 203d 3d0a 2020 2020 2020  s_ids) ==.      
+000177a0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000177b0: 7463 2e69 6e64 6976 6964 7561 6c73 2e6e  tc.individuals.n
+000177c0: 756d 5f72 6f77 7329 0a20 2020 2020 2020  um_rows).       
+000177d0: 2063 6f75 6e74 7320 3d20 4328 7265 6369   counts = C(reci
+000177e0: 705f 7463 5f69 6e64 6976 6964 7561 6c73  p_tc_individuals
+000177f0: 5f69 6473 290a 2020 2020 2020 2020 666f  _ids).        fo
+00017800: 7220 6b2c 2076 2069 6e20 636f 756e 7473  r k, v in counts
+00017810: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00017820: 2020 2020 2020 6966 206b 2021 3d20 303a        if k != 0:
+00017830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017840: 2061 7373 6572 7420 7620 3d3d 2031 2c20   assert v == 1, 
+00017850: 2866 2267 6e78 2049 6e64 6976 6964 7561  (f"gnx Individua
+00017860: 6c20 6964 7820 7b69 7d20 6f63 6375 7273  l idx {i} occurs
+00017870: 206d 6f72 6520 7468 616e 206f 6e63 6520   more than once 
+00017880: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00017890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178a0: 2020 2022 696e 2074 6865 206d 6574 6164     "in the metad
+000178b0: 6174 6120 636f 6c75 6d6e 206f 6620 7468  ata column of th
+000178c0: 6520 756e 696f 6e20 6f66 2022 0a20 2020  e union of ".   
+000178d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178e0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+000178f0: 6865 2072 6563 6970 6965 6e74 2061 6e64  he recipient and
+00017900: 2073 6f75 7263 6520 5370 6563 6965 7327   source Species'
+00017910: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00017920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017930: 2020 2020 2254 6162 6c65 436f 6c6c 6563      "TableCollec
+00017940: 7469 6f6e 7320 696e 6469 7669 6475 616c  tions individual
+00017950: 7320 7461 626c 6573 2e22 290a 0a20 2020  s tables.")..   
+00017960: 2020 2020 2023 2061 6464 2069 6e20 7468       # add in th
+00017970: 6520 496e 6469 7669 6475 616c 732c 206b  e Individuals, k
+00017980: 6579 6564 2062 7920 6964 780a 2020 2020  eyed by idx.    
+00017990: 2020 2020 706f 705f 7369 7a65 5f62 3420      pop_size_b4 
+000179a0: 3d20 6c65 6e28 7365 6c66 290a 2020 2020  = len(self).    
+000179b0: 2020 2020 666f 7220 696e 6420 696e 2069      for ind in i
+000179c0: 6e64 6976 6964 733a 0a20 2020 2020 2020  ndivids:.       
+000179d0: 2020 2020 2073 656c 665b 696e 642e 6964       self[ind.id
+000179e0: 785d 203d 2069 6e64 0a20 2020 2020 2020  x] = ind.       
+000179f0: 2070 6f70 5f73 697a 655f 6166 203d 206c   pop_size_af = l
+00017a00: 656e 2873 656c 6629 0a20 2020 2020 2020  en(self).       
+00017a10: 2061 7373 6572 7420 2870 6f70 5f73 697a   assert (pop_siz
+00017a20: 655f 6166 202d 2070 6f70 5f73 697a 655f  e_af - pop_size_
+00017a30: 6234 2920 3d3d 206c 656e 2869 6e64 6976  b4) == len(indiv
+00017a40: 6964 7329 2c20 2822 496e 636f 7272 6563  ids), ("Incorrec
+00017a50: 7420 6e75 6d62 6572 220a 2020 2020 2020  t number".      
+00017a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a70: 2020 2020 2020 2020 2020 2220 6f66 2049            " of I
+00017a80: 6e64 6976 6964 7561 6c73 2061 6464 6564  ndividuals added
+00017a90: 2074 6f20 7265 6369 7069 656e 7420 5370   to recipient Sp
+00017aa0: 6563 6965 732e 2229 0a0a 2020 2020 2020  ecies.")..      
+00017ab0: 2020 2320 7570 6461 7465 2065 6163 6820    # update each 
+00017ac0: 496e 6469 7669 6475 616c 2773 205f 696e  Individual's _in
+00017ad0: 6469 7669 6475 616c 735f 7461 625f 6964  dividuals_tab_id
+00017ae0: 2061 6e64 205f 6e6f 6465 735f 7461 625f   and _nodes_tab_
+00017af0: 6964 730a 2020 2020 2020 2020 2320 746f  ids.        # to
+00017b00: 206d 6174 6368 2074 6865 206e 6577 2c20   match the new, 
+00017b10: 756e 696f 6e65 6420 5461 626c 6543 6f6c  unioned TableCol
+00017b20: 6c65 6374 696f 6e0a 2020 2020 2020 2020  lection.        
+00017b30: 6e6f 6465 735f 7461 625f 696e 6469 7669  nodes_tab_indivi
+00017b40: 6475 616c 7320 3d20 7365 6c66 2e5f 7463  duals = self._tc
+00017b50: 2e6e 6f64 6573 2e69 6e64 6976 6964 7561  .nodes.individua
+00017b60: 6c0a 2020 2020 2020 2020 666f 7220 6964  l.        for id
+00017b70: 782c 2069 6e64 2069 6e20 7365 6c66 2e69  x, ind in self.i
+00017b80: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+00017b90: 2020 2020 696e 6469 7669 6475 616c 735f      individuals_
+00017ba0: 7461 625f 6964 203d 206e 702e 6172 6777  tab_id = np.argw
+00017bb0: 6865 7265 280a 2020 2020 2020 2020 2020  here(.          
+00017bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bd0: 2020 6e70 2e61 7272 6179 2872 6563 6970    np.array(recip
+00017be0: 5f74 635f 696e 6469 7669 6475 616c 735f  _tc_individuals_
+00017bf0: 6964 7329 203d 3d20 6964 7829 2e72 6176  ids) == idx).rav
+00017c00: 656c 2829 0a20 2020 2020 2020 2020 2020  el().           
+00017c10: 2061 7373 6572 7420 6c65 6e28 696e 6469   assert len(indi
+00017c20: 7669 6475 616c 735f 7461 625f 6964 2920  viduals_tab_id) 
+00017c30: 3d3d 2031 0a20 2020 2020 2020 2020 2020  == 1.           
+00017c40: 2069 6e64 6976 6964 7561 6c73 5f74 6162   individuals_tab
+00017c50: 5f69 6420 3d20 696e 6469 7669 6475 616c  _id = individual
+00017c60: 735f 7461 625f 6964 5b30 5d0a 2020 2020  s_tab_id[0].    
+00017c70: 2020 2020 2020 2020 696e 642e 5f69 6e64          ind._ind
+00017c80: 6976 6964 7561 6c73 5f74 6162 5f69 6420  ividuals_tab_id 
+00017c90: 3d20 696e 6469 7669 6475 616c 735f 7461  = individuals_ta
+00017ca0: 625f 6964 0a20 2020 2020 2020 2020 2020  b_id.           
+00017cb0: 206e 6f64 6573 5f74 6162 5f69 6473 203d   nodes_tab_ids =
+00017cc0: 206e 702e 6172 6777 6865 7265 286e 6f64   np.argwhere(nod
+00017cd0: 6573 5f74 6162 5f69 6e64 6976 6964 7561  es_tab_individua
+00017ce0: 6c73 203d 3d0a 2020 2020 2020 2020 2020  ls ==.          
+00017cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d00: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00017d10: 6469 7669 6475 616c 735f 7461 625f 6964  dividuals_tab_id
+00017d20: 292e 7261 7665 6c28 290a 2020 2020 2020  ).ravel().      
+00017d30: 2020 2020 2020 6173 7365 7274 206c 656e        assert len
+00017d40: 286e 6f64 6573 5f74 6162 5f69 6473 2920  (nodes_tab_ids) 
+00017d50: 3d3d 2032 0a20 2020 2020 2020 2020 2020  == 2.           
+00017d60: 2069 6e64 2e5f 6e6f 6465 735f 7461 625f   ind._nodes_tab_
+00017d70: 6964 7320 3d20 7b69 3a20 6964 2066 6f72  ids = {i: id for
+00017d80: 2069 2c20 6964 2069 6e20 656e 756d 6572   i, id in enumer
+00017d90: 6174 6528 6e6f 6465 735f 7461 625f 6964  ate(nodes_tab_id
+00017da0: 7329 7d0a 0a20 2020 2020 2020 2023 2066  s)}..        # f
+00017db0: 696e 616c 2063 6865 636b 2074 6861 7420  inal check that 
+00017dc0: 696e 6469 6365 7320 6368 6563 6b20 6f75  indices check ou
+00017dd0: 7420 696e 2074 6865 206f 7468 6572 2064  t in the other d
+00017de0: 6972 6563 7469 6f6e 0a20 2020 2020 2020  irection.       
+00017df0: 2023 2028 692e 652e 2c20 6672 6f6d 206e   # (i.e., from n
+00017e00: 6f64 6573 2074 6162 2074 6f20 696e 6469  odes tab to indi
+00017e10: 7669 6475 616c 7320 7461 6220 746f 2067  viduals tab to g
+00017e20: 6e78 2049 6e64 6976 6964 7561 6c73 0a20  nx Individuals. 
+00017e30: 2020 2020 2020 2023 2061 6e64 2074 6861         # and tha
+00017e40: 7420 6e6f 6465 7320 6964 7320 6368 6563  t nodes ids chec
+00017e50: 6b20 6f75 7420 746f 6f0a 2020 2020 2020  k out too.      
+00017e60: 2020 6375 7272 5f6e 6f64 655f 6374 203d    curr_node_ct =
+00017e70: 2030 0a20 2020 2020 2020 2066 6f72 206e   0.        for n
+00017e80: 6f64 655f 6964 2c20 6e6f 6465 2069 6e20  ode_id, node in 
+00017e90: 656e 756d 6572 6174 6528 7365 6c66 2e5f  enumerate(self._
+00017ea0: 7463 2e6e 6f64 6573 293a 0a20 2020 2020  tc.nodes):.     
+00017eb0: 2020 2020 2020 2023 204e 4f54 453a 2069         # NOTE: i
+00017ec0: 676e 6f72 6520 2d31 733b 2074 6865 7920  gnore -1s; they 
+00017ed0: 6172 6520 6d73 7072 696d 6520 666c 6167  are msprime flag
+00017ee0: 7320 666f 7220 6e6f 6e2d 7361 6d70 6c65  s for non-sample
+00017ef0: 206e 6f64 6573 2062 7574 0a20 2020 2020   nodes but.     
+00017f00: 2020 2020 2020 2023 2020 2020 2020 2062         #       b
+00017f10: 6561 6876 6520 6173 2061 2050 7974 686f  eahve as a Pytho
+00017f20: 6e20 696e 6465 7865 7220 6f66 2074 6865  n indexer of the
+00017f30: 206c 6173 7420 496e 6469 7669 6475 616c   last Individual
+00017f40: 2069 6e20 7468 650a 2020 2020 2020 2020   in the.        
+00017f50: 2020 2020 2320 2020 2020 2020 5370 6563      #       Spec
+00017f60: 6965 7320 616e 6420 7468 7573 2074 6872  ies and thus thr
+00017f70: 6f77 2061 6e20 6572 726f 720a 2020 2020  ow an error.    
+00017f80: 2020 2020 2020 2020 6966 206e 6f64 652e          if node.
+00017f90: 696e 6469 7669 6475 616c 2021 3d20 2d31  individual != -1
+00017fa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017fb0: 2020 676e 785f 696e 6469 7669 6475 616c    gnx_individual
+00017fc0: 5f69 6420 3d20 696e 742e 6672 6f6d 5f62  _id = int.from_b
+00017fd0: 7974 6573 2873 656c 662e 5f74 632e 696e  ytes(self._tc.in
+00017fe0: 6469 7669 6475 616c 735b 0a20 2020 2020  dividuals[.     
+00017ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018010: 2020 2020 2020 206e 6f64 652e 696e 6469         node.indi
+00018020: 7669 6475 616c 5d2e 6d65 7461 6461 7461  vidual].metadata
+00018030: 2c20 276c 6974 746c 6527 290a 2020 2020  , 'little').    
+00018040: 2020 2020 2020 2020 2020 2020 6966 2067              if g
+00018050: 6e78 5f69 6e64 6976 6964 7561 6c5f 6964  nx_individual_id
+00018060: 2069 6e20 5b2a 7365 6c66 5d3a 0a20 2020   in [*self]:.   
+00018070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018080: 2063 7572 725f 6e6f 6465 5f63 7420 2b3d   curr_node_ct +=
+00018090: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
+000180a0: 2020 2020 2020 2061 7373 6572 7420 2873         assert (s
+000180b0: 656c 665b 676e 785f 696e 6469 7669 6475  elf[gnx_individu
+000180c0: 616c 5f69 645d 2e5f 696e 6469 7669 6475  al_id]._individu
+000180d0: 616c 735f 7461 625f 6964 203d 3d0a 2020  als_tab_id ==.  
+000180e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180f0: 2020 2020 2020 2020 2020 6e6f 6465 2e69            node.i
+00018100: 6e64 6976 6964 7561 6c20 616e 6420 6e6f  ndividual and no
+00018110: 6465 5f69 6420 696e 0a20 2020 2020 2020  de_id in.       
+00018120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018130: 2020 2020 2073 656c 665b 676e 785f 696e       self[gnx_in
+00018140: 6469 7669 6475 616c 5f69 645d 2e5f 6e6f  dividual_id]._no
+00018150: 6465 735f 7461 625f 6964 732e 7661 6c75  des_tab_ids.valu
+00018160: 6573 2829 290a 2020 2020 2020 2020 6173  es()).        as
+00018170: 7365 7274 2063 7572 725f 6e6f 6465 5f63  sert curr_node_c
+00018180: 7420 3d3d 2032 2a6c 656e 2873 656c 6629  t == 2*len(self)
+00018190: 2c20 2822 4e75 6d62 6572 206f 6620 6375  , ("Number of cu
+000181a0: 7272 656e 7420 496e 6469 7669 6475 616c  rrent Individual
+000181b0: 7320 220a 2020 2020 2020 2020 2020 2020  s ".            
+000181c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181e0: 2020 2022 696e 2074 6865 2072 6563 6970     "in the recip
+000181f0: 6965 6e74 2053 7065 6369 6573 2064 6f65  ient Species doe
+00018200: 7320 6e6f 7420 220a 2020 2020 2020 2020  s not ".        
+00018210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018230: 2020 2020 2020 2022 6d61 7463 6820 7468         "match th
+00018240: 6520 6e75 6d62 6572 2065 7870 6563 7465  e number expecte
+00018250: 6420 6261 7365 6420 6f6e 2022 0a20 2020  d based on ".   
+00018260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018280: 2020 2020 2020 2020 2020 2020 2254 6162              "Tab
+00018290: 6c65 436f 6c6c 6563 7469 6f6e 2063 6f6e  leCollection con
+000182a0: 7465 6e74 732e 2229 0a0a 2020 2020 2020  tents.")..      
+000182b0: 2020 2320 736f 7274 2061 6e64 2073 696d    # sort and sim
+000182c0: 706c 6966 7920 7468 6520 7473 6b69 742e  plify the tskit.
+000182d0: 5461 626c 6543 6f6c 6c65 6374 696f 6e20  TableCollection 
+000182e0: 6167 6169 6e0a 2020 2020 2020 2020 7365  again.        se
+000182f0: 6c66 2e5f 736f 7274 5f61 6e64 5f73 696d  lf._sort_and_sim
+00018300: 706c 6966 795f 7461 626c 655f 636f 6c6c  plify_table_coll
+00018310: 6563 7469 6f6e 2829 0a0a 2020 2020 2020  ection()..      
+00018320: 2020 2320 7265 7365 7420 7468 6520 636f    # reset the co
+00018330: 6f72 6473 2061 6e64 2063 656c 6c73 2061  ords and cells a
+00018340: 7474 7273 0a20 2020 2020 2020 2073 656c  ttrs.        sel
+00018350: 662e 5f73 6574 5f63 6f6f 7264 735f 616e  f._set_coords_an
+00018360: 645f 6365 6c6c 7328 290a 0a20 2020 2020  d_cells()..     
+00018370: 2020 2023 2072 6573 6574 2074 6865 204b     # reset the K
+00018380: 4454 7265 6520 6166 7465 7220 6164 6469  DTree after addi
+00018390: 6e67 2074 6865 206e 6577 2069 6e64 6976  ng the new indiv
+000183a0: 6964 7561 6c73 0a20 2020 2020 2020 2073  iduals.        s
+000183b0: 656c 662e 5f73 6574 5f6b 645f 7472 6565  elf._set_kd_tree
+000183c0: 2829 0a0a 2020 2020 2020 2020 2320 7265  ()..        # re
+000183d0: 7365 7420 7468 6520 6465 6e73 6974 7920  set the density 
+000183e0: 6772 6964 730a 2020 2020 2020 2020 7365  grids.        se
+000183f0: 6c66 2e5f 7365 745f 6465 6e73 5f67 7269  lf._set_dens_gri
+00018400: 6473 286c 616e 6429 0a0a 2020 2020 2020  ds(land)..      
+00018410: 2020 2320 7265 7365 742f 7365 7420 736f    # reset/set so
+00018420: 7572 6365 2049 6e64 6976 6964 7561 6c73  urce Individuals
+00018430: 2720 656e 7669 726f 6e6d 656e 7461 6c20  ' environmental 
+00018440: 616e 6420 6669 746e 6573 7320 7661 6c75  and fitness valu
+00018450: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
+00018460: 5f73 6574 5f65 286c 616e 6429 0a0a 2020  _set_e(land)..  
+00018470: 2020 2020 2020 2372 6573 6574 2070 6865        #reset phe
+00018480: 6e6f 7479 7065 7320 616e 6420 6669 746e  notypes and fitn
+00018490: 6573 7365 730a 2020 2020 2020 2020 6966  esses.        if
+000184a0: 2073 656c 662e 6765 6e5f 6172 6368 2069   self.gen_arch i
+000184b0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2073  s not None and s
+000184c0: 656c 662e 6765 6e5f 6172 6368 2e74 7261  elf.gen_arch.tra
+000184d0: 6974 7320 6973 206e 6f74 204e 6f6e 653a  its is not None:
+000184e0: 0a20 2020 2020 2020 2020 2020 205b 696e  .            [in
+000184f0: 642e 5f73 6574 5f7a 2873 656c 662e 6765  d._set_z(self.ge
+00018500: 6e5f 6172 6368 2920 666f 7220 696e 6420  n_arch) for ind 
+00018510: 696e 2073 656c 662e 7661 6c75 6573 2829  in self.values()
+00018520: 5d0a 2020 2020 2020 2020 2020 2020 7365  ].            se
+00018530: 6c66 2e5f 6361 6c63 5f66 6974 6e65 7373  lf._calc_fitness
+00018540: 2873 6574 5f66 6974 3d54 7275 6529 0a0a  (set_fit=True)..
+00018550: 2020 2020 2020 2020 2320 7072 696e 7420          # print 
+00018560: 696e 666f 726d 6174 6976 6520 6f75 7470  informative outp
+00018570: 7574 0a20 2020 2020 2020 2070 7269 6e74  ut.        print
+00018580: 2866 225c 6e7b 6c65 6e28 696e 6469 7669  (f"\n{len(indivi
+00018590: 6473 297d 2049 6e64 6976 6964 7561 6c73  ds)} Individuals
+000185a0: 2073 7563 6365 7373 6675 6c6c 7920 220a   successfully ".
+000185b0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+000185c0: 6164 6465 6420 746f 2053 7065 6369 6573  added to Species
+000185d0: 207b 7365 6c66 2e69 6478 7d20 2827 7b73   {self.idx} ('{s
+000185e0: 656c 662e 6e61 6d65 7d27 292e 5c6e 2229  elf.name}').\n")
+000185f0: 0a0a 0a20 2020 2064 6566 205f 696e 6974  ...    def _init
+00018600: 5f6d 7370 7269 6d65 5f70 6f70 2873 656c  _msprime_pop(sel
+00018610: 662c 206c 616e 642c 206d 7370 7269 6d65  f, land, msprime
+00018620: 5f69 6e69 745f 7061 7261 6d73 293a 0a20  _init_params):. 
+00018630: 2020 2020 2020 2023 2067 6574 2069 6e74         # get int
+00018640: 656e 6465 6420 746f 7461 6c20 696e 6974  ended total init
+00018650: 6961 6c20 706f 7020 7369 7a65 0a20 2020  ial pop size.   
+00018660: 2020 2020 2074 6172 6765 745f 7369 7a65       target_size
+00018670: 203d 206e 702e 7375 6d28 5b5b 2a76 2e6b   = np.sum([[*v.k
+00018680: 6579 7328 295d 5b30 5d20 666f 720a 2020  eys()][0] for.  
+00018690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186b0: 2020 2020 2020 2020 2020 7620 696e 206d            v in m
+000186c0: 7370 7269 6d65 5f69 6e69 745f 7061 7261  sprime_init_para
+000186d0: 6d73 2e76 616c 7565 7328 295d 290a 2020  ms.values()]).  
+000186e0: 2020 2020 2020 2320 7265 6d6f 7665 2061        # remove a
+000186f0: 6c6c 2063 7572 7265 6e74 2069 6e64 6976  ll current indiv
+00018700: 6964 730a 2020 2020 2020 2020 7365 6c66  ids.        self
+00018710: 2e5f 7265 6d6f 7665 5f69 6e64 6976 6964  ._remove_individ
+00018720: 7561 6c73 286e 3d6c 656e 2873 656c 6629  uals(n=len(self)
+00018730: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00018740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018750: 2020 206b 6565 705f 7369 7465 735f 7461     keep_sites_ta
+00018760: 623d 4661 6c73 652c 0a20 2020 2020 2020  b=False,.       
+00018770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018780: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
+00018790: 653d 5472 7565 2c0a 2020 2020 2020 2020  e=True,.        
+000187a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000187c0: 2020 6173 7365 7274 206c 656e 2873 656c    assert len(sel
+000187d0: 6629 203d 3d20 300a 2020 2020 2020 2020  f) == 0.        
+000187e0: 2320 6c6f 6f70 206f 7665 7220 736f 7572  # loop over sour
+000187f0: 6365 2070 6f70 7320 616e 6420 6164 6420  ce pops and add 
+00018800: 696e 6469 7669 6475 616c 7320 6672 6f6d  individuals from
+00018810: 2065 6163 6820 6f6e 650a 2020 2020 2020   each one.      
+00018820: 2020 666f 7220 706f 7020 696e 206d 7370    for pop in msp
+00018830: 7269 6d65 5f69 6e69 745f 7061 7261 6d73  rime_init_params
+00018840: 2e76 616c 7565 7328 293a 0a20 2020 2020  .values():.     
+00018850: 2020 2020 2020 2061 7373 6572 7420 6c65         assert le
+00018860: 6e28 706f 702e 6b65 7973 2829 2920 3d3d  n(pop.keys()) ==
+00018870: 2031 2c20 2822 4561 6368 206d 7370 7269   1, ("Each mspri
+00018880: 6d65 2073 6f75 7263 6520 706f 7075 6c61  me source popula
+00018890: 7469 6f6e 2022 0a20 2020 2020 2020 2020  tion ".         
+000188a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000188b0: 7061 7261 6d65 7465 7269 7a65 6420 696e  parameterized in
+000188c0: 2061 2053 7065 6369 6573 2720 2769 6e69   a Species' 'ini
+000188d0: 7427 2073 6563 7469 6f6e 2022 0a20 2020  t' section ".   
+000188e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188f0: 2020 2020 2022 6f66 2074 6865 2070 6172       "of the par
+00018900: 616d 6574 6572 7320 6669 6c65 220a 2020  ameters file".  
+00018910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018920: 2020 2020 2020 226d 7573 7420 6265 2072        "must be r
+00018930: 6570 7265 7365 6e74 6564 2062 7920 6120  epresented by a 
+00018940: 6469 6374 2077 6974 6820 6120 7369 6e67  dict with a sing
+00018950: 6c65 206b 6579 2028 7468 6520 220a 2020  le key (the ".  
 00018960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018970: 2020 2020 2273 6563 7469 6f6e 206f 6620      "section of 
-00018980: 7468 6520 7061 7261 6d65 7465 7273 2066  the parameters f
-00018990: 696c 6520 6d75 7374 2062 6520 616e 2069  ile must be an i
-000189a0: 6e74 2022 0a20 2020 2020 2020 2020 2020  nt ".           
-000189b0: 2020 2020 2020 2020 2020 2020 2022 696e               "in
-000189c0: 6469 6361 7469 6e67 2074 6865 206e 756d  dicating the num
-000189d0: 6265 7220 6f66 2073 7461 7274 696e 6720  ber of starting 
-000189e0: 496e 6469 7669 6475 616c 7320 220a 2020  Individuals ".  
-000189f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a00: 2020 2020 2020 2274 6f20 6265 2073 6f75        "to be sou
-00018a10: 7263 6564 2066 726f 6d20 7468 6174 2070  rced from that p
-00018a20: 6f70 756c 6174 696f 6e2e 2229 0a20 2020  opulation.").   
-00018a30: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00018a40: 2763 6f6f 7264 7327 2069 6e20 706f 705b  'coords' in pop[
-00018a50: 6e5d 2c20 2822 4561 6368 206d 7370 7269  n], ("Each mspri
-00018a60: 6d65 2073 6f75 7263 6520 706f 7075 6c61  me source popula
-00018a70: 7469 6f6e 2773 2022 0a20 2020 2020 2020  tion's ".       
+00018970: 2020 2020 2020 226e 756d 6265 7220 6f66        "number of
+00018980: 2049 6e64 6976 6964 7561 6c73 2074 6f20   Individuals to 
+00018990: 7361 6d70 6c65 2066 726f 6d20 7468 6520  sample from the 
+000189a0: 706f 7075 6c61 7469 6f6e 2920 220a 2020  population) ".  
+000189b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189c0: 2020 2020 2020 2277 686f 7365 2076 616c        "whose val
+000189d0: 7565 2069 7320 6120 6469 6374 2063 6f6e  ue is a dict con
+000189e0: 7461 696e 696e 6720 312e 2920 6120 2763  taining 1.) a 'c
+000189f0: 6f6f 7264 7327 206b 6579 2022 0a20 2020  oords' key ".   
+00018a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a10: 2020 2020 2022 696e 6469 6361 7469 6e67       "indicating
+00018a20: 2074 6865 206c 6f63 6174 696f 6e2f 7320   the location/s 
+00018a30: 746f 2070 6c61 6365 2074 6865 2022 0a20  to place the ". 
+00018a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a50: 2020 2020 2020 2022 7361 6d70 6c65 6420         "sampled 
+00018a60: 496e 6469 7669 6475 616c 7320 6174 2061  Individuals at a
+00018a70: 6e64 2032 2e29 2022 0a20 2020 2020 2020  nd 2.) ".       
 00018a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018aa0: 2022 696e 6974 2070 6172 616d 6574 6572   "init parameter
-00018ab0: 7320 6469 6374 206d 7573 7420 696e 636c  s dict must incl
-00018ac0: 7564 6520 220a 2020 2020 2020 2020 2020  ude ".          
-00018ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ae0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-00018af0: 2027 636f 6f72 6473 2720 6b65 7920 7768   'coords' key wh
-00018b00: 6f73 6520 7661 6c75 6520 696e 6469 6361  ose value indica
-00018b10: 7465 7320 220a 2020 2020 2020 2020 2020  tes ".          
-00018b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b30: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00018b40: 6865 206c 6f63 6174 696f 6e2f 7320 7768  he location/s wh
-00018b50: 6572 6520 616c 6c20 7361 6d70 6c65 6420  ere all sampled 
-00018b60: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00018b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b80: 2020 2020 2020 2020 2020 2249 6e64 6976            "Indiv
-00018b90: 6964 7561 6c73 2073 686f 756c 6420 6265  iduals should be
-00018ba0: 2070 6c61 6365 642e 2229 0a20 2020 2020   placed.").     
-00018bb0: 2020 2020 2020 2063 6f6f 7264 7320 3d20         coords = 
-00018bc0: 706f 705b 6e5d 2e70 6f70 2827 636f 6f72  pop[n].pop('coor
-00018bd0: 6473 2729 0a20 2020 2020 2020 2020 2020  ds').           
-00018be0: 2061 7373 6572 7420 2869 7369 6e73 7461   assert (isinsta
-00018bf0: 6e63 6528 636f 6f72 6473 2c20 6c69 7374  nce(coords, list
-00018c00: 2920 6f72 0a20 2020 2020 2020 2020 2020  ) or.           
-00018c10: 2020 2020 2020 2020 2069 7369 6e73 7461           isinsta
-00018c20: 6e63 6528 636f 6f72 6473 2c20 7475 706c  nce(coords, tupl
-00018c30: 6529 206f 720a 2020 2020 2020 2020 2020  e) or.          
-00018c40: 2020 2020 2020 2020 2020 6973 696e 7374            isinst
-00018c50: 616e 6365 2863 6f6f 7264 732c 206e 702e  ance(coords, np.
-00018c60: 6e64 6172 7261 7929 292c 2028 2254 6865  ndarray)), ("The
-00018c70: 2027 636f 6f72 6473 2720 6b65 7920 220a   'coords' key ".
-00018c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c90: 2020 2020 2020 2020 2269 6e20 7468 6520          "in the 
-00018ca0: 696e 6974 2064 6963 7420 666f 7220 616e  init dict for an
-00018cb0: 206d 7370 7269 6d65 2073 6f75 7263 6520   msprime source 
-00018cc0: 706f 7075 6c61 7469 6f6e 2022 0a20 2020  population ".   
-00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ce0: 2020 2020 2022 6d75 7374 2068 6176 6520       "must have 
-00018cf0: 6120 6c69 7374 2c20 7475 706c 652c 206f  a list, tuple, o
-00018d00: 7220 6e75 6d70 792e 6e64 6172 7261 7920  r numpy.ndarray 
-00018d10: 6173 2022 0a20 2020 2020 2020 2020 2020  as ".           
-00018d20: 2020 2020 2020 2020 2020 2020 2022 6974               "it
-00018d30: 7320 7661 6c75 652e 2229 0a20 2020 2020  s value.").     
-00018d40: 2020 2020 2020 2063 6f6f 7264 735f 7374         coords_st
-00018d50: 7275 6374 5f65 7272 5f6d 7367 203d 2028  ruct_err_msg = (
-00018d60: 2254 6865 2027 636f 6f72 6473 2720 7661  "The 'coords' va
-00018d70: 6c75 6520 666f 7220 220a 2020 2020 2020  lue for ".      
-00018d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d90: 2020 2261 6e20 6d73 7072 696d 6520 736f    "an msprime so
-00018da0: 7572 6365 2070 6f70 756c 6174 6f6e 206d  urce populaton m
-00018db0: 7573 7420 6265 206f 6e65 206f 663a 2022  ust be one of: "
-00018dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018dd0: 2020 2020 2020 2020 2022 312e 2920 6120           "1.) a 
-00018de0: 6c69 7374 206f 7220 7475 706c 6520 6f66  list or tuple of
-00018df0: 206c 656e 6774 6820 322c 2067 6976 696e   length 2, givin
-00018e00: 6720 7468 6520 220a 2020 2020 2020 2020  g the ".        
-00018e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e20: 2263 6f6f 7264 696e 6174 6520 7061 6972  "coordinate pair
-00018e30: 2061 7420 7768 6963 6820 616c 6c20 496e   at which all In
-00018e40: 6469 7669 6475 616c 7320 220a 2020 2020  dividuals ".    
-00018e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e60: 2020 2020 2277 696c 6c20 6265 6769 6e20      "will begin 
-00018e70: 7468 6520 7369 6d75 6c61 7469 6f6e 3b20  the simulation; 
-00018e80: 322e 2920 6120 6c69 7374 206f 7220 7475  2.) a list or tu
-00018e90: 706c 6520 6f66 2022 0a20 2020 2020 2020  ple of ".       
-00018ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018eb0: 2022 636f 6f72 6469 6e61 7465 2070 6169   "coordinate pai
-00018ec0: 7273 2066 6f72 2061 6c6c 2049 6e64 6976  rs for all Indiv
-00018ed0: 6964 7561 6c73 2028 7374 7275 6374 7572  iduals (structur
-00018ee0: 6564 2022 0a20 2020 2020 2020 2020 2020  ed ".           
-00018ef0: 2020 2020 2020 2020 2020 2020 2022 6173               "as
-00018f00: 206e 2073 7562 6c69 7374 7320 6f72 2073   n sublists or s
-00018f10: 7562 7475 706c 6573 2c20 6561 6368 206f  ubtuples, each o
-00018f20: 6620 6c65 6e67 7468 2032 293b 206f 7220  f length 2); or 
-00018f30: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00018f40: 2020 2020 2020 2020 2020 2233 2e29 2061            "3.) a
-00018f50: 206e 756d 7079 2e6e 6461 7272 6179 206f   numpy.ndarray o
-00018f60: 6620 7468 6520 7361 6d65 2073 7472 7563  f the same struc
-00018f70: 7475 7265 2028 692e 652e 2c20 220a 2020  ture (i.e., ".  
-00018f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f90: 2020 2020 2020 2265 6974 6865 7220 3178        "either 1x
-00018fa0: 322c 2067 6976 696e 6720 6120 7369 6e67  2, giving a sing
-00018fb0: 6c65 2063 6f6f 7264 696e 6174 6520 7061  le coordinate pa
-00018fc0: 6972 2066 6f72 2022 0a20 2020 2020 2020  ir for ".       
-00018fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fe0: 2022 616c 6c20 496e 6469 7669 6475 616c   "all Individual
-00018ff0: 732c 206f 7220 6e78 322c 2073 7065 6369  s, or nx2, speci
-00019000: 6679 696e 6720 6c6f 6361 7469 6f6e 7320  fying locations 
-00019010: 666f 7220 220a 2020 2020 2020 2020 2020  for ".          
-00019020: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-00019030: 6c6c 206e 2049 6e64 6976 6964 7561 6c73  ll n Individuals
-00019040: 292e 2229 0a20 2020 2020 2020 2020 2020  ).").           
-00019050: 2069 6620 6973 696e 7374 616e 6365 2863   if isinstance(c
-00019060: 6f6f 7264 732c 206c 6973 7429 206f 7220  oords, list) or 
-00019070: 6973 696e 7374 616e 6365 2863 6f6f 7264  isinstance(coord
-00019080: 732c 2074 7570 6c65 293a 0a20 2020 2020  s, tuple):.     
-00019090: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-000190a0: 696e 7374 616e 6365 2863 6f6f 7264 735b  instance(coords[
-000190b0: 305d 2c20 6c69 7374 2920 6f72 2069 7369  0], list) or isi
-000190c0: 6e73 7461 6e63 6528 636f 6f72 6473 5b30  nstance(coords[0
-000190d0: 5d2c 2074 7570 6c65 293a 0a20 2020 2020  ], tuple):.     
-000190e0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000190f0: 7373 6572 7420 286e 702e 616c 6c28 5b6c  ssert (np.all([l
-00019100: 656e 2863 2920 3d3d 2032 2066 6f72 2063  en(c) == 2 for c
-00019110: 2069 6e20 636f 6f72 6473 5d29 2061 6e64   in coords]) and
+00018a90: 2022 6120 7365 7420 6f66 2076 616c 6964   "a set of valid
+00018aa0: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
+00018ab0: 7473 2074 6861 7420 220a 2020 2020 2020  ts that ".      
+00018ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ad0: 2020 2263 616e 2062 6520 7072 6f76 6964    "can be provid
+00018ae0: 6564 2074 6f20 4d6f 6465 6c2e 6164 645f  ed to Model.add_
+00018af0: 696e 6469 7669 6475 616c 7320 220a 2020  individuals ".  
+00018b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b10: 2020 2020 2020 2261 7320 7468 6520 2773        "as the 's
+00018b20: 6f75 7263 655f 6d73 7072 696d 655f 7061  ource_msprime_pa
+00018b30: 7261 6d73 2720 6469 6374 2e22 290a 2020  rams' dict.").  
+00018b40: 2020 2020 2020 2020 2020 6e20 3d20 5b2a            n = [*
+00018b50: 706f 702e 6b65 7973 2829 5d5b 305d 0a20  pop.keys()][0]. 
+00018b60: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00018b70: 7420 6973 696e 7374 616e 6365 286e 2c20  t isinstance(n, 
+00018b80: 696e 7429 2c20 2822 5468 6520 6b65 7920  int), ("The key 
+00018b90: 6f66 2065 6163 6820 220a 2020 2020 2020  of each ".      
+00018ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bb0: 2020 226d 7370 7269 6d65 2073 6f75 7263    "msprime sourc
+00018bc0: 6520 706f 7075 6c61 7469 6f6e 2069 6e20  e population in 
+00018bd0: 6120 5370 6563 6965 7327 2027 696e 6974  a Species' 'init
+00018be0: 2720 220a 2020 2020 2020 2020 2020 2020  ' ".            
+00018bf0: 2020 2020 2020 2020 2020 2020 2273 6563              "sec
+00018c00: 7469 6f6e 206f 6620 7468 6520 7061 7261  tion of the para
+00018c10: 6d65 7465 7273 2066 696c 6520 6d75 7374  meters file must
+00018c20: 2062 6520 616e 2069 6e74 2022 0a20 2020   be an int ".   
+00018c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c40: 2020 2020 2022 696e 6469 6361 7469 6e67       "indicating
+00018c50: 2074 6865 206e 756d 6265 7220 6f66 2073   the number of s
+00018c60: 7461 7274 696e 6720 496e 6469 7669 6475  tarting Individu
+00018c70: 616c 7320 220a 2020 2020 2020 2020 2020  als ".          
+00018c80: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00018c90: 6f20 6265 2073 6f75 7263 6564 2066 726f  o be sourced fro
+00018ca0: 6d20 7468 6174 2070 6f70 756c 6174 696f  m that populatio
+00018cb0: 6e2e 2229 0a20 2020 2020 2020 2020 2020  n.").           
+00018cc0: 2061 7373 6572 7420 2763 6f6f 7264 7327   assert 'coords'
+00018cd0: 2069 6e20 706f 705b 6e5d 2c20 2822 4561   in pop[n], ("Ea
+00018ce0: 6368 206d 7370 7269 6d65 2073 6f75 7263  ch msprime sourc
+00018cf0: 6520 706f 7075 6c61 7469 6f6e 2773 2022  e population's "
+00018d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d20: 2020 2020 2020 2020 2022 696e 6974 2070           "init p
+00018d30: 6172 616d 6574 6572 7320 6469 6374 206d  arameters dict m
+00018d40: 7573 7420 696e 636c 7564 6520 220a 2020  ust include ".  
+00018d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d70: 2020 2020 2020 2261 2027 636f 6f72 6473        "a 'coords
+00018d80: 2720 6b65 7920 7768 6f73 6520 7661 6c75  ' key whose valu
+00018d90: 6520 696e 6469 6361 7465 7320 220a 2020  e indicates ".  
+00018da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018dc0: 2020 2020 2020 2274 6865 206c 6f63 6174        "the locat
+00018dd0: 696f 6e2f 7320 7768 6572 6520 616c 6c20  ion/s where all 
+00018de0: 7361 6d70 6c65 6420 220a 2020 2020 2020  sampled ".      
+00018df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e10: 2020 2249 6e64 6976 6964 7561 6c73 2073    "Individuals s
+00018e20: 686f 756c 6420 6265 2070 6c61 6365 642e  hould be placed.
+00018e30: 2229 0a20 2020 2020 2020 2020 2020 2063  ").            c
+00018e40: 6f6f 7264 7320 3d20 706f 705b 6e5d 2e70  oords = pop[n].p
+00018e50: 6f70 2827 636f 6f72 6473 2729 0a20 2020  op('coords').   
+00018e60: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00018e70: 2869 7369 6e73 7461 6e63 6528 636f 6f72  (isinstance(coor
+00018e80: 6473 2c20 6c69 7374 2920 6f72 0a20 2020  ds, list) or.   
+00018e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ea0: 2069 7369 6e73 7461 6e63 6528 636f 6f72   isinstance(coor
+00018eb0: 6473 2c20 7475 706c 6529 206f 720a 2020  ds, tuple) or.  
+00018ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ed0: 2020 6973 696e 7374 616e 6365 2863 6f6f    isinstance(coo
+00018ee0: 7264 732c 206e 702e 6e64 6172 7261 7929  rds, np.ndarray)
+00018ef0: 292c 2028 2254 6865 2027 636f 6f72 6473  ), ("The 'coords
+00018f00: 2720 6b65 7920 220a 2020 2020 2020 2020  ' key ".        
+00018f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f20: 2269 6e20 7468 6520 696e 6974 2064 6963  "in the init dic
+00018f30: 7420 666f 7220 616e 206d 7370 7269 6d65  t for an msprime
+00018f40: 2073 6f75 7263 6520 706f 7075 6c61 7469   source populati
+00018f50: 6f6e 2022 0a20 2020 2020 2020 2020 2020  on ".           
+00018f60: 2020 2020 2020 2020 2020 2020 2022 6d75               "mu
+00018f70: 7374 2068 6176 6520 6120 6c69 7374 2c20  st have a list, 
+00018f80: 7475 706c 652c 206f 7220 6e75 6d70 792e  tuple, or numpy.
+00018f90: 6e64 6172 7261 7920 6173 2022 0a20 2020  ndarray as ".   
+00018fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fb0: 2020 2020 2022 6974 7320 7661 6c75 652e       "its value.
+00018fc0: 2229 0a20 2020 2020 2020 2020 2020 2063  ").            c
+00018fd0: 6f6f 7264 735f 7374 7275 6374 5f65 7272  oords_struct_err
+00018fe0: 5f6d 7367 203d 2028 2254 6865 2027 636f  _msg = ("The 'co
+00018ff0: 6f72 6473 2720 7661 6c75 6520 666f 7220  ords' value for 
+00019000: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00019010: 2020 2020 2020 2020 2020 2261 6e20 6d73            "an ms
+00019020: 7072 696d 6520 736f 7572 6365 2070 6f70  prime source pop
+00019030: 756c 6174 6f6e 206d 7573 7420 6265 206f  ulaton must be o
+00019040: 6e65 206f 663a 2022 0a20 2020 2020 2020  ne of: ".       
+00019050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019060: 2022 312e 2920 6120 6c69 7374 206f 7220   "1.) a list or 
+00019070: 7475 706c 6520 6f66 206c 656e 6774 6820  tuple of length 
+00019080: 322c 2067 6976 696e 6720 7468 6520 220a  2, giving the ".
+00019090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190a0: 2020 2020 2020 2020 2263 6f6f 7264 696e          "coordin
+000190b0: 6174 6520 7061 6972 2061 7420 7768 6963  ate pair at whic
+000190c0: 6820 616c 6c20 496e 6469 7669 6475 616c  h all Individual
+000190d0: 7320 220a 2020 2020 2020 2020 2020 2020  s ".            
+000190e0: 2020 2020 2020 2020 2020 2020 2277 696c              "wil
+000190f0: 6c20 6265 6769 6e20 7468 6520 7369 6d75  l begin the simu
+00019100: 6c61 7469 6f6e 3b20 322e 2920 6120 6c69  lation; 2.) a li
+00019110: 7374 206f 7220 7475 706c 6520 6f66 2022  st or tuple of "
 00019120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019130: 2020 2020 2020 2020 2020 2020 206c 656e               len
-00019140: 2863 6f6f 7264 7329 203d 3d20 6e29 2c20  (coords) == n), 
-00019150: 636f 6f72 6473 5f73 7472 7563 745f 6572  coords_struct_er
-00019160: 725f 6d73 670a 2020 2020 2020 2020 2020  r_msg.          
-00019170: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00019180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019190: 6173 7365 7274 206c 656e 2863 6f6f 7264  assert len(coord
-000191a0: 7329 203d 3d20 322c 2063 6f6f 7264 735f  s) == 2, coords_
-000191b0: 7374 7275 6374 5f65 7272 5f6d 7367 0a20  struct_err_msg. 
-000191c0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-000191d0: 6973 696e 7374 616e 6365 2863 6f6f 7264  isinstance(coord
-000191e0: 732c 206e 702e 6e64 6172 7261 7929 3a0a  s, np.ndarray):.
-000191f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019200: 6173 7365 7274 2028 636f 6f72 6473 2e73  assert (coords.s
-00019210: 6861 7065 203d 3d20 2831 2c20 3229 206f  hape == (1, 2) o
-00019220: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00019230: 2020 2020 2020 2020 2020 636f 6f72 6473            coords
-00019240: 2e73 6861 7065 203d 3d20 286e 2c20 3229  .shape == (n, 2)
-00019250: 292c 2063 6f6f 7264 735f 7374 7275 7374  ), coords_strust
-00019260: 5f65 7272 5f6d 7367 0a20 2020 2020 2020  _err_msg.       
-00019270: 2020 2020 2023 2073 696d 756c 6174 6520       # simulate 
-00019280: 7468 6520 696e 6469 7669 6475 616c 7320  the individuals 
-00019290: 616e 6420 6164 6420 7468 656d 2074 6f20  and add them to 
-000192a0: 7468 6520 5370 6563 6965 730a 2020 2020  the Species.    
-000192b0: 2020 2020 2020 2020 7365 6c66 2e5f 6164          self._ad
-000192c0: 645f 696e 6469 7669 6475 616c 7328 6e3d  d_individuals(n=
-000192d0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-000192e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192f0: 2020 2020 2063 6f6f 7264 733d 636f 6f72       coords=coor
-00019300: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
-00019310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019320: 2020 2020 2020 6c61 6e64 3d6c 616e 642c        land=land,
-00019330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019350: 2020 2073 6f75 7263 655f 6d73 7072 696d     source_msprim
-00019360: 655f 7061 7261 6d73 3d70 6f70 5b6e 5d2c  e_params=pop[n],
-00019370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019390: 2020 290a 2020 2020 2020 2020 2320 6368    ).        # ch
-000193a0: 6563 6b20 7468 6174 2074 6865 2053 7065  eck that the Spe
-000193b0: 6369 6573 2077 6f75 6e64 2075 7020 6861  cies wound up ha
-000193c0: 7669 6e67 2074 6865 2063 6f72 7265 6374  ving the correct
-000193d0: 2070 6f70 756c 6174 696f 6e20 7369 7a65   population size
-000193e0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000193f0: 6c65 6e28 7365 6c66 2920 3d3d 2074 6172  len(self) == tar
-00019400: 6765 745f 7369 7a65 2c20 2822 4166 7465  get_size, ("Afte
-00019410: 7220 616c 6c20 6d73 7072 696d 6520 736f  r all msprime so
-00019420: 7572 6365 2022 0a20 2020 2020 2020 2020  urce ".         
-00019430: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00019440: 706f 7075 6c61 7469 6f6e 7320 7765 7265  populations were
-00019450: 2073 616d 706c 6564 2c20 7468 6520 7265   sampled, the re
-00019460: 7375 6c74 696e 6720 220a 2020 2020 2020  sulting ".      
-00019470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019480: 2020 2270 6f70 756c 6174 696f 6e20 7369    "population si
-00019490: 7a65 2064 6f65 7320 6e6f 7420 6167 7265  ze does not agre
-000194a0: 6520 7769 7468 2022 0a20 2020 2020 2020  e with ".       
+00019130: 2020 2020 2020 2020 2022 636f 6f72 6469           "coordi
+00019140: 6e61 7465 2070 6169 7273 2066 6f72 2061  nate pairs for a
+00019150: 6c6c 2049 6e64 6976 6964 7561 6c73 2028  ll Individuals (
+00019160: 7374 7275 6374 7572 6564 2022 0a20 2020  structured ".   
+00019170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019180: 2020 2020 2022 6173 206e 2073 7562 6c69       "as n subli
+00019190: 7374 7320 6f72 2073 7562 7475 706c 6573  sts or subtuples
+000191a0: 2c20 6561 6368 206f 6620 6c65 6e67 7468  , each of length
+000191b0: 2032 293b 206f 7220 220a 2020 2020 2020   2); or ".      
+000191c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191d0: 2020 2233 2e29 2061 206e 756d 7079 2e6e    "3.) a numpy.n
+000191e0: 6461 7272 6179 206f 6620 7468 6520 7361  darray of the sa
+000191f0: 6d65 2073 7472 7563 7475 7265 2028 692e  me structure (i.
+00019200: 652e 2c20 220a 2020 2020 2020 2020 2020  e., ".          
+00019210: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00019220: 6974 6865 7220 3178 322c 2067 6976 696e  ither 1x2, givin
+00019230: 6720 6120 7369 6e67 6c65 2063 6f6f 7264  g a single coord
+00019240: 696e 6174 6520 7061 6972 2066 6f72 2022  inate pair for "
+00019250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019260: 2020 2020 2020 2020 2022 616c 6c20 496e           "all In
+00019270: 6469 7669 6475 616c 732c 206f 7220 6e78  dividuals, or nx
+00019280: 322c 2073 7065 6369 6679 696e 6720 6c6f  2, specifying lo
+00019290: 6361 7469 6f6e 7320 666f 7220 220a 2020  cations for ".  
+000192a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192b0: 2020 2020 2020 2261 6c6c 206e 2049 6e64        "all n Ind
+000192c0: 6976 6964 7561 6c73 292e 2229 0a20 2020  ividuals).").   
+000192d0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+000192e0: 7374 616e 6365 2863 6f6f 7264 732c 206c  stance(coords, l
+000192f0: 6973 7429 206f 7220 6973 696e 7374 616e  ist) or isinstan
+00019300: 6365 2863 6f6f 7264 732c 2074 7570 6c65  ce(coords, tuple
+00019310: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00019320: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00019330: 2863 6f6f 7264 735b 305d 2c20 6c69 7374  (coords[0], list
+00019340: 2920 6f72 2069 7369 6e73 7461 6e63 6528  ) or isinstance(
+00019350: 636f 6f72 6473 5b30 5d2c 2074 7570 6c65  coords[0], tuple
+00019360: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00019370: 2020 2020 2020 2061 7373 6572 7420 286e         assert (n
+00019380: 702e 616c 6c28 5b6c 656e 2863 2920 3d3d  p.all([len(c) ==
+00019390: 2032 2066 6f72 2063 2069 6e20 636f 6f72   2 for c in coor
+000193a0: 6473 5d29 2061 6e64 0a20 2020 2020 2020  ds]) and.       
+000193b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193c0: 2020 2020 206c 656e 2863 6f6f 7264 7329       len(coords)
+000193d0: 203d 3d20 6e29 2c20 636f 6f72 6473 5f73   == n), coords_s
+000193e0: 7472 7563 745f 6572 725f 6d73 670a 2020  truct_err_msg.  
+000193f0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00019400: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00019410: 2020 2020 2020 2020 6173 7365 7274 206c          assert l
+00019420: 656e 2863 6f6f 7264 7329 203d 3d20 322c  en(coords) == 2,
+00019430: 2063 6f6f 7264 735f 7374 7275 6374 5f65   coords_struct_e
+00019440: 7272 5f6d 7367 0a20 2020 2020 2020 2020  rr_msg.         
+00019450: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00019460: 6365 2863 6f6f 7264 732c 206e 702e 6e64  ce(coords, np.nd
+00019470: 6172 7261 7929 3a0a 2020 2020 2020 2020  array):.        
+00019480: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
+00019490: 636f 6f72 6473 2e73 6861 7065 203d 3d20  coords.shape == 
+000194a0: 2831 2c20 3229 206f 720a 2020 2020 2020  (1, 2) or.      
 000194b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194c0: 2022 7468 6520 7375 6d20 6f66 2074 6865   "the sum of the
-000194d0: 2073 6f75 7263 6520 706f 7075 6c61 7469   source populati
-000194e0: 6f6e 2073 616d 706c 6573 2022 0a20 2020  on samples ".   
-000194f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019500: 2020 2020 2022 7374 6970 756c 6174 6564       "stipulated
-00019510: 2069 6e20 7468 6520 7061 7261 6d65 7465   in the paramete
-00019520: 7273 2066 696c 652e 2229 0a0a 0a20 2020  rs file.")...   
-00019530: 2023 7573 6520 7468 6520 6b64 5f74 7265   #use the kd_tre
-00019540: 6520 6174 7472 6962 7574 6520 746f 2066  e attribute to f
-00019550: 696e 6420 6d61 7469 6e67 2070 6169 7273  ind mating pairs
-00019560: 2065 6974 6865 720a 2020 2020 2377 6974   either.    #wit
-00019570: 6869 6e20 7468 6520 7370 6563 6965 732c  hin the species,
-00019580: 2069 6620 7769 7468 696e 203d 3d20 5472   if within == Tr
-00019590: 7565 2c20 6f72 2062 6574 7765 656e 2074  ue, or between t
-000195a0: 6865 2073 7065 6369 6573 0a20 2020 2023  he species.    #
-000195b0: 616e 6420 7468 6520 706f 696e 7473 2070  and the points p
-000195c0: 726f 7669 6465 642c 2069 6620 7769 7468  rovided, if with
-000195d0: 696e 203d 3d20 4661 6c73 6520 616e 6420  in == False and 
-000195e0: 706f 696e 7473 2069 7320 6e6f 7420 4e6f  points is not No
-000195f0: 6e65 0a20 2020 2064 6566 205f 6765 745f  ne.    def _get_
-00019600: 6d61 7469 6e67 5f70 6169 7273 2873 656c  mating_pairs(sel
-00019610: 662c 2077 6974 6869 6e3d 5472 7565 2c20  f, within=True, 
-00019620: 636f 6f72 6473 3d4e 6f6e 652c 0a20 2020  coords=None,.   
-00019630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019640: 2020 2020 2020 2063 686f 6f73 655f 6e65         choose_ne
-00019650: 6172 6573 743d 4661 6c73 652c 2069 6e76  arest=False, inv
-00019660: 6572 7365 5f64 6973 745f 6d61 7469 6e67  erse_dist_mating
-00019670: 3d46 616c 7365 293a 0a20 2020 2020 2020  =False):.       
-00019680: 2023 4e4f 5445 3a20 496e 206c 6965 7520   #NOTE: In lieu 
-00019690: 6f66 2061 206d 6f72 6520 736f 7068 6973  of a more sophis
-000196a0: 7469 6361 7465 6420 7761 7920 6f66 0a20  ticated way of. 
-000196b0: 2020 2020 2020 2023 6465 7465 726d 696e         #determin
-000196c0: 696e 6720 7768 6574 6865 7220 7468 6520  ing whether the 
-000196d0: 6b64 5f74 7265 6520 6e65 6564 7320 746f  kd_tree needs to
-000196e0: 2062 6520 7570 6461 7465 6420 0a20 2020   be updated .   
-000196f0: 2020 2020 2023 2869 2e65 2e20 6966 2074       #(i.e. if t
-00019700: 6865 2073 7065 6369 6573 2068 6176 6520  he species have 
-00019710: 756e 6465 7267 6f6e 6520 6d6f 7665 6d65  undergone moveme
-00019720: 6e74 2c20 6d61 7469 6e67 2c0a 2020 2020  nt, mating,.    
-00019730: 2020 2020 236f 7220 6d6f 7274 616c 6974      #or mortalit
-00019740: 7920 7369 6e63 6520 7468 6520 6c61 7374  y since the last
-00019750: 2074 696d 6520 6974 2077 6173 200a 2020   time it was .  
-00019760: 2020 2020 2020 2363 6f6e 7374 7275 6374        #construct
-00019770: 6564 292c 2061 6e64 2069 6e20 616e 2065  ed), and in an e
-00019780: 6666 6f72 7420 746f 206d 696e 696d 697a  ffort to minimiz
-00019790: 6520 7468 6520 6e75 6d62 6572 0a20 2020  e the number.   
-000197a0: 2020 2020 2023 6f66 2074 696d 6573 2069       #of times i
-000197b0: 7420 6973 2063 6f6e 7374 7275 6374 6564  t is constructed
-000197c0: 2065 6163 6820 7469 6d65 2028 7369 6e63   each time (sinc
-000197d0: 650a 2020 2020 2020 2020 2369 7427 7320  e.        #it's 
-000197e0: 6e6f 7420 616e 2069 6e63 6f6e 7365 7175  not an inconsequ
-000197f0: 656e 7469 616c 2072 756e 7469 6d65 2c20  ential runtime, 
-00019800: 736f 2074 656c 6c69 6e67 2074 6865 0a20  so telling the. 
-00019810: 2020 2020 2020 2023 6d6f 6465 6c20 746f         #model to
-00019820: 2072 6562 7569 6c64 2069 7420 6166 7465   rebuild it afte
-00019830: 7220 6561 6368 206d 6f76 652c 2062 6972  r each move, bir
-00019840: 7468 2c20 6f72 0a20 2020 2020 2020 2023  th, or.        #
-00019850: 6465 6174 6820 7374 6570 2063 6f75 6c64  death step could
-00019860: 2062 6520 756e 6e63 6573 7361 7269 6c79   be unncessarily
-00019870: 2063 6f73 746c 7929 2c20 666f 7220 6e6f   costly), for no
-00019880: 7720 490a 2020 2020 2020 2020 2361 6d20  w I.        #am 
-00019890: 6a75 7374 2074 656c 6c69 6e67 2074 6865  just telling the
-000198a0: 2074 7265 6520 746f 2062 6520 7265 6275   tree to be rebu
-000198b0: 696c 7420 6561 6368 2074 696d 6520 0a20  ilt each time . 
-000198c0: 2020 2020 2020 2023 7468 6520 7370 702e         #the spp.
-000198d0: 5f67 6574 5f6d 6174 696e 675f 7061 6972  _get_mating_pair
-000198e0: 7328 2920 6d65 7468 6f64 2069 7320 6361  s() method is ca
-000198f0: 6c6c 6564 210a 2020 2020 2020 2020 7365  lled!.        se
-00019900: 6c66 2e5f 7365 745f 6b64 5f74 7265 6528  lf._set_kd_tree(
-00019910: 290a 0a20 2020 2020 2020 2023 2069 6620  )..        # if 
-00019920: 6d61 7469 6e67 5f72 6164 6975 7320 6973  mating_radius is
-00019930: 204e 6f6e 652c 2074 6865 6e20 6a75 7374   None, then just
-00019940: 2075 7365 2057 7269 6768 742d 4669 7368   use Wright-Fish
-00019950: 6572 0a20 2020 2020 2020 2023 2073 7479  er.        # sty
-00019960: 6c65 2070 616e 6d69 7869 6120 2864 7261  le panmixia (dra
-00019970: 7720 7769 7468 2072 6570 6c61 6365 6d65  w with replaceme
-00019980: 6e74 2061 2073 616d 706c 650a 2020 2020  nt a sample.    
-00019990: 2020 2020 2320 6f66 2073 697a 6520 3d20      # of size = 
-000199a0: 4e74 2a62 2c20 7768 6572 6520 4e74 2069  Nt*b, where Nt i
-000199b0: 7320 7468 6520 0a20 2020 2020 2020 2023  s the .        #
-000199c0: 2063 7572 7265 6e74 2070 6f70 2073 697a   current pop siz
-000199d0: 6520 616e 6420 6220 6973 2074 6865 2062  e and b is the b
-000199e0: 6972 7468 2072 6174 6520 2869 2e65 2e20  irth rate (i.e. 
-000199f0: 6d61 7469 6e67 2070 726f 6261 6269 6c69  mating probabili
-00019a00: 7479 293b 0a20 2020 2020 2020 2023 2074  ty);.        # t
-00019a10: 6861 7420 7361 6d70 6c65 2072 6570 7265  hat sample repre
-00019a20: 7365 6e74 7320 616c 6c20 6d61 7469 6e67  sents all mating
-00019a30: 2069 6e64 6976 6964 7561 6c73 2c20 616e   individuals, an
-00019a40: 6420 6561 6368 206f 6620 7468 6f73 650a  d each of those.
-00019a50: 2020 2020 2020 2020 2320 696e 6469 7669          # indivi
-00019a60: 6475 616c 7320 7261 6e64 6f6d 6c79 2063  duals randomly c
-00019a70: 686f 6f73 6573 2069 7473 206d 6174 650a  hooses its mate.
-00019a80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00019a90: 6d61 7469 6e67 5f72 6164 6975 7320 6973  mating_radius is
-00019aa0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00019ab0: 2020 2023 2064 7261 7720 6120 6e75 6d62     # draw a numb
-00019ac0: 6572 206f 6620 6d61 7469 6e67 2069 6e64  er of mating ind
-00019ad0: 6976 6964 7561 6c73 2061 7320 6120 6269  ividuals as a bi
-00019ae0: 6e6f 6d69 616c 2072 760a 2020 2020 2020  nomial rv.      
-00019af0: 2020 2020 2020 2320 7769 7468 206e 756d        # with num
-00019b00: 2074 7269 616c 7320 6571 7561 6c20 746f   trials equal to
-00019b10: 2070 6f70 2073 697a 6520 616e 6420 7072   pop size and pr
-00019b20: 6f62 6162 696c 6974 7920 6571 7561 6c20  obability equal 
-00019b30: 746f 0a20 2020 2020 2020 2020 2020 2023  to.            #
-00019b40: 2074 6865 2073 7065 6369 6573 2720 6269   the species' bi
-00019b50: 7274 6820 7261 7465 0a20 2020 2020 2020  rth rate.       
-00019b60: 2020 2020 2069 6620 7365 6c66 2e62 203c       if self.b <
-00019b70: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-00019b80: 2020 2020 6e5f 6d61 7465 7320 3d20 6e70      n_mates = np
-00019b90: 2e72 616e 646f 6d2e 6269 6e6f 6d69 616c  .random.binomial
-00019ba0: 286e 3d6c 656e 2873 656c 6629 2c20 703d  (n=len(self), p=
-00019bb0: 7365 6c66 2e62 290a 2020 2020 2020 2020  self.b).        
-00019bc0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00019bd0: 2020 2020 2020 2020 2020 6e5f 6d61 7465            n_mate
-00019be0: 7320 3d20 6c65 6e28 7365 6c66 290a 2020  s = len(self).  
-00019bf0: 2020 2020 2020 2020 2020 7472 6565 5f69            tree_i
-00019c00: 6e64 7320 3d20 7365 6c66 2e5f 6b64 5f74  nds = self._kd_t
-00019c10: 7265 652e 7472 6565 2e69 6e64 6963 6573  ree.tree.indices
-00019c20: 0a20 2020 2020 2020 2020 2020 2023 2064  .            # d
-00019c30: 7261 7720 322a 6e5f 6d61 7465 7320 6d61  raw 2*n_mates ma
-00019c40: 7469 6e67 2069 6e64 6976 6964 7561 6c73  ting individuals
-00019c50: 2c20 7769 7468 2072 6570 6c61 6365 6d65  , with replaceme
-00019c60: 6e74 2028 6173 2069 6e20 5746 0a20 2020  nt (as in WF.   
-00019c70: 2020 2020 2020 2020 2023 206d 6f64 656c           # model
-00019c80: 292c 2074 6865 6e20 666f 6c64 2069 6e74  ), then fold int
-00019c90: 6f20 616e 206e 5f6d 6174 6573 2078 2032  o an n_mates x 2
-00019ca0: 206d 6174 652d 7061 6972 7320 6172 7261   mate-pairs arra
-00019cb0: 790a 2020 2020 2020 2020 2020 2020 7061  y.            pa
-00019cc0: 6972 7320 3d20 6e70 2e72 616e 646f 6d2e  irs = np.random.
-00019cd0: 6368 6f69 6365 2874 7265 655f 696e 6473  choice(tree_inds
-00019ce0: 2c20 7265 706c 6163 653d 5472 7565 2c0a  , replace=True,.
-00019cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d10: 2020 2020 2073 697a 653d 6e5f 6d61 7465       size=n_mate
-00019d20: 732a 3229 2e72 6573 6861 7065 2828 6e5f  s*2).reshape((n_
-00019d30: 6d61 7465 732c 2032 2929 0a20 2020 2020  mates, 2)).     
-00019d40: 2020 2020 2020 2023 2067 6574 2072 6964         # get rid
-00019d50: 206f 6620 7365 6c66 696e 6720 7061 6972   of selfing pair
-00019d60: 730a 2020 2020 2020 2020 2020 2020 7061  s.            pa
-00019d70: 6972 7320 3d20 6e70 2e61 7272 6179 285b  irs = np.array([
-00019d80: 6c69 7374 2870 6169 7229 2066 6f72 2070  list(pair) for p
-00019d90: 6169 7220 696e 206c 6973 7428 0a20 2020  air in list(.   
-00019da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019dc0: 206d 6170 2873 6574 2c20 7061 6972 7329   map(set, pairs)
-00019dd0: 2920 6966 206c 656e 2870 6169 7229 203d  ) if len(pair) =
-00019de0: 3d20 325d 290a 2020 2020 2020 2020 2020  = 2]).          
-00019df0: 2020 7061 6972 7320 3d20 6e70 2e61 7272    pairs = np.arr
-00019e00: 6179 2870 6169 7273 290a 0a20 2020 2020  ay(pairs)..     
-00019e10: 2020 2023 206f 7468 6572 7769 7365 2c20     # otherwise, 
-00019e20: 6368 6f6f 7365 206d 6174 6573 2075 7369  choose mates usi
-00019e30: 6e67 206d 6174 696e 6720 7261 6469 7573  ng mating radius
-00019e40: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00019e50: 2020 2020 2020 2020 2020 2023 6966 206e             #if n
-00019e60: 6569 6768 626f 7273 2061 7265 2074 6f20  eighbors are to 
-00019e70: 6265 2066 6f75 6e64 2077 6974 6869 6e20  be found within 
-00019e80: 7468 6520 7370 6563 6965 732c 0a20 2020  the species,.   
-00019e90: 2020 2020 2020 2020 2023 7365 7420 636f           #set co
-00019ea0: 6f72 6473 2074 6f20 7365 6c66 2e5f 636f  ords to self._co
-00019eb0: 6f72 6473 2028 6f74 6865 7277 6973 652c  ords (otherwise,
-00019ec0: 2074 6865 2063 6f6f 7264 7320 746f 0a20   the coords to. 
-00019ed0: 2020 2020 2020 2020 2020 2023 6669 6e64             #find
-00019ee0: 206e 6561 7265 7374 206e 6569 6768 626f   nearest neighbo
-00019ef0: 7273 2077 6974 6820 7368 6f75 6c64 2068  rs with should h
-00019f00: 6176 6520 6265 656e 2070 726f 7669 6465  ave been provide
-00019f10: 6429 0a20 2020 2020 2020 2020 2020 2069  d).            i
-00019f20: 6620 7769 7468 696e 3a0a 2020 2020 2020  f within:.      
-00019f30: 2020 2020 2020 2020 2020 636f 6f72 6473            coords
-00019f40: 203d 2073 656c 662e 5f63 6f6f 7264 730a   = self._coords.
-00019f50: 0a20 2020 2020 2020 2020 2020 2023 7175  .            #qu
-00019f60: 6572 7920 7468 6520 7472 6565 2074 6f20  ery the tree to 
-00019f70: 6765 7420 6d61 7469 6e67 2070 6169 7273  get mating pairs
-00019f80: 0a20 2020 2020 2020 2020 2020 2070 6169  .            pai
-00019f90: 7273 203d 2073 656c 662e 5f6b 645f 7472  rs = self._kd_tr
-00019fa0: 6565 2e5f 6765 745f 6d61 7469 6e67 5f70  ee._get_mating_p
-00019fb0: 6169 7273 2863 6f6f 7264 733d 636f 6f72  airs(coords=coor
-00019fc0: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
-00019fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ff0: 2020 2020 6469 7374 3d73 656c 662e 6d61      dist=self.ma
-0001a000: 7469 6e67 5f72 6164 6975 732c 0a20 2020  ting_radius,.   
-0001a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a030: 2020 2020 2020 2020 2020 2020 2063 686f               cho
-0001a040: 6f73 655f 6e65 6172 6573 743d 6368 6f6f  ose_nearest=choo
-0001a050: 7365 5f6e 6561 7265 7374 2c0a 2020 2020  se_nearest,.    
-0001a060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a080: 2020 2020 696e 7665 7273 655f 6469 7374      inverse_dist
-0001a090: 5f6d 6174 696e 673d 696e 7665 7273 655f  _mating=inverse_
-0001a0a0: 6469 7374 5f6d 6174 696e 6729 0a0a 2020  dist_mating)..  
-0001a0b0: 2020 2020 2020 2020 2020 2320 7573 6520            # use 
-0001a0c0: 7468 6520 7370 6563 6965 7327 2062 6972  the species' bir
-0001a0d0: 7468 2072 6174 6520 746f 2064 6563 6964  th rate to decid
-0001a0e0: 6520 2861 7320 6265 726e 6f75 6c6c 6920  e (as bernoulli 
-0001a0f0: 6472 6177 7329 0a20 2020 2020 2020 2020  draws).         
-0001a100: 2020 2023 2077 6865 7468 6572 2065 6163     # whether eac
-0001a110: 6820 7061 6972 2063 616e 206d 6174 650a  h pair can mate.
-0001a120: 2020 2020 2020 2020 2020 2020 6361 6e5f              can_
-0001a130: 6d61 7465 203d 206e 702e 626f 6f6c 3828  mate = np.bool8(
-0001a140: 6e70 2e72 616e 646f 6d2e 6269 6e6f 6d69  np.random.binomi
-0001a150: 616c 286e 3d31 2c20 703d 7365 6c66 2e62  al(n=1, p=self.b
-0001a160: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a190: 2020 2020 2073 697a 653d 7061 6972 732e       size=pairs.
-0001a1a0: 7368 6170 655b 305d 2929 0a20 2020 2020  shape[0])).     
-0001a1b0: 2020 2020 2020 2070 6169 7273 203d 2070         pairs = p
-0001a1c0: 6169 7273 5b63 616e 5f6d 6174 652c 203a  airs[can_mate, :
-0001a1d0: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
-0001a1e0: 2070 6169 7273 0a0a 0a20 2020 2064 6566   pairs...    def
-0001a1f0: 205f 6d61 6b65 5f67 6561 5f64 6628 7365   _make_gea_df(se
-0001a200: 6c66 2c20 6c79 725f 6e75 6d3d 3129 3a0a  lf, lyr_num=1):.
-0001a210: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-0001a220: 2020 2020 204d 616b 6573 2061 2064 6174       Makes a dat
-0001a230: 6166 7261 6d65 2066 6f72 2047 4541 2061  aframe for GEA a
-0001a240: 6e61 6c79 7369 7320 636f 6e74 6169 6e69  nalysis containi
-0001a250: 6e67 2067 656e 6f74 7970 6573 2c20 636f  ng genotypes, co
-0001a260: 6f72 6469 6e61 7465 732c 0a20 2020 2020  ordinates,.     
-0001a270: 2020 2061 6e64 2065 6e76 2076 616c 7565     and env value
-0001a280: 7320 666f 7220 616c 6c20 696e 6469 7669  s for all indivi
-0001a290: 6475 616c 732e 0a0a 2020 2020 2020 2020  duals...        
-0001a2a0: 4e4f 5445 3a20 4375 7272 656e 746c 7920  NOTE: Currently 
-0001a2b0: 6f6e 6c79 2061 6363 6570 7473 206f 6e65  only accepts one
-0001a2c0: 204c 616e 6473 6361 7065 204c 6179 6572   Landscape Layer
-0001a2d0: 2028 692e 652e 2065 6e76 6972 6f6e 6d65   (i.e. environme
-0001a2e0: 6e74 616c 0a20 2020 2020 2020 2020 2020  ntal.           
-0001a2f0: 2020 2076 6172 6961 626c 6529 0a0a 2020     variable)..  
-0001a300: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0001a310: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0001a320: 2d2d 2d0a 2020 2020 2020 2020 6c79 725f  ---.        lyr_
-0001a330: 6e75 6d20 3a20 696e 740a 2020 2020 2020  num : int.      
-0001a340: 2020 2020 2020 5468 6520 6e75 6d62 6572        The number
-0001a350: 206f 6620 7468 6520 4c61 6e64 7363 6170   of the Landscap
-0001a360: 6520 4c61 7965 7220 6672 6f6d 2077 6869  e Layer from whi
-0001a370: 6368 2074 6f20 6578 7472 6163 740a 2020  ch to extract.  
-0001a380: 2020 2020 2020 2020 2020 656e 7669 726f            enviro
-0001a390: 6e6d 656e 7461 6c20 7661 6c75 6573 2e20  nmental values. 
-0001a3a0: 4465 6661 756c 7473 2074 6f20 312e 0a0a  Defaults to 1...
-0001a3b0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0001a3c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0001a3d0: 2020 2020 2020 2020 6f75 7420 3a20 7061          out : pa
-0001a3e0: 6e64 6173 2e44 6174 6146 7261 6d65 0a20  ndas.DataFrame. 
-0001a3f0: 2020 2020 2020 2020 2020 2041 2044 6174             A Dat
-0001a400: 6146 7261 6d65 2069 6e20 7768 6963 6820  aFrame in which 
-0001a410: 636f 6c75 6d6e 7320 6172 6520 6c6f 6369  columns are loci
-0001a420: 2061 6e64 2072 6f77 7320 6172 6520 696e   and rows are in
-0001a430: 6469 7669 6475 616c 730a 2020 2020 2020  dividuals.      
-0001a440: 2020 2222 220a 2020 2020 2020 2020 2367    """.        #g
-0001a450: 6574 2061 7272 6179 206f 6620 5b30 7c30  et array of [0|0
-0001a460: 2e35 7c31 5d20 6765 6e6f 7479 7065 730a  .5|1] genotypes.
-0001a470: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0001a480: 2020 2020 6765 6e20 3d20 7365 6c66 2e5f      gen = self._
-0001a490: 6765 745f 6765 6e6f 7479 7065 7328 290a  get_genotypes().
-0001a4a0: 0a20 2020 2020 2020 2023 6c6f 6f70 2074  .        #loop t
-0001a4b0: 6f20 636f 6e76 6572 7420 6269 6e61 7279  o convert binary
-0001a4c0: 2061 6c6c 656c 6520 6765 6e6f 7479 7065   allele genotype
-0001a4d0: 7320 2830 7c31 290a 2020 2020 2020 2020  s (0|1).        
-0001a4e0: 2369 6e74 6f20 7369 6e67 6c65 2064 6967  #into single dig
-0001a4f0: 6974 2067 656e 6f74 7970 6573 2028 302c  it genotypes (0,
-0001a500: 2030 2e35 2c20 3129 0a20 2020 2020 2020   0.5, 1).       
-0001a510: 2067 656e 6f5f 696e 6420 3d20 5b5d 0a20   geno_ind = []. 
-0001a520: 2020 2020 2020 2066 6f72 2069 6e64 2069         for ind i
-0001a530: 6e20 7261 6e67 6528 6c65 6e28 6765 6e29  n range(len(gen)
-0001a540: 293a 0a20 2020 2020 2020 2020 2020 2067  ):.            g
-0001a550: 656e 6f5f 6c6f 6320 3d20 5b5d 0a20 2020  eno_loc = [].   
-0001a560: 2020 2020 2020 2020 2066 6f72 206c 6f63           for loc
-0001a570: 6920 696e 2072 616e 6765 286c 656e 2867  i in range(len(g
-0001a580: 656e 5b69 6e64 5d29 293a 0a20 2020 2020  en[ind])):.     
-0001a590: 2020 2020 2020 2020 2020 2067 656e 6f74             genot
-0001a5a0: 7970 6520 3d20 6765 6e5b 696e 645d 5b6c  ype = gen[ind][l
-0001a5b0: 6f63 695d 2e6d 6561 6e28 2920 2320 636f  oci].mean() # co
-0001a5c0: 6465 6420 6173 2030 2f30 2e35 2f31 0a20  ded as 0/0.5/1. 
-0001a5d0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-0001a5e0: 656e 6f5f 6c6f 632e 6170 7065 6e64 2867  eno_loc.append(g
-0001a5f0: 656e 6f74 7970 6529 0a20 2020 2020 2020  enotype).       
-0001a600: 2020 2020 2067 656e 6f5f 696e 642e 6170       geno_ind.ap
-0001a610: 7065 6e64 2867 656e 6f5f 6c6f 6329 0a20  pend(geno_loc). 
-0001a620: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001a630: 2020 2067 7473 203d 2073 656c 662e 5f67     gts = self._g
-0001a640: 6574 5f67 656e 6f74 7970 6573 2862 6961  et_genotypes(bia
-0001a650: 6c6c 656c 6963 3d46 616c 7365 290a 0a20  llelic=False).. 
-0001a660: 2020 2020 2020 2023 636f 6e76 6572 7420         #convert 
-0001a670: 746f 2064 6174 6166 7261 6d65 0a20 2020  to dataframe.   
-0001a680: 2020 2020 2067 6561 5f64 6620 3d20 7064       gea_df = pd
-0001a690: 2e44 6174 6146 7261 6d65 2867 7473 290a  .DataFrame(gts).
-0001a6a0: 0a20 2020 2020 2020 2023 6765 7420 656e  .        #get en
-0001a6b0: 7669 726f 6e6d 656e 7461 6c20 6461 7461  vironmental data
-0001a6c0: 0a20 2020 2020 2020 2065 6e76 203d 2073  .        env = s
-0001a6d0: 656c 662e 5f67 6574 5f65 2829 0a20 2020  elf._get_e().   
-0001a6e0: 2020 2020 2067 6561 5f64 665b 2765 6e76       gea_df['env
-0001a6f0: 275d 203d 206c 6973 7428 656e 765b 3a2c  '] = list(env[:,
-0001a700: 6c79 725f 6e75 6d5d 290a 0a20 2020 2020  lyr_num])..     
-0001a710: 2020 2023 6765 7420 636f 6f72 6473 0a20     #get coords. 
-0001a720: 2020 2020 2020 2063 6f6f 7264 203d 2073         coord = s
-0001a730: 656c 662e 5f67 6574 5f63 6f6f 7264 7328  elf._get_coords(
-0001a740: 290a 2020 2020 2020 2020 6765 615f 6466  ).        gea_df
-0001a750: 5b27 6c61 7427 5d20 3d20 6c69 7374 2863  ['lat'] = list(c
-0001a760: 6f6f 7264 5b3a 2c30 5d29 0a20 2020 2020  oord[:,0]).     
-0001a770: 2020 2067 6561 5f64 665b 276c 6f6e 6727     gea_df['long'
-0001a780: 5d20 3d20 6c69 7374 2863 6f6f 7264 5b3a  ] = list(coord[:
-0001a790: 2c31 5d29 0a0a 2020 2020 2020 2020 7265  ,1])..        re
-0001a7a0: 7475 726e 2067 6561 5f64 660a 0a0a 2020  turn gea_df...  
-0001a7b0: 2020 6465 6620 5f72 756e 5f63 6361 2873    def _run_cca(s
-0001a7c0: 656c 662c 2074 7274 5f6e 756d 3d30 2c20  elf, trt_num=0, 
-0001a7d0: 7363 616c 653d 5472 7565 2c20 706c 6f74  scale=True, plot
-0001a7e0: 3d54 7275 652c 2070 6c6f 745f 7364 3d54  =True, plot_sd=T
-0001a7f0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-0001a800: 2020 2020 2020 7364 3d33 293a 0a20 2020        sd=3):.   
-0001a810: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001a820: 2052 756e 7320 6120 6361 6e6f 6e69 6361   Runs a canonica
-0001a830: 6c20 636f 7272 656c 6174 696f 6e20 616e  l correlation an
-0001a840: 616c 7973 6973 2028 4343 4129 206f 6e20  alysis (CCA) on 
-0001a850: 7468 6520 6375 7272 656e 7420 6765 6e65  the current gene
-0001a860: 7469 6320 616e 640a 2020 2020 2020 2020  tic and.        
-0001a870: 656e 7669 726f 6e6d 656e 7461 6c20 6461  environmental da
-0001a880: 7461 2066 6f72 2074 6865 2053 7065 6369  ta for the Speci
-0001a890: 6573 2720 6375 7272 656e 7420 706f 7075  es' current popu
-0001a8a0: 6c61 7469 6f6e 2c20 7573 696e 6720 7468  lation, using th
-0001a8b0: 650a 2020 2020 2020 2020 696e 6469 6361  e.        indica
-0001a8c0: 7465 6420 5472 6169 742e 2050 6c6f 7473  ted Trait. Plots
-0001a8d0: 2074 6865 2072 6573 756c 7473 2061 6e64   the results and
-0001a8e0: 2072 6574 7572 6e73 2074 6865 6d20 696e   returns them in
-0001a8f0: 2061 2064 6963 742e 0a0a 2020 2020 2020   a dict...      
-0001a900: 2020 4343 4120 6d6f 6465 6c20 666f 726d    CCA model form
-0001a910: 756c 613a 2067 656e 6f74 7970 6520 7e20  ula: genotype ~ 
-0001a920: 656e 7620 2b20 6c61 7420 2b20 6c6f 6e67  env + lat + long
-0001a930: 0a0a 2020 2020 2020 2020 4e4f 5445 3a20  ..        NOTE: 
-0001a940: 6375 7272 656e 746c 7920 6f6e 6c79 2070  currently only p
-0001a950: 6f73 7369 626c 6520 746f 2064 6f20 3320  ossible to do 3 
-0001a960: 636f 6d70 6f6e 656e 7473 2f33 2076 6172  components/3 var
-0001a970: 6961 626c 6573 3b0a 2020 2020 2020 2020  iables;.        
-0001a980: 2020 2020 2020 7769 6c6c 2061 6464 2067        will add g
-0001a990: 7265 6174 6572 2066 756e 6374 696f 6e61  reater functiona
-0001a9a0: 6c69 7479 2069 6e20 7468 6520 6675 7475  lity in the futu
-0001a9b0: 7265 0a0a 2020 2020 2020 2020 5061 7261  re..        Para
-0001a9c0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-0001a9d0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-0001a9e0: 2020 7472 745f 6e75 6d20 3a20 696e 740a    trt_num : int.
-0001a9f0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0001aa00: 6e75 6d62 6572 206f 6620 7468 6520 5472  number of the Tr
-0001aa10: 6169 7420 746f 2072 756e 2074 6865 2047  ait to run the G
-0001aa20: 4541 206f 6e2e 2044 6566 6175 6c74 7320  EA on. Defaults 
-0001aa30: 746f 2030 2e0a 2020 2020 2020 2020 7363  to 0..        sc
-0001aa40: 616c 6520 3a20 626f 6f6c 0a20 2020 2020  ale : bool.     
-0001aa50: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
-0001aa60: 7363 616c 6573 2074 6865 2076 6172 6961  scales the varia
-0001aa70: 626c 652c 2069 6e64 6976 6964 7561 6c2c  ble, individual,
-0001aa80: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-0001aa90: 206c 6f63 7573 206c 6f61 6469 6e67 7320   locus loadings 
-0001aaa0: 6672 6f6d 202d 3120 746f 2031 2074 6f20  from -1 to 1 to 
-0001aab0: 6d61 6b65 2074 6865 6d20 6561 7369 6572  make them easier
-0001aac0: 0a20 2020 2020 2020 2020 2020 2074 6f20  .            to 
-0001aad0: 7669 7375 616c 697a 652e 2044 6566 6175  visualize. Defau
-0001aae0: 6c74 7320 746f 2054 7275 652e 0a20 2020  lts to True..   
-0001aaf0: 2020 2020 2070 6c6f 7420 3a20 626f 6f6c       plot : bool
-0001ab00: 0a20 2020 2020 2020 2020 2020 2057 6865  .            Whe
-0001ab10: 7468 6572 206f 7220 6e6f 7420 746f 2070  ther or not to p
-0001ab20: 6c6f 7420 7468 6520 6d6f 6465 6c2e 2044  lot the model. D
-0001ab30: 6566 6175 6c74 7320 746f 2054 7275 652e  efaults to True.
-0001ab40: 0a20 2020 2020 2020 2070 6c6f 745f 7364  .        plot_sd
-0001ab50: 203a 2062 6f6f 6c0a 2020 2020 2020 2020   : bool.        
-0001ab60: 2020 2020 4966 2054 7275 652c 2061 2073      If True, a s
-0001ab70: 7461 6e64 6172 6420 6465 7669 6174 696f  tandard deviatio
-0001ab80: 6e20 656c 6c69 7073 6520 6973 2070 6c6f  n ellipse is plo
-0001ab90: 7474 6564 2c20 7573 696e 6720 7468 6520  tted, using the 
-0001aba0: 6e75 6d62 6572 0a20 2020 2020 2020 2020  number.         
-0001abb0: 2020 206f 6620 7374 616e 6461 7264 2064     of standard d
-0001abc0: 6576 6961 7469 6f6e 7320 696e 6469 6361  eviations indica
-0001abd0: 7465 6420 6279 2074 6865 2061 7267 756d  ted by the argum
-0001abe0: 656e 7420 2773 6427 2e20 4465 6661 756c  ent 'sd'. Defaul
-0001abf0: 7473 2074 6f0a 2020 2020 2020 2020 2020  ts to.          
-0001ac00: 2020 5472 7565 2e0a 2020 2020 2020 2020    True..        
-0001ac10: 7364 203a 207b 696e 742c 2066 6c6f 6174  sd : {int, float
-0001ac20: 7d0a 2020 2020 2020 2020 2020 2020 4e75  }.            Nu
-0001ac30: 6d62 6572 206f 6620 7374 616e 6461 7264  mber of standard
-0001ac40: 2064 6576 6961 7469 6f6e 7320 746f 2075   deviations to u
-0001ac50: 7365 2066 6f72 2070 6c6f 7474 696e 6720  se for plotting 
-0001ac60: 7468 6520 7374 616e 6461 7264 0a20 2020  the standard.   
-0001ac70: 2020 2020 2020 2020 2064 6576 6961 7469           deviati
-0001ac80: 6f6e 2065 6c6c 6970 7365 2e20 4465 6661  on ellipse. Defa
-0001ac90: 756c 7473 2074 6f20 332e 0a0a 2020 2020  ults to 3...    
-0001aca0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0001acb0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0001acc0: 2020 2020 6f75 7420 3a20 6469 6374 0a20      out : dict. 
-0001acd0: 2020 2020 2020 2020 2020 2041 2064 6963             A dic
-0001ace0: 7420 6f66 2074 6865 2066 6f6c 6c6f 7769  t of the followi
-0001acf0: 6e67 206b 6579 2d76 616c 7565 2070 6169  ng key-value pai
-0001ad00: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-0001ad10: 2020 2020 2267 6561 5f64 6622 3a20 6120      "gea_df": a 
-0001ad20: 4461 7461 4672 616d 6520 6f66 2069 6e64  DataFrame of ind
-0001ad30: 6976 6964 7561 6c73 2720 6765 6e6f 7479  ividuals' genoty
-0001ad40: 7065 732c 2065 6e76 6972 6f6e 6d65 6e74  pes, environment
-0001ad50: 616c 0a20 2020 2020 2020 2020 2020 2020  al.             
-0001ad60: 2020 2020 2020 2020 2020 2020 2076 616c               val
-0001ad70: 7565 732c 2061 6e64 2063 6f6f 7264 696e  ues, and coordin
-0001ad80: 6174 6573 0a20 2020 2020 2020 2020 2020  ates.           
-0001ad90: 2020 2020 2022 696e 645f 4343 4164 6622       "ind_CCAdf"
-0001ada0: 3a20 696e 6469 7669 6475 616c 206c 6f61  : individual loa
-0001adb0: 6469 6e67 7320 2863 6f6c 756d 6e73 203d  dings (columns =
-0001adc0: 2061 7865 732c 0a20 2020 2020 2020 2020   axes,.         
-0001add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ade0: 2020 2020 726f 7773 203d 2069 6e64 6976      rows = indiv
-0001adf0: 6964 7561 6c73 290a 2020 2020 2020 2020  iduals).        
-0001ae00: 2020 2020 2020 2020 226c 6f63 695f 4343          "loci_CC
-0001ae10: 4164 6622 3a20 6c6f 6375 7320 6c6f 6164  Adf": locus load
-0001ae20: 696e 6773 2028 636f 6c75 6d6e 7320 3d20  ings (columns = 
-0001ae30: 6178 6573 2c20 726f 7773 203d 206c 6f63  axes, rows = loc
-0001ae40: 6929 0a20 2020 2020 2020 2020 2020 2020  i).             
-0001ae50: 2020 2022 7661 725f 4343 4164 6622 3a20     "var_CCAdf": 
-0001ae60: 7661 7269 6162 6c65 206c 6f61 6469 6e67  variable loading
-0001ae70: 7320 2863 6f6c 756d 6e73 203d 2061 7865  s (columns = axe
-0001ae80: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0001ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aea0: 726f 7773 203d 2076 6172 6961 626c 6520  rows = variable 
-0001aeb0: 2865 6e76 2c20 6c61 742c 206c 6f6e 6729  (env, lat, long)
-0001aec0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001aed0: 2020 2274 7261 6974 5f6c 6f63 6922 3a20    "trait_loci": 
-0001aee0: 6c69 7374 206f 6620 696e 6465 7865 7320  list of indexes 
-0001aef0: 666f 7220 6c6f 6369 2074 6861 7420 756e  for loci that un
-0001af00: 6465 726c 6965 2074 6865 2074 7261 6974  derlie the trait
-0001af10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001af20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001af30: 6f72 2077 6869 6368 2074 6865 2043 4341  or which the CCA
-0001af40: 2077 6173 2072 756e 0a20 2020 2020 2020   was run.       
-0001af50: 2022 2222 0a20 2020 2020 2020 2023 6d61   """.        #ma
-0001af60: 6b65 2044 460a 2020 2020 2020 2020 6765  ke DF.        ge
-0001af70: 615f 6466 203d 7365 6c66 2e5f 6d61 6b65  a_df =self._make
-0001af80: 5f67 6561 5f64 6628 6c79 725f 6e75 6d3d  _gea_df(lyr_num=
-0001af90: 7365 6c66 2e67 656e 5f61 7263 682e 7472  self.gen_arch.tr
-0001afa0: 6169 7473 5b74 7274 5f6e 756d 5d2e 6c79  aits[trt_num].ly
-0001afb0: 725f 6e75 6d29 0a0a 2020 2020 2020 2020  r_num)..        
-0001afc0: 2367 6574 2061 6461 7074 6976 6520 6c6f  #get adaptive lo
-0001afd0: 6369 2028 7573 6564 206c 6174 6572 2069  ci (used later i
-0001afe0: 6e20 706c 6f74 7469 6e67 290a 2020 2020  n plotting).    
-0001aff0: 2020 2020 7472 6169 745f 6c6f 6369 203d      trait_loci =
-0001b000: 2073 656c 662e 6765 6e5f 6172 6368 2e74   self.gen_arch.t
-0001b010: 7261 6974 735b 7472 745f 6e75 6d5d 2e6c  raits[trt_num].l
-0001b020: 6f63 6920 2367 6574 7320 7472 6169 7420  oci #gets trait 
-0001b030: 6c6f 6369 2069 6e64 6578 6573 0a0a 2020  loci indexes..  
-0001b040: 2020 2020 2020 2367 6574 206e 756d 6265        #get numbe
-0001b050: 7220 6f66 206c 6f63 690a 2020 2020 2020  r of loci.      
-0001b060: 2020 4c20 3d20 7365 6c66 2e67 656e 5f61    L = self.gen_a
-0001b070: 7263 682e 4c0a 2020 2020 2020 2020 2364  rch.L.        #d
-0001b080: 6566 696e 6520 7820 616e 6420 793a 0a20  efine x and y:. 
-0001b090: 2020 2020 2020 2023 2070 756c 6c20 6f75         # pull ou
-0001b0a0: 7420 6765 6e6f 7479 7065 730a 2020 2020  t genotypes.    
-0001b0b0: 2020 2020 5920 3d20 6765 615f 6466 2e69      Y = gea_df.i
-0001b0c0: 6c6f 635b 3a2c 7261 6e67 6528 4c29 5d0a  loc[:,range(L)].
-0001b0d0: 2020 2020 2020 2020 2320 7075 6c6c 206f          # pull o
-0001b0e0: 7574 2070 7265 6469 6374 6f72 2076 6172  ut predictor var
-0001b0f0: 6961 626c 6573 0a20 2020 2020 2020 2023  iables.        #
-0001b100: 2054 4f44 4f3a 206d 616b 6520 6974 2070   TODO: make it p
-0001b110: 6f73 7369 626c 6520 746f 2063 686f 6f73  ossible to choos
-0001b120: 6520 6d6f 7265 2076 6172 7320 696e 2066  e more vars in f
-0001b130: 7574 7572 650a 2020 2020 2020 2020 5820  uture.        X 
-0001b140: 3d20 6765 615f 6466 5b5b 2765 6e76 272c  = gea_df[['env',
-0001b150: 276c 6174 272c 276c 6f6e 6727 5d5d 0a0a  'lat','long']]..
-0001b160: 2020 2020 2020 2020 2364 6566 696e 6520          #define 
-0001b170: 6e5f 636f 6d70 6f6e 656e 7473 0a20 2020  n_components.   
-0001b180: 2020 2020 206e 5f63 6f6d 706f 6e65 6e74       n_component
-0001b190: 7320 3d20 330a 2020 2020 2020 2020 2363  s = 3.        #c
-0001b1a0: 7265 6174 6520 7468 6520 4343 4120 6d6f  reate the CCA mo
-0001b1b0: 6465 6c20 616e 6420 6669 7420 6974 2074  del and fit it t
-0001b1c0: 6f20 7468 6520 6461 7461 0a20 2020 2020  o the data.     
-0001b1d0: 2020 2063 6361 203d 2043 4341 286e 5f63     cca = CCA(n_c
-0001b1e0: 6f6d 706f 6e65 6e74 7320 3d20 6e5f 636f  omponents = n_co
-0001b1f0: 6d70 6f6e 656e 7473 290a 2020 2020 2020  mponents).      
-0001b200: 2020 6363 612e 6669 7428 592c 2058 290a    cca.fit(Y, X).
-0001b210: 0a20 2020 2020 2020 2023 7472 616e 7366  .        #transf
-0001b220: 6f72 6d20 6461 7461 0a20 2020 2020 2020  orm data.       
-0001b230: 2059 5f63 203d 2063 6361 2e74 7261 6e73   Y_c = cca.trans
-0001b240: 666f 726d 2859 290a 0a20 2020 2020 2020  form(Y)..       
-0001b250: 2023 6372 6561 7465 2064 6620 666f 7220   #create df for 
-0001b260: 696e 6469 7669 6475 616c 730a 2020 2020  individuals.    
-0001b270: 2020 2020 696e 645f 6466 203d 2070 642e      ind_df = pd.
-0001b280: 4461 7461 4672 616d 6528 595f 6329 0a20  DataFrame(Y_c). 
-0001b290: 2020 2020 2020 2023 6e61 6d69 6e67 2043         #naming C
-0001b2a0: 4341 2063 6f6c 756d 6e73 2073 7461 7274  CA columns start
-0001b2b0: 696e 6720 6174 2031 0a20 2020 2020 2020  ing at 1.       
-0001b2c0: 2069 6e64 5f64 662e 636f 6c75 6d6e 7320   ind_df.columns 
-0001b2d0: 3d20 5b73 7472 2872 2920 666f 7220 7220  = [str(r) for r 
-0001b2e0: 696e 2072 616e 6765 2831 2c20 6e5f 636f  in range(1, n_co
-0001b2f0: 6d70 6f6e 656e 7473 202b 2031 295d 0a0a  mponents + 1)]..
-0001b300: 2020 2020 2020 2020 2363 7265 6174 6520          #create 
-0001b310: 6466 2066 6f72 206c 6f63 690a 2020 2020  df for loci.    
-0001b320: 2020 2020 6c6f 6369 5f64 6620 3d20 7064      loci_df = pd
-0001b330: 2e44 6174 6146 7261 6d65 2863 6361 2e78  .DataFrame(cca.x
-0001b340: 5f6c 6f61 6469 6e67 735f 290a 2020 2020  _loadings_).    
-0001b350: 2020 2020 6c6f 6369 5f64 662e 636f 6c75      loci_df.colu
-0001b360: 6d6e 7320 3d20 696e 645f 6466 2e63 6f6c  mns = ind_df.col
-0001b370: 756d 6e73 2023 7361 6d65 2063 6f6c 756d  umns #same colum
-0001b380: 6e20 6e61 6d65 730a 0a20 2020 2020 2020  n names..       
-0001b390: 2023 6372 6561 7465 2064 6620 666f 7220   #create df for 
-0001b3a0: 7661 7269 6162 6c65 730a 2020 2020 2020  variables.      
-0001b3b0: 2020 7661 725f 6466 203d 2070 642e 4461    var_df = pd.Da
-0001b3c0: 7461 4672 616d 6528 6363 612e 795f 6c6f  taFrame(cca.y_lo
-0001b3d0: 6164 696e 6773 5f29 0a20 2020 2020 2020  adings_).       
-0001b3e0: 2076 6172 5f64 662e 636f 6c75 6d6e 7320   var_df.columns 
-0001b3f0: 3d20 696e 645f 6466 2e63 6f6c 756d 6e73  = ind_df.columns
-0001b400: 2023 7361 6d65 2063 6f6c 756d 6e20 6e61   #same column na
-0001b410: 6d65 730a 0a20 2020 2020 2020 2023 6d61  mes..        #ma
-0001b420: 6b65 2064 6963 7469 6f6e 6172 7920 6f66  ke dictionary of
-0001b430: 2064 6174 6166 7261 6d65 7320 746f 2072   dataframes to r
-0001b440: 6574 7572 6e0a 2020 2020 2020 2020 6363  eturn.        cc
-0001b450: 615f 6469 6374 203d 207b 2767 6561 5f64  a_dict = {'gea_d
-0001b460: 6627 3a67 6561 5f64 662c 0a20 2020 2020  f':gea_df,.     
-0001b470: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0001b480: 696e 645f 6466 273a 696e 645f 6466 2c0a  ind_df':ind_df,.
-0001b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b4a0: 2020 2020 276c 6f63 695f 6466 273a 6c6f      'loci_df':lo
-0001b4b0: 6369 5f64 662c 0a20 2020 2020 2020 2020  ci_df,.         
-0001b4c0: 2020 2020 2020 2020 2020 2027 7661 725f             'var_
-0001b4d0: 6466 273a 7661 725f 6466 2c0a 2020 2020  df':var_df,.    
-0001b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b4f0: 2774 7261 6974 5f6c 6f63 6927 3a74 7261  'trait_loci':tra
-0001b500: 6974 5f6c 6f63 697d 0a0a 2020 2020 2020  it_loci}..      
-0001b510: 2020 2320 4e4f 5445 3a20 7269 6768 7420    # NOTE: right 
-0001b520: 6e6f 7720 7468 6973 2070 6c6f 7474 696e  now this plottin
-0001b530: 6720 6c6f 6f70 206f 6e6c 7920 776f 726b  g loop only work
-0001b540: 7320 666f 7220 6120 6d61 7869 6d75 6d20  s for a maximum 
-0001b550: 6f66 2033 2061 7865 733b 0a20 2020 2020  of 3 axes;.     
-0001b560: 2020 2023 2020 2020 2020 2069 6e20 7468     #       in th
-0001b570: 6520 6675 7475 7265 2061 7320 6d6f 7265  e future as more
-0001b580: 2065 6e76 2076 6172 7320 6172 6520 6164   env vars are ad
-0001b590: 6465 642c 2063 6f75 6c64 2061 6464 206d  ded, could add m
-0001b5a0: 6f72 6520 6178 6573 0a20 2020 2020 2020  ore axes.       
-0001b5b0: 2069 6620 706c 6f74 3a0a 2020 2020 2020   if plot:.      
-0001b5c0: 2020 2020 2020 2353 6361 6c65 2064 6174        #Scale dat
-0001b5d0: 6166 7261 6d65 7320 6672 6f6d 202d 3120  aframes from -1 
-0001b5e0: 746f 2031 2069 6620 7363 616c 6520 3d20  to 1 if scale = 
-0001b5f0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0001b600: 2069 6620 7363 616c 6520 3d3d 2054 7275   if scale == Tru
-0001b610: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001b620: 2020 2072 6d69 6e20 3d20 2d31 0a20 2020     rmin = -1.   
-0001b630: 2020 2020 2020 2020 2020 2020 2072 6d61               rma
-0001b640: 7820 3d20 310a 2020 2020 2020 2020 2020  x = 1.          
-0001b650: 2020 2020 2020 6c6f 6369 5f64 6620 3d20        loci_df = 
-0001b660: 726d 696e 202b 2028 6c6f 6369 5f64 6620  rmin + (loci_df 
-0001b670: 2d20 6c6f 6369 5f64 662e 7661 6c75 6573  - loci_df.values
-0001b680: 2e6d 696e 2829 2920 2a20 2872 6d61 7820  .min()) * (rmax 
-0001b690: 2d0a 2020 2020 2020 2020 2020 2020 2020  -.              
-0001b6a0: 2020 2020 2020 2020 2020 2872 6d69 6e29            (rmin)
-0001b6b0: 2920 2f20 286c 6f63 695f 6466 2e76 616c  ) / (loci_df.val
-0001b6c0: 7565 732e 6d61 7828 2920 2d20 6c6f 6369  ues.max() - loci
-0001b6d0: 5f64 662e 7661 6c75 6573 2e6d 696e 2829  _df.values.min()
-0001b6e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001b6f0: 2020 7661 725f 6466 203d 2072 6d69 6e20    var_df = rmin 
-0001b700: 2b20 2876 6172 5f64 6620 2d20 7661 725f  + (var_df - var_
-0001b710: 6466 2e76 616c 7565 732e 6d69 6e28 2929  df.values.min())
-0001b720: 202a 2028 726d 6178 202d 0a20 2020 2020   * (rmax -.     
-0001b730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b740: 2020 2028 726d 696e 2929 202f 2028 7661     (rmin)) / (va
-0001b750: 725f 6466 2e76 616c 7565 732e 6d61 7828  r_df.values.max(
-0001b760: 2920 2d20 7661 725f 6466 2e76 616c 7565  ) - var_df.value
-0001b770: 732e 6d69 6e28 2929 0a20 2020 2020 2020  s.min()).       
-0001b780: 2020 2020 2020 2020 2069 6e64 5f64 6620           ind_df 
-0001b790: 3d20 726d 696e 202b 2028 696e 645f 6466  = rmin + (ind_df
-0001b7a0: 202d 2069 6e64 5f64 662e 7661 6c75 6573   - ind_df.values
-0001b7b0: 2e6d 696e 2829 2920 2a20 2872 6d61 7820  .min()) * (rmax 
-0001b7c0: 2d0a 2020 2020 2020 2020 2020 2020 2020  -.              
-0001b7d0: 2020 2020 2020 2020 2020 2872 6d69 6e29            (rmin)
-0001b7e0: 2920 2f20 2869 6e64 5f64 662e 7661 6c75  ) / (ind_df.valu
-0001b7f0: 6573 2e6d 6178 2829 202d 2069 6e64 5f64  es.max() - ind_d
-0001b800: 662e 7661 6c75 6573 2e6d 696e 2829 290a  f.values.min()).
-0001b810: 0a0a 2020 2020 2020 2020 2020 2020 2367  ..            #g
-0001b820: 6574 206d 6178 2061 6e64 206d 696e 7320  et max and mins 
-0001b830: 746f 2073 6574 2061 7869 7320 6c61 7465  to set axis late
-0001b840: 7220 6f6e 0a20 2020 2020 2020 2020 2020  r on.           
-0001b850: 206d 6178 6466 203d 206d 6178 2869 6e64   maxdf = max(ind
-0001b860: 5f64 662e 7661 6c75 6573 2e6d 6178 2829  _df.values.max()
-0001b870: 2c20 7661 725f 6466 2e76 616c 7565 732e  , var_df.values.
-0001b880: 6d61 7828 292c 0a20 2020 2020 2020 2020  max(),.         
-0001b890: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0001b8a0: 6f63 695f 6466 2e76 616c 7565 732e 6d61  oci_df.values.ma
-0001b8b0: 7828 2929 0a20 2020 2020 2020 2020 2020  x()).           
-0001b8c0: 206d 696e 6466 203d 2061 6273 286d 696e   mindf = abs(min
-0001b8d0: 2869 6e64 5f64 662e 7661 6c75 6573 2e6d  (ind_df.values.m
-0001b8e0: 696e 2829 2c20 7661 725f 6466 2e76 616c  in(), var_df.val
-0001b8f0: 7565 732e 6d69 6e28 292c 0a20 2020 2020  ues.min(),.     
-0001b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b910: 2020 2020 2020 206c 6f63 695f 6466 2e76         loci_df.v
-0001b920: 616c 7565 732e 6d69 6e28 2929 290a 2020  alues.min())).  
-0001b930: 2020 2020 2020 2020 2020 6178 6d61 7820            axmax 
-0001b940: 3d20 6d61 7828 6d61 7864 662c 206d 696e  = max(maxdf, min
-0001b950: 6466 2920 2a20 312e 3230 2023 6164 6469  df) * 1.20 #addi
-0001b960: 6e67 2061 2032 3025 2062 7566 6665 720a  ng a 20% buffer.
-0001b970: 0a20 2020 2020 2020 2020 2020 2023 7365  .            #se
-0001b980: 7420 7570 2066 6967 7572 650a 2020 2020  t up figure.    
-0001b990: 2020 2020 2020 2020 6669 6720 3d20 706c          fig = pl
-0001b9a0: 742e 6669 6775 7265 2866 6967 7369 7a65  t.figure(figsize
-0001b9b0: 3d28 3230 2c20 3135 2929 0a20 2020 2020  =(20, 15)).     
-0001b9c0: 2020 2020 2020 2066 6f72 206e 2c20 6363         for n, cc
-0001b9d0: 5f61 7865 735f 7061 6972 2069 6e20 656e  _axes_pair in en
-0001b9e0: 756d 6572 6174 6528 5b5b 312c 2032 5d2c  umerate([[1, 2],
-0001b9f0: 205b 312c 2033 5d2c 205b 322c 2033 5d5d   [1, 3], [2, 3]]
-0001ba00: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001ba10: 2020 2023 6465 6669 6e65 2063 6f6d 706f     #define compo
-0001ba20: 6e65 6e74 7320 666f 7220 6178 6973 0a20  nents for axis. 
-0001ba30: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001ba40: 635f 6178 6973 3120 3d20 6363 5f61 7865  c_axis1 = cc_axe
-0001ba50: 735f 7061 6972 5b30 5d20 2378 2d61 7869  s_pair[0] #x-axi
-0001ba60: 7320 4343 0a20 2020 2020 2020 2020 2020  s CC.           
-0001ba70: 2020 2020 2063 635f 6178 6973 3220 3d20       cc_axis2 = 
-0001ba80: 6363 5f61 7865 735f 7061 6972 5b31 5d20  cc_axes_pair[1] 
-0001ba90: 2379 2d61 7869 7320 4343 0a0a 2020 2020  #y-axis CC..    
-0001baa0: 2020 2020 2020 2020 2020 2020 6178 203d              ax =
-0001bab0: 2066 6967 2e61 6464 5f73 7562 706c 6f74   fig.add_subplot
-0001bac0: 2831 3331 2b6e 290a 0a20 2020 2020 2020  (131+n)..       
-0001bad0: 2020 2020 2020 2020 2023 6164 6420 6365           #add ce
-0001bae0: 6e74 6572 206c 696e 6573 0a20 2020 2020  nter lines.     
-0001baf0: 2020 2020 2020 2020 2020 2061 782e 6178             ax.ax
-0001bb00: 686c 696e 6528 793d 302c 2063 6f6c 6f72  hline(y=0, color
-0001bb10: 3d27 6c69 6768 7467 7261 7927 2c20 6c69  ='lightgray', li
-0001bb20: 6e65 7374 796c 653d 2764 6f74 7465 6427  nestyle='dotted'
-0001bb30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001bb40: 2020 6178 2e61 7876 6c69 6e65 2878 3d30    ax.axvline(x=0
-0001bb50: 2c20 636f 6c6f 723d 276c 6967 6874 6772  , color='lightgr
-0001bb60: 6179 272c 206c 696e 6573 7479 6c65 3d27  ay', linestyle='
-0001bb70: 646f 7474 6564 2729 0a0a 2020 2020 2020  dotted')..      
-0001bb80: 2020 2020 2020 2020 2020 2320 7365 7420            # set 
-0001bb90: 6178 6573 2072 616e 6765 0a20 2020 2020  axes range.     
-0001bba0: 2020 2020 2020 2020 2020 2070 6c74 2e78             plt.x
-0001bbb0: 6c69 6d28 2d61 786d 6178 2c20 6178 6d61  lim(-axmax, axma
-0001bbc0: 7829 0a20 2020 2020 2020 2020 2020 2020  x).             
-0001bbd0: 2020 2070 6c74 2e79 6c69 6d28 2d61 786d     plt.ylim(-axm
-0001bbe0: 6178 2c20 6178 6d61 7829 0a0a 2020 2020  ax, axmax)..    
-0001bbf0: 2020 2020 2020 2020 2020 2020 2370 6c6f              #plo
-0001bc00: 7420 6e65 7574 7261 6c20 534e 5073 0a20  t neutral SNPs. 
-0001bc10: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0001bc20: 782e 7363 6174 7465 7228 6c6f 6369 5f64  x.scatter(loci_d
-0001bc30: 665b 7374 7228 6363 5f61 7869 7331 295d  f[str(cc_axis1)]
-0001bc40: 2c20 6c6f 6369 5f64 665b 7374 7228 6363  , loci_df[str(cc
-0001bc50: 5f61 7869 7332 295d 2c0a 2020 2020 2020  _axis2)],.      
-0001bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc70: 2020 2020 206d 6172 6b65 7220 3d20 272b       marker = '+
-0001bc80: 272c 2063 6f6c 6f72 203d 2027 6772 6179  ', color = 'gray
-0001bc90: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-0001bca0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-0001bcb0: 6265 6c20 3d20 274e 6575 7472 616c 2053  bel = 'Neutral S
-0001bcc0: 4e50 7327 2c20 616c 7068 6120 3d20 302e  NPs', alpha = 0.
-0001bcd0: 3729 0a20 2020 2020 2020 2020 2020 2020  7).             
-0001bce0: 2020 2023 706c 6f74 2069 6e64 6976 6964     #plot individ
-0001bcf0: 7561 6c73 0a20 2020 2020 2020 2020 2020  uals.           
-0001bd00: 2020 2020 2063 6d61 705f 7363 6174 203d       cmap_scat =
-0001bd10: 2061 782e 7363 6174 7465 7228 696e 645f   ax.scatter(ind_
-0001bd20: 6466 5b73 7472 2863 635f 6178 6973 3129  df[str(cc_axis1)
-0001bd30: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0001bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd50: 2020 2020 2020 2020 2020 696e 645f 6466            ind_df
-0001bd60: 5b73 7472 2863 635f 6178 6973 3229 5d2c  [str(cc_axis2)],
-0001bd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd90: 2020 2020 2020 2020 6320 3d20 6765 615f          c = gea_
-0001bda0: 6466 2e65 6e76 2c20 636d 6170 3d27 7669  df.env, cmap='vi
-0001bdb0: 7269 6469 7327 2c0a 2020 2020 2020 2020  ridis',.        
-0001bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bdd0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0001bde0: 6162 656c 203d 2022 496e 6469 7669 6475  abel = "Individu
-0001bdf0: 616c 7322 2c20 616c 7068 6120 3d20 302e  als", alpha = 0.
-0001be00: 3529 0a20 2020 2020 2020 2020 2020 2020  5).             
-0001be10: 2020 2023 706c 6f74 2061 6461 7074 6976     #plot adaptiv
-0001be20: 6520 534e 5073 0a20 2020 2020 2020 2020  e SNPs.         
-0001be30: 2020 2020 2020 2061 782e 7363 6174 7465         ax.scatte
-0001be40: 7228 6c6f 6369 5f64 665b 7374 7228 6363  r(loci_df[str(cc
-0001be50: 5f61 7869 7331 295d 5b74 7261 6974 5f6c  _axis1)][trait_l
-0001be60: 6f63 695d 2c0a 2020 2020 2020 2020 2020  oci],.          
-0001be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be80: 206c 6f63 695f 6466 5b73 7472 2863 635f   loci_df[str(cc_
-0001be90: 6178 6973 3229 5d5b 7472 6169 745f 6c6f  axis2)][trait_lo
-0001bea0: 6369 5d2c 0a20 2020 2020 2020 2020 2020  ci],.           
-0001beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bec0: 6d61 726b 6572 3d22 2b22 2c20 636f 6c6f  marker="+", colo
-0001bed0: 7220 3d20 2272 6564 222c 2073 3d31 3030  r = "red", s=100
-0001bee0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001bef0: 2020 2020 2020 2020 2020 2020 206c 6162               lab
-0001bf00: 656c 203d 2027 4164 6170 7469 7665 2053  el = 'Adaptive S
-0001bf10: 4e50 7327 290a 0a20 2020 2020 2020 2020  NPs')..         
-0001bf20: 2020 2020 2020 2023 706c 6f74 2076 6172         #plot var
-0001bf30: 6961 626c 6520 7665 6374 6f72 7320 6173  iable vectors as
-0001bf40: 2061 7272 6f77 730a 2020 2020 2020 2020   arrows.        
-0001bf50: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-0001bf60: 2072 616e 6765 2876 6172 5f64 662e 7368   range(var_df.sh
-0001bf70: 6170 655b 305d 293a 0a20 2020 2020 2020  ape[0]):.       
-0001bf80: 2020 2020 2020 2020 2020 2020 2078 203d               x =
-0001bf90: 2076 6172 5f64 665b 7374 7228 6363 5f61   var_df[str(cc_a
-0001bfa0: 7869 7331 295d 5b69 5d0a 2020 2020 2020  xis1)][i].      
-0001bfb0: 2020 2020 2020 2020 2020 2020 2020 7920                y 
-0001bfc0: 3d20 7661 725f 6466 5b73 7472 2863 635f  = var_df[str(cc_
-0001bfd0: 6178 6973 3229 5d5b 695d 0a20 2020 2020  axis2)][i].     
-0001bfe0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001bff0: 6c74 2e61 7272 6f77 2830 2c20 302c 2078  lt.arrow(0, 0, x
-0001c000: 2c20 792c 2077 6964 7468 203d 2030 2e30  , y, width = 0.0
-0001c010: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-0001c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c030: 2068 6561 645f 7769 6474 6820 3d20 302e   head_width = 0.
-0001c040: 3035 2c20 636f 6c6f 7220 3d20 2762 6c61  05, color = 'bla
-0001c050: 636b 2729 0a20 2020 2020 2020 2020 2020  ck').           
-0001c060: 2020 2020 2020 2020 2073 7820 3d20 302e           sx = 0.
-0001c070: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-0001c080: 2020 2020 2020 7379 203d 2030 2e31 0a20        sy = 0.1. 
-0001c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c0a0: 2020 2023 2074 6869 7320 6d65 7373 2069     # this mess i
-0001c0b0: 7320 6a75 7374 2074 6f20 6172 7261 6e67  s just to arrang
-0001c0c0: 6520 7468 6520 7465 7874 0a20 2020 2020  e the text.     
-0001c0d0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001c0e0: 206e 6578 7420 746f 2061 7272 6f77 7320   next to arrows 
-0001c0f0: 6275 7420 6974 2069 7320 6120 5749 500a  but it is a WIP.
+000194c0: 2020 636f 6f72 6473 2e73 6861 7065 203d    coords.shape =
+000194d0: 3d20 286e 2c20 3229 292c 2063 6f6f 7264  = (n, 2)), coord
+000194e0: 735f 7374 7275 6374 5f65 7272 5f6d 7367  s_struct_err_msg
+000194f0: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
+00019500: 696d 756c 6174 6520 7468 6520 696e 6469  imulate the indi
+00019510: 7669 6475 616c 7320 616e 6420 6164 6420  viduals and add 
+00019520: 7468 656d 2074 6f20 7468 6520 5370 6563  them to the Spec
+00019530: 6965 730a 2020 2020 2020 2020 2020 2020  ies.            
+00019540: 7365 6c66 2e5f 6164 645f 696e 6469 7669  self._add_indivi
+00019550: 6475 616c 7328 6e3d 6e2c 0a20 2020 2020  duals(n=n,.     
+00019560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019570: 2020 2020 2020 2020 2020 2020 2063 6f6f               coo
+00019580: 7264 733d 636f 6f72 6473 2c0a 2020 2020  rds=coords,.    
+00019590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195a0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+000195b0: 6e64 3d6c 616e 642c 0a20 2020 2020 2020  nd=land,.       
+000195c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195d0: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+000195e0: 655f 6d73 7072 696d 655f 7061 7261 6d73  e_msprime_params
+000195f0: 3d70 6f70 5b6e 5d2c 0a20 2020 2020 2020  =pop[n],.       
+00019600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019610: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00019620: 2020 2020 2320 6368 6563 6b20 7468 6174      # check that
+00019630: 2074 6865 2053 7065 6369 6573 2077 6f75   the Species wou
+00019640: 6e64 2075 7020 6861 7669 6e67 2074 6865  nd up having the
+00019650: 2063 6f72 7265 6374 2070 6f70 756c 6174   correct populat
+00019660: 696f 6e20 7369 7a65 0a20 2020 2020 2020  ion size.       
+00019670: 2061 7373 6572 7420 6c65 6e28 7365 6c66   assert len(self
+00019680: 2920 3d3d 2074 6172 6765 745f 7369 7a65  ) == target_size
+00019690: 2c20 2822 4166 7465 7220 616c 6c20 6d73  , ("After all ms
+000196a0: 7072 696d 6520 736f 7572 6365 2022 0a20  prime source ". 
+000196b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196c0: 2020 2020 2020 2022 706f 7075 6c61 7469         "populati
+000196d0: 6f6e 7320 7765 7265 2073 616d 706c 6564  ons were sampled
+000196e0: 2c20 7468 6520 7265 7375 6c74 696e 6720  , the resulting 
+000196f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00019700: 2020 2020 2020 2020 2020 2270 6f70 756c            "popul
+00019710: 6174 696f 6e20 7369 7a65 2064 6f65 7320  ation size does 
+00019720: 6e6f 7420 6167 7265 6520 7769 7468 2022  not agree with "
+00019730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019740: 2020 2020 2020 2020 2022 7468 6520 7375           "the su
+00019750: 6d20 6f66 2074 6865 2073 6f75 7263 6520  m of the source 
+00019760: 706f 7075 6c61 7469 6f6e 2073 616d 706c  population sampl
+00019770: 6573 2022 0a20 2020 2020 2020 2020 2020  es ".           
+00019780: 2020 2020 2020 2020 2020 2020 2022 7374               "st
+00019790: 6970 756c 6174 6564 2069 6e20 7468 6520  ipulated in the 
+000197a0: 7061 7261 6d65 7465 7273 2066 696c 652e  parameters file.
+000197b0: 2229 0a0a 0a20 2020 2023 7573 6520 7468  ")...    #use th
+000197c0: 6520 6b64 5f74 7265 6520 6174 7472 6962  e kd_tree attrib
+000197d0: 7574 6520 746f 2066 696e 6420 6d61 7469  ute to find mati
+000197e0: 6e67 2070 6169 7273 2065 6974 6865 720a  ng pairs either.
+000197f0: 2020 2020 2377 6974 6869 6e20 7468 6520      #within the 
+00019800: 7370 6563 6965 732c 2069 6620 7769 7468  species, if with
+00019810: 696e 203d 3d20 5472 7565 2c20 6f72 2062  in == True, or b
+00019820: 6574 7765 656e 2074 6865 2073 7065 6369  etween the speci
+00019830: 6573 0a20 2020 2023 616e 6420 7468 6520  es.    #and the 
+00019840: 706f 696e 7473 2070 726f 7669 6465 642c  points provided,
+00019850: 2069 6620 7769 7468 696e 203d 3d20 4661   if within == Fa
+00019860: 6c73 6520 616e 6420 706f 696e 7473 2069  lse and points i
+00019870: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2064  s not None.    d
+00019880: 6566 205f 6765 745f 6d61 7469 6e67 5f70  ef _get_mating_p
+00019890: 6169 7273 2873 656c 662c 2077 6974 6869  airs(self, withi
+000198a0: 6e3d 5472 7565 2c20 636f 6f72 6473 3d4e  n=True, coords=N
+000198b0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+000198c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000198d0: 686f 6f73 655f 6e65 6172 6573 743d 4661  hoose_nearest=Fa
+000198e0: 6c73 652c 2069 6e76 6572 7365 5f64 6973  lse, inverse_dis
+000198f0: 745f 6d61 7469 6e67 3d46 616c 7365 293a  t_mating=False):
+00019900: 0a20 2020 2020 2020 2023 4e4f 5445 3a20  .        #NOTE: 
+00019910: 496e 206c 6965 7520 6f66 2061 206d 6f72  In lieu of a mor
+00019920: 6520 736f 7068 6973 7469 6361 7465 6420  e sophisticated 
+00019930: 7761 7920 6f66 0a20 2020 2020 2020 2023  way of.        #
+00019940: 6465 7465 726d 696e 696e 6720 7768 6574  determining whet
+00019950: 6865 7220 7468 6520 6b64 5f74 7265 6520  her the kd_tree 
+00019960: 6e65 6564 7320 746f 2062 6520 7570 6461  needs to be upda
+00019970: 7465 6420 0a20 2020 2020 2020 2023 2869  ted .        #(i
+00019980: 2e65 2e20 6966 2074 6865 2073 7065 6369  .e. if the speci
+00019990: 6573 2068 6176 6520 756e 6465 7267 6f6e  es have undergon
+000199a0: 6520 6d6f 7665 6d65 6e74 2c20 6d61 7469  e movement, mati
+000199b0: 6e67 2c0a 2020 2020 2020 2020 236f 7220  ng,.        #or 
+000199c0: 6d6f 7274 616c 6974 7920 7369 6e63 6520  mortality since 
+000199d0: 7468 6520 6c61 7374 2074 696d 6520 6974  the last time it
+000199e0: 2077 6173 200a 2020 2020 2020 2020 2363   was .        #c
+000199f0: 6f6e 7374 7275 6374 6564 292c 2061 6e64  onstructed), and
+00019a00: 2069 6e20 616e 2065 6666 6f72 7420 746f   in an effort to
+00019a10: 206d 696e 696d 697a 6520 7468 6520 6e75   minimize the nu
+00019a20: 6d62 6572 0a20 2020 2020 2020 2023 6f66  mber.        #of
+00019a30: 2074 696d 6573 2069 7420 6973 2063 6f6e   times it is con
+00019a40: 7374 7275 6374 6564 2065 6163 6820 7469  structed each ti
+00019a50: 6d65 2028 7369 6e63 650a 2020 2020 2020  me (since.      
+00019a60: 2020 2369 7427 7320 6e6f 7420 616e 2069    #it's not an i
+00019a70: 6e63 6f6e 7365 7175 656e 7469 616c 2072  nconsequential r
+00019a80: 756e 7469 6d65 2c20 736f 2074 656c 6c69  untime, so telli
+00019a90: 6e67 2074 6865 0a20 2020 2020 2020 2023  ng the.        #
+00019aa0: 6d6f 6465 6c20 746f 2072 6562 7569 6c64  model to rebuild
+00019ab0: 2069 7420 6166 7465 7220 6561 6368 206d   it after each m
+00019ac0: 6f76 652c 2062 6972 7468 2c20 6f72 0a20  ove, birth, or. 
+00019ad0: 2020 2020 2020 2023 6465 6174 6820 7374         #death st
+00019ae0: 6570 2063 6f75 6c64 2062 6520 756e 6e63  ep could be unnc
+00019af0: 6573 7361 7269 6c79 2063 6f73 746c 7929  essarily costly)
+00019b00: 2c20 666f 7220 6e6f 7720 490a 2020 2020  , for now I.    
+00019b10: 2020 2020 2361 6d20 6a75 7374 2074 656c      #am just tel
+00019b20: 6c69 6e67 2074 6865 2074 7265 6520 746f  ling the tree to
+00019b30: 2062 6520 7265 6275 696c 7420 6561 6368   be rebuilt each
+00019b40: 2074 696d 6520 0a20 2020 2020 2020 2023   time .        #
+00019b50: 7468 6520 7370 702e 5f67 6574 5f6d 6174  the spp._get_mat
+00019b60: 696e 675f 7061 6972 7328 2920 6d65 7468  ing_pairs() meth
+00019b70: 6f64 2069 7320 6361 6c6c 6564 210a 2020  od is called!.  
+00019b80: 2020 2020 2020 7365 6c66 2e5f 7365 745f        self._set_
+00019b90: 6b64 5f74 7265 6528 290a 0a20 2020 2020  kd_tree()..     
+00019ba0: 2020 2023 2069 6620 6d61 7469 6e67 5f72     # if mating_r
+00019bb0: 6164 6975 7320 6973 204e 6f6e 652c 2074  adius is None, t
+00019bc0: 6865 6e20 6a75 7374 2075 7365 2057 7269  hen just use Wri
+00019bd0: 6768 742d 4669 7368 6572 0a20 2020 2020  ght-Fisher.     
+00019be0: 2020 2023 2073 7479 6c65 2070 616e 6d69     # style panmi
+00019bf0: 7869 6120 2864 7261 7720 7769 7468 2072  xia (draw with r
+00019c00: 6570 6c61 6365 6d65 6e74 2061 2073 616d  eplacement a sam
+00019c10: 706c 650a 2020 2020 2020 2020 2320 6f66  ple.        # of
+00019c20: 2073 697a 6520 3d20 4e74 2a62 2c20 7768   size = Nt*b, wh
+00019c30: 6572 6520 4e74 2069 7320 7468 6520 0a20  ere Nt is the . 
+00019c40: 2020 2020 2020 2023 2063 7572 7265 6e74         # current
+00019c50: 2070 6f70 2073 697a 6520 616e 6420 6220   pop size and b 
+00019c60: 6973 2074 6865 2062 6972 7468 2072 6174  is the birth rat
+00019c70: 6520 2869 2e65 2e20 6d61 7469 6e67 2070  e (i.e. mating p
+00019c80: 726f 6261 6269 6c69 7479 293b 0a20 2020  robability);.   
+00019c90: 2020 2020 2023 2074 6861 7420 7361 6d70       # that samp
+00019ca0: 6c65 2072 6570 7265 7365 6e74 7320 616c  le represents al
+00019cb0: 6c20 6d61 7469 6e67 2069 6e64 6976 6964  l mating individ
+00019cc0: 7561 6c73 2c20 616e 6420 6561 6368 206f  uals, and each o
+00019cd0: 6620 7468 6f73 650a 2020 2020 2020 2020  f those.        
+00019ce0: 2320 696e 6469 7669 6475 616c 7320 7261  # individuals ra
+00019cf0: 6e64 6f6d 6c79 2063 686f 6f73 6573 2069  ndomly chooses i
+00019d00: 7473 206d 6174 650a 2020 2020 2020 2020  ts mate.        
+00019d10: 6966 2073 656c 662e 6d61 7469 6e67 5f72  if self.mating_r
+00019d20: 6164 6975 7320 6973 204e 6f6e 653a 0a20  adius is None:. 
+00019d30: 2020 2020 2020 2020 2020 2023 2064 7261             # dra
+00019d40: 7720 6120 6e75 6d62 6572 206f 6620 6d61  w a number of ma
+00019d50: 7469 6e67 2069 6e64 6976 6964 7561 6c73  ting individuals
+00019d60: 2061 7320 6120 6269 6e6f 6d69 616c 2072   as a binomial r
+00019d70: 760a 2020 2020 2020 2020 2020 2020 2320  v.            # 
+00019d80: 7769 7468 206e 756d 2074 7269 616c 7320  with num trials 
+00019d90: 6571 7561 6c20 746f 2070 6f70 2073 697a  equal to pop siz
+00019da0: 6520 616e 6420 7072 6f62 6162 696c 6974  e and probabilit
+00019db0: 7920 6571 7561 6c20 746f 0a20 2020 2020  y equal to.     
+00019dc0: 2020 2020 2020 2023 2074 6865 2073 7065         # the spe
+00019dd0: 6369 6573 2720 6269 7274 6820 7261 7465  cies' birth rate
+00019de0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00019df0: 7365 6c66 2e62 203c 2031 3a0a 2020 2020  self.b < 1:.    
+00019e00: 2020 2020 2020 2020 2020 2020 6e5f 6d61              n_ma
+00019e10: 7465 7320 3d20 6e70 2e72 616e 646f 6d2e  tes = np.random.
+00019e20: 6269 6e6f 6d69 616c 286e 3d6c 656e 2873  binomial(n=len(s
+00019e30: 656c 6629 2c20 703d 7365 6c66 2e62 290a  elf), p=self.b).
+00019e40: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00019e50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00019e60: 2020 6e5f 6d61 7465 7320 3d20 6c65 6e28    n_mates = len(
+00019e70: 7365 6c66 290a 2020 2020 2020 2020 2020  self).          
+00019e80: 2020 7472 6565 5f69 6e64 7320 3d20 7365    tree_inds = se
+00019e90: 6c66 2e5f 6b64 5f74 7265 652e 7472 6565  lf._kd_tree.tree
+00019ea0: 2e69 6e64 6963 6573 0a20 2020 2020 2020  .indices.       
+00019eb0: 2020 2020 2023 2064 7261 7720 322a 6e5f       # draw 2*n_
+00019ec0: 6d61 7465 7320 6d61 7469 6e67 2069 6e64  mates mating ind
+00019ed0: 6976 6964 7561 6c73 2c20 7769 7468 2072  ividuals, with r
+00019ee0: 6570 6c61 6365 6d65 6e74 2028 6173 2069  eplacement (as i
+00019ef0: 6e20 5746 0a20 2020 2020 2020 2020 2020  n WF.           
+00019f00: 2023 206d 6f64 656c 292c 2074 6865 6e20   # model), then 
+00019f10: 666f 6c64 2069 6e74 6f20 616e 206e 5f6d  fold into an n_m
+00019f20: 6174 6573 2078 2032 206d 6174 652d 7061  ates x 2 mate-pa
+00019f30: 6972 7320 6172 7261 790a 2020 2020 2020  irs array.      
+00019f40: 2020 2020 2020 7061 6972 7320 3d20 6e70        pairs = np
+00019f50: 2e72 616e 646f 6d2e 6368 6f69 6365 2874  .random.choice(t
+00019f60: 7265 655f 696e 6473 2c20 7265 706c 6163  ree_inds, replac
+00019f70: 653d 5472 7565 2c0a 2020 2020 2020 2020  e=True,.        
+00019f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f90: 2020 2020 2020 2020 2020 2020 2073 697a               siz
+00019fa0: 653d 6e5f 6d61 7465 732a 3229 2e72 6573  e=n_mates*2).res
+00019fb0: 6861 7065 2828 6e5f 6d61 7465 732c 2032  hape((n_mates, 2
+00019fc0: 2929 0a20 2020 2020 2020 2020 2020 2023  )).            #
+00019fd0: 2067 6574 2072 6964 206f 6620 7365 6c66   get rid of self
+00019fe0: 696e 6720 7061 6972 730a 2020 2020 2020  ing pairs.      
+00019ff0: 2020 2020 2020 7061 6972 7320 3d20 6e70        pairs = np
+0001a000: 2e61 7272 6179 285b 6c69 7374 2870 6169  .array([list(pai
+0001a010: 7229 2066 6f72 2070 6169 7220 696e 206c  r) for pair in l
+0001a020: 6973 7428 0a20 2020 2020 2020 2020 2020  ist(.           
+0001a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a040: 2020 2020 2020 2020 206d 6170 2873 6574           map(set
+0001a050: 2c20 7061 6972 7329 2920 6966 206c 656e  , pairs)) if len
+0001a060: 2870 6169 7229 203d 3d20 325d 290a 2020  (pair) == 2]).  
+0001a070: 2020 2020 2020 2020 2020 7061 6972 7320            pairs 
+0001a080: 3d20 6e70 2e61 7272 6179 2870 6169 7273  = np.array(pairs
+0001a090: 290a 0a20 2020 2020 2020 2023 206f 7468  )..        # oth
+0001a0a0: 6572 7769 7365 2c20 6368 6f6f 7365 206d  erwise, choose m
+0001a0b0: 6174 6573 2075 7369 6e67 206d 6174 696e  ates using matin
+0001a0c0: 6720 7261 6469 7573 0a20 2020 2020 2020  g radius.       
+0001a0d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001a0e0: 2020 2023 6966 206e 6569 6768 626f 7273     #if neighbors
+0001a0f0: 2061 7265 2074 6f20 6265 2066 6f75 6e64   are to be found
+0001a100: 2077 6974 6869 6e20 7468 6520 7370 6563   within the spec
+0001a110: 6965 732c 0a20 2020 2020 2020 2020 2020  ies,.           
+0001a120: 2023 7365 7420 636f 6f72 6473 2074 6f20   #set coords to 
+0001a130: 7365 6c66 2e5f 636f 6f72 6473 2028 6f74  self._coords (ot
+0001a140: 6865 7277 6973 652c 2074 6865 2063 6f6f  herwise, the coo
+0001a150: 7264 7320 746f 0a20 2020 2020 2020 2020  rds to.         
+0001a160: 2020 2023 6669 6e64 206e 6561 7265 7374     #find nearest
+0001a170: 206e 6569 6768 626f 7273 2077 6974 6820   neighbors with 
+0001a180: 7368 6f75 6c64 2068 6176 6520 6265 656e  should have been
+0001a190: 2070 726f 7669 6465 6429 0a20 2020 2020   provided).     
+0001a1a0: 2020 2020 2020 2069 6620 7769 7468 696e         if within
+0001a1b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001a1c0: 2020 636f 6f72 6473 203d 2073 656c 662e    coords = self.
+0001a1d0: 5f63 6f6f 7264 730a 0a20 2020 2020 2020  _coords..       
+0001a1e0: 2020 2020 2023 7175 6572 7920 7468 6520       #query the 
+0001a1f0: 7472 6565 2074 6f20 6765 7420 6d61 7469  tree to get mati
+0001a200: 6e67 2070 6169 7273 0a20 2020 2020 2020  ng pairs.       
+0001a210: 2020 2020 2070 6169 7273 203d 2073 656c       pairs = sel
+0001a220: 662e 5f6b 645f 7472 6565 2e5f 6765 745f  f._kd_tree._get_
+0001a230: 6d61 7469 6e67 5f70 6169 7273 2863 6f6f  mating_pairs(coo
+0001a240: 7264 733d 636f 6f72 6473 2c0a 2020 2020  rds=coords,.    
+0001a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a270: 2020 2020 2020 2020 2020 2020 6469 7374              dist
+0001a280: 3d73 656c 662e 6d61 7469 6e67 5f72 6164  =self.mating_rad
+0001a290: 6975 732c 0a20 2020 2020 2020 2020 2020  ius,.           
+0001a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a2c0: 2020 2020 2063 686f 6f73 655f 6e65 6172       choose_near
+0001a2d0: 6573 743d 6368 6f6f 7365 5f6e 6561 7265  est=choose_neare
+0001a2e0: 7374 2c0a 2020 2020 2020 2020 2020 2020  st,.            
+0001a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a300: 2020 2020 2020 2020 2020 2020 696e 7665              inve
+0001a310: 7273 655f 6469 7374 5f6d 6174 696e 673d  rse_dist_mating=
+0001a320: 696e 7665 7273 655f 6469 7374 5f6d 6174  inverse_dist_mat
+0001a330: 696e 6729 0a0a 2020 2020 2020 2020 2020  ing)..          
+0001a340: 2020 2320 7573 6520 7468 6520 7370 6563    # use the spec
+0001a350: 6965 7327 2062 6972 7468 2072 6174 6520  ies' birth rate 
+0001a360: 746f 2064 6563 6964 6520 2861 7320 6265  to decide (as be
+0001a370: 726e 6f75 6c6c 6920 6472 6177 7329 0a20  rnoulli draws). 
+0001a380: 2020 2020 2020 2020 2020 2023 2077 6865             # whe
+0001a390: 7468 6572 2065 6163 6820 7061 6972 2063  ther each pair c
+0001a3a0: 616e 206d 6174 650a 2020 2020 2020 2020  an mate.        
+0001a3b0: 2020 2020 6361 6e5f 6d61 7465 203d 206e      can_mate = n
+0001a3c0: 702e 626f 6f6c 3828 6e70 2e72 616e 646f  p.bool8(np.rando
+0001a3d0: 6d2e 6269 6e6f 6d69 616c 286e 3d31 2c20  m.binomial(n=1, 
+0001a3e0: 703d 7365 6c66 2e62 2c0a 2020 2020 2020  p=self.b,.      
+0001a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a410: 2020 2020 2020 2020 2020 2020 2073 697a               siz
+0001a420: 653d 7061 6972 732e 7368 6170 655b 305d  e=pairs.shape[0]
+0001a430: 2929 0a20 2020 2020 2020 2020 2020 2070  )).            p
+0001a440: 6169 7273 203d 206e 702e 6174 6c65 6173  airs = np.atleas
+0001a450: 745f 3264 2870 6169 7273 295b 6361 6e5f  t_2d(pairs)[can_
+0001a460: 6d61 7465 2c20 3a5d 0a20 2020 2020 2020  mate, :].       
+0001a470: 2072 6574 7572 6e20 7061 6972 730a 0a0a   return pairs...
+0001a480: 2020 2020 6465 6620 5f6d 616b 655f 6765      def _make_ge
+0001a490: 615f 6466 2873 656c 662c 206c 7972 5f6e  a_df(self, lyr_n
+0001a4a0: 756d 3d31 293a 0a20 2020 2020 2020 2022  um=1):.        "
+0001a4b0: 2222 0a0a 2020 2020 2020 2020 4d61 6b65  ""..        Make
+0001a4c0: 7320 6120 6461 7461 6672 616d 6520 666f  s a dataframe fo
+0001a4d0: 7220 4745 4120 616e 616c 7973 6973 2063  r GEA analysis c
+0001a4e0: 6f6e 7461 696e 696e 6720 6765 6e6f 7479  ontaining genoty
+0001a4f0: 7065 732c 2063 6f6f 7264 696e 6174 6573  pes, coordinates
+0001a500: 2c0a 2020 2020 2020 2020 616e 6420 656e  ,.        and en
+0001a510: 7620 7661 6c75 6573 2066 6f72 2061 6c6c  v values for all
+0001a520: 2069 6e64 6976 6964 7561 6c73 2e0a 0a20   individuals... 
+0001a530: 2020 2020 2020 204e 4f54 453a 2043 7572         NOTE: Cur
+0001a540: 7265 6e74 6c79 206f 6e6c 7920 6163 6365  rently only acce
+0001a550: 7074 7320 6f6e 6520 4c61 6e64 7363 6170  pts one Landscap
+0001a560: 6520 4c61 7965 7220 2869 2e65 2e20 656e  e Layer (i.e. en
+0001a570: 7669 726f 6e6d 656e 7461 6c0a 2020 2020  vironmental.    
+0001a580: 2020 2020 2020 2020 2020 7661 7269 6162            variab
+0001a590: 6c65 290a 0a20 2020 2020 2020 2050 6172  le)..        Par
+0001a5a0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+0001a5b0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0001a5c0: 2020 206c 7972 5f6e 756d 203a 2069 6e74     lyr_num : int
+0001a5d0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+0001a5e0: 206e 756d 6265 7220 6f66 2074 6865 204c   number of the L
+0001a5f0: 616e 6473 6361 7065 204c 6179 6572 2066  andscape Layer f
+0001a600: 726f 6d20 7768 6963 6820 746f 2065 7874  rom which to ext
+0001a610: 7261 6374 0a20 2020 2020 2020 2020 2020  ract.           
+0001a620: 2065 6e76 6972 6f6e 6d65 6e74 616c 2076   environmental v
+0001a630: 616c 7565 732e 2044 6566 6175 6c74 7320  alues. Defaults 
+0001a640: 746f 2031 2e0a 0a20 2020 2020 2020 2052  to 1...        R
+0001a650: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+0001a660: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 206f  ------.        o
+0001a670: 7574 203a 2070 616e 6461 732e 4461 7461  ut : pandas.Data
+0001a680: 4672 616d 650a 2020 2020 2020 2020 2020  Frame.          
+0001a690: 2020 4120 4461 7461 4672 616d 6520 696e    A DataFrame in
+0001a6a0: 2077 6869 6368 2063 6f6c 756d 6e73 2061   which columns a
+0001a6b0: 7265 206c 6f63 6920 616e 6420 726f 7773  re loci and rows
+0001a6c0: 2061 7265 2069 6e64 6976 6964 7561 6c73   are individuals
+0001a6d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001a6e0: 2020 2020 2023 6765 7420 6172 7261 7920       #get array 
+0001a6f0: 6f66 205b 307c 302e 357c 315d 2067 656e  of [0|0.5|1] gen
+0001a700: 6f74 7970 6573 0a20 2020 2020 2020 2022  otypes.        "
+0001a710: 2222 0a20 2020 2020 2020 2067 656e 203d  "".        gen =
+0001a720: 2073 656c 662e 5f67 6574 5f67 656e 6f74   self._get_genot
+0001a730: 7970 6573 2829 0a0a 2020 2020 2020 2020  ypes()..        
+0001a740: 236c 6f6f 7020 746f 2063 6f6e 7665 7274  #loop to convert
+0001a750: 2062 696e 6172 7920 616c 6c65 6c65 2067   binary allele g
+0001a760: 656e 6f74 7970 6573 2028 307c 3129 0a20  enotypes (0|1). 
+0001a770: 2020 2020 2020 2023 696e 746f 2073 696e         #into sin
+0001a780: 676c 6520 6469 6769 7420 6765 6e6f 7479  gle digit genoty
+0001a790: 7065 7320 2830 2c20 302e 352c 2031 290a  pes (0, 0.5, 1).
+0001a7a0: 2020 2020 2020 2020 6765 6e6f 5f69 6e64          geno_ind
+0001a7b0: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
+0001a7c0: 7220 696e 6420 696e 2072 616e 6765 286c  r ind in range(l
+0001a7d0: 656e 2867 656e 2929 3a0a 2020 2020 2020  en(gen)):.      
+0001a7e0: 2020 2020 2020 6765 6e6f 5f6c 6f63 203d        geno_loc =
+0001a7f0: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
+0001a800: 666f 7220 6c6f 6369 2069 6e20 7261 6e67  for loci in rang
+0001a810: 6528 6c65 6e28 6765 6e5b 696e 645d 2929  e(len(gen[ind]))
+0001a820: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001a830: 2020 6765 6e6f 7479 7065 203d 2067 656e    genotype = gen
+0001a840: 5b69 6e64 5d5b 6c6f 6369 5d2e 6d65 616e  [ind][loci].mean
+0001a850: 2829 2023 2063 6f64 6564 2061 7320 302f  () # coded as 0/
+0001a860: 302e 352f 310a 2020 2020 2020 2020 2020  0.5/1.          
+0001a870: 2020 2020 2020 6765 6e6f 5f6c 6f63 2e61        geno_loc.a
+0001a880: 7070 656e 6428 6765 6e6f 7479 7065 290a  ppend(genotype).
+0001a890: 2020 2020 2020 2020 2020 2020 6765 6e6f              geno
+0001a8a0: 5f69 6e64 2e61 7070 656e 6428 6765 6e6f  _ind.append(geno
+0001a8b0: 5f6c 6f63 290a 2020 2020 2020 2020 2222  _loc).        ""
+0001a8c0: 220a 2020 2020 2020 2020 6774 7320 3d20  ".        gts = 
+0001a8d0: 7365 6c66 2e5f 6765 745f 6765 6e6f 7479  self._get_genoty
+0001a8e0: 7065 7328 6269 616c 6c65 6c69 633d 4661  pes(biallelic=Fa
+0001a8f0: 6c73 6529 0a0a 2020 2020 2020 2020 2363  lse)..        #c
+0001a900: 6f6e 7665 7274 2074 6f20 6461 7461 6672  onvert to datafr
+0001a910: 616d 650a 2020 2020 2020 2020 6765 615f  ame.        gea_
+0001a920: 6466 203d 2070 642e 4461 7461 4672 616d  df = pd.DataFram
+0001a930: 6528 6774 7329 0a0a 2020 2020 2020 2020  e(gts)..        
+0001a940: 2367 6574 2065 6e76 6972 6f6e 6d65 6e74  #get environment
+0001a950: 616c 2064 6174 610a 2020 2020 2020 2020  al data.        
+0001a960: 656e 7620 3d20 7365 6c66 2e5f 6765 745f  env = self._get_
+0001a970: 6528 290a 2020 2020 2020 2020 6765 615f  e().        gea_
+0001a980: 6466 5b27 656e 7627 5d20 3d20 6c69 7374  df['env'] = list
+0001a990: 2865 6e76 5b3a 2c6c 7972 5f6e 756d 5d29  (env[:,lyr_num])
+0001a9a0: 0a0a 2020 2020 2020 2020 2367 6574 2063  ..        #get c
+0001a9b0: 6f6f 7264 730a 2020 2020 2020 2020 636f  oords.        co
+0001a9c0: 6f72 6420 3d20 7365 6c66 2e5f 6765 745f  ord = self._get_
+0001a9d0: 636f 6f72 6473 2829 0a20 2020 2020 2020  coords().       
+0001a9e0: 2067 6561 5f64 665b 276c 6174 275d 203d   gea_df['lat'] =
+0001a9f0: 206c 6973 7428 636f 6f72 645b 3a2c 305d   list(coord[:,0]
+0001aa00: 290a 2020 2020 2020 2020 6765 615f 6466  ).        gea_df
+0001aa10: 5b27 6c6f 6e67 275d 203d 206c 6973 7428  ['long'] = list(
+0001aa20: 636f 6f72 645b 3a2c 315d 290a 0a20 2020  coord[:,1])..   
+0001aa30: 2020 2020 2072 6574 7572 6e20 6765 615f       return gea_
+0001aa40: 6466 0a0a 0a20 2020 2064 6566 205f 7275  df...    def _ru
+0001aa50: 6e5f 6363 6128 7365 6c66 2c20 7472 745f  n_cca(self, trt_
+0001aa60: 6e75 6d3d 302c 2073 6361 6c65 3d54 7275  num=0, scale=Tru
+0001aa70: 652c 2070 6c6f 743d 5472 7565 2c20 706c  e, plot=True, pl
+0001aa80: 6f74 5f73 643d 5472 7565 2c0a 2020 2020  ot_sd=True,.    
+0001aa90: 2020 2020 2020 2020 2020 2020 2073 643d               sd=
+0001aaa0: 3329 3a0a 2020 2020 2020 2020 2222 220a  3):.        """.
+0001aab0: 2020 2020 2020 2020 5275 6e73 2061 2063          Runs a c
+0001aac0: 616e 6f6e 6963 616c 2063 6f72 7265 6c61  anonical correla
+0001aad0: 7469 6f6e 2061 6e61 6c79 7369 7320 2843  tion analysis (C
+0001aae0: 4341 2920 6f6e 2074 6865 2063 7572 7265  CA) on the curre
+0001aaf0: 6e74 2067 656e 6574 6963 2061 6e64 0a20  nt genetic and. 
+0001ab00: 2020 2020 2020 2065 6e76 6972 6f6e 6d65         environme
+0001ab10: 6e74 616c 2064 6174 6120 666f 7220 7468  ntal data for th
+0001ab20: 6520 5370 6563 6965 7327 2063 7572 7265  e Species' curre
+0001ab30: 6e74 2070 6f70 756c 6174 696f 6e2c 2075  nt population, u
+0001ab40: 7369 6e67 2074 6865 0a20 2020 2020 2020  sing the.       
+0001ab50: 2069 6e64 6963 6174 6564 2054 7261 6974   indicated Trait
+0001ab60: 2e20 506c 6f74 7320 7468 6520 7265 7375  . Plots the resu
+0001ab70: 6c74 7320 616e 6420 7265 7475 726e 7320  lts and returns 
+0001ab80: 7468 656d 2069 6e20 6120 6469 6374 2e0a  them in a dict..
+0001ab90: 0a20 2020 2020 2020 2043 4341 206d 6f64  .        CCA mod
+0001aba0: 656c 2066 6f72 6d75 6c61 3a20 6765 6e6f  el formula: geno
+0001abb0: 7479 7065 207e 2065 6e76 202b 206c 6174  type ~ env + lat
+0001abc0: 202b 206c 6f6e 670a 0a20 2020 2020 2020   + long..       
+0001abd0: 204e 4f54 453a 2063 7572 7265 6e74 6c79   NOTE: currently
+0001abe0: 206f 6e6c 7920 706f 7373 6962 6c65 2074   only possible t
+0001abf0: 6f20 646f 2033 2063 6f6d 706f 6e65 6e74  o do 3 component
+0001ac00: 732f 3320 7661 7269 6162 6c65 733b 0a20  s/3 variables;. 
+0001ac10: 2020 2020 2020 2020 2020 2020 2077 696c               wil
+0001ac20: 6c20 6164 6420 6772 6561 7465 7220 6675  l add greater fu
+0001ac30: 6e63 7469 6f6e 616c 6974 7920 696e 2074  nctionality in t
+0001ac40: 6865 2066 7574 7572 650a 0a20 2020 2020  he future..     
+0001ac50: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0001ac60: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+0001ac70: 0a20 2020 2020 2020 2074 7274 5f6e 756d  .        trt_num
+0001ac80: 203a 2069 6e74 0a20 2020 2020 2020 2020   : int.         
+0001ac90: 2020 2054 6865 206e 756d 6265 7220 6f66     The number of
+0001aca0: 2074 6865 2054 7261 6974 2074 6f20 7275   the Trait to ru
+0001acb0: 6e20 7468 6520 4745 4120 6f6e 2e20 4465  n the GEA on. De
+0001acc0: 6661 756c 7473 2074 6f20 302e 0a20 2020  faults to 0..   
+0001acd0: 2020 2020 2073 6361 6c65 203a 2062 6f6f       scale : boo
+0001ace0: 6c0a 2020 2020 2020 2020 2020 2020 4966  l.            If
+0001acf0: 2054 7275 652c 2073 6361 6c65 7320 7468   True, scales th
+0001ad00: 6520 7661 7269 6162 6c65 2c20 696e 6469  e variable, indi
+0001ad10: 7669 6475 616c 2c0a 2020 2020 2020 2020  vidual,.        
+0001ad20: 2020 2020 616e 6420 6c6f 6375 7320 6c6f      and locus lo
+0001ad30: 6164 696e 6773 2066 726f 6d20 2d31 2074  adings from -1 t
+0001ad40: 6f20 3120 746f 206d 616b 6520 7468 656d  o 1 to make them
+0001ad50: 2065 6173 6965 720a 2020 2020 2020 2020   easier.        
+0001ad60: 2020 2020 746f 2076 6973 7561 6c69 7a65      to visualize
+0001ad70: 2e20 4465 6661 756c 7473 2074 6f20 5472  . Defaults to Tr
+0001ad80: 7565 2e0a 2020 2020 2020 2020 706c 6f74  ue..        plot
+0001ad90: 203a 2062 6f6f 6c0a 2020 2020 2020 2020   : bool.        
+0001ada0: 2020 2020 5768 6574 6865 7220 6f72 206e      Whether or n
+0001adb0: 6f74 2074 6f20 706c 6f74 2074 6865 206d  ot to plot the m
+0001adc0: 6f64 656c 2e20 4465 6661 756c 7473 2074  odel. Defaults t
+0001add0: 6f20 5472 7565 2e0a 2020 2020 2020 2020  o True..        
+0001ade0: 706c 6f74 5f73 6420 3a20 626f 6f6c 0a20  plot_sd : bool. 
+0001adf0: 2020 2020 2020 2020 2020 2049 6620 5472             If Tr
+0001ae00: 7565 2c20 6120 7374 616e 6461 7264 2064  ue, a standard d
+0001ae10: 6576 6961 7469 6f6e 2065 6c6c 6970 7365  eviation ellipse
+0001ae20: 2069 7320 706c 6f74 7465 642c 2075 7369   is plotted, usi
+0001ae30: 6e67 2074 6865 206e 756d 6265 720a 2020  ng the number.  
+0001ae40: 2020 2020 2020 2020 2020 6f66 2073 7461            of sta
+0001ae50: 6e64 6172 6420 6465 7669 6174 696f 6e73  ndard deviations
+0001ae60: 2069 6e64 6963 6174 6564 2062 7920 7468   indicated by th
+0001ae70: 6520 6172 6775 6d65 6e74 2027 7364 272e  e argument 'sd'.
+0001ae80: 2044 6566 6175 6c74 7320 746f 0a20 2020   Defaults to.   
+0001ae90: 2020 2020 2020 2020 2054 7275 652e 0a20           True.. 
+0001aea0: 2020 2020 2020 2073 6420 3a20 7b69 6e74         sd : {int
+0001aeb0: 2c20 666c 6f61 747d 0a20 2020 2020 2020  , float}.       
+0001aec0: 2020 2020 204e 756d 6265 7220 6f66 2073       Number of s
+0001aed0: 7461 6e64 6172 6420 6465 7669 6174 696f  tandard deviatio
+0001aee0: 6e73 2074 6f20 7573 6520 666f 7220 706c  ns to use for pl
+0001aef0: 6f74 7469 6e67 2074 6865 2073 7461 6e64  otting the stand
+0001af00: 6172 640a 2020 2020 2020 2020 2020 2020  ard.            
+0001af10: 6465 7669 6174 696f 6e20 656c 6c69 7073  deviation ellips
+0001af20: 652e 2044 6566 6175 6c74 7320 746f 2033  e. Defaults to 3
+0001af30: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0001af40: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+0001af50: 2d2d 0a20 2020 2020 2020 206f 7574 203a  --.        out :
+0001af60: 2064 6963 740a 2020 2020 2020 2020 2020   dict.          
+0001af70: 2020 4120 6469 6374 206f 6620 7468 6520    A dict of the 
+0001af80: 666f 6c6c 6f77 696e 6720 6b65 792d 7661  following key-va
+0001af90: 6c75 6520 7061 6972 733a 0a20 2020 2020  lue pairs:.     
+0001afa0: 2020 2020 2020 2020 2020 2022 6765 615f             "gea_
+0001afb0: 6466 223a 2061 2044 6174 6146 7261 6d65  df": a DataFrame
+0001afc0: 206f 6620 696e 6469 7669 6475 616c 7327   of individuals'
+0001afd0: 2067 656e 6f74 7970 6573 2c20 656e 7669   genotypes, envi
+0001afe0: 726f 6e6d 656e 7461 6c0a 2020 2020 2020  ronmental.      
+0001aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b000: 2020 2020 7661 6c75 6573 2c20 616e 6420      values, and 
+0001b010: 636f 6f72 6469 6e61 7465 730a 2020 2020  coordinates.    
+0001b020: 2020 2020 2020 2020 2020 2020 2269 6e64              "ind
+0001b030: 5f43 4341 6466 223a 2069 6e64 6976 6964  _CCAdf": individ
+0001b040: 7561 6c20 6c6f 6164 696e 6773 2028 636f  ual loadings (co
+0001b050: 6c75 6d6e 7320 3d20 6178 6573 2c0a 2020  lumns = axes,.  
+0001b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b070: 2020 2020 2020 2020 2020 2072 6f77 7320             rows 
+0001b080: 3d20 696e 6469 7669 6475 616c 7329 0a20  = individuals). 
+0001b090: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001b0a0: 6c6f 6369 5f43 4341 6466 223a 206c 6f63  loci_CCAdf": loc
+0001b0b0: 7573 206c 6f61 6469 6e67 7320 2863 6f6c  us loadings (col
+0001b0c0: 756d 6e73 203d 2061 7865 732c 2072 6f77  umns = axes, row
+0001b0d0: 7320 3d20 6c6f 6369 290a 2020 2020 2020  s = loci).      
+0001b0e0: 2020 2020 2020 2020 2020 2276 6172 5f43            "var_C
+0001b0f0: 4341 6466 223a 2076 6172 6961 626c 6520  CAdf": variable 
+0001b100: 6c6f 6164 696e 6773 2028 636f 6c75 6d6e  loadings (column
+0001b110: 7320 3d20 6178 6573 2c0a 2020 2020 2020  s = axes,.      
+0001b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b130: 2020 2020 2020 2072 6f77 7320 3d20 7661         rows = va
+0001b140: 7269 6162 6c65 2028 656e 762c 206c 6174  riable (env, lat
+0001b150: 2c20 6c6f 6e67 2929 0a20 2020 2020 2020  , long)).       
+0001b160: 2020 2020 2020 2020 2022 7472 6169 745f           "trait_
+0001b170: 6c6f 6369 223a 206c 6973 7420 6f66 2069  loci": list of i
+0001b180: 6e64 6578 6573 2066 6f72 206c 6f63 6920  ndexes for loci 
+0001b190: 7468 6174 2075 6e64 6572 6c69 6520 7468  that underlie th
+0001b1a0: 6520 7472 6169 740a 2020 2020 2020 2020  e trait.        
+0001b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b1c0: 2020 2020 2020 666f 7220 7768 6963 6820        for which 
+0001b1d0: 7468 6520 4343 4120 7761 7320 7275 6e0a  the CCA was run.
+0001b1e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001b1f0: 2020 2020 236d 616b 6520 4446 0a20 2020      #make DF.   
+0001b200: 2020 2020 2067 6561 5f64 6620 3d73 656c       gea_df =sel
+0001b210: 662e 5f6d 616b 655f 6765 615f 6466 286c  f._make_gea_df(l
+0001b220: 7972 5f6e 756d 3d73 656c 662e 6765 6e5f  yr_num=self.gen_
+0001b230: 6172 6368 2e74 7261 6974 735b 7472 745f  arch.traits[trt_
+0001b240: 6e75 6d5d 2e6c 7972 5f6e 756d 290a 0a20  num].lyr_num).. 
+0001b250: 2020 2020 2020 2023 6765 7420 6164 6170         #get adap
+0001b260: 7469 7665 206c 6f63 6920 2875 7365 6420  tive loci (used 
+0001b270: 6c61 7465 7220 696e 2070 6c6f 7474 696e  later in plottin
+0001b280: 6729 0a20 2020 2020 2020 2074 7261 6974  g).        trait
+0001b290: 5f6c 6f63 6920 3d20 7365 6c66 2e67 656e  _loci = self.gen
+0001b2a0: 5f61 7263 682e 7472 6169 7473 5b74 7274  _arch.traits[trt
+0001b2b0: 5f6e 756d 5d2e 6c6f 6369 2023 6765 7473  _num].loci #gets
+0001b2c0: 2074 7261 6974 206c 6f63 6920 696e 6465   trait loci inde
+0001b2d0: 7865 730a 0a20 2020 2020 2020 2023 6765  xes..        #ge
+0001b2e0: 7420 6e75 6d62 6572 206f 6620 6c6f 6369  t number of loci
+0001b2f0: 0a20 2020 2020 2020 204c 203d 2073 656c  .        L = sel
+0001b300: 662e 6765 6e5f 6172 6368 2e4c 0a20 2020  f.gen_arch.L.   
+0001b310: 2020 2020 2023 6465 6669 6e65 2078 2061       #define x a
+0001b320: 6e64 2079 3a0a 2020 2020 2020 2020 2320  nd y:.        # 
+0001b330: 7075 6c6c 206f 7574 2067 656e 6f74 7970  pull out genotyp
+0001b340: 6573 0a20 2020 2020 2020 2059 203d 2067  es.        Y = g
+0001b350: 6561 5f64 662e 696c 6f63 5b3a 2c72 616e  ea_df.iloc[:,ran
+0001b360: 6765 284c 295d 0a20 2020 2020 2020 2023  ge(L)].        #
+0001b370: 2070 756c 6c20 6f75 7420 7072 6564 6963   pull out predic
+0001b380: 746f 7220 7661 7269 6162 6c65 730a 2020  tor variables.  
+0001b390: 2020 2020 2020 2320 544f 444f 3a20 6d61        # TODO: ma
+0001b3a0: 6b65 2069 7420 706f 7373 6962 6c65 2074  ke it possible t
+0001b3b0: 6f20 6368 6f6f 7365 206d 6f72 6520 7661  o choose more va
+0001b3c0: 7273 2069 6e20 6675 7475 7265 0a20 2020  rs in future.   
+0001b3d0: 2020 2020 2058 203d 2067 6561 5f64 665b       X = gea_df[
+0001b3e0: 5b27 656e 7627 2c27 6c61 7427 2c27 6c6f  ['env','lat','lo
+0001b3f0: 6e67 275d 5d0a 0a20 2020 2020 2020 2023  ng']]..        #
+0001b400: 6465 6669 6e65 206e 5f63 6f6d 706f 6e65  define n_compone
+0001b410: 6e74 730a 2020 2020 2020 2020 6e5f 636f  nts.        n_co
+0001b420: 6d70 6f6e 656e 7473 203d 2033 0a20 2020  mponents = 3.   
+0001b430: 2020 2020 2023 6372 6561 7465 2074 6865       #create the
+0001b440: 2043 4341 206d 6f64 656c 2061 6e64 2066   CCA model and f
+0001b450: 6974 2069 7420 746f 2074 6865 2064 6174  it it to the dat
+0001b460: 610a 2020 2020 2020 2020 6363 6120 3d20  a.        cca = 
+0001b470: 4343 4128 6e5f 636f 6d70 6f6e 656e 7473  CCA(n_components
+0001b480: 203d 206e 5f63 6f6d 706f 6e65 6e74 7329   = n_components)
+0001b490: 0a20 2020 2020 2020 2063 6361 2e66 6974  .        cca.fit
+0001b4a0: 2859 2c20 5829 0a0a 2020 2020 2020 2020  (Y, X)..        
+0001b4b0: 2374 7261 6e73 666f 726d 2064 6174 610a  #transform data.
+0001b4c0: 2020 2020 2020 2020 595f 6320 3d20 6363          Y_c = cc
+0001b4d0: 612e 7472 616e 7366 6f72 6d28 5929 0a0a  a.transform(Y)..
+0001b4e0: 2020 2020 2020 2020 2363 7265 6174 6520          #create 
+0001b4f0: 6466 2066 6f72 2069 6e64 6976 6964 7561  df for individua
+0001b500: 6c73 0a20 2020 2020 2020 2069 6e64 5f64  ls.        ind_d
+0001b510: 6620 3d20 7064 2e44 6174 6146 7261 6d65  f = pd.DataFrame
+0001b520: 2859 5f63 290a 2020 2020 2020 2020 236e  (Y_c).        #n
+0001b530: 616d 696e 6720 4343 4120 636f 6c75 6d6e  aming CCA column
+0001b540: 7320 7374 6172 7469 6e67 2061 7420 310a  s starting at 1.
+0001b550: 2020 2020 2020 2020 696e 645f 6466 2e63          ind_df.c
+0001b560: 6f6c 756d 6e73 203d 205b 7374 7228 7229  olumns = [str(r)
+0001b570: 2066 6f72 2072 2069 6e20 7261 6e67 6528   for r in range(
+0001b580: 312c 206e 5f63 6f6d 706f 6e65 6e74 7320  1, n_components 
+0001b590: 2b20 3129 5d0a 0a20 2020 2020 2020 2023  + 1)]..        #
+0001b5a0: 6372 6561 7465 2064 6620 666f 7220 6c6f  create df for lo
+0001b5b0: 6369 0a20 2020 2020 2020 206c 6f63 695f  ci.        loci_
+0001b5c0: 6466 203d 2070 642e 4461 7461 4672 616d  df = pd.DataFram
+0001b5d0: 6528 6363 612e 785f 6c6f 6164 696e 6773  e(cca.x_loadings
+0001b5e0: 5f29 0a20 2020 2020 2020 206c 6f63 695f  _).        loci_
+0001b5f0: 6466 2e63 6f6c 756d 6e73 203d 2069 6e64  df.columns = ind
+0001b600: 5f64 662e 636f 6c75 6d6e 7320 2373 616d  _df.columns #sam
+0001b610: 6520 636f 6c75 6d6e 206e 616d 6573 0a0a  e column names..
+0001b620: 2020 2020 2020 2020 2363 7265 6174 6520          #create 
+0001b630: 6466 2066 6f72 2076 6172 6961 626c 6573  df for variables
+0001b640: 0a20 2020 2020 2020 2076 6172 5f64 6620  .        var_df 
+0001b650: 3d20 7064 2e44 6174 6146 7261 6d65 2863  = pd.DataFrame(c
+0001b660: 6361 2e79 5f6c 6f61 6469 6e67 735f 290a  ca.y_loadings_).
+0001b670: 2020 2020 2020 2020 7661 725f 6466 2e63          var_df.c
+0001b680: 6f6c 756d 6e73 203d 2069 6e64 5f64 662e  olumns = ind_df.
+0001b690: 636f 6c75 6d6e 7320 2373 616d 6520 636f  columns #same co
+0001b6a0: 6c75 6d6e 206e 616d 6573 0a0a 2020 2020  lumn names..    
+0001b6b0: 2020 2020 236d 616b 6520 6469 6374 696f      #make dictio
+0001b6c0: 6e61 7279 206f 6620 6461 7461 6672 616d  nary of datafram
+0001b6d0: 6573 2074 6f20 7265 7475 726e 0a20 2020  es to return.   
+0001b6e0: 2020 2020 2063 6361 5f64 6963 7420 3d20       cca_dict = 
+0001b6f0: 7b27 6765 615f 6466 273a 6765 615f 6466  {'gea_df':gea_df
+0001b700: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001b710: 2020 2020 2020 2769 6e64 5f64 6627 3a69        'ind_df':i
+0001b720: 6e64 5f64 662c 0a20 2020 2020 2020 2020  nd_df,.         
+0001b730: 2020 2020 2020 2020 2020 2027 6c6f 6369             'loci
+0001b740: 5f64 6627 3a6c 6f63 695f 6466 2c0a 2020  _df':loci_df,.  
+0001b750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b760: 2020 2776 6172 5f64 6627 3a76 6172 5f64    'var_df':var_d
+0001b770: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+0001b780: 2020 2020 2020 2027 7472 6169 745f 6c6f         'trait_lo
+0001b790: 6369 273a 7472 6169 745f 6c6f 6369 7d0a  ci':trait_loci}.
+0001b7a0: 0a20 2020 2020 2020 2023 204e 4f54 453a  .        # NOTE:
+0001b7b0: 2072 6967 6874 206e 6f77 2074 6869 7320   right now this 
+0001b7c0: 706c 6f74 7469 6e67 206c 6f6f 7020 6f6e  plotting loop on
+0001b7d0: 6c79 2077 6f72 6b73 2066 6f72 2061 206d  ly works for a m
+0001b7e0: 6178 696d 756d 206f 6620 3320 6178 6573  aximum of 3 axes
+0001b7f0: 3b0a 2020 2020 2020 2020 2320 2020 2020  ;.        #     
+0001b800: 2020 696e 2074 6865 2066 7574 7572 6520    in the future 
+0001b810: 6173 206d 6f72 6520 656e 7620 7661 7273  as more env vars
+0001b820: 2061 7265 2061 6464 6564 2c20 636f 756c   are added, coul
+0001b830: 6420 6164 6420 6d6f 7265 2061 7865 730a  d add more axes.
+0001b840: 2020 2020 2020 2020 6966 2070 6c6f 743a          if plot:
+0001b850: 0a20 2020 2020 2020 2020 2020 2023 5363  .            #Sc
+0001b860: 616c 6520 6461 7461 6672 616d 6573 2066  ale dataframes f
+0001b870: 726f 6d20 2d31 2074 6f20 3120 6966 2073  rom -1 to 1 if s
+0001b880: 6361 6c65 203d 2054 7275 650a 2020 2020  cale = True.    
+0001b890: 2020 2020 2020 2020 6966 2073 6361 6c65          if scale
+0001b8a0: 203d 3d20 5472 7565 3a0a 2020 2020 2020   == True:.      
+0001b8b0: 2020 2020 2020 2020 2020 726d 696e 203d            rmin =
+0001b8c0: 202d 310a 2020 2020 2020 2020 2020 2020   -1.            
+0001b8d0: 2020 2020 726d 6178 203d 2031 0a20 2020      rmax = 1.   
+0001b8e0: 2020 2020 2020 2020 2020 2020 206c 6f63               loc
+0001b8f0: 695f 6466 203d 2072 6d69 6e20 2b20 286c  i_df = rmin + (l
+0001b900: 6f63 695f 6466 202d 206c 6f63 695f 6466  oci_df - loci_df
+0001b910: 2e76 616c 7565 732e 6d69 6e28 2929 202a  .values.min()) *
+0001b920: 2028 726d 6178 202d 0a20 2020 2020 2020   (rmax -.       
+0001b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b940: 2028 726d 696e 2929 202f 2028 6c6f 6369   (rmin)) / (loci
+0001b950: 5f64 662e 7661 6c75 6573 2e6d 6178 2829  _df.values.max()
+0001b960: 202d 206c 6f63 695f 6466 2e76 616c 7565   - loci_df.value
+0001b970: 732e 6d69 6e28 2929 0a20 2020 2020 2020  s.min()).       
+0001b980: 2020 2020 2020 2020 2076 6172 5f64 6620           var_df 
+0001b990: 3d20 726d 696e 202b 2028 7661 725f 6466  = rmin + (var_df
+0001b9a0: 202d 2076 6172 5f64 662e 7661 6c75 6573   - var_df.values
+0001b9b0: 2e6d 696e 2829 2920 2a20 2872 6d61 7820  .min()) * (rmax 
+0001b9c0: 2d0a 2020 2020 2020 2020 2020 2020 2020  -.              
+0001b9d0: 2020 2020 2020 2020 2020 2872 6d69 6e29            (rmin)
+0001b9e0: 2920 2f20 2876 6172 5f64 662e 7661 6c75  ) / (var_df.valu
+0001b9f0: 6573 2e6d 6178 2829 202d 2076 6172 5f64  es.max() - var_d
+0001ba00: 662e 7661 6c75 6573 2e6d 696e 2829 290a  f.values.min()).
+0001ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ba20: 696e 645f 6466 203d 2072 6d69 6e20 2b20  ind_df = rmin + 
+0001ba30: 2869 6e64 5f64 6620 2d20 696e 645f 6466  (ind_df - ind_df
+0001ba40: 2e76 616c 7565 732e 6d69 6e28 2929 202a  .values.min()) *
+0001ba50: 2028 726d 6178 202d 0a20 2020 2020 2020   (rmax -.       
+0001ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ba70: 2028 726d 696e 2929 202f 2028 696e 645f   (rmin)) / (ind_
+0001ba80: 6466 2e76 616c 7565 732e 6d61 7828 2920  df.values.max() 
+0001ba90: 2d20 696e 645f 6466 2e76 616c 7565 732e  - ind_df.values.
+0001baa0: 6d69 6e28 2929 0a0a 0a20 2020 2020 2020  min())...       
+0001bab0: 2020 2020 2023 6765 7420 6d61 7820 616e       #get max an
+0001bac0: 6420 6d69 6e73 2074 6f20 7365 7420 6178  d mins to set ax
+0001bad0: 6973 206c 6174 6572 206f 6e0a 2020 2020  is later on.    
+0001bae0: 2020 2020 2020 2020 6d61 7864 6620 3d20          maxdf = 
+0001baf0: 6d61 7828 696e 645f 6466 2e76 616c 7565  max(ind_df.value
+0001bb00: 732e 6d61 7828 292c 2076 6172 5f64 662e  s.max(), var_df.
+0001bb10: 7661 6c75 6573 2e6d 6178 2829 2c0a 2020  values.max(),.  
+0001bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb30: 2020 2020 2020 6c6f 6369 5f64 662e 7661        loci_df.va
+0001bb40: 6c75 6573 2e6d 6178 2829 290a 2020 2020  lues.max()).    
+0001bb50: 2020 2020 2020 2020 6d69 6e64 6620 3d20          mindf = 
+0001bb60: 6162 7328 6d69 6e28 696e 645f 6466 2e76  abs(min(ind_df.v
+0001bb70: 616c 7565 732e 6d69 6e28 292c 2076 6172  alues.min(), var
+0001bb80: 5f64 662e 7661 6c75 6573 2e6d 696e 2829  _df.values.min()
+0001bb90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001bba0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0001bbb0: 6369 5f64 662e 7661 6c75 6573 2e6d 696e  ci_df.values.min
+0001bbc0: 2829 2929 0a20 2020 2020 2020 2020 2020  ())).           
+0001bbd0: 2061 786d 6178 203d 206d 6178 286d 6178   axmax = max(max
+0001bbe0: 6466 2c20 6d69 6e64 6629 202a 2031 2e32  df, mindf) * 1.2
+0001bbf0: 3020 2361 6464 696e 6720 6120 3230 2520  0 #adding a 20% 
+0001bc00: 6275 6666 6572 0a0a 2020 2020 2020 2020  buffer..        
+0001bc10: 2020 2020 2373 6574 2075 7020 6669 6775      #set up figu
+0001bc20: 7265 0a20 2020 2020 2020 2020 2020 2066  re.            f
+0001bc30: 6967 203d 2070 6c74 2e66 6967 7572 6528  ig = plt.figure(
+0001bc40: 6669 6773 697a 653d 2832 302c 2031 3529  figsize=(20, 15)
+0001bc50: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0001bc60: 7220 6e2c 2063 635f 6178 6573 5f70 6169  r n, cc_axes_pai
+0001bc70: 7220 696e 2065 6e75 6d65 7261 7465 285b  r in enumerate([
+0001bc80: 5b31 2c20 325d 2c20 5b31 2c20 335d 2c20  [1, 2], [1, 3], 
+0001bc90: 5b32 2c20 335d 5d29 3a0a 2020 2020 2020  [2, 3]]):.      
+0001bca0: 2020 2020 2020 2020 2020 2364 6566 696e            #defin
+0001bcb0: 6520 636f 6d70 6f6e 656e 7473 2066 6f72  e components for
+0001bcc0: 2061 7869 730a 2020 2020 2020 2020 2020   axis.          
+0001bcd0: 2020 2020 2020 6363 5f61 7869 7331 203d        cc_axis1 =
+0001bce0: 2063 635f 6178 6573 5f70 6169 725b 305d   cc_axes_pair[0]
+0001bcf0: 2023 782d 6178 6973 2043 430a 2020 2020   #x-axis CC.    
+0001bd00: 2020 2020 2020 2020 2020 2020 6363 5f61              cc_a
+0001bd10: 7869 7332 203d 2063 635f 6178 6573 5f70  xis2 = cc_axes_p
+0001bd20: 6169 725b 315d 2023 792d 6178 6973 2043  air[1] #y-axis C
+0001bd30: 430a 0a20 2020 2020 2020 2020 2020 2020  C..             
+0001bd40: 2020 2061 7820 3d20 6669 672e 6164 645f     ax = fig.add_
+0001bd50: 7375 6270 6c6f 7428 3133 312b 6e29 0a0a  subplot(131+n)..
+0001bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bd70: 2361 6464 2063 656e 7465 7220 6c69 6e65  #add center line
+0001bd80: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0001bd90: 2020 6178 2e61 7868 6c69 6e65 2879 3d30    ax.axhline(y=0
+0001bda0: 2c20 636f 6c6f 723d 276c 6967 6874 6772  , color='lightgr
+0001bdb0: 6179 272c 206c 696e 6573 7479 6c65 3d27  ay', linestyle='
+0001bdc0: 646f 7474 6564 2729 0a20 2020 2020 2020  dotted').       
+0001bdd0: 2020 2020 2020 2020 2061 782e 6178 766c           ax.axvl
+0001bde0: 696e 6528 783d 302c 2063 6f6c 6f72 3d27  ine(x=0, color='
+0001bdf0: 6c69 6768 7467 7261 7927 2c20 6c69 6e65  lightgray', line
+0001be00: 7374 796c 653d 2764 6f74 7465 6427 290a  style='dotted').
+0001be10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001be20: 2023 2073 6574 2061 7865 7320 7261 6e67   # set axes rang
+0001be30: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0001be40: 2020 706c 742e 786c 696d 282d 6178 6d61    plt.xlim(-axma
+0001be50: 782c 2061 786d 6178 290a 2020 2020 2020  x, axmax).      
+0001be60: 2020 2020 2020 2020 2020 706c 742e 796c            plt.yl
+0001be70: 696d 282d 6178 6d61 782c 2061 786d 6178  im(-axmax, axmax
+0001be80: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001be90: 2020 2023 706c 6f74 206e 6575 7472 616c     #plot neutral
+0001bea0: 2053 4e50 730a 2020 2020 2020 2020 2020   SNPs.          
+0001beb0: 2020 2020 2020 6178 2e73 6361 7474 6572        ax.scatter
+0001bec0: 286c 6f63 695f 6466 5b73 7472 2863 635f  (loci_df[str(cc_
+0001bed0: 6178 6973 3129 5d2c 206c 6f63 695f 6466  axis1)], loci_df
+0001bee0: 5b73 7472 2863 635f 6178 6973 3229 5d2c  [str(cc_axis2)],
+0001bef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bf00: 2020 2020 2020 2020 2020 2020 6d61 726b              mark
+0001bf10: 6572 203d 2027 2b27 2c20 636f 6c6f 7220  er = '+', color 
+0001bf20: 3d20 2767 7261 7927 2c0a 2020 2020 2020  = 'gray',.      
+0001bf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf40: 2020 2020 206c 6162 656c 203d 2027 4e65       label = 'Ne
+0001bf50: 7574 7261 6c20 534e 5073 272c 2061 6c70  utral SNPs', alp
+0001bf60: 6861 203d 2030 2e37 290a 2020 2020 2020  ha = 0.7).      
+0001bf70: 2020 2020 2020 2020 2020 2370 6c6f 7420            #plot 
+0001bf80: 696e 6469 7669 6475 616c 730a 2020 2020  individuals.    
+0001bf90: 2020 2020 2020 2020 2020 2020 636d 6170              cmap
+0001bfa0: 5f73 6361 7420 3d20 6178 2e73 6361 7474  _scat = ax.scatt
+0001bfb0: 6572 2869 6e64 5f64 665b 7374 7228 6363  er(ind_df[str(cc
+0001bfc0: 5f61 7869 7331 295d 2c0a 2020 2020 2020  _axis1)],.      
+0001bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bff0: 2069 6e64 5f64 665b 7374 7228 6363 5f61   ind_df[str(cc_a
+0001c000: 7869 7332 295d 2c0a 2020 2020 2020 2020  xis2)],.        
+0001c010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c020: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001c030: 203d 2067 6561 5f64 662e 656e 762c 2063   = gea_df.env, c
+0001c040: 6d61 703d 2776 6972 6964 6973 272c 0a20  map='viridis',. 
+0001c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c070: 2020 2020 2020 6c61 6265 6c20 3d20 2249        label = "I
+0001c080: 6e64 6976 6964 7561 6c73 222c 2061 6c70  ndividuals", alp
+0001c090: 6861 203d 2030 2e35 290a 2020 2020 2020  ha = 0.5).      
+0001c0a0: 2020 2020 2020 2020 2020 2370 6c6f 7420            #plot 
+0001c0b0: 6164 6170 7469 7665 2053 4e50 730a 2020  adaptive SNPs.  
+0001c0c0: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+0001c0d0: 2e73 6361 7474 6572 286c 6f63 695f 6466  .scatter(loci_df
+0001c0e0: 5b73 7472 2863 635f 6178 6973 3129 5d5b  [str(cc_axis1)][
+0001c0f0: 7472 6169 745f 6c6f 6369 5d2c 0a20 2020  trait_loci],.   
 0001c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c110: 2020 2020 6966 2028 7820 3c20 3020 616e      if (x < 0 an
-0001c120: 6420 7920 3c20 3029 3a0a 2020 2020 2020  d y < 0):.      
-0001c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c140: 2070 6c74 2e74 6578 7428 7820 2d20 7378   plt.text(x - sx
-0001c150: 2c20 7920 2d20 7379 2c20 582e 636f 6c75  , y - sy, X.colu
-0001c160: 6d6e 735b 695d 290a 2020 2020 2020 2020  mns[i]).        
-0001c170: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-0001c180: 7820 3c20 3020 616e 6420 7920 3e20 3029  x < 0 and y > 0)
-0001c190: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001c1a0: 2020 2020 2020 2020 2070 6c74 2e74 6578           plt.tex
-0001c1b0: 7428 7820 2d20 7378 2c20 7920 2b20 7379  t(x - sx, y + sy
-0001c1c0: 2c20 582e 636f 6c75 6d6e 735b 695d 290a  , X.columns[i]).
-0001c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c1e0: 2020 2020 6966 2028 7820 3e20 3020 616e      if (x > 0 an
-0001c1f0: 6420 7920 3e20 3029 3a0a 2020 2020 2020  d y > 0):.      
-0001c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c210: 2070 6c74 2e74 6578 7428 7820 2b20 7378   plt.text(x + sx
-0001c220: 2c20 7920 2b20 7379 2c20 582e 636f 6c75  , y + sy, X.colu
-0001c230: 6d6e 735b 695d 290a 2020 2020 2020 2020  mns[i]).        
-0001c240: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-0001c250: 7820 3e20 3020 616e 6420 7920 3c20 3029  x > 0 and y < 0)
-0001c260: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001c270: 2020 2020 2020 2020 2070 6c74 2e74 6578           plt.tex
-0001c280: 7428 7820 2b20 7378 2c20 7920 2d20 7379  t(x + sx, y - sy
-0001c290: 2c20 582e 636f 6c75 6d6e 735b 695d 290a  , X.columns[i]).
-0001c2a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c2b0: 2023 706c 6f74 2053 4420 656c 6c69 7073   #plot SD ellips
-0001c2c0: 6520 666f 7220 534e 5020 6461 7461 2069  e for SNP data i
-0001c2d0: 6620 706c 6f74 5f73 6420 3d20 5472 7565  f plot_sd = True
-0001c2e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c2f0: 2069 6620 706c 6f74 5f73 643a 0a20 2020   if plot_sd:.   
-0001c300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c310: 2072 3120 3d20 6e70 2e73 7464 286c 6f63   r1 = np.std(loc
-0001c320: 695f 6466 5b73 7472 2863 635f 6178 6973  i_df[str(cc_axis
-0001c330: 3129 5d29 202a 2073 640a 2020 2020 2020  1)]) * sd.      
-0001c340: 2020 2020 2020 2020 2020 2020 2020 7232                r2
-0001c350: 203d 206e 702e 7374 6428 6c6f 6369 5f64   = np.std(loci_d
-0001c360: 665b 7374 7228 6363 5f61 7869 7332 295d  f[str(cc_axis2)]
-0001c370: 2920 2a20 7364 0a20 2020 2020 2020 2020  ) * sd.         
-0001c380: 2020 2020 2020 2020 2020 2074 203d 206e             t = n
-0001c390: 702e 6c69 6e73 7061 6365 2830 2c20 322a  p.linspace(0, 2*
-0001c3a0: 6d61 7468 5f70 692c 2031 3030 290a 2020  math_pi, 100).  
-0001c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c3c0: 2020 6178 2e70 6c6f 7428 7231 2a6e 702e    ax.plot(r1*np.
-0001c3d0: 636f 7328 7429 202c 2072 322a 6e70 2e73  cos(t) , r2*np.s
-0001c3e0: 696e 2874 292c 206c 696e 6573 7479 6c65  in(t), linestyle
-0001c3f0: 203d 2027 6461 7368 6564 272c 0a20 2020   = 'dashed',.   
+0001c110: 2020 2020 2020 2020 6c6f 6369 5f64 665b          loci_df[
+0001c120: 7374 7228 6363 5f61 7869 7332 295d 5b74  str(cc_axis2)][t
+0001c130: 7261 6974 5f6c 6f63 695d 2c0a 2020 2020  rait_loci],.    
+0001c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c150: 2020 2020 2020 206d 6172 6b65 723d 222b         marker="+
+0001c160: 222c 2063 6f6c 6f72 203d 2022 7265 6422  ", color = "red"
+0001c170: 2c20 733d 3130 302c 0a20 2020 2020 2020  , s=100,.       
+0001c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c190: 2020 2020 6c61 6265 6c20 3d20 2741 6461      label = 'Ada
+0001c1a0: 7074 6976 6520 534e 5073 2729 0a0a 2020  ptive SNPs')..  
+0001c1b0: 2020 2020 2020 2020 2020 2020 2020 2370                #p
+0001c1c0: 6c6f 7420 7661 7269 6162 6c65 2076 6563  lot variable vec
+0001c1d0: 746f 7273 2061 7320 6172 726f 7773 0a20  tors as arrows. 
+0001c1e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001c1f0: 6f72 2069 2069 6e20 7261 6e67 6528 7661  or i in range(va
+0001c200: 725f 6466 2e73 6861 7065 5b30 5d29 3a0a  r_df.shape[0]):.
+0001c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c220: 2020 2020 7820 3d20 7661 725f 6466 5b73      x = var_df[s
+0001c230: 7472 2863 635f 6178 6973 3129 5d5b 695d  tr(cc_axis1)][i]
+0001c240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c250: 2020 2020 2079 203d 2076 6172 5f64 665b       y = var_df[
+0001c260: 7374 7228 6363 5f61 7869 7332 295d 5b69  str(cc_axis2)][i
+0001c270: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0001c280: 2020 2020 2020 706c 742e 6172 726f 7728        plt.arrow(
+0001c290: 302c 2030 2c20 782c 2079 2c20 7769 6474  0, 0, x, y, widt
+0001c2a0: 6820 3d20 302e 3031 2c0a 2020 2020 2020  h = 0.01,.      
+0001c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c2c0: 2020 2020 2020 2020 6865 6164 5f77 6964          head_wid
+0001c2d0: 7468 203d 2030 2e30 352c 2063 6f6c 6f72  th = 0.05, color
+0001c2e0: 203d 2027 626c 6163 6b27 290a 2020 2020   = 'black').    
+0001c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c300: 7378 203d 2030 2e31 0a20 2020 2020 2020  sx = 0.1.       
+0001c310: 2020 2020 2020 2020 2020 2020 2073 7920               sy 
+0001c320: 3d20 302e 310a 2020 2020 2020 2020 2020  = 0.1.          
+0001c330: 2020 2020 2020 2020 2020 2320 7468 6973            # this
+0001c340: 206d 6573 7320 6973 206a 7573 7420 746f   mess is just to
+0001c350: 2061 7272 616e 6765 2074 6865 2074 6578   arrange the tex
+0001c360: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0001c370: 2020 2020 2020 2320 6e65 7874 2074 6f20        # next to 
+0001c380: 6172 726f 7773 2062 7574 2069 7420 6973  arrows but it is
+0001c390: 2061 2057 4950 0a20 2020 2020 2020 2020   a WIP.         
+0001c3a0: 2020 2020 2020 2020 2020 2069 6620 2878             if (x
+0001c3b0: 203c 2030 2061 6e64 2079 203c 2030 293a   < 0 and y < 0):
+0001c3c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c3d0: 2020 2020 2020 2020 706c 742e 7465 7874          plt.text
+0001c3e0: 2878 202d 2073 782c 2079 202d 2073 792c  (x - sx, y - sy,
+0001c3f0: 2058 2e63 6f6c 756d 6e73 5b69 5d29 0a20   X.columns[i]). 
 0001c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c410: 2020 2020 2020 2020 2063 203d 2027 7265           c = 're
-0001c420: 6427 2c20 6c61 6265 6c20 3d20 7374 7228  d', label = str(
-0001c430: 7364 2920 2b20 2220 5374 6444 6576 2229  sd) + " StdDev")
-0001c440: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001c450: 2020 2345 5645 5259 5448 494e 4720 4245    #EVERYTHING BE
-0001c460: 4c4f 5720 5448 4953 204c 494e 4520 494e  LOW THIS LINE IN
-0001c470: 2054 4845 204c 4f4f 5020 4953 204a 5553   THE LOOP IS JUS
-0001c480: 5420 504c 4f54 2046 4f52 4d41 5454 494e  T PLOT FORMATTIN
-0001c490: 4720 0a20 2020 2020 2020 2020 2020 2020  G .             
-0001c4a0: 2020 2023 786c 6162 656c 2069 7320 7468     #xlabel is th
-0001c4b0: 6520 6c61 6265 6c20 6174 2074 6865 2062  e label at the b
-0001c4c0: 6f74 746f 6d20 2876 6572 7469 6361 6c20  ottom (vertical 
-0001c4d0: 6178 6973 206c 6162 656c 290a 2020 2020  axis label).    
-0001c4e0: 2020 2020 2020 2020 2020 2020 2320 616e              # an
-0001c4f0: 6420 796c 6162 656c 2069 7320 6f6e 2074  d ylabel is on t
-0001c500: 6865 206c 6566 7420 7369 6465 2028 686f  he left side (ho
-0001c510: 7269 7a6f 6e74 616c 2061 7869 7320 6c61  rizontal axis la
-0001c520: 6265 6c29 0a20 2020 2020 2020 2020 2020  bel).           
-0001c530: 2020 2020 206c 6162 656c 203d 2061 782e       label = ax.
-0001c540: 7365 745f 786c 6162 656c 2827 4343 4127  set_xlabel('CCA'
-0001c550: 202b 2073 7472 2863 635f 6178 6973 3229   + str(cc_axis2)
-0001c560: 2c20 666f 6e74 7369 7a65 203d 2039 290a  , fontsize = 9).
-0001c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c580: 6178 2e78 6178 6973 2e73 6574 5f6c 6162  ax.xaxis.set_lab
-0001c590: 656c 5f63 6f6f 7264 7328 302e 352c 202d  el_coords(0.5, -
-0001c5a0: 302e 3032 290a 2020 2020 2020 2020 2020  0.02).          
-0001c5b0: 2020 2020 2020 6c61 6265 6c20 3d20 6178        label = ax
-0001c5c0: 2e73 6574 5f79 6c61 6265 6c28 2743 4341  .set_ylabel('CCA
-0001c5d0: 2720 2b20 7374 7228 6363 5f61 7869 7331  ' + str(cc_axis1
-0001c5e0: 292c 2066 6f6e 7473 697a 6520 3d20 3929  ), fontsize = 9)
-0001c5f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c600: 2061 782e 7961 7869 732e 7365 745f 6c61   ax.yaxis.set_la
-0001c610: 6265 6c5f 636f 6f72 6473 282d 302e 3032  bel_coords(-0.02
-0001c620: 2c20 302e 3535 290a 0a20 2020 2020 2020  , 0.55)..       
-0001c630: 2020 2020 2020 2020 2023 6d61 6b65 2069           #make i
-0001c640: 6e74 6f20 626f 780a 2020 2020 2020 2020  nto box.        
-0001c650: 2020 2020 2020 2020 6178 2e73 6574 5f61          ax.set_a
-0001c660: 7370 6563 7428 2765 7175 616c 272c 2061  spect('equal', a
-0001c670: 646a 7573 7461 626c 653d 2762 6f78 2729  djustable='box')
-0001c680: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001c690: 2020 234d 6f76 6520 6c65 6674 2079 2d61    #Move left y-a
-0001c6a0: 7869 7320 2620 626f 7474 6f6d 2078 2d61  xis & bottom x-a
-0001c6b0: 7869 7320 746f 2063 656e 7465 722c 2070  xis to center, p
-0001c6c0: 6173 7369 6e67 2074 6872 7520 2830 2c30  assing thru (0,0
-0001c6d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001c6e0: 2020 6178 2e73 7069 6e65 735b 276c 6566    ax.spines['lef
-0001c6f0: 7427 5d2e 7365 745f 706f 7369 7469 6f6e  t'].set_position
-0001c700: 2827 6365 6e74 6572 2729 0a20 2020 2020  ('center').     
-0001c710: 2020 2020 2020 2020 2020 2061 782e 7370             ax.sp
-0001c720: 696e 6573 5b27 626f 7474 6f6d 275d 2e73  ines['bottom'].s
-0001c730: 6574 5f70 6f73 6974 696f 6e28 2763 656e  et_position('cen
-0001c740: 7465 7227 290a 0a20 2020 2020 2020 2020  ter')..         
-0001c750: 2020 2020 2020 2023 6368 616e 6765 2063         #change c
-0001c760: 6f6c 6f72 732f 7265 6d6f 7665 2064 6566  olors/remove def
-0001c770: 6175 6c74 2061 7869 730a 2020 2020 2020  ault axis.      
-0001c780: 2020 2020 2020 2020 2020 6178 636f 6c6f            axcolo
-0001c790: 7220 3d20 276e 6f6e 6527 0a20 2020 2020  r = 'none'.     
-0001c7a0: 2020 2020 2020 2020 2020 2061 782e 7370             ax.sp
-0001c7b0: 696e 6573 5b27 6c65 6674 275d 2e73 6574  ines['left'].set
-0001c7c0: 5f63 6f6c 6f72 2861 7863 6f6c 6f72 290a  _color(axcolor).
-0001c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c7e0: 6178 2e73 7069 6e65 735b 2762 6f74 746f  ax.spines['botto
-0001c7f0: 6d27 5d2e 7365 745f 636f 6c6f 7228 6178  m'].set_color(ax
-0001c800: 636f 6c6f 7229 0a20 2020 2020 2020 2020  color).         
-0001c810: 2020 2020 2020 2061 782e 7370 696e 6573         ax.spines
-0001c820: 5b27 7269 6768 7427 5d2e 7365 745f 636f  ['right'].set_co
-0001c830: 6c6f 7228 6178 636f 6c6f 7229 0a20 2020  lor(axcolor).   
-0001c840: 2020 2020 2020 2020 2020 2020 2061 782e               ax.
-0001c850: 7370 696e 6573 5b27 746f 7027 5d2e 7365  spines['top'].se
-0001c860: 745f 636f 6c6f 7228 6178 636f 6c6f 7229  t_color(axcolor)
-0001c870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c880: 2061 782e 7469 636b 5f70 6172 616d 7328   ax.tick_params(
-0001c890: 6178 6973 203d 2027 7827 2c20 636f 6c6f  axis = 'x', colo
-0001c8a0: 7273 3d61 7863 6f6c 6f72 290a 2020 2020  rs=axcolor).    
-0001c8b0: 2020 2020 2020 2020 2020 2020 6178 2e74              ax.t
-0001c8c0: 6963 6b5f 7061 7261 6d73 2861 7869 7320  ick_params(axis 
-0001c8d0: 3d20 2779 272c 2063 6f6c 6f72 733d 6178  = 'y', colors=ax
-0001c8e0: 636f 6c6f 7229 0a0a 2020 2020 2020 2020  color)..        
-0001c8f0: 2020 2020 2020 2020 6178 2e79 6178 6973          ax.yaxis
-0001c900: 2e6c 6162 656c 2e73 6574 5f63 6f6c 6f72  .label.set_color
-0001c910: 2827 6772 6179 2729 0a20 2020 2020 2020  ('gray').       
-0001c920: 2020 2020 2020 2020 2061 782e 7861 7869           ax.xaxi
-0001c930: 732e 6c61 6265 6c2e 7365 745f 636f 6c6f  s.label.set_colo
-0001c940: 7228 2767 7261 7927 290a 0a20 2020 2020  r('gray')..     
-0001c950: 2020 2020 2020 2020 2020 2023 6c65 6765             #lege
-0001c960: 6e64 730a 2020 2020 2020 2020 2020 2020  nds.            
-0001c970: 2020 2020 6966 206e 203d 3d20 323a 0a20      if n == 2:. 
-0001c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c990: 2020 2061 782e 6c65 6765 6e64 286c 6f63     ax.legend(loc
-0001c9a0: 203d 2022 7570 7065 7220 6c65 6674 222c   = "upper left",
-0001c9b0: 2062 626f 785f 746f 5f61 6e63 686f 723d   bbox_to_anchor=
-0001c9c0: 2831 2e33 2c20 312e 3035 2929 0a20 2020  (1.3, 1.05)).   
-0001c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c9e0: 2070 6c74 2e63 6f6c 6f72 6261 7228 636d   plt.colorbar(cm
-0001c9f0: 6170 5f73 6361 742c 206c 6162 656c 3d22  ap_scat, label="
-0001ca00: 656e 7622 290a 2020 2020 2020 2020 2020  env").          
-0001ca10: 2020 6669 672e 7368 6f77 2829 0a0a 2020    fig.show()..  
-0001ca20: 2020 2020 2020 7265 7475 726e 2063 6361        return cca
-0001ca30: 5f64 6963 740a 0a0a 2020 2020 2320 6d65  _dict...    # me
-0001ca40: 7468 6f64 2066 6f72 2070 6c6f 7474 696e  thod for plottin
-0001ca50: 6720 7468 6520 7370 6563 6965 7320 286f  g the species (o
-0001ca60: 7220 6120 7375 6273 6574 206f 6620 6974  r a subset of it
-0001ca70: 7320 696e 6469 7669 6475 616c 732c 2062  s individuals, b
-0001ca80: 7920 4944 290a 2020 2020 2320 6f6e 2074  y ID).    # on t
-0001ca90: 6f70 206f 6620 6120 6c61 7965 7220 286f  op of a layer (o
-0001caa0: 7220 6c61 6e64 7363 6170 6529 0a20 2020  r landscape).   
-0001cab0: 2064 6566 205f 706c 6f74 2873 656c 662c   def _plot(self,
-0001cac0: 206c 7972 5f6e 756d 3d4e 6f6e 652c 206c   lyr_num=None, l
-0001cad0: 616e 643d 4e6f 6e65 2c20 6869 6465 5f6c  and=None, hide_l
-0001cae0: 616e 643d 4661 6c73 652c 2069 6e64 6976  and=False, indiv
-0001caf0: 6964 733d 4e6f 6e65 2c0a 2020 2020 2020  ids=None,.      
-0001cb00: 2020 2020 2020 2020 7465 7874 3d46 616c          text=Fal
-0001cb10: 7365 2c20 636f 6c6f 723d 2762 6c61 636b  se, color='black
-0001cb20: 272c 2065 6467 655f 636f 6c6f 723d 2766  ', edge_color='f
-0001cb30: 6163 6527 2c20 7465 7874 5f63 6f6c 6f72  ace', text_color
-0001cb40: 3d27 626c 6163 6b27 2c0a 2020 2020 2020  ='black',.      
-0001cb50: 2020 2020 2020 2020 6362 6172 3d54 7275          cbar=Tru
-0001cb60: 652c 2073 697a 653d 3235 2c20 7465 7874  e, size=25, text
-0001cb70: 5f73 697a 653d 392c 206c 616e 645f 636d  _size=9, land_cm
-0001cb80: 6170 3d4e 6f6e 652c 2070 745f 636d 6170  ap=None, pt_cmap
-0001cb90: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-0001cba0: 2020 2020 2061 6c70 6861 3d46 616c 7365       alpha=False
-0001cbb0: 2c20 7a6f 6f6d 5f77 6964 7468 3d4e 6f6e  , zoom_width=Non
-0001cbc0: 652c 2078 3d4e 6f6e 652c 2079 3d4e 6f6e  e, x=None, y=Non
-0001cbd0: 652c 2076 6d69 6e3d 4e6f 6e65 2c0a 2020  e, vmin=None,.  
-0001cbe0: 2020 2020 2020 2020 2020 2020 766d 6178              vmax
-0001cbf0: 3d4e 6f6e 652c 2074 6963 6b73 3d4e 6f6e  =None, ticks=Non
-0001cc00: 652c 206d 6173 6b5f 7261 7374 3d4e 6f6e  e, mask_rast=Non
-0001cc10: 652c 2061 6e69 6d61 7465 3d46 616c 7365  e, animate=False
-0001cc20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001cc30: 6365 6c6c 5f63 6f6f 7264 733d 4661 6c73  cell_coords=Fals
-0001cc40: 6529 3a0a 2020 2020 2020 2020 2320 636f  e):.        # co
-0001cc50: 6e76 6572 7420 696e 6469 7669 6473 2074  nvert individs t
-0001cc60: 6f20 6120 6c69 7374 2028 696e 2063 6173  o a list (in cas
-0001cc70: 6520 636f 6d65 7320 696e 2061 7320 6120  e comes in as a 
-0001cc80: 6e75 6d70 7920 6172 7261 7929 0a20 2020  numpy array).   
-0001cc90: 2020 2020 2069 6620 696e 6469 7669 6473       if individs
-0001cca0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0001ccb0: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-0001ccc0: 696e 6469 7669 6473 2c20 6c69 7374 293a  individs, list):
-0001ccd0: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
-0001cce0: 6976 6964 7320 3d20 6c69 7374 2869 6e64  ivids = list(ind
-0001ccf0: 6976 6964 7329 0a20 2020 2020 2020 2023  ivids).        #
-0001cd00: 2067 6574 2063 6f6f 7264 730a 2020 2020   get coords.    
-0001cd10: 2020 2020 636f 6f72 6473 203d 2073 656c      coords = sel
-0001cd20: 662e 5f67 6574 5f70 6c6f 745f 636f 6f72  f._get_plot_coor
-0001cd30: 6473 2869 6e64 6976 6964 733d 696e 6469  ds(individs=indi
-0001cd40: 7669 6473 2c0a 2020 2020 2020 2020 2020  vids,.          
-0001cd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd60: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-0001cd70: 6c5f 636f 6f72 6473 3d63 656c 6c5f 636f  l_coords=cell_co
-0001cd80: 6f72 6473 290a 2020 2020 2020 2020 2320  ords).        # 
-0001cd90: 6765 7420 7465 7874 0a20 2020 2020 2020  get text.       
-0001cda0: 2069 6620 7465 7874 3a0a 2020 2020 2020   if text:.      
-0001cdb0: 2020 2020 2020 6966 2069 6e64 6976 6964        if individ
-0001cdc0: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
-0001cdd0: 2020 2020 2020 2020 2020 2074 6578 7420             text 
-0001cde0: 3d20 5b2a 7365 6c66 5d0a 2020 2020 2020  = [*self].      
-0001cdf0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001ce00: 2020 2020 2020 2020 2020 2020 7465 7874              text
-0001ce10: 203d 2069 6e64 6976 6964 730a 2020 2020   = individs.    
-0001ce20: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001ce30: 2020 2020 2020 7465 7874 203d 204e 6f6e        text = Non
-0001ce40: 650a 2020 2020 2020 2020 2320 7365 7420  e.        # set 
-0001ce50: 7468 6520 706c 745f 6c69 6d73 0a20 2020  the plt_lims.   
-0001ce60: 2020 2020 2070 6c74 5f6c 696d 7320 3d20       plt_lims = 
-0001ce70: 7669 7a2e 5f67 6574 5f70 6c74 5f6c 696d  viz._get_plt_lim
-0001ce80: 7328 6c61 6e64 2c20 782c 2079 2c20 7a6f  s(land, x, y, zo
-0001ce90: 6f6d 5f77 6964 7468 290a 2020 2020 2020  om_width).      
-0001cea0: 2020 2320 706c 6f74 2074 6865 206c 6179    # plot the lay
-0001ceb0: 6572 2873 290a 2020 2020 2020 2020 6966  er(s).        if
-0001cec0: 2068 6964 655f 6c61 6e64 3a0a 2020 2020   hide_land:.    
-0001ced0: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-0001cee0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0001cef0: 2020 2020 2020 2023 2067 6574 2074 6865         # get the
-0001cf00: 206c 6179 6572 7327 2076 6d69 6e20 616e   layers' vmin an
-0001cf10: 6420 766d 6178 2076 616c 7565 732c 2069  d vmax values, i
-0001cf20: 6620 616e 7920 6f66 2074 6865 206c 6179  f any of the lay
-0001cf30: 6572 7320 746f 0a20 2020 2020 2020 2020  ers to.         
-0001cf40: 2020 2023 2062 6520 706c 6f74 7465 6420     # be plotted 
-0001cf50: 6861 7320 6120 6368 616e 6765 2065 7665  has a change eve
-0001cf60: 6e74 0a20 2020 2020 2020 2020 2020 2069  nt.            i
-0001cf70: 6620 2828 6c79 725f 6e75 6d20 6973 204e  f ((lyr_num is N
-0001cf80: 6f6e 6520 616e 6420 6c61 6e64 2e5f 6368  one and land._ch
-0001cf90: 616e 6765 7220 6973 206e 6f74 204e 6f6e  anger is not Non
-0001cfa0: 6529 206f 720a 2020 2020 2020 2020 2020  e) or.          
-0001cfb0: 2020 2020 2020 286c 616e 642e 5f63 6861        (land._cha
-0001cfc0: 6e67 6572 2069 7320 6e6f 7420 4e6f 6e65  nger is not None
-0001cfd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001cfe0: 2020 616e 6420 6c79 725f 6e75 6d20 696e    and lyr_num in
-0001cff0: 205b 2a6c 616e 642e 5f63 6861 6e67 6572   [*land._changer
-0001d000: 2e63 6861 6e67 655f 696e 666f 5d29 293a  .change_info])):
-0001d010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d020: 2069 6620 6c79 725f 6e75 6d20 6973 204e   if lyr_num is N
-0001d030: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0001d040: 2020 2020 2020 2020 206c 616e 645f 766d           land_vm
-0001d050: 696e 203d 205b 6c79 722e 5f73 6361 6c65  in = [lyr._scale
-0001d060: 5f6d 696e 2066 6f72 206c 7972 2069 6e20  _min for lyr in 
-0001d070: 6c61 6e64 2e76 616c 7565 7328 295d 0a20  land.values()]. 
-0001d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d090: 2020 206c 616e 645f 766d 6178 203d 205b     land_vmax = [
-0001d0a0: 6c79 722e 5f73 6361 6c65 5f6d 6178 2066  lyr._scale_max f
-0001d0b0: 6f72 206c 7972 2069 6e20 6c61 6e64 2e76  or lyr in land.v
-0001d0c0: 616c 7565 7328 295d 0a20 2020 2020 2020  alues()].       
-0001d0d0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0001d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d0f0: 2020 206c 616e 645f 766d 696e 203d 205b     land_vmin = [
-0001d100: 6c61 6e64 5b6c 7972 5f6e 756d 5d2e 5f73  land[lyr_num]._s
-0001d110: 6361 6c65 5f6d 696e 5d0a 2020 2020 2020  cale_min].      
-0001d120: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-0001d130: 6e64 5f76 6d61 7820 3d20 5b6c 616e 645b  nd_vmax = [land[
-0001d140: 6c79 725f 6e75 6d5d 2e5f 7363 616c 655f  lyr_num]._scale_
-0001d150: 6d61 785d 0a20 2020 2020 2020 2020 2020  max].           
-0001d160: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001d170: 2020 2020 2020 206c 616e 645f 766d 696e         land_vmin
-0001d180: 203d 206c 616e 645f 766d 6178 203d 204e   = land_vmax = N
-0001d190: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0001d1a0: 7669 7a2e 5f70 6c6f 745f 7261 7374 6572  viz._plot_raster
-0001d1b0: 7328 6c61 6e64 2c20 6c79 725f 6e75 6d3d  s(land, lyr_num=
-0001d1c0: 6c79 725f 6e75 6d2c 0a20 2020 2020 2020  lyr_num,.       
-0001d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1e0: 2020 2020 2020 2063 6261 723d 6362 6172         cbar=cbar
-0001d1f0: 2c20 636d 6170 3d6c 616e 645f 636d 6170  , cmap=land_cmap
-0001d200: 2c20 706c 745f 6c69 6d73 3d70 6c74 5f6c  , plt_lims=plt_l
-0001d210: 696d 732c 0a20 2020 2020 2020 2020 2020  ims,.           
-0001d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d230: 2020 2074 6963 6b73 3d74 6963 6b73 2c20     ticks=ticks, 
-0001d240: 6d61 736b 5f72 6173 743d 6d61 736b 5f72  mask_rast=mask_r
-0001d250: 6173 742c 0a20 2020 2020 2020 2020 2020  ast,.           
-0001d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d270: 2020 2076 6d69 6e3d 6c61 6e64 5f76 6d69     vmin=land_vmi
-0001d280: 6e2c 2076 6d61 783d 6c61 6e64 5f76 6d61  n, vmax=land_vma
-0001d290: 7829 0a20 2020 2020 2020 2023 2061 6e64  x).        # and
-0001d2a0: 2070 6c6f 7420 7468 6520 696e 6469 7669   plot the indivi
-0001d2b0: 6475 616c 730a 2020 2020 2020 2020 706f  duals.        po
-0001d2c0: 696e 7473 203d 2076 697a 2e5f 706c 6f74  ints = viz._plot
-0001d2d0: 5f70 6f69 6e74 7328 636f 6f72 6473 2c20  _points(coords, 
-0001d2e0: 6c79 725f 6e75 6d3d 6c79 725f 6e75 6d2c  lyr_num=lyr_num,
-0001d2f0: 2063 6f6c 6f72 3d63 6f6c 6f72 2c0a 2020   color=color,.  
-0001d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d320: 6564 6765 5f63 6f6c 6f72 3d65 6467 655f  edge_color=edge_
-0001d330: 636f 6c6f 722c 0a20 2020 2020 2020 2020  color,.         
-0001d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d350: 2020 2020 2020 2020 2074 6578 745f 636f           text_co
-0001d360: 6c6f 723d 7465 7874 5f63 6f6c 6f72 2c20  lor=text_color, 
-0001d370: 7369 7a65 3d73 697a 652c 0a20 2020 2020  size=size,.     
-0001d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d390: 2020 2020 2020 2020 2020 2020 2074 6578               tex
-0001d3a0: 745f 7369 7a65 3d74 6578 745f 7369 7a65  t_size=text_size
-0001d3b0: 2c20 616c 7068 613d 616c 7068 612c 0a20  , alpha=alpha,. 
-0001d3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3e0: 2074 6578 743d 7465 7874 2c20 706c 745f   text=text, plt_
-0001d3f0: 6c69 6d73 3d70 6c74 5f6c 696d 732c 0a20  lims=plt_lims,. 
-0001d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d420: 2070 745f 636d 6170 3d70 745f 636d 6170   pt_cmap=pt_cmap
-0001d430: 2c20 766d 696e 3d76 6d69 6e2c 2076 6d61  , vmin=vmin, vma
-0001d440: 783d 766d 6178 2c0a 2020 2020 2020 2020  x=vmax,.        
-0001d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d460: 2020 2020 2020 2020 2020 616e 696d 6174            animat
-0001d470: 653d 616e 696d 6174 6529 0a20 2020 2020  e=animate).     
-0001d480: 2020 2072 6574 7572 6e20 706f 696e 7473     return points
-0001d490: 0a0a 0a20 2020 2023 6d65 7468 6f64 2066  ...    #method f
-0001d4a0: 6f72 2070 6c6f 7474 696e 6720 7468 6520  or plotting the 
-0001d4b0: 7370 6563 6965 7320 6f6e 2074 6f70 206f  species on top o
-0001d4c0: 6620 6974 7320 6573 7469 6d61 7465 640a  f its estimated.
-0001d4d0: 2020 2020 2373 7065 6369 6573 2d64 656e      #species-den
-0001d4e0: 7369 7479 2072 6173 7465 720a 2020 2020  sity raster.    
-0001d4f0: 6465 6620 5f70 6c6f 745f 6465 6e73 6974  def _plot_densit
-0001d500: 7928 7365 6c66 2c20 6c61 6e64 2c20 6e6f  y(self, land, no
-0001d510: 726d 616c 697a 653d 4661 6c73 652c 2069  rmalize=False, i
-0001d520: 6e64 6976 6964 733d 4e6f 6e65 2c0a 2020  ndivids=None,.  
-0001d530: 2020 2020 2020 2020 2020 7465 7874 3d46            text=F
-0001d540: 616c 7365 2c20 636f 6c6f 723d 2762 6c61  alse, color='bla
-0001d550: 636b 272c 2065 6467 655f 636f 6c6f 723d  ck', edge_color=
-0001d560: 2766 6163 6527 2c0a 2020 2020 2020 2020  'face',.        
-0001d570: 2020 2020 7465 7874 5f63 6f6c 6f72 3d27      text_color='
-0001d580: 626c 6163 6b27 2c20 7369 7a65 3d32 352c  black', size=25,
-0001d590: 2074 6578 745f 7369 7a65 203d 2039 2c0a   text_size = 9,.
-0001d5a0: 2020 2020 2020 2020 2020 2020 616c 7068              alph
-0001d5b0: 613d 302e 352c 207a 6f6f 6d5f 7769 6474  a=0.5, zoom_widt
-0001d5c0: 683d 4e6f 6e65 2c20 783d 4e6f 6e65 2c20  h=None, x=None, 
-0001d5d0: 793d 4e6f 6e65 2c20 7469 636b 733d 4e6f  y=None, ticks=No
-0001d5e0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0001d5f0: 6d61 736b 5f72 6173 743d 4e6f 6e65 293a  mask_rast=None):
-0001d600: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0001d610: 7479 7065 286e 6f72 6d61 6c69 7a65 2920  type(normalize) 
-0001d620: 6973 2062 6f6f 6c2c 2028 2254 6865 2027  is bool, ("The '
-0001d630: 6e6f 726d 616c 697a 6527 2061 7267 756d  normalize' argum
-0001d640: 656e 7420 7461 6b65 7320 220a 2020 2020  ent takes ".    
-0001d650: 2020 2020 2020 2020 2261 2062 6f6f 6c65          "a boole
-0001d660: 616e 2076 616c 7565 2e5c 6e22 290a 2020  an value.\n").  
-0001d670: 2020 2020 2020 2375 7064 6174 6520 7468        #update th
-0001d680: 6520 7370 6563 6965 7327 2063 6f6f 7264  e species' coord
-0001d690: 696e 6174 6573 2061 6e64 2063 656c 6c73  inates and cells
-0001d6a0: 2c20 696e 2063 6173 6520 6974 2068 6173  , in case it has
-0001d6b0: 6e27 740a 2020 2020 2020 2020 2362 6565  n't.        #bee
-0001d6c0: 6e20 7570 6461 7465 6420 7369 6e63 6520  n updated since 
-0001d6d0: 736f 6d65 2069 6e74 6572 6e61 6c20 6f72  some internal or
-0001d6e0: 206d 616e 7561 6c20 6368 616e 6765 7320   manual changes 
-0001d6f0: 696e 2070 6f70 756c 6174 696f 6e2d 7369  in population-si
-0001d700: 7a65 0a20 2020 2020 2020 2023 6861 7665  ze.        #have
-0001d710: 206f 6363 7572 7265 640a 2020 2020 2020   occurred.      
-0001d720: 2020 7365 6c66 2e5f 7365 745f 636f 6f72    self._set_coor
-0001d730: 6473 5f61 6e64 5f63 656c 6c73 2829 0a20  ds_and_cells(). 
-0001d740: 2020 2020 2020 2064 656e 7320 3d20 7365         dens = se
-0001d750: 6c66 2e5f 6361 6c63 5f64 656e 7369 7479  lf._calc_density
-0001d760: 286e 6f72 6d61 6c69 7a65 203d 206e 6f72  (normalize = nor
-0001d770: 6d61 6c69 7a65 290a 2020 2020 2020 2020  malize).        
-0001d780: 706c 745f 6c69 6d73 203d 2076 697a 2e5f  plt_lims = viz._
-0001d790: 6765 745f 706c 745f 6c69 6d73 286c 616e  get_plt_lims(lan
-0001d7a0: 642c 2078 2c20 792c 207a 6f6f 6d5f 7769  d, x, y, zoom_wi
-0001d7b0: 6474 6829 0a20 2020 2020 2020 2069 6620  dth).        if 
-0001d7c0: 6e6f 726d 616c 697a 653a 0a20 2020 2020  normalize:.     
-0001d7d0: 2020 2020 2020 2076 697a 2e5f 706c 6f74         viz._plot
-0001d7e0: 5f72 6173 7465 7273 2864 656e 732c 2070  _rasters(dens, p
-0001d7f0: 6c74 5f6c 696d 7320 3d20 706c 745f 6c69  lt_lims = plt_li
-0001d800: 6d73 2c20 6c79 725f 6e61 6d65 203d 2027  ms, lyr_name = '
-0001d810: 6465 6e73 6974 7927 2c0a 2020 2020 2020  density',.      
-0001d820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d830: 2020 2020 2020 2020 7469 636b 733d 7469          ticks=ti
-0001d840: 636b 732c 206d 6173 6b5f 7261 7374 3d6d  cks, mask_rast=m
-0001d850: 6173 6b5f 7261 7374 290a 2020 2020 2020  ask_rast).      
-0001d860: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001d870: 2020 2020 7669 7a2e 5f70 6c6f 745f 7261      viz._plot_ra
-0001d880: 7374 6572 7328 6465 6e73 2c20 706c 745f  sters(dens, plt_
-0001d890: 6c69 6d73 203d 2070 6c74 5f6c 696d 732c  lims = plt_lims,
-0001d8a0: 2076 6d61 7820 3d20 6465 6e73 2e6d 6178   vmax = dens.max
-0001d8b0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-0001d8c0: 2020 2020 6c79 725f 6e61 6d65 203d 2027      lyr_name = '
-0001d8d0: 6465 6e73 6974 7927 2c20 7469 636b 733d  density', ticks=
-0001d8e0: 7469 636b 732c 206d 6173 6b5f 7261 7374  ticks, mask_rast
-0001d8f0: 3d6d 6173 6b5f 7261 7374 290a 2020 2020  =mask_rast).    
-0001d900: 2020 2020 7365 6c66 2e5f 706c 6f74 2868      self._plot(h
-0001d910: 6964 655f 6c61 6e64 3d54 7275 652c 2069  ide_land=True, i
-0001d920: 6e64 6976 6964 7320 3d20 696e 6469 7669  ndivids = indivi
-0001d930: 6473 2c20 7465 7874 203d 2074 6578 742c  ds, text = text,
-0001d940: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-0001d950: 6f72 3d63 6f6c 6f72 2c20 6564 6765 5f63  or=color, edge_c
-0001d960: 6f6c 6f72 203d 2065 6467 655f 636f 6c6f  olor = edge_colo
-0001d970: 722c 2074 6578 745f 636f 6c6f 7220 3d20  r, text_color = 
-0001d980: 7465 7874 5f63 6f6c 6f72 2c0a 2020 2020  text_color,.    
-0001d990: 2020 2020 2020 2020 7369 7a65 3d73 697a          size=siz
-0001d9a0: 652c 2074 6578 745f 7369 7a65 203d 2074  e, text_size = t
-0001d9b0: 6578 745f 7369 7a65 2c20 616c 7068 613d  ext_size, alpha=
-0001d9c0: 616c 7068 612c 0a20 2020 2020 2020 2020  alpha,.         
-0001d9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d9e0: 2020 2020 2020 2020 2020 207a 6f6f 6d5f             zoom_
-0001d9f0: 7769 6474 6820 3d20 7a6f 6f6d 5f77 6964  width = zoom_wid
-0001da00: 7468 2c20 7820 3d20 782c 2079 203d 2079  th, x = x, y = y
-0001da10: 290a 0a0a 2020 2020 2320 6d65 7468 6f64  )...    # method
-0001da20: 2066 6f72 2070 6c6f 7474 696e 6720 696e   for plotting in
-0001da30: 6469 7669 6475 616c 7320 636f 6c6f 7265  dividuals colore
-0001da40: 6420 6279 2074 6865 6972 2067 656e 6f74  d by their genot
-0001da50: 7970 6520 6174 2061 206c 6f63 7573 0a20  ype at a locus. 
-0001da60: 2020 2064 6566 205f 706c 6f74 5f67 656e     def _plot_gen
-0001da70: 6f74 7970 6528 7365 6c66 2c20 6c6f 6375  otype(self, locu
-0001da80: 732c 206c 7972 5f6e 756d 3d4e 6f6e 652c  s, lyr_num=None,
-0001da90: 206c 616e 643d 4e6f 6e65 2c20 696e 6469   land=None, indi
-0001daa0: 7669 6473 3d4e 6f6e 652c 0a20 2020 2020  vids=None,.     
-0001dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dac0: 2020 7465 7874 3d46 616c 7365 2c20 7369    text=False, si
-0001dad0: 7a65 3d32 352c 2074 6578 745f 7369 7a65  ze=25, text_size
-0001dae0: 203d 2039 2c20 6564 6765 5f63 6f6c 6f72   = 9, edge_color
-0001daf0: 3d27 626c 6163 6b27 2c0a 2020 2020 2020  ='black',.      
-0001db00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db10: 2074 6578 745f 636f 6c6f 723d 2762 6c61   text_color='bla
-0001db20: 636b 272c 2063 6261 723d 5472 7565 2c20  ck', cbar=True, 
-0001db30: 616c 7068 613d 312c 0a20 2020 2020 2020  alpha=1,.       
-0001db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db50: 6279 5f64 6f6d 696e 616e 6365 3d46 616c  by_dominance=Fal
-0001db60: 7365 2c20 7a6f 6f6d 5f77 6964 7468 3d4e  se, zoom_width=N
-0001db70: 6f6e 652c 2078 3d4e 6f6e 652c 2079 3d4e  one, x=None, y=N
-0001db80: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0001db90: 2020 2020 2020 2020 2020 2020 7469 636b              tick
-0001dba0: 733d 4e6f 6e65 2c20 6d61 736b 5f72 6173  s=None, mask_ras
-0001dbb0: 743d 4e6f 6e65 293a 0a0a 2020 2020 2020  t=None):..      
-0001dbc0: 2020 6765 6e6f 7479 7065 7320 3d20 7365    genotypes = se
-0001dbd0: 6c66 2e5f 6765 745f 6765 6e6f 7479 7065  lf._get_genotype
-0001dbe0: 7328 6c6f 6369 3d5b 6c6f 6375 735d 2c20  s(loci=[locus], 
-0001dbf0: 696e 6469 7669 6473 3d69 6e64 6976 6964  individs=individ
-0001dc00: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0001dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dc20: 2020 2020 2020 2020 2020 2062 6961 6c6c             biall
-0001dc30: 656c 6963 3d46 616c 7365 2c20 6173 5f64  elic=False, as_d
-0001dc40: 6963 743d 5472 7565 290a 2020 2020 2020  ict=True).      
-0001dc50: 2020 6966 2062 795f 646f 6d69 6e61 6e63    if by_dominanc
-0001dc60: 6520 3d3d 2054 7275 653a 0a20 2020 2020  e == True:.     
-0001dc70: 2020 2020 2020 2069 6620 6c6f 6375 7320         if locus 
-0001dc80: 696e 2073 656c 662e 6765 6e5f 6172 6368  in self.gen_arch
-0001dc90: 2e6e 6f6e 6e65 7574 5f6c 6f63 693a 0a20  .nonneut_loci:. 
-0001dca0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0001dcb0: 6f6d 203d 2073 656c 662e 6765 6e5f 6172  om = self.gen_ar
-0001dcc0: 6368 2e64 6f6d 5b6c 6f63 7573 5d0a 2020  ch.dom[locus].  
-0001dcd0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0001dce0: 4e4f 5445 3a20 776f 756c 6420 6265 2073  NOTE: would be s
-0001dcf0: 696d 706c 6572 2074 6f20 6a75 7374 2075  impler to just u
-0001dd00: 7365 206e 702e 6365 696c 2068 6572 652e  se np.ceil here.
-0001dd10: 2e2e 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001dd20: 2020 2023 2020 2020 2020 2064 6f6e 2774     #       don't
-0001dd30: 2073 6565 2077 6879 2049 2064 6964 6e27   see why I didn'
-0001dd40: 742e 2e2e 3f0a 2020 2020 2020 2020 2020  t...?.          
-0001dd50: 2020 2020 2020 6765 6e6f 7479 7065 7320        genotypes 
-0001dd60: 3d20 7b69 3a6e 702e 636c 6970 2867 7420  = {i:np.clip(gt 
-0001dd70: 2a20 2831 202b 2064 6f6d 292c 0a20 2020  * (1 + dom),.   
-0001dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dda0: 2020 2020 615f 6d69 6e3d 4e6f 6e65 2c0a      a_min=None,.
-0001ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ddd0: 2020 2020 2020 2061 5f6d 6178 3d31 2920         a_max=1) 
-0001dde0: 666f 7220 692c 2067 7420 696e 2067 656e  for i, gt in gen
-0001ddf0: 6f74 7970 6573 2e69 7465 6d73 2829 7d0a  otypes.items()}.
-0001de00: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001de10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001de20: 2020 7072 696e 7428 2827 5c6e 5c74 5741    print(('\n\tWA
-0001de30: 524e 494e 473a 2054 6865 2062 795f 646f  RNING: The by_do
-0001de40: 6d69 6e61 6e63 6520 6172 6775 6d65 6e74  minance argument
-0001de50: 2069 7320 5472 7565 2c20 270a 2020 2020   is True, '.    
-0001de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de70: 2020 2027 6275 7420 6120 6e65 7574 7261     'but a neutra
-0001de80: 6c20 6c6f 6375 7320 7761 7320 6368 6f73  l locus was chos
-0001de90: 656e 2c20 270a 2020 2020 2020 2020 2020  en, '.          
-0001dea0: 2020 2020 2020 2020 2020 2020 2027 736f               'so
-0001deb0: 2074 6865 2061 7267 756d 656e 7420 7761   the argument wa
-0001dec0: 7320 6e6f 7420 7573 6564 2e5c 6e27 2929  s not used.\n'))
-0001ded0: 0a0a 2020 2020 2020 2020 2320 6a75 7374  ..        # just
-0001dee0: 2061 7373 6967 6e20 626c 6163 6b2c 2067   assign black, g
-0001def0: 7261 792c 2061 6e64 2077 6869 7465 2028  ray, and white (
-0001df00: 7369 6e63 6520 7468 6572 6527 7320 6e6f  since there's no
-0001df10: 2072 6561 736f 6e0a 2020 2020 2020 2020   reason.        
-0001df20: 2320 6e65 6365 7373 6172 696c 7920 7468  # necessarily th
-0001df30: 6174 2074 6865 7365 2073 686f 756c 6420  at these should 
-0001df40: 6265 206d 6170 7065 6420 746f 2061 2063  be mapped to a c
-0001df50: 6572 7461 696e 206c 6179 6572 2c20 7468  ertain layer, th
-0001df60: 6520 7761 790a 2020 2020 2020 2020 2320  e way.        # 
-0001df70: 7068 656e 6f74 7970 6520 7368 6f75 6c64  phenotype should
-0001df80: 0a20 2020 2020 2020 2063 6f6c 6f72 7320  .        colors 
-0001df90: 3d20 5b27 2330 3030 3030 3027 2c20 2723  = ['#000000', '#
-0001dfa0: 3830 3830 3830 272c 2027 2346 4646 4646  808080', '#FFFFF
-0001dfb0: 4627 5d0a 0a20 2020 2020 2020 2066 6f72  F']..        for
-0001dfc0: 206e 2c20 6765 6e6f 7479 7065 2069 6e20   n, genotype in 
-0001dfd0: 656e 756d 6572 6174 6528 5b30 2e30 2c20  enumerate([0.0, 
-0001dfe0: 302e 352c 2031 2e30 5d29 3a0a 2020 2020  0.5, 1.0]):.    
-0001dff0: 2020 2020 2020 2020 6765 6e6f 7479 7065          genotype
-0001e000: 5f69 6e64 6976 6964 7320 3d20 5b69 2066  _individs = [i f
-0001e010: 6f72 2069 2c20 6720 696e 2067 656e 6f74  or i, g in genot
-0001e020: 7970 6573 2e69 7465 6d73 280a 2020 2020  ypes.items(.    
-0001e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e050: 2020 2020 2920 6966 206e 702e 6174 6c65      ) if np.atle
-0001e060: 6173 745f 3164 2867 295b 305d 203d 3d20  ast_1d(g)[0] == 
-0001e070: 6765 6e6f 7479 7065 5d0a 2020 2020 2020  genotype].      
-0001e080: 2020 2020 2020 2320 7769 6c6c 2068 6964        # will hid
-0001e090: 6520 7468 6520 6c61 6e64 2069 6620 7468  e the land if th
-0001e0a0: 6973 2069 7320 6e6f 7420 7468 6520 6669  is is not the fi
-0001e0b0: 7273 7420 706c 6f74 206d 6164 650a 2020  rst plot made.  
-0001e0c0: 2020 2020 2020 2020 2020 6869 6465 5f6c            hide_l
-0001e0d0: 616e 6420 3d20 6e20 3e20 300a 2020 2020  and = n > 0.    
-0001e0e0: 2020 2020 2020 2020 2320 706c 6f74 2069          # plot i
-0001e0f0: 6620 7468 6572 6520 6172 6520 616e 7920  f there are any 
-0001e100: 696e 6469 7669 6475 616c 7320 6f66 2074  individuals of t
-0001e110: 6869 7320 6765 6e6f 7479 7065 0a20 2020  his genotype.   
-0001e120: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-0001e130: 6765 6e6f 7479 7065 5f69 6e64 6976 6964  genotype_individ
-0001e140: 7329 203e 3d20 313a 0a20 2020 2020 2020  s) >= 1:.       
-0001e150: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
-0001e160: 6c6f 7428 6c79 725f 6e75 6d3d 6c79 725f  lot(lyr_num=lyr_
-0001e170: 6e75 6d2c 206c 616e 643d 6c61 6e64 2c20  num, land=land, 
-0001e180: 6869 6465 5f6c 616e 643d 6869 6465 5f6c  hide_land=hide_l
-0001e190: 616e 642c 0a20 2020 2020 2020 2020 2020  and,.           
-0001e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1b0: 696e 6469 7669 6473 3d67 656e 6f74 7970  individs=genotyp
-0001e1c0: 655f 696e 6469 7669 6473 2c0a 2020 2020  e_individs,.    
-0001e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1e0: 2020 2020 2020 2074 6578 743d 7465 7874         text=text
-0001e1f0: 2c20 636f 6c6f 723d 636f 6c6f 7273 5b6e  , color=colors[n
-0001e200: 5d2c 2065 6467 655f 636f 6c6f 723d 6564  ], edge_color=ed
-0001e210: 6765 5f63 6f6c 6f72 2c0a 2020 2020 2020  ge_color,.      
-0001e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e230: 2020 2020 2074 6578 745f 636f 6c6f 723d       text_color=
-0001e240: 7465 7874 5f63 6f6c 6f72 2c20 6362 6172  text_color, cbar
-0001e250: 3d63 6261 722c 0a20 2020 2020 2020 2020  =cbar,.         
-0001e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e270: 2020 7369 7a65 3d73 697a 652c 2074 6578    size=size, tex
-0001e280: 745f 7369 7a65 3d74 6578 745f 7369 7a65  t_size=text_size
-0001e290: 2c20 616c 7068 613d 616c 7068 612c 0a20  , alpha=alpha,. 
-0001e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e2b0: 2020 2020 2020 2020 2020 7a6f 6f6d 5f77            zoom_w
-0001e2c0: 6964 7468 3d7a 6f6f 6d5f 7769 6474 682c  idth=zoom_width,
-0001e2d0: 2078 3d78 2c20 793d 792c 2076 6d69 6e3d   x=x, y=y, vmin=
-0001e2e0: 302c 2076 6d61 783d 312c 0a20 2020 2020  0, vmax=1,.     
-0001e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e300: 2020 2020 2020 7469 636b 733d 7469 636b        ticks=tick
-0001e310: 732c 206d 6173 6b5f 7261 7374 3d6d 6173  s, mask_rast=mas
-0001e320: 6b5f 7261 7374 290a 0a0a 2020 2020 2320  k_rast)...    # 
-0001e330: 6d65 7468 6f64 2066 6f72 2070 6c6f 7474  method for plott
-0001e340: 696e 6720 696e 6469 7669 6475 616c 7320  ing individuals 
-0001e350: 636f 6c6f 7265 6420 6279 2074 6865 6972  colored by their
-0001e360: 2070 6865 6e6f 7479 7065 730a 2020 2020   phenotypes.    
-0001e370: 2366 6f72 2061 2067 6976 656e 2074 7261  #for a given tra
-0001e380: 6974 0a20 2020 2064 6566 205f 706c 6f74  it.    def _plot
-0001e390: 5f70 6865 6e6f 7479 7065 2873 656c 662c  _phenotype(self,
-0001e3a0: 2074 7261 6974 2c20 6c79 725f 6e75 6d3d   trait, lyr_num=
-0001e3b0: 4e6f 6e65 2c20 6c61 6e64 3d4e 6f6e 652c  None, land=None,
-0001e3c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e3d0: 2020 2020 2020 2020 2069 6e64 6976 6964           individ
-0001e3e0: 733d 4e6f 6e65 2c20 7465 7874 3d46 616c  s=None, text=Fal
-0001e3f0: 7365 2c20 7369 7a65 3d32 352c 2074 6578  se, size=25, tex
-0001e400: 745f 7369 7a65 3d39 2c0a 2020 2020 2020  t_size=9,.      
-0001e410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e420: 2020 6564 6765 5f63 6f6c 6f72 3d27 626c    edge_color='bl
-0001e430: 6163 6b27 2c20 7465 7874 5f63 6f6c 6f72  ack', text_color
-0001e440: 3d27 626c 6163 6b27 2c20 6362 6172 3d54  ='black', cbar=T
-0001e450: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-0001e460: 2020 2020 2020 2020 2020 2020 2061 6c70               alp
-0001e470: 6861 3d31 2c20 7a6f 6f6d 5f77 6964 7468  ha=1, zoom_width
-0001e480: 3d4e 6f6e 652c 2078 3d4e 6f6e 652c 2079  =None, x=None, y
-0001e490: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-0001e4a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001e4b0: 6963 6b73 3d4e 6f6e 652c 206d 6173 6b5f  icks=None, mask_
-0001e4c0: 7261 7374 3d4e 6f6e 652c 2061 6e69 6d61  rast=None, anima
-0001e4d0: 7465 3d46 616c 7365 293a 0a0a 2020 2020  te=False):..    
-0001e4e0: 2020 2020 2320 6765 7420 7468 6520 7472      # get the tr
-0001e4f0: 6169 7427 7320 6c79 725f 6e75 6d2c 2069  ait's lyr_num, i
-0001e500: 6620 6e6f 206c 7972 5f6e 756d 2070 726f  f no lyr_num pro
-0001e510: 7669 6465 640a 2020 2020 2020 2020 6c79  vided.        ly
-0001e520: 725f 6e75 6d20 3d20 7365 6c66 2e67 656e  r_num = self.gen
-0001e530: 5f61 7263 682e 7472 6169 7473 5b74 7261  _arch.traits[tra
-0001e540: 6974 5d2e 6c79 725f 6e75 6d0a 0a20 2020  it].lyr_num..   
-0001e550: 2020 2020 207a 203d 204f 4428 7a69 7028       z = OD(zip(
-0001e560: 5b2a 7365 6c66 5d2c 2073 656c 662e 5f67  [*self], self._g
-0001e570: 6574 5f7a 2829 5b3a 2c20 7472 6169 745d  et_z()[:, trait]
-0001e580: 2929 0a20 2020 2020 2020 2069 6620 696e  )).        if in
-0001e590: 6469 7669 6473 2069 7320 6e6f 7420 4e6f  divids is not No
-0001e5a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0001e5b0: 7a20 3d20 7b69 3a20 7620 666f 7220 692c  z = {i: v for i,
-0001e5c0: 2076 2069 6e20 7a2e 6974 656d 7328 2920   v in z.items() 
-0001e5d0: 6966 2069 2069 6e20 696e 6469 7669 6473  if i in individs
-0001e5e0: 7d0a 0a20 2020 2020 2020 2023 2067 6574  }..        # get
-0001e5f0: 2074 6865 2063 6f72 7265 6374 2063 6d61   the correct cma
-0001e600: 7020 666f 7220 7468 6973 2074 7261 6974  p for this trait
-0001e610: 2773 206c 6179 6572 0a20 2020 2020 2020  's layer.       
-0001e620: 2070 745f 636d 6170 203d 2076 697a 2e5f   pt_cmap = viz._
-0001e630: 6368 6f6f 7365 5f63 6d61 7028 7365 6c66  choose_cmap(self
-0001e640: 2e67 656e 5f61 7263 682e 7472 6169 7473  .gen_arch.traits
-0001e650: 5b74 7261 6974 5d2e 6c79 725f 6e75 6d29  [trait].lyr_num)
-0001e660: 0a0a 2020 2020 2020 2020 706f 696e 7473  ..        points
-0001e670: 203d 2073 656c 662e 5f70 6c6f 7428 6c79   = self._plot(ly
-0001e680: 725f 6e75 6d20 3d20 6c79 725f 6e75 6d2c  r_num = lyr_num,
-0001e690: 206c 616e 6420 3d20 6c61 6e64 2c0a 2020   land = land,.  
-0001e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e6b0: 2020 2020 2020 2020 2020 696e 6469 7669            indivi
-0001e6c0: 6473 203d 2069 6e64 6976 6964 732c 2074  ds = individs, t
-0001e6d0: 6578 7420 3d20 7465 7874 2c0a 2020 2020  ext = text,.    
-0001e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e6f0: 2020 2020 2020 2020 636f 6c6f 7220 3d20          color = 
-0001e700: 6c69 7374 287a 2e76 616c 7565 7328 2929  list(z.values())
-0001e710: 2c20 7074 5f63 6d61 7020 3d20 7074 5f63  , pt_cmap = pt_c
-0001e720: 6d61 702c 0a20 2020 2020 2020 2020 2020  map,.           
+0001c410: 2020 2069 6620 2878 203c 2030 2061 6e64     if (x < 0 and
+0001c420: 2079 203e 2030 293a 0a20 2020 2020 2020   y > 0):.       
+0001c430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c440: 706c 742e 7465 7874 2878 202d 2073 782c  plt.text(x - sx,
+0001c450: 2079 202b 2073 792c 2058 2e63 6f6c 756d   y + sy, X.colum
+0001c460: 6e73 5b69 5d29 0a20 2020 2020 2020 2020  ns[i]).         
+0001c470: 2020 2020 2020 2020 2020 2069 6620 2878             if (x
+0001c480: 203e 2030 2061 6e64 2079 203e 2030 293a   > 0 and y > 0):
+0001c490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c4a0: 2020 2020 2020 2020 706c 742e 7465 7874          plt.text
+0001c4b0: 2878 202b 2073 782c 2079 202b 2073 792c  (x + sx, y + sy,
+0001c4c0: 2058 2e63 6f6c 756d 6e73 5b69 5d29 0a20   X.columns[i]). 
+0001c4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c4e0: 2020 2069 6620 2878 203e 2030 2061 6e64     if (x > 0 and
+0001c4f0: 2079 203c 2030 293a 0a20 2020 2020 2020   y < 0):.       
+0001c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c510: 706c 742e 7465 7874 2878 202b 2073 782c  plt.text(x + sx,
+0001c520: 2079 202d 2073 792c 2058 2e63 6f6c 756d   y - sy, X.colum
+0001c530: 6e73 5b69 5d29 0a0a 2020 2020 2020 2020  ns[i])..        
+0001c540: 2020 2020 2020 2020 2370 6c6f 7420 5344          #plot SD
+0001c550: 2065 6c6c 6970 7365 2066 6f72 2053 4e50   ellipse for SNP
+0001c560: 2064 6174 6120 6966 2070 6c6f 745f 7364   data if plot_sd
+0001c570: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
+0001c580: 2020 2020 2020 2020 6966 2070 6c6f 745f          if plot_
+0001c590: 7364 3a0a 2020 2020 2020 2020 2020 2020  sd:.            
+0001c5a0: 2020 2020 2020 2020 7231 203d 206e 702e          r1 = np.
+0001c5b0: 7374 6428 6c6f 6369 5f64 665b 7374 7228  std(loci_df[str(
+0001c5c0: 6363 5f61 7869 7331 295d 2920 2a20 7364  cc_axis1)]) * sd
+0001c5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c5e0: 2020 2020 2072 3220 3d20 6e70 2e73 7464       r2 = np.std
+0001c5f0: 286c 6f63 695f 6466 5b73 7472 2863 635f  (loci_df[str(cc_
+0001c600: 6178 6973 3229 5d29 202a 2073 640a 2020  axis2)]) * sd.  
+0001c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c620: 2020 7420 3d20 6e70 2e6c 696e 7370 6163    t = np.linspac
+0001c630: 6528 302c 2032 2a6d 6174 685f 7069 2c20  e(0, 2*math_pi, 
+0001c640: 3130 3029 0a20 2020 2020 2020 2020 2020  100).           
+0001c650: 2020 2020 2020 2020 2061 782e 706c 6f74           ax.plot
+0001c660: 2872 312a 6e70 2e63 6f73 2874 2920 2c20  (r1*np.cos(t) , 
+0001c670: 7232 2a6e 702e 7369 6e28 7429 2c20 6c69  r2*np.sin(t), li
+0001c680: 6e65 7374 796c 6520 3d20 2764 6173 6865  nestyle = 'dashe
+0001c690: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
+0001c6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c6b0: 6320 3d20 2772 6564 272c 206c 6162 656c  c = 'red', label
+0001c6c0: 203d 2073 7472 2873 6429 202b 2022 2053   = str(sd) + " S
+0001c6d0: 7464 4465 7622 290a 0a20 2020 2020 2020  tdDev")..       
+0001c6e0: 2020 2020 2020 2020 2023 4556 4552 5954           #EVERYT
+0001c6f0: 4849 4e47 2042 454c 4f57 2054 4849 5320  HING BELOW THIS 
+0001c700: 4c49 4e45 2049 4e20 5448 4520 4c4f 4f50  LINE IN THE LOOP
+0001c710: 2049 5320 4a55 5354 2050 4c4f 5420 464f   IS JUST PLOT FO
+0001c720: 524d 4154 5449 4e47 200a 2020 2020 2020  RMATTING .      
+0001c730: 2020 2020 2020 2020 2020 2378 6c61 6265            #xlabe
+0001c740: 6c20 6973 2074 6865 206c 6162 656c 2061  l is the label a
+0001c750: 7420 7468 6520 626f 7474 6f6d 2028 7665  t the bottom (ve
+0001c760: 7274 6963 616c 2061 7869 7320 6c61 6265  rtical axis labe
+0001c770: 6c29 0a20 2020 2020 2020 2020 2020 2020  l).             
+0001c780: 2020 2023 2061 6e64 2079 6c61 6265 6c20     # and ylabel 
+0001c790: 6973 206f 6e20 7468 6520 6c65 6674 2073  is on the left s
+0001c7a0: 6964 6520 2868 6f72 697a 6f6e 7461 6c20  ide (horizontal 
+0001c7b0: 6178 6973 206c 6162 656c 290a 2020 2020  axis label).    
+0001c7c0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+0001c7d0: 6c20 3d20 6178 2e73 6574 5f78 6c61 6265  l = ax.set_xlabe
+0001c7e0: 6c28 2743 4341 2720 2b20 7374 7228 6363  l('CCA' + str(cc
+0001c7f0: 5f61 7869 7332 292c 2066 6f6e 7473 697a  _axis2), fontsiz
+0001c800: 6520 3d20 3929 0a20 2020 2020 2020 2020  e = 9).         
+0001c810: 2020 2020 2020 2061 782e 7861 7869 732e         ax.xaxis.
+0001c820: 7365 745f 6c61 6265 6c5f 636f 6f72 6473  set_label_coords
+0001c830: 2830 2e35 2c20 2d30 2e30 3229 0a20 2020  (0.5, -0.02).   
+0001c840: 2020 2020 2020 2020 2020 2020 206c 6162               lab
+0001c850: 656c 203d 2061 782e 7365 745f 796c 6162  el = ax.set_ylab
+0001c860: 656c 2827 4343 4127 202b 2073 7472 2863  el('CCA' + str(c
+0001c870: 635f 6178 6973 3129 2c20 666f 6e74 7369  c_axis1), fontsi
+0001c880: 7a65 203d 2039 290a 2020 2020 2020 2020  ze = 9).        
+0001c890: 2020 2020 2020 2020 6178 2e79 6178 6973          ax.yaxis
+0001c8a0: 2e73 6574 5f6c 6162 656c 5f63 6f6f 7264  .set_label_coord
+0001c8b0: 7328 2d30 2e30 322c 2030 2e35 3529 0a0a  s(-0.02, 0.55)..
+0001c8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c8d0: 236d 616b 6520 696e 746f 2062 6f78 0a20  #make into box. 
+0001c8e0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0001c8f0: 782e 7365 745f 6173 7065 6374 2827 6571  x.set_aspect('eq
+0001c900: 7561 6c27 2c20 6164 6a75 7374 6162 6c65  ual', adjustable
+0001c910: 3d27 626f 7827 290a 0a20 2020 2020 2020  ='box')..       
+0001c920: 2020 2020 2020 2020 2023 4d6f 7665 206c           #Move l
+0001c930: 6566 7420 792d 6178 6973 2026 2062 6f74  eft y-axis & bot
+0001c940: 746f 6d20 782d 6178 6973 2074 6f20 6365  tom x-axis to ce
+0001c950: 6e74 6572 2c20 7061 7373 696e 6720 7468  nter, passing th
+0001c960: 7275 2028 302c 3029 0a20 2020 2020 2020  ru (0,0).       
+0001c970: 2020 2020 2020 2020 2061 782e 7370 696e           ax.spin
+0001c980: 6573 5b27 6c65 6674 275d 2e73 6574 5f70  es['left'].set_p
+0001c990: 6f73 6974 696f 6e28 2763 656e 7465 7227  osition('center'
+0001c9a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001c9b0: 2020 6178 2e73 7069 6e65 735b 2762 6f74    ax.spines['bot
+0001c9c0: 746f 6d27 5d2e 7365 745f 706f 7369 7469  tom'].set_positi
+0001c9d0: 6f6e 2827 6365 6e74 6572 2729 0a0a 2020  on('center')..  
+0001c9e0: 2020 2020 2020 2020 2020 2020 2020 2363                #c
+0001c9f0: 6861 6e67 6520 636f 6c6f 7273 2f72 656d  hange colors/rem
+0001ca00: 6f76 6520 6465 6661 756c 7420 6178 6973  ove default axis
+0001ca10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ca20: 2061 7863 6f6c 6f72 203d 2027 6e6f 6e65   axcolor = 'none
+0001ca30: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0001ca40: 2020 6178 2e73 7069 6e65 735b 276c 6566    ax.spines['lef
+0001ca50: 7427 5d2e 7365 745f 636f 6c6f 7228 6178  t'].set_color(ax
+0001ca60: 636f 6c6f 7229 0a20 2020 2020 2020 2020  color).         
+0001ca70: 2020 2020 2020 2061 782e 7370 696e 6573         ax.spines
+0001ca80: 5b27 626f 7474 6f6d 275d 2e73 6574 5f63  ['bottom'].set_c
+0001ca90: 6f6c 6f72 2861 7863 6f6c 6f72 290a 2020  olor(axcolor).  
+0001caa0: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+0001cab0: 2e73 7069 6e65 735b 2772 6967 6874 275d  .spines['right']
+0001cac0: 2e73 6574 5f63 6f6c 6f72 2861 7863 6f6c  .set_color(axcol
+0001cad0: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
+0001cae0: 2020 2020 6178 2e73 7069 6e65 735b 2774      ax.spines['t
+0001caf0: 6f70 275d 2e73 6574 5f63 6f6c 6f72 2861  op'].set_color(a
+0001cb00: 7863 6f6c 6f72 290a 2020 2020 2020 2020  xcolor).        
+0001cb10: 2020 2020 2020 2020 6178 2e74 6963 6b5f          ax.tick_
+0001cb20: 7061 7261 6d73 2861 7869 7320 3d20 2778  params(axis = 'x
+0001cb30: 272c 2063 6f6c 6f72 733d 6178 636f 6c6f  ', colors=axcolo
+0001cb40: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+0001cb50: 2020 2061 782e 7469 636b 5f70 6172 616d     ax.tick_param
+0001cb60: 7328 6178 6973 203d 2027 7927 2c20 636f  s(axis = 'y', co
+0001cb70: 6c6f 7273 3d61 7863 6f6c 6f72 290a 0a20  lors=axcolor).. 
+0001cb80: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0001cb90: 782e 7961 7869 732e 6c61 6265 6c2e 7365  x.yaxis.label.se
+0001cba0: 745f 636f 6c6f 7228 2767 7261 7927 290a  t_color('gray').
+0001cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cbc0: 6178 2e78 6178 6973 2e6c 6162 656c 2e73  ax.xaxis.label.s
+0001cbd0: 6574 5f63 6f6c 6f72 2827 6772 6179 2729  et_color('gray')
+0001cbe0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001cbf0: 2020 236c 6567 656e 6473 0a20 2020 2020    #legends.     
+0001cc00: 2020 2020 2020 2020 2020 2069 6620 6e20             if n 
+0001cc10: 3d3d 2032 3a0a 2020 2020 2020 2020 2020  == 2:.          
+0001cc20: 2020 2020 2020 2020 2020 6178 2e6c 6567            ax.leg
+0001cc30: 656e 6428 6c6f 6320 3d20 2275 7070 6572  end(loc = "upper
+0001cc40: 206c 6566 7422 2c20 6262 6f78 5f74 6f5f   left", bbox_to_
+0001cc50: 616e 6368 6f72 3d28 312e 332c 2031 2e30  anchor=(1.3, 1.0
+0001cc60: 3529 290a 2020 2020 2020 2020 2020 2020  5)).            
+0001cc70: 2020 2020 2020 2020 706c 742e 636f 6c6f          plt.colo
+0001cc80: 7262 6172 2863 6d61 705f 7363 6174 2c20  rbar(cmap_scat, 
+0001cc90: 6c61 6265 6c3d 2265 6e76 2229 0a20 2020  label="env").   
+0001cca0: 2020 2020 2020 2020 2066 6967 2e73 686f           fig.sho
+0001ccb0: 7728 290a 0a20 2020 2020 2020 2072 6574  w()..        ret
+0001ccc0: 7572 6e20 6363 615f 6469 6374 0a0a 0a20  urn cca_dict... 
+0001ccd0: 2020 2023 206d 6574 686f 6420 666f 7220     # method for 
+0001cce0: 706c 6f74 7469 6e67 2074 6865 2073 7065  plotting the spe
+0001ccf0: 6369 6573 2028 6f72 2061 2073 7562 7365  cies (or a subse
+0001cd00: 7420 6f66 2069 7473 2069 6e64 6976 6964  t of its individ
+0001cd10: 7561 6c73 2c20 6279 2049 4429 0a20 2020  uals, by ID).   
+0001cd20: 2023 206f 6e20 746f 7020 6f66 2061 206c   # on top of a l
+0001cd30: 6179 6572 2028 6f72 206c 616e 6473 6361  ayer (or landsca
+0001cd40: 7065 290a 2020 2020 6465 6620 5f70 6c6f  pe).    def _plo
+0001cd50: 7428 7365 6c66 2c20 6c79 725f 6e75 6d3d  t(self, lyr_num=
+0001cd60: 4e6f 6e65 2c20 6c61 6e64 3d4e 6f6e 652c  None, land=None,
+0001cd70: 2068 6964 655f 6c61 6e64 3d46 616c 7365   hide_land=False
+0001cd80: 2c20 696e 6469 7669 6473 3d4e 6f6e 652c  , individs=None,
+0001cd90: 0a20 2020 2020 2020 2020 2020 2020 2074  .              t
+0001cda0: 6578 743d 4661 6c73 652c 2063 6f6c 6f72  ext=False, color
+0001cdb0: 3d27 626c 6163 6b27 2c20 6564 6765 5f63  ='black', edge_c
+0001cdc0: 6f6c 6f72 3d27 6661 6365 272c 2074 6578  olor='face', tex
+0001cdd0: 745f 636f 6c6f 723d 2762 6c61 636b 272c  t_color='black',
+0001cde0: 0a20 2020 2020 2020 2020 2020 2020 2063  .              c
+0001cdf0: 6261 723d 5472 7565 2c20 7369 7a65 3d32  bar=True, size=2
+0001ce00: 352c 2074 6578 745f 7369 7a65 3d39 2c20  5, text_size=9, 
+0001ce10: 6c61 6e64 5f63 6d61 703d 4e6f 6e65 2c20  land_cmap=None, 
+0001ce20: 7074 5f63 6d61 703d 4e6f 6e65 2c0a 2020  pt_cmap=None,.  
+0001ce30: 2020 2020 2020 2020 2020 2020 616c 7068              alph
+0001ce40: 613d 4661 6c73 652c 207a 6f6f 6d5f 7769  a=False, zoom_wi
+0001ce50: 6474 683d 4e6f 6e65 2c20 783d 4e6f 6e65  dth=None, x=None
+0001ce60: 2c20 793d 4e6f 6e65 2c20 766d 696e 3d4e  , y=None, vmin=N
+0001ce70: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0001ce80: 2020 2076 6d61 783d 4e6f 6e65 2c20 7469     vmax=None, ti
+0001ce90: 636b 733d 4e6f 6e65 2c20 6d61 736b 5f72  cks=None, mask_r
+0001cea0: 6173 743d 4e6f 6e65 2c20 616e 696d 6174  ast=None, animat
+0001ceb0: 653d 4661 6c73 652c 0a20 2020 2020 2020  e=False,.       
+0001cec0: 2020 2020 2020 2063 656c 6c5f 636f 6f72         cell_coor
+0001ced0: 6473 3d46 616c 7365 293a 0a20 2020 2020  ds=False):.     
+0001cee0: 2020 2023 2063 6f6e 7665 7274 2069 6e64     # convert ind
+0001cef0: 6976 6964 7320 746f 2061 206c 6973 7420  ivids to a list 
+0001cf00: 2869 6e20 6361 7365 2063 6f6d 6573 2069  (in case comes i
+0001cf10: 6e20 6173 2061 206e 756d 7079 2061 7272  n as a numpy arr
+0001cf20: 6179 290a 2020 2020 2020 2020 6966 2069  ay).        if i
+0001cf30: 6e64 6976 6964 7320 6973 206e 6f74 204e  ndivids is not N
+0001cf40: 6f6e 6520 616e 6420 6e6f 7420 6973 696e  one and not isin
+0001cf50: 7374 616e 6365 2869 6e64 6976 6964 732c  stance(individs,
+0001cf60: 206c 6973 7429 3a0a 2020 2020 2020 2020   list):.        
+0001cf70: 2020 2020 696e 6469 7669 6473 203d 206c      individs = l
+0001cf80: 6973 7428 696e 6469 7669 6473 290a 2020  ist(individs).  
+0001cf90: 2020 2020 2020 2320 6765 7420 636f 6f72        # get coor
+0001cfa0: 6473 0a20 2020 2020 2020 2063 6f6f 7264  ds.        coord
+0001cfb0: 7320 3d20 7365 6c66 2e5f 6765 745f 706c  s = self._get_pl
+0001cfc0: 6f74 5f63 6f6f 7264 7328 696e 6469 7669  ot_coords(indivi
+0001cfd0: 6473 3d69 6e64 6976 6964 732c 0a20 2020  ds=individs,.   
+0001cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d000: 2020 2020 6365 6c6c 5f63 6f6f 7264 733d      cell_coords=
+0001d010: 6365 6c6c 5f63 6f6f 7264 7329 0a20 2020  cell_coords).   
+0001d020: 2020 2020 2023 2067 6574 2074 6578 740a       # get text.
+0001d030: 2020 2020 2020 2020 6966 2074 6578 743a          if text:
+0001d040: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001d050: 696e 6469 7669 6473 2069 7320 4e6f 6e65  individs is None
+0001d060: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001d070: 2020 7465 7874 203d 205b 2a73 656c 665d    text = [*self]
+0001d080: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0001d090: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001d0a0: 2020 2074 6578 7420 3d20 696e 6469 7669     text = indivi
+0001d0b0: 6473 0a20 2020 2020 2020 2065 6c73 653a  ds.        else:
+0001d0c0: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
+0001d0d0: 7420 3d20 4e6f 6e65 0a20 2020 2020 2020  t = None.       
+0001d0e0: 2023 2073 6574 2074 6865 2070 6c74 5f6c   # set the plt_l
+0001d0f0: 696d 730a 2020 2020 2020 2020 706c 745f  ims.        plt_
+0001d100: 6c69 6d73 203d 2076 697a 2e5f 6765 745f  lims = viz._get_
+0001d110: 706c 745f 6c69 6d73 286c 616e 642c 2078  plt_lims(land, x
+0001d120: 2c20 792c 207a 6f6f 6d5f 7769 6474 6829  , y, zoom_width)
+0001d130: 0a20 2020 2020 2020 2023 2070 6c6f 7420  .        # plot 
+0001d140: 7468 6520 6c61 7965 7228 7329 0a20 2020  the layer(s).   
+0001d150: 2020 2020 2069 6620 6869 6465 5f6c 616e       if hide_lan
+0001d160: 643a 0a20 2020 2020 2020 2020 2020 2070  d:.            p
+0001d170: 6173 730a 2020 2020 2020 2020 656c 7365  ass.        else
+0001d180: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0001d190: 6765 7420 7468 6520 6c61 7965 7273 2720  get the layers' 
+0001d1a0: 766d 696e 2061 6e64 2076 6d61 7820 7661  vmin and vmax va
+0001d1b0: 6c75 6573 2c20 6966 2061 6e79 206f 6620  lues, if any of 
+0001d1c0: 7468 6520 6c61 7965 7273 2074 6f0a 2020  the layers to.  
+0001d1d0: 2020 2020 2020 2020 2020 2320 6265 2070            # be p
+0001d1e0: 6c6f 7474 6564 2068 6173 2061 2063 6861  lotted has a cha
+0001d1f0: 6e67 6520 6576 656e 740a 2020 2020 2020  nge event.      
+0001d200: 2020 2020 2020 6966 2028 286c 7972 5f6e        if ((lyr_n
+0001d210: 756d 2069 7320 4e6f 6e65 2061 6e64 206c  um is None and l
+0001d220: 616e 642e 5f63 6861 6e67 6572 2069 7320  and._changer is 
+0001d230: 6e6f 7420 4e6f 6e65 2920 6f72 0a20 2020  not None) or.   
+0001d240: 2020 2020 2020 2020 2020 2020 2028 6c61               (la
+0001d250: 6e64 2e5f 6368 616e 6765 7220 6973 206e  nd._changer is n
+0001d260: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+0001d270: 2020 2020 2020 2020 2061 6e64 206c 7972           and lyr
+0001d280: 5f6e 756d 2069 6e20 5b2a 6c61 6e64 2e5f  _num in [*land._
+0001d290: 6368 616e 6765 722e 6368 616e 6765 5f69  changer.change_i
+0001d2a0: 6e66 6f5d 2929 3a0a 2020 2020 2020 2020  nfo])):.        
+0001d2b0: 2020 2020 2020 2020 6966 206c 7972 5f6e          if lyr_n
+0001d2c0: 756d 2069 7320 4e6f 6e65 3a0a 2020 2020  um is None:.    
+0001d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d2e0: 6c61 6e64 5f76 6d69 6e20 3d20 5b6c 7972  land_vmin = [lyr
+0001d2f0: 2e5f 7363 616c 655f 6d69 6e20 666f 7220  ._scale_min for 
+0001d300: 6c79 7220 696e 206c 616e 642e 7661 6c75  lyr in land.valu
+0001d310: 6573 2829 5d0a 2020 2020 2020 2020 2020  es()].          
+0001d320: 2020 2020 2020 2020 2020 6c61 6e64 5f76            land_v
+0001d330: 6d61 7820 3d20 5b6c 7972 2e5f 7363 616c  max = [lyr._scal
+0001d340: 655f 6d61 7820 666f 7220 6c79 7220 696e  e_max for lyr in
+0001d350: 206c 616e 642e 7661 6c75 6573 2829 5d0a   land.values()].
+0001d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d370: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001d380: 2020 2020 2020 2020 2020 6c61 6e64 5f76            land_v
+0001d390: 6d69 6e20 3d20 5b6c 616e 645b 6c79 725f  min = [land[lyr_
+0001d3a0: 6e75 6d5d 2e5f 7363 616c 655f 6d69 6e5d  num]._scale_min]
+0001d3b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d3c0: 2020 2020 206c 616e 645f 766d 6178 203d       land_vmax =
+0001d3d0: 205b 6c61 6e64 5b6c 7972 5f6e 756d 5d2e   [land[lyr_num].
+0001d3e0: 5f73 6361 6c65 5f6d 6178 5d0a 2020 2020  _scale_max].    
+0001d3f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001d400: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+0001d410: 6e64 5f76 6d69 6e20 3d20 6c61 6e64 5f76  nd_vmin = land_v
+0001d420: 6d61 7820 3d20 4e6f 6e65 0a20 2020 2020  max = None.     
+0001d430: 2020 2020 2020 2076 697a 2e5f 706c 6f74         viz._plot
+0001d440: 5f72 6173 7465 7273 286c 616e 642c 206c  _rasters(land, l
+0001d450: 7972 5f6e 756d 3d6c 7972 5f6e 756d 2c0a  yr_num=lyr_num,.
+0001d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d470: 2020 2020 2020 2020 2020 2020 2020 6362                cb
+0001d480: 6172 3d63 6261 722c 2063 6d61 703d 6c61  ar=cbar, cmap=la
+0001d490: 6e64 5f63 6d61 702c 2070 6c74 5f6c 696d  nd_cmap, plt_lim
+0001d4a0: 733d 706c 745f 6c69 6d73 2c0a 2020 2020  s=plt_lims,.    
+0001d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4c0: 2020 2020 2020 2020 2020 7469 636b 733d            ticks=
+0001d4d0: 7469 636b 732c 206d 6173 6b5f 7261 7374  ticks, mask_rast
+0001d4e0: 3d6d 6173 6b5f 7261 7374 2c0a 2020 2020  =mask_rast,.    
+0001d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d500: 2020 2020 2020 2020 2020 766d 696e 3d6c            vmin=l
+0001d510: 616e 645f 766d 696e 2c20 766d 6178 3d6c  and_vmin, vmax=l
+0001d520: 616e 645f 766d 6178 290a 2020 2020 2020  and_vmax).      
+0001d530: 2020 2320 616e 6420 706c 6f74 2074 6865    # and plot the
+0001d540: 2069 6e64 6976 6964 7561 6c73 0a20 2020   individuals.   
+0001d550: 2020 2020 2070 6f69 6e74 7320 3d20 7669       points = vi
+0001d560: 7a2e 5f70 6c6f 745f 706f 696e 7473 2863  z._plot_points(c
+0001d570: 6f6f 7264 732c 206c 7972 5f6e 756d 3d6c  oords, lyr_num=l
+0001d580: 7972 5f6e 756d 2c20 636f 6c6f 723d 636f  yr_num, color=co
+0001d590: 6c6f 722c 0a20 2020 2020 2020 2020 2020  lor,.           
+0001d5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5b0: 2020 2020 2020 2065 6467 655f 636f 6c6f         edge_colo
+0001d5c0: 723d 6564 6765 5f63 6f6c 6f72 2c0a 2020  r=edge_color,.  
+0001d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5f0: 7465 7874 5f63 6f6c 6f72 3d74 6578 745f  text_color=text_
+0001d600: 636f 6c6f 722c 2073 697a 653d 7369 7a65  color, size=size
+0001d610: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d630: 2020 2020 7465 7874 5f73 697a 653d 7465      text_size=te
+0001d640: 7874 5f73 697a 652c 2061 6c70 6861 3d61  xt_size, alpha=a
+0001d650: 6c70 6861 2c0a 2020 2020 2020 2020 2020  lpha,.          
+0001d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d670: 2020 2020 2020 2020 7465 7874 3d74 6578          text=tex
+0001d680: 742c 2070 6c74 5f6c 696d 733d 706c 745f  t, plt_lims=plt_
+0001d690: 6c69 6d73 2c0a 2020 2020 2020 2020 2020  lims,.          
+0001d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d6b0: 2020 2020 2020 2020 7074 5f63 6d61 703d          pt_cmap=
+0001d6c0: 7074 5f63 6d61 702c 2076 6d69 6e3d 766d  pt_cmap, vmin=vm
+0001d6d0: 696e 2c20 766d 6178 3d76 6d61 782c 0a20  in, vmax=vmax,. 
+0001d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d700: 2061 6e69 6d61 7465 3d61 6e69 6d61 7465   animate=animate
+0001d710: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0001d720: 2070 6f69 6e74 730a 0a0a 2020 2020 236d   points...    #m
+0001d730: 6574 686f 6420 666f 7220 706c 6f74 7469  ethod for plotti
+0001d740: 6e67 2074 6865 2073 7065 6369 6573 206f  ng the species o
+0001d750: 6e20 746f 7020 6f66 2069 7473 2065 7374  n top of its est
+0001d760: 696d 6174 6564 0a20 2020 2023 7370 6563  imated.    #spec
+0001d770: 6965 732d 6465 6e73 6974 7920 7261 7374  ies-density rast
+0001d780: 6572 0a20 2020 2064 6566 205f 706c 6f74  er.    def _plot
+0001d790: 5f64 656e 7369 7479 2873 656c 662c 206c  _density(self, l
+0001d7a0: 616e 642c 206e 6f72 6d61 6c69 7a65 3d46  and, normalize=F
+0001d7b0: 616c 7365 2c20 696e 6469 7669 6473 3d4e  alse, individs=N
+0001d7c0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0001d7d0: 2074 6578 743d 4661 6c73 652c 2063 6f6c   text=False, col
+0001d7e0: 6f72 3d27 626c 6163 6b27 2c20 6564 6765  or='black', edge
+0001d7f0: 5f63 6f6c 6f72 3d27 6661 6365 272c 0a20  _color='face',. 
+0001d800: 2020 2020 2020 2020 2020 2074 6578 745f             text_
+0001d810: 636f 6c6f 723d 2762 6c61 636b 272c 2073  color='black', s
+0001d820: 697a 653d 3235 2c20 7465 7874 5f73 697a  ize=25, text_siz
+0001d830: 6520 3d20 392c 0a20 2020 2020 2020 2020  e = 9,.         
+0001d840: 2020 2061 6c70 6861 3d30 2e35 2c20 7a6f     alpha=0.5, zo
+0001d850: 6f6d 5f77 6964 7468 3d4e 6f6e 652c 2078  om_width=None, x
+0001d860: 3d4e 6f6e 652c 2079 3d4e 6f6e 652c 2074  =None, y=None, t
+0001d870: 6963 6b73 3d4e 6f6e 652c 0a20 2020 2020  icks=None,.     
+0001d880: 2020 2020 2020 206d 6173 6b5f 7261 7374         mask_rast
+0001d890: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0001d8a0: 6173 7365 7274 2074 7970 6528 6e6f 726d  assert type(norm
+0001d8b0: 616c 697a 6529 2069 7320 626f 6f6c 2c20  alize) is bool, 
+0001d8c0: 2822 5468 6520 276e 6f72 6d61 6c69 7a65  ("The 'normalize
+0001d8d0: 2720 6172 6775 6d65 6e74 2074 616b 6573  ' argument takes
+0001d8e0: 2022 0a20 2020 2020 2020 2020 2020 2022   ".            "
+0001d8f0: 6120 626f 6f6c 6561 6e20 7661 6c75 652e  a boolean value.
+0001d900: 5c6e 2229 0a20 2020 2020 2020 2023 7570  \n").        #up
+0001d910: 6461 7465 2074 6865 2073 7065 6369 6573  date the species
+0001d920: 2720 636f 6f72 6469 6e61 7465 7320 616e  ' coordinates an
+0001d930: 6420 6365 6c6c 732c 2069 6e20 6361 7365  d cells, in case
+0001d940: 2069 7420 6861 736e 2774 0a20 2020 2020   it hasn't.     
+0001d950: 2020 2023 6265 656e 2075 7064 6174 6564     #been updated
+0001d960: 2073 696e 6365 2073 6f6d 6520 696e 7465   since some inte
+0001d970: 726e 616c 206f 7220 6d61 6e75 616c 2063  rnal or manual c
+0001d980: 6861 6e67 6573 2069 6e20 706f 7075 6c61  hanges in popula
+0001d990: 7469 6f6e 2d73 697a 650a 2020 2020 2020  tion-size.      
+0001d9a0: 2020 2368 6176 6520 6f63 6375 7272 6564    #have occurred
+0001d9b0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+0001d9c0: 6574 5f63 6f6f 7264 735f 616e 645f 6365  et_coords_and_ce
+0001d9d0: 6c6c 7328 290a 2020 2020 2020 2020 6465  lls().        de
+0001d9e0: 6e73 203d 2073 656c 662e 5f63 616c 635f  ns = self._calc_
+0001d9f0: 6465 6e73 6974 7928 6e6f 726d 616c 697a  density(normaliz
+0001da00: 6520 3d20 6e6f 726d 616c 697a 6529 0a20  e = normalize). 
+0001da10: 2020 2020 2020 2070 6c74 5f6c 696d 7320         plt_lims 
+0001da20: 3d20 7669 7a2e 5f67 6574 5f70 6c74 5f6c  = viz._get_plt_l
+0001da30: 696d 7328 6c61 6e64 2c20 782c 2079 2c20  ims(land, x, y, 
+0001da40: 7a6f 6f6d 5f77 6964 7468 290a 2020 2020  zoom_width).    
+0001da50: 2020 2020 6966 206e 6f72 6d61 6c69 7a65      if normalize
+0001da60: 3a0a 2020 2020 2020 2020 2020 2020 7669  :.            vi
+0001da70: 7a2e 5f70 6c6f 745f 7261 7374 6572 7328  z._plot_rasters(
+0001da80: 6465 6e73 2c20 706c 745f 6c69 6d73 203d  dens, plt_lims =
+0001da90: 2070 6c74 5f6c 696d 732c 206c 7972 5f6e   plt_lims, lyr_n
+0001daa0: 616d 6520 3d20 2764 656e 7369 7479 272c  ame = 'density',
+0001dab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001dac0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0001dad0: 6963 6b73 3d74 6963 6b73 2c20 6d61 736b  icks=ticks, mask
+0001dae0: 5f72 6173 743d 6d61 736b 5f72 6173 7429  _rast=mask_rast)
+0001daf0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0001db00: 2020 2020 2020 2020 2020 2076 697a 2e5f             viz._
+0001db10: 706c 6f74 5f72 6173 7465 7273 2864 656e  plot_rasters(den
+0001db20: 732c 2070 6c74 5f6c 696d 7320 3d20 706c  s, plt_lims = pl
+0001db30: 745f 6c69 6d73 2c20 766d 6178 203d 2064  t_lims, vmax = d
+0001db40: 656e 732e 6d61 7828 292c 0a20 2020 2020  ens.max(),.     
+0001db50: 2020 2020 2020 2020 2020 206c 7972 5f6e             lyr_n
+0001db60: 616d 6520 3d20 2764 656e 7369 7479 272c  ame = 'density',
+0001db70: 2074 6963 6b73 3d74 6963 6b73 2c20 6d61   ticks=ticks, ma
+0001db80: 736b 5f72 6173 743d 6d61 736b 5f72 6173  sk_rast=mask_ras
+0001db90: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+0001dba0: 5f70 6c6f 7428 6869 6465 5f6c 616e 643d  _plot(hide_land=
+0001dbb0: 5472 7565 2c20 696e 6469 7669 6473 203d  True, individs =
+0001dbc0: 2069 6e64 6976 6964 732c 2074 6578 7420   individs, text 
+0001dbd0: 3d20 7465 7874 2c0a 2020 2020 2020 2020  = text,.        
+0001dbe0: 2020 2020 636f 6c6f 723d 636f 6c6f 722c      color=color,
+0001dbf0: 2065 6467 655f 636f 6c6f 7220 3d20 6564   edge_color = ed
+0001dc00: 6765 5f63 6f6c 6f72 2c20 7465 7874 5f63  ge_color, text_c
+0001dc10: 6f6c 6f72 203d 2074 6578 745f 636f 6c6f  olor = text_colo
+0001dc20: 722c 0a20 2020 2020 2020 2020 2020 2073  r,.            s
+0001dc30: 697a 653d 7369 7a65 2c20 7465 7874 5f73  ize=size, text_s
+0001dc40: 697a 6520 3d20 7465 7874 5f73 697a 652c  ize = text_size,
+0001dc50: 2061 6c70 6861 3d61 6c70 6861 2c0a 2020   alpha=alpha,.  
+0001dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc80: 2020 7a6f 6f6d 5f77 6964 7468 203d 207a    zoom_width = z
+0001dc90: 6f6f 6d5f 7769 6474 682c 2078 203d 2078  oom_width, x = x
+0001dca0: 2c20 7920 3d20 7929 0a0a 0a20 2020 2023  , y = y)...    #
+0001dcb0: 206d 6574 686f 6420 666f 7220 706c 6f74   method for plot
+0001dcc0: 7469 6e67 2069 6e64 6976 6964 7561 6c73  ting individuals
+0001dcd0: 2063 6f6c 6f72 6564 2062 7920 7468 6569   colored by thei
+0001dce0: 7220 6765 6e6f 7479 7065 2061 7420 6120  r genotype at a 
+0001dcf0: 6c6f 6375 730a 2020 2020 6465 6620 5f70  locus.    def _p
+0001dd00: 6c6f 745f 6765 6e6f 7479 7065 2873 656c  lot_genotype(sel
+0001dd10: 662c 206c 6f63 7573 2c20 6c79 725f 6e75  f, locus, lyr_nu
+0001dd20: 6d3d 4e6f 6e65 2c20 6c61 6e64 3d4e 6f6e  m=None, land=Non
+0001dd30: 652c 2069 6e64 6976 6964 733d 4e6f 6e65  e, individs=None
+0001dd40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001dd50: 2020 2020 2020 2020 2074 6578 743d 4661           text=Fa
+0001dd60: 6c73 652c 2073 697a 653d 3235 2c20 7465  lse, size=25, te
+0001dd70: 7874 5f73 697a 6520 3d20 392c 2065 6467  xt_size = 9, edg
+0001dd80: 655f 636f 6c6f 723d 2762 6c61 636b 272c  e_color='black',
+0001dd90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001dda0: 2020 2020 2020 2020 7465 7874 5f63 6f6c          text_col
+0001ddb0: 6f72 3d27 626c 6163 6b27 2c20 6362 6172  or='black', cbar
+0001ddc0: 3d54 7275 652c 2061 6c70 6861 3d31 2c0a  =True, alpha=1,.
+0001ddd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dde0: 2020 2020 2020 2062 795f 646f 6d69 6e61         by_domina
+0001ddf0: 6e63 653d 4661 6c73 652c 207a 6f6f 6d5f  nce=False, zoom_
+0001de00: 7769 6474 683d 4e6f 6e65 2c20 783d 4e6f  width=None, x=No
+0001de10: 6e65 2c20 793d 4e6f 6e65 2c0a 2020 2020  ne, y=None,.    
+0001de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de30: 2020 2074 6963 6b73 3d4e 6f6e 652c 206d     ticks=None, m
+0001de40: 6173 6b5f 7261 7374 3d4e 6f6e 6529 3a0a  ask_rast=None):.
+0001de50: 0a20 2020 2020 2020 2067 656e 6f74 7970  .        genotyp
+0001de60: 6573 203d 2073 656c 662e 5f67 6574 5f67  es = self._get_g
+0001de70: 656e 6f74 7970 6573 286c 6f63 693d 5b6c  enotypes(loci=[l
+0001de80: 6f63 7573 5d2c 2069 6e64 6976 6964 733d  ocus], individs=
+0001de90: 696e 6469 7669 6473 2c0a 2020 2020 2020  individs,.      
+0001dea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dec0: 2020 6269 616c 6c65 6c69 633d 4661 6c73    biallelic=Fals
+0001ded0: 652c 2061 735f 6469 6374 3d54 7275 6529  e, as_dict=True)
+0001dee0: 0a20 2020 2020 2020 2069 6620 6279 5f64  .        if by_d
+0001def0: 6f6d 696e 616e 6365 203d 3d20 5472 7565  ominance == True
+0001df00: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0001df10: 206c 6f63 7573 2069 6e20 7365 6c66 2e67   locus in self.g
+0001df20: 656e 5f61 7263 682e 6e6f 6e6e 6575 745f  en_arch.nonneut_
+0001df30: 6c6f 6369 3a0a 2020 2020 2020 2020 2020  loci:.          
+0001df40: 2020 2020 2020 646f 6d20 3d20 7365 6c66        dom = self
+0001df50: 2e67 656e 5f61 7263 682e 646f 6d5b 6c6f  .gen_arch.dom[lo
+0001df60: 6375 735d 0a20 2020 2020 2020 2020 2020  cus].           
+0001df70: 2020 2020 2023 204e 4f54 453a 2077 6f75       # NOTE: wou
+0001df80: 6c64 2062 6520 7369 6d70 6c65 7220 746f  ld be simpler to
+0001df90: 206a 7573 7420 7573 6520 6e70 2e63 6569   just use np.cei
+0001dfa0: 6c20 6865 7265 2e2e 2e0a 2020 2020 2020  l here....      
+0001dfb0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+0001dfc0: 2020 646f 6e27 7420 7365 6520 7768 7920    don't see why 
+0001dfd0: 4920 6469 646e 2774 2e2e 2e3f 0a20 2020  I didn't...?.   
+0001dfe0: 2020 2020 2020 2020 2020 2020 2067 656e               gen
+0001dff0: 6f74 7970 6573 203d 207b 693a 6e70 2e63  otypes = {i:np.c
+0001e000: 6c69 7028 6774 202a 2028 3120 2b20 646f  lip(gt * (1 + do
+0001e010: 6d29 2c0a 2020 2020 2020 2020 2020 2020  m),.            
+0001e020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e030: 2020 2020 2020 2020 2020 2061 5f6d 696e             a_min
+0001e040: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+0001e050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e060: 2020 2020 2020 2020 2020 2020 2020 615f                a_
+0001e070: 6d61 783d 3129 2066 6f72 2069 2c20 6774  max=1) for i, gt
+0001e080: 2069 6e20 6765 6e6f 7479 7065 732e 6974   in genotypes.it
+0001e090: 656d 7328 297d 0a20 2020 2020 2020 2020  ems()}.         
+0001e0a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001e0b0: 2020 2020 2020 2020 2070 7269 6e74 2828           print((
+0001e0c0: 275c 6e5c 7457 4152 4e49 4e47 3a20 5468  '\n\tWARNING: Th
+0001e0d0: 6520 6279 5f64 6f6d 696e 616e 6365 2061  e by_dominance a
+0001e0e0: 7267 756d 656e 7420 6973 2054 7275 652c  rgument is True,
+0001e0f0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+0001e100: 2020 2020 2020 2020 2020 2762 7574 2061            'but a
+0001e110: 206e 6575 7472 616c 206c 6f63 7573 2077   neutral locus w
+0001e120: 6173 2063 686f 7365 6e2c 2027 0a20 2020  as chosen, '.   
+0001e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e140: 2020 2020 2773 6f20 7468 6520 6172 6775      'so the argu
+0001e150: 6d65 6e74 2077 6173 206e 6f74 2075 7365  ment was not use
+0001e160: 642e 5c6e 2729 290a 0a20 2020 2020 2020  d.\n'))..       
+0001e170: 2023 206a 7573 7420 6173 7369 676e 2062   # just assign b
+0001e180: 6c61 636b 2c20 6772 6179 2c20 616e 6420  lack, gray, and 
+0001e190: 7768 6974 6520 2873 696e 6365 2074 6865  white (since the
+0001e1a0: 7265 2773 206e 6f20 7265 6173 6f6e 0a20  re's no reason. 
+0001e1b0: 2020 2020 2020 2023 206e 6563 6573 7361         # necessa
+0001e1c0: 7269 6c79 2074 6861 7420 7468 6573 6520  rily that these 
+0001e1d0: 7368 6f75 6c64 2062 6520 6d61 7070 6564  should be mapped
+0001e1e0: 2074 6f20 6120 6365 7274 6169 6e20 6c61   to a certain la
+0001e1f0: 7965 722c 2074 6865 2077 6179 0a20 2020  yer, the way.   
+0001e200: 2020 2020 2023 2070 6865 6e6f 7479 7065       # phenotype
+0001e210: 2073 686f 756c 640a 2020 2020 2020 2020   should.        
+0001e220: 636f 6c6f 7273 203d 205b 2723 3030 3030  colors = ['#0000
+0001e230: 3030 272c 2027 2338 3038 3038 3027 2c20  00', '#808080', 
+0001e240: 2723 4646 4646 4646 275d 0a0a 2020 2020  '#FFFFFF']..    
+0001e250: 2020 2020 666f 7220 6e2c 2067 656e 6f74      for n, genot
+0001e260: 7970 6520 696e 2065 6e75 6d65 7261 7465  ype in enumerate
+0001e270: 285b 302e 302c 2030 2e35 2c20 312e 305d  ([0.0, 0.5, 1.0]
+0001e280: 293a 0a20 2020 2020 2020 2020 2020 2067  ):.            g
+0001e290: 656e 6f74 7970 655f 696e 6469 7669 6473  enotype_individs
+0001e2a0: 203d 205b 6920 666f 7220 692c 2067 2069   = [i for i, g i
+0001e2b0: 6e20 6765 6e6f 7479 7065 732e 6974 656d  n genotypes.item
+0001e2c0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+0001e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e2e0: 2020 2020 2020 2020 2020 2029 2069 6620             ) if 
+0001e2f0: 6e70 2e61 746c 6561 7374 5f31 6428 6729  np.atleast_1d(g)
+0001e300: 5b30 5d20 3d3d 2067 656e 6f74 7970 655d  [0] == genotype]
+0001e310: 0a20 2020 2020 2020 2020 2020 2023 2077  .            # w
+0001e320: 696c 6c20 6869 6465 2074 6865 206c 616e  ill hide the lan
+0001e330: 6420 6966 2074 6869 7320 6973 206e 6f74  d if this is not
+0001e340: 2074 6865 2066 6972 7374 2070 6c6f 7420   the first plot 
+0001e350: 6d61 6465 0a20 2020 2020 2020 2020 2020  made.           
+0001e360: 2068 6964 655f 6c61 6e64 203d 206e 203e   hide_land = n >
+0001e370: 2030 0a20 2020 2020 2020 2020 2020 2023   0.            #
+0001e380: 2070 6c6f 7420 6966 2074 6865 7265 2061   plot if there a
+0001e390: 7265 2061 6e79 2069 6e64 6976 6964 7561  re any individua
+0001e3a0: 6c73 206f 6620 7468 6973 2067 656e 6f74  ls of this genot
+0001e3b0: 7970 650a 2020 2020 2020 2020 2020 2020  ype.            
+0001e3c0: 6966 206c 656e 2867 656e 6f74 7970 655f  if len(genotype_
+0001e3d0: 696e 6469 7669 6473 2920 3e3d 2031 3a0a  individs) >= 1:.
+0001e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e3f0: 7365 6c66 2e5f 706c 6f74 286c 7972 5f6e  self._plot(lyr_n
+0001e400: 756d 3d6c 7972 5f6e 756d 2c20 6c61 6e64  um=lyr_num, land
+0001e410: 3d6c 616e 642c 2068 6964 655f 6c61 6e64  =land, hide_land
+0001e420: 3d68 6964 655f 6c61 6e64 2c0a 2020 2020  =hide_land,.    
+0001e430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e440: 2020 2020 2020 2069 6e64 6976 6964 733d         individs=
+0001e450: 6765 6e6f 7479 7065 5f69 6e64 6976 6964  genotype_individ
+0001e460: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0001e470: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0001e480: 7874 3d74 6578 742c 2063 6f6c 6f72 3d63  xt=text, color=c
+0001e490: 6f6c 6f72 735b 6e5d 2c20 6564 6765 5f63  olors[n], edge_c
+0001e4a0: 6f6c 6f72 3d65 6467 655f 636f 6c6f 722c  olor=edge_color,
+0001e4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e4c0: 2020 2020 2020 2020 2020 2020 7465 7874              text
+0001e4d0: 5f63 6f6c 6f72 3d74 6578 745f 636f 6c6f  _color=text_colo
+0001e4e0: 722c 2063 6261 723d 6362 6172 2c0a 2020  r, cbar=cbar,.  
+0001e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e500: 2020 2020 2020 2020 2073 697a 653d 7369           size=si
+0001e510: 7a65 2c20 7465 7874 5f73 697a 653d 7465  ze, text_size=te
+0001e520: 7874 5f73 697a 652c 2061 6c70 6861 3d61  xt_size, alpha=a
+0001e530: 6c70 6861 2c0a 2020 2020 2020 2020 2020  lpha,.          
+0001e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e550: 207a 6f6f 6d5f 7769 6474 683d 7a6f 6f6d   zoom_width=zoom
+0001e560: 5f77 6964 7468 2c20 783d 782c 2079 3d79  _width, x=x, y=y
+0001e570: 2c20 766d 696e 3d30 2c20 766d 6178 3d31  , vmin=0, vmax=1
+0001e580: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001e590: 2020 2020 2020 2020 2020 2020 2074 6963               tic
+0001e5a0: 6b73 3d74 6963 6b73 2c20 6d61 736b 5f72  ks=ticks, mask_r
+0001e5b0: 6173 743d 6d61 736b 5f72 6173 7429 0a0a  ast=mask_rast)..
+0001e5c0: 0a20 2020 2023 206d 6574 686f 6420 666f  .    # method fo
+0001e5d0: 7220 706c 6f74 7469 6e67 2069 6e64 6976  r plotting indiv
+0001e5e0: 6964 7561 6c73 2063 6f6c 6f72 6564 2062  iduals colored b
+0001e5f0: 7920 7468 6569 7220 7068 656e 6f74 7970  y their phenotyp
+0001e600: 6573 0a20 2020 2023 666f 7220 6120 6769  es.    #for a gi
+0001e610: 7665 6e20 7472 6169 740a 2020 2020 6465  ven trait.    de
+0001e620: 6620 5f70 6c6f 745f 7068 656e 6f74 7970  f _plot_phenotyp
+0001e630: 6528 7365 6c66 2c20 7472 6169 742c 206c  e(self, trait, l
+0001e640: 7972 5f6e 756d 3d4e 6f6e 652c 206c 616e  yr_num=None, lan
+0001e650: 643d 4e6f 6e65 2c0a 2020 2020 2020 2020  d=None,.        
+0001e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e670: 696e 6469 7669 6473 3d4e 6f6e 652c 2074  individs=None, t
+0001e680: 6578 743d 4661 6c73 652c 2073 697a 653d  ext=False, size=
+0001e690: 3235 2c20 7465 7874 5f73 697a 653d 392c  25, text_size=9,
+0001e6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e6b0: 2020 2020 2020 2020 2065 6467 655f 636f           edge_co
+0001e6c0: 6c6f 723d 2762 6c61 636b 272c 2074 6578  lor='black', tex
+0001e6d0: 745f 636f 6c6f 723d 2762 6c61 636b 272c  t_color='black',
+0001e6e0: 2063 6261 723d 5472 7565 2c0a 2020 2020   cbar=True,.    
+0001e6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e700: 2020 2020 616c 7068 613d 312c 207a 6f6f      alpha=1, zoo
+0001e710: 6d5f 7769 6474 683d 4e6f 6e65 2c20 783d  m_width=None, x=
+0001e720: 4e6f 6e65 2c20 793d 4e6f 6e65 2c0a 2020  None, y=None,.  
 0001e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e740: 2065 6467 655f 636f 6c6f 7220 3d20 6564   edge_color = ed
-0001e750: 6765 5f63 6f6c 6f72 2c20 7465 7874 5f63  ge_color, text_c
-0001e760: 6f6c 6f72 203d 2074 6578 745f 636f 6c6f  olor = text_colo
-0001e770: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0001e780: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001e790: 6261 7220 3d20 6362 6172 2c20 7369 7a65  bar = cbar, size
-0001e7a0: 203d 2073 697a 652c 2074 6578 745f 7369   = size, text_si
-0001e7b0: 7a65 203d 2074 6578 745f 7369 7a65 2c0a  ze = text_size,.
-0001e7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e7d0: 2020 2020 2020 2020 2020 2020 616c 7068              alph
-0001e7e0: 6120 3d20 616c 7068 612c 207a 6f6f 6d5f  a = alpha, zoom_
-0001e7f0: 7769 6474 6820 3d20 7a6f 6f6d 5f77 6964  width = zoom_wid
-0001e800: 7468 2c20 7820 3d20 782c 0a20 2020 2020  th, x = x,.     
-0001e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e820: 2020 2020 2020 2079 203d 2079 2c20 766d         y = y, vm
-0001e830: 696e 203d 2030 2c20 766d 6178 203d 2031  in = 0, vmax = 1
-0001e840: 2c20 7469 636b 733d 7469 636b 732c 0a20  , ticks=ticks,. 
-0001e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e860: 2020 2020 2020 2020 2020 206d 6173 6b5f             mask_
-0001e870: 7261 7374 3d6d 6173 6b5f 7261 7374 2c20  rast=mask_rast, 
-0001e880: 616e 696d 6174 653d 616e 696d 6174 6529  animate=animate)
-0001e890: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001e8a0: 2070 6f69 6e74 730a 0a0a 2020 2020 2320   points...    # 
-0001e8b0: 6d65 7468 6f64 2066 6f72 2070 6c6f 7474  method for plott
-0001e8c0: 696e 6720 696e 6469 7669 6475 616c 7320  ing individuals 
-0001e8d0: 636f 6c6f 7265 6420 6279 2074 6865 6972  colored by their
-0001e8e0: 206f 7665 7261 6c6c 2066 6974 6e65 7373   overall fitness
-0001e8f0: 6573 2c0a 2020 2020 236f 7220 6279 2074  es,.    #or by t
-0001e900: 6865 6972 2066 6974 6e65 7373 6573 2066  heir fitnesses f
-0001e910: 6f72 2061 2073 696e 676c 6520 7472 6169  or a single trai
-0001e920: 7420 2869 6620 7472 6169 7420 6973 206e  t (if trait is n
-0001e930: 6f74 204e 6f6e 6529 0a20 2020 2064 6566  ot None).    def
-0001e940: 205f 706c 6f74 5f66 6974 6e65 7373 2873   _plot_fitness(s
-0001e950: 656c 662c 2074 7274 5f6e 756d 3d4e 6f6e  elf, trt_num=Non
-0001e960: 652c 206c 7972 5f6e 756d 3d4e 6f6e 652c  e, lyr_num=None,
-0001e970: 206c 616e 643d 4e6f 6e65 2c0a 2020 2020   land=None,.    
-0001e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e990: 2020 696e 6469 7669 6473 3d4e 6f6e 652c    individs=None,
-0001e9a0: 2074 6578 743d 4661 6c73 652c 2070 6865   text=False, phe
-0001e9b0: 6e6f 7479 7065 5f74 6578 743d 4661 6c73  notype_text=Fals
-0001e9c0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0001e9d0: 2020 2020 2020 2020 2070 6865 6e6f 7479           phenoty
-0001e9e0: 7065 5f74 6578 745f 636f 6c6f 723d 2762  pe_text_color='b
-0001e9f0: 6c61 636b 272c 2066 6974 6e65 7373 5f74  lack', fitness_t
-0001ea00: 6578 743d 4661 6c73 652c 0a20 2020 2020  ext=False,.     
+0001e740: 2020 2020 2020 7469 636b 733d 4e6f 6e65        ticks=None
+0001e750: 2c20 6d61 736b 5f72 6173 743d 4e6f 6e65  , mask_rast=None
+0001e760: 2c20 616e 696d 6174 653d 4661 6c73 6529  , animate=False)
+0001e770: 3a0a 0a20 2020 2020 2020 2023 2067 6574  :..        # get
+0001e780: 2074 6865 2074 7261 6974 2773 206c 7972   the trait's lyr
+0001e790: 5f6e 756d 2c20 6966 206e 6f20 6c79 725f  _num, if no lyr_
+0001e7a0: 6e75 6d20 7072 6f76 6964 6564 0a20 2020  num provided.   
+0001e7b0: 2020 2020 206c 7972 5f6e 756d 203d 2073       lyr_num = s
+0001e7c0: 656c 662e 6765 6e5f 6172 6368 2e74 7261  elf.gen_arch.tra
+0001e7d0: 6974 735b 7472 6169 745d 2e6c 7972 5f6e  its[trait].lyr_n
+0001e7e0: 756d 0a0a 2020 2020 2020 2020 7a20 3d20  um..        z = 
+0001e7f0: 4f44 287a 6970 285b 2a73 656c 665d 2c20  OD(zip([*self], 
+0001e800: 7365 6c66 2e5f 6765 745f 7a28 295b 3a2c  self._get_z()[:,
+0001e810: 2074 7261 6974 5d29 290a 2020 2020 2020   trait])).      
+0001e820: 2020 6966 2069 6e64 6976 6964 7320 6973    if individs is
+0001e830: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0001e840: 2020 2020 2020 207a 203d 207b 693a 2076         z = {i: v
+0001e850: 2066 6f72 2069 2c20 7620 696e 207a 2e69   for i, v in z.i
+0001e860: 7465 6d73 2829 2069 6620 6920 696e 2069  tems() if i in i
+0001e870: 6e64 6976 6964 737d 0a0a 2020 2020 2020  ndivids}..      
+0001e880: 2020 2320 6765 7420 7468 6520 636f 7272    # get the corr
+0001e890: 6563 7420 636d 6170 2066 6f72 2074 6869  ect cmap for thi
+0001e8a0: 7320 7472 6169 7427 7320 6c61 7965 720a  s trait's layer.
+0001e8b0: 2020 2020 2020 2020 7074 5f63 6d61 7020          pt_cmap 
+0001e8c0: 3d20 7669 7a2e 5f63 686f 6f73 655f 636d  = viz._choose_cm
+0001e8d0: 6170 2873 656c 662e 6765 6e5f 6172 6368  ap(self.gen_arch
+0001e8e0: 2e74 7261 6974 735b 7472 6169 745d 2e6c  .traits[trait].l
+0001e8f0: 7972 5f6e 756d 290a 0a20 2020 2020 2020  yr_num)..       
+0001e900: 2070 6f69 6e74 7320 3d20 7365 6c66 2e5f   points = self._
+0001e910: 706c 6f74 286c 7972 5f6e 756d 203d 206c  plot(lyr_num = l
+0001e920: 7972 5f6e 756d 2c20 6c61 6e64 203d 206c  yr_num, land = l
+0001e930: 616e 642c 0a20 2020 2020 2020 2020 2020  and,.           
+0001e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e950: 2069 6e64 6976 6964 7320 3d20 696e 6469   individs = indi
+0001e960: 7669 6473 2c20 7465 7874 203d 2074 6578  vids, text = tex
+0001e970: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+0001e980: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001e990: 6f6c 6f72 203d 206c 6973 7428 7a2e 7661  olor = list(z.va
+0001e9a0: 6c75 6573 2829 292c 2070 745f 636d 6170  lues()), pt_cmap
+0001e9b0: 203d 2070 745f 636d 6170 2c0a 2020 2020   = pt_cmap,.    
+0001e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e9d0: 2020 2020 2020 2020 6564 6765 5f63 6f6c          edge_col
+0001e9e0: 6f72 203d 2065 6467 655f 636f 6c6f 722c  or = edge_color,
+0001e9f0: 2074 6578 745f 636f 6c6f 7220 3d20 7465   text_color = te
+0001ea00: 7874 5f63 6f6c 6f72 2c0a 2020 2020 2020  xt_color,.      
 0001ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea20: 2066 6974 6e65 7373 5f74 6578 745f 636f   fitness_text_co
-0001ea30: 6c6f 723d 2723 3333 3333 3333 272c 2073  lor='#333333', s
-0001ea40: 697a 653d 3130 302c 2074 6578 745f 7369  ize=100, text_si
-0001ea50: 7a65 203d 2039 2c0a 2020 2020 2020 2020  ze = 9,.        
-0001ea60: 2020 2020 2020 2020 2020 2020 2020 6564                ed
-0001ea70: 6765 5f63 6f6c 6f72 3d27 626c 6163 6b27  ge_color='black'
-0001ea80: 2c20 7465 7874 5f63 6f6c 6f72 3d27 626c  , text_color='bl
-0001ea90: 6163 6b27 2c0a 2020 2020 2020 2020 2020  ack',.          
-0001eaa0: 2020 2020 2020 2020 2020 2020 6669 745f              fit_
-0001eab0: 636d 6170 203d 2027 5264 596c 476e 272c  cmap = 'RdYlGn',
-0001eac0: 2063 6261 723d 5472 7565 2c20 6669 746e   cbar=True, fitn
-0001ead0: 6573 735f 6362 6172 3d54 7275 652c 0a20  ess_cbar=True,. 
-0001eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eaf0: 2020 2020 2061 6c70 6861 3d31 2c20 7a6f       alpha=1, zo
-0001eb00: 6f6d 5f77 6964 7468 3d4e 6f6e 652c 2078  om_width=None, x
-0001eb10: 3d4e 6f6e 652c 2079 3d4e 6f6e 652c 2074  =None, y=None, t
-0001eb20: 6963 6b73 3d4e 6f6e 652c 0a20 2020 2020  icks=None,.     
-0001eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb40: 206d 6173 6b5f 7261 7374 3d4e 6f6e 6529   mask_rast=None)
-0001eb50: 3a0a 0a20 2020 2020 2020 2023 7265 7475  :..        #retu
-0001eb60: 726e 206d 6573 7361 6765 7320 6966 2073  rn messages if s
-0001eb70: 7065 6369 6573 2064 6f65 7320 6e6f 7420  pecies does not 
-0001eb80: 6861 7665 2067 656e 6f6d 6573 206f 7220  have genomes or 
-0001eb90: 7472 6169 7473 0a20 2020 2020 2020 2069  traits.        i
-0001eba0: 6620 7365 6c66 2e67 656e 5f61 7263 6820  f self.gen_arch 
-0001ebb0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0001ebc0: 2020 2020 2070 7269 6e74 2828 2253 7065       print(("Spe
-0001ebd0: 6369 6573 2e5f 706c 6f74 5f66 6974 6e65  cies._plot_fitne
-0001ebe0: 7373 2069 7320 6e6f 7420 7661 6c69 6420  ss is not valid 
-0001ebf0: 666f 7220 7370 6563 6965 7320 220a 2020  for species ".  
-0001ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ec10: 2022 7769 7468 6f75 7420 6765 6e6f 6d65   "without genome
-0001ec20: 732e 5c6e 2229 290a 2020 2020 2020 2020  s.\n")).        
-0001ec30: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0001ec40: 2020 2065 6c69 6620 7365 6c66 2e67 656e     elif self.gen
-0001ec50: 5f61 7263 682e 7472 6169 7473 2069 7320  _arch.traits is 
-0001ec60: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0001ec70: 2020 7072 696e 7428 2822 5370 6563 6965    print(("Specie
-0001ec80: 732e 5f70 6c6f 745f 6669 746e 6573 7320  s._plot_fitness 
-0001ec90: 6973 206e 6f74 2076 616c 6964 2066 6f72  is not valid for
-0001eca0: 2073 7065 6369 6573 2022 0a20 2020 2020   species ".     
-0001ecb0: 2020 2020 2020 2020 2020 2020 2020 2277                "w
-0001ecc0: 6974 686f 7574 2074 7261 6974 732e 5c6e  ithout traits.\n
-0001ecd0: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
-0001ece0: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
-0001ecf0: 2320 6765 7420 7468 6520 7472 6169 7427  # get the trait'
-0001ed00: 7320 6c79 725f 6e75 6d2c 2069 6620 6c79  s lyr_num, if ly
-0001ed10: 725f 6e75 6d20 7761 736e 2774 2070 726f  r_num wasn't pro
-0001ed20: 7669 6465 6420 6275 7420 7472 745f 6e75  vided but trt_nu
-0001ed30: 6d20 7761 730a 2020 2020 2020 2020 6966  m was.        if
-0001ed40: 2074 7274 5f6e 756d 2069 7320 6e6f 7420   trt_num is not 
-0001ed50: 4e6f 6e65 2061 6e64 206c 7972 5f6e 756d  None and lyr_num
-0001ed60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0001ed70: 2020 2020 2020 6c79 725f 6e75 6d20 3d20        lyr_num = 
-0001ed80: 7365 6c66 2e67 656e 5f61 7263 682e 7472  self.gen_arch.tr
-0001ed90: 6169 7473 5b74 7274 5f6e 756d 5d2e 6c79  aits[trt_num].ly
-0001eda0: 725f 6e75 6d0a 0a20 2020 2020 2020 2023  r_num..        #
-0001edb0: 2067 6574 2061 6c6c 2069 6e64 6976 6964   get all individ
-0001edc0: 7327 2066 6974 6e65 7373 2076 616c 7565  s' fitness value
-0001edd0: 732c 0a20 2020 2020 2020 2023 2061 6e64  s,.        # and
-0001ede0: 2067 6574 2061 7070 726f 7072 6961 7465   get appropriate
-0001edf0: 2063 6f6c 6f72 6d61 700a 2020 2020 2020   colormap.      
-0001ee00: 2020 6966 2074 7274 5f6e 756d 2069 7320    if trt_num is 
-0001ee10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0001ee20: 2020 7720 3d20 7365 6c66 2e5f 6361 6c63    w = self._calc
-0001ee30: 5f66 6974 6e65 7373 2829 0a20 2020 2020  _fitness().     
-0001ee40: 2020 2020 2020 2070 745f 636d 6170 203d         pt_cmap =
-0001ee50: 2027 4772 6579 735f 7227 0a20 2020 2020   'Greys_r'.     
-0001ee60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0001ee70: 2020 2020 2077 203d 2073 656c 662e 5f63       w = self._c
-0001ee80: 616c 635f 6669 746e 6573 7328 7472 6169  alc_fitness(trai
-0001ee90: 745f 6e75 6d20 3d20 7472 745f 6e75 6d29  t_num = trt_num)
-0001eea0: 0a0a 2020 2020 2020 2020 2366 696c 7465  ..        #filte
-0001eeb0: 7220 6f75 7420 756e 7761 6e74 6564 2069  r out unwanted i
-0001eec0: 6e64 6976 6964 732c 2069 6620 6e65 6365  ndivids, if nece
-0001eed0: 7373 6172 790a 2020 2020 2020 2020 7720  ssary.        w 
-0001eee0: 3d20 4f44 287a 6970 285b 2a73 656c 665d  = OD(zip([*self]
-0001eef0: 2c20 7729 290a 2020 2020 2020 2020 6966  , w)).        if
-0001ef00: 2069 6e64 6976 6964 7320 6973 206e 6f74   individs is not
-0001ef10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0001ef20: 2020 2077 203d 207b 693a 7620 666f 7220     w = {i:v for 
-0001ef30: 692c 7620 696e 2077 2e69 7465 6d73 2829  i,v in w.items()
-0001ef40: 2069 6620 6920 696e 2069 6e64 6976 6964   if i in individ
-0001ef50: 737d 0a0a 2020 2020 2020 2020 2320 6361  s}..        # ca
-0001ef60: 6c63 206d 696e 696d 756d 2070 6f73 7369  lc minimum possi
-0001ef70: 626c 6520 6669 746e 6573 7320 2866 6f72  ble fitness (for
-0001ef80: 2070 6865 6e6f 7479 7065 7320 7769 7468   phenotypes with
-0001ef90: 696e 2030 203c 3d20 7a20 3c3d 2031 2c0a  in 0 <= z <= 1,.
-0001efa0: 2020 2020 2020 2020 2377 6869 6368 2069          #which i
-0001efb0: 6e20 7265 616c 6974 7920 6973 6e27 7420  n reality isn't 
-0001efc0: 6120 636f 6e73 7472 6169 6e74 2c20 6275  a constraint, bu
-0001efd0: 7420 7661 6c75 6573 206c 6f77 6572 2074  t values lower t
-0001efe0: 6861 6e0a 2020 2020 2020 2020 2374 6869  han.        #thi
-0001eff0: 7320 7769 6c6c 2061 6c73 6f20 6265 2063  s will also be c
-0001f000: 6f6e 7374 7261 696e 6564 2074 6f20 7468  onstrained to th
-0001f010: 6520 6d69 6e69 6d75 6d2d 7661 6c75 6520  e minimum-value 
-0001f020: 636f 6c6f 7220 666f 7220 706c 6f74 7469  color for plotti
-0001f030: 6e67 290a 2020 2020 2020 2020 234e 4f54  ng).        #NOT
-0001f040: 453a 2074 6865 206e 702e 6174 6c65 6173  E: the np.atleas
-0001f050: 745f 3264 282e 2e2e 292e 6d69 6e28 2920  t_2d(...).min() 
-0001f060: 636f 6e73 7472 7563 7420 6d61 6b65 7320  construct makes 
-0001f070: 7468 6973 0a20 2020 2020 2020 2023 776f  this.        #wo
-0001f080: 726b 2062 6f74 6820 666f 7220 6669 7865  rk both for fixe
-0001f090: 6420 616e 6420 7370 6174 6961 6c6c 7920  d and spatially 
-0001f0a0: 7661 7279 696e 6720 7068 690a 2020 2020  varying phi.    
-0001f0b0: 2020 2020 6966 2074 7274 5f6e 756d 2069      if trt_num i
-0001f0c0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0001f0d0: 2020 2020 6d69 6e5f 6669 7420 3d20 6e70      min_fit = np
-0001f0e0: 2e70 726f 6475 6374 285b 3120 2d20 6e70  .product([1 - np
-0001f0f0: 2e61 746c 6561 7374 5f32 6428 742e 7068  .atleast_2d(t.ph
-0001f100: 6929 2e6d 696e 280a 2020 2020 2020 2020  i).min(.        
-0001f110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f120: 2020 2020 2920 666f 7220 7420 696e 206c      ) for t in l
-0001f130: 6973 7428 7365 6c66 2e67 656e 5f61 7263  ist(self.gen_arc
-0001f140: 682e 7472 6169 7473 2e76 616c 7565 7328  h.traits.values(
-0001f150: 2929 5d29 0a20 2020 2020 2020 2065 6c73  ))]).        els
-0001f160: 653a 0a20 2020 2020 2020 2020 2020 206d  e:.            m
-0001f170: 696e 5f66 6974 203d 2031 202d 206e 702e  in_fit = 1 - np.
-0001f180: 6174 6c65 6173 745f 3264 2873 656c 662e  atleast_2d(self.
-0001f190: 6765 6e5f 6172 6368 2e74 7261 6974 735b  gen_arch.traits[
-0001f1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f1d0: 2020 2020 2020 2020 2074 7274 5f6e 756d           trt_num
-0001f1e0: 5d2e 7068 6929 2e6d 696e 2829 0a0a 2020  ].phi).min()..  
-0001f1f0: 2020 2020 2020 2374 6865 6e20 6765 7420        #then get 
-0001f200: 756e 6576 656e 2063 6d61 7020 616e 6420  uneven cmap and 
-0001f210: 6362 6172 2d6d 616b 6572 2028 6e65 6564  cbar-maker (need
-0001f220: 7320 746f 2062 6520 756e 6576 656e 2074  s to be uneven t
-0001f230: 6f0a 2020 2020 2020 2020 2367 6976 6520  o.        #give 
-0001f240: 636f 6c6f 722d 7265 736f 6c75 7469 6f6e  color-resolution
-0001f250: 2074 6f20 7661 6c75 6573 2076 6172 7969   to values varyi
-0001f260: 6e67 0a20 2020 2020 2020 2023 6265 7477  ng.        #betw
-0001f270: 6565 6e20 3120 616e 6420 7468 6520 6d69  een 1 and the mi
-0001f280: 6e69 6d75 6d2d 6669 746e 6573 7320 7661  nimum-fitness va
-0001f290: 6c75 6520 6173 7375 6d69 6e67 2061 6c6c  lue assuming all
-0001f2a0: 0a20 2020 2020 2020 2023 7068 656e 6f74  .        #phenot
-0001f2b0: 7970 6573 2061 7265 2063 6f6e 7374 7261  ypes are constra
-0001f2c0: 696e 6564 2030 3c3d 7a3c 3d31 2c20 6275  ined 0<=z<=1, bu
-0001f2d0: 7420 7468 656e 2061 6c73 6f0a 2020 2020  t then also.    
-0001f2e0: 2020 2020 2361 6c6c 6f77 2067 7261 6475      #allow gradu
-0001f2f0: 616c 6c79 2064 6565 7065 6e69 6e67 2072  ally deepening r
-0001f300: 6564 7320 666f 7220 6669 746e 6573 7320  eds for fitness 
-0001f310: 7661 6c75 6573 206c 6f77 6572 0a20 2020  values lower.   
-0001f320: 2020 2020 2023 7468 616e 2074 6861 7420       #than that 
-0001f330: 6d69 6e69 6d75 6d20 7661 6c75 6529 2c20  minimum value), 
-0001f340: 7573 696e 6720 7468 6520 6d69 6e5f 6669  using the min_fi
-0001f350: 7420 7661 6c0a 2020 2020 2020 2020 636d  t val.        cm
-0001f360: 6170 2c20 6d61 6b65 5f63 6261 725f 666e  ap, make_cbar_fn
-0001f370: 203d 2076 697a 2e5f 6d61 6b65 5f66 6974   = viz._make_fit
-0001f380: 6e65 7373 5f63 6d61 705f 616e 645f 6362  ness_cmap_and_cb
-0001f390: 6172 5f6d 616b 6572 280a 2020 2020 2020  ar_maker(.      
-0001f3a0: 2020 2020 2020 6d69 6e5f 7661 6c20 3d20        min_val = 
-0001f3b0: 6d69 6e5f 6669 742c 206d 6178 5f76 616c  min_fit, max_val
-0001f3c0: 203d 2031 2c20 636d 6170 203d 2066 6974   = 1, cmap = fit
-0001f3d0: 5f63 6d61 702c 0a20 2020 2020 2020 2020  _cmap,.         
-0001f3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f400: 2020 2020 2020 2074 7274 5f6e 756d 203d         trt_num =
-0001f410: 2074 7274 5f6e 756d 290a 0a20 2020 2020   trt_num)..     
-0001f420: 2020 2023 706c 6f74 2074 6865 2074 7261     #plot the tra
-0001f430: 6974 2070 6865 6e6f 7479 7065 2069 6e20  it phenotype in 
-0001f440: 6c61 7267 6572 2063 6972 636c 6573 2066  larger circles f
-0001f450: 6972 7374 2c20 6966 2074 7261 6974 2069  irst, if trait i
-0001f460: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-0001f470: 2020 2069 6620 7472 745f 6e75 6d20 6973     if trt_num is
-0001f480: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0001f490: 2020 2020 2020 2023 706c 6f74 2074 6865         #plot the
-0001f4a0: 206f 7574 6572 2028 7068 656e 6f74 7970   outer (phenotyp
-0001f4b0: 6529 2063 6972 636c 6573 0a20 2020 2020  e) circles.     
-0001f4c0: 2020 2020 2020 2073 656c 662e 5f70 6c6f         self._plo
-0001f4d0: 745f 7068 656e 6f74 7970 6528 7472 6169  t_phenotype(trai
-0001f4e0: 7420 3d20 7472 745f 6e75 6d2c 206c 7972  t = trt_num, lyr
-0001f4f0: 5f6e 756d 203d 206c 7972 5f6e 756d 2c0a  _num = lyr_num,.
-0001f500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f510: 6c61 6e64 203d 206c 616e 642c 2069 6e64  land = land, ind
-0001f520: 6976 6964 7320 3d20 696e 6469 7669 6473  ivids = individs
-0001f530: 2c20 7465 7874 203d 2046 616c 7365 2c20  , text = False, 
-0001f540: 7369 7a65 203d 2073 697a 652c 0a20 2020  size = size,.   
-0001f550: 2020 2020 2020 2020 2020 2020 2074 6578               tex
-0001f560: 745f 7369 7a65 203d 2074 6578 745f 7369  t_size = text_si
-0001f570: 7a65 2c20 6564 6765 5f63 6f6c 6f72 3d65  ze, edge_color=e
-0001f580: 6467 655f 636f 6c6f 722c 0a20 2020 2020  dge_color,.     
-0001f590: 2020 2020 2020 2020 2020 2074 6578 745f             text_
-0001f5a0: 636f 6c6f 7220 3d20 7465 7874 5f63 6f6c  color = text_col
-0001f5b0: 6f72 2c20 6362 6172 203d 2063 6261 722c  or, cbar = cbar,
-0001f5c0: 2061 6c70 6861 203d 2061 6c70 6861 2c0a   alpha = alpha,.
-0001f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f5e0: 7a6f 6f6d 5f77 6964 7468 203d 207a 6f6f  zoom_width = zoo
-0001f5f0: 6d5f 7769 6474 682c 2078 203d 2078 2c20  m_width, x = x, 
-0001f600: 7920 3d20 792c 2074 6963 6b73 3d74 6963  y = y, ticks=tic
-0001f610: 6b73 2c0a 2020 2020 2020 2020 2020 2020  ks,.            
-0001f620: 2020 2020 6d61 736b 5f72 6173 743d 6d61      mask_rast=ma
-0001f630: 736b 5f72 6173 7429 0a20 2020 2020 2020  sk_rast).       
-0001f640: 2020 2020 2023 6d61 6b65 2073 697a 6520       #make size 
-0001f650: 736d 616c 6c65 7220 666f 7220 7468 6520  smaller for the 
-0001f660: 6e65 7874 206c 6179 6572 206f 6620 696e  next layer of in
-0001f670: 6e65 7220 2866 6974 6e65 7373 2920 6369  ner (fitness) ci
-0001f680: 7263 6c65 730a 2020 2020 2020 2020 2020  rcles.          
-0001f690: 2020 7369 7a65 203d 2072 6f75 6e64 2830    size = round(0
-0001f6a0: 2e34 2a73 697a 6529 0a20 2020 2020 2020  .4*size).       
-0001f6b0: 2020 2020 2023 2067 6574 2073 697a 6573       # get sizes
-0001f6c0: 2066 6f72 2061 6c6c 2069 6e64 6976 6964   for all individ
-0001f6d0: 7561 6c73 2720 696e 6e65 722d 6369 7263  uals' inner-circ
-0001f6e0: 6c65 2066 6974 6e65 7373 2070 6f69 6e74  le fitness point
-0001f6f0: 732c 2069 660a 2020 2020 2020 2020 2020  s, if.          
-0001f700: 2020 2320 7472 745f 6e75 6d20 6973 206e    # trt_num is n
-0001f710: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
-0001f720: 2020 2020 6966 2074 7274 5f6e 756d 2069      if trt_num i
-0001f730: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0001f740: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-0001f750: 203d 2073 697a 6520 2a20 2831 202d 2028   = size * (1 - (
-0001f760: 286e 702e 6172 7261 7928 5b2a 772e 7661  (np.array([*w.va
-0001f770: 6c75 6573 280a 2020 2020 2020 2020 2020  lues(.          
-0001f780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f7a0: 2020 295d 2920 2d20 6d69 6e5f 6669 7429    )]) - min_fit)
-0001f7b0: 202f 2028 3120 2d20 6d69 6e5f 6669 7429   / (1 - min_fit)
-0001f7c0: 2929 0a0a 2020 2020 2020 2020 7365 6c66  ))..        self
-0001f7d0: 2e5f 706c 6f74 286c 7972 5f6e 756d 3d6c  ._plot(lyr_num=l
-0001f7e0: 7972 5f6e 756d 2c20 6c61 6e64 3d6c 616e  yr_num, land=lan
-0001f7f0: 642c 2068 6964 655f 6c61 6e64 3d54 7275  d, hide_land=Tru
-0001f800: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0001f810: 2020 2020 2020 696e 6469 7669 6473 3d69        individs=i
-0001f820: 6e64 6976 6964 732c 2074 6578 743d 7465  ndivids, text=te
-0001f830: 7874 2c20 636f 6c6f 723d 6c69 7374 2877  xt, color=list(w
-0001f840: 2e76 616c 7565 7328 2929 2c0a 2020 2020  .values()),.    
-0001f850: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001f860: 745f 636d 6170 3d63 6d61 702c 2073 697a  t_cmap=cmap, siz
-0001f870: 653d 7369 7a65 2c20 6564 6765 5f63 6f6c  e=size, edge_col
-0001f880: 6f72 3d65 6467 655f 636f 6c6f 722c 0a20  or=edge_color,. 
-0001f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f8a0: 2020 7465 7874 5f63 6f6c 6f72 3d74 6578    text_color=tex
-0001f8b0: 745f 636f 6c6f 722c 2063 6261 723d 6362  t_color, cbar=cb
-0001f8c0: 6172 2c20 7465 7874 5f73 697a 653d 7465  ar, text_size=te
-0001f8d0: 7874 5f73 697a 652c 0a20 2020 2020 2020  xt_size,.       
-0001f8e0: 2020 2020 2020 2020 2020 2020 616c 7068              alph
-0001f8f0: 613d 616c 7068 612c 207a 6f6f 6d5f 7769  a=alpha, zoom_wi
-0001f900: 6474 683d 7a6f 6f6d 5f77 6964 7468 2c20  dth=zoom_width, 
-0001f910: 783d 782c 2079 3d79 2c20 7469 636b 733d  x=x, y=y, ticks=
-0001f920: 7469 636b 732c 0a20 2020 2020 2020 2020  ticks,.         
-0001f930: 2020 2020 2020 2020 2020 6d61 736b 5f72            mask_r
-0001f940: 6173 743d 6d61 736b 5f72 6173 7429 0a0a  ast=mask_rast)..
-0001f950: 2020 2020 2020 2020 2370 6c6f 7420 7068          #plot ph
-0001f960: 656e 6f74 7970 6520 7465 7874 2028 776f  enotype text (wo
-0001f970: 726b 7320 6f6e 6c79 2069 6620 706c 6f74  rks only if plot
-0001f980: 7469 6e67 2061 2073 7065 6369 6669 6320  ting a specific 
-0001f990: 7472 6169 7429 0a20 2020 2020 2020 2069  trait).        i
-0001f9a0: 6620 7068 656e 6f74 7970 655f 7465 7874  f phenotype_text
-0001f9b0: 2061 6e64 2074 7274 5f6e 756d 2069 7320   and trt_num is 
-0001f9c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0001f9d0: 2020 2020 2020 666f 7220 696e 6420 696e        for ind in
-0001f9e0: 2073 656c 662e 7661 6c75 6573 2829 3a0a   self.values():.
-0001f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fa00: 706c 742e 7465 7874 2869 6e64 2e78 2d30  plt.text(ind.x-0
-0001fa10: 2e35 2c20 696e 642e 792d 302e 352c 2027  .5, ind.y-0.5, '
-0001fa20: 2530 2e32 6627 2025 2069 6e64 2e7a 5b74  %0.2f' % ind.z[t
-0001fa30: 7274 5f6e 756d 5d2c 0a20 2020 2020 2020  rt_num],.       
-0001fa40: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-0001fa50: 6f72 203d 2070 6865 6e6f 7479 7065 5f74  or = phenotype_t
-0001fa60: 6578 745f 636f 6c6f 722c 2073 697a 6520  ext_color, size 
-0001fa70: 3d20 7465 7874 5f73 697a 6529 0a0a 2020  = text_size)..  
-0001fa80: 2020 2020 2020 2370 6c6f 7420 6669 746e        #plot fitn
-0001fa90: 6573 7320 7465 7874 0a20 2020 2020 2020  ess text.       
-0001faa0: 2069 6620 6669 746e 6573 735f 7465 7874   if fitness_text
-0001fab0: 3a0a 2020 2020 2020 2020 2020 2020 6f66  :.            of
-0001fac0: 6673 6574 5f66 726f 6d5f 7068 656e 6f74  fset_from_phenot
-0001fad0: 7970 655f 7465 7874 203d 2030 2e30 3031  ype_text = 0.001
-0001fae0: 2a6d 6178 2873 656c 662e 5f6c 616e 645f  *max(self._land_
-0001faf0: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
-0001fb00: 2066 6f72 2069 6e64 2069 6e20 7365 6c66   for ind in self
-0001fb10: 2e76 616c 7565 7328 293a 0a20 2020 2020  .values():.     
-0001fb20: 2020 2020 2020 2020 2020 2070 6c74 2e74             plt.t
-0001fb30: 6578 7428 696e 642e 782d 302e 352b 6f66  ext(ind.x-0.5+of
-0001fb40: 6673 6574 5f66 726f 6d5f 7068 656e 6f74  fset_from_phenot
-0001fb50: 7970 655f 7465 7874 2c0a 2020 2020 2020  ype_text,.      
-0001fb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb70: 2020 2069 6e64 2e79 2d30 2e35 2b6f 6666     ind.y-0.5+off
-0001fb80: 7365 745f 6672 6f6d 5f70 6865 6e6f 7479  set_from_phenoty
-0001fb90: 7065 5f74 6578 742c 0a20 2020 2020 2020  pe_text,.       
-0001fba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fbb0: 2020 2725 302e 3266 2720 2520 696e 642e    '%0.2f' % ind.
-0001fbc0: 6669 742c 2063 6f6c 6f72 203d 2066 6974  fit, color = fit
-0001fbd0: 6e65 7373 5f74 6578 745f 636f 6c6f 722c  ness_text_color,
-0001fbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001fbf0: 2020 2020 2020 2020 2020 7369 7a65 203d            size =
-0001fc00: 2074 6578 745f 7369 7a65 290a 0a20 2020   text_size)..   
-0001fc10: 2020 2020 2023 616e 6420 6d61 6b65 2061       #and make a
-0001fc20: 2063 6f6c 6f72 6261 7220 666f 7220 7468   colorbar for th
-0001fc30: 6520 6669 746e 6573 7320 7661 6c75 6573  e fitness values
-0001fc40: 200a 2020 2020 2020 2020 6966 2066 6974   .        if fit
-0001fc50: 6e65 7373 5f63 6261 723a 0a20 2020 2020  ness_cbar:.     
-0001fc60: 2020 2020 2020 2076 697a 2e5f 6d61 6b65         viz._make
-0001fc70: 5f66 6974 6e65 7373 5f63 6261 7228 6d61  _fitness_cbar(ma
-0001fc80: 6b65 5f63 6261 725f 666e 2c20 6d69 6e5f  ke_cbar_fn, min_
-0001fc90: 6669 7429 0a0a 2020 2020 236d 6574 686f  fit)..    #metho
-0001fca0: 6420 746f 2070 6c6f 7420 6120 7370 6563  d to plot a spec
-0001fcb0: 6965 7327 2061 6c6c 656c 6520 6672 6571  ies' allele freq
-0001fcc0: 7565 6e63 6965 730a 2020 2020 6465 6620  uencies.    def 
-0001fcd0: 5f70 6c6f 745f 616c 6c65 6c65 5f66 7265  _plot_allele_fre
-0001fce0: 7175 656e 6369 6573 2873 656c 662c 2063  quencies(self, c
-0001fcf0: 6f6c 6f72 3d27 7265 6427 293a 0a20 2020  olor='red'):.   
-0001fd00: 2020 2020 2069 6620 7365 6c66 2e67 656e       if self.gen
-0001fd10: 5f61 7263 6820 6973 204e 6f6e 653a 0a20  _arch is None:. 
-0001fd20: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0001fd30: 2828 2253 7065 6369 6573 2e5f 706c 6f74  (("Species._plot
-0001fd40: 5f61 6c6c 656c 655f 6672 6571 7565 6e63  _allele_frequenc
-0001fd50: 6965 7320 6973 206e 6f74 2076 616c 6964  ies is not valid
-0001fd60: 2066 6f72 2022 0a20 2020 2020 2020 2020   for ".         
-0001fd70: 2020 2020 2020 2020 2020 2273 7065 6369            "speci
-0001fd80: 6573 2077 6974 686f 7574 2067 656e 6f6d  es without genom
-0001fd90: 6573 2e5c 6e22 2929 0a20 2020 2020 2020  es.\n")).       
-0001fda0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001fdb0: 2020 2073 656c 662e 6765 6e5f 6172 6368     self.gen_arch
-0001fdc0: 2e5f 706c 6f74 5f61 6c6c 656c 655f 6672  ._plot_allele_fr
-0001fdd0: 6571 7565 6e63 6965 7328 7365 6c66 2c20  equencies(self, 
-0001fde0: 636f 6c6f 723d 636f 6c6f 7229 0a0a 2020  color=color)..  
-0001fdf0: 2020 2320 6d65 7468 6f64 2066 6f72 2070    # method for p
-0001fe00: 6c6f 7474 696e 6720 6120 6869 7374 6f67  lotting a histog
-0001fe10: 7261 6d20 6f66 2074 6865 2063 7572 7265  ram of the curre
-0001fe20: 6e74 2066 6974 6e65 7373 2076 616c 7565  nt fitness value
-0001fe30: 730a 2020 2020 6465 6620 5f70 6c6f 745f  s.    def _plot_
-0001fe40: 6869 7374 5f66 6974 6e65 7373 2873 656c  hist_fitness(sel
-0001fe50: 6629 3a0a 2020 2020 2020 2020 706c 742e  f):.        plt.
-0001fe60: 6869 7374 286c 6973 7428 7365 6c66 2e5f  hist(list(self._
-0001fe70: 6361 6c63 5f66 6974 6e65 7373 2829 2929  calc_fitness()))
-0001fe80: 0a20 2020 2020 2020 2070 6c74 2e78 6c61  .        plt.xla
-0001fe90: 6265 6c28 2746 6974 6e65 7373 2729 0a20  bel('Fitness'). 
-0001fea0: 2020 2020 2020 2070 6c74 2e79 6c61 6265         plt.ylabe
-0001feb0: 6c28 2743 6f75 6e74 2729 0a0a 2020 2020  l('Count')..    
-0001fec0: 2320 6d65 7468 6f64 2066 6f72 2070 6c6f  # method for plo
-0001fed0: 7474 696e 6720 7468 6520 6d6f 7665 6d65  tting the moveme
-0001fee0: 6e74 2073 7572 6661 6365 2028 696e 2076  nt surface (in v
-0001fef0: 6172 696f 7573 2066 6f72 6d61 7473 290a  arious formats).
-0001ff00: 2020 2020 6465 6620 5f70 6c6f 745f 6469      def _plot_di
-0001ff10: 7265 6374 696f 6e5f 7375 7266 6163 6528  rection_surface(
-0001ff20: 7365 6c66 2c20 6c61 6e64 2c20 7375 7266  self, land, surf
-0001ff30: 5f74 7970 652c 2073 7479 6c65 2c20 783d  _type, style, x=
-0001ff40: 4e6f 6e65 2c20 793d 4e6f 6e65 2c0a 2020  None, y=None,.  
-0001ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ff60: 2020 2020 2020 2020 2020 2020 2020 7a6f                zo
-0001ff70: 6f6d 5f77 6964 7468 3d4e 6f6e 652c 2073  om_width=None, s
-0001ff80: 6361 6c65 5f66 6163 743d 342e 352c 0a20  cale_fact=4.5,. 
-0001ff90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ffa0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001ffb0: 6f6c 6f72 3d27 626c 6163 6b27 2c20 6362  olor='black', cb
-0001ffc0: 6172 3d54 7275 652c 2074 6963 6b73 3d4e  ar=True, ticks=N
-0001ffd0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0001ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fff0: 2020 2020 2063 6d61 703d 2770 6c61 736d       cmap='plasm
-00020000: 6127 2c20 6d61 736b 5f72 6173 743d 4e6f  a', mask_rast=No
-00020010: 6e65 293a 0a20 2020 2020 2020 2023 2067  ne):.        # g
-00020020: 6574 2074 6865 2063 6f72 7265 6374 2073  et the correct s
-00020030: 7572 6661 6365 0a20 2020 2020 2020 2069  urface.        i
-00020040: 6620 7375 7266 5f74 7970 6520 3d3d 2027  f surf_type == '
-00020050: 6d6f 7665 273a 0a20 2020 2020 2020 2020  move':.         
-00020060: 2020 2073 7572 6620 3d20 7365 6c66 2e5f     surf = self._
-00020070: 6d6f 7665 5f73 7572 660a 2020 2020 2020  move_surf.      
-00020080: 2020 656c 6966 2073 7572 665f 7479 7065    elif surf_type
-00020090: 203d 3d20 2764 6973 7027 3a0a 2020 2020   == 'disp':.    
-000200a0: 2020 2020 2020 2020 7375 7266 203d 3d20          surf == 
-000200b0: 7365 6c66 2e5f 6469 7370 5f73 7572 660a  self._disp_surf.
-000200c0: 0a20 2020 2020 2020 2023 2067 6574 2061  .        # get a
-000200d0: 6c6c 2078 2773 2061 6e64 2079 2773 2c20  ll x's and y's, 
-000200e0: 6966 2078 2061 6e64 2079 2061 7265 204e  if x and y are N
-000200f0: 6f6e 650a 2020 2020 2020 2020 6966 2078  one.        if x
-00020100: 2069 7320 4e6f 6e65 2061 6e64 2079 2069   is None and y i
-00020110: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00020120: 2020 2020 7820 3d20 5b2a 7261 6e67 6528      x = [*range(
-00020130: 6c61 6e64 2e64 696d 5b30 5d29 5d0a 2020  land.dim[0])].  
-00020140: 2020 2020 2020 2020 2020 7920 3d20 5b2a            y = [*
-00020150: 7261 6e67 6528 6c61 6e64 2e64 696d 5b31  range(land.dim[1
-00020160: 5d29 5d0a 2020 2020 2020 2020 656c 7365  ])].        else
-00020170: 3a0a 2020 2020 2020 2020 2020 2020 7820  :.            x 
-00020180: 3d20 5b78 5d0a 2020 2020 2020 2020 2020  = [x].          
-00020190: 2020 7920 3d20 5b79 5d0a 2020 2020 2020    y = [y].      
-000201a0: 2020 2363 6865 636b 2069 6620 7468 6520    #check if the 
-000201b0: 7375 7266 6163 6520 6973 206e 6f6e 650a  surface is none.
-000201c0: 2020 2020 2020 2020 6966 2073 7572 6620          if surf 
-000201d0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-000201e0: 2020 2020 2070 7269 6e74 2828 2746 756e       print(('Fun
-000201f0: 6374 696f 6e20 6e6f 7420 7661 6c69 6420  ction not valid 
-00020200: 666f 7220 6120 5370 6563 6965 7320 7769  for a Species wi
-00020210: 7468 206e 6f20 270a 2020 2020 2020 2020  th no '.        
-00020220: 2020 2020 2020 2020 2020 2027 5f25 7353             '_%sS
-00020230: 7572 6661 6365 2e27 2920 2520 287b 0a20  urface.') % ({. 
-00020240: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00020250: 6d6f 7665 273a 2027 4d6f 7665 6d65 6e74  move': 'Movement
-00020260: 272c 2027 6469 7370 273a 2027 4469 7370  ', 'disp': 'Disp
-00020270: 6572 7361 6c27 7d5b 7375 7266 5f74 7970  ersal'}[surf_typ
-00020280: 655d 2929 0a20 2020 2020 2020 2020 2020  e])).           
-00020290: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-000202a0: 656c 6966 2073 7479 6c65 206e 6f74 2069  elif style not i
-000202b0: 6e20 5b27 6869 7374 272c 2027 6368 6973  n ['hist', 'chis
-000202c0: 7427 2c20 2776 6563 7427 2c20 2763 6472  t', 'vect', 'cdr
-000202d0: 6177 7327 5d3a 0a20 2020 2020 2020 2020  aws']:.         
-000202e0: 2020 2070 7269 6e74 2828 2254 6865 2027     print(("The '
-000202f0: 7374 796c 6527 2061 7267 756d 656e 7420  style' argument 
-00020300: 6d75 7374 2074 616b 6520 6f6e 6520 6f66  must take one of
-00020310: 2074 6865 2022 0a20 2020 2020 2020 2020   the ".         
-00020320: 2020 2020 2020 2020 2020 2266 6f6c 6c6f            "follo
-00020330: 7769 6e67 2076 616c 7565 733a 2027 6869  wing values: 'hi
-00020340: 7374 272c 2027 6368 6973 7427 2c20 220a  st', 'chist', ".
-00020350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020360: 2020 2022 2776 6563 7427 2c20 2763 6472     "'vect', 'cdr
-00020370: 6177 7327 2229 290a 2020 2020 2020 2020  aws'")).        
-00020380: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00020390: 2020 2065 6c69 6620 7374 796c 6520 3d3d     elif style ==
-000203a0: 2027 6869 7374 273a 0a20 2020 2020 2020   'hist':.       
-000203b0: 2020 2020 2078 203d 2078 5b30 5d0a 2020       x = x[0].  
-000203c0: 2020 2020 2020 2020 2020 7920 3d20 795b            y = y[
-000203d0: 305d 0a20 2020 2020 2020 2020 2020 2070  0].            p
-000203e0: 6c74 2e68 6973 7428 722e 6368 6f69 6365  lt.hist(r.choice
-000203f0: 2873 7572 662e 7375 7266 5b79 2c78 2c3a  (surf.surf[y,x,:
-00020400: 5d2c 2073 697a 6520 3d20 3130 3030 302c  ], size = 10000,
-00020410: 2072 6570 6c61 6365 203d 2054 7275 6529   replace = True)
-00020420: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00020430: 2020 2020 2020 2062 696e 733d 3130 302c         bins=100,
-00020440: 2064 656e 7369 7479 3d54 7275 652c 2061   density=True, a
-00020450: 6c70 6861 3d30 2e35 2c20 636f 6c6f 723d  lpha=0.5, color=
-00020460: 636f 6c6f 7229 0a0a 2020 2020 2020 2020  color)..        
-00020470: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00020480: 2020 2364 6973 706c 6179 2074 6865 206d    #display the m
-00020490: 6f76 656d 656e 742d 7375 7266 6163 6520  ovement-surface 
-000204a0: 7261 7374 6572 0a20 2020 2020 2020 2020  raster.         
-000204b0: 2020 206c 7972 5f6e 756d 203d 2073 7572     lyr_num = sur
-000204c0: 662e 6c79 725f 6e75 6d0a 2020 2020 2020  f.lyr_num.      
-000204d0: 2020 2020 2020 6c61 6e64 5b6c 7972 5f6e        land[lyr_n
-000204e0: 756d 5d2e 5f70 6c6f 7428 7a6f 6f6d 5f77  um]._plot(zoom_w
-000204f0: 6964 7468 203d 207a 6f6f 6d5f 7769 6474  idth = zoom_widt
-00020500: 682c 2078 3d6e 702e 6d65 616e 2878 292c  h, x=np.mean(x),
-00020510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020530: 2079 3d6e 702e 6d65 616e 2879 292c 2074   y=np.mean(y), t
-00020540: 6963 6b73 3d74 6963 6b73 2c20 636d 6170  icks=ticks, cmap
-00020550: 3d63 6d61 702c 0a20 2020 2020 2020 2020  =cmap,.         
-00020560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020570: 2020 2020 2020 206d 6173 6b5f 7261 7374         mask_rast
-00020580: 3d6d 6173 6b5f 7261 7374 290a 0a20 2020  =mask_rast)..   
-00020590: 2020 2020 2020 2020 2069 6620 7374 796c           if styl
-000205a0: 6520 3d3d 2027 6368 6973 7427 3a0a 2020  e == 'chist':.  
-000205b0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-000205c0: 7220 785f 7661 6c20 696e 2078 3a0a 2020  r x_val in x:.  
-000205d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000205e0: 2020 666f 7220 795f 7661 6c20 696e 2079    for y_val in y
-000205f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00020600: 2020 2020 2020 2020 2020 762c 2061 203d            v, a =
-00020610: 206e 702e 6869 7374 6f67 7261 6d28 722e   np.histogram(r.
-00020620: 6368 6f69 6365 2873 7572 662e 7375 7266  choice(surf.surf
-00020630: 5b79 5f76 616c 2c0a 2020 2020 2020 2020  [y_val,.        
-00020640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020670: 2020 2020 2020 2078 5f76 616c 2c20 3a5d         x_val, :]
-00020680: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00020690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000206a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000206b0: 2020 2020 2020 2072 6570 6c61 6365 3d54         replace=T
-000206c0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-000206d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000206e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000206f0: 2020 2020 2020 2020 2020 7369 7a65 3d37            size=7
-00020700: 3530 3029 2c20 6269 6e73 3d31 3529 0a20  500), bins=15). 
-00020710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020720: 2020 2020 2020 2076 203d 2076 202f 2066         v = v / f
-00020730: 6c6f 6174 2876 2e73 756d 2829 290a 2020  loat(v.sum()).  
-00020740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020750: 2020 2020 2020 6120 3d20 5b28 615b 6e5d        a = [(a[n]
-00020760: 202b 2061 5b6e 202b 2031 5d29 202f 2032   + a[n + 1]) / 2
-00020770: 2066 6f72 206e 2069 6e20 7261 6e67 6528   for n in range(
-00020780: 6c65 6e28 6129 202d 2031 295d 0a20 2020  len(a) - 1)].   
-00020790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000207a0: 2020 2020 2078 7320 3d20 5b6e 702e 636f       xs = [np.co
-000207b0: 7328 615b 6e5d 2920 2a20 302e 3735 2066  s(a[n]) * 0.75 f
-000207c0: 6f72 206e 2069 6e20 7261 6e67 6528 6c65  or n in range(le
-000207d0: 6e28 6129 295d 0a20 2020 2020 2020 2020  n(a))].         
-000207e0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-000207f0: 7320 3d20 5b6e 702e 7369 6e28 615b 6e5d  s = [np.sin(a[n]
-00020800: 2920 2a20 302e 3735 2066 6f72 206e 2069  ) * 0.75 for n i
-00020810: 6e20 7261 6e67 6528 6c65 6e28 6129 295d  n range(len(a))]
-00020820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020830: 2020 2020 2020 2020 2078 7320 3d20 6e70           xs = np
-00020840: 2e61 7272 6179 2878 7329 202a 2076 202a  .array(xs) * v *
-00020850: 2073 6361 6c65 5f66 6163 740a 2020 2020   scale_fact.    
-00020860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020870: 2020 2020 7973 203d 206e 702e 6172 7261      ys = np.arra
-00020880: 7928 7973 2920 2a20 7620 2a20 7363 616c  y(ys) * v * scal
-00020890: 655f 6661 6374 0a20 2020 2020 2020 2020  e_fact.         
-000208a0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-000208b0: 706c 742e 706c 6f74 2828 785f 7661 6c20  plt.plot((x_val 
-000208c0: 2b20 302e 352c 2028 785f 7661 6c20 2b20  + 0.5, (x_val + 
-000208d0: 302e 3520 2b20 7873 5b6e 5d29 292c 0a20  0.5 + xs[n])),. 
+0001ea20: 2020 2020 2020 6362 6172 203d 2063 6261        cbar = cba
+0001ea30: 722c 2073 697a 6520 3d20 7369 7a65 2c20  r, size = size, 
+0001ea40: 7465 7874 5f73 697a 6520 3d20 7465 7874  text_size = text
+0001ea50: 5f73 697a 652c 0a20 2020 2020 2020 2020  _size,.         
+0001ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ea70: 2020 2061 6c70 6861 203d 2061 6c70 6861     alpha = alpha
+0001ea80: 2c20 7a6f 6f6d 5f77 6964 7468 203d 207a  , zoom_width = z
+0001ea90: 6f6f 6d5f 7769 6474 682c 2078 203d 2078  oom_width, x = x
+0001eaa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001eab0: 2020 2020 2020 2020 2020 2020 2020 7920                y 
+0001eac0: 3d20 792c 2076 6d69 6e20 3d20 302c 2076  = y, vmin = 0, v
+0001ead0: 6d61 7820 3d20 312c 2074 6963 6b73 3d74  max = 1, ticks=t
+0001eae0: 6963 6b73 2c0a 2020 2020 2020 2020 2020  icks,.          
+0001eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb00: 2020 6d61 736b 5f72 6173 743d 6d61 736b    mask_rast=mask
+0001eb10: 5f72 6173 742c 2061 6e69 6d61 7465 3d61  _rast, animate=a
+0001eb20: 6e69 6d61 7465 290a 0a20 2020 2020 2020  nimate)..       
+0001eb30: 2072 6574 7572 6e20 706f 696e 7473 0a0a   return points..
+0001eb40: 0a20 2020 2023 206d 6574 686f 6420 666f  .    # method fo
+0001eb50: 7220 706c 6f74 7469 6e67 2069 6e64 6976  r plotting indiv
+0001eb60: 6964 7561 6c73 2063 6f6c 6f72 6564 2062  iduals colored b
+0001eb70: 7920 7468 6569 7220 6f76 6572 616c 6c20  y their overall 
+0001eb80: 6669 746e 6573 7365 732c 0a20 2020 2023  fitnesses,.    #
+0001eb90: 6f72 2062 7920 7468 6569 7220 6669 746e  or by their fitn
+0001eba0: 6573 7365 7320 666f 7220 6120 7369 6e67  esses for a sing
+0001ebb0: 6c65 2074 7261 6974 2028 6966 2074 7261  le trait (if tra
+0001ebc0: 6974 2069 7320 6e6f 7420 4e6f 6e65 290a  it is not None).
+0001ebd0: 2020 2020 6465 6620 5f70 6c6f 745f 6669      def _plot_fi
+0001ebe0: 746e 6573 7328 7365 6c66 2c20 7472 745f  tness(self, trt_
+0001ebf0: 6e75 6d3d 4e6f 6e65 2c20 6c79 725f 6e75  num=None, lyr_nu
+0001ec00: 6d3d 4e6f 6e65 2c20 6c61 6e64 3d4e 6f6e  m=None, land=Non
+0001ec10: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0001ec20: 2020 2020 2020 2020 2069 6e64 6976 6964           individ
+0001ec30: 733d 4e6f 6e65 2c20 7465 7874 3d46 616c  s=None, text=Fal
+0001ec40: 7365 2c20 7068 656e 6f74 7970 655f 7465  se, phenotype_te
+0001ec50: 7874 3d46 616c 7365 2c0a 2020 2020 2020  xt=False,.      
+0001ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ec70: 7068 656e 6f74 7970 655f 7465 7874 5f63  phenotype_text_c
+0001ec80: 6f6c 6f72 3d27 626c 6163 6b27 2c20 6669  olor='black', fi
+0001ec90: 746e 6573 735f 7465 7874 3d46 616c 7365  tness_text=False
+0001eca0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001ecb0: 2020 2020 2020 2020 6669 746e 6573 735f          fitness_
+0001ecc0: 7465 7874 5f63 6f6c 6f72 3d27 2333 3333  text_color='#333
+0001ecd0: 3333 3327 2c20 7369 7a65 3d31 3030 2c20  333', size=100, 
+0001ece0: 7465 7874 5f73 697a 6520 3d20 392c 0a20  text_size = 9,. 
+0001ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ed00: 2020 2020 2065 6467 655f 636f 6c6f 723d       edge_color=
+0001ed10: 2762 6c61 636b 272c 2074 6578 745f 636f  'black', text_co
+0001ed20: 6c6f 723d 2762 6c61 636b 272c 0a20 2020  lor='black',.   
+0001ed30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ed40: 2020 2066 6974 5f63 6d61 7020 3d20 2752     fit_cmap = 'R
+0001ed50: 6459 6c47 6e27 2c20 6362 6172 3d54 7275  dYlGn', cbar=Tru
+0001ed60: 652c 2066 6974 6e65 7373 5f63 6261 723d  e, fitness_cbar=
+0001ed70: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+0001ed80: 2020 2020 2020 2020 2020 2020 616c 7068              alph
+0001ed90: 613d 312c 207a 6f6f 6d5f 7769 6474 683d  a=1, zoom_width=
+0001eda0: 4e6f 6e65 2c20 783d 4e6f 6e65 2c20 793d  None, x=None, y=
+0001edb0: 4e6f 6e65 2c20 7469 636b 733d 4e6f 6e65  None, ticks=None
+0001edc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001edd0: 2020 2020 2020 2020 6d61 736b 5f72 6173          mask_ras
+0001ede0: 743d 4e6f 6e65 293a 0a0a 2020 2020 2020  t=None):..      
+0001edf0: 2020 2372 6574 7572 6e20 6d65 7373 6167    #return messag
+0001ee00: 6573 2069 6620 7370 6563 6965 7320 646f  es if species do
+0001ee10: 6573 206e 6f74 2068 6176 6520 6765 6e6f  es not have geno
+0001ee20: 6d65 7320 6f72 2074 7261 6974 730a 2020  mes or traits.  
+0001ee30: 2020 2020 2020 6966 2073 656c 662e 6765        if self.ge
+0001ee40: 6e5f 6172 6368 2069 7320 4e6f 6e65 3a0a  n_arch is None:.
+0001ee50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0001ee60: 7428 2822 5370 6563 6965 732e 5f70 6c6f  t(("Species._plo
+0001ee70: 745f 6669 746e 6573 7320 6973 206e 6f74  t_fitness is not
+0001ee80: 2076 616c 6964 2066 6f72 2073 7065 6369   valid for speci
+0001ee90: 6573 2022 0a20 2020 2020 2020 2020 2020  es ".           
+0001eea0: 2020 2020 2020 2020 2277 6974 686f 7574          "without
+0001eeb0: 2067 656e 6f6d 6573 2e5c 6e22 2929 0a20   genomes.\n")). 
+0001eec0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001eed0: 6e0a 2020 2020 2020 2020 656c 6966 2073  n.        elif s
+0001eee0: 656c 662e 6765 6e5f 6172 6368 2e74 7261  elf.gen_arch.tra
+0001eef0: 6974 7320 6973 204e 6f6e 653a 0a20 2020  its is None:.   
+0001ef00: 2020 2020 2020 2020 2070 7269 6e74 2828           print((
+0001ef10: 2253 7065 6369 6573 2e5f 706c 6f74 5f66  "Species._plot_f
+0001ef20: 6974 6e65 7373 2069 7320 6e6f 7420 7661  itness is not va
+0001ef30: 6c69 6420 666f 7220 7370 6563 6965 7320  lid for species 
+0001ef40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0001ef50: 2020 2020 2022 7769 7468 6f75 7420 7472       "without tr
+0001ef60: 6169 7473 2e5c 6e22 2929 0a20 2020 2020  aits.\n")).     
+0001ef70: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+0001ef80: 2020 2020 2020 2023 2067 6574 2074 6865         # get the
+0001ef90: 2074 7261 6974 2773 206c 7972 5f6e 756d   trait's lyr_num
+0001efa0: 2c20 6966 206c 7972 5f6e 756d 2077 6173  , if lyr_num was
+0001efb0: 6e27 7420 7072 6f76 6964 6564 2062 7574  n't provided but
+0001efc0: 2074 7274 5f6e 756d 2077 6173 0a20 2020   trt_num was.   
+0001efd0: 2020 2020 2069 6620 7472 745f 6e75 6d20       if trt_num 
+0001efe0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+0001eff0: 6c79 725f 6e75 6d20 6973 204e 6f6e 653a  lyr_num is None:
+0001f000: 0a20 2020 2020 2020 2020 2020 206c 7972  .            lyr
+0001f010: 5f6e 756d 203d 2073 656c 662e 6765 6e5f  _num = self.gen_
+0001f020: 6172 6368 2e74 7261 6974 735b 7472 745f  arch.traits[trt_
+0001f030: 6e75 6d5d 2e6c 7972 5f6e 756d 0a0a 2020  num].lyr_num..  
+0001f040: 2020 2020 2020 2320 6765 7420 616c 6c20        # get all 
+0001f050: 696e 6469 7669 6473 2720 6669 746e 6573  individs' fitnes
+0001f060: 7320 7661 6c75 6573 2c0a 2020 2020 2020  s values,.      
+0001f070: 2020 2320 616e 6420 6765 7420 6170 7072    # and get appr
+0001f080: 6f70 7269 6174 6520 636f 6c6f 726d 6170  opriate colormap
+0001f090: 0a20 2020 2020 2020 2069 6620 7472 745f  .        if trt_
+0001f0a0: 6e75 6d20 6973 204e 6f6e 653a 0a20 2020  num is None:.   
+0001f0b0: 2020 2020 2020 2020 2077 203d 2073 656c           w = sel
+0001f0c0: 662e 5f63 616c 635f 6669 746e 6573 7328  f._calc_fitness(
+0001f0d0: 290a 2020 2020 2020 2020 2020 2020 7074  ).            pt
+0001f0e0: 5f63 6d61 7020 3d20 2747 7265 7973 5f72  _cmap = 'Greys_r
+0001f0f0: 270a 2020 2020 2020 2020 656c 7365 3a0a  '.        else:.
+0001f100: 2020 2020 2020 2020 2020 2020 7720 3d20              w = 
+0001f110: 7365 6c66 2e5f 6361 6c63 5f66 6974 6e65  self._calc_fitne
+0001f120: 7373 2874 7261 6974 5f6e 756d 203d 2074  ss(trait_num = t
+0001f130: 7274 5f6e 756d 290a 0a20 2020 2020 2020  rt_num)..       
+0001f140: 2023 6669 6c74 6572 206f 7574 2075 6e77   #filter out unw
+0001f150: 616e 7465 6420 696e 6469 7669 6473 2c20  anted individs, 
+0001f160: 6966 206e 6563 6573 7361 7279 0a20 2020  if necessary.   
+0001f170: 2020 2020 2077 203d 204f 4428 7a69 7028       w = OD(zip(
+0001f180: 5b2a 7365 6c66 5d2c 2077 2929 0a20 2020  [*self], w)).   
+0001f190: 2020 2020 2069 6620 696e 6469 7669 6473       if individs
+0001f1a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0001f1b0: 2020 2020 2020 2020 2020 7720 3d20 7b69            w = {i
+0001f1c0: 3a76 2066 6f72 2069 2c76 2069 6e20 772e  :v for i,v in w.
+0001f1d0: 6974 656d 7328 2920 6966 2069 2069 6e20  items() if i in 
+0001f1e0: 696e 6469 7669 6473 7d0a 0a20 2020 2020  individs}..     
+0001f1f0: 2020 2023 2063 616c 6320 6d69 6e69 6d75     # calc minimu
+0001f200: 6d20 706f 7373 6962 6c65 2066 6974 6e65  m possible fitne
+0001f210: 7373 2028 666f 7220 7068 656e 6f74 7970  ss (for phenotyp
+0001f220: 6573 2077 6974 6869 6e20 3020 3c3d 207a  es within 0 <= z
+0001f230: 203c 3d20 312c 0a20 2020 2020 2020 2023   <= 1,.        #
+0001f240: 7768 6963 6820 696e 2072 6561 6c69 7479  which in reality
+0001f250: 2069 736e 2774 2061 2063 6f6e 7374 7261   isn't a constra
+0001f260: 696e 742c 2062 7574 2076 616c 7565 7320  int, but values 
+0001f270: 6c6f 7765 7220 7468 616e 0a20 2020 2020  lower than.     
+0001f280: 2020 2023 7468 6973 2077 696c 6c20 616c     #this will al
+0001f290: 736f 2062 6520 636f 6e73 7472 6169 6e65  so be constraine
+0001f2a0: 6420 746f 2074 6865 206d 696e 696d 756d  d to the minimum
+0001f2b0: 2d76 616c 7565 2063 6f6c 6f72 2066 6f72  -value color for
+0001f2c0: 2070 6c6f 7474 696e 6729 0a20 2020 2020   plotting).     
+0001f2d0: 2020 2023 4e4f 5445 3a20 7468 6520 6e70     #NOTE: the np
+0001f2e0: 2e61 746c 6561 7374 5f32 6428 2e2e 2e29  .atleast_2d(...)
+0001f2f0: 2e6d 696e 2829 2063 6f6e 7374 7275 6374  .min() construct
+0001f300: 206d 616b 6573 2074 6869 730a 2020 2020   makes this.    
+0001f310: 2020 2020 2377 6f72 6b20 626f 7468 2066      #work both f
+0001f320: 6f72 2066 6978 6564 2061 6e64 2073 7061  or fixed and spa
+0001f330: 7469 616c 6c79 2076 6172 7969 6e67 2070  tially varying p
+0001f340: 6869 0a20 2020 2020 2020 2069 6620 7472  hi.        if tr
+0001f350: 745f 6e75 6d20 6973 204e 6f6e 653a 0a20  t_num is None:. 
+0001f360: 2020 2020 2020 2020 2020 206d 696e 5f66             min_f
+0001f370: 6974 203d 206e 702e 7072 6f64 7563 7428  it = np.product(
+0001f380: 5b31 202d 206e 702e 6174 6c65 6173 745f  [1 - np.atleast_
+0001f390: 3264 2874 2e70 6869 292e 6d69 6e28 0a20  2d(t.phi).min(. 
+0001f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f3b0: 2020 2020 2020 2020 2020 2029 2066 6f72             ) for
+0001f3c0: 2074 2069 6e20 6c69 7374 2873 656c 662e   t in list(self.
+0001f3d0: 6765 6e5f 6172 6368 2e74 7261 6974 732e  gen_arch.traits.
+0001f3e0: 7661 6c75 6573 2829 295d 290a 2020 2020  values())]).    
+0001f3f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001f400: 2020 2020 2020 6d69 6e5f 6669 7420 3d20        min_fit = 
+0001f410: 3120 2d20 6e70 2e61 746c 6561 7374 5f32  1 - np.atleast_2
+0001f420: 6428 7365 6c66 2e67 656e 5f61 7263 682e  d(self.gen_arch.
+0001f430: 7472 6169 7473 5b0a 2020 2020 2020 2020  traits[.        
+0001f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f470: 7472 745f 6e75 6d5d 2e70 6869 292e 6d69  trt_num].phi).mi
+0001f480: 6e28 290a 0a20 2020 2020 2020 2023 7468  n()..        #th
+0001f490: 656e 2067 6574 2075 6e65 7665 6e20 636d  en get uneven cm
+0001f4a0: 6170 2061 6e64 2063 6261 722d 6d61 6b65  ap and cbar-make
+0001f4b0: 7220 286e 6565 6473 2074 6f20 6265 2075  r (needs to be u
+0001f4c0: 6e65 7665 6e20 746f 0a20 2020 2020 2020  neven to.       
+0001f4d0: 2023 6769 7665 2063 6f6c 6f72 2d72 6573   #give color-res
+0001f4e0: 6f6c 7574 696f 6e20 746f 2076 616c 7565  olution to value
+0001f4f0: 7320 7661 7279 696e 670a 2020 2020 2020  s varying.      
+0001f500: 2020 2362 6574 7765 656e 2031 2061 6e64    #between 1 and
+0001f510: 2074 6865 206d 696e 696d 756d 2d66 6974   the minimum-fit
+0001f520: 6e65 7373 2076 616c 7565 2061 7373 756d  ness value assum
+0001f530: 696e 6720 616c 6c0a 2020 2020 2020 2020  ing all.        
+0001f540: 2370 6865 6e6f 7479 7065 7320 6172 6520  #phenotypes are 
+0001f550: 636f 6e73 7472 6169 6e65 6420 303c 3d7a  constrained 0<=z
+0001f560: 3c3d 312c 2062 7574 2074 6865 6e20 616c  <=1, but then al
+0001f570: 736f 0a20 2020 2020 2020 2023 616c 6c6f  so.        #allo
+0001f580: 7720 6772 6164 7561 6c6c 7920 6465 6570  w gradually deep
+0001f590: 656e 696e 6720 7265 6473 2066 6f72 2066  ening reds for f
+0001f5a0: 6974 6e65 7373 2076 616c 7565 7320 6c6f  itness values lo
+0001f5b0: 7765 720a 2020 2020 2020 2020 2374 6861  wer.        #tha
+0001f5c0: 6e20 7468 6174 206d 696e 696d 756d 2076  n that minimum v
+0001f5d0: 616c 7565 292c 2075 7369 6e67 2074 6865  alue), using the
+0001f5e0: 206d 696e 5f66 6974 2076 616c 0a20 2020   min_fit val.   
+0001f5f0: 2020 2020 2063 6d61 702c 206d 616b 655f       cmap, make_
+0001f600: 6362 6172 5f66 6e20 3d20 7669 7a2e 5f6d  cbar_fn = viz._m
+0001f610: 616b 655f 6669 746e 6573 735f 636d 6170  ake_fitness_cmap
+0001f620: 5f61 6e64 5f63 6261 725f 6d61 6b65 7228  _and_cbar_maker(
+0001f630: 0a20 2020 2020 2020 2020 2020 206d 696e  .            min
+0001f640: 5f76 616c 203d 206d 696e 5f66 6974 2c20  _val = min_fit, 
+0001f650: 6d61 785f 7661 6c20 3d20 312c 2063 6d61  max_val = 1, cma
+0001f660: 7020 3d20 6669 745f 636d 6170 2c0a 2020  p = fit_cmap,.  
+0001f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f690: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+0001f6a0: 745f 6e75 6d20 3d20 7472 745f 6e75 6d29  t_num = trt_num)
+0001f6b0: 0a0a 2020 2020 2020 2020 2370 6c6f 7420  ..        #plot 
+0001f6c0: 7468 6520 7472 6169 7420 7068 656e 6f74  the trait phenot
+0001f6d0: 7970 6520 696e 206c 6172 6765 7220 6369  ype in larger ci
+0001f6e0: 7263 6c65 7320 6669 7273 742c 2069 6620  rcles first, if 
+0001f6f0: 7472 6169 7420 6973 206e 6f74 204e 6f6e  trait is not Non
+0001f700: 650a 2020 2020 2020 2020 6966 2074 7274  e.        if trt
+0001f710: 5f6e 756d 2069 7320 6e6f 7420 4e6f 6e65  _num is not None
+0001f720: 3a0a 2020 2020 2020 2020 2020 2020 2370  :.            #p
+0001f730: 6c6f 7420 7468 6520 6f75 7465 7220 2870  lot the outer (p
+0001f740: 6865 6e6f 7479 7065 2920 6369 7263 6c65  henotype) circle
+0001f750: 730a 2020 2020 2020 2020 2020 2020 7365  s.            se
+0001f760: 6c66 2e5f 706c 6f74 5f70 6865 6e6f 7479  lf._plot_phenoty
+0001f770: 7065 2874 7261 6974 203d 2074 7274 5f6e  pe(trait = trt_n
+0001f780: 756d 2c20 6c79 725f 6e75 6d20 3d20 6c79  um, lyr_num = ly
+0001f790: 725f 6e75 6d2c 0a20 2020 2020 2020 2020  r_num,.         
+0001f7a0: 2020 2020 2020 206c 616e 6420 3d20 6c61         land = la
+0001f7b0: 6e64 2c20 696e 6469 7669 6473 203d 2069  nd, individs = i
+0001f7c0: 6e64 6976 6964 732c 2074 6578 7420 3d20  ndivids, text = 
+0001f7d0: 4661 6c73 652c 2073 697a 6520 3d20 7369  False, size = si
+0001f7e0: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
+0001f7f0: 2020 2020 7465 7874 5f73 697a 6520 3d20      text_size = 
+0001f800: 7465 7874 5f73 697a 652c 2065 6467 655f  text_size, edge_
+0001f810: 636f 6c6f 723d 6564 6765 5f63 6f6c 6f72  color=edge_color
+0001f820: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001f830: 2020 7465 7874 5f63 6f6c 6f72 203d 2074    text_color = t
+0001f840: 6578 745f 636f 6c6f 722c 2063 6261 7220  ext_color, cbar 
+0001f850: 3d20 6362 6172 2c20 616c 7068 6120 3d20  = cbar, alpha = 
+0001f860: 616c 7068 612c 0a20 2020 2020 2020 2020  alpha,.         
+0001f870: 2020 2020 2020 207a 6f6f 6d5f 7769 6474         zoom_widt
+0001f880: 6820 3d20 7a6f 6f6d 5f77 6964 7468 2c20  h = zoom_width, 
+0001f890: 7820 3d20 782c 2079 203d 2079 2c20 7469  x = x, y = y, ti
+0001f8a0: 636b 733d 7469 636b 732c 0a20 2020 2020  cks=ticks,.     
+0001f8b0: 2020 2020 2020 2020 2020 206d 6173 6b5f             mask_
+0001f8c0: 7261 7374 3d6d 6173 6b5f 7261 7374 290a  rast=mask_rast).
+0001f8d0: 2020 2020 2020 2020 2020 2020 236d 616b              #mak
+0001f8e0: 6520 7369 7a65 2073 6d61 6c6c 6572 2066  e size smaller f
+0001f8f0: 6f72 2074 6865 206e 6578 7420 6c61 7965  or the next laye
+0001f900: 7220 6f66 2069 6e6e 6572 2028 6669 746e  r of inner (fitn
+0001f910: 6573 7329 2063 6972 636c 6573 0a20 2020  ess) circles.   
+0001f920: 2020 2020 2020 2020 2073 697a 6520 3d20           size = 
+0001f930: 726f 756e 6428 302e 342a 7369 7a65 290a  round(0.4*size).
+0001f940: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
+0001f950: 7420 7369 7a65 7320 666f 7220 616c 6c20  t sizes for all 
+0001f960: 696e 6469 7669 6475 616c 7327 2069 6e6e  individuals' inn
+0001f970: 6572 2d63 6972 636c 6520 6669 746e 6573  er-circle fitnes
+0001f980: 7320 706f 696e 7473 2c20 6966 0a20 2020  s points, if.   
+0001f990: 2020 2020 2020 2020 2023 2074 7274 5f6e           # trt_n
+0001f9a0: 756d 2069 7320 6e6f 7420 4e6f 6e65 0a20  um is not None. 
+0001f9b0: 2020 2020 2020 2020 2020 2069 6620 7472             if tr
+0001f9c0: 745f 6e75 6d20 6973 206e 6f74 204e 6f6e  t_num is not Non
+0001f9d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001f9e0: 2020 2073 697a 6520 3d20 7369 7a65 202a     size = size *
+0001f9f0: 2028 3120 2d20 2828 6e70 2e61 7272 6179   (1 - ((np.array
+0001fa00: 285b 2a77 2e76 616c 7565 7328 0a20 2020  ([*w.values(.   
+0001fa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fa30: 2020 2020 2020 2020 2029 5d29 202d 206d           )]) - m
+0001fa40: 696e 5f66 6974 2920 2f20 2831 202d 206d  in_fit) / (1 - m
+0001fa50: 696e 5f66 6974 2929 290a 0a20 2020 2020  in_fit)))..     
+0001fa60: 2020 2073 656c 662e 5f70 6c6f 7428 6c79     self._plot(ly
+0001fa70: 725f 6e75 6d3d 6c79 725f 6e75 6d2c 206c  r_num=lyr_num, l
+0001fa80: 616e 643d 6c61 6e64 2c20 6869 6465 5f6c  and=land, hide_l
+0001fa90: 616e 643d 5472 7565 2c0a 2020 2020 2020  and=True,.      
+0001faa0: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+0001fab0: 6976 6964 733d 696e 6469 7669 6473 2c20  ivids=individs, 
+0001fac0: 7465 7874 3d74 6578 742c 2063 6f6c 6f72  text=text, color
+0001fad0: 3d6c 6973 7428 772e 7661 6c75 6573 2829  =list(w.values()
+0001fae0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001faf0: 2020 2020 2020 7074 5f63 6d61 703d 636d        pt_cmap=cm
+0001fb00: 6170 2c20 7369 7a65 3d73 697a 652c 2065  ap, size=size, e
+0001fb10: 6467 655f 636f 6c6f 723d 6564 6765 5f63  dge_color=edge_c
+0001fb20: 6f6c 6f72 2c0a 2020 2020 2020 2020 2020  olor,.          
+0001fb30: 2020 2020 2020 2020 2074 6578 745f 636f           text_co
+0001fb40: 6c6f 723d 7465 7874 5f63 6f6c 6f72 2c20  lor=text_color, 
+0001fb50: 6362 6172 3d63 6261 722c 2074 6578 745f  cbar=cbar, text_
+0001fb60: 7369 7a65 3d74 6578 745f 7369 7a65 2c0a  size=text_size,.
+0001fb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fb80: 2020 2061 6c70 6861 3d61 6c70 6861 2c20     alpha=alpha, 
+0001fb90: 7a6f 6f6d 5f77 6964 7468 3d7a 6f6f 6d5f  zoom_width=zoom_
+0001fba0: 7769 6474 682c 2078 3d78 2c20 793d 792c  width, x=x, y=y,
+0001fbb0: 2074 6963 6b73 3d74 6963 6b73 2c0a 2020   ticks=ticks,.  
+0001fbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fbd0: 206d 6173 6b5f 7261 7374 3d6d 6173 6b5f   mask_rast=mask_
+0001fbe0: 7261 7374 290a 0a20 2020 2020 2020 2023  rast)..        #
+0001fbf0: 706c 6f74 2070 6865 6e6f 7479 7065 2074  plot phenotype t
+0001fc00: 6578 7420 2877 6f72 6b73 206f 6e6c 7920  ext (works only 
+0001fc10: 6966 2070 6c6f 7474 696e 6720 6120 7370  if plotting a sp
+0001fc20: 6563 6966 6963 2074 7261 6974 290a 2020  ecific trait).  
+0001fc30: 2020 2020 2020 6966 2070 6865 6e6f 7479        if phenoty
+0001fc40: 7065 5f74 6578 7420 616e 6420 7472 745f  pe_text and trt_
+0001fc50: 6e75 6d20 6973 206e 6f74 204e 6f6e 653a  num is not None:
+0001fc60: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0001fc70: 2069 6e64 2069 6e20 7365 6c66 2e76 616c   ind in self.val
+0001fc80: 7565 7328 293a 0a20 2020 2020 2020 2020  ues():.         
+0001fc90: 2020 2020 2020 2070 6c74 2e74 6578 7428         plt.text(
+0001fca0: 696e 642e 782d 302e 352c 2069 6e64 2e79  ind.x-0.5, ind.y
+0001fcb0: 2d30 2e35 2c20 2725 302e 3266 2720 2520  -0.5, '%0.2f' % 
+0001fcc0: 696e 642e 7a5b 7472 745f 6e75 6d5d 2c0a  ind.z[trt_num],.
+0001fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fce0: 2020 2020 636f 6c6f 7220 3d20 7068 656e      color = phen
+0001fcf0: 6f74 7970 655f 7465 7874 5f63 6f6c 6f72  otype_text_color
+0001fd00: 2c20 7369 7a65 203d 2074 6578 745f 7369  , size = text_si
+0001fd10: 7a65 290a 0a20 2020 2020 2020 2023 706c  ze)..        #pl
+0001fd20: 6f74 2066 6974 6e65 7373 2074 6578 740a  ot fitness text.
+0001fd30: 2020 2020 2020 2020 6966 2066 6974 6e65          if fitne
+0001fd40: 7373 5f74 6578 743a 0a20 2020 2020 2020  ss_text:.       
+0001fd50: 2020 2020 206f 6666 7365 745f 6672 6f6d       offset_from
+0001fd60: 5f70 6865 6e6f 7479 7065 5f74 6578 7420  _phenotype_text 
+0001fd70: 3d20 302e 3030 312a 6d61 7828 7365 6c66  = 0.001*max(self
+0001fd80: 2e5f 6c61 6e64 5f64 696d 290a 2020 2020  ._land_dim).    
+0001fd90: 2020 2020 2020 2020 666f 7220 696e 6420          for ind 
+0001fda0: 696e 2073 656c 662e 7661 6c75 6573 2829  in self.values()
+0001fdb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001fdc0: 2020 706c 742e 7465 7874 2869 6e64 2e78    plt.text(ind.x
+0001fdd0: 2d30 2e35 2b6f 6666 7365 745f 6672 6f6d  -0.5+offset_from
+0001fde0: 5f70 6865 6e6f 7479 7065 5f74 6578 742c  _phenotype_text,
+0001fdf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fe00: 2020 2020 2020 2020 2020 696e 642e 792d            ind.y-
+0001fe10: 302e 352b 6f66 6673 6574 5f66 726f 6d5f  0.5+offset_from_
+0001fe20: 7068 656e 6f74 7970 655f 7465 7874 2c0a  phenotype_text,.
+0001fe30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fe40: 2020 2020 2020 2020 2027 2530 2e32 6627           '%0.2f'
+0001fe50: 2025 2069 6e64 2e66 6974 2c20 636f 6c6f   % ind.fit, colo
+0001fe60: 7220 3d20 6669 746e 6573 735f 7465 7874  r = fitness_text
+0001fe70: 5f63 6f6c 6f72 2c0a 2020 2020 2020 2020  _color,.        
+0001fe80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fe90: 2073 697a 6520 3d20 7465 7874 5f73 697a   size = text_siz
+0001fea0: 6529 0a0a 2020 2020 2020 2020 2361 6e64  e)..        #and
+0001feb0: 206d 616b 6520 6120 636f 6c6f 7262 6172   make a colorbar
+0001fec0: 2066 6f72 2074 6865 2066 6974 6e65 7373   for the fitness
+0001fed0: 2076 616c 7565 7320 0a20 2020 2020 2020   values .       
+0001fee0: 2069 6620 6669 746e 6573 735f 6362 6172   if fitness_cbar
+0001fef0: 3a0a 2020 2020 2020 2020 2020 2020 7669  :.            vi
+0001ff00: 7a2e 5f6d 616b 655f 6669 746e 6573 735f  z._make_fitness_
+0001ff10: 6362 6172 286d 616b 655f 6362 6172 5f66  cbar(make_cbar_f
+0001ff20: 6e2c 206d 696e 5f66 6974 290a 0a20 2020  n, min_fit)..   
+0001ff30: 2023 6d65 7468 6f64 2074 6f20 706c 6f74   #method to plot
+0001ff40: 2061 2073 7065 6369 6573 2720 616c 6c65   a species' alle
+0001ff50: 6c65 2066 7265 7175 656e 6369 6573 0a20  le frequencies. 
+0001ff60: 2020 2064 6566 205f 706c 6f74 5f61 6c6c     def _plot_all
+0001ff70: 656c 655f 6672 6571 7565 6e63 6965 7328  ele_frequencies(
+0001ff80: 7365 6c66 2c20 636f 6c6f 723d 2772 6564  self, color='red
+0001ff90: 2729 3a0a 2020 2020 2020 2020 6966 2073  '):.        if s
+0001ffa0: 656c 662e 6765 6e5f 6172 6368 2069 7320  elf.gen_arch is 
+0001ffb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0001ffc0: 2020 7072 696e 7428 2822 5370 6563 6965    print(("Specie
+0001ffd0: 732e 5f70 6c6f 745f 616c 6c65 6c65 5f66  s._plot_allele_f
+0001ffe0: 7265 7175 656e 6369 6573 2069 7320 6e6f  requencies is no
+0001fff0: 7420 7661 6c69 6420 666f 7220 220a 2020  t valid for ".  
+00020000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020010: 2022 7370 6563 6965 7320 7769 7468 6f75   "species withou
+00020020: 7420 6765 6e6f 6d65 732e 5c6e 2229 290a  t genomes.\n")).
+00020030: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00020040: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+00020050: 656e 5f61 7263 682e 5f70 6c6f 745f 616c  en_arch._plot_al
+00020060: 6c65 6c65 5f66 7265 7175 656e 6369 6573  lele_frequencies
+00020070: 2873 656c 662c 2063 6f6c 6f72 3d63 6f6c  (self, color=col
+00020080: 6f72 290a 0a20 2020 2023 206d 6574 686f  or)..    # metho
+00020090: 6420 666f 7220 706c 6f74 7469 6e67 2061  d for plotting a
+000200a0: 2068 6973 746f 6772 616d 206f 6620 7468   histogram of th
+000200b0: 6520 6375 7272 656e 7420 6669 746e 6573  e current fitnes
+000200c0: 7320 7661 6c75 6573 0a20 2020 2064 6566  s values.    def
+000200d0: 205f 706c 6f74 5f68 6973 745f 6669 746e   _plot_hist_fitn
+000200e0: 6573 7328 7365 6c66 293a 0a20 2020 2020  ess(self):.     
+000200f0: 2020 2070 6c74 2e68 6973 7428 6c69 7374     plt.hist(list
+00020100: 2873 656c 662e 5f63 616c 635f 6669 746e  (self._calc_fitn
+00020110: 6573 7328 2929 290a 2020 2020 2020 2020  ess())).        
+00020120: 706c 742e 786c 6162 656c 2827 4669 746e  plt.xlabel('Fitn
+00020130: 6573 7327 290a 2020 2020 2020 2020 706c  ess').        pl
+00020140: 742e 796c 6162 656c 2827 436f 756e 7427  t.ylabel('Count'
+00020150: 290a 0a20 2020 2023 206d 6574 686f 6420  )..    # method 
+00020160: 666f 7220 706c 6f74 7469 6e67 2074 6865  for plotting the
+00020170: 206d 6f76 656d 656e 7420 7375 7266 6163   movement surfac
+00020180: 6520 2869 6e20 7661 7269 6f75 7320 666f  e (in various fo
+00020190: 726d 6174 7329 0a20 2020 2064 6566 205f  rmats).    def _
+000201a0: 706c 6f74 5f64 6972 6563 7469 6f6e 5f73  plot_direction_s
+000201b0: 7572 6661 6365 2873 656c 662c 206c 616e  urface(self, lan
+000201c0: 642c 2073 7572 665f 7479 7065 2c20 7374  d, surf_type, st
+000201d0: 796c 652c 2078 3d4e 6f6e 652c 2079 3d4e  yle, x=None, y=N
+000201e0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+000201f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020200: 2020 2020 207a 6f6f 6d5f 7769 6474 683d       zoom_width=
+00020210: 4e6f 6e65 2c20 7363 616c 655f 6661 6374  None, scale_fact
+00020220: 3d34 2e35 2c0a 2020 2020 2020 2020 2020  =4.5,.          
+00020230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020240: 2020 2020 2020 636f 6c6f 723d 2762 6c61        color='bla
+00020250: 636b 272c 2063 6261 723d 5472 7565 2c20  ck', cbar=True, 
+00020260: 7469 636b 733d 4e6f 6e65 2c0a 2020 2020  ticks=None,.    
+00020270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020280: 2020 2020 2020 2020 2020 2020 636d 6170              cmap
+00020290: 3d27 706c 6173 6d61 272c 206d 6173 6b5f  ='plasma', mask_
+000202a0: 7261 7374 3d4e 6f6e 6529 3a0a 2020 2020  rast=None):.    
+000202b0: 2020 2020 2320 6765 7420 7468 6520 636f      # get the co
+000202c0: 7272 6563 7420 7375 7266 6163 650a 2020  rrect surface.  
+000202d0: 2020 2020 2020 6966 2073 7572 665f 7479        if surf_ty
+000202e0: 7065 203d 3d20 276d 6f76 6527 3a0a 2020  pe == 'move':.  
+000202f0: 2020 2020 2020 2020 2020 7375 7266 203d            surf =
+00020300: 2073 656c 662e 5f6d 6f76 655f 7375 7266   self._move_surf
+00020310: 0a20 2020 2020 2020 2065 6c69 6620 7375  .        elif su
+00020320: 7266 5f74 7970 6520 3d3d 2027 6469 7370  rf_type == 'disp
+00020330: 273a 0a20 2020 2020 2020 2020 2020 2073  ':.            s
+00020340: 7572 6620 3d3d 2073 656c 662e 5f64 6973  urf == self._dis
+00020350: 705f 7375 7266 0a0a 2020 2020 2020 2020  p_surf..        
+00020360: 2320 6765 7420 616c 6c20 7827 7320 616e  # get all x's an
+00020370: 6420 7927 732c 2069 6620 7820 616e 6420  d y's, if x and 
+00020380: 7920 6172 6520 4e6f 6e65 0a20 2020 2020  y are None.     
+00020390: 2020 2069 6620 7820 6973 204e 6f6e 6520     if x is None 
+000203a0: 616e 6420 7920 6973 204e 6f6e 653a 0a20  and y is None:. 
+000203b0: 2020 2020 2020 2020 2020 2078 203d 205b             x = [
+000203c0: 2a72 616e 6765 286c 616e 642e 6469 6d5b  *range(land.dim[
+000203d0: 305d 295d 0a20 2020 2020 2020 2020 2020  0])].           
+000203e0: 2079 203d 205b 2a72 616e 6765 286c 616e   y = [*range(lan
+000203f0: 642e 6469 6d5b 315d 295d 0a20 2020 2020  d.dim[1])].     
+00020400: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00020410: 2020 2020 2078 203d 205b 785d 0a20 2020       x = [x].   
+00020420: 2020 2020 2020 2020 2079 203d 205b 795d           y = [y]
+00020430: 0a20 2020 2020 2020 2023 6368 6563 6b20  .        #check 
+00020440: 6966 2074 6865 2073 7572 6661 6365 2069  if the surface i
+00020450: 7320 6e6f 6e65 0a20 2020 2020 2020 2069  s none.        i
+00020460: 6620 7375 7266 2069 7320 4e6f 6e65 3a0a  f surf is None:.
+00020470: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00020480: 7428 2827 4675 6e63 7469 6f6e 206e 6f74  t(('Function not
+00020490: 2076 616c 6964 2066 6f72 2061 2053 7065   valid for a Spe
+000204a0: 6369 6573 2077 6974 6820 6e6f 2027 0a20  cies with no '. 
+000204b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000204c0: 2020 275f 2573 5375 7266 6163 652e 2729    '_%sSurface.')
+000204d0: 2025 2028 7b0a 2020 2020 2020 2020 2020   % ({.          
+000204e0: 2020 2020 2020 276d 6f76 6527 3a20 274d        'move': 'M
+000204f0: 6f76 656d 656e 7427 2c20 2764 6973 7027  ovement', 'disp'
+00020500: 3a20 2744 6973 7065 7273 616c 277d 5b73  : 'Dispersal'}[s
+00020510: 7572 665f 7479 7065 5d29 290a 2020 2020  urf_type])).    
+00020520: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00020530: 2020 2020 2020 2065 6c69 6620 7374 796c         elif styl
+00020540: 6520 6e6f 7420 696e 205b 2768 6973 7427  e not in ['hist'
+00020550: 2c20 2763 6869 7374 272c 2027 7665 6374  , 'chist', 'vect
+00020560: 272c 2027 6364 7261 7773 275d 3a0a 2020  ', 'cdraws']:.  
+00020570: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00020580: 2822 5468 6520 2773 7479 6c65 2720 6172  ("The 'style' ar
+00020590: 6775 6d65 6e74 206d 7573 7420 7461 6b65  gument must take
+000205a0: 206f 6e65 206f 6620 7468 6520 220a 2020   one of the ".  
+000205b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000205c0: 2022 666f 6c6c 6f77 696e 6720 7661 6c75   "following valu
+000205d0: 6573 3a20 2768 6973 7427 2c20 2763 6869  es: 'hist', 'chi
+000205e0: 7374 272c 2022 0a20 2020 2020 2020 2020  st', ".         
+000205f0: 2020 2020 2020 2020 2020 2227 7665 6374            "'vect
+00020600: 272c 2027 6364 7261 7773 2722 2929 0a20  ', 'cdraws'")). 
+00020610: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00020620: 6e0a 2020 2020 2020 2020 656c 6966 2073  n.        elif s
+00020630: 7479 6c65 203d 3d20 2768 6973 7427 3a0a  tyle == 'hist':.
+00020640: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
+00020650: 785b 305d 0a20 2020 2020 2020 2020 2020  x[0].           
+00020660: 2079 203d 2079 5b30 5d0a 2020 2020 2020   y = y[0].      
+00020670: 2020 2020 2020 706c 742e 6869 7374 2872        plt.hist(r
+00020680: 2e63 686f 6963 6528 7375 7266 2e73 7572  .choice(surf.sur
+00020690: 665b 792c 782c 3a5d 2c20 7369 7a65 203d  f[y,x,:], size =
+000206a0: 2031 3030 3030 2c20 7265 706c 6163 6520   10000, replace 
+000206b0: 3d20 5472 7565 292c 0a20 2020 2020 2020  = True),.       
+000206c0: 2020 2020 2020 2020 2020 2020 2020 6269                bi
+000206d0: 6e73 3d31 3030 2c20 6465 6e73 6974 793d  ns=100, density=
+000206e0: 5472 7565 2c20 616c 7068 613d 302e 352c  True, alpha=0.5,
+000206f0: 2063 6f6c 6f72 3d63 6f6c 6f72 290a 0a20   color=color).. 
+00020700: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00020710: 2020 2020 2020 2020 2023 6469 7370 6c61           #displa
+00020720: 7920 7468 6520 6d6f 7665 6d65 6e74 2d73  y the movement-s
+00020730: 7572 6661 6365 2072 6173 7465 720a 2020  urface raster.  
+00020740: 2020 2020 2020 2020 2020 6c79 725f 6e75            lyr_nu
+00020750: 6d20 3d20 7375 7266 2e6c 7972 5f6e 756d  m = surf.lyr_num
+00020760: 0a20 2020 2020 2020 2020 2020 206c 616e  .            lan
+00020770: 645b 6c79 725f 6e75 6d5d 2e5f 706c 6f74  d[lyr_num]._plot
+00020780: 287a 6f6f 6d5f 7769 6474 6820 3d20 7a6f  (zoom_width = zo
+00020790: 6f6d 5f77 6964 7468 2c20 783d 6e70 2e6d  om_width, x=np.m
+000207a0: 6561 6e28 7829 2c0a 2020 2020 2020 2020  ean(x),.        
+000207b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000207c0: 2020 2020 2020 2020 793d 6e70 2e6d 6561          y=np.mea
+000207d0: 6e28 7929 2c20 7469 636b 733d 7469 636b  n(y), ticks=tick
+000207e0: 732c 2063 6d61 703d 636d 6170 2c0a 2020  s, cmap=cmap,.  
+000207f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020800: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00020810: 736b 5f72 6173 743d 6d61 736b 5f72 6173  sk_rast=mask_ras
+00020820: 7429 0a0a 2020 2020 2020 2020 2020 2020  t)..            
+00020830: 6966 2073 7479 6c65 203d 3d20 2763 6869  if style == 'chi
+00020840: 7374 273a 0a20 2020 2020 2020 2020 2020  st':.           
+00020850: 2020 2020 2066 6f72 2078 5f76 616c 2069       for x_val i
+00020860: 6e20 783a 0a20 2020 2020 2020 2020 2020  n x:.           
+00020870: 2020 2020 2020 2020 2066 6f72 2079 5f76           for y_v
+00020880: 616c 2069 6e20 793a 0a20 2020 2020 2020  al in y:.       
+00020890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000208a0: 2076 2c20 6120 3d20 6e70 2e68 6973 746f   v, a = np.histo
+000208b0: 6772 616d 2872 2e63 686f 6963 6528 7375  gram(r.choice(su
+000208c0: 7266 2e73 7572 665b 795f 7661 6c2c 0a20  rf.surf[y_val,. 
+000208d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000208e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000208f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020900: 2028 795f 7661 6c20 2b20 302e 352c 2028   (y_val + 0.5, (
-00020910: 795f 7661 6c20 2b20 302e 3520 2b20 7973  y_val + 0.5 + ys
-00020920: 5b6e 5d29 292c 0a20 2020 2020 2020 2020  [n])),.         
+00020900: 2020 2020 2020 2020 2020 2020 2020 785f                x_
+00020910: 7661 6c2c 203a 5d2c 0a20 2020 2020 2020  val, :],.       
+00020920: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020940: 2020 2020 2020 2020 206c 696e 6577 6964           linewid
-00020950: 7468 3d32 2c0a 2020 2020 2020 2020 2020  th=2,.          
+00020940: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00020950: 706c 6163 653d 5472 7565 2c0a 2020 2020  place=True,.    
 00020960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020970: 2020 2020 2020 2020 636f 6c6f 723d 636f          color=co
-00020980: 6c6f 7229 2066 6f72 206e 2069 6e20 7261  lor) for n in ra
-00020990: 6e67 6528 6c65 6e28 7873 2929 5d0a 0a20  nge(len(xs))].. 
-000209a0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-000209b0: 7374 796c 6520 3d3d 2027 6364 7261 7773  style == 'cdraws
-000209c0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-000209d0: 2020 2066 6f72 2078 5f76 616c 2069 6e20     for x_val in 
-000209e0: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
-000209f0: 2020 2020 2020 2066 6f72 2079 5f76 616c         for y_val
-00020a00: 2069 6e20 793a 0a20 2020 2020 2020 2020   in y:.         
-00020a10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00020a20: 7473 203d 205b 286e 702e 636f 7328 6129  ts = [(np.cos(a)
-00020a30: 2c20 6e70 2e73 696e 2861 2929 2066 6f72  , np.sin(a)) for
-00020a40: 2061 2069 6e20 722e 6368 6f69 6365 280a   a in r.choice(.
-00020a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020a70: 7375 7266 2e73 7572 665b 795f 7661 6c2c  surf.surf[y_val,
-00020a80: 2078 5f76 616c 2c20 3a5d 2c20 7369 7a65   x_val, :], size
-00020a90: 3d31 3030 302c 0a20 2020 2020 2020 2020  =1000,.         
-00020aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ab0: 2020 2020 2020 2072 6570 6c61 6365 3d54         replace=T
-00020ac0: 7275 6529 5d0a 2020 2020 2020 2020 2020  rue)].          
-00020ad0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00020ae0: 742e 7363 6174 7465 7228 5b70 745b 305d  t.scatter([pt[0]
-00020af0: 202a 2030 2e35 202b 2078 5f76 616c 202b   * 0.5 + x_val +
-00020b00: 2030 2e35 2066 6f72 2070 7420 696e 2070   0.5 for pt in p
-00020b10: 7473 5d2c 0a20 2020 2020 2020 2020 2020  ts],.           
-00020b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b30: 2020 2020 2020 2020 205b 7074 5b31 5d20           [pt[1] 
-00020b40: 2a20 302e 3520 2b20 795f 7661 6c20 2b20  * 0.5 + y_val + 
-00020b50: 302e 3520 666f 7220 7074 2069 6e20 7074  0.5 for pt in pt
-00020b60: 735d 2c0a 2020 2020 2020 2020 2020 2020  s],.            
-00020b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b80: 2020 2020 2020 2020 636f 6c6f 723d 636f          color=co
-00020b90: 6c6f 722c 2061 6c70 6861 3d30 2e31 2c20  lor, alpha=0.1, 
-00020ba0: 6d61 726b 6572 3d27 2e27 290a 0a20 2020  marker='.')..   
-00020bb0: 2020 2020 2020 2020 2065 6c69 6620 7374           elif st
-00020bc0: 796c 6520 3d3d 2027 7665 6374 273a 0a20  yle == 'vect':. 
-00020bd0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00020be0: 6566 2070 6c6f 745f 6f6e 655f 6365 6c6c  ef plot_one_cell
-00020bf0: 2878 2c20 7929 3a0a 2020 2020 2020 2020  (x, y):.        
-00020c00: 2020 2020 2020 2020 2020 2020 2320 6472              # dr
-00020c10: 6177 2073 616d 706c 6520 6f66 2061 6e67  aw sample of ang
-00020c20: 6c65 7320 6672 6f6d 2074 6865 2047 6175  les from the Gau
-00020c30: 7373 6961 6e20 4b44 450a 2020 2020 2020  ssian KDE.      
-00020c40: 2020 2020 2020 2020 2020 2020 2020 2372                #r
-00020c50: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
-00020c60: 766f 6e20 6d69 7365 7320 6d69 7874 7572  von mises mixtur
-00020c70: 6520 6469 7374 7269 6275 7469 6f6e 2028  e distribution (
-00020c80: 4b44 4529 0a20 2020 2020 2020 2020 2020  KDE).           
-00020c90: 2020 2020 2020 2020 2073 616d 7020 3d20           samp = 
-00020ca0: 7375 7266 2e73 7572 665b 792c 782c 3a5d  surf.surf[y,x,:]
-00020cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020cc0: 2020 2020 2023 2063 7265 6174 6520 6c69       # create li
-00020cd0: 7374 7320 6f66 2074 6865 2078 2061 6e64  sts of the x and
-00020ce0: 2079 2028 692e 652e 2063 6f73 2061 6e64   y (i.e. cos and
-00020cf0: 2073 696e 290a 2020 2020 2020 2020 2020   sin).          
-00020d00: 2020 2020 2020 2020 2020 2363 6f6d 706f            #compo
-00020d10: 6e65 6e74 7320 6f66 2065 6163 6820 616e  nents of each an
-00020d20: 676c 6520 696e 2074 6865 2073 616d 706c  gle in the sampl
-00020d30: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00020d40: 2020 2020 2020 785f 7665 6374 7320 3d20        x_vects = 
-00020d50: 6e70 2e63 6f73 2873 616d 7029 0a20 2020  np.cos(samp).   
+00020970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020990: 2073 697a 653d 3735 3030 292c 2062 696e   size=7500), bin
+000209a0: 733d 3135 290a 2020 2020 2020 2020 2020  s=15).          
+000209b0: 2020 2020 2020 2020 2020 2020 2020 7620                v 
+000209c0: 3d20 7620 2f20 666c 6f61 7428 762e 7375  = v / float(v.su
+000209d0: 6d28 2929 0a20 2020 2020 2020 2020 2020  m()).           
+000209e0: 2020 2020 2020 2020 2020 2020 2061 203d               a =
+000209f0: 205b 2861 5b6e 5d20 2b20 615b 6e20 2b20   [(a[n] + a[n + 
+00020a00: 315d 2920 2f20 3220 666f 7220 6e20 696e  1]) / 2 for n in
+00020a10: 2072 616e 6765 286c 656e 2861 2920 2d20   range(len(a) - 
+00020a20: 3129 5d0a 2020 2020 2020 2020 2020 2020  1)].            
+00020a30: 2020 2020 2020 2020 2020 2020 7873 203d              xs =
+00020a40: 205b 6e70 2e63 6f73 2861 5b6e 5d29 202a   [np.cos(a[n]) *
+00020a50: 2030 2e37 3520 666f 7220 6e20 696e 2072   0.75 for n in r
+00020a60: 616e 6765 286c 656e 2861 2929 5d0a 2020  ange(len(a))].  
+00020a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020a80: 2020 2020 2020 7973 203d 205b 6e70 2e73        ys = [np.s
+00020a90: 696e 2861 5b6e 5d29 202a 2030 2e37 3520  in(a[n]) * 0.75 
+00020aa0: 666f 7220 6e20 696e 2072 616e 6765 286c  for n in range(l
+00020ab0: 656e 2861 2929 5d0a 2020 2020 2020 2020  en(a))].        
+00020ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020ad0: 7873 203d 206e 702e 6172 7261 7928 7873  xs = np.array(xs
+00020ae0: 2920 2a20 7620 2a20 7363 616c 655f 6661  ) * v * scale_fa
+00020af0: 6374 0a20 2020 2020 2020 2020 2020 2020  ct.             
+00020b00: 2020 2020 2020 2020 2020 2079 7320 3d20             ys = 
+00020b10: 6e70 2e61 7272 6179 2879 7329 202a 2076  np.array(ys) * v
+00020b20: 202a 2073 6361 6c65 5f66 6163 740a 2020   * scale_fact.  
+00020b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020b40: 2020 2020 2020 5b70 6c74 2e70 6c6f 7428        [plt.plot(
+00020b50: 2878 5f76 616c 202b 2030 2e35 2c20 2878  (x_val + 0.5, (x
+00020b60: 5f76 616c 202b 2030 2e35 202b 2078 735b  _val + 0.5 + xs[
+00020b70: 6e5d 2929 2c0a 2020 2020 2020 2020 2020  n])),.          
+00020b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020b90: 2020 2020 2020 2020 2879 5f76 616c 202b          (y_val +
+00020ba0: 2030 2e35 2c20 2879 5f76 616c 202b 2030   0.5, (y_val + 0
+00020bb0: 2e35 202b 2079 735b 6e5d 2929 2c0a 2020  .5 + ys[n])),.  
+00020bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020be0: 6c69 6e65 7769 6474 683d 322c 0a20 2020  linewidth=2,.   
+00020bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00020c10: 6f6c 6f72 3d63 6f6c 6f72 2920 666f 7220  olor=color) for 
+00020c20: 6e20 696e 2072 616e 6765 286c 656e 2878  n in range(len(x
+00020c30: 7329 295d 0a0a 2020 2020 2020 2020 2020  s))]..          
+00020c40: 2020 656c 6966 2073 7479 6c65 203d 3d20    elif style == 
+00020c50: 2763 6472 6177 7327 3a0a 2020 2020 2020  'cdraws':.      
+00020c60: 2020 2020 2020 2020 2020 666f 7220 785f            for x_
+00020c70: 7661 6c20 696e 2078 3a0a 2020 2020 2020  val in x:.      
+00020c80: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00020c90: 7220 795f 7661 6c20 696e 2079 3a0a 2020  r y_val in y:.  
+00020ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020cb0: 2020 2020 2020 7074 7320 3d20 5b28 6e70        pts = [(np
+00020cc0: 2e63 6f73 2861 292c 206e 702e 7369 6e28  .cos(a), np.sin(
+00020cd0: 6129 2920 666f 7220 6120 696e 2072 2e63  a)) for a in r.c
+00020ce0: 686f 6963 6528 0a20 2020 2020 2020 2020  hoice(.         
+00020cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d00: 2020 2020 2020 2073 7572 662e 7375 7266         surf.surf
+00020d10: 5b79 5f76 616c 2c20 785f 7661 6c2c 203a  [y_val, x_val, :
+00020d20: 5d2c 2073 697a 653d 3130 3030 2c0a 2020  ], size=1000,.  
+00020d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d40: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00020d50: 706c 6163 653d 5472 7565 295d 0a20 2020  place=True)].   
 00020d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d70: 2079 5f76 6563 7473 203d 206e 702e 7369   y_vects = np.si
-00020d80: 6e28 7361 6d70 290a 2020 2020 2020 2020  n(samp).        
-00020d90: 2020 2020 2020 2020 2020 2020 2320 6465              # de
-00020da0: 6669 6e65 2074 6865 2064 7820 616e 6420  fine the dx and 
-00020db0: 6479 2064 6973 7461 6e63 6573 2075 7365  dy distances use
-00020dc0: 6420 746f 2074 6865 0a20 2020 2020 2020  d to the.       
-00020dd0: 2020 2020 2020 2020 2020 2020 2023 706f               #po
-00020de0: 7369 7469 6f6e 2074 6865 2061 7272 6f77  sition the arrow
-00020df0: 6865 6164 2028 6469 7669 6465 2062 7920  head (divide by 
-00020e00: 7371 7274 2832 292f 322c 2074 6f20 0a20  sqrt(2)/2, to . 
-00020e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e20: 2020 2023 7363 616c 6520 746f 2074 6865     #scale to the
-00020e30: 2073 697a 6520 6f66 2068 616c 6620 6f66   size of half of
-00020e40: 2074 6865 2064 6961 676f 6e61 6c20 6f66   the diagonal of
-00020e50: 2061 2063 656c 6c29 0a20 2020 2020 2020   a cell).       
-00020e60: 2020 2020 2020 2020 2020 2020 2064 7820               dx 
-00020e70: 3d20 6e70 2e6d 6561 6e28 785f 7665 6374  = np.mean(x_vect
-00020e80: 7329 202f 206e 702e 7371 7274 2832 290a  s) / np.sqrt(2).
+00020d70: 2020 2020 2070 6c74 2e73 6361 7474 6572       plt.scatter
+00020d80: 285b 7074 5b30 5d20 2a20 302e 3520 2b20  ([pt[0] * 0.5 + 
+00020d90: 785f 7661 6c20 2b20 302e 3520 666f 7220  x_val + 0.5 for 
+00020da0: 7074 2069 6e20 7074 735d 2c0a 2020 2020  pt in pts],.    
+00020db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020dd0: 5b70 745b 315d 202a 2030 2e35 202b 2079  [pt[1] * 0.5 + y
+00020de0: 5f76 616c 202b 2030 2e35 2066 6f72 2070  _val + 0.5 for p
+00020df0: 7420 696e 2070 7473 5d2c 0a20 2020 2020  t in pts],.     
+00020e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020e10: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00020e20: 6f6c 6f72 3d63 6f6c 6f72 2c20 616c 7068  olor=color, alph
+00020e30: 613d 302e 312c 206d 6172 6b65 723d 272e  a=0.1, marker='.
+00020e40: 2729 0a0a 2020 2020 2020 2020 2020 2020  ')..            
+00020e50: 656c 6966 2073 7479 6c65 203d 3d20 2776  elif style == 'v
+00020e60: 6563 7427 3a0a 2020 2020 2020 2020 2020  ect':.          
+00020e70: 2020 2020 2020 6465 6620 706c 6f74 5f6f        def plot_o
+00020e80: 6e65 5f63 656c 6c28 782c 2079 293a 0a20  ne_cell(x, y):. 
 00020e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ea0: 2020 2020 6479 203d 206e 702e 6d65 616e      dy = np.mean
-00020eb0: 2879 5f76 6563 7473 2920 2f20 6e70 2e73  (y_vects) / np.s
-00020ec0: 7172 7428 3229 0a20 2020 2020 2020 2020  qrt(2).         
-00020ed0: 2020 2020 2020 2020 2020 2023 206e 6f77             # now
-00020ee0: 2070 6c6f 7420 7468 6520 6172 726f 770a   plot the arrow.
-00020ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020f00: 2020 2020 706c 742e 6172 726f 7728 7820      plt.arrow(x 
-00020f10: 2b20 302e 352c 2079 202b 2030 2e35 2c20  + 0.5, y + 0.5, 
-00020f20: 6478 2c20 6479 2c20 616c 7068 613d 302e  dx, dy, alpha=0.
-00020f30: 3735 2c0a 2020 2020 2020 2020 2020 2020  75,.            
-00020f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020f50: 2020 636f 6c6f 723d 636f 6c6f 722c 2068    color=color, h
-00020f60: 6561 645f 7769 6474 683d 302e 3234 2c20  ead_width=0.24, 
-00020f70: 6865 6164 5f6c 656e 6774 683d 302e 3332  head_length=0.32
-00020f80: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00020f90: 2020 2023 2063 616c 6c20 7468 6520 696e     # call the in
-00020fa0: 7465 726e 616c 6c79 2064 6566 696e 6564  ternally defined
-00020fb0: 2066 756e 6374 696f 6e20 6173 2061 206e   function as a n
-00020fc0: 6573 7465 6420 6c69 7374 0a20 2020 2020  ested list.     
-00020fd0: 2020 2020 2020 2020 2020 2023 636f 6d70             #comp
-00020fe0: 7265 6865 6e73 696f 6e20 666f 7220 616c  rehension for al
-00020ff0: 6c20 7261 7374 6572 2063 656c 6c73 2c20  l raster cells, 
-00021000: 7768 6963 6820 4920 6265 6c69 6576 650a  which I believe.
-00021010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021020: 2373 686f 756c 6420 646f 2069 7473 2062  #should do its b
-00021030: 6573 7420 746f 2076 6563 746f 7269 7a65  est to vectorize
-00021040: 2074 6865 2077 686f 6c65 206f 7065 7261   the whole opera
-00021050: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00021060: 2020 2020 205b 5b70 6c6f 745f 6f6e 655f       [[plot_one_
-00021070: 6365 6c6c 286a 2c20 6929 2066 6f72 2069  cell(j, i) for i
-00021080: 2069 6e20 7261 6e67 6528 0a20 2020 2020   in range(.     
-00021090: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000210a0: 7572 662e 7375 7266 2e73 6861 7065 5b30  urf.surf.shape[0
-000210b0: 5d29 5d20 666f 7220 6a20 696e 2072 616e  ])] for j in ran
-000210c0: 6765 280a 2020 2020 2020 2020 2020 2020  ge(.            
-000210d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000210e0: 2020 2020 2020 2020 7375 7266 2e73 7572          surf.sur
-000210f0: 662e 7368 6170 655b 315d 295d 0a0a 0a20  f.shape[1])]... 
-00021100: 2020 2023 2070 6c6f 7420 7468 6520 6c69     # plot the li
-00021110: 6e65 6167 6520 666f 7220 6120 6769 7665  neage for a give
-00021120: 6e20 6e6f 6465 2061 6e64 206c 6f63 7573  n node and locus
-00021130: 0a20 2020 2064 6566 205f 706c 6f74 5f67  .    def _plot_g
-00021140: 656e 655f 666c 6f77 2873 656c 662c 206c  ene_flow(self, l
-00021150: 6f63 7573 2c20 7374 796c 652c 206c 616e  ocus, style, lan
-00021160: 642c 206e 6f64 6573 3d4e 6f6e 652c 2069  d, nodes=None, i
-00021170: 6e64 6976 6964 733d 4e6f 6e65 2c0a 2020  ndivids=None,.  
-00021180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021190: 2020 2020 2063 6f6c 6f72 3d4e 6f6e 652c       color=None,
-000211a0: 2070 6865 6e6f 7479 7065 3d4e 6f6e 652c   phenotype=None,
-000211b0: 206c 7972 5f6e 756d 3d30 2c20 6a69 7474   lyr_num=0, jitt
-000211c0: 6572 3d54 7275 652c 0a20 2020 2020 2020  er=True,.       
+00020ea0: 2020 2023 2064 7261 7720 7361 6d70 6c65     # draw sample
+00020eb0: 206f 6620 616e 676c 6573 2066 726f 6d20   of angles from 
+00020ec0: 7468 6520 4761 7573 7369 616e 204b 4445  the Gaussian KDE
+00020ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020ee0: 2020 2020 2023 7265 7072 6573 656e 7469       #representi
+00020ef0: 6e67 2074 6865 2076 6f6e 206d 6973 6573  ng the von mises
+00020f00: 206d 6978 7475 7265 2064 6973 7472 6962   mixture distrib
+00020f10: 7574 696f 6e20 284b 4445 290a 2020 2020  ution (KDE).    
+00020f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020f30: 7361 6d70 203d 2073 7572 662e 7375 7266  samp = surf.surf
+00020f40: 5b79 2c78 2c3a 5d0a 2020 2020 2020 2020  [y,x,:].        
+00020f50: 2020 2020 2020 2020 2020 2020 2320 6372              # cr
+00020f60: 6561 7465 206c 6973 7473 206f 6620 7468  eate lists of th
+00020f70: 6520 7820 616e 6420 7920 2869 2e65 2e20  e x and y (i.e. 
+00020f80: 636f 7320 616e 6420 7369 6e29 0a20 2020  cos and sin).   
+00020f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020fa0: 2023 636f 6d70 6f6e 656e 7473 206f 6620   #components of 
+00020fb0: 6561 6368 2061 6e67 6c65 2069 6e20 7468  each angle in th
+00020fc0: 6520 7361 6d70 6c65 0a20 2020 2020 2020  e sample.       
+00020fd0: 2020 2020 2020 2020 2020 2020 2078 5f76               x_v
+00020fe0: 6563 7473 203d 206e 702e 636f 7328 7361  ects = np.cos(sa
+00020ff0: 6d70 290a 2020 2020 2020 2020 2020 2020  mp).            
+00021000: 2020 2020 2020 2020 795f 7665 6374 7320          y_vects 
+00021010: 3d20 6e70 2e73 696e 2873 616d 7029 0a20  = np.sin(samp). 
+00021020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021030: 2020 2023 2064 6566 696e 6520 7468 6520     # define the 
+00021040: 6478 2061 6e64 2064 7920 6469 7374 616e  dx and dy distan
+00021050: 6365 7320 7573 6564 2074 6f20 7468 650a  ces used to the.
+00021060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021070: 2020 2020 2370 6f73 6974 696f 6e20 7468      #position th
+00021080: 6520 6172 726f 7768 6561 6420 2864 6976  e arrowhead (div
+00021090: 6964 6520 6279 2073 7172 7428 3229 2f32  ide by sqrt(2)/2
+000210a0: 2c20 746f 200a 2020 2020 2020 2020 2020  , to .          
+000210b0: 2020 2020 2020 2020 2020 2373 6361 6c65            #scale
+000210c0: 2074 6f20 7468 6520 7369 7a65 206f 6620   to the size of 
+000210d0: 6861 6c66 206f 6620 7468 6520 6469 6167  half of the diag
+000210e0: 6f6e 616c 206f 6620 6120 6365 6c6c 290a  onal of a cell).
+000210f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021100: 2020 2020 6478 203d 206e 702e 6d65 616e      dx = np.mean
+00021110: 2878 5f76 6563 7473 2920 2f20 6e70 2e73  (x_vects) / np.s
+00021120: 7172 7428 3229 0a20 2020 2020 2020 2020  qrt(2).         
+00021130: 2020 2020 2020 2020 2020 2064 7920 3d20             dy = 
+00021140: 6e70 2e6d 6561 6e28 795f 7665 6374 7329  np.mean(y_vects)
+00021150: 202f 206e 702e 7371 7274 2832 290a 2020   / np.sqrt(2).  
+00021160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021170: 2020 2320 6e6f 7720 706c 6f74 2074 6865    # now plot the
+00021180: 2061 7272 6f77 0a20 2020 2020 2020 2020   arrow.         
+00021190: 2020 2020 2020 2020 2020 2070 6c74 2e61             plt.a
+000211a0: 7272 6f77 2878 202b 2030 2e35 2c20 7920  rrow(x + 0.5, y 
+000211b0: 2b20 302e 352c 2064 782c 2064 792c 2061  + 0.5, dx, dy, a
+000211c0: 6c70 6861 3d30 2e37 352c 0a20 2020 2020  lpha=0.75,.     
 000211d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000211e0: 616c 7068 613d 302e 352c 2073 697a 653d  alpha=0.5, size=
-000211f0: 3235 2c20 6164 645f 726f 6f74 733d 4661  25, add_roots=Fa
-00021200: 6c73 6529 3a0a 2020 2020 2020 2020 6966  lse):.        if
-00021210: 206e 6f74 2073 656c 662e 6765 6e5f 6172   not self.gen_ar
-00021220: 6368 2e75 7365 5f74 736b 6974 3a0a 2020  ch.use_tskit:.  
-00021230: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00021240: 4578 6365 7074 696f 6e28 2822 4765 6e65  Exception(("Gene
-00021250: 2066 6c6f 7720 6361 6e6e 6f74 2062 6520   flow cannot be 
-00021260: 706c 6f74 7465 6420 666f 7220 6120 5370  plotted for a Sp
-00021270: 6563 6965 7320 220a 2020 2020 2020 2020  ecies ".        
-00021280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021290: 2020 2020 2022 7768 6f73 6520 7370 6174       "whose spat
-000212a0: 6961 6c20 7065 6469 6772 6565 2069 7320  ial pedigree is 
-000212b0: 6e6f 7420 6265 696e 6720 7472 6163 6b65  not being tracke
-000212c0: 6420 220a 2020 2020 2020 2020 2020 2020  d ".            
-000212d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000212e0: 2022 6279 2074 736b 6974 2e22 2929 0a20   "by tskit.")). 
-000212f0: 2020 2020 2020 2061 7373 6572 7420 7374         assert st
-00021300: 796c 6520 696e 205b 276c 696e 6561 6765  yle in ['lineage
-00021310: 272c 2027 7665 6374 6f72 275d 2c20 2822  ', 'vector'], ("
-00021320: 5468 6520 7374 796c 6520 6172 6775 6d65  The style argume
-00021330: 6e74 206d 7573 7420 6265 2022 0a20 2020  nt must be ".   
-00021340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021360: 2020 2020 2020 2020 2020 2020 2022 6769               "gi
-00021370: 7665 6e20 6569 7468 6572 2027 6c69 6e65  ven either 'line
-00021380: 6167 6527 206f 7220 220a 2020 2020 2020  age' or ".      
-00021390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000213a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000213b0: 2020 2020 2020 2020 2020 2227 7665 6374            "'vect
-000213c0: 6f72 2720 6173 2061 2076 616c 7565 2e22  or' as a value."
-000213d0: 290a 2020 2020 2020 2020 6966 206e 6f64  ).        if nod
-000213e0: 6573 2069 7320 4e6f 6e65 3a0a 2020 2020  es is None:.    
-000213f0: 2020 2020 2020 2020 2320 6765 7420 6120          # get a 
-00021400: 7261 6e64 6f6d 2073 656c 6563 7469 6f6e  random selection
-00021410: 206f 6620 6e20 696e 6469 7669 6475 616c   of n individual
-00021420: 732c 2069 6620 696e 6469 7669 6473 2720  s, if individs' 
-00021430: 7661 6c75 6520 6973 2069 6e74 0a20 2020  value is int.   
-00021440: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-00021450: 7374 616e 6365 2869 6e64 6976 6964 732c  stance(individs,
-00021460: 2069 6e74 293a 0a20 2020 2020 2020 2020   int):.         
-00021470: 2020 2020 2020 2069 6e64 6976 6964 7320         individs 
-00021480: 3d20 6e70 2e72 616e 646f 6d2e 6368 6f69  = np.random.choi
-00021490: 6365 285b 2a73 656c 665d 2c20 696e 6469  ce([*self], indi
-000214a0: 7669 6473 2c20 7265 706c 6163 653d 4661  vids, replace=Fa
-000214b0: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-000214c0: 2023 736f 7274 2061 6e64 2073 696d 706c   #sort and simpl
-000214d0: 6966 7920 7468 6520 5461 626c 6543 6f6c  ify the TableCol
-000214e0: 6c65 6374 696f 6e2c 2069 6620 6e65 6564  lection, if need
-000214f0: 6564 200a 2020 2020 2020 2020 2020 2020  ed .            
-00021500: 6966 206e 6f74 2073 656c 662e 5f74 635f  if not self._tc_
-00021510: 736f 7274 6564 5f61 6e64 5f73 696d 706c  sorted_and_simpl
-00021520: 6966 6965 643a 0a20 2020 2020 2020 2020  ified:.         
-00021530: 2020 2020 2020 2073 656c 662e 5f73 6f72         self._sor
-00021540: 745f 616e 645f 7369 6d70 6c69 6679 5f74  t_and_simplify_t
-00021550: 6162 6c65 5f63 6f6c 6c65 6374 696f 6e28  able_collection(
-00021560: 290a 2020 2020 2020 2020 2020 2020 6e6f  ).            no
-00021570: 6465 7320 3d20 7365 6c66 2e5f 6765 745f  des = self._get_
-00021580: 6e6f 6465 7328 696e 6469 7669 6473 3d69  nodes(individs=i
-00021590: 6e64 6976 6964 7329 0a0a 2020 2020 2020  ndivids)..      
-000215a0: 2020 2320 736f 7274 2061 6e64 2073 696d    # sort and sim
-000215b0: 706c 6966 7920 7468 6520 5461 626c 6543  plify the TableC
-000215c0: 6f6c 6c65 6374 696f 6e20 6966 206e 6565  ollection if nee
-000215d0: 6465 640a 2020 2020 2020 2020 6966 206e  ded.        if n
-000215e0: 6f74 2073 656c 662e 5f74 635f 736f 7274  ot self._tc_sort
-000215f0: 6564 5f61 6e64 5f73 696d 706c 6966 6965  ed_and_simplifie
-00021600: 643a 0a20 2020 2020 2020 2020 2020 2073  d:.            s
-00021610: 656c 662e 5f73 6f72 745f 616e 645f 7369  elf._sort_and_si
-00021620: 6d70 6c69 6679 5f74 6162 6c65 5f63 6f6c  mplify_table_col
-00021630: 6c65 6374 696f 6e28 290a 2020 2020 2020  lection().      
-00021640: 2020 2320 6772 6162 2074 6865 2054 6162    # grab the Tab
-00021650: 6c65 436f 6c6c 6563 7469 6f6e 2061 6e64  leCollection and
-00021660: 2069 7473 2054 7265 6553 6571 7565 6e63   its TreeSequenc
-00021670: 650a 2020 2020 2020 2020 7463 203d 2073  e.        tc = s
-00021680: 656c 662e 5f74 630a 2020 2020 2020 2020  elf._tc.        
-00021690: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-000216a0: 2074 7320 3d20 7463 2e74 7265 655f 7365   ts = tc.tree_se
-000216b0: 7175 656e 6365 2829 0a20 2020 2020 2020  quence().       
-000216c0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-000216d0: 6e3a 0a20 2020 2020 2020 2020 2020 2072  n:.            r
-000216e0: 6169 7365 2045 7863 6570 7469 6f6e 2828  aise Exception((
-000216f0: 2254 6865 2073 7065 6369 6573 2720 5461  "The species' Ta
-00021700: 626c 6543 6f6c 6c65 6374 696f 6e20 6d75  bleCollection mu
-00021710: 7374 2062 6520 736f 7274 6564 2061 6e64  st be sorted and
-00021720: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00021730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021740: 2273 696d 706c 6966 6965 6420 6265 666f  "simplified befo
-00021750: 7265 2074 6869 7320 6d65 7468 6f64 2069  re this method i
-00021760: 7320 6361 6c6c 6564 2e22 2929 0a0a 2020  s called."))..  
-00021770: 2020 2020 2020 6e6f 6465 5f63 7572 725f        node_curr_
-00021780: 6c6f 6373 203d 205b 5b69 2e78 2c20 692e  locs = [[i.x, i.
-00021790: 795d 2066 6f72 206e 2069 6e20 6e6f 6465  y] for n in node
-000217a0: 7320 666f 7220 6920 696e 2073 656c 662e  s for i in self.
-000217b0: 7661 6c75 6573 280a 2020 2020 2020 2020  values(.        
-000217c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000217d0: 2920 6966 206e 2069 6e20 692e 5f6e 6f64  ) if n in i._nod
-000217e0: 6573 5f74 6162 5f69 6473 2e76 616c 7565  es_tab_ids.value
-000217f0: 7328 295d 0a0a 2020 2020 2020 2020 2320  s()]..        # 
-00021800: 6765 7420 7468 6520 7472 6565 2066 6f72  get the tree for
-00021810: 2074 6869 7320 6c6f 6375 730a 2020 2020   this locus.    
-00021820: 2020 2020 7472 6565 203d 2074 732e 6173      tree = ts.as
-00021830: 6c69 7374 2829 5b5f 6765 745f 7472 6565  list()[_get_tree
-00021840: 6e75 6d73 2874 732c 205b 6c6f 6375 735d  nums(ts, [locus]
-00021850: 295b 305d 5d0a 2020 2020 2020 2020 2320  )[0]].        # 
-00021860: 6765 7420 7468 6520 6c69 6e65 6167 655f  get the lineage_
-00021870: 6469 6374 2028 7769 7468 2062 6972 7468  dict (with birth
-00021880: 2074 696d 6573 2061 6e64 2062 6972 7468   times and birth
-00021890: 206c 6f63 6174 696f 6e73 290a 2020 2020   locations).    
-000218a0: 2020 2020 6c69 6e5f 6469 6374 203d 205f      lin_dict = _
-000218b0: 6765 745f 6c69 6e65 6167 655f 6469 6374  get_lineage_dict
-000218c0: 735f 6f6e 655f 7472 6565 2874 632c 2074  s_one_tree(tc, t
-000218d0: 7265 652c 206e 6f64 6573 2c20 7365 6c66  ree, nodes, self
-000218e0: 2e74 290a 2020 2020 2020 2020 6966 2063  .t).        if c
-000218f0: 6f6c 6f72 2069 7320 4e6f 6e65 3a0a 2020  olor is None:.  
-00021900: 2020 2020 2020 2020 2020 2320 6372 6561            # crea
-00021910: 7465 2073 7461 7274 2d63 6f6c 6f72 2076  te start-color v
-00021920: 616c 7565 7320 666f 7220 6e6f 6465 7327  alues for nodes'
-00021930: 2073 6570 6172 6174 6520 6c69 6e65 6167   separate lineag
-00021940: 6520 7472 6163 6b73 0a20 2020 2020 2020  e tracks.       
-00021950: 2020 2020 2063 6f6c 6f72 7320 3d20 5b6d       colors = [m
-00021960: 706c 2e63 6f6c 6f72 732e 746f 5f68 6578  pl.colors.to_hex
-00021970: 2870 6c74 2e63 6d2e 5365 7431 5f72 280a  (plt.cm.Set1_r(.
-00021980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000219a0: 2020 2020 2020 2020 6e29 2920 666f 7220          n)) for 
-000219b0: 6e20 696e 206e 702e 6c69 6e73 7061 6365  n in np.linspace
-000219c0: 2830 2c20 302e 3835 2c20 3829 5d0a 2020  (0, 0.85, 8)].  
-000219d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000219e0: 2020 2020 2020 2020 636f 6c6f 7273 203d          colors =
-000219f0: 205b 636f 6c6f 7220 666f 7220 5f20 696e   [color for _ in
-00021a00: 2072 616e 6765 2838 295d 0a20 2020 2020   range(8)].     
-00021a10: 2020 2023 2070 6c6f 7420 7468 6520 7370     # plot the sp
-00021a20: 6563 6965 732c 2065 6974 6865 7220 7769  ecies, either wi
-00021a30: 7468 206f 7220 7769 7468 6f75 7420 7068  th or without ph
-00021a40: 656e 6f74 7970 652d 7061 696e 7469 6e67  enotype-painting
-00021a50: 0a20 2020 2020 2020 2069 6620 7068 656e  .        if phen
-00021a60: 6f74 7970 6520 6973 204e 6f6e 653a 0a20  otype is None:. 
-00021a70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00021a80: 5f70 6c6f 7428 6c79 725f 6e75 6d3d 6c79  _plot(lyr_num=ly
-00021a90: 725f 6e75 6d2c 206c 616e 643d 6c61 6e64  r_num, land=land
-00021aa0: 2c20 7369 7a65 3d73 697a 6529 0a20 2020  , size=size).   
-00021ab0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00021ac0: 2020 2020 2020 2073 656c 662e 5f70 6c6f         self._plo
-00021ad0: 745f 7068 656e 6f74 7970 6528 7068 656e  t_phenotype(phen
-00021ae0: 6f74 7970 652c 206c 616e 643d 6c61 6e64  otype, land=land
-00021af0: 2c20 7369 7a65 3d73 697a 6529 0a20 2020  , size=size).   
-00021b00: 2020 2020 2061 7820 3d20 706c 742e 6763       ax = plt.gc
-00021b10: 6128 290a 2020 2020 2020 2020 2320 6578  a().        # ex
-00021b20: 7472 6163 7420 616e 6420 706c 6f74 2074  tract and plot t
-00021b30: 6865 2073 6572 6965 7320 6f66 2070 6f69  he series of poi
-00021b40: 6e74 7320 666f 7220 6561 6368 206e 6f64  nts for each nod
-00021b50: 650a 2020 2020 2020 2020 666f 7220 692c  e.        for i,
-00021b60: 206e 6f64 6520 696e 2065 6e75 6d65 7261   node in enumera
-00021b70: 7465 286e 6f64 6573 293a 0a20 2020 2020  te(nodes):.     
-00021b80: 2020 2020 2020 2073 7461 7274 5f63 6f6c         start_col
-00021b90: 203d 2063 6f6c 6f72 735b 6920 2520 6c65   = colors[i % le
-00021ba0: 6e28 636f 6c6f 7273 295d 0a20 2020 2020  n(colors)].     
-00021bb0: 2020 2020 2020 2069 6620 7374 796c 6520         if style 
-00021bc0: 3d3d 2027 6c69 6e65 6167 6527 3a0a 2020  == 'lineage':.  
-00021bd0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00021be0: 6373 203d 206e 702e 7673 7461 636b 285b  cs = np.vstack([
-00021bf0: 765b 315d 2066 6f72 2076 2069 6e20 6c69  v[1] for v in li
-00021c00: 6e5f 6469 6374 5b6e 6f64 655d 2e76 616c  n_dict[node].val
-00021c10: 7565 7328 295d 290a 2020 2020 2020 2020  ues()]).        
-00021c20: 2020 2020 2020 2020 6966 206a 6974 7465          if jitte
-00021c30: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00021c40: 2020 2020 2020 206c 6f63 7320 3d20 6c6f         locs = lo
-00021c50: 6373 202b 206e 702e 7261 6e64 6f6d 2e6e  cs + np.random.n
-00021c60: 6f72 6d61 6c28 302c 2030 2e30 312c 0a20  ormal(0, 0.01,. 
-00021c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021c90: 2020 2020 2020 2020 2020 2073 697a 653d             size=
-00021ca0: 6c6f 6373 2e73 697a 6529 2e72 6573 6861  locs.size).resha
-00021cb0: 7065 286c 6f63 732e 7368 6170 6529 0a20  pe(locs.shape). 
-00021cc0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00021cd0: 2063 7265 6174 6520 6c69 7374 206f 6620   create list of 
-00021ce0: 636f 6c6f 7273 2066 6f72 2070 6c6f 7474  colors for plott
-00021cf0: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
-00021d00: 2020 2020 2023 2075 7369 6e67 206c 696e       # using lin
-00021d10: 6561 726c 7920 696e 7465 7270 6f6c 6174  early interpolat
-00021d20: 6564 2063 6f6c 6f72 730a 2020 2020 2020  ed colors.      
-00021d30: 2020 2020 2020 2020 2020 2320 6966 2074            # if t
-00021d40: 6865 2063 6f6c 6f72 2061 7267 756d 656e  he color argumen
-00021d50: 7420 7761 7320 6e6f 7420 7072 6f76 6964  t was not provid
-00021d60: 6564 2c20 0a20 2020 2020 2020 2020 2020  ed, .           
-00021d70: 2020 2020 2023 206f 7220 656c 7365 206a       # or else j
-00021d80: 7573 7420 7573 696e 6720 7468 6520 736f  ust using the so
-00021d90: 6c69 6420 636f 6c6f 720a 2020 2020 2020  lid color.      
-00021da0: 2020 2020 2020 2020 2020 2320 7072 6f76            # prov
-00021db0: 6964 6564 2074 6f20 7468 6520 636f 6c6f  ided to the colo
-00021dc0: 7220 6172 6775 6d65 6e74 0a20 2020 2020  r argument.     
-00021dd0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-00021de0: 5f6e 756d 7320 3d20 6e70 2e69 6e74 3828  _nums = np.int8(
-00021df0: 6e70 2e6c 696e 7370 6163 6528 302c 2031  np.linspace(0, 1
-00021e00: 3030 2c20 6c6f 6373 2e73 6861 7065 5b30  00, locs.shape[0
-00021e10: 5d2d 3129 290a 2020 2020 2020 2020 2020  ]-1)).          
-00021e20: 2020 2020 2020 6966 2063 6f6c 6f72 2069        if color i
-00021e30: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00021e40: 2020 2020 2020 2020 2020 2020 706c 6f74              plot
-00021e50: 5f63 6f6c 6f72 7320 3d5b 7669 7a2e 5f63  _colors =[viz._c
-00021e60: 616c 635f 7265 7368 6164 6564 5f63 6f6c  alc_reshaded_col
-00021e70: 6f72 2873 7461 7274 5f63 6f6c 2c0a 2020  or(start_col,.  
-00021e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021eb0: 6e75 6d29 2066 6f72 206e 756d 2069 6e20  num) for num in 
-00021ec0: 636f 6c6f 725f 6e75 6d73 5d0a 2020 2020  color_nums].    
-00021ed0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00021ee0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00021ef0: 2020 2020 2020 706c 6f74 5f63 6f6c 6f72        plot_color
-00021f00: 7320 3d20 5b73 7461 7274 5f63 6f6c 2066  s = [start_col f
-00021f10: 6f72 206e 756d 2069 6e20 636f 6c6f 725f  or num in color_
-00021f20: 6e75 6d73 5d0a 2020 2020 2020 2020 2020  nums].          
-00021f30: 2020 2020 2020 2320 6372 6561 7465 2061        # create a
-00021f40: 206c 696e 6561 7220 696e 7465 7270 6f6c   linear interpol
-00021f50: 6174 696f 6e20 6f66 206c 696e 6577 6964  ation of linewid
-00021f60: 7468 730a 2020 2020 2020 2020 2020 2020  ths.            
-00021f70: 2020 2020 6c69 6e65 7769 6474 6873 203d      linewidths =
-00021f80: 206e 702e 6c69 6e73 7061 6365 2833 2c20   np.linspace(3, 
-00021f90: 302e 3835 2c20 6c6f 6373 2e73 6861 7065  0.85, locs.shape
-00021fa0: 5b30 5d2d 3129 0a20 2020 2020 2020 2020  [0]-1).         
-00021fb0: 2020 2020 2020 2066 6f72 206e 2c20 636f         for n, co
-00021fc0: 6c20 696e 2065 6e75 6d65 7261 7465 2870  l in enumerate(p
-00021fd0: 6c6f 745f 636f 6c6f 7273 293a 0a20 2020  lot_colors):.   
-00021fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021ff0: 2023 204e 4f54 4520 6e65 6564 2074 6f20   # NOTE need to 
-00022000: 7573 6520 6f6e 6c79 2074 6865 2066 6972  use only the fir
-00022010: 7374 2032 2076 616c 7565 7320 696e 2074  st 2 values in t
-00022020: 6865 206c 6f63 6174 696f 6e0a 2020 2020  he location.    
-00022030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022040: 2320 6461 7461 2062 6563 6175 7365 2073  # data because s
-00022050: 7562 7365 7175 656e 7420 7661 6c75 6573  ubsequent values
-00022060: 2061 7265 2075 7365 640a 2020 2020 2020   are used.      
-00022070: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00022080: 746f 2073 746f 7265 2069 6e64 6976 6964  to store individ
-00022090: 7561 6c73 2720 7068 656e 6f74 7970 6573  uals' phenotypes
-000220a0: 2061 6e64 2066 6974 6e65 7373 0a20 2020   and fitness.   
-000220b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000220c0: 2061 782e 706c 6f74 286c 6f63 735b 6e3a   ax.plot(locs[n:
-000220d0: 6e2b 322c 2030 5d2c 206c 6f63 735b 6e3a  n+2, 0], locs[n:
-000220e0: 6e2b 322c 2031 5d2c 206c 696e 6573 7479  n+2, 1], linesty
-000220f0: 6c65 3d27 736f 6c69 6427 2c0a 2020 2020  le='solid',.    
-00022100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022110: 2020 2020 2020 2020 6d61 726b 6572 3d27          marker='
-00022120: 6f27 2c20 6d61 726b 6572 7369 7a65 3d73  o', markersize=s
-00022130: 697a 652a 2a28 312f 3229 2c20 636f 6c6f  ize**(1/2), colo
-00022140: 723d 636f 6c2c 0a20 2020 2020 2020 2020  r=col,.         
-00022150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022160: 2020 206c 696e 6577 6964 7468 3d6c 696e     linewidth=lin
-00022170: 6577 6964 7468 735b 6e5d 2c20 616c 7068  ewidths[n], alph
-00022180: 613d 616c 7068 6129 0a20 2020 2020 2020  a=alpha).       
-00022190: 2020 2020 2065 6c69 6620 7374 796c 6520       elif style 
-000221a0: 3d3d 2027 7665 6374 6f72 273a 0a20 2020  == 'vector':.   
-000221b0: 2020 2020 2020 2020 2020 2020 2023 2067               # g
-000221c0: 6574 2074 6865 2073 7461 7274 2061 6e64  et the start and
-000221d0: 2065 6e64 206c 6f63 6174 696f 6e73 0a20   end locations. 
-000221e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000221f0: 204e 4f54 4520 6e65 6564 2074 6f20 7461   NOTE need to ta
-00022200: 6b65 206f 6e6c 7920 7468 6520 6669 7273  ke only the firs
-00022210: 7420 3220 7661 6c75 6573 2069 6e20 7468  t 2 values in th
-00022220: 6520 6c6f 6361 7469 6f6e 0a20 2020 2020  e location.     
-00022230: 2020 2020 2020 2020 2020 2023 2064 6174             # dat
-00022240: 6120 6265 6361 7573 6520 7375 6273 6571  a because subseq
-00022250: 7565 6e74 2076 616c 7565 7320 6172 6520  uent values are 
-00022260: 7573 6564 2074 6f20 7374 6f72 6520 696e  used to store in
-00022270: 6469 7669 6475 616c 7327 200a 2020 2020  dividuals' .    
-00022280: 2020 2020 2020 2020 2020 2020 2320 7068              # ph
-00022290: 656e 6f74 7970 6573 2061 6e64 2066 6974  enotypes and fit
-000222a0: 6e65 7373 0a20 2020 2020 2020 2020 2020  ness.           
-000222b0: 2020 2020 2062 6567 5f6c 6f63 203d 205b       beg_loc = [
-000222c0: 2a6c 696e 5f64 6963 745b 6e6f 6465 5d2e  *lin_dict[node].
-000222d0: 7661 6c75 6573 2829 5d5b 2d31 5d5b 315d  values()][-1][1]
-000222e0: 5b3a 325d 0a20 2020 2020 2020 2020 2020  [:2].           
-000222f0: 2020 2020 2065 6e64 5f6c 6f63 203d 205b       end_loc = [
-00022300: 2a6c 696e 5f64 6963 745b 6e6f 6465 5d2e  *lin_dict[node].
-00022310: 7661 6c75 6573 2829 5d5b 305d 5b31 5d5b  values()][0][1][
-00022320: 3a32 5d0a 2020 2020 2020 2020 2020 2020  :2].            
-00022330: 2020 2020 6478 2c20 6479 203d 205b 656e      dx, dy = [en
-00022340: 645f 6c6f 635b 695d 202d 2062 6567 5f6c  d_loc[i] - beg_l
-00022350: 6f63 5b69 5d20 666f 7220 6920 696e 2072  oc[i] for i in r
-00022360: 616e 6765 2832 295d 0a20 2020 2020 2020  ange(2)].       
-00022370: 2020 2020 2020 2020 2023 2070 6c6f 7420           # plot 
-00022380: 7468 6520 7665 6374 6f72 0a20 2020 2020  the vector.     
-00022390: 2020 2020 2020 2020 2020 2023 204e 4f54             # NOT
-000223a0: 453a 2053 484f 554c 4420 4920 4245 2046  E: SHOULD I BE F
-000223b0: 4954 5449 4e47 2041 2052 4547 5245 5353  ITTING A REGRESS
-000223c0: 494f 4e20 4c49 4e45 2054 4f20 5448 4520  ION LINE TO THE 
-000223d0: 5820 414e 4420 590a 2020 2020 2020 2020  X AND Y.        
-000223e0: 2020 2020 2020 2020 2320 4c4f 4341 5449          # LOCATI
-000223f0: 4f4e 532c 2054 4f20 4745 5420 5448 4520  ONS, TO GET THE 
-00022400: 2741 5645 5241 4745 2720 5645 4354 4f52  'AVERAGE' VECTOR
-00022410: 2c20 5241 5448 4552 2054 4841 4e20 4a55  , RATHER THAN JU
-00022420: 5354 0a20 2020 2020 2020 2020 2020 2020  ST.             
-00022430: 2020 2023 2050 4c4f 5454 494e 4720 5448     # PLOTTING TH
-00022440: 4520 5645 4354 4f52 2042 4554 5745 454e  E VECTOR BETWEEN
-00022450: 2054 4845 204f 4c44 4553 5420 414e 4420   THE OLDEST AND 
-00022460: 4355 5252 454e 5420 504f 5349 5449 4f4e  CURRENT POSITION
-00022470: 530a 2020 2020 2020 2020 2020 2020 2020  S.              
-00022480: 2020 2320 2857 4849 4348 2043 4f55 4c44    # (WHICH COULD
-00022490: 2045 4153 494c 5920 4d49 5352 4550 5245   EASILY MISREPRE
-000224a0: 5345 4e54 2054 4845 204f 5645 5241 4c4c  SENT THE OVERALL
-000224b0: 2054 5245 4e44 2042 4543 4155 5345 200a   TREND BECAUSE .
-000224c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000224d0: 2320 4f46 2043 4841 4e43 4520 4154 5950  # OF CHANCE ATYP
-000224e0: 4943 414c 204c 4f43 4154 494f 4e53 2046  ICAL LOCATIONS F
-000224f0: 4f52 2045 4954 4845 5220 4f46 2054 484f  OR EITHER OF THO
-00022500: 5345 2054 574f 2050 4f53 4954 494f 4e53  SE TWO POSITIONS
-00022510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022520: 2061 782e 6172 726f 7728 2a62 6567 5f6c   ax.arrow(*beg_l
-00022530: 6f63 2c20 6478 2c20 6479 2c20 636f 6c6f  oc, dx, dy, colo
-00022540: 723d 7374 6172 745f 636f 6c2c 0a20 2020  r=start_col,.   
-00022550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022560: 2020 2020 2020 7769 6474 683d 302e 3035        width=0.05
-00022570: 2c20 6865 6164 5f77 6964 7468 3d30 2e34  , head_width=0.4
-00022580: 2c20 6c65 6e67 7468 5f69 6e63 6c75 6465  , length_include
-00022590: 735f 6865 6164 3d54 7275 6529 0a20 2020  s_head=True).   
-000225a0: 2020 2020 2020 2020 2023 2070 6c6f 7420           # plot 
-000225b0: 7468 6520 6e6f 6465 7327 2063 7572 7265  the nodes' curre
-000225c0: 6e74 206c 6f63 6174 696f 6e73 2061 6e64  nt locations and
-000225d0: 2074 6865 6972 2062 6972 7468 206c 6f63   their birth loc
-000225e0: 6174 696f 6e73 2c0a 2020 2020 2020 2020  ations,.        
-000225f0: 2020 2020 2320 636f 6e6e 6563 7465 6420      # connected 
-00022600: 6279 2061 2074 6869 6e20 626c 6163 6b20  by a thin black 
-00022610: 6c69 6e65 0a20 2020 2020 2020 2020 2020  line.           
-00022620: 206e 6f64 655f 6375 7272 5f6c 6f63 203d   node_curr_loc =
-00022630: 206e 6f64 655f 6375 7272 5f6c 6f63 735b   node_curr_locs[
-00022640: 695d 0a20 2020 2020 2020 2020 2020 206e  i].            n
-00022650: 6f64 655f 6269 7274 685f 6c6f 6320 3d20  ode_birth_loc = 
-00022660: 5b2a 6c69 6e5f 6469 6374 5b6e 6f64 655d  [*lin_dict[node]
-00022670: 2e76 616c 7565 7328 295d 5b30 5d5b 315d  .values()][0][1]
-00022680: 0a20 2020 2020 2020 2020 2020 2070 6c74  .            plt
-00022690: 2e70 6c6f 7428 5b6e 6f64 655f 6269 7274  .plot([node_birt
-000226a0: 685f 6c6f 635b 305d 2c20 6e6f 6465 5f63  h_loc[0], node_c
-000226b0: 7572 725f 6c6f 635b 305d 5d2c 0a20 2020  urr_loc[0]],.   
-000226c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000226d0: 2020 5b6e 6f64 655f 6269 7274 685f 6c6f    [node_birth_lo
-000226e0: 635b 315d 2c20 6e6f 6465 5f63 7572 725f  c[1], node_curr_
-000226f0: 6c6f 635b 315d 5d2c 0a20 2020 2020 2020  loc[1]],.       
-00022700: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00022710: 6c6f 723d 7374 6172 745f 636f 6c2c 206c  lor=start_col, l
-00022720: 696e 6573 7479 6c65 3d27 3a27 2c20 616c  inestyle=':', al
-00022730: 7068 613d 616c 7068 612c 0a20 2020 2020  pha=alpha,.     
-00022740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022750: 6c69 6e65 7769 6474 683d 312e 3229 0a0a  linewidth=1.2)..
-00022760: 2020 2020 2020 2020 6966 2061 6464 5f72          if add_r
-00022770: 6f6f 7473 3a0a 2020 2020 2020 2020 2020  oots:.          
-00022780: 2020 7365 6c66 2e5f 706c 6f74 5f6c 696e    self._plot_lin
-00022790: 6561 6765 5f72 6f6f 7473 2874 632c 2074  eage_roots(tc, t
-000227a0: 7265 6529 0a0a 0a20 2020 2023 2070 6c6f  ree)...    # plo
-000227b0: 7420 7468 6520 6c69 6e65 6167 6520 666f  t the lineage fo
-000227c0: 7220 6120 6769 7665 6e20 6e6f 6465 2061  r a given node a
-000227d0: 6e64 206c 6f63 7573 0a20 2020 2064 6566  nd locus.    def
-000227e0: 205f 706c 6f74 5f6c 696e 6561 6765 5f72   _plot_lineage_r
-000227f0: 6f6f 7473 2873 656c 662c 2074 632c 2074  oots(self, tc, t
-00022800: 7265 652c 2061 6c70 6861 3d30 2e38 2c20  ree, alpha=0.8, 
-00022810: 7369 7a65 3d37 3529 3a0a 2020 2020 2020  size=75):.      
-00022820: 2020 6966 206e 6f74 2073 656c 662e 6765    if not self.ge
-00022830: 6e5f 6172 6368 2e75 7365 5f74 736b 6974  n_arch.use_tskit
-00022840: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00022850: 6973 6520 4578 6365 7074 696f 6e28 2822  ise Exception(("
-00022860: 4c69 6e65 6167 6520 726f 6f74 7320 6361  Lineage roots ca
-00022870: 6e6e 6f74 2062 6520 706c 6f74 7465 6420  nnot be plotted 
-00022880: 666f 7220 6120 5370 6563 6965 7320 220a  for a Species ".
-00022890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000228a0: 2020 2020 2020 2020 2020 2020 2022 7768               "wh
-000228b0: 6f73 6520 7370 6174 6961 6c20 7065 6469  ose spatial pedi
-000228c0: 6772 6565 2069 7320 6e6f 7420 6265 696e  gree is not bein
-000228d0: 6720 7472 6163 6b65 6420 220a 2020 2020  g tracked ".    
-000228e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000228f0: 2020 2020 2020 2020 2022 6279 2074 736b           "by tsk
-00022900: 6974 2e22 2929 0a0a 2020 2020 2020 2020  it."))..        
-00022910: 2320 6765 7420 7468 6520 6e6f 6465 730a  # get the nodes.
-00022920: 2020 2020 2020 2020 616c 6c5f 6e6f 6465          all_node
-00022930: 7320 3d20 7365 6c66 2e5f 6765 745f 6e6f  s = self._get_no
-00022940: 6465 7328 290a 0a20 2020 2020 2020 2023  des()..        #
-00022950: 2067 6574 2074 6865 206c 696e 6561 6765   get the lineage
-00022960: 2064 6963 7420 666f 7220 616c 6c20 6e6f   dict for all no
-00022970: 6465 730a 2020 2020 2020 2020 6c69 6e5f  des.        lin_
-00022980: 6469 6374 203d 205f 6765 745f 6c69 6e65  dict = _get_line
-00022990: 6167 655f 6469 6374 735f 6f6e 655f 7472  age_dicts_one_tr
-000229a0: 6565 2874 632c 2074 7265 652c 2061 6c6c  ee(tc, tree, all
-000229b0: 5f6e 6f64 6573 2c20 7365 6c66 2e74 290a  _nodes, self.t).
-000229c0: 0a20 2020 2020 2020 2023 2067 6574 2074  .        # get t
-000229d0: 6865 2072 6f6f 7473 2066 6f72 2061 6c6c  he roots for all
-000229e0: 2064 6973 7469 6e63 7420 6c69 6e65 6167   distinct lineag
-000229f0: 6573 2061 7420 7468 6973 206c 6f63 7573  es at this locus
-00022a00: 0a20 2020 2020 2020 2072 6f6f 745f 6e6f  .        root_no
-00022a10: 6465 7320 3d20 6e70 2e75 6e69 7175 6528  des = np.unique(
-00022a20: 5b5b 2a6c 696e 5f64 6963 745b 6e5d 2e6b  [[*lin_dict[n].k
-00022a30: 6579 7328 295d 5b2d 315d 2066 6f72 206e  eys()][-1] for n
-00022a40: 2069 6e20 616c 6c5f 6e6f 6465 735d 290a   in all_nodes]).
-00022a50: 0a20 2020 2020 2020 2023 2067 6574 2062  .        # get b
-00022a60: 6972 7468 206c 6f63 6174 696f 6e73 2066  irth locations f
-00022a70: 6f72 2065 6163 6820 726f 6f74 206e 6f64  or each root nod
-00022a80: 650a 2020 2020 2020 2020 726f 6f74 5f69  e.        root_i
-00022a90: 6e64 6976 6964 7320 3d20 5b74 632e 6e6f  ndivids = [tc.no
-00022aa0: 6465 735b 6e5d 2e69 6e64 6976 6964 7561  des[n].individua
-00022ab0: 6c20 666f 7220 6e20 696e 2072 6f6f 745f  l for n in root_
-00022ac0: 6e6f 6465 735d 0a20 2020 2020 2020 2072  nodes].        r
-00022ad0: 6f6f 745f 6c6f 6373 203d 205b 7463 2e69  oot_locs = [tc.i
-00022ae0: 6e64 6976 6964 7561 6c73 5b69 5d2e 6c6f  ndividuals[i].lo
-00022af0: 6361 7469 6f6e 2066 6f72 2069 2069 6e20  cation for i in 
-00022b00: 726f 6f74 5f69 6e64 6976 6964 735d 0a0a  root_individs]..
-00022b10: 2020 2020 2020 2020 2320 6578 7472 6163          # extrac
-00022b20: 7420 616e 6420 706c 6f74 2074 6865 2073  t and plot the s
-00022b30: 6572 6965 7320 6f66 2070 6f69 6e74 7320  eries of points 
-00022b40: 666f 7220 6561 6368 206e 6f64 650a 2020  for each node.  
-00022b50: 2020 2020 2020 666f 7220 782c 2079 2069        for x, y i
-00022b60: 6e20 726f 6f74 5f6c 6f63 733a 0a20 2020  n root_locs:.   
-00022b70: 2020 2020 2020 2020 2023 2070 6c6f 7420           # plot 
-00022b80: 7468 6520 726f 6f74 206e 6f64 6573 2720  the root nodes' 
-00022b90: 6269 7274 6820 6c6f 6361 7469 6f6e 730a  birth locations.
-00022ba0: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-00022bb0: 7363 6174 7465 7228 782c 2079 2c20 633d  scatter(x, y, c=
-00022bc0: 2777 6869 7465 272c 2073 3d73 697a 652c  'white', s=size,
-00022bd0: 2061 6c70 6861 3d61 6c70 6861 2c20 6d61   alpha=alpha, ma
-00022be0: 726b 6572 3d27 7327 290a 2020 2020 2020  rker='s').      
-00022bf0: 2020 706c 742e 7368 6f77 2829 0a0a 0a20    plt.show()... 
-00022c00: 2020 2023 206d 6574 686f 6420 666f 7220     # method for 
-00022c10: 706c 6f74 7469 6e67 2061 2073 7065 6369  plotting a speci
-00022c20: 6573 2720 706f 7075 6c61 7469 6f6e 2070  es' population p
-00022c30: 7972 616d 6964 0a20 2020 2064 6566 205f  yramid.    def _
-00022c40: 706c 6f74 5f64 656d 6f67 7261 7068 6963  plot_demographic
-00022c50: 5f70 7972 616d 6964 2873 656c 6629 3a0a  _pyramid(self):.
-00022c60: 2020 2020 2020 2020 236d 616b 6520 6469          #make di
-00022c70: 6374 206f 6620 6665 6d61 6c65 2061 6e64  ct of female and
-00022c80: 206d 616c 6520 636f 6c6f 7273 0a20 2020   male colors.   
-00022c90: 2020 2020 2063 6f6c 5f64 6963 7420 3d20       col_dict = 
-00022ca0: 7b2d 313a 2027 6379 616e 272c 2031 3a20  {-1: 'cyan', 1: 
-00022cb0: 2770 696e 6b27 7d0a 2020 2020 2020 2020  'pink'}.        
-00022cc0: 2363 7265 6174 6520 6120 6669 6775 7265  #create a figure
-00022cd0: 0a20 2020 2020 2020 2066 6967 203d 2070  .        fig = p
-00022ce0: 6c74 2e66 6967 7572 6528 290a 2020 2020  lt.figure().    
-00022cf0: 2020 2020 2376 6172 6961 626c 6573 2074      #variables t
-00022d00: 6f20 6772 6162 2074 6865 206d 6178 2063  o grab the max c
-00022d10: 6f75 6e74 0a20 2020 2020 2020 206d 6178  ount.        max
-00022d20: 5f63 6f75 6e74 203d 2030 0a20 2020 2020  _count = 0.     
-00022d30: 2020 2023 666f 7220 6561 6368 2073 6578     #for each sex
-00022d40: 0a20 2020 2020 2020 2066 6f72 2073 6578  .        for sex
-00022d50: 5f76 616c 2069 6e20 5b2a 636f 6c5f 6469  _val in [*col_di
-00022d60: 6374 5d3a 0a20 2020 2020 2020 2020 2020  ct]:.           
-00022d70: 2023 6765 7420 6120 636f 756e 7465 720a   #get a counter.
-00022d80: 2020 2020 2020 2020 2020 2020 636f 756e              coun
-00022d90: 7473 203d 2043 285b 696e 642e 6167 6520  ts = C([ind.age 
-00022da0: 666f 7220 696e 6420 696e 2073 656c 662e  for ind in self.
-00022db0: 7661 6c75 6573 280a 2020 2020 2020 2020  values(.        
-00022dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022de0: 2020 2020 2920 6966 2069 6e64 2e73 6578      ) if ind.sex
-00022df0: 203d 3d20 696e 7428 7365 785f 7661 6c20   == int(sex_val 
-00022e00: 3c20 3029 5d29 0a20 2020 2020 2020 2020  < 0)]).         
-00022e10: 2020 2023 6772 6162 2074 6865 2061 6765     #grab the age
-00022e20: 7320 6672 6f6d 2069 740a 2020 2020 2020  s from it.      
-00022e30: 2020 2020 2020 6167 6573 203d 205b 2a63        ages = [*c
-00022e40: 6f75 6e74 735d 0a20 2020 2020 2020 2020  ounts].         
-00022e50: 2020 2023 616e 6420 6772 6162 2074 6865     #and grab the
-00022e60: 2063 6f75 6e74 7320 6672 6f6d 2069 7420   counts from it 
-00022e70: 286d 756c 7469 706c 7969 6e67 2062 7920  (multiplying by 
-00022e80: 2d31 2066 6f72 2066 656d 616c 6573 2c0a  -1 for females,.
-00022e90: 2020 2020 2020 2020 2020 2020 2374 6f20              #to 
-00022ea0: 7365 7420 6f6e 6520 7365 7820 6f6e 2065  set one sex on e
-00022eb0: 6974 6865 7220 7369 6465 206f 6620 783d  ither side of x=
-00022ec0: 302c 2066 6f72 2074 6865 2070 7972 616d  0, for the pyram
-00022ed0: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
-00022ee0: 636f 756e 7473 203d 205b 7365 785f 7661  counts = [sex_va
-00022ef0: 6c2a 636f 756e 7420 666f 7220 636f 756e  l*count for coun
-00022f00: 7420 696e 2063 6f75 6e74 732e 7661 6c75  t in counts.valu
-00022f10: 6573 2829 5d0a 2020 2020 2020 2020 2020  es()].          
-00022f20: 2020 2375 7064 6174 6520 7468 6520 6d61    #update the ma
-00022f30: 785f 636f 756e 7420 7661 720a 2020 2020  x_count var.    
-00022f40: 2020 2020 2020 2020 6d61 785f 636f 756e          max_coun
-00022f50: 7420 3d20 6d61 7828 6d61 7828 636f 756e  t = max(max(coun
-00022f60: 7473 292c 206d 6178 5f63 6f75 6e74 290a  ts), max_count).
-00022f70: 2020 2020 2020 2020 2020 2020 2374 6865              #the
-00022f80: 6e20 6372 6561 7465 2074 6865 2068 6f72  n create the hor
-00022f90: 697a 6f6e 7461 6c20 6261 7270 6c6f 740a  izontal barplot.
-00022fa0: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-00022fb0: 6261 7268 2861 6765 732c 2063 6f75 6e74  barh(ages, count
-00022fc0: 732c 2063 6f6c 6f72 203d 2063 6f6c 5f64  s, color = col_d
-00022fd0: 6963 745b 7365 785f 7661 6c5d 290a 2020  ict[sex_val]).  
-00022fe0: 2020 2020 2020 2375 7365 206d 6178 5f63        #use max_c
-00022ff0: 6f75 6e74 2074 6f20 7365 7420 7468 6520  ount to set the 
-00023000: 782d 6c69 6d69 7473 2061 6e64 2079 2d6c  x-limits and y-l
-00023010: 696d 6974 730a 2020 2020 2020 2020 706c  imits.        pl
-00023020: 742e 786c 696d 2828 2d31 2a6d 6178 5f63  t.xlim((-1*max_c
-00023030: 6f75 6e74 2d32 2c20 6d61 785f 636f 756e  ount-2, max_coun
-00023040: 742b 3229 290a 2020 2020 2020 2020 2373  t+2)).        #s
-00023050: 6574 2074 6865 2061 7869 7320 6c61 6265  et the axis labe
-00023060: 6c73 0a20 2020 2020 2020 2070 6c74 2e78  ls.        plt.x
-00023070: 6c61 6265 6c28 2753 7065 6369 6573 2028  label('Species (
-00023080: 696e 6469 7669 6475 616c 7329 2729 0a20  individuals)'). 
-00023090: 2020 2020 2020 2070 6c74 2e79 6c61 6265         plt.ylabe
-000230a0: 6c28 2741 6765 2028 7469 6d65 7374 6570  l('Age (timestep
-000230b0: 7329 2729 0a20 2020 2020 2020 2023 7468  s)').        #th
-000230c0: 656e 2073 6574 2074 6865 2078 6c61 6265  en set the xlabe
-000230d0: 6c73 2074 6f20 706f 7369 7469 7665 206e  ls to positive n
-000230e0: 756d 6265 7273 206f 6e20 6569 7468 6572  umbers on either
-000230f0: 2073 6964 650a 2020 2020 2020 2020 6c6f   side.        lo
-00023100: 6373 2c20 6c61 6265 6c73 203d 2070 6c74  cs, labels = plt
-00023110: 2e78 7469 636b 7328 290a 2020 2020 2020  .xticks().      
-00023120: 2020 706c 742e 7874 6963 6b73 286c 6f63    plt.xticks(loc
-00023130: 732c 205b 7374 7228 696e 7428 6c6f 6329  s, [str(int(loc)
-00023140: 2920 666f 7220 6c6f 6320 696e 206e 702e  ) for loc in np.
-00023150: 6162 7328 6c6f 6373 295d 290a 2020 2020  abs(locs)]).    
-00023160: 2020 2020 2361 6464 2073 6578 2073 796d      #add sex sym
-00023170: 626f 6c73 2061 7320 7469 746c 650a 2020  bols as title.  
-00023180: 2020 2020 2020 706c 742e 7375 7074 6974        plt.suptit
-00023190: 6c65 2827 5c75 3236 3432 2573 5c75 3236  le('\u2642%s\u26
-000231a0: 3430 2720 2520 2727 2e6a 6f69 6e28 5b27  40' % ''.join(['
-000231b0: 2027 2066 6f72 205f 2069 6e20 7261 6e67   ' for _ in rang
-000231c0: 6528 3230 295d 292c 0a20 2020 2020 2020  e(20)]),.       
-000231d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000231e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000231f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023200: 2020 2020 2020 2020 2020 2020 2073 697a               siz
-00023210: 6520 3d20 3330 290a 2020 2020 2020 2020  e = 30).        
-00023220: 2373 686f 7720 6974 0a20 2020 2020 2020  #show it.       
-00023230: 2070 6c74 2e73 686f 7728 290a 0a20 2020   plt.show()..   
-00023240: 2064 6566 205f 706c 6f74 5f70 6f70 5f67   def _plot_pop_g
-00023250: 726f 7774 6828 7365 6c66 2c20 6578 7065  rowth(self, expe
-00023260: 6374 6564 3d54 7275 652c 2061 6374 7561  cted=True, actua
-00023270: 6c3d 5472 7565 2c20 6578 7065 6374 6564  l=True, expected
-00023280: 5f63 6f6c 6f72 3d27 7265 6427 2c0a 2020  _color='red',.  
-00023290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000232a0: 2020 2020 2020 6163 7475 616c 5f63 6f6c        actual_col
-000232b0: 6f72 3d27 626c 7565 2729 3a0a 2020 2020  or='blue'):.    
-000232c0: 2020 2020 5420 3d20 7261 6e67 6528 6c65      T = range(le
-000232d0: 6e28 7365 6c66 2e4e 7429 290a 2020 2020  n(self.Nt)).    
-000232e0: 2020 2020 7830 203d 2073 656c 662e 4e74      x0 = self.Nt
-000232f0: 5b30 5d20 2f20 7365 6c66 2e4b 2e73 756d  [0] / self.K.sum
-00023300: 2829 0a20 2020 2020 2020 2069 6620 6578  ().        if ex
-00023310: 7065 6374 6564 3a0a 2020 2020 2020 2020  pected:.        
-00023320: 2020 2020 706c 742e 706c 6f74 2854 2c20      plt.plot(T, 
-00023330: 5b5f 6361 6c63 5f6c 6f67 6973 7469 635f  [_calc_logistic_
-00023340: 736f 6c6e 2878 302c 2073 656c 662e 522c  soln(x0, self.R,
-00023350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023370: 2074 2920 2a20 7365 6c66 2e4b 2e73 756d   t) * self.K.sum
-00023380: 2829 2066 6f72 2074 2069 6e20 545d 2c0a  () for t in T],.
-00023390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000233a0: 2020 2020 2063 6f6c 6f72 3d65 7870 6563       color=expec
-000233b0: 7465 645f 636f 6c6f 7229 0a20 2020 2020  ted_color).     
-000233c0: 2020 2069 6620 6163 7475 616c 3a0a 2020     if actual:.  
-000233d0: 2020 2020 2020 2020 2020 706c 742e 706c            plt.pl
-000233e0: 6f74 2854 2c20 7365 6c66 2e4e 742c 2063  ot(T, self.Nt, c
-000233f0: 6f6c 6f72 3d61 6374 7561 6c5f 636f 6c6f  olor=actual_colo
-00023400: 7229 0a20 2020 2020 2020 2070 6c74 2e78  r).        plt.x
-00023410: 6c61 6265 6c28 2774 2729 0a20 2020 2020  label('t').     
-00023420: 2020 2070 6c74 2e79 6c61 6265 6c28 274e     plt.ylabel('N
-00023430: 2874 2927 290a 0a20 2020 2064 6566 205f  (t)')..    def _
-00023440: 706c 6f74 5f64 656d 6f67 7261 7068 6963  plot_demographic
-00023450: 5f63 6861 6e67 6573 2873 656c 6629 3a0a  _changes(self):.
-00023460: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00023470: 5f63 6861 6e67 6572 2069 7320 4e6f 6e65  _changer is None
-00023480: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00023490: 696e 7428 2822 5370 6563 6965 732e 5f70  int(("Species._p
-000234a0: 6c6f 745f 6465 6d6f 6772 6170 6869 635f  lot_demographic_
-000234b0: 6368 616e 6765 7320 6973 206e 6f74 2076  changes is not v
-000234c0: 616c 6964 2022 0a20 2020 2020 2020 2020  alid ".         
-000234d0: 2020 2020 2020 2022 666f 7220 7370 6563         "for spec
-000234e0: 6965 7320 7769 7468 206e 6f20 5f53 7065  ies with no _Spe
-000234f0: 6369 6573 4368 616e 6765 7220 6f62 6a65  ciesChanger obje
-00023500: 6374 2e5c 6e22 2929 0a20 2020 2020 2020  ct.\n")).       
-00023510: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00023520: 2020 2073 656c 662e 5f63 6861 6e67 6572     self._changer
-00023530: 2e5f 706c 6f74 5f64 656d 5f63 6861 6e67  ._plot_dem_chang
-00023540: 6573 2873 656c 6629 0a0a 0a20 2020 2064  es(self)...    d
-00023550: 6566 205f 706c 6f74 5f65 7861 6d70 6c65  ef _plot_example
-00023560: 5f72 6563 6f6d 6269 6e61 6e74 5f67 656e  _recombinant_gen
-00023570: 6f6d 6528 7365 6c66 293a 0a20 2020 2020  ome(self):.     
-00023580: 2020 2070 7269 6e74 2827 544f 444f 3a20     print('TODO: 
-00023590: 4649 5820 4d45 2127 290a 2020 2020 2020  FIX ME!').      
-000235a0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-000235b0: 2061 7373 6572 7420 7365 6c66 2e67 656e   assert self.gen
-000235c0: 5f61 7263 6820 6973 206e 6f74 204e 6f6e  _arch is not Non
-000235d0: 652c 2028 2254 6869 7320 7370 6563 6965  e, ("This specie
-000235e0: 7320 646f 6573 206e 6f74 2068 6176 6520  s does not have 
-000235f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00023600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023610: 2020 2020 2020 2020 2020 2020 2020 2267                "g
-00023620: 656e 6f6d 6573 2c20 736f 2069 7420 6361  enomes, so it ca
-00023630: 6e6e 6f74 2062 6520 7573 6564 2022 0a20  nnot be used ". 
-00023640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023660: 2020 2020 2020 2020 2020 2022 746f 2070             "to p
-00023670: 6c6f 7420 616e 2065 7861 6d70 6c65 2072  lot an example r
-00023680: 6563 6f6d 6269 6e61 6e74 2022 0a20 2020  ecombinant ".   
-00023690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000236a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000236b0: 2020 2020 2020 2020 2022 6765 6e6f 6d65           "genome
-000236c0: 2e22 290a 0a20 2020 2020 2020 2072 6563  .")..        rec
-000236d0: 6f6d 625f 7061 7468 7320 3d20 7365 6c66  omb_paths = self
-000236e0: 2e67 656e 5f61 7263 682e 5f72 6563 6f6d  .gen_arch._recom
-000236f0: 625f 7061 7468 732e 5f67 6574 5f70 6174  b_paths._get_pat
-00023700: 6873 2832 290a 2020 2020 2020 2020 6964  hs(2).        id
-00023710: 7873 203d 2028 302c 2032 290a 2020 2020  xs = (0, 2).    
-00023720: 2020 2020 6d6f 636b 5f73 7070 203d 207b      mock_spp = {
-00023730: 7d0a 2020 2020 2020 2020 666f 7220 6964  }.        for id
-00023740: 7820 696e 2069 6478 733a 0a20 2020 2020  x in idxs:.     
-00023750: 2020 2020 2020 206e 6577 5f67 656e 6f6d         new_genom
-00023760: 6520 3d20 6e70 2e68 7374 6163 6b28 5b28  e = np.hstack([(
-00023770: 6e70 2e6f 6e65 7328 2873 656c 662e 6765  np.ones((self.ge
-00023780: 6e5f 6172 6368 2e4c 2c0a 2020 2020 2020  n_arch.L,.      
-00023790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000237a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000237b0: 2020 2020 2020 2020 3129 2920 2a20 6e20          1)) * n 
-000237c0: 2920 2b20 6964 7820 666f 7220 6e20 696e  ) + idx for n in
-000237d0: 2028 312c 3229 5d29 0a20 2020 2020 2020   (1,2)]).       
-000237e0: 2020 2020 206d 6f63 6b5f 7370 705b 6964       mock_spp[id
-000237f0: 785d 203d 2049 6e64 6976 6964 7561 6c28  x] = Individual(
-00023800: 6964 783d 6964 782c 2078 3d30 2c20 793d  idx=idx, x=0, y=
-00023810: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-00023820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023830: 2020 2020 2020 2020 2020 6e65 775f 6765            new_ge
-00023840: 6e6f 6d65 3d6e 6577 5f67 656e 6f6d 6529  nome=new_genome)
-00023850: 0a0a 2020 2020 2020 2020 7265 636f 6d62  ..        recomb
-00023860: 5f67 656e 6f6d 6520 3d20 5f64 6f5f 6d61  _genome = _do_ma
-00023870: 7469 6e67 2873 7070 3d6d 6f63 6b5f 7370  ting(spp=mock_sp
-00023880: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
+000211e0: 2020 2020 2020 2020 2063 6f6c 6f72 3d63           color=c
+000211f0: 6f6c 6f72 2c20 6865 6164 5f77 6964 7468  olor, head_width
+00021200: 3d30 2e32 342c 2068 6561 645f 6c65 6e67  =0.24, head_leng
+00021210: 7468 3d30 2e33 3229 0a0a 2020 2020 2020  th=0.32)..      
+00021220: 2020 2020 2020 2020 2020 2320 6361 6c6c            # call
+00021230: 2074 6865 2069 6e74 6572 6e61 6c6c 7920   the internally 
+00021240: 6465 6669 6e65 6420 6675 6e63 7469 6f6e  defined function
+00021250: 2061 7320 6120 6e65 7374 6564 206c 6973   as a nested lis
+00021260: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00021270: 2020 2363 6f6d 7072 6568 656e 7369 6f6e    #comprehension
+00021280: 2066 6f72 2061 6c6c 2072 6173 7465 7220   for all raster 
+00021290: 6365 6c6c 732c 2077 6869 6368 2049 2062  cells, which I b
+000212a0: 656c 6965 7665 0a20 2020 2020 2020 2020  elieve.         
+000212b0: 2020 2020 2020 2023 7368 6f75 6c64 2064         #should d
+000212c0: 6f20 6974 7320 6265 7374 2074 6f20 7665  o its best to ve
+000212d0: 6374 6f72 697a 6520 7468 6520 7768 6f6c  ctorize the whol
+000212e0: 6520 6f70 6572 6174 696f 6e0a 2020 2020  e operation.    
+000212f0: 2020 2020 2020 2020 2020 2020 5b5b 706c              [[pl
+00021300: 6f74 5f6f 6e65 5f63 656c 6c28 6a2c 2069  ot_one_cell(j, i
+00021310: 2920 666f 7220 6920 696e 2072 616e 6765  ) for i in range
+00021320: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00021330: 2020 2020 2020 7375 7266 2e73 7572 662e        surf.surf.
+00021340: 7368 6170 655b 305d 295d 2066 6f72 206a  shape[0])] for j
+00021350: 2069 6e20 7261 6e67 6528 0a20 2020 2020   in range(.     
+00021360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021370: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00021380: 7572 662e 7375 7266 2e73 6861 7065 5b31  urf.surf.shape[1
+00021390: 5d29 5d0a 0a0a 2020 2020 2320 706c 6f74  ])]...    # plot
+000213a0: 2074 6865 206c 696e 6561 6765 2066 6f72   the lineage for
+000213b0: 2061 2067 6976 656e 206e 6f64 6520 616e   a given node an
+000213c0: 6420 6c6f 6375 730a 2020 2020 6465 6620  d locus.    def 
+000213d0: 5f70 6c6f 745f 6765 6e65 5f66 6c6f 7728  _plot_gene_flow(
+000213e0: 7365 6c66 2c20 6c6f 6375 732c 2073 7479  self, locus, sty
+000213f0: 6c65 2c20 6c61 6e64 2c20 6e6f 6465 733d  le, land, nodes=
+00021400: 4e6f 6e65 2c20 696e 6469 7669 6473 3d4e  None, individs=N
+00021410: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00021420: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+00021430: 723d 4e6f 6e65 2c20 7068 656e 6f74 7970  r=None, phenotyp
+00021440: 653d 4e6f 6e65 2c20 6c79 725f 6e75 6d3d  e=None, lyr_num=
+00021450: 302c 206a 6974 7465 723d 5472 7565 2c0a  0, jitter=True,.
+00021460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021470: 2020 2020 2020 2061 6c70 6861 3d30 2e35         alpha=0.5
+00021480: 2c20 7369 7a65 3d32 352c 2061 6464 5f72  , size=25, add_r
+00021490: 6f6f 7473 3d46 616c 7365 293a 0a20 2020  oots=False):.   
+000214a0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+000214b0: 2e67 656e 5f61 7263 682e 7573 655f 7473  .gen_arch.use_ts
+000214c0: 6b69 743a 0a20 2020 2020 2020 2020 2020  kit:.           
+000214d0: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
+000214e0: 2828 2247 656e 6520 666c 6f77 2063 616e  (("Gene flow can
+000214f0: 6e6f 7420 6265 2070 6c6f 7474 6564 2066  not be plotted f
+00021500: 6f72 2061 2053 7065 6369 6573 2022 0a20  or a Species ". 
+00021510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021520: 2020 2020 2020 2020 2020 2020 2277 686f              "who
+00021530: 7365 2073 7061 7469 616c 2070 6564 6967  se spatial pedig
+00021540: 7265 6520 6973 206e 6f74 2062 6569 6e67  ree is not being
+00021550: 2074 7261 636b 6564 2022 0a20 2020 2020   tracked ".     
+00021560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021570: 2020 2020 2020 2020 2262 7920 7473 6b69          "by tski
+00021580: 742e 2229 290a 2020 2020 2020 2020 6173  t.")).        as
+00021590: 7365 7274 2073 7479 6c65 2069 6e20 5b27  sert style in ['
+000215a0: 6c69 6e65 6167 6527 2c20 2776 6563 746f  lineage', 'vecto
+000215b0: 7227 5d2c 2028 2254 6865 2073 7479 6c65  r'], ("The style
+000215c0: 2061 7267 756d 656e 7420 6d75 7374 2062   argument must b
+000215d0: 6520 220a 2020 2020 2020 2020 2020 2020  e ".            
+000215e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000215f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021600: 2020 2020 2267 6976 656e 2065 6974 6865      "given eithe
+00021610: 7220 276c 696e 6561 6765 2720 6f72 2022  r 'lineage' or "
+00021620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021650: 2022 2776 6563 746f 7227 2061 7320 6120   "'vector' as a 
+00021660: 7661 6c75 652e 2229 0a20 2020 2020 2020  value.").       
+00021670: 2069 6620 6e6f 6465 7320 6973 204e 6f6e   if nodes is Non
+00021680: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
+00021690: 2067 6574 2061 2072 616e 646f 6d20 7365   get a random se
+000216a0: 6c65 6374 696f 6e20 6f66 206e 2069 6e64  lection of n ind
+000216b0: 6976 6964 7561 6c73 2c20 6966 2069 6e64  ividuals, if ind
+000216c0: 6976 6964 7327 2076 616c 7565 2069 7320  ivids' value is 
+000216d0: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+000216e0: 6966 2069 7369 6e73 7461 6e63 6528 696e  if isinstance(in
+000216f0: 6469 7669 6473 2c20 696e 7429 3a0a 2020  divids, int):.  
+00021700: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00021710: 6469 7669 6473 203d 206e 702e 7261 6e64  divids = np.rand
+00021720: 6f6d 2e63 686f 6963 6528 5b2a 7365 6c66  om.choice([*self
+00021730: 5d2c 2069 6e64 6976 6964 732c 2072 6570  ], individs, rep
+00021740: 6c61 6365 3d46 616c 7365 290a 2020 2020  lace=False).    
+00021750: 2020 2020 2020 2020 2373 6f72 7420 616e          #sort an
+00021760: 6420 7369 6d70 6c69 6679 2074 6865 2054  d simplify the T
+00021770: 6162 6c65 436f 6c6c 6563 7469 6f6e 2c20  ableCollection, 
+00021780: 6966 206e 6565 6465 6420 0a20 2020 2020  if needed .     
+00021790: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+000217a0: 6c66 2e5f 7463 5f73 6f72 7465 645f 616e  lf._tc_sorted_an
+000217b0: 645f 7369 6d70 6c69 6669 6564 3a0a 2020  d_simplified:.  
+000217c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000217d0: 6c66 2e5f 736f 7274 5f61 6e64 5f73 696d  lf._sort_and_sim
+000217e0: 706c 6966 795f 7461 626c 655f 636f 6c6c  plify_table_coll
+000217f0: 6563 7469 6f6e 2829 0a20 2020 2020 2020  ection().       
+00021800: 2020 2020 206e 6f64 6573 203d 2073 656c       nodes = sel
+00021810: 662e 5f67 6574 5f6e 6f64 6573 2869 6e64  f._get_nodes(ind
+00021820: 6976 6964 733d 696e 6469 7669 6473 290a  ivids=individs).
+00021830: 0a20 2020 2020 2020 2023 2073 6f72 7420  .        # sort 
+00021840: 616e 6420 7369 6d70 6c69 6679 2074 6865  and simplify the
+00021850: 2054 6162 6c65 436f 6c6c 6563 7469 6f6e   TableCollection
+00021860: 2069 6620 6e65 6564 6564 0a20 2020 2020   if needed.     
+00021870: 2020 2069 6620 6e6f 7420 7365 6c66 2e5f     if not self._
+00021880: 7463 5f73 6f72 7465 645f 616e 645f 7369  tc_sorted_and_si
+00021890: 6d70 6c69 6669 6564 3a0a 2020 2020 2020  mplified:.      
+000218a0: 2020 2020 2020 7365 6c66 2e5f 736f 7274        self._sort
+000218b0: 5f61 6e64 5f73 696d 706c 6966 795f 7461  _and_simplify_ta
+000218c0: 626c 655f 636f 6c6c 6563 7469 6f6e 2829  ble_collection()
+000218d0: 0a20 2020 2020 2020 2023 2067 7261 6220  .        # grab 
+000218e0: 7468 6520 5461 626c 6543 6f6c 6c65 6374  the TableCollect
+000218f0: 696f 6e20 616e 6420 6974 7320 5472 6565  ion and its Tree
+00021900: 5365 7175 656e 6365 0a20 2020 2020 2020  Sequence.       
+00021910: 2074 6320 3d20 7365 6c66 2e5f 7463 0a20   tc = self._tc. 
+00021920: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00021930: 2020 2020 2020 2020 7473 203d 2074 632e          ts = tc.
+00021940: 7472 6565 5f73 6571 7565 6e63 6528 290a  tree_sequence().
+00021950: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00021960: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
+00021970: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
+00021980: 7074 696f 6e28 2822 5468 6520 7370 6563  ption(("The spec
+00021990: 6965 7327 2054 6162 6c65 436f 6c6c 6563  ies' TableCollec
+000219a0: 7469 6f6e 206d 7573 7420 6265 2073 6f72  tion must be sor
+000219b0: 7465 6420 616e 6420 220a 2020 2020 2020  ted and ".      
+000219c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000219d0: 2020 2020 2020 2022 7369 6d70 6c69 6669         "simplifi
+000219e0: 6564 2062 6566 6f72 6520 7468 6973 206d  ed before this m
+000219f0: 6574 686f 6420 6973 2063 616c 6c65 642e  ethod is called.
+00021a00: 2229 290a 0a20 2020 2020 2020 206e 6f64  "))..        nod
+00021a10: 655f 6375 7272 5f6c 6f63 7320 3d20 5b5b  e_curr_locs = [[
+00021a20: 692e 782c 2069 2e79 5d20 666f 7220 6e20  i.x, i.y] for n 
+00021a30: 696e 206e 6f64 6573 2066 6f72 2069 2069  in nodes for i i
+00021a40: 6e20 7365 6c66 2e76 616c 7565 7328 0a20  n self.values(. 
+00021a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021a60: 2020 2020 2020 2029 2069 6620 6e20 696e         ) if n in
+00021a70: 2069 2e5f 6e6f 6465 735f 7461 625f 6964   i._nodes_tab_id
+00021a80: 732e 7661 6c75 6573 2829 5d0a 0a20 2020  s.values()]..   
+00021a90: 2020 2020 2023 2067 6574 2074 6865 2074       # get the t
+00021aa0: 7265 6520 666f 7220 7468 6973 206c 6f63  ree for this loc
+00021ab0: 7573 0a20 2020 2020 2020 2074 7265 6520  us.        tree 
+00021ac0: 3d20 7473 2e61 736c 6973 7428 295b 5f67  = ts.aslist()[_g
+00021ad0: 6574 5f74 7265 656e 756d 7328 7473 2c20  et_treenums(ts, 
+00021ae0: 5b6c 6f63 7573 5d29 5b30 5d5d 0a20 2020  [locus])[0]].   
+00021af0: 2020 2020 2023 2067 6574 2074 6865 206c       # get the l
+00021b00: 696e 6561 6765 5f64 6963 7420 2877 6974  ineage_dict (wit
+00021b10: 6820 6269 7274 6820 7469 6d65 7320 616e  h birth times an
+00021b20: 6420 6269 7274 6820 6c6f 6361 7469 6f6e  d birth location
+00021b30: 7329 0a20 2020 2020 2020 206c 696e 5f64  s).        lin_d
+00021b40: 6963 7420 3d20 5f67 6574 5f6c 696e 6561  ict = _get_linea
+00021b50: 6765 5f64 6963 7473 5f6f 6e65 5f74 7265  ge_dicts_one_tre
+00021b60: 6528 7463 2c20 7472 6565 2c20 6e6f 6465  e(tc, tree, node
+00021b70: 732c 2073 656c 662e 7429 0a20 2020 2020  s, self.t).     
+00021b80: 2020 2069 6620 636f 6c6f 7220 6973 204e     if color is N
+00021b90: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00021ba0: 2023 2063 7265 6174 6520 7374 6172 742d   # create start-
+00021bb0: 636f 6c6f 7220 7661 6c75 6573 2066 6f72  color values for
+00021bc0: 206e 6f64 6573 2720 7365 7061 7261 7465   nodes' separate
+00021bd0: 206c 696e 6561 6765 2074 7261 636b 730a   lineage tracks.
+00021be0: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+00021bf0: 7273 203d 205b 6d70 6c2e 636f 6c6f 7273  rs = [mpl.colors
+00021c00: 2e74 6f5f 6865 7828 706c 742e 636d 2e53  .to_hex(plt.cm.S
+00021c10: 6574 315f 7228 0a20 2020 2020 2020 2020  et1_r(.         
+00021c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021c30: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00021c40: 2929 2066 6f72 206e 2069 6e20 6e70 2e6c  )) for n in np.l
+00021c50: 696e 7370 6163 6528 302c 2030 2e38 352c  inspace(0, 0.85,
+00021c60: 2038 295d 0a20 2020 2020 2020 2065 6c73   8)].        els
+00021c70: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
+00021c80: 6f6c 6f72 7320 3d20 5b63 6f6c 6f72 2066  olors = [color f
+00021c90: 6f72 205f 2069 6e20 7261 6e67 6528 3829  or _ in range(8)
+00021ca0: 5d0a 2020 2020 2020 2020 2320 706c 6f74  ].        # plot
+00021cb0: 2074 6865 2073 7065 6369 6573 2c20 6569   the species, ei
+00021cc0: 7468 6572 2077 6974 6820 6f72 2077 6974  ther with or wit
+00021cd0: 686f 7574 2070 6865 6e6f 7479 7065 2d70  hout phenotype-p
+00021ce0: 6169 6e74 696e 670a 2020 2020 2020 2020  ainting.        
+00021cf0: 6966 2070 6865 6e6f 7479 7065 2069 7320  if phenotype is 
+00021d00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00021d10: 2020 7365 6c66 2e5f 706c 6f74 286c 7972    self._plot(lyr
+00021d20: 5f6e 756d 3d6c 7972 5f6e 756d 2c20 6c61  _num=lyr_num, la
+00021d30: 6e64 3d6c 616e 642c 2073 697a 653d 7369  nd=land, size=si
+00021d40: 7a65 290a 2020 2020 2020 2020 656c 7365  ze).        else
+00021d50: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00021d60: 6c66 2e5f 706c 6f74 5f70 6865 6e6f 7479  lf._plot_phenoty
+00021d70: 7065 2870 6865 6e6f 7479 7065 2c20 6c61  pe(phenotype, la
+00021d80: 6e64 3d6c 616e 642c 2073 697a 653d 7369  nd=land, size=si
+00021d90: 7a65 290a 2020 2020 2020 2020 6178 203d  ze).        ax =
+00021da0: 2070 6c74 2e67 6361 2829 0a20 2020 2020   plt.gca().     
+00021db0: 2020 2023 2065 7874 7261 6374 2061 6e64     # extract and
+00021dc0: 2070 6c6f 7420 7468 6520 7365 7269 6573   plot the series
+00021dd0: 206f 6620 706f 696e 7473 2066 6f72 2065   of points for e
+00021de0: 6163 6820 6e6f 6465 0a20 2020 2020 2020  ach node.       
+00021df0: 2066 6f72 2069 2c20 6e6f 6465 2069 6e20   for i, node in 
+00021e00: 656e 756d 6572 6174 6528 6e6f 6465 7329  enumerate(nodes)
+00021e10: 3a0a 2020 2020 2020 2020 2020 2020 7374  :.            st
+00021e20: 6172 745f 636f 6c20 3d20 636f 6c6f 7273  art_col = colors
+00021e30: 5b69 2025 206c 656e 2863 6f6c 6f72 7329  [i % len(colors)
+00021e40: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
+00021e50: 2073 7479 6c65 203d 3d20 276c 696e 6561   style == 'linea
+00021e60: 6765 273a 0a20 2020 2020 2020 2020 2020  ge':.           
+00021e70: 2020 2020 206c 6f63 7320 3d20 6e70 2e76       locs = np.v
+00021e80: 7374 6163 6b28 5b76 5b31 5d20 666f 7220  stack([v[1] for 
+00021e90: 7620 696e 206c 696e 5f64 6963 745b 6e6f  v in lin_dict[no
+00021ea0: 6465 5d2e 7661 6c75 6573 2829 5d29 0a20  de].values()]). 
+00021eb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00021ec0: 6620 6a69 7474 6572 3a0a 2020 2020 2020  f jitter:.      
+00021ed0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00021ee0: 6373 203d 206c 6f63 7320 2b20 6e70 2e72  cs = locs + np.r
+00021ef0: 616e 646f 6d2e 6e6f 726d 616c 2830 2c20  andom.normal(0, 
+00021f00: 302e 3031 2c0a 2020 2020 2020 2020 2020  0.01,.          
+00021f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021f30: 2020 7369 7a65 3d6c 6f63 732e 7369 7a65    size=locs.size
+00021f40: 292e 7265 7368 6170 6528 6c6f 6373 2e73  ).reshape(locs.s
+00021f50: 6861 7065 290a 2020 2020 2020 2020 2020  hape).          
+00021f60: 2020 2020 2020 2320 6372 6561 7465 206c        # create l
+00021f70: 6973 7420 6f66 2063 6f6c 6f72 7320 666f  ist of colors fo
+00021f80: 7220 706c 6f74 7469 6e67 2c0a 2020 2020  r plotting,.    
+00021f90: 2020 2020 2020 2020 2020 2020 2320 7573              # us
+00021fa0: 696e 6720 6c69 6e65 6172 6c79 2069 6e74  ing linearly int
+00021fb0: 6572 706f 6c61 7465 6420 636f 6c6f 7273  erpolated colors
+00021fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021fd0: 2023 2069 6620 7468 6520 636f 6c6f 7220   # if the color 
+00021fe0: 6172 6775 6d65 6e74 2077 6173 206e 6f74  argument was not
+00021ff0: 2070 726f 7669 6465 642c 200a 2020 2020   provided, .    
+00022000: 2020 2020 2020 2020 2020 2020 2320 6f72              # or
+00022010: 2065 6c73 6520 6a75 7374 2075 7369 6e67   else just using
+00022020: 2074 6865 2073 6f6c 6964 2063 6f6c 6f72   the solid color
+00022030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022040: 2023 2070 726f 7669 6465 6420 746f 2074   # provided to t
+00022050: 6865 2063 6f6c 6f72 2061 7267 756d 656e  he color argumen
+00022060: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00022070: 2020 636f 6c6f 725f 6e75 6d73 203d 206e    color_nums = n
+00022080: 702e 696e 7438 286e 702e 6c69 6e73 7061  p.int8(np.linspa
+00022090: 6365 2830 2c20 3130 302c 206c 6f63 732e  ce(0, 100, locs.
+000220a0: 7368 6170 655b 305d 2d31 2929 0a20 2020  shape[0]-1)).   
+000220b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000220c0: 636f 6c6f 7220 6973 204e 6f6e 653a 0a20  color is None:. 
+000220d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000220e0: 2020 2070 6c6f 745f 636f 6c6f 7273 203d     plot_colors =
+000220f0: 5b76 697a 2e5f 6361 6c63 5f72 6573 6861  [viz._calc_resha
+00022100: 6465 645f 636f 6c6f 7228 7374 6172 745f  ded_color(start_
+00022110: 636f 6c2c 0a20 2020 2020 2020 2020 2020  col,.           
+00022120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022140: 2020 2020 2020 206e 756d 2920 666f 7220         num) for 
+00022150: 6e75 6d20 696e 2063 6f6c 6f72 5f6e 756d  num in color_num
+00022160: 735d 0a20 2020 2020 2020 2020 2020 2020  s].             
+00022170: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00022180: 2020 2020 2020 2020 2020 2020 2070 6c6f               plo
+00022190: 745f 636f 6c6f 7273 203d 205b 7374 6172  t_colors = [star
+000221a0: 745f 636f 6c20 666f 7220 6e75 6d20 696e  t_col for num in
+000221b0: 2063 6f6c 6f72 5f6e 756d 735d 0a20 2020   color_nums].   
+000221c0: 2020 2020 2020 2020 2020 2020 2023 2063               # c
+000221d0: 7265 6174 6520 6120 6c69 6e65 6172 2069  reate a linear i
+000221e0: 6e74 6572 706f 6c61 7469 6f6e 206f 6620  nterpolation of 
+000221f0: 6c69 6e65 7769 6474 6873 0a20 2020 2020  linewidths.     
+00022200: 2020 2020 2020 2020 2020 206c 696e 6577             linew
+00022210: 6964 7468 7320 3d20 6e70 2e6c 696e 7370  idths = np.linsp
+00022220: 6163 6528 332c 2030 2e38 352c 206c 6f63  ace(3, 0.85, loc
+00022230: 732e 7368 6170 655b 305d 2d31 290a 2020  s.shape[0]-1).  
+00022240: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00022250: 7220 6e2c 2063 6f6c 2069 6e20 656e 756d  r n, col in enum
+00022260: 6572 6174 6528 706c 6f74 5f63 6f6c 6f72  erate(plot_color
+00022270: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00022280: 2020 2020 2020 2020 2320 4e4f 5445 206e          # NOTE n
+00022290: 6565 6420 746f 2075 7365 206f 6e6c 7920  eed to use only 
+000222a0: 7468 6520 6669 7273 7420 3220 7661 6c75  the first 2 valu
+000222b0: 6573 2069 6e20 7468 6520 6c6f 6361 7469  es in the locati
+000222c0: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+000222d0: 2020 2020 2020 2023 2064 6174 6120 6265         # data be
+000222e0: 6361 7573 6520 7375 6273 6571 7565 6e74  cause subsequent
+000222f0: 2076 616c 7565 7320 6172 6520 7573 6564   values are used
+00022300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022310: 2020 2020 2023 2074 6f20 7374 6f72 6520       # to store 
+00022320: 696e 6469 7669 6475 616c 7327 2070 6865  individuals' phe
+00022330: 6e6f 7479 7065 7320 616e 6420 6669 746e  notypes and fitn
+00022340: 6573 730a 2020 2020 2020 2020 2020 2020  ess.            
+00022350: 2020 2020 2020 2020 6178 2e70 6c6f 7428          ax.plot(
+00022360: 6c6f 6373 5b6e 3a6e 2b32 2c20 305d 2c20  locs[n:n+2, 0], 
+00022370: 6c6f 6373 5b6e 3a6e 2b32 2c20 315d 2c20  locs[n:n+2, 1], 
+00022380: 6c69 6e65 7374 796c 653d 2773 6f6c 6964  linestyle='solid
+00022390: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+000223a0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000223b0: 6172 6b65 723d 276f 272c 206d 6172 6b65  arker='o', marke
+000223c0: 7273 697a 653d 7369 7a65 2a2a 2831 2f32  rsize=size**(1/2
+000223d0: 292c 2063 6f6c 6f72 3d63 6f6c 2c0a 2020  ), color=col,.  
+000223e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000223f0: 2020 2020 2020 2020 2020 6c69 6e65 7769            linewi
+00022400: 6474 683d 6c69 6e65 7769 6474 6873 5b6e  dth=linewidths[n
+00022410: 5d2c 2061 6c70 6861 3d61 6c70 6861 290a  ], alpha=alpha).
+00022420: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00022430: 2073 7479 6c65 203d 3d20 2776 6563 746f   style == 'vecto
+00022440: 7227 3a0a 2020 2020 2020 2020 2020 2020  r':.            
+00022450: 2020 2020 2320 6765 7420 7468 6520 7374      # get the st
+00022460: 6172 7420 616e 6420 656e 6420 6c6f 6361  art and end loca
+00022470: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
+00022480: 2020 2020 2020 2320 4e4f 5445 206e 6565        # NOTE nee
+00022490: 6420 746f 2074 616b 6520 6f6e 6c79 2074  d to take only t
+000224a0: 6865 2066 6972 7374 2032 2076 616c 7565  he first 2 value
+000224b0: 7320 696e 2074 6865 206c 6f63 6174 696f  s in the locatio
+000224c0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+000224d0: 2020 2320 6461 7461 2062 6563 6175 7365    # data because
+000224e0: 2073 7562 7365 7175 656e 7420 7661 6c75   subsequent valu
+000224f0: 6573 2061 7265 2075 7365 6420 746f 2073  es are used to s
+00022500: 746f 7265 2069 6e64 6976 6964 7561 6c73  tore individuals
+00022510: 2720 0a20 2020 2020 2020 2020 2020 2020  ' .             
+00022520: 2020 2023 2070 6865 6e6f 7479 7065 7320     # phenotypes 
+00022530: 616e 6420 6669 746e 6573 730a 2020 2020  and fitness.    
+00022540: 2020 2020 2020 2020 2020 2020 6265 675f              beg_
+00022550: 6c6f 6320 3d20 5b2a 6c69 6e5f 6469 6374  loc = [*lin_dict
+00022560: 5b6e 6f64 655d 2e76 616c 7565 7328 295d  [node].values()]
+00022570: 5b2d 315d 5b31 5d5b 3a32 5d0a 2020 2020  [-1][1][:2].    
+00022580: 2020 2020 2020 2020 2020 2020 656e 645f              end_
+00022590: 6c6f 6320 3d20 5b2a 6c69 6e5f 6469 6374  loc = [*lin_dict
+000225a0: 5b6e 6f64 655d 2e76 616c 7565 7328 295d  [node].values()]
+000225b0: 5b30 5d5b 315d 5b3a 325d 0a20 2020 2020  [0][1][:2].     
+000225c0: 2020 2020 2020 2020 2020 2064 782c 2064             dx, d
+000225d0: 7920 3d20 5b65 6e64 5f6c 6f63 5b69 5d20  y = [end_loc[i] 
+000225e0: 2d20 6265 675f 6c6f 635b 695d 2066 6f72  - beg_loc[i] for
+000225f0: 2069 2069 6e20 7261 6e67 6528 3229 5d0a   i in range(2)].
+00022600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022610: 2320 706c 6f74 2074 6865 2076 6563 746f  # plot the vecto
+00022620: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+00022630: 2020 2320 4e4f 5445 3a20 5348 4f55 4c44    # NOTE: SHOULD
+00022640: 2049 2042 4520 4649 5454 494e 4720 4120   I BE FITTING A 
+00022650: 5245 4752 4553 5349 4f4e 204c 494e 4520  REGRESSION LINE 
+00022660: 544f 2054 4845 2058 2041 4e44 2059 0a20  TO THE X AND Y. 
+00022670: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00022680: 204c 4f43 4154 494f 4e53 2c20 544f 2047   LOCATIONS, TO G
+00022690: 4554 2054 4845 2027 4156 4552 4147 4527  ET THE 'AVERAGE'
+000226a0: 2056 4543 544f 522c 2052 4154 4845 5220   VECTOR, RATHER 
+000226b0: 5448 414e 204a 5553 540a 2020 2020 2020  THAN JUST.      
+000226c0: 2020 2020 2020 2020 2020 2320 504c 4f54            # PLOT
+000226d0: 5449 4e47 2054 4845 2056 4543 544f 5220  TING THE VECTOR 
+000226e0: 4245 5457 4545 4e20 5448 4520 4f4c 4445  BETWEEN THE OLDE
+000226f0: 5354 2041 4e44 2043 5552 5245 4e54 2050  ST AND CURRENT P
+00022700: 4f53 4954 494f 4e53 0a20 2020 2020 2020  OSITIONS.       
+00022710: 2020 2020 2020 2020 2023 2028 5748 4943           # (WHIC
+00022720: 4820 434f 554c 4420 4541 5349 4c59 204d  H COULD EASILY M
+00022730: 4953 5245 5052 4553 454e 5420 5448 4520  ISREPRESENT THE 
+00022740: 4f56 4552 414c 4c20 5452 454e 4420 4245  OVERALL TREND BE
+00022750: 4341 5553 4520 0a20 2020 2020 2020 2020  CAUSE .         
+00022760: 2020 2020 2020 2023 204f 4620 4348 414e         # OF CHAN
+00022770: 4345 2041 5459 5049 4341 4c20 4c4f 4341  CE ATYPICAL LOCA
+00022780: 5449 4f4e 5320 464f 5220 4549 5448 4552  TIONS FOR EITHER
+00022790: 204f 4620 5448 4f53 4520 5457 4f20 504f   OF THOSE TWO PO
+000227a0: 5349 5449 4f4e 530a 2020 2020 2020 2020  SITIONS.        
+000227b0: 2020 2020 2020 2020 6178 2e61 7272 6f77          ax.arrow
+000227c0: 282a 6265 675f 6c6f 632c 2064 782c 2064  (*beg_loc, dx, d
+000227d0: 792c 2063 6f6c 6f72 3d73 7461 7274 5f63  y, color=start_c
+000227e0: 6f6c 2c0a 2020 2020 2020 2020 2020 2020  ol,.            
+000227f0: 2020 2020 2020 2020 2020 2020 2077 6964               wid
+00022800: 7468 3d30 2e30 352c 2068 6561 645f 7769  th=0.05, head_wi
+00022810: 6474 683d 302e 342c 206c 656e 6774 685f  dth=0.4, length_
+00022820: 696e 636c 7564 6573 5f68 6561 643d 5472  includes_head=Tr
+00022830: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00022840: 2320 706c 6f74 2074 6865 206e 6f64 6573  # plot the nodes
+00022850: 2720 6375 7272 656e 7420 6c6f 6361 7469  ' current locati
+00022860: 6f6e 7320 616e 6420 7468 6569 7220 6269  ons and their bi
+00022870: 7274 6820 6c6f 6361 7469 6f6e 732c 0a20  rth locations,. 
+00022880: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
+00022890: 6e65 6374 6564 2062 7920 6120 7468 696e  nected by a thin
+000228a0: 2062 6c61 636b 206c 696e 650a 2020 2020   black line.    
+000228b0: 2020 2020 2020 2020 6e6f 6465 5f63 7572          node_cur
+000228c0: 725f 6c6f 6320 3d20 6e6f 6465 5f63 7572  r_loc = node_cur
+000228d0: 725f 6c6f 6373 5b69 5d0a 2020 2020 2020  r_locs[i].      
+000228e0: 2020 2020 2020 6e6f 6465 5f62 6972 7468        node_birth
+000228f0: 5f6c 6f63 203d 205b 2a6c 696e 5f64 6963  _loc = [*lin_dic
+00022900: 745b 6e6f 6465 5d2e 7661 6c75 6573 2829  t[node].values()
+00022910: 5d5b 305d 5b31 5d0a 2020 2020 2020 2020  ][0][1].        
+00022920: 2020 2020 706c 742e 706c 6f74 285b 6e6f      plt.plot([no
+00022930: 6465 5f62 6972 7468 5f6c 6f63 5b30 5d2c  de_birth_loc[0],
+00022940: 206e 6f64 655f 6375 7272 5f6c 6f63 5b30   node_curr_loc[0
+00022950: 5d5d 2c0a 2020 2020 2020 2020 2020 2020  ]],.            
+00022960: 2020 2020 2020 2020 205b 6e6f 6465 5f62           [node_b
+00022970: 6972 7468 5f6c 6f63 5b31 5d2c 206e 6f64  irth_loc[1], nod
+00022980: 655f 6375 7272 5f6c 6f63 5b31 5d5d 2c0a  e_curr_loc[1]],.
+00022990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000229a0: 2020 2020 2063 6f6c 6f72 3d73 7461 7274       color=start
+000229b0: 5f63 6f6c 2c20 6c69 6e65 7374 796c 653d  _col, linestyle=
+000229c0: 273a 272c 2061 6c70 6861 3d61 6c70 6861  ':', alpha=alpha
+000229d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000229e0: 2020 2020 2020 206c 696e 6577 6964 7468         linewidth
+000229f0: 3d31 2e32 290a 0a20 2020 2020 2020 2069  =1.2)..        i
+00022a00: 6620 6164 645f 726f 6f74 733a 0a20 2020  f add_roots:.   
+00022a10: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
+00022a20: 6c6f 745f 6c69 6e65 6167 655f 726f 6f74  lot_lineage_root
+00022a30: 7328 7463 2c20 7472 6565 290a 0a0a 2020  s(tc, tree)...  
+00022a40: 2020 2320 706c 6f74 2074 6865 206c 696e    # plot the lin
+00022a50: 6561 6765 2066 6f72 2061 2067 6976 656e  eage for a given
+00022a60: 206e 6f64 6520 616e 6420 6c6f 6375 730a   node and locus.
+00022a70: 2020 2020 6465 6620 5f70 6c6f 745f 6c69      def _plot_li
+00022a80: 6e65 6167 655f 726f 6f74 7328 7365 6c66  neage_roots(self
+00022a90: 2c20 7463 2c20 7472 6565 2c20 616c 7068  , tc, tree, alph
+00022aa0: 613d 302e 382c 2073 697a 653d 3735 293a  a=0.8, size=75):
+00022ab0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00022ac0: 7365 6c66 2e67 656e 5f61 7263 682e 7573  self.gen_arch.us
+00022ad0: 655f 7473 6b69 743a 0a20 2020 2020 2020  e_tskit:.       
+00022ae0: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
+00022af0: 7469 6f6e 2828 224c 696e 6561 6765 2072  tion(("Lineage r
+00022b00: 6f6f 7473 2063 616e 6e6f 7420 6265 2070  oots cannot be p
+00022b10: 6c6f 7474 6564 2066 6f72 2061 2053 7065  lotted for a Spe
+00022b20: 6369 6573 2022 0a20 2020 2020 2020 2020  cies ".         
+00022b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b40: 2020 2020 2277 686f 7365 2073 7061 7469      "whose spati
+00022b50: 616c 2070 6564 6967 7265 6520 6973 206e  al pedigree is n
+00022b60: 6f74 2062 6569 6e67 2074 7261 636b 6564  ot being tracked
+00022b70: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00022b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b90: 2262 7920 7473 6b69 742e 2229 290a 0a20  "by tskit.")).. 
+00022ba0: 2020 2020 2020 2023 2067 6574 2074 6865         # get the
+00022bb0: 206e 6f64 6573 0a20 2020 2020 2020 2061   nodes.        a
+00022bc0: 6c6c 5f6e 6f64 6573 203d 2073 656c 662e  ll_nodes = self.
+00022bd0: 5f67 6574 5f6e 6f64 6573 2829 0a0a 2020  _get_nodes()..  
+00022be0: 2020 2020 2020 2320 6765 7420 7468 6520        # get the 
+00022bf0: 6c69 6e65 6167 6520 6469 6374 2066 6f72  lineage dict for
+00022c00: 2061 6c6c 206e 6f64 6573 0a20 2020 2020   all nodes.     
+00022c10: 2020 206c 696e 5f64 6963 7420 3d20 5f67     lin_dict = _g
+00022c20: 6574 5f6c 696e 6561 6765 5f64 6963 7473  et_lineage_dicts
+00022c30: 5f6f 6e65 5f74 7265 6528 7463 2c20 7472  _one_tree(tc, tr
+00022c40: 6565 2c20 616c 6c5f 6e6f 6465 732c 2073  ee, all_nodes, s
+00022c50: 656c 662e 7429 0a0a 2020 2020 2020 2020  elf.t)..        
+00022c60: 2320 6765 7420 7468 6520 726f 6f74 7320  # get the roots 
+00022c70: 666f 7220 616c 6c20 6469 7374 696e 6374  for all distinct
+00022c80: 206c 696e 6561 6765 7320 6174 2074 6869   lineages at thi
+00022c90: 7320 6c6f 6375 730a 2020 2020 2020 2020  s locus.        
+00022ca0: 726f 6f74 5f6e 6f64 6573 203d 206e 702e  root_nodes = np.
+00022cb0: 756e 6971 7565 285b 5b2a 6c69 6e5f 6469  unique([[*lin_di
+00022cc0: 6374 5b6e 5d2e 6b65 7973 2829 5d5b 2d31  ct[n].keys()][-1
+00022cd0: 5d20 666f 7220 6e20 696e 2061 6c6c 5f6e  ] for n in all_n
+00022ce0: 6f64 6573 5d29 0a0a 2020 2020 2020 2020  odes])..        
+00022cf0: 2320 6765 7420 6269 7274 6820 6c6f 6361  # get birth loca
+00022d00: 7469 6f6e 7320 666f 7220 6561 6368 2072  tions for each r
+00022d10: 6f6f 7420 6e6f 6465 0a20 2020 2020 2020  oot node.       
+00022d20: 2072 6f6f 745f 696e 6469 7669 6473 203d   root_individs =
+00022d30: 205b 7463 2e6e 6f64 6573 5b6e 5d2e 696e   [tc.nodes[n].in
+00022d40: 6469 7669 6475 616c 2066 6f72 206e 2069  dividual for n i
+00022d50: 6e20 726f 6f74 5f6e 6f64 6573 5d0a 2020  n root_nodes].  
+00022d60: 2020 2020 2020 726f 6f74 5f6c 6f63 7320        root_locs 
+00022d70: 3d20 5b74 632e 696e 6469 7669 6475 616c  = [tc.individual
+00022d80: 735b 695d 2e6c 6f63 6174 696f 6e20 666f  s[i].location fo
+00022d90: 7220 6920 696e 2072 6f6f 745f 696e 6469  r i in root_indi
+00022da0: 7669 6473 5d0a 0a20 2020 2020 2020 2023  vids]..        #
+00022db0: 2065 7874 7261 6374 2061 6e64 2070 6c6f   extract and plo
+00022dc0: 7420 7468 6520 7365 7269 6573 206f 6620  t the series of 
+00022dd0: 706f 696e 7473 2066 6f72 2065 6163 6820  points for each 
+00022de0: 6e6f 6465 0a20 2020 2020 2020 2066 6f72  node.        for
+00022df0: 2078 2c20 7920 696e 2072 6f6f 745f 6c6f   x, y in root_lo
+00022e00: 6373 3a0a 2020 2020 2020 2020 2020 2020  cs:.            
+00022e10: 2320 706c 6f74 2074 6865 2072 6f6f 7420  # plot the root 
+00022e20: 6e6f 6465 7327 2062 6972 7468 206c 6f63  nodes' birth loc
+00022e30: 6174 696f 6e73 0a20 2020 2020 2020 2020  ations.         
+00022e40: 2020 2070 6c74 2e73 6361 7474 6572 2878     plt.scatter(x
+00022e50: 2c20 792c 2063 3d27 7768 6974 6527 2c20  , y, c='white', 
+00022e60: 733d 7369 7a65 2c20 616c 7068 613d 616c  s=size, alpha=al
+00022e70: 7068 612c 206d 6172 6b65 723d 2773 2729  pha, marker='s')
+00022e80: 0a20 2020 2020 2020 2070 6c74 2e73 686f  .        plt.sho
+00022e90: 7728 290a 0a0a 2020 2020 2320 6d65 7468  w()...    # meth
+00022ea0: 6f64 2066 6f72 2070 6c6f 7474 696e 6720  od for plotting 
+00022eb0: 6120 7370 6563 6965 7327 2070 6f70 756c  a species' popul
+00022ec0: 6174 696f 6e20 7079 7261 6d69 640a 2020  ation pyramid.  
+00022ed0: 2020 6465 6620 5f70 6c6f 745f 6465 6d6f    def _plot_demo
+00022ee0: 6772 6170 6869 635f 7079 7261 6d69 6428  graphic_pyramid(
+00022ef0: 7365 6c66 293a 0a20 2020 2020 2020 2023  self):.        #
+00022f00: 6d61 6b65 2064 6963 7420 6f66 2066 656d  make dict of fem
+00022f10: 616c 6520 616e 6420 6d61 6c65 2063 6f6c  ale and male col
+00022f20: 6f72 730a 2020 2020 2020 2020 636f 6c5f  ors.        col_
+00022f30: 6469 6374 203d 207b 2d31 3a20 2763 7961  dict = {-1: 'cya
+00022f40: 6e27 2c20 313a 2027 7069 6e6b 277d 0a20  n', 1: 'pink'}. 
+00022f50: 2020 2020 2020 2023 6372 6561 7465 2061         #create a
+00022f60: 2066 6967 7572 650a 2020 2020 2020 2020   figure.        
+00022f70: 6669 6720 3d20 706c 742e 6669 6775 7265  fig = plt.figure
+00022f80: 2829 0a20 2020 2020 2020 2023 7661 7269  ().        #vari
+00022f90: 6162 6c65 7320 746f 2067 7261 6220 7468  ables to grab th
+00022fa0: 6520 6d61 7820 636f 756e 740a 2020 2020  e max count.    
+00022fb0: 2020 2020 6d61 785f 636f 756e 7420 3d20      max_count = 
+00022fc0: 300a 2020 2020 2020 2020 2366 6f72 2065  0.        #for e
+00022fd0: 6163 6820 7365 780a 2020 2020 2020 2020  ach sex.        
+00022fe0: 666f 7220 7365 785f 7661 6c20 696e 205b  for sex_val in [
+00022ff0: 2a63 6f6c 5f64 6963 745d 3a0a 2020 2020  *col_dict]:.    
+00023000: 2020 2020 2020 2020 2367 6574 2061 2063          #get a c
+00023010: 6f75 6e74 6572 0a20 2020 2020 2020 2020  ounter.         
+00023020: 2020 2063 6f75 6e74 7320 3d20 4328 5b69     counts = C([i
+00023030: 6e64 2e61 6765 2066 6f72 2069 6e64 2069  nd.age for ind i
+00023040: 6e20 7365 6c66 2e76 616c 7565 7328 0a20  n self.values(. 
+00023050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023070: 2020 2020 2020 2020 2020 2029 2069 6620             ) if 
+00023080: 696e 642e 7365 7820 3d3d 2069 6e74 2873  ind.sex == int(s
+00023090: 6578 5f76 616c 203c 2030 295d 290a 2020  ex_val < 0)]).  
+000230a0: 2020 2020 2020 2020 2020 2367 7261 6220            #grab 
+000230b0: 7468 6520 6167 6573 2066 726f 6d20 6974  the ages from it
+000230c0: 0a20 2020 2020 2020 2020 2020 2061 6765  .            age
+000230d0: 7320 3d20 5b2a 636f 756e 7473 5d0a 2020  s = [*counts].  
+000230e0: 2020 2020 2020 2020 2020 2361 6e64 2067            #and g
+000230f0: 7261 6220 7468 6520 636f 756e 7473 2066  rab the counts f
+00023100: 726f 6d20 6974 2028 6d75 6c74 6970 6c79  rom it (multiply
+00023110: 696e 6720 6279 202d 3120 666f 7220 6665  ing by -1 for fe
+00023120: 6d61 6c65 732c 0a20 2020 2020 2020 2020  males,.         
+00023130: 2020 2023 746f 2073 6574 206f 6e65 2073     #to set one s
+00023140: 6578 206f 6e20 6569 7468 6572 2073 6964  ex on either sid
+00023150: 6520 6f66 2078 3d30 2c20 666f 7220 7468  e of x=0, for th
+00023160: 6520 7079 7261 6d69 6429 0a20 2020 2020  e pyramid).     
+00023170: 2020 2020 2020 2063 6f75 6e74 7320 3d20         counts = 
+00023180: 5b73 6578 5f76 616c 2a63 6f75 6e74 2066  [sex_val*count f
+00023190: 6f72 2063 6f75 6e74 2069 6e20 636f 756e  or count in coun
+000231a0: 7473 2e76 616c 7565 7328 295d 0a20 2020  ts.values()].   
+000231b0: 2020 2020 2020 2020 2023 7570 6461 7465           #update
+000231c0: 2074 6865 206d 6178 5f63 6f75 6e74 2076   the max_count v
+000231d0: 6172 0a20 2020 2020 2020 2020 2020 206d  ar.            m
+000231e0: 6178 5f63 6f75 6e74 203d 206d 6178 286d  ax_count = max(m
+000231f0: 6178 2863 6f75 6e74 7329 2c20 6d61 785f  ax(counts), max_
+00023200: 636f 756e 7429 0a20 2020 2020 2020 2020  count).         
+00023210: 2020 2023 7468 656e 2063 7265 6174 6520     #then create 
+00023220: 7468 6520 686f 7269 7a6f 6e74 616c 2062  the horizontal b
+00023230: 6172 706c 6f74 0a20 2020 2020 2020 2020  arplot.         
+00023240: 2020 2070 6c74 2e62 6172 6828 6167 6573     plt.barh(ages
+00023250: 2c20 636f 756e 7473 2c20 636f 6c6f 7220  , counts, color 
+00023260: 3d20 636f 6c5f 6469 6374 5b73 6578 5f76  = col_dict[sex_v
+00023270: 616c 5d29 0a20 2020 2020 2020 2023 7573  al]).        #us
+00023280: 6520 6d61 785f 636f 756e 7420 746f 2073  e max_count to s
+00023290: 6574 2074 6865 2078 2d6c 696d 6974 7320  et the x-limits 
+000232a0: 616e 6420 792d 6c69 6d69 7473 0a20 2020  and y-limits.   
+000232b0: 2020 2020 2070 6c74 2e78 6c69 6d28 282d       plt.xlim((-
+000232c0: 312a 6d61 785f 636f 756e 742d 322c 206d  1*max_count-2, m
+000232d0: 6178 5f63 6f75 6e74 2b32 2929 0a20 2020  ax_count+2)).   
+000232e0: 2020 2020 2023 7365 7420 7468 6520 6178       #set the ax
+000232f0: 6973 206c 6162 656c 730a 2020 2020 2020  is labels.      
+00023300: 2020 706c 742e 786c 6162 656c 2827 5370    plt.xlabel('Sp
+00023310: 6563 6965 7320 2869 6e64 6976 6964 7561  ecies (individua
+00023320: 6c73 2927 290a 2020 2020 2020 2020 706c  ls)').        pl
+00023330: 742e 796c 6162 656c 2827 4167 6520 2874  t.ylabel('Age (t
+00023340: 696d 6573 7465 7073 2927 290a 2020 2020  imesteps)').    
+00023350: 2020 2020 2374 6865 6e20 7365 7420 7468      #then set th
+00023360: 6520 786c 6162 656c 7320 746f 2070 6f73  e xlabels to pos
+00023370: 6974 6976 6520 6e75 6d62 6572 7320 6f6e  itive numbers on
+00023380: 2065 6974 6865 7220 7369 6465 0a20 2020   either side.   
+00023390: 2020 2020 206c 6f63 732c 206c 6162 656c       locs, label
+000233a0: 7320 3d20 706c 742e 7874 6963 6b73 2829  s = plt.xticks()
+000233b0: 0a20 2020 2020 2020 2070 6c74 2e78 7469  .        plt.xti
+000233c0: 636b 7328 6c6f 6373 2c20 5b73 7472 2869  cks(locs, [str(i
+000233d0: 6e74 286c 6f63 2929 2066 6f72 206c 6f63  nt(loc)) for loc
+000233e0: 2069 6e20 6e70 2e61 6273 286c 6f63 7329   in np.abs(locs)
+000233f0: 5d29 0a20 2020 2020 2020 2023 6164 6420  ]).        #add 
+00023400: 7365 7820 7379 6d62 6f6c 7320 6173 2074  sex symbols as t
+00023410: 6974 6c65 0a20 2020 2020 2020 2070 6c74  itle.        plt
+00023420: 2e73 7570 7469 746c 6528 275c 7532 3634  .suptitle('\u264
+00023430: 3225 735c 7532 3634 3027 2025 2027 272e  2%s\u2640' % ''.
+00023440: 6a6f 696e 285b 2720 2720 666f 7220 5f20  join([' ' for _ 
+00023450: 696e 2072 616e 6765 2832 3029 5d29 2c0a  in range(20)]),.
+00023460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000234a0: 2020 2020 7369 7a65 203d 2033 3029 0a20      size = 30). 
+000234b0: 2020 2020 2020 2023 7368 6f77 2069 740a         #show it.
+000234c0: 2020 2020 2020 2020 706c 742e 7368 6f77          plt.show
+000234d0: 2829 0a0a 2020 2020 6465 6620 5f70 6c6f  ()..    def _plo
+000234e0: 745f 706f 705f 6772 6f77 7468 2873 656c  t_pop_growth(sel
+000234f0: 662c 2065 7870 6563 7465 643d 5472 7565  f, expected=True
+00023500: 2c20 6163 7475 616c 3d54 7275 652c 2065  , actual=True, e
+00023510: 7870 6563 7465 645f 636f 6c6f 723d 2772  xpected_color='r
+00023520: 6564 272c 0a20 2020 2020 2020 2020 2020  ed',.           
+00023530: 2020 2020 2020 2020 2020 2020 2061 6374               act
+00023540: 7561 6c5f 636f 6c6f 723d 2762 6c75 6527  ual_color='blue'
+00023550: 293a 0a20 2020 2020 2020 2054 203d 2072  ):.        T = r
+00023560: 616e 6765 286c 656e 2873 656c 662e 4e74  ange(len(self.Nt
+00023570: 2929 0a20 2020 2020 2020 2078 3020 3d20  )).        x0 = 
+00023580: 7365 6c66 2e4e 745b 305d 202f 2073 656c  self.Nt[0] / sel
+00023590: 662e 4b2e 7375 6d28 290a 2020 2020 2020  f.K.sum().      
+000235a0: 2020 6966 2065 7870 6563 7465 643a 0a20    if expected:. 
+000235b0: 2020 2020 2020 2020 2020 2070 6c74 2e70             plt.p
+000235c0: 6c6f 7428 542c 205b 5f63 616c 635f 6c6f  lot(T, [_calc_lo
+000235d0: 6769 7374 6963 5f73 6f6c 6e28 7830 2c20  gistic_soln(x0, 
+000235e0: 7365 6c66 2e52 2c0a 2020 2020 2020 2020  self.R,.        
+000235f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023600: 2020 2020 2020 2020 7429 202a 2073 656c          t) * sel
+00023610: 662e 4b2e 7375 6d28 2920 666f 7220 7420  f.K.sum() for t 
+00023620: 696e 2054 5d2c 0a20 2020 2020 2020 2020  in T],.         
+00023630: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+00023640: 723d 6578 7065 6374 6564 5f63 6f6c 6f72  r=expected_color
+00023650: 290a 2020 2020 2020 2020 6966 2061 6374  ).        if act
+00023660: 7561 6c3a 0a20 2020 2020 2020 2020 2020  ual:.           
+00023670: 2070 6c74 2e70 6c6f 7428 542c 2073 656c   plt.plot(T, sel
+00023680: 662e 4e74 2c20 636f 6c6f 723d 6163 7475  f.Nt, color=actu
+00023690: 616c 5f63 6f6c 6f72 290a 2020 2020 2020  al_color).      
+000236a0: 2020 706c 742e 786c 6162 656c 2827 7427    plt.xlabel('t'
+000236b0: 290a 2020 2020 2020 2020 706c 742e 796c  ).        plt.yl
+000236c0: 6162 656c 2827 4e28 7429 2729 0a0a 2020  abel('N(t)')..  
+000236d0: 2020 6465 6620 5f70 6c6f 745f 6465 6d6f    def _plot_demo
+000236e0: 6772 6170 6869 635f 6368 616e 6765 7328  graphic_changes(
+000236f0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+00023700: 6620 7365 6c66 2e5f 6368 616e 6765 7220  f self._changer 
+00023710: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00023720: 2020 2020 2070 7269 6e74 2828 2253 7065       print(("Spe
+00023730: 6369 6573 2e5f 706c 6f74 5f64 656d 6f67  cies._plot_demog
+00023740: 7261 7068 6963 5f63 6861 6e67 6573 2069  raphic_changes i
+00023750: 7320 6e6f 7420 7661 6c69 6420 220a 2020  s not valid ".  
+00023760: 2020 2020 2020 2020 2020 2020 2020 2266                "f
+00023770: 6f72 2073 7065 6369 6573 2077 6974 6820  or species with 
+00023780: 6e6f 205f 5370 6563 6965 7343 6861 6e67  no _SpeciesChang
+00023790: 6572 206f 626a 6563 742e 5c6e 2229 290a  er object.\n")).
+000237a0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000237b0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000237c0: 6368 616e 6765 722e 5f70 6c6f 745f 6465  changer._plot_de
+000237d0: 6d5f 6368 616e 6765 7328 7365 6c66 290a  m_changes(self).
+000237e0: 0a0a 2020 2020 6465 6620 5f70 6c6f 745f  ..    def _plot_
+000237f0: 6578 616d 706c 655f 7265 636f 6d62 696e  example_recombin
+00023800: 616e 745f 6765 6e6f 6d65 2873 656c 6629  ant_genome(self)
+00023810: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+00023820: 2754 4f44 4f3a 2046 4958 204d 4521 2729  'TODO: FIX ME!')
+00023830: 0a20 2020 2020 2020 2072 6574 7572 6e0a  .        return.
+00023840: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+00023850: 656c 662e 6765 6e5f 6172 6368 2069 7320  elf.gen_arch is 
+00023860: 6e6f 7420 4e6f 6e65 2c20 2822 5468 6973  not None, ("This
+00023870: 2073 7065 6369 6573 2064 6f65 7320 6e6f   species does no
+00023880: 7420 6861 7665 2022 0a20 2020 2020 2020  t have ".       
 00023890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000238a0: 2020 2020 2020 6d61 7469 6e67 5f70 6169        mating_pai
-000238b0: 7273 3d5b 6964 7873 5d2c 0a20 2020 2020  rs=[idxs],.     
-000238c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000238d0: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
-000238e0: 6f66 6673 7072 696e 673d 5b31 5d2c 0a20  offspring=[1],. 
+000238a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000238b0: 2020 2020 2022 6765 6e6f 6d65 732c 2073       "genomes, s
+000238c0: 6f20 6974 2063 616e 6e6f 7420 6265 2075  o it cannot be u
+000238d0: 7365 6420 220a 2020 2020 2020 2020 2020  sed ".          
+000238e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000238f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023910: 2020 7265 636f 6d62 5f70 6174 6873 3d72    recomb_paths=r
-00023920: 6563 6f6d 625f 7061 7468 7329 5b30 5d5b  ecomb_paths)[0][
-00023930: 305d 0a20 2020 2020 2020 2023 7265 636f  0].        #reco
-00023940: 6d62 5f67 656e 6f6d 6520 3d20 7265 636f  mb_genome = reco
-00023950: 6d62 5f67 656e 6f6d 652b 310a 2020 2020  mb_genome+1.    
-00023960: 2020 2020 2372 6563 6f6d 625f 6765 6e6f      #recomb_geno
-00023970: 6d65 5b3a 2c31 5d20 3d20 7265 636f 6d62  me[:,1] = recomb
-00023980: 5f67 656e 6f6d 655b 3a2c 315d 202a 2035  _genome[:,1] * 5
-00023990: 0a20 2020 2020 2020 2066 6967 203d 2070  .        fig = p
-000239a0: 6c74 2e66 6967 7572 6528 290a 2020 2020  lt.figure().    
-000239b0: 2020 2020 6178 203d 2066 6967 2e61 6464      ax = fig.add
-000239c0: 5f73 7562 706c 6f74 2831 3131 290a 2020  _subplot(111).  
-000239d0: 2020 2020 2020 6178 2e69 6d73 686f 7728        ax.imshow(
-000239e0: 6e70 2e72 6570 6561 7428 7265 636f 6d62  np.repeat(recomb
-000239f0: 5f67 656e 6f6d 652c 0a20 2020 2020 2020  _genome,.       
-00023a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023a10: 2020 2020 2069 6e74 2830 2e30 3520 2a20       int(0.05 * 
-00023a20: 7365 6c66 2e67 656e 5f61 7263 682e 4c29  self.gen_arch.L)
-00023a30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00023a40: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-00023a50: 6973 3d31 292c 0a20 2020 2020 2020 2020  is=1),.         
-00023a60: 2020 2020 2020 2020 2063 6d61 703d 2774           cmap='t
-00023a70: 6572 7261 696e 2729 0a20 2020 2020 2020  errain').       
-00023a80: 2061 782e 7365 745f 7469 746c 6528 2267   ax.set_title("g
-00023a90: 616d 6574 6520 3020 2020 2020 6761 6d65  amete 0     game
-00023aa0: 7465 3122 290a 2020 2020 2020 2020 6178  te1").        ax
-00023ab0: 2e73 6574 5f78 7469 636b 7328 5b5d 290a  .set_xticks([]).
-00023ac0: 2020 2020 2020 2020 6178 2e73 6574 5f79          ax.set_y
-00023ad0: 6c61 6265 6c28 276c 6f63 7573 2729 0a20  label('locus'). 
-00023ae0: 2020 2020 2020 2070 6c74 2e73 686f 7728         plt.show(
-00023af0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00023b00: 2872 6563 6f6d 625f 7061 7468 732c 206d  (recomb_paths, m
-00023b10: 6f63 6b5f 7370 702c 2072 6563 6f6d 625f  ock_spp, recomb_
-00023b20: 6765 6e6f 6d65 290a 0a0a 2020 2020 6465  genome)...    de
-00023b30: 6620 5f70 6c6f 745f 7374 6174 2873 656c  f _plot_stat(sel
-00023b40: 662c 2073 7461 7429 3a0a 2020 2020 2020  f, stat):.      
-00023b50: 2020 6966 2073 656c 662e 5f73 7461 7473    if self._stats
-00023b60: 5f63 6f6c 6c65 6374 6f72 2069 7320 4e6f  _collector is No
-00023b70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00023b80: 7072 696e 7428 2822 5370 6563 6965 732e  print(("Species.
-00023b90: 5f70 6c6f 745f 7374 6174 2069 7320 6e6f  _plot_stat is no
-00023ba0: 7420 7661 6c69 6420 220a 2020 2020 2020  t valid ".      
-00023bb0: 2020 2020 2020 2020 2020 2266 6f72 2073            "for s
-00023bc0: 7065 6369 6573 2077 6974 6820 6e6f 205f  pecies with no _
-00023bd0: 5374 6174 7343 6f6c 6c65 6374 6f72 206f  StatsCollector o
-00023be0: 626a 6563 742e 5c6e 2229 290a 0a20 2020  bject.\n"))..   
-00023bf0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00023c00: 2020 2020 2020 2073 656c 662e 5f73 7461         self._sta
-00023c10: 7473 5f63 6f6c 6c65 6374 6f72 2e5f 706c  ts_collector._pl
-00023c20: 6f74 5f73 7461 7428 7374 6174 2c20 7370  ot_stat(stat, sp
-00023c30: 705f 6e61 6d65 203d 2073 656c 662e 6e61  p_name = self.na
-00023c40: 6d65 290a 0a0a 2020 2020 2020 2020 2323  me)...        ##
-00023c50: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
-00023c60: 2020 2020 2020 2023 7075 626c 6963 206d         #public m
-00023c70: 6574 686f 6473 230a 2020 2020 2020 2020  ethods#.        
-00023c80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023c90: 0a0a 2020 2020 6465 6620 5f77 7269 7465  ..    def _write
-00023ca0: 5f70 6963 6b6c 6528 7365 6c66 2c20 6669  _pickle(self, fi
-00023cb0: 6c65 6e61 6d65 293a 0a20 2020 2020 2020  lename):.       
-00023cc0: 2069 6d70 6f72 7420 6350 6963 6b6c 650a   import cPickle.
-00023cd0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-00023ce0: 6e28 6669 6c65 6e61 6d65 2c20 2777 6227  n(filename, 'wb'
-00023cf0: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-00023d00: 2020 2020 6350 6963 6b6c 652e 6475 6d70      cPickle.dump
-00023d10: 2873 656c 662c 2066 290a 0a0a 2323 2323  (self, f)...####
-00023d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023d30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023d40: 2323 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d  ##.# -----------
-00023d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00023d60: 2d2d 2d2d 2d2d 2d2d 230a 2320 4655 4e43  --------#.# FUNC
-00023d70: 5449 4f4e 5320 2d2d 2d2d 2d2d 2d2d 2d2d  TIONS ----------
-00023d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d23  ---------------#
-00023d90: 0a23 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .# -------------
-00023da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00023db0: 2d2d 2d2d 2d2d 230a 2323 2323 2323 2323  ------#.########
-00023dc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00023dd0: 2323 2323 2323 2323 2323 2323 2323 0a0a  ##############..
-00023de0: 2366 756e 6374 696f 6e20 746f 2062 6520  #function to be 
-00023df0: 6361 6c6c 6564 2077 6865 6e20 6120 5370  called when a Sp
-00023e00: 6563 6965 7320 6973 2069 6e69 7469 6174  ecies is initiat
-00023e10: 6564 2c0a 2377 6869 6368 2075 7365 7320  ed,.#which uses 
-00023e20: 7468 6520 7061 7261 6d73 2e73 7065 6369  the params.speci
-00023e30: 6573 5b3c 7370 705f 6e75 6d3e 5d2e 696e  es[<spp_num>].in
-00023e40: 6974 2e5b 274b 5f3c 3e27 5d20 7061 7261  it.['K_<>'] para
-00023e50: 6d65 7465 7273 200a 2374 6f20 6d61 6b65  meters .#to make
-00023e60: 2074 6865 2069 6e69 7469 616c 2063 6172   the initial car
-00023e70: 7279 696e 672d 6361 7061 6369 7479 2072  rying-capacity r
-00023e80: 6173 7465 722c 2061 6e64 2061 6c73 6f0a  aster, and also.
-00023e90: 2373 6574 7320 7468 6520 5370 6563 6965  #sets the Specie
-00023ea0: 7327 204b 5f6c 6179 6572 2061 6e64 204b  s' K_layer and K
-00023eb0: 5f66 6163 746f 7220 6174 7472 6962 7574  _factor attribut
-00023ec0: 6573 0a64 6566 205f 6d61 6b65 5f4b 2873  es.def _make_K(s
-00023ed0: 7070 2c20 6c61 6e64 2c20 4b5f 6c61 7965  pp, land, K_laye
-00023ee0: 722c 204b 5f66 6163 746f 7229 3a0a 2020  r, K_factor):.  
-00023ef0: 2020 236d 616b 6520 7375 7265 2077 6520    #make sure we 
-00023f00: 6669 6e64 206f 6e6c 7920 6120 7369 6e67  find only a sing
-00023f10: 6c65 206c 6179 6572 2077 6974 6820 7468  le layer with th
-00023f20: 6520 6e61 6d65 2073 7065 6369 6669 6564  e name specified
-00023f30: 2062 7920 4b5f 6c61 7965 720a 2020 2020   by K_layer.    
-00023f40: 4b5f 6c61 7965 7220 3d20 5b6c 7972 2066  K_layer = [lyr f
-00023f50: 6f72 206c 7972 2069 6e20 6c61 6e64 2e76  or lyr in land.v
-00023f60: 616c 7565 7328 2920 6966 206c 7972 2e6e  alues() if lyr.n
-00023f70: 616d 6520 3d3d 204b 5f6c 6179 6572 5d0a  ame == K_layer].
-00023f80: 2020 2020 6173 7365 7274 206c 656e 284b      assert len(K
-00023f90: 5f6c 6179 6572 2920 3d3d 2031 2c20 2822  _layer) == 1, ("
-00023fa0: 5468 6520 4b5f 6c61 7965 7220 7061 7261  The K_layer para
-00023fb0: 6d65 7465 7220 7368 6f75 6c64 2070 6f69  meter should poi
-00023fc0: 6e74 2074 6f22 0a20 2020 2020 2020 2022  nt to".        "
-00023fd0: 6120 7369 6e67 6c65 204c 6179 6572 2c20  a single Layer, 
-00023fe0: 6275 7420 696e 7374 6561 6420 2569 204c  but instead %i L
-00023ff0: 6179 6572 7320 7765 7265 2066 6f75 6e64  ayers were found
-00024000: 2e22 2920 2520 6c65 6e28 4b5f 6c61 7965  .") % len(K_laye
-00024010: 7229 0a20 2020 2023 6772 6162 2074 6865  r).    #grab the
-00024020: 2069 6465 6e74 6966 6965 6420 6c61 7965   identified laye
-00024030: 720a 2020 2020 4b5f 6c61 7965 7220 3d20  r.    K_layer = 
-00024040: 4b5f 6c61 7965 725b 305d 0a20 2020 2023  K_layer[0].    #
-00024050: 7365 7420 7468 6520 5370 6563 6965 7327  set the Species'
-00024060: 204b 5f6c 6179 6572 2061 6e64 204b 5f66   K_layer and K_f
-00024070: 6163 746f 7220 6174 7472 6962 7574 6573  actor attributes
-00024080: 0a20 2020 2073 7070 2e4b 5f6c 6179 6572  .    spp.K_layer
-00024090: 203d 204b 5f6c 6179 6572 2e69 6478 0a20   = K_layer.idx. 
-000240a0: 2020 2073 7070 2e4b 5f66 6163 746f 7220     spp.K_factor 
-000240b0: 3d20 4b5f 6661 6374 6f72 0a20 2020 2023  = K_factor.    #
-000240c0: 6164 6420 7468 6973 2053 7065 6369 6573  add this Species
-000240d0: 2074 6f20 7468 6973 204c 6179 6572 2773   to this Layer's
-000240e0: 202e 5f69 735f 4b20 6174 7472 6962 7574   ._is_K attribut
-000240f0: 650a 2020 2020 2328 7768 6963 6820 7769  e.    #(which wi
-00024100: 6c6c 2062 6520 7573 6564 2074 6f20 7570  ll be used to up
-00024110: 6461 7465 2053 7065 6369 6573 2e4b 2069  date Species.K i
-00024120: 6620 7468 6973 204c 6179 6572 2075 6e64  f this Layer und
-00024130: 6572 676f 6573 0a20 2020 2023 616e 7920  ergoes.    #any 
-00024140: 6b61 6e64 7363 6170 6520 6368 616e 6765  kandscape change
-00024150: 7329 0a20 2020 204b 5f6c 6179 6572 2e5f  s).    K_layer._
-00024160: 6973 5f4b 2e61 7070 656e 6428 7370 702e  is_K.append(spp.
-00024170: 6964 7829 0a20 2020 2023 6e6f 7720 6361  idx).    #now ca
-00024180: 6c63 756c 6174 6520 616e 6420 7365 7420  lculate and set 
-00024190: 7468 6520 4b20 7261 7374 6572 0a20 2020  the K raster.   
-000241a0: 2073 7070 2e5f 7365 745f 4b28 6c61 6e64   spp._set_K(land
-000241b0: 290a 0a0a 6465 6620 5f6d 616b 655f 7370  )...def _make_sp
-000241c0: 6563 6965 7328 6c61 6e64 2c20 6e61 6d65  ecies(land, name
-000241d0: 2c20 6964 782c 2073 7070 5f70 6172 616d  , idx, spp_param
-000241e0: 732c 2062 7572 6e3d 4661 6c73 652c 2076  s, burn=False, v
-000241f0: 6572 626f 7365 3d46 616c 7365 293a 0a20  erbose=False):. 
-00024200: 2020 2023 6765 7420 7370 7027 7320 696e     #get spp's in
-00024210: 7469 616c 697a 696e 6720 7061 7261 6d73  tializing params
-00024220: 0a20 2020 2069 6e69 745f 7061 7261 6d73  .    init_params
-00024230: 203d 2064 6565 7063 6f70 7928 7370 705f   = deepcopy(spp_
-00024240: 7061 7261 6d73 2e69 6e69 7429 0a0a 2020  params.init)..  
-00024250: 2020 2320 7072 696e 7420 7665 7262 6f73    # print verbos
-00024260: 6520 6f75 7470 7574 0a20 2020 2069 6620  e output.    if 
-00024270: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
-00024280: 2070 7269 6e74 2827 5c74 5c74 4d41 4b49   print('\t\tMAKI
-00024290: 4e47 2053 5045 4349 4553 2025 732e 2e2e  NG SPECIES %s...
-000242a0: 5c6e 2720 2520 6e61 6d65 2c20 666c 7573  \n' % name, flus
-000242b0: 683d 5472 7565 290a 0a20 2020 2023 6966  h=True)..    #if
-000242c0: 2074 6869 7320 7370 6563 6965 7320 7368   this species sh
-000242d0: 6f75 6c64 2068 6176 6520 6765 6e6f 6d65  ould have genome
-000242e0: 732c 2063 7265 6174 6520 7468 6520 6765  s, create the ge
-000242f0: 6e6f 6d69 6320 6172 6368 6974 6563 7475  nomic architectu
-00024300: 7265 0a20 2020 2069 6620 2767 656e 5f61  re.    if 'gen_a
-00024310: 7263 6827 2069 6e20 7370 705f 7061 7261  rch' in spp_para
-00024320: 6d73 2e6b 6579 7328 293a 0a20 2020 2020  ms.keys():.     
-00024330: 2020 2023 2070 7269 6e74 2076 6572 626f     # print verbo
-00024340: 7365 206f 7574 7075 740a 2020 2020 2020  se output.      
-00024350: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
-00024360: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00024370: 275c 745c 745c 746d 616b 696e 6720 6765  '\t\t\tmaking ge
-00024380: 6e6f 6d69 6320 6172 6368 6974 6563 7475  nomic architectu
-00024390: 7265 2e2e 2e5c 6e27 2c20 666c 7573 683d  re...\n', flush=
-000243a0: 5472 7565 290a 2020 2020 2020 2020 675f  True).        g_
-000243b0: 7061 7261 6d73 203d 2073 7070 5f70 6172  params = spp_par
-000243c0: 616d 732e 6765 6e5f 6172 6368 0a20 2020  ams.gen_arch.   
-000243d0: 2020 2020 2023 6d61 6b65 2067 656e 6f6d       #make genom
-000243e0: 6963 5f61 7263 6869 7465 6374 7572 650a  ic_architecture.
-000243f0: 2020 2020 2020 2020 6765 6e5f 6172 6368          gen_arch
-00024400: 203d 205f 6d61 6b65 5f67 656e 6f6d 6963   = _make_genomic
-00024410: 5f61 7263 6869 7465 6374 7572 6528 7370  _architecture(sp
-00024420: 705f 7061 7261 6d73 203d 2073 7070 5f70  p_params = spp_p
-00024430: 6172 616d 732c 0a20 2020 2020 2020 2020  arams,.         
-00024440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024470: 2020 2020 2020 206c 616e 6420 3d20 6c61         land = la
-00024480: 6e64 290a 2020 2020 656c 7365 3a0a 2020  nd).    else:.  
-00024490: 2020 2020 2020 6765 6e5f 6172 6368 203d        gen_arch =
-000244a0: 204e 6f6e 650a 0a20 2020 2023 2070 7269   None..    # pri
-000244b0: 6e74 2076 6572 626f 7365 206f 7574 7075  nt verbose outpu
-000244c0: 740a 2020 2020 6966 2076 6572 626f 7365  t.    if verbose
-000244d0: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
-000244e0: 275c 745c 745c 746d 616b 696e 6720 696e  '\t\t\tmaking in
-000244f0: 6469 7669 6475 616c 732e 2e2e 5c6e 272c  dividuals...\n',
-00024500: 2066 6c75 7368 3d54 7275 6529 0a20 2020   flush=True).   
-00024510: 2023 6d61 6b65 2069 6e64 6976 6964 730a   #make individs.
-00024520: 2020 2020 4e20 3d20 696e 6974 5f70 6172      N = init_par
-00024530: 616d 732e 706f 7028 274e 2729 0a20 2020  ams.pop('N').   
-00024540: 2023 6372 6561 7465 2061 6e20 6f72 6465   #create an orde
-00024550: 7265 6420 6469 6374 696f 6e61 7279 2074  red dictionary t
-00024560: 6f20 686f 6c64 2074 6865 2069 6e64 6976  o hold the indiv
-00024570: 6964 7561 6c73 2c20 616e 6420 6669 6c6c  iduals, and fill
-00024580: 2069 7420 7570 0a20 2020 2069 6e64 7320   it up.    inds 
-00024590: 3d20 4f44 2829 0a20 2020 2066 6f72 2069  = OD().    for i
-000245a0: 6e64 5f69 6478 2069 6e20 7261 6e67 6528  nd_idx in range(
-000245b0: 4e29 3a0a 2020 2020 2020 2020 2320 7573  N):.        # us
-000245c0: 6520 696e 6469 7669 6475 616c 2e63 7265  e individual.cre
-000245d0: 6174 655f 696e 6469 7669 6475 616c 2074  ate_individual t
-000245e0: 6f20 7369 6d75 6c61 7465 2069 6e64 6976  o simulate indiv
-000245f0: 6964 7561 6c73 0a20 2020 2020 2020 2023  iduals.        #
-00024600: 616e 6420 6164 6420 7468 656d 2074 6f20  and add them to 
-00024610: 7468 6520 7370 6563 6965 730a 2020 2020  the species.    
-00024620: 2020 2020 696e 6420 3d20 5f6d 616b 655f      ind = _make_
-00024630: 696e 6469 7669 6475 616c 2869 6478 3d69  individual(idx=i
-00024640: 6e64 5f69 6478 2c20 6f66 6673 7072 696e  nd_idx, offsprin
-00024650: 673d 4661 6c73 652c 0a20 2020 2020 2020  g=False,.       
-00024660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024670: 2020 2020 2020 2020 6469 6d3d 6c61 6e64          dim=land
-00024680: 2e64 696d 2c20 6765 6e6f 6d69 635f 6172  .dim, genomic_ar
-00024690: 6368 6974 6563 7475 7265 3d67 656e 5f61  chitecture=gen_a
-000246a0: 7263 682c 0a20 2020 2020 2020 2020 2020  rch,.           
-000246b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000246c0: 2020 2020 6275 726e 3d62 7572 6e29 0a20      burn=burn). 
-000246d0: 2020 2020 2020 2069 6e64 735b 696e 645f         inds[ind_
-000246e0: 6964 785d 203d 2069 6e64 0a0a 2020 2020  idx] = ind..    
-000246f0: 2363 7265 6174 6520 7468 6520 7370 6563  #create the spec
-00024700: 6965 7320 6672 6f6d 2074 686f 7365 2069  ies from those i
-00024710: 6e64 6976 6964 7561 6c73 0a20 2020 2073  ndividuals.    s
-00024720: 7070 203d 2053 7065 6369 6573 286e 616d  pp = Species(nam
-00024730: 6520 3d20 6e61 6d65 2c20 6964 7820 3d20  e = name, idx = 
-00024740: 6964 782c 2069 6e64 7320 3d20 696e 6473  idx, inds = inds
-00024750: 2c20 6c61 6e64 203d 206c 616e 642c 0a20  , land = land,. 
-00024760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024770: 2020 2020 7370 705f 7061 7261 6d73 203d      spp_params =
-00024780: 2073 7070 5f70 6172 616d 732c 2067 656e   spp_params, gen
-00024790: 6f6d 6963 5f61 7263 6869 7465 6374 7572  omic_architectur
-000247a0: 653d 6765 6e5f 6172 6368 290a 0a20 2020  e=gen_arch)..   
-000247b0: 2023 7573 6520 7468 6520 7265 6d61 696e   #use the remain
-000247c0: 696e 6720 696e 6974 5f70 6172 616d 7320  ing init_params 
-000247d0: 746f 2073 6574 2074 6865 2063 6172 7279  to set the carry
-000247e0: 696e 672d 6361 7061 6369 7479 2072 6173  ing-capacity ras
-000247f0: 7465 7220 284b 290a 2020 2020 5f6d 616b  ter (K).    _mak
-00024800: 655f 4b28 7370 702c 206c 616e 642c 202a  e_K(spp, land, *
-00024810: 2a7b 6b3a 7620 666f 7220 6b2c 7620 696e  *{k:v for k,v in
-00024820: 2069 6e69 745f 7061 7261 6d73 2e69 7465   init_params.ite
-00024830: 6d73 2829 2069 6620 6b20 213d 2027 6d73  ms() if k != 'ms
-00024840: 7072 696d 6527 7d29 0a20 2020 2023 7365  prime'}).    #se
-00024850: 7420 696e 6974 6961 6c20 656e 7669 726f  t initial enviro
-00024860: 6e6d 656e 7420 7661 6c75 6573 0a20 2020  nment values.   
-00024870: 2073 7070 2e5f 7365 745f 6528 6c61 6e64   spp._set_e(land
-00024880: 290a 2020 2020 2373 6574 2069 6e69 7469  ).    #set initi
-00024890: 616c 2063 6f6f 7264 7320 616e 6420 6365  al coords and ce
-000248a0: 6c6c 730a 2020 2020 7370 702e 5f73 6574  lls.    spp._set
-000248b0: 5f63 6f6f 7264 735f 616e 645f 6365 6c6c  _coords_and_cell
-000248c0: 7328 290a 2020 2020 2373 6574 2074 6865  s().    #set the
-000248d0: 206b 645f 7472 6565 0a20 2020 2073 7070   kd_tree.    spp
-000248e0: 2e5f 7365 745f 6b64 5f74 7265 6528 290a  ._set_kd_tree().
-000248f0: 0a20 2020 2023 7365 7420 7068 656e 6f74  .    #set phenot
-00024900: 7970 6573 2c20 6966 2074 6865 2073 7065  ypes, if the spe
-00024910: 6369 6573 2068 6173 2067 656e 6f6d 6573  cies has genomes
-00024920: 0a20 2020 2069 6620 7370 702e 6765 6e5f  .    if spp.gen_
-00024930: 6172 6368 2069 7320 6e6f 7420 4e6f 6e65  arch is not None
-00024940: 2061 6e64 206e 6f74 2062 7572 6e3a 0a20   and not burn:. 
-00024950: 2020 2020 2020 205b 696e 642e 5f73 6574         [ind._set
-00024960: 5f7a 2873 7070 2e67 656e 5f61 7263 6829  _z(spp.gen_arch)
-00024970: 2066 6f72 2069 6e64 2069 6e20 7370 702e   for ind in spp.
-00024980: 7661 6c75 6573 2829 5d0a 0a20 2020 2023  values()]..    #
-00024990: 6d61 6b65 2064 656e 7369 7479 5f67 7269  make density_gri
-000249a0: 640a 2020 2020 7370 702e 5f73 6574 5f64  d.    spp._set_d
-000249b0: 656e 735f 6772 6964 7328 6c61 6e64 290a  ens_grids(land).
-000249c0: 0a20 2020 2023 6d61 6b65 206d 6f76 656d  .    #make movem
-000249d0: 656e 7420 7375 7266 6163 652c 2069 6620  ent surface, if 
-000249e0: 6e65 6564 6564 0a20 2020 2069 6620 7370  needed.    if sp
-000249f0: 702e 5f6d 6f76 653a 0a20 2020 2020 2020  p._move:.       
-00024a00: 2069 6620 276d 6f76 655f 7375 7266 2720   if 'move_surf' 
-00024a10: 696e 2073 7070 5f70 6172 616d 732e 6d6f  in spp_params.mo
-00024a20: 7665 6d65 6e74 2e6b 6579 7328 293a 0a20  vement.keys():. 
-00024a30: 2020 2020 2020 2020 2020 2069 6620 7665             if ve
-00024a40: 7262 6f73 653a 0a20 2020 2020 2020 2020  rbose:.         
-00024a50: 2020 2020 2020 2070 7269 6e74 2828 275c         print(('\
-00024a60: 745c 745c 746d 616b 696e 6720 6d6f 7665  t\t\tmaking move
-00024a70: 6d65 6e74 2073 7572 6661 6365 2e2e 2e5c  ment surface...\
-00024a80: 6e27 0a20 2020 2020 2020 2020 2020 2020  n'.             
-00024a90: 2020 2020 2020 2020 2020 275c 745c 745c            '\t\t\
-00024aa0: 745c 745b 6361 6e20 7461 6b65 2061 2062  t\t[can take a b
-00024ab0: 6974 5d5c 6e27 292c 2066 6c75 7368 3d54  it]\n'), flush=T
-00024ac0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-00024ad0: 206d 735f 7061 7261 6d73 203d 2064 6565   ms_params = dee
-00024ae0: 7063 6f70 7928 7370 705f 7061 7261 6d73  pcopy(spp_params
-00024af0: 2e6d 6f76 656d 656e 742e 6d6f 7665 5f73  .movement.move_s
-00024b00: 7572 6629 0a20 2020 2020 2020 2020 2020  urf).           
-00024b10: 2023 6772 6162 2074 6865 206c 7972 206e   #grab the lyr n
-00024b20: 756d 6265 7220 666f 7220 7468 6520 6c79  umber for the ly
-00024b30: 7220 7468 6174 2074 6865 200a 2020 2020  r that the .    
-00024b40: 2020 2020 2020 2020 236d 6f76 656d 656e          #movemen
-00024b50: 7420 7375 7266 6163 6520 6973 2074 6f20  t surface is to 
-00024b60: 6265 2062 6173 6564 206f 6e0a 2020 2020  be based on.    
-00024b70: 2020 2020 2020 2020 6d6f 7665 5f73 7572          move_sur
-00024b80: 665f 6c79 7220 3d20 6d73 5f70 6172 616d  f_lyr = ms_param
-00024b90: 732e 706f 7028 276c 6179 6572 2729 0a20  s.pop('layer'). 
-00024ba0: 2020 2020 2020 2020 2020 206d 6f76 655f             move_
-00024bb0: 7375 7266 5f6c 7972 5f6e 756d 203d 205b  surf_lyr_num = [
-00024bc0: 6b20 666f 7220 6b2c 7620 696e 206c 616e  k for k,v in lan
-00024bd0: 642e 6974 656d 7328 0a20 2020 2020 2020  d.items(.       
-00024be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024c00: 2020 2020 2029 2069 6620 762e 6e61 6d65       ) if v.name
-00024c10: 203d 3d20 6d6f 7665 5f73 7572 665f 6c79   == move_surf_ly
-00024c20: 725d 0a20 2020 2020 2020 2020 2020 2061  r].            a
-00024c30: 7373 6572 7420 6c65 6e28 6d6f 7665 5f73  ssert len(move_s
-00024c40: 7572 665f 6c79 725f 6e75 6d29 203d 3d20  urf_lyr_num) == 
-00024c50: 312c 2028 2245 7870 6563 7465 6420 746f  1, ("Expected to
-00024c60: 2066 696e 6420 6f6e 6c79 2061 2022 0a20   find only a ". 
-00024c70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00024c80: 7369 6e67 6c65 204c 6179 6572 2077 6974  single Layer wit
-00024c90: 6820 7468 6520 6e61 6d65 2070 726f 7669  h the name provi
-00024ca0: 6465 6420 666f 7220 7468 6520 220a 2020  ded for the ".  
-00024cb0: 2020 2020 2020 2020 2020 2020 2020 225f                "_
-00024cc0: 436f 6e64 7563 7461 6e63 6553 7572 6661  ConductanceSurfa
-00024cd0: 6365 2c22 0a20 2020 2020 2020 2020 2020  ce,".           
-00024ce0: 2020 2020 2022 2062 7574 2069 6e73 7465       " but inste
-00024cf0: 6164 2066 6f75 6e64 2025 6922 2920 2520  ad found %i") % 
-00024d00: 6c65 6e28 6d6f 7665 5f73 7572 665f 6c79  len(move_surf_ly
-00024d10: 725f 6e75 6d29 0a20 2020 2020 2020 2020  r_num).         
-00024d20: 2020 206d 6f76 655f 7375 7266 5f6c 7972     move_surf_lyr
-00024d30: 5f6e 756d 203d 206d 6f76 655f 7375 7266  _num = move_surf
-00024d40: 5f6c 7972 5f6e 756d 5b30 5d0a 2020 2020  _lyr_num[0].    
-00024d50: 2020 2020 2020 2020 236d 616b 6520 7468          #make th
-00024d60: 6520 6d6f 7665 6d65 6e74 2073 7572 6661  e movement surfa
-00024d70: 6365 2061 6e64 2073 6574 2069 7420 6173  ce and set it as
-00024d80: 2074 6865 2073 7070 2773 0a20 2020 2020   the spp's.     
-00024d90: 2020 2020 2020 2023 6d6f 7665 5f73 7572         #move_sur
-00024da0: 6620 6174 7472 6962 7574 650a 2020 2020  f attribute.    
-00024db0: 2020 2020 2020 2020 7370 702e 5f6d 6f76          spp._mov
-00024dc0: 655f 7375 7266 3d20 7370 742e 5f43 6f6e  e_surf= spt._Con
-00024dd0: 6475 6374 616e 6365 5375 7266 6163 6528  ductanceSurface(
-00024de0: 6c61 6e64 5b6d 6f76 655f 7375 7266 5f6c  land[move_surf_l
-00024df0: 7972 5f6e 756d 5d2c 0a20 2020 2020 2020  yr_num],.       
-00024e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024e30: 2020 2020 2020 2020 202a 2a6d 735f 7061           **ms_pa
-00024e40: 7261 6d73 290a 2020 2020 236d 616b 6520  rams).    #make 
-00024e50: 6469 7370 6572 7361 6c20 7375 7266 6163  dispersal surfac
-00024e60: 652c 2069 6620 6e65 6564 6564 0a20 2020  e, if needed.   
-00024e70: 2069 6620 2764 6973 705f 7375 7266 2720   if 'disp_surf' 
-00024e80: 696e 2073 7070 5f70 6172 616d 732e 6d6f  in spp_params.mo
-00024e90: 7665 6d65 6e74 2e6b 6579 7328 293a 0a20  vement.keys():. 
-00024ea0: 2020 2020 2020 2023 2070 7269 6e74 2076         # print v
-00024eb0: 6572 626f 7365 206f 7574 7075 740a 2020  erbose output.  
-00024ec0: 2020 2020 2020 6966 2076 6572 626f 7365        if verbose
-00024ed0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00024ee0: 696e 7428 2827 5c74 5c74 5c74 6d61 6b69  int(('\t\t\tmaki
-00024ef0: 6e67 2064 6973 7065 7273 616c 2073 7572  ng dispersal sur
-00024f00: 6661 6365 2e2e 2e5c 6e27 0a20 2020 2020  face...\n'.     
-00024f10: 2020 2020 2020 2020 2020 2020 2020 275c                '\
-00024f20: 745c 745c 745c 745b 6361 6e20 7461 6b65  t\t\t\t[can take
-00024f30: 2061 2062 6974 5d5c 6e27 292c 2066 6c75   a bit]\n'), flu
-00024f40: 7368 3d54 7275 6529 0a20 2020 2020 2020  sh=True).       
-00024f50: 2064 735f 7061 7261 6d73 203d 2064 6565   ds_params = dee
-00024f60: 7063 6f70 7928 7370 705f 7061 7261 6d73  pcopy(spp_params
-00024f70: 2e6d 6f76 656d 656e 742e 6469 7370 5f73  .movement.disp_s
-00024f80: 7572 6629 0a20 2020 2020 2020 2023 6772  urf).        #gr
-00024f90: 6162 2074 6865 206c 7972 206e 756d 6265  ab the lyr numbe
-00024fa0: 7220 666f 7220 7468 6520 6c79 7220 7468  r for the lyr th
-00024fb0: 6174 2074 6865 200a 2020 2020 2020 2020  at the .        
-00024fc0: 2364 6973 7065 7273 616c 2073 7572 6661  #dispersal surfa
-00024fd0: 6365 2069 7320 746f 2062 6520 6261 7365  ce is to be base
-00024fe0: 6420 6f6e 0a20 2020 2020 2020 2064 6973  d on.        dis
-00024ff0: 705f 7375 7266 5f6c 7972 203d 2064 735f  p_surf_lyr = ds_
-00025000: 7061 7261 6d73 2e70 6f70 2827 6c61 7965  params.pop('laye
-00025010: 7227 290a 2020 2020 2020 2020 6469 7370  r').        disp
-00025020: 5f73 7572 665f 6c79 725f 6e75 6d20 3d20  _surf_lyr_num = 
-00025030: 5b6b 2066 6f72 206b 2c76 2069 6e20 6c61  [k for k,v in la
-00025040: 6e64 2e69 7465 6d73 280a 2020 2020 2020  nd.items(.      
-00025050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025070: 2020 2920 6966 2076 2e6e 616d 6520 3d3d    ) if v.name ==
-00025080: 2064 6973 705f 7375 7266 5f6c 7972 5d0a   disp_surf_lyr].
-00025090: 2020 2020 2020 2020 6173 7365 7274 206c          assert l
-000250a0: 656e 2864 6973 705f 7375 7266 5f6c 7972  en(disp_surf_lyr
-000250b0: 5f6e 756d 2920 3d3d 2031 2c20 2822 4578  _num) == 1, ("Ex
-000250c0: 7065 6374 6564 2074 6f20 6669 6e64 206f  pected to find o
-000250d0: 6e6c 7920 6120 220a 2020 2020 2020 2020  nly a ".        
-000250e0: 2020 2020 2273 696e 676c 6520 4c61 7965      "single Laye
-000250f0: 7220 7769 7468 2074 6865 206e 616d 6520  r with the name 
-00025100: 7072 6f76 6964 6564 2066 6f72 2074 6865  provided for the
-00025110: 2022 0a20 2020 2020 2020 2020 2020 2022   ".            "
-00025120: 5f43 6f6e 6475 6374 616e 6365 5375 7266  _ConductanceSurf
-00025130: 6163 652c 2022 0a20 2020 2020 2020 2020  ace, ".         
-00025140: 2020 2022 6275 7420 696e 7374 6561 6420     "but instead 
-00025150: 666f 756e 6420 2569 2229 2025 206c 656e  found %i") % len
-00025160: 2864 6973 705f 7375 7266 5f6c 7972 5f6e  (disp_surf_lyr_n
-00025170: 756d 290a 2020 2020 2020 2020 6469 7370  um).        disp
-00025180: 5f73 7572 665f 6c79 725f 6e75 6d20 3d20  _surf_lyr_num = 
-00025190: 6469 7370 5f73 7572 665f 6c79 725f 6e75  disp_surf_lyr_nu
-000251a0: 6d5b 305d 0a20 2020 2020 2020 2023 6d61  m[0].        #ma
-000251b0: 6b65 2074 6865 2064 6973 7065 7273 616c  ke the dispersal
-000251c0: 2073 7572 6661 6365 2061 6e64 2073 6574   surface and set
-000251d0: 2069 7420 6173 2074 6865 2073 7070 2773   it as the spp's
-000251e0: 0a20 2020 2020 2020 2023 6469 7370 5f73  .        #disp_s
-000251f0: 7572 6620 6174 7472 6962 7574 650a 2020  urf attribute.  
-00025200: 2020 2020 2020 7370 702e 5f64 6973 705f        spp._disp_
-00025210: 7375 7266 203d 2073 7074 2e5f 436f 6e64  surf = spt._Cond
-00025220: 7563 7461 6e63 6553 7572 6661 6365 286c  uctanceSurface(l
-00025230: 616e 645b 6469 7370 5f73 7572 665f 6c79  and[disp_surf_ly
-00025240: 725f 6e75 6d5d 2c0a 2020 2020 2020 2020  r_num],.        
-00025250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025280: 2020 2020 2020 2020 2a2a 6473 5f70 6172          **ds_par
-00025290: 616d 7329 0a0a 2020 2020 2369 6620 7468  ams)..    #if th
-000252a0: 6973 2073 7065 6369 6573 2068 6173 2063  is species has c
-000252b0: 6861 6e67 6573 2070 6172 616d 6574 6572  hanges parameter
-000252c0: 697a 6564 2c20 6f72 2069 6620 6e6f 7420  ized, or if not 
-000252d0: 6275 7420 6974 2068 6173 0a20 2020 2023  but it has.    #
-000252e0: 6569 7468 6572 2061 204d 6f76 656d 656e  either a Movemen
-000252f0: 7453 7572 6620 6f72 2061 2044 6973 7065  tSurf or a Dispe
-00025300: 7273 616c 5375 7266 2062 6173 6564 206f  rsalSurf based o
-00025310: 6e20 6120 4c61 7965 7220 7468 6174 0a20  n a Layer that. 
-00025320: 2020 2023 7769 6c6c 2075 6e64 6572 676f     #will undergo
-00025330: 206c 616e 6473 6361 7065 2063 6861 6e67   landscape chang
-00025340: 652c 2074 6865 6e20 6372 6561 7465 2061  e, then create a
-00025350: 205f 5370 6563 6965 7343 6861 6e67 6572   _SpeciesChanger
-00025360: 206f 626a 6563 7420 666f 7220 6974 0a20   object for it. 
-00025370: 2020 2069 6620 2827 6368 616e 6765 2720     if ('change' 
-00025380: 696e 2073 7070 5f70 6172 616d 732e 6b65  in spp_params.ke
-00025390: 7973 2829 0a20 2020 2020 2020 206f 7220  ys().        or 
-000253a0: 2873 7070 2e5f 6d6f 7665 5f73 7572 6620  (spp._move_surf 
-000253b0: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
-000253c0: 2020 2020 616e 6420 6c61 6e64 2e5f 6368      and land._ch
-000253d0: 616e 6765 7220 6973 206e 6f74 204e 6f6e  anger is not Non
-000253e0: 650a 2020 2020 2020 2020 616e 6420 7370  e.        and sp
-000253f0: 702e 5f6d 6f76 655f 7375 7266 2e6c 7972  p._move_surf.lyr
-00025400: 5f6e 756d 2069 6e20 6c61 6e64 2e5f 6368  _num in land._ch
-00025410: 616e 6765 722e 6368 616e 6765 5f69 6e66  anger.change_inf
-00025420: 6f2e 6b65 7973 2829 290a 2020 2020 2020  o.keys()).      
-00025430: 2020 6f72 2028 7370 702e 5f64 6973 705f    or (spp._disp_
-00025440: 7375 7266 2069 7320 6e6f 7420 4e6f 6e65  surf is not None
-00025450: 0a20 2020 2020 2020 2061 6e64 206c 616e  .        and lan
-00025460: 642e 5f63 6861 6e67 6572 2069 7320 6e6f  d._changer is no
-00025470: 7420 4e6f 6e65 0a20 2020 2020 2020 2061  t None.        a
-00025480: 6e64 2073 7070 2e5f 6469 7370 5f73 7572  nd spp._disp_sur
-00025490: 662e 6c79 725f 6e75 6d20 696e 206c 616e  f.lyr_num in lan
-000254a0: 642e 5f63 6861 6e67 6572 2e63 6861 6e67  d._changer.chang
-000254b0: 655f 696e 666f 2e6b 6579 7328 2929 293a  e_info.keys())):
-000254c0: 0a20 2020 2020 2020 2023 2070 7269 6e74  .        # print
-000254d0: 2076 6572 626f 7365 206f 7574 7075 740a   verbose output.
-000254e0: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
-000254f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00025500: 7072 696e 7428 2827 5c74 5c74 5c74 7365  print(('\t\t\tse
-00025510: 7474 696e 6720 7570 2073 7065 6369 6573  tting up species
-00025520: 2063 6861 6e67 6573 2e2e 2e5c 6e27 0a20   changes...\n'. 
-00025530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025540: 2020 275c 745c 745c 745c 745b 6361 6e20    '\t\t\t\t[can 
-00025550: 7461 6b65 2061 2077 6869 6c65 2c5c 6e5c  take a while,\n\
-00025560: 745c 745c 745c 7420 6966 206d 6f76 656d  t\t\t\t if movem
-00025570: 656e 7420 6f72 2027 0a20 2020 2020 2020  ent or '.       
-00025580: 2020 2020 2020 2020 2020 2020 2764 6973              'dis
-00025590: 7065 7273 616c 5c6e 5c74 5c74 5c74 5c74  persal\n\t\t\t\t
-000255a0: 2073 7572 6661 6365 7320 7769 6c6c 2063   surfaces will c
-000255b0: 6861 6e67 655d 5c6e 2729 2c20 666c 7573  hange]\n'), flus
-000255c0: 683d 5472 7565 290a 2020 2020 2020 2020  h=True).        
-000255d0: 2367 7261 6220 7468 6520 6368 616e 6765  #grab the change
-000255e0: 2070 6172 616d 7320 286f 7220 4e6f 6e65   params (or None
-000255f0: 2c20 6966 0a20 2020 2020 2020 2069 6620  , if.        if 
-00025600: 2763 6861 6e67 6527 2069 6e20 7370 705f  'change' in spp_
-00025610: 7061 7261 6d73 2e6b 6579 7328 293a 0a20  params.keys():. 
-00025620: 2020 2020 2020 2020 2020 2063 685f 7061             ch_pa
-00025630: 7261 6d73 203d 2073 7070 5f70 6172 616d  rams = spp_param
-00025640: 732e 6368 616e 6765 0a20 2020 2020 2020  s.change.       
-00025650: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00025660: 2020 2063 685f 7061 7261 6d73 203d 204e     ch_params = N
-00025670: 6f6e 650a 2020 2020 2020 2020 236d 616b  one.        #mak
-00025680: 6520 5f53 7065 6369 6573 4368 616e 6765  e _SpeciesChange
-00025690: 7220 616e 6420 7365 7420 6974 2074 6f20  r and set it to 
-000256a0: 7468 6520 7370 7027 7320 6368 616e 6765  the spp's change
-000256b0: 7220 6174 7472 6962 7574 650a 2020 2020  r attribute.    
-000256c0: 2020 2020 7370 702e 5f63 6861 6e67 6572      spp._changer
-000256d0: 203d 205f 5370 6563 6965 7343 6861 6e67   = _SpeciesChang
-000256e0: 6572 2873 7070 2c20 6368 5f70 6172 616d  er(spp, ch_param
-000256f0: 732c 206c 616e 6420 3d20 6c61 6e64 290a  s, land = land).
-00025700: 0a20 2020 2072 6574 7572 6e20 7370 700a  .    return spp.
-00025710: 0a0a 2320 6675 6e63 7469 6f6e 2066 6f72  ..# function for
-00025720: 2072 6561 6469 6e67 2069 6e20 6120 7069   reading in a pi
-00025730: 636b 6c65 6420 7370 700a 6465 6620 7265  ckled spp.def re
-00025740: 6164 5f70 6963 6b6c 6564 5f73 7070 2866  ad_pickled_spp(f
-00025750: 696c 656e 616d 6529 3a0a 2020 2020 696d  ilename):.    im
-00025760: 706f 7274 2063 5069 636b 6c65 0a20 2020  port cPickle.   
-00025770: 2077 6974 6820 6f70 656e 2866 696c 656e   with open(filen
-00025780: 616d 652c 2027 7262 2729 2061 7320 663a  ame, 'rb') as f:
-00025790: 0a20 2020 2020 2020 2073 7070 203d 2063  .        spp = c
-000257a0: 5069 636b 6c65 2e6c 6f61 6428 6629 0a20  Pickle.load(f). 
-000257b0: 2020 2072 6574 7572 6e20 7370 700a 0a0a     return spp...
+00023900: 2020 2274 6f20 706c 6f74 2061 6e20 6578    "to plot an ex
+00023910: 616d 706c 6520 7265 636f 6d62 696e 616e  ample recombinan
+00023920: 7420 220a 2020 2020 2020 2020 2020 2020  t ".            
+00023930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023950: 2267 656e 6f6d 652e 2229 0a0a 2020 2020  "genome.")..    
+00023960: 2020 2020 7265 636f 6d62 5f70 6174 6873      recomb_paths
+00023970: 203d 2073 656c 662e 6765 6e5f 6172 6368   = self.gen_arch
+00023980: 2e5f 7265 636f 6d62 5f70 6174 6873 2e5f  ._recomb_paths._
+00023990: 6765 745f 7061 7468 7328 3229 0a20 2020  get_paths(2).   
+000239a0: 2020 2020 2069 6478 7320 3d20 2830 2c20       idxs = (0, 
+000239b0: 3229 0a20 2020 2020 2020 206d 6f63 6b5f  2).        mock_
+000239c0: 7370 7020 3d20 7b7d 0a20 2020 2020 2020  spp = {}.       
+000239d0: 2066 6f72 2069 6478 2069 6e20 6964 7873   for idx in idxs
+000239e0: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
+000239f0: 775f 6765 6e6f 6d65 203d 206e 702e 6873  w_genome = np.hs
+00023a00: 7461 636b 285b 286e 702e 6f6e 6573 2828  tack([(np.ones((
+00023a10: 7365 6c66 2e67 656e 5f61 7263 682e 4c2c  self.gen_arch.L,
+00023a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023a40: 2020 2020 2020 2020 2020 2020 2020 2031                 1
+00023a50: 2929 202a 206e 2029 202b 2069 6478 2066  )) * n ) + idx f
+00023a60: 6f72 206e 2069 6e20 2831 2c32 295d 290a  or n in (1,2)]).
+00023a70: 2020 2020 2020 2020 2020 2020 6d6f 636b              mock
+00023a80: 5f73 7070 5b69 6478 5d20 3d20 496e 6469  _spp[idx] = Indi
+00023a90: 7669 6475 616c 2869 6478 3d69 6478 2c20  vidual(idx=idx, 
+00023aa0: 783d 302c 2079 3d30 2c0a 2020 2020 2020  x=0, y=0,.      
+00023ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023ad0: 206e 6577 5f67 656e 6f6d 653d 6e65 775f   new_genome=new_
+00023ae0: 6765 6e6f 6d65 290a 0a20 2020 2020 2020  genome)..       
+00023af0: 2072 6563 6f6d 625f 6765 6e6f 6d65 203d   recomb_genome =
+00023b00: 205f 646f 5f6d 6174 696e 6728 7370 703d   _do_mating(spp=
+00023b10: 6d6f 636b 5f73 7070 2c0a 2020 2020 2020  mock_spp,.      
+00023b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023b30: 2020 2020 2020 2020 2020 2020 206d 6174               mat
+00023b40: 696e 675f 7061 6972 733d 5b69 6478 735d  ing_pairs=[idxs]
+00023b50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00023b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023b70: 2020 2020 206e 5f6f 6666 7370 7269 6e67       n_offspring
+00023b80: 3d5b 315d 2c0a 2020 2020 2020 2020 2020  =[1],.          
+00023b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023ba0: 2020 2020 2020 2020 2072 6563 6f6d 625f           recomb_
+00023bb0: 7061 7468 733d 7265 636f 6d62 5f70 6174  paths=recomb_pat
+00023bc0: 6873 295b 305d 5b30 5d0a 2020 2020 2020  hs)[0][0].      
+00023bd0: 2020 2372 6563 6f6d 625f 6765 6e6f 6d65    #recomb_genome
+00023be0: 203d 2072 6563 6f6d 625f 6765 6e6f 6d65   = recomb_genome
+00023bf0: 2b31 0a20 2020 2020 2020 2023 7265 636f  +1.        #reco
+00023c00: 6d62 5f67 656e 6f6d 655b 3a2c 315d 203d  mb_genome[:,1] =
+00023c10: 2072 6563 6f6d 625f 6765 6e6f 6d65 5b3a   recomb_genome[:
+00023c20: 2c31 5d20 2a20 350a 2020 2020 2020 2020  ,1] * 5.        
+00023c30: 6669 6720 3d20 706c 742e 6669 6775 7265  fig = plt.figure
+00023c40: 2829 0a20 2020 2020 2020 2061 7820 3d20  ().        ax = 
+00023c50: 6669 672e 6164 645f 7375 6270 6c6f 7428  fig.add_subplot(
+00023c60: 3131 3129 0a20 2020 2020 2020 2061 782e  111).        ax.
+00023c70: 696d 7368 6f77 286e 702e 7265 7065 6174  imshow(np.repeat
+00023c80: 2872 6563 6f6d 625f 6765 6e6f 6d65 2c0a  (recomb_genome,.
+00023c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023ca0: 2020 2020 2020 2020 2020 2020 696e 7428              int(
+00023cb0: 302e 3035 202a 2073 656c 662e 6765 6e5f  0.05 * self.gen_
+00023cc0: 6172 6368 2e4c 292c 0a20 2020 2020 2020  arch.L),.       
+00023cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023ce0: 2020 2020 2061 7869 733d 3129 2c0a 2020       axis=1),.  
+00023cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023d00: 636d 6170 3d27 7465 7272 6169 6e27 290a  cmap='terrain').
+00023d10: 2020 2020 2020 2020 6178 2e73 6574 5f74          ax.set_t
+00023d20: 6974 6c65 2822 6761 6d65 7465 2030 2020  itle("gamete 0  
+00023d30: 2020 2067 616d 6574 6531 2229 0a20 2020     gamete1").   
+00023d40: 2020 2020 2061 782e 7365 745f 7874 6963       ax.set_xtic
+00023d50: 6b73 285b 5d29 0a20 2020 2020 2020 2061  ks([]).        a
+00023d60: 782e 7365 745f 796c 6162 656c 2827 6c6f  x.set_ylabel('lo
+00023d70: 6375 7327 290a 2020 2020 2020 2020 706c  cus').        pl
+00023d80: 742e 7368 6f77 2829 0a20 2020 2020 2020  t.show().       
+00023d90: 2072 6574 7572 6e28 7265 636f 6d62 5f70   return(recomb_p
+00023da0: 6174 6873 2c20 6d6f 636b 5f73 7070 2c20  aths, mock_spp, 
+00023db0: 7265 636f 6d62 5f67 656e 6f6d 6529 0a0a  recomb_genome)..
+00023dc0: 0a20 2020 2064 6566 205f 706c 6f74 5f73  .    def _plot_s
+00023dd0: 7461 7428 7365 6c66 2c20 7374 6174 293a  tat(self, stat):
+00023de0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00023df0: 2e5f 7374 6174 735f 636f 6c6c 6563 746f  ._stats_collecto
+00023e00: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
+00023e10: 2020 2020 2020 2070 7269 6e74 2828 2253         print(("S
+00023e20: 7065 6369 6573 2e5f 706c 6f74 5f73 7461  pecies._plot_sta
+00023e30: 7420 6973 206e 6f74 2076 616c 6964 2022  t is not valid "
+00023e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023e50: 2022 666f 7220 7370 6563 6965 7320 7769   "for species wi
+00023e60: 7468 206e 6f20 5f53 7461 7473 436f 6c6c  th no _StatsColl
+00023e70: 6563 746f 7220 6f62 6a65 6374 2e5c 6e22  ector object.\n"
+00023e80: 2929 0a0a 2020 2020 2020 2020 656c 7365  ))..        else
+00023e90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00023ea0: 6c66 2e5f 7374 6174 735f 636f 6c6c 6563  lf._stats_collec
+00023eb0: 746f 722e 5f70 6c6f 745f 7374 6174 2873  tor._plot_stat(s
+00023ec0: 7461 742c 2073 7070 5f6e 616d 6520 3d20  tat, spp_name = 
+00023ed0: 7365 6c66 2e6e 616d 6529 0a0a 0a20 2020  self.name)...   
+00023ee0: 2020 2020 2023 2323 2323 2323 2323 2323       ###########
+00023ef0: 2323 2323 230a 2020 2020 2020 2020 2370  #####.        #p
+00023f00: 7562 6c69 6320 6d65 7468 6f64 7323 0a20  ublic methods#. 
+00023f10: 2020 2020 2020 2023 2323 2323 2323 2323         #########
+00023f20: 2323 2323 2323 230a 0a20 2020 2064 6566  #######..    def
+00023f30: 205f 7772 6974 655f 7069 636b 6c65 2873   _write_pickle(s
+00023f40: 656c 662c 2066 696c 656e 616d 6529 3a0a  elf, filename):.
+00023f50: 2020 2020 2020 2020 696d 706f 7274 2063          import c
+00023f60: 5069 636b 6c65 0a20 2020 2020 2020 2077  Pickle.        w
+00023f70: 6974 6820 6f70 656e 2866 696c 656e 616d  ith open(filenam
+00023f80: 652c 2027 7762 2729 2061 7320 663a 0a20  e, 'wb') as f:. 
+00023f90: 2020 2020 2020 2020 2020 2063 5069 636b             cPick
+00023fa0: 6c65 2e64 756d 7028 7365 6c66 2c20 6629  le.dump(self, f)
+00023fb0: 0a0a 0a23 2323 2323 2323 2323 2323 2323  ...#############
+00023fc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00023fd0: 2323 2323 2323 2323 230a 2320 2d2d 2d2d  #########.# ----
+00023fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d23  ---------------#
+00024000: 0a23 2046 554e 4354 494f 4e53 202d 2d2d  .# FUNCTIONS ---
+00024010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024020: 2d2d 2d2d 2d2d 230a 2320 2d2d 2d2d 2d2d  ------#.# ------
+00024030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d23 0a23  -------------#.#
+00024050: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024060: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00024070: 2323 2323 230a 0a23 6675 6e63 7469 6f6e  #####..#function
+00024080: 2074 6f20 6265 2063 616c 6c65 6420 7768   to be called wh
+00024090: 656e 2061 2053 7065 6369 6573 2069 7320  en a Species is 
+000240a0: 696e 6974 6961 7465 642c 0a23 7768 6963  initiated,.#whic
+000240b0: 6820 7573 6573 2074 6865 2070 6172 616d  h uses the param
+000240c0: 732e 7370 6563 6965 735b 3c73 7070 5f6e  s.species[<spp_n
+000240d0: 756d 3e5d 2e69 6e69 742e 5b27 4b5f 3c3e  um>].init.['K_<>
+000240e0: 275d 2070 6172 616d 6574 6572 7320 0a23  '] parameters .#
+000240f0: 746f 206d 616b 6520 7468 6520 696e 6974  to make the init
+00024100: 6961 6c20 6361 7272 7969 6e67 2d63 6170  ial carrying-cap
+00024110: 6163 6974 7920 7261 7374 6572 2c20 616e  acity raster, an
+00024120: 6420 616c 736f 0a23 7365 7473 2074 6865  d also.#sets the
+00024130: 2053 7065 6369 6573 2720 4b5f 6c61 7965   Species' K_laye
+00024140: 7220 616e 6420 4b5f 6661 6374 6f72 2061  r and K_factor a
+00024150: 7474 7269 6275 7465 730a 6465 6620 5f6d  ttributes.def _m
+00024160: 616b 655f 4b28 7370 702c 206c 616e 642c  ake_K(spp, land,
+00024170: 204b 5f6c 6179 6572 2c20 4b5f 6661 6374   K_layer, K_fact
+00024180: 6f72 293a 0a20 2020 2023 6d61 6b65 2073  or):.    #make s
+00024190: 7572 6520 7765 2066 696e 6420 6f6e 6c79  ure we find only
+000241a0: 2061 2073 696e 676c 6520 6c61 7965 7220   a single layer 
+000241b0: 7769 7468 2074 6865 206e 616d 6520 7370  with the name sp
+000241c0: 6563 6966 6965 6420 6279 204b 5f6c 6179  ecified by K_lay
+000241d0: 6572 0a20 2020 204b 5f6c 6179 6572 203d  er.    K_layer =
+000241e0: 205b 6c79 7220 666f 7220 6c79 7220 696e   [lyr for lyr in
+000241f0: 206c 616e 642e 7661 6c75 6573 2829 2069   land.values() i
+00024200: 6620 6c79 722e 6e61 6d65 203d 3d20 4b5f  f lyr.name == K_
+00024210: 6c61 7965 725d 0a20 2020 2061 7373 6572  layer].    asser
+00024220: 7420 6c65 6e28 4b5f 6c61 7965 7229 203d  t len(K_layer) =
+00024230: 3d20 312c 2028 2254 6865 204b 5f6c 6179  = 1, ("The K_lay
+00024240: 6572 2070 6172 616d 6574 6572 2073 686f  er parameter sho
+00024250: 756c 6420 706f 696e 7420 746f 220a 2020  uld point to".  
+00024260: 2020 2020 2020 2261 2073 696e 676c 6520        "a single 
+00024270: 4c61 7965 722c 2062 7574 2069 6e73 7465  Layer, but inste
+00024280: 6164 2025 6920 4c61 7965 7273 2077 6572  ad %i Layers wer
+00024290: 6520 666f 756e 642e 2229 2025 206c 656e  e found.") % len
+000242a0: 284b 5f6c 6179 6572 290a 2020 2020 2367  (K_layer).    #g
+000242b0: 7261 6220 7468 6520 6964 656e 7469 6669  rab the identifi
+000242c0: 6564 206c 6179 6572 0a20 2020 204b 5f6c  ed layer.    K_l
+000242d0: 6179 6572 203d 204b 5f6c 6179 6572 5b30  ayer = K_layer[0
+000242e0: 5d0a 2020 2020 2373 6574 2074 6865 2053  ].    #set the S
+000242f0: 7065 6369 6573 2720 4b5f 6c61 7965 7220  pecies' K_layer 
+00024300: 616e 6420 4b5f 6661 6374 6f72 2061 7474  and K_factor att
+00024310: 7269 6275 7465 730a 2020 2020 7370 702e  ributes.    spp.
+00024320: 4b5f 6c61 7965 7220 3d20 4b5f 6c61 7965  K_layer = K_laye
+00024330: 722e 6964 780a 2020 2020 7370 702e 4b5f  r.idx.    spp.K_
+00024340: 6661 6374 6f72 203d 204b 5f66 6163 746f  factor = K_facto
+00024350: 720a 2020 2020 2361 6464 2074 6869 7320  r.    #add this 
+00024360: 5370 6563 6965 7320 746f 2074 6869 7320  Species to this 
+00024370: 4c61 7965 7227 7320 2e5f 6973 5f4b 2061  Layer's ._is_K a
+00024380: 7474 7269 6275 7465 0a20 2020 2023 2877  ttribute.    #(w
+00024390: 6869 6368 2077 696c 6c20 6265 2075 7365  hich will be use
+000243a0: 6420 746f 2075 7064 6174 6520 5370 6563  d to update Spec
+000243b0: 6965 732e 4b20 6966 2074 6869 7320 4c61  ies.K if this La
+000243c0: 7965 7220 756e 6465 7267 6f65 730a 2020  yer undergoes.  
+000243d0: 2020 2361 6e79 206b 616e 6473 6361 7065    #any kandscape
+000243e0: 2063 6861 6e67 6573 290a 2020 2020 4b5f   changes).    K_
+000243f0: 6c61 7965 722e 5f69 735f 4b2e 6170 7065  layer._is_K.appe
+00024400: 6e64 2873 7070 2e69 6478 290a 2020 2020  nd(spp.idx).    
+00024410: 236e 6f77 2063 616c 6375 6c61 7465 2061  #now calculate a
+00024420: 6e64 2073 6574 2074 6865 204b 2072 6173  nd set the K ras
+00024430: 7465 720a 2020 2020 7370 702e 5f73 6574  ter.    spp._set
+00024440: 5f4b 286c 616e 6429 0a0a 0a64 6566 205f  _K(land)...def _
+00024450: 6d61 6b65 5f73 7065 6369 6573 286c 616e  make_species(lan
+00024460: 642c 206e 616d 652c 2069 6478 2c20 7370  d, name, idx, sp
+00024470: 705f 7061 7261 6d73 2c20 6275 726e 3d46  p_params, burn=F
+00024480: 616c 7365 2c20 7665 7262 6f73 653d 4661  alse, verbose=Fa
+00024490: 6c73 6529 3a0a 2020 2020 2367 6574 2073  lse):.    #get s
+000244a0: 7070 2773 2069 6e74 6961 6c69 7a69 6e67  pp's intializing
+000244b0: 2070 6172 616d 730a 2020 2020 696e 6974   params.    init
+000244c0: 5f70 6172 616d 7320 3d20 6465 6570 636f  _params = deepco
+000244d0: 7079 2873 7070 5f70 6172 616d 732e 696e  py(spp_params.in
+000244e0: 6974 290a 0a20 2020 2023 2070 7269 6e74  it)..    # print
+000244f0: 2076 6572 626f 7365 206f 7574 7075 740a   verbose output.
+00024500: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+00024510: 2020 2020 2020 2020 7072 696e 7428 275c          print('\
+00024520: 745c 744d 414b 494e 4720 5350 4543 4945  t\tMAKING SPECIE
+00024530: 5320 2573 2e2e 2e5c 6e27 2025 206e 616d  S %s...\n' % nam
+00024540: 652c 2066 6c75 7368 3d54 7275 6529 0a0a  e, flush=True)..
+00024550: 2020 2020 2369 6620 7468 6973 2073 7065      #if this spe
+00024560: 6369 6573 2073 686f 756c 6420 6861 7665  cies should have
+00024570: 2067 656e 6f6d 6573 2c20 6372 6561 7465   genomes, create
+00024580: 2074 6865 2067 656e 6f6d 6963 2061 7263   the genomic arc
+00024590: 6869 7465 6374 7572 650a 2020 2020 6966  hitecture.    if
+000245a0: 2027 6765 6e5f 6172 6368 2720 696e 2073   'gen_arch' in s
+000245b0: 7070 5f70 6172 616d 732e 6b65 7973 2829  pp_params.keys()
+000245c0: 3a0a 2020 2020 2020 2020 2320 7072 696e  :.        # prin
+000245d0: 7420 7665 7262 6f73 6520 6f75 7470 7574  t verbose output
+000245e0: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
+000245f0: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+00024600: 2070 7269 6e74 2827 5c74 5c74 5c74 6d61   print('\t\t\tma
+00024610: 6b69 6e67 2067 656e 6f6d 6963 2061 7263  king genomic arc
+00024620: 6869 7465 6374 7572 652e 2e2e 5c6e 272c  hitecture...\n',
+00024630: 2066 6c75 7368 3d54 7275 6529 0a20 2020   flush=True).   
+00024640: 2020 2020 2067 5f70 6172 616d 7320 3d20       g_params = 
+00024650: 7370 705f 7061 7261 6d73 2e67 656e 5f61  spp_params.gen_a
+00024660: 7263 680a 2020 2020 2020 2020 236d 616b  rch.        #mak
+00024670: 6520 6765 6e6f 6d69 635f 6172 6368 6974  e genomic_archit
+00024680: 6563 7475 7265 0a20 2020 2020 2020 2067  ecture.        g
+00024690: 656e 5f61 7263 6820 3d20 5f6d 616b 655f  en_arch = _make_
+000246a0: 6765 6e6f 6d69 635f 6172 6368 6974 6563  genomic_architec
+000246b0: 7475 7265 2873 7070 5f70 6172 616d 7320  ture(spp_params 
+000246c0: 3d20 7370 705f 7061 7261 6d73 2c0a 2020  = spp_params,.  
+000246d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000246e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000246f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024700: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00024710: 6e64 203d 206c 616e 6429 0a20 2020 2065  nd = land).    e
+00024720: 6c73 653a 0a20 2020 2020 2020 2067 656e  lse:.        gen
+00024730: 5f61 7263 6820 3d20 4e6f 6e65 0a0a 2020  _arch = None..  
+00024740: 2020 2320 7072 696e 7420 7665 7262 6f73    # print verbos
+00024750: 6520 6f75 7470 7574 0a20 2020 2069 6620  e output.    if 
+00024760: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
+00024770: 2070 7269 6e74 2827 5c74 5c74 5c74 6d61   print('\t\t\tma
+00024780: 6b69 6e67 2069 6e64 6976 6964 7561 6c73  king individuals
+00024790: 2e2e 2e5c 6e27 2c20 666c 7573 683d 5472  ...\n', flush=Tr
+000247a0: 7565 290a 2020 2020 236d 616b 6520 696e  ue).    #make in
+000247b0: 6469 7669 6473 0a20 2020 204e 203d 2069  divids.    N = i
+000247c0: 6e69 745f 7061 7261 6d73 2e70 6f70 2827  nit_params.pop('
+000247d0: 4e27 290a 2020 2020 2363 7265 6174 6520  N').    #create 
+000247e0: 616e 206f 7264 6572 6564 2064 6963 7469  an ordered dicti
+000247f0: 6f6e 6172 7920 746f 2068 6f6c 6420 7468  onary to hold th
+00024800: 6520 696e 6469 7669 6475 616c 732c 2061  e individuals, a
+00024810: 6e64 2066 696c 6c20 6974 2075 700a 2020  nd fill it up.  
+00024820: 2020 696e 6473 203d 204f 4428 290a 2020    inds = OD().  
+00024830: 2020 666f 7220 696e 645f 6964 7820 696e    for ind_idx in
+00024840: 2072 616e 6765 284e 293a 0a20 2020 2020   range(N):.     
+00024850: 2020 2023 2075 7365 2069 6e64 6976 6964     # use individ
+00024860: 7561 6c2e 6372 6561 7465 5f69 6e64 6976  ual.create_indiv
+00024870: 6964 7561 6c20 746f 2073 696d 756c 6174  idual to simulat
+00024880: 6520 696e 6469 7669 6475 616c 730a 2020  e individuals.  
+00024890: 2020 2020 2020 2361 6e64 2061 6464 2074        #and add t
+000248a0: 6865 6d20 746f 2074 6865 2073 7065 6369  hem to the speci
+000248b0: 6573 0a20 2020 2020 2020 2069 6e64 203d  es.        ind =
+000248c0: 205f 6d61 6b65 5f69 6e64 6976 6964 7561   _make_individua
+000248d0: 6c28 6964 783d 696e 645f 6964 782c 206f  l(idx=ind_idx, o
+000248e0: 6666 7370 7269 6e67 3d46 616c 7365 2c0a  ffspring=False,.
+000248f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024900: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00024910: 696d 3d6c 616e 642e 6469 6d2c 2067 656e  im=land.dim, gen
+00024920: 6f6d 6963 5f61 7263 6869 7465 6374 7572  omic_architectur
+00024930: 653d 6765 6e5f 6172 6368 2c0a 2020 2020  e=gen_arch,.    
+00024940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024950: 2020 2020 2020 2020 2020 2062 7572 6e3d             burn=
+00024960: 6275 726e 290a 2020 2020 2020 2020 696e  burn).        in
+00024970: 6473 5b69 6e64 5f69 6478 5d20 3d20 696e  ds[ind_idx] = in
+00024980: 640a 0a20 2020 2023 6372 6561 7465 2074  d..    #create t
+00024990: 6865 2073 7065 6369 6573 2066 726f 6d20  he species from 
+000249a0: 7468 6f73 6520 696e 6469 7669 6475 616c  those individual
+000249b0: 730a 2020 2020 7370 7020 3d20 5370 6563  s.    spp = Spec
+000249c0: 6965 7328 6e61 6d65 203d 206e 616d 652c  ies(name = name,
+000249d0: 2069 6478 203d 2069 6478 2c20 696e 6473   idx = idx, inds
+000249e0: 203d 2069 6e64 732c 206c 616e 6420 3d20   = inds, land = 
+000249f0: 6c61 6e64 2c0a 2020 2020 2020 2020 2020  land,.          
+00024a00: 2020 2020 2020 2020 2020 2073 7070 5f70             spp_p
+00024a10: 6172 616d 7320 3d20 7370 705f 7061 7261  arams = spp_para
+00024a20: 6d73 2c20 6765 6e6f 6d69 635f 6172 6368  ms, genomic_arch
+00024a30: 6974 6563 7475 7265 3d67 656e 5f61 7263  itecture=gen_arc
+00024a40: 6829 0a0a 2020 2020 2375 7365 2074 6865  h)..    #use the
+00024a50: 2072 656d 6169 6e69 6e67 2069 6e69 745f   remaining init_
+00024a60: 7061 7261 6d73 2074 6f20 7365 7420 7468  params to set th
+00024a70: 6520 6361 7272 7969 6e67 2d63 6170 6163  e carrying-capac
+00024a80: 6974 7920 7261 7374 6572 2028 4b29 0a20  ity raster (K). 
+00024a90: 2020 205f 6d61 6b65 5f4b 2873 7070 2c20     _make_K(spp, 
+00024aa0: 6c61 6e64 2c20 2a2a 7b6b 3a76 2066 6f72  land, **{k:v for
+00024ab0: 206b 2c76 2069 6e20 696e 6974 5f70 6172   k,v in init_par
+00024ac0: 616d 732e 6974 656d 7328 2920 6966 206b  ams.items() if k
+00024ad0: 2021 3d20 276d 7370 7269 6d65 277d 290a   != 'msprime'}).
+00024ae0: 2020 2020 2373 6574 2069 6e69 7469 616c      #set initial
+00024af0: 2065 6e76 6972 6f6e 6d65 6e74 2076 616c   environment val
+00024b00: 7565 730a 2020 2020 7370 702e 5f73 6574  ues.    spp._set
+00024b10: 5f65 286c 616e 6429 0a20 2020 2023 7365  _e(land).    #se
+00024b20: 7420 696e 6974 6961 6c20 636f 6f72 6473  t initial coords
+00024b30: 2061 6e64 2063 656c 6c73 0a20 2020 2073   and cells.    s
+00024b40: 7070 2e5f 7365 745f 636f 6f72 6473 5f61  pp._set_coords_a
+00024b50: 6e64 5f63 656c 6c73 2829 0a20 2020 2023  nd_cells().    #
+00024b60: 7365 7420 7468 6520 6b64 5f74 7265 650a  set the kd_tree.
+00024b70: 2020 2020 7370 702e 5f73 6574 5f6b 645f      spp._set_kd_
+00024b80: 7472 6565 2829 0a0a 2020 2020 2373 6574  tree()..    #set
+00024b90: 2070 6865 6e6f 7479 7065 732c 2069 6620   phenotypes, if 
+00024ba0: 7468 6520 7370 6563 6965 7320 6861 7320  the species has 
+00024bb0: 6765 6e6f 6d65 730a 2020 2020 6966 2073  genomes.    if s
+00024bc0: 7070 2e67 656e 5f61 7263 6820 6973 206e  pp.gen_arch is n
+00024bd0: 6f74 204e 6f6e 6520 616e 6420 6e6f 7420  ot None and not 
+00024be0: 6275 726e 3a0a 2020 2020 2020 2020 5b69  burn:.        [i
+00024bf0: 6e64 2e5f 7365 745f 7a28 7370 702e 6765  nd._set_z(spp.ge
+00024c00: 6e5f 6172 6368 2920 666f 7220 696e 6420  n_arch) for ind 
+00024c10: 696e 2073 7070 2e76 616c 7565 7328 295d  in spp.values()]
+00024c20: 0a0a 2020 2020 236d 616b 6520 6465 6e73  ..    #make dens
+00024c30: 6974 795f 6772 6964 0a20 2020 2073 7070  ity_grid.    spp
+00024c40: 2e5f 7365 745f 6465 6e73 5f67 7269 6473  ._set_dens_grids
+00024c50: 286c 616e 6429 0a0a 2020 2020 236d 616b  (land)..    #mak
+00024c60: 6520 6d6f 7665 6d65 6e74 2073 7572 6661  e movement surfa
+00024c70: 6365 2c20 6966 206e 6565 6465 640a 2020  ce, if needed.  
+00024c80: 2020 6966 2073 7070 2e5f 6d6f 7665 3a0a    if spp._move:.
+00024c90: 2020 2020 2020 2020 6966 2027 6d6f 7665          if 'move
+00024ca0: 5f73 7572 6627 2069 6e20 7370 705f 7061  _surf' in spp_pa
+00024cb0: 7261 6d73 2e6d 6f76 656d 656e 742e 6b65  rams.movement.ke
+00024cc0: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
+00024cd0: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
+00024ce0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00024cf0: 696e 7428 2827 5c74 5c74 5c74 6d61 6b69  int(('\t\t\tmaki
+00024d00: 6e67 206d 6f76 656d 656e 7420 7375 7266  ng movement surf
+00024d10: 6163 652e 2e2e 5c6e 270a 2020 2020 2020  ace...\n'.      
+00024d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024d30: 2027 5c74 5c74 5c74 5c74 5b63 616e 2074   '\t\t\t\t[can t
+00024d40: 616b 6520 6120 6269 745d 5c6e 2729 2c20  ake a bit]\n'), 
+00024d50: 666c 7573 683d 5472 7565 290a 2020 2020  flush=True).    
+00024d60: 2020 2020 2020 2020 6d73 5f70 6172 616d          ms_param
+00024d70: 7320 3d20 6465 6570 636f 7079 2873 7070  s = deepcopy(spp
+00024d80: 5f70 6172 616d 732e 6d6f 7665 6d65 6e74  _params.movement
+00024d90: 2e6d 6f76 655f 7375 7266 290a 2020 2020  .move_surf).    
+00024da0: 2020 2020 2020 2020 2367 7261 6220 7468          #grab th
+00024db0: 6520 6c79 7220 6e75 6d62 6572 2066 6f72  e lyr number for
+00024dc0: 2074 6865 206c 7972 2074 6861 7420 7468   the lyr that th
+00024dd0: 6520 0a20 2020 2020 2020 2020 2020 2023  e .            #
+00024de0: 6d6f 7665 6d65 6e74 2073 7572 6661 6365  movement surface
+00024df0: 2069 7320 746f 2062 6520 6261 7365 6420   is to be based 
+00024e00: 6f6e 0a20 2020 2020 2020 2020 2020 206d  on.            m
+00024e10: 6f76 655f 7375 7266 5f6c 7972 203d 206d  ove_surf_lyr = m
+00024e20: 735f 7061 7261 6d73 2e70 6f70 2827 6c61  s_params.pop('la
+00024e30: 7965 7227 290a 2020 2020 2020 2020 2020  yer').          
+00024e40: 2020 6d6f 7665 5f73 7572 665f 6c79 725f    move_surf_lyr_
+00024e50: 6e75 6d20 3d20 5b6b 2066 6f72 206b 2c76  num = [k for k,v
+00024e60: 2069 6e20 6c61 6e64 2e69 7465 6d73 280a   in land.items(.
+00024e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024e90: 2020 2020 2020 2020 2020 2020 2920 6966              ) if
+00024ea0: 2076 2e6e 616d 6520 3d3d 206d 6f76 655f   v.name == move_
+00024eb0: 7375 7266 5f6c 7972 5d0a 2020 2020 2020  surf_lyr].      
+00024ec0: 2020 2020 2020 6173 7365 7274 206c 656e        assert len
+00024ed0: 286d 6f76 655f 7375 7266 5f6c 7972 5f6e  (move_surf_lyr_n
+00024ee0: 756d 2920 3d3d 2031 2c20 2822 4578 7065  um) == 1, ("Expe
+00024ef0: 6374 6564 2074 6f20 6669 6e64 206f 6e6c  cted to find onl
+00024f00: 7920 6120 220a 2020 2020 2020 2020 2020  y a ".          
+00024f10: 2020 2020 2020 2273 696e 676c 6520 4c61        "single La
+00024f20: 7965 7220 7769 7468 2074 6865 206e 616d  yer with the nam
+00024f30: 6520 7072 6f76 6964 6564 2066 6f72 2074  e provided for t
+00024f40: 6865 2022 0a20 2020 2020 2020 2020 2020  he ".           
+00024f50: 2020 2020 2022 5f43 6f6e 6475 6374 616e       "_Conductan
+00024f60: 6365 5375 7266 6163 652c 220a 2020 2020  ceSurface,".    
+00024f70: 2020 2020 2020 2020 2020 2020 2220 6275              " bu
+00024f80: 7420 696e 7374 6561 6420 666f 756e 6420  t instead found 
+00024f90: 2569 2229 2025 206c 656e 286d 6f76 655f  %i") % len(move_
+00024fa0: 7375 7266 5f6c 7972 5f6e 756d 290a 2020  surf_lyr_num).  
+00024fb0: 2020 2020 2020 2020 2020 6d6f 7665 5f73            move_s
+00024fc0: 7572 665f 6c79 725f 6e75 6d20 3d20 6d6f  urf_lyr_num = mo
+00024fd0: 7665 5f73 7572 665f 6c79 725f 6e75 6d5b  ve_surf_lyr_num[
+00024fe0: 305d 0a20 2020 2020 2020 2020 2020 2023  0].            #
+00024ff0: 6d61 6b65 2074 6865 206d 6f76 656d 656e  make the movemen
+00025000: 7420 7375 7266 6163 6520 616e 6420 7365  t surface and se
+00025010: 7420 6974 2061 7320 7468 6520 7370 7027  t it as the spp'
+00025020: 730a 2020 2020 2020 2020 2020 2020 236d  s.            #m
+00025030: 6f76 655f 7375 7266 2061 7474 7269 6275  ove_surf attribu
+00025040: 7465 0a20 2020 2020 2020 2020 2020 2073  te.            s
+00025050: 7070 2e5f 6d6f 7665 5f73 7572 663d 2073  pp._move_surf= s
+00025060: 7074 2e5f 436f 6e64 7563 7461 6e63 6553  pt._ConductanceS
+00025070: 7572 6661 6365 286c 616e 645b 6d6f 7665  urface(land[move
+00025080: 5f73 7572 665f 6c79 725f 6e75 6d5d 2c0a  _surf_lyr_num],.
+00025090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000250a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000250b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000250c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000250d0: 2a2a 6d73 5f70 6172 616d 7329 0a20 2020  **ms_params).   
+000250e0: 2023 6d61 6b65 2064 6973 7065 7273 616c   #make dispersal
+000250f0: 2073 7572 6661 6365 2c20 6966 206e 6565   surface, if nee
+00025100: 6465 640a 2020 2020 6966 2027 6469 7370  ded.    if 'disp
+00025110: 5f73 7572 6627 2069 6e20 7370 705f 7061  _surf' in spp_pa
+00025120: 7261 6d73 2e6d 6f76 656d 656e 742e 6b65  rams.movement.ke
+00025130: 7973 2829 3a0a 2020 2020 2020 2020 2320  ys():.        # 
+00025140: 7072 696e 7420 7665 7262 6f73 6520 6f75  print verbose ou
+00025150: 7470 7574 0a20 2020 2020 2020 2069 6620  tput.        if 
+00025160: 7665 7262 6f73 653a 0a20 2020 2020 2020  verbose:.       
+00025170: 2020 2020 2070 7269 6e74 2828 275c 745c       print(('\t\
+00025180: 745c 746d 616b 696e 6720 6469 7370 6572  t\tmaking disper
+00025190: 7361 6c20 7375 7266 6163 652e 2e2e 5c6e  sal surface...\n
+000251a0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+000251b0: 2020 2020 2027 5c74 5c74 5c74 5c74 5b63       '\t\t\t\t[c
+000251c0: 616e 2074 616b 6520 6120 6269 745d 5c6e  an take a bit]\n
+000251d0: 2729 2c20 666c 7573 683d 5472 7565 290a  '), flush=True).
+000251e0: 2020 2020 2020 2020 6473 5f70 6172 616d          ds_param
+000251f0: 7320 3d20 6465 6570 636f 7079 2873 7070  s = deepcopy(spp
+00025200: 5f70 6172 616d 732e 6d6f 7665 6d65 6e74  _params.movement
+00025210: 2e64 6973 705f 7375 7266 290a 2020 2020  .disp_surf).    
+00025220: 2020 2020 2367 7261 6220 7468 6520 6c79      #grab the ly
+00025230: 7220 6e75 6d62 6572 2066 6f72 2074 6865  r number for the
+00025240: 206c 7972 2074 6861 7420 7468 6520 0a20   lyr that the . 
+00025250: 2020 2020 2020 2023 6469 7370 6572 7361         #dispersa
+00025260: 6c20 7375 7266 6163 6520 6973 2074 6f20  l surface is to 
+00025270: 6265 2062 6173 6564 206f 6e0a 2020 2020  be based on.    
+00025280: 2020 2020 6469 7370 5f73 7572 665f 6c79      disp_surf_ly
+00025290: 7220 3d20 6473 5f70 6172 616d 732e 706f  r = ds_params.po
+000252a0: 7028 276c 6179 6572 2729 0a20 2020 2020  p('layer').     
+000252b0: 2020 2064 6973 705f 7375 7266 5f6c 7972     disp_surf_lyr
+000252c0: 5f6e 756d 203d 205b 6b20 666f 7220 6b2c  _num = [k for k,
+000252d0: 7620 696e 206c 616e 642e 6974 656d 7328  v in land.items(
+000252e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000252f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025300: 2020 2020 2020 2020 2029 2069 6620 762e           ) if v.
+00025310: 6e61 6d65 203d 3d20 6469 7370 5f73 7572  name == disp_sur
+00025320: 665f 6c79 725d 0a20 2020 2020 2020 2061  f_lyr].        a
+00025330: 7373 6572 7420 6c65 6e28 6469 7370 5f73  ssert len(disp_s
+00025340: 7572 665f 6c79 725f 6e75 6d29 203d 3d20  urf_lyr_num) == 
+00025350: 312c 2028 2245 7870 6563 7465 6420 746f  1, ("Expected to
+00025360: 2066 696e 6420 6f6e 6c79 2061 2022 0a20   find only a ". 
+00025370: 2020 2020 2020 2020 2020 2022 7369 6e67             "sing
+00025380: 6c65 204c 6179 6572 2077 6974 6820 7468  le Layer with th
+00025390: 6520 6e61 6d65 2070 726f 7669 6465 6420  e name provided 
+000253a0: 666f 7220 7468 6520 220a 2020 2020 2020  for the ".      
+000253b0: 2020 2020 2020 225f 436f 6e64 7563 7461        "_Conducta
+000253c0: 6e63 6553 7572 6661 6365 2c20 220a 2020  nceSurface, ".  
+000253d0: 2020 2020 2020 2020 2020 2262 7574 2069            "but i
+000253e0: 6e73 7465 6164 2066 6f75 6e64 2025 6922  nstead found %i"
+000253f0: 2920 2520 6c65 6e28 6469 7370 5f73 7572  ) % len(disp_sur
+00025400: 665f 6c79 725f 6e75 6d29 0a20 2020 2020  f_lyr_num).     
+00025410: 2020 2064 6973 705f 7375 7266 5f6c 7972     disp_surf_lyr
+00025420: 5f6e 756d 203d 2064 6973 705f 7375 7266  _num = disp_surf
+00025430: 5f6c 7972 5f6e 756d 5b30 5d0a 2020 2020  _lyr_num[0].    
+00025440: 2020 2020 236d 616b 6520 7468 6520 6469      #make the di
+00025450: 7370 6572 7361 6c20 7375 7266 6163 6520  spersal surface 
+00025460: 616e 6420 7365 7420 6974 2061 7320 7468  and set it as th
+00025470: 6520 7370 7027 730a 2020 2020 2020 2020  e spp's.        
+00025480: 2364 6973 705f 7375 7266 2061 7474 7269  #disp_surf attri
+00025490: 6275 7465 0a20 2020 2020 2020 2073 7070  bute.        spp
+000254a0: 2e5f 6469 7370 5f73 7572 6620 3d20 7370  ._disp_surf = sp
+000254b0: 742e 5f43 6f6e 6475 6374 616e 6365 5375  t._ConductanceSu
+000254c0: 7266 6163 6528 6c61 6e64 5b64 6973 705f  rface(land[disp_
+000254d0: 7375 7266 5f6c 7972 5f6e 756d 5d2c 0a20  surf_lyr_num],. 
+000254e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000254f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025510: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+00025520: 2a64 735f 7061 7261 6d73 290a 0a20 2020  *ds_params)..   
+00025530: 2023 6966 2074 6869 7320 7370 6563 6965   #if this specie
+00025540: 7320 6861 7320 6368 616e 6765 7320 7061  s has changes pa
+00025550: 7261 6d65 7465 7269 7a65 642c 206f 7220  rameterized, or 
+00025560: 6966 206e 6f74 2062 7574 2069 7420 6861  if not but it ha
+00025570: 730a 2020 2020 2365 6974 6865 7220 6120  s.    #either a 
+00025580: 4d6f 7665 6d65 6e74 5375 7266 206f 7220  MovementSurf or 
+00025590: 6120 4469 7370 6572 7361 6c53 7572 6620  a DispersalSurf 
+000255a0: 6261 7365 6420 6f6e 2061 204c 6179 6572  based on a Layer
+000255b0: 2074 6861 740a 2020 2020 2377 696c 6c20   that.    #will 
+000255c0: 756e 6465 7267 6f20 6c61 6e64 7363 6170  undergo landscap
+000255d0: 6520 6368 616e 6765 2c20 7468 656e 2063  e change, then c
+000255e0: 7265 6174 6520 6120 5f53 7065 6369 6573  reate a _Species
+000255f0: 4368 616e 6765 7220 6f62 6a65 6374 2066  Changer object f
+00025600: 6f72 2069 740a 2020 2020 6966 2028 2763  or it.    if ('c
+00025610: 6861 6e67 6527 2069 6e20 7370 705f 7061  hange' in spp_pa
+00025620: 7261 6d73 2e6b 6579 7328 290a 2020 2020  rams.keys().    
+00025630: 2020 2020 6f72 2028 7370 702e 5f6d 6f76      or (spp._mov
+00025640: 655f 7375 7266 2069 7320 6e6f 7420 4e6f  e_surf is not No
+00025650: 6e65 0a20 2020 2020 2020 2061 6e64 206c  ne.        and l
+00025660: 616e 642e 5f63 6861 6e67 6572 2069 7320  and._changer is 
+00025670: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+00025680: 2061 6e64 2073 7070 2e5f 6d6f 7665 5f73   and spp._move_s
+00025690: 7572 662e 6c79 725f 6e75 6d20 696e 206c  urf.lyr_num in l
+000256a0: 616e 642e 5f63 6861 6e67 6572 2e63 6861  and._changer.cha
+000256b0: 6e67 655f 696e 666f 2e6b 6579 7328 2929  nge_info.keys())
+000256c0: 0a20 2020 2020 2020 206f 7220 2873 7070  .        or (spp
+000256d0: 2e5f 6469 7370 5f73 7572 6620 6973 206e  ._disp_surf is n
+000256e0: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+000256f0: 616e 6420 6c61 6e64 2e5f 6368 616e 6765  and land._change
+00025700: 7220 6973 206e 6f74 204e 6f6e 650a 2020  r is not None.  
+00025710: 2020 2020 2020 616e 6420 7370 702e 5f64        and spp._d
+00025720: 6973 705f 7375 7266 2e6c 7972 5f6e 756d  isp_surf.lyr_num
+00025730: 2069 6e20 6c61 6e64 2e5f 6368 616e 6765   in land._change
+00025740: 722e 6368 616e 6765 5f69 6e66 6f2e 6b65  r.change_info.ke
+00025750: 7973 2829 2929 3a0a 2020 2020 2020 2020  ys())):.        
+00025760: 2320 7072 696e 7420 7665 7262 6f73 6520  # print verbose 
+00025770: 6f75 7470 7574 0a20 2020 2020 2020 2069  output.        i
+00025780: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
+00025790: 2020 2020 2020 2070 7269 6e74 2828 275c         print(('\
+000257a0: 745c 745c 7473 6574 7469 6e67 2075 7020  t\t\tsetting up 
+000257b0: 7370 6563 6965 7320 6368 616e 6765 732e  species changes.
+000257c0: 2e2e 5c6e 270a 2020 2020 2020 2020 2020  ..\n'.          
+000257d0: 2020 2020 2020 2020 2027 5c74 5c74 5c74           '\t\t\t
+000257e0: 5c74 5b63 616e 2074 616b 6520 6120 7768  \t[can take a wh
+000257f0: 696c 652c 5c6e 5c74 5c74 5c74 5c74 2069  ile,\n\t\t\t\t i
+00025800: 6620 6d6f 7665 6d65 6e74 206f 7220 270a  f movement or '.
+00025810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025820: 2020 2027 6469 7370 6572 7361 6c5c 6e5c     'dispersal\n\
+00025830: 745c 745c 745c 7420 7375 7266 6163 6573  t\t\t\t surfaces
+00025840: 2077 696c 6c20 6368 616e 6765 5d5c 6e27   will change]\n'
+00025850: 292c 2066 6c75 7368 3d54 7275 6529 0a20  ), flush=True). 
+00025860: 2020 2020 2020 2023 6772 6162 2074 6865         #grab the
+00025870: 2063 6861 6e67 6520 7061 7261 6d73 2028   change params (
+00025880: 6f72 204e 6f6e 652c 2069 660a 2020 2020  or None, if.    
+00025890: 2020 2020 6966 2027 6368 616e 6765 2720      if 'change' 
+000258a0: 696e 2073 7070 5f70 6172 616d 732e 6b65  in spp_params.ke
+000258b0: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
+000258c0: 2020 6368 5f70 6172 616d 7320 3d20 7370    ch_params = sp
+000258d0: 705f 7061 7261 6d73 2e63 6861 6e67 650a  p_params.change.
+000258e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000258f0: 2020 2020 2020 2020 2020 6368 5f70 6172            ch_par
+00025900: 616d 7320 3d20 4e6f 6e65 0a20 2020 2020  ams = None.     
+00025910: 2020 2023 6d61 6b65 205f 5370 6563 6965     #make _Specie
+00025920: 7343 6861 6e67 6572 2061 6e64 2073 6574  sChanger and set
+00025930: 2069 7420 746f 2074 6865 2073 7070 2773   it to the spp's
+00025940: 2063 6861 6e67 6572 2061 7474 7269 6275   changer attribu
+00025950: 7465 0a20 2020 2020 2020 2073 7070 2e5f  te.        spp._
+00025960: 6368 616e 6765 7220 3d20 5f53 7065 6369  changer = _Speci
+00025970: 6573 4368 616e 6765 7228 7370 702c 2063  esChanger(spp, c
+00025980: 685f 7061 7261 6d73 2c20 6c61 6e64 203d  h_params, land =
+00025990: 206c 616e 6429 0a0a 2020 2020 7265 7475   land)..    retu
+000259a0: 726e 2073 7070 0a0a 0a23 2066 756e 6374  rn spp...# funct
+000259b0: 696f 6e20 666f 7220 7265 6164 696e 6720  ion for reading 
+000259c0: 696e 2061 2070 6963 6b6c 6564 2073 7070  in a pickled spp
+000259d0: 0a64 6566 2072 6561 645f 7069 636b 6c65  .def read_pickle
+000259e0: 645f 7370 7028 6669 6c65 6e61 6d65 293a  d_spp(filename):
+000259f0: 0a20 2020 2069 6d70 6f72 7420 6350 6963  .    import cPic
+00025a00: 6b6c 650a 2020 2020 7769 7468 206f 7065  kle.    with ope
+00025a10: 6e28 6669 6c65 6e61 6d65 2c20 2772 6227  n(filename, 'rb'
+00025a20: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
+00025a30: 7370 7020 3d20 6350 6963 6b6c 652e 6c6f  spp = cPickle.lo
+00025a40: 6164 2866 290a 2020 2020 7265 7475 726e  ad(f).    return
+00025a50: 2073 7070 0a0a 0a                         spp...
```

### Comparing `geonomics-1.4.2/geonomics/utils/_str_repr_.py` & `geonomics-1.4.3/geonomics/utils/_str_repr_.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/utils/io.py` & `geonomics-1.4.3/geonomics/utils/io.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/utils/spatial.py` & `geonomics-1.4.3/geonomics/utils/spatial.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics/utils/viz.py` & `geonomics-1.4.3/geonomics/utils/viz.py`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/geonomics.egg-info/PKG-INFO` & `geonomics-1.4.3/geonomics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: geonomics
-Version: 1.4.2
+Version: 1.4.3
 Summary: A package for landscape genomic simulation
 Home-page: https://github.com/drewhart/geonomics
-Download-URL: https://github.com/drewhart/geonomics/archive/1.4.2.tar.gz
+Download-URL: https://github.com/drewhart/geonomics/archive/1.4.3.tar.gz
 Author: Drew Ellison Hart
 Author-email: drew.ellison.hart@gmail.com
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/drewhart/geonomics/blob/master/doc/built/doc.html
 Project-URL: Methods Paper, https://doi.org/10.1093/molbev/msab175
 Project-URL: Source, https://github.com/drewhart/geonomics
 Keywords: landscape genomics genetics ecology evolution simulation model environmental model agent-based
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geonomics-1.4.2/geonomics.egg-info/SOURCES.txt` & `geonomics-1.4.3/geonomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geonomics-1.4.2/setup.py` & `geonomics-1.4.3/setup.py`

 * *Files identical despite different names*

