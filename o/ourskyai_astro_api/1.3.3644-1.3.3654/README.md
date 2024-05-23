# Comparing `tmp/ourskyai_astro_api-1.3.3644.tar.gz` & `tmp/ourskyai_astro_api-1.3.3654.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_astro_api-1.3.3644.tar", max compression
+gzip compressed data, was "ourskyai_astro_api-1.3.3654.tar", max compression
```

## Comparing `ourskyai_astro_api-1.3.3644.tar` & `ourskyai_astro_api-1.3.3654.tar`

### file list

```diff
@@ -1,73 +1,77 @@
--rw-r--r--   0        0        0    11093 2024-05-22 19:37:35.265254 ourskyai_astro_api-1.3.3644/README.md
--rw-r--r--   0        0        0     5802 2024-05-22 19:37:38.657292 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/__init__.py
--rw-r--r--   0        0        0      106 2024-05-22 19:37:38.689292 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api/__init__.py
--rw-r--r--   0        0        0   253842 2024-05-22 19:37:38.929294 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api/default_api.py
--rw-r--r--   0        0        0    30352 2024-05-22 19:37:38.993295 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-22 19:37:39.041296 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api_response.py
--rw-r--r--   0        0        0    14687 2024-05-22 19:37:39.101297 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/configuration.py
--rw-r--r--   0        0        0     5433 2024-05-22 19:37:39.189297 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/exceptions.py
--rw-r--r--   0        0        0     5161 2024-05-22 19:37:39.233298 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/__init__.py
--rw-r--r--   0        0        0      819 2024-05-22 19:37:39.361299 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/asset_file_type.py
--rw-r--r--   0        0        0      931 2024-05-22 19:37:39.449300 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/asset_type.py
--rw-r--r--   0        0        0      809 2024-05-22 19:37:39.509301 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/calibration_master_type.py
--rw-r--r--   0        0        0     1904 2024-05-22 19:37:39.549301 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/empty_success.py
--rw-r--r--   0        0        0     1186 2024-05-22 19:37:39.637302 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/filter_type.py
--rw-r--r--   0        0        0     1930 2024-05-22 19:37:39.689303 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/fits_header.py
--rw-r--r--   0        0        0     2155 2024-05-22 19:37:39.781304 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/location.py
--rw-r--r--   0        0        0      747 2024-05-22 19:37:39.833305 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/mount_type.py
--rw-r--r--   0        0        0      887 2024-05-22 19:37:39.897305 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/node_state.py
--rw-r--r--   0        0        0      827 2024-05-22 19:37:39.949306 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/optical_tube_type.py
--rw-r--r--   0        0        0      751 2024-05-22 19:37:40.021307 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/shutter_type.py
--rw-r--r--   0        0        0     1892 2024-05-22 19:37:40.077307 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/successful_create.py
--rw-r--r--   0        0        0      768 2024-05-22 19:37:40.129308 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/tracking_type.py
--rw-r--r--   0        0        0     3258 2024-05-22 19:37:40.229309 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project.py
--rw-r--r--   0        0        0     3969 2024-05-22 19:37:40.285309 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project_asset.py
--rw-r--r--   0        0        0     2569 2024-05-22 19:37:40.333310 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
--rw-r--r--   0        0        0     2399 2024-05-22 19:37:40.425311 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
--rw-r--r--   0        0        0     2381 2024-05-22 19:37:40.469311 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_target.py
--rw-r--r--   0        0        0     3640 2024-05-22 19:37:40.529312 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_calibration_master.py
--rw-r--r--   0        0        0     4908 2024-05-22 19:37:40.609313 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_camera.py
--rw-r--r--   0        0        0     2421 2024-05-22 19:37:40.653313 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
--rw-r--r--   0        0        0     2668 2024-05-22 19:37:40.693314 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_astro_project_request.py
--rw-r--r--   0        0        0     2121 2024-05-22 19:37:40.745314 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_astro_project_response.py
--rw-r--r--   0        0        0     3777 2024-05-22 19:37:40.797315 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_calibration_master_request.py
--rw-r--r--   0        0        0     2147 2024-05-22 19:37:40.861316 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_calibration_master_response.py
--rw-r--r--   0        0        0     7059 2024-05-22 19:37:40.929317 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_camera_request.py
--rw-r--r--   0        0        0     2044 2024-05-22 19:37:40.981317 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2115 2024-05-22 19:37:41.053318 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2683 2024-05-22 19:37:41.161319 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2296 2024-05-22 19:37:41.209320 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     3146 2024-05-22 19:37:41.245320 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2447 2024-05-22 19:37:41.289321 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2441 2024-05-22 19:37:41.337321 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0     3289 2024-05-22 19:37:41.377321 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2051 2024-05-22 19:37:41.433322 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2096 2024-05-22 19:37:41.481323 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
--rw-r--r--   0        0        0     2364 2024-05-22 19:37:41.537323 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7066 2024-05-22 19:37:41.577324 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2324 2024-05-22 19:37:41.629324 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2513 2024-05-22 19:37:41.689325 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     3436 2024-05-22 19:37:41.785326 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5797 2024-05-22 19:37:41.825326 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0      795 2024-05-22 19:37:41.893327 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_job_kind.py
--rw-r--r--   0        0        0     2632 2024-05-22 19:37:41.945328 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_job_log.py
--rw-r--r--   0        0        0      803 2024-05-22 19:37:42.153330 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_job_status.py
--rw-r--r--   0        0        0     1914 2024-05-22 19:37:42.237331 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_mount.py
--rw-r--r--   0        0        0     4458 2024-05-22 19:37:42.325332 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_node.py
--rw-r--r--   0        0        0     2564 2024-05-22 19:37:42.377332 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     2239 2024-05-22 19:37:42.461333 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     3057 2024-05-22 19:37:42.529334 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit.py
--rw-r--r--   0        0        0      870 2024-05-22 19:37:42.597335 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit_source.py
--rw-r--r--   0        0        0      800 2024-05-22 19:37:42.653335 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit_type.py
--rw-r--r--   0        0        0      776 2024-05-22 19:37:42.705336 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit_unit.py
--rw-r--r--   0        0        0     2045 2024-05-22 19:37:42.745336 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
--rw-r--r--   0        0        0     2051 2024-05-22 19:37:42.813337 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2050 2024-05-22 19:37:42.869338 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2940 2024-05-22 19:37:42.925338 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2240 2024-05-22 19:37:42.973339 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     4605 2024-05-22 19:37:43.029340 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2522 2024-05-22 19:37:43.073340 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0        0 2024-05-22 19:37:43.105340 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/py.typed
--rw-r--r--   0        0        0    12935 2024-05-22 19:37:43.145341 ourskyai_astro_api-1.3.3644/ourskyai_astro_api/rest.py
--rw-r--r--   0        0        0      739 2024-05-22 19:37:43.205341 ourskyai_astro_api-1.3.3644/pyproject.toml
--rw-r--r--   0        0        0    12061 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3644/PKG-INFO
+-rw-r--r--   0        0        0    11493 2024-05-23 19:26:18.682597 ourskyai_astro_api-1.3.3654/README.md
+-rw-r--r--   0        0        0     6218 2024-05-23 19:26:22.446235 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-23 19:26:22.482232 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api/__init__.py
+-rw-r--r--   0        0        0   260295 2024-05-23 19:26:22.582222 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api/default_api.py
+-rw-r--r--   0        0        0    30352 2024-05-23 19:26:22.630218 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-23 19:26:22.718209 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api_response.py
+-rw-r--r--   0        0        0    14687 2024-05-23 19:26:22.826199 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/configuration.py
+-rw-r--r--   0        0        0     5433 2024-05-23 19:26:22.874194 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/exceptions.py
+-rw-r--r--   0        0        0     5577 2024-05-23 19:26:22.918190 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-23 19:26:22.962186 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/asset_file_type.py
+-rw-r--r--   0        0        0      931 2024-05-23 19:26:23.010181 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/asset_type.py
+-rw-r--r--   0        0        0      809 2024-05-23 19:26:23.066176 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/calibration_master_type.py
+-rw-r--r--   0        0        0     4308 2024-05-23 19:26:23.126170 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/daily_weather_forecast_item.py
+-rw-r--r--   0        0        0     2527 2024-05-23 19:26:23.210162 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py
+-rw-r--r--   0        0        0     2551 2024-05-23 19:26:23.246158 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py
+-rw-r--r--   0        0        0     2562 2024-05-23 19:26:23.290154 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/daily_weather_forecast_list_response.py
+-rw-r--r--   0        0        0     1904 2024-05-23 19:26:23.350149 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/empty_success.py
+-rw-r--r--   0        0        0     1186 2024-05-23 19:26:23.386145 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/filter_type.py
+-rw-r--r--   0        0        0     1930 2024-05-23 19:26:23.430141 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/fits_header.py
+-rw-r--r--   0        0        0     2155 2024-05-23 19:26:23.490135 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/location.py
+-rw-r--r--   0        0        0      747 2024-05-23 19:26:23.530131 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/mount_type.py
+-rw-r--r--   0        0        0      887 2024-05-23 19:26:23.642120 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/node_state.py
+-rw-r--r--   0        0        0      827 2024-05-23 19:26:23.678117 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0      751 2024-05-23 19:26:23.738111 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1892 2024-05-23 19:26:23.798105 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/successful_create.py
+-rw-r--r--   0        0        0      768 2024-05-23 19:26:23.886097 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/tracking_type.py
+-rw-r--r--   0        0        0     3258 2024-05-23 19:26:23.970089 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project.py
+-rw-r--r--   0        0        0     3969 2024-05-23 19:26:24.014085 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project_asset.py
+-rw-r--r--   0        0        0     2569 2024-05-23 19:26:24.066080 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
+-rw-r--r--   0        0        0     2399 2024-05-23 19:26:24.122074 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
+-rw-r--r--   0        0        0     2381 2024-05-23 19:26:24.186068 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_target.py
+-rw-r--r--   0        0        0     3640 2024-05-23 19:26:24.238063 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_calibration_master.py
+-rw-r--r--   0        0        0     4908 2024-05-23 19:26:24.290058 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2421 2024-05-23 19:26:24.330054 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
+-rw-r--r--   0        0        0     2668 2024-05-23 19:26:24.398048 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_astro_project_request.py
+-rw-r--r--   0        0        0     2121 2024-05-23 19:26:24.434044 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_astro_project_response.py
+-rw-r--r--   0        0        0     3777 2024-05-23 19:26:24.474040 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_calibration_master_request.py
+-rw-r--r--   0        0        0     2147 2024-05-23 19:26:24.518036 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_calibration_master_response.py
+-rw-r--r--   0        0        0     7059 2024-05-23 19:26:24.582030 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_camera_request.py
+-rw-r--r--   0        0        0     2044 2024-05-23 19:26:24.638025 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2115 2024-05-23 19:26:24.690020 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2683 2024-05-23 19:26:24.738015 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2296 2024-05-23 19:26:24.798009 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     3146 2024-05-23 19:26:24.854004 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2447 2024-05-23 19:26:24.917998 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2441 2024-05-23 19:26:24.973992 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0     3289 2024-05-23 19:26:25.013989 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2051 2024-05-23 19:26:25.061984 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2096 2024-05-23 19:26:25.133977 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
+-rw-r--r--   0        0        0     2364 2024-05-23 19:26:25.181972 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7066 2024-05-23 19:26:25.209970 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2324 2024-05-23 19:26:25.289962 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2513 2024-05-23 19:26:25.321959 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     3436 2024-05-23 19:26:25.365955 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5797 2024-05-23 19:26:25.409951 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0      795 2024-05-23 19:26:25.441947 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_job_kind.py
+-rw-r--r--   0        0        0     2632 2024-05-23 19:26:25.485943 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_job_log.py
+-rw-r--r--   0        0        0      803 2024-05-23 19:26:25.573935 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_job_status.py
+-rw-r--r--   0        0        0     1914 2024-05-23 19:26:25.621930 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4458 2024-05-23 19:26:25.701923 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_node.py
+-rw-r--r--   0        0        0     2564 2024-05-23 19:26:25.753917 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     2239 2024-05-23 19:26:25.805912 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     3057 2024-05-23 19:26:25.889904 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit.py
+-rw-r--r--   0        0        0      870 2024-05-23 19:26:25.949899 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit_source.py
+-rw-r--r--   0        0        0      800 2024-05-23 19:26:25.985895 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit_type.py
+-rw-r--r--   0        0        0      776 2024-05-23 19:26:26.065888 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit_unit.py
+-rw-r--r--   0        0        0     2045 2024-05-23 19:26:26.121882 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
+-rw-r--r--   0        0        0     2051 2024-05-23 19:26:26.157878 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2050 2024-05-23 19:26:26.221872 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2940 2024-05-23 19:26:26.269868 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2240 2024-05-23 19:26:26.313864 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     4605 2024-05-23 19:26:26.373858 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2522 2024-05-23 19:26:26.437852 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:26:26.469848 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/py.typed
+-rw-r--r--   0        0        0    12935 2024-05-23 19:26:26.513844 ourskyai_astro_api-1.3.3654/ourskyai_astro_api/rest.py
+-rw-r--r--   0        0        0      739 2024-05-23 19:26:26.573839 ourskyai_astro_api-1.3.3654/pyproject.toml
+-rw-r--r--   0        0        0    12461 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3654/PKG-INFO
```

### Comparing `ourskyai_astro_api-1.3.3644/README.md` & `ourskyai_astro_api-1.3.3654/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-astro-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3644
-- Package version: 1.3.3644
+- API version: 1.3.3654
+- Package version: 1.3.3654
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -120,26 +120,31 @@
 *DefaultApi* | [**v1_get_image_sets**](docs/DefaultApi.md#v1_get_image_sets) | **GET** /v1/image-sets | 
 *DefaultApi* | [**v1_get_job_logs**](docs/DefaultApi.md#v1_get_job_logs) | **GET** /v1/job-logs | 
 *DefaultApi* | [**v1_get_nodes**](docs/DefaultApi.md#v1_get_nodes) | **GET** /v1/nodes | 
 *DefaultApi* | [**v1_get_or_create_camera**](docs/DefaultApi.md#v1_get_or_create_camera) | **PUT** /v1/camera-match | 
 *DefaultApi* | [**v1_get_or_create_mount**](docs/DefaultApi.md#v1_get_or_create_mount) | **PUT** /v1/mount-match | 
 *DefaultApi* | [**v1_get_or_create_optical_tube**](docs/DefaultApi.md#v1_get_or_create_optical_tube) | **PUT** /v1/optical-tube-match | 
 *DefaultApi* | [**v1_get_platform_credits**](docs/DefaultApi.md#v1_get_platform_credits) | **GET** /v1/platform-credits | 
+*DefaultApi* | [**v1_get_weather**](docs/DefaultApi.md#v1_get_weather) | **GET** /v1/weather | 
 *DefaultApi* | [**v1_match_astro_project**](docs/DefaultApi.md#v1_match_astro_project) | **GET** /v1/astro-project-match | 
 *DefaultApi* | [**v1_mount_match**](docs/DefaultApi.md#v1_mount_match) | **GET** /v1/mount-match | 
 *DefaultApi* | [**v1_optical_tube_match**](docs/DefaultApi.md#v1_optical_tube_match) | **GET** /v1/optical-tube-match | 
 *DefaultApi* | [**v1_put_stack_astro_project**](docs/DefaultApi.md#v1_put_stack_astro_project) | **PUT** /v1/stack-astro-project | 
 *DefaultApi* | [**v1_update_node**](docs/DefaultApi.md#v1_update_node) | **PUT** /v1/node | 
 
 
 ## Documentation For Models
 
  - [AssetFileType](docs/AssetFileType.md)
  - [AssetType](docs/AssetType.md)
  - [CalibrationMasterType](docs/CalibrationMasterType.md)
+ - [DailyWeatherForecastItem](docs/DailyWeatherForecastItem.md)
+ - [DailyWeatherForecastItemTemp](docs/DailyWeatherForecastItemTemp.md)
+ - [DailyWeatherForecastItemWeatherInner](docs/DailyWeatherForecastItemWeatherInner.md)
+ - [DailyWeatherForecastListResponse](docs/DailyWeatherForecastListResponse.md)
  - [EmptySuccess](docs/EmptySuccess.md)
  - [FilterType](docs/FilterType.md)
  - [FitsHeader](docs/FitsHeader.md)
  - [Location](docs/Location.md)
  - [MountType](docs/MountType.md)
  - [NodeState](docs/NodeState.md)
  - [OpticalTubeType](docs/OpticalTubeType.md)
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/__init__.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3644"
+__version__ = "1.3.3654"
 
 # import apis into sdk package
 from ourskyai_astro_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_astro_api.api_response import ApiResponse
 from ourskyai_astro_api.api_client import ApiClient
@@ -30,14 +30,18 @@
 from ourskyai_astro_api.exceptions import ApiAttributeError
 from ourskyai_astro_api.exceptions import ApiException
 
 # import models into sdk package
 from ourskyai_astro_api.models.asset_file_type import AssetFileType
 from ourskyai_astro_api.models.asset_type import AssetType
 from ourskyai_astro_api.models.calibration_master_type import CalibrationMasterType
+from ourskyai_astro_api.models.daily_weather_forecast_item import DailyWeatherForecastItem
+from ourskyai_astro_api.models.daily_weather_forecast_item_temp import DailyWeatherForecastItemTemp
+from ourskyai_astro_api.models.daily_weather_forecast_item_weather_inner import DailyWeatherForecastItemWeatherInner
+from ourskyai_astro_api.models.daily_weather_forecast_list_response import DailyWeatherForecastListResponse
 from ourskyai_astro_api.models.empty_success import EmptySuccess
 from ourskyai_astro_api.models.filter_type import FilterType
 from ourskyai_astro_api.models.fits_header import FitsHeader
 from ourskyai_astro_api.models.location import Location
 from ourskyai_astro_api.models.mount_type import MountType
 from ourskyai_astro_api.models.node_state import NodeState
 from ourskyai_astro_api.models.optical_tube_type import OpticalTubeType
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api/default_api.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
@@ -18,14 +18,15 @@
 
 from pydantic import validate_arguments, ValidationError
 
 from pydantic import StrictBool, StrictFloat, StrictInt, StrictStr, conlist
 
 from typing import List, Optional, Union
 
+from ourskyai_astro_api.models.daily_weather_forecast_list_response import DailyWeatherForecastListResponse
 from ourskyai_astro_api.models.empty_success import EmptySuccess
 from ourskyai_astro_api.models.successful_create import SuccessfulCreate
 from ourskyai_astro_api.models.v1_astro_project import V1AstroProject
 from ourskyai_astro_api.models.v1_astro_project_asset import V1AstroProjectAsset
 from ourskyai_astro_api.models.v1_astro_target import V1AstroTarget
 from ourskyai_astro_api.models.v1_calibration_master import V1CalibrationMaster
 from ourskyai_astro_api.models.v1_camera import V1Camera
@@ -5096,14 +5097,162 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def v1_get_weather(self, latitude : Union[StrictFloat, StrictInt], longitude : Union[StrictFloat, StrictInt], **kwargs) -> DailyWeatherForecastListResponse:  # noqa: E501
+        """v1_get_weather  # noqa: E501
+
+        Get weather.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_get_weather(latitude, longitude, async_req=True)
+        >>> result = thread.get()
+
+        :param latitude: (required)
+        :type latitude: float
+        :param longitude: (required)
+        :type longitude: float
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: DailyWeatherForecastListResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the v1_get_weather_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        return self.v1_get_weather_with_http_info(latitude, longitude, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def v1_get_weather_with_http_info(self, latitude : Union[StrictFloat, StrictInt], longitude : Union[StrictFloat, StrictInt], **kwargs) -> ApiResponse:  # noqa: E501
+        """v1_get_weather  # noqa: E501
+
+        Get weather.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_get_weather_with_http_info(latitude, longitude, async_req=True)
+        >>> result = thread.get()
+
+        :param latitude: (required)
+        :type latitude: float
+        :param longitude: (required)
+        :type longitude: float
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(DailyWeatherForecastListResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'latitude',
+            'longitude'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_get_weather" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('latitude') is not None:  # noqa: E501
+            _query_params.append(('latitude', _params['latitude']))
+
+        if _params.get('longitude') is not None:  # noqa: E501
+            _query_params.append(('longitude', _params['longitude']))
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['Roles', 'BearerToken']  # noqa: E501
+
+        _response_types_map = {
+            '200': "DailyWeatherForecastListResponse",
+        }
+
+        return self.api_client.call_api(
+            '/v1/weather', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api_client.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.3.3644/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3654/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/api_response.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/configuration.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -371,16 +371,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.3.3644\n"\
-               "SDK Package Version: 1.3.3644".\
+               "Version of the API: 1.3.3654\n"\
+               "SDK Package Version: 1.3.3654".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/exceptions.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/__init__.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 
 # flake8: noqa
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from ourskyai_astro_api.models.asset_file_type import AssetFileType
 from ourskyai_astro_api.models.asset_type import AssetType
 from ourskyai_astro_api.models.calibration_master_type import CalibrationMasterType
+from ourskyai_astro_api.models.daily_weather_forecast_item import DailyWeatherForecastItem
+from ourskyai_astro_api.models.daily_weather_forecast_item_temp import DailyWeatherForecastItemTemp
+from ourskyai_astro_api.models.daily_weather_forecast_item_weather_inner import DailyWeatherForecastItemWeatherInner
+from ourskyai_astro_api.models.daily_weather_forecast_list_response import DailyWeatherForecastListResponse
 from ourskyai_astro_api.models.empty_success import EmptySuccess
 from ourskyai_astro_api.models.filter_type import FilterType
 from ourskyai_astro_api.models.fits_header import FitsHeader
 from ourskyai_astro_api.models.location import Location
 from ourskyai_astro_api.models.mount_type import MountType
 from ourskyai_astro_api.models.node_state import NodeState
 from ourskyai_astro_api.models.optical_tube_type import OpticalTubeType
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/asset_file_type.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/asset_file_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/asset_type.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/asset_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/calibration_master_type.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/calibration_master_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/empty_success.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/empty_success.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/filter_type.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/filter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/fits_header.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/fits_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/location.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/mount_type.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/mount_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/node_state.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/node_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/optical_tube_type.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/optical_tube_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/shutter_type.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/shutter_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/successful_create.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/successful_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/tracking_type.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_job_kind.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,25 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class TrackingType(str, Enum):
+class V1JobKind(str, Enum):
     """
-    TrackingType
+    V1JobKind
     """
 
     """
     allowed enum values
     """
-    SIDEREAL = 'SIDEREAL'
-    TARGET_RATE = 'TARGET_RATE'
+    STACK = 'STACK'
+    REPROCESS = 'REPROCESS'
+    OBSERVATION_POTENTIAL = 'OBSERVATION_POTENTIAL'
 
     @classmethod
-    def from_json(cls, json_str: str) -> TrackingType:
-        """Create an instance of TrackingType from a JSON string"""
-        return TrackingType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1JobKind:
+        """Create an instance of V1JobKind from a JSON string"""
+        return V1JobKind(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project_asset.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project_asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_astro_target.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_astro_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_calibration_master.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_calibration_master.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_camera.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_astro_project_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_astro_project_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_astro_project_response.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_astro_project_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_calibration_master_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_calibration_master_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_calibration_master_response.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_calibration_master_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_camera_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_image_set_image_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_image_set_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_image_set_image_response.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_image_set_image_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_image_set_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_image_set_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_mount_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_node_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_create_optical_tube_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_elevation_mask_point.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_elevation_mask_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_gain_curve.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_gain_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_gain_curve_point.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_gain_curve_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_nodes.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_or_create_camera_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_or_create_camera_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_or_create_mount_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_or_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_image_set.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_image_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_image_set_image.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_job_kind.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_job_status.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,25 +17,26 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1JobKind(str, Enum):
+class V1JobStatus(str, Enum):
     """
-    V1JobKind
+    V1JobStatus
     """
 
     """
     allowed enum values
     """
-    STACK = 'STACK'
-    REPROCESS = 'REPROCESS'
-    OBSERVATION_POTENTIAL = 'OBSERVATION_POTENTIAL'
+    PENDING = 'PENDING'
+    RUNNING = 'RUNNING'
+    SUCCEEDED = 'SUCCEEDED'
+    FAILED = 'FAILED'
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1JobKind:
-        """Create an instance of V1JobKind from a JSON string"""
-        return V1JobKind(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1JobStatus:
+        """Create an instance of V1JobStatus from a JSON string"""
+        return V1JobStatus(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_job_log.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_job_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_job_status.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/tracking_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,26 +17,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1JobStatus(str, Enum):
+class TrackingType(str, Enum):
     """
-    V1JobStatus
+    TrackingType
     """
 
     """
     allowed enum values
     """
-    PENDING = 'PENDING'
-    RUNNING = 'RUNNING'
-    SUCCEEDED = 'SUCCEEDED'
-    FAILED = 'FAILED'
+    SIDEREAL = 'SIDEREAL'
+    TARGET_RATE = 'TARGET_RATE'
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1JobStatus:
-        """Create an instance of V1JobStatus from a JSON string"""
-        return V1JobStatus(json.loads(json_str))
+    def from_json(cls, json_str: str) -> TrackingType:
+        """Create an instance of TrackingType from a JSON string"""
+        return TrackingType(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_mount.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_node.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_node_with_location.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_node_with_location.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_optical_tube.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit_source.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit_type.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_platform_credit_unit.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_platform_credit_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_read_noise_point.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_read_noise_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_setup_action.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_setup_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_slew_timing.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_slew_timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_slew_timing_interval.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_slew_timing_interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_update_node_request.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_update_node_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/models/v1_video_mode_framerate_property.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/models/v1_video_mode_framerate_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3644/ourskyai_astro_api/rest.py` & `ourskyai_astro_api-1.3.3654/ourskyai_astro_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3644
+    The version of the OpenAPI document: 1.3.3654
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_astro_api-1.3.3644/pyproject.toml` & `ourskyai_astro_api-1.3.3654/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_astro_api"
-version = "1.3.3644"
+version = "1.3.3654"
 description = "OurSky Astro"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Astro"]
 include = ["ourskyai_astro_api/py.typed"]
```

### Comparing `ourskyai_astro_api-1.3.3644/PKG-INFO` & `ourskyai_astro_api-1.3.3654/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_astro_api
-Version: 1.3.3644
+Version: 1.3.3654
 Summary: OurSky Astro
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Astro
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-astro-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3644
-- Package version: 1.3.3644
+- API version: 1.3.3654
+- Package version: 1.3.3654
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -145,26 +145,31 @@
 *DefaultApi* | [**v1_get_image_sets**](docs/DefaultApi.md#v1_get_image_sets) | **GET** /v1/image-sets | 
 *DefaultApi* | [**v1_get_job_logs**](docs/DefaultApi.md#v1_get_job_logs) | **GET** /v1/job-logs | 
 *DefaultApi* | [**v1_get_nodes**](docs/DefaultApi.md#v1_get_nodes) | **GET** /v1/nodes | 
 *DefaultApi* | [**v1_get_or_create_camera**](docs/DefaultApi.md#v1_get_or_create_camera) | **PUT** /v1/camera-match | 
 *DefaultApi* | [**v1_get_or_create_mount**](docs/DefaultApi.md#v1_get_or_create_mount) | **PUT** /v1/mount-match | 
 *DefaultApi* | [**v1_get_or_create_optical_tube**](docs/DefaultApi.md#v1_get_or_create_optical_tube) | **PUT** /v1/optical-tube-match | 
 *DefaultApi* | [**v1_get_platform_credits**](docs/DefaultApi.md#v1_get_platform_credits) | **GET** /v1/platform-credits | 
+*DefaultApi* | [**v1_get_weather**](docs/DefaultApi.md#v1_get_weather) | **GET** /v1/weather | 
 *DefaultApi* | [**v1_match_astro_project**](docs/DefaultApi.md#v1_match_astro_project) | **GET** /v1/astro-project-match | 
 *DefaultApi* | [**v1_mount_match**](docs/DefaultApi.md#v1_mount_match) | **GET** /v1/mount-match | 
 *DefaultApi* | [**v1_optical_tube_match**](docs/DefaultApi.md#v1_optical_tube_match) | **GET** /v1/optical-tube-match | 
 *DefaultApi* | [**v1_put_stack_astro_project**](docs/DefaultApi.md#v1_put_stack_astro_project) | **PUT** /v1/stack-astro-project | 
 *DefaultApi* | [**v1_update_node**](docs/DefaultApi.md#v1_update_node) | **PUT** /v1/node | 
 
 
 ## Documentation For Models
 
  - [AssetFileType](docs/AssetFileType.md)
  - [AssetType](docs/AssetType.md)
  - [CalibrationMasterType](docs/CalibrationMasterType.md)
+ - [DailyWeatherForecastItem](docs/DailyWeatherForecastItem.md)
+ - [DailyWeatherForecastItemTemp](docs/DailyWeatherForecastItemTemp.md)
+ - [DailyWeatherForecastItemWeatherInner](docs/DailyWeatherForecastItemWeatherInner.md)
+ - [DailyWeatherForecastListResponse](docs/DailyWeatherForecastListResponse.md)
  - [EmptySuccess](docs/EmptySuccess.md)
  - [FilterType](docs/FilterType.md)
  - [FitsHeader](docs/FitsHeader.md)
  - [Location](docs/Location.md)
  - [MountType](docs/MountType.md)
  - [NodeState](docs/NodeState.md)
  - [OpticalTubeType](docs/OpticalTubeType.md)
```

