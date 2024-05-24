# Comparing `tmp/foxes-0.7.0.6.tar.gz` & `tmp/foxes-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxes-0.7.0.6.tar", last modified: Wed May  8 17:21:29 2024, max compression
+gzip compressed data, was "foxes-0.7.1.tar", last modified: Fri May 24 09:03:02 2024, max compression
```

## Comparing `foxes-0.7.0.6.tar` & `foxes-0.7.1.tar`

### file list

```diff
@@ -1,314 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.961060 foxes-0.7.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-08 17:21:26.000000 foxes-0.7.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40774 2024-05-08 17:21:26.000000 foxes-0.7.0.6/Logo_FOXES.svg
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-08 17:21:26.000000 foxes-0.7.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-08 17:21:29.961060 foxes-0.7.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-08 17:21:26.000000 foxes-0.7.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.909060 foxes-0.7.0.6/foxes/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.913060 foxes-0.7.0.6/foxes/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.913060 foxes-0.7.0.6/foxes/algorithms/downwind/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/downwind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21612 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/downwind/downwind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.913060 foxes-0.7.0.6/foxes/algorithms/downwind/models/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/downwind/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/downwind/models/farm_wakes_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/downwind/models/init_farm_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/downwind/models/point_wakes_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/downwind/models/reorder_farm_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/downwind/models/set_amb_farm_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/downwind/models/set_amb_point_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.913060 foxes-0.7.0.6/foxes/algorithms/iterative/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/iterative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/iterative/iterative.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.917060 foxes-0.7.0.6/foxes/algorithms/iterative/models/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/iterative/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/iterative/models/convergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/iterative/models/farm_wakes_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/iterative/models/urelax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.917060 foxes-0.7.0.6/foxes/algorithms/sequential/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/sequential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.917060 foxes-0.7.0.6/foxes/algorithms/sequential/models/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/sequential/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/sequential/models/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/sequential/models/seq_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/algorithms/sequential/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.921060 foxes-0.7.0.6/foxes/core/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15169 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/axial_induction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14581 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/data_calc_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/farm_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/farm_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/farm_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/partial_wakes_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/point_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/rotor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/turbine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/turbine_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/turbine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/vertical_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/wake_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/wake_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/wake_superposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/core/wind_farm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.921060 foxes-0.7.0.6/foxes/data/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.921060 foxes-0.7.0.6/foxes/data/farms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/farms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/farms/test_farm_67.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.921060 foxes-0.7.0.6/foxes/data/power_ct_curves/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/power_ct_curves/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.925060 foxes-0.7.0.6/foxes/data/states/
--rw-r--r--   0 runner    (1001) docker     (127)   427815 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/states/WRF-Timeseries-4464.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   126124 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/states/abl_states_6000.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/states/timeseries_100.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/states/timeseries_3000.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    78694 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/states/timeseries_8000.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/states/wind_rose_bremen.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/states/wind_rotation.nc
--rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/states/winds100.tab
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/data/static_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.925060 foxes-0.7.0.6/foxes/input/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.925060 foxes-0.7.0.6/foxes/input/farm_layout/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/farm_layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/farm_layout/from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/farm_layout/from_df.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/farm_layout/from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/farm_layout/from_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/farm_layout/from_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/farm_layout/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/farm_layout/row.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.929060 foxes-0.7.0.6/foxes/input/states/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.929060 foxes-0.7.0.6/foxes/input/states/create/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/states/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/states/create/random_abl_states.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/states/create/random_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)    18693 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/states/field_data_nc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/states/multi_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/states/scan_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/states/single.py
--rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/states/states_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.929060 foxes-0.7.0.6/foxes/input/windio/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/windio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/input/windio/windio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.929060 foxes-0.7.0.6/foxes/models/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.929060 foxes-0.7.0.6/foxes/models/axial_induction_models/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/axial_induction_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/axial_induction_models/betz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/axial_induction_models/madsen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.929060 foxes-0.7.0.6/foxes/models/farm_controllers/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/farm_controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/farm_controllers/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.929060 foxes-0.7.0.6/foxes/models/farm_models/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/farm_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/farm_models/turbine2farm.py
--rw-r--r--   0 runner    (1001) docker     (127)    21372 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/model_book.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.933060 foxes-0.7.0.6/foxes/models/partial_wakes/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/partial_wakes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/partial_wakes/axiwake.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/partial_wakes/centre.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/partial_wakes/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/partial_wakes/rotor_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/partial_wakes/segregated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/partial_wakes/top_hat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.933060 foxes-0.7.0.6/foxes/models/point_models/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/point_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/point_models/set_uniform_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/point_models/tke2ti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/point_models/wake_deltas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.933060 foxes-0.7.0.6/foxes/models/rotor_models/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/rotor_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/rotor_models/centre.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/rotor_models/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/rotor_models/levels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.933060 foxes-0.7.0.6/foxes/models/turbine_models/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_models/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_models/kTI_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_models/lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_models/power_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_models/rotor_centre_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_models/sector_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_models/set_farm_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_models/table_factors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_models/thrust2ct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_models/yaw2yawm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_models/yawm2yaw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.937060 foxes-0.7.0.6/foxes/models/turbine_types/
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_types/CpCt_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_types/CpCt_from_two.py
--rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_types/PCt_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_types/PCt_from_two.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_types/null_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11143 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_types/wsrho2PCt_from_two.py
--rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/turbine_types/wsti2PCt_from_two.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.937060 foxes-0.7.0.6/foxes/models/vertical_profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/vertical_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/vertical_profiles/abl_log_neutral_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/vertical_profiles/abl_log_stable_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/vertical_profiles/abl_log_unstable_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/vertical_profiles/abl_log_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/vertical_profiles/data_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/vertical_profiles/sheared_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/vertical_profiles/uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.937060 foxes-0.7.0.6/foxes/models/wake_frames/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_frames/farm_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_frames/rotor_wd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_frames/seq_dynamic_wakes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_frames/streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_frames/timelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_frames/yawed_wakes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.941060 foxes-0.7.0.6/foxes/models/wake_models/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/axisymmetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/dist_sliced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.941060 foxes-0.7.0.6/foxes/models/wake_models/induction/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/induction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/induction/rankine_half_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/induction/rathmann.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/induction/self_similar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/induction/self_similar2020.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.941060 foxes-0.7.0.6/foxes/models/wake_models/ti/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/ti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/ti/crespo_hernandez.py
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/ti/iec_ti.py
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/top_hat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/wake_mirror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.941060 foxes-0.7.0.6/foxes/models/wake_models/wind/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/wind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/wind/bastankhah14.py
--rw-r--r--   0 runner    (1001) docker     (127)    17629 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/wind/bastankhah16.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/wind/jensen.py
--rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_models/wind/turbopark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.945060 foxes-0.7.0.6/foxes/models/wake_superpositions/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_superpositions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_superpositions/ti_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_superpositions/ti_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_superpositions/ti_pow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_superpositions/ti_quadratic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_superpositions/ws_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_superpositions/ws_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_superpositions/ws_pow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_superpositions/ws_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/models/wake_superpositions/ws_quadratic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.945060 foxes-0.7.0.6/foxes/opt/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.945060 foxes-0.7.0.6/foxes/opt/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/constraints/area_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/constraints/min_dist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.945060 foxes-0.7.0.6/foxes/opt/core/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/core/farm_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/core/farm_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/core/farm_opt_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/core/farm_vars_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/core/pop_states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.945060 foxes-0.7.0.6/foxes/opt/objectives/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/objectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/objectives/farm_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/objectives/max_n_turbines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.945060 foxes-0.7.0.6/foxes/opt/problems/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/problems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.945060 foxes-0.7.0.6/foxes/opt/problems/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/problems/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/problems/layout/farm_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.949060 foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/geom_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
--rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/problems/layout/reggrids_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/problems/layout/regular_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    19425 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/opt/problems/opt_farm_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.949060 foxes-0.7.0.6/foxes/output/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/calc_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/farm_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    17663 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/farm_results_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.953060 foxes-0.7.0.6/foxes/output/flow_plots_2d/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/flow_plots_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/flow_plots_2d/flow_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/flow_plots_2d/get_fig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/flow_plots_2d/seq_flow_ani_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/flow_plots_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/results_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/rose_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/rotor_point_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/round.py
--rw-r--r--   0 runner    (1001) docker     (127)    31519 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/slice_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/state_turbine_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/output/turbine_type_curves.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.953060 foxes-0.7.0.6/foxes/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.957060 foxes-0.7.0.6/foxes/utils/abl/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/abl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/abl/neutral.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/abl/sheared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/abl/stable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/abl/unstable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/cubic_roots.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/data_book.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/exec_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.957060 foxes-0.7.0.6/foxes/utils/geom2d/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/geom2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19120 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/geom2d/area_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/geom2d/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/geom2d/example_intersection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/geom2d/example_union.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/geom2d/half_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/geom2d/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/geopandas_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/geopandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/pandas_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/random_xy.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/regularize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.957060 foxes-0.7.0.6/foxes/utils/runners/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/runners/runners.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/subclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/tab_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/two_circles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/wind_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/windrose_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/utils/xarray_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-08 17:21:26.000000 foxes-0.7.0.6/foxes/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:21:29.957060 foxes-0.7.0.6/foxes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-08 17:21:29.000000 foxes-0.7.0.6/foxes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-05-08 17:21:29.000000 foxes-0.7.0.6/foxes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:21:29.000000 foxes-0.7.0.6/foxes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-08 17:21:29.000000 foxes-0.7.0.6/foxes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 17:21:29.000000 foxes-0.7.0.6/foxes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:21:29.000000 foxes-0.7.0.6/foxes.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-08 17:21:26.000000 foxes-0.7.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-08 17:21:29.961060 foxes-0.7.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 17:21:26.000000 foxes-0.7.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.682548 foxes-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 09:02:58.000000 foxes-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40774 2024-05-24 09:02:58.000000 foxes-0.7.1/Logo_FOXES.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-24 09:02:58.000000 foxes-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-05-24 09:03:02.682548 foxes-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-24 09:02:58.000000 foxes-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.638548 foxes-0.7.1/foxes/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.638548 foxes-0.7.1/foxes/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.638548 foxes-0.7.1/foxes/algorithms/downwind/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21652 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/downwind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.642548 foxes-0.7.1/foxes/algorithms/downwind/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/farm_wakes_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/init_farm_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/point_wakes_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/reorder_farm_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/set_amb_farm_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/set_amb_point_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.642548 foxes-0.7.1/foxes/algorithms/iterative/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/iterative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/iterative/iterative.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.642548 foxes-0.7.1/foxes/algorithms/iterative/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/iterative/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/iterative/models/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/iterative/models/farm_wakes_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/iterative/models/urelax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.642548 foxes-0.7.1/foxes/algorithms/sequential/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/sequential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.642548 foxes-0.7.1/foxes/algorithms/sequential/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/sequential/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/sequential/models/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/sequential/models/seq_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/sequential/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.646548 foxes-0.7.1/foxes/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15169 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/axial_induction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14581 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/data_calc_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/farm_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/farm_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/farm_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/partial_wakes_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/point_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/rotor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/turbine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/turbine_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/turbine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/vertical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/wake_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/wake_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/wake_superposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/wind_farm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.646548 foxes-0.7.1/foxes/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.646548 foxes-0.7.1/foxes/data/farms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/farms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/farms/test_farm_67.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.650548 foxes-0.7.1/foxes/data/power_ct_curves/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/power_ct_curves/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.650548 foxes-0.7.1/foxes/data/states/
+-rw-r--r--   0 runner    (1001) docker     (127)   427815 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/WRF-Timeseries-4464.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126124 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/abl_states_6000.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/timeseries_100.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/timeseries_3000.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    78694 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/timeseries_8000.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/wind_rose_bremen.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/wind_rotation.nc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/winds100.tab
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/static_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.650548 foxes-0.7.1/foxes/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/input/farm_layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/from_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/from_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/from_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/row.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/input/states/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/input/states/create/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/create/random_abl_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/create/random_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18693 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/field_data_nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/multi_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/scan_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/single.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/states_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/input/windio/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/windio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/windio/windio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/models/axial_induction_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/axial_induction_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/axial_induction_models/betz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/axial_induction_models/madsen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/models/farm_controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/farm_controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/farm_controllers/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/models/farm_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/farm_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/farm_models/turbine2farm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26376 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/model_book.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.658548 foxes-0.7.1/foxes/models/partial_wakes/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/axiwake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/centre.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/rotor_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/segregated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/top_hat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.658548 foxes-0.7.1/foxes/models/point_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/point_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/point_models/set_uniform_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/point_models/tke2ti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/point_models/wake_deltas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.658548 foxes-0.7.1/foxes/models/rotor_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/rotor_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/rotor_models/centre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/rotor_models/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/rotor_models/levels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.658548 foxes-0.7.1/foxes/models/turbine_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/kTI_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/power_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/rotor_centre_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/sector_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/set_farm_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/table_factors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/thrust2ct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/yaw2yawm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/yawm2yaw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.662548 foxes-0.7.1/foxes/models/turbine_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/CpCt_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/CpCt_from_two.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/PCt_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/PCt_from_two.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/null_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11143 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/wsrho2PCt_from_two.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/wsti2PCt_from_two.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.662548 foxes-0.7.1/foxes/models/vertical_profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/abl_log_neutral_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/abl_log_stable_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/abl_log_unstable_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/abl_log_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/data_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/sheared_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.662548 foxes-0.7.1/foxes/models/wake_frames/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/farm_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/rotor_wd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/seq_dynamic_wakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/timelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/yawed_wakes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.666548 foxes-0.7.1/foxes/models/wake_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/axisymmetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/dist_sliced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.666548 foxes-0.7.1/foxes/models/wake_models/induction/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/induction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/induction/rankine_half_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/induction/rathmann.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/induction/self_similar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/induction/self_similar2020.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.666548 foxes-0.7.1/foxes/models/wake_models/ti/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/ti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/ti/crespo_hernandez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/ti/iec_ti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/top_hat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/wake_mirror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.666548 foxes-0.7.1/foxes/models/wake_models/wind/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/wind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/wind/bastankhah14.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17629 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/wind/bastankhah16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/wind/jensen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/wind/turbopark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.666548 foxes-0.7.1/foxes/models/wake_superpositions/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ti_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ti_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ti_pow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ti_quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ws_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ws_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ws_pow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ws_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ws_quadratic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.670548 foxes-0.7.1/foxes/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.670548 foxes-0.7.1/foxes/opt/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/constraints/area_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/constraints/min_dist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.670548 foxes-0.7.1/foxes/opt/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/core/farm_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/core/farm_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/core/farm_opt_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/core/farm_vars_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/core/pop_states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.670548 foxes-0.7.1/foxes/opt/objectives/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/objectives/farm_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/objectives/max_n_turbines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.670548 foxes-0.7.1/foxes/opt/problems/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.670548 foxes-0.7.1/foxes/opt/problems/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/farm_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.674548 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/reggrids_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/regular_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19425 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/opt_farm_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.674548 foxes-0.7.1/foxes/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/calc_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/farm_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17663 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/farm_results_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.674548 foxes-0.7.1/foxes/output/flow_plots_2d/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/flow_plots_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/flow_plots_2d/flow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/flow_plots_2d/get_fig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/flow_plots_2d/seq_flow_ani_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/flow_plots_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/results_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/rose_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/rotor_point_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/round.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31519 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/slice_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/state_turbine_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/turbine_type_curves.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.678548 foxes-0.7.1/foxes/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.678548 foxes-0.7.1/foxes/utils/abl/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/abl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/abl/neutral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/abl/sheared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/abl/stable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/abl/unstable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/cubic_roots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/data_book.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/exec_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.682548 foxes-0.7.1/foxes/utils/geom2d/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19120 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/area_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/example_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/example_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/half_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geopandas_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geopandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/pandas_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/random_xy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/regularize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.682548 foxes-0.7.1/foxes/utils/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/runners/runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/tab_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/two_circles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/wind_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/windrose_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/xarray_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.682548 foxes-0.7.1/foxes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-05-24 09:03:02.000000 foxes-0.7.1/foxes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-05-24 09:03:02.000000 foxes-0.7.1/foxes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:03:02.000000 foxes-0.7.1/foxes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-24 09:03:02.000000 foxes-0.7.1/foxes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 09:03:02.000000 foxes-0.7.1/foxes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:03:02.000000 foxes-0.7.1/foxes.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-24 09:02:58.000000 foxes-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-24 09:03:02.682548 foxes-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 09:02:58.000000 foxes-0.7.1/setup.py
```

### Comparing `foxes-0.7.0.6/LICENSE` & `foxes-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/Logo_FOXES.svg` & `foxes-0.7.1/Logo_FOXES.svg`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/PKG-INFO` & `foxes-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.7.0.6
+Version: 0.7.1
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
```

### Comparing `foxes-0.7.0.6/README.md` & `foxes-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/__init__.py` & `foxes-0.7.1/foxes/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/algorithms/downwind/downwind.py` & `foxes-0.7.1/foxes/algorithms/downwind/downwind.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,25 +213,25 @@
             print(f"  states   : {self.states}")
             print(f"  rotor    : {self.rotor_model}")
             print(f"  controller: {self.farm_controller}")
             print(f"  wake frame: {self.wake_frame}")
             print(deco)
             print(f"  wakes:")
             for i, w in enumerate(self.wake_models.values()):
-                print(f"    {i}) {w}")
+                print(f"    {i}) {w.name}: {w}")
             print(deco)
             print(f"  partial wakes:")
             for i, (w, p) in enumerate(self.partial_wakes.items()):
-                print(f"    {i}) {w}: {p}")
+                print(f"    {i}) {w}: {p.name}, {p}")
             print(deco)
             print(f"  turbine models:")
             for i, m in enumerate(self.farm_controller.pre_rotor_models.models):
-                print(f"    {i}) {m} [pre-rotor]")
+                print(f"    {i}) {m.name}: {m} [pre-rotor]")
             for i, m in enumerate(self.farm_controller.post_rotor_models.models):
-                print(f"    {i+len(self.farm_controller.pre_rotor_models.models)}) {m}")
+                print(f"    {i+len(self.farm_controller.pre_rotor_models.models)}) {m.name}: {m}")
             print(deco)
             print()
 
     def _print_model_oder(self, mlist, calc_pars):
         """
         Helper function for printing model names
         """
```

### Comparing `foxes-0.7.0.6/foxes/algorithms/downwind/models/farm_wakes_calc.py` & `foxes-0.7.1/foxes/algorithms/downwind/models/farm_wakes_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/algorithms/downwind/models/init_farm_data.py` & `foxes-0.7.1/foxes/algorithms/downwind/models/init_farm_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/algorithms/downwind/models/point_wakes_calc.py` & `foxes-0.7.1/foxes/algorithms/downwind/models/point_wakes_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/algorithms/downwind/models/reorder_farm_output.py` & `foxes-0.7.1/foxes/algorithms/downwind/models/reorder_farm_output.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/algorithms/downwind/models/set_amb_farm_results.py` & `foxes-0.7.1/foxes/algorithms/downwind/models/set_amb_farm_results.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/algorithms/downwind/models/set_amb_point_results.py` & `foxes-0.7.1/foxes/algorithms/downwind/models/set_amb_point_results.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/algorithms/iterative/iterative.py` & `foxes-0.7.1/foxes/algorithms/iterative/iterative.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/algorithms/iterative/models/convergence.py` & `foxes-0.7.1/foxes/algorithms/iterative/models/convergence.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/algorithms/iterative/models/farm_wakes_calc.py` & `foxes-0.7.1/foxes/algorithms/iterative/models/farm_wakes_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/algorithms/iterative/models/urelax.py` & `foxes-0.7.1/foxes/algorithms/iterative/models/urelax.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/algorithms/sequential/models/plugin.py` & `foxes-0.7.1/foxes/algorithms/sequential/models/plugin.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/algorithms/sequential/models/seq_state.py` & `foxes-0.7.1/foxes/algorithms/sequential/models/seq_state.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/algorithms/sequential/sequential.py` & `foxes-0.7.1/foxes/algorithms/sequential/sequential.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/constants.py` & `foxes-0.7.1/foxes/constants.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/__init__.py` & `foxes-0.7.1/foxes/core/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/algorithm.py` & `foxes-0.7.1/foxes/core/algorithm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/data.py` & `foxes-0.7.1/foxes/core/data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/data_calc_model.py` & `foxes-0.7.1/foxes/core/data_calc_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/farm_controller.py` & `foxes-0.7.1/foxes/core/farm_controller.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/farm_data_model.py` & `foxes-0.7.1/foxes/core/farm_data_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/model.py` & `foxes-0.7.1/foxes/core/model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/partial_wakes_model.py` & `foxes-0.7.1/foxes/core/partial_wakes_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/point_data_model.py` & `foxes-0.7.1/foxes/core/point_data_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/rotor_model.py` & `foxes-0.7.1/foxes/core/rotor_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/states.py` & `foxes-0.7.1/foxes/core/states.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/turbine.py` & `foxes-0.7.1/foxes/core/turbine.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/turbine_model.py` & `foxes-0.7.1/foxes/core/turbine_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/turbine_type.py` & `foxes-0.7.1/foxes/core/turbine_type.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/vertical_profile.py` & `foxes-0.7.1/foxes/core/vertical_profile.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/wake_frame.py` & `foxes-0.7.1/foxes/core/wake_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 from scipy.interpolate import interpn
 
 from foxes.utils import all_subclasses
 import foxes.constants as FC
 import foxes.variables as FV
 
-from .data import Data
+from .data import MData, FData, TData
 from .model import Model
 
 
 class WakeFrame(Model):
     """
     Abstract base class for wake frames.
 
@@ -33,17 +33,17 @@
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata: foxes.core.Data
+        mdata: foxes.core.MData
             The model data
-        fdata: foxes.core.Data
+        fdata: foxes.core.FData
             The farm data
 
         Returns
         -------
         order: numpy.ndarray
             The turbine order, shape: (n_states, n_turbines)
 
@@ -248,15 +248,15 @@
         n_ix = n_steps + 1
         xs = np.arange(xmin, xmin + n_ix * dx, dx)
         xpts = np.zeros((n_states, n_steps), dtype=FC.DTYPE)
         xpts[:] = xs[None, 1:]
         pts = self.get_centreline_points(algo, mdata, fdata, downwind_index, xpts)
 
         # run ambient calculation:
-        tdata = Data.from_points(
+        tdata = TData.from_points(
             pts,
             data={
                 v: np.full((n_states, n_steps, 1), np.nan, dtype=FC.DTYPE) for v in vrs
             },
             dims={v: (FC.STATE, FC.TARGET, FC.TPOINT) for v in vrs},
         )
         res = algo.states.calculate(algo, mdata, fdata, tdata)
```

### Comparing `foxes-0.7.0.6/foxes/core/wake_model.py` & `foxes-0.7.1/foxes/core/wake_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/wake_superposition.py` & `foxes-0.7.1/foxes/core/wake_superposition.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/core/wind_farm.py` & `foxes-0.7.1/foxes/core/wind_farm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/data/farms/test_farm_67.csv` & `foxes-0.7.1/foxes/data/farms/test_farm_67.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/data/parse.py` & `foxes-0.7.1/foxes/data/parse.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv` & `foxes-0.7.1/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/data/states/WRF-Timeseries-4464.csv.gz` & `foxes-0.7.1/foxes/data/states/WRF-Timeseries-4464.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/data/states/abl_states_6000.csv.gz` & `foxes-0.7.1/foxes/data/states/abl_states_6000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/data/states/timeseries_3000.csv.gz` & `foxes-0.7.1/foxes/data/states/timeseries_3000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/data/states/timeseries_8000.csv.gz` & `foxes-0.7.1/foxes/data/states/timeseries_8000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/data/states/wind_rose_bremen.csv` & `foxes-0.7.1/foxes/data/states/wind_rose_bremen.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/data/states/wind_rotation.nc` & `foxes-0.7.1/foxes/data/states/wind_rotation.nc`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/data/states/winds100.tab` & `foxes-0.7.1/foxes/data/states/winds100.tab`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/data/static_data.py` & `foxes-0.7.1/foxes/data/static_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/farm_layout/from_csv.py` & `foxes-0.7.1/foxes/input/farm_layout/from_csv.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/farm_layout/from_df.py` & `foxes-0.7.1/foxes/input/farm_layout/from_df.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/farm_layout/from_file.py` & `foxes-0.7.1/foxes/input/farm_layout/from_file.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/farm_layout/from_json.py` & `foxes-0.7.1/foxes/input/farm_layout/from_json.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/farm_layout/from_random.py` & `foxes-0.7.1/foxes/input/farm_layout/from_random.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/farm_layout/grid.py` & `foxes-0.7.1/foxes/input/farm_layout/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/farm_layout/row.py` & `foxes-0.7.1/foxes/input/farm_layout/row.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/states/create/random_abl_states.py` & `foxes-0.7.1/foxes/input/states/create/random_abl_states.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/states/create/random_timeseries.py` & `foxes-0.7.1/foxes/input/states/create/random_timeseries.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/states/field_data_nc.py` & `foxes-0.7.1/foxes/input/states/field_data_nc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/states/multi_height.py` & `foxes-0.7.1/foxes/input/states/multi_height.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/states/scan_ws.py` & `foxes-0.7.1/foxes/input/states/scan_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/states/single.py` & `foxes-0.7.1/foxes/input/states/single.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/states/states_table.py` & `foxes-0.7.1/foxes/input/states/states_table.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/input/windio/windio.py` & `foxes-0.7.1/foxes/input/windio/windio.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/axial_induction_models/betz.py` & `foxes-0.7.1/foxes/models/axial_induction_models/betz.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/axial_induction_models/madsen.py` & `foxes-0.7.1/foxes/models/axial_induction_models/madsen.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/farm_models/turbine2farm.py` & `foxes-0.7.1/foxes/models/farm_models/turbine2farm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/model_book.py` & `foxes-0.7.1/foxes/models/model_book.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from math import sqrt
 import foxes.models as fm
 import foxes.variables as FV
-from foxes.utils import Dict
+from foxes.utils import Dict, FDict
 
 from foxes.core import (
     PointDataModel,
     FarmDataModel,
     FarmController,
     RotorModel,
     TurbineType,
@@ -75,25 +76,54 @@
         Pct_file: str, optional
             Path to power/ct curve file, for creation
             of default turbine type model
         """
         self.point_models = Dict(name="point_models")
         self.point_models["tke2ti"] = fm.point_models.TKE2TI()
 
-        self.rotor_models = Dict(name="rotor_models")
+        self.rotor_models = FDict(name="rotor_models")
         rvars = [FV.REWS, FV.REWS2, FV.REWS3, FV.TI, FV.RHO]
         self.rotor_models["centre"] = fm.rotor_models.CentreRotor(calc_vars=rvars)
-        nlist = list(range(2, 11)) + [20]
-        for n in nlist:
-            self.rotor_models[f"grid{n**2}"] = fm.rotor_models.GridRotor(
-                calc_vars=rvars, n=n, reduce=True
-            )
-            self.rotor_models[f"level{n}"] = fm.rotor_models.LevelRotor(
-                calc_vars=rvars, n=n, reduce=True
-            )
+
+        def _n2n(n2):
+            n2 = float(n2)
+            n = int(sqrt(n2))
+            if n**2 != n2:
+                raise Exception(f"GridRotor factory: Value {n2} is not the square of an integer")
+            return n
+        self.rotor_models.add_factory(
+            fm.rotor_models.GridRotor,
+            "grid<n2>",
+            kwargs=dict(calc_vars=rvars, reduce=True),
+            var2arg={"n2": "n"},
+            n2=_n2n,
+            hints={"n2": "(Number of points in square grid)"},
+        )
+        self.rotor_models.add_factory(
+            fm.rotor_models.GridRotor,
+            "raw_grid<n2>",
+            kwargs=dict(calc_vars=rvars, reduce=False),
+            var2arg={"n2": "n"},
+            n2=_n2n,
+            hints={"n2": "(Number of points in square grid)"},
+        )
+        self.rotor_models.add_factory(
+            fm.rotor_models.LevelRotor,
+            "level<n>",
+            kwargs=dict(calc_vars=rvars, reduce=True),
+            n=lambda x: int(x),
+            hints={"n": "(Number of vertical levels)"},
+        )
+        self.rotor_models.add_factory(
+            fm.rotor_models.LevelRotor,
+            "raw_level<n>",
+            kwargs=dict(calc_vars=rvars, reduce=False),
+            n=lambda x: int(x),
+            hints={"n": "(Number of vertical levels)"},
+        )
 
         self.turbine_types = Dict(name="turbine_types")
         self.turbine_types["null_type"] = fm.turbine_types.NullType()
         self.turbine_types["NREL5MW"] = fm.turbine_types.PCtFile(
             "NREL-5MW-D126-H90.csv", rho=1.225
         )
         self.turbine_types["DTU10MW"] = fm.turbine_types.PCtFile(
@@ -104,29 +134,54 @@
         )
         self.turbine_types["IWT7.5MW"] = fm.turbine_types.PCtFile(
             "IWT-7d5MW-D164-H100.csv", rho=1.225
         )
         if Pct_file is not None:
             self.turbine_types["Pct"] = fm.turbine_types.PCtFile(Pct_file)
 
-        self.turbine_models = Dict(
+        self.turbine_models = FDict(
             name="turbine_models",
             kTI=fm.turbine_models.kTI(),
-            kTI_02=fm.turbine_models.kTI(kTI=0.2),
-            kTI_04=fm.turbine_models.kTI(kTI=0.4),
-            kTI_05=fm.turbine_models.kTI(kTI=0.5),
             kTI_amb=fm.turbine_models.kTI(ti_var=FV.AMB_TI),
-            kTI_amb_02=fm.turbine_models.kTI(ti_var=FV.AMB_TI, kTI=0.2),
-            kTI_amb_04=fm.turbine_models.kTI(ti_var=FV.AMB_TI, kTI=0.4),
-            kTI_amb_05=fm.turbine_models.kTI(ti_var=FV.AMB_TI, kTI=0.5),
             thrust2ct=fm.turbine_models.Thrust2Ct(),
             PMask=fm.turbine_models.PowerMask(),
             yaw2yawm=fm.turbine_models.YAW2YAWM(),
             yawm2yaw=fm.turbine_models.YAWM2YAW(),
         )
+        self.turbine_models.add_factory(
+            fm.turbine_models.kTI,
+            "kTI_<kTI>",
+            kTI=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"kTI": "(Value, e.g. 004 for 0.04)"},
+        )
+        self.turbine_models.add_factory(
+            fm.turbine_models.kTI,
+            "kTI_amb_<kTI>",
+            kwargs=dict(ti_var=FV.AMB_TI),
+            kTI=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"kTI": "(Value, e.g. 004 for 0.04)"},
+        )
+        self.turbine_models.add_factory(
+            fm.turbine_models.kTI,
+            "kTI_<kTI>_<kb>",
+            kTI=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            kb=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"kTI": "(Value, e.g. 004 for 0.04)",
+                   "kb": "(Value, e.g. 004 for 0.04)"},
+        )
+        self.turbine_models.add_factory(
+            fm.turbine_models.kTI,
+            "kTI_amb_<kTI>_<kb>",
+            kwargs=dict(ti_var=FV.AMB_TI),
+            kTI=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            kb=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"kTI": "(Value, e.g. 004 for 0.04)",
+                   "kb": "(Value, e.g. 004 for 0.04)"},
+        )
+
         self.turbine_models["hubh_data"] = fm.turbine_models.RotorCentreCalc(
             {
                 f"{FV.WD}_HH": FV.WD,
                 f"{FV.WS}_HH": FV.WS,
                 f"{FV.TI}_HH": FV.TI,
                 f"{FV.RHO}_HH": FV.RHO,
             }
@@ -141,91 +196,114 @@
         )
 
         self.farm_controllers = Dict(
             name="farm_controllers",
             basic_ctrl=fm.farm_controllers.BasicFarmController(),
         )
 
-        self.partial_wakes = Dict(
+        self.partial_wakes = FDict(
             name="partial_wakes",
             rotor_points=fm.partial_wakes.RotorPoints(),
             top_hat=fm.partial_wakes.PartialTopHat(),
             centre=fm.partial_wakes.PartialCentre(),
         )
-        nlst = list(range(2, 11)) + [20]
-        for n in nlst:
-            self.partial_wakes[f"axiwake{n}"] = fm.partial_wakes.PartialAxiwake(n)
-        for n in nlist:
-            self.partial_wakes[f"grid{n**2}"] = fm.partial_wakes.PartialGrid(n=n)
+        self.partial_wakes.add_factory(
+            fm.partial_wakes.PartialAxiwake,
+            "axiwake<n>",
+            n=lambda x: int(x),
+            hints={"n": "(Number of evaluation points)"},
+        )
+        self.partial_wakes.add_factory(
+            fm.partial_wakes.PartialGrid,
+            "grid<n2>",
+            var2arg={"n2": "n"},
+            n2=_n2n,
+            hints={"n2": "(Number of points in square grid)"},
+        )
 
-        self.wake_frames = Dict(
+        self.wake_frames = FDict(
             name="wake_frames",
             rotor_wd=fm.wake_frames.RotorWD(var_wd=FV.WD),
             rotor_wd_farmo=fm.wake_frames.FarmOrder(),
             yawed=fm.wake_frames.YawedWakes(),
-            yawed_k002=fm.wake_frames.YawedWakes(k=0.02),
-            yawed_k004=fm.wake_frames.YawedWakes(k=0.04),
         )
-        stps = [1.0, 5.0, 10.0, 50.0, 100.0, 500.0]
-        for s in stps:
-            self.wake_frames[f"streamlines_{int(s)}"] = fm.wake_frames.Streamlines2D(
-                step=s
-            )
-        for s in stps:
-            self.wake_frames[f"streamlines_{int(s)}_yawed"] = fm.wake_frames.YawedWakes(
-                base_frame=fm.wake_frames.Streamlines2D(step=s)
-            )
-        for s in stps:
-            self.wake_frames[f"streamlines_{int(s)}_farmo"] = fm.wake_frames.FarmOrder(
-                base_frame=fm.wake_frames.Streamlines2D(step=s)
-            )
-        dtlist = [
-            ("1s", 1 / 60),
-            ("10s", 1 / 6),
-            ("30s", 0.5),
-            ("1min", 1),
-            ("10min", 10),
-            ("30min", 30),
-        ]
+        self.wake_frames.add_factory(
+            fm.wake_frames.YawedWakes,
+            "yawed_k<k>",
+            k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"k": "(Value, e.g. 004 for 0.04)"},
+        )
+        self.wake_frames.add_factory(
+            fm.wake_frames.Streamlines2D,
+            "streamlines_<step>",
+            step=lambda x: float(x),
+            hints={"step": "(Step size in m)"},
+        )
+        self.wake_frames.add_factory(
+            fm.wake_frames.Streamlines2D,
+            "streamlines_<step>",
+            step=lambda x: float(x),
+            hints={"step": "(Step size in m)"},
+        )
+
         self.wake_frames["timelines"] = fm.wake_frames.Timelines()
-        for s, t in dtlist:
-            self.wake_frames[f"timelines_{s}"] = fm.wake_frames.Timelines(dt_min=t)
-        self.wake_frames["timelines_1km"] = fm.wake_frames.Timelines(
-            max_wake_length=1000.0
-        )
-        self.wake_frames["seq_dyn_wakes"] = fm.wake_frames.SeqDynamicWakes()
-        for s, t in dtlist:
-            self.wake_frames[f"seq_dyn_wakes_{s}"] = fm.wake_frames.SeqDynamicWakes(
-                dt_min=t
-            )
+        def _todt(x):
+            if x[-1] == "s":
+                return float(x[:-1])/60
+            elif x[-3:] == "min":
+                return float(x[:-3])
+        self.wake_frames.add_factory(
+            fm.wake_frames.Timelines,
+            "timelines_<dt>",
+            dt=_todt,
+            var2arg={"dt": "dt_min"},
+            hints={"dt": "(Time step, e.g '10s', '1min' etc.)"},
+        )
+        self.wake_frames.add_factory(
+            fm.wake_frames.SeqDynamicWakes,
+            "seq_dyn_wakes_<dt>",
+            dt=_todt,
+            var2arg={"dt": "dt_min"},
+            hints={"dt": "(Time step, e.g '10s', '1min' etc.)"},
+        )
 
         self.wake_superpositions = Dict(
             name="wake_superpositions",
             ws_linear=fm.wake_superpositions.WSLinear(scale_amb=False),
             ws_linear_lim=fm.wake_superpositions.WSLinear(
                 scale_amb=False, lim_low=1e-4
             ),
             ws_linear_amb=fm.wake_superpositions.WSLinear(scale_amb=True),
             ws_linear_amb_lim=fm.wake_superpositions.WSLinear(
                 scale_amb=True, lim_low=1e-4
             ),
+            ws_linear_loc=fm.wake_superpositions.WSLinearLocal(),
+            ws_linear_loc_lim=fm.wake_superpositions.WSLinearLocal(lim_low=1e-4),
             ws_quadratic=fm.wake_superpositions.WSQuadratic(scale_amb=False),
             ws_quadratic_lim=fm.wake_superpositions.WSQuadratic(
                 scale_amb=False, lim_low=1e-4
             ),
             ws_quadratic_amb=fm.wake_superpositions.WSQuadratic(scale_amb=True),
             ws_quadratic_amb_lim=fm.wake_superpositions.WSQuadratic(
                 scale_amb=True, lim_low=1e-4
             ),
+            ws_quadratic_loc=fm.wake_superpositions.WSQuadraticLocal(),
+            ws_quadratic_loc_lim=fm.wake_superpositions.WSQuadraticLocal(lim_low=1e-4),
             ws_cubic=fm.wake_superpositions.WSPow(pow=3, scale_amb=False),
             ws_cubic_amb=fm.wake_superpositions.WSPow(pow=3, scale_amb=True),
+            ws_cubic_loc=fm.wake_superpositions.WSPowLocal(pow=3),
+            ws_cubic_loc_lim=fm.wake_superpositions.WSPowLocal(pow=3, lim_low=1e-4),
             ws_quartic=fm.wake_superpositions.WSPow(pow=4, scale_amb=False),
             ws_quartic_amb=fm.wake_superpositions.WSPow(pow=4, scale_amb=True),
+            ws_quartic_loc=fm.wake_superpositions.WSPowLocal(pow=4),
+            ws_quartic_loc_lim=fm.wake_superpositions.WSPowLocal(pow=4, lim_low=1e-4),
             ws_max=fm.wake_superpositions.WSMax(scale_amb=False),
             ws_max_amb=fm.wake_superpositions.WSMax(scale_amb=True),
+            ws_max_loc=fm.wake_superpositions.WSMaxLocal(),
+            ws_max_loc_lim=fm.wake_superpositions.WSMaxLocal(lim_low=1e-4),
             ws_product=fm.wake_superpositions.WSProduct(),
             ws_product_lim=fm.wake_superpositions.WSProduct(lim_low=1e-4),
             ti_linear=fm.wake_superpositions.TILinear(superp_to_amb="quadratic"),
             ti_quadratic=fm.wake_superpositions.TIQuadratic(superp_to_amb="quadratic"),
             ti_cubic=fm.wake_superpositions.TIPow(pow=3, superp_to_amb="quadratic"),
             ti_quartic=fm.wake_superpositions.TIPow(pow=4, superp_to_amb="quadratic"),
             ti_max=fm.wake_superpositions.TIMax(superp_to_amb="quadratic"),
@@ -233,189 +311,211 @@
 
         self.axial_induction = Dict(name="induction_models")
         self.axial_induction["Betz"] = fm.axial_induction_models.BetzAxialInduction()
         self.axial_induction["Madsen"] = (
             fm.axial_induction_models.MadsenAxialInduction()
         )
 
-        self.wake_models = Dict(name="wake_models")
-        slist = [
-            "linear",
-            "linear_lim",
-            "linear_amb",
-            "linear_amb_lim",
-            "quadratic",
-            "quadratic_lim",
-            "quadratic_amb",
-            "quadratic_amb_lim",
-            "cubic",
-            "cubic_amb",
-            "quartic",
-            "quartic_amb",
-            "wmax",
-            "max_amb",
-            "product",
-            "product_lim",
-        ]
-        for s in slist:
-            self.wake_models[f"Jensen_{s}"] = fm.wake_models.wind.JensenWake(
-                superposition=f"ws_{s}"
-            )
-            self.wake_models[f"Jensen_{s}_k002"] = fm.wake_models.wind.JensenWake(
-                k=0.02, superposition=f"ws_{s}"
-            )
-            self.wake_models[f"Jensen_{s}_k004"] = fm.wake_models.wind.JensenWake(
-                k=0.04, superposition=f"ws_{s}"
-            )
-            self.wake_models[f"Jensen_{s}_k007"] = fm.wake_models.wind.JensenWake(
-                k=0.07, superposition=f"ws_{s}"
-            )
-            self.wake_models[f"Jensen_{s}_k0075"] = fm.wake_models.wind.JensenWake(
-                k=0.075, superposition=f"ws_{s}"
-            )
-
-            self.wake_models[f"Bastankhah2014_{s}"] = (
-                fm.wake_models.wind.Bastankhah2014(
-                    superposition=f"ws_{s}", sbeta_factor=0.2
-                )
-            )
-            self.wake_models[f"Bastankhah2014_{s}_k002"] = (
-                fm.wake_models.wind.Bastankhah2014(
-                    k=0.02, sbeta_factor=0.2, superposition=f"ws_{s}"
-                )
-            )
-            self.wake_models[f"Bastankhah2014_{s}_k004"] = (
-                fm.wake_models.wind.Bastankhah2014(
-                    k=0.04, sbeta_factor=0.2, superposition=f"ws_{s}"
-                )
-            )
-
-            self.wake_models[f"Bastankhah2014B_{s}"] = (
-                fm.wake_models.wind.Bastankhah2014(
-                    superposition=f"ws_{s}", sbeta_factor=0.2, induction="Betz"
-                )
-            )
-            self.wake_models[f"Bastankhah2014B_{s}_k002"] = (
-                fm.wake_models.wind.Bastankhah2014(
-                    k=0.02, sbeta_factor=0.2, superposition=f"ws_{s}", induction="Betz"
-                )
-            )
-            self.wake_models[f"Bastankhah2014B_{s}_k004"] = (
-                fm.wake_models.wind.Bastankhah2014(
-                    k=0.04, sbeta_factor=0.2, superposition=f"ws_{s}", induction="Betz"
-                )
-            )
-
-            self.wake_models[f"Bastankhah025_{s}"] = fm.wake_models.wind.Bastankhah2014(
-                superposition=f"ws_{s}", sbeta_factor=0.25
-            )
-            self.wake_models[f"Bastankhah025_{s}_k002"] = (
-                fm.wake_models.wind.Bastankhah2014(
-                    k=0.02, superposition=f"ws_{s}", sbeta_factor=0.25
-                )
-            )
-            self.wake_models[f"Bastankhah025_{s}_k004"] = (
-                fm.wake_models.wind.Bastankhah2014(
-                    k=0.04, superposition=f"ws_{s}", sbeta_factor=0.25
-                )
-            )
-
-            self.wake_models[f"Bastankhah025B_{s}"] = (
-                fm.wake_models.wind.Bastankhah2014(
-                    superposition=f"ws_{s}", sbeta_factor=0.25, induction="Betz"
-                )
-            )
-            self.wake_models[f"Bastankhah025B_{s}_k002"] = (
-                fm.wake_models.wind.Bastankhah2014(
-                    k=0.02, superposition=f"ws_{s}", sbeta_factor=0.25, induction="Betz"
-                )
-            )
-            self.wake_models[f"Bastankhah025B_{s}_k004"] = (
-                fm.wake_models.wind.Bastankhah2014(
-                    k=0.04, superposition=f"ws_{s}", sbeta_factor=0.25, induction="Betz"
-                )
-            )
-
-            self.wake_models[f"Bastankhah2016_{s}"] = (
-                fm.wake_models.wind.Bastankhah2016(superposition=f"ws_{s}")
-            )
-            self.wake_models[f"Bastankhah2016_{s}_k002"] = (
-                fm.wake_models.wind.Bastankhah2016(superposition=f"ws_{s}", k=0.02)
-            )
-            self.wake_models[f"Bastankhah2016_{s}_k004"] = (
-                fm.wake_models.wind.Bastankhah2016(superposition=f"ws_{s}", k=0.04)
-            )
-
-            self.wake_models[f"Bastankhah2016B_{s}"] = (
-                fm.wake_models.wind.Bastankhah2016(
-                    superposition=f"ws_{s}", induction="Betz"
-                )
-            )
-            self.wake_models[f"Bastankhah2016B_{s}_k002"] = (
-                fm.wake_models.wind.Bastankhah2016(
-                    superposition=f"ws_{s}", k=0.02, induction="Betz"
-                )
-            )
-            self.wake_models[f"Bastankhah2016B_{s}_k004"] = (
-                fm.wake_models.wind.Bastankhah2016(
-                    superposition=f"ws_{s}", k=0.04, induction="Betz"
-                )
-            )
-
-            self.wake_models[f"TurbOPark_{s}_A002"] = fm.wake_models.wind.TurbOParkWake(
-                A=0.02, superposition=f"ws_{s}"
-            )
-            self.wake_models[f"TurbOPark_{s}_A004"] = fm.wake_models.wind.TurbOParkWake(
-                A=0.04, superposition=f"ws_{s}"
-            )
-
-            self.wake_models[f"TurbOParkB_{s}_A002"] = (
-                fm.wake_models.wind.TurbOParkWake(
-                    A=0.02, superposition=f"ws_{s}", induction="Betz"
-                )
-            )
-            self.wake_models[f"TurbOParkB_{s}_A004"] = (
-                fm.wake_models.wind.TurbOParkWake(
-                    A=0.04, superposition=f"ws_{s}", induction="Betz"
-                )
-            )
-
-            As = [0.02, 0.04]
-            dxs = [0.01, 1.0, 5.0, 10.0, 50.0, 100.0]
-            for A in As:
-                for dx in dxs:
-                    a = str(A).replace(".", "")
-                    d = str(dx).replace(".", "") if dx < 1 else int(dx)
-                    self.wake_models[f"TurbOParkIX_{s}_A{a}_dx{d}"] = (
-                        fm.wake_models.wind.TurbOParkWakeIX(
-                            A=A, superposition=f"ws_{s}", dx=dx
-                        )
-                    )
-
-        slist = ["linear", "quadratic", "cubic", "quartic", "max"]
-        for s in slist:
-            self.wake_models[f"CrespoHernandez_{s}"] = (
-                fm.wake_models.ti.CrespoHernandezTIWake(superposition=f"ti_{s}")
-            )
-            self.wake_models[f"CrespoHernandez_ambti_{s}"] = (
-                fm.wake_models.ti.CrespoHernandezTIWake(
-                    superposition=f"ti_{s}", use_ambti=True
-                )
-            )
-            self.wake_models[f"CrespoHernandez_{s}_k002"] = (
-                fm.wake_models.ti.CrespoHernandezTIWake(k=0.02, superposition=f"ti_{s}")
-            )
-
-            self.wake_models[f"IECTI2005_{s}"] = fm.wake_models.ti.IECTIWake(
-                superposition=f"ti_{s}", iec_type="2005"
-            )
-
-            self.wake_models[f"IECTI2019_{s}"] = fm.wake_models.ti.IECTIWake(
-                superposition=f"ti_{s}", iec_type="2019"
-            )
+        self.wake_models = FDict(name="wake_models")
+
+        self.wake_models.add_factory(
+            fm.wake_models.wind.JensenWake,
+            "Jensen_<superposition>",
+            superposition=lambda s: f"ws_{s}",
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.JensenWake,
+            "Jensen_<superposition>_k<k>",
+            superposition=lambda s: f"ws_{s}",
+            k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
+                   "k": "(Value, e.g. 004 for 0.04)"},
+        )
+
+        self.wake_models.add_factory(
+            fm.wake_models.wind.Bastankhah2014,
+            "Bastankhah2014_<superposition>",
+            kwargs=dict(sbeta_factor=0.2),
+            superposition=lambda s: f"ws_{s}",
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.Bastankhah2014,
+            "Bastankhah2014_<superposition>_k<k>",
+            kwargs=dict(sbeta_factor=0.2),
+            superposition=lambda s: f"ws_{s}",
+            k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
+                   "k": "(Value, e.g. 004 for 0.04)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.Bastankhah2014,
+            "Bastankhah2014B_<superposition>",
+            kwargs=dict(sbeta_factor=0.2, induction="Betz"),
+            superposition=lambda s: f"ws_{s}",
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.Bastankhah2014,
+            "Bastankhah2014B_<superposition>_k<k>",
+            kwargs=dict(sbeta_factor=0.2, induction="Betz"),
+            superposition=lambda s: f"ws_{s}",
+            k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
+                   "k": "(Value, e.g. 004 for 0.04)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.Bastankhah2014,
+            "Bastankhah025_<superposition>",
+            kwargs=dict(sbeta_factor=0.25),
+            superposition=lambda s: f"ws_{s}",
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.Bastankhah2014,
+            "Bastankhah025_<superposition>_k<k>",
+            kwargs=dict(sbeta_factor=0.25),
+            superposition=lambda s: f"ws_{s}",
+            k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
+                   "k": "(Value, e.g. 004 for 0.04)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.Bastankhah2014,
+            "Bastankhah025B_<superposition>",
+            kwargs=dict(sbeta_factor=0.25, induction="Betz"),
+            superposition=lambda s: f"ws_{s}",
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.Bastankhah2014,
+            "Bastankhah025B_<superposition>_k<k>",
+            kwargs=dict(sbeta_factor=0.25, induction="Betz"),
+            superposition=lambda s: f"ws_{s}",
+            k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
+                   "k": "(Value, e.g. 004 for 0.04)"},
+        )
+
+        self.wake_models.add_factory(
+            fm.wake_models.wind.Bastankhah2016,
+            "Bastankhah2016_<superposition>",
+            superposition=lambda s: f"ws_{s}",
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.Bastankhah2016,
+            "Bastankhah2016_<superposition>_k<k>",
+            superposition=lambda s: f"ws_{s}",
+            k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
+                   "k": "(Value, e.g. 004 for 0.04)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.Bastankhah2016,
+            "Bastankhah2016B_<superposition>",
+            kwargs=dict(induction="Betz"),
+            superposition=lambda s: f"ws_{s}",
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.Bastankhah2016,
+            "Bastankhah2016B_<superposition>_k<k>",
+            kwargs=dict(induction="Betz"),
+            superposition=lambda s: f"ws_{s}",
+            k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
+                   "k": "(Value, e.g. 004 for 0.04)"},
+        )
+
+        self.wake_models.add_factory(
+            fm.wake_models.wind.TurbOParkWake,
+            "TurbOPark_<superposition>",
+            superposition=lambda s: f"ws_{s}",
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.TurbOParkWake,
+            "TurbOPark_<superposition>_k<k>",
+            superposition=lambda s: f"ws_{s}",
+            k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
+                   "k": "(Value, e.g. 004 for 0.04)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.TurbOParkWake,
+            "TurbOParkB_<superposition>",
+            kwargs=dict(induction="Betz"),
+            superposition=lambda s: f"ws_{s}",
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
+        )
+        self.wake_models.add_factory(
+            fm.wake_models.wind.TurbOParkWake,
+            "TurbOParkB_<superposition>_k<k>",
+            kwargs=dict(induction="Betz"),
+            superposition=lambda s: f"ws_{s}",
+            k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
+                   "k": "(Value, e.g. 004 for 0.04)"},
+        )
+
+        self.wake_models.add_factory(
+            fm.wake_models.wind.TurbOParkWakeIX,
+            "TurbOParkIX_<superposition>_dx<dx>",
+            superposition=lambda s: f"ws_{s}",
+            dx=lambda x: float(x),
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
+                   "dx": "(Integration step in m)"},
+        )
+
+        self.wake_models.add_factory(
+            fm.wake_models.wind.TurbOParkWakeIX,
+            "TurbOParkIX_<superposition>_k<k>_dx<dx>",
+            superposition=lambda s: f"ws_{s}",
+            k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            dx=lambda x: float(x),
+            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
+                   "k": "(Value, e.g. 004 for 0.04)",
+                   "dx": "(Integration step in m)"},
+        )
+
+        self.wake_models.add_factory(
+            fm.wake_models.ti.CrespoHernandezTIWake,
+            "CrespoHernandez_<superposition>",
+            kwargs=dict(use_ambti=False),
+            superposition=lambda s: f"ti_{s}",
+            hints={"superposition": "(Superposition, e.g. linear for ti_linear)"},
+        )
+
+        self.wake_models.add_factory(
+            fm.wake_models.ti.CrespoHernandezTIWake,
+            "CrespoHernandez_<superposition>_k<k>",
+            kwargs=dict(use_ambti=False),
+            superposition=lambda s: f"ti_{s}",
+            k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
+            hints={"superposition": "(Superposition, e.g. linear for ti_linear)",
+                   "k": "(Value, e.g. 004 for 0.04)"},
+        )
+
+        self.wake_models.add_factory(
+            fm.wake_models.ti.IECTIWake,
+            "IECTI2005_<superposition>",
+            kwargs=dict(iec_type="2005"),
+            superposition=lambda s: f"ti_{s}",
+            hints={"superposition": "(Superposition, e.g. linear for ti_linear)"},
+        )
+
+        self.wake_models.add_factory(
+            fm.wake_models.ti.IECTIWake,
+            "IECTI2019_<superposition>",
+            kwargs=dict(iec_type="2019"),
+            superposition=lambda s: f"ti_{s}",
+            hints={"superposition": "(Superposition, e.g. linear for ti_linear)"},
+        )
 
         self.wake_models[f"RHB"] = fm.wake_models.induction.RankineHalfBody()
         self.wake_models[f"Rathmann"] = fm.wake_models.induction.Rathmann()
         self.wake_models[f"SelfSimilar"] = fm.wake_models.induction.SelfSimilar()
         self.wake_models[f"SelfSimilar2020"] = (
             fm.wake_models.induction.SelfSimilar2020()
         )
@@ -464,23 +564,29 @@
         ----------
         subset: list of str, optional
             Selection of model types
         search:  str, optional
             String that has to be part of the model name
 
         """
+
         for k in sorted(list(self.sources.keys())):
             ms = self.sources[k]
             if subset is None or k in subset:
                 print(k)
                 print("-" * len(k))
                 if len(ms):
                     for mname in sorted(list(ms.keys())):
                         if search is None or search in mname:
                             print(f"{mname}: {ms[mname]}")
+                    if isinstance(ms, FDict):
+                        for f in ms.factories:
+                            if search is None or search in f.name_template:
+                                print()
+                                print(f)
                 else:
                     print("(none)")
                 print()
 
     def get(self, model_type, name, class_name=None, *args, **kwargs):
         """
         Gets a model object.
```

### Comparing `foxes-0.7.0.6/foxes/models/partial_wakes/axiwake.py` & `foxes-0.7.1/foxes/models/partial_wakes/axiwake.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/partial_wakes/centre.py` & `foxes-0.7.1/foxes/models/partial_wakes/centre.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/partial_wakes/grid.py` & `foxes-0.7.1/foxes/models/partial_wakes/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/partial_wakes/rotor_points.py` & `foxes-0.7.1/foxes/models/partial_wakes/rotor_points.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/partial_wakes/segregated.py` & `foxes-0.7.1/foxes/models/partial_wakes/segregated.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/partial_wakes/top_hat.py` & `foxes-0.7.1/foxes/models/partial_wakes/top_hat.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/point_models/set_uniform_data.py` & `foxes-0.7.1/foxes/models/point_models/set_uniform_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/point_models/tke2ti.py` & `foxes-0.7.1/foxes/models/point_models/tke2ti.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/point_models/wake_deltas.py` & `foxes-0.7.1/foxes/models/point_models/wake_deltas.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/rotor_models/centre.py` & `foxes-0.7.1/foxes/models/rotor_models/centre.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/rotor_models/grid.py` & `foxes-0.7.1/foxes/models/rotor_models/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/rotor_models/levels.py` & `foxes-0.7.1/foxes/models/rotor_models/levels.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_models/calculator.py` & `foxes-0.7.1/foxes/models/turbine_models/calculator.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_models/kTI_model.py` & `foxes-0.7.1/foxes/models/turbine_models/kTI_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_models/lookup_table.py` & `foxes-0.7.1/foxes/models/turbine_models/lookup_table.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_models/power_mask.py` & `foxes-0.7.1/foxes/models/turbine_models/power_mask.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_models/rotor_centre_calc.py` & `foxes-0.7.1/foxes/models/turbine_models/rotor_centre_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_models/sector_management.py` & `foxes-0.7.1/foxes/models/turbine_models/sector_management.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_models/set_farm_vars.py` & `foxes-0.7.1/foxes/models/turbine_models/set_farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_models/table_factors.py` & `foxes-0.7.1/foxes/models/turbine_models/table_factors.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_models/thrust2ct.py` & `foxes-0.7.1/foxes/models/turbine_models/thrust2ct.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_models/yaw2yawm.py` & `foxes-0.7.1/foxes/models/turbine_models/yaw2yawm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_models/yawm2yaw.py` & `foxes-0.7.1/foxes/models/turbine_models/yawm2yaw.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_types/CpCt_file.py` & `foxes-0.7.1/foxes/models/turbine_types/CpCt_file.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_types/CpCt_from_two.py` & `foxes-0.7.1/foxes/models/turbine_types/CpCt_from_two.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_types/PCt_file.py` & `foxes-0.7.1/foxes/models/turbine_types/PCt_file.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_types/PCt_from_two.py` & `foxes-0.7.1/foxes/models/turbine_types/PCt_from_two.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_types/null_type.py` & `foxes-0.7.1/foxes/models/turbine_types/null_type.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_types/wsrho2PCt_from_two.py` & `foxes-0.7.1/foxes/models/turbine_types/wsrho2PCt_from_two.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/turbine_types/wsti2PCt_from_two.py` & `foxes-0.7.1/foxes/models/turbine_types/wsti2PCt_from_two.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/vertical_profiles/abl_log_neutral_ws.py` & `foxes-0.7.1/foxes/models/vertical_profiles/abl_log_neutral_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/vertical_profiles/abl_log_stable_ws.py` & `foxes-0.7.1/foxes/models/vertical_profiles/abl_log_stable_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/vertical_profiles/abl_log_unstable_ws.py` & `foxes-0.7.1/foxes/models/vertical_profiles/abl_log_unstable_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/vertical_profiles/abl_log_ws.py` & `foxes-0.7.1/foxes/models/vertical_profiles/abl_log_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/vertical_profiles/data_profile.py` & `foxes-0.7.1/foxes/models/vertical_profiles/data_profile.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/vertical_profiles/sheared_ws.py` & `foxes-0.7.1/foxes/models/vertical_profiles/sheared_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/vertical_profiles/uniform.py` & `foxes-0.7.1/foxes/models/vertical_profiles/uniform.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_frames/farm_order.py` & `foxes-0.7.1/foxes/models/wake_frames/farm_order.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_frames/rotor_wd.py` & `foxes-0.7.1/foxes/models/wake_frames/rotor_wd.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_frames/seq_dynamic_wakes.py` & `foxes-0.7.1/foxes/models/wake_frames/seq_dynamic_wakes.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_frames/streamlines.py` & `foxes-0.7.1/foxes/models/wake_frames/streamlines.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_frames/timelines.py` & `foxes-0.7.1/foxes/models/wake_frames/timelines.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_frames/yawed_wakes.py` & `foxes-0.7.1/foxes/models/wake_frames/yawed_wakes.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/axisymmetric.py` & `foxes-0.7.1/foxes/models/wake_models/axisymmetric.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/dist_sliced.py` & `foxes-0.7.1/foxes/models/wake_models/dist_sliced.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/gaussian.py` & `foxes-0.7.1/foxes/models/wake_models/gaussian.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/induction/rankine_half_body.py` & `foxes-0.7.1/foxes/models/wake_models/induction/rankine_half_body.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/induction/rathmann.py` & `foxes-0.7.1/foxes/models/wake_models/induction/rathmann.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/induction/self_similar.py` & `foxes-0.7.1/foxes/models/wake_models/induction/self_similar.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/induction/self_similar2020.py` & `foxes-0.7.1/foxes/models/wake_models/induction/self_similar2020.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/ti/crespo_hernandez.py` & `foxes-0.7.1/foxes/models/wake_models/ti/crespo_hernandez.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/ti/iec_ti.py` & `foxes-0.7.1/foxes/models/wake_models/ti/iec_ti.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/top_hat.py` & `foxes-0.7.1/foxes/models/wake_models/top_hat.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/wake_mirror.py` & `foxes-0.7.1/foxes/models/wake_models/wake_mirror.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/wind/bastankhah14.py` & `foxes-0.7.1/foxes/models/wake_models/wind/bastankhah14.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Reference:
     "A new analytical model for wind-turbine wakes"
     Majid Bastankhah, Fernando Porté-Agel
     https://doi.org/10.1016/j.renene.2014.01.002
 
     Attributes
     ----------
-    k: float, optional
+    k: float
         The wake growth parameter k. If not given here
         it will be searched in the farm data.
     sbeta_factor: float
         Factor multiplying sbeta
     k_var: str
         The variable name for k
     induction: foxes.core.AxialInductionModel or str
```

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/wind/bastankhah16.py` & `foxes-0.7.1/foxes/models/wake_models/wind/bastankhah16.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/wind/jensen.py` & `foxes-0.7.1/foxes/models/wake_models/wind/jensen.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_models/wind/turbopark.py` & `foxes-0.7.1/foxes/models/wake_models/wind/turbopark.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     Reference:
     "Turbulence Optimized Park model with Gaussian wake profile"
     J G Pedersen, E Svensson, L Poulsen and N G Nygaard
     https://iopscience.iop.org/article/10.1088/1742-6596/2265/2/022063/pdf
 
     Attributes
     ----------
-    A: float
-        The wake growth parameter A.
+    k: float
+        The wake growth parameter k.
     sbeta_factor: float
         Factor multiplying sbeta
     c1: float
         Factor from Frandsen turbulence model
     c2: float
         Factor from Frandsen turbulence model
     induction: foxes.core.AxialInductionModel or str
@@ -32,53 +32,65 @@
     :group: models.wake_models.wind
 
     """
 
     def __init__(
         self,
         superposition,
-        A,
+        k=None,
         sbeta_factor=0.25,
         c1=1.5,
         c2=0.8,
+        k_var=FV.K,
         induction="Madsen",
     ):
         """
         Constructor.
 
         Parameters
         ----------
         superposition: str
             The wind deficit superposition
-        A: float
-            The wake growth parameter A.
+        k: float, optional
+            The wake growth parameter k. If not given here
+            it will be searched in the farm data.
         sbeta_factor: float
             Factor multiplying sbeta
         c1: float
             Factor from Frandsen turbulence model
         c2: float
             Factor from Frandsen turbulence model
+        k_var: str
+            The variable name for k
         induction: foxes.core.AxialInductionModel or str
             The induction model
 
         """
         super().__init__(superpositions={FV.WS: superposition})
 
-        self.A = A
         self.sbeta_factor = sbeta_factor
         self.c1 = c1
         self.c2 = c2
+        self.k_var = k_var
         self.induction = induction
 
+        setattr(self, k_var, k)
+
     def __repr__(self):
+        k = getattr(self, self.k_var)
         iname = (
             self.induction if isinstance(self.induction, str) else self.induction.name
         )
         s = f"{type(self).__name__}"
-        s += f"({self.superpositions[FV.WS]}, A={self.A}, induction={iname})"
+        s += f"({self.superpositions[FV.WS]}, induction={iname}"
+        if k is None:
+            s += f", k_var={self.k_var}"
+        else:
+            s += f", {self.k_var}={k}"
+        s += ")"
         return s
 
     def sub_models(self):
         """
         List of all sub-models
 
         Returns
@@ -184,28 +196,40 @@
                 algo=algo,
                 fdata=fdata,
                 tdata=tdata,
                 downwind_index=downwind_index,
                 upcast=True,
             )[st_sel]
 
+            # get k:
+            k = self.get_data(
+                self.k_var,
+                FC.STATE_TARGET,
+                lookup="sw",
+                algo=algo,
+                fdata=fdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
+                upcast=True,
+            )[st_sel]
+
             # calculate sigma:
             # beta = np.sqrt(0.5 * (1 + np.sqrt(1.0 - ct)) / np.sqrt(1.0 - ct))
             a = self.induction.ct2a(ct)
             beta = (1 - a) / (1 - 2 * a)
             epsilon = self.sbeta_factor * np.sqrt(beta)
             del a, beta
 
             alpha = self.c1 * ati
             beta = self.c2 * ati / np.sqrt(ct)
 
             # calculate sigma (eqn 4)
             sigma = D * (
                 epsilon
-                + self.A
+                + k
                 * ati
                 / beta
                 * (
                     np.sqrt((alpha + beta * x / D) ** 2 + 1)
                     - np.sqrt(1 + alpha**2)
                     - np.log(
                         (np.sqrt((alpha + beta * x / D) ** 2 + 1) + 1)
@@ -242,18 +266,20 @@
 
     https://iopscience.iop.org/article/10.1088/1742-6596/2265/2/022063/pdf
 
     Attributes
     ----------
     dx: float
         The step size of the integral
-    A: float
-        The wake growth parameter A.
+    k: float
+        The wake growth parameter k.
     sbeta_factor: float
         Factor multiplying sbeta
+    k_var: str
+        The variable name for k
     ti_var:  str
         The TI variable
     self_wake: bool
         Flag for considering only own wake in ti integral
     induction: foxes.core.AxialInductionModel or str
         The induction model
     ipars: dict
@@ -263,61 +289,73 @@
 
     """
 
     def __init__(
         self,
         superposition,
         dx,
-        A,
+        k=None,
         sbeta_factor=0.25,
+        k_var=FV.K,
         ti_var=FV.TI,
         self_wake=True,
         induction="Madsen",
         **ipars,
     ):
         """
         Constructor.
 
         Parameters
         ----------
         superposition: str
             The wind deficit superposition
         dx: float
             The step size of the integral
-        A: float, optional
-            The wake growth parameter A.
+        k: float, optional
+            The wake growth parameter k. If not given here
+            it will be searched in the farm data.
         sbeta_factor: float
             Factor multiplying sbeta
+        k_var: str
+            The variable name for k
         ti_var:  str
             The TI variable
         self_wake: bool
             Flag for considering only own wake in ti integral
         induction: foxes.core.AxialInductionModel or str
             The induction model
         ipars: dict, optional
             Additional parameters for centreline integration
 
         """
         super().__init__(superpositions={FV.WS: superposition})
 
         self.dx = dx
-        self.A = A
         self.sbeta_factor = sbeta_factor
+        self.k_var = k_var
         self.ti_var = ti_var
         self.ipars = ipars
         self._tiwakes = None
         self.self_wake = self_wake
         self.induction = induction
 
+        setattr(self, k_var, k)
+
     def __repr__(self):
+        k = getattr(self, self.k_var)
         iname = (
             self.induction if isinstance(self.induction, str) else self.induction.name
         )
-        s = f"{type(self).__name__}({self.superpositions[FV.WS]}"
-        s += f", ti={self.ti_var}, dx={self.dx}, A={self.A}, induction={iname})"
+        s = f"{type(self).__name__}"
+        s += f"({self.superpositions[FV.WS]}, induction={iname}, dx={self.dx}"
+        if k is None:
+            s += f", k_var={self.k_var}"
+        else:
+            s += f", {self.k_var}={k}"
+        s += f", ti_var={self.ti_var})"
         return s
 
     def sub_models(self):
         """
         List of all sub-models
 
         Returns
@@ -447,14 +485,26 @@
                 algo=algo,
                 fdata=fdata,
                 tdata=tdata,
                 downwind_index=downwind_index,
                 upcast=True,
             )[st_sel]
 
+            # get k:
+            k = self.get_data(
+                self.k_var,
+                FC.STATE_TARGET,
+                lookup="sw",
+                algo=algo,
+                fdata=fdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
+                upcast=True,
+            )[st_sel]
+
             # calculate sigma:
             # beta = np.sqrt(0.5 * (1 + np.sqrt(1.0 - ct)) / np.sqrt(1.0 - ct))
             a = self.induction.ct2a(ct)
             beta = (1 - a) / (1 - 2 * a)
             epsilon = self.sbeta_factor * np.sqrt(beta)
             del a, beta
 
@@ -469,15 +519,15 @@
                 dx=self.dx,
                 wake_models=self._tiwakes,
                 self_wake=self.self_wake,
                 **self.ipars,
             )[:, :, 0]
 
             # calculate sigma (eqn 1, plus epsilon from eqn 4 for x = 0)
-            sigma = D * epsilon + self.A * ti_ix[st_sel]
+            sigma = D * epsilon + k * ti_ix[st_sel]
             del x, epsilon
 
             # calculate amplitude, same as in Bastankhah model (eqn 7)
             ct_eff = ct / (8 * (sigma / D) ** 2)
             ampld = np.maximum(-2 * self.induction.ct2a(ct_eff), -1)
 
         # case no targets:
```

### Comparing `foxes-0.7.0.6/foxes/models/wake_superpositions/ti_linear.py` & `foxes-0.7.1/foxes/models/wake_superpositions/ti_linear.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_superpositions/ti_max.py` & `foxes-0.7.1/foxes/models/wake_superpositions/ti_max.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_superpositions/ti_pow.py` & `foxes-0.7.1/foxes/models/wake_superpositions/ti_pow.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_superpositions/ti_quadratic.py` & `foxes-0.7.1/foxes/models/wake_superpositions/ti_quadratic.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/models/wake_superpositions/ws_linear.py` & `foxes-0.7.1/foxes/models/wake_superpositions/ws_product.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 import numpy as np
 
 from foxes.core import WakeSuperposition
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class WSLinear(WakeSuperposition):
+class WSProduct(WakeSuperposition):
     """
-    Linear supersposition of wind deficit results
+    Product supersposition of wind deficit results
+
+    This is based on the idea that the dimensionless
+    wind deficit should be rescaled with the wake
+    corrected wind field, rather than the rotor
+    equivalent wind speed.
+
+    Source: https://arxiv.org/pdf/2010.03873.pdf
+            Equation (8)
 
     Attributes
     ----------
-    scale_amb: bool
-        Flag for scaling wind deficit with ambient wind speed
-        instead of waked wind speed
     lim_low: float
         Lower limit of the final waked wind speed
     lim_high: float
         Upper limit of the final waked wind speed
 
     :group: models.wake_superpositions
 
     """
 
-    def __init__(self, scale_amb=False, lim_low=None, lim_high=None):
+    def __init__(self, lim_low=None, lim_high=None):
         """
         Constructor.
 
         Parameters
         ----------
-        scale_amb: bool
-            Flag for scaling wind deficit with ambient wind speed
-            instead of waked wind speed
         lim_low: float
             Lower limit of the final waked wind speed
         lim_high: float
             Upper limit of the final waked wind speed
 
         """
         super().__init__()
 
-        self.scale_amb = scale_amb
         self.lim_low = lim_low
         self.lim_high = lim_high
 
     def __repr__(self):
-        a = f"scale_amb={self.scale_amb}, lim_low={self.lim_low}, lim_high={self.lim_high}"
+        a = f"lim_low={self.lim_low}, lim_high={self.lim_high}"
         return f"{type(self).__name__}({a})"
 
     def input_farm_vars(self, algo):
         """
         The variables which are needed for running
         the model.
 
@@ -115,26 +116,18 @@
         """
         if variable not in [FV.REWS, FV.REWS2, FV.REWS3, FV.WS]:
             raise ValueError(
                 f"Superposition '{self.name}': Expecting wind speed variable, got {variable}"
             )
 
         if np.any(st_sel):
-            scale = self.get_data(
-                FV.AMB_REWS if self.scale_amb else FV.REWS,
-                FC.STATE_TARGET,
-                lookup="w",
-                algo=algo,
-                fdata=fdata,
-                tdata=tdata,
-                downwind_index=downwind_index,
-                upcast=True,
-            )[st_sel, None]
+            if np.max(np.abs(wake_delta)) < 1e-14:
+                wake_delta[:] = 1
 
-            wake_delta[st_sel] += scale * wake_model_result
+            wake_delta[st_sel] *= 1 + wake_model_result
 
         return wake_delta
 
     def calc_final_wake_delta(
         self,
         algo,
         mdata,
@@ -168,13 +161,13 @@
         -------
         final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
             results by simple plus operation. Shape:
             (n_states, n_targets, n_tpoints)
 
         """
-        w = wake_delta
+        w = amb_results * (wake_delta - 1)
         if self.lim_low is not None:
             w = np.maximum(w, self.lim_low - amb_results)
         if self.lim_high is not None:
             w = np.minimum(w, self.lim_high - amb_results)
         return w
```

### Comparing `foxes-0.7.0.6/foxes/models/wake_superpositions/ws_max.py` & `foxes-0.7.1/foxes/models/wake_superpositions/ws_quadratic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 
 from foxes.core import WakeSuperposition
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class WSMax(WakeSuperposition):
+class WSQuadratic(WakeSuperposition):
     """
-    Max supersposition of wind deficit results
+    Quadratic supersposition of wind deficit results
 
     Attributes
     ----------
     scale_amb: bool
         Flag for scaling wind deficit with ambient wind speed
         instead of waked wind speed
     lim_low: float
@@ -126,18 +126,170 @@
                 algo=algo,
                 fdata=fdata,
                 tdata=tdata,
                 downwind_index=downwind_index,
                 upcast=True,
             )[st_sel, None]
 
-            wake_model_result = np.abs(scale * wake_model_result)
-            odelta = wake_delta[st_sel]
+            wake_delta[st_sel] += (scale * wake_model_result) ** 2
 
-            wake_delta[st_sel] = np.maximum(odelta, wake_model_result)
+        return wake_delta
+
+    def calc_final_wake_delta(
+        self,
+        algo,
+        mdata,
+        fdata,
+        variable,
+        amb_results,
+        wake_delta,
+    ):
+        """
+        Calculate the final wake delta after adding all
+        contributions.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        variable: str
+            The variable name for which the wake deltas applies
+        amb_results: numpy.ndarray
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
+        wake_delta: numpy.ndarray
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
+
+        Returns
+        -------
+        final_wake_delta: numpy.ndarray
+            The final wake delta, which will be added to the ambient
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
+
+        """
+        w = -np.sqrt(wake_delta)
+        if self.lim_low is not None:
+            w = np.maximum(w, self.lim_low - amb_results)
+        if self.lim_high is not None:
+            w = np.minimum(w, self.lim_high - amb_results)
+        return w
+
+class WSQuadraticLocal(WakeSuperposition):
+    """
+    Local quadratic supersposition of wind deficit results
+
+    Attributes
+    ----------
+    lim_low: float
+        Lower limit of the final waked wind speed
+    lim_high: float
+        Upper limit of the final waked wind speed
+
+    :group: models.wake_superpositions
+
+    """
+
+    def __init__(self, lim_low=None, lim_high=None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        lim_low: float
+            Lower limit of the final waked wind speed
+        lim_high: float
+            Upper limit of the final waked wind speed
+
+        """
+        super().__init__()
+        self.lim_low = lim_low
+        self.lim_high = lim_high
+
+    def __repr__(self):
+        a = f"lim_low={self.lim_low}, lim_high={self.lim_high}"
+        return f"{type(self).__name__}({a})"
+
+    def input_farm_vars(self, algo):
+        """
+        The variables which are needed for running
+        the model.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+
+        Returns
+        -------
+        input_vars: list of str
+            The input variable names
+
+        """
+        return []
+
+    def add_wake(
+        self,
+        algo,
+        mdata,
+        fdata,
+        tdata,
+        downwind_index,
+        st_sel,
+        variable,
+        wake_delta,
+        wake_model_result,
+    ):
+        """
+        Add a wake delta to previous wake deltas,
+        at rotor points.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
+        variable: str
+            The variable name for which the wake deltas applies
+        wake_delta: numpy.ndarray
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
+        wake_model_result: numpy.ndarray
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
+
+        Returns
+        -------
+        wdelta: numpy.ndarray
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
+
+        """
+        if variable not in [FV.REWS, FV.REWS2, FV.REWS3, FV.WS]:
+            raise ValueError(
+                f"Superposition '{self.name}': Expecting wind speed variable, got {variable}"
+            )
+
+        if np.any(st_sel):
+            wake_delta[st_sel] += wake_model_result**2
 
         return wake_delta
 
     def calc_final_wake_delta(
         self,
         algo,
         mdata,
@@ -171,13 +323,13 @@
         -------
         final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
             results by simple plus operation. Shape:
             (n_states, n_targets, n_tpoints)
 
         """
-        w = -wake_delta
+        w = -np.sqrt(wake_delta) * amb_results
         if self.lim_low is not None:
             w = np.maximum(w, self.lim_low - amb_results)
         if self.lim_high is not None:
             w = np.minimum(w, self.lim_high - amb_results)
         return w
```

### Comparing `foxes-0.7.0.6/foxes/models/wake_superpositions/ws_pow.py` & `foxes-0.7.1/foxes/models/wake_superpositions/ws_pow.py`

 * *Files 23% similar despite different names*

```diff
@@ -179,7 +179,168 @@
         """
         w = -(wake_delta ** (1 / self.pow))
         if self.lim_low is not None:
             w = np.maximum(w, self.lim_low - amb_results)
         if self.lim_high is not None:
             w = np.minimum(w, self.lim_high - amb_results)
         return w
+
+class WSPowLocal(WakeSuperposition):
+    """
+    Local power supersposition of wind deficit results
+
+    Attributes
+    ----------
+    pow: float
+        The power to which to take the wake results
+    lim_low: float
+        Lower limit of the final waked wind speed
+    lim_high: float
+        Upper limit of the final waked wind speed
+
+    :group: models.wake_superpositions
+
+    """
+
+    def __init__(self, pow, lim_low=None, lim_high=None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        pow: float
+            The power to which to take the wake results
+        lim_low: float
+            Lower limit of the final waked wind speed
+        lim_high: float
+            Upper limit of the final waked wind speed
+
+        """
+        super().__init__()
+
+        self.pow = pow
+        self.lim_low = lim_low
+        self.lim_high = lim_high
+
+    def __repr__(self):
+        a = f"pow={self.pow}, lim_low={self.lim_low}, lim_high={self.lim_high}"
+        return f"{type(self).__name__}({a})"
+
+    def input_farm_vars(self, algo):
+        """
+        The variables which are needed for running
+        the model.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+
+        Returns
+        -------
+        input_vars: list of str
+            The input variable names
+
+        """
+        return []
+
+    def add_wake(
+        self,
+        algo,
+        mdata,
+        fdata,
+        tdata,
+        downwind_index,
+        st_sel,
+        variable,
+        wake_delta,
+        wake_model_result,
+    ):
+        """
+        Add a wake delta to previous wake deltas,
+        at rotor points.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
+        variable: str
+            The variable name for which the wake deltas applies
+        wake_delta: numpy.ndarray
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
+        wake_model_result: numpy.ndarray
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
+
+        Returns
+        -------
+        wdelta: numpy.ndarray
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
+
+        """
+        if variable not in [FV.REWS, FV.REWS2, FV.REWS3, FV.WS]:
+            raise ValueError(
+                f"Superposition '{self.name}': Expecting wind speed variable, got {variable}"
+            )
+
+        if np.any(st_sel):
+            wake_delta[st_sel] += np.abs(wake_model_result) ** self.pow
+
+        return wake_delta
+
+    def calc_final_wake_delta(
+        self,
+        algo,
+        mdata,
+        fdata,
+        variable,
+        amb_results,
+        wake_delta,
+    ):
+        """
+        Calculate the final wake delta after adding all
+        contributions.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        variable: str
+            The variable name for which the wake deltas applies
+        amb_results: numpy.ndarray
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
+        wake_delta: numpy.ndarray
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
+
+        Returns
+        -------
+        final_wake_delta: numpy.ndarray
+            The final wake delta, which will be added to the ambient
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
+
+        """
+        w = -(wake_delta ** (1 / self.pow)) * amb_results
+        if self.lim_low is not None:
+            w = np.maximum(w, self.lim_low - amb_results)
+        if self.lim_high is not None:
+            w = np.minimum(w, self.lim_high - amb_results)
+        return w
```

### Comparing `foxes-0.7.0.6/foxes/models/wake_superpositions/ws_product.py` & `foxes-0.7.1/foxes/models/wake_superpositions/ws_linear.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,192 @@
 import numpy as np
 
 from foxes.core import WakeSuperposition
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class WSProduct(WakeSuperposition):
+class WSLinear(WakeSuperposition):
     """
-    Product supersposition of wind deficit results
+    Linear supersposition of wind deficit results
 
-    This is based on the idea that the dimensionless
-    wind deficit should be rescaled with the wake
-    corrected wind field, rather than the rotor
-    equivalent wind speed.
+    Attributes
+    ----------
+    scale_amb: bool
+        Flag for scaling wind deficit with ambient wind speed
+        instead of waked wind speed
+    lim_low: float
+        Lower limit of the final waked wind speed
+    lim_high: float
+        Upper limit of the final waked wind speed
+
+    :group: models.wake_superpositions
+
+    """
 
-    Source: https://arxiv.org/pdf/2010.03873.pdf
-            Equation (8)
+    def __init__(self, scale_amb=False, lim_low=None, lim_high=None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        scale_amb: bool
+            Flag for scaling wind deficit with ambient wind speed
+            instead of waked wind speed
+        lim_low: float
+            Lower limit of the final waked wind speed
+        lim_high: float
+            Upper limit of the final waked wind speed
+
+        """
+        super().__init__()
+
+        self.scale_amb = scale_amb
+        self.lim_low = lim_low
+        self.lim_high = lim_high
+
+    def __repr__(self):
+        a = f"scale_amb={self.scale_amb}, lim_low={self.lim_low}, lim_high={self.lim_high}"
+        return f"{type(self).__name__}({a})"
+
+    def input_farm_vars(self, algo):
+        """
+        The variables which are needed for running
+        the model.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+
+        Returns
+        -------
+        input_vars: list of str
+            The input variable names
+
+        """
+        return [FV.AMB_REWS] if self.scale_amb else [FV.REWS]
+
+    def add_wake(
+        self,
+        algo,
+        mdata,
+        fdata,
+        tdata,
+        downwind_index,
+        st_sel,
+        variable,
+        wake_delta,
+        wake_model_result,
+    ):
+        """
+        Add a wake delta to previous wake deltas,
+        at rotor points.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
+        variable: str
+            The variable name for which the wake deltas applies
+        wake_delta: numpy.ndarray
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
+        wake_model_result: numpy.ndarray
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
+
+        Returns
+        -------
+        wdelta: numpy.ndarray
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
+
+        """
+        if variable not in [FV.REWS, FV.REWS2, FV.REWS3, FV.WS]:
+            raise ValueError(
+                f"Superposition '{self.name}': Expecting wind speed variable, got {variable}"
+            )
+
+        if np.any(st_sel):
+            scale = self.get_data(
+                FV.AMB_REWS if self.scale_amb else FV.REWS,
+                FC.STATE_TARGET,
+                lookup="w",
+                algo=algo,
+                fdata=fdata,
+                tdata=tdata,
+                downwind_index=downwind_index,
+                upcast=True,
+            )[st_sel, None]
+
+            wake_delta[st_sel] += scale * wake_model_result
+
+        return wake_delta
+
+    def calc_final_wake_delta(
+        self,
+        algo,
+        mdata,
+        fdata,
+        variable,
+        amb_results,
+        wake_delta,
+    ):
+        """
+        Calculate the final wake delta after adding all
+        contributions.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        variable: str
+            The variable name for which the wake deltas applies
+        amb_results: numpy.ndarray
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
+        wake_delta: numpy.ndarray
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
+
+        Returns
+        -------
+        final_wake_delta: numpy.ndarray
+            The final wake delta, which will be added to the ambient
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
+
+        """
+        w = wake_delta
+        if self.lim_low is not None:
+            w = np.maximum(w, self.lim_low - amb_results)
+        if self.lim_high is not None:
+            w = np.minimum(w, self.lim_high - amb_results)
+        return w
+
+
+class WSLinearLocal(WakeSuperposition):
+    """
+    Local linear supersposition of wind deficit results
 
     Attributes
     ----------
     lim_low: float
         Lower limit of the final waked wind speed
     lim_high: float
         Upper limit of the final waked wind speed
@@ -37,15 +204,14 @@
         lim_low: float
             Lower limit of the final waked wind speed
         lim_high: float
             Upper limit of the final waked wind speed
 
         """
         super().__init__()
-
         self.lim_low = lim_low
         self.lim_high = lim_high
 
     def __repr__(self):
         a = f"lim_low={self.lim_low}, lim_high={self.lim_high}"
         return f"{type(self).__name__}({a})"
 
@@ -61,15 +227,15 @@
 
         Returns
         -------
         input_vars: list of str
             The input variable names
 
         """
-        return [FV.AMB_REWS] if self.scale_amb else [FV.REWS]
+        return []
 
     def add_wake(
         self,
         algo,
         mdata,
         fdata,
         tdata,
@@ -116,18 +282,15 @@
         """
         if variable not in [FV.REWS, FV.REWS2, FV.REWS3, FV.WS]:
             raise ValueError(
                 f"Superposition '{self.name}': Expecting wind speed variable, got {variable}"
             )
 
         if np.any(st_sel):
-            if np.max(np.abs(wake_delta)) < 1e-14:
-                wake_delta[:] = 1
-
-            wake_delta[st_sel] *= 1 + wake_model_result
+            wake_delta[st_sel] += wake_model_result
 
         return wake_delta
 
     def calc_final_wake_delta(
         self,
         algo,
         mdata,
@@ -161,13 +324,13 @@
         -------
         final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
             results by simple plus operation. Shape:
             (n_states, n_targets, n_tpoints)
 
         """
-        w = amb_results * (wake_delta - 1)
+        w = wake_delta * amb_results
         if self.lim_low is not None:
             w = np.maximum(w, self.lim_low - amb_results)
         if self.lim_high is not None:
             w = np.minimum(w, self.lim_high - amb_results)
         return w
```

### Comparing `foxes-0.7.0.6/foxes/models/wake_superpositions/ws_quadratic.py` & `foxes-0.7.1/foxes/models/wake_superpositions/ws_max.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 
 from foxes.core import WakeSuperposition
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class WSQuadratic(WakeSuperposition):
+class WSMax(WakeSuperposition):
     """
-    Quadratic supersposition of wind deficit results
+    Max supersposition of wind deficit results
 
     Attributes
     ----------
     scale_amb: bool
         Flag for scaling wind deficit with ambient wind speed
         instead of waked wind speed
     lim_low: float
@@ -126,15 +126,176 @@
                 algo=algo,
                 fdata=fdata,
                 tdata=tdata,
                 downwind_index=downwind_index,
                 upcast=True,
             )[st_sel, None]
 
-            wake_delta[st_sel] += (scale * wake_model_result) ** 2
+            wake_model_result = np.abs(scale * wake_model_result)
+            odelta = wake_delta[st_sel]
+
+            wake_delta[st_sel] = np.maximum(odelta, wake_model_result)
+
+        return wake_delta
+
+    def calc_final_wake_delta(
+        self,
+        algo,
+        mdata,
+        fdata,
+        variable,
+        amb_results,
+        wake_delta,
+    ):
+        """
+        Calculate the final wake delta after adding all
+        contributions.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        variable: str
+            The variable name for which the wake deltas applies
+        amb_results: numpy.ndarray
+            The ambient results at targets,
+            shape: (n_states, n_targets, n_tpoints)
+        wake_delta: numpy.ndarray
+            The wake deltas at targets, shape:
+            (n_states, n_targets, n_tpoints)
+
+        Returns
+        -------
+        final_wake_delta: numpy.ndarray
+            The final wake delta, which will be added to the ambient
+            results by simple plus operation. Shape:
+            (n_states, n_targets, n_tpoints)
+
+        """
+        w = -wake_delta
+        if self.lim_low is not None:
+            w = np.maximum(w, self.lim_low - amb_results)
+        if self.lim_high is not None:
+            w = np.minimum(w, self.lim_high - amb_results)
+        return w
+
+class WSMaxLocal(WakeSuperposition):
+    """
+    Local max supersposition of wind deficit results
+
+    Attributes
+    ----------
+    lim_low: float
+        Lower limit of the final waked wind speed
+    lim_high: float
+        Upper limit of the final waked wind speed
+
+    :group: models.wake_superpositions
+
+    """
+
+    def __init__(self, lim_low=None, lim_high=None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        lim_low: float
+            Lower limit of the final waked wind speed
+        lim_high: float
+            Upper limit of the final waked wind speed
+
+        """
+        super().__init__()
+        self.lim_low = lim_low
+        self.lim_high = lim_high
+
+    def __repr__(self):
+        a = f"lim_low={self.lim_low}, lim_high={self.lim_high}"
+        return f"{type(self).__name__}({a})"
+
+    def input_farm_vars(self, algo):
+        """
+        The variables which are needed for running
+        the model.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+
+        Returns
+        -------
+        input_vars: list of str
+            The input variable names
+
+        """
+        return []
+
+    def add_wake(
+        self,
+        algo,
+        mdata,
+        fdata,
+        tdata,
+        downwind_index,
+        st_sel,
+        variable,
+        wake_delta,
+        wake_model_result,
+    ):
+        """
+        Add a wake delta to previous wake deltas,
+        at rotor points.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.MData
+            The model data
+        fdata: foxes.core.FData
+            The farm data
+        tdata: foxes.core.TData
+            The target point data
+        downwind_index: int
+            The index of the wake causing turbine
+            in the downwnd order
+        st_sel: numpy.ndarray of bool
+            The selection of targets, shape: (n_states, n_targets)
+        variable: str
+            The variable name for which the wake deltas applies
+        wake_delta: numpy.ndarray
+            The original wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
+        wake_model_result: numpy.ndarray
+            The new wake deltas of the selected rotors,
+            shape: (n_st_sel, n_tpoints, ...)
+
+        Returns
+        -------
+        wdelta: numpy.ndarray
+            The updated wake deltas, shape:
+            (n_states, n_targets, n_tpoints, ...)
+
+        """
+        if variable not in [FV.REWS, FV.REWS2, FV.REWS3, FV.WS]:
+            raise ValueError(
+                f"Superposition '{self.name}': Expecting wind speed variable, got {variable}"
+            )
+
+        if np.any(st_sel):
+            wake_model_result = np.abs(wake_model_result)
+            odelta = wake_delta[st_sel]
+
+            wake_delta[st_sel] = np.maximum(odelta, wake_model_result)
 
         return wake_delta
 
     def calc_final_wake_delta(
         self,
         algo,
         mdata,
@@ -168,13 +329,13 @@
         -------
         final_wake_delta: numpy.ndarray
             The final wake delta, which will be added to the ambient
             results by simple plus operation. Shape:
             (n_states, n_targets, n_tpoints)
 
         """
-        w = -np.sqrt(wake_delta)
+        w = -wake_delta * amb_results
         if self.lim_low is not None:
             w = np.maximum(w, self.lim_low - amb_results)
         if self.lim_high is not None:
             w = np.minimum(w, self.lim_high - amb_results)
         return w
```

### Comparing `foxes-0.7.0.6/foxes/opt/constraints/area_geometry.py` & `foxes-0.7.1/foxes/opt/constraints/area_geometry.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/constraints/min_dist.py` & `foxes-0.7.1/foxes/opt/constraints/min_dist.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/core/farm_constraint.py` & `foxes-0.7.1/foxes/opt/core/farm_constraint.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/core/farm_objective.py` & `foxes-0.7.1/foxes/opt/core/farm_objective.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/core/farm_opt_problem.py` & `foxes-0.7.1/foxes/opt/core/farm_opt_problem.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/core/farm_vars_problem.py` & `foxes-0.7.1/foxes/opt/core/farm_vars_problem.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/core/pop_states.py` & `foxes-0.7.1/foxes/opt/core/pop_states.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/objectives/farm_vars.py` & `foxes-0.7.1/foxes/opt/objectives/farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/objectives/max_n_turbines.py` & `foxes-0.7.1/foxes/opt/objectives/max_n_turbines.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/problems/layout/farm_layout.py` & `foxes-0.7.1/foxes/opt/problems/layout/farm_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/constraints.py` & `foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/constraints.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/geom_layout.py` & `foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py` & `foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py` & `foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py` & `foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/problems/layout/geom_layouts/objectives.py` & `foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/objectives.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/problems/layout/reggrids_layout.py` & `foxes-0.7.1/foxes/opt/problems/layout/reggrids_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/problems/layout/regular_layout.py` & `foxes-0.7.1/foxes/opt/problems/layout/regular_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/opt/problems/opt_farm_vars.py` & `foxes-0.7.1/foxes/opt/problems/opt_farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/__init__.py` & `foxes-0.7.1/foxes/output/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/animation.py` & `foxes-0.7.1/foxes/output/animation.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/calc_points.py` & `foxes-0.7.1/foxes/output/calc_points.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/farm_layout.py` & `foxes-0.7.1/foxes/output/farm_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/farm_results_eval.py` & `foxes-0.7.1/foxes/output/farm_results_eval.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/flow_plots_2d/flow_plots.py` & `foxes-0.7.1/foxes/output/flow_plots_2d/flow_plots.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/flow_plots_2d/get_fig.py` & `foxes-0.7.1/foxes/output/flow_plots_2d/get_fig.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/flow_plots_2d/seq_flow_ani_plugin.py` & `foxes-0.7.1/foxes/output/flow_plots_2d/seq_flow_ani_plugin.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/grids.py` & `foxes-0.7.1/foxes/output/grids.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/output.py` & `foxes-0.7.1/foxes/output/output.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/results_writer.py` & `foxes-0.7.1/foxes/output/results_writer.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/rose_plot.py` & `foxes-0.7.1/foxes/output/rose_plot.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/rotor_point_plots.py` & `foxes-0.7.1/foxes/output/rotor_point_plots.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/slice_data.py` & `foxes-0.7.1/foxes/output/slice_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/state_turbine_map.py` & `foxes-0.7.1/foxes/output/state_turbine_map.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/output/turbine_type_curves.py` & `foxes-0.7.1/foxes/output/turbine_type_curves.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/abl/neutral.py` & `foxes-0.7.1/foxes/utils/abl/neutral.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/abl/stable.py` & `foxes-0.7.1/foxes/utils/abl/stable.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/abl/unstable.py` & `foxes-0.7.1/foxes/utils/abl/unstable.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/cubic_roots.py` & `foxes-0.7.1/foxes/utils/cubic_roots.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/data_book.py` & `foxes-0.7.1/foxes/utils/data_book.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/dict.py` & `foxes-0.7.1/foxes/utils/dict.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/exec_python.py` & `foxes-0.7.1/foxes/utils/exec_python.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/geom2d/area_geometry.py` & `foxes-0.7.1/foxes/utils/geom2d/area_geometry.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/geom2d/circle.py` & `foxes-0.7.1/foxes/utils/geom2d/circle.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/geom2d/example_intersection.py` & `foxes-0.7.1/foxes/utils/geom2d/example_intersection.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/geom2d/example_union.py` & `foxes-0.7.1/foxes/utils/geom2d/example_union.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/geom2d/half_plane.py` & `foxes-0.7.1/foxes/utils/geom2d/half_plane.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/geom2d/polygon.py` & `foxes-0.7.1/foxes/utils/geom2d/polygon.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/geopandas_helpers.py` & `foxes-0.7.1/foxes/utils/geopandas_helpers.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/geopandas_utils.py` & `foxes-0.7.1/foxes/utils/geopandas_utils.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/load.py` & `foxes-0.7.1/foxes/utils/load.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/pandas_helpers.py` & `foxes-0.7.1/foxes/utils/pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/pandas_utils.py` & `foxes-0.7.1/foxes/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/random_xy.py` & `foxes-0.7.1/foxes/utils/random_xy.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/regularize.py` & `foxes-0.7.1/foxes/utils/regularize.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/runners/runners.py` & `foxes-0.7.1/foxes/utils/runners/runners.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/tab_files.py` & `foxes-0.7.1/foxes/utils/tab_files.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/two_circles.py` & `foxes-0.7.1/foxes/utils/two_circles.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/wind_dir.py` & `foxes-0.7.1/foxes/utils/wind_dir.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/windrose_plot.py` & `foxes-0.7.1/foxes/utils/windrose_plot.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/utils/xarray_utils.py` & `foxes-0.7.1/foxes/utils/xarray_utils.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes/variables.py` & `foxes-0.7.1/foxes/variables.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.0.6/foxes.egg-info/PKG-INFO` & `foxes-0.7.1/foxes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.7.0.6
+Version: 0.7.1
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
```

### Comparing `foxes-0.7.0.6/foxes.egg-info/SOURCES.txt` & `foxes-0.7.1/foxes.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -230,14 +230,15 @@
 foxes/output/flow_plots_2d/get_fig.py
 foxes/output/flow_plots_2d/seq_flow_ani_plugin.py
 foxes/utils/__init__.py
 foxes/utils/cubic_roots.py
 foxes/utils/data_book.py
 foxes/utils/dict.py
 foxes/utils/exec_python.py
+foxes/utils/factory.py
 foxes/utils/geopandas_helpers.py
 foxes/utils/geopandas_utils.py
 foxes/utils/load.py
 foxes/utils/pandas_helpers.py
 foxes/utils/pandas_utils.py
 foxes/utils/plotly_helpers.py
 foxes/utils/random_xy.py
```

### Comparing `foxes-0.7.0.6/setup.cfg` & `foxes-0.7.1/setup.cfg`

 * *Files identical despite different names*

