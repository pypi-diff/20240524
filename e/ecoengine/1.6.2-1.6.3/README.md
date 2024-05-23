# Comparing `tmp/ecoengine-1.6.2.tar.gz` & `tmp/ecoengine-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoengine-1.6.2.tar", last modified: Mon May 20 22:43:36 2024, max compression
+gzip compressed data, was "ecoengine-1.6.3.tar", last modified: Thu May 23 23:53:32 2024, max compression
```

## Comparing `ecoengine-1.6.2.tar` & `ecoengine-1.6.3.tar`

### file list

```diff
@@ -1,300 +1,300 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.218585 ecoengine-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-20 22:41:57.000000 ecoengine-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-20 22:43:36.218585 ecoengine-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-20 22:41:57.000000 ecoengine-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-20 22:41:57.000000 ecoengine-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-20 22:43:36.218585 ecoengine-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 22:41:57.000000 ecoengine-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.134584 ecoengine-1.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.138584 ecoengine-1.6.2/src/ecoengine/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.138584 ecoengine-1.6.2/src/ecoengine/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/constants/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.138584 ecoengine-1.6.2/src/ecoengine/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.146584 ecoengine-1.6.2/src/ecoengine/data/climate_data/
--rw-r--r--   0 runner    (1001) docker     (127)  3784790 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv
--rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/climate_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1728735 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.150584 ecoengine-1.6.2/src/ecoengine/data/load_shapes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/apartment.json
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/elementary_school.json
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/food_service_a.json
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/food_service_b.json
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/junior_high.json
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/mens_dorm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/motel.json
--rw-r--r--   0 runner    (1001) docker     (127)   262011 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/multi_family.json
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/nursing_home.json
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/office_building.json
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/senior_high.json
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/load_shapes/womens_dorm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.150584 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58109 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/maps.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.214585 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19141 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19445 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18191 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19680 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19737 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18589 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    17837 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18580 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18932 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    18022 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21000 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.214585 ecoengine-1.6.2/src/ecoengine/engine/
--rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/engine/BuildingCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)    44309 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/engine/EcosizerEngine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/engine/Simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/engine/SystemCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.214585 ecoengine-1.6.2/src/ecoengine/objects/
--rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/Building.py
--rw-r--r--   0 runner    (1001) docker     (127)    30767 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/PrefMapTracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    34744 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/SimulationRun.py
--rw-r--r--   0 runner    (1001) docker     (127)    48934 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/SystemConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/UtilityCostTracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systemConfigUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.218585 ecoengine-1.6.2/src/ecoengine/objects/systems/
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/MultiPass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/MultiPassRecirc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/ParallelLoopTank.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/PrimaryWithRecirc.py
--rw-r--r--   0 runner    (1001) docker     (127)    26555 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/SwingTank.py
--rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/SwingTankER.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:41:57.000000 ecoengine-1.6.2/src/ecoengine/objects/systems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:43:36.218585 ecoengine-1.6.2/src/ecoengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-20 22:43:36.000000 ecoengine-1.6.2/src/ecoengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23016 2024-05-20 22:43:36.000000 ecoengine-1.6.2/src/ecoengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:43:36.000000 ecoengine-1.6.2/src/ecoengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 22:43:36.000000 ecoengine-1.6.2/src/ecoengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 22:43:36.000000 ecoengine-1.6.2/src/ecoengine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.958510 ecoengine-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-23 23:51:43.000000 ecoengine-1.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-23 23:53:32.958510 ecoengine-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-23 23:51:43.000000 ecoengine-1.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-23 23:51:43.000000 ecoengine-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 23:53:32.958510 ecoengine-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 23:51:43.000000 ecoengine-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.866510 ecoengine-1.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.866510 ecoengine-1.6.3/src/ecoengine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.870509 ecoengine-1.6.3/src/ecoengine/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/constants/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.870509 ecoengine-1.6.3/src/ecoengine/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.874509 ecoengine-1.6.3/src/ecoengine/data/climate_data/
+-rw-r--r--   0 runner    (1001) docker     (127)  3784790 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/climate_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1728735 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.878509 ecoengine-1.6.3/src/ecoengine/data/load_shapes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/apartment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/elementary_school.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/food_service_a.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/food_service_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/junior_high.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/mens_dorm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/motel.json
+-rw-r--r--   0 runner    (1001) docker     (127)   262011 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/multi_family.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/nursing_home.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/office_building.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/senior_high.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/load_shapes/womens_dorm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.878509 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58109 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/maps.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.954510 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19141 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374730 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19445 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387706 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   370550 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18191 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   353846 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19680 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   387526 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364494 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383718 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   376446 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   373434 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19737 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   383822 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18589 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   364226 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18505 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   358582 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   374554 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   368874 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    17837 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   349178 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   399586 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18580 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   365854 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   390254 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18932 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   372098 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   356322 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   354146 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    18022 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   359030 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21000 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   411666 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   414014 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   121180 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   424354 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.958510 ecoengine-1.6.3/src/ecoengine/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/engine/BuildingCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44309 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/engine/EcosizerEngine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/engine/Simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/engine/SystemCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.958510 ecoengine-1.6.3/src/ecoengine/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/Building.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30767 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/PrefMapTracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34828 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/SimulationRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48946 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/SystemConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/UtilityCostTracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systemConfigUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.958510 ecoengine-1.6.3/src/ecoengine/objects/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/MultiPass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/MultiPassRecirc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/ParallelLoopTank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/PrimaryWithRecirc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26558 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/SwingTank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/SwingTankER.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:51:43.000000 ecoengine-1.6.3/src/ecoengine/objects/systems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:53:32.958510 ecoengine-1.6.3/src/ecoengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-23 23:53:32.000000 ecoengine-1.6.3/src/ecoengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23016 2024-05-23 23:53:32.000000 ecoengine-1.6.3/src/ecoengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:53:32.000000 ecoengine-1.6.3/src/ecoengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 23:53:32.000000 ecoengine-1.6.3/src/ecoengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 23:53:32.000000 ecoengine-1.6.3/src/ecoengine.egg-info/top_level.txt
```

### Comparing `ecoengine-1.6.2/PKG-INFO` & `ecoengine-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 1.6.2
+Version: 1.6.3
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-1.6.2/README.md` & `ecoengine-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/setup.cfg` & `ecoengine-1.6.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecoengine
-version = 1.6.2
+version = 1.6.3
 author = Nolan
 author_email = nolan@ecotope.com
 description = A software for sizing Heat Pump Water Heaters for buildings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://ecosizer.ecotope.com/sizer/
 project_urls =
```

### Comparing `ecoengine-1.6.2/src/ecoengine/__init__.py` & `ecoengine-1.6.3/src/ecoengine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/constants/Constants.py` & `ecoengine-1.6.3/src/ecoengine/constants/Constants.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv` & `ecoengine-1.6.3/src/ecoengine/data/climate_data/DryBulbTemperatures_ByClimateZone.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv` & `ecoengine-1.6.3/src/ecoengine/data/climate_data/InletWaterTemperatures_ByClimateZone.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv` & `ecoengine-1.6.3/src/ecoengine/data/climate_data/WeatherStation_ClimateZone_Lookup.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv` & `ecoengine-1.6.3/src/ecoengine/data/climate_data/ZipCode_ClimateZone_Lookup.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv` & `ecoengine-1.6.3/src/ecoengine/data/climate_data/kGperkWh_ByClimateZone.csv`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/load_shapes/apartment.json` & `ecoengine-1.6.3/src/ecoengine/data/load_shapes/apartment.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/load_shapes/elementary_school.json` & `ecoengine-1.6.3/src/ecoengine/data/load_shapes/elementary_school.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/load_shapes/food_service_a.json` & `ecoengine-1.6.3/src/ecoengine/data/load_shapes/food_service_a.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/load_shapes/food_service_b.json` & `ecoengine-1.6.3/src/ecoengine/data/load_shapes/food_service_b.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/load_shapes/junior_high.json` & `ecoengine-1.6.3/src/ecoengine/data/load_shapes/junior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/load_shapes/mens_dorm.json` & `ecoengine-1.6.3/src/ecoengine/data/load_shapes/mens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/load_shapes/motel.json` & `ecoengine-1.6.3/src/ecoengine/data/load_shapes/motel.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/load_shapes/multi_family.json` & `ecoengine-1.6.3/src/ecoengine/data/load_shapes/multi_family.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/load_shapes/nursing_home.json` & `ecoengine-1.6.3/src/ecoengine/data/load_shapes/nursing_home.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/load_shapes/office_building.json` & `ecoengine-1.6.3/src/ecoengine/data/load_shapes/office_building.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/load_shapes/senior_high.json` & `ecoengine-1.6.3/src/ecoengine/data/load_shapes/senior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/load_shapes/womens_dorm.json` & `ecoengine-1.6.3/src/ecoengine/data/load_shapes/womens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/maps.json` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/maps.json`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA10_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_R513a_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA20_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA25_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Oversized_Condenser_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_R513a_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxA30_VFD_35_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_45_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV15_VFD_60_Hz_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_CxV5_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_R513a_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Colmac_HPA4_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Laars_eTherm_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Lync_Aegis_500_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Mitsubishi_QAHV_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C125A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C185A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C250A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C25A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C60A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_C90A_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_HT_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Nyle_e360_LT_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135HNU_483_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_135VNU_483_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60HNU_201_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/Rheem_HPHD_60VNU_201_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/SANCO2_GS4_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP140_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP200_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP280_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP350_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Multi_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lochinvar_AHP60_Single_Pass_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a250_simulated_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a350_simulated_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_bounds.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_capacity_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl` & `ecoengine-1.6.3/src/ecoengine/data/preformanceMaps/pkls/lync_a500_simulated_power_in_interpolator.pkl`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/engine/BuildingCreator.py` & `ecoengine-1.6.3/src/ecoengine/engine/BuildingCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/engine/EcosizerEngine.py` & `ecoengine-1.6.3/src/ecoengine/engine/EcosizerEngine.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/engine/Simulator.py` & `ecoengine-1.6.3/src/ecoengine/engine/Simulator.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,14 +64,17 @@
                             simRun.addTMCap(system.getTMOutputCapacity(kW=True), system.getTMInputCapacity(kW=True))
                             kGofCO2 += simRun.getTMCapIn(i)*(simRun.tmRun[i]/60)
                         if building.isInCalifornia():
                             kGofCO2 *= float(kG_row[building.climateZone-1])
                             simRun.addKGCO2(kGofCO2)   
                     else:
                         system.runOneSystemStep(simRun, i, minuteIntervals = minuteIntervals)
+                        simRun.addCap(system.getOutputCapacity(kW=True), system.getInputCapacity(kW=True))
+                        if(hasattr(simRun, 'tmRun')):
+                            simRun.addTMCap(system.getTMOutputCapacity(kW=True), system.getTMInputCapacity(kW=True))
             
             except Exception as e:
                 if not exceptOnWaterShortage and (str(e) == "Primary storage ran out of Volume!" or str(e) == "The swing tank dropped below the supply temperature! The system is undersized"):
                     print(f"{str(e)} Returning simulation result for analysis.")
                 else:
                     raise
```

### Comparing `ecoengine-1.6.2/src/ecoengine/engine/SystemCreator.py` & `ecoengine-1.6.3/src/ecoengine/engine/SystemCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/engine/__init__.py` & `ecoengine-1.6.3/src/ecoengine/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/objects/Building.py` & `ecoengine-1.6.3/src/ecoengine/objects/Building.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/objects/PrefMapTracker.py` & `ecoengine-1.6.3/src/ecoengine/objects/PrefMapTracker.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/objects/SimulationRun.py` & `ecoengine-1.6.3/src/ecoengine/objects/SimulationRun.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,43 +58,43 @@
 
     def passedCOPAssumptionThreshold(self, times_COP_assumed : int):
         """
         returns True if COP has been assumed more times than the threshold. False Otherwise.
         """
         return times_COP_assumed > self.copAssumeThreshold
 
-    def initializeTMValue(self, initST, storageT_F, TMCap_kBTUhr, swingOut = True):
+    def initializeTMValue(self, initST, supplyT_F, TMCap_kBTUhr, swingOut = True):
         """
         Initializes temperature maintenance values
 
         Parameters
         ----------
         initST : float
             temperature maintenance tank temperature at start of the simulation.
-        storageT_F : float
+        supplyT_F : float
             storage temperature setpoint for temperature maintenance system
         TMCap_kBTUhr : float
             temperature maintenance heating capacity in kBTUhr
         swingOut : boolean
             set to True for swing tank systems so that DHW leaving temperature maintenance system is recorded
         """
-        self.tmT_F = [0] * (len(self.hwDemand) - 1) + [storageT_F]
+        self.tmT_F = [0] * (len(self.hwDemand) - 1) + [supplyT_F]
         self.tmRun = [0] * (len(self.hwDemand))
         if swingOut:
             self.hw_outSwing = [0] * (len(self.hwDemand))
         # self.hw_outSwing[0] = self.hwDemand[0]
         if initST:
             self.tmT_F[-1] = initST
         self.tmheating = False
 
         self.tm_cap_out = [] # output tm capacity at every time interval
         self.tm_cap_in = [] # input tm capacity at every time interval
 
         # next two items are for the resulting plotly plot
-        self.storageT_F = storageT_F
+        self.TM_setpoint = supplyT_F
         self.TMCap_kBTUhr = TMCap_kBTUhr
 
     def getLoadShiftMode(self, i):
         """
         returns the load shifting setting at interval i of the simulation
 
         Parameters
@@ -718,15 +718,15 @@
 
         if any(i < 0 for i in V):
             raise Exception("Primary storage ran out of Volume!")
 
         fig = Figure()
 
         #swing tank
-        if hasattr(self, 'tmT_F') and hasattr(self, 'tmRun') and hasattr(self, 'TMCap_kBTUhr') and hasattr(self, 'storageT_F'):
+        if hasattr(self, 'tmT_F') and hasattr(self, 'tmRun') and hasattr(self, 'TMCap_kBTUhr') and hasattr(self, 'TM_setpoint'):
             fig = make_subplots(rows=2, cols=1,
                                 specs=[[{"secondary_y": False}],
                                         [{"secondary_y": True}]])
 
 
         # Do primary components
         x_data = list(range(len(V)))
@@ -753,15 +753,15 @@
         fig.update_layout(title="Hot Water Simulation",
                           xaxis_title= "Minute of Day",
                           yaxis_title="Gallons or\nGallons per Hour",
                           width=900,
                           height=700)
         
         # Swing tank
-        if hasattr(self, 'tmT_F') and hasattr(self, 'tmRun') and hasattr(self, 'TMCap_kBTUhr') and hasattr(self, 'storageT_F') and hasattr(self, 'hw_outSwing'):
+        if hasattr(self, 'tmT_F') and hasattr(self, 'tmRun') and hasattr(self, 'TMCap_kBTUhr') and hasattr(self, 'TM_setpoint') and hasattr(self, 'hw_outSwing'):
 
             # Do Swing Tank components:
             tmT_F = np.array(roundList(self.tmT_F,3)[-(60*hrind_fromback):])
             tmRun = np.array(roundList(self.tmRun,3)[-(60*hrind_fromback):]) * self.TMCap_kBTUhr/W_TO_BTUHR #tmRun is logical so convert to kW
 
             fig.add_trace(Scatter(x=x_data, y=tmT_F,
                                     name='Swing Tank Temperature',
@@ -775,15 +775,15 @@
                                     mode='lines', line_shape='hv',
                                     opacity=0.8, marker_color='goldenrod'),
                             row=2,col=1,
                             secondary_y=True)
 
             fig.update_yaxes(title_text="Swing Tank\nTemperature (\N{DEGREE SIGN}F)",
                                 showgrid=False, row=2, col=1,
-                                secondary_y=False, range=[self.building.supplyT_F-5, self.storageT_F])
+                                secondary_y=False, range=[self.building.supplyT_F-5, self.TM_setpoint + 30])
 
             fig.update_yaxes(title_text="Resistance Element\nOutput (kW)",
                                 showgrid=False, row=2, col=1,
                                 secondary_y=True, range=[0,np.ceil(max(tmRun)/10)*10])
 
         if return_as_div:
             plot_div = plot(fig, output_type='div', show_link=False, link_text="",
@@ -816,29 +816,32 @@
         ----------
         file_path : string
             the file path for the output csv file
         """
         
         hours = [(i // (60/self.minuteIntervals)) + 1 for i in range(len(self.getPrimaryVolume()))]
         column_names = ['Hour','Primary Volume (Gallons Storage Temp)', 'Primary Generation (Gallons Storage Temp)', 'HW Demand (Gallons Supply Temp)', 'Recirculation Loss to Primary System (Gallons Supply Temp)',
-                        'Theoretical HW Generation (Gallons Supply Temp)', 'Primary Run Time (Min)', 'OAT (F)', 'Input Capacity (kW)', 'Output Capacity (kW)', 'Primary COP']
+                        'Theoretical HW Generation (Gallons Supply Temp)', 'Primary Run Time (Min)', 'Input Capacity (kW)', 'Output Capacity (kW)', 'Primary COP']
         columns = [
             hours,
             self.getPrimaryVolume(),
             self.getPrimaryGeneration(),
             self.getHWDemand(),
             self.getRecircLoss(),
             self.getHWGeneration(),
             self.getPrimaryRun(),
-            self.getOAT(),
             self.getCapIn(),
             self.getCapOut(),
             self.getPrimaryCOP()
         ]
 
+        if len(self.oat) > 0:
+            column_names.append('OAT (F)')
+            columns.append(self.getOAT(),)
+
         if hasattr(self, 'tmRun'):
             column_names.append('TM Temp (F)')
             columns.append(self.getTMTemp())
             column_names.append('TM Runtime (Min)')
             columns.append(self.getTMRun())
             column_names.append('TM Input Capacity (kW)')
             columns.append(self.getTMCapIn())
```

### Comparing `ecoengine-1.6.2/src/ecoengine/objects/SystemConfig.py` & `ecoengine-1.6.3/src/ecoengine/objects/SystemConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
             hwDemand = np.array(hrTo15MinList(hwDemand)) / 4
             loadshiftSched = np.array(hrTo15MinList(loadshiftSched))
         elif minuteIntervals != 60:
             raise Exception("Invalid input given for granularity. Must be 1, 15, or 60.")
 
         pV = [0] * (len(hwDemand) - 1) + [V0_normal]
 
-        if initPV:
+        if initPV is not None:
             pV[-1] = initPV
         return SimulationRun(hwGenRate, hwDemand, V0_normal, pV, building, loadshiftSched, minuteIntervals, self.doLoadShift, LS_sched)
     
     def preSystemStepSetUp(self, simRun : SimulationRun, i, incomingWater_T, minuteIntervals, oat):
         """
         helper function for runOneSystemStep
         """
```

### Comparing `ecoengine-1.6.2/src/ecoengine/objects/UtilityCostTracker.py` & `ecoengine-1.6.3/src/ecoengine/objects/UtilityCostTracker.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/objects/__init__.py` & `ecoengine-1.6.3/src/ecoengine/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/objects/systemConfigUtils.py` & `ecoengine-1.6.3/src/ecoengine/objects/systemConfigUtils.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/objects/systems/MultiPass.py` & `ecoengine-1.6.3/src/ecoengine/objects/systems/MultiPass.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/objects/systems/MultiPassRecirc.py` & `ecoengine-1.6.3/src/ecoengine/objects/systems/MultiPassRecirc.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/objects/systems/ParallelLoopTank.py` & `ecoengine-1.6.3/src/ecoengine/objects/systems/ParallelLoopTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/objects/systems/PrimaryWithRecirc.py` & `ecoengine-1.6.3/src/ecoengine/objects/systems/PrimaryWithRecirc.py`

 * *Files identical despite different names*

### Comparing `ecoengine-1.6.2/src/ecoengine/objects/systems/SwingTank.py` & `ecoengine-1.6.3/src/ecoengine/objects/systems/SwingTank.py`

 * *Files 1% similar despite different names*

```diff
@@ -474,15 +474,15 @@
                 heatCap = LUheatCap
                 genRate = LUgenRate
             
         return heatCap, genRate
     
     def getInitializedSimulation(self, building : Building, initPV=None, initST=None, minuteIntervals = 1, nDays = 3, forcePeakyLoadshape = False) -> SimulationRun:
         simRun = super().getInitializedSimulation(building, initPV, initST, minuteIntervals, nDays, forcePeakyLoadshape)
-        simRun.initializeTMValue(initST, self.storageT_F, self.TMCap_kBTUhr)
+        simRun.initializeTMValue(initST, building.supplyT_F, self.TMCap_kBTUhr)
         return simRun
 
     def runOneSystemStep(self, simRun : SimulationRun, i, minuteIntervals = 1, oat = None, erCalc = False):
         incomingWater_T = simRun.getIncomingWaterT(i)
         self.preSystemStepSetUp(simRun, i, incomingWater_T + 15.0, minuteIntervals, oat) # CHPWH IWT is assumed 15°F (adjustable) warmer than DCW temperature on average, based on lab test data. 
             
         # aquire draw amount for time step
```

### Comparing `ecoengine-1.6.2/src/ecoengine/objects/systems/SwingTankER.py` & `ecoengine-1.6.3/src/ecoengine/objects/systems/SwingTankER.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,49 +42,30 @@
         # create a temporary performance map that will return ONLY that output capacity values for the sizing simulation
         perfMap_holder = self.perfMap # Store existing performance map in a temporary variable
         self.perfMap = PrefMapTracker(output_kBTUhr, usePkl=False, kBTUhr = True) # create simple performance map that only uses default output capacity
         self.setCapacity(self.perfMap.getDefaultCapacity())
         self.setLoadUPVolumeAndTrigger(building.getDesignInlet())
 
         # start the 72-hour sizing simulation to find HW deficit. Starting with the primary storage tank almost empty to ensure that water runs out if system is undersized.
-        simRun = self.getInitializedSimulation(building, initPV = 0.1, initST=building.supplyT_F, minuteIntervals = minuteIntervals, nDays = 3, forcePeakyLoadshape = True)
+        simRun_empty = self.getInitializedSimulation(building, initPV = 0, initST=building.supplyT_F, minuteIntervals = minuteIntervals, nDays = 2, forcePeakyLoadshape = True)
+        simRun_full = self.getInitializedSimulation(building, initPV = None, initST=building.supplyT_F, minuteIntervals = minuteIntervals, nDays = 2, forcePeakyLoadshape = True)
         i = 0
-        normalFunction = True
-        swingV = [0]*len(simRun.hwDemand)
-        waterDeficit = [0]*len(simRun.hwDemand)
-        while i < len(simRun.hwDemand):
-            if normalFunction:
-                i = self._findNextIndexOfHWDeficit(simRun, i)
-                if i < len(simRun.hwDemand):
-                    normalFunction = False
-            else:
-                # get available supply temperature volume in system to simulate as though water is completely stratified swing tank
-                swingV[i-1] = convertVolume(self.TMVol_G, building.supplyT_F, building.getDesignInlet(), simRun.tmT_F[i-1]) + \
-                    convertVolume(simRun.pV[i-1], building.supplyT_F, building.getDesignInlet(), self.storageT_F)
-                # get full hwGeneration rate of swing tank plus hw coming in from primary system
-                fullHWGenRate = (1000 * self.original_TMCap_kBTUhr / (60/minuteIntervals) /rhoCp / (building.supplyT_F - building.getDesignInlet()) * self.defrostFactor) + \
-                    simRun.hwGenRate
-                recircLossAtTime = (building.recirc_loss / (rhoCp * (building.supplyT_F - building.getDesignInlet()))) / (60/minuteIntervals)
-                while i < len(simRun.hwDemand) and not normalFunction:
-                    waterLeavingSystem = simRun.hwDemand[i] + recircLossAtTime
-                    if convertVolume(simRun.hwGenRate, self.storageT_F, building.getDesignInlet(), building.supplyT_F) >= simRun.hwDemand[i]:
-                        simRun.pV[i-1] = 0
-                        if swingV[i-1] <= self.TMVol_G:
-                            # Once appropriatly sized, water should never dip below supply temp so correct to supply temp once deficit is no longer an issue
-                            simRun.tmT_F[i-1] = building.supplyT_F
-                        else:
-                            simRun.tmT_F[i-1] =  ((swingV[i-1] * (building.supplyT_F - building.getDesignInlet()))/self.TMVol_G) + building.getDesignInlet()
-                        normalFunction = True
-                    else:
-                        swingV[i] = swingV[i-1] + fullHWGenRate - waterLeavingSystem
-                        waterDeficit[i] = max(waterLeavingSystem - fullHWGenRate, 0) # add water deficit if positive
-                        i += 1
-        # add additional ER to compensate for undersized CHPWH
-        self.TMCap_kBTUhr = self.original_TMCap_kBTUhr + (((max(waterDeficit) * (60/minuteIntervals) * rhoCp * (building.supplyT_F - building.getDesignInlet())) / 1000.) * saftey_factor)
+        tempDeficit = [0]*len(simRun_empty.hwDemand)
+        while i < len(simRun_empty.hwDemand):
+            self.runOneSystemStep(simRun_empty, i, minuteIntervals = minuteIntervals, oat = None, erCalc=True)
+            self.runOneSystemStep(simRun_full, i, minuteIntervals = minuteIntervals, oat = None, erCalc=True)
+            if simRun_empty.tmT_F[i] < building.supplyT_F:
+                tempDeficit[i] = simRun_empty.building.supplyT_F - simRun_empty.tmT_F[i]
+                simRun_empty.tmT_F[i] = building.supplyT_F
+            if simRun_full.tmT_F[i] < building.supplyT_F:
+                tempDeficit[i] = max(simRun_full.building.supplyT_F - simRun_full.tmT_F[i], tempDeficit[i])
+                simRun_full.tmT_F[i] = building.supplyT_F
+            i = i + 1
 
+        self.TMCap_kBTUhr = self.original_TMCap_kBTUhr + (((self.TMVol_G * (60/minuteIntervals) * rhoCp * (max(tempDeficit))) / 1000.) * saftey_factor)
         # set performance map back to its original form
         self.perfMap = perfMap_holder
         self.resetToDefaultCapacity()
         return self.TMCap_kBTUhr
 
     def _findNextIndexOfHWDeficit(self, simRun : SimulationRun, i):
         incomingWater_T = simRun.building.getDesignInlet()
@@ -118,18 +99,18 @@
         simRun.hw_outSwing[i] = convertVolume(simRun.hwDemand[i], last_temp, incomingWater_T, simRun.building.supplyT_F)
         #Get the generation rate in storage temp
         mixedGHW = convertVolume(simRun.hwGenRate, self.storageT_F, incomingWater_T, simRun.building.supplyT_F)
         if simRun.hw_outSwing[i] > simRun.pV[i-1] + mixedGHW:
             hwVol_G = simRun.pV[i-1] + mixedGHW
             mixedT_F = getMixedTemp(incomingWater_T, self.storageT_F, simRun.hw_outSwing[i] - hwVol_G, hwVol_G)
             simRun.tmheating, simRun.tmT_F[i], simRun.tmRun[i] = self._runOneSwingStep(simRun.building, 
-                simRun.tmheating, last_temp, simRun.hw_outSwing[i], mixedT_F, minuteIntervals = minuteIntervals)#, erCalc=True)
+                simRun.tmheating, last_temp, simRun.hw_outSwing[i], mixedT_F, minuteIntervals = minuteIntervals, erCalc=erCalc)
         else:
             simRun.tmheating, simRun.tmT_F[i], simRun.tmRun[i] = self._runOneSwingStep(simRun.building, 
-                simRun.tmheating, last_temp, simRun.hw_outSwing[i], self.storageT_F, minuteIntervals = minuteIntervals)#, erCalc=True)
+                simRun.tmheating, last_temp, simRun.hw_outSwing[i], self.storageT_F, minuteIntervals = minuteIntervals, erCalc=erCalc)
 
         simRun.pheating, simRun.pV[i], simRun.pGen[i], simRun.pRun[i] = self.runOnePrimaryStep(pheating = simRun.pheating,
                                                                                                 Vcurr = simRun.pV[i-1], 
                                                                                                 hw_out = simRun.hw_outSwing[i], 
                                                                                                 hw_in = mixedGHW, 
                                                                                                 mode = simRun.getLoadShiftMode(i),
                                                                                                 modeChanged = (simRun.getLoadShiftMode(i) != simRun.getLoadShiftMode(i-1)),
@@ -173,20 +154,24 @@
         while self.TMCap_kBTUhr > self.original_TMCap_kBTUhr and i > 0: # stopping point is normal sizing point
             if i == 100:
                 startind = len(fract_covered)
                 er_cap_kBTUhr = original_erSize_kBTUhr
             else:
                 fract = i/100.
                 building.magnitude = original_magnitude * fract
-                er_cap_kBTUhr = self.sizeERElement(building, additionalERSaftey, 15)
+                er_cap_kBTUhr = self.sizeERElement(building, additionalERSaftey, 1)
             er_cap_kW.append(round(er_cap_kBTUhr/W_TO_BTUHR,0))
             fract_covered.append(i)
             i -= 10
 
-        # except Exception:
+        # reverse the lists because they are backwards:
+        # fract_covered.reverse()
+        # er_cap_kW.reverse()
+        # startind = (len(fract_covered)-1)-startind
+
         building.magnitude = original_magnitude
         self.TMCap_kBTUhr = original_erSize_kBTUhr
         return [er_cap_kW, fract_covered, startind] # TODO edge cases around start index
     
     
     def getERCurveAndSlider(self, x, y, startind, returnAsDiv = True):
         """
```

### Comparing `ecoengine-1.6.2/src/ecoengine.egg-info/PKG-INFO` & `ecoengine-1.6.3/src/ecoengine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 1.6.2
+Version: 1.6.3
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-1.6.2/src/ecoengine.egg-info/SOURCES.txt` & `ecoengine-1.6.3/src/ecoengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

