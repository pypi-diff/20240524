# Comparing `tmp/ourskyai_astro_api-1.3.3657.tar.gz` & `tmp/ourskyai_astro_api-1.3.3661.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_astro_api-1.3.3657.tar", max compression
+gzip compressed data, was "ourskyai_astro_api-1.3.3661.tar", max compression
```

## Comparing `ourskyai_astro_api-1.3.3657.tar` & `ourskyai_astro_api-1.3.3661.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rw-r--r--   0        0        0    11493 2024-05-23 23:15:12.509300 ourskyai_astro_api-1.3.3657/README.md
--rw-r--r--   0        0        0     6218 2024-05-23 23:15:15.948699 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/__init__.py
--rw-r--r--   0        0        0      106 2024-05-23 23:15:15.976694 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api/__init__.py
--rw-r--r--   0        0        0   260295 2024-05-23 23:15:16.052681 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api/default_api.py
--rw-r--r--   0        0        0    30352 2024-05-23 23:15:16.096673 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-23 23:15:16.136666 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api_response.py
--rw-r--r--   0        0        0    14687 2024-05-23 23:15:16.172660 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/configuration.py
--rw-r--r--   0        0        0     5433 2024-05-23 23:15:16.208654 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/exceptions.py
--rw-r--r--   0        0        0     5577 2024-05-23 23:15:16.252646 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/__init__.py
--rw-r--r--   0        0        0      819 2024-05-23 23:15:16.292639 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/asset_file_type.py
--rw-r--r--   0        0        0      931 2024-05-23 23:15:16.320634 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/asset_type.py
--rw-r--r--   0        0        0      809 2024-05-23 23:15:16.388622 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/calibration_master_type.py
--rw-r--r--   0        0        0     4308 2024-05-23 23:15:16.440613 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_item.py
--rw-r--r--   0        0        0     2527 2024-05-23 23:15:16.488605 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py
--rw-r--r--   0        0        0     2551 2024-05-23 23:15:16.548594 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py
--rw-r--r--   0        0        0     2562 2024-05-23 23:15:16.600585 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_list_response.py
--rw-r--r--   0        0        0     1904 2024-05-23 23:15:16.652576 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/empty_success.py
--rw-r--r--   0        0        0     1186 2024-05-23 23:15:16.704567 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/filter_type.py
--rw-r--r--   0        0        0     1930 2024-05-23 23:15:16.768556 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/fits_header.py
--rw-r--r--   0        0        0     2155 2024-05-23 23:15:16.824546 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/location.py
--rw-r--r--   0        0        0      747 2024-05-23 23:15:16.864539 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/mount_type.py
--rw-r--r--   0        0        0      887 2024-05-23 23:15:16.932527 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/node_state.py
--rw-r--r--   0        0        0      827 2024-05-23 23:15:16.972520 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/optical_tube_type.py
--rw-r--r--   0        0        0      751 2024-05-23 23:15:17.056506 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/shutter_type.py
--rw-r--r--   0        0        0     1892 2024-05-23 23:15:17.104497 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/successful_create.py
--rw-r--r--   0        0        0      768 2024-05-23 23:15:17.148489 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/tracking_type.py
--rw-r--r--   0        0        0     3258 2024-05-23 23:15:17.240473 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project.py
--rw-r--r--   0        0        0     3969 2024-05-23 23:15:17.284466 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project_asset.py
--rw-r--r--   0        0        0     2569 2024-05-23 23:15:17.348454 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
--rw-r--r--   0        0        0     2399 2024-05-23 23:15:17.392447 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
--rw-r--r--   0        0        0     2381 2024-05-23 23:15:17.452436 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_target.py
--rw-r--r--   0        0        0     3640 2024-05-23 23:15:17.540421 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_calibration_master.py
--rw-r--r--   0        0        0     4908 2024-05-23 23:15:17.596411 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_camera.py
--rw-r--r--   0        0        0     2421 2024-05-23 23:15:17.644403 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
--rw-r--r--   0        0        0     2668 2024-05-23 23:15:17.692394 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_astro_project_request.py
--rw-r--r--   0        0        0     2121 2024-05-23 23:15:17.740386 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_astro_project_response.py
--rw-r--r--   0        0        0     3777 2024-05-23 23:15:17.792377 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_calibration_master_request.py
--rw-r--r--   0        0        0     2147 2024-05-23 23:15:17.832370 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_calibration_master_response.py
--rw-r--r--   0        0        0     7059 2024-05-23 23:15:17.892359 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_camera_request.py
--rw-r--r--   0        0        0     2044 2024-05-23 23:15:17.936352 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2115 2024-05-23 23:15:17.988343 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2683 2024-05-23 23:15:18.044333 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2296 2024-05-23 23:15:18.100323 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     3146 2024-05-23 23:15:18.156313 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2447 2024-05-23 23:15:18.204305 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2441 2024-05-23 23:15:18.256296 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0     3289 2024-05-23 23:15:18.312286 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2051 2024-05-23 23:15:18.380274 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2096 2024-05-23 23:15:18.464259 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
--rw-r--r--   0        0        0     2364 2024-05-23 23:15:18.520250 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7066 2024-05-23 23:15:18.576240 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2324 2024-05-23 23:15:18.608234 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2513 2024-05-23 23:15:18.656226 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     3436 2024-05-23 23:15:18.720215 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5797 2024-05-23 23:15:18.764207 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0      795 2024-05-23 23:15:18.812198 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_job_kind.py
--rw-r--r--   0        0        0     2632 2024-05-23 23:15:18.860190 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_job_log.py
--rw-r--r--   0        0        0      803 2024-05-23 23:15:18.928178 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_job_status.py
--rw-r--r--   0        0        0     1914 2024-05-23 23:15:18.972171 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_mount.py
--rw-r--r--   0        0        0     4458 2024-05-23 23:15:19.020162 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_node.py
--rw-r--r--   0        0        0     2564 2024-05-23 23:15:19.088150 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     2239 2024-05-23 23:15:19.128143 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     3057 2024-05-23 23:15:19.176135 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit.py
--rw-r--r--   0        0        0      870 2024-05-23 23:15:19.232125 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit_source.py
--rw-r--r--   0        0        0      800 2024-05-23 23:15:19.272118 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit_type.py
--rw-r--r--   0        0        0      776 2024-05-23 23:15:19.324109 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit_unit.py
--rw-r--r--   0        0        0     2045 2024-05-23 23:15:19.368101 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
--rw-r--r--   0        0        0     2051 2024-05-23 23:15:19.444088 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2050 2024-05-23 23:15:19.496079 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2940 2024-05-23 23:15:19.548070 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2240 2024-05-23 23:15:19.592062 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     4605 2024-05-23 23:15:19.652052 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2522 2024-05-23 23:15:19.700043 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0        0 2024-05-23 23:15:19.732038 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/py.typed
--rw-r--r--   0        0        0    12935 2024-05-23 23:15:19.780029 ourskyai_astro_api-1.3.3657/ourskyai_astro_api/rest.py
--rw-r--r--   0        0        0      739 2024-05-23 23:15:19.812024 ourskyai_astro_api-1.3.3657/pyproject.toml
--rw-r--r--   0        0        0    12461 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3657/PKG-INFO
+-rw-r--r--   0        0        0    11541 2024-05-24 01:28:40.893336 ourskyai_astro_api-1.3.3661/README.md
+-rw-r--r--   0        0        0     6292 2024-05-24 01:28:44.445374 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-24 01:28:44.481374 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/api/__init__.py
+-rw-r--r--   0        0        0   260295 2024-05-24 01:28:44.589375 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/api/default_api.py
+-rw-r--r--   0        0        0    30352 2024-05-24 01:28:44.633376 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-24 01:28:44.673376 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/api_response.py
+-rw-r--r--   0        0        0    14687 2024-05-24 01:28:44.725377 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/configuration.py
+-rw-r--r--   0        0        0     5433 2024-05-24 01:28:44.761377 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/exceptions.py
+-rw-r--r--   0        0        0     5651 2024-05-24 01:28:44.793377 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-24 01:28:44.837378 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/asset_file_type.py
+-rw-r--r--   0        0        0      931 2024-05-24 01:28:44.937379 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/asset_type.py
+-rw-r--r--   0        0        0      809 2024-05-24 01:28:44.977379 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/calibration_master_type.py
+-rw-r--r--   0        0        0     2092 2024-05-24 01:28:45.037380 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/daily_weather_city.py
+-rw-r--r--   0        0        0     4308 2024-05-24 01:28:45.093380 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/daily_weather_forecast_item.py
+-rw-r--r--   0        0        0     2527 2024-05-24 01:28:45.141381 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py
+-rw-r--r--   0        0        0     2551 2024-05-24 01:28:45.193381 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py
+-rw-r--r--   0        0        0     2947 2024-05-24 01:28:45.245382 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/daily_weather_forecast_list_response.py
+-rw-r--r--   0        0        0     1904 2024-05-24 01:28:45.293382 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/empty_success.py
+-rw-r--r--   0        0        0     1186 2024-05-24 01:28:45.345383 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/filter_type.py
+-rw-r--r--   0        0        0     1930 2024-05-24 01:28:45.401383 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/fits_header.py
+-rw-r--r--   0        0        0     2155 2024-05-24 01:28:45.453384 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/location.py
+-rw-r--r--   0        0        0      747 2024-05-24 01:28:45.501385 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/mount_type.py
+-rw-r--r--   0        0        0      887 2024-05-24 01:28:45.549385 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/node_state.py
+-rw-r--r--   0        0        0      827 2024-05-24 01:28:45.605386 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0      751 2024-05-24 01:28:45.681386 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1892 2024-05-24 01:28:45.729387 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/successful_create.py
+-rw-r--r--   0        0        0      768 2024-05-24 01:28:45.793388 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/tracking_type.py
+-rw-r--r--   0        0        0     3258 2024-05-24 01:28:45.853388 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_astro_project.py
+-rw-r--r--   0        0        0     3969 2024-05-24 01:28:45.901389 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_astro_project_asset.py
+-rw-r--r--   0        0        0     2569 2024-05-24 01:28:45.949389 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
+-rw-r--r--   0        0        0     2399 2024-05-24 01:28:45.997389 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
+-rw-r--r--   0        0        0     2381 2024-05-24 01:28:46.045390 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_astro_target.py
+-rw-r--r--   0        0        0     3640 2024-05-24 01:28:46.101390 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_calibration_master.py
+-rw-r--r--   0        0        0     4908 2024-05-24 01:28:46.165391 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2421 2024-05-24 01:28:46.205392 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
+-rw-r--r--   0        0        0     2668 2024-05-24 01:28:46.253392 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_astro_project_request.py
+-rw-r--r--   0        0        0     2121 2024-05-24 01:28:46.309393 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_astro_project_response.py
+-rw-r--r--   0        0        0     3777 2024-05-24 01:28:46.361393 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_calibration_master_request.py
+-rw-r--r--   0        0        0     2147 2024-05-24 01:28:46.401394 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_calibration_master_response.py
+-rw-r--r--   0        0        0     7059 2024-05-24 01:28:46.457394 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_camera_request.py
+-rw-r--r--   0        0        0     2044 2024-05-24 01:28:46.493394 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2115 2024-05-24 01:28:46.537395 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2683 2024-05-24 01:28:46.589396 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2296 2024-05-24 01:28:46.645396 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     3146 2024-05-24 01:28:46.685397 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2447 2024-05-24 01:28:46.729397 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2441 2024-05-24 01:28:46.781397 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0     3289 2024-05-24 01:28:46.837398 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2051 2024-05-24 01:28:46.881399 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2096 2024-05-24 01:28:46.921399 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
+-rw-r--r--   0        0        0     2364 2024-05-24 01:28:46.961399 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7066 2024-05-24 01:28:47.009400 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2324 2024-05-24 01:28:47.069400 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2513 2024-05-24 01:28:47.149401 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     3436 2024-05-24 01:28:47.201402 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5797 2024-05-24 01:28:47.245402 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0      795 2024-05-24 01:28:47.285403 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_job_kind.py
+-rw-r--r--   0        0        0     2632 2024-05-24 01:28:47.341403 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_job_log.py
+-rw-r--r--   0        0        0      803 2024-05-24 01:28:47.381404 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_job_status.py
+-rw-r--r--   0        0        0     1914 2024-05-24 01:28:47.449404 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4458 2024-05-24 01:28:47.497405 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_node.py
+-rw-r--r--   0        0        0     2564 2024-05-24 01:28:47.533405 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     2239 2024-05-24 01:28:47.573406 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     3057 2024-05-24 01:28:47.625406 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_platform_credit.py
+-rw-r--r--   0        0        0      870 2024-05-24 01:28:47.705407 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_platform_credit_source.py
+-rw-r--r--   0        0        0      800 2024-05-24 01:28:47.769408 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_platform_credit_type.py
+-rw-r--r--   0        0        0      776 2024-05-24 01:28:47.813408 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_platform_credit_unit.py
+-rw-r--r--   0        0        0     2045 2024-05-24 01:28:47.873409 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
+-rw-r--r--   0        0        0     2051 2024-05-24 01:28:47.933409 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2050 2024-05-24 01:28:47.989410 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2940 2024-05-24 01:28:48.045410 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2240 2024-05-24 01:28:48.105411 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     4605 2024-05-24 01:28:48.157411 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2522 2024-05-24 01:28:48.197412 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:28:48.225412 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/py.typed
+-rw-r--r--   0        0        0    12935 2024-05-24 01:28:48.273413 ourskyai_astro_api-1.3.3661/ourskyai_astro_api/rest.py
+-rw-r--r--   0        0        0      739 2024-05-24 01:28:48.317413 ourskyai_astro_api-1.3.3661/pyproject.toml
+-rw-r--r--   0        0        0    12509 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3661/PKG-INFO
```

### Comparing `ourskyai_astro_api-1.3.3657/README.md` & `ourskyai_astro_api-1.3.3661/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-astro-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3657
-- Package version: 1.3.3657
+- API version: 1.3.3661
+- Package version: 1.3.3661
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -133,14 +133,15 @@
 
 
 ## Documentation For Models
 
  - [AssetFileType](docs/AssetFileType.md)
  - [AssetType](docs/AssetType.md)
  - [CalibrationMasterType](docs/CalibrationMasterType.md)
+ - [DailyWeatherCity](docs/DailyWeatherCity.md)
  - [DailyWeatherForecastItem](docs/DailyWeatherForecastItem.md)
  - [DailyWeatherForecastItemTemp](docs/DailyWeatherForecastItemTemp.md)
  - [DailyWeatherForecastItemWeatherInner](docs/DailyWeatherForecastItemWeatherInner.md)
  - [DailyWeatherForecastListResponse](docs/DailyWeatherForecastListResponse.md)
  - [EmptySuccess](docs/EmptySuccess.md)
  - [FilterType](docs/FilterType.md)
  - [FitsHeader](docs/FitsHeader.md)
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/__init__.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3657"
+__version__ = "1.3.3661"
 
 # import apis into sdk package
 from ourskyai_astro_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_astro_api.api_response import ApiResponse
 from ourskyai_astro_api.api_client import ApiClient
@@ -30,14 +30,15 @@
 from ourskyai_astro_api.exceptions import ApiAttributeError
 from ourskyai_astro_api.exceptions import ApiException
 
 # import models into sdk package
 from ourskyai_astro_api.models.asset_file_type import AssetFileType
 from ourskyai_astro_api.models.asset_type import AssetType
 from ourskyai_astro_api.models.calibration_master_type import CalibrationMasterType
+from ourskyai_astro_api.models.daily_weather_city import DailyWeatherCity
 from ourskyai_astro_api.models.daily_weather_forecast_item import DailyWeatherForecastItem
 from ourskyai_astro_api.models.daily_weather_forecast_item_temp import DailyWeatherForecastItemTemp
 from ourskyai_astro_api.models.daily_weather_forecast_item_weather_inner import DailyWeatherForecastItemWeatherInner
 from ourskyai_astro_api.models.daily_weather_forecast_list_response import DailyWeatherForecastListResponse
 from ourskyai_astro_api.models.empty_success import EmptySuccess
 from ourskyai_astro_api.models.filter_type import FilterType
 from ourskyai_astro_api.models.fits_header import FitsHeader
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api/default_api.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api_client.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
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
-        self.user_agent = 'OpenAPI-Generator/1.3.3657/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3661/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/api_response.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/configuration.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
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
-               "Version of the API: 1.3.3657\n"\
-               "SDK Package Version: 1.3.3657".\
+               "Version of the API: 1.3.3661\n"\
+               "SDK Package Version: 1.3.3661".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/exceptions.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/__init__.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 # flake8: noqa
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from ourskyai_astro_api.models.asset_file_type import AssetFileType
 from ourskyai_astro_api.models.asset_type import AssetType
 from ourskyai_astro_api.models.calibration_master_type import CalibrationMasterType
+from ourskyai_astro_api.models.daily_weather_city import DailyWeatherCity
 from ourskyai_astro_api.models.daily_weather_forecast_item import DailyWeatherForecastItem
 from ourskyai_astro_api.models.daily_weather_forecast_item_temp import DailyWeatherForecastItemTemp
 from ourskyai_astro_api.models.daily_weather_forecast_item_weather_inner import DailyWeatherForecastItemWeatherInner
 from ourskyai_astro_api.models.daily_weather_forecast_list_response import DailyWeatherForecastListResponse
 from ourskyai_astro_api.models.empty_success import EmptySuccess
 from ourskyai_astro_api.models.filter_type import FilterType
 from ourskyai_astro_api.models.fits_header import FitsHeader
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/asset_file_type.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/asset_file_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/asset_type.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/asset_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/calibration_master_type.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/calibration_master_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_item.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/daily_weather_forecast_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/daily_weather_forecast_list_response.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/daily_weather_forecast_list_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, conlist
+from ourskyai_astro_api.models.daily_weather_city import DailyWeatherCity
 from ourskyai_astro_api.models.daily_weather_forecast_item import DailyWeatherForecastItem
 
 class DailyWeatherForecastListResponse(BaseModel):
     """
     DailyWeatherForecastListResponse
     """
+    city: Optional[DailyWeatherCity] = None
     days: Optional[conlist(DailyWeatherForecastItem)] = None
-    __properties = ["days"]
+    __properties = ["city", "days"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -49,14 +51,17 @@
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of city
+        if self.city:
+            _dict['city'] = self.city.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in days (list)
         _items = []
         if self.days:
             for _item in self.days:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['days'] = _items
@@ -68,12 +73,13 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return DailyWeatherForecastListResponse.parse_obj(obj)
 
         _obj = DailyWeatherForecastListResponse.parse_obj({
+            "city": DailyWeatherCity.from_dict(obj.get("city")) if obj.get("city") is not None else None,
             "days": [DailyWeatherForecastItem.from_dict(_item) for _item in obj.get("days")] if obj.get("days") is not None else None
         })
         return _obj
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/empty_success.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/empty_success.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/filter_type.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/filter_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/fits_header.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/fits_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/location.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/mount_type.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/optical_tube_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,27 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class MountType(str, Enum):
+class OpticalTubeType(str, Enum):
     """
-    MountType
+    OpticalTubeType
     """
 
     """
     allowed enum values
     """
-    ALT_AZ = 'ALT_AZ'
-    EQUITORIAL = 'EQUITORIAL'
+    NEWTONIAN = 'NEWTONIAN'
+    SCT = 'SCT'
+    MCT = 'MCT'
+    RC = 'RC'
+    REFRACTOR = 'REFRACTOR'
 
     @classmethod
-    def from_json(cls, json_str: str) -> MountType:
-        """Create an instance of MountType from a JSON string"""
-        return MountType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> OpticalTubeType:
+        """Create an instance of OpticalTubeType from a JSON string"""
+        return OpticalTubeType(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/node_state.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/node_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/optical_tube_type.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_job_status.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,27 +17,26 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class OpticalTubeType(str, Enum):
+class V1JobStatus(str, Enum):
     """
-    OpticalTubeType
+    V1JobStatus
     """
 
     """
     allowed enum values
     """
-    NEWTONIAN = 'NEWTONIAN'
-    SCT = 'SCT'
-    MCT = 'MCT'
-    RC = 'RC'
-    REFRACTOR = 'REFRACTOR'
+    PENDING = 'PENDING'
+    RUNNING = 'RUNNING'
+    SUCCEEDED = 'SUCCEEDED'
+    FAILED = 'FAILED'
 
     @classmethod
-    def from_json(cls, json_str: str) -> OpticalTubeType:
-        """Create an instance of OpticalTubeType from a JSON string"""
-        return OpticalTubeType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1JobStatus:
+        """Create an instance of V1JobStatus from a JSON string"""
+        return V1JobStatus(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/shutter_type.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/shutter_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/successful_create.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/successful_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/tracking_type.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/tracking_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_astro_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project_asset.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_astro_project_asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_astro_target.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_astro_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_calibration_master.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_calibration_master.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_camera.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_astro_project_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_astro_project_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_astro_project_response.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_astro_project_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_calibration_master_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_calibration_master_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_calibration_master_response.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_calibration_master_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_camera_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_camera_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_image_set_image_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_image_set_image_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_image_set_image_response.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_image_set_image_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_image_set_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_image_set_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_mount_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_mount_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_node_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_create_optical_tube_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_elevation_mask_point.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_elevation_mask_point.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_gain_curve.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_gain_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_gain_curve_point.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_gain_curve_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_nodes.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_get_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_or_create_camera_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_get_or_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_or_create_mount_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_get_or_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_image_set.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_image_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_image_set_image.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_job_kind.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_job_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_job_log.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_job_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_mount.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_node.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_node_with_location.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_node_with_location.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_optical_tube.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_platform_credit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit_source.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_platform_credit_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit_type.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_platform_credit_unit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,23 +17,23 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1PlatformCreditType(str, Enum):
+class V1PlatformCreditUnit(str, Enum):
     """
-    V1PlatformCreditType
+    V1PlatformCreditUnit
     """
 
     """
     allowed enum values
     """
-    ASTRO_PLATFORM_USAGE = 'ASTRO_PLATFORM_USAGE'
+    MEGABYTE = 'MEGABYTE'
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1PlatformCreditType:
-        """Create an instance of V1PlatformCreditType from a JSON string"""
-        return V1PlatformCreditType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1PlatformCreditUnit:
+        """Create an instance of V1PlatformCreditUnit from a JSON string"""
+        return V1PlatformCreditUnit(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_platform_credit_unit.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/mount_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,23 +17,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1PlatformCreditUnit(str, Enum):
+class MountType(str, Enum):
     """
-    V1PlatformCreditUnit
+    MountType
     """
 
     """
     allowed enum values
     """
-    MEGABYTE = 'MEGABYTE'
+    ALT_AZ = 'ALT_AZ'
+    EQUITORIAL = 'EQUITORIAL'
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1PlatformCreditUnit:
-        """Create an instance of V1PlatformCreditUnit from a JSON string"""
-        return V1PlatformCreditUnit(json.loads(json_str))
+    def from_json(cls, json_str: str) -> MountType:
+        """Create an instance of MountType from a JSON string"""
+        return MountType(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_read_noise_point.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_read_noise_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_setup_action.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_setup_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_slew_timing.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_slew_timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_slew_timing_interval.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_slew_timing_interval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_update_node_request.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_update_node_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/models/v1_video_mode_framerate_property.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/models/v1_video_mode_framerate_property.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3657/ourskyai_astro_api/rest.py` & `ourskyai_astro_api-1.3.3661/ourskyai_astro_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3657
+    The version of the OpenAPI document: 1.3.3661
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_astro_api-1.3.3657/pyproject.toml` & `ourskyai_astro_api-1.3.3661/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_astro_api"
-version = "1.3.3657"
+version = "1.3.3661"
 description = "OurSky Astro"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Astro"]
 include = ["ourskyai_astro_api/py.typed"]
```

### Comparing `ourskyai_astro_api-1.3.3657/PKG-INFO` & `ourskyai_astro_api-1.3.3661/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_astro_api
-Version: 1.3.3657
+Version: 1.3.3661
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
 
-- API version: 1.3.3657
-- Package version: 1.3.3657
+- API version: 1.3.3661
+- Package version: 1.3.3661
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -158,14 +158,15 @@
 
 
 ## Documentation For Models
 
  - [AssetFileType](docs/AssetFileType.md)
  - [AssetType](docs/AssetType.md)
  - [CalibrationMasterType](docs/CalibrationMasterType.md)
+ - [DailyWeatherCity](docs/DailyWeatherCity.md)
  - [DailyWeatherForecastItem](docs/DailyWeatherForecastItem.md)
  - [DailyWeatherForecastItemTemp](docs/DailyWeatherForecastItemTemp.md)
  - [DailyWeatherForecastItemWeatherInner](docs/DailyWeatherForecastItemWeatherInner.md)
  - [DailyWeatherForecastListResponse](docs/DailyWeatherForecastListResponse.md)
  - [EmptySuccess](docs/EmptySuccess.md)
  - [FilterType](docs/FilterType.md)
  - [FitsHeader](docs/FitsHeader.md)
```

