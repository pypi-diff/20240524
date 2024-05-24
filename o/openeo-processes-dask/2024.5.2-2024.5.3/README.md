# Comparing `tmp/openeo_processes_dask-2024.5.2.tar.gz` & `tmp/openeo_processes_dask-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openeo_processes_dask-2024.5.2.tar", max compression
+gzip compressed data, was "openeo_processes_dask-2024.5.3.tar", max compression
```

## Comparing `openeo_processes_dask-2024.5.2.tar` & `openeo_processes_dask-2024.5.3.tar`

### file list

```diff
@@ -1,221 +1,221 @@
--rw-r--r--   0        0        0    10765 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/LICENSE
--rw-r--r--   0        0        0     3355 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/README.md
--rw-r--r--   0        0        0       93 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/__init__.py
--rw-r--r--   0        0        0      808 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/__init__.py
--rw-r--r--   0        0        0    10955 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/arrays.py
--rw-r--r--   0        0        0     2997 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/comparison.py
--rw-r--r--   0        0        0     4127 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/core.py
--rw-r--r--   0        0        0      250 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/__init__.py
--rw-r--r--   0        0        0     8361 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/_filter.py
--rw-r--r--   0        0        0     3900 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/_xr_interop.py
--rw-r--r--   0        0        0     5730 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/aggregate.py
--rw-r--r--   0        0        0     4081 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/apply.py
--rw-r--r--   0        0        0     2617 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/experimental.py
--rw-r--r--   0        0        0     2418 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/general.py
--rw-r--r--   0        0        0     2131 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/indices.py
--rw-r--r--   0        0        0     8139 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/load.py
--rw-r--r--   0        0        0     5294 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/mask.py
--rw-r--r--   0        0        0     4951 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/mask_polygon.py
--rw-r--r--   0        0        0    10568 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/merge.py
--rw-r--r--   0        0        0     1792 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/reduce.py
--rw-r--r--   0        0        0     4546 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/resample.py
--rw-r--r--   0        0        0      442 2024-05-21 16:43:58.047829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/utils.py
--rw-r--r--   0        0        0      233 2024-05-21 16:43:58.051829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/data_model.py
--rw-r--r--   0        0        0     1387 2024-05-21 16:43:58.051829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-21 16:43:58.051829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/experimental/__init__.py
--rw-r--r--   0        0        0     2317 2024-05-21 16:43:58.051829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/logic.py
--rw-r--r--   0        0        0     6785 2024-05-21 16:43:58.051829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/math.py
--rw-r--r--   0        0        0       58 2024-05-21 16:43:58.051829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/ml/__init__.py
--rw-r--r--   0        0        0     4834 2024-05-21 16:43:58.051829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/ml/curve_fitting.py
--rw-r--r--   0        0        0     4761 2024-05-21 16:43:58.051829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/ml/random_forest.py
--rw-r--r--   0        0        0      233 2024-05-21 16:43:58.051829 openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/utils.py
--rw-r--r--   0        0        0      892 2024-05-21 16:43:58.051829 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/__init__.py
--rw-r--r--   0        0        0       75 2024-05-21 16:43:58.827831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/.git
--rw-r--r--   0        0        0       27 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      445 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/issue-or-clarification-for-existing-process.md
--rw-r--r--   0        0        0      856 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-parameter.md
--rw-r--r--   0        0        0     1516 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-proposal.md
--rw-r--r--   0        0        0      167 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/other.md
--rw-r--r--   0        0        0     1953 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/.github/workflows/docs.yml
--rw-r--r--   0        0        0      329 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/.github/workflows/tests.yml
--rw-r--r--   0        0        0    19276 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/LICENSE
--rw-r--r--   0        0        0     4577 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/README.md
--rw-r--r--   0        0        0     2325 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/absolute.json
--rw-r--r--   0        0        0     1735 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/adaptive_threshold.json
--rw-r--r--   0        0        0     2390 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/add.json
--rw-r--r--   0        0        0     2009 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/add_dimension.json
--rw-r--r--   0        0        0     7128 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/aggregate_spatial.json
--rw-r--r--   0        0        0    10948 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/aggregate_temporal.json
--rw-r--r--   0        0        0     7770 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/aggregate_temporal_period.json
--rw-r--r--   0        0        0     3799 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/all.json
--rw-r--r--   0        0        0     2371 2024-05-21 16:43:58.835831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/and.json
--rw-r--r--   0        0        0     3768 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/any.json
--rw-r--r--   0        0        0     2724 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/apply.json
--rw-r--r--   0        0        0     6535 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/apply_dimension.json
--rw-r--r--   0        0        0     5329 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/apply_kernel.json
--rw-r--r--   0        0        0     1145 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/arccos.json
--rw-r--r--   0        0        0     1192 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/arcosh.json
--rw-r--r--   0        0        0     1133 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/arcsin.json
--rw-r--r--   0        0        0     1151 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/arctan.json
--rw-r--r--   0        0        0     1720 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/arctan2.json
--rw-r--r--   0        0        0     6022 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/ard_normalized_radar_backscatter.json
--rw-r--r--   0        0        0     6651 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/ard_surface_reflectance.json
--rw-r--r--   0        0        0     1572 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_append.json
--rw-r--r--   0        0        0     1591 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_concat.json
--rw-r--r--   0        0        0     4992 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_contains.json
--rw-r--r--   0        0        0     2619 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_create.json
--rw-r--r--   0        0        0     3377 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_element.json
--rw-r--r--   0        0        0     3594 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_filter.json
--rw-r--r--   0        0        0     5266 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_find.json
--rw-r--r--   0        0        0      831 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_labels.json
--rw-r--r--   0        0        0     5638 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_modify.json
--rw-r--r--   0        0        0     1182 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/arsinh.json
--rw-r--r--   0        0        0     1197 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/artanh.json
--rw-r--r--   0        0        0     3537 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/atmospheric_correction.json
--rw-r--r--   0        0        0     6511 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/between.json
--rw-r--r--   0        0        0     3621 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/cab.json
--rw-r--r--   0        0        0     1402 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/ceil.json
--rw-r--r--   0        0        0     2811 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/clip.json
--rw-r--r--   0        0        0      585 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/constant.json
--rw-r--r--   0        0        0     1038 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/cos.json
--rw-r--r--   0        0        0     1093 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/cosh.json
--rw-r--r--   0        0        0     5028 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/count.json
--rw-r--r--   0        0        0      685 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/create_raster_cube.json
--rw-r--r--   0        0        0     1217 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/dimension_labels.json
--rw-r--r--   0        0        0     2235 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/divide.json
--rw-r--r--   0        0        0     1666 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/drop_dimension.json
--rw-r--r--   0        0        0      713 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/e.json
--rw-r--r--   0        0        0     5450 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/eq.json
--rw-r--r--   0        0        0     1652 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/examples/array_contains_nodata.json
--rw-r--r--   0        0        0     1810 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/examples/array_find_nodata.json
--rw-r--r--   0        0        0     1728 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/examples/rename-enumerated-labels.json
--rw-r--r--   0        0        0     1672 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/exp.json
--rw-r--r--   0        0        0     3089 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/extrema.json
--rw-r--r--   0        0        0     3681 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/fapar.json
--rw-r--r--   0        0        0     3638 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/fcover.json
--rw-r--r--   0        0        0     3780 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/filter_bands.json
--rw-r--r--   0        0        0     6644 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/filter_bbox.json
--rw-r--r--   0        0        0     4600 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/filter_labels.json
--rw-r--r--   0        0        0     3572 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/filter_spatial.json
--rw-r--r--   0        0        0     4640 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/filter_temporal.json
--rw-r--r--   0        0        0     2047 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/first.json
--rw-r--r--   0        0        0     3578 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/fit_curve.json
--rw-r--r--   0        0        0     3985 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/fit_regr_random_forest.json
--rw-r--r--   0        0        0     1574 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/floor.json
--rw-r--r--   0        0        0     2645 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/gt.json
--rw-r--r--   0        0        0     3797 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/gte.json
--rw-r--r--   0        0        0     2521 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/if.json
--rw-r--r--   0        0        0     1569 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/int.json
--rw-r--r--   0        0        0     1132 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/is_infinite.json
--rw-r--r--   0        0        0     1646 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/is_nan.json
--rw-r--r--   0        0        0     1398 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/is_nodata.json
--rw-r--r--   0        0        0     1760 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/is_valid.json
--rw-r--r--   0        0        0     3586 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/lai.json
--rw-r--r--   0        0        0     2042 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/last.json
--rw-r--r--   0        0        0     5011 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/linear_scale_range.json
--rw-r--r--   0        0        0     2111 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/ln.json
--rw-r--r--   0        0        0    17245 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/load_collection.json
--rw-r--r--   0        0        0     1956 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/load_ml_model.json
--rw-r--r--   0        0        0    17030 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/load_stac.json
--rw-r--r--   0        0        0     2015 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/load_url.json
--rw-r--r--   0        0        0     1463 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/load_vector_cube.json
--rw-r--r--   0        0        0     2322 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/log.json
--rw-r--r--   0        0        0     2634 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/lt.json
--rw-r--r--   0        0        0     3787 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/lte.json
--rw-r--r--   0        0        0     3207 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/mask.json
--rw-r--r--   0        0        0     4045 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/mask_polygon.json
--rw-r--r--   0        0        0     2476 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/max.json
--rw-r--r--   0        0        0     4412 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/mean.json
--rw-r--r--   0        0        0     4029 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/median.json
--rw-r--r--   0        0        0     7807 2024-05-21 16:43:58.839831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/merge_cubes.json
--rw-r--r--   0        0        0    11001 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/meta/implementation.md
--rw-r--r--   0        0        0    19134 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/meta/subtype-schemas.json
--rw-r--r--   0        0        0     2408 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/min.json
--rw-r--r--   0        0        0     4358 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/anomaly.json
--rw-r--r--   0        0        0    11277 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/apply_neighborhood.json
--rw-r--r--   0        0        0     4087 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/array_apply.json
--rw-r--r--   0        0        0     3970 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/climatological_normal.json
--rw-r--r--   0        0        0     5205 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/filter_bbox.json
--rw-r--r--   0        0        0     1633 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_dimension.json
--rw-r--r--   0        0        0     4437 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_labels.json
--rw-r--r--   0        0        0     6869 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/resample_spatial.json
--rw-r--r--   0        0        0     3908 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/run_udf.json
--rw-r--r--   0        0        0     2605 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/text_begins.json
--rw-r--r--   0        0        0     2573 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/text_contains.json
--rw-r--r--   0        0        0     2579 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/text_ends.json
--rw-r--r--   0        0        0     2863 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/text_merge.json
--rw-r--r--   0        0        0      883 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/trim_cube.json
--rw-r--r--   0        0        0     2634 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/mod.json
--rw-r--r--   0        0        0     2564 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/multiply.json
--rw-r--r--   0        0        0      879 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/nan.json
--rw-r--r--   0        0        0     6014 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/ndvi.json
--rw-r--r--   0        0        0     6037 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/neq.json
--rw-r--r--   0        0        0     2566 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/normalized_difference.json
--rw-r--r--   0        0        0     1111 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/not.json
--rw-r--r--   0        0        0     2368 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/or.json
--rw-r--r--   0        0        0     5506 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/order.json
--rw-r--r--   0        0        0      686 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/pi.json
--rw-r--r--   0        0        0     2278 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/power.json
--rw-r--r--   0        0        0     3907 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/predict_curve.json
--rw-r--r--   0        0        0     1988 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/predict_random_forest.json
--rw-r--r--   0        0        0     3035 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/product.json
--rw-r--r--   0        0        0     5560 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/aggregate_spatial_window.json
--rw-r--r--   0        0        0     5380 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/ard_normalized_radar_backscatter.json
--rw-r--r--   0        0        0     6009 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/ard_surface_reflectance.json
--rw-r--r--   0        0        0     1702 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/array_append.json
--rw-r--r--   0        0        0     1601 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/array_create_labeled.json
--rw-r--r--   0        0        0     1454 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/array_find_label.json
--rw-r--r--   0        0        0     2405 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/array_interpolate_linear.json
--rw-r--r--   0        0        0     2895 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/atmospheric_correction.json
--rw-r--r--   0        0        0     2892 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/cloud_detection.json
--rw-r--r--   0        0        0     2814 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/cummax.json
--rw-r--r--   0        0        0     2815 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/cummin.json
--rw-r--r--   0        0        0     2888 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/cumproduct.json
--rw-r--r--   0        0        0     2777 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/cumsum.json
--rw-r--r--   0        0        0     5608 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/date_shift.json
--rw-r--r--   0        0        0     4600 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/filter_labels.json
--rw-r--r--   0        0        0     2214 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/inspect.json
--rw-r--r--   0        0        0     1132 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/is_infinite.json
--rw-r--r--   0        0        0    11705 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/load_result.json
--rw-r--r--   0        0        0     2292 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/load_uploaded_files.json
--rw-r--r--   0        0        0     4000 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/resample_cube_temporal.json
--rw-r--r--   0        0        0     2624 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/run_udf_externally.json
--rw-r--r--   0        0        0     5986 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/sar_backscatter.json
--rw-r--r--   0        0        0     5910 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/quantiles.json
--rw-r--r--   0        0        0     2703 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/rearrange.json
--rw-r--r--   0        0        0     3471 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/reduce_dimension.json
--rw-r--r--   0        0        0     3655 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/reduce_spatial.json
--rw-r--r--   0        0        0     4178 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/resample_cube_spatial.json
--rw-r--r--   0        0        0     6566 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/resample_spatial.json
--rw-r--r--   0        0        0     2759 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/round.json
--rw-r--r--   0        0        0     6628 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sar_backscatter.json
--rw-r--r--   0        0        0     1181 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/save_ml_model.json
--rw-r--r--   0        0        0     3077 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/save_result.json
--rw-r--r--   0        0        0     1094 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/save_vector_cube.json
--rw-r--r--   0        0        0     3086 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sd.json
--rw-r--r--   0        0        0     2790 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sen2like.json
--rw-r--r--   0        0        0     2503 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sgn.json
--rw-r--r--   0        0        0     1028 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sin.json
--rw-r--r--   0        0        0     1083 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sinh.json
--rw-r--r--   0        0        0     5177 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sort.json
--rw-r--r--   0        0        0     1891 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sqrt.json
--rw-r--r--   0        0        0     1975 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/subtract.json
--rw-r--r--   0        0        0     3008 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sum.json
--rw-r--r--   0        0        0     1114 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tan.json
--rw-r--r--   0        0        0     1191 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tanh.json
--rw-r--r--   0        0        0       50 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/.gitignore
--rw-r--r--   0        0        0      371 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/.words
--rw-r--r--   0        0        0     2075 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/README.md
--rw-r--r--   0        0        0     3396 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/docs.html
--rw-r--r--   0        0        0     1977 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/examples.test.js
--rw-r--r--   0        0        0     1013 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/package.json
--rw-r--r--   0        0        0     8960 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/processes.test.js
--rw-r--r--   0        0        0     1021 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/subtypes-file.test.js
--rw-r--r--   0        0        0     1929 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/subtypes-schemas.test.js
--rw-r--r--   0        0        0     4776 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/testHelpers.js
--rw-r--r--   0        0        0     4488 2024-05-21 16:43:58.843831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/variance.json
--rw-r--r--   0        0        0     1262 2024-05-21 16:43:58.847831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/vessel_detection.json
--rw-r--r--   0        0        0     3119 2024-05-21 16:43:58.847831 openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/xor.json
--rw-r--r--   0        0        0     2456 2024-05-21 16:43:58.051829 openeo_processes_dask-2024.5.2/pyproject.toml
--rw-r--r--   0        0        0     5481 1970-01-01 00:00:00.000000 openeo_processes_dask-2024.5.2/PKG-INFO
+-rw-r--r--   0        0        0    10765 2024-05-24 08:57:23.345887 openeo_processes_dask-2024.5.3/LICENSE
+-rw-r--r--   0        0        0     3355 2024-05-24 08:57:23.345887 openeo_processes_dask-2024.5.3/README.md
+-rw-r--r--   0        0        0       93 2024-05-24 08:57:23.345887 openeo_processes_dask-2024.5.3/openeo_processes_dask/__init__.py
+-rw-r--r--   0        0        0      808 2024-05-24 08:57:23.345887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/__init__.py
+-rw-r--r--   0        0        0    10955 2024-05-24 08:57:23.345887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/arrays.py
+-rw-r--r--   0        0        0     2997 2024-05-24 08:57:23.345887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/comparison.py
+-rw-r--r--   0        0        0     4127 2024-05-24 08:57:23.345887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/core.py
+-rw-r--r--   0        0        0      250 2024-05-24 08:57:23.345887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/__init__.py
+-rw-r--r--   0        0        0     8361 2024-05-24 08:57:23.345887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/_filter.py
+-rw-r--r--   0        0        0     3900 2024-05-24 08:57:23.345887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/_xr_interop.py
+-rw-r--r--   0        0        0     5730 2024-05-24 08:57:23.345887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/aggregate.py
+-rw-r--r--   0        0        0     4081 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/apply.py
+-rw-r--r--   0        0        0     2617 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/experimental.py
+-rw-r--r--   0        0        0     2418 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/general.py
+-rw-r--r--   0        0        0     2131 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/indices.py
+-rw-r--r--   0        0        0     8139 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/load.py
+-rw-r--r--   0        0        0     5294 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/mask.py
+-rw-r--r--   0        0        0     4951 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/mask_polygon.py
+-rw-r--r--   0        0        0    10568 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/merge.py
+-rw-r--r--   0        0        0     1792 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/reduce.py
+-rw-r--r--   0        0        0     4662 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/resample.py
+-rw-r--r--   0        0        0      442 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/utils.py
+-rw-r--r--   0        0        0      233 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/data_model.py
+-rw-r--r--   0        0        0     1387 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/experimental/__init__.py
+-rw-r--r--   0        0        0     2317 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/logic.py
+-rw-r--r--   0        0        0     6785 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/math.py
+-rw-r--r--   0        0        0       58 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/ml/__init__.py
+-rw-r--r--   0        0        0     4834 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/ml/curve_fitting.py
+-rw-r--r--   0        0        0     4761 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/ml/random_forest.py
+-rw-r--r--   0        0        0      233 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/utils.py
+-rw-r--r--   0        0        0      892 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/__init__.py
+-rw-r--r--   0        0        0       75 2024-05-24 08:57:23.773887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/.git
+-rw-r--r--   0        0        0       27 2024-05-24 08:57:23.777887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      445 2024-05-24 08:57:23.777887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/issue-or-clarification-for-existing-process.md
+-rw-r--r--   0        0        0      856 2024-05-24 08:57:23.777887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-parameter.md
+-rw-r--r--   0        0        0     1516 2024-05-24 08:57:23.777887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-proposal.md
+-rw-r--r--   0        0        0      167 2024-05-24 08:57:23.777887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/other.md
+-rw-r--r--   0        0        0     1953 2024-05-24 08:57:23.777887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      329 2024-05-24 08:57:23.777887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/.github/workflows/tests.yml
+-rw-r--r--   0        0        0    19276 2024-05-24 08:57:23.777887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-05-24 08:57:23.777887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/LICENSE
+-rw-r--r--   0        0        0     4577 2024-05-24 08:57:23.777887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/README.md
+-rw-r--r--   0        0        0     2325 2024-05-24 08:57:23.777887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/absolute.json
+-rw-r--r--   0        0        0     1735 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/adaptive_threshold.json
+-rw-r--r--   0        0        0     2390 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/add.json
+-rw-r--r--   0        0        0     2009 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/add_dimension.json
+-rw-r--r--   0        0        0     7128 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/aggregate_spatial.json
+-rw-r--r--   0        0        0    10948 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/aggregate_temporal.json
+-rw-r--r--   0        0        0     7770 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/aggregate_temporal_period.json
+-rw-r--r--   0        0        0     3799 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/all.json
+-rw-r--r--   0        0        0     2371 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/and.json
+-rw-r--r--   0        0        0     3768 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/any.json
+-rw-r--r--   0        0        0     2724 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/apply.json
+-rw-r--r--   0        0        0     6535 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/apply_dimension.json
+-rw-r--r--   0        0        0     5329 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/apply_kernel.json
+-rw-r--r--   0        0        0     1145 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/arccos.json
+-rw-r--r--   0        0        0     1192 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/arcosh.json
+-rw-r--r--   0        0        0     1133 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/arcsin.json
+-rw-r--r--   0        0        0     1151 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/arctan.json
+-rw-r--r--   0        0        0     1720 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/arctan2.json
+-rw-r--r--   0        0        0     6022 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/ard_normalized_radar_backscatter.json
+-rw-r--r--   0        0        0     6651 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/ard_surface_reflectance.json
+-rw-r--r--   0        0        0     1572 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_append.json
+-rw-r--r--   0        0        0     1591 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_concat.json
+-rw-r--r--   0        0        0     4992 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_contains.json
+-rw-r--r--   0        0        0     2619 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_create.json
+-rw-r--r--   0        0        0     3377 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_element.json
+-rw-r--r--   0        0        0     3594 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_filter.json
+-rw-r--r--   0        0        0     5266 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_find.json
+-rw-r--r--   0        0        0      831 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_labels.json
+-rw-r--r--   0        0        0     5638 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_modify.json
+-rw-r--r--   0        0        0     1182 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/arsinh.json
+-rw-r--r--   0        0        0     1197 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/artanh.json
+-rw-r--r--   0        0        0     3537 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/atmospheric_correction.json
+-rw-r--r--   0        0        0     6511 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/between.json
+-rw-r--r--   0        0        0     3621 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/cab.json
+-rw-r--r--   0        0        0     1402 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/ceil.json
+-rw-r--r--   0        0        0     2811 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/clip.json
+-rw-r--r--   0        0        0      585 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/constant.json
+-rw-r--r--   0        0        0     1038 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/cos.json
+-rw-r--r--   0        0        0     1093 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/cosh.json
+-rw-r--r--   0        0        0     5028 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/count.json
+-rw-r--r--   0        0        0      685 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/create_raster_cube.json
+-rw-r--r--   0        0        0     1217 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/dimension_labels.json
+-rw-r--r--   0        0        0     2235 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/divide.json
+-rw-r--r--   0        0        0     1666 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/drop_dimension.json
+-rw-r--r--   0        0        0      713 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/e.json
+-rw-r--r--   0        0        0     5450 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/eq.json
+-rw-r--r--   0        0        0     1652 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/examples/array_contains_nodata.json
+-rw-r--r--   0        0        0     1810 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/examples/array_find_nodata.json
+-rw-r--r--   0        0        0     1728 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/examples/rename-enumerated-labels.json
+-rw-r--r--   0        0        0     1672 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/exp.json
+-rw-r--r--   0        0        0     3089 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/extrema.json
+-rw-r--r--   0        0        0     3681 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/fapar.json
+-rw-r--r--   0        0        0     3638 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/fcover.json
+-rw-r--r--   0        0        0     3780 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/filter_bands.json
+-rw-r--r--   0        0        0     6644 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/filter_bbox.json
+-rw-r--r--   0        0        0     4600 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/filter_labels.json
+-rw-r--r--   0        0        0     3572 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/filter_spatial.json
+-rw-r--r--   0        0        0     4640 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/filter_temporal.json
+-rw-r--r--   0        0        0     2047 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/first.json
+-rw-r--r--   0        0        0     3578 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/fit_curve.json
+-rw-r--r--   0        0        0     3985 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/fit_regr_random_forest.json
+-rw-r--r--   0        0        0     1574 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/floor.json
+-rw-r--r--   0        0        0     2645 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/gt.json
+-rw-r--r--   0        0        0     3797 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/gte.json
+-rw-r--r--   0        0        0     2521 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/if.json
+-rw-r--r--   0        0        0     1569 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/int.json
+-rw-r--r--   0        0        0     1132 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/is_infinite.json
+-rw-r--r--   0        0        0     1646 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/is_nan.json
+-rw-r--r--   0        0        0     1398 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/is_nodata.json
+-rw-r--r--   0        0        0     1760 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/is_valid.json
+-rw-r--r--   0        0        0     3586 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/lai.json
+-rw-r--r--   0        0        0     2042 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/last.json
+-rw-r--r--   0        0        0     5011 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/linear_scale_range.json
+-rw-r--r--   0        0        0     2111 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/ln.json
+-rw-r--r--   0        0        0    17245 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/load_collection.json
+-rw-r--r--   0        0        0     1956 2024-05-24 08:57:23.781887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/load_ml_model.json
+-rw-r--r--   0        0        0    17030 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/load_stac.json
+-rw-r--r--   0        0        0     2015 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/load_url.json
+-rw-r--r--   0        0        0     1463 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/load_vector_cube.json
+-rw-r--r--   0        0        0     2322 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/log.json
+-rw-r--r--   0        0        0     2634 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/lt.json
+-rw-r--r--   0        0        0     3787 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/lte.json
+-rw-r--r--   0        0        0     3207 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/mask.json
+-rw-r--r--   0        0        0     4045 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/mask_polygon.json
+-rw-r--r--   0        0        0     2476 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/max.json
+-rw-r--r--   0        0        0     4412 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/mean.json
+-rw-r--r--   0        0        0     4029 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/median.json
+-rw-r--r--   0        0        0     7807 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/merge_cubes.json
+-rw-r--r--   0        0        0    11001 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/meta/implementation.md
+-rw-r--r--   0        0        0    19134 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/meta/subtype-schemas.json
+-rw-r--r--   0        0        0     2408 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/min.json
+-rw-r--r--   0        0        0     4358 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/anomaly.json
+-rw-r--r--   0        0        0    11277 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/apply_neighborhood.json
+-rw-r--r--   0        0        0     4087 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/array_apply.json
+-rw-r--r--   0        0        0     3970 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/climatological_normal.json
+-rw-r--r--   0        0        0     5205 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/filter_bbox.json
+-rw-r--r--   0        0        0     1633 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_dimension.json
+-rw-r--r--   0        0        0     4437 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_labels.json
+-rw-r--r--   0        0        0     6869 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/resample_spatial.json
+-rw-r--r--   0        0        0     3908 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/run_udf.json
+-rw-r--r--   0        0        0     2605 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/text_begins.json
+-rw-r--r--   0        0        0     2573 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/text_contains.json
+-rw-r--r--   0        0        0     2579 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/text_ends.json
+-rw-r--r--   0        0        0     2863 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/text_merge.json
+-rw-r--r--   0        0        0      883 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/trim_cube.json
+-rw-r--r--   0        0        0     2634 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/mod.json
+-rw-r--r--   0        0        0     2564 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/multiply.json
+-rw-r--r--   0        0        0      879 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/nan.json
+-rw-r--r--   0        0        0     6014 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/ndvi.json
+-rw-r--r--   0        0        0     6037 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/neq.json
+-rw-r--r--   0        0        0     2566 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/normalized_difference.json
+-rw-r--r--   0        0        0     1111 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/not.json
+-rw-r--r--   0        0        0     2368 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/or.json
+-rw-r--r--   0        0        0     5506 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/order.json
+-rw-r--r--   0        0        0      686 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/pi.json
+-rw-r--r--   0        0        0     2278 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/power.json
+-rw-r--r--   0        0        0     3907 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/predict_curve.json
+-rw-r--r--   0        0        0     1988 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/predict_random_forest.json
+-rw-r--r--   0        0        0     3035 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/product.json
+-rw-r--r--   0        0        0     5560 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/aggregate_spatial_window.json
+-rw-r--r--   0        0        0     5380 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/ard_normalized_radar_backscatter.json
+-rw-r--r--   0        0        0     6009 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/ard_surface_reflectance.json
+-rw-r--r--   0        0        0     1702 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/array_append.json
+-rw-r--r--   0        0        0     1601 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/array_create_labeled.json
+-rw-r--r--   0        0        0     1454 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/array_find_label.json
+-rw-r--r--   0        0        0     2405 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/array_interpolate_linear.json
+-rw-r--r--   0        0        0     2895 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/atmospheric_correction.json
+-rw-r--r--   0        0        0     2892 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/cloud_detection.json
+-rw-r--r--   0        0        0     2814 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/cummax.json
+-rw-r--r--   0        0        0     2815 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/cummin.json
+-rw-r--r--   0        0        0     2888 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/cumproduct.json
+-rw-r--r--   0        0        0     2777 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/cumsum.json
+-rw-r--r--   0        0        0     5608 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/date_shift.json
+-rw-r--r--   0        0        0     4600 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/filter_labels.json
+-rw-r--r--   0        0        0     2214 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/inspect.json
+-rw-r--r--   0        0        0     1132 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/is_infinite.json
+-rw-r--r--   0        0        0    11705 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/load_result.json
+-rw-r--r--   0        0        0     2292 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/load_uploaded_files.json
+-rw-r--r--   0        0        0     4000 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/resample_cube_temporal.json
+-rw-r--r--   0        0        0     2624 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/run_udf_externally.json
+-rw-r--r--   0        0        0     5986 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/sar_backscatter.json
+-rw-r--r--   0        0        0     5910 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/quantiles.json
+-rw-r--r--   0        0        0     2703 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/rearrange.json
+-rw-r--r--   0        0        0     3471 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/reduce_dimension.json
+-rw-r--r--   0        0        0     3655 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/reduce_spatial.json
+-rw-r--r--   0        0        0     4178 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/resample_cube_spatial.json
+-rw-r--r--   0        0        0     6566 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/resample_spatial.json
+-rw-r--r--   0        0        0     2759 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/round.json
+-rw-r--r--   0        0        0     6628 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sar_backscatter.json
+-rw-r--r--   0        0        0     1181 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/save_ml_model.json
+-rw-r--r--   0        0        0     3077 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/save_result.json
+-rw-r--r--   0        0        0     1094 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/save_vector_cube.json
+-rw-r--r--   0        0        0     3086 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sd.json
+-rw-r--r--   0        0        0     2790 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sen2like.json
+-rw-r--r--   0        0        0     2503 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sgn.json
+-rw-r--r--   0        0        0     1028 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sin.json
+-rw-r--r--   0        0        0     1083 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sinh.json
+-rw-r--r--   0        0        0     5177 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sort.json
+-rw-r--r--   0        0        0     1891 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sqrt.json
+-rw-r--r--   0        0        0     1975 2024-05-24 08:57:23.785887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/subtract.json
+-rw-r--r--   0        0        0     3008 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sum.json
+-rw-r--r--   0        0        0     1114 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tan.json
+-rw-r--r--   0        0        0     1191 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tanh.json
+-rw-r--r--   0        0        0       50 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/.gitignore
+-rw-r--r--   0        0        0      371 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/.words
+-rw-r--r--   0        0        0     2075 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/README.md
+-rw-r--r--   0        0        0     3396 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/docs.html
+-rw-r--r--   0        0        0     1977 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/examples.test.js
+-rw-r--r--   0        0        0     1013 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/package.json
+-rw-r--r--   0        0        0     8960 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/processes.test.js
+-rw-r--r--   0        0        0     1021 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/subtypes-file.test.js
+-rw-r--r--   0        0        0     1929 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/subtypes-schemas.test.js
+-rw-r--r--   0        0        0     4776 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/testHelpers.js
+-rw-r--r--   0        0        0     4488 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/variance.json
+-rw-r--r--   0        0        0     1262 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/vessel_detection.json
+-rw-r--r--   0        0        0     3119 2024-05-24 08:57:23.789887 openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/xor.json
+-rw-r--r--   0        0        0     2456 2024-05-24 08:57:23.349887 openeo_processes_dask-2024.5.3/pyproject.toml
+-rw-r--r--   0        0        0     5481 1970-01-01 00:00:00.000000 openeo_processes_dask-2024.5.3/PKG-INFO
```

### Comparing `openeo_processes_dask-2024.5.2/LICENSE` & `openeo_processes_dask-2024.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/README.md` & `openeo_processes_dask-2024.5.3/README.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/__init__.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/arrays.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/arrays.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/comparison.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/comparison.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/core.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/core.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/_filter.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/_filter.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/_xr_interop.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/_xr_interop.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/aggregate.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/aggregate.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/apply.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/apply.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/experimental.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/experimental.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/general.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/general.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/indices.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/indices.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/load.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/load.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/mask.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/mask.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/mask_polygon.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/mask_polygon.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/merge.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/merge.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/reduce.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/reduce.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/cubes/resample.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/cubes/resample.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,20 +49,20 @@
         raise OpenEOException(
             f'Selected resampling method "{method}" is not available! Please select one of '
             f"[{', '.join(resample_methods_list)}]"
         )
 
     dims = list(data.dims)
 
-    known_dims = [
-        data.openeo.band_dims[0],
-        data.openeo.temporal_dims[0],
-        data.openeo.y_dim,
-        data.openeo.x_dim,
-    ]
+    known_dims = []
+    if len(data.openeo.band_dims) > 0:
+        known_dims.append(data.openeo.band_dims[0])
+    if len(data.openeo.temporal_dims) > 0:
+        known_dims.append(data.openeo.temporal_dims[0])
+    known_dims += [data.openeo.y_dim, data.openeo.x_dim]
 
     other_dims = [dim for dim in dims if dim not in known_dims]
 
     data_cp = data.transpose(*other_dims, *known_dims)
 
     if projection is None:
         projection = data_cp.rio.crs
```

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/exceptions.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/exceptions.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/logic.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/logic.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/math.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/math.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/ml/curve_fitting.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/ml/curve_fitting.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/process_implementations/ml/random_forest.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/process_implementations/ml/random_forest.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/__init__.py` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-parameter.md` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-parameter.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-proposal.md` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/.github/ISSUE_TEMPLATE/new-process-proposal.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/.github/workflows/docs.yml` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/CHANGELOG.md` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/LICENSE` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/LICENSE`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/README.md` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/README.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/absolute.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/absolute.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/adaptive_threshold.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/adaptive_threshold.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/add.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/add.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/add_dimension.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/add_dimension.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/aggregate_spatial.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/aggregate_spatial.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/aggregate_temporal.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/aggregate_temporal.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/aggregate_temporal_period.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/aggregate_temporal_period.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/all.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/all.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/and.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/and.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/any.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/any.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/apply.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/apply.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/apply_dimension.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/apply_dimension.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/apply_kernel.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/apply_kernel.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/arccos.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/arccos.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/arcosh.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/arcosh.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/arcsin.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/arcsin.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/arctan.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/arctan.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/arctan2.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/arctan2.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/ard_normalized_radar_backscatter.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/ard_normalized_radar_backscatter.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/ard_surface_reflectance.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/ard_surface_reflectance.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_append.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_append.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_concat.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_concat.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_contains.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_contains.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_create.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_create.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_element.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_element.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_filter.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_filter.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_find.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_find.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_labels.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_labels.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/array_modify.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/array_modify.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/arsinh.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/arsinh.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/artanh.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/artanh.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/atmospheric_correction.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/atmospheric_correction.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/between.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/between.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/cab.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/cab.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/ceil.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/ceil.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/clip.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/clip.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/constant.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/constant.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/cos.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/cos.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/cosh.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/cosh.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/count.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/count.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/create_raster_cube.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/create_raster_cube.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/dimension_labels.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/dimension_labels.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/divide.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/divide.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/drop_dimension.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/drop_dimension.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/e.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/e.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/eq.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/eq.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/examples/array_contains_nodata.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/examples/array_contains_nodata.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/examples/array_find_nodata.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/examples/array_find_nodata.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/examples/rename-enumerated-labels.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/examples/rename-enumerated-labels.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/exp.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/exp.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/extrema.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/extrema.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/fapar.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/fapar.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/fcover.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/fcover.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/filter_bands.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/filter_bands.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/filter_bbox.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/filter_bbox.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/filter_labels.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/filter_labels.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/filter_spatial.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/filter_spatial.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/filter_temporal.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/filter_temporal.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/first.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/first.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/fit_curve.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/fit_curve.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/fit_regr_random_forest.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/fit_regr_random_forest.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/floor.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/floor.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/gt.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/gt.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/gte.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/gte.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/if.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/if.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/int.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/int.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/is_infinite.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/is_infinite.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/is_nan.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/is_nan.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/is_nodata.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/is_nodata.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/is_valid.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/is_valid.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/lai.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/lai.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/last.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/last.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/linear_scale_range.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/linear_scale_range.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/ln.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/ln.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/load_collection.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/load_collection.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/load_ml_model.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/load_ml_model.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/load_stac.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/load_stac.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/load_url.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/load_url.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/load_vector_cube.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/load_vector_cube.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/log.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/log.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/lt.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/lt.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/lte.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/lte.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/mask.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/mask.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/mask_polygon.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/mask_polygon.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/max.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/max.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/mean.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/mean.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/median.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/median.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/merge_cubes.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/merge_cubes.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/meta/implementation.md` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/meta/implementation.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/meta/subtype-schemas.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/meta/subtype-schemas.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/min.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/min.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/anomaly.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/anomaly.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/apply_neighborhood.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/apply_neighborhood.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/array_apply.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/array_apply.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/climatological_normal.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/climatological_normal.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/filter_bbox.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/filter_bbox.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_dimension.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_dimension.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_labels.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/rename_labels.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/resample_spatial.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/resample_spatial.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/run_udf.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/run_udf.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/text_begins.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/text_begins.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/text_contains.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/text_contains.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/text_ends.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/text_ends.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/text_merge.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/text_merge.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/missing-processes/trim_cube.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/missing-processes/trim_cube.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/mod.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/mod.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/multiply.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/multiply.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/nan.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/nan.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/ndvi.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/ndvi.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/neq.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/neq.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/normalized_difference.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/normalized_difference.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/not.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/not.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/or.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/or.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/order.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/order.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/pi.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/pi.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/power.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/power.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/predict_curve.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/predict_curve.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/predict_random_forest.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/predict_random_forest.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/product.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/product.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/aggregate_spatial_window.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/aggregate_spatial_window.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/ard_normalized_radar_backscatter.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/ard_normalized_radar_backscatter.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/ard_surface_reflectance.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/ard_surface_reflectance.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/array_append.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/array_append.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/array_create_labeled.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/array_create_labeled.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/array_find_label.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/array_find_label.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/array_interpolate_linear.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/array_interpolate_linear.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/atmospheric_correction.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/atmospheric_correction.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/cloud_detection.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/cloud_detection.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/cummax.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/cummax.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/cummin.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/cummin.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/cumproduct.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/cumproduct.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/cumsum.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/cumsum.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/date_shift.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/date_shift.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/filter_labels.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/filter_labels.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/inspect.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/inspect.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/is_infinite.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/is_infinite.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/load_result.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/load_result.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/load_uploaded_files.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/load_uploaded_files.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/resample_cube_temporal.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/resample_cube_temporal.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/run_udf_externally.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/run_udf_externally.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/proposals/sar_backscatter.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/proposals/sar_backscatter.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/quantiles.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/quantiles.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/rearrange.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/rearrange.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/reduce_dimension.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/reduce_dimension.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/reduce_spatial.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/reduce_spatial.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/resample_cube_spatial.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/resample_cube_spatial.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/resample_spatial.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/resample_spatial.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/round.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/round.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sar_backscatter.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sar_backscatter.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/save_ml_model.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/save_ml_model.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/save_result.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/save_result.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/save_vector_cube.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/save_vector_cube.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sd.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sd.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sen2like.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sen2like.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sgn.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sgn.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sin.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sin.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sinh.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sinh.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sort.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sort.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sqrt.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sqrt.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/subtract.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/subtract.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/sum.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/sum.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tan.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tan.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tanh.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tanh.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/README.md` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/README.md`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/docs.html` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/docs.html`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/examples.test.js` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/examples.test.js`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/package.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/package.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/processes.test.js` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/processes.test.js`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/subtypes-file.test.js` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/subtypes-file.test.js`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/subtypes-schemas.test.js` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/subtypes-schemas.test.js`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/tests/testHelpers.js` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/tests/testHelpers.js`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/variance.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/variance.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/vessel_detection.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/vessel_detection.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/openeo_processes_dask/specs/openeo-processes/xor.json` & `openeo_processes_dask-2024.5.3/openeo_processes_dask/specs/openeo-processes/xor.json`

 * *Files identical despite different names*

### Comparing `openeo_processes_dask-2024.5.2/pyproject.toml` & `openeo_processes_dask-2024.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openeo-processes-dask"
-version = "2024.5.2"
+version = "2024.5.3"
 description = "Python implementations of many OpenEO processes, dask-friendly by default."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/Open-EO/openeo-processes-dask"
 classifiers = [
```

### Comparing `openeo_processes_dask-2024.5.2/PKG-INFO` & `openeo_processes_dask-2024.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openeo-processes-dask
-Version: 2024.5.2
+Version: 2024.5.3
 Summary: Python implementations of many OpenEO processes, dask-friendly by default.
 Home-page: https://github.com/Open-EO/openeo-processes-dask
 License: Apache 2.0
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
```

